# Comparing `tmp/crosscompute-views-map-0.1.5.tar.gz` & `tmp/crosscompute-views-map-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-views-map-0.1.5.tar", last modified: Sat Feb 18 04:58:07 2023, max compression
+gzip compressed data, was "crosscompute-views-map-0.2.0.tar", last modified: Tue Apr 25 22:54:45 2023, max compression
```

## Comparing `crosscompute-views-map-0.1.5.tar` & `crosscompute-views-map-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 04:58:07.190754 crosscompute-views-map-0.1.5/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-08-23 20:11:01.000000 crosscompute-views-map-0.1.5/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2147 2023-02-18 04:58:07.190754 crosscompute-views-map-0.1.5/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1183 2022-08-23 20:11:01.000000 crosscompute-views-map-0.1.5/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 04:58:07.186754 crosscompute-views-map-0.1.5/crosscompute_views_map/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/__init__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 04:58:07.189754 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      221 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/deck-screengrid-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1417 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/deck-screengrid-output-variable.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      801 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      772 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-location-input-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      363 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-location-input-variable.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      114 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-location-input.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      322 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-output-header.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      607 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-output-variable.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      126 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      415 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/constants.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 04:58:07.189754 crosscompute-views-map-0.1.5/crosscompute_views_map/routines/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      138 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     8482 2023-02-18 04:54:49.000000 crosscompute-views-map-0.1.5/crosscompute_views_map/routines/variable.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 04:58:07.187754 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2147 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1068 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      259 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       41 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       23 2023-02-18 04:58:07.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-23 22:59:08.000000 crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1489 2023-02-18 04:58:07.190754 crosscompute-views-map-0.1.5/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-23 20:11:01.000000 crosscompute-views-map-0.1.5/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2023-04-25 22:39:14.000000 crosscompute-views-map-0.2.0/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1187 2023-04-25 22:39:54.000000 crosscompute-views-map-0.2.0/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.746627 crosscompute-views-map-0.2.0/crosscompute_views_map/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/__init__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.750627 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      221 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1417 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       47 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/map.css
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      801 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      772 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      114 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      363 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      322 2023-02-18 04:54:49.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output-header.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      607 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      131 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      468 2023-04-01 12:03:40.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/constants.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.751627 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1012 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     7769 2023-04-25 16:46:28.000000 crosscompute-views-map-0.2.0/crosscompute_views_map/routines/variable.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:54:45.748627 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2151 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1079 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      259 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       41 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       23 2023-04-25 22:54:45.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-08-23 22:59:08.000000 crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1503 2023-04-25 22:54:45.753627 crosscompute-views-map-0.2.0/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-08-23 20:11:01.000000 crosscompute-views-map-0.2.0/setup.py
```

### Comparing `crosscompute-views-map-0.1.5/LICENSE.md` & `crosscompute-views-map-0.2.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 CrossCompute Inc.
+Copyright 2023 CrossCompute Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `crosscompute-views-map-0.1.5/PKG-INFO` & `crosscompute-views-map-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-map
-Version: 0.1.5
+Version: 0.2.0
 Summary: Render maps in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-map/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-map
@@ -58,16 +58,16 @@
 
 ```
 $ pip install crosscompute-views-map
 ERROR: Could not find a version that satisfies the requirement crosscompute-views-map (from versions: none)
 ERROR: No matching distribution found for crosscompute-views-map
 ```
 
-To solve this issue, create a virtual environment using python >= 3.9.
+To solve this issue, create a virtual environment using python >= 3.10.
 
 ```
-sudo dnf -y install python3.9
-# sudo apt -y install python3.9
-python3.9 -m venv ~/.virtualenvs/crosscompute
+sudo dnf -y install python3.10
+# sudo apt -y install python3.10
+python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 pip install crosscompute-views-map
 ```
```

### Comparing `crosscompute-views-map-0.1.5/README.md` & `crosscompute-views-map-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 ```
 $ pip install crosscompute-views-map
 ERROR: Could not find a version that satisfies the requirement crosscompute-views-map (from versions: none)
 ERROR: No matching distribution found for crosscompute-views-map
 ```
 
-To solve this issue, create a virtual environment using python >= 3.9.
+To solve this issue, create a virtual environment using python >= 3.10.
 
 ```
