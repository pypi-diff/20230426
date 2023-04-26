# Comparing `tmp/JustTry-0.0.4.tar.gz` & `tmp/JustTry-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JustTry-0.0.4.tar", last modified: Tue Apr 25 18:46:18 2023, max compression
+gzip compressed data, was "JustTry-0.0.7.tar", last modified: Tue Apr 25 22:12:50 2023, max compression
```

## Comparing `JustTry-0.0.4.tar` & `JustTry-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:46:18.537340 JustTry-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-25 18:46:18.516546 JustTry-0.0.4/JustTry/
--rw-rw-rw-   0        0        0        0 2023-04-25 18:32:37.000000 JustTry-0.0.4/JustTry/__init__.py
--rw-rw-rw-   0        0        0       98 2023-04-25 18:37:38.000000 JustTry-0.0.4/JustTry/calculator.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:46:18.529782 JustTry-0.0.4/JustTry.egg-info/
--rw-rw-rw-   0        0        0      561 2023-04-25 18:46:18.000000 JustTry-0.0.4/JustTry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-25 18:46:18.000000 JustTry-0.0.4/JustTry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:46:18.000000 JustTry-0.0.4/JustTry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 18:46:18.000000 JustTry-0.0.4/JustTry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2023-04-25 18:46:18.537340 JustTry-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2023-04-24 15:23:38.000000 JustTry-0.0.4/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 18:46:18.537340 JustTry-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-25 18:45:33.000000 JustTry-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:12:50.446737 JustTry-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-04-25 22:12:50.424601 JustTry-0.0.7/JustTry/
+-rw-rw-rw-   0        0        0        0 2023-04-25 22:06:53.000000 JustTry-0.0.7/JustTry/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-04-25 18:37:38.000000 JustTry-0.0.7/JustTry/calculator.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:12:50.437968 JustTry-0.0.7/JustTry.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-04-25 22:12:50.000000 JustTry-0.0.7/JustTry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-25 22:12:50.000000 JustTry-0.0.7/JustTry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:12:50.000000 JustTry-0.0.7/JustTry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 22:12:50.000000 JustTry-0.0.7/JustTry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2023-04-25 22:12:50.437968 JustTry-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2023-04-24 15:23:38.000000 JustTry-0.0.7/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:12:50.446737 JustTry-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2023-04-25 22:08:06.000000 JustTry-0.0.7/setup.py
```

### Comparing `JustTry-0.0.4/JustTry.egg-info/PKG-INFO` & `JustTry-0.0.7/JustTry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustTry
-Version: 0.0.4
+Version: 0.0.7
 Summary: This is very basic
 Author: Vishali
 Author-email: vishali.nagathevan@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `JustTry-0.0.4/PKG-INFO` & `JustTry-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JustTry
-Version: 0.0.4
+Version: 0.0.7
 Summary: This is very basic
 Author: Vishali
 Author-email: vishali.nagathevan@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `JustTry-0.0.4/license.txt` & `JustTry-0.0.7/license.txt`

 * *Files identical despite different names*

### Comparing `JustTry-0.0.4/setup.py` & `JustTry-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
+from packaging.version import Version
 
-VERSION = '0.0.4' 
 DESCRIPTION = 'vishali first Python package'
 LONG_DESCRIPTION = 'vishali first Python package with a slightly longer description'
+VERSION = "0.0.7"
+
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="JustTry", 
         version=VERSION,
         author="Vishali",
```

