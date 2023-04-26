# Comparing `tmp/trame-leaflet-1.1.0.tar.gz` & `tmp/trame-leaflet-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-leaflet-1.1.0.tar", last modified: Thu Feb 23 16:47:29 2023, max compression
+gzip compressed data, was "trame-leaflet-1.1.1.tar", last modified: Tue Apr 25 16:19:44 2023, max compression
```

## Comparing `trame-leaflet-1.1.0.tar` & `trame-leaflet-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.059549 trame-leaflet-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1301 2023-02-23 16:47:29.059549 trame-leaflet-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      877 2023-02-23 16:47:29.059549 trame-leaflet-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame/modules/leaflet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame/widgets/leaflet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame_leaflet/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame_leaflet/LICENSE
--rw-r--r--   0 root         (0) root         (0)       95 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame_leaflet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame_leaflet/module/
--rw-r--r--   0 root         (0) root         (0)      433 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame_leaflet/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.059549 trame-leaflet-1.1.0/trame_leaflet/module/serve/
--rw-r--r--   0 root         (0) root         (0)      207 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)   717137 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.common.js
--rw-r--r--   0 root         (0) root         (0)   903405 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.common.js.map
--rw-r--r--   0 root         (0) root         (0)    15148 2023-02-23 16:47:24.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.css
--rw-r--r--   0 root         (0) root         (0)   717715 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.js
--rw-r--r--   0 root         (0) root         (0)   903996 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.js.map
--rw-r--r--   0 root         (0) root         (0)   255453 2023-02-23 16:47:24.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.min.js
--rw-r--r--   0 root         (0) root         (0)  1093905 2023-02-23 16:47:24.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.min.js.map
--rw-r--r--   0 root         (0) root         (0)     1259 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/tramelayers-2x.png
--rw-r--r--   0 root         (0) root         (0)      696 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/tramelayers.png
--rw-r--r--   0 root         (0) root         (0)     2464 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-icon-2x.png
--rw-r--r--   0 root         (0) root         (0)     1466 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-icon.png
--rw-r--r--   0 root         (0) root         (0)      618 2023-02-23 16:47:21.000000 trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-shadow.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.059549 trame-leaflet-1.1.0/trame_leaflet/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame_leaflet/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14584 2023-02-23 16:46:57.000000 trame-leaflet-1.1.0/trame_leaflet/widgets/leaflet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 16:47:29.051549 trame-leaflet-1.1.0/trame_leaflet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1301 2023-02-23 16:47:29.000000 trame-leaflet-1.1.0/trame_leaflet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1135 2023-02-23 16:47:29.000000 trame-leaflet-1.1.0/trame_leaflet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 16:47:29.000000 trame-leaflet-1.1.0/trame_leaflet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-23 16:47:29.000000 trame-leaflet-1.1.0/trame_leaflet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-23 16:47:29.000000 trame-leaflet-1.1.0/trame_leaflet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.029441 trame-leaflet-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-25 16:19:44.029441 trame-leaflet-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-25 16:19:44.029441 trame-leaflet-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame/modules/leaflet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame/widgets/leaflet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame_leaflet/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame_leaflet/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       95 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame_leaflet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame_leaflet/module/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame_leaflet/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.029441 trame-leaflet-1.1.1/trame_leaflet/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)   717137 2023-04-25 16:19:36.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.common.js
+-rw-r--r--   0 root         (0) root         (0)   903405 2023-04-25 16:19:36.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.common.js.map
+-rw-r--r--   0 root         (0) root         (0)    15148 2023-04-25 16:19:38.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.css
+-rw-r--r--   0 root         (0) root         (0)   717715 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.js
+-rw-r--r--   0 root         (0) root         (0)   903996 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)   255453 2023-04-25 16:19:38.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)  1093905 2023-04-25 16:19:38.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.min.js.map
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/tramelayers-2x.png
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/tramelayers.png
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-icon-2x.png
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-icon.png
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-25 16:19:35.000000 trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-shadow.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.029441 trame-leaflet-1.1.1/trame_leaflet/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame_leaflet/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15064 2023-04-25 16:19:11.000000 trame-leaflet-1.1.1/trame_leaflet/widgets/leaflet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:19:44.021441 trame-leaflet-1.1.1/trame_leaflet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-25 16:19:44.000000 trame-leaflet-1.1.1/trame_leaflet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-04-25 16:19:44.000000 trame-leaflet-1.1.1/trame_leaflet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:19:44.000000 trame-leaflet-1.1.1/trame_leaflet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 16:19:44.000000 trame-leaflet-1.1.1/trame_leaflet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 16:19:44.000000 trame-leaflet-1.1.1/trame_leaflet.egg-info/top_level.txt
```

### Comparing `trame-leaflet-1.1.0/LICENSE` & `trame-leaflet-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/PKG-INFO` & `trame-leaflet-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-leaflet
-Version: 1.1.0
+Version: 1.1.1
 Summary: Leaflet widget for trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-leaflet-1.1.0/README.rst` & `trame-leaflet-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/setup.cfg` & `trame-leaflet-1.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-leaflet
-version = 1.1.0
+version = 1.1.1
 description = Leaflet widget for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-leaflet-1.1.0/trame_leaflet/LICENSE` & `trame-leaflet-1.1.1/trame_leaflet/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.common.js` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.common.js`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.common.js.map` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.common.js.map`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.css` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.css`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.js` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.js`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.js.map` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.js.map`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.min.js` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.min.js`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/trame-leaflet.umd.min.js.map` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/trame-leaflet.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/tramelayers-2x.png` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/tramelayers-2x.png`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/tramelayers.png` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/tramelayers.png`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-icon-2x.png` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-icon.png` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-icon.png`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/module/serve/tramemarker-shadow.png` & `trame-leaflet-1.1.1/trame_leaflet/module/serve/tramemarker-shadow.png`

 * *Files identical despite different names*

### Comparing `trame-leaflet-1.1.0/trame_leaflet/widgets/leaflet.py` & `trame-leaflet-1.1.1/trame_leaflet/widgets/leaflet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,38 @@
+"""Leaflet Widgets only support vue2 for now.
+"""
 from trame_client.widgets.core import AbstractElement
 from .. import module
 
+__all__ = [
+    "LCircle",
+    "LCircleMarker",
+    "LControl",
+    "LControlAttribution",
+    "LControlLayers",
+    "LControlScale",
+    "LControlZoom",
+    "LFeatureGroup",
+    "LGeoJson",
+    "LGridLayer",
+    "LIcon",
+    "LImageOverlay",
+    "LLayerGroup",
+    "LMap",
+    "LMarker",
+    "LPolygon",
+    "LPolyline",
+    "LPopup",
+    "LRectangle",
+    "LTileLayer",
+    "LTooltip",
+    "LWMSTileLayer",
+    "VGeosearch",
+]
+
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
```

### Comparing `trame-leaflet-1.1.0/trame_leaflet.egg-info/PKG-INFO` & `trame-leaflet-1.1.1/trame_leaflet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-leaflet
-Version: 1.1.0
+Version: 1.1.1
 Summary: Leaflet widget for trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-leaflet-1.1.0/trame_leaflet.egg-info/SOURCES.txt` & `trame-leaflet-1.1.1/trame_leaflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

