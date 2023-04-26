# Comparing `tmp/frat_brain-1.3.7.tar.gz` & `tmp/frat_brain-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.3.7.tar", max compression
+gzip compressed data, was "frat_brain-1.4.0.tar", max compression
```

## Comparing `frat_brain-1.3.7.tar` & `frat_brain-1.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.3.7/LICENSE
--rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.3.7/README.md
--rw-r--r--   0        0        0    53941 2023-04-24 16:58:06.275544 frat_brain-1.3.7/fRAT/__main__.py
--rw-r--r--   0        0        0       22 2023-04-24 16:55:00.522387 frat_brain-1.3.7/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.3.7/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.3.7/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4291 2023-04-24 16:58:42.676825 frat_brain-1.3.7/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.3.7/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17981 2023-04-24 16:59:58.274205 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.3.7/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.3.7/fRAT/nogui.py
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.3.7/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.3.7/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.3.7/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.3.7/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.3.7/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.3.7/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22288 2023-04-24 16:45:56.879209 frat_brain-1.3.7/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.3.7/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.3.7/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.3.7/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.3.7/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.3.7/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.3.7/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.3.7/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.3.7/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.3.7/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.3.7/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.3.7/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36718 2023-04-24 17:03:51.405210 frat_brain-1.3.7/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.3.7/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.3.7/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.3.7/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.3.7/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.3.7/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.3.7/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.3.7/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-04-24 17:02:53.370793 frat_brain-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.3.7/setup.py
--rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.4.0/README.md
+-rw-r--r--   0        0        0    53941 2023-04-24 16:58:06.275544 frat_brain-1.4.0/fRAT/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-26 15:19:49.684640 frat_brain-1.4.0/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.4.0/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.4.0/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4291 2023-04-24 16:58:42.676825 frat_brain-1.4.0/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.4.0/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17981 2023-04-24 16:59:58.274205 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.4.0/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.4.0/fRAT/nogui.py
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.4.0/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.4.0/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.4.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.4.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.4.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.4.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.4.0/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.4.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.4.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.4.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.4.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.4.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.4.0/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.4.0/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.4.0/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.4.0/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.4.0/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.4.0/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.4.0/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.4.0/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.4.0/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.4.0/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.4.0/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.4.0/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.4.0/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.4.0/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-04-26 15:20:04.978955 frat_brain-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.4.0/setup.py
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.4.0/PKG-INFO
```

### Comparing `frat_brain-1.3.7/LICENSE` & `frat_brain-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/README.md` & `frat_brain-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/__main__.py` & `frat_brain-1.4.0/fRAT/__main__.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/images/fRAT.gif` & `frat_brain-1.4.0/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/nogui.py` & `frat_brain-1.4.0/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 16:45:54 2023 UTC, .py size: 36654 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-00000000: 6f0d 0d0a 0000 0000 42b2 4664 2e8f 0000  o.......B.Fd....
+00000000: 6f0d 0d0a 0000 0000 a8b6 4664 6f8f 0000  o.........Fdo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c08 6d09 5a0a 0100 6400 6401 6c0b  d.l.m.Z...d.d.l.
 00000080: 5a0c 6400 6401 6c0d 5a0e 6400 6401 6c0f  Z.d.d.l.Z.d.d.l.
 00000090: 5a10 6400 6401 6c11 5a12 6400 6401 6c13  Z.d.d.l.Z.d.d.l.
 000000a0: 5a14 6400 6404 6c15 6d16 5a16 0100 6400  Z.d.d.l.m.Z...d.
 000000b0: 6405 6c17 6d18 5a19 0100 6400 6406 6c1a  d.l.m.Z...d.d.l.
-000000c0: 6d1b 5a1b 0100 6400 6401 6c17 5a17 6517  m.Z...d.d.l.Z.e.
-000000d0: a01c 6407 a101 0100 6408 6409 6c1d 6d1e  ..d.....d.d.l.m.
-000000e0: 5a1e 0100 4700 640a 640b 8400 640b 8302  Z...G.d.d...d...
+000000c0: 6d1b 5a1b 0100 6407 6408 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
+000000d0: 0100 6400 6401 6c17 5a17 6517 a01e 6409  ..d.d.l.Z.e...d.
+000000e0: a101 0100 4700 640a 640b 8400 640b 8302  ....G.d.d...d...
 000000f0: 5a1f 4700 640c 640d 8400 640d 651f 8303  Z.G.d.d...d.e...
 00000100: 5a20 4700 640e 640f 8400 640f 651f 8303  Z G.d.d...d.e...
 00000110: 5a21 4700 6410 6411 8400 6411 651f 8303  Z!G.d.d...d.e...
 00000120: 5a22 4700 6412 6413 8400 6413 651f 8303  Z"G.d.d...d.e...
 00000130: 5a23 4700 6414 6415 8400 6415 651f 8303  Z#G.d.d...d.e...
 00000140: 5a24 6401 5300 2916 e900 0000 004e a901  Z$d.S.)......N..
 00000150: da04 676c 6f62 2901 da04 5061 7468 2901  ..glob)...Path).
 00000160: da08 706c 6f74 7469 6e67 2901 da06 7079  ..plotting)...py
-00000170: 706c 6f74 2901 da05 496d 6167 65da 0361  plot)...Image..a
-00000180: 6767 e901 0000 0029 01da 0555 7469 6c73  gg.....)...Utils
+00000170: 706c 6f74 2901 da05 496d 6167 65e9 0100  plot)...Image...
+00000180: 0000 2901 da05 5574 696c 73da 0361 6767  ..)...Utils..agg
 00000190: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 000001a0: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
 000001b0: 5a01 6400 5a02 6401 5a03 6504 6402 6403  Z.d.Z.d.Z.e.d.d.
 000001c0: 8400 8301 5a05 6506 6404 6405 8400 8301  ....Z.e.d.d.....
 000001d0: 5a07 6506 6406 6407 8400 8301 5a08 6506  Z.e.d.d.....Z.e.
 000001e0: 6408 6409 8400 8301 5a09 6401 5300 290a  d.d.....Z.d.S.).
 000001f0: da07 4669 6775 7265 734e 6304 0000 0000  ..FiguresNc.....
@@ -63,15 +63,15 @@
 000003e0: 0a55 7369 6e67 207a 1820 6461 7461 2074  .Using z. data t
 000003f0: 6f20 6372 6561 7465 2066 6967 7572 6573  o create figures
 00000400: 2e7a 1c0a 2d2d 2d20 4272 6169 6e20 6772  .z..--- Brain gr
 00000410: 6964 2063 7265 6174 696f 6e20 2d2d 2d7a  id creation ---z
 00000420: 1d0a 2d2d 2d20 5669 6f6c 696e 2070 6c6f  ..--- Violin plo
 00000430: 7420 6372 6561 7469 6f6e 202d 2d2d 7a14  t creation ---z.
 00000440: 4669 6775 7265 732f 5669 6f6c 696e 5f70  Figures/Violin_p
-00000450: 6c6f 7473 291d da06 636f 6e66 6967 720a  lots)...configr.
+00000450: 6c6f 7473 291d da06 636f 6e66 6967 7209  lots)...configr.
 00000460: 0000 00da 1572 6561 645f 636f 6d62 696e  .....read_combin
 00000470: 6564 5f72 6573 756c 7473 da02 6f73 da06  ed_results..os..
 00000480: 6765 7463 7764 da0e 6176 6572 6167 696e  getcwd..averagin
 00000490: 675f 7479 7065 da04 7061 7468 da06 6578  g_type..path..ex
 000004a0: 6973 7473 da08 6d61 6b65 6469 7273 da0b  ists..makedirs..
 000004b0: 7361 7665 5f63 6f6e 6669 67da 0772 6570  save_config..rep
 000004c0: 6c61 6365 da05 6c6f 7765 72da 0776 6572  lace..lower..ver
@@ -146,15 +146,15 @@
 00000910: 2c7d 720f 0000 00fa 0127 7245 0000 007a  ,}r......'rE...z
 00000920: 0846 6967 7572 6573 2f7a 0273 2ffa 012f  .Figures/z.s/../
 00000930: 720f 0000 00fa 042e 706e 67e9 0300 0000  r.......png.....
 00000940: 46a9 04da 0668 6569 6768 74da 0577 6964  F....height..wid
 00000950: 7468 721f 0000 005a 096c 696d 6974 7369  thr....Z.limitsi
 00000960: 7a65 fa04 2e73 7667 7a06 5361 7665 6420  ze...svgz.Saved 
 00000970: 290a 721d 0000 00da 0272 65da 0373 7562  ).r......re..sub
-00000980: 720a 0000 0072 2900 0000 da05 7469 746c  r....r).....titl
+00000980: 7209 0000 0072 2900 0000 da05 7469 746c  r....r).....titl
 00000990: 65da 0473 6176 65da 0a70 6c6f 745f 7363  e..save..plot_sc
 000009a0: 616c 6572 1f00 0000 7220 0000 0029 0872  aler....r ...).r
 000009b0: 4000 0000 723f 0000 00da 0666 6f6c 6465  @...r?.....folde
 000009c0: 725a 0a63 6861 7274 5f74 7970 6572 1400  rZ.chart_typer..
 000009d0: 0000 da0c 7265 706c 6163 656d 656e 7473  ....replacements
 000009e0: da03 6f6c 64da 036e 6577 7236 0000 0072  ..old..newr6...r
 000009f0: 3600 0000 7237 0000 00da 0b66 6967 7572  6...r7.....figur
@@ -198,23 +198,23 @@
 00000c50: 74da 0172 da04 4d65 616e da06 566f 7865  t..r..Mean..Voxe
 00000c60: 6c73 2903 da03 5f70 73da 045f 7261 777a  ls)..._ps.._rawz
 00000c70: 052e 6a73 6f6e 7201 0000 007a 0a73 7562  ..jsonr....z.sub
 00000c80: 2d5b 302d 395d 2ae9 0200 0000 da03 524f  -[0-9]*.......RO
 00000c90: 49da 0b76 6f78 656c 5f76 616c 7565 2903  I..voxel_value).
 00000ca0: da07 6964 5f76 6172 73da 0876 6172 5f6e  ..id_vars..var_n
 00000cb0: 616d 65da 0a76 616c 7565 5f6e 616d 6572  ame..value_namer
-00000cc0: 0900 0000 5a0c 766f 7865 6c5f 616d 6f75  ....Z.voxel_amou
+00000cc0: 0800 0000 5a0c 766f 7865 6c5f 616d 6f75  ....Z.voxel_amou
 00000cd0: 6e74 5429 01da 0769 6e70 6c61 6365 291c  ntT)...inplace).
 00000ce0: da02 7064 da09 4461 7461 4672 616d 65da  ..pd..DataFrame.
 00000cf0: 046c 6973 74da 0666 696c 7465 72da 0f70  .list..filter..p
 00000d00: 6172 616d 6574 6572 5f64 6963 7431 da15  arameter_dict1..
 00000d10: 6869 7374 6f67 7261 6d5f 6669 675f 785f  histogram_fig_x_
 00000d20: 6661 6365 74da 1568 6973 746f 6772 616d  facet..histogram
 00000d30: 5f66 6967 5f79 5f66 6163 6574 da04 6f70  _fig_y_facet..op
-00000d40: 656e 720a 0000 00da 1164 6963 745f 746f  enr......dict_to
+00000d40: 656e 7209 0000 00da 1164 6963 745f 746f  enr......dict_to
 00000d50: 5f64 6174 6166 7261 6d65 da04 6a73 6f6e  _dataframe..json
 00000d60: da04 6c6f 6164 da03 6c6f 63da 084b 6579  ..load..loc..Key
 00000d70: 4572 726f 7272 1600 0000 7219 0000 00da  Errorr....r.....
 00000d80: 0862 6173 656e 616d 65da 0672 7370 6c69  .basename..rspli
 00000d90: 74da 0373 7472 721e 0000 00da 0763 6f6c  t..strr......col
 00000da0: 756d 6e73 da04 696c 6f63 da0a 496e 6465  umns..iloc..Inde
 00000db0: 7845 7272 6f72 724e 0000 00da 0766 696e  xErrorrN.....fin
@@ -222,15 +222,15 @@
 00000dd0: 6c74 da06 6472 6f70 6e61 2910 7214 0000  lt..dropna).r...
 00000de0: 00da 056a 736f 6e73 da0b 636f 6d62 696e  ...jsons..combin
 00000df0: 6564 5f64 66da 0964 6174 615f 7479 7065  ed_df..data_type
 00000e00: da0f 636f 6d62 696e 6564 5f72 6177 5f64  ..combined_raw_d
 00000e10: 66da 0e73 6967 6e69 665f 636f 6c75 6d6e  f..signif_column
 00000e20: 73da 096a 736f 6e5f 6669 6c65 da01 665a  s..json_file..fZ
 00000e30: 0c63 7572 7265 6e74 5f6a 736f 6e5a 0a64  .current_jsonZ.d
-00000e40: 656c 696d 6574 6572 73da 0e6a 736f 6e5f  elimeters..json_
+00000e40: 656c 696d 6574 6572 735a 0e6a 736f 6e5f  elimetersZ.json_
 00000e50: 6669 6c65 5f6e 616d 655a 0964 656c 696d  file_nameZ.delim
 00000e60: 6574 6572 5a12 636f 6d62 696e 6564 5f64  eterZ.combined_d
 00000e70: 665f 7365 6172 6368 da06 636f 6c75 6d6e  f_search..column
 00000e80: 5a09 6d65 616e 5f64 6174 615a 0a76 6f78  Z.mean_dataZ.vox
 00000e90: 656c 5f64 6174 6172 3600 0000 7236 0000  el_datar6...r6..
 00000ea0: 0072 3700 0000 da1a 6c6f 6164 5f61 6e64  .r7.....load_and
 00000eb0: 5f72 6573 7472 7563 7475 7265 5f6a 736f  _restructure_jso
@@ -243,15 +243,15 @@
 00000f20: 2e6c 6f61 645f 616e 645f 7265 7374 7275  .load_and_restru
 00000f30: 6374 7572 655f 6a73 6f6e 7329 0ada 085f  cture_jsons)..._
 00000f40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000f50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000f60: 5f72 1400 0000 da0b 636c 6173 736d 6574  _r......classmet
 00000f70: 686f 6472 3800 0000 da0c 7374 6174 6963  hodr8.....static
 00000f80: 6d65 7468 6f64 7244 0000 0072 5700 0000  methodrD...rW...
