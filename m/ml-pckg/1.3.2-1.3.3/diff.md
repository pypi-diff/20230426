# Comparing `tmp/ml_pckg-1.3.2.tar.gz` & `tmp/ml_pckg-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pckg-1.3.2.tar", last modified: Wed Apr 26 17:28:40 2023, max compression
+gzip compressed data, was "ml_pckg-1.3.3.tar", last modified: Wed Apr 26 17:28:53 2023, max compression
```

## Comparing `ml_pckg-1.3.2.tar` & `ml_pckg-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:40.671816 ml_pckg-1.3.2/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.3.2/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:28:40.672083 ml_pckg-1.3.2/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      266 2023-04-26 17:13:37.000000 ml_pckg-1.3.2/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:40.669646 ml_pckg-1.3.2/ml_pckg/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      172 2023-04-26 17:09:14.000000 ml_pckg-1.3.2/ml_pckg/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 ml_pckg-1.3.2/ml_pckg/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 ml_pckg-1.3.2/ml_pckg/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 ml_pckg-1.3.2/ml_pckg/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 ml_pckg-1.3.2/ml_pckg/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 ml_pckg-1.3.2/ml_pckg/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:40.671062 ml_pckg-1.3.2/ml_pckg.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:28:40.000000 ml_pckg-1.3.2/ml_pckg.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-26 17:28:40.000000 ml_pckg-1.3.2/ml_pckg.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 17:28:40.000000 ml_pckg-1.3.2/ml_pckg.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 17:28:40.000000 ml_pckg-1.3.2/ml_pckg.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-26 17:28:40.000000 ml_pckg-1.3.2/ml_pckg.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 17:28:40.672793 ml_pckg-1.3.2/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      855 2023-04-26 17:28:28.000000 ml_pckg-1.3.2/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:53.163535 ml_pckg-1.3.3/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 ml_pckg-1.3.3/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:28:53.163619 ml_pckg-1.3.3/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      266 2023-04-26 17:13:37.000000 ml_pckg-1.3.3/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:53.162315 ml_pckg-1.3.3/ml_pckg/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      172 2023-04-26 17:09:14.000000 ml_pckg-1.3.3/ml_pckg/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 ml_pckg-1.3.3/ml_pckg/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 ml_pckg-1.3.3/ml_pckg/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 ml_pckg-1.3.3/ml_pckg/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 ml_pckg-1.3.3/ml_pckg/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 ml_pckg-1.3.3/ml_pckg/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 17:28:53.163391 ml_pckg-1.3.3/ml_pckg.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      595 2023-04-26 17:28:53.000000 ml_pckg-1.3.3/ml_pckg.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      327 2023-04-26 17:28:53.000000 ml_pckg-1.3.3/ml_pckg.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 17:28:53.000000 ml_pckg-1.3.3/ml_pckg.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 17:28:53.000000 ml_pckg-1.3.3/ml_pckg.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        8 2023-04-26 17:28:53.000000 ml_pckg-1.3.3/ml_pckg.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 17:28:53.163926 ml_pckg-1.3.3/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      855 2023-04-26 17:28:40.000000 ml_pckg-1.3.3/setup.py
```

### Comparing `ml_pckg-1.3.2/LICENSE` & `ml_pckg-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/PKG-INFO` & `ml_pckg-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml_pckg
-Version: 1.3.2
+Version: 1.3.3
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.2.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.3.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.3.2/ml_pckg/classifiers.py` & `ml_pckg-1.3.3/ml_pckg/classifiers.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/ml_pckg/data_processing.py` & `ml_pckg-1.3.3/ml_pckg/data_processing.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/ml_pckg/linear_algebra.py` & `ml_pckg-1.3.3/ml_pckg/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/ml_pckg/metrics.py` & `ml_pckg-1.3.3/ml_pckg/metrics.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/ml_pckg/regressors.py` & `ml_pckg-1.3.3/ml_pckg/regressors.py`

 * *Files identical despite different names*

### Comparing `ml_pckg-1.3.2/ml_pckg.egg-info/PKG-INFO` & `ml_pckg-1.3.3/ml_pckg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ml-pckg
-Version: 1.3.2
+Version: 1.3.3
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.2.tar.gz
+Download-URL: https://github.com/Glebmaksimov/ml_pckg/archive/refs/tags/1.3.3.tar.gz
 Keywords: ML,FROM SWCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ml_pckg-1.3.2/setup.py` & `ml_pckg-1.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 import re
 
 
-current_version = '1.3.2'
+current_version = '1.3.3'
 
 setup(
     name='ml_pckg',
     packages=['ml_pckg'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
```

