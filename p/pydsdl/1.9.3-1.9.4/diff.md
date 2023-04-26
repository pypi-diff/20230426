# Comparing `tmp/pydsdl-1.9.3.tar.gz` & `tmp/pydsdl-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydsdl-1.9.3.tar", last modified: Fri Nov 13 04:43:40 2020, max compression
+gzip compressed data, was "dist/pydsdl-1.9.4.tar", last modified: Thu Nov 19 12:31:17 2020, max compression
```

## Comparing `pydsdl-1.9.3.tar` & `pydsdl-1.9.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.994156 pydsdl-1.9.3/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2819 2020-11-13 04:43:40.994156 pydsdl-1.9.3/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1616 2020-11-13 04:43:11.000000 pydsdl-1.9.3/README.md
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.986156 pydsdl-1.9.3/pydsdl/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4643 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15804 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_bit_length_set.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4057 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_data_schema_builder.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16858 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_data_type_builder.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10257 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_dsdl_definition.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5860 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_error.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.990156 pydsdl-1.9.3/pydsdl/_expression/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1744 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5038 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/_any.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8946 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/_container.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6906 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/_operator.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8007 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/_primitive.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4716 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_expression/_test.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    23491 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_namespace.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24093 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_parser.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2307 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_port_id_ranges.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.990156 pydsdl-1.9.3/pydsdl/_serializable/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1355 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10695 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_array.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8414 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_attribute.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    49984 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_composite.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3029 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_name.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9736 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_primitive.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3649 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_serializable.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2040 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_serializable/_void.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    56832 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/_test.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.990156 pydsdl-1.9.3/pydsdl/third_party/
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.994156 pydsdl-1.9.3/pydsdl/third_party/parsimonious/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)      421 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/__init__.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3763 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/exceptions.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16484 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/expressions.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19436 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/grammar.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13167 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/nodes.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1161 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/parsimonious/utils.py
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)    34159 2020-11-13 04:43:11.000000 pydsdl-1.9.3/pydsdl/third_party/six.py
-drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-13 04:43:40.986156 pydsdl-1.9.3/pydsdl.egg-info/
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2819 2020-11-13 04:43:40.000000 pydsdl-1.9.3/pydsdl.egg-info/PKG-INFO
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1146 2020-11-13 04:43:40.000000 pydsdl-1.9.3/pydsdl.egg-info/SOURCES.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2020-11-13 04:43:40.000000 pydsdl-1.9.3/pydsdl.egg-info/dependency_links.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2020-11-13 04:43:40.000000 pydsdl-1.9.3/pydsdl.egg-info/not-zip-safe
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)        7 2020-11-13 04:43:40.000000 pydsdl-1.9.3/pydsdl.egg-info/top_level.txt
--rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2069 2020-11-13 04:43:40.994156 pydsdl-1.9.3/setup.cfg
--rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      466 2020-11-13 04:43:11.000000 pydsdl-1.9.3/setup.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.786384 pydsdl-1.9.4/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2819 2020-11-19 12:31:17.786384 pydsdl-1.9.4/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1616 2020-11-19 12:30:36.000000 pydsdl-1.9.4/README.md
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.778384 pydsdl-1.9.4/pydsdl/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4643 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    15804 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_bit_length_set.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4057 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_data_schema_builder.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16858 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_data_type_builder.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10257 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_dsdl_definition.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5860 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_error.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.782384 pydsdl-1.9.4/pydsdl/_expression/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1744 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5038 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/_any.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8946 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/_container.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     6906 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/_operator.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8007 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/_primitive.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     4716 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_expression/_test.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    26186 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_namespace.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    24093 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_parser.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2307 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_port_id_ranges.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.782384 pydsdl-1.9.4/pydsdl/_serializable/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1400 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    10695 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_array.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8414 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_attribute.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    49984 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_composite.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3029 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_name.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     9736 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_primitive.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3649 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_serializable.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2040 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_serializable/_void.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    56832 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/_test.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.786384 pydsdl-1.9.4/pydsdl/third_party/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.786384 pydsdl-1.9.4/pydsdl/third_party/parsimonious/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      421 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3763 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/exceptions.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    16484 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/expressions.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    19436 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/grammar.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    13167 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/nodes.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1161 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/parsimonious/utils.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    34159 2020-11-19 12:30:36.000000 pydsdl-1.9.4/pydsdl/third_party/six.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2020-11-19 12:31:17.778384 pydsdl-1.9.4/pydsdl.egg-info/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2819 2020-11-19 12:31:17.000000 pydsdl-1.9.4/pydsdl.egg-info/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1146 2020-11-19 12:31:17.000000 pydsdl-1.9.4/pydsdl.egg-info/SOURCES.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2020-11-19 12:31:17.000000 pydsdl-1.9.4/pydsdl.egg-info/dependency_links.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2020-11-19 12:31:17.000000 pydsdl-1.9.4/pydsdl.egg-info/not-zip-safe
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        7 2020-11-19 12:31:17.000000 pydsdl-1.9.4/pydsdl.egg-info/top_level.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2069 2020-11-19 12:31:17.786384 pydsdl-1.9.4/setup.cfg
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      466 2020-11-19 12:30:36.000000 pydsdl-1.9.4/setup.py
```

### Comparing `pydsdl-1.9.3/PKG-INFO` & `pydsdl-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydsdl
-Version: 1.9.3
+Version: 1.9.4
 Summary: UAVCAN DSDL processing frontend implemented in Python
 Home-page: https://uavcan.org
 Author: UAVCAN Development Team
 Author-email: pavel.kirienko@zubax.com
 License: MIT
 Description: # PyDSDL
