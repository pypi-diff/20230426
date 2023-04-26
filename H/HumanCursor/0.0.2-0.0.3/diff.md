# Comparing `tmp/HumanCursor-0.0.2.tar.gz` & `tmp/HumanCursor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.2.tar", last modified: Wed Apr 26 15:23:44 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.3.tar", last modified: Wed Apr 26 15:32:20 2023, max compression
```

## Comparing `HumanCursor-0.0.2.tar` & `HumanCursor-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.318408 HumanCursor-0.0.2/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5040 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5040 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.345242 HumanCursor-0.0.2/cursors/
--rw-rw-rw-   0        0        0       90 2023-04-25 16:41:52.000000 HumanCursor-0.0.2/cursors/__init__.py
--rw-rw-rw-   0        0        0     1114 2023-04-25 15:16:55.000000 HumanCursor-0.0.2/cursors/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/cursors/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.2/cursors/utilities/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-04-25 15:13:53.000000 HumanCursor-0.0.2/cursors/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     8523 2023-04-25 15:16:55.000000 HumanCursor-0.0.2/cursors/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6919 2023-04-25 16:44:12.000000 HumanCursor-0.0.2/cursors/web_cursor.py
--rw-rw-rw-   0        0        0      643 2023-04-26 15:22:58.000000 HumanCursor-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.413518 HumanCursor-0.0.3/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5040 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5040 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.422080 HumanCursor-0.0.3/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.428037 HumanCursor-0.0.3/humancursor/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.3/humancursor/utilities/__init__.py
+-rw-rw-rw-   0        0        0     7848 2023-04-25 15:13:53.000000 HumanCursor-0.0.3/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     8531 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      643 2023-04-26 15:31:53.000000 HumanCursor-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/setup.cfg
```

### Comparing `HumanCursor-0.0.2/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.3/HumanCursor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.2/LICENSE` & `HumanCursor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.2/PKG-INFO` & `HumanCursor-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.2/README.md` & `HumanCursor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.2/cursors/system_cursor.py` & `HumanCursor-0.0.3/humancursor/system_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
 import random
 import pyautogui
 
-from cursors.utilities.human_curve_generator import HumanizeMouseTrajectory
+from humancursor.utilities.human_curve_generator import HumanizeMouseTrajectory
 
 
 class SystemCursor:
     def __init__(self):
         pyautogui.MINIMUM_DURATION = 0
         pyautogui.MINIMUM_SLEEP = 0
         pyautogui.PAUSE = 0.015
```

### Comparing `HumanCursor-0.0.2/cursors/utilities/human_curve_generator.py` & `HumanCursor-0.0.3/humancursor/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.2/cursors/utilities/web_adjuster.py` & `HumanCursor-0.0.3/humancursor/utilities/web_adjuster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import pytweening
 
 from selenium.common import MoveTargetOutOfBoundsException
 from selenium.webdriver.common.action_chains import ActionChains
 
-from cursors.utilities.human_curve_generator import HumanizeMouseTrajectory
+from humancursor.utilities.human_curve_generator import HumanizeMouseTrajectory
 
 
 class WebAdjuster:
     def __init__(self, driver):
         self.__driver = driver
         self.__action = ActionChains(self.__driver, duration=0)
         self.origin_coordinate = [0, 0]
@@ -17,15 +17,15 @@
         self,
         element_or_pos,
         origin_coordinates=None,
         absolute_offset=False,
         relative_position=None,
         human_curve=None,
     ):
-        """Moves the cursors, trying to mimic human behaviour!"""
+        """Moves the humancursor, trying to mimic human behaviour!"""
         origin = origin_coordinates
         if origin_coordinates is None:
             origin = self.origin_coordinate
 
         pre_origin = tuple(origin)
         if isinstance(element_or_pos, list):
             if not absolute_offset:
```

### Comparing `HumanCursor-0.0.2/cursors/web_cursor.py` & `HumanCursor-0.0.3/humancursor/web_cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import sleep
 import random
 
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.remote.webelement import WebElement
 
-from cursors.utilities.web_adjuster import WebAdjuster
+from humancursor.utilities.web_adjuster import WebAdjuster
 
 
 class WebCursor:
     def __init__(self, driver):
         self.__driver = driver
         self.__action = ActionChains(self.__driver, duration=1500)
         self.human = WebAdjuster(self.__driver)
```

### Comparing `HumanCursor-0.0.2/pyproject.toml` & `HumanCursor-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

