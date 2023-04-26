# Comparing `tmp/recon_lw-2.0.0.dev4807700343.tar.gz` & `tmp/recon_lw-2.0.0.dev4808598137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4807700343.tar", last modified: Wed Apr 26 10:36:01 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4808598137.tar", last modified: Wed Apr 26 12:22:56 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4807700343.tar` & `recon_lw-2.0.0.dev4808598137.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-26 10:35:37.000000 recon_lw-2.0.0.dev4807700343/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    19709 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 10:36:01.000000 recon_lw-2.0.0.dev4807700343/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-26 10:35:30.000000 recon_lw-2.0.0.dev4807700343/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-26 12:22:35.000000 recon_lw-2.0.0.dev4808598137/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2757 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19709 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 12:22:56.000000 recon_lw-2.0.0.dev4808598137/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-26 12:22:27.000000 recon_lw-2.0.0.dev4808598137/setup.py
```

### Comparing `recon_lw-2.0.0.dev4807700343/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4808598137/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4807700343/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4808598137/recon_lw/TimeCacheMatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,22 @@
         self._horizon_delay_seconds = horizon_delay_seconds
         self._custom_settings = custom_settings
 
     def process_objects_batch(self, batch):
         stream_time = None
         for o in batch:
             ts, key1, key2 = self._get_timestamp_key1_key2(o, self._custom_settings)
+            log_event =  self._create_event ("MatcherLog" + str(self._custom_settings),
+                                             "MatcherLog",
+                                             False,
+                                             {"ts": ts,
+                                              "key1": key1,
+                                              "key2": key2,
+                                              "sourceEventId": o["eventId"]})
+            self._send_events([log_event])
             if ts is None:
                 continue
             stream_time = ts
             if key1 is not None:
                 if key1 not in self._match_index:
                     self._match_index[key1] = [o, None]
                     self._time_index.add([ts, key1])
```

### Comparing `recon_lw-2.0.0.dev4807700343/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4808598137/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4807700343/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4807700343/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4808598137/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4807700343/setup.py` & `recon_lw-2.0.0.dev4808598137/setup.py`

 * *Files identical despite different names*

