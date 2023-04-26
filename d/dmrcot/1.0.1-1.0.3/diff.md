# Comparing `tmp/dmrcot-1.0.1.tar.gz` & `tmp/dmrcot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmrcot-1.0.1.tar", last modified: Wed Apr 26 04:25:47 2023, max compression
+gzip compressed data, was "dmrcot-1.0.3.tar", last modified: Wed Apr 26 04:47:49 2023, max compression
```

## Comparing `dmrcot-1.0.1.tar` & `dmrcot-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:25:47.487998 dmrcot-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-26 04:25:36.000000 dmrcot-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 04:25:36.000000 dmrcot-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-26 04:25:47.487998 dmrcot-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-26 04:25:36.000000 dmrcot-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:25:47.483998 dmrcot-1.0.1/dmrcot/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 04:25:36.000000 dmrcot-1.0.1/dmrcot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-26 04:25:36.000000 dmrcot-1.0.1/dmrcot/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-26 04:25:36.000000 dmrcot-1.0.1/dmrcot/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-26 04:25:36.000000 dmrcot-1.0.1/dmrcot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-26 04:25:36.000000 dmrcot-1.0.1/dmrcot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:25:47.487998 dmrcot-1.0.1/dmrcot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 04:25:47.000000 dmrcot-1.0.1/dmrcot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 04:25:47.487998 dmrcot-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-26 04:25:36.000000 dmrcot-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:47:49.120707 dmrcot-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-26 04:47:37.000000 dmrcot-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 04:47:37.000000 dmrcot-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-26 04:47:49.120707 dmrcot-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-26 04:47:37.000000 dmrcot-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:47:49.116707 dmrcot-1.0.3/dmrcot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-26 04:47:37.000000 dmrcot-1.0.3/dmrcot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-26 04:47:37.000000 dmrcot-1.0.3/dmrcot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-26 04:47:37.000000 dmrcot-1.0.3/dmrcot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-26 04:47:37.000000 dmrcot-1.0.3/dmrcot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-26 04:47:37.000000 dmrcot-1.0.3/dmrcot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:47:49.120707 dmrcot-1.0.3/dmrcot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 04:47:49.000000 dmrcot-1.0.3/dmrcot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 04:47:49.120707 dmrcot-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-26 04:47:37.000000 dmrcot-1.0.3/setup.py
```

### Comparing `dmrcot-1.0.1/LICENSE` & `dmrcot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmrcot-1.0.1/PKG-INFO` & `dmrcot-1.0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1
-Name: dmrcot
-Version: 1.0.1
-Summary: DMR Trunking Node Controller to Cursor on Target Gateway.
-Home-page: https://github.com/snstac/dmrcot
-Author: Greg Albrecht
-Author-email: gba@snstac.com
-License: Apache License, Version 2.0
-Keywords: DMR,Cursor on Target,ATAK,TAK,CoT,iTAK
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-License-File: LICENSE
-
 DMR to Cursor on Target Gateway
 *********************************
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png?token=GHSAT0AAAAAAB5KT72KYMKM7HC3VWKFNTQAZCIXEJQ
    :alt: Screenshot of DMRCOT in ATAK.
 
 The DMR to Cursor on Target Gateway (DMRCOT) transforms Tait DMR Unit Information into 
 Cursor on Target (CoT) for display on `TAK Products <https://tak.gov/>`_ such as ATAK, 
 WinTAK & iTAK.
 
 Concept of Operations
 =====================
 DMRCOT reads Tait DMR subscriber radio positioning information from a DMR NC.
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png?token=GHSAT0AAAAAAB5KT72KJV6UBJNG6KLWKZTYZCIXFQA
    :alt: DMRCOT Concept of Operations (CONOP).
    :target: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
 
 
 Install
 =======
 DMRCOT functionality is provided via a command-line tool named ``dmrcot``. 
@@ -152,10 +139,10 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 
 A PyTAK Project
 ===============
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png?token=GHSAT0AAAAAAB5KT72LUEKHWJ464J3XTTLUZCIXGAA
     :alt: PyTAK Logo
     :target: https://github.com/snstac/pytak
```

### Comparing `dmrcot-1.0.1/README.rst` & `dmrcot-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+Metadata-Version: 2.1
+Name: dmrcot
+Version: 1.0.3
+Summary: DMR Trunking Node Controller to Cursor on Target Gateway.
+Home-page: https://github.com/snstac/dmrcot
+Author: Greg Albrecht
+Author-email: gba@snstac.com
+License: Apache License, Version 2.0
+Keywords: DMR,Cursor on Target,ATAK,TAK,CoT,iTAK
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+License-File: LICENSE
+
 DMR to Cursor on Target Gateway
 *********************************
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png?token=GHSAT0AAAAAAB5KT72KYMKM7HC3VWKFNTQAZCIXEJQ
    :alt: Screenshot of DMRCOT in ATAK.
 
 The DMR to Cursor on Target Gateway (DMRCOT) transforms Tait DMR Unit Information into 
 Cursor on Target (CoT) for display on `TAK Products <https://tak.gov/>`_ such as ATAK, 
 WinTAK & iTAK.
 
 Concept of Operations
 =====================
 DMRCOT reads Tait DMR subscriber radio positioning information from a DMR NC.
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png?token=GHSAT0AAAAAAB5KT72KJV6UBJNG6KLWKZTYZCIXFQA
    :alt: DMRCOT Concept of Operations (CONOP).
    :target: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
 
 
 Install
 =======
 DMRCOT functionality is provided via a command-line tool named ``dmrcot``. 
