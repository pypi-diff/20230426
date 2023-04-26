# Comparing `tmp/trame-keycloak-0.1.0.tar.gz` & `tmp/trame-keycloak-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-keycloak-0.1.0.tar", last modified: Mon Apr 24 00:05:38 2023, max compression
+gzip compressed data, was "trame-keycloak-0.1.1.tar", last modified: Tue Apr 25 16:33:42 2023, max compression
```

## Comparing `trame-keycloak-0.1.0.tar` & `trame-keycloak-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      583 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1139 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      909 2023-04-24 00:05:38.724781 trame-keycloak-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame/modules/keycloak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame/widgets/keycloak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame_keycloak/
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame_keycloak/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame_keycloak/module/
--rw-r--r--   0 root         (0) root         (0)      817 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame_keycloak/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame_keycloak/module/serve/
--rw-r--r--   0 root         (0) root         (0)    38370 2023-04-24 00:05:35.000000 trame-keycloak-0.1.0/trame_keycloak/module/serve/trame-keycloak.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame_keycloak/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame_keycloak/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5119 2023-04-24 00:05:15.000000 trame-keycloak-0.1.0/trame_keycloak/widgets/keycloak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 00:05:38.720780 trame-keycloak-0.1.0/trame_keycloak.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1139 2023-04-24 00:05:38.000000 trame-keycloak-0.1.0/trame_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-04-24 00:05:38.000000 trame-keycloak-0.1.0/trame_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 00:05:38.000000 trame-keycloak-0.1.0/trame_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 00:05:38.000000 trame-keycloak-0.1.0/trame_keycloak.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 00:05:38.000000 trame-keycloak-0.1.0/trame_keycloak.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      909 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.976814 trame-keycloak-0.1.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.976814 trame-keycloak-0.1.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame/modules/keycloak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame/widgets/keycloak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame_keycloak/
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame_keycloak/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame_keycloak/module/
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame_keycloak/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame_keycloak/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    38370 2023-04-25 16:33:40.000000 trame-keycloak-0.1.1/trame_keycloak/module/serve/trame-keycloak.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame_keycloak/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame_keycloak/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-04-25 16:33:25.000000 trame-keycloak-0.1.1/trame_keycloak/widgets/keycloak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:33:42.980814 trame-keycloak-0.1.1/trame_keycloak.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-25 16:33:42.000000 trame-keycloak-0.1.1/trame_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-04-25 16:33:42.000000 trame-keycloak-0.1.1/trame_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:33:42.000000 trame-keycloak-0.1.1/trame_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 16:33:42.000000 trame-keycloak-0.1.1/trame_keycloak.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 16:33:42.000000 trame-keycloak-0.1.1/trame_keycloak.egg-info/top_level.txt
```

### Comparing `trame-keycloak-0.1.0/LICENSE` & `trame-keycloak-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-keycloak-0.1.0/PKG-INFO` & `trame-keycloak-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-keycloak
-Version: 0.1.0
+Version: 0.1.1
 Summary: Keycloak Authentication trame widget
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-keycloak-0.1.0/setup.cfg` & `trame-keycloak-0.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-keycloak
-version = 0.1.0
+version = 0.1.1
 description = Keycloak Authentication trame widget
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-keycloak-0.1.0/trame_keycloak/module/__init__.py` & `trame-keycloak-0.1.1/trame_keycloak/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-keycloak-0.1.0/trame_keycloak/module/serve/trame-keycloak.umd.js` & `trame-keycloak-0.1.1/trame_keycloak/module/serve/trame-keycloak.umd.js`

 * *Files identical despite different names*

### Comparing `trame-keycloak-0.1.0/trame_keycloak/widgets/keycloak.py` & `trame-keycloak-0.1.1/trame_keycloak/widgets/keycloak.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+"""Keycloak Widget support both vue2 and vue3 backend.
+
+(Currently Work-In-Progress)
+"""
 from trame_client.widgets.core import AbstractElement
 from .. import module
 
+__all__ = [
+    "Auth",
+]
+
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-keycloak-0.1.0/trame_keycloak.egg-info/PKG-INFO` & `trame-keycloak-0.1.1/trame_keycloak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-keycloak
-Version: 0.1.0
+Version: 0.1.1
 Summary: Keycloak Authentication trame widget
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-keycloak-0.1.0/trame_keycloak.egg-info/SOURCES.txt` & `trame-keycloak-0.1.1/trame_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

