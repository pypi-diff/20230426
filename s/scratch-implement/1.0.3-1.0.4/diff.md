# Comparing `tmp/scratch_implement-1.0.3.tar.gz` & `tmp/scratch_implement-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch_implement-1.0.3.tar", last modified: Wed Apr 26 18:47:44 2023, max compression
+gzip compressed data, was "scratch_implement-1.0.4.tar", last modified: Wed Apr 26 18:48:17 2023, max compression
```

## Comparing `scratch_implement-1.0.3.tar` & `scratch_implement-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:47:44.579516 scratch_implement-1.0.3/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 scratch_implement-1.0.3/LICENSE
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      671 2023-04-26 18:47:44.579630 scratch_implement-1.0.3/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      284 2023-04-26 18:30:20.000000 scratch_implement-1.0.3/README.md
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:47:44.577991 scratch_implement-1.0.3/scratch_implement/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      222 2023-04-26 18:29:01.000000 scratch_implement-1.0.3/scratch_implement/__init__.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 scratch_implement-1.0.3/scratch_implement/classifiers.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 scratch_implement-1.0.3/scratch_implement/data_processing.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 scratch_implement-1.0.3/scratch_implement/linear_algebra.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 scratch_implement-1.0.3/scratch_implement/metrics.py
--rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 scratch_implement-1.0.3/scratch_implement/regressors.py
-drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:47:44.579324 scratch_implement-1.0.3/scratch_implement.egg-info/
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      671 2023-04-26 18:47:44.000000 scratch_implement-1.0.3/scratch_implement.egg-info/PKG-INFO
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      437 2023-04-26 18:47:44.000000 scratch_implement-1.0.3/scratch_implement.egg-info/SOURCES.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 18:47:44.000000 scratch_implement-1.0.3/scratch_implement.egg-info/dependency_links.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 18:47:44.000000 scratch_implement-1.0.3/scratch_implement.egg-info/requires.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       18 2023-04-26 18:47:44.000000 scratch_implement-1.0.3/scratch_implement.egg-info/top_level.txt
--rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 18:47:44.579953 scratch_implement-1.0.3/setup.cfg
--rw-r--r--   0 glebmaksimov   (501) staff       (20)      941 2023-04-26 18:45:47.000000 scratch_implement-1.0.3/setup.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:48:17.514088 scratch_implement-1.0.4/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     1073 2023-04-21 13:24:22.000000 scratch_implement-1.0.4/LICENSE
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      671 2023-04-26 18:48:17.514212 scratch_implement-1.0.4/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      284 2023-04-26 18:30:20.000000 scratch_implement-1.0.4/README.md
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:48:17.512765 scratch_implement-1.0.4/scratch_implement/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      222 2023-04-26 18:29:01.000000 scratch_implement-1.0.4/scratch_implement/__init__.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17566 2023-04-26 17:07:06.000000 scratch_implement-1.0.4/scratch_implement/classifiers.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     4615 2023-04-26 17:08:39.000000 scratch_implement-1.0.4/scratch_implement/data_processing.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     2655 2023-04-26 16:54:21.000000 scratch_implement-1.0.4/scratch_implement/linear_algebra.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)     3155 2023-04-26 16:52:03.000000 scratch_implement-1.0.4/scratch_implement/metrics.py
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)    17048 2023-04-26 17:09:17.000000 scratch_implement-1.0.4/scratch_implement/regressors.py
+drwxr-xr-x   0 glebmaksimov   (501) staff       (20)        0 2023-04-26 18:48:17.513918 scratch_implement-1.0.4/scratch_implement.egg-info/
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      671 2023-04-26 18:48:17.000000 scratch_implement-1.0.4/scratch_implement.egg-info/PKG-INFO
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      437 2023-04-26 18:48:17.000000 scratch_implement-1.0.4/scratch_implement.egg-info/SOURCES.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)        1 2023-04-26 18:48:17.000000 scratch_implement-1.0.4/scratch_implement.egg-info/dependency_links.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       53 2023-04-26 18:48:17.000000 scratch_implement-1.0.4/scratch_implement.egg-info/requires.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       18 2023-04-26 18:48:17.000000 scratch_implement-1.0.4/scratch_implement.egg-info/top_level.txt
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)       79 2023-04-26 18:48:17.514529 scratch_implement-1.0.4/setup.cfg
+-rw-r--r--   0 glebmaksimov   (501) staff       (20)      941 2023-04-26 18:47:44.000000 scratch_implement-1.0.4/setup.py
```

### Comparing `scratch_implement-1.0.3/LICENSE` & `scratch_implement-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/PKG-INFO` & `scratch_implement-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scratch_implement
-Version: 1.0.3
+Version: 1.0.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://files.pythonhosted.org/packages/47/0b/dc732a9a9f51b14f1c98ab9011eb13bf76a4e3b3622881f3fd0cf5f2094b/scratch_implement-1.0.3.tar.gz
+Download-URL: https://files.pythonhosted.org/packages/47/0b/dc732a9a9f51b14f1c98ab9011eb13bf76a4e3b3622881f3fd0cf5f2094b/scratch_implement-1.0.4.tar.gz
 Keywords: ML,FROM SCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scratch_implement-1.0.3/scratch_implement/classifiers.py` & `scratch_implement-1.0.4/scratch_implement/classifiers.py`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/scratch_implement/data_processing.py` & `scratch_implement-1.0.4/scratch_implement/data_processing.py`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/scratch_implement/linear_algebra.py` & `scratch_implement-1.0.4/scratch_implement/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/scratch_implement/metrics.py` & `scratch_implement-1.0.4/scratch_implement/metrics.py`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/scratch_implement/regressors.py` & `scratch_implement-1.0.4/scratch_implement/regressors.py`

 * *Files identical despite different names*

### Comparing `scratch_implement-1.0.3/scratch_implement.egg-info/PKG-INFO` & `scratch_implement-1.0.4/scratch_implement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scratch-implement
-Version: 1.0.3
+Version: 1.0.4
 Summary: Machine Learning Models
 Home-page: UNKNOWN
 Author: Gleb Maksimov
 Author-email: glebmaksimov092@gmail.com
 License: MIT
-Download-URL: https://files.pythonhosted.org/packages/47/0b/dc732a9a9f51b14f1c98ab9011eb13bf76a4e3b3622881f3fd0cf5f2094b/scratch_implement-1.0.3.tar.gz
+Download-URL: https://files.pythonhosted.org/packages/47/0b/dc732a9a9f51b14f1c98ab9011eb13bf76a4e3b3622881f3fd0cf5f2094b/scratch_implement-1.0.4.tar.gz
 Keywords: ML,FROM SCRATCH,ADVANCED
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scratch_implement-1.0.3/setup.py` & `scratch_implement-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 import re
 
 
-current_version = '1.0.3'
+current_version = '1.0.4'
 
 setup(
     name='scratch_implement',
     packages=['scratch_implement'],
     version=current_version,
     license='MIT',
     description='Machine Learning Models',
```