@@ -139,10 +152,10 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 
 A PyTAK Project
 ===============
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png?token=GHSAT0AAAAAAB5KT72LUEKHWJ464J3XTTLUZCIXGAA
     :alt: PyTAK Logo
     :target: https://github.com/snstac/pytak
```

### Comparing `dmrcot-1.0.1/dmrcot/__init__.py` & `dmrcot-1.0.3/dmrcot/__init__.py`

 * *Files identical despite different names*

### Comparing `dmrcot-1.0.1/dmrcot/classes.py` & `dmrcot-1.0.3/dmrcot/classes.py`

 * *Files identical despite different names*

### Comparing `dmrcot-1.0.1/dmrcot/commands.py` & `dmrcot-1.0.3/dmrcot/commands.py`

 * *Files identical despite different names*

### Comparing `dmrcot-1.0.1/dmrcot/constants.py` & `dmrcot-1.0.3/dmrcot/constants.py`

 * *Files identical despite different names*

### Comparing `dmrcot-1.0.1/dmrcot/functions.py` & `dmrcot-1.0.3/dmrcot/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
     if fleet_addr is None:
         return None
 
     badpos = [None, 0, 0.0, "0", "0.0"]
     if lat in badpos and lon in badpos:
         return None
 
+    if not lat or not lon:
+        return None
+
     config = config or {}
 
     remarks_fields: list = []
 
     emer = unit.get("emergency")
     if emer:
         remarks_fields.append("EMERGENCY")
@@ -192,14 +195,17 @@
     if fleet_addr is None:
         return None
 
     badpos = [None, 0, 0.0, "0", "0.0"]
     if lat in badpos and lon in badpos:
         return None
 
+    if not lat or not lon:
+        return None
+
     cot_uid = f"DMRCOT-{fleet_addr}-9-1-1"
     cot_type = "b-a-o-tbl"
     callsign = f"{unit.get('alias', fleet_addr)}-Alert"
 
     point: ET.Element = ET.Element("point")
     point.set("lat", str(lat))
     point.set("lon", str(lon))
```

### Comparing `dmrcot-1.0.1/dmrcot.egg-info/PKG-INFO` & `dmrcot-1.0.3/dmrcot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: dmrcot
-Version: 1.0.1
+Version: 1.0.3
 Summary: DMR Trunking Node Controller to Cursor on Target Gateway.
 Home-page: https://github.com/snstac/dmrcot
 Author: Greg Albrecht
 Author-email: gba@snstac.com
 License: Apache License, Version 2.0
 Keywords: DMR,Cursor on Target,ATAK,TAK,CoT,iTAK
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE
 
 DMR to Cursor on Target Gateway
 *********************************
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/atak_screenshot.png?token=GHSAT0AAAAAAB5KT72KYMKM7HC3VWKFNTQAZCIXEJQ
    :alt: Screenshot of DMRCOT in ATAK.
 
 The DMR to Cursor on Target Gateway (DMRCOT) transforms Tait DMR Unit Information into 
 Cursor on Target (CoT) for display on `TAK Products <https://tak.gov/>`_ such as ATAK, 
 WinTAK & iTAK.
 
 Concept of Operations
 =====================
 DMRCOT reads Tait DMR subscriber radio positioning information from a DMR NC.
 
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png?token=GHSAT0AAAAAAB5KT72KJV6UBJNG6KLWKZTYZCIXFQA
    :alt: DMRCOT Concept of Operations (CONOP).
    :target: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/dmrcot_conop.png
 
 
 Install
 =======
 DMRCOT functionality is provided via a command-line tool named ``dmrcot``. 
@@ -152,10 +152,10 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 
 A PyTAK Project
 ===============
-.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png
+.. image:: https://raw.githubusercontent.com/snstac/dmrcot/main/docs/pytak_logo-256x264.png?token=GHSAT0AAAAAAB5KT72LUEKHWJ464J3XTTLUZCIXGAA
     :alt: PyTAK Logo
     :target: https://github.com/snstac/pytak
```

### Comparing `dmrcot-1.0.1/setup.py` & `dmrcot-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import os
 import sys
 
 import setuptools
 
 __title__ = "dmrcot"
-__version__ = "1.0.1"
+__version__ = "1.0.3"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 __description__ = "DMR Trunking Node Controller to Cursor on Target Gateway."
 
 
 def publish():
```

