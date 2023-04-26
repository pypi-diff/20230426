# Comparing `tmp/gocart-0.1.9.tar.gz` & `tmp/gocart-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.1.9.tar", last modified: Wed Apr 19 15:03:34 2023, max compression
+gzip compressed data, was "gocart-0.2.0.tar", last modified: Wed Apr 26 14:26:01 2023, max compression
```

## Comparing `gocart-0.1.9.tar` & `gocart-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      990 2023-04-19 14:58:37.000000 gocart-0.1.9/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-19 14:58:37.000000 gocart-0.1.9/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-19 14:58:37.000000 gocart-0.1.9/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-19 15:03:34.625041 gocart-0.1.9/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-19 14:58:37.000000 gocart-0.1.9/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.613040 gocart-0.1.9/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     7204 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.621040 gocart-0.1.9/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12117 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2303 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.625041 gocart-0.1.9/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6509 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/parsers/lvk.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2069 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-19 14:58:37.000000 gocart-0.1.9/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-19 15:03:34.617040 gocart-0.1.9/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      718 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-19 15:02:25.000000 gocart-0.1.9/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-19 15:03:34.000000 gocart-0.1.9/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-19 15:03:34.625041 gocart-0.1.9/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-19 14:58:37.000000 gocart-0.1.9/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1454 2023-04-26 14:21:44.000000 gocart-0.2.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-26 14:21:44.000000 gocart-0.2.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-26 14:21:44.000000 gocart-0.2.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 14:26:01.174921 gocart-0.2.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-26 14:21:44.000000 gocart-0.2.0/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8322 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12416 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.174921 gocart-0.2.0/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12929 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/parsers/lvk.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-26 14:21:44.000000 gocart-0.2.0/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 14:26:01.170920 gocart-0.2.0/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      748 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 14:25:03.000000 gocart-0.2.0/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-26 14:26:00.000000 gocart-0.2.0/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-26 14:26:01.174921 gocart-0.2.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-26 14:21:44.000000 gocart-0.2.0/setup.py
```

### Comparing `gocart-0.1.9/CHANGES.md` & `gocart-0.2.0/CHANGES.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 
 ## Release Notes
 
-<!-- **vx.x.x - xxdatexx** -->
+**v0.2.0 - April 26, 2023**  
 
-**v0.1.9 - April 19, 2023**
+- **FEATURE**: filtering of alerts is now possible via options in the settings file (see docs)  
+- **ENHANCEMENT**: option added to write the original json alert to file  
+- **ENHANCEMENT**: gocart *should* be robust enough to handle burst events (tested against a hand crafted burst alert packet as none exist in the LVK Public Alert Guide yet).  
 
-- **REFACTOR** -- sun and moon footprints replace terminator
+**v0.1.10 - April 21, 2023**  
 
-**v0.1.8 - April 6, 2023**
+- **REFACTOR**: splitting mockevents from superevents   
 
-- **FIXED** -- echo command now parses message to the end of the partition queue
-- **FIXED** -- listen command remembers where it left off
-- **FIXED** -- sun & moon coordinates ... they were not geocentric!
+**v0.1.9 - April 19, 2023**  
 
-**v0.1.7 - April 4, 2023**
+- **REFACTOR**: sun and moon footprints replace terminator  
 
-- **FIXED** -- unit test fix
+**v0.1.8 - April 6, 2023**  
 
-**v0.1.6 - April 4, 2023**
+- **FIXED**: echo command now parses message to the end of the partition queue  
+- **FIXED**: listen command remembers where it left off  
+- **FIXED**: sun & moon coordinates ... they were not geocentric!  
 
-- **ENHANCEMENT** -- added localisation type to aitoff maps
-- **FIXED** -- first time listen command no longer starteds from time zero but listens from first connection
-- **FIXED** -- doc builds
+**v0.1.7 - April 4, 2023**  
 
-**v0.1.5 - April 4, 2023**
+- **FIXED**: unit test fix  
 
-- **FEATURE**: listen command added
-- **FEATURE**: echo command added
-- **FEATURE**: maps converted to ascii format
-- **FEATURE**: maps rendered as aitoff plots
-- **FEATURE**: meta.yaml file written with alert, FITS header and extra useful content
+**v0.1.6 - April 4, 2023**  
+ 
+- **ENHANCEMENT**: added localisation type to aitoff maps  
+- **FIXED**: first time listen command no longer starteds from time zero but listens from first connection  
+- **FIXED**: doc builds  
 
-**v0.1.4 - March 16, 2023**
+**v0.1.5 - April 4, 2023**  
 
-- fixing docsting test
+- **FEATURE**: listen command added  
+- **FEATURE**: echo command added  
+- **FEATURE**: maps converted to ascii format  
+- **FEATURE**: maps rendered as aitoff plots  
+- **FEATURE**: meta.yaml file written with alert, FITS header and extra useful content  
+
+**v0.1.4 - March 16, 2023**  
+
+- fixing docsting test
```

### Comparing `gocart-0.1.9/LICENSE` & `gocart-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/PKG-INFO` & `gocart-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.1.9
+Version: 0.2.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.9.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.1.9/README.md` & `gocart-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/cl_utils.py` & `gocart-0.2.0/gocart/cl_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,14 +112,45 @@
 
     topic = 'igwn.gwalert'
 
     if len(settings['gcn-kafka']['client_id']) < 6 or len(settings['gcn-kafka']['client_secret']) < 6:
         print("Please add your gcn-kafka client ID and secret to the gocart.yaml settings file.")
         return
 
