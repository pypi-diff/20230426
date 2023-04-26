# Comparing `tmp/parameter-space-2d-0.1.2.tar.gz` & `tmp/parameter-space-2d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parameter-space-2d-0.1.2.tar", last modified: Tue Jan 24 10:21:15 2023, max compression
+gzip compressed data, was "parameter-space-2d-0.1.3.tar", last modified: Wed Apr 26 14:37:04 2023, max compression
```

## Comparing `parameter-space-2d-0.1.2.tar` & `parameter-space-2d-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 parameter-space-2d-0.1.2/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     2931 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-01-24 10:19:29.000000 parameter-space-2d-0.1.2/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     2931 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      297 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       17 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       13 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/parameter_space_2d.egg-info/top_level.txt
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/paramspace2d/
--rw-r--r--   0 blandt   (743162876) 1934034978       26 2023-01-23 16:34:38.000000 parameter-space-2d-0.1.2/paramspace2d/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15422 2023-01-23 17:30:25.000000 parameter-space-2d-0.1.2/paramspace2d/paramspace.py
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-24 10:21:15.000000 parameter-space-2d-0.1.2/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      606 2023-01-24 10:21:09.000000 parameter-space-2d-0.1.2/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.386889 parameter-space-2d-0.1.3/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 parameter-space-2d-0.1.3/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     3004 2023-04-26 14:37:04.387287 parameter-space-2d-0.1.3/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-01-24 10:19:29.000000 parameter-space-2d-0.1.3/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.301099 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     3004 2023-04-26 14:37:03.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      297 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:37:03.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       17 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       13 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/top_level.txt
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.385649 parameter-space-2d-0.1.3/paramspace2d/
+-rw-r--r--   0 blandt   (743162876) 1934034978       26 2023-01-23 16:34:38.000000 parameter-space-2d-0.1.3/paramspace2d/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    15422 2023-01-23 17:30:25.000000 parameter-space-2d-0.1.3/paramspace2d/paramspace.py
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:37:04.391010 parameter-space-2d-0.1.3/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978      705 2023-04-26 14:36:54.000000 parameter-space-2d-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `parameter-space-2d-0.1.2/LICENSE` & `parameter-space-2d-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parameter-space-2d-0.1.2/PKG-INFO` & `parameter-space-2d-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: parameter-space-2d
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for performing 2D parameter space analysis for deterministic models
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/parameter-space-2d
 Description: # parameter-space-2d
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/parameter-space/HEAD?filepath=%2Fscripts/INDEX.ipynb)
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/parameter-space-2d/)](https://pypi.org/project/parameter-space-2d)
         
         <p align="center">
```

### Comparing `parameter-space-2d-0.1.2/README.md` & `parameter-space-2d-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `parameter-space-2d-0.1.2/parameter_space_2d.egg-info/PKG-INFO` & `parameter-space-2d-0.1.3/parameter_space_2d.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: parameter-space-2d
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for performing 2D parameter space analysis for deterministic models
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/parameter-space-2d
 Description: # parameter-space-2d
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/parameter-space/HEAD?filepath=%2Fscripts/INDEX.ipynb)
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/parameter-space-2d/)](https://pypi.org/project/parameter-space-2d)
         
         <p align="center">
```

### Comparing `parameter-space-2d-0.1.2/paramspace2d/paramspace.py` & `parameter-space-2d-0.1.3/paramspace2d/paramspace.py`

 * *Files identical despite different names*

### Comparing `parameter-space-2d-0.1.2/setup.py` & `parameter-space-2d-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='parameter-space-2d',
-    version='0.1.2',
+    version='0.1.3',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib'],
     description='Tools for performing 2D parameter space analysis for deterministic models',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Source Code": "https://github.com/tsmbland/parameter-space-2d",
+    }
 )
```

