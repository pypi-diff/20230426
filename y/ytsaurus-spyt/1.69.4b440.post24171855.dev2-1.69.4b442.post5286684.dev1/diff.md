# Comparing `tmp/ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar.gz` & `tmp/ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar", last modified: Tue Apr 18 10:21:21 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar", last modified: Wed Apr 26 10:19:35 2023, max compression
```

## Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2.tar` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11036 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-18 10:21:20.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-10 15:29:49.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3493 2023-03-18 23:30:06.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35663 2023-04-18 10:20:39.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-03-14 10:41:35.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-04-18 10:20:58.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-02-22 20:15:30.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-10 10:41:56.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-18 10:21:21.000000 ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35832 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-04-26 10:19:12.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-20 21:24:26.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-20 21:24:26.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.cfg
```

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-launch-yt`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,21 @@
     group = parser.add_mutually_exclusive_group(required=False)
     group.add_argument('--enable-mtn', dest='enable_mtn', action='store_true')
     group.add_argument('--disable-mtn', dest='enable_mtn',
                        action='store_false')
     parser.set_defaults(enable_mtn=default_enablers.enable_mtn)
 
     group = parser.add_mutually_exclusive_group(required=False)
+    group.add_argument('--prefer-ipv6', dest='enable_preference_ipv6',
+                       action='store_true')
+    group.add_argument('--prefer-ipv4', dest='enable_preference_ipv6',
+                       action='store_false')
+    parser.set_defaults(enable_preference_ipv6=default_enablers.enable_preference_ipv6)
+
+    group = parser.add_mutually_exclusive_group(required=False)
     group.add_argument('--enable-advanced-event-log',
                        dest='advanced_event_log', action='store_true')
     group.add_argument('--disable-advanced-event-log',
                        dest='advanced_event_log', action='store_false')
     parser.set_defaults(advanced_event_log=False)
 
     group = parser.add_mutually_exclusive_group(required=False)
@@ -172,15 +179,16 @@
                         params=args.params,
                         shs_location=args.shs_location,
                         spark_cluster_version=args.spark_cluster_version,
                         enablers=SpytEnablers(
                             enable_byop=args.enable_byop,
                             enable_profiling=args.enable_profiling,
                             enable_mtn=args.enable_mtn,
-                            enable_solomon_agent=args.enable_solomon_agent
+                            enable_solomon_agent=args.enable_solomon_agent,
+                            enable_preference_ipv6=args.enable_preference_ipv6
                         ),
                         client=yt_client,
                         preemption_mode=args.preemption_mode,
                         enable_multi_operation_mode=args.enable_multi_operation_mode,
                         dedicated_operation_mode=args.dedicated_operation_mode,
                         driver_cores=args.driver_cores,
                         driver_memory=args.driver_memory,
```

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/client.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/common.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/conf.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/enabler.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/enabler.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(name)s - %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class SpytEnablers(object):
     def __init__(self, enable_byop=True, enable_profiling=False, enable_arrow=None,
-                 enable_mtn=False, enable_solomon_agent=True):
+                 enable_mtn=False, enable_solomon_agent=True, enable_preference_ipv6=True):
         self.enable_byop = enable_byop
         self.enable_profiling = enable_profiling
         self.enable_arrow = enable_byop if enable_arrow is None else enable_arrow
         self.enable_mtn = enable_mtn
         self.enable_solomon_agent = enable_solomon_agent
+        self.enable_preference_ipv6 = enable_preference_ipv6
         self.config_enablers = {}
 
     def _get_enabler(self, enabler, enabler_name):
         config_enabler = self.config_enablers.get(enabler_name) or False
         if enabler and not config_enabler:
             logger.warning("{} is enabled in start arguments, but disabled for current cluster version. "
                            "It will be disabled".format(enabler_name))
@@ -25,31 +26,34 @@
 
     def apply_config(self, config):
         self.config_enablers = config.get("enablers") or {}
         self.enable_byop = self._get_enabler(self.enable_byop, "enable_byop")
         self.enable_arrow = self._get_enabler(self.enable_arrow, "enable_arrow")
         self.enable_mtn = self._get_enabler(self.enable_mtn, "enable_mtn")
         self.enable_solomon_agent = self._get_enabler(self.enable_solomon_agent, "enable_solomon_agent")
+        self.enable_preference_ipv6 = self._get_enabler(self.enable_preference_ipv6, "enable_preference_ipv6")
 
     def get_spark_conf(self):
         enable_byop_conf_name = "spark.hadoop.yt.byop.enabled"
         enable_arrow_conf_name = "spark.hadoop.yt.read.arrow.enabled"
         enable_profiling_conf_name = "spark.hadoop.yt.profiling.enabled"
         enable_mtn_conf_name = "spark.hadoop.yt.mtn.enabled"
         enable_solomon_agent_name = "spark.hadoop.yt.solomonAgent.enabled"
+        enable_preference_ipv6_name = "spark.hadoop.yt.preferenceIpv6.enabled"
         enablers = [
             enable_byop_conf_name, enable_profiling_conf_name, enable_arrow_conf_name,
-            enable_mtn_conf_name, enable_solomon_agent_name
+            enable_mtn_conf_name, enable_solomon_agent_name, enable_preference_ipv6_name
         ]
         return {
             enable_byop_conf_name: str(self.enable_byop),
             enable_profiling_conf_name: str(self.enable_profiling),
             enable_arrow_conf_name: str(self.enable_arrow),
             enable_mtn_conf_name: str(self.enable_mtn),
             enable_solomon_agent_name: str(self.enable_solomon_agent),
+            enable_preference_ipv6_name: str(self.enable_preference_ipv6),
             "spark.yt.enablers": ",".join(enablers)
         }
 
 
 SPARK_DEFAULTS = SpytEnablers().get_spark_conf()
 
 def safe_get(d, key):
```

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/standalone.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/standalone.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,36 +213,27 @@
     _add_python_version(python_version, spark_base_args, client)
     _add_dedicated_driver_op_conf(spark_base_args, dedicated_driver_op)
     spark_env = _create_spark_env(client, spark_home)
 
     if local_files:
         remote_paths = {}
         new_spark_args = []
