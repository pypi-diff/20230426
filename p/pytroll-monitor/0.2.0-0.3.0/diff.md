# Comparing `tmp/pytroll-monitor-0.2.0.tar.gz` & `tmp/pytroll-monitor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytroll-monitor-0.2.0.tar", last modified: Mon Jul 18 07:57:41 2022, max compression
+gzip compressed data, was "pytroll-monitor-0.3.0.tar", last modified: Wed Apr 26 12:55:51 2023, max compression
```

## Comparing `pytroll-monitor-0.2.0.tar` & `pytroll-monitor-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/pytroll_monitor/
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/checkmk_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/createTestcase.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/monitor_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/op5_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     7595 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/pytroll_monitor/pps_posttroll_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/pytroll_monitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-18 07:57:41.000000 pytroll-monitor-0.2.0/pytroll_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-18 07:57:41.108011 pytroll-monitor-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68587 2022-07-18 07:57:40.000000 pytroll-monitor-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/pytroll_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/checkmk_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/createTestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/monitor_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/op5_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/pytroll_monitor/pps_posttroll_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/pytroll_monitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 12:55:51.000000 pytroll-monitor-0.3.0/pytroll_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 12:55:51.323233 pytroll-monitor-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68587 2023-04-26 12:55:50.000000 pytroll-monitor-0.3.0/versioneer.py
```

### Comparing `pytroll-monitor-0.2.0/README.md` & `pytroll-monitor-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/__init__.py` & `pytroll-monitor-0.3.0/pytroll_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/checkmk_logger.py` & `pytroll-monitor-0.3.0/pytroll_monitor/checkmk_logger.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/createTestcase.py` & `pytroll-monitor-0.3.0/pytroll_monitor/createTestcase.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/monitor_hook.py` & `pytroll-monitor-0.3.0/pytroll_monitor/monitor_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 """A generic OP5 post hook to be run to update the passive monitoring status."""
 
 import os
 import logging
 import requests
 import json
-from six.moves.urllib.parse import urljoin
+from urllib.parse import urljoin
 
 LOG = logging.getLogger(__name__)
 
 
 class OP5Monitor(object):
     """A class to trigger the sending of a notification to an Op5 monitor server."""
```

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/op5_logger.py` & `pytroll-monitor-0.3.0/pytroll_monitor/op5_logger.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/pytroll_monitor/pps_posttroll_hook.py` & `pytroll-monitor-0.3.0/pytroll_monitor/pps_posttroll_hook.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/setup.py` & `pytroll-monitor-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytroll-monitor-0.2.0/versioneer.py` & `pytroll-monitor-0.3.0/versioneer.py`

 * *Files identical despite different names*

