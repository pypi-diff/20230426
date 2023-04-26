# Comparing `tmp/crosscompute-views-barcode-0.1.0.tar.gz` & `tmp/crosscompute-views-barcode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-views-barcode-0.1.0.tar", last modified: Sat Feb 18 05:00:56 2023, max compression
+gzip compressed data, was "crosscompute-views-barcode-0.2.0.tar", last modified: Tue Apr 25 22:57:56 2023, max compression
```

## Comparing `crosscompute-views-barcode-0.1.0.tar` & `crosscompute-views-barcode-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 05:00:56.903013 crosscompute-views-barcode-0.1.0/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.1.0/LICENSE.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1604 2023-02-18 05:00:56.903013 crosscompute-views-barcode-0.1.0/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      622 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.1.0/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 05:00:56.901013 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/__init__.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 05:00:56.902013 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/assets/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      111 2023-02-17 07:43:23.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/assets/barcode.html
--rw-r--r--   0 rhh       (1000) rhh       (1000)      448 2023-02-17 07:43:23.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/assets/barcode.js
--rw-r--r--   0 rhh       (1000) rhh       (1000)      270 2023-02-17 07:43:23.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/constants.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 05:00:56.903013 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/routines/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/routines/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      151 2023-02-08 16:43:09.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/routines/asset.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1554 2023-02-08 16:43:09.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/routines/variable.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-02-18 05:00:56.902013 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1604 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      698 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       88 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/entry_points.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       20 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       27 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1314 2023-02-18 05:00:56.904013 crosscompute-views-barcode-0.1.0/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.1.0/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:57:56.172023 crosscompute-views-barcode-0.2.0/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1057 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.2.0/LICENSE.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1604 2023-04-25 22:57:56.172023 crosscompute-views-barcode-0.2.0/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      622 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.2.0/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:57:56.169023 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/__init__.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:57:56.171023 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/assets/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      448 2023-04-25 16:48:06.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/assets/barcode-output.js
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      111 2023-02-17 07:43:23.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/assets/barcode.html
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      270 2023-04-25 19:51:53.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/constants.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:57:56.172023 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/routines/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/routines/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      294 2023-04-25 16:48:06.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/routines/asset.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1422 2023-04-05 02:03:29.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/routines/variable.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-04-25 22:57:56.171023 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1604 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      705 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       88 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/entry_points.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       20 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       27 2023-04-25 22:57:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-02-18 05:00:56.000000 crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1314 2023-04-25 22:57:56.173023 crosscompute-views-barcode-0.2.0/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2022-12-16 03:52:20.000000 crosscompute-views-barcode-0.2.0/setup.py
```

### Comparing `crosscompute-views-barcode-0.1.0/LICENSE.md` & `crosscompute-views-barcode-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crosscompute-views-barcode-0.1.0/PKG-INFO` & `crosscompute-views-barcode-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-barcode
-Version: 0.1.0
+Version: 0.2.0
 Summary: Scan barcodes in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-barcode/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-barcode
```

### Comparing `crosscompute-views-barcode-0.1.0/README.md` & `crosscompute-views-barcode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-views-barcode-0.1.0/crosscompute_views_barcode/routines/variable.py` & `crosscompute-views-barcode-0.2.0/crosscompute_views_barcode/routines/variable.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,25 @@
     VariableView)
 
 from ..constants import (
     BARCODE_JS_URI,
     FRAMES_PER_SECOND,
     SCANNER_HEIGHT_IN_PIXELS,
     SCANNER_WIDTH_IN_PIXELS)
-from .asset import asset_storage
+from .asset import (
+    BARCODE_OUTPUT_HTML,
+    BARCODE_OUTPUT_JS)
 
 
 class BarcodeView(VariableView):
 
     def render_output(self, b: Batch, x: Element):
         element_id = x.id
         variable_id = self.variable_id
         variable_definition = self.variable_definition
-        # data = b.get_data(variable_definition)
         c = b.get_variable_configuration(variable_definition)
         main_text = BARCODE_OUTPUT_HTML.substitute({
             'element_id': element_id,
             'mode_name': x.mode_name,
             'view_name': self.view_name,
             'variable_id': variable_id})
         js_texts = [
@@ -31,13 +32,9 @@
                 'frames_per_second': c.get(
                     'frames-per-second', FRAMES_PER_SECOND),
                 'scanner_width_in_pixels': c.get(
                     'scanner-width-in-pixels', SCANNER_WIDTH_IN_PIXELS),
                 'scanner_height_in_pixels': c.get(
                     'scanner-height-in-pixels', SCANNER_HEIGHT_IN_PIXELS)})]
         return {
-            'css_uris': [], 'js_uris': [BARCODE_JS_URI],
-            'main_text': main_text, 'js_texts': js_texts}
-
-
-BARCODE_OUTPUT_HTML = asset_storage.load_string_text('barcode.html')
-BARCODE_OUTPUT_JS = asset_storage.load_string_text('barcode.js')
+            'css_uris': [], 'css_texts': [], 'js_uris': [BARCODE_JS_URI],
+            'js_texts': js_texts, 'main_text': main_text}
```

### Comparing `crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/PKG-INFO` & `crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-views-barcode
-Version: 0.1.0
+Version: 0.2.0
 Summary: Scan barcodes in your automations.
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-views-barcode/issues
 Project-URL: Documentation, https://github.com/crosscompute/crosscompute-views-barcode
```

### Comparing `crosscompute-views-barcode-0.1.0/crosscompute_views_barcode.egg-info/SOURCES.txt` & `crosscompute-views-barcode-0.2.0/crosscompute_views_barcode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 crosscompute_views_barcode.egg-info/PKG-INFO
 crosscompute_views_barcode.egg-info/SOURCES.txt
 crosscompute_views_barcode.egg-info/dependency_links.txt
 crosscompute_views_barcode.egg-info/entry_points.txt
 crosscompute_views_barcode.egg-info/requires.txt
 crosscompute_views_barcode.egg-info/top_level.txt
 crosscompute_views_barcode.egg-info/zip-safe
+crosscompute_views_barcode/assets/barcode-output.js
 crosscompute_views_barcode/assets/barcode.html
-crosscompute_views_barcode/assets/barcode.js
 crosscompute_views_barcode/routines/__init__.py
 crosscompute_views_barcode/routines/asset.py
 crosscompute_views_barcode/routines/variable.py
```

### Comparing `crosscompute-views-barcode-0.1.0/setup.cfg` & `crosscompute-views-barcode-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-views-barcode
-version = 0.1.0
+version = 0.2.0
 description = Scan barcodes in your automations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -24,15 +24,15 @@
 	Documentation = https://github.com/crosscompute/crosscompute-views-barcode
 	Source Code = https://github.com/crosscompute/crosscompute-views-barcode
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
-	crosscompute>=0.9.3
+	crosscompute>=0.9.4
 zip_safe = True
 
 [options.package_data]
 crosscompute_views_barcode = 
 	assets/*.html
 	assets/*.js
```

