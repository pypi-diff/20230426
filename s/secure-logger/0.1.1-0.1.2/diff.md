# Comparing `tmp/secure-logger-0.1.1.tar.gz` & `tmp/secure-logger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-logger-0.1.1.tar", last modified: Tue Apr 25 19:19:27 2023, max compression
+gzip compressed data, was "secure-logger-0.1.2.tar", last modified: Tue Apr 25 21:25:13 2023, max compression
```

## Comparing `secure-logger-0.1.1.tar` & `secure-logger-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 19:19:27.341799 secure-logger-0.1.1/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.1/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4596 2023-04-25 19:19:27.341852 secure-logger-0.1.1/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3040 2023-04-25 19:16:25.000000 secure-logger-0.1.1/README.md
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2508 2023-04-25 19:17:32.000000 secure-logger-0.1.1/pyproject.toml
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 19:19:27.340944 secure-logger-0.1.1/secure_logger/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.1/secure_logger/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2729 2023-04-25 19:15:20.000000 secure-logger-0.1.1/secure_logger/decorators.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2069 2023-04-25 19:06:14.000000 secure-logger-0.1.1/secure_logger/masked_dict.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 19:19:27.341681 secure-logger-0.1.1/secure_logger.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4596 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      362 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       73 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       85 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-25 19:19:27.000000 secure-logger-0.1.1/secure_logger.egg-info/top_level.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)      760 2023-04-25 19:19:27.342098 secure-logger-0.1.1/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5004 2023-04-25 18:54:18.000000 secure-logger-0.1.1/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 21:25:13.485987 secure-logger-0.1.2/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.2/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4276 2023-04-25 21:25:13.486038 secure-logger-0.1.2/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3013 2023-04-25 19:56:11.000000 secure-logger-0.1.2/README.md
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1835 2023-04-25 20:07:27.000000 secure-logger-0.1.2/pyproject.toml
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 21:25:13.485160 secure-logger-0.1.2/secure_logger/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.2/secure_logger/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2729 2023-04-25 19:15:20.000000 secure-logger-0.1.2/secure_logger/decorators.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2180 2023-04-25 19:38:45.000000 secure-logger-0.1.2/secure_logger/masked_dict.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-25 21:25:13.485884 secure-logger-0.1.2/secure_logger.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4276 2023-04-25 21:25:13.000000 secure-logger-0.1.2/secure_logger.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-25 21:25:13.000000 secure-logger-0.1.2/secure_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-25 21:25:13.000000 secure-logger-0.1.2/secure_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-25 21:25:13.000000 secure-logger-0.1.2/secure_logger.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-25 21:25:13.000000 secure-logger-0.1.2/secure_logger.egg-info/top_level.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-25 21:25:13.486293 secure-logger-0.1.2/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4651 2023-04-25 20:02:51.000000 secure-logger-0.1.2/setup.py
```

### Comparing `secure-logger-0.1.1/LICENSE.txt` & `secure-logger-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.1/PKG-INFO` & `secure-logger-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A function decorator for beautiful and complete logging
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
 Project-URL: Homepage, https://github.com/lpm0073/secure-logger
 Project-URL: Documentation, https://github.com/lpm0073/secure-logger
 Project-URL: Repository, https://github.com/lpm0073/secure-logger
 Project-URL: Changelog, https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/lpm0073/secure-logger/issues
