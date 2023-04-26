# Comparing `tmp/larry_utils-0.3.1.tar.gz` & `tmp/larry_utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "larry_utils-0.3.1.tar", last modified: Tue Apr 25 10:35:02 2023, max compression
+gzip compressed data, was "larry_utils-0.3.2.tar", last modified: Wed Apr 26 08:47:43 2023, max compression
```

## Comparing `larry_utils-0.3.1.tar` & `larry_utils-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.649432 larry_utils-0.3.1/
--rw-r--r--   0 root         (0) staff       (20)      162 2023-04-25 10:35:02.649193 larry_utils-0.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.648161 larry_utils-0.3.1/larry_utils/
--rw-r--r--   0 root         (0) staff       (20)     3263 2023-04-25 10:34:48.000000 larry_utils-0.3.1/larry_utils/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      530 2023-02-21 04:24:25.000000 larry_utils-0.3.1/larry_utils/create.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.648911 larry_utils-0.3.1/larry_utils.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      162 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      228 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       12 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-25 10:35:02.649510 larry_utils-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      369 2023-04-25 10:34:58.000000 larry_utils-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-26 08:47:43.231937 larry_utils-0.3.2/
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-04-26 08:47:43.231771 larry_utils-0.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-26 08:47:43.230921 larry_utils-0.3.2/larry_utils/
+-rw-r--r--   0 root         (0) staff       (20)     3272 2023-04-25 10:36:06.000000 larry_utils-0.3.2/larry_utils/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      530 2023-02-21 04:24:25.000000 larry_utils-0.3.2/larry_utils/create.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-26 08:47:43.231612 larry_utils-0.3.2/larry_utils.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-04-26 08:47:43.000000 larry_utils-0.3.2/larry_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      228 2023-04-26 08:47:43.000000 larry_utils-0.3.2/larry_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-26 08:47:43.000000 larry_utils-0.3.2/larry_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-26 08:47:43.000000 larry_utils-0.3.2/larry_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       12 2023-04-26 08:47:43.000000 larry_utils-0.3.2/larry_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-26 08:47:43.231991 larry_utils-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      369 2023-04-26 08:47:39.000000 larry_utils-0.3.2/setup.py
```

### Comparing `larry_utils-0.3.1/larry_utils/__init__.py` & `larry_utils-0.3.2/larry_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,8 @@
                 Bmatch = match
                 Bdistance = abs(ratio - distance)
     return Bmatch
 
 
 def hash(x):
     import hashlib
-    return hashlib.md5(x).hexdigest()
+    return hashlib.md5(x.encode()).hexdigest()
```

### Comparing `larry_utils-0.3.1/larry_utils/create.py` & `larry_utils-0.3.2/larry_utils/create.py`

 * *Files identical despite different names*

