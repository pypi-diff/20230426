# Comparing `tmp/pymodaq_plugins_holoeye-1.0.0.tar.gz` & `tmp/pymodaq_plugins_holoeye-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_holoeye-1.0.0.tar", last modified: Thu Apr 13 15:32:18 2023, max compression
+gzip compressed data, was "pymodaq_plugins_holoeye-1.0.2.tar", last modified: Tue Apr 25 13:58:26 2023, max compression
```

## Comparing `pymodaq_plugins_holoeye-1.0.0.tar` & `pymodaq_plugins_holoeye-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.812586 pymodaq_plugins_holoeye-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-13 15:32:18.812586 pymodaq_plugins_holoeye-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:32:18.812586 pymodaq_plugins_holoeye-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.800586 pymodaq_plugins_holoeye-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.804586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFullScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeSplitScreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.808586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/hardware/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.812586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/resources/config_template.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-13 15:32:06.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/resources/daq_move_HoloeyeBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:32:18.804586 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 15:32:18.000000 pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:58:26.759338 pymodaq_plugins_holoeye-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.751338 pymodaq_plugins_holoeye-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFullScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeSplitScreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/hardware/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/resources/config_template.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-25 13:58:13.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/resources/daq_move_HoloeyeBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:58:26.755339 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 13:58:26.000000 pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_holoeye-1.0.0/LICENSE` & `pymodaq_plugins_holoeye-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/PKG-INFO` & `pymodaq_plugins_holoeye-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_holoeye
-Version: 1.0.0
+Version: 1.0.2
 Summary: Set of PyMoDAQ plugins for Holoeye Spatial Light Modulator (SLM)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_holoeye
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,26 +14,14 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 License-File: LICENSE
 
-# PyMoDAQ Plugins
-
-PyMoDAQ, Modular Data Acquisition with Python, is a set of **python** modules used to perform automated measurements. 
-
-This repository contains a set of PyMoDAQ plugins for Holoeye Spatial Light Modulator (SLM)
-
-For an exhaustive list of the available plugins, see https://github.com/PyMoDAQ/pymodaq_plugin_manager/blob/main/pymodaq_plugin_manager/doc/PluginList.md
-
-GitHub repo: https://github.com/PyMoDAQ
-
-Documentation: http://pymodaq.cnrs.fr/
-
 pymodaq_plugins_holoeye (HoloEye Instruments)
 #############################################
 
 .. the following must be adapted to your developped package, links to pypi, github  description...
 
 .. image:: https://img.shields.io/pypi/v/pymodaq_plugins_holoeye.svg
    :target: https://pypi.org/project/pymodaq_plugins_holoeye/
```

### Comparing `pymodaq_plugins_holoeye-1.0.0/README.rst` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-# PyMoDAQ Plugins
-
-PyMoDAQ, Modular Data Acquisition with Python, is a set of **python** modules used to perform automated measurements. 
-
-This repository contains a set of PyMoDAQ plugins for Holoeye Spatial Light Modulator (SLM)
-
-For an exhaustive list of the available plugins, see https://github.com/PyMoDAQ/pymodaq_plugin_manager/blob/main/pymodaq_plugin_manager/doc/PluginList.md
-
-GitHub repo: https://github.com/PyMoDAQ
-
-Documentation: http://pymodaq.cnrs.fr/
+Metadata-Version: 2.1
+Name: pymodaq-plugins-holoeye
+Version: 1.0.2
+Summary: Set of PyMoDAQ plugins for Holoeye Spatial Light Modulator (SLM)
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_holoeye
+Author: Sébastien Weber
+Author-email: sebastien.weber@cemes.fr
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+License-File: LICENSE
 
 pymodaq_plugins_holoeye (HoloEye Instruments)
 #############################################
 
 .. the following must be adapted to your developped package, links to pypi, github  description...
 
 .. image:: https://img.shields.io/pypi/v/pymodaq_plugins_holoeye.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodaq_plugins_holoeye-1.0.0/setup.py` & `pymodaq_plugins_holoeye-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/__init__.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 
 environs = []
 for env in os.environ.keys():
     if 'HEDS' in env and 'MODULES' in env:
         environs.append(env)
 
-sorted(environs)
-sys.path.append(os.getenv(environs[0], ''))
+environs = sorted(environs)
+if 'HEDS_PYTHON_MODULES' in environs:
+    environs.remove('HEDS_PYTHON_MODULES', )
+sys.path.append(os.getenv(environs[-1], ''))
 
 
 class Config(BaseConfig):
     """Main class to deal with configuration values for PyMoDAQ"""
     config_template_path = Path(__file__).parent.joinpath('resources/config_template.toml')
     config_name = 'config_holoeye'
```

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFile.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFile.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFullScreen.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeFullScreen.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeSplitScreen.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/daq_move_plugins/daq_move_HoloeyeSplitScreen.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/hardware/basic.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/hardware/basic.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye/resources/daq_move_HoloeyeBase.py` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye/resources/daq_move_HoloeyeBase.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_holoeye-1.0.0/src/pymodaq_plugins_holoeye.egg-info/SOURCES.txt` & `pymodaq_plugins_holoeye-1.0.2/src/pymodaq_plugins_holoeye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

