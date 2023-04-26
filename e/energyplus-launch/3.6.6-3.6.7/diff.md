# Comparing `tmp/energyplus_launch-3.6.6.tar.gz` & `tmp/energyplus_launch-3.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.6.tar", last modified: Mon Apr 24 17:23:21 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.7.tar", last modified: Wed Apr 26 21:38:00 2023, max compression
```

## Comparing `energyplus_launch-3.6.6.tar` & `energyplus_launch-3.6.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.666286 energyplus_launch-3.6.6/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.666286 energyplus_launch-3.6.6/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.670286 energyplus_launch-3.6.6/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    70664 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.670286 energyplus_launch-3.6.6/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-26 21:38:00.000000 energyplus_launch-3.6.7/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.742522 energyplus_launch-3.6.7/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72348 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-26 21:38:00.746522 energyplus_launch-3.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-26 21:37:48.000000 energyplus_launch-3.6.7/setup.py
```

### Comparing `energyplus_launch-3.6.6/LICENSE` & `energyplus_launch-3.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/PKG-INFO` & `energyplus_launch-3.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.6
+Version: 3.6.7
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.6/README.md` & `energyplus_launch-3.6.7/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.7/energyplus_launch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.6
+Version: 3.6.7
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.6/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.7/energyplus_launch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 eplaunch/interface/dialog_generic.py
 eplaunch/interface/dialog_output.py
 eplaunch/interface/dialog_weather.py
 eplaunch/interface/dialog_workflow_dirs.py
 eplaunch/interface/frame_main.py
 eplaunch/interface/widget_dir_list.py
 eplaunch/interface/widget_file_list.py
+eplaunch/interface/widget_group_list.py
 eplaunch/utilities/__init__.py
 eplaunch/utilities/cache.py
 eplaunch/utilities/crossplatform.py
 eplaunch/utilities/exceptions.py
 eplaunch/utilities/version.py
 eplaunch/workflows/__init__.py
 eplaunch/workflows/base.py