-sudo dnf -y install python3.9
-# sudo apt -y install python3.9
-python3.9 -m venv ~/.virtualenvs/crosscompute
+sudo dnf -y install python3.10
+# sudo apt -y install python3.10
+python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 pip install crosscompute-views-map
 ```
```

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map/assets/deck-screengrid-output-variable.js` & `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/deck-screengrid-output.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-header.js` & `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-header.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-location-input-header.js` & `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-location-input-header.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,20 +18,20 @@
         value: {
             bounds: [_sw.lng, _sw.lat, _ne.lng, _ne.lat],
             center: [lng, lat],
             zoom
         },
     };
 };
-for (var e of document.getElementsByClassName('_{{ view_name }}-geolocate')) {
+for (var l of document.getElementsByClassName('_{{ view_name }}-geolocate')) {
     if (isSecure) {
-        e.onclick = function() {
+        l.onclick = function() {
             const {
                 element: elementId
-            } = e.dataset;
+            } = l.dataset;
             MAP_BY_ELEMENT_ID[elementId].controlByName.geolocate.trigger();
         }
     } else {
-        e.disabled = true;
-        e.innerHTML = 'Geolocation is disabled because connection is not secure';
+        l.disabled = true;
+        l.innerHTML = 'Geolocation is disabled because connection is not secure';
     }
 }
```

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map/assets/mapbox-output-variable.js` & `crosscompute-views-map-0.2.0/crosscompute_views_map/assets/mapbox-output.js`

 * *Files identical despite different names*

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map/routines/variable.py` & `crosscompute-views-map-0.2.0/crosscompute_views_map/routines/variable.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,41 @@
 import json
 from os import environ
 
 import geojson
 import numpy as np
 from crosscompute.routines.interface import Batch
 from crosscompute.routines.variable import (
-    Element, VariableView, add_label_html)
+    Element, VariableView)
 
 from ..constants import (
     DECK_JS_URI,
     MAPBOX_CSS_URI,
     MAPBOX_JS_URI,
+    MAPBOX_STYLE_URI,
     TURF_JS_URI)
-from .asset import asset_storage
+from .asset import (
+    MAP_CSS,
+    MAP_DECK_SCREENGRID_OUTPUT_HEADER_JS,
+    MAP_DECK_SCREENGRID_OUTPUT_JS,
+    MAP_MAPBOX_HEADER_JS,
+    MAP_MAPBOX_HTML,
+    MAP_MAPBOX_LOCATION_INPUT_HEADER_JS,
+    MAP_MAPBOX_LOCATION_INPUT_HTML,
+    MAP_MAPBOX_LOCATION_INPUT_JS,
+    MAP_MAPBOX_OUTPUT_HEADER_JS,
+    MAP_MAPBOX_OUTPUT_JS)
 
 
 class MapMapboxView(VariableView):
 
     view_name = 'map-mapbox'
     environment_variable_definitions = [{'id': 'MAPBOX_TOKEN'}]
     css_uris = [MAPBOX_CSS_URI]
+    css_texts = [MAP_CSS]
     js_uris = [MAPBOX_JS_URI, TURF_JS_URI]
 
     def process(self, path):
         with path.open('rt') as f:
             array = np.array(list(geojson.utils.coords(json.load(f))))
         save_map_configuration(array, path)
 
