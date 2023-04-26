# Comparing `tmp/tableY-0.1.2.tar.gz` & `tmp/tableY-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tableY-0.1.2.tar", last modified: Wed Apr 26 05:22:28 2023, max compression
+gzip compressed data, was "dist\tableY-0.1.3.tar", last modified: Wed Apr 26 05:25:05 2023, max compression
```

## Comparing `tableY-0.1.2.tar` & `tableY-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 05:22:28.515188 tableY-0.1.2/
--rw-rw-rw-   0        0        0      745 2023-04-26 05:22:28.515188 tableY-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 05:22:28.515188 tableY-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-04-26 05:21:35.000000 tableY-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 05:22:28.501225 tableY-0.1.2/tableY/
--rw-rw-rw-   0        0        0     1612 2023-04-26 05:22:17.000000 tableY-0.1.2/tableY/combining.py
-drwxrwxrwx   0        0        0        0 2023-04-26 05:22:28.512197 tableY-0.1.2/tableY.egg-info/
--rw-rw-rw-   0        0        0      745 2023-04-26 05:22:28.000000 tableY-0.1.2/tableY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-26 05:22:28.000000 tableY-0.1.2/tableY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 05:22:28.000000 tableY-0.1.2/tableY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 05:22:28.000000 tableY-0.1.2/tableY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 05:22:28.000000 tableY-0.1.2/tableY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 05:25:05.937987 tableY-0.1.3/
+-rw-rw-rw-   0        0        0    18235 2023-04-26 05:25:05.936990 tableY-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-26 05:25:05.937987 tableY-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2023-04-26 05:24:50.000000 tableY-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:25:05.925022 tableY-0.1.3/tableY/
+-rw-rw-rw-   0        0        0     1612 2023-04-26 05:22:17.000000 tableY-0.1.3/tableY/combining.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:25:05.934996 tableY-0.1.3/tableY.egg-info/
+-rw-rw-rw-   0        0        0    18235 2023-04-26 05:25:05.000000 tableY-0.1.3/tableY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-04-26 05:25:05.000000 tableY-0.1.3/tableY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 05:25:05.000000 tableY-0.1.3/tableY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 05:25:05.000000 tableY-0.1.3/tableY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 05:25:05.000000 tableY-0.1.3/tableY.egg-info/top_level.txt
```

### Comparing `tableY-0.1.2/setup.py` & `tableY-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 
 from __future__ import print_function
 from setuptools import setup, find_packages
 import sys
 import io,os
 here = os.path.abspath(os.path.dirname(__file__))
-
-with open("readme.md", "r", encoding='utf-8') as fh:
-    long_description = fh.read()
-
+try:
+    with open("readme.md", "r", encoding='utf-8') as fh:
+        long_description = fh.read()
+except FileNotFoundError:
+    long_description = ''
 # def read_file(filename):
 #     with open(filename) as fp:
 #         return fp.read().strip()
 #
 # def read_requirements(filename):
 #     return [line.strip() for line in read_file(filename).splitlines()
 #             if not line.startswith('#')]
 
 # REQUIRED = read_requirements('requirements.txt')
 setup(
     name='tableY',
-    version='0.1.2',
+    version='0.1.3',
     author='White.tie',
     author_email='1042798703@qq.com',
     url='https://github.com/tyj-1995',
     description='Convert the columns of the table to json',
-    long_description='将table中的列转成json',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=['tableY'],
     install_requires=["pandas"],
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Topic :: Text Processing :: Indexing",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tableY-0.1.2/tableY/combining.py` & `tableY-0.1.3/tableY/combining.py`

 * *Files identical despite different names*

