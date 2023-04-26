# Comparing `tmp/refac-0.0.3.tar.gz` & `tmp/refac-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refac-0.0.3.tar", last modified: Tue Mar 28 21:18:48 2023, max compression
+gzip compressed data, was "refac-0.0.4.tar", last modified: Tue Apr 25 23:36:38 2023, max compression
```

## Comparing `refac-0.0.3.tar` & `refac-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:48.688699 refac-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-28 21:18:39.000000 refac-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-28 21:18:48.688699 refac-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-28 21:18:39.000000 refac-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 21:18:48.688699 refac-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-28 21:18:39.000000 refac-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:48.688699 refac-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:48.688699 refac-0.0.3/src/refac/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/move_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/move_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/move_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/replace_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:48.688699 refac-0.0.3/src/refac/visitors/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/add_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/inplace_replace_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/remove_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-03-28 21:18:39.000000 refac-0.0.3/src/refac/visitors/replace_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:18:48.688699 refac-0.0.3/src/refac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 21:18:48.000000 refac-0.0.3/src/refac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:37.998445 refac-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 23:36:27.000000 refac-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-25 23:36:37.998445 refac-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-25 23:36:27.000000 refac-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:36:37.998445 refac-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 23:36:27.000000 refac-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:37.990445 refac-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:37.994445 refac-0.0.4/src/refac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/move_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/move_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/move_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:37.998445 refac-0.0.4/src/refac/visitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/add_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/inplace_replace_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/remove_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-04-25 23:36:27.000000 refac-0.0.4/src/refac/visitors/replace_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:36:37.994445 refac-0.0.4/src/refac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 23:36:37.000000 refac-0.0.4/src/refac.egg-info/top_level.txt
```

### Comparing `refac-0.0.3/LICENSE` & `refac-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/PKG-INFO` & `refac-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refac
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to move around Python source code.
 Home-page: https://github.com/benchling/refac
 Author: Benchling Open Source
 Author-email: opensource@benchling.com
 Maintainer: Benchling Open Source
 Maintainer-email: opensource@benchling.com
 License: MIT License
```

### Comparing `refac-0.0.3/README.md` & `refac-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/setup.py` & `refac-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/__init__.py` & `refac-0.0.4/src/refac/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __description__ = "Tool to move around Python source code."
 __license__ = "MIT License"
 __uri__ = "https://github.com/benchling/refac"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Benchling Open Source"
 __email__ = "opensource@benchling.com"
 
 import argparse
 import sys
 
 from .move_file import move_file
```

### Comparing `refac-0.0.3/src/refac/move_file.py` & `refac-0.0.4/src/refac/move_file.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/move_symbol.py` & `refac-0.0.4/src/refac/move_symbol.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/replace_str.py` & `refac-0.0.4/src/refac/replace_str.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/utils.py` & `refac-0.0.4/src/refac/utils.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/visitors/add_symbols.py` & `refac-0.0.4/src/refac/visitors/add_symbols.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/visitors/import_utils.py` & `refac-0.0.4/src/refac/visitors/import_utils.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/visitors/inplace_replace_import.py` & `refac-0.0.4/src/refac/visitors/inplace_replace_import.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/visitors/remove_symbols.py` & `refac-0.0.4/src/refac/visitors/remove_symbols.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac/visitors/replace_import.py` & `refac-0.0.4/src/refac/visitors/replace_import.py`

 * *Files identical despite different names*

### Comparing `refac-0.0.3/src/refac.egg-info/PKG-INFO` & `refac-0.0.4/src/refac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refac
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to move around Python source code.
 Home-page: https://github.com/benchling/refac
 Author: Benchling Open Source
 Author-email: opensource@benchling.com
 Maintainer: Benchling Open Source
 Maintainer-email: opensource@benchling.com
 License: MIT License
```

### Comparing `refac-0.0.3/src/refac.egg-info/SOURCES.txt` & `refac-0.0.4/src/refac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

