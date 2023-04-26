# Comparing `tmp/jupyterhub-backendspawner-0.1.4.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.4.tar", last modified: Tue Apr 25 13:31:28 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.5.tar", last modified: Wed Apr 26 11:17:10 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.4.tar` & `jupyterhub-backendspawner-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.4/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.4/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.4/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.4/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-25 12:26:26.000000 jupyterhub-backendspawner-0.1.4/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10080 2023-04-25 13:29:32.000000 jupyterhub-backendspawner-0.1.4/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 13:31:23.000000 jupyterhub-backendspawner-0.1.4/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.5/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.5/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.5/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.5/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.1.5/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10080 2023-04-25 13:29:32.000000 jupyterhub-backendspawner-0.1.5/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-26 11:17:10.000000 jupyterhub-backendspawner-0.1.5/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 11:17:10.301560 jupyterhub-backendspawner-0.1.5/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-26 11:16:45.000000 jupyterhub-backendspawner-0.1.5/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.4/LICENSE` & `jupyterhub-backendspawner-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.4/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.5/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.4/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.5/backendspawner/backendspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,19 +178,19 @@
         """
     ).tag(config=True)
 
     @default("failed_spawn_request_hook")
     def _failed_spawn_request_hook(self):
         return self._default_failed_spawn_request_hook
 
-    def _default_failed_spawn_request_hook(self, exception):
+    def _default_failed_spawn_request_hook(self, spawner, exception):
         return
 
     def run_failed_spawn_request_hook(self, exception):
-        return self.failed_spawn_request_hook(exception)
+        return self.failed_spawn_request_hook(self, exception)
 
     post_spawn_request_hook = Callable(
         help="""
         If a start of a single-user server was successful, you can run additional commands here.
         This allows you to handle a successful start attempt properly, according to
         your specific backend API.
         
@@ -203,24 +203,15 @@
         """
     ).tag(config=True)
 
     @default("post_spawn_request_hook")
     def _post_spawn_request_hook(self):
         return self._default_post_spawn_request_hook
 
-    def _default_post_spawn_request_hook(self, resp_json):
-        self.log.info(
-            f"Start communication with backend answered with: {resp_json}.",
-            extra={
-                "uuidcode": self.name,
-                "log_name": self._log_name,
-                "user": self.user.name,
-                "action": "start",
-            },
-        )
+    def _default_post_spawn_request_hook(self, spawner, resp_json):
         return
 
     def run_post_spawn_request_hook(self, resp_json):
         return self.post_spawn_request_hook(self, resp_json)
 
     request_url_poll = Union(
         [Unicode(), Callable()],
```

### Comparing `jupyterhub-backendspawner-0.1.4/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.5/backendspawner/eventspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.4/setup.py` & `jupyterhub-backendspawner-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.4",
+    version="0.1.5",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