-00000f90: 7287 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
+00000f90: 7286 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
 00000fa0: 3600 0000 7237 0000 0072 0b00 0000 1900  6...r7...r......
 00000fb0: 0000 7314 0000 0008 0004 0102 020a 0102  ..s.............
 00000fc0: 2e0a 0102 0f0a 0102 170e 0172 0b00 0000  ...........r....
 00000fd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000fe0: 0003 0000 0040 0000 0073 6000 0000 6500  .....@...s`...e.
 00000ff0: 5a01 6400 5a02 6503 6401 6402 8400 8301  Z.d.Z.e.d.d.....
 00001000: 5a04 6503 6403 6404 8400 8301 5a05 6503  Z.e.d.d.....Z.e.
@@ -288,15 +288,15 @@
 000011f0: 645f 7265 7375 6c74 73fa 124f 7665 7261  d_results..Overa
 00001200: 6c6c 2f4e 4946 5449 5f52 4f49 2f7a 022f  ll/NIFTI_ROI/z./
 00001210: 2ada 012a 7a15 2f46 6967 7572 6573 2f42  *..*z./Figures/B
 00001220: 7261 696e 5f67 7269 6473 2f72 0f00 0000  rain_grids/r....
 00001230: fa07 2e6e 6969 2e67 7a7a 195f 7769 7468  ...nii.gzz._with
 00001240: 696e 5f72 6f69 5f73 6361 6c65 642e 6e69  in_roi_scaled.ni
 00001250: 692e 677a da01 0a29 0c72 1600 0000 7217  i.gz...).r....r.
-00001260: 0000 0072 0a00 0000 7229 0000 0072 1400  ...r....r)...r..
+00001260: 0000 0072 0900 0000 7229 0000 0072 1400  ...r....r)...r..
 00001270: 0000 7218 0000 00da 1173 7461 7469 7374  ..r......statist
 00001280: 6963 5f6f 7074 696f 6e73 7203 0000 0072  ic_optionsr....r
 00001290: 2c00 0000 da09 6d6f 7665 5f66 696c 6572  ,.....move_filer
 000012a0: 1f00 0000 7220 0000 0029 0a72 3000 0000  ....r ...).r0...
 000012b0: 7234 0000 005a 1069 6e64 6976 5f62 7261  r4...Z.indiv_bra
 000012c0: 696e 735f 6469 72da 1073 7461 7469 7374  ins_dir..statist
 000012d0: 6963 5f6c 6162 656c 73da 0973 7562 666f  ic_labels..subfo
@@ -333,35 +333,35 @@
 000014c0: 0100 7c00 a00c 7c05 8800 7c09 7c06 7c07  ..|...|...|.|.|.
 000014d0: 7c08 7c03 7c0e 7c0f 7c10 7c0b 7c0a 8801  |.|.|.|.|.|.|...
 000014e0: a10d 7d06 7c0e 6400 7501 72a8 0900 7c06  ..}.|.d.u.r...|.
 000014f0: 5300 740d 7c0f 8301 6417 1900 7d0f 7c0f  S.t.|...d...}.|.
 00001500: 6401 1900 7d0e 7c00 6a07 6a0a 72c7 740b  d...}.|.j.j.r.t.
 00001510: 6418 740e 7c0f 6401 1900 8301 9b00 6419  d.t.|.d.......d.
 00001520: 7c0f 6402 1900 9b00 641a 9d05 8301 0100  |.d.....d.......
-00001530: 7167 291b 4e72 0100 0000 7209 0000 0072  qg).Nr....r....r
+00001530: 7167 291b 4e72 0100 0000 7208 0000 0072  qg).Nr....r....r
 00001540: 5900 0000 6301 0000 0000 0000 0000 0000  Y...c...........
 00001550: 0002 0000 0008 0000 0013 0000 0073 2800  .............s(.
 00001560: 0000 6700 7c00 5d10 7d01 7400 6400 8801  ..g.|.].}.t.d...
 00001570: 9b00 6401 7c01 9b00 8800 9b00 9d05 8301  ..d.|...........
-00001580: 7202 7c01 9102 7102 5300 2902 728d 0000  r.|...q.S.).r...
+00001580: 7202 7c01 9102 7102 5300 2902 728c 0000  r.|...q.S.).r...
 00001590: 0072 4700 0000 7202 0000 00a9 02da 022e  .rG...r.........
-000015a0: 30da 036a 736e a902 7296 0000 0072 9400  0..jsn..r....r..
+000015a0: 30da 036a 736e a902 7295 0000 0072 9300  0..jsn..r....r..
 000015b0: 0000 7236 0000 0072 3700 0000 da0a 3c6c  ..r6...r7.....<l
 000015c0: 6973 7463 6f6d 703e d600 0000 7302 0000  istcomp>....s...
 000015d0: 0028 007a 2342 7261 696e 4772 6964 2e73  .(.z#BrainGrid.s
 000015e0: 6574 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c  etup.<locals>.<l
-000015f0: 6973 7463 6f6d 703e 2902 7209 0000 0072  istcomp>).r....r
+000015f0: 6973 7463 6f6d 703e 2902 7208 0000 0072  istcomp>).r....r
 00001600: 6000 0000 e920 0000 00e9 1000 0000 e90f  `.... ..........
 00001610: 0000 007a 0e66 6967 7572 652e 6669 6773  ...z.figure.figs
 00001620: 697a 6567 7b14 ae47 e17a 843f 7a15 6669  izeg{..G.z.?z.fi
 00001630: 6775 7265 2e73 7562 706c 6f74 2e77 7370  gure.subplot.wsp
 00001640: 6163 65e7 9a99 9999 9999 b93f 7a15 6669  ace........?z.fi
 00001650: 6775 7265 2e73 7562 706c 6f74 2e68 7370  gure.subplot.hsp
 00001660: 6163 6529 0272 5c00 0000 da06 4d65 6469  ace).r\.....Medi
-00001670: 616e 5472 0f00 0000 728f 0000 00e9 6400  anTr....r.....d.
+00001670: 616e 5472 0f00 0000 728e 0000 00e9 6400  anTr....r.....d.
 00001680: 0000 da0b 5f73 616d 655f 7363 616c 657a  ...._same_scalez
 00001690: 0753 6176 696e 6720 7a07 2074 6162 6c65  .Saving z. table
 000016a0: 2ee9 ffff ffff 7a16 4d61 7869 6d75 6d20  ......z.Maximum 
 000016b0: 524f 4920 7661 6c75 6520 6f66 3a20 7a21  ROI value of: z!
 000016c0: 2073 6565 6e20 666f 7220 7061 7261 6d65   seen for parame
 000016d0: 7465 7220 636f 6d62 696e 6174 696f 6e3a  ter combination:
 000016e0: 207a 2d2e 2043 7265 6174 696e 6720 6669   z-. Creating fi
@@ -372,26 +372,26 @@
 00001730: 7461 626c 655f 7365 7475 70da 0370 6c74  table_setup..plt
 00001740: da08 7263 5061 7261 6d73 7214 0000 00da  ..rcParamsr.....
 00001750: 1362 7261 696e 5f66 6967 5f76 616c 7565  .brain_fig_value
 00001760: 5f6d 6178 da13 6272 6169 6e5f 6669 675f  _max..brain_fig_
 00001770: 7661 6c75 655f 6d69 6e72 1f00 0000 7220  value_minr....r 
 00001780: 0000 00da 0a6d 616b 655f 7461 626c 65da  .....make_table.
 00001790: 0673 6f72 7465 64da 0572 6f75 6e64 2911  .sorted..round).
-000017a0: 7230 0000 00da 0264 6672 9600 0000 7295  r0.....dfr....r.
-000017b0: 0000 0072 9400 0000 da0e 6261 7365 5f65  ...r......base_e
-000017c0: 7874 5f63 6c65 616e 7297 0000 00da 0a6a  xt_cleanr......j
+000017a0: 7230 0000 00da 0264 6672 9500 0000 7294  r0.....dfr....r.
+000017b0: 0000 0072 9300 0000 da0e 6261 7365 5f65  ...r......base_e
+000017c0: 7874 5f63 6c65 616e 7296 0000 00da 0a6a  xt_cleanr......j
 000017d0: 736f 6e5f 6172 7261 79da 0f63 7269 7469  son_array..criti
 000017e0: 6361 6c5f 7061 7261 6d73 da09 6365 6c6c  cal_params..cell
 000017f0: 5f6e 756d 73da 0b79 5f61 7869 735f 7369  _nums..y_axis_si
 00001800: 7a65 da0b 785f 6178 6973 5f73 697a 655a  ze..x_axis_sizeZ
 00001810: 1262 7261 696e 5f74 6162 6c65 5f78 5f73  .brain_table_x_s
 00001820: 697a 655a 1262 7261 696e 5f74 6162 6c65  izeZ.brain_table
 00001830: 5f79 5f73 697a 65da 0476 6d61 78da 0c76  _y_size..vmax..v
 00001840: 6d61 785f 7374 6f72 6167 65da 0476 6d69  max_storage..vmi
-00001850: 6e72 3600 0000 729c 0000 0072 3700 0000  nr6...r....r7...
+00001850: 6e72 3600 0000 729b 0000 0072 3700 0000  nr6...r....r7...
 00001860: 722c 0000 00ce 0000 0073 5200 0000 2402  r,.......sR...$.
 00001870: 0401 0c02 1403 1202 0802 0601 0802 0402  ................
 00001880: 0e02 0a01 0a01 0802 0c01 0a01 0802 0401  ................
 00001890: 0802 0401 0202 1001 0402 0601 1801 0801  ................
 000018a0: 0802 1001 0e02 0c01 0401 04fe 0804 0201  ................
 000018b0: 040c 0cf8 0801 0802 0201 1c01 04ff 02e8  ................
 000018c0: 7a0f 4272 6169 6e47 7269 642e 7365 7475  z.BrainGrid.setu
@@ -421,26 +421,26 @@
 00001a40: 088d 0201 0071 047c 00a0 167c 067c 037c  .....q.|...|.|.|
 00001a50: 0b7c 0c7c 11a1 0501 007c 006a 106a 1772  .|.|.....|.j.j.r
 00001a60: bd74 04a0 18a1 0001 0074 046a 1964 097c  .t.......t.j.d.|
 00001a70: 079b 0064 0a7c 019b 0064 0b9d 057c 006a  ...d.|...d...|.j
 00001a80: 106a 1a64 0c64 0d8d 0301 0074 046a 1964  .j.d.d.....t.j.d
 00001a90: 097c 079b 0064 0a7c 019b 0064 0e9d 057c  .|...d.|...d...|
 00001aa0: 006a 106a 1a64 0c64 0d8d 0301 0074 04a0  .j.j.d.d.....t..
-00001ab0: 1ba1 0001 007c 0453 0029 0f4e 7209 0000  .....|.S.).Nr...
+00001ab0: 1ba1 0001 007c 0453 0029 0f4e 7208 0000  .....|.S.).Nr...
 00001ac0: 00da 0472 6f77 73da 056f 7264 6572 7201  ...rows..orderr.
 00001ad0: 0000 00da 0463 6f6c 73da 0676 616c 7565  .....cols..value
 00001ae0: 7372 0e00 0000 a901 da08 666f 6e74 7369  sr........fontsi
 00001af0: 7a65 7a14 4669 6775 7265 732f 4272 6169  zez.Figures/Brai
 00001b00: 6e5f 6772 6964 732f 7247 0000 0072 4800  n_grids/rG...rH.
 00001b10: 0000 da05 7469 6768 7429 02da 0364 7069  ....tight)...dpi
 00001b20: 5a0b 6262 6f78 5f69 6e63 6865 7372 4d00  Z.bbox_inchesrM.
 00001b30: 0000 291c da09 656e 756d 6572 6174 65da  ..)...enumerate.
 00001b40: 0f73 6176 655f 6272 6169 6e5f 696d 6773  .save_brain_imgs
 00001b50: da05 6d70 696d 67da 0669 6d72 6561 6472  ..mpimg..imreadr
-00001b60: a900 0000 da07 7375 6270 6c6f 74da 0669  ......subplot..i
+00001b60: a800 0000 da07 7375 6270 6c6f 74da 0669  ......subplot..i
 00001b70: 6d73 686f 77da 0367 6361 5a0a 7365 745f  mshow..gcaZ.set_
 00001b80: 7974 6963 6b73 723c 0000 0072 3a00 0000  yticksr<...r:...
 00001b90: 5a0e 7365 745f 7469 636b 6c61 6265 6c73  Z.set_ticklabels
 00001ba0: da0a 7365 745f 7874 6963 6b73 7239 0000  ..set_xticksr9..
 00001bb0: 00da 036c 656e 7250 0000 0072 1400 0000  ...lenrP...r....
 00001bc0: da16 6272 6169 6e5f 7461 626c 655f 636f  ..brain_table_co
 00001bd0: 6c5f 6c61 6265 6c73 7276 0000 00da 0e70  l_labelsrv.....p
@@ -448,22 +448,22 @@
 00001bf0: 6c61 6265 6cda 1662 7261 696e 5f74 6162  label..brain_tab
 00001c00: 6c65 5f72 6f77 5f6c 6162 656c 73da 156c  le_row_labels..l
 00001c10: 6162 656c 5f62 6c61 6e6b 5f63 656c 6c5f  abel_blank_cell_
 00001c20: 6178 6573 da12 6272 6169 6e5f 7469 6768  axes..brain_tigh
 00001c30: 745f 6c61 796f 7574 da0c 7469 6768 745f  t_layout..tight_
 00001c40: 6c61 796f 7574 da07 7361 7665 6669 67da  layout..savefig.
 00001c50: 0870 6c6f 745f 6470 6972 2e00 0000 2914  .plot_dpir....).
-00001c60: 7230 0000 0072 b100 0000 7296 0000 0072  r0...r....r....r
-00001c70: b400 0000 7297 0000 0072 b200 0000 72b3  ....r....r....r.
-00001c80: 0000 0072 9500 0000 72b7 0000 0072 b800  ...r....r....r..
-00001c90: 0000 72b9 0000 0072 b600 0000 72b5 0000  ..r....r....r...
-00001ca0: 0072 9400 0000 da08 6669 6c65 5f6e 756d  .r......file_num
+00001c60: 7230 0000 0072 b000 0000 7295 0000 0072  r0...r....r....r
+00001c70: b300 0000 7296 0000 0072 b100 0000 72b2  ....r....r....r.
+00001c80: 0000 0072 9400 0000 72b6 0000 0072 b700  ...r....r....r..
+00001c90: 0000 72b8 0000 0072 b500 0000 72b4 0000  ..r....r....r...
+00001ca0: 0072 9300 0000 da08 6669 6c65 5f6e 756d  .r......file_num
 00001cb0: 7270 0000 005a 0962 7261 696e 5f69 6d67  rp...Z.brain_img
-00001cc0: da04 6469 6d73 7298 0000 00da 0261 7872  ..dimsr......axr
-00001cd0: 3600 0000 7236 0000 0072 3700 0000 72ad  6...r6...r7...r.
+00001cc0: da04 6469 6d73 7297 0000 00da 0261 7872  ..dimsr......axr
+00001cd0: 3600 0000 7236 0000 0072 3700 0000 72ac  6...r6...r7...r.
 00001ce0: 0000 000d 0100 0073 4a00 0000 1003 0a01  .......sJ.......
 00001cf0: 0801 0401 0afe 0a05 1601 0a01 0802 0a01  ................
 00001d00: 0e01 0a02 0e01 2802 0e01 1e01 02ff 0602  ......(.........
 00001d10: 06fe 2804 0e01 1e01 02ff 0602 06fe 0280  ..(.............
 00001d20: 1204 0802 0801 1a02 0201 06ff 1a02 0201  ................
 00001d30: 06ff 0802 0402 7a14 4272 6169 6e47 7269  ......z.BrainGri
 00001d40: 642e 6d61 6b65 5f74 6162 6c65 630a 0000  d.make_tablec...
@@ -483,41 +483,41 @@
 00001e20: 6a0d 6a0e 7c00 6a0d 6a0f 6602 640b 640c  j.j.|.j.j.f.d.d.
 00001e30: 8d09 7d0e 7c0e 6a10 7c0a 7c00 6a0d 6a11  ..}.|.j.|.|.j.j.
 00001e40: 640d 8d02 0100 7c0e a012 a100 0100 7413  d.....|.......t.
 00001e50: a014 7c0a a101 8f0d 7d0f 7c0f 6a15 5c02  ..|.....}.|.j.\.
 00001e60: 7d10 7d11 5700 6400 0400 0400 8303 0100  }.}.W.d.........
 00001e70: 6e08 3100 7387 7701 0100 0100 0100 5900  n.1.s.w.......Y.
 00001e80: 0100 7c0a 7c07 7c10 7c11 6602 6603 5300  ..|.|.|.|.f.f.S.
