# Comparing `tmp/sdss_cherno-0.5.2.tar.gz` & `tmp/sdss_cherno-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.5.2.tar", max compression
+gzip compressed data, was "sdss_cherno-0.6.0.tar", max compression
```

## Comparing `sdss_cherno-0.5.2.tar` & `sdss_cherno-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0     1504 2023-01-15 17:37:44.377105 sdss_cherno-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     2714 2023-01-15 17:37:44.377584 sdss_cherno-0.5.2/README.md
--rw-r--r--   0        0        0     1251 2023-01-15 17:37:44.378020 sdss_cherno-0.5.2/cherno/__init__.py
--rw-r--r--   0        0        0     2207 2023-01-15 17:37:44.378390 sdss_cherno-0.5.2/cherno/__main__.py
--rw-r--r--   0        0        0      747 2023-01-15 17:37:44.378855 sdss_cherno-0.5.2/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4493 2023-01-15 17:37:44.379262 sdss_cherno-0.5.2/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2023-01-15 17:37:44.379486 sdss_cherno-0.5.2/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2023-01-15 17:37:44.379921 sdss_cherno-0.5.2/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2023-01-15 17:37:44.380322 sdss_cherno-0.5.2/cherno/actor/commands/config.py
--rw-r--r--   0        0        0     8099 2023-01-15 17:37:44.380742 sdss_cherno-0.5.2/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2023-01-15 17:37:44.381155 sdss_cherno-0.5.2/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1007 2023-01-15 17:37:44.381535 sdss_cherno-0.5.2/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2023-01-15 17:37:44.381915 sdss_cherno-0.5.2/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3119 2023-01-15 17:37:44.382320 sdss_cherno-0.5.2/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2023-01-15 17:37:44.382679 sdss_cherno-0.5.2/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2023-01-15 17:37:44.383082 sdss_cherno-0.5.2/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2023-01-15 17:37:44.383486 sdss_cherno-0.5.2/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2023-01-15 17:37:44.383877 sdss_cherno-0.5.2/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10862 2023-01-15 17:37:44.384240 sdss_cherno-0.5.2/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2023-01-15 17:37:44.384620 sdss_cherno-0.5.2/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2023-01-15 17:37:44.384930 sdss_cherno-0.5.2/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     1940 2023-01-15 17:37:44.385267 sdss_cherno-0.5.2/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     1929 2023-01-15 17:37:44.385587 sdss_cherno-0.5.2/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     4906 2023-01-15 17:37:44.385899 sdss_cherno-0.5.2/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2023-01-15 17:37:44.386311 sdss_cherno-0.5.2/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2023-01-15 17:37:44.386746 sdss_cherno-0.5.2/cherno/extraction.py
--rw-r--r--   0        0        0    36868 2023-01-15 17:37:44.387274 sdss_cherno-0.5.2/cherno/guider.py
--rw-r--r--   0        0        0     4105 2023-01-15 17:37:44.387669 sdss_cherno-0.5.2/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2023-01-15 17:37:44.388017 sdss_cherno-0.5.2/cherno/maskbits.py
--rw-r--r--   0        0        0     4649 2023-01-15 17:37:44.388379 sdss_cherno-0.5.2/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2023-01-15 17:37:44.388748 sdss_cherno-0.5.2/cherno/utils.py
--rw-r--r--   0        0        0     2335 2023-01-15 17:37:44.396969 sdss_cherno-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 sdss_cherno-0.5.2/setup.py
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 sdss_cherno-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-25 16:03:17.263097 sdss_cherno-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     2714 2023-04-25 16:03:17.263503 sdss_cherno-0.6.0/README.md
+-rw-r--r--   0        0        0     1251 2023-04-25 16:03:17.263912 sdss_cherno-0.6.0/cherno/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-25 16:03:17.264935 sdss_cherno-0.6.0/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2023-04-25 16:03:17.265416 sdss_cherno-0.6.0/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     4493 2023-04-25 16:03:17.267569 sdss_cherno-0.6.0/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:03:17.268005 sdss_cherno-0.6.0/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-25 16:03:17.269274 sdss_cherno-0.6.0/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2023-04-25 16:03:17.269777 sdss_cherno-0.6.0/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0     8213 2023-04-25 16:03:17.270233 sdss_cherno-0.6.0/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2023-04-25 16:03:17.270821 sdss_cherno-0.6.0/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1007 2023-04-25 16:03:17.271351 sdss_cherno-0.6.0/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2023-04-25 16:03:17.271808 sdss_cherno-0.6.0/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3119 2023-04-25 16:03:17.272781 sdss_cherno-0.6.0/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2023-04-25 16:03:17.273181 sdss_cherno-0.6.0/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2023-04-25 16:03:17.273587 sdss_cherno-0.6.0/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2023-04-25 16:03:17.274051 sdss_cherno-0.6.0/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2023-04-25 16:03:17.274411 sdss_cherno-0.6.0/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10857 2023-04-25 16:03:17.274768 sdss_cherno-0.6.0/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2023-04-25 16:03:17.275193 sdss_cherno-0.6.0/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2023-04-25 16:03:17.275770 sdss_cherno-0.6.0/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     1994 2023-04-25 16:03:17.276124 sdss_cherno-0.6.0/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     1958 2023-04-25 16:03:17.301758 sdss_cherno-0.6.0/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2023-04-25 16:03:17.302240 sdss_cherno-0.6.0/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2023-04-25 16:03:17.302599 sdss_cherno-0.6.0/cherno/exceptions.py
+-rw-r--r--   0        0        0    14028 2023-04-25 16:03:17.303956 sdss_cherno-0.6.0/cherno/extraction.py
+-rw-r--r--   0        0        0    40248 2023-04-25 16:03:17.304689 sdss_cherno-0.6.0/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2023-04-25 16:03:17.305802 sdss_cherno-0.6.0/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2023-04-25 16:03:17.306236 sdss_cherno-0.6.0/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2023-04-25 16:03:17.306612 sdss_cherno-0.6.0/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2023-04-25 16:03:17.307096 sdss_cherno-0.6.0/cherno/utils.py
+-rw-r--r--   0        0        0     2314 2023-04-25 16:03:17.315859 sdss_cherno-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 sdss_cherno-0.6.0/PKG-INFO
```

### Comparing `sdss_cherno-0.5.2/LICENSE.md` & `sdss_cherno-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/README.md` & `sdss_cherno-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/__init__.py` & `sdss_cherno-0.6.0/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/__main__.py` & `sdss_cherno-0.6.0/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/__init__.py` & `sdss_cherno-0.6.0/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/actor.py` & `sdss_cherno-0.6.0/cherno/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/acquire.py` & `sdss_cherno-0.6.0/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/config.py` & `sdss_cherno-0.6.0/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/guide.py` & `sdss_cherno-0.6.0/cherno/actor/commands/guide.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,28 +192,33 @@
 
 def get_callback(
     params: GuideParams,
     target_rms: float | None = None,
 ):
     """Returns the Guide.process() callback."""
 
