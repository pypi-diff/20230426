# Comparing `tmp/vijaikfirstpackage-0.1.0.tar.gz` & `tmp/vijaikfirstpackage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vijaikfirstpackage-0.1.0.tar", last modified: Wed Apr 26 08:08:29 2023, max compression
+gzip compressed data, was "vijaikfirstpackage-0.1.1.tar", last modified: Wed Apr 26 09:10:46 2023, max compression
```

## Comparing `vijaikfirstpackage-0.1.0.tar` & `vijaikfirstpackage-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 08:08:29.150240 vijaikfirstpackage-0.1.0/
--rw-rw-rw-   0        0        0      564 2023-04-26 08:08:29.150240 vijaikfirstpackage-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 08:08:29.134229 vijaikfirstpackage-0.1.0/extras/
--rw-rw-rw-   0        0        0       63 2023-04-25 06:51:47.000000 vijaikfirstpackage-0.1.0/extras/__init__.py
--rw-rw-rw-   0        0        0      266 2023-04-25 06:46:21.000000 vijaikfirstpackage-0.1.0/extras/divide.py
--rw-rw-rw-   0        0        0      267 2023-04-25 06:45:07.000000 vijaikfirstpackage-0.1.0/extras/multiply.py
--rw-rw-rw-   0        0        0       42 2023-04-26 08:08:29.150240 vijaikfirstpackage-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-04-26 07:53:16.000000 vijaikfirstpackage-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:08:29.142464 vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/
--rw-rw-rw-   0        0        0      564 2023-04-26 08:08:28.000000 vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-26 08:08:28.000000 vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 08:08:28.000000 vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 08:08:28.000000 vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:10:46.265891 vijaikfirstpackage-0.1.1/
+-rw-rw-rw-   0        0        0      564 2023-04-26 09:10:46.264575 vijaikfirstpackage-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 09:10:46.256434 vijaikfirstpackage-0.1.1/extras/
+-rw-rw-rw-   0        0        0       63 2023-04-25 06:51:47.000000 vijaikfirstpackage-0.1.1/extras/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-04-25 06:46:21.000000 vijaikfirstpackage-0.1.1/extras/divide.py
+-rw-rw-rw-   0        0        0      267 2023-04-25 06:45:07.000000 vijaikfirstpackage-0.1.1/extras/multiply.py
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:10:46.265891 vijaikfirstpackage-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-04-26 09:09:49.000000 vijaikfirstpackage-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:10:46.263510 vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-04-26 09:10:45.000000 vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-26 09:10:46.000000 vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:10:45.000000 vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 09:10:46.000000 vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/top_level.txt
```

### Comparing `vijaikfirstpackage-0.1.0/PKG-INFO` & `vijaikfirstpackage-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vijaikfirstpackage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Setting up a python package
 Author: Vijai Kannan
 Author-email: vijaik.nd@gmail.com
 License: UNKNOWN
 Keywords: python,test package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vijaikfirstpackage-0.1.0/setup.py` & `vijaikfirstpackage-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0    ' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'My test Python package'
 LONG_DESCRIPTION = 'My test Python package with description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="vijaikfirstpackage",
```

### Comparing `vijaikfirstpackage-0.1.0/vijaikfirstpackage.egg-info/PKG-INFO` & `vijaikfirstpackage-0.1.1/vijaikfirstpackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vijaikfirstpackage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Setting up a python package
 Author: Vijai Kannan
 Author-email: vijaik.nd@gmail.com
 License: UNKNOWN
 Keywords: python,test package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