-00001e90: 290e 4e72 0f00 0000 7248 0000 0072 8d00  ).Nr....rH...r..
-00001ea0: 0000 7247 0000 0072 8f00 0000 72a4 0000  ..rG...r....r...
-00001eb0: 0072 a500 0000 4654 da02 787a da07 696e  .r....FT..xz..in
+00001e90: 290e 4e72 0f00 0000 7248 0000 0072 8c00  ).Nr....rH...r..
+00001ea0: 0000 7247 0000 0072 8e00 0000 72a3 0000  ..rG...r....r...
+00001eb0: 0072 a400 0000 4654 da02 787a da07 696e  .r....FT..xz..in
 00001ec0: 6665 726e 6f29 085a 0a64 7261 775f 6372  ferno).Z.draw_cr
 00001ed0: 6f73 735a 0861 6e6e 6f74 6174 65da 0863  ossZ.annotate..c
 00001ee0: 6f6c 6f72 6261 725a 0c64 6973 706c 6179  olorbarZ.display
-00001ef0: 5f6d 6f64 6572 b900 0000 72b7 0000 005a  _moder....r....Z
+00001ef0: 5f6d 6f64 6572 b800 0000 72b6 0000 005a  _moder....r....Z
 00001f00: 0a63 7574 5f63 6f6f 7264 73da 0463 6d61  .cut_coords..cma
-00001f10: 7029 0172 c100 0000 2916 da06 6170 7065  p).r....)...appe
+00001f10: 7029 0172 c000 0000 2916 da06 6170 7065  p).r....)...appe
 00001f20: 6e64 da04 6669 6e64 da03 6e69 6272 7100  nd..find..nibrq.
 00001f30: 0000 da09 6765 745f 6664 6174 61da 026e  ....get_fdata..n
 00001f40: 70da 066e 616e 6d61 78da 0b4e 6966 7469  p..nanmax..Nifti
 00001f50: 3149 6d61 6765 da0a 6e61 6e5f 746f 5f6e  1Image..nan_to_n
 00001f60: 756d da06 6166 6669 6e65 da06 6865 6164  um..affine..head
 00001f70: 6572 7205 0000 005a 0970 6c6f 745f 616e  err....Z.plot_an
 00001f80: 6174 7214 0000 00da 0d62 7261 696e 5f78  atr......brain_x
 00001f90: 5f63 6f6f 7264 da0d 6272 6169 6e5f 7a5f  _coord..brain_z_
-00001fa0: 636f 6f72 6472 d200 0000 72d3 0000 0072  coordr....r....r
+00001fa0: 636f 6f72 6472 d100 0000 72d2 0000 0072  coordr....r....r
 00001fb0: 2e00 0000 7207 0000 0072 6e00 0000 da04  ....r....rn.....
 00001fc0: 7369 7a65 2912 7230 0000 0072 7000 0000  size).r0...rp...
-00001fd0: 72b1 0000 0072 9600 0000 72b7 0000 0072  r....r....r....r
-00001fe0: b800 0000 72b9 0000 0072 9700 0000 7295  ....r....r....r.
-00001ff0: 0000 0072 9400 0000 5a08 706e 675f 7061  ...r....Z.png_pa
+00001fd0: 72b0 0000 0072 9500 0000 72b6 0000 0072  r....r....r....r
+00001fe0: b700 0000 72b8 0000 0072 9600 0000 7294  ....r....r....r.
+00001ff0: 0000 0072 9300 0000 5a08 706e 675f 7061  ...r....Z.png_pa
 00002000: 7468 5a0a 6e69 6674 695f 7061 7468 da05  thZ.nifti_path..
-00002010: 6272 6169 6e72 9800 0000 da04 706c 6f74  brainr......plot
+00002010: 6272 6169 6e72 9700 0000 da04 706c 6f74  brainr......plot
 00002020: da02 696d 724c 0000 0072 4b00 0000 7236  ..imrL...rK...r6
-00002030: 0000 0072 3600 0000 7237 0000 0072 c300  ...r6...r7...r..
+00002030: 0000 0072 3600 0000 7237 0000 0072 c200  ...r6...r7...r..
 00002040: 0000 3801 0000 732c 0000 0010 040a 0114  ..8...s,........
 00002050: 021e 020a 0208 010a 0214 040a 031c 0106  ................
 00002060: 0208 0104 010e 0102 0106 fc12 0508 010c  ................
 00002070: 020c 011c ff0e 037a 1942 7261 696e 4772  .......z.BrainGr
 00002080: 6964 2e73 6176 655f 6272 6169 6e5f 696d  id.save_brain_im
 00002090: 6773 6302 0000 0000 0000 0000 0000 0011  gsc.............
 000020a0: 0000 0008 0000 0043 0000 0073 be01 0000  .......C...s....
@@ -549,44 +549,44 @@
 00002240: a005 740e a00f 7c0e 640d 1900 7c0e 6403  ..t...|.d...|.d.
 00002250: 1900 6602 7c0b 7c0a 6602 a102 a101 0100  ..f.|.|.f.......
 00002260: 7173 7c08 7c03 7c0b 7c0a 6604 5300 290e  qs|.|.|.|.f.S.).
 00002270: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
 00002280: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
 00002290: 007c 005d 067d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
 000022a0: 0253 0072 3600 0000 2901 7276 0000 0029  .S.r6...).rv...)
-000022b0: 0272 9a00 0000 da05 7061 7261 6d72 3600  .r......paramr6.
-000022c0: 0000 7236 0000 0072 3700 0000 729d 0000  ..r6...r7...r...
+000022b0: 0272 9900 0000 da05 7061 7261 6d72 3600  .r......paramr6.
+000022c0: 0000 7236 0000 0072 3700 0000 729c 0000  ..r6...r7...r...
 000022d0: 0064 0100 00f3 0200 0000 1400 7a29 4272  .d..........z)Br
 000022e0: 6169 6e47 7269 642e 7461 626c 655f 7365  ainGrid.table_se
 000022f0: 7475 702e 3c6c 6f63 616c 733e 2e3c 6c69  tup.<locals>.<li
-00002300: 7374 636f 6d70 3e72 0100 0000 2903 72eb  stcomp>r....).r.
-00002310: 0000 0072 bd00 0000 72bb 0000 0029 0272  ...r....r....).r
-00002320: bc00 0000 72ba 0000 0072 eb00 0000 7245  ....r....r....rE
-00002330: 0000 0072 bd00 0000 72bc 0000 0072 ba00  ...r....r....r..
-00002340: 0000 7259 0000 0072 bb00 0000 7209 0000  ..rY...r....r...
+00002300: 7374 636f 6d70 3e72 0100 0000 2903 72ea  stcomp>r....).r.
+00002310: 0000 0072 bc00 0000 72ba 0000 0029 0272  ...r....r....).r
+00002320: bb00 0000 72b9 0000 0072 ea00 0000 7245  ....r....r....rE
+00002330: 0000 0072 bc00 0000 72bb 0000 0072 b900  ...r....r....r..
+00002340: 0000 7259 0000 0072 ba00 0000 7208 0000  ..rY...r....r...
 00002350: 0029 1072 1400 0000 da0e 7061 7261 6d65  .).r......parame
-00002360: 7465 725f 6469 6374 72ae 0000 0072 6900  ter_dictr....ri.
-00002370: 0000 72a7 0000 0072 db00 0000 da04 6b65  ..r....r......ke
+00002360: 7465 725f 6469 6374 72ad 0000 0072 6900  ter_dictr....ri.
+00002370: 0000 72a6 0000 0072 da00 0000 da04 6b65  ..r....r......ke
 00002380: 7973 da10 6272 6169 6e5f 7461 626c 655f  ys..brain_table_
 00002390: 636f 6c73 da10 6272 6169 6e5f 7461 626c  cols..brain_tabl
-000023a0: 655f 726f 7773 da05 696e 6465 7872 ca00  e_rows..indexr..
-000023b0: 0000 72c2 0000 0072 7800 0000 7276 0000  ..r....rx...rv..
-000023c0: 0072 df00 0000 da11 7261 7665 6c5f 6d75  .r......ravel_mu
+000023a0: 655f 726f 7773 da05 696e 6465 7872 c900  e_rows..indexr..
+000023b0: 0000 72c1 0000 0072 7800 0000 7276 0000  ..r....rx...rv..
+000023c0: 0072 de00 0000 da11 7261 7665 6c5f 6d75  .r......ravel_mu
 000023d0: 6c74 695f 696e 6465 7829 1172 3000 0000  lti_index).r0...
-000023e0: 72b0 0000 005a 0d75 6e69 7175 655f 7061  r....Z.unique_pa
-000023f0: 7261 6d73 72b4 0000 00da 036b 6579 da06  ramsr......key..
+000023e0: 72af 0000 005a 0d75 6e69 7175 655f 7061  r....Z.unique_pa
+000023f0: 7261 6d73 72b3 0000 00da 036b 6579 da06  ramsr......key..
 00002400: 7061 7261 6d73 5a0b 706c 6f74 5f76 616c  paramsZ.plot_val
 00002410: 7565 735a 0b61 7869 735f 7469 746c 6573  uesZ.axis_titles
-00002420: 72b3 0000 0072 4100 0000 72b6 0000 0072  r....rA...r....r
-00002430: b500 0000 72d4 0000 00da 0966 696c 655f  ....r......file_
+00002420: 72b2 0000 0072 4100 0000 72b5 0000 0072  r....rA...r....r
+00002430: b400 0000 72d3 0000 00da 0966 696c 655f  ....r......file_
 00002440: 6e61 6d65 5a10 7465 6d70 5f6f 7264 6572  nameZ.temp_order
 00002450: 5f73 746f 7265 5a0d 6669 6c65 5f6e 616d  _storeZ.file_nam
 00002460: 655f 726f 775a 0a66 696c 655f 7061 7261  e_rowZ.file_para
 00002470: 6d72 3600 0000 7236 0000 0072 3700 0000  mr6...r6...r7...
-00002480: 72a8 0000 005d 0100 0073 4200 0000 0402  r....]...sB.....
+00002480: 72a7 0000 005d 0100 0073 4200 0000 0402  r....]...sB.....
 00002490: 0401 0c02 1401 0e01 0c01 0402 1001 1002  ................
 000024a0: 1001 06ff 0803 1001 0201 0202 1001 0eff  ................
 000024b0: 1003 1001 1802 0401 1601 0802 1201 1402  ................
 000024c0: 2002 1a01 1202 0c01 1602 0601 08ff 0c03   ...............
 000024d0: 7a15 4272 6169 6e47 7269 642e 7461 626c  z.BrainGrid.tabl
 000024e0: 655f 7365 7475 7063 0600 0000 0000 0000  e_setupc........
 000024f0: 0000 0000 0b00 0000 0700 0000 4300 0000  ............C...
@@ -607,30 +607,30 @@
 000025e0: 0a74 03a0 047c 0764 0266 027c 047c 0366  .t...|.d.f.|.|.f
 000025f0: 02a1 027d 097c 097c 0276 0172 a17c 0964  ...}.|.|.v.r.|.d
 00002600: 026b 0372 a174 05a0 067c 047c 037c 0964  .k.r.t...|.|.|.d
 00002610: 0317 00a1 0301 0074 05a0 077c 06a1 0101  .......t...|....
 00002620: 007c 00a0 08a1 0001 0074 056a 0d7c 006a  .|.......t.j.|.j
 00002630: 0a6a 0e64 0717 007c 0a17 007c 006a 0a6a  .j.d...|...|.j.j
 00002640: 0c64 088d 0201 0071 6a64 0053 0029 0a4e  .d.....qjd.S.).N
-00002650: da03 5247 4272 0100 0000 7209 0000 0029  ..RGBr....r....)
-00002660: 03e9 ff00 0000 72f7 0000 0072 f700 0000  ......r....r....
-00002670: 72bc 0000 0072 bd00 0000 720e 0000 0072  r....r....r....r
-00002680: be00 0000 72ba 0000 0029 0f72 0700 0000  ....r....).r....
-00002690: 7256 0000 0072 c200 0000 72df 0000 0072  rV...r....r....r
-000026a0: f200 0000 72a9 0000 0072 c600 0000 72c7  ....r....r....r.
+00002650: da03 5247 4272 0100 0000 7208 0000 0029  ..RGBr....r....)
+00002660: 03e9 ff00 0000 72f6 0000 0072 f600 0000  ......r....r....
+00002670: 72bb 0000 0072 bc00 0000 720e 0000 0072  r....r....r....r
+00002680: bd00 0000 72b9 0000 0029 0f72 0700 0000  ....r....).r....
+00002690: 7256 0000 0072 c100 0000 72de 0000 0072  rV...r....r....r
+000026a0: f100 0000 72a8 0000 0072 c500 0000 72c6  ....r....r....r.
 000026b0: 0000 00da 136d 616b 655f 6365 6c6c 5f69  .....make_cell_i
 000026c0: 6e76 6973 6962 6c65 7250 0000 0072 1400  nvisiblerP...r..
-000026d0: 0000 72cb 0000 0072 cc00 0000 72cd 0000  ..r....r....r...
-000026e0: 0072 ce00 0000 290b 7230 0000 0072 b300  .r....).r0...r..
-000026f0: 0000 72b4 0000 0072 b600 0000 72b5 0000  ..r....r....r...
-00002700: 0072 d500 0000 7298 0000 00da 0763 6f75  .r....r......cou
+000026d0: 0000 72ca 0000 0072 cb00 0000 72cc 0000  ..r....r....r...
+000026e0: 0072 cd00 0000 290b 7230 0000 0072 b200  .r....).r0...r..
+000026f0: 0000 72b3 0000 0072 b500 0000 72b4 0000  ..r....r....r...
+00002700: 0072 d400 0000 7297 0000 00da 0763 6f75  .r....r......cou
 00002710: 6e74 6572 5a07 785f 7469 746c 655a 0b68  nterZ.x_titleZ.h
 00002720: 6964 6465 6e5f 6365 6c6c 5a07 795f 7469  idden_cellZ.y_ti
 00002730: 746c 6572 3600 0000 7236 0000 0072 3700  tler6...r6...r7.
-00002740: 0000 72cf 0000 008b 0100 0073 2c00 0000  ..r........s,...
+00002740: 0000 72ce 0000 008b 0100 0073 2c00 0000  ..r........s,...
 00002750: 1a03 1802 1401 0802 1201 0a01 0801 1e02  ................
 00002760: 0802 1e01 0601 06ff 0280 1803 1401 1002  ................
 00002770: 1201 0a01 0801 1e02 0280 04f8 7a1f 4272  ............z.Br
 00002780: 6169 6e47 7269 642e 6c61 6265 6c5f 626c  ainGrid.label_bl
 00002790: 616e 6b5f 6365 6c6c 5f61 7865 7363 0000  ank_cell_axesc..
 000027a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
 000027b0: 0000 4300 0000 736c 0000 0074 00a0 01a1  ..C...sl...t....
