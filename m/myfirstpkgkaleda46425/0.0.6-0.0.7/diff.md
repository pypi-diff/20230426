# Comparing `tmp/myfirstpkgkaleda46425-0.0.6.tar.gz` & `tmp/myfirstpkgkaleda46425-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfirstpkgkaleda46425-0.0.6.tar", last modified: Wed Apr 26 06:55:25 2023, max compression
+gzip compressed data, was "myfirstpkgkaleda46425-0.0.7.tar", last modified: Wed Apr 26 06:59:18 2023, max compression
```

## Comparing `myfirstpkgkaleda46425-0.0.6.tar` & `myfirstpkgkaleda46425-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:55:25.494166 myfirstpkgkaleda46425-0.0.6/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      576 2023-04-26 06:55:25.493974 myfirstpkgkaleda46425-0.0.6/PKG-INFO
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:55:25.490952 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425/
--rw-r--r--   0 kaledadenton   (501) staff       (20)       22 2023-04-26 06:52:59.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425/__init__.py
--rw-r--r--   0 kaledadenton   (501) staff       (20)      329 2023-04-26 06:54:54.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425/add.py
-drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:55:25.493758 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/
--rw-r--r--   0 kaledadenton   (501) staff       (20)      576 2023-04-26 06:55:25.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/PKG-INFO
--rw-r--r--   0 kaledadenton   (501) staff       (20)      251 2023-04-26 06:55:25.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/SOURCES.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 06:55:25.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/dependency_links.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       22 2023-04-26 06:55:25.000000 myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/top_level.txt
--rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 06:55:25.494239 myfirstpkgkaleda46425-0.0.6/setup.cfg
--rw-r--r--   0 kaledadenton   (501) staff       (20)      949 2023-04-26 06:55:23.000000 myfirstpkgkaleda46425-0.0.6/setup.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:59:18.180574 myfirstpkgkaleda46425-0.0.7/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      576 2023-04-26 06:59:18.180414 myfirstpkgkaleda46425-0.0.7/PKG-INFO
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:59:18.179493 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       22 2023-04-26 06:52:59.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425/__init__.py
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      350 2023-04-26 06:58:13.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425/add.py
+drwxr-xr-x   0 kaledadenton   (501) staff       (20)        0 2023-04-26 06:59:18.180230 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      576 2023-04-26 06:59:18.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/PKG-INFO
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      251 2023-04-26 06:59:18.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/SOURCES.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)        1 2023-04-26 06:59:18.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/dependency_links.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       22 2023-04-26 06:59:18.000000 myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/top_level.txt
+-rw-r--r--   0 kaledadenton   (501) staff       (20)       38 2023-04-26 06:59:18.180630 myfirstpkgkaleda46425-0.0.7/setup.cfg
+-rw-r--r--   0 kaledadenton   (501) staff       (20)      949 2023-04-26 06:59:12.000000 myfirstpkgkaleda46425-0.0.7/setup.py
```

### Comparing `myfirstpkgkaleda46425-0.0.6/PKG-INFO` & `myfirstpkgkaleda46425-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfirstpkgkaleda46425
-Version: 0.0.6
+Version: 0.0.7
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: KD
 Author-email: <youremail@email.com>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `myfirstpkgkaleda46425-0.0.6/myfirstpkgkaleda46425.egg-info/PKG-INFO` & `myfirstpkgkaleda46425-0.0.7/myfirstpkgkaleda46425.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfirstpkgkaleda46425
-Version: 0.0.6
+Version: 0.0.7
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: KD
 Author-email: <youremail@email.com>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `myfirstpkgkaleda46425-0.0.6/setup.py` & `myfirstpkgkaleda46425-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="myfirstpkgkaleda46425",
```

