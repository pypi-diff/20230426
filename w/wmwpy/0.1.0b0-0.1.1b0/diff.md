# Comparing `tmp/wmwpy-0.1.0b0.tar.gz` & `tmp/wmwpy-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.1.0b0.tar", last modified: Mon Apr 24 18:54:34 2023, max compression
+gzip compressed data, was "wmwpy-0.1.1b0.tar", last modified: Tue Apr 25 17:18:19 2023, max compression
```

## Comparing `wmwpy-0.1.0b0.tar` & `wmwpy-0.1.1b0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.714650 wmwpy-0.1.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/Widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.1.0b0/LICENSE` & `wmwpy-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/PKG-INFO` & `wmwpy-0.1.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.1.0b0/README.md` & `wmwpy-0.1.1b0/README.md`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/pyproject.toml` & `wmwpy-0.1.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Game.py` & `wmwpy-0.1.1b0/src/wmwpy/Game.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.1.1b0/src/wmwpy/Utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Utils/textures.py` & `wmwpy-0.1.1b0/src/wmwpy/Utils/textures.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.1.1b0/src/wmwpy/Utils/waltex.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/__init__.py` & `wmwpy-0.1.1b0/src/wmwpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0-beta"
+__version__ = "0.1.1-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
 
 from .Game import Game
 from . import classes
 from . import Font
```

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/Widgets.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/curves.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/imagelist.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/layout.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/layout.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/level.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/level.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/object.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/object.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/sprite.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/sprite.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/widget/Widget.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/widget/widget.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.1.1b0/src/wmwpy/classes/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/gameobject.py` & `wmwpy-0.1.1b0/src/wmwpy/gameobject.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy/gametemplate.py` & `wmwpy-0.1.1b0/src/wmwpy/gametemplate.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.0b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.1.1b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.1.0b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.1.1b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 src/wmwpy/classes/widget/WT_LABEL.py
 src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
 src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
 src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
 src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
 src/wmwpy/classes/widget/WT_SLIDER.py
 src/wmwpy/classes/widget/WT_TOGGLE.py
-src/wmwpy/classes/widget/Widget.py
-src/wmwpy/classes/widget/__init__.py
+src/wmwpy/classes/widget/__init__.py
+src/wmwpy/classes/widget/widget.py
```

