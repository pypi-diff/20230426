# Comparing `tmp/kmlb-0.0.87.tar.gz` & `tmp/kmlb-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmlb-0.0.87.tar", last modified: Fri Apr  7 18:55:41 2023, max compression
+gzip compressed data, was "kmlb-0.0.88.tar", last modified: Wed Apr 26 02:31:30 2023, max compression
```

## Comparing `kmlb-0.0.87.tar` & `kmlb-0.0.88.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 18:55:41.902452 kmlb-0.0.87/
--rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.87/LICENSE.md
--rw-rw-rw-   0        0        0    38527 2023-04-07 18:55:41.900986 kmlb-0.0.87/PKG-INFO
--rw-rw-rw-   0        0        0    38044 2023-04-07 16:36:25.000000 kmlb-0.0.87/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 18:55:41.885244 kmlb-0.0.87/kmlb/
--rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.87/kmlb/__init__.py
--rw-rw-rw-   0        0        0    37252 2023-04-07 18:04:47.000000 kmlb-0.0.87/kmlb/base.py
--rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.87/kmlb/gis_basics.py
--rw-rw-rw-   0        0        0     2491 2023-04-07 16:36:25.000000 kmlb-0.0.87/kmlb/shapes.py
-drwxrwxrwx   0        0        0        0 2023-04-07 18:55:41.900986 kmlb-0.0.87/kmlb.egg-info/
--rw-rw-rw-   0        0        0    38527 2023-04-07 18:55:41.000000 kmlb-0.0.87/kmlb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-04-07 18:55:41.000000 kmlb-0.0.87/kmlb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 18:55:41.000000 kmlb-0.0.87/kmlb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-07 18:55:41.000000 kmlb-0.0.87/kmlb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 18:55:41.902452 kmlb-0.0.87/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-07 18:53:39.000000 kmlb-0.0.87/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.954977 kmlb-0.0.88/
+-rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.88/LICENSE.md
+-rw-rw-rw-   0        0        0    38527 2023-04-26 02:31:30.954977 kmlb-0.0.88/PKG-INFO
+-rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.88/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.920969 kmlb-0.0.88/kmlb/
+-rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.88/kmlb/__init__.py
+-rw-rw-rw-   0        0        0    37252 2023-04-26 00:13:57.000000 kmlb-0.0.88/kmlb/base.py
+-rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.88/kmlb/gis_basics.py
+-rw-rw-rw-   0        0        0     6919 2023-04-26 02:24:30.000000 kmlb-0.0.88/kmlb/shapes.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:31:30.953970 kmlb-0.0.88/kmlb.egg-info/
+-rw-rw-rw-   0        0        0    38527 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-26 02:31:30.000000 kmlb-0.0.88/kmlb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 02:31:30.954977 kmlb-0.0.88/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-26 02:27:06.000000 kmlb-0.0.88/setup.py
```

### Comparing `kmlb-0.0.87/LICENSE.md` & `kmlb-0.0.88/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.87/PKG-INFO` & `kmlb-0.0.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.87
+Version: 0.0.88
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -670,15 +670,15 @@
 placemark = kmlb.polygon(coords, name, attribute_titles, attributes, style_to_use='Purple Polygon')
 ```
 
 ## Folder Function
 
 ### Create a Folder
 
-Create a folder to hold loose KLM geometry elements or other folders.
+Create a folder to hold loose KML geometry elements or other folders.
 
 `folder()`
 
 ```python
 folder(name, loose_items, description='', collapsed=True, hidden=True)
 ```
```

### Comparing `kmlb-0.0.87/README.md` & `kmlb-0.0.88/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
 placemark = kmlb.polygon(coords, name, attribute_titles, attributes, style_to_use='Purple Polygon')
 ```
 
 ## Folder Function
 
 ### Create a Folder
 
-Create a folder to hold loose KLM geometry elements or other folders.
+Create a folder to hold loose KML geometry elements or other folders.
 
 `folder()`
 
 ```python
 folder(name, loose_items, description='', collapsed=True, hidden=True)
 ```
```

### Comparing `kmlb-0.0.87/kmlb/base.py` & `kmlb-0.0.88/kmlb/base.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.87/kmlb/gis_basics.py` & `kmlb-0.0.88/kmlb/gis_basics.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.87/kmlb.egg-info/PKG-INFO` & `kmlb-0.0.88/kmlb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.87
+Version: 0.0.88
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
@@ -670,15 +670,15 @@
 placemark = kmlb.polygon(coords, name, attribute_titles, attributes, style_to_use='Purple Polygon')
 ```
 
 ## Folder Function
 
 ### Create a Folder
 
-Create a folder to hold loose KLM geometry elements or other folders.
+Create a folder to hold loose KML geometry elements or other folders.
 
 `folder()`
 
 ```python
 folder(name, loose_items, description='', collapsed=True, hidden=True)
 ```
```

### Comparing `kmlb-0.0.87/setup.py` & `kmlb-0.0.88/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmlb",
-    version="0.0.87",
+    version="0.0.88",
     author="HFM3",
     description="A Straightforward Google Earth KML Builder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HFM3/kmlb",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "images", "art"]),
     classifiers=[
```

