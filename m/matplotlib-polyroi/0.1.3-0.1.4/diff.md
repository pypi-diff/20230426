# Comparing `tmp/matplotlib-polyroi-0.1.3.tar.gz` & `tmp/matplotlib-polyroi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matplotlib-polyroi-0.1.3.tar", last modified: Tue Jan 24 10:02:14 2023, max compression
+gzip compressed data, was "matplotlib-polyroi-0.1.4.tar", last modified: Wed Apr 26 14:48:43 2023, max compression
```

## Comparing `matplotlib-polyroi-0.1.3.tar` & `matplotlib-polyroi-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:02:14.000000 matplotlib-polyroi-0.1.3/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 matplotlib-polyroi-0.1.3/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     2077 2023-01-24 10:02:14.000000 matplotlib-polyroi-0.1.3/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     1344 2023-01-24 09:54:13.000000 matplotlib-polyroi-0.1.3/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:02:14.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi/
--rw-r--r--   0 blandt   (743162876) 1934034978       40 2023-01-23 19:32:08.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      361 2023-01-24 09:26:01.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi/funcs.py
--rw-r--r--   0 blandt   (743162876) 1934034978    16086 2023-01-24 09:40:30.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi/roi.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-24 10:02:14.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     2077 2023-01-24 10:02:13.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      330 2023-01-24 10:02:13.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-24 10:02:13.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       55 2023-01-24 10:02:13.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-01-24 10:02:13.000000 matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-24 10:02:14.000000 matplotlib-polyroi-0.1.3/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      782 2023-01-24 10:01:45.000000 matplotlib-polyroi-0.1.3/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.910197 matplotlib-polyroi-0.1.4/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 matplotlib-polyroi-0.1.4/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     2150 2023-04-26 14:48:43.910567 matplotlib-polyroi-0.1.4/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978     1344 2023-01-24 09:54:13.000000 matplotlib-polyroi-0.1.4/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.896574 matplotlib-polyroi-0.1.4/matplotlib_polyroi/
+-rw-r--r--   0 blandt   (743162876) 1934034978       40 2023-01-23 19:32:08.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978      361 2023-01-24 09:26:01.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/funcs.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    16086 2023-01-24 09:40:30.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi/roi.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:48:43.908325 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     2150 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      330 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       55 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-04-26 14:48:43.000000 matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/top_level.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:48:43.915171 matplotlib-polyroi-0.1.4/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978      881 2023-04-26 14:48:30.000000 matplotlib-polyroi-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `matplotlib-polyroi-0.1.3/LICENSE` & `matplotlib-polyroi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib-polyroi-0.1.3/PKG-INFO` & `matplotlib-polyroi-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: matplotlib-polyroi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/matplotlib-polyroi
 Description: # matplotlib-polyroi
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/matplotlib-polyroi/)](https://pypi.org/project/matplotlib-polyroi)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/matplotlib-polyroi/HEAD?filepath=%2Fscripts/Demonstration.ipynb)
```

### Comparing `matplotlib-polyroi-0.1.3/README.md` & `matplotlib-polyroi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib-polyroi-0.1.3/matplotlib_polyroi/roi.py` & `matplotlib-polyroi-0.1.4/matplotlib_polyroi/roi.py`

 * *Files identical despite different names*

### Comparing `matplotlib-polyroi-0.1.3/matplotlib_polyroi.egg-info/PKG-INFO` & `matplotlib-polyroi-0.1.4/matplotlib_polyroi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: matplotlib-polyroi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/matplotlib-polyroi
 Description: # matplotlib-polyroi
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/matplotlib-polyroi/)](https://pypi.org/project/matplotlib-polyroi)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/matplotlib-polyroi/HEAD?filepath=%2Fscripts/Demonstration.ipynb)
```

### Comparing `matplotlib-polyroi-0.1.3/setup.py` & `matplotlib-polyroi-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='matplotlib-polyroi',
-    version='0.1.3',
+    version='0.1.4',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
                       'ipywidgets',
                       'scikit-image',
                       'jupyter'],
     description='Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Source Code": "https://github.com/tsmbland/matplotlib-polyroi",
+    }
 )
```

