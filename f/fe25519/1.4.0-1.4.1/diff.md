# Comparing `tmp/fe25519-1.4.0.tar.gz` & `tmp/fe25519-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fe25519-1.4.0.tar", last modified: Tue Apr 25 18:54:05 2023, max compression
+gzip compressed data, was "fe25519-1.4.1.tar", last modified: Wed Apr 26 19:34:17 2023, max compression
```

## Comparing `fe25519-1.4.0.tar` & `fe25519-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917619 fe25519-1.4.0/
--rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-15 14:39:26.000000 fe25519-1.4.0/LICENSE
--rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-25 18:54:05.917703 fe25519-1.4.0/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)     5262 2023-04-15 13:28:07.000000 fe25519-1.4.0/README.rst
--rw-r--r--   0 alapets    (502) staff       (20)      996 2023-04-15 13:26:56.000000 fe25519-1.4.0/pyproject.toml
--rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-25 18:54:05.917979 fe25519-1.4.0/setup.cfg
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.915043 fe25519-1.4.0/src/
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.916456 fe25519-1.4.0/src/fe25519/
--rw-r--r--   0 alapets    (502) staff       (20)       78 2023-04-15 14:39:26.000000 fe25519-1.4.0/src/fe25519/__init__.py
--rw-r--r--   0 alapets    (502) staff       (20)    21433 2023-04-15 14:39:26.000000 fe25519-1.4.0/src/fe25519/fe25519.py
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917332 fe25519-1.4.0/src/fe25519.egg-info/
--rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/PKG-INFO
--rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/SOURCES.txt
--rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/dependency_links.txt
--rw-r--r--   0 alapets    (502) staff       (20)      221 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/requires.txt
--rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/top_level.txt
-drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917468 fe25519-1.4.0/test/
--rw-r--r--   0 alapets    (502) staff       (20)     9114 2023-04-15 14:39:26.000000 fe25519-1.4.0/test/test_fe25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:34:17.123968 fe25519-1.4.1/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-15 14:39:26.000000 fe25519-1.4.1/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-26 19:34:17.124055 fe25519-1.4.1/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5262 2023-04-15 13:28:07.000000 fe25519-1.4.1/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)      996 2023-04-26 19:24:17.000000 fe25519-1.4.1/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 19:34:17.124297 fe25519-1.4.1/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:34:17.121090 fe25519-1.4.1/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:34:17.122531 fe25519-1.4.1/src/fe25519/
+-rw-r--r--   0 alapets    (502) staff       (20)       78 2023-04-15 14:39:26.000000 fe25519-1.4.1/src/fe25519/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)    21433 2023-04-15 14:39:26.000000 fe25519-1.4.1/src/fe25519/fe25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:34:17.123614 fe25519-1.4.1/src/fe25519.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-26 19:34:17.000000 fe25519-1.4.1/src/fe25519.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-26 19:34:17.000000 fe25519-1.4.1/src/fe25519.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 19:34:17.000000 fe25519-1.4.1/src/fe25519.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      221 2023-04-26 19:34:17.000000 fe25519-1.4.1/src/fe25519.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-26 19:34:17.000000 fe25519-1.4.1/src/fe25519.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:34:17.123769 fe25519-1.4.1/test/
+-rw-r--r--   0 alapets    (502) staff       (20)     9114 2023-04-15 14:39:26.000000 fe25519-1.4.1/test/test_fe25519.py
```

### Comparing `fe25519-1.4.0/LICENSE` & `fe25519-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fe25519-1.4.0/PKG-INFO` & `fe25519-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fe25519
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/fe25519
 Project-URL: Documentation, https://fe25519.readthedocs.io
 Requires-Python: >=3.7
```

### Comparing `fe25519-1.4.0/README.rst` & `fe25519-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fe25519-1.4.0/pyproject.toml` & `fe25519-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fe25519"
-version = "1.4.0"
+version = "1.4.1"
 description = """\
     Pure-Python data structure for working with Ed25519 \
     (and Ristretto) field elements and operations.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
@@ -22,17 +22,17 @@
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

### Comparing `fe25519-1.4.0/src/fe25519/fe25519.py` & `fe25519-1.4.1/src/fe25519/fe25519.py`

 * *Files identical despite different names*

### Comparing `fe25519-1.4.0/src/fe25519.egg-info/PKG-INFO` & `fe25519-1.4.1/src/fe25519.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fe25519
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/fe25519
 Project-URL: Documentation, https://fe25519.readthedocs.io
 Requires-Python: >=3.7
```

### Comparing `fe25519-1.4.0/test/test_fe25519.py` & `fe25519-1.4.1/test/test_fe25519.py`

 * *Files identical despite different names*

