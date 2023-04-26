# Comparing `tmp/trame-formkit-0.1.1.tar.gz` & `tmp/trame-formkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-formkit-0.1.1.tar", last modified: Thu Feb 23 02:09:28 2023, max compression
+gzip compressed data, was "trame-formkit-0.1.2.tar", last modified: Tue Apr 25 16:39:24 2023, max compression
```

## Comparing `trame-formkit-0.1.1.tar` & `trame-formkit-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      874 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      886 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.761162 trame-formkit-0.1.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.761162 trame-formkit-0.1.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame/modules/formkit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.761162 trame-formkit-0.1.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame/widgets/formkit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.761162 trame-formkit-0.1.1/trame_formkit/
--rw-r--r--   0 root         (0) root         (0)       95 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame_formkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/trame_formkit/module/
--rw-r--r--   0 root         (0) root         (0)      365 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame_formkit/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/trame_formkit/module/serve/
--rw-r--r--   0 root         (0) root         (0)   331006 2023-02-23 02:09:25.000000 trame-formkit-0.1.1/trame_formkit/module/serve/formkit.js
--rw-r--r--   0 root         (0) root         (0)      296 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame_formkit/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.765162 trame-formkit-0.1.1/trame_formkit/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame_formkit/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-02-23 02:09:22.000000 trame-formkit-0.1.1/trame_formkit/widgets/formkit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 02:09:28.761162 trame-formkit-0.1.1/trame_formkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      874 2023-02-23 02:09:28.000000 trame-formkit-0.1.1/trame_formkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2023-02-23 02:09:28.000000 trame-formkit-0.1.1/trame_formkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 02:09:28.000000 trame-formkit-0.1.1/trame_formkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-23 02:09:28.000000 trame-formkit-0.1.1/trame_formkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-23 02:09:28.000000 trame-formkit-0.1.1/trame_formkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      874 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame/modules/formkit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame/widgets/formkit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame_formkit/
+-rw-r--r--   0 root         (0) root         (0)       95 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame_formkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame_formkit/module/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame_formkit/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame_formkit/module/serve/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-25 16:39:22.000000 trame-formkit-0.1.2/trame_formkit/module/serve/formkit.js
+-rw-r--r--   0 root         (0) root         (0)      296 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame_formkit/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame_formkit/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame_formkit/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-04-25 16:39:19.000000 trame-formkit-0.1.2/trame_formkit/widgets/formkit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:39:24.644076 trame-formkit-0.1.2/trame_formkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-04-25 16:39:24.000000 trame-formkit-0.1.2/trame_formkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2023-04-25 16:39:24.000000 trame-formkit-0.1.2/trame_formkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:39:24.000000 trame-formkit-0.1.2/trame_formkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 16:39:24.000000 trame-formkit-0.1.2/trame_formkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 16:39:24.000000 trame-formkit-0.1.2/trame_formkit.egg-info/top_level.txt
```

### Comparing `trame-formkit-0.1.1/LICENSE` & `trame-formkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-formkit-0.1.1/PKG-INFO` & `trame-formkit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-formkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: FormKit integration into trame widgets
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-formkit-0.1.1/setup.cfg` & `trame-formkit-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-formkit
-version = 0.1.1
+version = 0.1.2
 description = FormKit integration into trame widgets
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-formkit-0.1.1/trame_formkit/widgets/formkit.py` & `trame-formkit-0.1.2/trame_formkit/widgets/formkit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+"""Formkit Widgets only support vue3.
+"""
 from trame_client.widgets.core import AbstractElement, Template
 from .. import module
 
+__all__ = [
+    "FormKit",
+    "FormKitSchema",
+]
+
 # FormKit section keys
 slot_names = [
     "outer",  # The outermost wrapping element.
     "wrapper",  # A wrapper around the label and input.
     "label",  # The label of the input.
     "prefix",  # Has no output by default, but allows content directly before an input element.
     "prefixIcon",  # An element for outputting an icon before the prefix section.
```

### Comparing `trame-formkit-0.1.1/trame_formkit.egg-info/PKG-INFO` & `trame-formkit-0.1.2/trame_formkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-formkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: FormKit integration into trame widgets
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-formkit-0.1.1/trame_formkit.egg-info/SOURCES.txt` & `trame-formkit-0.1.2/trame_formkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

