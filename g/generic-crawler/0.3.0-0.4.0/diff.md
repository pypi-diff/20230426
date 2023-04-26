# Comparing `tmp/generic_crawler-0.3.0.tar.gz` & `tmp/generic_crawler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic_crawler-0.3.0.tar", last modified: Tue Apr 25 17:09:08 2023, max compression
+gzip compressed data, was "generic_crawler-0.4.0.tar", last modified: Tue Apr 25 17:14:31 2023, max compression
```

## Comparing `generic_crawler-0.3.0.tar` & `generic_crawler-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:09:08.304612 generic_crawler-0.3.0/
--rw-r-----   0 msaid     (1043) msaid     (1044)      718 2023-04-25 17:09:08.304612 generic_crawler-0.3.0/PKG-INFO
--rw-r-----   0 msaid     (1043) msaid     (1044)       19 2023-04-24 09:31:59.000000 generic_crawler-0.3.0/README.md
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:09:08.304612 generic_crawler-0.3.0/generic-crawler/
--rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-04-25 17:00:02.000000 generic_crawler-0.3.0/generic-crawler/__init__.py
--rw-r-----   0 msaid     (1043) msaid     (1044)     6251 2023-04-25 16:39:57.000000 generic_crawler-0.3.0/generic-crawler/webscraper.py
-drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:09:08.304612 generic_crawler-0.3.0/generic_crawler.egg-info/
--rw-r-----   0 msaid     (1043) msaid     (1044)      718 2023-04-25 17:09:08.000000 generic_crawler-0.3.0/generic_crawler.egg-info/PKG-INFO
--rw-r-----   0 msaid     (1043) msaid     (1044)      270 2023-04-25 17:09:08.000000 generic_crawler-0.3.0/generic_crawler.egg-info/SOURCES.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-04-25 17:09:08.000000 generic_crawler-0.3.0/generic_crawler.egg-info/dependency_links.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       50 2023-04-25 17:09:08.000000 generic_crawler-0.3.0/generic_crawler.egg-info/requires.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       16 2023-04-25 17:09:08.000000 generic_crawler-0.3.0/generic_crawler.egg-info/top_level.txt
--rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-04-25 17:09:08.304612 generic_crawler-0.3.0/setup.cfg
--rw-r-----   0 msaid     (1043) msaid     (1044)     1099 2023-04-25 17:08:50.000000 generic_crawler-0.3.0/setup.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:14:31.644604 generic_crawler-0.4.0/
+-rw-r-----   0 msaid     (1043) msaid     (1044)      718 2023-04-25 17:14:31.644604 generic_crawler-0.4.0/PKG-INFO
+-rw-r-----   0 msaid     (1043) msaid     (1044)       19 2023-04-25 17:12:00.000000 generic_crawler-0.4.0/README.md
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:14:31.644604 generic_crawler-0.4.0/generic_crawler/
+-rw-rw-r--   0 msaid     (1043) msaid     (1044)       34 2023-04-25 17:00:02.000000 generic_crawler-0.4.0/generic_crawler/__init__.py
+-rw-r-----   0 msaid     (1043) msaid     (1044)     6251 2023-04-25 16:39:57.000000 generic_crawler-0.4.0/generic_crawler/webscraper.py
+drwxr-x---   0 msaid     (1043) msaid     (1044)        0 2023-04-25 17:14:31.644604 generic_crawler-0.4.0/generic_crawler.egg-info/
+-rw-r-----   0 msaid     (1043) msaid     (1044)      718 2023-04-25 17:14:31.000000 generic_crawler-0.4.0/generic_crawler.egg-info/PKG-INFO
+-rw-r-----   0 msaid     (1043) msaid     (1044)      270 2023-04-25 17:14:31.000000 generic_crawler-0.4.0/generic_crawler.egg-info/SOURCES.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)        1 2023-04-25 17:14:31.000000 generic_crawler-0.4.0/generic_crawler.egg-info/dependency_links.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       50 2023-04-25 17:14:31.000000 generic_crawler-0.4.0/generic_crawler.egg-info/requires.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       16 2023-04-25 17:14:31.000000 generic_crawler-0.4.0/generic_crawler.egg-info/top_level.txt
+-rw-r-----   0 msaid     (1043) msaid     (1044)       38 2023-04-25 17:14:31.644604 generic_crawler-0.4.0/setup.cfg
+-rw-r-----   0 msaid     (1043) msaid     (1044)     1099 2023-04-25 17:14:16.000000 generic_crawler-0.4.0/setup.py
```

### Comparing `generic_crawler-0.3.0/PKG-INFO` & `generic_crawler-0.4.0/generic_crawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: generic_crawler
-Version: 0.3.0
+Name: generic-crawler
+Version: 0.4.0
 Summary: A simple web scraper for downloading images, tables, and text from a webpage.
 Author: Said Mohamed Amine
 Author-email: amine8said@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,9 +12,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# generic-crawler
+# generic_crawler
```

### Comparing `generic_crawler-0.3.0/generic-crawler/webscraper.py` & `generic_crawler-0.4.0/generic_crawler/webscraper.py`

 * *Files identical despite different names*

### Comparing `generic_crawler-0.3.0/generic_crawler.egg-info/PKG-INFO` & `generic_crawler-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: generic-crawler
-Version: 0.3.0
+Name: generic_crawler
+Version: 0.4.0
 Summary: A simple web scraper for downloading images, tables, and text from a webpage.
 Author: Said Mohamed Amine
 Author-email: amine8said@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,9 +12,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# generic-crawler
+# generic_crawler
```

### Comparing `generic_crawler-0.3.0/setup.py` & `generic_crawler-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="generic_crawler",
-    version="0.3.0",
+    version="0.4.0",
     description="A simple web scraper for downloading images, tables, and text from a webpage.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Said Mohamed Amine",
     author_email="amine8said@gmail.com",
     packages=find_packages(),
     install_requires=[
```

