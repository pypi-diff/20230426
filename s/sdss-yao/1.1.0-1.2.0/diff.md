# Comparing `tmp/sdss_yao-1.1.0.tar.gz` & `tmp/sdss_yao-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_yao-1.1.0.tar", max compression
+gzip compressed data, was "sdss_yao-1.2.0.tar", max compression
```

## Comparing `sdss_yao-1.1.0.tar` & `sdss_yao-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1504 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/LICENSE.md
--rw-r--r--   0        0        0      386 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/README.md
--rw-r--r--   0        0        0     2317 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      450 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/__init__.py
--rw-r--r--   0        0        0     1410 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/__main__.py
--rw-r--r--   0        0        0     4797 2023-04-13 21:35:38.776322 sdss_yao-1.1.0/yao/actor.py
--rw-r--r--   0        0        0     6680 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/alerts.py
--rw-r--r--   0        0        0     4893 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/commands.py
--rw-r--r--   0        0        0     3831 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/controller.py
--rw-r--r--   0        0        0    17514 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/delegate.py
--rw-r--r--   0        0        0    32902 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra.acf
--rw-r--r--   0        0        0    49124 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v2.acf
--rw-r--r--   0        0        0    49106 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v3.acf
--rw-r--r--   0        0        0    55310 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v4.acf
--rw-r--r--   0        0        0    57565 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v5.acf
--rw-r--r--   0        0        0    55553 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v6.acf
--rw-r--r--   0        0        0     1258 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/README.md
--rw-r--r--   0        0        0     2649 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/schema.json
--rw-r--r--   0        0        0     2136 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/etc/yao.yml
--rw-r--r--   0        0        0     1062 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/exceptions.py
--rw-r--r--   0        0        0    15317 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/mech_commands.py
--rw-r--r--   0        0        0    19483 2023-04-13 21:35:38.780322 sdss_yao-1.1.0/yao/mech_controller.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sdss_yao-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-26 18:40:31.719757 sdss_yao-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0      386 2023-04-26 18:40:31.719757 sdss_yao-1.2.0/README.md
+-rw-r--r--   0        0        0     2317 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/__init__.py
+-rw-r--r--   0        0        0     1410 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/__main__.py
+-rw-r--r--   0        0        0     4797 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/actor.py
+-rw-r--r--   0        0        0     6680 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/alerts.py
+-rw-r--r--   0        0        0     4893 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/commands.py
+-rw-r--r--   0        0        0     3831 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/controller.py
+-rw-r--r--   0        0        0    17514 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/delegate.py
+-rw-r--r--   0        0        0    32902 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/etc/BOSS_extra.acf
+-rw-r--r--   0        0        0    49124 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v2.acf
+-rw-r--r--   0        0        0    49106 2023-04-26 18:40:31.723757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v3.acf
+-rw-r--r--   0        0        0    55310 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v4.acf
+-rw-r--r--   0        0        0    57565 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v5.acf
+-rw-r--r--   0        0        0    55553 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v6.acf
+-rw-r--r--   0        0        0    55599 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v8.acf
+-rw-r--r--   0        0        0     1258 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/README.md
+-rw-r--r--   0        0        0     2649 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/schema.json
+-rw-r--r--   0        0        0     2136 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/etc/yao.yml
+-rw-r--r--   0        0        0     1062 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/exceptions.py
+-rw-r--r--   0        0        0    15317 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/mech_commands.py
+-rw-r--r--   0        0        0    19483 2023-04-26 18:40:31.727757 sdss_yao-1.2.0/yao/mech_controller.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sdss_yao-1.2.0/PKG-INFO
```

### Comparing `sdss_yao-1.1.0/LICENSE.md` & `sdss_yao-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/pyproject.toml` & `sdss_yao-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-yao"
-version = "1.1.0"
+version = "1.2.0"
 description = "BOSS spectrograph actor that uses an STA Archon controller"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Aidan Gray <Aidan.Gray@idg.jhu.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/yao"
 repository = "https://github.com/sdss/yao"
 documentation = "https://sdss-yao.readthedocs.org"
```

### Comparing `sdss_yao-1.1.0/yao/__main__.py` & `sdss_yao-1.2.0/yao/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/actor.py` & `sdss_yao-1.2.0/yao/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/alerts.py` & `sdss_yao-1.2.0/yao/alerts.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/commands.py` & `sdss_yao-1.2.0/yao/commands.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/controller.py` & `sdss_yao-1.2.0/yao/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/delegate.py` & `sdss_yao-1.2.0/yao/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v2.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v2.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v3.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v3.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v4.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v4.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v5.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v5.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/BOSS_extra_purge_erase_v6.acf` & `sdss_yao-1.2.0/yao/etc/BOSS_extra_purge_erase_v6.acf`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/README.md` & `sdss_yao-1.2.0/yao/etc/README.md`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/schema.json` & `sdss_yao-1.2.0/yao/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/etc/yao.yml` & `sdss_yao-1.2.0/yao/etc/yao.yml`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
   template: 'sdR-{ccd}-{exposure_no:08d}.fit.gz'
 
 checksum:
   write: true
   mode: sha1
 
 archon:
-  acf_file: BOSS_extra_purge_erase_v6.acf
+  acf_file: BOSS_extra_purge_erase_v8.acf
 
 timeouts:
   controller_connect: 5
   write_config_timeout: 2
   write_config_delay: 0.0001
   expose_timeout: 2
   readout_expected: 40
```

### Comparing `sdss_yao-1.1.0/yao/exceptions.py` & `sdss_yao-1.2.0/yao/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/mech_commands.py` & `sdss_yao-1.2.0/yao/mech_commands.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/yao/mech_controller.py` & `sdss_yao-1.2.0/yao/mech_controller.py`

 * *Files identical despite different names*

### Comparing `sdss_yao-1.1.0/PKG-INFO` & `sdss_yao-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-yao
-Version: 1.1.0
+Version: 1.2.0
 Summary: BOSS spectrograph actor that uses an STA Archon controller
 Home-page: https://github.com/sdss/yao
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.12
```