@@ -36,34 +48,36 @@
         data_uri = b.get_data_uri(variable_definition, x)
         c = b.get_variable_configuration(variable_definition)
         main_text = get_map_html(
             element_id, variable_id, c, x.mode_name, self.view_name,
             x.design_name)
         js_texts = [
             "mapboxgl.accessToken = '%s';" % environ['MAPBOX_TOKEN'],
-            MAP_MAPBOX_JS_HEADER,
-            MAP_MAPBOX_OUTPUT_JS_HEADER,
-            MAP_MAPBOX_OUTPUT_JS_VARIABLE.render({
+            MAP_MAPBOX_HEADER_JS,
+            MAP_MAPBOX_OUTPUT_HEADER_JS,
+            MAP_MAPBOX_OUTPUT_JS.render({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri,
                 'bounds': c.get('bounds'),
                 'map': get_map_definition(element_id, c, x.for_print),
                 'sources': get_source_definitions(element_id, c, data_uri),
                 'layers': get_layer_definitions(element_id, c)})]
         return {
-            'css_uris': self.css_uris, 'js_uris': self.js_uris,
-            'main_text': main_text, 'js_texts': js_texts}
+            'css_uris': self.css_uris, 'css_texts': self.css_texts,
+            'js_uris': self.js_uris, 'js_texts': js_texts,
+            'main_text': main_text}
 
 
 class MapMapboxLocationView(VariableView):
 
     view_name = 'map-mapbox-location'
     environment_variable_definitions = [{'id': 'MAPBOX_TOKEN'}]
     css_uris = [MAPBOX_CSS_URI]
+    css_texts = [MAP_CSS]
     js_uris = [MAPBOX_JS_URI]
 
     def render_input(self, b: Batch, x: Element):
         variable_definition = self.variable_definition
         element_id = x.id
         view_name = self.view_name
         c = b.get_variable_configuration(variable_definition)
@@ -79,31 +93,32 @@
             c['zoom'] = zoom
         main_text = get_map_html(
             element_id, self.variable_id, c, x.mode_name, view_name,
             x.design_name, MAP_MAPBOX_LOCATION_INPUT_HTML.render({
                 'view_name': view_name, 'element_id': element_id}))
         js_texts = [
             "mapboxgl.accessToken = '%s';" % environ['MAPBOX_TOKEN'],
-            MAP_MAPBOX_JS_HEADER,
-            MAP_MAPBOX_LOCATION_INPUT_JS_HEADER.render({
+            MAP_MAPBOX_HEADER_JS,
+            MAP_MAPBOX_LOCATION_INPUT_HEADER_JS.render({
                 'view_name': view_name}),
-            MAP_MAPBOX_LOCATION_INPUT_JS_VARIABLE.render({
+            MAP_MAPBOX_LOCATION_INPUT_JS.render({
                 'element_id': element_id,
-                'map': get_map_definition(element_id, c, x.for_print)}),
-        ]
+                'map': get_map_definition(element_id, c, x.for_print)})]
         return {
-            'css_uris': self.css_uris, 'js_uris': self.js_uris,
-            'main_text': main_text, 'js_texts': js_texts}
+            'css_uris': self.css_uris, 'css_texts': self.css_texts,
+            'js_uris': self.js_uris, 'js_texts': js_texts,
+            'main_text': main_text}
 
 
 class MapDeckScreenGridView(VariableView):
 
     view_name = 'map-deck-screengrid'
     environment_variable_definitions = [{'id': 'MAPBOX_TOKEN'}]
     css_uris = [MAPBOX_CSS_URI]
+    css_texts = [MAP_CSS]
     js_uris = [MAPBOX_JS_URI, DECK_JS_URI]
 
     def process(self, path):
         with path.open('rt') as f:
             array = np.array(json.load(f))
         save_map_configuration(array, path)
 
@@ -115,48 +130,42 @@
         c = b.get_variable_configuration(variable_definition)
         mapbox_token = environ['MAPBOX_TOKEN']
         main_text = get_map_html(
             element_id, variable_id, c, x.mode_name, self.view_name,
             x.design_name)
         js_texts = [
             f"mapboxgl.accessToken = '{mapbox_token}';",
-            MAP_DECK_SCREENGRID_OUTPUT_JS_HEADER,
-            MAP_DECK_SCREENGRID_OUTPUT_JS_VARIABLE.render({
+            MAP_DECK_SCREENGRID_OUTPUT_HEADER_JS,
+            MAP_DECK_SCREENGRID_OUTPUT_JS.render({
                 'variable_id': variable_id,
                 'element_id': element_id,
                 'data_uri': data_uri,
                 'opacity': c.get('opacity', 0.5),
                 'get_position_definition_string': c.get('position', 'd => d'),
                 'get_weight_definition_string': c.get('weight', 1),
-                'style_uri': c.get('style', MAP_MAPBOX_STYLE_URI),
+                'style_uri': c.get('style', MAPBOX_STYLE_URI),
                 'bounds': c.get('bounds'),
                 'longitude': c.get('longitude', 0),
                 'latitude': c.get('latitude', 0),
                 'zoom': c.get('zoom', 0),
                 'for_print': x.for_print})]
         return {
-            'css_uris': self.css_uris, 'js_uris': self.js_uris,
-            'main_text': main_text, 'js_texts': js_texts}
+            'css_uris': self.css_uris, 'css_texts': self.css_texts,
+            'js_uris': self.js_uris, 'js_texts': js_texts,
+            'main_text': main_text}
 
 
 def save_map_configuration(xy_array, source_path):
     try:
         xs = xy_array[:, 0]
         ys = xy_array[:, 1]
     except IndexError:
-        d = {
-            'longitude': 0,
-            'latitude': 0,
-            'zoom': 0,
-        }
+        d = {'longitude': 0, 'latitude': 0, 'zoom': 0}
     else:
-        d = {
-            'longitude': xs.mean(),
-            'latitude': ys.mean(),
-        }
+        d = {'longitude': xs.mean(), 'latitude': ys.mean()}
         if len(xs) == 1:
             d['zoom'] = 15
         else:
             d['bounds'] = xs.min(), ys.min(), xs.max(), ys.max()
     with open(str(source_path) + '.configuration', 'wt') as f:
         json.dump(d, f)
 
@@ -164,75 +173,44 @@
 def get_map_html(
         element_id, variable_id, variable_configuration, mode_name, view_name,
         design_name, prefix_html=''):
     main_text = prefix_html + MAP_MAPBOX_HTML.substitute({
         'element_id': element_id,
         'mode_name': mode_name,
         'view_name': view_name,
-        'variable_id': variable_id,
-    })
-    if design_name not in ['none']:
-        main_text = add_label_html(
-            main_text, variable_configuration, variable_id, element_id)
+        'variable_id': variable_id})
     return main_text
 
 
 def get_map_definition(element_id, variable_configuration, for_print):
