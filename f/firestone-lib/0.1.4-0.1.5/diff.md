# Comparing `tmp/firestone_lib-0.1.4.tar.gz` & `tmp/firestone_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestone_lib-0.1.4.tar", max compression
+gzip compressed data, was "firestone_lib-0.1.5.tar", max compression
```

## Comparing `firestone_lib-0.1.4.tar` & `firestone_lib-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/LICENSE
--rw-r--r--   0        0        0      311 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/__init__.py
--rw-r--r--   0        0        0     4047 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/cli.py
--rw-r--r--   0        0        0     1419 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/resource.py
--rw-r--r--   0        0        0        0 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/resources/logging/__init__.py
--rw-r--r--   0        0        0      396 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/resources/logging/cli.conf
--rw-r--r--   0        0        0      354 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/firestone_lib/utils.py
--rw-r--r--   0        0        0      970 2023-03-22 13:07:25.655469 firestone_lib-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/LICENSE
+-rw-r--r--   0        0        0      311 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/__init__.py
+-rw-r--r--   0        0        0     4047 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/cli.py
+-rw-r--r--   0        0        0     1419 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resource.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/logging/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/resources/logging/cli.conf
+-rw-r--r--   0        0        0      318 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/firestone_lib/utils.py
+-rw-r--r--   0        0        0      970 2023-04-26 10:10:42.912048 firestone_lib-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 firestone_lib-0.1.5/PKG-INFO
```

### Comparing `firestone_lib-0.1.4/LICENSE` & `firestone_lib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.4/firestone_lib/cli.py` & `firestone_lib-0.1.5/firestone_lib/cli.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.4/firestone_lib/resource.py` & `firestone_lib-0.1.5/firestone_lib/resource.py`

 * *Files identical despite different names*

### Comparing `firestone_lib-0.1.4/pyproject.toml` & `firestone_lib-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestone-lib"
-version = "0.1.4"
+version = "0.1.5"
 description = "Library to help build OpneAPI, AsyncAPI and gRPC specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "firestone_lib" }
 ]
```

### Comparing `firestone_lib-0.1.4/PKG-INFO` & `firestone_lib-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestone-lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to help build OpneAPI, AsyncAPI and gRPC specs based off one or more resource json schema files
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