```

### Comparing `pydsdl-1.9.3/README.md` & `pydsdl-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/__init__.py` & `pydsdl-1.9.4/pydsdl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2018-2020  UAVCAN Development Team  <uavcan.org>
 # This software is distributed under the terms of the MIT License.
 #
 
 import os as _os
 import sys as _sys
 
-__version__ = '1.9.3'
+__version__ = '1.9.4'
 __version_info__ = tuple(map(int, __version__.split('.')))
 __license__ = 'MIT'
 __author__ = 'UAVCAN Development Team'
 
 # Our unorthodox approach to dependency management requires us to apply certain workarounds.
 # Here, the objective is to allow our library to import stuff from its third-party dependency directory,
 # but at the same time we don't want to interfere with the application that depends on this library.
```

### Comparing `pydsdl-1.9.3/pydsdl/_bit_length_set.py` & `pydsdl-1.9.4/pydsdl/_bit_length_set.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_data_schema_builder.py` & `pydsdl-1.9.4/pydsdl/_data_schema_builder.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_data_type_builder.py` & `pydsdl-1.9.4/pydsdl/_data_type_builder.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_dsdl_definition.py` & `pydsdl-1.9.4/pydsdl/_dsdl_definition.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_error.py` & `pydsdl-1.9.4/pydsdl/_error.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/__init__.py` & `pydsdl-1.9.4/pydsdl/_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/_any.py` & `pydsdl-1.9.4/pydsdl/_expression/_any.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/_container.py` & `pydsdl-1.9.4/pydsdl/_expression/_container.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/_operator.py` & `pydsdl-1.9.4/pydsdl/_expression/_operator.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/_primitive.py` & `pydsdl-1.9.4/pydsdl/_expression/_primitive.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_expression/_test.py` & `pydsdl-1.9.4/pydsdl/_expression/_test.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_namespace.py` & `pydsdl-1.9.4/pydsdl/_namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,17 @@
     root_namespace_directory = os.path.abspath(root_namespace_directory)
     lookup_directories_sorted_path_list = list(
         map(lambda d: str(os.path.abspath(d)), lookup_directories_sorted_path_list))
     _logger.debug('Lookup directories are listed below:')
     for a in lookup_directories_sorted_path_list:
         _logger.debug(_LOG_LIST_ITEM_PREFIX + a)
 
+    # Check for common usage errors and warn the user if anything looks suspicious.
+    _ensure_no_common_usage_errors(root_namespace_directory, lookup_directories_sorted_path_list, _logger.warning)
+
     # Check the namespaces.
     _ensure_no_nested_root_namespaces(lookup_directories_sorted_path_list)
     _ensure_no_namespace_name_collisions(lookup_directories_sorted_path_list)
 
     # Construct DSDL definitions from the target and the lookup dirs.
     target_dsdl_definitions = _construct_dsdl_definitions_from_namespace(root_namespace_directory)
     if not target_dsdl_definitions:
@@ -363,14 +366,51 @@
                     a, sealing_name[a_sealed],
                     b, sealing_name[b_sealed],
                 ),
                 path=a.source_file_path
             )
 
 
