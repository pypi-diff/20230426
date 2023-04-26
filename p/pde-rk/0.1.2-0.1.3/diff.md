# Comparing `tmp/pde-rk-0.1.2.tar.gz` & `tmp/pde-rk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pde-rk-0.1.2.tar", last modified: Tue Jan 24 10:07:38 2023, max compression
+gzip compressed data, was "pde-rk-0.1.3.tar", last modified: Wed Apr 26 14:22:21 2023, max compression
```

## Comparing `pde-rk-0.1.2.tar` & `pde-rk-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:07:37.994707 pde-rk-0.1.2/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 pde-rk-0.1.2/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     2015 2023-01-24 10:07:37.994945 pde-rk-0.1.2/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     1303 2023-01-24 10:06:48.000000 pde-rk-0.1.2/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:07:37.977778 pde-rk-0.1.2/pde_rk/
--rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-01-23 17:09:04.000000 pde-rk-0.1.2/pde_rk/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978     6824 2023-01-23 17:09:04.000000 pde-rk-0.1.2/pde_rk/pde.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:07:37.993388 pde-rk-0.1.2/pde_rk.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     2015 2023-01-24 10:07:37.000000 pde-rk-0.1.2/pde_rk.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      218 2023-01-24 10:07:37.000000 pde-rk-0.1.2/pde_rk.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-24 10:07:37.000000 pde-rk-0.1.2/pde_rk.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-01-24 10:07:37.000000 pde-rk-0.1.2/pde_rk.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-01-24 10:07:37.000000 pde-rk-0.1.2/pde_rk.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-24 10:07:37.997790 pde-rk-0.1.2/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      571 2023-01-24 10:06:48.000000 pde-rk-0.1.2/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.794171 pde-rk-0.1.3/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 pde-rk-0.1.3/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-04-26 14:22:21.794451 pde-rk-0.1.3/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978     1303 2023-01-24 10:06:48.000000 pde-rk-0.1.3/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.778601 pde-rk-0.1.3/pde_rk/
+-rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-01-23 17:09:04.000000 pde-rk-0.1.3/pde_rk/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978     6824 2023-01-23 17:09:04.000000 pde-rk-0.1.3/pde_rk/pde.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.793128 pde-rk-0.1.3/pde_rk.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      218 2023-04-26 14:22:20.000000 pde-rk-0.1.3/pde_rk.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/top_level.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:22:21.797444 pde-rk-0.1.3/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978      666 2023-04-26 14:21:31.000000 pde-rk-0.1.3/setup.py
```

### Comparing `pde-rk-0.1.2/LICENSE` & `pde-rk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pde-rk-0.1.2/PKG-INFO` & `pde-rk-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pde-rk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for simulating one-dimensional PDE models with and adaptive Runge-Kutta scheme
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/pde-rk
 Description: # pde-rk
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/pde-rk/HEAD?filepath=%2Fscripts/simulate_par.ipynb)
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/pde-rk/)](https://pypi.org/project/pde-rk)
         
         Functions for simulating PDE models with an adaptive Runge-Kutta scheme
```

### Comparing `pde-rk-0.1.2/README.md` & `pde-rk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pde-rk-0.1.2/pde_rk/pde.py` & `pde-rk-0.1.3/pde_rk/pde.py`

 * *Files identical despite different names*

### Comparing `pde-rk-0.1.2/pde_rk.egg-info/PKG-INFO` & `pde-rk-0.1.3/pde_rk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pde-rk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for simulating one-dimensional PDE models with and adaptive Runge-Kutta scheme
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/pde-rk
 Description: # pde-rk
         
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/pde-rk/HEAD?filepath=%2Fscripts/simulate_par.ipynb)
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/pde-rk/)](https://pypi.org/project/pde-rk)
         
         Functions for simulating PDE models with an adaptive Runge-Kutta scheme
```

### Comparing `pde-rk-0.1.2/setup.py` & `pde-rk-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pde-rk',
-    version='0.1.2',
+    version='0.1.3',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy'],
     description='Package for simulating one-dimensional PDE models with and adaptive Runge-Kutta scheme',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+            "Source Code": "https://github.com/tsmbland/pde-rk",
+        }
 )
```

