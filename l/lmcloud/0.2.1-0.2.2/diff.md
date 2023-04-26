# Comparing `tmp/lmcloud-0.2.1.tar.gz` & `tmp/lmcloud-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.2.1.tar", last modified: Wed Apr 26 06:19:48 2023, max compression
+gzip compressed data, was "lmcloud-0.2.2.tar", last modified: Wed Apr 26 08:49:39 2023, max compression
```

## Comparing `lmcloud-0.2.1.tar` & `lmcloud-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:48.374198 lmcloud-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 06:19:24.000000 lmcloud-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 06:19:48.374198 lmcloud-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-26 06:19:24.000000 lmcloud-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:48.370197 lmcloud-0.2.1/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20838 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-26 06:19:24.000000 lmcloud-0.2.1/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:48.374198 lmcloud-0.2.1/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 06:19:48.000000 lmcloud-0.2.1/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 06:19:48.000000 lmcloud-0.2.1/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:48.000000 lmcloud-0.2.1/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 06:19:48.000000 lmcloud-0.2.1/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 06:19:48.000000 lmcloud-0.2.1/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:19:48.374198 lmcloud-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-26 06:19:24.000000 lmcloud-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.488324 lmcloud-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 08:49:25.000000 lmcloud-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 08:49:39.488324 lmcloud-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-26 08:49:25.000000 lmcloud-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.484324 lmcloud-0.2.2/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-26 08:49:25.000000 lmcloud-0.2.2/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:49:39.488324 lmcloud-0.2.2/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 08:49:39.000000 lmcloud-0.2.2/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:49:39.488324 lmcloud-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-26 08:49:25.000000 lmcloud-0.2.2/setup.py
```

### Comparing `lmcloud-0.2.1/LICENSE` & `lmcloud-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.1/PKG-INFO` & `lmcloud-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.2.1/README.md` & `lmcloud-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.1/lmcloud/const.py` & `lmcloud-0.2.2/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.1/lmcloud/helpers.py` & `lmcloud-0.2.2/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.1/lmcloud/lmcloud.py` & `lmcloud-0.2.2/lmcloud/lmcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 conf = await self._lm_local_api.local_get_config()
                 self._config = {k.upper():v for k,v in conf.items()}
             except RequestException as e:
                 _logger.warn(f"Could not connect to local API although initialized. Full error: {e}")
                 await self._update_config_obj()
 
             if self._lm_local_api._timestamp_last_websocket_msg == None or (datetime.now() - self._lm_local_api._timestamp_last_websocket_msg).total_seconds() > 30: 
-                if not in_init: # during init we don't want to log this warning
+                if self._use_websocket and not in_init: # during init we don't want to log this warning
                     _logger.warn("Could not get local machine status. Falling back to cloud status.")
                 await self._update_status_obj()
                 self._status[ACTIVE_BREW] = False
             else:
                 # Get local status from WebSockets
                 print("Using local status")
                 self._status = self._lm_local_api._status # reference to the same object tp get websocket updates
```

### Comparing `lmcloud-0.2.1/lmcloud/lmlocalapi.py` & `lmcloud-0.2.2/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.2.1/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.2.2/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.2.1/setup.py` & `lmcloud-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.2.1",
+    version="0.2.2",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

