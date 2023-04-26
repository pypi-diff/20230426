# Comparing `tmp/jupyterhub-backendspawner-0.1.5.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.5.tar", last modified: Wed Apr 26 11:17:10 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.6.tar", last modified: Wed Apr 26 14:22:59 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.5.tar` & `jupyterhub-backendspawner-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.5/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.5/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.5/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.5/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.1.5/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10080 2023-04-25 13:29:32.000000 jupyterhub-backendspawner-0.1.5/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-26 11:16:45.000000 jupyterhub-backendspawner-0.1.5/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:22:59.470335 jupyterhub-backendspawner-0.1.6/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.6/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 14:22:59.470335 jupyterhub-backendspawner-0.1.6/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.6/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:22:59.470335 jupyterhub-backendspawner-0.1.6/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.6/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5140 2023-04-26 14:17:35.000000 jupyterhub-backendspawner-0.1.6/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.1.6/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10170 2023-04-26 14:16:45.000000 jupyterhub-backendspawner-0.1.6/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:22:59.470335 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 14:22:59.000000 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-26 14:22:59.000000 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 14:22:59.000000 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-26 14:22:59.000000 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-26 14:22:59.000000 jupyterhub-backendspawner-0.1.6/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 14:22:59.470335 jupyterhub-backendspawner-0.1.6/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-26 14:21:26.000000 jupyterhub-backendspawner-0.1.6/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.5/LICENSE` & `jupyterhub-backendspawner-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.5/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.6/backendspawner/api_events.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,15 +62,25 @@
                         "uuidcode": uuidcode,
                         "log_name": f"{user_name}:{server_name}",
                         "user": user_name,
                         "action": "cancel",
                         "event": event,
                     },
                 )
-                asyncio.create_task(spawner.stop(cancel=True, event=None))
+                # Add correct timestamp to event, at the moment it will be used.
+                async def stop_event(spawner):
+                    now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
+                    return {
+                        "failed": True,
+                        "ready": False,
+                        "progress": 100,
+                        "message": "",
+                        "html_message": f"<details><summary>{now}: {user_cancel_message}",
+                    }
+                asyncio.create_task(spawner.stop(cancel=True, event=stop_event))
             else:
                 self.log.debug(
                     "APICall: SpawnUpdate",
                     extra={
                         "uuidcode": uuidcode,
                         "log_name": f"{user_name}:{server_name}",
                         "user": user_name,
```

### Comparing `jupyterhub-backendspawner-0.1.5/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.6/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.5/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.6/backendspawner/eventspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,11 +270,13 @@
         try:
             # always use cancel=False, and call the function later if neccessary.
             # Otherwise the stop_event would be attached after run_post_stop_hook was called.
             await super().stop(now, cancel=False)
         finally:
             if not event:
                 event = await self.get_stop_event()
+            elif callable(event):
+                event = await maybe_future(event(self))
             self.latest_events.append(event)
 
         if cancel:
             await self.cancel()
```

### Comparing `jupyterhub-backendspawner-0.1.5/setup.py` & `jupyterhub-backendspawner-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.5",
+    version="0.1.6",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