@@ -638,28 +638,28 @@
 000027d0: 0101 007c 006a 02a0 05a1 00a0 0467 00a1  ...|.j.......g..
 000027e0: 0101 007c 006a 0664 0119 00a0 0764 02a1  ...|.j.d.....d..
 000027f0: 0101 007c 006a 0664 0319 00a0 0764 02a1  ...|.j.d.....d..
 00002800: 0101 007c 006a 0664 0419 00a0 0764 02a1  ...|.j.d.....d..
 00002810: 0101 007c 006a 0664 0519 00a0 0764 02a1  ...|.j.d.....d..
 00002820: 0101 0064 0053 0029 064e da04 6c65 6674  ...d.S.).N..left
 00002830: 46da 0572 6967 6874 da06 626f 7474 6f6d  F..right..bottom
-00002840: da03 746f 7029 0872 a900 0000 72c8 0000  ..top).r....r...
+00002840: da03 746f 7029 0872 a800 0000 72c7 0000  ..top).r....r...
 00002850: 0072 3c00 0000 da09 6765 745f 7861 7869  .r<.....get_xaxi
 00002860: 735a 0973 6574 5f74 6963 6b73 da09 6765  sZ.set_ticks..ge
 00002870: 745f 7961 7869 735a 0673 7069 6e65 73da  t_yaxisZ.spines.
 00002880: 0b73 6574 5f76 6973 6962 6c65 2901 da05  .set_visible)...
 00002890: 6672 616d 6572 3600 0000 7236 0000 0072  framer6...r6...r
-000028a0: 3700 0000 72f8 0000 00a8 0100 0073 0e00  7...r........s..
+000028a0: 3700 0000 72f7 0000 00a8 0100 0073 0e00  7...r........s..
 000028b0: 0000 0802 1001 1001 1001 1001 1001 1401  ................
 000028c0: 7a1d 4272 6169 6e47 7269 642e 6d61 6b65  z.BrainGrid.make
 000028d0: 5f63 656c 6c5f 696e 7669 7369 626c 654e  _cell_invisibleN
-000028e0: 290c 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
-000028f0: 0072 8b00 0000 7227 0000 0072 2c00 0000  .r....r'...r,...
-00002900: 72ad 0000 0072 c300 0000 72a8 0000 0072  r....r....r....r
-00002910: cf00 0000 728c 0000 0072 f800 0000 7236  ....r....r....r6
+000028e0: 290c 7287 0000 0072 8800 0000 7289 0000  ).r....r....r...
+000028f0: 0072 8a00 0000 7227 0000 0072 2c00 0000  .r....r'...r,...
+00002900: 72ac 0000 0072 c200 0000 72a7 0000 0072  r....r....r....r
+00002910: ce00 0000 728b 0000 0072 f700 0000 7236  ....r....r....r6
 00002920: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
 00002930: 0000 7226 0000 00aa 0000 0073 1e00 0000  ..r&.......s....
 00002940: 0800 0201 0a01 0222 0a01 023e 0a01 022a  ......."...>...*
 00002950: 0a01 0224 0a01 022d 0a01 021c 0e01 7226  ...$...-......r&
 00002960: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00002970: 0000 0000 0300 0000 4000 0000 7318 0000  ........@...s...
 00002980: 0065 005a 0164 005a 0265 0364 0164 0284  .e.Z.d.Z.e.d.d..
@@ -700,54 +700,54 @@
 00002bb0: 6405 6423 8d02 3700 7d06 6e06 7c06 7408  d.d#..7.}.n.|.t.
 00002bc0: a020 a100 3700 7d06 7c06 6a21 6424 7c00  . ..7.}.|.j!d$|.
 00002bd0: 6a02 6a22 7c00 6a02 6a22 6425 1400 6426  j.j"|.j.j"d%..d&
 00002be0: 6426 6427 8d05 0100 7c06 6a21 6428 7c00  d&d'....|.j!d(|.
 00002bf0: 6a02 6a22 7c00 6a02 6a22 6425 1400 6426  j.j"|.j.j"d%..d&
 00002c00: 6426 6427 8d05 0100 7c00 6a02 6a23 9001  d&d'....|.j.j#..
 00002c10: 7230 7424 6429 8301 0100 6400 5300 6400  r0t$d)....d.S.d.
-00002c20: 5300 292a 4e72 f100 0000 da07 4f76 6572  S.)*Nr......Over
+00002c20: 5300 292a 4e72 f000 0000 da07 4f76 6572  S.)*Nr......Over
 00002c30: 616c 6cfa 064e 6f20 524f 4972 5c00 0000  all..No ROIr\...
 00002c40: 7201 0000 0072 4500 0000 6301 0000 0000  r....rE...c.....
 00002c50: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
 00002c60: 0000 00f3 0c00 0000 7c00 a000 6401 6701  ........|...d.g.
 00002c70: a101 5300 a902 4e72 5c00 0000 a901 da0b  ..S...Nr\.......
 00002c80: 736f 7274 5f76 616c 7565 73a9 01da 0178  sort_values....x
 00002c90: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
 00002ca0: 083c 6c61 6d62 6461 3ebd 0100 00f3 0200  .<lambda>.......
 00002cb0: 0000 0c00 7a21 5669 6f6c 696e 506c 6f74  ....z!ViolinPlot
 00002cc0: 2e6d 616b 652e 3c6c 6f63 616c 733e 2e3c  .make.<locals>.<
 00002cd0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
 00002ce0: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-00002cf0: 7204 0100 0072 0501 0000 7206 0100 0072  r....r....r....r
-00002d00: 0801 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
-00002d10: 0000 0072 0a01 0000 c001 0000 720b 0100  ...r........r...
+00002cf0: 7203 0100 0072 0401 0000 7205 0100 0072  r....r....r....r
+00002d00: 0701 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00002d10: 0000 0072 0901 0000 c001 0000 720a 0100  ...r........r...
 00002d20: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002d30: 0000 0300 0000 5300 0000 7204 0100 0072  ......S...r....r
-00002d40: 0501 0000 7206 0100 0072 0801 0000 7236  ....r....r....r6
-00002d50: 0000 0072 3600 0000 7237 0000 0072 0a01  ...r6...r7...r..
-00002d60: 0000 c301 0000 720b 0100 0054 a901 da04  ......r....T....
-00002d70: 6472 6f70 7209 0000 00da 0863 6f6e 7374  dropr......const
-00002d80: 616e 7472 a100 0000 7a07 782b 7368 6966  antr....z.x+shif
+00002d30: 0000 0300 0000 5300 0000 7203 0100 0072  ......S...r....r
+00002d40: 0401 0000 7205 0100 0072 0701 0000 7236  ....r....r....r6
+00002d50: 0000 0072 3600 0000 7237 0000 0072 0901  ...r6...r7...r..
+00002d60: 0000 c301 0000 720a 0100 0054 a901 da04  ......r....T....
+00002d70: 6472 6f70 7208 0000 00da 0863 6f6e 7374  dropr......const
+00002d80: 616e 7472 a000 0000 7a07 782b 7368 6966  antr....z.x+shif
 00002d90: 7429 015a 0b61 6674 6572 5f73 6361 6c65  t).Z.after_scale
-00002da0: 7208 0100 007a 0778 2d73 6869 6674 a902  r....z.x-shift..
-00002db0: 7209 0100 00da 0179 72fa 0000 0067 3333  r......yr....g33
+00002da0: 7207 0100 007a 0778 2d73 6869 6674 a902  r....z.x-shift..
+00002db0: 7208 0100 00da 0179 72f9 0000 0067 3333  r......yr....g33
 00002dc0: 3333 3333 e33f 2904 da05 6e61 5f72 6dda  3333.?)...na_rm.
-00002dd0: 0573 7479 6c65 da04 6669 6c6c 72e7 0000  .style..fillr...
+00002dd0: 0573 7479 6c65 da04 6669 6c6c 72e6 0000  .style..fillr...
 00002de0: 0029 0472 4c00 0000 5a0d 6f75 746c 6965  .).rL...Z.outlie
-00002df0: 725f 616c 7068 6172 1301 0000 72e7 0000  r_alphar....r...
+00002df0: 725f 616c 7068 6172 1201 0000 72e6 0000  r_alphar....r...
 00002e00: 0067 9a99 9999 9999 d93f 6766 6666 6666  .g.......?gfffff
 00002e10: 66f6 3fda 017e da0a 6c61 6265 6c5f 626f  f.?..~..label_bo
-00002e20: 7468 a902 720d 0100 005a 086c 6162 656c  th..r....Z.label
+00002e20: 7468 a902 720c 0100 005a 086c 6162 656c  th..r....Z.label
 00002e30: 6c65 72a9 01da 0561 6c70 6861 da04 6772  ler....alpha..gr
-00002e40: 6179 a902 7213 0100 0072 1801 0000 2905  ay..r....r....).
+00002e40: 6179 a902 7212 0100 0072 1701 0000 2905  ay..r....r....).
 00002e50: da12 7061 6e65 6c5f 6772 6964 5f6d 616a  ..panel_grid_maj
 00002e60: 6f72 5f79 da12 7061 6e65 6c5f 6772 6964  or_y..panel_grid
 00002e70: 5f6d 616a 6f72 5f78 da10 7061 6e65 6c5f  _major_x..panel_
 00002e80: 6261 636b 6772 6f75 6e64 da0b 6178 6973  background..axis
-00002e90: 5f74 6578 745f 7872 c100 0000 677b 14ae  _text_xr....g{..
+00002e90: 5f74 6578 745f 7872 c000 0000 677b 14ae  _text_xr....g{..
 00002ea0: 47e1 7aa4 3f29 0272 4c00 0000 724b 0000  G.z.?).rL...rK..
 00002eb0: 007a 2346 6967 7572 6573 2f56 696f 6c69  .z#Figures/Violi
 00002ec0: 6e5f 706c 6f74 732f 7669 6f6c 696e 706c  n_plots/violinpl
 00002ed0: 6f74 2e70 6e67 7249 0000 0046 724a 0000  ot.pngrI...FrJ..
 00002ee0: 007a 2346 6967 7572 6573 2f56 696f 6c69  .z#Figures/Violi
 00002ef0: 6e5f 706c 6f74 732f 7669 6f6c 696e 706c  n_plots/violinpl
 00002f00: 6f74 2e73 7667 7a12 5361 7665 6420 7669  ot.svgz.Saved vi
@@ -765,35 +765,35 @@
 00002fc0: da04 796c 696d 5a04 796c 6162 da0d 7461  ..ylimZ.ylab..ta
 00002fd0: 626c 655f 785f 6c61 6265 6c5a 0478 6c61  ble_x_labelZ.xla
 00002fe0: 62da 0a66 6163 6574 5f67 7269 64da 0974  b..facet_grid..t
 00002ff0: 6865 6d65 5f35 3338 da05 7468 656d 65da  heme_538..theme.
 00003000: 0674 6865 6d65 73da 0c65 6c65 6d65 6e74  .themes..element
 00003010: 5f6c 696e 65da 0c65 6c65 6d65 6e74 5f72  _line..element_r
 00003020: 6563 745a 0d65 6c65 6d65 6e74 5f62 6c61  ectZ.element_bla
-00003030: 6e6b 72d3 0000 00da 1076 696f 6c69 6e5f  nkr......violin_
+00003030: 6e6b 72d2 0000 00da 1076 696f 6c69 6e5f  nkr......violin_
 00003040: 7368 6f77 5f64 6174 61da 0d76 696f 6c69  show_data..violi
 00003050: 6e5f 6a69 7474 6572 5a0b 6765 6f6d 5f6a  n_jitterZ.geom_j
 00003060: 6974 7465 72da 0a67 656f 6d5f 706f 696e  itter..geom_poin
 00003070: 7472 5100 0000 7252 0000 0072 1f00 0000  trQ...rR...r....
 00003080: 7220 0000 0029 0772 3000 0000 5a07 6f72  r ...).r0...Z.or
-00003090: 6967 5f64 6672 b000 0000 da05 7368 6966  ig_dfr......shif
+00003090: 6967 5f64 6672 af00 0000 da05 7368 6966  ig_dfr......shif
 000030a0: 74da 0b72 6967 6874 5f73 6869 6674 da0a  t..right_shift..
 000030b0: 6c65 6674 5f73 6869 6674 7240 0000 0072  left_shiftr@...r
 000030c0: 3600 0000 7236 0000 0072 3700 0000 7227  6...r6...r7...r'
 000030d0: 0000 00b4 0100 0073 7200 0000 0a02 1c02  .......sr.......
 000030e0: 1001 1802 2202 0c02 1a01 0c02 1801 0c02  ...."...........
 000030f0: 0802 0403 1602 1601 0802 0c01 02ff 1602  ................
 00003100: 02fe 1403 02fd 0a04 02fc 0a05 02fb 0c06  ................
 00003110: 02fa 0807 02f9 1a08 0201 04ff 02f8 060a  ................
 00003120: 02f6 100b 0c01 0c01 0601 0601 04fc 04f5  ................
 00003130: 0a11 0801 1401 0c02 0c02 0a01 0401 06fe  ................
 00003140: 0c04 0a01 0401 06fe 0a04 0c01 04ff 7a0f  ..............z.
 00003150: 5669 6f6c 696e 506c 6f74 2e6d 616b 654e  ViolinPlot.makeN
-00003160: 2905 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
-00003170: 0072 8b00 0000 7227 0000 0072 3600 0000  .r....r'...r6...
+00003160: 2905 7287 0000 0072 8800 0000 7289 0000  ).r....r....r...
+00003170: 0072 8a00 0000 7227 0000 0072 3600 0000  .r....r'...r6...
 00003180: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
 00003190: 2a00 0000 b301 0000 7306 0000 0008 0002  *.......s.......
 000031a0: 010e 0172 2a00 0000 6300 0000 0000 0000  ...r*...c.......
 000031b0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 000031c0: 0073 2400 0000 6500 5a01 6400 5a02 6503  .s$...e.Z.d.Z.e.
 000031d0: 6401 6402 8400 8301 5a04 6505 6403 6404  d.d.....Z.e.d.d.
 000031e0: 8400 8301 5a06 6405 5300 2906 722b 0000  ....Z.d.S.).r+..
@@ -822,52 +822,52 @@
 00003350: 0064 1019 007d 056e 0264 0053 0071 4629  .d...}.n.d.S.qF)
 00003360: 144e 7245 0000 007a 4550 6172 616d 6574  .NrE...zEParamet
 00003370: 6572 2074 6f20 706c 6f74 2061 6c6f 6e67  er to plot along
 00003380: 2074 6865 2078 2d61 7865 7320 6f66 2074   the x-axes of t
 00003390: 6865 2062 6172 6368 6172 7473 2068 6173  he barcharts has
 000033a0: 206e 6f74 2062 6565 6e20 7365 742e 7a11   not been set.z.
 000033b0: 4669 6775 7265 732f 4261 7263 6861 7274  Figures/Barchart