-    style_uri = variable_configuration.get('style', MAP_MAPBOX_STYLE_URI)
+    style_uri = variable_configuration.get('style', MAPBOX_STYLE_URI)
     longitude = variable_configuration.get('longitude', 0)
     latitude = variable_configuration.get('latitude', 0)
     zoom = variable_configuration.get('zoom', 0)
     d = {
         'container': element_id,
         'style': style_uri,
         'center': [longitude, latitude],
-        'zoom': zoom,
-    }
+        'zoom': zoom}
     if for_print:
         d['preserveDrawingBuffer'] = 1
     return d
 
 
 def get_source_definitions(element_id, variable_configuration, data_uri):
     return variable_configuration.get('sources', [{
         'id': element_id,
         'type': 'geojson',
-        'data': data_uri,
-    }])
+        'data': data_uri}])
 
 
 def get_layer_definitions(element_id, variable_configuration):
     definitions = []
     for index, d in enumerate(variable_configuration.get('layers', [{
         'type': 'circle',
     }])):
         if 'id' not in d:
             d['id'] = element_id
         if 'source' not in d:
             d['source'] = element_id
         definitions.append(d)
     return definitions
-
-
-MAP_MAPBOX_STYLE_URI = 'mapbox://styles/mapbox/dark-v10'
-
-
-MAP_MAPBOX_HTML = asset_storage.load_string_text('mapbox.html')
-MAP_MAPBOX_JS_HEADER = asset_storage.load_raw_text('mapbox-header.js')
-MAP_MAPBOX_OUTPUT_JS_HEADER = asset_storage.load_raw_text(
-    'mapbox-output-header.js')
-MAP_MAPBOX_OUTPUT_JS_VARIABLE = asset_storage.load_jinja_text(
-    'mapbox-output-variable.js')
-
-
-MAP_MAPBOX_LOCATION_INPUT_HTML = asset_storage.load_jinja_text(
-    'mapbox-location-input.html')
-MAP_MAPBOX_LOCATION_INPUT_JS_HEADER = asset_storage.load_jinja_text(
-    'mapbox-location-input-header.js')
-MAP_MAPBOX_LOCATION_INPUT_JS_VARIABLE = asset_storage.load_jinja_text(
-    'mapbox-location-input-variable.js')
-
-
-MAP_DECK_SCREENGRID_OUTPUT_JS_HEADER = asset_storage.load_raw_text(
-    'deck-screengrid-output-header.js')
-MAP_DECK_SCREENGRID_OUTPUT_JS_VARIABLE = asset_storage.load_jinja_text(
-    'deck-screengrid-output-variable.js')
```

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/PKG-INFO` & `crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-map
-Version: 0.1.5
+Version: 0.2.0
 Summary: Render maps in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-map/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-map
@@ -58,16 +58,16 @@
 
 ```
 $ pip install crosscompute-views-map
 ERROR: Could not find a version that satisfies the requirement crosscompute-views-map (from versions: none)
 ERROR: No matching distribution found for crosscompute-views-map
 ```
 
-To solve this issue, create a virtual environment using python >= 3.9.
+To solve this issue, create a virtual environment using python >= 3.10.
 
 ```
