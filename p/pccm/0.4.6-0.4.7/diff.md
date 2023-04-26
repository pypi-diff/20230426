# Comparing `tmp/pccm-0.4.6.tar.gz` & `tmp/pccm-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pccm-0.4.6.tar", last modified: Mon Feb  6 10:34:55 2023, max compression
+gzip compressed data, was "pccm-0.4.7.tar", last modified: Wed Apr 26 06:01:03 2023, max compression
```

## Comparing `pccm-0.4.6.tar` & `pccm-0.4.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.640710 pccm-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-06 10:34:09.000000 pccm-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-06 10:34:55.636710 pccm-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-06 10:34:09.000000 pccm-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.632710 pccm-0.4.6/pccm/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.632710 pccm-0.4.6/pccm/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33852 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/builder/inliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/builder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/builder/pybind.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/core/
--rw-r--r--   0 runner    (1001) docker     (123)   105033 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/buildmeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/funccode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/inspecttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/core/pycore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/libs/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/libs/numpylib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/libs/stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/libs/tvten.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/middlewares/expose_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    51082 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/middlewares/pybind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/source/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/source/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/targets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/targets/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/targets/cuda_ptx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/pccm/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/test_data/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/test_data/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-06 10:34:09.000000 pccm-0.4.6/pccm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.632710 pccm-0.4.6/pccm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-06 10:34:55.000000 pccm-0.4.6/pccm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-06 10:34:09.000000 pccm-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 10:34:55.640710 pccm-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-02-06 10:34:09.000000 pccm-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 10:34:55.636710 pccm-0.4.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-02-06 10:34:09.000000 pccm-0.4.6/test/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.344854 pccm-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 06:00:20.000000 pccm-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 06:01:03.344854 pccm-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 06:00:20.000000 pccm-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.336854 pccm-0.4.7/pccm/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35550 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/inliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/pybind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)   105155 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/buildmeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/funccode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/inspecttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/pycore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/numpylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/tvten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/expose_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51082 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/pybind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/source/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/targets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/cuda_ptx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.336854 pccm-0.4.7/pccm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 06:00:20.000000 pccm-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:01:03.344854 pccm-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-26 06:00:20.000000 pccm-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-26 06:00:20.000000 pccm-0.4.7/test/test_core.py
```

### Comparing `pccm-0.4.6/LICENSE` & `pccm-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/PKG-INFO` & `pccm-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccm
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python C++ Code Manager.
 Home-page: https://github.com/FindDefinition/PCCM
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pccm-0.4.6/pccm/__init__.py` & `pccm-0.4.7/pccm/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/builder/inliner.py` & `pccm-0.4.7/pccm/builder/inliner.py`

 * *Files 5% similar despite different names*

```diff
@@ -423,34 +423,50 @@
                          "string", "iostream", "fstream")
         self.add_dependency(PyBind11)
 
 
 class _ModuleMeta:
 
     def __init__(self, func: Any, captures: List[CaptureStmt],
-                 capture_ctypes: List[BaseType], inner_code: str) -> None:
+                 capture_ctypes: List[BaseType], inner_code: str,
+                 kernel_code: str, raw_code: str) -> None:
         self.func = func
         self.captures = captures
         self.capture_ctypes = capture_ctypes
         self.inner_code = inner_code
+        self.kernel_code = kernel_code
+        self.user_raw_code = raw_code
 
 
 class InlineBuilder:
     """
     inliner.inline(...)    
+    TODO improve the performance of capture analysis
+    Args:
+        deps: dependencies of the module
+        plugins: plugins for custom types
+        root: root path of the module
+        build_root: build root path
+        build_kwargs: kwargs for build
+        param_deps: parameterized dependencies
+        reload_when_code_change: whether to reload the module when code changes
+        reload_compare_use_raw: whether to use raw code to compare when reload.
+            if false, compare will happen after all captures are applied, which
+            is slow.
     """
 
     def __init__(self,
                  deps: List[Type[Class]],
                  plugins: Optional[Dict[str, InlineBuilderPlugin]] = None,
                  root: Optional[Path] = None,
                  build_root: Optional[Path] = None,
                  build_kwargs: Optional[Dict[str, Any]] = None,
                  param_deps: Optional[List[pccm.ParameterizedClass]] = None,
-                 reload_when_code_change: bool = False) -> None:
+                 reload_when_code_change: bool = False,
+                 reload_compare_use_raw: bool = True) -> None:
         self.deps = deps
         if param_deps is None:
             param_deps = []
         self.param_deps = param_deps
         if plugins is None:
             self.plugins = _DEFAULT_PLUGINS
         else:
@@ -459,14 +475,15 @@
             build_kwargs = {}
         self.build_kwargs = build_kwargs
         self.modules: Dict[Tuple[str, str, int], _ModuleMeta] = {}
         # self.cached_captures: Dict[Tuple[str, str, int],
         #                            List[CaptureStmt]] = {}
         # self.cached_capture_ctypes: Dict[Tuple[str, str, int],
         #                                  List[BaseType]] = {}
+        self._reload_compare_use_raw = reload_compare_use_raw
 
         self.lock = threading.Lock()
 
         self.dep_ids = [get_qualname_of_type(t) for t in self.deps]
         self.dep_ids.sort()
         self.used_names: Set[Tuple[str, str]] = set()
         self.root = root
@@ -570,32 +587,36 @@
         assert cur_frame is not None
         frame = cur_frame
         while _frame_cnt > 0:
             frame = cur_frame.f_back
             assert frame is not None
             cur_frame = frame
             _frame_cnt -= 1
-        # del frame
+        del frame
         local_vars = cur_frame.f_locals.copy()
         local_vars.update(additional_vars)
         code_path = cur_frame.f_code.co_filename
         lineno = cur_frame.f_lineno
         key = (code_path, name)
         unique_key = (code_path, name, lineno)
         if self._reload_when_code_change:
             unique_key = (code_path, name, -1)
-        # del cur_frame
+        del cur_frame
         with self.lock:
             if not disable_cache and not self._reload_when_code_change:
                 exist = unique_key in self.modules
                 if key in self.used_names and not exist:
                     raise ValueError("you use duplicate name in same file.",
                                      unique_key)
             else:
                 exist = False
+                if self._reload_when_code_change and self._reload_compare_use_raw:
+                    if unique_key in self.modules:
+                        data = self.modules[unique_key]
+                        exist = data.user_raw_code == code_str
             if not exist:
                 # 1. extract captured vars
                 all_captures = _get_captures_in_code(code_str)
                 # 2. find captures in prev frame
                 container_fcode = FunctionCode()
                 inner_fcode = FunctionCode()
                 # 3. inference c++ types
@@ -683,39 +704,41 @@
                                         str(mapped_cpp_type),
                                         array=mapped_cpp_type.count)
                     args.append(v)
 
                 inner_code_str = execute_modifiers(code_str, replaces)
 
                 assert inner_code_str is not None
-                if self._reload_when_code_change:
+                if self._reload_when_code_change and not self._reload_compare_use_raw:
                     exist = unique_key in self.modules
                     if exist:
                         prev_inner_code = self.modules[unique_key].inner_code
                         if prev_inner_code == inner_code_str:
                             module_meta = self.modules[unique_key]
                             func = module_meta.func
                             all_captures = module_meta.captures
                             all_base_types = module_meta.capture_ctypes
                             args = []
                             for cap, bt in zip(all_captures, all_base_types):
-                                if not cap.is_expr:
-                                    if cap.name not in local_vars:
-                                        raise ValueError(
-                                            f"can't find your capture {cap.name} in prev frame."
-                                        )
-                                    obj = local_vars[cap.name]
+                                if cap.name in pre_capture_map:
+                                    obj = pre_capture_map[cap.name]
                                 else:
-                                    for cap_name in cap.expr_names:
-                                        if cap_name not in local_vars:
+                                    if not cap.is_expr: 
+                                        if cap.name not in local_vars:
                                             raise ValueError(
-                                                f"can't find your capture {cap_name} in prev frame."
-                                            )
-                                    # eval expr in prev frame
-                                    obj = eval(cap.name, local_vars)
+                                                f"can't find your capture {cap.name} in prev frame.")
+                                        obj = local_vars[cap.name]
+                                    else:
+                                        for cap_name in cap.expr_names:
+                                            if cap_name not in local_vars:
+                                                raise ValueError(
+                                                    f"can't find your capture {cap_name} in prev frame."
+                                                )
+                                        # eval expr in prev frame
+                                        obj = eval(cap.name, local_vars)
                                 obj = _nested_apply_plugin_transform(
                                     bt, obj, self.plugins, user_arg)
                                 args.append(obj)
                             for v in additional_vars.values():
                                 args.append(v)
                             return self.run_func(func,
                                                  *args,
@@ -723,15 +746,14 @@
                 if isinstance(code, FunctionCode):
                     container_fcode.ret(code.return_type)
                 meta = self.handle_container_code(inner_code_str,
                                                   container_fcode, user_arg)
                 inner_decl = self.create_inner_decl(inner_code_str,
                                                     container_fcode,
                                                     inner_fcode, user_arg)
-
                 # now we have complete code. we need to determine a history build dir and use it to build library if need.
                 # here we must reserve build dir because we need to rebuild when dependency change.
                 if meta is None:
                     meta = StaticMemberFunctionMeta(
                         impl_file_suffix=impl_file_suffix)
                     meta.mw_metas.append(Pybind11MethodMeta())
                 decl = FunctionDecl(meta, container_fcode)
@@ -773,16 +795,18 @@
                                                pdep_cls_name)
                 pccm_class.namespace = PCCM_INLINE_NAMESPACE
                 mod_root = self.get_save_root(Path(code_path), self.root,
                                               self.build_root)
                 func = self.build(pccm_class, mod_root, name, timeout,
                                   user_arg)
                 if not disable_cache:
+                    code_for_inspect = "\n".join(pccm.core.generate_code(container_fcode.get_impl(PCCM_INLINE_FUNCTION_NAME, meta), 0, 2))
                     module_meta = _ModuleMeta(func, all_captures, capture_bts,
-                                              inner_code_str)
+                                              inner_code_str, code_for_inspect,
+                                              code_str)
                     self.modules[unique_key] = module_meta
                     # self.cached_captures[unique_key] = all_captures
                     # self.cached_capture_ctypes[unique_key] = capture_bts
                     self.used_names.add(key)
                     # breakpoint()
                 return self.run_func(func, *args, user_args=user_arg)
 
@@ -813,14 +837,20 @@
             obj = _nested_apply_plugin_transform(bt, obj, self.plugins,
                                                  user_arg)
             args.append(obj)
         for v in additional_vars.values():
             args.append(v)
         return self.run_func(func, *args, user_args=user_arg)
 
+    def search_codes_by_name(self, name: str):
+        res: List[str] = []
+        for k, v in self.modules.items():
+            if name == k[1]:
+                res.append(v.kernel_code)
+        return res 
 
 def main():
     print(_expr_str_to_identifier("a.shape[0] + 5"))
     import ast
 
     import numpy as np
     tree = ast.parse("a.shape[0] + b + c")
```

### Comparing `pccm-0.4.6/pccm/builder/main.py` & `pccm-0.4.7/pccm/builder/main.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/builder/pybind.py` & `pccm-0.4.7/pccm/builder/pybind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 import os 
 import ccimport
+import time 
 from ccimport.buildtools.writer import DEFAULT_MSVC_DEP_PREFIX, group_dict_by_split
 
 from pccm.core import Class, CodeFormatter, CodeGenerator, ManualClassGenerator
 from pccm.core.buildmeta import BuildMeta
 from pccm.middlewares import expose_main, pybind
 
 from pccm.constants import PCCM_DISABLE_CODE_CHANGE
@@ -113,15 +114,15 @@
                 if not init_path.exists():
                     with init_path.open("w") as f:
                         f.write("")
                 mk_init = mk_init / part
             with pyi_path.open("w") as f:
                 f.write(v)
 