```

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/config.py` & `energyplus_launch-3.6.7/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.7/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.7/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.7/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.7/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.7/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.7/eplaunch/interface/frame_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from platform import system
 from queue import Queue
 from sys import version_info
 
 from subprocess import Popen
 from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, Frame, Label, NSEW, E, VERTICAL, \
     SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, NORMAL, RIGHT, EW, NS, filedialog, \
-    ALL, Listbox, Scrollbar, SINGLE, Variable, HORIZONTAL
+    ALL, Scrollbar, SINGLE, Variable, HORIZONTAL
 from tkinter.ttk import Combobox, PanedWindow as ttkPanedWindow, OptionMenu, LabelFrame
 if system() == 'Darwin':
     from tkmacosx import Button
 else:
     from tkinter.ttk import Button
 from typing import Dict, List, Optional, Tuple
 from uuid import uuid4
@@ -24,14 +24,15 @@
 
 from eplaunch import VERSION, DOCS_URL, NAME
 from eplaunch.interface.dialog_generic import TkGenericDialog
 from eplaunch.utilities.exceptions import EPLaunchFileException
 from eplaunch.interface.config import ConfigManager
 from eplaunch.interface.widget_dir_list import DirListScrollableFrame
 from eplaunch.interface.widget_file_list import FileListScrollableFrame
+from eplaunch.interface.widget_group_list import GroupListBox
 from eplaunch.interface.dialog_external_viewers import TkViewerDialog
 from eplaunch.interface.dialog_weather import TkWeatherDialog
 from eplaunch.interface.dialog_workflow_dirs import TkWorkflowsDialog
 from eplaunch.interface.dialog_output import TkOutputDialog
 from eplaunch.workflows.workflow_thread import WorkflowThread
 from eplaunch.utilities.cache import CacheFile
 from eplaunch.workflows.base import BaseEPLaunchWorkflow1, EPLaunchWorkflowResponse1
@@ -204,15 +205,15 @@
         menu_group.add_command(label="Clear Current Group", command=self._clear_group)
         menu_group.add_command(label="Load new Group file...", command=self._load_new_group_file)
         menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
         menu_group.add_command(
             label="Add selected files to current group", command=self._add_current_files_to_group
         )
         menu_group.add_command(
-            label="Remove selected files from current group", command=self._remove_current_files_from_group
+            label="Set weather for current group", command=self._set_weather_for_current_group
         )
         menu_group.add_command(
             label="Cycle through current group entries", command=self._cycle_through_group
         )
         menubar.add_cascade(label="Group", menu=menu_group)
 
         menu_settings = Menu(menubar, tearoff=False)
@@ -355,20 +356,20 @@
         self.file_list = FileListScrollableFrame(
             self.dir_files_pw, on_selection_changed=self._callback_file_selection_changed
         )
         self.dir_files_pw.add(self.file_list, weight=1)
         self.list_group_pw.add(self.dir_files_pw, weight=5)
         # the bottom part of the primary pane will be a label frame containing a group listbox, add it with lower weight
         group_label_frame = LabelFrame(self.list_group_pw, text="Current Group")
-        self.group_list_box = Listbox(group_label_frame, height=5, selectmode=SINGLE)
+        self.group_list_box = GroupListBox(group_label_frame, self._group_item_delete, height=5, selectmode=SINGLE)
         self.group_list_box.bind('<Double-1>', self._handle_group_selection_from_widget)
         from string import ascii_uppercase
         for i, e in enumerate(ascii_uppercase):
             self.group_list_box.insert(i + 1, e)
-        self.group_list_box.pack(side=LEFT, fill=BOTH, expand=True)
+        self.group_list_box.pack(side=LEFT, fill=BOTH, expand=True, **self.pad)
         scroll = Scrollbar(group_label_frame)
         scroll.pack(side=RIGHT, fill=BOTH)
         self.group_list_box.config(yscrollcommand=scroll.set)
         scroll.config(command=self.group_list_box.yview)
         self.list_group_pw.add(group_label_frame, weight=1)
         # add the left paned window to the primary panes
         self.list_group_pw.pack(fill=BOTH, expand=True, **self.pad)
@@ -512,42 +513,49 @@
                 issue_warning = True
             else:
                 self.conf.group_locations.append(potential_path)
         if issue_warning:
             messagebox.showwarning("Warning", "At least one file path was already in the group and skipped")
         self._rebuild_group_menu()
 
-    def _remove_current_files_from_group(self):
-        issue_warning = False
-        for f in self.conf.file_selection:
-            potential_path = self.conf.directory / f
-            if potential_path in self.conf.group_locations:
-                self.conf.group_locations.remove(potential_path)
-            else:
-                issue_warning = True
-        if issue_warning:
-            messagebox.showwarning("Warning", "At least one file path was not in the current group and was skipped")
+    def _group_item_delete(self, indices_to_delete):
+        for i in indices_to_delete[::-1]:
+            del self.conf.group_locations[i]
         self._rebuild_group_menu()
 
     def _cycle_through_group(self):
         if len(self.conf.group_locations) == 0:
             messagebox.showwarning("Invalid Group Cycle", "Could not cycle through empty group list")
             return
         self.group_list_box.selection_clear(0, END)
         self.group_list_box.selection_set(self.group_cycle_next_index)
         self._handle_group_selection(self.group_cycle_next_index)
         self.group_cycle_next_index += 1
         if self.group_cycle_next_index + 1 > len(self.conf.group_locations):
             self.group_cycle_next_index = 0
 
+    def _get_weather_if_exists_in_cache(self, file_path: Path):
+        if not self.workflow_manager.current_workflow.uses_weather:
+            return ""
+        cache = CacheFile(file_path.parent)
+        files_in_current_workflow = cache.get_files_for_workflow(self.workflow_manager.current_workflow.name)
+        if file_path.name in files_in_current_workflow:
+            cached_file_info = files_in_current_workflow[file_path.name]
+            if CacheFile.ParametersKey in cached_file_info:
+                if CacheFile.WeatherFileKey in cached_file_info[CacheFile.ParametersKey]:
+                    return cached_file_info[CacheFile.ParametersKey][CacheFile.WeatherFileKey]
+        return ""
+
     def _rebuild_group_menu(self):
         self.group_cycle_next_index = 0
         self.group_list_box.delete(0, END)
         for index, entry in enumerate(self.conf.group_locations):
-            self.group_list_box.insert(index, str(entry))
+            known_weather_file_string = self._get_weather_if_exists_in_cache(entry)
+            suffix = f"   --   {known_weather_file_string}" if known_weather_file_string else ""
+            self.group_list_box.insert(index, f"{entry}{suffix}")
 
     def _handle_group_selection_from_widget(self, *_):
         self._handle_group_selection()
 
     def _handle_group_selection(self, specific_index: Optional[int] = None):
         if isinstance(specific_index, int):
             idx = specific_index
@@ -736,14 +744,15 @@
             # always add the row to the main list
             control_list_rows.append(row)
 
         # clear all items from the listview and then add them back in
         self.file_list.tree.set_files(control_list_rows)
         if previous_selected_files:
             self.file_list.tree.try_to_reselect(previous_selected_files)
+        self._rebuild_group_menu()
 
     def _is_file_stale(self, input_file_name: str) -> Optional[bool]:
         """
         Returns a tri-state value trying to characterize whether the current file is "stale."
         It tries to determine this based on the output suffixes of the current workflow.
         If the current workflow does not include any output suffixes, "stale" cannot be determined.
         If '.err' is in the output suffixes, this is the only suffix checked.
@@ -803,14 +812,35 @@
             cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
                 {'weather': str(new_weather_path)}
             )
         self._update_file_list()
 
+    def _set_weather_for_current_group(self):
+        dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
+        self.wait_window(dialog_weather)
+        if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
+            return
+        if not dialog_weather.selected_weather_file:
+            weather_file_to_use = self.dd_only_string
+        else:
+            weather_file_to_use = dialog_weather.selected_weather_file
+            if weather_file_to_use not in self.conf.weathers_recent:
+                self.conf.weathers_recent.appendleft(weather_file_to_use)
+                self._repopulate_recent_weather_list(weather_file_to_use)
+        for selected_path in self.conf.group_locations:
+            workflow_directory_cache = CacheFile(selected_path.parent)
+            workflow_directory_cache.add_config(
+                self.workflow_manager.current_workflow.name,
+                selected_path.name,
+                {'weather': str(weather_file_to_use)}
+            )
+        self._update_file_list()
+
     def _open_weather_dialog(self) -> None:
         dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
         self.wait_window(dialog_weather)
         if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
             return
         if not dialog_weather.selected_weather_file:
             weather_file_to_use = self.dd_only_string
@@ -937,15 +967,15 @@
         self._tk_var_output_3.set(suffixes[2] if len(suffixes) > 2 else '--')
         self.button_open_output_4.configure(state=NORMAL if len(suffixes) > 3 else DISABLED)
         self._tk_var_output_4.set(suffixes[3] if len(suffixes) > 3 else '--')
         self.button_open_output_5.configure(state=NORMAL if len(suffixes) > 4 else DISABLED)
         self._tk_var_output_5.set(suffixes[4] if len(suffixes) > 4 else '--')
         self._refresh_output_suffix_buttons_based_on_selection()
 
-    def suffixed_paths_exist(self, original_path: Path, new_suffix: str) -> Tuple[Optional[Path], Optional[Path]]:
+    def _suffixed_paths_exist(self, original_path: Path, new_suffix: str) -> Tuple[Optional[Path], Optional[Path]]:
         filename_no_ext = original_path.with_suffix('').name
         new_path = self.conf.directory / (filename_no_ext + new_suffix)
         eplus_sub_dir = f"EPLaunchRun_{filename_no_ext}"
         eplus_specific_output_path = self.conf.directory / eplus_sub_dir / f"{filename_no_ext}{new_suffix}"
         primary_path_to_return = new_path if new_path.exists() else None
         eplus_path_to_return = eplus_specific_output_path if eplus_specific_output_path.exists() else None
         return primary_path_to_return, eplus_path_to_return
@@ -954,15 +984,15 @@
         if tk_var.get() == '--':
             return
         else:
             suffix_to_open = tk_var.get()
             all_files_have_this_suffix = True
             for f in self.conf.file_selection:
                 original_path = self.conf.directory / f
-                new_path, eplus_path = self.suffixed_paths_exist(original_path, suffix_to_open)
+                new_path, eplus_path = self._suffixed_paths_exist(original_path, suffix_to_open)
                 if (new_path and new_path.exists()) or (eplus_path and eplus_path.exists()):
                     pass  # good
                 else:
                     all_files_have_this_suffix = False
                     break
             button.configure(state=NORMAL if all_files_have_this_suffix else DISABLED)
 
@@ -1050,15 +1080,15 @@
     def _run_workflow_on_group(self) -> None:
         file_paths = self.conf.group_locations
         self._run_workflow_on_list_of_file_paths(file_paths)
 
     def _run_workflow_on_list_of_file_paths(self, file_paths: List[Path]):
 
         # error out early
-        if self.conf.directory and self.conf.file_selection and self.workflow_manager.current_workflow:
+        if self.conf.directory and file_paths and self.workflow_manager.current_workflow:
             pass
         else:
             messagebox.showerror(title='Selection', message='ERROR: Select a workflow, directory and a file')
             return
 
         already_running_instances = []
         cur_workflow = self.workflow_manager.current_workflow
```

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.7/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.7/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.7/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.7/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/utilities/version.py` & `energyplus_launch-3.6.7/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/base.py` & `energyplus_launch-3.6.7/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.7/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.7/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.7/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.7/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.7/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.7/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.7/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.6/setup.py` & `energyplus_launch-3.6.7/setup.py`

 * *Files identical despite different names*

