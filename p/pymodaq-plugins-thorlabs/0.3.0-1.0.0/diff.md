# Comparing `tmp/pymodaq_plugins_thorlabs-0.3.0.tar.gz` & `tmp/pymodaq_plugins_thorlabs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_thorlabs-0.3.0.tar", last modified: Wed Jan 25 19:36:57 2023, max compression
+gzip compressed data, was "pymodaq_plugins_thorlabs-1.0.0.tar", last modified: Tue Apr 25 16:29:49 2023, max compression
```

## Comparing `pymodaq_plugins_thorlabs-0.3.0.tar` & `pymodaq_plugins_thorlabs-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.909058 pymodaq_plugins_thorlabs-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.909058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.909058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.909058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.913058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-01-25 19:36:46.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:36:57.909058 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 19:36:57.000000 pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/LICENSE` & `pymodaq_plugins_thorlabs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-0.3.0/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq_plugins_thorlabs
-Version: 0.3.0
+Name: pymodaq-plugins-thorlabs
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/README.rst` & `pymodaq_plugins_thorlabs-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-0.3.0/setup.py` & `pymodaq_plugins_thorlabs-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,12 +38,13 @@
 
 
 setup(
     version=version,
     packages=find_packages(where='./src'),
     package_dir={'': 'src'},
     include_package_data=True,
-    entry_points={'pymodaq.plugins': f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}'},
+    entry_points={'pymodaq.plugins': f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}',
+                  'pymodaq.pid_models': f"{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}"},
     install_requires=['toml', ]+config['plugin-install']['packages-required'],
     **setupOpts
 )
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Plugin for the K10CR1 Integrated Stepper motor for rotation
 Its is using the Instrumental package with its kinesis driver (based from the C-libraries)
 Thorlabs Kinesis drivers and SDKs should be installed and the path to where are located the dlls should be added to
 the PATH system environment variable
 """
 
-from pymodaq.daq_move.utility_classes import DAQ_Move_base, main
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, find_dict_in_list_from_key_val
-import clr
-import sys
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
+from pymodaq.control_modules.move_utility_classes import comon_parameters
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo, find_dict_in_list_from_key_val
 from easydict import EasyDict as edict
 from instrumental.drivers.motion.kinesis import list_instruments
 from instrumental import instrument
 
 parameter_sets = list_instruments()
 serialnumbers = [pset['serial'] for pset in parameter_sets if pset['classname'] == 'K10CR1']
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from pymodaq.daq_move.utility_classes import DAQ_Move_base, main
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, set_logger, get_module_name
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
+from pymodaq.control_modules.move_utility_classes import comon_parameters
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.logger import set_logger, get_module_name
 import clr
 from qtpy import QtWidgets
 import sys
 from easydict import EasyDict as edict
 
-
-
 from System import Decimal
 from System import Action
 from System import UInt64
 
 kinesis_path = 'C:\\Program Files\\Thorlabs\\Kinesis'
 sys.path.append(kinesis_path)
 clr.AddReference("Thorlabs.MotionControl.DeviceManagerCLI")
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from pymodaq.daq_move.utility_classes import DAQ_Move_base
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
+from pymodaq.control_modules.move_utility_classes import comon_parameters
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
 import clr
 import sys
+
+
 class DAQ_Move_Kinesis_Flipper(DAQ_Move_base):
     """
         Wrapper object to access the conex fonctionnalities, similar wrapper for all controllers.
 
         ================ =================
         **Attributes**    **Type**
         *Kinesis_path*    string
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pymodaq.daq_move.utility_classes import DAQ_Move_base
-from pymodaq.daq_move.utility_classes import comon_parameters
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
+from pymodaq.control_modules.move_utility_classes import comon_parameters
 from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
 
 import pylablib.devices.Thorlabs as Thorlabs
 
 is_multiaxes = False
 stage_names = []
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pymodaq.daq_move.utility_classes import DAQ_Move_base
-from pymodaq.daq_move.utility_classes import comon_parameters
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
+from pymodaq.control_modules.move_utility_classes import comon_parameters
 from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
 
 import pylablib.devices.Thorlabs as Thorlabs
 
 is_multiaxes = False
 stage_names = []
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
 from qtpy.QtCore import QThread
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
 from collections import OrderedDict
 import numpy as np
 import clr
-from pymodaq.daq_viewer.utility_classes import comon_parameters
-
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
 
 class DAQ_0DViewer_Kinesis_KPA101(DAQ_Viewer_base):
     """
         ==================== ========================
         **Attributes**        **Type**
         *data_grabed_signal*  instance of Signal
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,21 @@
 The installation should create (following the manual) an environment variable called either VXIPNPPATH64 or
 VXIPNPPATH depending on your platform (32 or 64 bits) pointing to where the TLPM library is
 (usually C:\Program Files\IVI Foundation\VISA)
 
 This plugin is making use of the TLPM.py script provided by thorlabs. An alternative is to use the TLPMPowermeterInst
 plugin using the Instrumental_lib package directly interfacing the C library with the nice Instrument wrapper
 """
-
-
-import sys
-from qtpy.QtCore import QThread
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, main
-from collections import OrderedDict
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
+
 import numpy as np