-    return ccimport.ccimport(
+    res = ccimport.ccimport(
         paths,
         out_path,
         build_meta,
         std=std,
         source_paths_for_hash=None,
         disable_hash=disable_hash,
         load_library=load_library,
@@ -131,15 +132,15 @@
         pch_to_sources=pch_to_sources,
         pch_to_include=pch_to_include,
         suffix_to_compiler=suffix_to_compiler,
         verbose=verbose,
         objects_folder=objects_folder,
         source_meta={str(p): v
                      for p, v in path_to_meta.items()})
-
+    return res 
 
 def gen_cmake(target_name: str,
               cus: List[Class],
               include_path: Union[str, Path],
               src_path: Union[str, Path],
               build_meta: Optional[BuildMeta] = None,
               cxx_standard="14",
```

### Comparing `pccm-0.4.6/pccm/core/__init__.py` & `pccm-0.4.7/pccm/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,25 +55,25 @@
 def _get_attr_hook(type_str: str):
     res = _FCODE_ARGUMENT_ATTR_HOOKS.get(type_str, None)
     return res
 
 
 def _clean_code(code: str):
     lines = code.split("\n")
-    # filter empty lines
-    lines = list(filter(lambda x: len(x.strip()) > 0, lines))
-    if not lines:
-        return ""
-    min_indent = max(len(l) for l in lines)
+    new_lines = []
+    min_indent = len(code)
     for l in lines:
-        for i in range(len(l)):
-            if l[i] != " ":
-                min_indent = min(min_indent, i)
-                break
-    return "\n".join(l[min_indent:] for l in lines)
+        l_strip = l.strip()
+        if not l_strip:
+            continue 
+        l_lstrip = l.lstrip()
+        min_indent = min(min_indent, len(l) - len(l_lstrip))
+        new_lines.append(l)
+
+    return "\n".join(l[min_indent:] for l in new_lines)
 
 
 _CPP_OPERATOR_ENC = {
     "+": "add",
     "-": "sub",
     "*": "mul",
     "/": "div",
@@ -1307,17 +1307,17 @@
 
     @graph_inited.setter
     def graph_inited(self, val: bool):
         self._graph_inited = val
 
     @property
     def uid(self) -> Optional[str]:
-        if self.namespace is None:
+        if self._namespace is None:
             return None
-        return "{}-{}".format(self.namespace, self.class_name)
+        return f"{self._namespace}-{self.class_name}"
 
     @property
     def camelcase_uid(self):
         assert self._namespace is not None
         return "_".join(self._namespace.split(".") + [self.class_name])
 
     def __repr__(self):
@@ -2383,55 +2383,58 @@
         path_to_cmake_content["CMakeLists.txt"] = "\n".join(main_cmake_contents)
         return header_dict, impl_dict, header_to_impls, impl_to_buildmeta, header_to_meta, path_to_cmake_content
 
 
     def code_written(self,
                      root: Union[str, Path],
                      code_dict: Dict[str, CodeSection],
-                     code_fmt: Optional[CodeFormatter] = None):
-        return self.code_written_v2(root, code_dict, {}, code_fmt)[0]
+                     code_fmt: Optional[CodeFormatter] = None,
+                     write_code: bool = True):
+        return self.code_written_v2(root, code_dict, {}, code_fmt, write_code)[0]
 
     def code_written_v2(self,
                      root: Union[str, Path],
                      code_dict: Dict[str, CodeSection],
                      build_meta_dict: Dict[str, BuildMeta],
-                     code_fmt: Optional[CodeFormatter] = None):
+                     code_fmt: Optional[CodeFormatter] = None,
+                     write_code: bool = True):
         # TODO insert md5 to code to detect manual code change
         root_path = Path(root)
         all_paths = []  # type: List[Path]
         path_to_meta: Dict[Path, BuildMeta] = {}
         if code_fmt is None:
             code_fmt = CodeFormatter()
         for k, v in code_dict.items():
             code_to_write = code_fmt(v.to_string())
             code_path = root_path / k
             if k in build_meta_dict:
                 path_to_meta[code_path] = build_meta_dict[k]
-            if code_path.exists():
-                # read first, if same, don't write to keep file state.
-                with code_path.open("r") as f:
-                    code = f.read()
-                if code.strip() == code_to_write.strip():
-                    all_paths.append(code_path)
-                    continue
-                if self.verbose:
-                    code_to_write_lines = code_to_write.strip().split("\n")
-                    code_old_lines = code.strip().split("\n")
-                    diff = difflib.unified_diff(code_old_lines,
-                                                code_to_write_lines)
-                    print(f"--- {code_path} ---")
-                    print("\n".join(diff))
-            code_path.parent.mkdir(0o755, exist_ok=True, parents=True)
-            with code_path.open("w") as f:
-                f.write(code_to_write)
+            if write_code:
+                if code_path.exists():
+                    # read first, if same, don't write to keep file state.
+                    with code_path.open("r") as f:
+                        code = f.read()
+                    if code.strip() == code_to_write.strip():
+                        all_paths.append(code_path)
+                        continue
+                    if self.verbose:
+                        code_to_write_lines = code_to_write.strip().split("\n")
+                        code_old_lines = code.strip().split("\n")
+                        diff = difflib.unified_diff(code_old_lines,
+                                                    code_to_write_lines)
+                        print(f"--- {code_path} ---")
+                        print("\n".join(diff))
+                code_path.parent.mkdir(0o755, exist_ok=True, parents=True)
+                with code_path.open("w") as f:
+                    f.write(code_to_write)
             all_paths.append(code_path)
         return all_paths, path_to_meta
 
-    def generate_cu_code_v2(self,
-                            cu: Class,
+    @staticmethod
+    def generate_cu_code_v2(cu: Class,
                             one_impl_one_file: bool = True,
                             include_root: Optional[Path] = None,
                             global_header_only: bool = False):
         """
         TODO multiple impl one file
         generate_code will put all Class in cus to one header file and same namespace.
         headers: {
```

### Comparing `pccm-0.4.6/pccm/core/codegen.py` & `pccm-0.4.7/pccm/core/codegen.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/core/funccode.py` & `pccm-0.4.7/pccm/core/funccode.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/core/inspecttools.py` & `pccm-0.4.7/pccm/core/inspecttools.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/core/markers.py` & `pccm-0.4.7/pccm/core/markers.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/core/parsers.py` & `pccm-0.4.7/pccm/core/parsers.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/core/pycore.py` & `pccm-0.4.7/pccm/core/pycore.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/extension.py` & `pccm-0.4.7/pccm/extension.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/graph/__init__.py` & `pccm-0.4.7/pccm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/libs/numpylib.py` & `pccm-0.4.7/pccm/libs/numpylib.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/libs/stl.py` & `pccm-0.4.7/pccm/libs/stl.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/libs/tvten.py` & `pccm-0.4.7/pccm/libs/tvten.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/middlewares/__init__.py` & `pccm-0.4.7/pccm/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/middlewares/expose_main.py` & `pccm-0.4.7/pccm/middlewares/expose_main.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/middlewares/pybind.py` & `pccm-0.4.7/pccm/middlewares/pybind.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/source/__init__.py` & `pccm-0.4.7/pccm/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/source/core.py` & `pccm-0.4.7/pccm/source/core.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/stubs/__init__.py` & `pccm-0.4.7/pccm/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/targets/cuda.py` & `pccm-0.4.7/pccm/targets/cuda.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/targets/cuda_ptx.py` & `pccm-0.4.7/pccm/targets/cuda_ptx.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/test_data/__init__.py` & `pccm-0.4.7/pccm/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/test_data/example.py` & `pccm-0.4.7/pccm/test_data/example.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/test_data/mod.py` & `pccm-0.4.7/pccm/test_data/mod.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm/utils.py` & `pccm-0.4.7/pccm/utils.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/pccm.egg-info/PKG-INFO` & `pccm-0.4.7/pccm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccm
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python C++ Code Manager.
 Home-page: https://github.com/FindDefinition/PCCM
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pccm-0.4.6/pccm.egg-info/SOURCES.txt` & `pccm-0.4.7/pccm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/setup.py` & `pccm-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.6/test/test_core.py` & `pccm-0.4.7/test/test_core.py`

 * *Files identical despite different names*

