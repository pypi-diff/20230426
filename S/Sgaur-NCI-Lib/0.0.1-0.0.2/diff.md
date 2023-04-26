# Comparing `tmp/Sgaur_NCI_Lib-0.0.1.tar.gz` & `tmp/Sgaur_NCI_Lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sgaur_NCI_Lib-0.0.1.tar", last modified: Sun Apr 23 18:40:29 2023, max compression
+gzip compressed data, was "Sgaur_NCI_Lib-0.0.2.tar", last modified: Sun Apr 23 18:49:15 2023, max compression
```

## Comparing `Sgaur_NCI_Lib-0.0.1.tar` & `Sgaur_NCI_Lib-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:40:29.244579 Sgaur_NCI_Lib-0.0.1/
--rw-rw-rw-   0        0        0      447 2023-04-23 18:40:29.243056 Sgaur_NCI_Lib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 18:40:29.215998 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/
-drwxrwxrwx   0        0        0        0 2023-04-23 18:40:29.240590 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 18:40:29.231519 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/
--rw-rw-rw-   0        0        0      447 2023-04-23 18:40:29.000000 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-04-23 18:40:29.000000 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:40:29.000000 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 18:40:29.000000 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      205 2023-04-23 18:36:35.000000 Sgaur_NCI_Lib-0.0.1/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.py
--rw-rw-rw-   0        0        0       42 2023-04-23 18:40:29.244579 Sgaur_NCI_Lib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1247 2023-04-23 18:09:05.000000 Sgaur_NCI_Lib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:49:15.595546 Sgaur_NCI_Lib-0.0.2/
+-rw-rw-rw-   0        0        0      447 2023-04-23 18:49:15.594781 Sgaur_NCI_Lib-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-23 18:49:15.581397 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/
+drwxrwxrwx   0        0        0        0 2023-04-23 18:49:15.591484 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 18:49:15.591484 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/
+-rw-rw-rw-   0        0        0      447 2023-04-23 18:49:15.000000 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-23 18:49:15.000000 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:49:15.000000 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-23 18:49:15.000000 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      205 2023-04-23 18:36:35.000000 Sgaur_NCI_Lib-0.0.2/Sgaur_NCI_Lib/src/Sgaur_NCI_Lib.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:49:15.595546 Sgaur_NCI_Lib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1247 2023-04-23 18:45:21.000000 Sgaur_NCI_Lib-0.0.2/setup.py
```

### Comparing `Sgaur_NCI_Lib-0.0.1/setup.py` & `Sgaur_NCI_Lib-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Sgaur_NCI_Lib",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The initial release version
     author="Shubham Gaur NCI",                     # Full name of the author
     description="Sample Library for Laboratory Application",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

