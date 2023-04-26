# Comparing `tmp/trame-rca-0.3.0.tar.gz` & `tmp/trame-rca-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-rca-0.3.0.tar", last modified: Thu Oct 27 23:54:06 2022, max compression
+gzip compressed data, was "trame-rca-0.3.1.tar", last modified: Tue Apr 25 16:19:13 2023, max compression
```

## Comparing `trame-rca-0.3.0.tar` & `trame-rca-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.818539 trame-rca-0.3.0/
--rw-r--r--   0 root         (0) root         (0)      583 2022-10-27 23:53:32.000000 trame-rca-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-10-27 23:53:32.000000 trame-rca-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1886 2022-10-27 23:54:06.818539 trame-rca-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1070 2022-10-27 23:53:32.000000 trame-rca-0.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      928 2022-10-27 23:54:06.818539 trame-rca-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-27 23:53:32.000000 trame-rca-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame/modules/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame/widgets/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame_rca/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame_rca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame_rca/module/
--rw-r--r--   0 root         (0) root         (0)      909 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame_rca/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame_rca/module/serve/
--rw-r--r--   0 root         (0) root         (0)      196 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   110587 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.common.js
--rw-r--r--   0 root         (0) root         (0)   157870 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.common.js.map
--rw-r--r--   0 root         (0) root         (0)      157 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.css
--rw-r--r--   0 root         (0) root         (0)   110981 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.js
--rw-r--r--   0 root         (0) root         (0)   158422 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.js.map
--rw-r--r--   0 root         (0) root         (0)    40503 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.min.js
--rw-r--r--   0 root         (0) root         (0)   165659 2022-10-27 23:54:00.000000 trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)     2531 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame_rca/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.818539 trame-rca-0.3.0/trame_rca/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame_rca/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2410 2022-10-27 23:53:32.000000 trame-rca-0.3.0/trame_rca/widgets/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 23:54:06.814539 trame-rca-0.3.0/trame_rca.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1886 2022-10-27 23:54:06.000000 trame-rca-0.3.0/trame_rca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      817 2022-10-27 23:54:06.000000 trame-rca-0.3.0/trame_rca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 23:54:06.000000 trame-rca-0.3.0/trame_rca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-10-27 23:54:06.000000 trame-rca-0.3.0/trame_rca.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-10-27 23:54:06.000000 trame-rca-0.3.0/trame_rca.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.047727 trame-rca-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-04-25 16:18:34.000000 trame-rca-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 16:18:34.000000 trame-rca-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-25 16:19:13.047727 trame-rca-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-25 16:18:34.000000 trame-rca-0.3.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-25 16:19:13.047727 trame-rca-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:18:34.000000 trame-rca-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.039727 trame-rca-0.3.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.043727 trame-rca-0.3.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame/modules/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.043727 trame-rca-0.3.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame/widgets/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.043727 trame-rca-0.3.1/trame_rca/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame_rca/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.043727 trame-rca-0.3.1/trame_rca/module/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame_rca/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.047727 trame-rca-0.3.1/trame_rca/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   110587 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.common.js
+-rw-r--r--   0 root         (0) root         (0)   157870 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.common.js.map
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.css
+-rw-r--r--   0 root         (0) root         (0)   110981 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.js
+-rw-r--r--   0 root         (0) root         (0)   158422 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)    40503 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)   165659 2023-04-25 16:19:08.000000 trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame_rca/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.047727 trame-rca-0.3.1/trame_rca/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame_rca/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-25 16:18:34.000000 trame-rca-0.3.1/trame_rca/widgets/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:13.043727 trame-rca-0.3.1/trame_rca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-25 16:19:13.000000 trame-rca-0.3.1/trame_rca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-25 16:19:13.000000 trame-rca-0.3.1/trame_rca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:19:13.000000 trame-rca-0.3.1/trame_rca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 16:19:13.000000 trame-rca-0.3.1/trame_rca.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 16:19:13.000000 trame-rca-0.3.1/trame_rca.egg-info/top_level.txt
```

### Comparing `trame-rca-0.3.0/LICENSE` & `trame-rca-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/PKG-INFO` & `trame-rca-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: trame-rca
-Version: 0.3.0
+Version: 0.3.1
 Summary: Remote Controlled Area widget for trame
-Home-page: UNKNOWN
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
@@ -55,9 +53,7 @@
     cd -
 
 Install the component
 
 .. code-block:: console
 
     pip install -e .
-
-
```

### Comparing `trame-rca-0.3.0/README.rst` & `trame-rca-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/setup.cfg` & `trame-rca-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-rca
-version = 0.3.0
+version = 0.3.1
 description = Remote Controlled Area widget for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-rca-0.3.0/trame_rca/module/__init__.py` & `trame-rca-0.3.1/trame_rca/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.common.js` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.common.js`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.common.js.map` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.common.js.map`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.js` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.js`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.js.map` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.js.map`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.min.js` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.min.js`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/module/serve/vue-trame_rca.umd.min.js.map` & `trame-rca-0.3.1/trame_rca/module/serve/vue-trame_rca.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/protocol.py` & `trame-rca-0.3.1/trame_rca/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-rca-0.3.0/trame_rca/widgets/rca.py` & `trame-rca-0.3.1/trame_rca/widgets/rca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+"""RCA Widgets only support vue2 for now.
+"""
 from trame_client.widgets.core import AbstractElement
 from .. import module
 
+__all__ = [
+    "RemoteControlledArea",
+    "DisplayArea",
+    "StatisticsDisplay",
+    "ImageDisplayArea",
+    "MediaSourceDisplayArea",
+    "VideoDecoderDisplayArea",
+    "RawImageDisplayArea",
+]
+
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-rca-0.3.0/trame_rca.egg-info/PKG-INFO` & `trame-rca-0.3.1/trame_rca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: trame-rca
-Version: 0.3.0
+Version: 0.3.1
 Summary: Remote Controlled Area widget for trame
-Home-page: UNKNOWN
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
@@ -55,9 +53,7 @@
     cd -
 
 Install the component
 
 .. code-block:: console
 
     pip install -e .
-
-
```

### Comparing `trame-rca-0.3.0/trame_rca.egg-info/SOURCES.txt` & `trame-rca-0.3.1/trame_rca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

