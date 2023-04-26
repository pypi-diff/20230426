# Comparing `tmp/rdf_data_manager-0.2.0.tar.gz` & `tmp/rdf_data_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdf_data_manager-0.2.0.tar", max compression
+gzip compressed data, was "rdf_data_manager-0.3.0.tar", max compression
```

## Comparing `rdf_data_manager-0.2.0.tar` & `rdf_data_manager-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      165 2023-04-25 14:18:29.760806 rdf_data_manager-0.2.0/README.md
--rw-r--r--   0        0        0      576 2023-04-25 15:57:04.535289 rdf_data_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7364 2023-04-25 15:51:40.035383 rdf_data_manager-0.2.0/rdf_data_manager/__init__.py
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 rdf_data_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-04-25 14:18:29.760806 rdf_data_manager-0.3.0/README.md
+-rw-r--r--   0        0        0      576 2023-04-26 09:50:16.173543 rdf_data_manager-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7871 2023-04-26 09:33:46.173789 rdf_data_manager-0.3.0/rdf_data_manager/__init__.py
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 rdf_data_manager-0.3.0/PKG-INFO
```

### Comparing `rdf_data_manager-0.2.0/pyproject.toml` & `rdf_data_manager-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rdf-data-manager"
-version = "0.2.0"
+version = "0.3.0"
 description = "Load RDF data from S3 to SPARQL endpoint"
 authors = ["Logilab"]
 readme = "README.md"
 packages = [{include = "rdf_data_manager"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `rdf_data_manager-0.2.0/rdf_data_manager/__init__.py` & `rdf_data_manager-0.3.0/rdf_data_manager/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import logging
 import sys
 import time
 import traceback
+from dataclasses import dataclass
 
 import boto3
 import requests
 
 from argparse import ArgumentParser
 from pathlib import Path
 
 from requests.auth import HTTPDigestAuth
 from tqdm import tqdm
 
-from rdflib import Dataset
+from rdflib import Dataset, Graph
+from rdflib.exceptions import ParserError
 
 # tqdm opt
 TQDM_OPTS = {
     "ncols": 100,
     "ascii": True,
     "desc": "Uploading",
 }
 
 
+@dataclass
+class VirtuosoCredentials:
+    url: str
+    user: str
+    password: str
+
+
 def redo_if_failure(call, max_redo=3, sleep_time=5, *args, **kwargs):
     """Redo a function if it fail, with a sleep time between each try"""
     i = 0
     while True:
         i += 1
         try:
             return call(*args, **kwargs)
@@ -39,46 +48,46 @@
                 )
             )
             time.sleep(sleep_time)
             sleep_time = sleep_time * 2
             continue  # redo
 
 
-def delete_graph(virtuoso_url, virtuoso_user, virtuoso_password, graph_uri):
-    logging.info(f"Deleting {graph_uri}…")
+def delete_graph(virtuoso_credentials, graph_uri):
+    logging.info(f"Deleting graph {graph_uri}…")
     response = requests.delete(
-        f"{virtuoso_url}/sparql-graph-crud-auth?",
-        auth=HTTPDigestAuth(virtuoso_user, virtuoso_password),
+        f"{virtuoso_credentials.url}/sparql-graph-crud-auth?",
+        auth=HTTPDigestAuth(virtuoso_credentials.user, virtuoso_credentials.password),
         params={"graph-uri": graph_uri},
     )
     if response.status_code == 404:
-        logging.warning(f"Graph {graph_uri} doesn't exist")
+        logging.info(f"Graph {graph_uri} doesn't exist")
     else:
         response.raise_for_status()
         # give virtuoso enough time to delete the graph
         time.sleep(3)
 
 
-def upload_triples_to_graph(
-    virtuoso_url,
-    virtuoso_user,
-    virtuoso_password,
+def upload_graph(
+    virtuoso_credentials,
     graph_uri,
-    triples_str,
+    graph,
     filename,
 ):
-    logging.info(f"Uploading {filename} into graph {graph_uri}")
+    logging.info(
+        f"Uploading {len(graph)} triples from {filename} into graph {graph_uri}"
+    )
     response = redo_if_failure(
         requests.post,
         3,
         5,
-        f"{virtuoso_url}/sparql-graph-crud-auth",
-        auth=HTTPDigestAuth(virtuoso_user, virtuoso_password),
+        f"{virtuoso_credentials.url}/sparql-graph-crud-auth",
+        auth=HTTPDigestAuth(virtuoso_credentials.user, virtuoso_credentials.password),
         params={"graph-uri": graph_uri},
-        data=triples_str,
+        data=graph.serialize(format="ttl", encoding="utf-8"),
         headers={"Content-type": "text/plain"},
     )
     response.raise_for_status()
 
 
 def main():
     parser = ArgumentParser()
@@ -89,40 +98,41 @@
     parser.add_argument("--s3-secret-key", type=str)
     parser.add_argument("--s3-bucket", type=str)
     parser.add_argument("--s3-dirs", type=str, nargs="+")
 
     parser.add_argument("--input-dirs", type=Path, nargs="+")
 
     parser.add_argument("--virtuoso-url", type=str, required=True)
-    parser.add_argument(
-        "--virtuoso-user", type=str, required=False, default="dba"
-    )
-    parser.add_argument(
-        "--virtuoso-password", type=str, required=False, default="dba"
-    )
+    parser.add_argument("--virtuoso-user", type=str, required=False, default="dba")
+    parser.add_argument("--virtuoso-password", type=str, required=False, default="dba")
 
     parser.add_argument("--rdf-graph", type=str, required=True)
     parser.add_argument("--delete-graph", action="store_true")
     parser.add_argument("--delete-only", action="store_true")
 
     parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("-p", "--progress", action="store_true", default=False)
 
     args = parser.parse_args()
 
     # Set verbosity
     VERBOSITY_MAPPING = {0: logging.WARNING, 1: logging.INFO, 2: logging.DEBUG}
     verbosity = args.verbose if args.verbose < 3 else 2
     logging.basicConfig(level=VERBOSITY_MAPPING[verbosity])
 
+    virtuoso_credentials = VirtuosoCredentials(
+        args.virtuoso_url,
+        args.virtuoso_user,
+        args.virtuoso_password,
+    )
+
     # Delete graph before upload
     if args.delete_graph or args.delete_only:
         delete_graph(
-            args.virtuoso_url,
-            args.virtuoso_user,
-            args.virtuoso_password,
+            virtuoso_credentials,
             args.rdf_graph,
         )
 
     if args.input_type == "s3":
         s3_resource = boto3.resource(
             "s3",
             endpoint_url=args.s3_url,
@@ -142,72 +152,78 @@
                 total = sum(1 for _ in s3_bucket.objects.filter(Prefix=prefix))
                 logging.info(
                     f"Upload {total} files form {args.s3_bucket}/{prefix} into"
                     f" {args.rdf_graph}"
                 )
                 # iter to upload
                 for obj in tqdm(
-                    s3_bucket.objects.all(), total=total, **TQDM_OPTS
+                    s3_bucket.objects.all(),
+                    total=total,
+                    disable=(not args.progress),
+                    **TQDM_OPTS,
                 ):
                     rdf_string = obj.get()["Body"].read().decode("utf-8")
 
                     response = redo_if_failure(
                         requests.post,
                         3,
                         5,
-                        f"{args.virtuoso_url}/sparql-graph-crud-auth",
+                        f"{virtuoso_credentials.url}/sparql-graph-crud-auth",
                         auth=HTTPDigestAuth(
-                            args.virtuoso_user, args.virtuoso_password
+                            virtuoso_credentials.user,
+                            virtuoso_credentials.password,
                         ),
                         params={"graph-uri": args.rdf_graph},
                         data=rdf_string.encode("utf-8"),
                         headers={"Content-type": "text/plain"},
                     )
                     response.raise_for_status()
     else:
         for input_dir in args.input_dirs:
-            total = sum(
-                1 for filepath in input_dir.rglob("*") if not filepath.is_dir()
-            )
-            logging.info(f"Upload {total} files form {input_dir}")
+            total = sum(1 for filepath in input_dir.rglob("*") if not filepath.is_dir())
+            logging.info(f"Found {total} files in {input_dir}")
             for filepath in tqdm(
-                input_dir.rglob("*"), total=total, **TQDM_OPTS
+                input_dir.rglob("*"),
+                total=total,
+                disable=(not args.progress),
+                **TQDM_OPTS,
             ):
                 if not filepath.is_dir():
-                    if filepath.suffix in [".nquads", ".trig"]:
-                        try:
+                    logging.info(f"Processing file {filepath}")
+                    try:
+                        if filepath.suffix in [".nquads", ".trig"]:
                             dataset = Dataset()
                             dataset.parse(filepath)
                             for g in dataset.graphs():
+                                if len(g) == 0:
+                                    logging.info(f"Skipping empty graph {g.identifier}")
+                                    continue
                                 delete_graph(
-                                    args.virtuoso_url,
-                                    args.virtuoso_user,
-                                    args.virtuoso_password,
+                                    virtuoso_credentials,
                                     g.identifier,
                                 )
-                                upload_triples_to_graph(
-                                    args.virtuoso_url,
-                                    args.virtuoso_user,
-                                    args.virtuoso_password,
+                                upload_graph(
+                                    virtuoso_credentials,
                                     g.identifier,
-                                    g.serialize(format="ttl", encoding="utf-8"),
+                                    g,
                                     filepath.name,
                                 )
-                        except Exception as e:
-                            logging.error(
-                                f"File {filepath} is supposed to be nquads"
-                                f" format, but it isn't ({str(e)})"
-                            )
-                    else:
-                        with filepath.open() as fp:
-                            upload_triples_to_graph(
-                                args.virtuoso_url,
-                                args.virtuoso_user,
-                                args.virtuoso_password,
+                        else:
+                            g = Graph()
+                            g.parse(filepath)
+                            if len(g) == 0:
+                                logging.info(f"Skipping empty file {filepath}")
+                                continue
+                            upload_graph(
+                                virtuoso_credentials,
                                 args.rdf_graph,
-                                fp.read().encode("utf-8"),
+                                g,
                                 filepath.name,
                             )
+                    except ParserError:
+                        logging.error(
+                            f"Skipping file {filepath} because of parse error."
+                        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `rdf_data_manager-0.2.0/PKG-INFO` & `rdf_data_manager-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-data-manager
-Version: 0.2.0
+Version: 0.3.0
 Summary: Load RDF data from S3 to SPARQL endpoint
 Author: Logilab
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