-        local_files_pattern = "[A-Za-z0-9]+:\/[^,]+(,[A-Za-z0-9]+:\/[^,]+)*" # Matches "FS:/..." path sequence
         for spark_arg in spark_args:
-            is_file_list = re.fullmatch(local_files_pattern, spark_arg)
-            if not is_file_list:
-                continue
-            file_list = spark_arg.split(",")
-            new_file_list = []
-            for single_file in file_list:
-                if single_file.startswith('local:/'):
-                    local_file_path = single_file[7:] # Drops prefix
-                    if local_file_path not in remote_paths:
-                        _, file_extension = os.path.splitext(local_file_path)
-                        destination = upload_file_to_cache(local_file_path, client=client)
-                        destination_ext = "{}{}".format(destination, file_extension)
-                        cypress_copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
-                        logger.info("%s has been uploaded to YT as %s", local_file_path, destination_ext)
-                        remote_paths[local_file_path] = "yt:/{}".format(destination_ext)
-                    new_file_list.append(remote_paths[local_file_path])
-                else:
-                    new_file_list.append(single_file)
-            new_spark_arg = ",".join(new_file_list)
-            new_spark_args.append(new_spark_arg)
+            if spark_arg.startswith('local:/'):
+                if spark_arg not in remote_paths:
+                    file_path = spark_arg[7:] # Drops prefix
+                    _, file_extension = os.path.splitext(file_path)
+                    destination = upload_file_to_cache(file_path, client=client)
+                    destination_ext = "{}{}".format(destination, file_extension)
+                    cypress_copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
+                    logger.info("%s has been uploaded to YT as %s", file_path, destination_ext)
+                    remote_paths[spark_arg] = "yt:/{}".format(destination_ext)
+                new_spark_args.append(remote_paths[spark_arg])
+            else:
+                new_spark_args.append(spark_arg)
         spark_args = new_spark_args
 
     # replace stdin to avoid https://bugs.openjdk.java.net/browse/JDK-8211842
     return subprocess.call(spark_base_args + spark_args, env=spark_env, stdin=subprocess.PIPE)
 
 
 def _add_dedicated_driver_op_conf(spark_args, dedicated_driver_op):
@@ -335,27 +326,34 @@
         spark_home = "."
     else:
         spark_home = "./tmpfs"
 
     def script_path(script):
         return "{}/{}".format(spark_home, driver_op_discovery_script)
 
-    def _launcher_command(component, xmx="512m"):
+    def _launcher_command(component, xmx="512m", additional_java_opts=None):
+        additional_java_opts = additional_java_opts or []
         create_dir = "mkdir -p {}".format(spark_home)
         unpack_tar = "tar --warning=no-unknown-keyword -xf spark.tgz -C {}".format(
             spark_home)
         move_java = "cp -r /opt/jdk11 ./tmpfs/jdk11"
-        run_launcher = "./tmpfs/jdk11/bin/java -Xmx{0} -cp spark-yt-launcher.jar -Djava.net.preferIPv6Addresses=true".format(
-            xmx)
+        run_launcher = "./tmpfs/jdk11/bin/java -Xmx{0} -cp spark-yt-launcher.jar {1}".format(
+            xmx, " ".join(additional_java_opts))
         spark_conf = get_spark_conf(config=config, enablers=enablers)
 
         return "{5} && {0} && {1} && {2} {3} tech.ytsaurus.spark.launcher.{4}Launcher ".format(
             unpack_tar, move_java, run_launcher, spark_conf, component, create_dir)
 
