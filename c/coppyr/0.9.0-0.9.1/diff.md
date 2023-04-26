# Comparing `tmp/coppyr-0.9.0.tar.gz` & `tmp/coppyr-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coppyr-0.9.0.tar", last modified: Tue Apr 25 15:27:01 2023, max compression
+gzip compressed data, was "coppyr-0.9.1.tar", last modified: Tue Apr 25 15:37:40 2023, max compression
```

## Comparing `coppyr-0.9.0.tar` & `coppyr-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:27:01.506750 coppyr-0.9.0/
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       83 2023-04-24 21:42:08.000000 coppyr-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:27:01.506750 coppyr-0.9.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:27:01.506750 coppyr-0.9.0/coppyr/
--rw-rw-r--   0 root         (0) root         (0)      476 2023-04-24 21:39:57.000000 coppyr-0.9.0/coppyr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:27:01.506750 coppyr-0.9.0/coppyr/collections/
--rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.0/coppyr/collections/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.0/coppyr/collections/cycle.py
--rw-rw-r--   0 root         (0) root         (0)      705 2023-04-24 20:00:23.000000 coppyr-0.9.0/coppyr/collections/dotdict.py
--rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.0/coppyr/concurrent.py
--rw-rw-r--   0 root         (0) root         (0)     1164 2023-04-25 02:55:52.000000 coppyr-0.9.0/coppyr/config.py
--rw-rw-r--   0 root         (0) root         (0)     4059 2023-04-24 19:54:46.000000 coppyr-0.9.0/coppyr/context.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.0/coppyr/daemon.py
--rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.0/coppyr/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:27:01.506750 coppyr-0.9.0/coppyr/extensions/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.0/coppyr/extensions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.0/coppyr/extensions/load.py
--rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.0/coppyr/lazyproperty.py
--rw-rw-r--   0 root         (0) root         (0)     4735 2023-04-24 19:57:57.000000 coppyr-0.9.0/coppyr/logger.py
--rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.0/coppyr/package.py
--rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.0/coppyr/parallel.py
--rw-rw-r--   0 root         (0) root         (0)     1163 2023-04-24 19:54:28.000000 coppyr-0.9.0/coppyr/singleton.py
--rw-rw-r--   0 root         (0) root         (0)     3482 2023-04-24 19:59:29.000000 coppyr-0.9.0/coppyr/subp.py
--rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.0/coppyr/testing.py
--rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.0/coppyr/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:27:01.506750 coppyr-0.9.0/coppyr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:27:01.000000 coppyr-0.9.0/coppyr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-25 15:27:01.000000 coppyr-0.9.0/coppyr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:27:01.000000 coppyr-0.9.0/coppyr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-25 15:27:01.000000 coppyr-0.9.0/coppyr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 15:27:01.000000 coppyr-0.9.0/coppyr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:27:01.506750 coppyr-0.9.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-24 19:48:14.000000 coppyr-0.9.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       83 2023-04-24 21:42:08.000000 coppyr-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:37:40.898836 coppyr-0.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4266 2023-04-24 21:55:15.000000 coppyr-0.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.894836 coppyr-0.9.1/coppyr/
+-rw-rw-r--   0 root         (0) root         (0)      476 2023-04-25 15:37:32.000000 coppyr-0.9.1/coppyr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr/collections/
+-rw-rw-r--   0 root         (0) root         (0)       78 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/collections/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1091 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/collections/cycle.py
+-rw-rw-r--   0 root         (0) root         (0)      705 2023-04-24 20:00:23.000000 coppyr-0.9.1/coppyr/collections/dotdict.py
+-rw-rw-r--   0 root         (0) root         (0)     1431 2023-04-24 19:55:39.000000 coppyr-0.9.1/coppyr/concurrent.py
+-rw-rw-r--   0 root         (0) root         (0)     1164 2023-04-25 02:55:52.000000 coppyr-0.9.1/coppyr/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4059 2023-04-24 19:54:46.000000 coppyr-0.9.1/coppyr/context.py
+-rw-rw-r--   0 root         (0) root         (0)     2316 2023-04-24 19:56:41.000000 coppyr-0.9.1/coppyr/daemon.py
+-rw-rw-r--   0 root         (0) root         (0)     1645 2023-04-24 19:57:04.000000 coppyr-0.9.1/coppyr/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr/extensions/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/extensions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-04-24 20:41:07.000000 coppyr-0.9.1/coppyr/extensions/load.py
+-rw-rw-r--   0 root         (0) root         (0)      351 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/lazyproperty.py
+-rw-rw-r--   0 root         (0) root         (0)     4735 2023-04-24 19:57:57.000000 coppyr-0.9.1/coppyr/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     2428 2023-04-25 15:19:57.000000 coppyr-0.9.1/coppyr/package.py
+-rw-rw-r--   0 root         (0) root         (0)    10912 2023-04-24 19:58:31.000000 coppyr-0.9.1/coppyr/parallel.py
+-rw-rw-r--   0 root         (0) root         (0)     1163 2023-04-24 19:54:28.000000 coppyr-0.9.1/coppyr/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)     3482 2023-04-24 19:59:29.000000 coppyr-0.9.1/coppyr/subp.py
+-rw-rw-r--   0 root         (0) root         (0)      389 2023-04-24 19:49:53.000000 coppyr-0.9.1/coppyr/testing.py
+-rw-rw-r--   0 root         (0) root         (0)     1028 2023-04-24 20:44:01.000000 coppyr-0.9.1/coppyr/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:37:40.898836 coppyr-0.9.1/coppyr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 15:37:40.000000 coppyr-0.9.1/coppyr.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-04-25 15:25:17.000000 coppyr-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:37:40.898836 coppyr-0.9.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1285 2023-04-25 15:26:56.000000 coppyr-0.9.1/setup.py
```

### Comparing `coppyr-0.9.0/LICENSE` & `coppyr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/PKG-INFO` & `coppyr-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.0/README.rst` & `coppyr-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/collections/cycle.py` & `coppyr-0.9.1/coppyr/collections/cycle.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/collections/dotdict.py` & `coppyr-0.9.1/coppyr/collections/dotdict.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/concurrent.py` & `coppyr-0.9.1/coppyr/concurrent.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/config.py` & `coppyr-0.9.1/coppyr/config.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/context.py` & `coppyr-0.9.1/coppyr/context.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/daemon.py` & `coppyr-0.9.1/coppyr/daemon.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/error.py` & `coppyr-0.9.1/coppyr/error.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/extensions/load.py` & `coppyr-0.9.1/coppyr/extensions/load.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/logger.py` & `coppyr-0.9.1/coppyr/logger.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/package.py` & `coppyr-0.9.1/coppyr/package.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/parallel.py` & `coppyr-0.9.1/coppyr/parallel.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/singleton.py` & `coppyr-0.9.1/coppyr/singleton.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/subp.py` & `coppyr-0.9.1/coppyr/subp.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr/web.py` & `coppyr-0.9.1/coppyr/web.py`

 * *Files identical despite different names*

### Comparing `coppyr-0.9.0/coppyr.egg-info/PKG-INFO` & `coppyr-0.9.1/coppyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coppyr
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of boilerplate for Python applications.
 Home-page: https://github.com/gshulegaard/coppyr
 Author: Grant Hulegaard
 Author-email: loki.labrys@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `coppyr-0.9.0/coppyr.egg-info/SOURCES.txt` & `coppyr-0.9.1/coppyr.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 coppyr/__init__.py
 coppyr/concurrent.py
 coppyr/config.py
 coppyr/context.py
 coppyr/daemon.py
 coppyr/error.py
```

### Comparing `coppyr-0.9.0/setup.py` & `coppyr-0.9.1/setup.py`

 * *Files identical despite different names*

