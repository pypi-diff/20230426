# Comparing `tmp/secure-logger-0.1.3.tar.gz` & `tmp/secure-logger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-logger-0.1.3.tar", last modified: Wed Apr 26 14:32:45 2023, max compression
+gzip compressed data, was "secure-logger-0.1.4.tar", last modified: Wed Apr 26 15:58:24 2023, max compression
```

## Comparing `secure-logger-0.1.3.tar` & `secure-logger-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 14:32:45.969590 secure-logger-0.1.3/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.3/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5360 2023-04-26 14:32:45.969649 secure-logger-0.1.3/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4097 2023-04-26 14:32:04.000000 secure-logger-0.1.3/README.md
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1835 2023-04-26 14:30:48.000000 secure-logger-0.1.3/pyproject.toml
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 14:32:45.968840 secure-logger-0.1.3/secure_logger/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.3/secure_logger/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.3/secure_logger/decorators.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2816 2023-04-26 14:30:48.000000 secure-logger-0.1.3/secure_logger/masked_dict.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 14:32:45.969467 secure-logger-0.1.3/secure_logger.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     5360 2023-04-26 14:32:45.000000 secure-logger-0.1.3/secure_logger.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 14:32:45.000000 secure-logger-0.1.3/secure_logger.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 14:32:45.000000 secure-logger-0.1.3/secure_logger.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 14:32:45.000000 secure-logger-0.1.3/secure_logger.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 14:32:45.000000 secure-logger-0.1.3/secure_logger.egg-info/top_level.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 14:32:45.969911 secure-logger-0.1.3/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4661 2023-04-26 14:30:48.000000 secure-logger-0.1.3/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.212520 secure-logger-0.1.4/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 secure-logger-0.1.4/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5377 2023-04-26 15:58:24.212567 secure-logger-0.1.4/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4114 2023-04-26 15:57:49.000000 secure-logger-0.1.4/README.md
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1835 2023-04-26 15:57:36.000000 secure-logger-0.1.4/pyproject.toml
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.211825 secure-logger-0.1.4/secure_logger/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-04-25 18:38:46.000000 secure-logger-0.1.4/secure_logger/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2883 2023-04-26 14:30:48.000000 secure-logger-0.1.4/secure_logger/decorators.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2829 2023-04-26 15:57:36.000000 secure-logger-0.1.4/secure_logger/masked_dict.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-26 15:58:24.212407 secure-logger-0.1.4/secure_logger.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     5377 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      322 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       52 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-04-26 15:58:24.000000 secure-logger-0.1.4/secure_logger.egg-info/top_level.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      685 2023-04-26 15:58:24.212813 secure-logger-0.1.4/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4661 2023-04-26 14:30:48.000000 secure-logger-0.1.4/setup.py
```

### Comparing `secure-logger-0.1.3/LICENSE.txt` & `secure-logger-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.3/PKG-INFO` & `secure-logger-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.3
+Version: 0.1.4
 Summary: A function decorator for beautiful and complete logging
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
@@ -31,15 +31,15 @@
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
```

### Comparing `secure-logger-0.1.3/README.md` & `secure-logger-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
```

### Comparing `secure-logger-0.1.3/pyproject.toml` & `secure-logger-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "secure-logger"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
 description = "A function decorator for beautiful and complete logging"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `secure-logger-0.1.3/secure_logger/decorators.py` & `secure-logger-0.1.4/secure_logger/decorators.py`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.3/secure_logger/masked_dict.py` & `secure-logger-0.1.4/secure_logger/masked_dict.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,59 +38,52 @@
         try:
             return json.JSONEncoder.default(self, obj)
         except Exception:  # noqa: B902
             # obj probably is not json serializable.
             return ""
 
 
-def masked_dict(obj, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS, message: str = DEFAULT_REDACTION_MESSAGE) -> dict:
+def masked_dict(
+    source_dict, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS, message: str = DEFAULT_REDACTION_MESSAGE
+) -> dict:
     """
     Mask sensitive key / value in log entries.
 
     Masks the value of specified key.
     obj: a dict or a string representation of a dict, or None
     """
