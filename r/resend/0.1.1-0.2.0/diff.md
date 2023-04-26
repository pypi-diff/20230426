# Comparing `tmp/resend-0.1.1.tar.gz` & `tmp/resend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resend-0.1.1.tar", last modified: Wed Apr 19 01:41:15 2023, max compression
+gzip compressed data, was "dist/resend-0.2.0.tar", last modified: Wed Apr 26 01:56:23 2023, max compression
```

## Comparing `resend-0.1.1.tar` & `resend-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2022-12-09 00:15:03.000000 resend-0.1.1/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2383 2023-04-19 01:41:15.000000 resend-0.1.1/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1263 2023-04-19 01:08:50.000000 resend-0.1.1/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/resend/
--rw-r--r--   0 derich     (501) staff       (20)       94 2023-04-19 00:43:26.000000 resend-0.1.1/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     2209 2023-04-19 00:43:26.000000 resend-0.1.1/resend/api.py
--rw-r--r--   0 derich     (501) staff       (20)     3385 2023-04-19 01:11:35.000000 resend-0.1.1/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)      163 2023-04-19 01:14:46.000000 resend-0.1.1/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2383 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      289 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-19 01:30:00.000000 resend-0.1.1/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       17 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2023-04-19 01:41:15.000000 resend-0.1.1/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1103 2023-04-19 01:26:20.000000 resend-0.1.1/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/
+-rw-r--r--   0 derich     (501) staff       (20)     2392 2023-04-26 01:56:23.000000 resend-0.2.0/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1263 2023-04-24 23:51:39.000000 resend-0.2.0/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/resend/
+-rw-r--r--   0 derich     (501) staff       (20)       94 2023-04-24 23:51:39.000000 resend-0.2.0/resend/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     2327 2023-04-26 01:56:07.000000 resend-0.2.0/resend/api.py
+-rw-r--r--   0 derich     (501) staff       (20)     3385 2023-04-24 23:51:39.000000 resend-0.2.0/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)      163 2023-04-26 01:56:07.000000 resend-0.2.0/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2392 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      278 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       17 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2023-04-26 01:56:23.000000 resend-0.2.0/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1112 2023-04-26 01:56:07.000000 resend-0.2.0/setup.py
```

### Comparing `resend-0.1.1/PKG-INFO` & `resend-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Resend Python SDK
-Home-page: https://github.com/drish/resend-py
+Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
```

### Comparing `resend-0.1.1/README.md` & `resend-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `resend-0.1.1/resend/api.py` & `resend-0.2.0/resend/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import Dict, List
 
 import requests
 
 from resend.exceptions import raise_for_code_and_type
 
 from .version import get_version
 
@@ -46,14 +46,15 @@
         sender: str,
         to: str,
         subject: str,
         text: str = None,
         bcc: str = None,
         cc: str = None,
         html: str = None,
+        attachments: List[Dict] = None,
     ):
         if not sender:
             raise ValueError("sender is required.")
         if not to:
             raise ValueError("to is required.")
         if not subject:
             raise ValueError("subject is required.")
@@ -67,14 +68,16 @@
         elif html:
             params["html"] = html
 
         if cc:
             params["cc"] = cc
         if bcc:
             params["bcc"] = bcc
+        if attachments:
+            params["attachments"] = attachments
 
         resp = self._make_request(url, params, headers)
 
         if resp.status_code != 200 or resp.json().get("error") is not None:
             error = resp.json().get("error")
             raise_for_code_and_type(
                 code=error.get("code"),
```

### Comparing `resend-0.1.1/resend/exceptions.py` & `resend-0.2.0/resend/exceptions.py`

 * *Files identical despite different names*

### Comparing `resend-0.1.1/resend.egg-info/PKG-INFO` & `resend-0.2.0/resend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Resend Python SDK
-Home-page: https://github.com/drish/resend-py
+Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
```

### Comparing `resend-0.1.1/setup.py` & `resend-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name="resend",
     version=get_version(),
     description="Resend Python SDK",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     author="Derich Pacheco",
     author_email="carlosderich@gmail.com",
-    url="https://github.com/drish/resend-py",
+    url="https://github.com/resendlabs/resend-python",
     packages=["resend"],
     include_package_data=True,
     install_requires=install_requires,
     zip_safe=False,
     python_requires=">=3.7",
     keywords=["email", "email platform"],
     classifiers=[
```

