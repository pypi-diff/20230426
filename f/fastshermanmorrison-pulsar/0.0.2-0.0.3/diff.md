# Comparing `tmp/fastshermanmorrison-pulsar-0.0.2.tar.gz` & `tmp/fastshermanmorrison-pulsar-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastshermanmorrison-pulsar-0.0.2.tar", last modified: Wed Apr 26 11:35:17 2023, max compression
+gzip compressed data, was "fastshermanmorrison-pulsar-0.0.3.tar", last modified: Wed Apr 26 11:45:16 2023, max compression
```

## Comparing `fastshermanmorrison-pulsar-0.0.2.tar` & `fastshermanmorrison-pulsar-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:35:17.492306 fastshermanmorrison-pulsar-0.0.2/
--rw-r--r--   0 vhaasteren   (501) staff       (20)      107 2023-04-21 13:47:28.000000 fastshermanmorrison-pulsar-0.0.2/AUTHORS.md
--rw-r--r--   0 vhaasteren   (501) staff       (20)     1077 2023-04-21 13:46:04.000000 fastshermanmorrison-pulsar-0.0.2/LICENSE
--rw-r--r--   0 vhaasteren   (501) staff       (20)     2645 2023-04-26 11:35:17.492194 fastshermanmorrison-pulsar-0.0.2/PKG-INFO
--rw-r--r--   0 vhaasteren   (501) staff       (20)      668 2023-04-25 09:50:33.000000 fastshermanmorrison-pulsar-0.0.2/README.md
-drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:35:17.491489 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/
--rw-r--r--   0 vhaasteren   (501) staff       (20)       67 2023-04-26 04:45:55.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/__init__.py
--rw-r--r--   0 vhaasteren   (501) staff       (20)  1585459 2023-04-25 12:56:51.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/cython_fastshermanmorrison.c
--rw-r--r--   0 vhaasteren   (501) staff       (20)     5708 2023-04-25 10:01:09.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/fastshermanmorrison.c
--rw-r--r--   0 vhaasteren   (501) staff       (20)     6192 2023-04-24 15:24:23.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/fastshermanmorrison.py
--rw-r--r--   0 vhaasteren   (501) staff       (20)       22 2023-04-26 11:35:06.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/version.py
-drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:35:17.492022 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/
--rw-r--r--   0 vhaasteren   (501) staff       (20)     2645 2023-04-26 11:35:17.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/PKG-INFO
--rw-r--r--   0 vhaasteren   (501) staff       (20)      498 2023-04-26 11:35:17.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/SOURCES.txt
--rw-r--r--   0 vhaasteren   (501) staff       (20)        1 2023-04-26 11:35:17.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/dependency_links.txt
--rw-r--r--   0 vhaasteren   (501) staff       (20)        1 2023-04-26 11:11:41.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/not-zip-safe
--rw-r--r--   0 vhaasteren   (501) staff       (20)       20 2023-04-26 11:35:17.000000 fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/top_level.txt
--rw-r--r--   0 vhaasteren   (501) staff       (20)      769 2023-04-26 11:34:59.000000 fastshermanmorrison-pulsar-0.0.2/pyproject.toml
--rw-r--r--   0 vhaasteren   (501) staff       (20)       38 2023-04-26 11:35:17.492339 fastshermanmorrison-pulsar-0.0.2/setup.cfg
--rwxr-xr-x   0 vhaasteren   (501) staff       (20)     2116 2023-04-26 11:34:52.000000 fastshermanmorrison-pulsar-0.0.2/setup.py
+drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:45:16.865570 fastshermanmorrison-pulsar-0.0.3/
+-rw-r--r--   0 vhaasteren   (501) staff       (20)      107 2023-04-21 13:47:28.000000 fastshermanmorrison-pulsar-0.0.3/AUTHORS.md
+-rw-r--r--   0 vhaasteren   (501) staff       (20)     1077 2023-04-21 13:46:04.000000 fastshermanmorrison-pulsar-0.0.3/LICENSE
+-rw-r--r--   0 vhaasteren   (501) staff       (20)      160 2023-04-26 11:43:51.000000 fastshermanmorrison-pulsar-0.0.3/MANIFEST.in
+-rw-r--r--   0 vhaasteren   (501) staff       (20)     2645 2023-04-26 11:45:16.865464 fastshermanmorrison-pulsar-0.0.3/PKG-INFO
+-rw-r--r--   0 vhaasteren   (501) staff       (20)      668 2023-04-25 09:50:33.000000 fastshermanmorrison-pulsar-0.0.3/README.md
+drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:45:16.864752 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/
+-rw-r--r--   0 vhaasteren   (501) staff       (20)       67 2023-04-26 04:45:55.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/__init__.py
+-rw-r--r--   0 vhaasteren   (501) staff       (20)  1585459 2023-04-25 12:56:51.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/cython_fastshermanmorrison.c
+-rw-r--r--   0 vhaasteren   (501) staff       (20)    31466 2023-04-25 12:33:37.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/cython_fastshermanmorrison.pyx
+-rw-r--r--   0 vhaasteren   (501) staff       (20)     5708 2023-04-25 10:01:09.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/fastshermanmorrison.c
+-rw-r--r--   0 vhaasteren   (501) staff       (20)     6192 2023-04-24 15:24:23.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/fastshermanmorrison.py
+-rw-r--r--   0 vhaasteren   (501) staff       (20)       22 2023-04-26 11:45:10.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/version.py
+drwxr-xr-x   0 vhaasteren   (501) staff       (20)        0 2023-04-26 11:45:16.865296 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/
+-rw-r--r--   0 vhaasteren   (501) staff       (20)     2645 2023-04-26 11:45:16.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/PKG-INFO
+-rw-r--r--   0 vhaasteren   (501) staff       (20)      561 2023-04-26 11:45:16.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/SOURCES.txt
+-rw-r--r--   0 vhaasteren   (501) staff       (20)        1 2023-04-26 11:45:16.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/dependency_links.txt
+-rw-r--r--   0 vhaasteren   (501) staff       (20)        1 2023-04-26 11:11:41.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/not-zip-safe
+-rw-r--r--   0 vhaasteren   (501) staff       (20)       20 2023-04-26 11:45:16.000000 fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/top_level.txt
+-rw-r--r--   0 vhaasteren   (501) staff       (20)      769 2023-04-26 11:45:04.000000 fastshermanmorrison-pulsar-0.0.3/pyproject.toml
+-rw-r--r--   0 vhaasteren   (501) staff       (20)       38 2023-04-26 11:45:16.865602 fastshermanmorrison-pulsar-0.0.3/setup.cfg
+-rwxr-xr-x   0 vhaasteren   (501) staff       (20)     2116 2023-04-26 11:45:08.000000 fastshermanmorrison-pulsar-0.0.3/setup.py
```

### Comparing `fastshermanmorrison-pulsar-0.0.2/LICENSE` & `fastshermanmorrison-pulsar-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastshermanmorrison-pulsar-0.0.2/PKG-INFO` & `fastshermanmorrison-pulsar-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastshermanmorrison-pulsar
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Enterprise add-on FastShermanMorrison for optimized EcorrKernel calculations
 Home-page: http://github.com/vhaasteren/fastshermanmorrison/
 Author: Rutger van Haasteren
 Author-email: Rutger van Haasteren <rutger@vhaasteren.com>
 License: MIT License
         
         Copyright (c) 2023 Rutger van Haasteren
