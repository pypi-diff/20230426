# Comparing `tmp/scoobi-0.0.1.tar.gz` & `tmp/scoobi-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.tar", last modified: Tue Apr 25 15:51:05 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.1.tar", last modified: Tue Apr 25 15:54:27 2023, max compression
```

## Comparing `scoobi-0.0.1.tar` & `scoobi-0.0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:51:05.325760 scoobi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 15:50:54.000000 scoobi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-25 15:51:05.325760 scoobi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 15:50:54.000000 scoobi-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 15:51:05.325760 scoobi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 15:50:54.000000 scoobi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:51:05.321760 scoobi-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:51:05.321760 scoobi-0.0.1/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-25 15:50:54.000000 scoobi-0.0.1/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-25 15:50:54.000000 scoobi-0.0.1/src/scoobi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:51:05.325760 scoobi-0.0.1/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 15:51:05.000000 scoobi-0.0.1/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.314221 scoobi-0.0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.314221 scoobi-0.0.1.1/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-25 15:54:16.000000 scoobi-0.0.1.1/src/scoobi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:54:27.318221 scoobi-0.0.1.1/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 15:54:27.000000 scoobi-0.0.1.1/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1/LICENSE` & `scoobi-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1/PKG-INFO` & `scoobi-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scoobi-0.0.1/README.md` & `scoobi-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1/setup.py` & `scoobi-0.0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1',
+    version = '0.0.1.1',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
@@ -18,15 +18,15 @@
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
                  "License :: OSI Approved :: BSD License",
                  "Intended Audience :: Science/Research",
                  ],
     long_description=desc,
     long_description_content_type = "text/markdown",
-    install_requires=["astropy>=4.2.1", "numpy>= 1.20.3", "exifread"
+    install_requires=["astropy", "numpy", "exifread"
                       ],
     extras_require = {
         "dev" : ["pytest>=3.7",
         ]
     },
      entry_points={ 
         "console_scripts": [
```

### Comparing `scoobi-0.0.1/src/scoobi/__init__.py` & `scoobi-0.0.1.1/src/scoobi/__init__.py`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1/src/scoobi/cli.py` & `scoobi-0.0.1.1/src/scoobi/cli.py`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.1/src/scoobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

