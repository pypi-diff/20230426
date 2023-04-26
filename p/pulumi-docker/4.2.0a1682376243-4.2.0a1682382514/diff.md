# Comparing `tmp/pulumi_docker-4.2.0a1682376243.tar.gz` & `tmp/pulumi_docker-4.2.0a1682382514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker-4.2.0a1682376243.tar", last modified: Mon Apr 24 22:48:18 2023, max compression
+gzip compressed data, was "pulumi_docker-4.2.0a1682382514.tar", last modified: Tue Apr 25 16:09:25 2023, max compression
```

## Comparing `pulumi_docker-4.2.0a1682376243.tar` & `pulumi_docker-4.2.0a1682382514.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/pulumi_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/pulumi_docker/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/get_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/get_remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:48:18.458650 pulumi_docker-4.2.0a1682376243/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 22:48:18.000000 pulumi_docker-4.2.0a1682376243/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:25.018600 pulumi_docker-4.2.0a1682382514/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 16:09:25.014600 pulumi_docker-4.2.0a1682382514/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:25.014600 pulumi_docker-4.2.0a1682382514/pulumi_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:25.014600 pulumi_docker-4.2.0a1682382514/pulumi_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/get_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/get_remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:09:25.014600 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 16:09:25.000000 pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:09:25.018600 pulumi_docker-4.2.0a1682382514/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 16:09:24.000000 pulumi_docker-4.2.0a1682382514/setup.py
```

### Comparing `pulumi_docker-4.2.0a1682376243/PKG-INFO` & `pulumi_docker-4.2.0a1682382514/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.2.0a1682376243
+Version: 4.2.0a1682382514
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-docker/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-docker/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdocker.svg)](https://www.npmjs.com/package/@pulumi/docker)
 [![Python version](https://badge.fury.io/py/pulumi-docker.svg)](https://pypi.org/project/pulumi-docker)
 [![NuGet version](https://badge.fury.io/nu/pulumi.docker.svg)](https://badge.fury.io/nu/pulumi.docker)
```

### Comparing `pulumi_docker-4.2.0a1682376243/README.md` & `pulumi_docker-4.2.0a1682382514/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/__init__.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/_enums.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/_inputs.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/_utilities.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/config/outputs.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/config/vars.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/container.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/get_logs.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/get_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
              show_stdout: Optional[bool] = None,
              since: Optional[str] = None,
              tail: Optional[str] = None,
              timestamps: Optional[bool] = None,
              until: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsResult:
     """
-    _get_logs_ provides logs from specific container
+    `get_logs` provides logs from specific container
 
 
     :param bool discard_headers: Discard headers that docker appends to each log entry
     :param bool logs_list_string_enabled: If true populate computed value `logs_list_string`
     :param str name: The name of the Docker Container
     """
     __args__ = dict()
@@ -225,15 +225,15 @@
                     show_stdout: Optional[pulumi.Input[Optional[bool]]] = None,
                     since: Optional[pulumi.Input[Optional[str]]] = None,
                     tail: Optional[pulumi.Input[Optional[str]]] = None,
                     timestamps: Optional[pulumi.Input[Optional[bool]]] = None,
                     until: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsResult]:
     """
-    _get_logs_ provides logs from specific container
+    `get_logs` provides logs from specific container
 
 
     :param bool discard_headers: Discard headers that docker appends to each log entry
     :param bool logs_list_string_enabled: If true populate computed value `logs_list_string`
     :param str name: The name of the Docker Container
     """
     ...
```

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/get_network.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/get_plugin.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/get_registry_image.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/get_remote_image.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/get_remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/image.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/secret.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,267 +4,245 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from ._enums import *
+from . import outputs
 from ._inputs import *
 
-__all__ = ['ImageArgs', 'Image']
+__all__ = ['SecretArgs', 'Secret']
 
 @pulumi.input_type
-class ImageArgs:
+class SecretArgs:
     def __init__(__self__, *,
-                 image_name: pulumi.Input[str],
-                 build: Optional[pulumi.Input['DockerBuildArgs']] = None,
-                 registry: Optional[pulumi.Input['RegistryArgs']] = None,
-                 skip_push: Optional[pulumi.Input[bool]] = None):
-        """
-        The set of arguments for constructing a Image resource.
-        :param pulumi.Input[str] image_name: The image name
-        :param pulumi.Input['DockerBuildArgs'] build: The Docker build context
-        :param pulumi.Input['RegistryArgs'] registry: The registry to push the image to
-        :param pulumi.Input[bool] skip_push: A flag to skip a registry push.
-        """
-        pulumi.set(__self__, "image_name", image_name)
-        if build is not None:
-            pulumi.set(__self__, "build", build)
-        if registry is not None:
-            pulumi.set(__self__, "registry", registry)
-        if skip_push is None:
-            skip_push = False
-        if skip_push is not None:
-            pulumi.set(__self__, "skip_push", skip_push)
+                 data: pulumi.Input[str],
+                 labels: Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Secret resource.
+        :param pulumi.Input[str] data: Base64-url-safe-encoded secret data
+        :param pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]] labels: User-defined key/value metadata
+        :param pulumi.Input[str] name: User-defined name of the secret
+        """
+        pulumi.set(__self__, "data", data)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
-    @pulumi.getter(name="imageName")
-    def image_name(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def data(self) -> pulumi.Input[str]:
+        """
+        Base64-url-safe-encoded secret data
+        """
+        return pulumi.get(self, "data")
+
+    @data.setter
+    def data(self, value: pulumi.Input[str]):
+        pulumi.set(self, "data", value)
+
+    @property
+    @pulumi.getter
+    def labels(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]]:
         """
-        The image name
+        User-defined key/value metadata
         """
-        return pulumi.get(self, "image_name")
+        return pulumi.get(self, "labels")
 
-    @image_name.setter
-    def image_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "image_name", value)
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]]):
+        pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
-    def build(self) -> Optional[pulumi.Input['DockerBuildArgs']]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The Docker build context
+        User-defined name of the secret
         """
-        return pulumi.get(self, "build")
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
-    @build.setter
-    def build(self, value: Optional[pulumi.Input['DockerBuildArgs']]):
-        pulumi.set(self, "build", value)
+
+@pulumi.input_type
+class _SecretState:
+    def __init__(__self__, *,
+                 data: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Secret resources.
+        :param pulumi.Input[str] data: Base64-url-safe-encoded secret data
+        :param pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]] labels: User-defined key/value metadata
+        :param pulumi.Input[str] name: User-defined name of the secret
+        """
+        if data is not None:
+            pulumi.set(__self__, "data", data)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def registry(self) -> Optional[pulumi.Input['RegistryArgs']]:
+    def data(self) -> Optional[pulumi.Input[str]]:
         """
-        The registry to push the image to
+        Base64-url-safe-encoded secret data
         """
-        return pulumi.get(self, "registry")
+        return pulumi.get(self, "data")
 
-    @registry.setter
-    def registry(self, value: Optional[pulumi.Input['RegistryArgs']]):
-        pulumi.set(self, "registry", value)
+    @data.setter
+    def data(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "data", value)
 
     @property
-    @pulumi.getter(name="skipPush")
-    def skip_push(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def labels(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]]:
         """
-        A flag to skip a registry push.
+        User-defined key/value metadata
         """
-        return pulumi.get(self, "skip_push")
+        return pulumi.get(self, "labels")
 
-    @skip_push.setter
-    def skip_push(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "skip_push", value)
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SecretLabelArgs']]]]):
+        pulumi.set(self, "labels", value)
 
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        User-defined name of the secret
+        """
+        return pulumi.get(self, "name")
 
-class Image(pulumi.CustomResource):
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+
+class Secret(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 build: Optional[pulumi.Input[pulumi.InputType['DockerBuildArgs']]] = None,
-                 image_name: Optional[pulumi.Input[str]] = None,
-                 registry: Optional[pulumi.Input[pulumi.InputType['RegistryArgs']]] = None,
-                 skip_push: Optional[pulumi.Input[bool]] = None,
+                 data: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretLabelArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Builds a Docker Image and pushes to a Docker registry.
+        ## Import
 
-        ## Example Usage
-        ### A Docker image build
-        ```python
-        import pulumi
-        import pulumi_docker as docker
-
-        demo_image = docker.Image("demo-image",
-            build=docker.DockerBuildArgs(
-                context=".",
-                dockerfile="Dockerfile",
-            ),
-            image_name="username/image:tag1",
-            skip_push=True)
-        pulumi.export("imageName", demo_image.image_name)
-        ```
+        #!/bin/bash Docker secret cannot be imported as the secret data, once set, is never exposed again.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['DockerBuildArgs']] build: The Docker build context
-        :param pulumi.Input[str] image_name: The image name
-        :param pulumi.Input[pulumi.InputType['RegistryArgs']] registry: The registry to push the image to
-        :param pulumi.Input[bool] skip_push: A flag to skip a registry push.
+        :param pulumi.Input[str] data: Base64-url-safe-encoded secret data
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretLabelArgs']]]] labels: User-defined key/value metadata
+        :param pulumi.Input[str] name: User-defined name of the secret
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ImageArgs,
+                 args: SecretArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Builds a Docker Image and pushes to a Docker registry.
+        ## Import
 
-        ## Example Usage
-        ### A Docker image build
-        ```python
-        import pulumi
-        import pulumi_docker as docker
-
-        demo_image = docker.Image("demo-image",
-            build=docker.DockerBuildArgs(
-                context=".",
-                dockerfile="Dockerfile",
-            ),
-            image_name="username/image:tag1",
-            skip_push=True)
-        pulumi.export("imageName", demo_image.image_name)
-        ```
+        #!/bin/bash Docker secret cannot be imported as the secret data, once set, is never exposed again.
 
         :param str resource_name: The name of the resource.
-        :param ImageArgs args: The arguments to use to populate this resource's properties.
+        :param SecretArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ImageArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SecretArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 build: Optional[pulumi.Input[pulumi.InputType['DockerBuildArgs']]] = None,
-                 image_name: Optional[pulumi.Input[str]] = None,
-                 registry: Optional[pulumi.Input[pulumi.InputType['RegistryArgs']]] = None,
-                 skip_push: Optional[pulumi.Input[bool]] = None,
+                 data: Optional[pulumi.Input[str]] = None,
+                 labels: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretLabelArgs']]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ImageArgs.__new__(ImageArgs)
+            __props__ = SecretArgs.__new__(SecretArgs)
 
-            __props__.__dict__["build"] = build
-            if image_name is None and not opts.urn:
-                raise TypeError("Missing required property 'image_name'")
-            __props__.__dict__["image_name"] = image_name
-            __props__.__dict__["registry"] = registry
-            if skip_push is None:
-                skip_push = False
-            __props__.__dict__["skip_push"] = skip_push
-            __props__.__dict__["base_image_name"] = None
-            __props__.__dict__["context"] = None
-            __props__.__dict__["dockerfile"] = None
-            __props__.__dict__["registry_server"] = None
-            __props__.__dict__["repo_digest"] = None
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="docker:image:Image")])
-        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(Image, __self__).__init__(
-            'docker:index/image:Image',
+            if data is None and not opts.urn:
+                raise TypeError("Missing required property 'data'")
+            __props__.__dict__["data"] = None if data is None else pulumi.Output.secret(data)
+            __props__.__dict__["labels"] = labels
+            __props__.__dict__["name"] = name
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["data"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(Secret, __self__).__init__(
+            'docker:index/secret:Secret',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Image':
+            opts: Optional[pulumi.ResourceOptions] = None,
+            data: Optional[pulumi.Input[str]] = None,
+            labels: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretLabelArgs']]]]] = None,
+            name: Optional[pulumi.Input[str]] = None) -> 'Secret':
         """
-        Get an existing Image resource's state with the given name, id, and optional extra
+        Get an existing Secret resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] data: Base64-url-safe-encoded secret data
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SecretLabelArgs']]]] labels: User-defined key/value metadata
+        :param pulumi.Input[str] name: User-defined name of the secret
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = ImageArgs.__new__(ImageArgs)
+        __props__ = _SecretState.__new__(_SecretState)
 
-        __props__.__dict__["base_image_name"] = None
-        __props__.__dict__["context"] = None
-        __props__.__dict__["dockerfile"] = None
-        __props__.__dict__["image_name"] = None
-        __props__.__dict__["registry_server"] = None
-        __props__.__dict__["repo_digest"] = None
-        return Image(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="baseImageName")
-    def base_image_name(self) -> pulumi.Output[str]:
-        """
-        The fully qualified image name that was pushed to the registry.
-        """
-        return pulumi.get(self, "base_image_name")
+        __props__.__dict__["data"] = data
+        __props__.__dict__["labels"] = labels
+        __props__.__dict__["name"] = name
+        return Secret(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def context(self) -> pulumi.Output[str]:
+    def data(self) -> pulumi.Output[str]:
         """
-        The path to the build context to use.
+        Base64-url-safe-encoded secret data
         """
-        return pulumi.get(self, "context")
+        return pulumi.get(self, "data")
 
     @property
     @pulumi.getter
-    def dockerfile(self) -> pulumi.Output[str]:
+    def labels(self) -> pulumi.Output[Optional[Sequence['outputs.SecretLabel']]]:
         """
-        The location of the Dockerfile relative to the docker build context.
+        User-defined key/value metadata
         """
-        return pulumi.get(self, "dockerfile")
+        return pulumi.get(self, "labels")
 
     @property
-    @pulumi.getter(name="imageName")
-    def image_name(self) -> pulumi.Output[str]:
-        """
-        The fully qualified image name
-        """
-        return pulumi.get(self, "image_name")
-
-    @property
-    @pulumi.getter(name="registryServer")
-    def registry_server(self) -> pulumi.Output[str]:
-        """
-        The name of the registry server hosting the image.
-        """
-        return pulumi.get(self, "registry_server")
-
-    @property
-    @pulumi.getter(name="repoDigest")
-    def repo_digest(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        The digest of the manifest pushed to the registry, e.g.: repo[:tag]@<algorithm>:<hash>
+        User-defined name of the secret
         """
-        return pulumi.get(self, "repo_digest")
+        return pulumi.get(self, "name")
```

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/network.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/outputs.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/plugin.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/provider.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/registry_image.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/remote_image.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/service.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/service_config.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/service_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/tag.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker/volume.py` & `pulumi_docker-4.2.0a1682382514/pulumi_docker/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/PKG-INFO` & `pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-docker
-Version: 4.2.0a1682376243
+Version: 4.2.0a1682382514
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-docker/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-docker/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fdocker.svg)](https://www.npmjs.com/package/@pulumi/docker)
 [![Python version](https://badge.fury.io/py/pulumi-docker.svg)](https://pypi.org/project/pulumi-docker)
 [![NuGet version](https://badge.fury.io/nu/pulumi.docker.svg)](https://badge.fury.io/nu/pulumi.docker)
```

### Comparing `pulumi_docker-4.2.0a1682376243/pulumi_docker.egg-info/SOURCES.txt` & `pulumi_docker-4.2.0a1682382514/pulumi_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1682376243/setup.py` & `pulumi_docker-4.2.0a1682382514/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.2.0a1682376243"
-PLUGIN_VERSION = "4.2.0-alpha.1682376243+115510c8"
+VERSION = "4.2.0a1682382514"
+PLUGIN_VERSION = "4.2.0-alpha.1682382514+1079638f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'docker', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "docker Pulumi Package - Development Version"
 
 
 setup(name='pulumi_docker',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for interacting with Docker in Pulumi programs",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

