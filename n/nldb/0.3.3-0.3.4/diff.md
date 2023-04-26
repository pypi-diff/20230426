# Comparing `tmp/nldb-0.3.3.tar.gz` & `tmp/nldb-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nldb-0.3.3.tar", last modified: Tue Apr 25 14:10:46 2023, max compression
+gzip compressed data, was "nldb-0.3.4.tar", last modified: Tue Apr 25 14:32:14 2023, max compression
```

## Comparing `nldb-0.3.3.tar` & `nldb-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1815 2023-04-25 12:52:44.252106 nldb-0.3.3/.gitignore
--rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.3/LICENSE
--rw-r--r--   0        0        0      118 2023-03-31 22:32:58.589210 nldb-0.3.3/README.md
--rw-r--r--   0        0        0       51 2023-04-25 13:51:50.853840 nldb-0.3.3/nldb/__init__.py
--rw-r--r--   0        0        0     1311 2023-04-18 16:47:22.620794 nldb-0.3.3/nldb/api.py
--rw-r--r--   0        0        0     2172 2023-04-04 13:49:33.604009 nldb-0.3.3/nldb/cli.py
--rw-r--r--   0        0        0     4595 2023-04-25 13:26:01.281585 nldb-0.3.3/nldb/core.py
--rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.3/nldb/templates/Dockerfile
--rw-r--r--   0        0        0     3803 2023-04-25 13:46:25.520393 nldb-0.3.3/nldb/templates/index.html
--rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.3/nldb/templates/prompt.txt
--rw-r--r--   0        0        0      435 2023-04-25 12:55:23.849992 nldb-0.3.3/notes.md
--rw-r--r--   0        0        0      539 2023-04-25 13:00:22.530315 nldb-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 nldb-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1815 2023-04-25 12:52:44.252106 nldb-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1076 2023-03-29 08:32:29.773266 nldb-0.3.4/LICENSE
+-rw-r--r--   0        0        0      118 2023-03-31 22:32:58.589210 nldb-0.3.4/README.md
+-rw-r--r--   0        0        0       51 2023-04-25 14:31:44.497372 nldb-0.3.4/nldb/__init__.py
+-rw-r--r--   0        0        0     1311 2023-04-18 16:47:22.620794 nldb-0.3.4/nldb/api.py
+-rw-r--r--   0        0        0     2358 2023-04-25 14:31:34.655466 nldb-0.3.4/nldb/cli.py
+-rw-r--r--   0        0        0     4595 2023-04-25 13:26:01.281585 nldb-0.3.4/nldb/core.py
+-rw-r--r--   0        0        0      102 2023-03-31 12:54:34.070465 nldb-0.3.4/nldb/templates/Dockerfile
+-rw-r--r--   0        0        0     3803 2023-04-25 13:46:25.520393 nldb-0.3.4/nldb/templates/index.html
+-rw-r--r--   0        0        0     2068 2023-04-25 13:51:14.723557 nldb-0.3.4/nldb/templates/prompt.txt
+-rw-r--r--   0        0        0      435 2023-04-25 12:55:23.849992 nldb-0.3.4/notes.md
+-rw-r--r--   0        0        0      539 2023-04-25 13:00:22.530315 nldb-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 nldb-0.3.4/PKG-INFO
```

### Comparing `nldb-0.3.3/.gitignore` & `nldb-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/LICENSE` & `nldb-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/nldb/api.py` & `nldb-0.3.4/nldb/api.py`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/nldb/cli.py` & `nldb-0.3.4/nldb/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 import shutil
 from typing import Optional
 
 import typer
 from nldb.api import serve
-from nldb.core import DATABASE
+from nldb.core import DATABASE, NLDB
 
 
 def preflight_checks():
     # check that the prompt.txt file exists
     failures = 0
     if not os.path.exists("prompt.txt"):
         typer.echo("prompt.txt file not found")
@@ -50,25 +50,33 @@
         # For Google Cloud Run:
         gcloud run deploy --source . --set-env-vars="OPENAI_API_KEY={openai_api_key}"
         """
     )
     print(instructions)
 
 
+def answer(query):
+    nldb = NLDB()
+    sql_statement = nldb.text_to_sql(query)
+    print(f"\n{sql_statement.strip()}")
+    answer = nldb.sql_to_answer(sql_statement)[2]
+    print(f"\n{answer}\n")
+
+
 def main(action: Optional[str] = typer.Argument(None)):
     if not action or action == "serve":
         preflight_checks()
         serve()
     elif action == "init":
         init()
     elif action == "deploy":
         preflight_checks()
         deploy_instructions()
     else:
-        print(f"Unknown action: {action}")
+        answer(action)
 
 
 # script entrypoint for flit
 def cli_wrapper():
     typer.run(main)
```

### Comparing `nldb-0.3.3/nldb/core.py` & `nldb-0.3.4/nldb/core.py`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/nldb/templates/index.html` & `nldb-0.3.4/nldb/templates/index.html`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/nldb/templates/prompt.txt` & `nldb-0.3.4/nldb/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/pyproject.toml` & `nldb-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nldb-0.3.3/PKG-INFO` & `nldb-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nldb
-Version: 0.3.3
+Version: 0.3.4
 Summary: talk to your database
 Author-email: Tom Dyson <tom@torchbox.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: openai
 Requires-Dist: fastapi
 Requires-Dist: uvicorn[standard]
```

