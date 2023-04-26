# Comparing `tmp/mypy-boto3-datasync-1.26.71.tar.gz` & `tmp/mypy-boto3-datasync-1.26.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.26.71.tar", last modified: Tue Feb 14 20:27:05 2023, max compression
+gzip compressed data, was "mypy-boto3-datasync-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
```

## Comparing `mypy-boto3-datasync-1.26.71.tar` & `mypy-boto3-datasync-1.26.77.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.962803 mypy-boto3-datasync-1.26.71/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-14 20:27:05.962803 mypy-boto3-datasync-1.26.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.958803 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-02-14 20:26:15.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-02-14 20:26:15.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39691 2023-02-14 20:26:15.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-14 20:26:14.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.958803 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-14 20:27:05.000000 mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 20:27:05.962803 mypy-boto3-datasync-1.26.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-14 20:26:13.000000 mypy-boto3-datasync-1.26.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39738 2023-02-22 20:33:58.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39691 2023-02-22 20:33:57.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 20:34:22.000000 mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.502112 mypy-boto3-datasync-1.26.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-22 20:33:56.000000 mypy-boto3-datasync-1.26.77/setup.py
```

### Comparing `mypy-boto3-datasync-1.26.71/LICENSE` & `mypy-boto3-datasync-1.26.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/PKG-INFO` & `mypy-boto3-datasync-1.26.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.26.71
-Summary: Type annotations for boto3.DataSync 1.26.71 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.77
+Summary: Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.26.71/README.md` & `mypy-boto3-datasync-1.26.77/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__init__.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__init__.pyi` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/__main__.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.26.71\nVersion:         1.26.71\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.DataSync 1.26.77\nVersion:         1.26.77\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.71")
+    print("1.26.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/client.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/client.pyi` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/literals.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,14 +443,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/literals.pyi` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -441,14 +441,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/paginator.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/paginator.pyi` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/type_defs.py` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync/type_defs.pyi` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.26.71
-Summary: Type annotations for boto3.DataSync 1.26.71 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.77
+Summary: Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datasync?color=blue)](https://pypistats.org/packages/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.26.71/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy-boto3-datasync-1.26.77/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.26.71/setup.py` & `mypy-boto3-datasync-1.26.77/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.26.71",
+    version="1.26.77",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataSync 1.26.71 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.DataSync 1.26.77 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

