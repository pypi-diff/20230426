# Comparing `tmp/detritalpy-1.3.7.tar.gz` & `tmp/detritalpy-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/detritalpy-1.3.7.tar", last modified: Fri Mar 27 01:38:22 2020, max compression
+gzip compressed data, was "dist/detritalpy-1.3.8.tar", last modified: Fri Mar 27 01:41:45 2020, max compression
```

## Comparing `detritalpy-1.3.7.tar` & `detritalpy-1.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:38:22.000000 detritalpy-1.3.7/
--rw-r--r--   0 gsharman   (501) staff       (20)     7915 2020-03-27 01:38:22.000000 detritalpy-1.3.7/PKG-INFO
--rw-r--r--   0 gsharman   (501) staff       (20)     6847 2020-03-25 19:14:30.000000 detritalpy-1.3.7/README.md
-drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy/
--rw-r--r--   0 gsharman   (501) staff       (20)    23110 2020-03-25 17:38:12.000000 detritalpy-1.3.7/detritalpy/MDAfuncs.py
--rw-------   0 gsharman   (501) staff       (20)       96 2019-12-30 17:14:51.000000 detritalpy-1.3.7/detritalpy/__init__.py
--rw-r--r--   0 gsharman   (501) staff       (20)    20740 2020-03-25 15:43:17.000000 detritalpy-1.3.7/detritalpy/adaptiveKDE.py
--rw-r--r--   0 gsharman   (501) staff       (20)   190976 2020-03-26 16:21:21.000000 detritalpy-1.3.7/detritalpy/detritalFuncs.py
--rw-------   0 gsharman   (501) staff       (20)   169732 2020-03-25 18:45:02.000000 detritalpy-1.3.7/detritalpy/detritalFuncs_axisSplit.py
-drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/
--rw-r--r--   0 gsharman   (501) staff       (20)     7915 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/PKG-INFO
--rw-r--r--   0 gsharman   (501) staff       (20)      528 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/SOURCES.txt
--rw-r--r--   0 gsharman   (501) staff       (20)        1 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/dependency_links.txt
--rw-r--r--   0 gsharman   (501) staff       (20)       90 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/requires.txt
--rw-r--r--   0 gsharman   (501) staff       (20)       11 2020-03-27 01:38:22.000000 detritalpy-1.3.7/detritalpy.egg-info/top_level.txt
--rw-r--r--   0 gsharman   (501) staff       (20)       38 2020-03-27 01:38:22.000000 detritalpy-1.3.7/setup.cfg
--rw-r--r--   0 gsharman   (501) staff       (20)     1098 2020-03-27 01:37:54.000000 detritalpy-1.3.7/setup.py
+drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:41:45.000000 detritalpy-1.3.8/
+-rw-r--r--   0 gsharman   (501) staff       (20)     7915 2020-03-27 01:41:45.000000 detritalpy-1.3.8/PKG-INFO
+-rw-r--r--   0 gsharman   (501) staff       (20)     6847 2020-03-25 19:14:30.000000 detritalpy-1.3.8/README.md
+drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy/
+-rw-r--r--   0 gsharman   (501) staff       (20)    23110 2020-03-25 17:38:12.000000 detritalpy-1.3.8/detritalpy/MDAfuncs.py
+-rw-------   0 gsharman   (501) staff       (20)       96 2019-12-30 17:14:51.000000 detritalpy-1.3.8/detritalpy/__init__.py
+-rw-r--r--   0 gsharman   (501) staff       (20)    20740 2020-03-25 15:43:17.000000 detritalpy-1.3.8/detritalpy/adaptiveKDE.py
+-rw-r--r--   0 gsharman   (501) staff       (20)   190976 2020-03-26 16:21:21.000000 detritalpy-1.3.8/detritalpy/detritalFuncs.py
+-rw-------   0 gsharman   (501) staff       (20)   169732 2020-03-25 18:45:02.000000 detritalpy-1.3.8/detritalpy/detritalFuncs_axisSplit.py
+drwxr-xr-x   0 gsharman   (501) staff       (20)        0 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/
+-rw-r--r--   0 gsharman   (501) staff       (20)     7915 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/PKG-INFO
+-rw-r--r--   0 gsharman   (501) staff       (20)      528 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gsharman   (501) staff       (20)        1 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gsharman   (501) staff       (20)       90 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/requires.txt
+-rw-r--r--   0 gsharman   (501) staff       (20)       11 2020-03-27 01:41:45.000000 detritalpy-1.3.8/detritalpy.egg-info/top_level.txt
+-rw-r--r--   0 gsharman   (501) staff       (20)       38 2020-03-27 01:41:45.000000 detritalpy-1.3.8/setup.cfg
+-rw-r--r--   0 gsharman   (501) staff       (20)     1098 2020-03-27 01:40:25.000000 detritalpy-1.3.8/setup.py
```

### Comparing `detritalpy-1.3.7/PKG-INFO` & `detritalpy-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: detritalpy
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python-based toolset for visualizing and analyzing detrital geo-thermochronologic data
 Home-page: https://github.com/grsharman/detritalpy
 Author: Glenn Sharman
 Author-email: gsharman@uark.edu
 License: UNKNOWN
