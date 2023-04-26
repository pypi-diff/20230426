# Comparing `tmp/mo_python-0.0.4.tar.gz` & `tmp/mo_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_python-0.0.4.tar", max compression
+gzip compressed data, was "mo_python-0.0.5.tar", max compression
```

## Comparing `mo_python-0.0.4.tar` & `mo_python-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0        0 2022-01-13 15:30:24.704263 mo_python-0.0.4/LICENSE
--rw-r--r--   0        0        0      410 2022-11-11 15:56:48.696139 mo_python-0.0.4/moalerts/__init__.py
--rw-r--r--   0        0        0     1923 2022-01-13 15:30:24.719888 mo_python-0.0.4/moalerts/alarms.csv
--rw-r--r--   0        0        0     5531 2022-11-11 15:56:48.697141 mo_python-0.0.4/moalerts/core.py
--rw-r--r--   0        0        0      613 2022-11-11 15:56:48.698140 mo_python-0.0.4/moalerts/helpers.py
--rw-r--r--   0        0        0      115 2022-01-13 15:30:24.719888 mo_python-0.0.4/moalerts/notes.txt
--rw-r--r--   0        0        0    13343 2022-01-13 15:30:24.719888 mo_python-0.0.4/moalerts/test.csv
--rw-r--r--   0        0        0      574 2022-11-21 15:38:52.154050 mo_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 mo_python-0.0.4/setup.py
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 mo_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-01-13 15:30:24.704263 mo_python-0.0.5/LICENSE
+-rw-r--r--   0        0        0      410 2022-11-11 15:56:48.696139 mo_python-0.0.5/moalerts/__init__.py
+-rw-r--r--   0        0        0     1923 2022-01-13 15:30:24.719888 mo_python-0.0.5/moalerts/alarms.csv
+-rw-r--r--   0        0        0     5531 2022-11-11 15:56:48.697141 mo_python-0.0.5/moalerts/core.py
+-rw-r--r--   0        0        0      613 2022-11-11 15:56:48.698140 mo_python-0.0.5/moalerts/helpers.py
+-rw-r--r--   0        0        0      115 2022-01-13 15:30:24.719888 mo_python-0.0.5/moalerts/notes.txt
+-rw-r--r--   0        0        0    13343 2022-01-13 15:30:24.719888 mo_python-0.0.5/moalerts/test.csv
+-rw-r--r--   0        0        0      574 2023-04-26 13:39:45.531032 mo_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 mo_python-0.0.5/PKG-INFO
```

### Comparing `mo_python-0.0.4/moalerts/alarms.csv` & `mo_python-0.0.5/moalerts/alarms.csv`

 * *Files identical despite different names*

### Comparing `mo_python-0.0.4/moalerts/core.py` & `mo_python-0.0.5/moalerts/core.py`

 * *Files identical despite different names*

### Comparing `mo_python-0.0.4/moalerts/helpers.py` & `mo_python-0.0.5/moalerts/helpers.py`

 * *Files identical despite different names*

### Comparing `mo_python-0.0.4/moalerts/test.csv` & `mo_python-0.0.5/moalerts/test.csv`

 * *Files identical despite different names*

### Comparing `mo_python-0.0.4/pyproject.toml` & `mo_python-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mo-python"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python package for adding alerts to the MO alerts database."
 authors = ["Gavin Bell <gavin.bell@optimeering.com>", "Jo Vederhus <jo.vederhus@optimeering.com>"]
 license = "Apache-2.0"
 packages = [{include = "moalerts"}]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
```

### Comparing `mo_python-0.0.4/PKG-INFO` & `mo_python-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for adding alerts to the MO alerts database.
 License: Apache-2.0
 Author: Gavin Bell
 Author-email: gavin.bell@optimeering.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

