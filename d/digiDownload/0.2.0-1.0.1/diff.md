# Comparing `tmp/digiDownload-0.2.0.tar.gz` & `tmp/digiDownload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiDownload-0.2.0.tar", last modified: Wed Apr 26 16:18:43 2023, max compression
+gzip compressed data, was "digiDownload-1.0.1.tar", last modified: Wed Apr 26 17:01:52 2023, max compression
```

## Comparing `digiDownload-0.2.0.tar` & `digiDownload-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1069 2023-04-20 11:45:13.000000 digiDownload-0.2.0/LICENSE
--rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 16:18:43.188696 digiDownload-0.2.0/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1142 2023-04-26 14:37:11.000000 digiDownload-0.2.0/README.md
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/digiDownload/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      194 2023-04-20 13:03:54.000000 digiDownload-0.2.0/digiDownload/AdBlockCookiePolicy.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     5553 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/Book.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      789 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/LTIParser.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     2084 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/Session.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)      214 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/__init__.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)     1695 2023-04-26 14:43:11.000000 digiDownload-0.2.0/digiDownload/cli_tool.py
--rw-r--r--   0 notyou    (1000) notyou    (1000)       85 2023-04-26 14:38:53.000000 digiDownload-0.2.0/digiDownload/exceptions.py
-drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 16:18:43.188696 digiDownload-0.2.0/digiDownload.egg-info/
--rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/PKG-INFO
--rw-r--r--   0 notyou    (1000) notyou    (1000)      399 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/SOURCES.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/dependency_links.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       42 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/requires.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-26 16:18:43.000000 digiDownload-0.2.0/digiDownload.egg-info/top_level.txt
--rw-r--r--   0 notyou    (1000) notyou    (1000)      102 2023-04-26 16:18:43.188696 digiDownload-0.2.0/setup.cfg
--rw-r--r--   0 notyou    (1000) notyou    (1000)      537 2023-04-26 16:14:25.000000 digiDownload-0.2.0/setup.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:01:52.325992 digiDownload-1.0.1/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1069 2023-04-20 11:45:13.000000 digiDownload-1.0.1/LICENSE
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 17:01:52.325992 digiDownload-1.0.1/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1142 2023-04-26 14:37:11.000000 digiDownload-1.0.1/README.md
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:01:52.325992 digiDownload-1.0.1/digiDownload/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      194 2023-04-20 13:03:54.000000 digiDownload-1.0.1/digiDownload/AdBlockCookiePolicy.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     5550 2023-04-26 16:57:58.000000 digiDownload-1.0.1/digiDownload/Book.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      787 2023-04-26 16:58:18.000000 digiDownload-1.0.1/digiDownload/LTIParser.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     2081 2023-04-26 16:59:50.000000 digiDownload-1.0.1/digiDownload/Session.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      165 2023-04-26 16:59:21.000000 digiDownload-1.0.1/digiDownload/__init__.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)     1690 2023-04-26 16:59:42.000000 digiDownload-1.0.1/digiDownload/cli_tool.py
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       85 2023-04-26 14:38:53.000000 digiDownload-1.0.1/digiDownload/exceptions.py
+drwxr-xr-x   0 notyou    (1000) notyou    (1000)        0 2023-04-26 17:01:52.325992 digiDownload-1.0.1/digiDownload.egg-info/
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      327 2023-04-26 17:01:52.000000 digiDownload-1.0.1/digiDownload.egg-info/PKG-INFO
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      399 2023-04-26 17:01:52.000000 digiDownload-1.0.1/digiDownload.egg-info/SOURCES.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)        1 2023-04-26 17:01:52.000000 digiDownload-1.0.1/digiDownload.egg-info/dependency_links.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       49 2023-04-26 17:01:52.000000 digiDownload-1.0.1/digiDownload.egg-info/requires.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)       13 2023-04-26 17:01:52.000000 digiDownload-1.0.1/digiDownload.egg-info/top_level.txt
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      102 2023-04-26 17:01:52.325992 digiDownload-1.0.1/setup.cfg
+-rw-r--r--   0 notyou    (1000) notyou    (1000)      555 2023-04-26 17:01:12.000000 digiDownload-1.0.1/setup.py
```

### Comparing `digiDownload-0.2.0/LICENSE` & `digiDownload-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `digiDownload-0.2.0/README.md` & `digiDownload-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `digiDownload-0.2.0/digiDownload/Book.py` & `digiDownload-1.0.1/digiDownload/Book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from digiDownload import LTIForm
+from LTIParser import LTIForm
 
 from httpx import AsyncClient, Response
 from bs4 import BeautifulSoup
 from svglib.svglib import svg2rlg
 from reportlab.graphics import renderPDF
 from reportlab.pdfgen.canvas import Canvas
 from PyPDF2 import PdfMerger
```

### Comparing `digiDownload-0.2.0/digiDownload/LTIParser.py` & `digiDownload-1.0.1/digiDownload/LTIParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from digiDownload import NotAnLtiLaunchForm
+from exceptions import NotAnLtiLaunchForm
 
 from httpx import AsyncClient, Response
 from bs4 import BeautifulSoup
 
 
 class LTIForm:
     def __init__(self, content: str):
```

### Comparing `digiDownload-0.2.0/digiDownload/Session.py` & `digiDownload-1.0.1/digiDownload/Session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from digiDownload import AdBlockPolicy
-from digiDownload import InvalidCredentials
-from digiDownload import Book
+from AdBlockCookiePolicy import AdBlockPolicy
+from exceptions import InvalidCredentials
+from Book import Book
 
 import httpx
 from bs4 import BeautifulSoup
 
 import asyncio
 from http import cookiejar
```

### Comparing `digiDownload-0.2.0/digiDownload/cli_tool.py` & `digiDownload-1.0.1/digiDownload/cli_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from digiDownload import Session
+from Session import Session
 
 import os
 from getpass import getpass
 
 
 async def run():
     try: session = await Session.create(os.environ["email"], os.environ["password"])
```

### Comparing `digiDownload-0.2.0/setup.py` & `digiDownload-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     name="digiDownload",
     url="https://github.com/DaniD3v/digiDownload",
     author="DaniD3v",
 
     description="API to download books from digi4school.at.",
     keywords=["digi4school", "books", "api"],
 
-    version="0.2.0",
+    version="1.0.1",
     license='MIT',
 
     packages=["digiDownload"],
     install_requires=[
         "httpx",
         "lxml",
         "reportlab",
+        "PyPDF2",
         "svglib"
         "beautifulsoup4"
     ],
 
-    download_url='https://github.com/DaniD3v/digiDownload/archive/refs/tags/1.0.0.tar.gz',
+    download_url='https://github.com/DaniD3v/digiDownload/archive/refs/tags/1.0.1.tar.gz',
 )
```