-Keywords: Python,Django,Logger
+Keywords: Python,Logger
 Platform: any
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Education
-Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
-[![AGPL License](https://img.shields.io/github/license/overhangio/tutor.svg?style=flat-square)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries of class instantiations, class method calls and standard Python function calls. Redacts function parameter values and dict values based on a customizable list.
 
 Redacts the following values by default:
 
 ```python
```

### Comparing `secure-logger-0.1.1/README.md` & `secure-logger-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
-[![AGPL License](https://img.shields.io/github/license/overhangio/tutor.svg?style=flat-square)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries of class instantiations, class method calls and standard Python function calls. Redacts function parameter values and dict values based on a customizable list.
 
 Redacts the following values by default:
 
 ```python
```

### Comparing `secure-logger-0.1.1/secure_logger/decorators.py` & `secure-logger-0.1.2/secure_logger/decorators.py`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.1/secure_logger/masked_dict.py` & `secure-logger-0.1.2/secure_logger/masked_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Authorization",
     "secret",
     "aws_access_key_id",
     "aws_secret_access_key",
 ]
 
 
-class ApploggerJSONEncoder(json.JSONEncoder):
+class _JSONEncoder(json.JSONEncoder):
     """encode json object for serialization."""
 
     def default(self, obj):
         """Handle unit test, unicode, and anything else that might throw a wrench in things."""
         if isinstance(obj, bytes):
             return str(obj, encoding="utf-8")
         if isinstance(obj, MagicMock):
@@ -30,43 +30,47 @@
         try:
             return json.JSONEncoder.default(self, obj)
         except Exception:  # noqa: B902
             # obj probably is not json serializable.
             return ""
 
 
-def masked_dict(obj: dict, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS) -> dict:
+def masked_dict(obj, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS) -> dict:
     """
     Mask sensitive key / value in log entries.
 
     Masks the value of specified key.
     obj: a dict or a string representation of a dict, or None
     """
+    if type(obj) == str:
+        obj = json.loads(obj)
+
+    if type(obj) != dict:
+        raise TypeError("obj must be a dict or a json serializable string")
+
     to_mask = {}
     for key in obj:
         value = obj[key]
         if type(value) == dict:
             value = masked_dict(value, sensitive_keys)
         to_mask[key] = value
 
     def redact(key: str, obj: dict) -> dict:
         if key in obj:
             obj[key] = "*** -- REDACTED -- ***"
         return obj
 
-    obj = to_mask
-    obj = dict(obj)
     for key in sensitive_keys:
-        obj = redact(key, obj)
-    return obj
+        to_mask = redact(key, to_mask)
+    return to_mask
 
 
 def serialized_masked_dict(obj: dict, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS, indent: int = 4) -> str:
     """Return a JSON encoded string representation of a masked dict."""
     to_serialize = {}
     for key in obj:
         value = obj[key]
         if type(value) == dict:
             value = masked_dict(value, sensitive_keys)
         to_serialize[key] = value
 
-    return json.dumps(masked_dict(to_serialize, sensitive_keys=sensitive_keys), cls=ApploggerJSONEncoder, indent=indent)
+    return json.dumps(masked_dict(to_serialize, sensitive_keys=sensitive_keys), cls=_JSONEncoder, indent=indent)
```

### Comparing `secure-logger-0.1.1/secure_logger.egg-info/PKG-INFO` & `secure-logger-0.1.2/secure_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: A function decorator for beautiful and complete logging
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
 Project-URL: Homepage, https://github.com/lpm0073/secure-logger
 Project-URL: Documentation, https://github.com/lpm0073/secure-logger
 Project-URL: Repository, https://github.com/lpm0073/secure-logger
 Project-URL: Changelog, https://github.com/lpm0073/secure-logger/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/lpm0073/secure-logger/issues
-Keywords: Python,Django,Logger
+Keywords: Python,Logger
 Platform: any
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Education
-Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: local
 License-File: LICENSE.txt
 
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
-[![AGPL License](https://img.shields.io/github/license/overhangio/tutor.svg?style=flat-square)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
 A Python decorator to generate redacted and nicely formatted log entries of class instantiations, class method calls and standard Python function calls. Redacts function parameter values and dict values based on a customizable list.
 
 Redacts the following values by default:
 
 ```python
```

### Comparing `secure-logger-0.1.1/setup.cfg` & `secure-logger-0.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [flake8]
 ignore = E128,E731,W503,W504
 max-line-length = 512
 exclude = venv/
 
 [tool:pytest]
-DJANGO_SETTINGS_MODULE = tests.testapp.settings
 norecursedirs = venv* .tox .eggs build dist secure_logger.egg-info secure_logger/mongodb
 addopts = --doctest-modules --doctest-ignore-import-errors --nomigrations --cov=secure_logger --cov-report html --cov-report term
 
 [isort]
 combine_as_imports = true
 default_section = THIRDPARTY
 include_trailing_comma = true
-known_third_party = django
 known_first_party = secure_logger
 multi_line_output = 5
 line_length = 128
 
 [pycodestyle]
 count = False
 max-line-length = 512
```

### Comparing `secure-logger-0.1.1/setup.py` & `secure-logger-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
-Lawrence McDaniel https://lawrencemcdaniel.com.
-
-The style and organizational scheme for this setup.py is largely copied from
-this project:
-        django_extensions: https://github.com/django-extensions/django-extensions/blob/main/setup.py
-"""
+"""Lawrence McDaniel https://lawrencemcdaniel.com."""
 # pylint: disable=open-builtin
 import io
 import os
 import sys
 from setuptools import find_packages, setup, __version__ as setuptools_version
 from distutils.command.install import INSTALL_SCHEMES
 from distutils.command.install_data import install_data
@@ -96,23 +90,19 @@
     license_files=("LICENSE.txt",),
     platforms=["any"],
     packages=find_packages(),
     package_data={"": ["*.html"]},  # include any Mako templates found in this repo.
     include_package_data=True,
     cmdclass=cmdclasses,
     python_requires=">=3.6",
-    install_requires=["Django>=3.2"],
+    install_requires=[],
     extras_require={},
     classifiers=[  # https://pypi.org/classifiers/
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
-        "Framework :: Django",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
```

