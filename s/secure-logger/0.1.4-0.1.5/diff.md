# Comparing `tmp/secure-logger-0.1.4.tar.gz` & `tmp/secure-logger-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-logger-0.1.4.tar", last modified: Wed Apr 26 15:58:24 2023, max compression
+gzip compressed data, was "secure-logger-0.1.5.tar", last modified: Wed Apr 26 18:36:25 2023, max compression
```

## Comparing `secure-logger-0.1.4.tar` & `secure-logger-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.212520 secure-logger-0.1.4/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.4/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5377 2023-04-26 15:58:24.212567 secure-logger-0.1.4/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4114 2023-04-26 15:57:49.000000 secure-logger-0.1.4/README.md
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1835 2023-04-26 15:57:36.000000 secure-logger-0.1.4/pyproject.toml
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.211825 secure-logger-0.1.4/secure_logger/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.4/secure_logger/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.4/secure_logger/decorators.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2829 2023-04-26 15:57:36.000000 secure-logger-0.1.4/secure_logger/masked_dict.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.212407 secure-logger-0.1.4/secure_logger.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5377 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/top_level.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 15:58:24.212813 secure-logger-0.1.4/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4661 2023-04-26 14:30:48.000000 secure-logger-0.1.4/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.184350 secure-logger-0.1.5/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.5/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5786 2023-04-26 18:36:25.184400 secure-logger-0.1.5/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4238 2023-04-26 18:34:09.000000 secure-logger-0.1.5/README.md
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2090 2023-04-26 18:34:35.000000 secure-logger-0.1.5/pyproject.toml
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.183611 secure-logger-0.1.5/secure_logger/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.5/secure_logger/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.5/secure_logger/decorators.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2836 2023-04-26 16:27:03.000000 secure-logger-0.1.5/secure_logger/masked_dict.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 18:36:25.184249 secure-logger-0.1.5/secure_logger.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5786 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 18:36:25.000000 secure-logger-0.1.5/secure_logger.egg-info/top_level.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 18:36:25.184643 secure-logger-0.1.5/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4754 2023-04-26 16:34:33.000000 secure-logger-0.1.5/setup.py
```

### Comparing `secure-logger-0.1.4/LICENSE.txt` & `secure-logger-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.4/PKG-INFO` & `secure-logger-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.4
-Summary: A function decorator for beautiful and complete logging
+Version: 0.1.5
+Summary: A decorator to generate secure, well-formatted log entries
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Homepage, https://github.com/lpm0073/secure-logger
-Project-URL: Documentation, https://github.com/lpm0073/secure-logger
+Project-URL: Homepage, https://pypi.org/project/secure-logger/
+Project-URL: Documentation, https://pypi.org/project/secure-logger/
 Project-URL: Repository, https://github.com/lpm0073/secure-logger
 Project-URL: Changelog, https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/lpm0073/secure-logger/issues
 Keywords: Python,Logger
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
 
-class TestClass(object):
+class Foo(object):
 
     @secure_logger()
-    def test_2(self, test_dict, test_list):
+    def bar(self, dict_data, list_data):
         pass
 
 # call your method, passing some sensitive data
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-test_list = ['foo', 'bar']
-o = TestClass()
-o.test_2(test_dict=test_dict, test_list=test_list)
+list_data = ['foo', 'bar']
+foo = Foo()
+foo.bar(dict_data=dict_data, list_data=list_data)
 ```
 
 Log output:
 
 ```log
