# Comparing `tmp/LoadingBar_Py_Diggs-0.1.0.tar.gz` & `tmp/LoadingBar_Py_Diggs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LoadingBar_Py_Diggs-0.1.0.tar", last modified: Tue Apr 25 12:01:11 2023, max compression
+gzip compressed data, was "LoadingBar_Py_Diggs-0.1.1.tar", last modified: Wed Apr 26 11:31:01 2023, max compression
```

## Comparing `LoadingBar_Py_Diggs-0.1.0.tar` & `LoadingBar_Py_Diggs-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:01:11.073609 LoadingBar_Py_Diggs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 12:00:59.000000 LoadingBar_Py_Diggs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 12:01:11.073609 LoadingBar_Py_Diggs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-25 12:00:59.000000 LoadingBar_Py_Diggs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-25 12:00:59.000000 LoadingBar_Py_Diggs-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:01:11.073609 LoadingBar_Py_Diggs-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:01:11.069609 LoadingBar_Py_Diggs-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:01:11.073609 LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 12:01:11.000000 LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 12:01:11.000000 LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:01:11.000000 LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 12:01:11.000000 LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:01:11.073609 LoadingBar_Py_Diggs-0.1.0/src/Loading_Bar/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 12:00:59.000000 LoadingBar_Py_Diggs-0.1.0/src/Loading_Bar/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-25 12:00:59.000000 LoadingBar_Py_Diggs-0.1.0/src/Loading_Bar/loadingBar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-26 11:30:47.000000 LoadingBar_Py_Diggs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 11:30:47.000000 LoadingBar_Py_Diggs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-26 11:30:47.000000 LoadingBar_Py_Diggs-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-26 11:31:01.000000 LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 11:31:01.000000 LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:31:01.000000 LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 11:31:01.000000 LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:01.664661 LoadingBar_Py_Diggs-0.1.1/src/Loading_Bar/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-26 11:30:47.000000 LoadingBar_Py_Diggs-0.1.1/src/Loading_Bar/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-26 11:30:47.000000 LoadingBar_Py_Diggs-0.1.1/src/Loading_Bar/loadingBar.py
```

### Comparing `LoadingBar_Py_Diggs-0.1.0/LICENSE` & `LoadingBar_Py_Diggs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LoadingBar_Py_Diggs-0.1.0/PKG-INFO` & `LoadingBar_Py_Diggs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: LoadingBar_Py_Diggs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Simple loading bar for python.
-Author-email: Velte Hollund <vetlehoo@gmail.com>
+Author-email: Vetle Hollund <vetlehoo@gmail.com>
 Project-URL: Homepage, https://github.com/VHollund/LoadingBar
 Project-URL: Bug Reports, https://github.com/VHollund/LoadingBar/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `LoadingBar_Py_Diggs-0.1.0/pyproject.toml` & `LoadingBar_Py_Diggs-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "LoadingBar_Py_Diggs"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
-  { name="Velte Hollund", email="vetlehoo@gmail.com" },
+  { name="Vetle Hollund", email="vetlehoo@gmail.com" },
 ]
 description = "A Simple loading bar for python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `LoadingBar_Py_Diggs-0.1.0/src/LoadingBar_Py_Diggs.egg-info/PKG-INFO` & `LoadingBar_Py_Diggs-0.1.1/src/LoadingBar_Py_Diggs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: LoadingBar-Py-Diggs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Simple loading bar for python.
-Author-email: Velte Hollund <vetlehoo@gmail.com>
+Author-email: Vetle Hollund <vetlehoo@gmail.com>
 Project-URL: Homepage, https://github.com/VHollund/LoadingBar
 Project-URL: Bug Reports, https://github.com/VHollund/LoadingBar/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `LoadingBar_Py_Diggs-0.1.0/src/Loading_Bar/loadingBar.py` & `LoadingBar_Py_Diggs-0.1.1/src/Loading_Bar/loadingBar.py`

 * *Files identical despite different names*

