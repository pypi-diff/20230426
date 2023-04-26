# Comparing `tmp/ge25519-1.4.0.tar.gz` & `tmp/ge25519-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ge25519-1.4.0.tar", last modified: Tue Apr 25 18:56:13 2023, max compression
+gzip compressed data, was "ge25519-1.4.1.tar", last modified: Wed Apr 26 19:36:01 2023, max compression
```

## Comparing `ge25519-1.4.0.tar` & `ge25519-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103663 ge25519-1.4.0/
--rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-25 14:57:02.000000 ge25519-1.4.0/LICENSE
--rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-25 18:56:13.103733 ge25519-1.4.0/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)     5258 2023-04-15 14:00:02.000000 ge25519-1.4.0/README.rst
--rw-r--r--   0 alapets    (502) staff       (20)     1034 2023-04-15 13:58:43.000000 ge25519-1.4.0/pyproject.toml
--rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-25 18:56:13.103947 ge25519-1.4.0/setup.cfg
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.100913 ge25519-1.4.0/src/
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.102225 ge25519-1.4.0/src/ge25519/
--rw-r--r--   0 alapets    (502) staff       (20)      166 2023-04-25 14:57:02.000000 ge25519-1.4.0/src/ge25519/__init__.py
--rw-r--r--   0 alapets    (502) staff       (20)   121618 2023-04-25 14:57:02.000000 ge25519-1.4.0/src/ge25519/ge25519.py
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103363 ge25519-1.4.0/src/ge25519.egg-info/
--rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/SOURCES.txt
--rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/dependency_links.txt
--rw-r--r--   0 alapets    (502) staff       (20)      234 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/requires.txt
--rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/top_level.txt
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103497 ge25519-1.4.0/test/
--rw-r--r--   0 alapets    (502) staff       (20)     8605 2023-04-25 14:57:02.000000 ge25519-1.4.0/test/test_ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186356 ge25519-1.4.1/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-25 14:57:02.000000 ge25519-1.4.1/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-26 19:36:01.186433 ge25519-1.4.1/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5258 2023-04-15 14:00:02.000000 ge25519-1.4.1/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)     1034 2023-04-26 19:27:36.000000 ge25519-1.4.1/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 19:36:01.186660 ge25519-1.4.1/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.183544 ge25519-1.4.1/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.184723 ge25519-1.4.1/src/ge25519/
+-rw-r--r--   0 alapets    (502) staff       (20)      166 2023-04-25 14:57:02.000000 ge25519-1.4.1/src/ge25519/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)   121618 2023-04-25 14:57:02.000000 ge25519-1.4.1/src/ge25519/ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186065 ge25519-1.4.1/src/ge25519.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      234 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-26 19:36:01.000000 ge25519-1.4.1/src/ge25519.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:36:01.186203 ge25519-1.4.1/test/
+-rw-r--r--   0 alapets    (502) staff       (20)     8605 2023-04-25 14:57:02.000000 ge25519-1.4.1/test/test_ge25519.py
```

### Comparing `ge25519-1.4.0/LICENSE` & `ge25519-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ge25519-1.4.0/PKG-INFO` & `ge25519-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ge25519
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/ge25519
 Project-URL: Documentation, https://ge25519.readthedocs.io
 Requires-Python: >=3.7
```

### Comparing `ge25519-1.4.0/README.rst` & `ge25519-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ge25519-1.4.0/pyproject.toml` & `ge25519-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "ge25519"
-version = "1.4.0"
+version = "1.4.1"
 description = """\
     Pure-Python data structure for working with Ed25519 \
     (and Ristretto) group elements and operations.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "fe25519~=1.3"
+    "fe25519~=1.4"
 ]
 
 [project.urls]
 Repository = "https://github.com/nthparty/ge25519"
 Documentation = "https://ge25519.readthedocs.io"
 
 [project.optional-dependencies]
@@ -25,17 +25,17 @@
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
 ]
 test = [
     "pytest~=7.2",
     "pytest-cov~=4.0",
-    "parts~=1.5",
-    "bitlist~=1.0",
-    "fountains~=2.0"
+    "parts~=1.6",
+    "bitlist~=1.1",
+    "fountains~=2.1"
 ]
 lint = [
     "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
```

### Comparing `ge25519-1.4.0/src/ge25519/ge25519.py` & `ge25519-1.4.1/src/ge25519/ge25519.py`

 * *Files identical despite different names*

### Comparing `ge25519-1.4.0/src/ge25519.egg-info/PKG-INFO` & `ge25519-1.4.1/src/ge25519.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ge25519
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/ge25519
 Project-URL: Documentation, https://ge25519.readthedocs.io
 Requires-Python: >=3.7
```

### Comparing `ge25519-1.4.0/test/test_ge25519.py` & `ge25519-1.4.1/test/test_ge25519.py`

 * *Files identical despite different names*

