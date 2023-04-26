# Comparing `tmp/usefulib-1.0.3.tar.gz` & `tmp/usefulib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulib-1.0.3.tar", last modified: Wed Apr 26 16:23:25 2023, max compression
+gzip compressed data, was "usefulib-1.0.4.tar", last modified: Wed Apr 26 16:25:48 2023, max compression
```

## Comparing `usefulib-1.0.3.tar` & `usefulib-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.691342 usefulib-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3150 2023-04-26 16:23:25.690344 usefulib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-04-26 16:22:01.000000 usefulib-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 16:23:25.691342 usefulib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3391 2023-04-26 16:20:23.000000 usefulib-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.660328 usefulib-1.0.3/usefulib/
--rw-rw-rw-   0        0        0      210 2023-04-26 16:20:46.000000 usefulib-1.0.3/usefulib/__init__.py
--rw-rw-rw-   0        0        0     4246 2023-04-26 16:20:39.000000 usefulib-1.0.3/usefulib/_usefulibs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.689359 usefulib-1.0.3/usefulib/temp_data/
--rw-rw-rw-   0        0        0      238 2023-04-21 10:04:28.000000 usefulib-1.0.3/usefulib/temp_data/__init__.py
--rw-rw-rw-   0        0        0     3276 2023-04-26 16:20:34.000000 usefulib-1.0.3/usefulib/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.682761 usefulib-1.0.3/usefulib.egg-info/
--rw-rw-rw-   0        0        0     3150 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.742083 usefulib-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3149 2023-04-26 16:25:48.742083 usefulib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-04-26 16:25:24.000000 usefulib-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 16:25:48.742083 usefulib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3364 2023-04-26 16:24:56.000000 usefulib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.710841 usefulib-1.0.4/usefulib/
+-rw-rw-rw-   0        0        0      210 2023-04-26 16:25:16.000000 usefulib-1.0.4/usefulib/__init__.py
+-rw-rw-rw-   0        0        0     4246 2023-04-26 16:25:07.000000 usefulib-1.0.4/usefulib/_usefulibs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.742083 usefulib-1.0.4/usefulib/temp_data/
+-rw-rw-rw-   0        0        0      238 2023-04-26 16:25:05.000000 usefulib-1.0.4/usefulib/temp_data/__init__.py
+-rw-rw-rw-   0        0        0     3276 2023-04-26 16:25:00.000000 usefulib-1.0.4/usefulib/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:25:48.726462 usefulib-1.0.4/usefulib.egg-info/
+-rw-rw-rw-   0        0        0     3149 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 16:25:48.000000 usefulib-1.0.4/usefulib.egg-info/top_level.txt
```

### Comparing `usefulib-1.0.3/LICENSE` & `usefulib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulib-1.0.3/PKG-INFO` & `usefulib-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: usefulib
-Version: 1.0.3
-Summary: A collection of assorted methods to make small tasks easier..
+Version: 1.0.4
+Summary: A collection of assorted methods to make small tasks easier.
 Home-page: UNKNOWN
 Author: Hamd Waseem
 Author-email: <codingboy.cw@gmail.com>
 License: UNKNOWN
 Keywords: python,useful,usefulib,collection
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 <a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.2</h1>
+<h1>usefulib v1.0.4</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
```

### Comparing `usefulib-1.0.3/README.md` & `usefulib-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.3</h1>
+<h1>usefulib v1.0.4</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
 $ pip install usefulib
 ```
```

### Comparing `usefulib-1.0.3/setup.py` & `usefulib-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '1.0.3'
-DESCRIPTION = 'A collection of assorted methods to make small tasks easier..'
+VERSION = '1.0.4'
+DESCRIPTION = 'A collection of assorted methods to make small tasks easier.'
 LONG_DESCRIPTION = """
 <div align="center">
   <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
 </div>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
 <a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.2</h1>
+<h1>usefulib v1.0.4</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
```

### Comparing `usefulib-1.0.3/usefulib/_usefulibs.py` & `usefulib-1.0.4/usefulib/_usefulibs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-usefulib v1.0.3
+usefulib v1.0.4
 Copyright Hamd Waseem (https://github.com/hamdivazim) under the GNU Public License 3.0.
 
 https://github.com/hamdivazim/usefulib
 
 Add your useful method here if you are contributing. Remember to add unit tests in tests.py :)
 """
```

### Comparing `usefulib-1.0.3/usefulib/tests.py` & `usefulib-1.0.4/usefulib/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-usefulib v1.0.3
+usefulib v1.0.4
 Copyright Hamd Waseem (https://github.com/hamdivazim) under the GNU Public License 3.0.
 
 https://github.com/hamdivazim/usefulib
 
 
 This is where you should write unit tests for your useful method. If you can't do so for any reason, mention so in your PR so I can help.
 """
```

### Comparing `usefulib-1.0.3/usefulib.egg-info/PKG-INFO` & `usefulib-1.0.4/usefulib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: usefulib
-Version: 1.0.3
-Summary: A collection of assorted methods to make small tasks easier..
+Version: 1.0.4
+Summary: A collection of assorted methods to make small tasks easier.
 Home-page: UNKNOWN
 Author: Hamd Waseem
 Author-email: <codingboy.cw@gmail.com>
 License: UNKNOWN
 Keywords: python,useful,usefulib,collection
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 <a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
 <a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
 <a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
 
 
 
-<h1>usefulib v1.0.2</h1>
+<h1>usefulib v1.0.4</h1>
 A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
```