-    guider = Guider(config["observatory"], target_rms=target_rms)
+    guider = Guider(
+        config["observatory"],
+        target_rms=target_rms,
+        command=params.command,
+    )
     params.command.actor.state._guider_obj = guider  # To update PID coeffs.
 
     return partial(
         guider.process,
         correct=params.apply,
         full_correction=params.full,
         wait_for_correction=(params.wait is None),
         only_radec=params.only_radec,
         auto_radec_min=params.auto_radec_min,
         gaia_phot_g_mean_mag_max=params.gaia_max_mag,
         gaia_cross_correlation_blur=params.cross_match_blur,
         fit_all_detections=params.fit_all_detections,
         plot=params.plot,
+        fit_focus=config["guider"].get("fit_focus", True),
         **params.mode_kwargs,
     )
 
 
 async def _guide(
     params: GuideParams,
     stop_condition: Callable[[], bool] | None = None,
```

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/offset.py` & `sdss_cherno-0.6.0/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/reprocess.py` & `sdss_cherno-0.6.0/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/scale.py` & `sdss_cherno-0.6.0/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/set.py` & `sdss_cherno-0.6.0/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/show.py` & `sdss_cherno-0.6.0/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/status.py` & `sdss_cherno-0.6.0/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/stop.py` & `sdss_cherno-0.6.0/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/commands/version.py` & `sdss_cherno-0.6.0/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/actor/exposer.py` & `sdss_cherno-0.6.0/cherno/actor/exposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 from __future__ import annotations
 
 import asyncio
 import os
 import re
 from glob import glob
 
-from typing import Any, Callable, Union
-
-from astropy.time import Time
+from typing import Any, Callable, NoReturn, Union
 
 from clu import Command
+from sdsstools.time import get_sjd
 
 from cherno import config
 from cherno.exceptions import ExposerError
 from cherno.maskbits import GuiderStatus
 
 from . import ChernoCommandType
 
@@ -59,15 +58,15 @@
         self._blocking: bool = True
 
     def set_blocking(self, blocking: bool):
         """Whether to block while calling the callback."""
 
         self._blocking = blocking
 
-    def fail(self, message=""):
+    def fail(self, message="") -> NoReturn:
         """Sets the guider status to failed and raises an exception."""
 
         self.actor_state.set_status(GuiderStatus.FAILED | GuiderStatus.IDLE)
         raise ExposerError(message)
 
     async def one(self, exposure_time: float, **kwargs):
         """Exposes the cameras once.
@@ -247,18 +246,16 @@
 
         if not all([int(ss) == 10 for ss in values]):
             self.command.warning("FFS petals are not open.")
 
     def _get_num(self, names: list[str]) -> int:
         """Returns the next sequence number."""
 
-        date = Time.now()
-        mjd = int(date.mjd)
-
-        dirpath = os.path.join(config["cameras"]["path"], str(mjd))
+        sjd = get_sjd()
+        dirpath = os.path.join(config["cameras"]["path"], str(sjd))
         if not os.path.exists(dirpath):
             return 1
 
         gimgs = glob(os.path.join(dirpath, "*.fits*"))
         matches = [
             int(m.group(1))
             for file_ in gimgs
```

### Comparing `sdss_cherno-0.5.2/cherno/etc/cherno_APO.yml` & `sdss_cherno-0.6.0/cherno/etc/cherno_APO.yml`

 * *Files 3% similar despite different names*

```diff
@@ -70,26 +70,29 @@
 
 guider:
   cpulimit: 15
   astrometry_net_config: etc/astrometrynet_APO.cfg
   astrometry_net_use_all_regions: true
   astrometry_dir: ./astrometry
   focus_r2_threshold: 0.2
+  fit_focus: true
   plot_focus: true
   auto_radec_min: -1
   use_astrometry_net: true
   astrometry_net_odds: 9
   gaia_connection_string: postgresql://sdss_user@sdss5-db/chernodb
   gaia_phot_g_mean_mag_max: 19
   gaia_search_radius: 0.09
   gaia_use_cross_correlation_shift: true
   gaia_cross_correlation_blur: 1
   gaia_cross_correlation_min_error: 0.6
   gaia_distance_upper_bound: 5
   fit_all_detections: true
+  fit_rms_sigma: 2
+  plot_rms: true
 
 extraction:
   output_dir: ./extraction
   method: marginal
   plot: false
   rejection_method: sigclip
   reject_sigma: 2.0
```

### Comparing `sdss_cherno-0.5.2/cherno/etc/cherno_LCO.yml` & `sdss_cherno-0.6.0/cherno/etc/cherno_LCO.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
   log_dir: /data/logs/actors/cherno
 
 cameras:
   path: /data/gcam/
   names: [gfa1, gfa2, gfa3, gfa4, gfa5, gfa6]
   focus_offset:
     gfa1: 0
-    gfa2: -594.5
-    gfa3: -174.
-    gfa4: -268.25
-    gfa5: 94.25
-    gfa6: 166.75
+    gfa2: 0
+    gfa3: 0
+    gfa4: 0
+    gfa5: 0
+    gfa6: 0
   rotation:
     gfa1: 300
     gfa2: 0
     gfa3: 60
     gfa4: 120
     gfa5: 180
     gfa6: 240
@@ -46,50 +46,53 @@
 
 guide_loop:
   ra:
     pid:
       k: 0.7
       ti: 0.01
     min_correction: 0.03
-    max_correction: 600
+    max_correction: 60
   dec:
     pid:
       k: 0.7
       ti: 0.01
     min_correction: 0.03
-    max_correction: 600
+    max_correction: 60
   rot:
     pid:
       k: 1
-    min_correction: 10
-    max_correction: 7200
+    min_correction: 15
+    max_correction: 1000
   focus:
     pid:
       k: 0.3
     min_correction: 10
     max_correction: 200
 
 guider:
   cpulimit: 15
   astrometry_net_config: etc/astrometrynet_LCO.cfg
   astrometry_net_use_all_regions: false
   astrometry_dir: ./astrometry
   focus_r2_threshold: 0.2
+  fit_focus: false
   plot_focus: true
   auto_radec_min: 2
   use_astrometry_net: true
   astrometry_net_odds: 9
   gaia_connection_string: postgresql://sdss_user@sdss5-db/chernodb
   gaia_phot_g_mean_mag_max: 19
   gaia_search_radius: 0.05
   gaia_use_cross_correlation_shift: true
   gaia_cross_correlation_blur: 1
   gaia_cross_correlation_min_error: 0.6
   gaia_distance_upper_bound: 100
   fit_all_detections: true
+  fit_rms_sigma: 2
+  plot_rms: true
 
 extraction:
   output_dir: ./extraction
   method: marginal
   plot: false
   rejection_method: sigclip
   reject_sigma: 3.0
```

### Comparing `sdss_cherno-0.5.2/cherno/etc/schema.json` & `sdss_cherno-0.6.0/cherno/etc/schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945652173913043%*

 * *Differences: {"'properties'": "{'fit_rms_camera': OrderedDict([('type', 'array'), ('items', "*

 * *                 "[OrderedDict([('title', 'fit_rms'), ('type', 'number')]), OrderedDict([('title', "*

 * *                 "'camera1_rms'), ('type', 'number')]), OrderedDict([('title', 'camera1_fit'), "*

 * *                 "('type', 'boolean')]), OrderedDict([('title', 'camera2_rms'), ('type', "*

 * *                 "'number')]), OrderedDict([('title', 'camera2_fit'), ('type', 'boolean')]), "*

 * *                 "OrderedDict([('title', 'camer […]*

```diff
@@ -155,14 +155,71 @@
         },
         "did_correct": {
             "type": "boolean"
         },
         "enabled_axes": {
             "type": "array"
         },
+        "fit_rms_camera": {
+            "items": [
+                {
+                    "title": "fit_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera1_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera1_fit",
+                    "type": "boolean"
+                },
+                {
+                    "title": "camera2_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera2_fit",
+                    "type": "boolean"
+                },
+                {
+                    "title": "camera3_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera3_fit",
+                    "type": "boolean"
+                },
+                {
+                    "title": "camera4_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera4_fit",
+                    "type": "boolean"
+                },
+                {
+                    "title": "camera5_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera5_fit",
+                    "type": "boolean"
+                },
+                {
+                    "title": "camera6_rms",
+                    "type": "number"
+                },
+                {
+                    "title": "camera6_fit",
+                    "type": "boolean"
+                }
+            ],
+            "type": "array"
+        },
         "focus_data": {
             "items": {
                 "type": "number"
             },
             "type": "array"
         },
         "focus_fit": {
```

### Comparing `sdss_cherno-0.5.2/cherno/exceptions.py` & `sdss_cherno-0.6.0/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/extraction.py` & `sdss_cherno-0.6.0/cherno/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/guider.py` & `sdss_cherno-0.6.0/cherno/guider.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 # @Filename: guider.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
 import pathlib
+import re
 import time
 import warnings
 from dataclasses import dataclass, field
 from functools import partial
 
 from typing import TYPE_CHECKING, Any, Coroutine
 
 import numpy
 import pandas
 from astropy.io import fits
+from astropy.stats.sigma_clipping import SigmaClip
 from astropy.table import Table
 from astropy.wcs import WCS, FITSFixedWarning
 from simple_pid.PID import PID
 
 from clu.command import FakeCommand
+from coordio import defaults
 from coordio.astrometry import AstrometryNet
 from coordio.guide import (
     GuiderFit,
     GuiderFitter,
     cross_match,
     gfa_to_radec,
     radec_to_gfa,
@@ -78,28 +81,33 @@
         self.exposure_no = self.extraction_data.exposure_no
         self.obstime = self.extraction_data.obstime
         self.observatory = self.extraction_data.observatory
         self.field_ra = self.extraction_data.field_ra
         self.field_dec = self.extraction_data.field_dec
         self.field_pa = self.extraction_data.field_pa
 
+        match = re.match(r".*([1-6]).*", self.camera)
+        if match:
+            self.camera_id = int(match.group(1))
+
     @property
     def e_data(self):
         """Shortcut for ``extraction_data``."""
 
         return self.extraction_data
 
 
 @dataclass
 class AstrometricSolution:
     """Astrometric solution data."""
 
     valid_solution: bool
     guide_data: list[GuideData]
     guider_fit: GuiderFit | None = None
+    fitter: GuiderFitter | None = None
     delta_ra: float = -999.0
     delta_dec: float = -999.0
     delta_rot: float = -999.0
     delta_scale: float = -999.0
     delta_focus: float = -999.0
     fit_mode: str = "full"
     rms: float = -999.0
@@ -314,14 +322,15 @@
             correct = False
 
         if correct and ast_solution.valid_solution is True:
             await self.correct(
                 ast_solution,
                 full=full_correction,
                 wait_for_correction=wait_for_correction,
+                apply_focus=fit_focus,
             )
         else:
             self.command.info(
                 acquisition_valid=ast_solution.valid_solution,
                 did_correct=any(ast_solution.correction_applied),
                 correction_applied=ast_solution.correction_applied,
             )
@@ -407,44 +416,81 @@
             only_radec = True
             self.command.warning(
                 f"Only {len(solved)} cameras solved. Only fitting RA/Dec. "
                 "The rotation and scale offsets are informational-only "
                 "and not corrected."
             )
 
-        guider_fit = self.fitter.fit(
-            field_ra,
-            field_dec,
-            field_pa,
-            offset=full_offset,
-            scale_rms=scale_rms,
-            only_radec=only_radec,
-        )
+        fit_cameras = [d.camera_id for d in solved]
+        fit_rms_sigma = config["guider"].get("fit_rms_sigma", 3)
+        guider_fit = None
+        while True:
+            tmp_guider_fit = self.fitter.fit(
+                field_ra,
+                field_dec,
+                field_pa,
+                offset=full_offset,
+                scale_rms=scale_rms,
+                only_radec=only_radec,
+                cameras=fit_cameras,
+            )
+
+            # If we already had a solution and this fit failed or the fit RMS is bad,
+            # just use the previous fit.
+            if guider_fit is not None and (fit_rms_sigma <= 0 or not tmp_guider_fit):
+                break
+
+            # Update the fit with the previous one.
+            guider_fit = tmp_guider_fit
+
+            # If only 3 cameras remain we exit. We don't want to reject any more.
+            if len(fit_cameras) <= 3:
+                break
+
+            sc = SigmaClip(fit_rms_sigma)
+            rms_clip = sc(guider_fit.fit_rms.loc[fit_cameras, "rms"])
+
+            # All the camera fit RMS are within X sigma. Exit.
+            if rms_clip.mask.sum() == 0:
+                break
+
+            # Find the camera with the largest fit RMS and remove it. Redo the fit.
+            cam_max_rms = int(guider_fit.fit_rms.loc[fit_cameras, "rms"].idxmax())
+
+            self.command.warning(
+                "Fit RMS found outlier detections. "
+                f"Refitting without camera {cam_max_rms}."
+            )
+            fit_cameras.remove(cam_max_rms)
+
+        plate_scale = defaults.PLATE_SCALE[self.observatory]
+        mm_to_arcsec = 1 / plate_scale * 3600
 
         exp_no = solved[0].exposure_no  # Should be the same for all.
 
-        if guider_fit is False:
+        if not guider_fit:
             rms = delta_ra = delta_dec = delta_rot = delta_scale = -999.0
             ast_solution.guider_fit = None
         else:
             delta_ra = guider_fit.delta_ra
             delta_dec = guider_fit.delta_dec
             delta_rot = guider_fit.delta_rot
             delta_scale = guider_fit.delta_scale
 
-            xrms = guider_fit.xrms
-            yrms = guider_fit.yrms
-            rms = guider_fit.rms
+            xrms = numpy.round(guider_fit.xrms * mm_to_arcsec, 3)
+            yrms = numpy.round(guider_fit.yrms * mm_to_arcsec, 3)
+            rms = numpy.round(guider_fit.rms * mm_to_arcsec, 3)
 
             ast_solution.guider_fit = guider_fit
+            ast_solution.fitter = self.fitter
 
             self.command.info(guide_rms=[exp_no, xrms, yrms, rms])
 
             # Store RMS. This is used to determine acquisition convergence.
-            if rms > 0:
+            if self.command.actor and rms > 0 and rms < 1:
                 self.command.actor.state.rms_history.append(rms)
 
         ast_solution.valid_solution = True
 
         ast_solution.delta_ra = float(delta_ra)
         ast_solution.delta_dec = float(delta_dec)
         ast_solution.delta_rot = float(delta_rot)
@@ -469,14 +515,25 @@
                 ast_solution.delta_focus = round(-x_min / focus_sensitivity, 1)
                 ast_solution.focus_coeff = [a, b, c]
                 ast_solution.focus_r2 = round(r2, 3)
 
             except Exception as err:
                 self.command.warning(f"Failed fitting focus curve: {err}.")
 
+        if guider_fit:
+            fit_rms = guider_fit.fit_rms
+            fit_rms_camera = [numpy.round(fit_rms.loc[0].rms * mm_to_arcsec, 4)]
+            for cid in range(1, 7):
+                rms_cam = fit_rms.loc[cid].rms if cid in fit_rms.index else -999.0
+                fit_rms_camera += [
+                    numpy.round(rms_cam * mm_to_arcsec, 4) if rms_cam != -999 else -999,
+                    cid in guider_fit.cameras,
+                ]
+            self.command.info(fit_rms_camera=fit_rms_camera)
+
         self.command.info(
             astrometry_fit=[
                 exp_no,
                 len(solved),
                 -999.0,
                 -999.0,
                 numpy.round(fwhm, 2),
@@ -497,45 +554,58 @@
                     int(d.camera[-1]),
                     d.extraction_data.fwhm_median,
                     d.extraction_data.focus_offset,
                 ]
 
         self.command.debug(focus_data=focus_data)
 
-        self.command.info(
-            focus_fit=[
-                exp_no,
-                ast_solution.fwhm_fit,
-                float(f"{ast_solution.focus_coeff[0]:.3e}"),
-                float(f"{ast_solution.focus_coeff[1]:.3e}"),
-                float(f"{ast_solution.focus_coeff[2]:.3e}"),
-                ast_solution.focus_r2,
-                ast_solution.delta_focus,
-            ]
-        )
+        if fit_focus:
+            self.command.info(
+                focus_fit=[
+                    exp_no,
+                    ast_solution.fwhm_fit,
+                    float(f"{ast_solution.focus_coeff[0]:.3e}"),
+                    float(f"{ast_solution.focus_coeff[1]:.3e}"),
+                    float(f"{ast_solution.focus_coeff[2]:.3e}"),
+                    ast_solution.focus_r2,
+                    ast_solution.delta_focus,
+                ]
+            )
 
         if (
             delta_scale > 0
             and self.command.actor
             and fwhm < 2.5
+            and rms > 0
+            and rms <= 1
             and guider_fit
             and not guider_fit.only_radec
         ):
             # If we measured the scale, add it to the actor state. This is later
             # used to compute the average scale over a period. We also add the time
             # because we'll want to reject measurements that are too old.
             self.command.actor.state.scale_history.append((time.time(), delta_scale))
 
+        if config["guider"].get("plot_rms", False):
+            e_data_test = data[0].e_data
+            path = e_data_test.path.parent
+            mjd = e_data_test.mjd
+            seq = e_data_test.exposure_no
+            outpath = path / "fit" / f"fit_rms-{mjd}-{seq}.pdf"
+            outpath.parent.mkdir(exist_ok=True)
+            self.fitter.plot_fit(outpath)
+
         return ast_solution
 
     async def correct(
         self,
         data: AstrometricSolution,
         full: bool = False,
         wait_for_correction: bool = True,
+        apply_focus: bool = True,
     ):
         """Runs the astrometric fit"""
 
         if not self.command.actor or self.command.status.is_done:
             raise ChernoError("Cannot run correct without a valid running command.")
 
         actor_state = self.command.actor.state
@@ -547,23 +617,29 @@
             data.correction_applied = [0.0, 0.0, 0.0, 0.0, 0.0]
             self.command.info(acquisition_valid=True, did_correct=False)
             return True
 
         self.command.info("Applying corrections.")
 
         if self.observatory == "APO":
-            await self._correct_apo(data, full=full)
+            await self._correct_apo(data, full=full, apply_focus=apply_focus)
         else:
             await self._correct_lco(
                 data,
                 full=full,
                 wait_for_correction=wait_for_correction,
+                apply_focus=apply_focus,
             )
 
-    async def _correct_apo(self, data: AstrometricSolution, full: bool = False):
+    async def _correct_apo(
+        self,
+        data: AstrometricSolution,
+        full: bool = False,
+        apply_focus: bool = True,
+    ):
         actor_state = self.command.actor.state
 
         min_isolated = actor_state.guide_loop["rot"]["min_isolated_correction"]
         if abs(data.delta_rot) >= min_isolated:
             self.command.debug("Applying only large rotator correction.")
             coro = apply_axes_correction(
                 self.command,
@@ -584,21 +660,22 @@
         correct_tasks: list[Coroutine[Any, Any, Any]] = [coro]
 
         do_focus: bool = False
 
         # Ignore focus correction when the r2 correlation is bad or when we got
         # an inverted parabola.
         if (
-            data.focus_r2 > config["guider"]["focus_r2_threshold"]
+            apply_focus
+            and data.focus_r2 > config["guider"]["focus_r2_threshold"]
             and data.focus_coeff[0] > 0
         ):
             do_focus = True
             coro = apply_focus_correction(self.command, self.pids, data.delta_focus)
             correct_tasks.append(coro)
-        else:
+        elif apply_focus:
             self.command.warning("Focus fit poorly constrained. Not correcting focus.")
 
         self.command.actor.state.set_status(GuiderStatus.CORRECTING, mode="add")
         applied_corrections: Any = await asyncio.gather(*correct_tasks)
         self.command.actor.state.set_status(GuiderStatus.CORRECTING, mode="remove")
 
         data.correction_applied[:4] = applied_corrections[0]
@@ -614,41 +691,47 @@
         )
 
     async def _correct_lco(
         self,
         data: AstrometricSolution,
         full: bool = False,
         wait_for_correction: bool = True,
+        apply_focus: bool = True,
     ):
         do_focus: bool = False
 
         enabled_axes = self.command.actor.state.enabled_axes
 
         # Ignore focus correction when the r2 correlation is bad or when we got
         # an inverted parabola.
         if (
-            data.focus_r2 > config["guider"]["focus_r2_threshold"]
+            apply_focus
+            and data.focus_r2 > config["guider"]["focus_r2_threshold"]
             and data.focus_coeff[0] > 0
             and "focus" in enabled_axes
         ):
             do_focus = True
-        else:
+        elif apply_focus:
             self.command.warning("Focus fit poorly constrained. Not correcting focus.")
 
         self.command.actor.state.set_status(GuiderStatus.CORRECTING, mode="add")
 
-        applied_corrections: Any = await apply_correction_lco(
-            self.command,
-            self.pids,
-            delta_radec=(data.delta_ra, data.delta_dec),
-            delta_rot=data.delta_rot if data.fit_mode == "full" else None,
-            delta_focus=data.delta_focus if do_focus else None,
-            full=full,
-            wait_for_correction=wait_for_correction,
-        )
+        try:
+            applied_corrections: Any = await apply_correction_lco(
+                self.command,
+                self.pids,
+                delta_radec=(data.delta_ra, data.delta_dec),
+                delta_rot=data.delta_rot if data.fit_mode == "full" else None,
+                delta_focus=data.delta_focus if do_focus else None,
+                full=full,
+                wait_for_correction=wait_for_correction,
+            )
+        except ChernoError as err:
+            self.command.warning(f"Failed applying correction: {err}")
+            applied_corrections = [0.0, 0.0, 0.0, 0.0, 0.0]
 
         self.command.actor.state.set_status(GuiderStatus.CORRECTING, mode="remove")
 
         data.correction_applied = applied_corrections
 
         self.command.info(
             acquisition_valid=True,
```

### Comparing `sdss_cherno-0.5.2/cherno/lcotcc.py` & `sdss_cherno-0.6.0/cherno/lcotcc.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     guide_loop = state.guide_loop
     enabled_axes = state.enabled_axes
 
     corr_radec = numpy.array([0.0, 0.0])
     corr_rot: float = 0.0
     corr_focus: float = 0.0
 
-    if delta_rot is not None and "rot" in enabled_axes:
+    if delta_rot is not None and "rot" in enabled_axes and delta_rot != -999.0:
         if full:
             corr_rot = -delta_rot
         else:
             corr_rot = pids.rot(delta_rot) or 0.0
 
         min_corr_arcsec = guide_loop["rot"]["min_correction"]
         max_corr_arcsec = guide_loop["rot"]["max_correction"]
@@ -60,17 +60,17 @@
             command.debug("Skipping small rotator correction.")
             corr_rot = 0.0
         elif numpy.abs(corr_rot) > max_corr_arcsec:
             raise ChernoError(f"Rotator correction too large: {corr_rot:.1f}.")
 
         corr_rot /= 3600
 
-    if corr_rot == 0.0 and delta_radec is not None:
+    if delta_radec is not None:
         for ax_idx, ax in enumerate(["ra", "dec"]):
-            if ax not in enabled_axes:
+            if ax not in enabled_axes or float(delta_radec[ax_idx]) == -999.0:
                 continue
 
             if full:
                 corr_ax = -float(delta_radec[ax_idx])
             else:
                 # This returns the correction (i.e., opposite sign).
                 corr_ax = getattr(pids, ax)(float(delta_radec[ax_idx])) or 0.0
@@ -82,15 +82,15 @@
                 command.debug(f"Skipping small {ax.lower()} correction.")
                 corr_ax = 0.0
             elif numpy.abs(corr_ax) > max_corr_arcsec:
                 raise ChernoError(f"{ax.upper()} correction too large: {corr_ax:.2f}.")
 
             corr_radec[ax_idx] = corr_ax / 3600
 
-    if delta_focus is not None and "focus" in enabled_axes:
+    if delta_focus is not None and "focus" in enabled_axes and delta_focus != -999.0:
         if full:
             corr_focus = -delta_focus
         else:
             corr_focus = pids.focus(delta_focus) or 0.0
 
         min_corr = guide_loop["focus"]["min_correction"]
         max_corr = guide_loop["focus"]["max_correction"]
```

### Comparing `sdss_cherno-0.5.2/cherno/maskbits.py` & `sdss_cherno-0.6.0/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/cherno/tcc.py` & `sdss_cherno-0.6.0/cherno/tcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # Correction applied in ra, dec, rot, scale, in arcsec.
     correction_applied = [0.0, 0.0, 0.0, 0.0]
 
     if delta_radec is not None:
         corr_radec = [0.0, 0.0]
 
         for ax_idx, ax in enumerate(["ra", "dec"]):
-            if ax not in enabled_axes:
+            if ax not in enabled_axes or float(delta_radec[ax_idx]) == -999.0:
                 continue
 
             if full:
                 corr_ax = -float(delta_radec[ax_idx])
             else:
                 # This returns the correction (i.e., opposite sign).
                 corr_ax = getattr(pids, ax)(float(delta_radec[ax_idx])) or 0.0
@@ -77,15 +77,15 @@
             if tcc_offset_cmd.status.did_fail:
                 command.error("Failed applying RA/Dec correction.")
                 return correction_applied
 
             correction_applied[0] = float(numpy.round(corr_radec[0] * 3600.0, 3))
             correction_applied[1] = float(numpy.round(corr_radec[1] * 3600.0, 3))
 
-    if delta_rot is not None and "rot" in enabled_axes:
+    if delta_rot is not None and "rot" in enabled_axes and delta_rot != -999.0:
         if full:
             corr_rot = -delta_rot
         else:
             corr_rot = pids.rot(delta_rot) or 0.0
 
         min_corr_arcsec = guide_loop["rot"]["min_correction"]
         max_corr_arcsec = guide_loop["rot"]["max_correction"]
@@ -126,15 +126,15 @@
 
     guide_loop = state.guide_loop
     enabled_axes = state.enabled_axes
 
     min_corr = guide_loop["focus"]["min_correction"]
     max_corr = guide_loop["focus"]["max_correction"]
 
-    if "focus" not in enabled_axes:
+    if "focus" not in enabled_axes or delta_focus == -999.0:
         return 0.0
 
     corr_focus = pids.focus(delta_focus) or 0.0
 
     if numpy.abs(corr_focus) < min_corr:
         command.debug("Skipping small focus correction.")
         return 0.0
```

### Comparing `sdss_cherno-0.5.2/cherno/utils.py` & `sdss_cherno-0.6.0/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.5.2/pyproject.toml` & `sdss_cherno-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.5.2"
+version = "0.6.0"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 sdsstools = "^1.0.0"
 sdss-clu = "^1.8.0"
 astropy = "^5.0.0"
 click-default-group = "^1.2.2"
-sdss-coordio = "^1.6.1"
+sdss-coordio = "^1.7.1"
 pandas = "^1.3.4"
 tables = ">=3.6.1"
 simple-pid = "^1.0.1"
 sqlalchemy = "^1.4.45"
 psycopg2-binary = "^2.9.5"
 
 [tool.poetry.dev-dependencies]
@@ -45,15 +45,14 @@
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
 isort = ">=4.3.21"
-codecov = ">=2.0.15"
 coverage = {version = ">=5.0", extras = ["toml"]}
 ipdb = ">=0.12.3"
 Sphinx = {version=">=3.0.0"}
 black = {version=">=20.8b1", allow-prereleases=true}
 sphinx-click = ">=2.6.0"
 sphinx-jsonschema = ">=1.16.7"
 myst-parser = ">=0.14.0"
```

### Comparing `sdss_cherno-0.5.2/PKG-INFO` & `sdss_cherno-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.5.2
+Version: 0.6.0
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.12
@@ -21,15 +21,15 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.0.0,<6.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sdss-clu (>=1.8.0,<2.0.0)
-Requires-Dist: sdss-coordio (>=1.6.1,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.7.1,<2.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: simple-pid (>=1.0.1,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.45,<2.0.0)
 Requires-Dist: tables (>=3.6.1)
 Project-URL: Documentation, https://sdss-cherno.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/cherno
 Description-Content-Type: text/markdown
```