+    if a['listen'] or a['echo']:
+
+        if a['listen']:
+            verb = "Listening for"
+        else:
+            verb = "Echoing"
+
+        parse_mock_events = settings["lvk"]["parse_mock_events"]
+        parse_real_events = settings["lvk"]["parse_real_events"]
+        # WHERE TO DOWNLOAD MAPS TO
+        if "download_dir" in settings["lvk"] and settings["lvk"]["download_dir"]:
+            download_dir = settings["lvk"]["download_dir"]
+            # MAKE RELATIVE HOME PATH ABSOLUTE
+            from os.path import expanduser
+            home = expanduser("~")
+            if download_dir == "~":
+                download_dir = download_dir.replace("~", home)
+        else:
+            download_dir = "."
+
+        mockDir = download_dir + "/mockevents/"
+        evertDir = download_dir + "/superevents/"
+        if parse_mock_events:
+            print(f"{verb} Mockevents")
+            if not os.path.exists(mockDir):
+                os.makedirs(mockDir)
+        if parse_real_events:
+            print(f"{verb} Superevents")
+            if not os.path.exists(evertDir):
+                os.makedirs(evertDir)
+
     # CALL FUNCTIONS/OBJECTS
     if a['listen']:
         from gcn_kafka import Consumer
         from confluent_kafka import TopicPartition
         from gocart.parsers import lvk
 
         config = {
```

### Comparing `gocart-0.1.9/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.2.0/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.2.0/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/convert/aitoff.py` & `gocart-0.2.0/gocart/convert/aitoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,15 +267,15 @@
                 else:
                     label = f"{l}%"
                 patch = mpatches.Patch(color=c, label=label)
                 handles.append(patch)
 
         if len(self.meta):
             data = ""
-            data += f"Event: {self.meta['ALERT']['superevent_id']}\n"
+            data += f"Event: {self.meta['ALERT']['superevent_id']} ({self.meta['ALERT']['event']['group']})\n"
             eventDate = Time(self.meta['HEADER']['DATE-OBS'], scale='utc').to_datetime().strftime("%Y-%m-%d %H:%M:%S")
             data += f"Event time: {eventDate}\n"
 
             data += "\n"
             data += f"Alert: {self.meta['ALERT']['alert_type'].replace('_',' ')}\n"
             alertDate = Time(self.meta['ALERT']['time_created'], scale='utc').to_datetime().strftime("%Y-%m-%d %H:%M:%S")
             data += f"Alert time: {alertDate}\n"
@@ -286,30 +286,34 @@
             far = 1 / (float(self.meta['ALERT']['event']['far']) * 60. * 60. * 24.)
             if far > 1000:
                 far /= 365.
                 data += f"FAR: 1 per {far:0.1f} yrs\n"
             else:
                 data += f"FAR: 1 per {far:0.1f} days\n"
 
-            data += f"Dist: {self.meta['HEADER']['DISTMEAN']:.2f} (±{self.meta['HEADER']['DISTSTD']:.2f}) Mpc\n"
+            if 'DISTMEAN' in self.meta['HEADER']:
+                data += f"Dist: {self.meta['HEADER']['DISTMEAN']:.2f} (±{self.meta['HEADER']['DISTSTD']:.2f}) Mpc\n"
 
             data += "\n"
-            for k, v in self.meta['ALERT']['event']['classification'].items():
-                data += f"{k}: {v:.2f}\n"
+            if "classification" in self.meta['ALERT']['event']:
+                for k, v in self.meta['ALERT']['event']['classification'].items():
+                    data += f"{k}: {v:.2f}\n"
 
             data += "\n"
-            for k, v in self.meta['ALERT']['event']['properties'].items():
-                data += f"{k}: {v:.2f}\n"
+            if "properties" in self.meta['ALERT']['event']:
+                for k, v in self.meta['ALERT']['event']['properties'].items():
+                    data += f"{k}: {v:.2f}\n"
 
             plt.text(3.42, 0.2, data, ha='left', va='top', fontsize=5, linespacing=1.8)
 
         # this = ax.clabel(line_c, inline=True, fontsize=6, colors=['#93a1a1'], fmt='{:.0f} '.format)
 
         ax.tick_params(axis='x', labelsize=12)
         ax.tick_params(axis='y', labelsize=12)
+        ax.grid(color='#657b83', alpha=0.2, linestyle='dotted')
         plt.grid(True)
         plt.legend(handles=handles, loc='upper left', scatterpoints=1, bbox_to_anchor=(1.01, 1), fontsize=6)
         ax.xaxis.zorder = 40
 
         plt.savefig(self.outputFolder + "/skymap.png", bbox_inches='tight', dpi=300)
 
         plt.close()
```

### Comparing `gocart-0.1.9/gocart/convert/ascii.py` & `gocart-0.2.0/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/convert/healpix2cart.py` & `gocart-0.2.0/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/setup.cfg` & `gocart-0.2.0/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart/utKit.py` & `gocart-0.2.0/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.1.9/gocart.egg-info/PKG-INFO` & `gocart-0.2.0/gocart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.1.9
+Version: 0.2.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.1.9.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.1.9/gocart.egg-info/SOURCES.txt` & `gocart-0.2.0/gocart.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 gocart/__init__.py
 gocart/__version__.py
+gocart/advanced_settings.yaml
 gocart/cl_utils.py
 gocart/default_settings.yaml
 gocart/setup.cfg
 gocart/test_settings.yaml
 gocart/utKit.py
 gocart.egg-info/PKG-INFO
 gocart.egg-info/SOURCES.txt
```

### Comparing `gocart-0.1.9/setup.py` & `gocart-0.2.0/setup.py`

 * *Files identical despite different names*

