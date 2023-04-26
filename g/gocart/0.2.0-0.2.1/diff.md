# Comparing `tmp/gocart-0.2.0.tar.gz` & `tmp/gocart-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.2.0.tar", last modified: Wed Apr 26 14:26:01 2023, max compression
+gzip compressed data, was "gocart-0.2.1.tar", last modified: Wed Apr 26 18:36:08 2023, max compression
```

## Comparing `gocart-0.2.0.tar` & `gocart-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1454 2023-04-26 14:21:44.000000 gocart-0.2.0/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-26 14:21:44.000000 gocart-0.2.0/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-26 14:21:44.000000 gocart-0.2.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 14:26:01.174921 gocart-0.2.0/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-26 14:21:44.000000 gocart-0.2.0/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8322 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12416 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12929 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/parsers/lvk.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      748 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 14:25:03.000000 gocart-0.2.0/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-26 14:26:01.174921 gocart-0.2.0/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-26 14:21:44.000000 gocart-0.2.0/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1545 2023-04-26 18:31:54.000000 gocart-0.2.1/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-26 18:31:54.000000 gocart-0.2.1/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-26 18:31:54.000000 gocart-0.2.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 18:36:08.053192 gocart-0.2.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-26 18:31:54.000000 gocart-0.2.1/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8322 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12416 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13302 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/parsers/lvk.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      748 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 18:35:09.000000 gocart-0.2.1/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-26 18:36:08.053192 gocart-0.2.1/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-26 18:31:54.000000 gocart-0.2.1/setup.py
```

### Comparing `gocart-0.2.0/CHANGES.md` & `gocart-0.2.1/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v0.2.1 - April 26, 2023**  
+
+- **FIXED**: listen command was tripping up on mock-events
+
 **v0.2.0 - April 26, 2023**  
 
 - **FEATURE**: filtering of alerts is now possible via options in the settings file (see docs)  
 - **ENHANCEMENT**: option added to write the original json alert to file  
 - **ENHANCEMENT**: gocart *should* be robust enough to handle burst events (tested against a hand crafted burst alert packet as none exist in the LVK Public Alert Guide yet).  
 
 **v0.1.10 - April 21, 2023**
```

### Comparing `gocart-0.2.0/LICENSE` & `gocart-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/PKG-INFO` & `gocart-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.2.0
+Version: 0.2.1
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.0.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.1.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.2.0/README.md` & `gocart-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/advanced_settings.yaml` & `gocart-0.2.1/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/cl_utils.py` & `gocart-0.2.1/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.2.1/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.2.1/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/convert/aitoff.py` & `gocart-0.2.1/gocart/convert/aitoff.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/convert/ascii.py` & `gocart-0.2.1/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/convert/healpix2cart.py` & `gocart-0.2.1/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/default_settings.yaml` & `gocart-0.2.1/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/parsers/lvk.py` & `gocart-0.2.1/gocart/parsers/lvk.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,22 @@
         import astropy_healpix as ah
         import numpy as np
         from astropy.time import Time
         from datetime import datetime
         import yaml
         import json
 
+        # WHICH EVENTS ARE WE TO PARSE?
+        parse_mock_events = self.settings["lvk"]["parse_mock_events"]
+        parse_real_events = self.settings["lvk"]["parse_real_events"]
+        if self.record['superevent_id'][0] == 'M' and not parse_mock_events:
+            return
+        if self.record['superevent_id'][0] != 'M' and not parse_real_events:
+            return
+
         print("\n----------------------------------------")
         if "event" in self.record and self.record["event"]:
             timeDelta = (Time(self.record["time_created"], scale='utc') - Time(self.record["event"]["time"], scale='utc')).to_value(unit='min')
             far = 1 / (float(self.record['event']['far']) * 60. * 60. * 24.)
             if far > 1000:
                 far /= 365.
                 far = f"1 per {far:0.1f} yrs"
```

### Comparing `gocart-0.2.0/gocart/setup.cfg` & `gocart-0.2.1/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/test_settings.yaml` & `gocart-0.2.1/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart/utKit.py` & `gocart-0.2.1/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/gocart.egg-info/PKG-INFO` & `gocart-0.2.1/gocart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.2.0
+Version: 0.2.1
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.0.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.1.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.2.0/gocart.egg-info/SOURCES.txt` & `gocart-0.2.1/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.2.0/setup.py` & `gocart-0.2.1/setup.py`

 * *Files identical despite different names*

