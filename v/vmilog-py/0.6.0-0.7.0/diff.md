# Comparing `tmp/vmilog-py-0.6.0.tar.gz` & `tmp/vmilog-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmilog-py-0.6.0.tar", last modified: Fri Apr 21 04:20:30 2023, max compression
+gzip compressed data, was "vmilog-py-0.7.0.tar", last modified: Wed Apr 26 14:33:54 2023, max compression
```

## Comparing `vmilog-py-0.6.0.tar` & `vmilog-py-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.080753 vmilog-py-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-21 04:20:30.080753 vmilog-py-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:20:30.080753 vmilog-py-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.072754 vmilog-py-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.076753 vmilog-py-0.6.0/src/vmi485tousb/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmi485tousb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmi485tousb/_uartChannel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.076753 vmilog-py-0.6.0/src/vmiiputil/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmiiputil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmiiputil/_iputil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.076753 vmilog-py-0.6.0/src/vmilog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmilog/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.080753 vmilog-py-0.6.0/src/vmilog_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-21 04:20:30.000000 vmilog-py-0.6.0/src/vmilog_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-21 04:20:30.000000 vmilog-py-0.6.0/src/vmilog_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:20:30.000000 vmilog-py-0.6.0/src/vmilog_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 04:20:30.000000 vmilog-py-0.6.0/src/vmilog_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 04:20:30.000000 vmilog-py-0.6.0/src/vmilog_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:20:30.080753 vmilog-py-0.6.0/src/vmimpeg/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmimpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-21 04:20:03.000000 vmilog-py-0.6.0/src/vmimpeg/_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.278957 vmilog-py-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.278957 vmilog-py-0.7.0/src/vmi485tousb/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmi485tousb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmi485tousb/_uartChannel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/src/vmiiputil/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmiiputil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmiiputil/_iputil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/src/vmilog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmilog/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/src/vmilog_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 14:33:54.000000 vmilog-py-0.7.0/src/vmilog_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 14:33:54.000000 vmilog-py-0.7.0/src/vmilog_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:33:54.000000 vmilog-py-0.7.0/src/vmilog_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 14:33:54.000000 vmilog-py-0.7.0/src/vmilog_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:33:54.000000 vmilog-py-0.7.0/src/vmilog_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:33:54.282957 vmilog-py-0.7.0/src/vmimpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmimpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 14:33:22.000000 vmilog-py-0.7.0/src/vmimpeg/_stream.py
```

### Comparing `vmilog-py-0.6.0/LICENSE` & `vmilog-py-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.6.0/PKG-INFO` & `vmilog-py-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmilog-py
-Version: 0.6.0
+Version: 0.7.0
 Summary: log library for vmilabs
 Home-page: https://github.com/openvmi/vmilog-py
 Author: vmilabs
 Author-email: zeekzhou@163.com
 License: Apache-2.0
 Keywords: vmilabs log sdk
 Requires-Python: >=3.6
```

### Comparing `vmilog-py-0.6.0/setup.py` & `vmilog-py-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.6.0"
+VERSION = "0.7.0"
 
 install_requires = [
     'netifaces==0.11.0',
     'pyserial'
 ]
 
 setup(
```

### Comparing `vmilog-py-0.6.0/src/vmi485tousb/_uartChannel.py` & `vmilog-py-0.7.0/src/vmi485tousb/_uartChannel.py`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.6.0/src/vmilog/_logging.py` & `vmilog-py-0.7.0/src/vmilog/_logging.py`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.6.0/src/vmilog_py.egg-info/PKG-INFO` & `vmilog-py-0.7.0/src/vmilog_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmilog-py
-Version: 0.6.0
+Version: 0.7.0
 Summary: log library for vmilabs
 Home-page: https://github.com/openvmi/vmilog-py
 Author: vmilabs
 Author-email: zeekzhou@163.com
 License: Apache-2.0
 Keywords: vmilabs log sdk
 Requires-Python: >=3.6
```