-000033c0: 7372 f100 0000 7a14 4f6e 6520 7265 6769  sr....z.One regi
+000033c0: 7372 f000 0000 7a14 4f6e 6520 7265 6769  sr....z.One regi
 000033d0: 6f6e 2062 6172 2063 6861 7274 a902 da09  on bar chart....
 000033e0: 6675 6e63 5f6e 616d 65da 1163 6f6e 6669  func_name..confi
 000033f0: 675f 7265 6769 6f6e 5f76 6172 7a1b 536b  g_region_varz.Sk
 00003400: 6970 7069 6e67 2062 6172 6368 6172 7420  ipping barchart 
 00003410: 6372 6561 7469 6f6e 2e7a 1a0a 2d2d 2d20  creation.z..--- 
 00003420: 4261 7263 6861 7274 2063 7265 6174 696f  Barchart creatio
 00003430: 6e20 2d2d 2d72 0100 0000 5463 0100 0000  n ---r....Tc....
 00003440: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00003450: 5300 0000 f308 0000 007c 0064 0119 0053  S........|.d...S
-00003460: 00a9 024e 7209 0000 0072 3600 0000 7208  ...Nr....r6...r.
+00003460: 00a9 024e 7208 0000 0072 3600 0000 7207  ...Nr....r6...r.
 00003470: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003480: 0000 720a 0100 0013 0200 00f3 0200 0000  ..r.............
+00003480: 0000 7209 0100 0013 0200 00f3 0200 0000  ..r.............
 00003490: 0800 7a20 4261 7263 6861 7274 2e73 6574  ..z Barchart.set
 000034a0: 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  up.<locals>.<lam
-000034b0: 6264 613e a901 72f3 0000 007a 144d 6178  bda>..r....z.Max
+000034b0: 6264 613e a901 72f2 0000 007a 144d 6178  bda>..r....z.Max
 000034c0: 696d 756d 2079 206c 696d 6974 206f 663a  imum y limit of:
-000034d0: 2072 a500 0000 7209 0000 00fa 1020 7365   r....r...... se
+000034d0: 2072 a400 0000 7208 0000 00fa 1020 7365   r....r...... se
 000034e0: 656e 2077 6974 6820 524f 493a 2072 6000  en with ROI: r`.
 000034f0: 0000 7a26 2e20 4372 6561 7469 6e67 2066  ..z&. Creating f
 00003500: 6967 7572 6573 2077 6974 6820 7468 6973  igures with this
 00003510: 2079 206c 696d 6974 2e0a 2917 7214 0000   y limit..).r...
 00003520: 00da 1573 696e 676c 655f 726f 695f 6669  ...single_roi_fi
 00003530: 675f 785f 6178 6973 da09 4578 6365 7074  g_x_axis..Except
-00003540: 696f 6e72 0a00 0000 7229 0000 0072 6900  ionr....r)...ri.
-00003550: 0000 72a7 0000 00da 1066 696e 645f 6368  ..r......find_ch
+00003540: 696f 6e72 0900 0000 7229 0000 0072 6900  ionr....r)...ri.
+00003550: 0000 72a6 0000 00da 1066 696e 645f 6368  ..r......find_ch
 00003560: 6f73 656e 5f72 6f69 73da 1172 6567 696f  osen_rois..regio
 00003570: 6e61 6c5f 6669 675f 726f 6973 da09 4e61  nal_fig_rois..Na
 00003580: 6d65 4572 726f 7272 1f00 0000 7220 0000  meErrorr....r ..
 00003590: 00da 037a 6970 da09 6974 6572 746f 6f6c  ...zip..itertool
 000035a0: 73da 0672 6570 6561 7472 2700 0000 7257  s..repeatr'...rW
 000035b0: 0000 0072 4400 0000 da07 7374 6172 6d61  ...rD.....starma
 000035c0: 70da 1463 6c61 7373 5f6d 6574 686f 645f  p..class_method_
 000035d0: 6861 6e64 6c65 72da 0361 6e79 da04 736f  handler..any..so
-000035e0: 7274 72af 0000 0029 0772 3000 0000 72b0  rtr....).r0...r.
+000035e0: 7274 72ae 0000 0029 0772 3000 0000 72af  rtr....).r0...r.
 000035f0: 0000 0072 3500 0000 da09 6c69 7374 5f72  ...r5.....list_r
 00003600: 6f69 73da 0b63 686f 7365 6e5f 726f 6973  ois..chosen_rois
-00003610: 722d 0100 00da 0869 7465 7261 626c 6572  r-.....iterabler
+00003610: 722c 0100 00da 0869 7465 7261 626c 6572  r,.....iterabler
 00003620: 3600 0000 7236 0000 0072 3700 0000 722c  6...r6...r7...r,
 00003630: 0000 00f3 0100 0073 4000 0000 0c02 0801  .......s@.......
 00003640: 0a02 1002 0801 0601 06ff 0202 0801 0c01  ................
 00003650: 0801 0e01 06ff 02ff 0804 0801 0402 0201  ................
 00003660: 1601 1201 1401 04fe 0404 1001 1203 0802  ................
 00003670: 1001 0802 2a01 0e03 0402 02ec 7a0e 4261  ....*.......z.Ba
 00003680: 7263 6861 7274 2e73 6574 7570 6306 0000  rchart.setupc...
@@ -907,95 +907,95 @@
 000038a0: 6a1b 7c05 6a1c 7c05 6a1d 7c05 6a1e 6433  j.|.j.|.j.|.j.d3
 000038b0: 8d03 3700 7d07 7c02 9001 7215 7c07 740a  ..7.}.|...r.|.t.
 000038c0: a01f 6400 7c02 a102 3700 7d07 7c00 6434  ..d.|...7.}.|.d4
 000038d0: 3700 7d00 6410 7d09 7c02 6410 6b02 9001  7.}.d.}.|.d.k...
 000038e0: 7225 7c04 7c00 7c07 6435 8303 7d09 6436  r%|.|.|.d5..}.d6
 000038f0: 7d0a 6e07 7c02 6410 6b03 9001 722c 6437  }.n.|.d.k...r,d7
 00003900: 7d0a 7c03 7c07 7c00 7c0a 6438 7c05 8305  }.|.|.|.|.d8|...
-00003910: 0100 7c09 5300 2939 4e72 f100 0000 5472  ..|.S.)9Nr....Tr
-00003920: 0c01 0000 2901 da0a 6361 7465 676f 7269  ....)...categori
+00003910: 0100 7c09 5300 2939 4e72 f000 0000 5472  ..|.S.)9Nr....Tr
+00003920: 0b01 0000 2901 da0a 6361 7465 676f 7269  ....)...categori
 00003930: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
 00003940: 0000 0006 0000 0053 0000 0073 1800 0000  .......S...s....
 00003950: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
 00003960: a102 9102 7102 5300 2902 720e 0000 0072  ....q.S.).r....r
-00003970: 0f00 0000 2901 721d 0000 0029 0272 9a00  ....).r....).r..
+00003970: 0f00 0000 2901 721d 0000 0029 0272 9900  ....).r....).r..
 00003980: 0000 da01 6372 3600 0000 7236 0000 0072  ....cr6...r6...r
-00003990: 3700 0000 729d 0000 0027 0200 00f3 0200  7...r....'......
+00003990: 3700 0000 729c 0000 0027 0200 00f3 0200  7...r....'......
 000039a0: 0000 1800 7a21 4261 7263 6861 7274 2e6d  ....z!Barchart.m
 000039b0: 616b 652e 3c6c 6f63 616c 733e 2e3c 6c69  ake.<locals>.<li
 000039c0: 7374 636f 6d70 3e72 0e00 0000 720f 0000  stcomp>r....r...
 000039d0: 00da 0673 696e 676c 65e7 9a99 9999 9999  ...single.......
 000039e0: e93f 2902 da08 7072 6573 6572 7665 724c  .?)...preserverL
 000039f0: 0000 0029 03da 0870 6f73 6974 696f 6e72  ...)...positionr
-00003a00: 4c00 0000 7211 0100 0072 0900 0000 2902  L...r....r....).
-00003a10: 72e7 0000 0072 5801 0000 2901 da06 6c61  r....rX...)...la
-00003a20: 6265 6c73 7201 0000 0072 1701 0000 da05  belsr....r......
-00003a30: 7768 6974 6567 9a99 9999 9999 c93f 721a  whiteg.......?r.
+00003a00: 4c00 0000 7210 0100 0072 0800 0000 2902  L...r....r....).
+00003a10: 72e6 0000 0072 5701 0000 2901 da06 6c61  r....rW...)...la
+00003a20: 6265 6c73 7201 0000 0072 1601 0000 da05  belsr....r......
+00003a30: 7768 6974 6567 9a99 9999 9999 c93f 7219  whiteg.......?r.
 00003a40: 0100 00da 0462 6f6c 64da 0562 6c61 636b  .....bold..black
 00003a50: e914 0000 00a9 03da 0677 6569 6768 74da  .........weight.
-00003a60: 0563 6f6c 6f72 72e7 0000 00a9 0272 e700  .colorr......r..
-00003a70: 0000 7260 0100 00da 0162 2904 72e7 0000  ..r`.....b).r...
-00003a80: 0072 5f01 0000 7260 0100 00da 066d 6172  .r_...r`.....mar
-00003a90: 6769 6eda 016c e905 0000 0029 0372 e700  gin..l.....).r..
-00003aa0: 0000 7260 0100 0072 6301 0000 e90a 0000  ..r`...rc.......
-00003ab0: 00e9 1e00 0000 72fb 0000 0067 3333 3333  ......r....g3333
+00003a60: 0563 6f6c 6f72 72e6 0000 00a9 0272 e600  .colorr......r..
+00003a70: 0000 725f 0100 00da 0162 2904 72e6 0000  ..r_.....b).r...
+00003a80: 0072 5e01 0000 725f 0100 00da 066d 6172  .r^...r_.....mar
+00003a90: 6769 6eda 016c e905 0000 0029 0372 e600  gin..l.....).r..
+00003aa0: 0000 725f 0100 0072 6201 0000 e90a 0000  ..r_...rb.......
+00003ab0: 00e9 1e00 0000 72fa 0000 0067 3333 3333  ......r....g3333
 00003ac0: 3333 eb3f 2902 67cd cccc cccc ccec 3f72  33.?).g.......?r
-00003ad0: 5601 0000 290c 721c 0100 0072 1d01 0000  V...).r....r....
+00003ad0: 5501 0000 290c 721b 0100 0072 1c01 0000  U...).r....r....
 00003ae0: da0c 6178 6973 5f74 6974 6c65 5f78 da0c  ..axis_title_x..
 00003af0: 6178 6973 5f74 6974 6c65 5f79 da0b 6178  axis_title_y..ax
 00003b00: 6973 5f74 6578 745f 795a 0c6c 6567 656e  is_text_yZ.legen
 00003b10: 645f 7469 746c 655a 0b6c 6567 656e 645f  d_titleZ.legend_
 00003b20: 7465 7874 5a14 6c65 6765 6e64 5f65 6e74  textZ.legend_ent
 00003b30: 7279 5f73 7061 6369 6e67 5a0f 6c65 6765  ry_spacingZ.lege
 00003b40: 6e64 5f6b 6579 5f73 697a 65da 0f73 7562  nd_key_size..sub
 00003b50: 706c 6f74 735f 6164 6a75 7374 da0f 6c65  plots_adjust..le
