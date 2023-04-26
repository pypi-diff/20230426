# Comparing `tmp/yea-wandb-0.9.6.tar.gz` & `tmp/yea-wandb-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yea-wandb-0.9.6.tar", last modified: Fri Mar 17 22:37:20 2023, max compression
+gzip compressed data, was "yea-wandb-0.9.7.tar", last modified: Wed Apr 26 18:34:11 2023, max compression
```

## Comparing `yea-wandb-0.9.6.tar` & `yea-wandb-0.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/
--rw-r--r--   0 kpt        (501) staff       (20)     1075 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/LICENSE
--rw-r--r--   0 kpt        (501) staff       (20)       58 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/MANIFEST.in
--rw-r--r--   0 kpt        (501) staff       (20)      154 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/PKG-INFO
--rw-r--r--   0 kpt        (501) staff       (20)      885 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/README.md
--rw-r--r--   0 kpt        (501) staff       (20)      112 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/pyproject.toml
--rw-r--r--   0 kpt        (501) staff       (20)       38 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/setup.cfg
--rw-r--r--   0 kpt        (501) staff       (20)      543 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/setup.py
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb/
--rw-r--r--   0 kpt        (501) staff       (20)       68 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/__init__.py
--rw-r--r--   0 kpt        (501) staff       (20)     6163 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/src/yea_wandb/artifact_emu.py
--rwxr-xr-x   0 kpt        (501) staff       (20)     8519 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/backend.py
--rw-r--r--   0 kpt        (501) staff       (20)     1676 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/hook.py
--rw-r--r--   0 kpt        (501) staff       (20)     3486 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/mitm.py
--rw-r--r--   0 kpt        (501) staff       (20)     9312 2022-08-19 03:13:13.000000 yea-wandb-0.9.6/src/yea_wandb/mock_requests.py
--rw-r--r--   0 kpt        (501) staff       (20)   105508 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/mock_server.py
--rw-r--r--   0 kpt        (501) staff       (20)    10623 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/plugin.py
--rw-r--r--   0 kpt        (501) staff       (20)     4847 2023-03-17 22:36:04.000000 yea-wandb-0.9.6/src/yea_wandb/setup.py
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/
--rw-r--r--   0 kpt        (501) staff       (20)      154 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/PKG-INFO
--rw-r--r--   0 kpt        (501) staff       (20)      545 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 kpt        (501) staff       (20)        1 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 kpt        (501) staff       (20)       43 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/entry_points.txt
--rw-r--r--   0 kpt        (501) staff       (20)        1 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/not-zip-safe
--rw-r--r--   0 kpt        (501) staff       (20)       43 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/requires.txt
--rw-r--r--   0 kpt        (501) staff       (20)       10 2023-03-17 22:37:20.000000 yea-wandb-0.9.6/src/yea_wandb.egg-info/top_level.txt
+drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.809271 yea-wandb-0.9.7/
+-rw-r--r--   0 kpt        (501) staff       (20)     1075 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/LICENSE
+-rw-r--r--   0 kpt        (501) staff       (20)       58 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/MANIFEST.in
+-rw-r--r--   0 kpt        (501) staff       (20)      154 2023-04-26 18:34:11.808911 yea-wandb-0.9.7/PKG-INFO
+-rw-r--r--   0 kpt        (501) staff       (20)      885 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/README.md
+-rw-r--r--   0 kpt        (501) staff       (20)      112 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/pyproject.toml
+-rw-r--r--   0 kpt        (501) staff       (20)       38 2023-04-26 18:34:11.809368 yea-wandb-0.9.7/setup.cfg
+-rw-r--r--   0 kpt        (501) staff       (20)      543 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/setup.py
+drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.794563 yea-wandb-0.9.7/src/
+drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.804062 yea-wandb-0.9.7/src/yea_wandb/
+-rw-r--r--   0 kpt        (501) staff       (20)       68 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/src/yea_wandb/__init__.py
+-rw-r--r--   0 kpt        (501) staff       (20)     6163 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/src/yea_wandb/artifact_emu.py
+-rwxr-xr-x   0 kpt        (501) staff       (20)     8703 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/src/yea_wandb/backend.py
+-rw-r--r--   0 kpt        (501) staff       (20)     1676 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/hook.py
+-rw-r--r--   0 kpt        (501) staff       (20)     3486 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/mitm.py
+-rw-r--r--   0 kpt        (501) staff       (20)     9312 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/src/yea_wandb/mock_requests.py
+-rw-r--r--   0 kpt        (501) staff       (20)   105508 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/mock_server.py
+-rw-r--r--   0 kpt        (501) staff       (20)    10623 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/plugin.py
+-rw-r--r--   0 kpt        (501) staff       (20)     4847 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/setup.py
+drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.808331 yea-wandb-0.9.7/src/yea_wandb.egg-info/
+-rw-r--r--   0 kpt        (501) staff       (20)      154 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 kpt        (501) staff       (20)      545 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 kpt        (501) staff       (20)        1 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 kpt        (501) staff       (20)       43 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/entry_points.txt
+-rw-r--r--   0 kpt        (501) staff       (20)        1 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 kpt        (501) staff       (20)       43 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/requires.txt
+-rw-r--r--   0 kpt        (501) staff       (20)       10 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yea-wandb-0.9.6/LICENSE` & `yea-wandb-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/README.md` & `yea-wandb-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/setup.py` & `yea-wandb-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """yea setup."""
 
 from setuptools import setup
 
 
 setup(
     name="yea-wandb",
-    version="0.9.6",
+    version="0.9.7",
     description="Test harness wandb plugin",
     packages=["yea_wandb"],
     install_requires=[
         "Flask",
         "requests",
         "responses",
         "pandas",
```

### Comparing `yea-wandb-0.9.6/src/yea_wandb/artifact_emu.py` & `yea-wandb-0.9.7/src/yea_wandb/artifact_emu.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/backend.py` & `yea-wandb-0.9.7/src/yea_wandb/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,34 +181,38 @@
             stdout=logfile,
             env=env,
             stderr=subprocess.STDOUT,
             bufsize=1,
             close_fds=True,
         )
 
+        headers = {"Content-type": "application/json", "Accept": "application/json"}
+
         def get_ctx():
-            return requests.get(server.base_url + "/ctx").json()
+            return requests.get(server.base_url + "/ctx", headers=headers).json()
 
         def set_ctx(payload):
-            return requests.put(server.base_url + "/ctx", json=payload).json()
+            return requests.put(
+                server.base_url + "/ctx", json=payload, headers=headers
+            ).json()
 
         def reset_ctx():
-            return requests.delete(server.base_url + "/ctx").json()
+            return requests.delete(server.base_url + "/ctx", headers=headers).json()
 
         server.get_ctx = get_ctx
         server.set_ctx = set_ctx
         server.reset_ctx = reset_ctx
 
         server._port = port
         server.base_url = f"http://{mockserver_host}:{server._port}"
         self._server = server
         started = False
         for _ in range(30):
             try:
-                res = requests.get(f"{server.base_url}/ctx", timeout=5)
+                res = requests.get(f"{server.base_url}/ctx", timeout=5, headers=headers)
                 if res.status_code == 200:
                     started = True
                     break
                 print(f"INFO: Attempting to connect but got: {res}")
             except requests.exceptions.RequestException:
                 print(
                     "INFO: Timed out waiting for server to start...",
```

### Comparing `yea-wandb-0.9.6/src/yea_wandb/hook.py` & `yea-wandb-0.9.7/src/yea_wandb/hook.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/mitm.py` & `yea-wandb-0.9.7/src/yea_wandb/mitm.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/mock_requests.py` & `yea-wandb-0.9.7/src/yea_wandb/mock_requests.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/mock_server.py` & `yea-wandb-0.9.7/src/yea_wandb/mock_server.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/plugin.py` & `yea-wandb-0.9.7/src/yea_wandb/plugin.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb/setup.py` & `yea-wandb-0.9.7/src/yea_wandb/setup.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.6/src/yea_wandb.egg-info/SOURCES.txt` & `yea-wandb-0.9.7/src/yea_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

