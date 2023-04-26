# Comparing `tmp/trame-grid-layout-1.0.2.tar.gz` & `tmp/trame-grid-layout-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-grid-layout-1.0.2.tar", last modified: Thu Feb 23 02:13:38 2023, max compression
+gzip compressed data, was "trame-grid-layout-1.0.3.tar", last modified: Tue Apr 25 16:35:05 2023, max compression
```

## Comparing `trame-grid-layout-1.0.2.tar` & `trame-grid-layout-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.297550 trame-grid-layout-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5306 2023-02-23 02:13:38.297550 trame-grid-layout-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4552 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      897 2023-02-23 02:13:38.297550 trame-grid-layout-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame/modules/grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame/widgets/grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame_grid/
--rw-r--r--   0 root         (0) root         (0)     1168 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame_grid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame_grid/module/
--rw-r--r--   0 root         (0) root         (0)      289 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame_grid/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame_grid/module/serve/
--rw-r--r--   0 root         (0) root         (0)   143453 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame_grid/module/serve/vue-grid-layout.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.293550 trame-grid-layout-1.0.2/trame_grid/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame_grid/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10484 2023-02-23 02:13:34.000000 trame-grid-layout-1.0.2/trame_grid/widgets/grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:13:38.297550 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5306 2023-02-23 02:13:38.000000 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      521 2023-02-23 02:13:38.000000 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 02:13:38.000000 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-23 02:13:38.000000 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-23 02:13:38.000000 trame-grid-layout-1.0.2/trame_grid_layout.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame/modules/grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame/widgets/grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame_grid/
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame_grid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame_grid/module/
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame_grid/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame_grid/module/serve/
+-rw-r--r--   0 root         (0) root         (0)   143453 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame_grid/module/serve/vue-grid-layout.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame_grid/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame_grid/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2023-04-25 16:35:01.000000 trame-grid-layout-1.0.3/trame_grid/widgets/grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:35:05.081317 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-04-25 16:35:05.000000 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-25 16:35:05.000000 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:35:05.000000 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 16:35:05.000000 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-25 16:35:05.000000 trame-grid-layout-1.0.3/trame_grid_layout.egg-info/top_level.txt
```

### Comparing `trame-grid-layout-1.0.2/LICENSE` & `trame-grid-layout-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-grid-layout-1.0.2/PKG-INFO` & `trame-grid-layout-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-grid-layout
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trame wrapper to vue-grid-layout
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-grid-layout-1.0.2/README.rst` & `trame-grid-layout-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `trame-grid-layout-1.0.2/setup.cfg` & `trame-grid-layout-1.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-grid-layout
-version = 1.0.2
+version = 1.0.3
 description = Trame wrapper to vue-grid-layout
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-grid-layout-1.0.2/trame_grid/__init__.py` & `trame-grid-layout-1.0.3/trame_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-grid-layout-1.0.2/trame_grid/module/serve/vue-grid-layout.js` & `trame-grid-layout-1.0.3/trame_grid/module/serve/vue-grid-layout.js`

 * *Files identical despite different names*

### Comparing `trame-grid-layout-1.0.2/trame_grid/widgets/grid.py` & `trame-grid-layout-1.0.3/trame_grid/widgets/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+"""Grid Widgets only support vue2.
+"""
 from trame_client.widgets.core import AbstractElement
 from trame_client.widgets.html import Div
 from .. import module, update_layout
 
+__all__ = [
+    "GridLayout",
+    "GridItem",
+]
+
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-grid-layout-1.0.2/trame_grid_layout.egg-info/PKG-INFO` & `trame-grid-layout-1.0.3/trame_grid_layout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-grid-layout
-Version: 1.0.2
+Version: 1.0.3
 Summary: Trame wrapper to vue-grid-layout
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-grid-layout-1.0.2/trame_grid_layout.egg-info/SOURCES.txt` & `trame-grid-layout-1.0.3/trame_grid_layout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

