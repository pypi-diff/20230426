# Comparing `tmp/secure-logger-0.1.5.tar.gz` & `tmp/secure-logger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-logger-0.1.5.tar", last modified: Wed Apr 26 18:36:25 2023, max compression
+gzip compressed data, was "secure-logger-0.1.6.tar", last modified: Wed Apr 26 18:53:48 2023, max compression
```

## Comparing `secure-logger-0.1.5.tar` & `secure-logger-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.184350 secure-logger-0.1.5/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.5/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5786 2023-04-26 18:36:25.184400 secure-logger-0.1.5/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4238 2023-04-26 18:34:09.000000 secure-logger-0.1.5/README.md
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2090 2023-04-26 18:34:35.000000 secure-logger-0.1.5/pyproject.toml
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.183611 secure-logger-0.1.5/secure_logger/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.5/secure_logger/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.5/secure_logger/decorators.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2836 2023-04-26 16:27:03.000000 secure-logger-0.1.5/secure_logger/masked_dict.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.184249 secure-logger-0.1.5/secure_logger.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5786 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/top_level.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 18:36:25.184643 secure-logger-0.1.5/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4754 2023-04-26 16:34:33.000000 secure-logger-0.1.5/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:53:48.505555 secure-logger-0.1.6/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.6/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5927 2023-04-26 18:53:48.505633 secure-logger-0.1.6/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4379 2023-04-26 18:46:40.000000 secure-logger-0.1.6/README.md
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2090 2023-04-26 18:51:48.000000 secure-logger-0.1.6/pyproject.toml
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:53:48.504655 secure-logger-0.1.6/secure_logger/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.6/secure_logger/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.6/secure_logger/decorators.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2836 2023-04-26 16:27:03.000000 secure-logger-0.1.6/secure_logger/masked_dict.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:53:48.505392 secure-logger-0.1.6/secure_logger.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5927 2023-04-26 18:53:48.000000 secure-logger-0.1.6/secure_logger.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 18:53:48.000000 secure-logger-0.1.6/secure_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 18:53:48.000000 secure-logger-0.1.6/secure_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 18:53:48.000000 secure-logger-0.1.6/secure_logger.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 18:53:48.000000 secure-logger-0.1.6/secure_logger.egg-info/top_level.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 18:53:48.505943 secure-logger-0.1.6/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4754 2023-04-26 16:34:33.000000 secure-logger-0.1.6/setup.py
```

### Comparing `secure-logger-0.1.5/LICENSE.txt` & `secure-logger-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.5/PKG-INFO` & `secure-logger-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A decorator to generate secure, well-formatted log entries
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
@@ -32,14 +32,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
+[![Tests](https://github.com/lpm0073/secure-logger/actions/workflows/tests.yml/badge.svg)](https://github.com/lpm0073/secure-logger/actions)
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
```

### Comparing `secure-logger-0.1.5/README.md` & `secure-logger-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Secure Logger
 
+[![Tests](https://github.com/lpm0073/secure-logger/actions/workflows/tests.yml/badge.svg)](https://github.com/lpm0073/secure-logger/actions)
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
```

### Comparing `secure-logger-0.1.5/pyproject.toml` & `secure-logger-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "secure-logger"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
 description = "A decorator to generate secure, well-formatted log entries"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `secure-logger-0.1.5/secure_logger/decorators.py` & `secure-logger-0.1.6/secure_logger/decorators.py`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.5/secure_logger/masked_dict.py` & `secure-logger-0.1.6/secure_logger/masked_dict.py`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.5/secure_logger.egg-info/PKG-INFO` & `secure-logger-0.1.6/secure_logger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A decorator to generate secure, well-formatted log entries
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
@@ -32,14 +32,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
+[![Tests](https://github.com/lpm0073/secure-logger/actions/workflows/tests.yml/badge.svg)](https://github.com/lpm0073/secure-logger/actions)
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
```

### Comparing `secure-logger-0.1.5/setup.cfg` & `secure-logger-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.5/setup.py` & `secure-logger-0.1.6/setup.py`

 * *Files identical despite different names*