-00003b60: 6765 6e64 5f70 6f73 6974 696f 6e72 c100  gend_positionr..
-00003b70: 0000 6766 6666 6666 66e6 bf29 0272 1001  ..gffffff..).r..
-00003b80: 0000 da05 6c61 6265 6c72 fd00 0000 2903  ....labelr....).
-00003b90: 7260 0100 0072 e700 0000 da02 7661 a901  r`...r......va..
-00003ba0: 72bd 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00003b60: 6765 6e64 5f70 6f73 6974 696f 6e72 c000  gend_positionr..
+00003b70: 0000 6766 6666 6666 66e6 bf29 0272 0f01  ..gffffff..).r..
+00003b80: 0000 da05 6c61 6265 6c72 fc00 0000 2903  ....labelr....).
+00003b90: 725f 0100 0072 e600 0000 da02 7661 a901  r_...r......va..
+00003ba0: 72bc 0000 0063 0100 0000 0000 0000 0000  r....c..........
 00003bb0: 0000 0200 0000 0400 0000 5300 0000 7318  ..........S...s.
 00003bc0: 0000 0067 007c 005d 087d 0164 007c 0176  ...g.|.].}.d.|.v
 00003bd0: 0072 027c 0191 0271 0253 0029 015a 0843  .r.|...q.S.).Z.C
-00003be0: 6f6e 665f 496e 7472 3600 0000 2902 729a  onf_Intr6...).r.
-00003bf0: 0000 0072 0901 0000 7236 0000 0072 3600  ...r....r6...r6.
-00003c00: 0000 7237 0000 0072 9d00 0000 4302 0000  ..r7...r....C...
-00003c10: 7254 0100 0072 4500 0000 725c 0000 007a  rT...rE...r\...z
+00003be0: 6f6e 665f 496e 7472 3600 0000 2902 7299  onf_Intr6...).r.
+00003bf0: 0000 0072 0801 0000 7236 0000 0072 3600  ...r....r6...r6.
+00003c00: 0000 7237 0000 0072 9c00 0000 4302 0000  ..r7...r....C...
+00003c10: 7253 0100 0072 4500 0000 725c 0000 007a  rS...rE...r\...z
 00003c20: 054d 6561 6e2d 7a05 4d65 616e 2b7a 0766  .Mean-z.Mean+z.f
-00003c30: 6163 746f 7228 fa01 2929 0572 0901 0000  actor(..)).r....
-00003c40: 7210 0100 00da 0479 6d69 6eda 0479 6d61  r......ymin..yma
-00003c50: 7872 1301 0000 2904 7209 0100 0072 1001  xr....).r....r..
-00003c60: 0000 7271 0100 0072 7201 0000 2903 7209  ..rq...rr...).r.
-00003c70: 0100 0072 1001 0000 7213 0100 005a 0a5f  ...r....r....Z._
+00003c30: 6163 746f 7228 fa01 2929 0572 0801 0000  actor(..)).r....
+00003c40: 720f 0100 00da 0479 6d69 6eda 0479 6d61  r......ymin..yma
+00003c50: 7872 1201 0000 2904 7208 0100 0072 0f01  xr....).r....r..
+00003c60: 0000 7270 0100 0072 7101 0000 2903 7208  ..rp...rq...).r.
+00003c70: 0100 0072 0f01 0000 7212 0100 005a 0a5f  ...r....r....Z._
 00003c80: 7361 6d65 5f79 6c69 6d72 3a00 0000 5a0f  same_ylimr:...Z.
 00003c90: 4469 6666 6572 656e 745f 7961 7869 735a  Different_yaxisZ
 00003ca0: 0a53 616d 655f 7961 7869 735a 0862 6172  .Same_yaxisZ.bar
-00003cb0: 6368 6172 7429 2072 7200 0000 7207 0100  chart) rr...r...
-00003cc0: 0072 4301 0000 7225 0100 0072 6700 0000  .rC...r%...rg...
-00003cd0: da0b 4361 7465 676f 7269 6361 6c72 a700  ..Categoricalr..
+00003cb0: 6368 6172 7429 2072 7200 0000 7206 0100  chart) rr...r...
+00003cc0: 0072 4201 0000 7224 0100 0072 6700 0000  .rB...r$...rg...
+00003cd0: da0b 4361 7465 676f 7269 6361 6c72 a600  ..Categoricalr..
 00003ce0: 0000 7277 0000 0072 1d00 0000 da15 7369  ..rw...r......si
 00003cf0: 6e67 6c65 5f72 6f69 5f66 6967 5f63 6f6c  ngle_roi_fig_col
-00003d00: 6f75 7272 2601 0000 7229 0100 0072 3001  ourr&...r)...r0.
+00003d00: 6f75 7272 2501 0000 7228 0100 0072 2f01  ourr%...r(...r/.
 00003d10: 0000 5a08 6765 6f6d 5f63 6f6c 5a0e 706f  ..Z.geom_colZ.po
 00003d20: 7369 7469 6f6e 5f64 6f64 6765 5a0d 6765  sition_dodgeZ.ge
 00003d30: 6f6d 5f65 7272 6f72 6261 725a 1073 6361  om_errorbarZ.sca
-00003d40: 6c65 5f78 5f64 6973 6372 6574 6572 3101  le_x_discreter1.
-00003d50: 0000 7233 0100 0072 3401 0000 da0c 656c  ..r3...r4.....el
-00003d60: 656d 656e 745f 7465 7874 72d3 0000 005a  ement_textr....Z
-00003d70: 0967 656f 6d5f 7465 7874 7227 0100 005a  .geom_textr'...Z
+00003d40: 6c65 5f78 5f64 6973 6372 6574 6572 3001  le_x_discreter0.
+00003d50: 0000 7232 0100 0072 3301 0000 da0c 656c  ..r2...r3.....el
+00003d60: 656d 656e 745f 7465 7874 72d2 0000 005a  ement_textr....Z
+00003d70: 0967 656f 6d5f 7465 7874 7226 0100 005a  .geom_textr&...Z
 00003d80: 1173 6361 6c65 5f66 696c 6c5f 6d61 6e75  .scale_fill_manu
 00003d90: 616c da20 636f 6c6f 7262 6c69 6e64 5f66  al. colorblind_f
 00003da0: 7269 656e 646c 795f 706c 6f74 5f63 6f6c  riendly_plot_col
-00003db0: 6f75 7273 72ee 0000 00da 046c 6162 73da  oursr......labs.
+00003db0: 6f75 7273 72ed 0000 00da 046c 6162 73da  oursr......labs.
 00003dc0: 1673 696e 676c 655f 726f 695f 6669 675f  .single_roi_fig_
 00003dd0: 6c61 6265 6c5f 78da 1673 696e 676c 655f  label_x..single_
 00003de0: 726f 695f 6669 675f 6c61 6265 6c5f 79da  roi_fig_label_y.
 00003df0: 1973 696e 676c 655f 726f 695f 6669 675f  .single_roi_fig_
-00003e00: 6c61 6265 6c5f 6669 6c6c 722d 0100 0029  label_fillr-...)
-00003e10: 0b72 3f00 0000 72b0 0000 005a 0679 6c69  .r?...r....Z.yli
+00003e00: 6c61 6265 6c5f 6669 6c6c 722c 0100 0029  label_fillr,...)
+00003e10: 0b72 3f00 0000 72af 0000 005a 0679 6c69  .r?...r....Z.yli
 00003e20: 6d69 74da 0d73 6176 655f 6675 6e63 7469  mit..save_functi
 00003e30: 6f6e 5a12 6669 6e64 5f79 6c69 6d5f 6675  onZ.find_ylim_fu
 00003e40: 6e63 7469 6f6e 7214 0000 00da 0a63 7572  nctionr......cur
 00003e50: 7265 6e74 5f64 6672 4000 0000 5a0f 636f  rent_dfr@...Z.co
 00003e60: 6e66 5f69 6e74 5f73 7472 696e 675a 0d72  nf_int_stringZ.r
 00003e70: 6574 7572 6e65 645f 796c 696d 7253 0000  eturned_ylimrS..
 00003e80: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
@@ -1005,16 +1005,16 @@
 00003ec0: 1603 02fd 0a04 02fc 0e05 0c01 0e01 0e01  ................
 00003ed0: 0c01 1401 1201 0201 0201 0601 0201 0401  ................
 00003ee0: 04f5 02fb 1212 0601 04ff 02ee 0c14 02ec  ................
 00003ef0: 02ff 1618 0a02 0c01 1001 0c01 0afe 0c04  ................
 00003f00: 1001 08ff 0e03 0401 08ff 0603 1002 0801  ................
 00003f10: 0402 0a01 0c01 0601 0a01 0401 1002 0402  ................
 00003f20: 7a0d 4261 7263 6861 7274 2e6d 616b 654e  z.Barchart.makeN
-00003f30: 2907 7288 0000 0072 8900 0000 728a 0000  ).r....r....r...
-00003f40: 0072 8b00 0000 722c 0000 0072 8c00 0000  .r....r,...r....
+00003f30: 2907 7287 0000 0072 8800 0000 7289 0000  ).r....r....r...
+00003f40: 0072 8a00 0000 722c 0000 0072 8b00 0000  .r....r,...r....
 00003f50: 7227 0000 0072 3600 0000 7236 0000 0072  r'...r6...r6...r
 00003f60: 3600 0000 7237 0000 0072 2b00 0000 f201  6...r7...r+.....
 00003f70: 0000 730a 0000 0008 0002 010a 0102 290e  ..s...........).
 00003f80: 0172 2b00 0000 6300 0000 0000 0000 0000  .r+...c.........
 00003f90: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 00003fa0: 3000 0000 6500 5a01 6400 5a02 6503 6401  0...e.Z.d.Z.e.d.
 00003fb0: 6402 8400 8301 5a04 6503 6403 6404 8400  d.....Z.e.d.d...
@@ -1045,61 +1045,61 @@
 00004140: 0059 006e 0177 007c 096a 1964 0f64 1084  .Y.n.w.|.j.d.d..
 00004150: 0064 118d 0101 007c 006a 056a 0872 c874  .d.....|.j.j.r.t
 00004160: 0964 1274 1a7c 0964 1319 0064 1419 0083  .d.t.|.d...d....
 00004170: 019b 0064 157c 0964 1319 0064 1619 009b  ...d.|.d...d....
 00004180: 0064 179d 0583 0101 007c 0964 1319 0064  .d.......|.d...d
 00004190: 1419 007d 096e 0264 0053 0071 6229 184e  ...}.n.d.S.qb).N
 000041a0: 7a12 4669 6775 7265 732f 4869 7374 6f67  z.Figures/Histog
-000041b0: 7261 6d73 72f1 0000 0072 2d00 0000 723b  ramsr....r-...r;
+000041b0: 7261 6d73 72f0 0000 0072 2d00 0000 723a  ramsr....r-...r:
 000041c0: 0100 007a 1c53 6b69 7070 696e 6720 6869  ...z.Skipping hi
 000041d0: 7374 6f67 7261 6d20 6372 6561 7469 6f6e  stogram creation
 000041e0: 2e7a 1b0a 2d2d 2d20 4869 7374 6f67 7261  .z..--- Histogra
 000041f0: 6d20 6372 6561 7469 6f6e 202d 2d2d 6301  m creation ---c.
 00004200: 0000 0000 0000 0000 0000 0002 0000 0005  ................
 00004210: 0000 0053 0000 0073 1e00 0000 6700 7c00  ...S...s....g.|.
 00004220: 5d0b 7d01 7400 a001 a100 9b00 6400 7c01  ].}.t.......d.|.
 00004230: 9b00 9d03 9102 7102 5300 2901 7a15 2f4f  ......q.S.).z./O
 00004240: 7665 7261 6c6c 2f52 6177 5f72 6573 756c  verall/Raw_resul
 00004250: 7473 2f29 0272 1600 0000 7217 0000 0072  ts/).r....r....r
-00004260: 9900 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
-00004270: 0000 0072 9d00 0000 7402 0000 7302 0000  ...r....t...s...
+00004260: 9800 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
+00004270: 0000 0072 9c00 0000 7402 0000 7302 0000  ...r....t...s...
 00004280: 001e 007a 2348 6973 746f 6772 616d 2e73  ...z#Histogram.s
 00004290: 6574 7570 2e3c 6c6f 6361 6c73 3e2e 3c6c  etup.<locals>.<l
 000042a0: 6973 7463 6f6d 703e 7a13 4f76 6572 616c  istcomp>z.Overal
 000042b0: 6c2f 5261 775f 7265 7375 6c74 7372 7000  l/Raw_resultsrp.
 000042c0: 0000 7205 0000 0029 0172 8000 0000 7201  ..r....).r....r.
 000042d0: 0000 0054 6301 0000 0000 0000 0000 0000  ...Tc...........
-000042e0: 0001 0000 0002 0000 0053 0000 0072 3e01  .........S...r>.
-000042f0: 0000 723f 0100 0072 3600 0000 7208 0100  ..r?...r6...r...
+000042e0: 0001 0000 0002 0000 0053 0000 0072 3d01  .........S...r=.
+000042f0: 0000 723e 0100 0072 3600 0000 7207 0100  ..r>...r6...r...
 00004300: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-00004310: 720a 0100 008e 0200 0072 4001 0000 7a21  r........r@...z!
+00004310: 7209 0100 008e 0200 0072 3f01 0000 7a21  r........r?...z!
 00004320: 4869 7374 6f67 7261 6d2e 7365 7475 702e  Histogram.setup.
 00004330: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00004340: 3e72 4101 0000 7a14 4d61 7869 6d75 6d20  >rA...z.Maximum 
-00004350: 7820 6c69 6d69 7420 6f66 3a20 72a5 0000  x limit of: r...
-00004360: 0072 0900 0000 7242 0100 0072 6000 0000  .r....rB...r`...
+00004340: 3e72 4001 0000 7a14 4d61 7869 6d75 6d20  >r@...z.Maximum 
+00004350: 7820 6c69 6d69 7420 6f66 3a20 72a4 0000  x limit of: r...
+00004360: 0072 0800 0000 7241 0100 0072 6000 0000  .r....rA...r`...
 00004370: 7a26 2e20 4372 6561 7469 6e67 2066 6967  z&. Creating fig
 00004380: 7572 6573 2077 6974 6820 7468 6973 2078  ures with this x
-00004390: 206c 696d 6974 2e0a 291b 720a 0000 0072   limit..).r....r
-000043a0: 2900 0000 7269 0000 0072 a700 0000 7245  )...ri...r....rE
-000043b0: 0100 0072 1400 0000 7246 0100 0072 4701  ...r....rF...rG.
+00004390: 206c 696d 6974 2e0a 291b 7209 0000 0072   limit..).r....r
+000043a0: 2900 0000 7269 0000 0072 a600 0000 7244  )...ri...r....rD
+000043b0: 0100 0072 1400 0000 7245 0100 0072 4601  ...r....rE...rF.
 000043c0: 0000 721f 0000 0072 2000 0000 da0a 6669  ..r....r .....fi
-000043d0: 6e64 5f66 696c 6573 7287 0000 0072 db00  nd_filesr....r..
+000043d0: 6e64 5f66 696c 6573 7286 0000 0072 da00  nd_filesr....r..
 000043e0: 0000 da27 6765 745f 6d65 616e 5f61 6e64  ...'get_mean_and
 000043f0: 5f6d 6564 6961 6e5f 666f 725f 6561 6368  _median_for_each
-00004400: 5f63 686f 7365 6e5f 726f 6972 4801 0000  _chosen_roirH...
-00004410: 7249 0100 0072 4a01 0000 7227 0000 0072  rI...rJ...r'...r
-00004420: 5700 0000 7244 0000 0072 4b01 0000 724c  W...rD...rK...rL
-00004430: 0100 0072 4d01 0000 da06 7265 6d6f 7665  ...rM.....remove
-00004440: da0a 5661 6c75 6545 7272 6f72 724e 0100  ..ValueErrorrN..
-00004450: 0072 af00 0000 290b 7230 0000 0072 7f00  .r....).r0...r..
-00004460: 0000 7235 0000 0072 4f01 0000 7250 0100  ..r5...rO...rP..
+00004400: 5f63 686f 7365 6e5f 726f 6972 4701 0000  _chosen_roirG...
+00004410: 7248 0100 0072 4901 0000 7227 0000 0072  rH...rI...r'...r
+00004420: 5700 0000 7244 0000 0072 4a01 0000 724b  W...rD...rJ...rK
+00004430: 0100 0072 4c01 0000 da06 7265 6d6f 7665  ...rL.....remove
+00004440: da0a 5661 6c75 6545 7272 6f72 724d 0100  ..ValueErrorrM..
+00004450: 0072 ae00 0000 290b 7230 0000 0072 7f00  .r....).r0...r..
+00004460: 0000 7235 0000 0072 4e01 0000 724f 0100  ..r5...rN...rO..
 00004470: 0072 7e00 0000 7281 0000 005a 1063 6f6d  .r~...r....Z.com
 00004480: 6269 6e65 645f 7261 775f 6466 73da 0372  bined_raw_dfs..r
-00004490: 6f69 722c 0100 0072 5101 0000 7236 0000  oir,...rQ...r6..
+00004490: 6f69 722b 0100 0072 5001 0000 7236 0000  oir+...rP...r6..
 000044a0: 0072 3600 0000 7237 0000 0072 2c00 0000  .r6...r7...r,...
 000044b0: 6202 0000 7358 0000 000a 0210 0208 0106  b...sX..........
 000044c0: 0106 ff02 0308 010c 0108 010e 0106 ff02  ................
 000044d0: ff08 0408 0106 030a 0106 ff14 0204 0208  ................
 000044e0: 0104 010c 0106 ff04 0302 0110 0112 0114  ................
 000044f0: 0104 fe04 0410 0112 0208 0202 010e 010c  ................
 00004500: 0104 0102 ff10 0308 022a 010e 0304 0202  .........*......
@@ -1120,34 +1120,34 @@
 000045f0: 7c04 6a0c 7c07 6405 8d01 7d04 7152 7400  |.j.|.d...}.qRt.
 00004600: 6a0d 7c04 7c06 6400 640b 8502 1900 640c  j.|.|.d.d.....d.
 00004610: 6409 640a 6702 640d 640e 8d05 7d04 7c00  d.d.g.d.d...}.|.
 00004620: 6a07 6a0e 7282 7c00 6a07 6a0f 7382 7c04  j.j.r.|.j.j.s.|.
 00004630: 6a10 7c04 640c 1900 6409 6b02 1900 7d04  j.|.d...d.k...}.
 00004640: 7c04 5300 7c00 6a07 6a0f 7293 7c00 6a07  |.S.|.j.j.r.|.j.
 00004650: 6a0e 7393 7c04 6a10 7c04 640c 1900 640a  j.s.|.j.|.d...d.
-00004660: 6b02 1900 7d04 7c04 5300 290f 4e72 0301  k...}.|.S.).Nr..
-00004670: 0000 7202 0100 0072 6100 0000 72f1 0000  ..r....ra...r...
-00004680: 0029 0172 7700 0000 72fa 0000 0029 02da  .).rw...r....)..
+00004660: 6b02 1900 7d04 7c04 5300 290f 4e72 0201  k...}.|.S.).Nr..
+00004670: 0000 7201 0100 0072 6100 0000 72f0 0000  ..r....ra...r...
+00004680: 0029 0172 7700 0000 72f9 0000 0029 02da  .).rw...r....)..
 00004690: 026f 6eda 0368 6f77 7262 0000 0072 5c00  .on..howrb...r\.
-000046a0: 0000 72a2 0000 00e9 feff ffff da09 5374  ..r...........St
+000046a0: 0000 72a1 0000 00e9 feff ffff da09 5374  ..r...........St
 000046b0: 6174 6973 7469 63da 0a73 7461 745f 7661  atistic..stat_va
 000046c0: 6c75 6529 0472 6300 0000 7264 0000 00da  lue).rc...rd....
 000046d0: 0a76 616c 7565 5f76 6172 7372 6500 0000  .value_varsre...
-000046e0: 2911 7267 0000 0072 6800 0000 721f 0100  ).rg...rh...r...
+000046e0: 2911 7267 0000 0072 6800 0000 721e 0100  ).rg...rh...r...
 000046f0: 0072 7d00 0000 da06 7265 6e61 6d65 7269  .r}.....renameri
 00004700: 0000 0072 6a00 0000 7214 0000 0072 6c00  ...rj...r....rl.
 00004710: 0000 726d 0000 00da 056d 6572 6765 7277  ..rm.....mergerw
-00004720: 0000 0072 0d01 0000 727c 0000 00da 1368  ...r....r|.....h
+00004720: 0000 0072 0c01 0000 727c 0000 00da 1368  ...r....r|.....h
 00004730: 6973 746f 6772 616d 5f73 686f 775f 6d65  istogram_show_me
 00004740: 616e da15 6869 7374 6f67 7261 6d5f 7368  an..histogram_sh
 00004750: 6f77 5f6d 6564 6961 6e72 7200 0000 2908  ow_medianrr...).
 00004760: 7230 0000 0072 3f00 0000 7281 0000 0072  r0...r?...r....r
-00004770: 7f00 0000 727c 0100 0072 8200 0000 72ee  ....r|...r....r.
-00004780: 0000 0072 8600 0000 7236 0000 0072 3600  ...r....r6...r6.
-00004790: 0000 7237 0000 0072 7e01 0000 9802 0000  ..r7...r~.......
+00004770: 7f00 0000 727b 0100 0072 8200 0000 72ed  ....r{...r....r.
+00004780: 0000 0072 8500 0000 7236 0000 0072 3600  ...r....r6...r6.
+00004790: 0000 7237 0000 0072 7d01 0000 9802 0000  ..r7...r}.......
 000047a0: 733a 0000 0008 0408 0108 0108 010a 0114  s:..............
 000047b0: 0208 0204 0306 0106 ff1a 0406 0108 0102  ................
 000047c0: 0106 fe18 050a 0208 010c 0102 8012 0208  ................
 000047d0: 0106 ff10 0312 0104 0410 fd12 0104 027a  ...............z
 000047e0: 3148 6973 746f 6772 616d 2e67 6574 5f6d  1Histogram.get_m
 000047f0: 6561 6e5f 616e 645f 6d65 6469 616e 5f66  ean_and_median_f
 00004800: 6f72 5f65 6163 685f 6368 6f73 656e 5f72  or_each_chosen_r
@@ -1184,78 +1184,78 @@
 000049f0: 6b03 72e4 6426 7d08 741e 6a1f 6427 7420  k.r.d&}.t.j.d't 
 00004a00: 6428 8d02 0100 7c03 7c06 7c00 7c08 6429  d(....|.|.|.|.d)
 00004a10: 7c05 8305 0100 741e 6a1f 642a 7420 6428  |.....t.j.d*t d(
 00004a20: 8d02 0100 7c07 5300 292b 4e7a 3849 4e46  ....|.S.)+Nz8INF
 00004a30: 4f3a 2048 6973 746f 6772 616d 7320 6361  O: Histograms ca
 00004a40: 6e6e 6f74 2062 6520 6d61 6465 2066 6f72  nnot be made for
 00004a50: 2074 6865 204e 6f20 524f 4920 6361 7465   the No ROI cate
-00004a60: 676f 7279 2e72 6200 0000 7208 0100 0072  gory.rb...r....r
+00004a60: 676f 7279 2e72 6200 0000 7207 0100 0072  gory.rb...r....r
 00004a70: 0100 0000 5429 04da 0862 696e 7769 6474  ....T)...binwidt
-00004a80: 6872 1301 0000 da08 626f 756e 6461 7279  hr......boundary
-00004a90: 7211 0100 0072 1401 0000 7215 0100 0072  r....r....r....r
-00004aa0: 1601 0000 720f 0100 0072 1701 0000 7209  ....r....r....r.
-00004ab0: 0000 0072 5a01 0000 a901 7213 0100 0072  ...rZ.....r....r
-00004ac0: 1901 0000 72a1 0000 0072 1a01 0000 725b  ....r....r....r[
-00004ad0: 0100 0072 5c01 0000 725d 0100 0072 5e01  ...r\...r]...r^.
-00004ae0: 0000 7266 0100 00a9 0372 5f01 0000 72e7  ..rf.....r_...r.
-00004af0: 0000 0072 6001 0000 7261 0100 00a9 0c5a  ...r`...ra.....Z
+00004a80: 6872 1201 0000 da08 626f 756e 6461 7279  hr......boundary
+00004a90: 7210 0100 0072 1301 0000 7214 0100 0072  r....r....r....r
+00004aa0: 1501 0000 720e 0100 0072 1601 0000 7208  ....r....r....r.
+00004ab0: 0000 0072 5901 0000 a901 7212 0100 0072  ...rY.....r....r
+00004ac0: 1801 0000 72a0 0000 0072 1901 0000 725a  ....r....r....rZ
+00004ad0: 0100 0072 5b01 0000 725c 0100 0072 5d01  ...r[...r\...r].
+00004ae0: 0000 7265 0100 00a9 0372 5e01 0000 72e6  ..re.....r^...r.
+00004af0: 0000 0072 5f01 0000 7260 0100 00a9 0c5a  ...r_...r`.....Z
 00004b00: 1270 616e 656c 5f67 7269 645f 6d69 6e6f  .panel_grid_mino
-00004b10: 725f 7872 1c01 0000 721b 0100 005a 0f70  r_xr....r....Z.p
-00004b20: 6c6f 745f 6261 636b 6772 6f75 6e64 721d  lot_backgroundr.
-00004b30: 0100 0072 6801 0000 7269 0100 005a 0c73  ...rh...ri...Z.s
+00004b10: 725f 7872 1b01 0000 721a 0100 005a 0f70  r_xr....r....Z.p
+00004b20: 6c6f 745f 6261 636b 6772 6f75 6e64 721c  lot_backgroundr.
+00004b30: 0100 0072 6701 0000 7268 0100 005a 0c73  ...rg...rh...Z.s
 00004b40: 7472 6970 5f74 6578 745f 785a 0c73 7472  trip_text_xZ.str
-00004b50: 6970 5f74 6578 745f 7972 1e01 0000 726a  ip_text_yr....rj
-00004b60: 0100 0072 c100 0000 7286 0100 0072 8501  ...r....r....r..
+00004b50: 6970 5f74 6578 745f 7972 1d01 0000 7269  ip_text_yr....ri
+00004b60: 0100 0072 c000 0000 7285 0100 0072 8401  ...r....r....r..
 00004b70: 0000 2902 5a0a 7869 6e74 6572 6365 7074  ..).Z.xintercept
-00004b80: 7260 0100 0029 0172 e700 0000 7249 0000  r`...).r....rI..
-00004b90: 0072 6f01 0000 da04 6e6f 6e65 2901 726c  .ro.....none).rl
-00004ba0: 0100 0072 a500 0000 5a0a 5f73 616d 655f  ...r....Z._same_
+00004b80: 725f 0100 0029 0172 e600 0000 7249 0000  r_...).r....rI..
+00004b90: 0072 6e01 0000 da04 6e6f 6e65 2901 726b  .rn.....none).rk
+00004ba0: 0100 0072 a400 0000 5a0a 5f73 616d 655f  ...r....Z._same_
 00004bb0: 786c 696d 7239 0000 005a 0f44 6966 6665  xlimr9...Z.Diffe
 00004bc0: 7265 6e74 5f78 6178 6973 5a0a 5361 6d65  rent_xaxisZ.Same
 00004bd0: 5f78 6178 6973 da06 6967 6e6f 7265 2902  _xaxis..ignore).
 00004be0: da06 6163 7469 6f6e da08 6361 7465 676f  ..action..catego
 00004bf0: 7279 da09 6869 7374 6f67 7261 6dda 0764  ry..histogram..d
 00004c00: 6566 6175 6c74 2921 da05 656d 7074 7972  efault)!..emptyr