-    master_command = _launcher_command("Master")
+    additional_java_opts = []
+    if enablers.enable_preference_ipv6:
+        additional_java_opts.append("-Djava.net.preferIPv6Addresses=true")
+        config["spark_conf"]["spark.driver.extraJavaOptions"] = "-Djava.net.preferIPv6Addresses=true"
+        config["spark_conf"]["spark.executor.extraJavaOptions"] = "-Djava.net.preferIPv6Addresses=true"
+
+    master_command = _launcher_command("Master", additional_java_opts=additional_java_opts)
 
     def _script_absolute_path(script):
         return "{}/{}".format(spark_home, script)
 
     worker_log_location = "yt:/{}".format(spark_discovery.worker_log())
     if "spark.workerLog.tablePath" not in config["spark_conf"]:
         config["spark_conf"]["spark.workerLog.tablePath"] = worker_log_location
@@ -371,30 +369,30 @@
     if autoscaler_enabled:
         config["spark_conf"]["spark.worker.resource.jobid.amount"] = "1"
         config["spark_conf"]["spark.worker.resource.jobid.discoveryScript"] = _script_absolute_path(
             "spark/bin/job-id-discovery.sh")
         config["spark_conf"]["spark.driver.resource.jobid.discoveryScript"] = _script_absolute_path(
             "spark/bin/job-id-discovery.sh")
 
-    worker_command = _launcher_command("Worker", "2g") + \
+    worker_command = _launcher_command("Worker", "2g", additional_java_opts=additional_java_opts) + \
         "--cores {0} --memory {1} --wait-master-timeout {2} --wlog-service-enabled {3} " \
         "--wlog-enable-json {4} --wlog-update-interval {5} --wlog-table-path {6} " \
         "--wlog-table-ttl {7}".format(
             worker.cores, worker.memory, worker.timeout, worker_log_transfer, worker_log_json_mode,
             worker_log_update_interval, worker_log_location, worker_log_table_ttl)
 
     if advanced_event_log:
         event_log_path = "ytEventLog:/{}".format(
             shs_location or spark_discovery.event_log_table())
     else:
         event_log_path = "yt:/{}".format(
             shs_location or spark_discovery.event_log())
     if "spark.history.fs.numReplayThreads" not in config["spark_conf"]:
         config["spark_conf"]["spark.history.fs.numReplayThreads"] = history_server_cpu_limit
-    history_command = _launcher_command("HistoryServer") + \
+    history_command = _launcher_command("HistoryServer", additional_java_opts=additional_java_opts) + \
         "--log-path {} --memory {}".format(event_log_path,
                                            history_server_memory_limit)
 
     user = get_user_name(client=client)
 
     operation_spec = config["operation_spec"]
 
@@ -415,14 +413,15 @@
         "Spark over YT": {
             "discovery_path": spark_discovery.base_discovery_path,
             "cluster_version": config["cluster_version"],
             "client_version": __version__,
             "enable_byop": enablers.enable_byop,
             "enable_arrow": enablers.enable_arrow,
             "enable_mtn": enablers.enable_mtn,
+            "enable_preference_ipv6": enablers.enable_preference_ipv6,
             "job_types": job_types
         }
     }
 
     operation_spec['preemption_mode'] = preemption_mode
 
     environment = config["environment"]
@@ -439,15 +438,16 @@
     environment["SPARK_LOCAL_DIRS"] = "./tmpfs"
     environment["SPARK_YT_SOLOMON_ENABLED"] = str(enablers.enable_solomon_agent)
     environment["SOLOMON_PUSH_PORT"] = "27099"
 
     ytserver_proxy_path = config.get("ytserver_proxy_path")
 
     worker_environment = {
-        "SPARK_YT_BYOP_ENABLED": str(enablers.enable_byop)
+        "SPARK_YT_BYOP_ENABLED": str(enablers.enable_byop),
+        "SPARK_YT_IPV6_PREFERENCE_ENABLED": str(enablers.enable_preference_ipv6)
     }
     worker_environment = update(environment, worker_environment)
     if enablers.enable_byop:
         ytserver_binary_name = ytserver_proxy_path.split(
             "/")[-1] if ytserver_proxy_path else "ytserver-proxy"
         byop_worker_environment = {
             "SPARK_YT_BYOP_BINARY_PATH": "$HOME/{}".format(ytserver_binary_name),
```

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/submit.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/types.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/spyt/utils.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b440.post24171855.dev2/setup.py` & `ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.py`

 * *Files identical despite different names*

