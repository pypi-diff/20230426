# Comparing `tmp/aafitrans-0.1.0.tar.gz` & `tmp/aafitrans-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aafitrans-0.1.0.tar", last modified: Tue Apr 25 19:20:50 2023, max compression
+gzip compressed data, was "aafitrans-0.1.1.tar", last modified: Tue Apr 25 19:35:29 2023, max compression
```

## Comparing `aafitrans-0.1.0.tar` & `aafitrans-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:20:50.902445 aafitrans-0.1.0/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.1.0/LICENSE.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:20:50.901445 aafitrans-0.1.0/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     4581 2023-04-25 05:53:18.000000 aafitrans-0.1.0/README.md
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      741 2023-04-03 06:04:32.000000 aafitrans-0.1.0/pyproject.toml
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-25 19:20:50.902445 aafitrans-0.1.0/setup.cfg
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:20:50.898445 aafitrans-0.1.0/src/
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:20:50.900445 aafitrans-0.1.0/src/aafitrans/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       65 2023-04-25 19:16:05.000000 aafitrans-0.1.0/src/aafitrans/__init__.py
--rwxrwx---   0 prajwel   (1000) prajwel   (1000)    15597 2023-04-25 19:16:17.000000 aafitrans-0.1.0/src/aafitrans/aafitrans.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:20:50.901445 aafitrans-0.1.0/src/aafitrans.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:20:50.000000 aafitrans-0.1.0/src/aafitrans.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      273 2023-04-25 19:20:50.000000 aafitrans-0.1.0/src/aafitrans.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-25 19:20:50.000000 aafitrans-0.1.0/src/aafitrans.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-04-25 19:20:50.000000 aafitrans-0.1.0/src/aafitrans.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-04-25 19:20:50.000000 aafitrans-0.1.0/src/aafitrans.egg-info/top_level.txt
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.725807 aafitrans-0.1.1/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1103 2023-04-02 07:47:45.000000 aafitrans-0.1.1/LICENSE.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:35:29.724807 aafitrans-0.1.1/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     4581 2023-04-25 05:53:18.000000 aafitrans-0.1.1/README.md
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      741 2023-04-03 06:04:32.000000 aafitrans-0.1.1/pyproject.toml
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-25 19:35:29.725807 aafitrans-0.1.1/setup.cfg
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.721807 aafitrans-0.1.1/src/
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.722807 aafitrans-0.1.1/src/aafitrans/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       65 2023-04-25 19:16:05.000000 aafitrans-0.1.1/src/aafitrans/__init__.py
+-rwxrwx---   0 prajwel   (1000) prajwel   (1000)    15597 2023-04-25 19:32:41.000000 aafitrans-0.1.1/src/aafitrans/aafitrans.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-25 19:35:29.724807 aafitrans-0.1.1/src/aafitrans.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     5084 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      273 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       25 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       10 2023-04-25 19:35:29.000000 aafitrans-0.1.1/src/aafitrans.egg-info/top_level.txt
```

### Comparing `aafitrans-0.1.0/LICENSE.txt` & `aafitrans-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aafitrans-0.1.0/PKG-INFO` & `aafitrans-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.1.0
+Version: 0.1.1
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aafitrans-0.1.0/README.md` & `aafitrans-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aafitrans-0.1.0/pyproject.toml` & `aafitrans-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aafitrans-0.1.0/src/aafitrans/aafitrans.py` & `aafitrans-0.1.1/src/aafitrans/aafitrans.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from scipy.spatial import KDTree
 from itertools import combinations
 from functools import partial
 from collections import Counter
 from skimage import transform
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 class _MatchTransform:
     def __init__(self, source, target, ttype):
         self.source = source
         self.target = target
         self.ttype = ttype
 
@@ -394,15 +394,15 @@
                 best_fit = good_fit 
                 improve_error_counter += 1
                 if improve_error_counter == 100:
                     break
             else:
                 best_fit = good_fit
 
-    if best_fit is None:
+    if good_fit is None:
         raise MaxIterError(
             "List of matching triangles exhausted before an acceptable "
             "transformation was found"
         )
 
     better_fit = best_fit
     previous_fit = best_fit.params + 1
```

### Comparing `aafitrans-0.1.0/src/aafitrans.egg-info/PKG-INFO` & `aafitrans-0.1.1/src/aafitrans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aafitrans
-Version: 0.1.0
+Version: 0.1.1
 Summary: match coordinate lists
 Author-email: Prajwel Joseph <prajwel.pj@gmail.com>
 Project-URL: Homepage, https://github.com/prajwel/aafitrans
 Project-URL: Bug Tracker, https://github.com/prajwel/aafitrans/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

