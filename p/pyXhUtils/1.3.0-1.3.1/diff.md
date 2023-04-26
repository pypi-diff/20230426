# Comparing `tmp/pyXhUtils-1.3.0.tar.gz` & `tmp/pyXhUtils-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyXhUtils-1.3.0.tar", last modified: Wed Apr 26 12:47:34 2023, max compression
+gzip compressed data, was "pyXhUtils-1.3.1.tar", last modified: Wed Apr 26 13:41:48 2023, max compression
```

## Comparing `pyXhUtils-1.3.0.tar` & `pyXhUtils-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/pyXhUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-26 12:47:34.000000 pyXhUtils-1.3.0/src/pyXhUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-26 12:47:34.000000 pyXhUtils-1.3.0/src/pyXhUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:47:34.000000 pyXhUtils-1.3.0/src/pyXhUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 12:47:34.000000 pyXhUtils-1.3.0/src/pyXhUtils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/xh_file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_file_utils/FileUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_file_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/xh_functional/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_functional/FunctionalUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/xh_ini_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_ini_modifier/InitModifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_ini_modifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/xh_utils_apache_log/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_apache_log/ApacheLog.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_apache_log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.560674 pyXhUtils-1.3.0/src/xh_utils_file_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_file_changes/FileChanges.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_file_changes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/src/xh_utils_ip/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_ip/IpHostFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_ip/IpTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/src/xh_utils_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_progress/ProgressPinger.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_progress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/src/xh_utils_script_file_writer/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_script_file_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_script_file_writer/script_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:47:34.564674 pyXhUtils-1.3.0/src/xh_utils_string/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_string/StringUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 12:47:23.000000 pyXhUtils-1.3.0/src/xh_utils_string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.660501 pyXhUtils-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/pyXhUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-26 13:41:48.000000 pyXhUtils-1.3.1/src/pyXhUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-26 13:41:48.000000 pyXhUtils-1.3.1/src/pyXhUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:41:48.000000 pyXhUtils-1.3.1/src/pyXhUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:41:48.000000 pyXhUtils-1.3.1/src/pyXhUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_file_utils/FileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_file_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_functional/FunctionalUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_ini_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_ini_modifier/InitModifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_ini_modifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_apache_log/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_apache_log/ApacheLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_apache_log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_file_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_file_changes/FileChanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_file_changes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_ip/IpHostFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_ip/IpTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_progress/ProgressPinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_script_file_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_script_file_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_script_file_writer/script_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:41:48.664501 pyXhUtils-1.3.1/src/xh_utils_string/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_string/StringUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 13:41:35.000000 pyXhUtils-1.3.1/src/xh_utils_string/__init__.py
```

### Comparing `pyXhUtils-1.3.0/LICENSE.txt` & `pyXhUtils-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/PKG-INFO` & `pyXhUtils-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.0
+Version: 1.3.1
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,15 @@
 
 ## Functional
 ```python
 from xh_functional import Scope
 
 Scope(1)\
     .apply(lambda x: x + 1)\
+    .verify(lambda x: x == 2, msg=lambda x: f"Exception: {x}")\
     .map(lambda x: f"Some number: {x}")\
     .get()
 
 # output
 # Some number: 2
 ```
 
@@ -141,15 +142,15 @@
         "\n")
     for ip in [ipu.Ip.from_regular_form(ipStr)]
 ]
 ```
 
 Find host by ip if applicable
 ```python
-form xh_utils_ip import defaultIpHostFinder as ipHostFinder
+from xh_utils_ip import defaultIpHostFinder as ipHostFinder
 ipHostFinder.find("127.0.0.1")
 ```
 
 ## xh_utils_string
 
 ```python
 import xh_utils_string as su
```

### Comparing `pyXhUtils-1.3.0/README.md` & `pyXhUtils-1.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Functional
 ```python
 from xh_functional import Scope
 
 Scope(1)\
     .apply(lambda x: x + 1)\
+    .verify(lambda x: x == 2, msg=lambda x: f"Exception: {x}")\
     .map(lambda x: f"Some number: {x}")\
     .get()
 
 # output
 # Some number: 2
 ```
 
@@ -127,15 +128,15 @@
         "\n")
     for ip in [ipu.Ip.from_regular_form(ipStr)]
 ]
 ```
 
 Find host by ip if applicable
 ```python
-form xh_utils_ip import defaultIpHostFinder as ipHostFinder
+from xh_utils_ip import defaultIpHostFinder as ipHostFinder
 ipHostFinder.find("127.0.0.1")
 ```
 
 ## xh_utils_string
 
 ```python
 import xh_utils_string as su
```

### Comparing `pyXhUtils-1.3.0/pyproject.toml` & `pyXhUtils-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyXhUtils"
-version = "1.3.0"
+version = "1.3.1"
 description = "A collection of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = []
 [[project.authors]]
 name = "xethhung"
```

### Comparing `pyXhUtils-1.3.0/src/pyXhUtils.egg-info/PKG-INFO` & `pyXhUtils-1.3.1/src/pyXhUtils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.3.0
+Version: 1.3.1
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,15 @@
 
 ## Functional
 ```python
 from xh_functional import Scope
 
 Scope(1)\
     .apply(lambda x: x + 1)\
+    .verify(lambda x: x == 2, msg=lambda x: f"Exception: {x}")\
     .map(lambda x: f"Some number: {x}")\
     .get()
 
 # output
 # Some number: 2
 ```
 
@@ -141,15 +142,15 @@
         "\n")
     for ip in [ipu.Ip.from_regular_form(ipStr)]
 ]
 ```
 
 Find host by ip if applicable
 ```python
-form xh_utils_ip import defaultIpHostFinder as ipHostFinder
+from xh_utils_ip import defaultIpHostFinder as ipHostFinder
 ipHostFinder.find("127.0.0.1")
 ```
 
 ## xh_utils_string
 
 ```python
 import xh_utils_string as su
```

### Comparing `pyXhUtils-1.3.0/src/pyXhUtils.egg-info/SOURCES.txt` & `pyXhUtils-1.3.1/src/pyXhUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_file_utils/FileUtils.py` & `pyXhUtils-1.3.1/src/xh_file_utils/FileUtils.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_ini_modifier/InitModifier.py` & `pyXhUtils-1.3.1/src/xh_ini_modifier/InitModifier.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_apache_log/ApacheLog.py` & `pyXhUtils-1.3.1/src/xh_utils_apache_log/ApacheLog.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_file_changes/FileChanges.py` & `pyXhUtils-1.3.1/src/xh_utils_file_changes/FileChanges.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_ip/IpTools.py` & `pyXhUtils-1.3.1/src/xh_utils_ip/IpTools.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_progress/ProgressPinger.py` & `pyXhUtils-1.3.1/src/xh_utils_progress/ProgressPinger.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_script_file_writer/script_writer.py` & `pyXhUtils-1.3.1/src/xh_utils_script_file_writer/script_writer.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.3.0/src/xh_utils_string/StringUtils.py` & `pyXhUtils-1.3.1/src/xh_utils_string/StringUtils.py`

 * *Files identical despite different names*

