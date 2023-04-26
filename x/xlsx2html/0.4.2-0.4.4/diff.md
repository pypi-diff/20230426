# Comparing `tmp/xlsx2html-0.4.2.tar.gz` & `tmp/xlsx2html-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/xlsx2html/xlsx2html/dist/.tmp-esf90ux8/xlsx2html-0.4.2.tar", last modified: Mon Mar 20 16:28:05 2023, max compression
+gzip compressed data, was "/home/runner/work/xlsx2html/xlsx2html/dist/.tmp-lii_zgzw/xlsx2html-0.4.4.tar", last modified: Wed Apr 26 12:41:17 2023, max compression
```

## Comparing `xlsx2html-0.4.2.tar` & `xlsx2html-0.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       34 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2605 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      529 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2267 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (116)     4711 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (116)      235 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/tests/test_locale_format.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html/
--rw-r--r--   0 runner    (1001) docker     (116)      276 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      209 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      120 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html/constants/
--rw-r--r--   0 runner    (1001) docker     (116)      124 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      593 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/constants/border.py
--rw-r--r--   0 runner    (1001) docker     (116)     1117 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/constants/builtin.py
--rw-r--r--   0 runner    (1001) docker     (116)     3059 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/constants/locale_format.py
--rw-r--r--   0 runner    (1001) docker     (116)    11390 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/core.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html/format/
--rw-r--r--   0 runner    (1001) docker     (116)     1667 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6886 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/format/dt.py
--rw-r--r--   0 runner    (1001) docker     (116)     2279 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/format/hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/format/locale.py
--rw-r--r--   0 runner    (1001) docker     (116)     7122 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/format/number.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      619 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/utils/cell.py
--rw-r--r--   0 runner    (1001) docker     (116)      420 2023-03-20 16:27:57.000000 xlsx2html-0.4.2/xlsx2html/utils/image.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2605 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      758 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       49 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2023-03-20 16:28:05.000000 xlsx2html-0.4.2/xlsx2html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2267 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/tests/test_locale_format.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html/
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/constants/border.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/constants/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/constants/locale_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11390 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html/format/
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/format/dt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/format/hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/format/locale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7122 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/format/number.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/utils/cell.py
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-04-26 12:41:06.000000 xlsx2html-0.4.4/xlsx2html/utils/image.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 12:41:17.000000 xlsx2html-0.4.4/xlsx2html.egg-info/top_level.txt
```

### Comparing `xlsx2html-0.4.2/LICENSE` & `xlsx2html-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/PKG-INFO` & `xlsx2html-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsx2html
-Version: 0.4.2
+Version: 0.4.4
 Summary: A simple export from xlsx format to html tables with keep cell formatting
 Home-page: https://github.com/Apkawa/xlsx2html
 Author: Apkawa
 Author-email: apkawa@gmail.com
 License: MIT
 Keywords: converter xlsx html
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xlsx2html-0.4.2/README.md` & `xlsx2html-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/setup.cfg` & `xlsx2html-0.4.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.2
+current_version = 0.4.4
 commit = True
 commit_args = --no-verify
 tag = True
 message = chore: bump version {current_version} → {new_version}
 
 [metadata]
 description-file = README.md
```

### Comparing `xlsx2html-0.4.2/setup.py` & `xlsx2html-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # !/usr/bin/env python
 import os
 import sys
 
 from setuptools import setup, find_packages
 
-version = "0.4.2"
+version = "0.4.4"
 
 if sys.argv[-1] == "publish":
     try:
         import wheel
 
         print("Wheel version: ", wheel.__version__)
     except ImportError:
```

### Comparing `xlsx2html-0.4.2/tests/test_files.py` & `xlsx2html-0.4.4/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/tests/test_format.py` & `xlsx2html-0.4.4/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/tests/test_image.py` & `xlsx2html-0.4.4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/constants/border.py` & `xlsx2html-0.4.4/xlsx2html/constants/border.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/constants/builtin.py` & `xlsx2html-0.4.4/xlsx2html/constants/builtin.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/constants/locale_format.py` & `xlsx2html-0.4.4/xlsx2html/constants/locale_format.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/core.py` & `xlsx2html-0.4.4/xlsx2html/core.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/format/__init__.py` & `xlsx2html-0.4.4/xlsx2html/format/__init__.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/format/dt.py` & `xlsx2html-0.4.4/xlsx2html/format/dt.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/format/hyperlink.py` & `xlsx2html-0.4.4/xlsx2html/format/hyperlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     if hyperlink.location is not None:
         href = "{}#{}".format(hyperlink.target or "", hyperlink.location)
     else:
         href = hyperlink.target
 
     # Maybe link to cell
-    if href.startswith("#"):
+    if href and href.startswith("#"):
         location_info = parse_cell_location(href)
         if location_info:
             href = "#{}.{}".format(
                 location_info["sheet_name"] or cell.parent.title, location_info["coord"]
             )
 
     return '<a href="{href}">{value}</a>'.format(href=href, value=value)
```

### Comparing `xlsx2html-0.4.2/xlsx2html/format/locale.py` & `xlsx2html-0.4.4/xlsx2html/format/locale.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/format/number.py` & `xlsx2html-0.4.4/xlsx2html/format/number.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html/utils/cell.py` & `xlsx2html-0.4.4/xlsx2html/utils/cell.py`

 * *Files identical despite different names*

### Comparing `xlsx2html-0.4.2/xlsx2html.egg-info/PKG-INFO` & `xlsx2html-0.4.4/xlsx2html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsx2html
-Version: 0.4.2
+Version: 0.4.4
 Summary: A simple export from xlsx format to html tables with keep cell formatting
 Home-page: https://github.com/Apkawa/xlsx2html
 Author: Apkawa
 Author-email: apkawa@gmail.com
 License: MIT
 Keywords: converter xlsx html
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xlsx2html-0.4.2/xlsx2html.egg-info/SOURCES.txt` & `xlsx2html-0.4.4/xlsx2html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

