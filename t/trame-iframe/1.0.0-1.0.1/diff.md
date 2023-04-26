# Comparing `tmp/trame-iframe-1.0.0.tar.gz` & `tmp/trame-iframe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-iframe-1.0.0.tar", last modified: Wed Apr  5 19:40:25 2023, max compression
+gzip compressed data, was "trame-iframe-1.0.1.tar", last modified: Tue Apr 25 16:34:10 2023, max compression
```

## Comparing `trame-iframe-1.0.0.tar` & `trame-iframe-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1788 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.275962 trame-iframe-1.0.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.275962 trame-iframe-1.0.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame/modules/iframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame/widgets/iframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame_iframe/
--rw-r--r--   0 root         (0) root         (0)       94 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame_iframe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame_iframe/module/
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame_iframe/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame_iframe/module/serve/
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-05 19:40:21.000000 trame-iframe-1.0.0/trame_iframe/module/serve/trame-iframe.mjs
--rw-r--r--   0 root         (0) root         (0)     1362 2023-04-05 19:40:21.000000 trame-iframe-1.0.0/trame_iframe/module/serve/trame-iframe.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame_iframe/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame_iframe/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5038 2023-04-05 19:40:04.000000 trame-iframe-1.0.0/trame_iframe/widgets/iframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 19:40:25.279963 trame-iframe-1.0.0/trame_iframe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-04-05 19:40:25.000000 trame-iframe-1.0.0/trame_iframe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-05 19:40:25.000000 trame-iframe-1.0.0/trame_iframe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 19:40:25.000000 trame-iframe-1.0.0/trame_iframe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-05 19:40:25.000000 trame-iframe-1.0.0/trame_iframe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-05 19:40:25.000000 trame-iframe-1.0.0/trame_iframe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.877457 trame-iframe-1.0.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.877457 trame-iframe-1.0.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame/modules/iframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.877457 trame-iframe-1.0.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame/widgets/iframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.877457 trame-iframe-1.0.1/trame_iframe/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame_iframe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/trame_iframe/module/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame_iframe/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/trame_iframe/module/serve/
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-25 16:34:07.000000 trame-iframe-1.0.1/trame_iframe/module/serve/trame-iframe.mjs
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-04-25 16:34:07.000000 trame-iframe-1.0.1/trame_iframe/module/serve/trame-iframe.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/trame_iframe/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame_iframe/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-04-25 16:33:53.000000 trame-iframe-1.0.1/trame_iframe/widgets/iframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:34:10.881457 trame-iframe-1.0.1/trame_iframe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-04-25 16:34:10.000000 trame-iframe-1.0.1/trame_iframe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-25 16:34:10.000000 trame-iframe-1.0.1/trame_iframe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:34:10.000000 trame-iframe-1.0.1/trame_iframe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 16:34:10.000000 trame-iframe-1.0.1/trame_iframe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-25 16:34:10.000000 trame-iframe-1.0.1/trame_iframe.egg-info/top_level.txt
```

### Comparing `trame-iframe-1.0.0/LICENSE` & `trame-iframe-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-iframe-1.0.0/PKG-INFO` & `trame-iframe-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-iframe
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper for iframe/cross-origin communication for trame
 Author: Kitware Inc
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-iframe-1.0.0/README.rst` & `trame-iframe-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-iframe-1.0.0/setup.cfg` & `trame-iframe-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-iframe
-version = 1.0.0
+version = 1.0.1
 description = Helper for iframe/cross-origin communication for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc
 license = Apache Software License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-iframe-1.0.0/trame_iframe/module/serve/trame-iframe.mjs` & `trame-iframe-1.0.1/trame_iframe/module/serve/trame-iframe.mjs`

 * *Files identical despite different names*

### Comparing `trame-iframe-1.0.0/trame_iframe/module/serve/trame-iframe.umd.js` & `trame-iframe-1.0.1/trame_iframe/module/serve/trame-iframe.umd.js`

 * *Files identical despite different names*

### Comparing `trame-iframe-1.0.0/trame_iframe/widgets/iframe.py` & `trame-iframe-1.0.1/trame_iframe/widgets/iframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+"""IFrame Widgets support both vue2 and vue3 backend.
+"""
+
 from trame_client.widgets.core import AbstractElement
 from .. import module
 
+__all__ = [
+    "IFrame",
+    "Communicator",
+]
+
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-iframe-1.0.0/trame_iframe.egg-info/PKG-INFO` & `trame-iframe-1.0.1/trame_iframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-iframe
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper for iframe/cross-origin communication for trame
 Author: Kitware Inc
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-iframe-1.0.0/trame_iframe.egg-info/SOURCES.txt` & `trame-iframe-1.0.1/trame_iframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

