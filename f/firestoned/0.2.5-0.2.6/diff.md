# Comparing `tmp/firestoned-0.2.5.tar.gz` & `tmp/firestoned-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.2.5.tar", max compression
+gzip compressed data, was "firestoned-0.2.6.tar", max compression
```

## Comparing `firestoned-0.2.5.tar` & `firestoned-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-26 12:24:13.798307 firestoned-0.2.5/LICENSE
--rw-r--r--   0        0        0     9344 2023-04-26 12:24:13.798307 firestoned-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/__init__.py
--rw-r--r--   0        0        0     4872 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/__main__.py
--rw-r--r--   0        0        0     2045 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/resource.py
--rw-r--r--   0        0        0        0 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     5843 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      408 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      175 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/spec/__init__.py
--rw-r--r--   0        0        0      866 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/spec/_base.py
--rw-r--r--   0        0        0    13390 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9184 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/spec/cli.py
--rw-r--r--   0        0        0    16097 2023-04-26 12:24:13.802307 firestoned-0.2.5/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1664 2023-04-26 12:24:13.802307 firestoned-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    10553 1970-01-01 00:00:00.000000 firestoned-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 14:03:38.877846 firestoned-0.2.6/LICENSE
+-rw-r--r--   0        0        0     9344 2023-04-26 14:03:38.877846 firestoned-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/__init__.py
+-rw-r--r--   0        0        0     4872 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/__main__.py
+-rw-r--r--   0        0        0     2045 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/resource.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     5906 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      408 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      175 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13390 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9184 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/cli.py
+-rw-r--r--   0        0        0    16137 2023-04-26 14:03:38.885846 firestoned-0.2.6/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1664 2023-04-26 14:03:38.885846 firestoned-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    10553 1970-01-01 00:00:00.000000 firestoned-0.2.6/PKG-INFO
```

### Comparing `firestoned-0.2.5/LICENSE` & `firestoned-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/README.md` & `firestoned-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/__main__.py` & `firestoned-0.2.6/firestone/__main__.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/resource.py` & `firestoned-0.2.6/firestone/resource.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/schema/main.py.jinja2` & `firestoned-0.2.6/firestone/schema/main.py.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 @click.option("--threads", help="The number of threads for client side", type=int, default=1)
 @click.pass_context
 def main(ctx, debug, api_key, api_url, threads, trust_proxy):
     """{{ title }}
 
     {{ description }}
     """
-	if not trust_proxy:
-		if "http_proxy" in os.environ:
-			del os.environ["http_proxy"]
-		if "https_proxy" in os.environ:
-			del os.environ["https_proxy"]
-		if "HTTP_PROXY" in os.environ:
-			del os.environ["HTTP_PROXY"]
-		if "HTTPS_PROXY" in os.environ:
-			del os.environ["HTTPS_PROXY"]
+    if not trust_proxy:
+        if "http_proxy" in os.environ:
+            del os.environ["http_proxy"]
+        if "https_proxy" in os.environ:
+            del os.environ["https_proxy"]
+        if "HTTP_PROXY" in os.environ:
+            del os.environ["HTTP_PROXY"]
+        if "HTTPS_PROXY" in os.environ:
+            del os.environ["HTTPS_PROXY"]
 
     try:
         cli.init_logging("{{ pkg }}.resources.logging", "cli.conf")
     # pylint: disable=broad-except
     except Exception:
         logging.basicConfig(
             level=logging.INFO,
```

### Comparing `firestoned-0.2.5/firestone/schema/resource.yaml` & `firestoned-0.2.6/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/spec/_base.py` & `firestoned-0.2.6/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/spec/asyncapi.py` & `firestoned-0.2.6/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/spec/cli.py` & `firestoned-0.2.6/firestone/spec/cli.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.5/firestone/spec/openapi.py` & `firestoned-0.2.6/firestone/spec/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     schema = rsrc["schema"] if "schema" in rsrc else rsrc
     methods = rsrc.get("methods", {})
     descs = rsrc.get("descriptions", {})
 
     if not paths:
         paths = {}
 
-    if schema["type"] == "array" and not "key" in schema:
+    if schema["type"] == "array" and schema["items"]["type"] == "object" and not "key" in schema:
         raise spec_base.SchemaMissingAttribute("A 'key' is missing in schema {yaml.dump(schema)}")
 
     key = None
     if "key" in schema:
         key = schema["key"]
         has_param = next((item for item in keys if item["name"] == key["name"]), None)
         _LOGGER.debug(f"has_param: {has_param}")
```

### Comparing `firestoned-0.2.5/pyproject.toml` & `firestoned-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.2.5"
+version = "0.2.6"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
```

### Comparing `firestoned-0.2.5/PKG-INFO` & `firestoned-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.2.5
+Version: 0.2.6
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.2.5 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.2.6 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.8,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: caching
```

