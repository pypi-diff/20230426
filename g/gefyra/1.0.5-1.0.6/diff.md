# Comparing `tmp/gefyra-1.0.5.tar.gz` & `tmp/gefyra-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.0.5.tar", max compression
+gzip compressed data, was "gefyra-1.0.6.tar", max compression
```

## Comparing `gefyra-1.0.5.tar` & `gefyra-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2151 2023-04-21 14:57:48.029554 gefyra-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/__init__.py
--rw-r--r--   0        0        0    13357 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/__main__.py
--rw-r--r--   0        0        0      169 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/list.py
--rw-r--r--   0        0        0     6218 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/up.py
--rw-r--r--   0        0        0     1078 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     5507 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8850 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     1608 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8959 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6677 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1037 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0      945 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/networking.py
--rw-r--r--   0        0        0     3918 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-04-21 14:57:48.033554 gefyra-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-04-26 14:08:38.703776 gefyra-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/__init__.py
+-rw-r--r--   0        0        0    13357 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/__main__.py
+-rw-r--r--   0        0        0      169 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/list.py
+-rw-r--r--   0        0        0     6142 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/up.py
+-rw-r--r--   0        0        0     1264 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:08:38.703776 gefyra-1.0.6/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     5507 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     1608 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8959 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1037 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0      945 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3918 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-04-26 14:08:38.707776 gefyra-1.0.6/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-04-26 14:08:38.707776 gefyra-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.6/PKG-INFO
```

### Comparing `gefyra-1.0.5/README.md` & `gefyra-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/__main__.py` & `gefyra-1.0.6/gefyra/__main__.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/bridge.py` & `gefyra-1.0.6/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/down.py` & `gefyra-1.0.6/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/list.py` & `gefyra-1.0.6/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/run.py` & `gefyra-1.0.6/gefyra/api/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import sys
 from threading import Thread
 
 from gefyra.configuration import default_configuration, ClientConfiguration
-from .utils import stopwatch, get_workload_type
+from .utils import generate_env_dict_from_strings, stopwatch, get_workload_type
 
 
 logger = logging.getLogger(__name__)
 
 
 def pod_ready_and_healthy(
     config: ClientConfiguration, pod_name: str, namespace: str, container_name: str
@@ -135,26 +135,21 @@
                 env_from, namespace=namespace, config=config
             )
             logger.debug(f"Using ENV from {env_from_pod}/{env_from_container}")
             raw_env = get_env_from_pod_container(
                 config, env_from_pod, namespace, env_from_container
             )
             logger.debug("ENV from pod/container is:\n" + raw_env)
-            env_dict = {
-                k[0]: k[1]
-                for k in [arg.split("=") for arg in raw_env.split("\n")]
-                if len(k) > 1
-            }
+            raw_env_vars = raw_env.split("\n")
+            env_dict = generate_env_dict_from_strings(raw_env_vars)
     except ApiException as e:
         logger.error(f"Cannot copy environment from Pod: {e.reason} ({e.status}).")
         return False
     if env:
-        env_overrides = {
-            k[0]: k[1] for k in [arg.split("=") for arg in env] if len(k) > 1
-        }
+        env_overrides = generate_env_dict_from_strings(env)
         env_dict.update(env_overrides)
 
     #
     # 2. deploy the requested container to Gefyra
     #
     try:
         container = deploy_app_container(
```

### Comparing `gefyra-1.0.5/gefyra/api/status.py` & `gefyra-1.0.6/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/up.py` & `gefyra-1.0.6/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/api/utils.py` & `gefyra-1.0.6/gefyra/api/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import time
+from typing import Iterable
 
 logger = logging.getLogger(__name__)
 
 
 def get_workload_type(workload_type_str: str):
     POD = ["pod", "po", "pods"]
     DEPLOYMENT = ["deploy", "deployment", "deployments"]
@@ -20,14 +21,18 @@
         return "pod"
     elif workload_type_str in DEPLOYMENT:
         return "deployment"
     elif workload_type_str in STATEFULSET:
         return "statefulset"
 
 
+def generate_env_dict_from_strings(env_vars: Iterable[str]) -> dict:
+    return {k[0]: k[1] for k in [arg.split("=", 1) for arg in env_vars] if len(k) > 1}
+
+
 def stopwatch(func):
     def wrapper(*args, **kwargs):
         tic = time.perf_counter()
         result = func(*args, **kwargs)
         toc = time.perf_counter()
         logger.debug(
             f"Operation time for '{func.__name__}(...)' was {(toc - tic)*1000:0.4f}ms"
```

### Comparing `gefyra-1.0.5/gefyra/cluster/manager.py` & `gefyra-1.0.6/gefyra/cluster/manager.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/cluster/resources.py` & `gefyra-1.0.6/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/cluster/utils.py` & `gefyra-1.0.6/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/configuration.py` & `gefyra-1.0.6/gefyra/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.0.5"
+__VERSION__ = "1.0.6"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
```

### Comparing `gefyra-1.0.5/gefyra/local/bridge.py` & `gefyra-1.0.6/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/cargo.py` & `gefyra-1.0.6/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.0.6/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/check.py` & `gefyra-1.0.6/gefyra/local/check.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/minikube.py` & `gefyra-1.0.6/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/networking.py` & `gefyra-1.0.6/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/telemetry.py` & `gefyra-1.0.6/gefyra/local/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/gefyra/local/utils.py` & `gefyra-1.0.6/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.5/pyproject.toml` & `gefyra-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.0.5"
+version = "1.0.6"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.0.5/PKG-INFO` & `gefyra-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.0.5
+Version: 1.0.6
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

