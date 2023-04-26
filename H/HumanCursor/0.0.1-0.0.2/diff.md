# Comparing `tmp/HumanCursor-0.0.1.tar.gz` & `tmp/HumanCursor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.1.tar", last modified: Tue Apr 25 17:12:16 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.2.tar", last modified: Wed Apr 26 15:23:44 2023, max compression
```

## Comparing `HumanCursor-0.0.1.tar` & `HumanCursor-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:12:16.612440 HumanCursor-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:12:16.595572 HumanCursor-0.0.1/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5034 2023-04-25 17:12:16.000000 HumanCursor-0.0.1/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-25 17:12:16.000000 HumanCursor-0.0.1/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:12:16.000000 HumanCursor-0.0.1/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 17:12:16.000000 HumanCursor-0.0.1/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5034 2023-04-25 17:12:16.612440 HumanCursor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4553 2023-04-25 17:11:41.000000 HumanCursor-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 17:12:16.603407 HumanCursor-0.0.1/cursors/
--rw-rw-rw-   0        0        0       90 2023-04-25 16:41:52.000000 HumanCursor-0.0.1/cursors/__init__.py
--rw-rw-rw-   0        0        0     1114 2023-04-25 15:16:55.000000 HumanCursor-0.0.1/cursors/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:12:16.612440 HumanCursor-0.0.1/cursors/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.1/cursors/utilities/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-04-25 15:13:53.000000 HumanCursor-0.0.1/cursors/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     8523 2023-04-25 15:16:55.000000 HumanCursor-0.0.1/cursors/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6919 2023-04-25 16:44:12.000000 HumanCursor-0.0.1/cursors/web_cursor.py
--rw-rw-rw-   0        0        0      569 2023-04-25 17:07:50.000000 HumanCursor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 17:12:16.618478 HumanCursor-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.318408 HumanCursor-0.0.2/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5040 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 15:23:44.000000 HumanCursor-0.0.2/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5040 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.345242 HumanCursor-0.0.2/cursors/
+-rw-rw-rw-   0        0        0       90 2023-04-25 16:41:52.000000 HumanCursor-0.0.2/cursors/__init__.py
+-rw-rw-rw-   0        0        0     1114 2023-04-25 15:16:55.000000 HumanCursor-0.0.2/cursors/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/cursors/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.2/cursors/utilities/__init__.py
+-rw-rw-rw-   0        0        0     7848 2023-04-25 15:13:53.000000 HumanCursor-0.0.2/cursors/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     8523 2023-04-25 15:16:55.000000 HumanCursor-0.0.2/cursors/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     6919 2023-04-25 16:44:12.000000 HumanCursor-0.0.2/cursors/web_cursor.py
+-rw-rw-rw-   0        0        0      643 2023-04-26 15:22:58.000000 HumanCursor-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:23:44.365259 HumanCursor-0.0.2/setup.cfg
```

### Comparing `HumanCursor-0.0.1/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.2/HumanCursor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,15 +32,15 @@
 ### WebCursor
 
 To use HumanCursor for Web, you need to import the `WebCursor` class, and create an instance:
 
 ```python
 from HumanCursor.cursors import WebCursor
 
-cursor = WebCursor()
+cursor = WebCursor(driver)
 ```
 
 Then, you can use the following methods to simulate mouse movements and actions:
 
 - `cursor.move_to()`: Moves the mouse cursor to the element or location on the webpage.
 - `cursor.click_on()`: Clicks on the element or location on the webpage.
 - `cursor.drag_and_drop()`: Drags the mouse cursor from one element and drops it to another element on the screen.
```

### Comparing `HumanCursor-0.0.1/LICENSE` & `HumanCursor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.1/PKG-INFO` & `HumanCursor-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,15 +32,15 @@
 ### WebCursor
 
 To use HumanCursor for Web, you need to import the `WebCursor` class, and create an instance:
 
 ```python
 from HumanCursor.cursors import WebCursor
 
-cursor = WebCursor()
+cursor = WebCursor(driver)
 ```
 
 Then, you can use the following methods to simulate mouse movements and actions:
 
 - `cursor.move_to()`: Moves the mouse cursor to the element or location on the webpage.
 - `cursor.click_on()`: Clicks on the element or location on the webpage.
 - `cursor.drag_and_drop()`: Drags the mouse cursor from one element and drops it to another element on the screen.
```

### Comparing `HumanCursor-0.0.1/README.md` & `HumanCursor-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ### WebCursor
 
 To use HumanCursor for Web, you need to import the `WebCursor` class, and create an instance:
 
 ```python
 from HumanCursor.cursors import WebCursor
 
-cursor = WebCursor()
+cursor = WebCursor(driver)
 ```
 
 Then, you can use the following methods to simulate mouse movements and actions:
 
 - `cursor.move_to()`: Moves the mouse cursor to the element or location on the webpage.
 - `cursor.click_on()`: Clicks on the element or location on the webpage.
 - `cursor.drag_and_drop()`: Drags the mouse cursor from one element and drops it to another element on the screen.
```

### Comparing `HumanCursor-0.0.1/cursors/system_cursor.py` & `HumanCursor-0.0.2/cursors/system_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.1/cursors/utilities/human_curve_generator.py` & `HumanCursor-0.0.2/cursors/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.1/cursors/utilities/web_adjuster.py` & `HumanCursor-0.0.2/cursors/utilities/web_adjuster.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.1/cursors/web_cursor.py` & `HumanCursor-0.0.2/cursors/web_cursor.py`

 * *Files identical despite different names*

