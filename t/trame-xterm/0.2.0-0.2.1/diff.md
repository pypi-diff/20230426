# Comparing `tmp/trame-xterm-0.2.0.tar.gz` & `tmp/trame-xterm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-xterm-0.2.0.tar", last modified: Wed Apr 19 20:47:51 2023, max compression
+gzip compressed data, was "trame-xterm-0.2.1.tar", last modified: Tue Apr 25 16:17:02 2023, max compression
```

## Comparing `trame-xterm-0.2.0.tar` & `trame-xterm-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      901 2023-04-19 20:47:51.476857 trame-xterm-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.468857 trame-xterm-0.2.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.468857 trame-xterm-0.2.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame/modules/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.468857 trame-xterm-0.2.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.468857 trame-xterm-0.2.0/trame_xterm/
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/trame_xterm/module/
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/trame_xterm/module/serve/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-04-19 20:47:47.000000 trame-xterm-0.2.0/trame_xterm/module/serve/style.css
--rw-r--r--   0 root         (0) root         (0)   466182 2023-04-19 20:47:47.000000 trame-xterm-0.2.0/trame_xterm/module/serve/trame-xterm.mjs
--rw-r--r--   0 root         (0) root         (0)   341052 2023-04-19 20:47:47.000000 trame-xterm-0.2.0/trame_xterm/module/serve/trame-xterm.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/trame_xterm/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/utils/terminal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/trame_xterm/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18925 2023-04-19 20:47:26.000000 trame-xterm-0.2.0/trame_xterm/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:47:51.472857 trame-xterm-0.2.0/trame_xterm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-19 20:47:51.000000 trame-xterm-0.2.0/trame_xterm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      635 2023-04-19 20:47:51.000000 trame-xterm-0.2.0/trame_xterm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:47:51.000000 trame-xterm-0.2.0/trame_xterm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 20:47:51.000000 trame-xterm-0.2.0/trame_xterm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-19 20:47:51.000000 trame-xterm-0.2.0/trame_xterm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.771162 trame-xterm-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 16:17:02.771162 trame-xterm-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      901 2023-04-25 16:17:02.775163 trame-xterm-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.763162 trame-xterm-0.2.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.763162 trame-xterm-0.2.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame/modules/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.763162 trame-xterm-0.2.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.767162 trame-xterm-0.2.1/trame_xterm/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.767162 trame-xterm-0.2.1/trame_xterm/module/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.771162 trame-xterm-0.2.1/trame_xterm/module/serve/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-04-25 16:16:58.000000 trame-xterm-0.2.1/trame_xterm/module/serve/style.css
+-rw-r--r--   0 root         (0) root         (0)   466182 2023-04-25 16:16:58.000000 trame-xterm-0.2.1/trame_xterm/module/serve/trame-xterm.mjs
+-rw-r--r--   0 root         (0) root         (0)   341052 2023-04-25 16:16:58.000000 trame-xterm-0.2.1/trame_xterm/module/serve/trame-xterm.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.771162 trame-xterm-0.2.1/trame_xterm/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/utils/terminal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.771162 trame-xterm-0.2.1/trame_xterm/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18982 2023-04-25 16:16:38.000000 trame-xterm-0.2.1/trame_xterm/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:17:02.767162 trame-xterm-0.2.1/trame_xterm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-25 16:17:02.000000 trame-xterm-0.2.1/trame_xterm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-25 16:17:02.000000 trame-xterm-0.2.1/trame_xterm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:17:02.000000 trame-xterm-0.2.1/trame_xterm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-25 16:17:02.000000 trame-xterm-0.2.1/trame_xterm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 16:17:02.000000 trame-xterm-0.2.1/trame_xterm.egg-info/top_level.txt
```

### Comparing `trame-xterm-0.2.0/LICENSE` & `trame-xterm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.2.0/PKG-INFO` & `trame-xterm-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,26 @@
 
 
 License
 -----------------------------------------------------------
 
 This library is distributed under the MIT License (Same as xterm.js)
 
+Usage Examples
+-----------------------------------------------------------
+
+.. image:: examples/multi-shells/git.png
+  :alt: Multi-shell with git log
+
+.. image:: examples/multi-shells/python.png
+  :alt: Multi-shell with python interpreter
+
+.. image:: examples/shell/htop.png
+  :alt: Interactive update with htop
+
 
 Development
 -----------------------------------------------------------
 
 Build and install the Vue components
 
 .. code-block:: console
```

### Comparing `trame-xterm-0.2.0/setup.cfg` & `trame-xterm-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-xterm
-version = 0.2.0
+version = 0.2.1
 description = Trame widget to expose xterm.js
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-xterm-0.2.0/trame_xterm/module/serve/style.css` & `trame-xterm-0.2.1/trame_xterm/module/serve/style.css`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.2.0/trame_xterm/module/serve/trame-xterm.mjs` & `trame-xterm-0.2.1/trame_xterm/module/serve/trame-xterm.mjs`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.2.0/trame_xterm/module/serve/trame-xterm.umd.js` & `trame-xterm-0.2.1/trame_xterm/module/serve/trame-xterm.umd.js`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.2.0/trame_xterm/utils/terminal.py` & `trame-xterm-0.2.1/trame_xterm/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.2.0/trame_xterm/widgets/xterm.py` & `trame-xterm-0.2.1/trame_xterm/widgets/xterm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""XTerm Widget support both vue2 and vue3 backend.
+"""
+
 import json
 from termcolor import colored
 from trame_client.widgets.core import AbstractElement
 from .. import module
 
 try:
     from ..utils.terminal import Terminal
 
     TERMINAL_AVAILABLE = True
 except ModuleNotFoundError:
     TERMINAL_AVAILABLE = False
 
 
-__ALL__ = ["XTerm", "colored", "THEME_NAMES"]
+__all__ = ["XTerm", "colored", "THEME_NAMES"]
 
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-xterm-0.2.0/trame_xterm.egg-info/PKG-INFO` & `trame-xterm-0.2.1/trame_xterm.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,26 @@
 
 
 License
 -----------------------------------------------------------
 
 This library is distributed under the MIT License (Same as xterm.js)
 
+Usage Examples
+-----------------------------------------------------------
+
+.. image:: examples/multi-shells/git.png
+  :alt: Multi-shell with git log
+
+.. image:: examples/multi-shells/python.png
+  :alt: Multi-shell with python interpreter
+
+.. image:: examples/shell/htop.png
+  :alt: Interactive update with htop
+
 
 Development
 -----------------------------------------------------------
 
 Build and install the Vue components
 
 .. code-block:: console
```

### Comparing `trame-xterm-0.2.0/trame_xterm.egg-info/SOURCES.txt` & `trame-xterm-0.2.1/trame_xterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

