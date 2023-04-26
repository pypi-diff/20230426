# Comparing `tmp/pymodaq_plugins_newport-1.0.0.tar.gz` & `tmp/pymodaq_plugins_newport-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_newport-1.0.0.tar", last modified: Tue Apr 25 16:24:42 2023, max compression
+gzip compressed data, was "pymodaq_plugins_newport-1.0.1.tar", last modified: Tue Apr 25 16:27:43 2023, max compression
```

## Comparing `pymodaq_plugins_newport-1.0.0.tar` & `pymodaq_plugins_newport-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.065218 pymodaq_plugins_newport-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/agilis_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/esp100.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/serial_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 16:24:27.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/smc100.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:24:42.069218 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 16:24:42.000000 pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.479519 pymodaq_plugins_newport-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.483519 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/agilis_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/esp100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/serial_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/smc100.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.483519 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_newport-1.0.0/LICENSE` & `pymodaq_plugins_newport-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/PKG-INFO` & `pymodaq_plugins_newport-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_newport
-Version: 1.0.0
+Version: 1.0.1
 Summary: Set of PyMoDAQ plugins for instruments from Newport (Conex, ESP100,...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_newport
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_newport-1.0.0/README.rst` & `pymodaq_plugins_newport-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/setup.py` & `pymodaq_plugins_newport-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/agilis_serial.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/agilis_serial.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/esp100.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/esp100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/serial_base.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/serial_base.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport/hardware/smc100.py` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/smc100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/PKG-INFO` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-newport
-Version: 1.0.0
+Version: 1.0.1
 Summary: Set of PyMoDAQ plugins for instruments from Newport (Conex, ESP100,...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_newport
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_newport-1.0.0/src/pymodaq_plugins_newport.egg-info/SOURCES.txt` & `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

