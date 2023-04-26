# Comparing `tmp/graphql_service_framework-1.1.2.tar.gz` & `tmp/graphql_service_framework-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.2.tar", last modified: Mon Apr 24 14:58:52 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.3.tar", last modified: Tue Apr 25 19:07:58 2023, max compression
```

## Comparing `graphql_service_framework-1.1.2.tar` & `graphql_service_framework-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 14:58:51.000000 graphql_service_framework-1.1.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.214325 graphql_service_framework-1.1.2/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15650 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/query.graphql
--rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.215325 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.584151 graphql_service_framework-1.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-25 19:07:58.585151 graphql_service_framework-1.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-25 19:07:57.000000 graphql_service_framework-1.1.3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.581151 graphql_service_framework-1.1.3/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5303 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.583151 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-25 19:07:58.585151 graphql_service_framework-1.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.584151 graphql_service_framework-1.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.2/LICENSE` & `graphql_service_framework-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/PKG-INFO` & `graphql_service_framework-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.2
+Version: 1.1.3
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.2.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.3.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.3/graphql_service_framework/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.3/graphql_service_framework/mesh.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.3/graphql_service_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.3/graphql_service_framework/schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.3/graphql_service_framework/schema_tracker.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/service.py` & `graphql_service_framework-1.1.3/graphql_service_framework/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         if not self.config.get("service_type"):
             self.config["service_type"] = "asgi"
 
         if not self.config.get("service_name"):
             self.config["service_name"] = to_snake_case(root.__class__.__name__)
 
         if not self.config.get("api_version"):
-            self.config["api_version"] = root.__class__.api_version
+            if root and hasattr(root.__class__, "api_version"):
+                self.config["api_version"] = root.__class__.api_version
 
         if not self.config.get("http_health_path"):
             self.config["http_health_path"] = f"{relative_path}/health"
 
         health_path = self.config.get("http_health_path")
 
         if not graphiql_default:
```

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.3/graphql_service_framework/utils.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.3/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.2
+Version: 1.1.3
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.2.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.3.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.2/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.3/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/setup.py` & `graphql_service_framework-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/tests/test_schema.py` & `graphql_service_framework-1.1.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/tests/test_service_manager.py` & `graphql_service_framework-1.1.3/tests/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.2/tests/utils.py` & `graphql_service_framework-1.1.3/tests/utils.py`

 * *Files identical despite different names*