```

### Comparing `fastshermanmorrison-pulsar-0.0.2/README.md` & `fastshermanmorrison-pulsar-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/cython_fastshermanmorrison.c` & `fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/cython_fastshermanmorrison.c`

 * *Files identical despite different names*

### Comparing `fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/fastshermanmorrison.c` & `fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/fastshermanmorrison.c`

 * *Files identical despite different names*

### Comparing `fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison/fastshermanmorrison.py` & `fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison/fastshermanmorrison.py`

 * *Files identical despite different names*

### Comparing `fastshermanmorrison-pulsar-0.0.2/fastshermanmorrison_pulsar.egg-info/PKG-INFO` & `fastshermanmorrison-pulsar-0.0.3/fastshermanmorrison_pulsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastshermanmorrison-pulsar
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Enterprise add-on FastShermanMorrison for optimized EcorrKernel calculations
 Home-page: http://github.com/vhaasteren/fastshermanmorrison/
 Author: Rutger van Haasteren
 Author-email: Rutger van Haasteren <rutger@vhaasteren.com>
 License: MIT License
         
         Copyright (c) 2023 Rutger van Haasteren
```

### Comparing `fastshermanmorrison-pulsar-0.0.2/pyproject.toml` & `fastshermanmorrison-pulsar-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "numpy>=1.16.3", "cython>=0.29.32", "scipy>=1.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastshermanmorrison-pulsar"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Rutger van Haasteren", email="rutger@vhaasteren.com"},
 ]
 description = "The Enterprise add-on FastShermanMorrison for optimized EcorrKernel calculations"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `fastshermanmorrison-pulsar-0.0.2/setup.py` & `fastshermanmorrison-pulsar-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools import Extension
 from distutils.command.build import build as build_orig
 
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 ext_modules=[
     Extension(
         name='fastshermanmorrison.cython_fastshermanmorrison',
         sources=[
                 'fastshermanmorrison/cython_fastshermanmorrison.pyx',
                 'fastshermanmorrison/fastshermanmorrison.c'
```