-from pymodaq.daq_viewer.utility_classes import comon_parameters
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 from pymodaq_plugins_thorlabs.hardware.powermeter import CustomTLPM, DEVICE_NAMES
 
 
 class DAQ_0DViewer_TLPMPowermeter(DAQ_Viewer_base):
 
     _controller_units = 'W'
     devices = DEVICE_NAMES
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 (usually C:\Program Files\IVI Foundation\VISA)
 
 This plugin is using the Instrumental_lib package directly interfacing the C library with the nice **instrument** wrapper
 """
 import sys
 from qtpy.QtCore import QThread
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, main
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 from collections import OrderedDict
 import numpy as np
-from pymodaq.daq_viewer.utility_classes import comon_parameters
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
 from instrumental import list_instruments, instrument, Q_
 
 
 psets = list_instruments(module='powermeters.thorlabs_tlpm')
 DEVICES = [f"{pset['model']}/{pset['serial']}" for pset in psets]
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, comon_parameters, main
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
 from instrumental import instrument, list_instruments, Q_
 
 # This is a (probably bad) way of importing the stuff needed to get exposure range
 import instrumental.drivers.cameras.uc480 as uc480module
 
 
 class DAQ_2DViewer_Thorlabs_DCx(DAQ_Viewer_base):
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from pymodaq.daq_utils.daq_utils import ThreadCommand
-from pymodaq.daq_utils.daq_utils import DataFromPlugins, Axis
+from pymodaq.utils.daq_utils import ThreadCommand
+from pymodaq.utils.data import DataFromPlugins, Axis
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
-from pymodaq.daq_utils.parameter import Parameter
+from pymodaq.utils.parameter import Parameter
 
 from pylablib.devices import Thorlabs
 from qtpy import QtWidgets, QtCore
 import numpy as np
 from time import perf_counter
 
 
@@ -51,15 +51,15 @@
         self.last_tick = 0.0  # time counter used to compute FPS
         self.fps = 0.0
 
         self.data_shape = 'Data2D'
         self.callback_thread = None
 
         # Disable "use ROI" option to avoid confusion with other buttons
-        self.settings.child('ROIselect', 'use_ROI').setOpts(visible=False)
+        #self.settings.child('ROIselect', 'use_ROI').setOpts(visible=False)
 
     def commit_settings(self, param: Parameter):
         """Apply the consequences of a change of value in the detector settings
 
         Parameters
         ----------
         param: Parameter
@@ -272,19 +272,14 @@
                 self.fps = 0.9 * self.fps + 0.1 / frame_time
 
         self.last_tick = current_tick
 
         # Update reading
         self.settings.child('timing_opts', 'fps').setValue(round(self.fps, 1))
 
-
-    def callback(self):
-        """optional asynchrone method called when the detector has finished its acquisition of data"""
-        raise NotImplementedError
-
     def close(self):
         """
         Terminate the communication protocol
         """
         # Terminate the communication
         self.controller.close()
         self.controller = None  # Garbage collect the controller
@@ -298,19 +293,21 @@
         self.controller.clear_acquisition()
         return ''
 
 
 class ThorlabsCallback(QtCore.QObject):
     """Callback object """
     data_sig = QtCore.Signal()
-    def __init__(self,wait_fn):
+
+    def __init__(self, wait_fn):
         super().__init__()
-        #Set the wait function
+        # Set the wait function
         self.wait_fn = wait_fn
 
     def wait_for_acquisition(self):
         new_data = self.wait_fn()
-        if new_data is not False: #will be returned if the main thread called CancelWait
+        if new_data is not False:  # will be returned if the main thread called CancelWait
             self.data_sig.emit()
 
+
 if __name__ == '__main__':
-    main(__file__)
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 import os
 import sys
 import importlib
 from pathlib import Path
 import ctypes
 import functools
 
-from pymodaq.daq_utils import daq_utils as utils
-
-logger = utils.set_logger(utils.get_module_name(__file__))
+from pymodaq.utils import daq_utils as utils
+from pymodaq.utils.logger import set_logger, get_module_name
+logger = set_logger(get_module_name(__file__))
 if utils.is_64bits():
     path_dll = str(Path(os.environ['VXIPNPPATH64']).joinpath('Win64', 'Bin'))
 else:
     path_dll = str(Path(os.environ['VXIPNPPATH']).joinpath('WinNT', 'Bin'))
 os.add_dll_directory(path_dll)
 
 try:
@@ -191,15 +191,19 @@
     @error_handling()
     def wavelength(self, wavelength: float):
         wavelength = ctypes.c_double(wavelength)
         self._tlpm.setWavelength(wavelength)
 
 
 if __name__ == '__main__':
+    from time import sleep
     print(Ndevices)
     print(DEVICE_NAMES)
 
     with CustomTLPM(0) as tlpm:
-        tlpm.wavelength
-        tlpm.get_power()
+        print(tlpm.wavelength)
+        tlpm.wavelength = 532.
+        sleep(1)
+        print(tlpm.wavelength)
+        print(tlpm.get_power())
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq-plugins-thorlabs
-Version: 0.3.0
+Name: pymodaq_plugins_thorlabs
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-0.3.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt` & `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

