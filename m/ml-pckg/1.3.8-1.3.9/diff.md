# Comparing `tmp/ml_pckg-1.3.8.tar.gz` & `tmp/ml_pckg-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pckg-1.3.8.tar", last modified: Wed Apr 26 17:43:37 2023, max compression
+gzip compressed data, was "ml_pckg-1.3.9.tar", last modified: Wed Apr 26 17:45:30 2023, max compression
```

## Comparing `ml_pckg-1.3.8.tar` & `ml_pckg-1.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:43:37.686414 ml_pckg-1.3.8/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.3.8/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:43:37.686517 ml_pckg-1.3.8/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      266 2023-04-26 17:13:37.000000 ml_pckg-1.3.8/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:43:37.684890 ml_pckg-1.3.8/ml_pckg/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      172 2023-04-26 17:09:14.000000 ml_pckg-1.3.8/ml_pckg/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 ml_pckg-1.3.8/ml_pckg/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 ml_pckg-1.3.8/ml_pckg/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 ml_pckg-1.3.8/ml_pckg/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 ml_pckg-1.3.8/ml_pckg/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 ml_pckg-1.3.8/ml_pckg/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:43:37.686234 ml_pckg-1.3.8/ml_pckg.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:43:37.000000 ml_pckg-1.3.8/ml_pckg.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-26 17:43:37.000000 ml_pckg-1.3.8/ml_pckg.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 17:43:37.000000 ml_pckg-1.3.8/ml_pckg.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 17:43:37.000000 ml_pckg-1.3.8/ml_pckg.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-26 17:43:37.000000 ml_pckg-1.3.8/ml_pckg.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 17:43:37.686817 ml_pckg-1.3.8/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      855 2023-04-26 17:42:41.000000 ml_pckg-1.3.8/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:45:30.787808 ml_pckg-1.3.9/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.3.9/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:45:30.787896 ml_pckg-1.3.9/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      266 2023-04-26 17:13:37.000000 ml_pckg-1.3.9/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:45:30.786464 ml_pckg-1.3.9/ml_pckg/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      172 2023-04-26 17:09:14.000000 ml_pckg-1.3.9/ml_pckg/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 ml_pckg-1.3.9/ml_pckg/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 ml_pckg-1.3.9/ml_pckg/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 ml_pckg-1.3.9/ml_pckg/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 ml_pckg-1.3.9/ml_pckg/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 ml_pckg-1.3.9/ml_pckg/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:45:30.787631 ml_pckg-1.3.9/ml_pckg.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:45:30.000000 ml_pckg-1.3.9/ml_pckg.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-26 17:45:30.000000 ml_pckg-1.3.9/ml_pckg.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 17:45:30.000000 ml_pckg-1.3.9/ml_pckg.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 17:45:30.000000 ml_pckg-1.3.9/ml_pckg.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-26 17:45:30.000000 ml_pckg-1.3.9/ml_pckg.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 17:45:30.788185 ml_pckg-1.3.9/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      855 2023-04-26 17:43:37.000000 ml_pckg-1.3.9/setup.py
```

### Comparing `ml_pckg-1.3.8/LICENSE` & `ml_pckg-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/PKG-INFO` & `ml_pckg-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml_pckg
-Version: 1.3.8
+Version: 1.3.9
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.8.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.9.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.3.8/ml_pckg/classifiers.py` & `ml_pckg-1.3.9/ml_pckg/classifiers.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/ml_pckg/data_processing.py` & `ml_pckg-1.3.9/ml_pckg/data_processing.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/ml_pckg/linear_algebra.py` & `ml_pckg-1.3.9/ml_pckg/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/ml_pckg/metrics.py` & `ml_pckg-1.3.9/ml_pckg/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/ml_pckg/regressors.py` & `ml_pckg-1.3.9/ml_pckg/regressors.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.8/ml_pckg.egg-info/PKG-INFO` & `ml_pckg-1.3.9/ml_pckg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml-pckg
-Version: 1.3.8
+Version: 1.3.9
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.8.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.9.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.3.8/setup.py` & `ml_pckg-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 import re
 
 
-current_version = '1.3.8'
+current_version = '1.3.9'
 
 setup(
     name='ml_pckg',
     packages=['ml_pckg'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
```

