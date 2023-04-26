# Comparing `tmp/longsight-1.0.5.tar.gz` & `tmp/longsight-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longsight-1.0.5.tar", last modified: Tue Apr 25 14:24:48 2023, max compression
+gzip compressed data, was "longsight-1.0.6.tar", last modified: Tue Apr 25 14:37:26 2023, max compression
```

## Comparing `longsight-1.0.5.tar` & `longsight-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:24:48.545919 longsight-1.0.5/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.5/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:24:48.545919 longsight-1.0.5/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6051 2023-04-24 10:53:59.000000 longsight-1.0.5/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-25 14:15:04.000000 longsight-1.0.5/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-25 14:24:48.545919 longsight-1.0.5/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:24:48.545919 longsight-1.0.5/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:24:48.545919 longsight-1.0.5/src/longsight/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.5/src/longsight/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12272 2023-04-25 14:22:59.000000 longsight-1.0.5/src/longsight/instrumentation.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:24:48.545919 longsight-1.0.5/src/longsight.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:24:48.000000 longsight-1.0.5/src/longsight.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-25 14:24:48.000000 longsight-1.0.5/src/longsight.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-25 14:24:48.000000 longsight-1.0.5/src/longsight.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-25 14:24:48.000000 longsight-1.0.5/src/longsight.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-25 14:24:48.000000 longsight-1.0.5/src/longsight.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:24:48.545919 longsight-1.0.5/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     6998 2023-03-31 15:41:47.000000 longsight-1.0.5/tests/test_instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.6/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:37:26.475587 longsight-1.0.6/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6051 2023-04-24 10:53:59.000000 longsight-1.0.6/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-25 14:37:12.000000 longsight-1.0.6/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-25 14:37:26.475587 longsight-1.0.6/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/longsight/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.6/src/longsight/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12538 2023-04-25 14:36:24.000000 longsight-1.0.6/src/longsight/instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/src/longsight.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-25 14:37:26.000000 longsight-1.0.6/src/longsight.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-25 14:37:26.475587 longsight-1.0.6/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6998 2023-03-31 15:41:47.000000 longsight-1.0.6/tests/test_instrumentation.py
```

### Comparing `longsight-1.0.5/LICENSE.md` & `longsight-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.5/PKG-INFO` & `longsight-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.5
+Version: 1.0.6
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.5/README.md` & `longsight-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.5/pyproject.toml` & `longsight-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longsight"
-version = "1.0.5"
+version = "1.0.6"
 description = "This library implements a range of common logging functions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `longsight-1.0.5/setup.cfg` & `longsight-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = longsight
-version = 1.0.5
+version = 1.0.6
 description = This library implements a range of common logging functions.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `longsight-1.0.5/src/longsight/instrumentation.py` & `longsight-1.0.6/src/longsight/instrumentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,26 +182,32 @@
             func_sig = inspect.signature(func)
 
             if inspect.iscoroutinefunction(func):
 
                 async def decorated(*args, **kwargs):
                     if "instrumentation" in func_sig.parameters:
                         with wrapping_logic(*args, **kwargs) as wl:
-                            if "instrumentation" not in kwargs:
+                            if (
+                                "instrumentation" not in kwargs
+                                or kwargs["instrumentation"] is None
+                            ):
                                 kwargs["instrumentation"] = wl
                             return await func(*args, **kwargs)
                     else:
                         return await func(*args, **kwargs)
 
             else:
 
                 def decorated(*args, **kwargs):
                     if "instrumentation" in func_sig.parameters:
                         with wrapping_logic(*args, **kwargs) as wl:
-                            if "instrumentation" not in kwargs:
+                            if (
+                                "instrumentation" not in kwargs
+                                or kwargs["instrumentation"] is None
+                            ):
                                 kwargs["instrumentation"] = wl
                             return func(*args, **kwargs)
                     else:
                         return func(*args, **kwargs)
 
             return functools.wraps(func)(decorated)
```

### Comparing `longsight-1.0.5/src/longsight.egg-info/PKG-INFO` & `longsight-1.0.6/src/longsight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.5
+Version: 1.0.6
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.5/tests/test_instrumentation.py` & `longsight-1.0.6/tests/test_instrumentation.py`

 * *Files identical despite different names*

