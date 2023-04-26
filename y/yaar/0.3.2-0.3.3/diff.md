# Comparing `tmp/yaar-0.3.2.tar.gz` & `tmp/yaar-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaar-0.3.2.tar", last modified: Tue Apr 25 21:46:57 2023, max compression
+gzip compressed data, was "yaar-0.3.3.tar", last modified: Tue Apr 25 21:52:57 2023, max compression
```

## Comparing `yaar-0.3.2.tar` & `yaar-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-25 21:46:57.590424 yaar-0.3.2/
--rw-rw-r--   0 juca      (1001) juca      (1001)     1128 2023-04-25 21:46:57.590424 yaar-0.3.2/PKG-INFO
--rw-rw-r--   0 juca      (1001) juca      (1001)      711 2023-04-25 20:46:14.000000 yaar-0.3.2/README.md
--rw-rw-r--   0 juca      (1001) juca      (1001)      719 2023-04-25 21:45:39.000000 yaar-0.3.2/pyproject.toml
--rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-04-25 21:46:57.590424 yaar-0.3.2/setup.cfg
-drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-25 21:46:57.590424 yaar-0.3.2/yaar.egg-info/
--rwxrwxrwx   0 juca      (1001) juca      (1001)     1128 2023-04-25 21:46:57.000000 yaar-0.3.2/yaar.egg-info/PKG-INFO
--rwxrwxrwx   0 juca      (1001) juca      (1001)      171 2023-04-25 21:46:57.000000 yaar-0.3.2/yaar.egg-info/SOURCES.txt
--rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-04-25 21:46:57.000000 yaar-0.3.2/yaar.egg-info/dependency_links.txt
--rwxrwxrwx   0 juca      (1001) juca      (1001)       15 2023-04-25 21:46:57.000000 yaar-0.3.2/yaar.egg-info/requires.txt
--rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-04-25 21:46:57.000000 yaar-0.3.2/yaar.egg-info/top_level.txt
--rw-rw-r--   0 juca      (1001) juca      (1001)     5894 2023-04-25 21:46:28.000000 yaar-0.3.2/yaar.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-25 21:52:57.669431 yaar-0.3.3/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1128 2023-04-25 21:52:57.669431 yaar-0.3.3/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      711 2023-04-25 20:46:14.000000 yaar-0.3.3/README.md
+-rw-rw-r--   0 juca      (1001) juca      (1001)      632 2023-04-25 21:52:08.000000 yaar-0.3.3/pyproject.toml
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-04-25 21:52:57.669431 yaar-0.3.3/setup.cfg
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-25 21:52:57.669431 yaar-0.3.3/yaar.egg-info/
+-rwxrwxrwx   0 juca      (1001) juca      (1001)     1128 2023-04-25 21:52:57.000000 yaar-0.3.3/yaar.egg-info/PKG-INFO
+-rwxrwxrwx   0 juca      (1001) juca      (1001)      171 2023-04-25 21:52:57.000000 yaar-0.3.3/yaar.egg-info/SOURCES.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-04-25 21:52:57.000000 yaar-0.3.3/yaar.egg-info/dependency_links.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)       15 2023-04-25 21:52:57.000000 yaar-0.3.3/yaar.egg-info/requires.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)        5 2023-04-25 21:52:57.000000 yaar-0.3.3/yaar.egg-info/top_level.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)     5894 2023-04-25 21:52:05.000000 yaar-0.3.3/yaar.py
```

### Comparing `yaar-0.3.2/PKG-INFO` & `yaar-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaar
-Version: 0.3.2
+Version: 0.3.3
 Summary: Yet Another Asyncio Requets
 Author: Juca Crispim
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Quality Assurance
```

### Comparing `yaar-0.3.2/README.md` & `yaar-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yaar-0.3.2/pyproject.toml` & `yaar-0.3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -25,12 +25,7 @@
     'Operating System :: Unix',
     'Topic :: Software Development :: Quality Assurance',
     'Programming Language :: Python :: 3'
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "yaar.__version__"}
-
-[tool.setuptools.packages.find]
-where = ["."]
-exclude = ["tests*"]
-include = ["yaar"]
```

### Comparing `yaar-0.3.2/yaar.egg-info/PKG-INFO` & `yaar-0.3.3/yaar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaar
-Version: 0.3.2
+Version: 0.3.3
 Summary: Yet Another Asyncio Requets
 Author: Juca Crispim
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Quality Assurance
```

### Comparing `yaar-0.3.2/yaar.py` & `yaar-0.3.3/yaar.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # along with yaar. If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import json
 import aiohttp
 
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 
 class HTTPRequestError(Exception):
     pass
 
 
 class Response:
```