-Download-URL: https://github.com/grsharman/detritalPy/archive/v1.3.7.tar.gz
+Download-URL: https://github.com/grsharman/detritalPy/archive/v1.3.8.tar.gz
 Description: ## Description
         
         detritalPy is a Python module for visualizing and analyzing detrital geo-thermochronologic data. Designed to be implemented via a Jupyter Notebook, detritalPy aims to provide an efficient means of processing and analyzing large detrital mineral isotopic and geochemical datasets. For more information, please refer to [Sharman et al., 2018](https://doi.org/10.1002/dep2.45).
         
         ## Installation
         
         <code>pip install detritalpy</code>
```

### Comparing `detritalpy-1.3.7/README.md` & `detritalpy-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/detritalpy/MDAfuncs.py` & `detritalpy-1.3.8/detritalpy/MDAfuncs.py`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/detritalpy/adaptiveKDE.py` & `detritalpy-1.3.8/detritalpy/adaptiveKDE.py`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/detritalpy/detritalFuncs.py` & `detritalpy-1.3.8/detritalpy/detritalFuncs.py`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/detritalpy/detritalFuncs_axisSplit.py` & `detritalpy-1.3.8/detritalpy/detritalFuncs_axisSplit.py`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/detritalpy.egg-info/PKG-INFO` & `detritalpy-1.3.8/detritalpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: detritalpy
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python-based toolset for visualizing and analyzing detrital geo-thermochronologic data
 Home-page: https://github.com/grsharman/detritalpy
 Author: Glenn Sharman
 Author-email: gsharman@uark.edu
 License: UNKNOWN
-Download-URL: https://github.com/grsharman/detritalPy/archive/v1.3.7.tar.gz
+Download-URL: https://github.com/grsharman/detritalPy/archive/v1.3.8.tar.gz
 Description: ## Description
         
         detritalPy is a Python module for visualizing and analyzing detrital geo-thermochronologic data. Designed to be implemented via a Jupyter Notebook, detritalPy aims to provide an efficient means of processing and analyzing large detrital mineral isotopic and geochemical datasets. For more information, please refer to [Sharman et al., 2018](https://doi.org/10.1002/dep2.45).
         
         ## Installation
         
         <code>pip install detritalpy</code>
```

### Comparing `detritalpy-1.3.7/detritalpy.egg-info/SOURCES.txt` & `detritalpy-1.3.8/detritalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `detritalpy-1.3.7/setup.py` & `detritalpy-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open('/Users/gsharman/Box/detritalPy/pip_installation/README.md', "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="detritalpy",
     packages=['detritalpy'],    
-    version="1.3.7",
+    version="1.3.8",
     author="Glenn Sharman",
     author_email="gsharman@uark.edu",
     description="A Python-based toolset for visualizing and analyzing detrital geo-thermochronologic data",
     keywords = 'detrital, zircon, provenance, stratigraphy, geochronology, thermochronology',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/grsharman/detritalpy",
-    download_url="https://github.com/grsharman/detritalPy/archive/v1.3.7.tar.gz",
+    download_url="https://github.com/grsharman/detritalPy/archive/v1.3.8.tar.gz",
     install_requires=['numpy','matplotlib','pandas','xlrd','folium','vincent','simplekml',
         'scipy','sklearn','statsmodels','peakutils'],
     classifiers=[
         "Programming Language :: Python :: 3",
         'Intended Audience :: Science/Research',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

