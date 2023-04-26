# Comparing `tmp/pygentrification-0.0.3.tar.gz` & `tmp/pygentrification-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentrification-0.0.3.tar", last modified: Tue Apr 25 18:52:56 2023, max compression
+gzip compressed data, was "pygentrification-0.0.4.tar", last modified: Tue Apr 25 19:05:09 2023, max compression
```

## Comparing `pygentrification-0.0.3.tar` & `pygentrification-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 18:52:56.473042 pygentrification-0.0.3/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     1508 2023-04-24 16:51:27.000000 pygentrification-0.0.3/LICENSE.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 18:52:56.472055 pygentrification-0.0.3/PKG-INFO
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19103 2023-04-25 18:50:19.000000 pygentrification-0.0.3/README.md
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      838 2023-04-25 18:50:36.000000 pygentrification-0.0.3/pyproject.toml
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       38 2023-04-25 18:52:56.473223 pygentrification-0.0.3/setup.cfg
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 18:52:56.445899 pygentrification-0.0.3/src/
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 18:52:56.464042 pygentrification-0.0.3/src/pygentrification/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-18 20:39:15.000000 pygentrification-0.0.3/src/pygentrification/__init__.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22690 2023-04-25 18:49:50.000000 pygentrification-0.0.3/src/pygentrification/api_calls.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    31174 2023-04-25 18:45:07.000000 pygentrification-0.0.3/src/pygentrification/bates_freeman_indices.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     9748 2023-04-24 19:28:05.000000 pygentrification-0.0.3/src/pygentrification/ding_index.py
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22886 2023-04-25 18:49:09.000000 pygentrification-0.0.3/src/pygentrification/folium_funcs.py
-drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 18:52:56.470896 pygentrification-0.0.3/src/pygentrification.egg-info/
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 18:52:56.000000 pygentrification-0.0.3/src/pygentrification.egg-info/PKG-INFO
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      440 2023-04-25 18:52:56.000000 pygentrification-0.0.3/src/pygentrification.egg-info/SOURCES.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-25 18:52:56.000000 pygentrification-0.0.3/src/pygentrification.egg-info/dependency_links.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       61 2023-04-25 18:52:56.000000 pygentrification-0.0.3/src/pygentrification.egg-info/requires.txt
--rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       17 2023-04-25 18:52:56.000000 pygentrification-0.0.3/src/pygentrification.egg-info/top_level.txt
+drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.073589 pygentrification-0.0.4/
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     1508 2023-04-24 16:51:27.000000 pygentrification-0.0.4/LICENSE.txt
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 19:05:09.072774 pygentrification-0.0.4/PKG-INFO
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19103 2023-04-25 18:50:19.000000 pygentrification-0.0.4/README.md
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      838 2023-04-25 19:04:15.000000 pygentrification-0.0.4/pyproject.toml
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       38 2023-04-25 19:05:09.073770 pygentrification-0.0.4/setup.cfg
+drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.023789 pygentrification-0.0.4/src/
+drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.063659 pygentrification-0.0.4/src/pygentrification/
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-18 20:39:15.000000 pygentrification-0.0.4/src/pygentrification/__init__.py
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22697 2023-04-25 19:04:05.000000 pygentrification-0.0.4/src/pygentrification/api_calls.py
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    31174 2023-04-25 18:45:07.000000 pygentrification-0.0.4/src/pygentrification/bates_freeman_indices.py
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)     9748 2023-04-24 19:28:05.000000 pygentrification-0.0.4/src/pygentrification/ding_index.py
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    22886 2023-04-25 18:49:09.000000 pygentrification-0.0.4/src/pygentrification/folium_funcs.py
+drwxr-xr-x   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        0 2023-04-25 19:05:09.069750 pygentrification-0.0.4/src/pygentrification.egg-info/
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)    19710 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/PKG-INFO
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)      440 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/SOURCES.txt
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)        1 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/dependency_links.txt
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       61 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/requires.txt
+-rw-r--r--   0 wc555    (407855680) DREXEL\Domain Users (1823260766)       17 2023-04-25 19:05:09.000000 pygentrification-0.0.4/src/pygentrification.egg-info/top_level.txt
```

### Comparing `pygentrification-0.0.3/LICENSE.txt` & `pygentrification-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.3/PKG-INFO` & `pygentrification-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentrification
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for calculating and visualizing gentrification indices from published academic research
 Author-email: Winn Costantini <wc555@drexel.edu>, Adam Thompson <adam.thompson0001@temple.edu>, Josh Scrabeck <joshua.scrabeck@temple.edu>
 Project-URL: Homepage, https://github.com/joshscrabeck/pygentrification
 Keywords: gentrification
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: !=3.10,>=3.9
```

### Comparing `pygentrification-0.0.3/README.md` & `pygentrification-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.3/pyproject.toml` & `pygentrification-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygentrification"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Winn Costantini", email="wc555@drexel.edu"}, {name = "Adam Thompson", email = "adam.thompson0001@temple.edu"}, {name = "Josh Scrabeck", email = "joshua.scrabeck@temple.edu"},
 ]
 description = "A python package for calculating and visualizing gentrification indices from published academic research"
 readme = "README.md"
 requires-python = ">=3.9, !=3.10"
 keywords = ["gentrification"]
```

### Comparing `pygentrification-0.0.3/src/pygentrification/api_calls.py` & `pygentrification-0.0.4/src/pygentrification/api_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from io import BytesIO
 import requests
 import pandas as pd
 from zipfile import ZipFile
 import urllib
 import os
 os.environ['USE_PYGEOS'] = '0'
-import geopandas
+import geopandas as gpd
 import warnings
 from tobler.area_weighted import area_interpolate
 from functools import reduce
 
 #%%
 
 ###Constants needed for acs and census api requests###
```

### Comparing `pygentrification-0.0.3/src/pygentrification/bates_freeman_indices.py` & `pygentrification-0.0.4/src/pygentrification/bates_freeman_indices.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.3/src/pygentrification/ding_index.py` & `pygentrification-0.0.4/src/pygentrification/ding_index.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.3/src/pygentrification/folium_funcs.py` & `pygentrification-0.0.4/src/pygentrification/folium_funcs.py`

 * *Files identical despite different names*

### Comparing `pygentrification-0.0.3/src/pygentrification.egg-info/PKG-INFO` & `pygentrification-0.0.4/src/pygentrification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentrification
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for calculating and visualizing gentrification indices from published academic research
 Author-email: Winn Costantini <wc555@drexel.edu>, Adam Thompson <adam.thompson0001@temple.edu>, Josh Scrabeck <joshua.scrabeck@temple.edu>
 Project-URL: Homepage, https://github.com/joshscrabeck/pygentrification
 Keywords: gentrification
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: !=3.10,>=3.9
```