-00004c10: 1f00 0000 7220 0000 0072 2601 0000 7229  ....r ...r&...r)
-00004c20: 0100 0072 2701 0000 7230 0100 005a 0e67  ...r'...r0...Z.g
+00004c10: 1f00 0000 7220 0000 0072 2501 0000 7228  ....r ...r%...r(
+00004c20: 0100 0072 2601 0000 722f 0100 005a 0e67  ...r&...r/...Z.g
 00004c30: 656f 6d5f 6869 7374 6f67 7261 6dda 1268  eom_histogram..h
 00004c40: 6973 746f 6772 616d 5f62 696e 7769 6474  istogram_binwidt
 00004c50: 68da 1468 6973 746f 6772 616d 5f66 6967  h..histogram_fig
-00004c60: 5f63 6f6c 6f75 7272 2f01 0000 726d 0000  _colourr/...rm..
-00004c70: 0072 6c00 0000 7277 0100 00da 1568 6973  .rl...rw.....his
+00004c60: 5f63 6f6c 6f75 7272 2e01 0000 726d 0000  _colourr....rm..
+00004c70: 0072 6c00 0000 7276 0100 00da 1568 6973  .rl...rv.....his
 00004c80: 746f 6772 616d 5f66 6967 5f6c 6162 656c  togram_fig_label
 00004c90: 5f78 da15 6869 7374 6f67 7261 6d5f 6669  _x..histogram_fi
-00004ca0: 675f 6c61 6265 6c5f 7972 3101 0000 7232  g_label_yr1...r2
-00004cb0: 0100 0072 3301 0000 7234 0100 0072 7501  ...r3...r4...ru.
-00004cc0: 0000 72d3 0000 0072 8a01 0000 728b 0100  ..r....r....r...
+00004ca0: 675f 6c61 6265 6c5f 7972 3001 0000 7231  g_label_yr0...r1
+00004cb0: 0100 0072 3201 0000 7233 0100 0072 7401  ...r2...r3...rt.
+00004cc0: 0000 72d2 0000 0072 8901 0000 728a 0100  ..r....r....r...
 00004cd0: 005a 0a67 656f 6d5f 766c 696e 65da 1868  .Z.geom_vline..h
 00004ce0: 6973 746f 6772 616d 5f73 7461 745f 6c69  istogram_stat_li
 00004cf0: 6e65 5f73 697a 655a 1273 6361 6c65 5f63  ne_sizeZ.scale_c
-00004d00: 6f6c 6f72 5f6d 616e 7561 6c72 7601 0000  olor_manualrv...
+00004d00: 6f6c 6f72 5f6d 616e 7561 6c72 7501 0000  olor_manualru...
 00004d10: da15 6869 7374 6f67 7261 6d5f 7368 6f77  ..histogram_show
-00004d20: 5f6c 6567 656e 6472 2c01 0000 da08 7761  _legendr,.....wa
+00004d20: 5f6c 6567 656e 6472 2b01 0000 da08 7761  _legendr+.....wa
 00004d30: 726e 696e 6773 da0c 7369 6d70 6c65 6669  rnings..simplefi
 00004d40: 6c74 6572 da0d 4675 7475 7265 5761 726e  lter..FutureWarn
 00004d50: 696e 6729 0972 3f00 0000 7281 0000 005a  ing).r?...r....Z
-00004d60: 0678 6c69 6d69 7472 7b01 0000 5a12 6669  .xlimitr{...Z.fi
+00004d60: 0678 6c69 6d69 7472 7a01 0000 5a12 6669  .xlimitrz...Z.fi
 00004d70: 6e64 5f78 6c69 6d5f 6675 6e63 7469 6f6e  nd_xlim_function
 00004d80: 7214 0000 0072 4000 0000 5a0d 7265 7475  r....r@...Z.retu
 00004d90: 726e 6564 5f78 6c69 6d72 5300 0000 7236  rned_xlimrS...r6
 00004da0: 0000 0072 3600 0000 7237 0000 0072 2700  ...r6...r7...r'.
 00004db0: 0000 c102 0000 7372 0000 0006 0206 0108  ......sr........
 00004dc0: 0104 0112 0306 0102 ff0c 0202 0102 0104  ................
 00004dd0: fe02 fe14 0504 0104 ff02 fb10 0702 f904  ................
 00004de0: 080c 010c 010a 010a 010c 010e 010e 010e  ................
 00004df0: 010e 010c 010c 0104 0104 f402 f802 ff0c  ................
 00004e00: 1a12 0104 0108 ff0e 0208 010a ff06 0410  ................
 00004e10: 0104 0210 020a 0110 0204 0208 010c 0106  ................
 00004e20: 0108 0104 010e 0310 020e 0204 027a 0e48  .............z.H
 00004e30: 6973 746f 6772 616d 2e6d 616b 654e 2908  istogram.makeN).
-00004e40: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
-00004e50: 8b00 0000 722c 0000 0072 7e01 0000 728c  ....r,...r~...r.
+00004e40: 7287 0000 0072 8800 0000 7289 0000 0072  r....r....r....r
+00004e50: 8a00 0000 722c 0000 0072 7d01 0000 728b  ....r,...r}...r.
 00004e60: 0000 0072 2700 0000 7236 0000 0072 3600  ...r'...r6...r6.
 00004e70: 0000 7236 0000 0072 3700 0000 722d 0000  ..r6...r7...r-..
 00004e80: 0061 0200 0073 0e00 0000 0800 0201 0a01  .a...s..........
 00004e90: 0235 0a01 0228 0e01 722d 0000 0063 0000  .5...(..r-...c..
 00004ea0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 00004eb0: 0000 4000 0000 7334 0000 0065 005a 0164  ..@...s4...e.Z.d
 00004ec0: 005a 0264 015a 0365 0464 0264 0384 0083  .Z.d.Z.e.d.d....
@@ -1264,15 +1264,15 @@
 00004ef0: 08da 0e43 6f6d 7061 7265 4f75 7470 7574  ...CompareOutput
 00004f00: 734e 6302 0000 0000 0000 0000 0000 0004  sNc.............
 00004f10: 0000 0005 0000 0043 0000 0073 2000 0000  .......C...s ...
 00004f20: 7c00 a000 7c01 a101 5c02 7d02 7d03 7c00  |...|...\.}.}.|.
 00004f30: a001 7c02 7c03 7c01 a103 0100 6400 5300  ..|.|.|.....d.S.
 00004f40: 2901 4e29 02da 0873 6574 7570 5f64 66da  ).N)...setup_df.
 00004f50: 0c4d 616b 655f 7363 6174 7465 7229 0472  .Make_scatter).r
-00004f60: 3000 0000 7214 0000 0072 b000 0000 7259  0...r....r....rY
+00004f60: 3000 0000 7214 0000 0072 af00 0000 7258  0...r....r....rX
 00004f70: 0100 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
 00004f80: 0000 da03 7275 6e07 0300 0073 0400 0000  ....run....s....
 00004f90: 0e02 1201 7a12 436f 6d70 6172 654f 7574  ....z.CompareOut
 00004fa0: 7075 7473 2e72 756e 6302 0000 0000 0000  puts.runc.......
 00004fb0: 0000 0000 000a 0000 0009 0000 0043 0000  .............C..
 00004fc0: 0073 b800 0000 6900 7d02 6700 7d03 7400  .s....i.}.g.}.t.
 00004fd0: 6401 8301 4400 5d3e 7d04 7401 6a02 6402  d...D.]>}.t.j.d.