+def _ensure_no_common_usage_errors(root_namespace_directory: str,
+                                   lookup_directories: typing.Iterable[str],
+                                   reporter: typing.Callable[[str], None]) -> None:
+    suspicious_base_names = [
+        'public_regulated_data_types',
+        'dsdl',
+    ]
+
+    def base(s: str) -> str:
+        return os.path.basename(os.path.normpath(s))
+
+    def is_valid_name(s: str) -> bool:
+        try:
+            _serializable.check_name(s)
+        except _error.InvalidDefinitionError:
+            return False
+        else:
+            return True
+
+    all_paths = set([root_namespace_directory] + list(lookup_directories))
+    for p in all_paths:
+        p = os.path.normcase(os.path.abspath(p))
+        try:
+            candidates = [
+                x for x in os.listdir(p)
+                if os.path.isdir(os.path.join(p, x)) and is_valid_name(x)
+            ]
+        except OSError:  # pragma: no cover
+            candidates = []
+        if candidates and base(p) in suspicious_base_names:
+            report = (
+                'Possibly incorrect usage detected: input path %r is likely incorrect because the last path component '
+                'should be the root namespace name rather than its parent directory. You probably meant:\n%s'
+            ) % (p, '\n'.join(('- %s' % os.path.join(p, s)) for s in candidates),)
+            reporter(report)
+
+
 def _ensure_no_nested_root_namespaces(directories: typing.Iterable[str]) -> None:
     directories = list(sorted([str(os.path.abspath(x)) for x in set(directories)]))
     for a in directories:
         for b in directories:
             if (a != b) and a.startswith(b):
                 raise NestedRootNamespaceError(
                     'The following namespace is nested inside this one, which is not permitted: %r' % a,
@@ -535,7 +575,39 @@
         _construct_dsdl_definitions_from_namespace(root_ns_dir + '/nested/super.bad')
     except FileNameFormatError as ex:
         print(ex)
     else:       # pragma: no cover
         assert False
 
     discard('nested/super.bad/Unreachable.1.0.uavcan')
+
+
+def _unittest_common_usage_errors() -> None:
+    import tempfile
+
+    directory = tempfile.TemporaryDirectory()
+    root_ns_dir = os.path.join(directory.name, 'foo')
+    os.mkdir(root_ns_dir)
+
+    reports = []  # type: typing.List[str]
+
+    _ensure_no_common_usage_errors(root_ns_dir, [], reports.append)
+    assert not reports
+    _ensure_no_common_usage_errors(root_ns_dir, ['/baz'], reports.append)
+    assert not reports
+
+    dir_dsdl = os.path.join(root_ns_dir, 'dsdl')
+    os.mkdir(dir_dsdl)
+    _ensure_no_common_usage_errors(dir_dsdl, ['/baz'], reports.append)
+    assert not reports  # Because empty.
+
+    dir_dsdl_vscode = os.path.join(dir_dsdl, '.vscode')
+    os.mkdir(dir_dsdl_vscode)
+    _ensure_no_common_usage_errors(dir_dsdl, ['/baz'], reports.append)
+    assert not reports  # Because the name is not valid.
+
+    dir_dsdl_uavcan = os.path.join(dir_dsdl, 'uavcan')
+    os.mkdir(dir_dsdl_uavcan)
+    _ensure_no_common_usage_errors(dir_dsdl, ['/baz'], reports.append)
+    rep, = reports
+    reports.clear()
+    assert os.path.normcase(dir_dsdl_uavcan) in rep
```

### Comparing `pydsdl-1.9.3/pydsdl/_parser.py` & `pydsdl-1.9.4/pydsdl/_parser.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_port_id_ranges.py` & `pydsdl-1.9.4/pydsdl/_port_id_ranges.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/__init__.py` & `pydsdl-1.9.4/pydsdl/_serializable/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,7 +27,9 @@
 from ._composite import ServiceType as ServiceType
 from ._composite import Version as Version
 
 from ._attribute import Attribute as Attribute
 from ._attribute import Field as Field
 from ._attribute import PaddingField as PaddingField
 from ._attribute import Constant as Constant
+
+from ._name import check_name as check_name
```

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_array.py` & `pydsdl-1.9.4/pydsdl/_serializable/_array.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_attribute.py` & `pydsdl-1.9.4/pydsdl/_serializable/_attribute.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_composite.py` & `pydsdl-1.9.4/pydsdl/_serializable/_composite.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_name.py` & `pydsdl-1.9.4/pydsdl/_serializable/_name.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_primitive.py` & `pydsdl-1.9.4/pydsdl/_serializable/_primitive.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_serializable.py` & `pydsdl-1.9.4/pydsdl/_serializable/_serializable.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_serializable/_void.py` & `pydsdl-1.9.4/pydsdl/_serializable/_void.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/_test.py` & `pydsdl-1.9.4/pydsdl/_test.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/parsimonious/exceptions.py` & `pydsdl-1.9.4/pydsdl/third_party/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/parsimonious/expressions.py` & `pydsdl-1.9.4/pydsdl/third_party/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/parsimonious/grammar.py` & `pydsdl-1.9.4/pydsdl/third_party/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/parsimonious/nodes.py` & `pydsdl-1.9.4/pydsdl/third_party/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/parsimonious/utils.py` & `pydsdl-1.9.4/pydsdl/third_party/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl/third_party/six.py` & `pydsdl-1.9.4/pydsdl/third_party/six.py`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/pydsdl.egg-info/PKG-INFO` & `pydsdl-1.9.4/pydsdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydsdl
-Version: 1.9.3
+Version: 1.9.4
 Summary: UAVCAN DSDL processing frontend implemented in Python
 Home-page: https://uavcan.org
 Author: UAVCAN Development Team
 Author-email: pavel.kirienko@zubax.com
 License: MIT
 Description: # PyDSDL
```

### Comparing `pydsdl-1.9.3/pydsdl.egg-info/SOURCES.txt` & `pydsdl-1.9.4/pydsdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydsdl-1.9.3/setup.cfg` & `pydsdl-1.9.4/setup.cfg`

 * *Files identical despite different names*

