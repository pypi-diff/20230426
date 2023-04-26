# Comparing `tmp/pyutils_basstal-0.4.0.tar.gz` & `tmp/pyutils_basstal-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutils_basstal-0.4.0.tar", last modified: Tue Apr 25 07:58:55 2023, max compression
+gzip compressed data, was "pyutils_basstal-0.4.1.tar", last modified: Wed Apr 26 03:59:01 2023, max compression
```

## Comparing `pyutils_basstal-0.4.0.tar` & `pyutils_basstal-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.824128 pyutils_basstal-0.4.0/
--rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1473 2023-04-25 07:58:55.823107 pyutils_basstal-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.800166 pyutils_basstal-0.4.0/pyutils/
--rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.0/pyutils/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.0/pyutils/autoupgrade.py
--rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.0/pyutils/executor.py
--rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.0/pyutils/fsext.py
--rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.0/pyutils/shorthand.py
--rw-rw-rw-   0        0        0     5071 2023-04-25 05:43:17.000000 pyutils_basstal-0.4.0/pyutils/simplelogger.py
--rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.0/pyutils/templite.py
-drwxrwxrwx   0        0        0        0 2023-04-25 07:58:55.822109 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/
--rw-rw-rw-   0        0        0     1473 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 07:58:55.000000 pyutils_basstal-0.4.0/pyutils_basstal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 07:58:55.824128 pyutils_basstal-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     8820 2023-04-25 06:09:37.000000 pyutils_basstal-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/
+-rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1473 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.812114 pyutils_basstal-0.4.1/pyutils/
+-rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.1/pyutils/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.1/pyutils/autoupgrade.py
+-rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.1/pyutils/executor.py
+-rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.1/pyutils/fsext.py
+-rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.1/pyutils/shorthand.py
+-rw-rw-rw-   0        0        0     5102 2023-04-25 08:50:55.000000 pyutils_basstal-0.4.1/pyutils/simplelogger.py
+-rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.1/pyutils/templite.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:59:01.834081 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 03:59:01.000000 pyutils_basstal-0.4.1/pyutils_basstal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 03:59:01.835052 pyutils_basstal-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     8820 2023-04-26 03:57:31.000000 pyutils_basstal-0.4.1/setup.py
```

### Comparing `pyutils_basstal-0.4.0/LICENSE.txt` & `pyutils_basstal-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/PKG-INFO` & `pyutils_basstal-0.4.1/pyutils_basstal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyutils_basstal
-Version: 0.4.0
+Name: pyutils-basstal
+Version: 0.4.1
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.0/README.md` & `pyutils_basstal-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils/autoupgrade.py` & `pyutils_basstal-0.4.1/pyutils/autoupgrade.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils/executor.py` & `pyutils_basstal-0.4.1/pyutils/executor.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils/fsext.py` & `pyutils_basstal-0.4.1/pyutils/fsext.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils/shorthand.py` & `pyutils_basstal-0.4.1/pyutils/shorthand.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils/simplelogger.py` & `pyutils_basstal-0.4.1/pyutils/simplelogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             return
         file_handler = SimpleLogger.__hanlder_cache[file_path]
         SimpleLogger._logger.removeHandler(file_handler)
         SimpleLogger._info_logger.removeHandler(file_handler)
         file_handler.close()
         del SimpleLogger.__hanlder_cache[file_path]
 
+logger = SimpleLogger._logger
 
 def info(message, bold=False):
     SimpleLogger.info(message, bold)
 
 
 def warning(message, bold=False):
     SimpleLogger.warning(message, bold)
```

### Comparing `pyutils_basstal-0.4.0/pyutils/templite.py` & `pyutils_basstal-0.4.1/pyutils/templite.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.0/pyutils_basstal.egg-info/PKG-INFO` & `pyutils_basstal-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyutils-basstal
-Version: 0.4.0
+Name: pyutils_basstal
+Version: 0.4.1
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.0/setup.py` & `pyutils_basstal-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="pyutils_basstal",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.0",  # Required
+    version="0.4.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="self used py utils",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