-INFO:secure_logger: __main__.TestClass().test_2()  keyword args: {
-    "test_dict": {
+INFO:secure_logger: __main__.Foo().bar()  keyword args: {
+    "dict_data": {
         "not_a_sensitive_key": "you-can-see-me",
-        "aws-access-key-id": "*** -- REDACTED -- ***",
-        "aws-secret-access-key": "*** -- REDACTED -- ***"
+        "aws-access-key-id": "*** -- secure_logger() -- ***",
+        "aws-secret-access-key": "*** -- secure_logger() -- ***"
     },
-    "test_list": [
+    "list_data": [
         "foo",
         "bar"
     ]
 }
 ```
 
 ### As library functions
 
 ```python
 from secure_logger.masked_dict import masked_dict, masked_dict2str
 
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-print(masked_dict2str(test_dict))
+print(masked_dict2str(dict_data))
 ```
 
 Output:
 
 ```bash
 {
     "not_a_sensitive_key": "you-can-see-me",
-    "aws-access-key-id": "*** -- REDACTED -- ***",
-    "aws-secret-access-key": "*** -- REDACTED -- ***"
+    "aws-access-key-id": "*** -- secure_logger() -- ***",
+    "aws-secret-access-key": "*** -- secure_logger() -- ***"
 }
 ```
 
 ## Installation
 
 ```bash
 pip install secure-logger
@@ -120,15 +126,15 @@
     @secure_logger(sensitive_keys=["password", "token", "crown_jewels"], message="***", indent=4)
     def another_def(self):
 ```
 
 ## Configuration Defaults
 
 ```python
-DEFAULT_REDACTION_MESSAGE = "*** -- REDACTED -- ***"
+DEFAULT_REDACTION_MESSAGE = "*** -- secure_logger() -- ***"
 DEFAULT_INDENT = 4
 DEFAULT_SENSITIVE_KEYS = [
     "password",
     "token",
     "client_id",
     "client_secret",
     "Authorization",
```

### Comparing `secure-logger-0.1.4/README.md` & `secure-logger-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
 
-class TestClass(object):
+class Foo(object):
 
     @secure_logger()
-    def test_2(self, test_dict, test_list):
+    def bar(self, dict_data, list_data):
         pass
 
 # call your method, passing some sensitive data
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-test_list = ['foo', 'bar']
-o = TestClass()
-o.test_2(test_dict=test_dict, test_list=test_list)
+list_data = ['foo', 'bar']
+foo = Foo()
+foo.bar(dict_data=dict_data, list_data=list_data)
 ```
 
 Log output:
 
 ```log
-INFO:secure_logger: __main__.TestClass().test_2()  keyword args: {
-    "test_dict": {
+INFO:secure_logger: __main__.Foo().bar()  keyword args: {
+    "dict_data": {
         "not_a_sensitive_key": "you-can-see-me",
-        "aws-access-key-id": "*** -- REDACTED -- ***",
-        "aws-secret-access-key": "*** -- REDACTED -- ***"
+        "aws-access-key-id": "*** -- secure_logger() -- ***",
+        "aws-secret-access-key": "*** -- secure_logger() -- ***"
     },
-    "test_list": [
+    "list_data": [
         "foo",
         "bar"
     ]
 }
 ```
 
 ### As library functions
 
 ```python
 from secure_logger.masked_dict import masked_dict, masked_dict2str
 
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-print(masked_dict2str(test_dict))
+print(masked_dict2str(dict_data))
 ```
 
 Output:
 
 ```bash
 {
     "not_a_sensitive_key": "you-can-see-me",
-    "aws-access-key-id": "*** -- REDACTED -- ***",
-    "aws-secret-access-key": "*** -- REDACTED -- ***"
+    "aws-access-key-id": "*** -- secure_logger() -- ***",
+    "aws-secret-access-key": "*** -- secure_logger() -- ***"
 }
 ```
 
 ## Installation
 
 ```bash
 pip install secure-logger
@@ -90,15 +90,15 @@
     @secure_logger(sensitive_keys=["password", "token", "crown_jewels"], message="***", indent=4)
     def another_def(self):
 ```
 
 ## Configuration Defaults
 
 ```python
-DEFAULT_REDACTION_MESSAGE = "*** -- REDACTED -- ***"
+DEFAULT_REDACTION_MESSAGE = "*** -- secure_logger() -- ***"
 DEFAULT_INDENT = 4
 DEFAULT_SENSITIVE_KEYS = [
     "password",
     "token",
     "client_id",
     "client_secret",
     "Authorization",
```

### Comparing `secure-logger-0.1.4/pyproject.toml` & `secure-logger-0.1.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -20,40 +20,46 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "secure-logger"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
-description = "A function decorator for beautiful and complete logging"
+description = "A decorator to generate secure, well-formatted log entries"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.6"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Utilities",
 ]
 dependencies = [
   "validators",
 ]
 
 keywords = ["Python", "Logger"]
 
 [project.urls]
-Homepage = "https://github.com/lpm0073/secure-logger"
-Documentation = "https://github.com/lpm0073/secure-logger"
+Homepage = "https://pypi.org/project/secure-logger/"
+Documentation = "https://pypi.org/project/secure-logger/"
 Repository = "https://github.com/lpm0073/secure-logger"
 Changelog = "https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/lpm0073/secure-logger/issues"
 
 #------------------------------------------------------------------------------
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 #------------------------------------------------------------------------------
```

### Comparing `secure-logger-0.1.4/secure_logger/decorators.py` & `secure-logger-0.1.5/secure_logger/decorators.py`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.4/secure_logger/masked_dict.py` & `secure-logger-0.1.5/secure_logger/masked_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "access-key-id",
     "secret-access-key",
     "aws_access_key_id",
     "aws_secret_access_key",
     "aws-access-key-id",
     "aws-secret-access-key",
 ]
-DEFAULT_REDACTION_MESSAGE = "*** -- REDACTED -- ***"
+DEFAULT_REDACTION_MESSAGE = "*** -- secure_logger() -- ***"
 DEFAULT_INDENT = 4
 
 
 class _JSONEncoder(json.JSONEncoder):
     """encode json object for serialization."""
 
     def default(self, obj):
```

### Comparing `secure-logger-0.1.4/secure_logger.egg-info/PKG-INFO` & `secure-logger-0.1.5/secure_logger.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.4
-Summary: A function decorator for beautiful and complete logging
+Version: 0.1.5
+Summary: A decorator to generate secure, well-formatted log entries
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Homepage, https://github.com/lpm0073/secure-logger
-Project-URL: Documentation, https://github.com/lpm0073/secure-logger
+Project-URL: Homepage, https://pypi.org/project/secure-logger/
+Project-URL: Documentation, https://pypi.org/project/secure-logger/
 Project-URL: Repository, https://github.com/lpm0073/secure-logger
 Project-URL: Changelog, https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/lpm0073/secure-logger/issues
 Keywords: Python,Logger
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys. Prevents your sensitive application data like cloud provider key-pairs from leaking into your application logs.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
 
-class TestClass(object):
+class Foo(object):
 
     @secure_logger()
-    def test_2(self, test_dict, test_list):
+    def bar(self, dict_data, list_data):
         pass
 
 # call your method, passing some sensitive data
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-test_list = ['foo', 'bar']
-o = TestClass()
-o.test_2(test_dict=test_dict, test_list=test_list)
+list_data = ['foo', 'bar']
+foo = Foo()
+foo.bar(dict_data=dict_data, list_data=list_data)
 ```
 
 Log output:
 
 ```log
-INFO:secure_logger: __main__.TestClass().test_2()  keyword args: {
-    "test_dict": {
+INFO:secure_logger: __main__.Foo().bar()  keyword args: {
+    "dict_data": {
         "not_a_sensitive_key": "you-can-see-me",
-        "aws-access-key-id": "*** -- REDACTED -- ***",
-        "aws-secret-access-key": "*** -- REDACTED -- ***"
+        "aws-access-key-id": "*** -- secure_logger() -- ***",
+        "aws-secret-access-key": "*** -- secure_logger() -- ***"
     },
-    "test_list": [
+    "list_data": [
         "foo",
         "bar"
     ]
 }
 ```
 
 ### As library functions
 
 ```python
 from secure_logger.masked_dict import masked_dict, masked_dict2str
 
-test_dict = {
+dict_data = {
     'not_a_sensitive_key': 'you-can-see-me',
     'aws-access-key_id': conf.AWS_ACCESS_KEY_ID,
     'aws-secret-access-key': conf.AWS_SECRET_ACCESS_KEY
 }
-print(masked_dict2str(test_dict))
+print(masked_dict2str(dict_data))
 ```
 
 Output:
 
 ```bash
 {
     "not_a_sensitive_key": "you-can-see-me",
-    "aws-access-key-id": "*** -- REDACTED -- ***",
-    "aws-secret-access-key": "*** -- REDACTED -- ***"
+    "aws-access-key-id": "*** -- secure_logger() -- ***",
+    "aws-secret-access-key": "*** -- secure_logger() -- ***"
 }
 ```
 
 ## Installation
 
 ```bash
 pip install secure-logger
@@ -120,15 +126,15 @@
     @secure_logger(sensitive_keys=["password", "token", "crown_jewels"], message="***", indent=4)
     def another_def(self):
 ```
 
 ## Configuration Defaults
 
 ```python
-DEFAULT_REDACTION_MESSAGE = "*** -- REDACTED -- ***"
+DEFAULT_REDACTION_MESSAGE = "*** -- secure_logger() -- ***"
 DEFAULT_INDENT = 4
 DEFAULT_SENSITIVE_KEYS = [
     "password",
     "token",
     "client_id",
     "client_secret",
     "Authorization",
```

### Comparing `secure-logger-0.1.4/setup.cfg` & `secure-logger-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.4/setup.py` & `secure-logger-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,32 +93,33 @@
     package_data={"": ["*.html"]},  # include any Mako templates found in this repo.
     include_package_data=True,
     cmdclass=cmdclasses,
     python_requires=">=3.6",
     install_requires=[],
     extras_require={},
     classifiers=[  # https://pypi.org/classifiers/
-        "Development Status :: 4 - Beta",
+        "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Utilities",
     ],
     project_urls={
-        "Documentation": "https://github.com/lpm0073/secure-logger/",
+        "Documentation": "https://pypi.org/project/secure-logger/",
         "Changelog": "https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md",
         "Source": "https://github.com/lpm0073/secure-logger",
         "Tracker": "https://github.com/lpm0073/secure-logger/issues",
     },
 )
```