@@ -1291,34 +1291,34 @@
 000050a0: 7075 7420 6279 2074 6865 2066 5241 5429  put by the fRAT)
 000050b0: 0172 5000 0000 7a29 2f53 756d 6d61 7269  .rP...z)/Summari
 000050c0: 7365 645f 7265 7375 6c74 732f 636f 6d62  sed_results/comb
 000050d0: 696e 6564 5f72 6573 756c 7473 2e6a 736f  ined_results.jso
 000050e0: 6e72 5b00 0000 6301 0000 0000 0000 0000  nr[...c.........
 000050f0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
 00005100: 1400 0000 6800 7c00 5d06 7d01 7c01 6400  ....h.|.].}.|.d.
-00005110: 1900 9202 7102 5300 2901 72f1 0000 0072  ....q.S.).r....r
-00005120: 3600 0000 2902 729a 0000 00da 0164 7236  6...).r......dr6
+00005110: 1900 9202 7102 5300 2901 72f0 0000 0072  ....q.S.).r....r
+00005120: 3600 0000 2902 7299 0000 00da 0164 7236  6...).r......dr6
 00005130: 0000 0072 3600 0000 7237 0000 00da 093c  ...r6...r7.....<
-00005140: 7365 7463 6f6d 703e 1803 0000 72ec 0000  setcomp>....r...
+00005140: 7365 7463 6f6d 703e 1803 0000 72eb 0000  setcomp>....r...
 00005150: 007a 2a43 6f6d 7061 7265 4f75 7470 7574  .z*CompareOutput
 00005160: 732e 7365 7475 705f 6466 2e3c 6c6f 6361  s.setup_df.<loca
 00005170: 6c73 3e2e 3c73 6574 636f 6d70 3e72 0100  ls>.<setcomp>r..
-00005180: 0000 7209 0000 00da 056f 7574 6572 72f1  ..r......outerr.
-00005190: 0000 0029 0272 8301 0000 7282 0100 0029  ...).r....r....)
-000051a0: 10da 0572 616e 6765 720a 0000 00da 0c66  ...ranger......f
+00005180: 0000 7208 0000 00da 056f 7574 6572 72f0  ..r......outerr.
+00005190: 0000 0029 0272 8201 0000 7281 0100 0029  ...).r....r....)
+000051a0: 10da 0572 616e 6765 7209 0000 00da 0c66  ...ranger......f
 000051b0: 696c 655f 6272 6f77 7365 7272 6e00 0000  ile_browserrn...
 000051c0: 7270 0000 0072 7100 0000 7267 0000 0072  rp...rq...rg...r
-000051d0: 6800 0000 72db 0000 0072 1600 0000 7219  h...r....r....r.
-000051e0: 0000 0072 7400 0000 72ae 0000 0072 8901  ...rt...r....r..
+000051d0: 6800 0000 72da 0000 0072 1600 0000 7219  h...r....r....r.
+000051e0: 0000 0072 7400 0000 72ad 0000 0072 8801  ...rt...r....r..
 000051f0: 0000 726d 0000 0072 6c00 0000 290a 7230  ..rm...rl...).r0
-00005200: 0000 0072 1400 0000 da03 6466 7372 5901  ...r......dfsrY.
-00005210: 0000 7209 0100 00da 0964 6972 6563 746f  ..r......directo
+00005200: 0000 0072 1400 0000 da03 6466 7372 5801  ...r......dfsrX.
+00005210: 0000 7208 0100 00da 0964 6972 6563 746f  ..r......directo
 00005220: 7279 da07 7265 7375 6c74 73da 0464 6174  ry..results..dat
 00005230: 615a 0472 6f69 735a 0364 666d 7236 0000  aZ.roisZ.dfmr6..
-00005240: 0072 3600 0000 7237 0000 0072 a201 0000  .r6...r7...r....
+00005240: 0072 3600 0000 7237 0000 0072 a101 0000  .r6...r7...r....
 00005250: 0c03 0000 731c 0000 0004 0204 010c 010c  ....s...........
 00005260: 0112 020a 010e 0112 0114 021e fb10 070c  ................
 00005270: 0106 ff08 037a 1743 6f6d 7061 7265 4f75  .....z.CompareOu
 00005280: 7470 7574 732e 7365 7475 705f 6466 6304  tputs.setup_dfc.
 00005290: 0000 0000 0000 0000 0000 0005 0000 0010  ................
 000052a0: 0000 0043 0000 0073 1c01 0000 7400 a001  ...C...s....t...
 000052b0: 7c01 7400 6a02 6401 6402 6403 8d02 a102  |.t.j.d.d.d.....
@@ -1335,59 +1335,59 @@
 00005360: 6413 6414 6415 8d03 7400 6a0e 6412 6416  d.d.d...t.j.d.d.
 00005370: 6413 6417 8d03 7400 6a0e 6412 6416 6413  d.d...t.j.d.d.d.
 00005380: 6417 8d03 7400 6a0e 6416 6413 6418 8d02  d...t.j.d.d.d...
 00005390: 7400 6a0e 6416 6413 6418 8d02 7c03 6a0f  t.j.d.d.d...|.j.
 000053a0: 6419 8d0c 1700 7d04 7c04 6a10 641a 7c03  d.....}.|.j.d.|.
 000053b0: 6a11 7c03 6a11 641b 1400 641c 641c 641d  j.|.j.d...d.d.d.
 000053c0: 8d05 0100 6400 5300 291e 4e5a 064d 6561  ....d.S.).NZ.Mea
-000053d0: 6e5f 785a 064d 6561 6e5f 7972 0f01 0000  n_xZ.Mean_yr....
-000053e0: 7214 0100 0054 7215 0100 0072 1601 0000  r....Tr....r....
-000053f0: da02 6c6d 2901 da06 6d65 7468 6f64 7209  ..lm)...methodr.
-00005400: 0000 0072 0100 0000 7217 0100 0072 5a01  ...r....r....rZ.
-00005410: 0000 728e 0100 0072 1901 0000 72a1 0000  ..r....r....r...
-00005420: 0072 1a01 0000 725b 0100 0072 5c01 0000  .r....r[...r\...
-00005430: 725d 0100 0072 5e01 0000 7266 0100 0072  r]...r^...rf...r
-00005440: 8f01 0000 7261 0100 0072 9001 0000 7a08  ....ra...r....z.
+000053d0: 6e5f 785a 064d 6561 6e5f 7972 0e01 0000  n_xZ.Mean_yr....
+000053e0: 7213 0100 0054 7214 0100 0072 1501 0000  r....Tr....r....
+000053f0: da02 6c6d 2901 da06 6d65 7468 6f64 7208  ..lm)...methodr.
+00005400: 0000 0072 0100 0000 7216 0100 0072 5901  ...r....r....rY.
+00005410: 0000 728d 0100 0072 1801 0000 72a0 0000  ..r....r....r...
+00005420: 0072 1901 0000 725a 0100 0072 5b01 0000  .r....rZ...r[...
+00005430: 725c 0100 0072 5d01 0000 7265 0100 0072  r\...r]...re...r
+00005440: 8e01 0000 7260 0100 0072 8f01 0000 7a08  ....r`...r....z.
 00005450: 5445 5354 2e70 6e67 7249 0000 0046 724a  TEST.pngrI...FrJ
-00005460: 0000 0029 1272 2601 0000 7229 0100 0072  ...).r&...r)...r
-00005470: 2701 0000 7230 0100 0072 3701 0000 722f  '...r0...r7...r/
+00005460: 0000 0029 1272 2501 0000 7228 0100 0072  ...).r%...r(...r
+00005470: 2601 0000 722f 0100 0072 3601 0000 722e  &...r/...r6...r.
 00005480: 0100 0072 6d00 0000 726c 0000 005a 0b67  ...rm...rl...Z.g
-00005490: 656f 6d5f 736d 6f6f 7468 7277 0100 0072  eom_smoothrw...r
-000054a0: 3101 0000 7232 0100 0072 3301 0000 7234  1...r2...r3...r4
-000054b0: 0100 0072 7501 0000 72d3 0000 0072 5100  ...ru...r....rQ.
-000054c0: 0000 7252 0000 0029 0572 3000 0000 72b0  ..rR...).r0...r.
-000054d0: 0000 0072 5901 0000 7214 0000 0072 4000  ...rY...r....r@.
+00005490: 656f 6d5f 736d 6f6f 7468 7276 0100 0072  eom_smoothrv...r
+000054a0: 3001 0000 7231 0100 0072 3201 0000 7233  0...r1...r2...r3
+000054b0: 0100 0072 7401 0000 72d2 0000 0072 5100  ...rt...r....rQ.
+000054c0: 0000 7252 0000 0029 0572 3000 0000 72af  ..rR...).r0...r.
+000054d0: 0000 0072 5801 0000 7214 0000 0072 4000  ...rX...r....r@.
 000054e0: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-000054f0: 0072 a301 0000 1f03 0000 7342 0000 0014  .r........sB....
+000054f0: 0072 a201 0000 1f03 0000 7342 0000 0014  .r........sB....
 00005500: 0306 0102 ff06 0202 fe14 0304 0104 ff02  ................
 00005510: fd0a 0502 fb14 0602 fa04 070c 010c 010a  ................
 00005520: 010a 010c 010e 010e 010e 010e 010c 010c  ................
 00005530: 0104 0104 f402 f902 ff0a 1808 0104 010a  ................
 00005540: fe7a 1b43 6f6d 7061 7265 4f75 7470 7574  .z.CompareOutput
 00005550: 732e 4d61 6b65 5f73 6361 7474 6572 2908  s.Make_scatter).
-00005560: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
-00005570: 7c01 0000 728b 0000 0072 a401 0000 72a2  |...r....r....r.
-00005580: 0100 0072 a301 0000 7236 0000 0072 3600  ...r....r6...r6.
-00005590: 0000 7236 0000 0072 3700 0000 72a1 0100  ..r6...r7...r...
+00005560: 7287 0000 0072 8800 0000 7289 0000 0072  r....r....r....r
+00005570: 7b01 0000 728a 0000 0072 a301 0000 72a1  {...r....r....r.
+00005580: 0100 0072 a201 0000 7236 0000 0072 3600  ...r....r6...r6.
+00005590: 0000 7236 0000 0072 3700 0000 72a0 0100  ..r6...r7...r...
 000055a0: 0004 0300 0073 1000 0000 0800 0401 0202  .....s..........
-000055b0: 0a01 0204 0a01 0212 0e01 72a1 0100 0029  ..........r....)
-000055c0: 2572 1f01 0000 7249 0100 0072 1600 0000  %r....rI...r....
-000055d0: 724e 0000 0072 9e01 0000 7203 0000 00da  rN...r....r.....
+000055b0: 0a01 0204 0a01 0212 0e01 72a0 0100 0029  ..........r....)
+000055c0: 2572 1e01 0000 7248 0100 0072 1600 0000  %r....rH...r....
+000055d0: 724e 0000 0072 9d01 0000 7203 0000 00da  rN...r....r.....
 000055e0: 0770 6174 686c 6962 7204 0000 00da 106d  .pathlibr......m
 000055f0: 6174 706c 6f74 6c69 622e 696d 6167 65da  atplotlib.image.
-00005600: 0569 6d61 6765 72c4 0000 00da 056e 756d  .imager......num
-00005610: 7079 72df 0000 00da 076e 6962 6162 656c  pyr......nibabel
-00005620: 72dd 0000 00da 0670 616e 6461 7372 6700  r......pandasrg.
-00005630: 0000 5a08 706c 6f74 6e69 6e65 7226 0100  ..Z.plotniner&..
+00005600: 0569 6d61 6765 72c3 0000 00da 056e 756d  .imager......num
+00005610: 7079 72de 0000 00da 076e 6962 6162 656c  pyr......nibabel
+00005620: 72dc 0000 00da 0670 616e 6461 7372 6700  r......pandasrg.
+00005630: 0000 5a08 706c 6f74 6e69 6e65 7225 0100  ..Z.plotniner%..
 00005640: 00da 0a73 696d 706c 656a 736f 6e72 7000  ...simplejsonrp.
 00005650: 0000 da07 6e69 6c65 6172 6e72 0500 0000  ....nilearnr....
 00005660: da0a 6d61 7470 6c6f 746c 6962 7206 0000  ..matplotlibr...
-00005670: 0072 a900 0000 da03 5049 4c72 0700 0000  .r......PILr....
-00005680: da03 7573 65da 0575 7469 6c73 720a 0000  ..use..utilsr...
-00005690: 0072 0b00 0000 7226 0000 0072 2a00 0000  .r....r&...r*...
-000056a0: 722b 0000 0072 2d00 0000 72a1 0100 0072  r+...r-...r....r
+00005670: 0072 a800 0000 da03 5049 4c72 0700 0000  .r......PILr....
+00005680: da05 7574 696c 7372 0900 0000 da03 7573  ..utilsr......us
+00005690: 6572 0b00 0000 7226 0000 0072 2a00 0000  er....r&...r*...
+000056a0: 722b 0000 0072 2d00 0000 72a0 0100 0072  r+...r-...r....r
 000056b0: 3600 0000 7236 0000 0072 3600 0000 7237  6...r6...r6...r7
 000056c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 000056d0: 0073 3a00 0000 0800 0801 0801 0801 0801  .s:.............
 000056e0: 0c01 0c01 0c02 0801 0801 0801 0801 0801  ................
-000056f0: 0c01 0c01 0c01 0802 0a01 0c02 0e03 007f  ................
+000056f0: 0c01 0c01 0c01 0c02 0802 0a01 0e03 007f  ................
 00005700: 1012 007f 007f 100b 103f 106f 007f 1424  .........?.o...$
```

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.4.0/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/analysis.py` & `frat_brain-1.4.0/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/bootstrap.css` & `frat_brain-1.4.0/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/dash_report.py` & `frat_brain-1.4.0/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/directory_comparison.py` & `frat_brain-1.4.0/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.4.0/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/figures.py` & `frat_brain-1.4.0/fRAT/utils/figures.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from nilearn import plotting
 from matplotlib import pyplot as plt
 from PIL import Image
 
 from .utils import Utils
 
 import matplotlib
-matplotlib.use('agg') # Use non-GUI backend to prevent memory leak caused by creating subplots in a loop
+matplotlib.use('agg')  # Use non-GUI backend to prevent memory leak caused by creating subplots in a loop
 
 
 class Figures:
     config = None
 
     @classmethod
     def make_figures(cls, cfg, config_path, config_filename):
```

### Comparing `frat_brain-1.3.7/fRAT/utils/html_report.py` & `frat_brain-1.4.0/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/printResults.py` & `frat_brain-1.4.0/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/statistics.py` & `frat_brain-1.4.0/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/statmap.py` & `frat_brain-1.4.0/fRAT/utils/statmap.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.4.0/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/fRAT/utils/utils.py` & `frat_brain-1.4.0/fRAT/utils/utils.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.7/pyproject.toml` & `frat_brain-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.3.7"
+version = "1.4.0"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.3.7/setup.py` & `frat_brain-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.3.7',
+    'version': '1.4.0',
     'description': 'Application for ROI fMRI data analysis.',
     'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
```

### Comparing `frat_brain-1.3.7/PKG-INFO` & `frat_brain-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.3.7
+Version: 1.4.0
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