-    if type(obj) == str:
-        obj = json.loads(obj)
+    if type(source_dict) == str:
+        source_dict = json.loads(source_dict)
 
-    if type(obj) != dict:
-        raise TypeError("obj must be a dict or a json serializable string")
+    if type(source_dict) != dict:
+        raise TypeError("source_dict must be a dict or a json serializable string")
 
-    to_mask = {}
-    for key in obj:
-        value = obj[key]
+    recursed_dict = {}
+    for key in source_dict:
+        value = source_dict[key]
         if type(value) == dict:
-            value = masked_dict(obj=value, sensitive_keys=sensitive_keys, message=message)
-        to_mask[key] = value
+            value = masked_dict(source_dict=value, sensitive_keys=sensitive_keys, message=message)
+        recursed_dict[key] = value
 
-    def redact(key: str, obj: dict) -> dict:
-        if key in obj:
-            obj[key] = message
-        return obj
-
-    for key in sensitive_keys:
-        to_mask = redact(key=key, obj=to_mask)
-    return to_mask
+    for lower_case_sensitive_key in [x.lower() for x in sensitive_keys]:
+        if lower_case_sensitive_key in [x.lower() for x in recursed_dict.keys()]:
+            for original_key in recursed_dict:
+                if original_key.lower() == lower_case_sensitive_key:
+                    recursed_dict[original_key] = message
+    return recursed_dict
 
 
 def masked_dict2str(
     obj: dict,
     sensitive_keys: list = DEFAULT_SENSITIVE_KEYS,
     indent: int = DEFAULT_INDENT,
     message: str = DEFAULT_REDACTION_MESSAGE,
 ) -> str:
     """Return a JSON encoded string representation of a masked dict."""
-    to_serialize = {}
-    for key in obj:
-        value = obj[key]
-        if type(value) == dict:
-            value = masked_dict(value, sensitive_keys, message=message)
-        to_serialize[key] = value
-
-    return json.dumps(masked_dict(to_serialize, sensitive_keys, message=message), cls=_JSONEncoder, indent=indent)
+    return json.dumps(masked_dict(obj, sensitive_keys, message=message), cls=_JSONEncoder, indent=indent)
 
 
 def serialized_masked_dict(
     obj: dict, sensitive_keys: list = DEFAULT_SENSITIVE_KEYS, indent: int = DEFAULT_INDENT
 ) -> str:
     """Backwards compatibility to 0.1.2 and prior."""
     return masked_dict2str(obj, sensitive_keys=sensitive_keys, indent=indent)
```

### Comparing `secure-logger-0.1.3/secure_logger.egg-info/PKG-INFO` & `secure-logger-0.1.4/secure_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-logger
-Version: 0.1.3
+Version: 0.1.4
 Summary: A function decorator for beautiful and complete logging
 Home-page: https://github.com/lpm0073/secure-logger
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
@@ -31,15 +31,15 @@
 # Secure Logger
 
 [![Source code](https://img.shields.io/static/v1?logo=github&label=Git&style=flat-square&color=brightgreen&message=Source%20code)](https://github.com/lpm0073/secure-logger)
 [![PyPI releases](https://img.shields.io/pypi/v/secure-logger?logo=python&logoColor=white)](https://pypi.org/project/secure-logger)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![hack.d Lawrence McDaniel](https://img.shields.io/badge/hack.d-Lawrence%20McDaniel-orange.svg)](https://lawrencemcdaniel.com)
 
-A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of keys.
+A Python decorator to generate redacted and nicely formatted log entries. Works on all callables: class, class methods, Python module functions. Recursively redacts Python dictionary key values based on a customizable list of case-insensitive keys.
 
 ## Usage
 
 ### As a decorator
 
 ```python
 from secure_logger.decorators import secure_logger
```

### Comparing `secure-logger-0.1.3/setup.cfg` & `secure-logger-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-logger-0.1.3/setup.py` & `secure-logger-0.1.4/setup.py`

 * *Files identical despite different names*

