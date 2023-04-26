# Comparing `tmp/wikiseriesmarklib-0.1.1.tar.gz` & `tmp/wikiseriesmarklib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiseriesmarklib-0.1.1.tar", last modified: Wed Apr 26 14:22:31 2023, max compression
+gzip compressed data, was "wikiseriesmarklib-0.1.2.tar", last modified: Wed Apr 26 14:33:14 2023, max compression
```

## Comparing `wikiseriesmarklib-0.1.1.tar` & `wikiseriesmarklib-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:22:31.305582 wikiseriesmarklib-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-26 14:22:31.305582 wikiseriesmarklib-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    77079 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2348 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:22:31.301582 wikiseriesmarklib-0.1.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6806 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9000 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/docs/usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-26 14:22:31.305582 wikiseriesmarklib-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2001 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:22:31.301582 wikiseriesmarklib-0.1.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2256 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/tests/test_wikiseriesmarklib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:22:31.305582 wikiseriesmarklib-0.1.1/wikiseriesmarklib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    77079 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2348 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2192 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/dev-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-04-26 14:22:30.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/wikiseriesmarklib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-04-26 14:21:00.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib/wikiseriesmarklibexceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:22:31.305582 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 14:22:31.000000 wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:14.405381 wikiseriesmarklib-0.1.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      408 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-26 14:33:14.405381 wikiseriesmarklib-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77079 2023-04-26 14:33:13.000000 wikiseriesmarklib-0.1.2/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2348 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:14.397381 wikiseriesmarklib-0.1.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6806 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9000 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/docs/usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-26 14:33:14.405381 wikiseriesmarklib-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2001 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:14.397381 wikiseriesmarklib-0.1.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2256 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/tests/test_wikiseriesmarklib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:14.405381 wikiseriesmarklib-0.1.2/wikiseriesmarklib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77079 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2348 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2192 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/wikiseriesmarklib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-04-26 14:31:47.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib/wikiseriesmarklibexceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:14.405381 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 14:33:14.000000 wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/top_level.txt
```

### Comparing `wikiseriesmarklib-0.1.1/CONTRIBUTING.rst` & `wikiseriesmarklib-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/LICENSE` & `wikiseriesmarklib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/PKG-INFO` & `wikiseriesmarklib-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiseriesmarklib
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library interfacing with wikipedia to retreive tv series information
 Home-page: https://github.com/mmdwmeewis/wikiseriesmarklib
 Author: UnknownUser
 Author-email: unknownuser@unknowndomain.com
 License: MIT
 Keywords: wikiseriesmarklib wiki series
 Classifier: Development Status :: 3 - Alpha
@@ -102,7 +102,13 @@
 * first release
 
 
 0.1.1 (26-04-2023)
 ------------------
 
 * Fix permissions
+
+
+0.1.2 (26-04-2023)
+------------------
+
+* Fixed pipeline
```

### Comparing `wikiseriesmarklib-0.1.1/Pipfile.lock` & `wikiseriesmarklib-0.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/README.rst` & `wikiseriesmarklib-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/USAGE.rst` & `wikiseriesmarklib-0.1.2/USAGE.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/dev-requirements.txt` & `wikiseriesmarklib-0.1.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/docs/Makefile` & `wikiseriesmarklib-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/docs/conf.py` & `wikiseriesmarklib-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/docs/index.rst` & `wikiseriesmarklib-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/setup.py` & `wikiseriesmarklib-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/tests/test_wikiseriesmarklib.py` & `wikiseriesmarklib-0.1.2/tests/test_wikiseriesmarklib.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/CONTRIBUTING.rst` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/LICENSE` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/Pipfile.lock` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/README.rst` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/README.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/USAGE.rst` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/__init__.py` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/__init__.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/_version.py` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/_version.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/dev-requirements.txt` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/wikiseriesmarklib.py` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/wikiseriesmarklib.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib/wikiseriesmarklibexceptions.py` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib/wikiseriesmarklibexceptions.py`

 * *Files identical despite different names*

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/PKG-INFO` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiseriesmarklib
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library interfacing with wikipedia to retreive tv series information
 Home-page: https://github.com/mmdwmeewis/wikiseriesmarklib
 Author: UnknownUser
 Author-email: unknownuser@unknowndomain.com
 License: MIT
 Keywords: wikiseriesmarklib wiki series
 Classifier: Development Status :: 3 - Alpha
@@ -102,7 +102,13 @@
 * first release
 
 
 0.1.1 (26-04-2023)
 ------------------
 
 * Fix permissions
+
+
+0.1.2 (26-04-2023)
+------------------
+
+* Fixed pipeline
```

### Comparing `wikiseriesmarklib-0.1.1/wikiseriesmarklib.egg-info/SOURCES.txt` & `wikiseriesmarklib-0.1.2/wikiseriesmarklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