-sudo dnf -y install python3.9
-# sudo apt -y install python3.9
-python3.9 -m venv ~/.virtualenvs/crosscompute
+sudo dnf -y install python3.10
+# sudo apt -y install python3.10
+python3.10 -m venv ~/.virtualenvs/crosscompute
 source ~/.virtualenvs/crosscompute/bin/activate
 pip install crosscompute-views-map
 ```
```

### Comparing `crosscompute-views-map-0.1.5/crosscompute_views_map.egg-info/SOURCES.txt` & `crosscompute-views-map-0.2.0/crosscompute_views_map.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 crosscompute_views_map.egg-info/SOURCES.txt
 crosscompute_views_map.egg-info/dependency_links.txt
 crosscompute_views_map.egg-info/entry_points.txt
 crosscompute_views_map.egg-info/requires.txt
 crosscompute_views_map.egg-info/top_level.txt
 crosscompute_views_map.egg-info/zip-safe
 crosscompute_views_map/assets/deck-screengrid-output-header.js
-crosscompute_views_map/assets/deck-screengrid-output-variable.js
+crosscompute_views_map/assets/deck-screengrid-output.js
+crosscompute_views_map/assets/map.css
 crosscompute_views_map/assets/mapbox-header.js
 crosscompute_views_map/assets/mapbox-location-input-header.js
-crosscompute_views_map/assets/mapbox-location-input-variable.js
 crosscompute_views_map/assets/mapbox-location-input.html
+crosscompute_views_map/assets/mapbox-location-input.js
 crosscompute_views_map/assets/mapbox-output-header.js
-crosscompute_views_map/assets/mapbox-output-variable.js
+crosscompute_views_map/assets/mapbox-output.js
 crosscompute_views_map/assets/mapbox.html
 crosscompute_views_map/routines/__init__.py
 crosscompute_views_map/routines/asset.py
 crosscompute_views_map/routines/variable.py
```

### Comparing `crosscompute-views-map-0.1.5/setup.cfg` & `crosscompute-views-map-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-views-map
-version = 0.1.5
+version = 0.2.0
 description = Render maps in your automations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -24,22 +24,23 @@
 	Documentation = https://github.com/crosscompute/crosscompute-views-map
 	Source Code = https://github.com/crosscompute/crosscompute-views-map
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
-	crosscompute>=0.9.3
+	crosscompute>=0.9.4
 	geojson
 	jinja2
 	numpy
 zip_safe = True
 
 [options.package_data]
 crosscompute_views_map = 
+	assets/*.css
 	assets/*.html
 	assets/*.js
 
 [options.entry_points]
 crosscompute.views = 
 	map-mapbox = crosscompute_views_map.routines.variable.MapMapboxView
 	map-mapbox-location = crosscompute_views_map.routines.variable.MapMapboxLocationView
```

