# Comparing `tmp/saibr-0.1.2.tar.gz` & `tmp/saibr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/saibr-0.1.2.tar", last modified: Mon Jan 23 19:36:59 2023, max compression
+gzip compressed data, was "saibr-0.1.3.tar", last modified: Wed Apr 26 14:31:49 2023, max compression
```

## Comparing `saibr-0.1.2.tar` & `saibr-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-23 19:36:59.000000 saibr-0.1.2/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 saibr-0.1.2/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     1413 2023-01-23 19:36:59.000000 saibr-0.1.2/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      833 2023-01-16 18:55:27.000000 saibr-0.1.2/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-23 19:36:59.000000 saibr-0.1.2/saibr/
--rw-r--r--   0 blandt   (743162876) 1934034978       63 2023-01-23 19:24:43.000000 saibr-0.1.2/saibr/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978      319 2023-01-14 15:33:40.000000 saibr-0.1.2/saibr/legacy.py
--rw-r--r--   0 blandt   (743162876) 1934034978     3094 2023-01-14 14:49:51.000000 saibr-0.1.2/saibr/misc.py
--rw-r--r--   0 blandt   (743162876) 1934034978    19923 2023-01-16 18:18:13.000000 saibr-0.1.2/saibr/saibr.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-01-23 19:36:59.000000 saibr-0.1.2/saibr.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     1413 2023-01-23 19:36:58.000000 saibr-0.1.2/saibr.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      243 2023-01-23 19:36:58.000000 saibr-0.1.2/saibr.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-01-23 19:36:58.000000 saibr-0.1.2/saibr.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       82 2023-01-23 19:36:58.000000 saibr-0.1.2/saibr.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-01-23 19:36:58.000000 saibr-0.1.2/saibr.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-01-23 19:36:59.000000 saibr-0.1.2/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      901 2023-01-23 19:36:35.000000 saibr-0.1.2/setup.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.020202 saibr-0.1.3/
+-rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 saibr-0.1.3/LICENSE
+-rw-r--r--   0 blandt   (743162876) 1934034978     1492 2023-04-26 14:31:49.020418 saibr-0.1.3/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      834 2023-01-23 21:47:17.000000 saibr-0.1.3/README.md
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.004396 saibr-0.1.3/saibr/
+-rw-r--r--   0 blandt   (743162876) 1934034978       63 2023-01-23 19:24:43.000000 saibr-0.1.3/saibr/__init__.py
+-rw-r--r--   0 blandt   (743162876) 1934034978      319 2023-01-14 15:33:40.000000 saibr-0.1.3/saibr/legacy.py
+-rw-r--r--   0 blandt   (743162876) 1934034978     3094 2023-01-14 14:49:51.000000 saibr-0.1.3/saibr/misc.py
+-rw-r--r--   0 blandt   (743162876) 1934034978    19923 2023-01-16 18:18:13.000000 saibr-0.1.3/saibr/saibr.py
+drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:31:49.019304 saibr-0.1.3/saibr.egg-info/
+-rw-r--r--   0 blandt   (743162876) 1934034978     1492 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/PKG-INFO
+-rw-r--r--   0 blandt   (743162876) 1934034978      243 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/SOURCES.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/dependency_links.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978       82 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/requires.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-04-26 14:31:48.000000 saibr-0.1.3/saibr.egg-info/top_level.txt
+-rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:31:49.022991 saibr-0.1.3/setup.cfg
+-rw-r--r--   0 blandt   (743162876) 1934034978      997 2023-04-26 14:31:32.000000 saibr-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `saibr-0.1.2/LICENSE` & `saibr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saibr-0.1.2/PKG-INFO` & `saibr-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: saibr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: https://github.com/goehringlab/saibr_python
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/goehringlab/saibr_python
 Description: # SAIBR (python)
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/saibr/)](https://pypi.org/project/saibr)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goehringlab/saibr_python/HEAD?filepath=%2Fscripts/SAIBRdemonstration.ipynb)
         
         
@@ -29,9 +30,10 @@
         [Creative Commons Attribution 4.0 International License][cc-by].
         
         [![CC BY 4.0][cc-by-image]][cc-by]
         
         [cc-by]: http://creativecommons.org/licenses/by/4.0/
         [cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
         [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `saibr-0.1.2/README.md` & `saibr-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 This work is licensed under a
 [Creative Commons Attribution 4.0 International License][cc-by].
 
 [![CC BY 4.0][cc-by-image]][cc-by]
 
 [cc-by]: http://creativecommons.org/licenses/by/4.0/
 [cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
-[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
```

### Comparing `saibr-0.1.2/saibr/misc.py` & `saibr-0.1.3/saibr/misc.py`

 * *Files identical despite different names*

### Comparing `saibr-0.1.2/saibr/saibr.py` & `saibr-0.1.3/saibr/saibr.py`

 * *Files identical despite different names*

### Comparing `saibr-0.1.2/saibr.egg-info/PKG-INFO` & `saibr-0.1.3/saibr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: saibr
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: https://github.com/goehringlab/saibr_python
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
+Project-URL: Source Code, https://github.com/goehringlab/saibr_python
 Description: # SAIBR (python)
         
         [![CC BY 4.0][cc-by-shield]][cc-by]
         [![PyPi version](https://badgen.net/pypi/v/saibr/)](https://pypi.org/project/saibr)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goehringlab/saibr_python/HEAD?filepath=%2Fscripts/SAIBRdemonstration.ipynb)
         
         
@@ -29,9 +30,10 @@
         [Creative Commons Attribution 4.0 International License][cc-by].
         
         [![CC BY 4.0][cc-by-image]][cc-by]
         
         [cc-by]: http://creativecommons.org/licenses/by/4.0/
         [cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
         [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `saibr-0.1.2/setup.py` & `saibr-0.1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='saibr',
-    version='0.1.2',
+    version='0.1.3',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     url='https://github.com/goehringlab/saibr_python',
     install_requires=['numpy',
                       'matplotlib',
@@ -18,9 +18,12 @@
                       'ipywidgets',
                       'scikit-learn',
                       'scikit-image',
                       'jupyter',
                       'opencv-python'],
     description='Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images',
     long_description=long_description,
-    long_description_content_type='text/markdown'
+    long_description_content_type='text/markdown',
+    project_urls={
+        "Source Code": "https://github.com/goehringlab/saibr_python",
+    }
 )
```

