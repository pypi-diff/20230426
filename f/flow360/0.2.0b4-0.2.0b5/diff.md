# Comparing `tmp/flow360-0.2.0b4.tar.gz` & `tmp/flow360-0.2.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b4.tar", max compression
+gzip compressed data, was "flow360-0.2.0b5.tar", max compression
```

## Comparing `flow360-0.2.0b4.tar` & `flow360-0.2.0b5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    26526 2023-04-19 18:35:50.436583 flow360-0.2.0b4/LICENSE
--rw-r--r--   0        0        0     1427 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2526 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     2944 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1466 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8847 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      222 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/__init__.py
--rw-r--r--   0        0        0    23078 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/constants.py
--rw-r--r--   0        0        0    25502 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    18013 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     7651 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      220 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6160 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     8586 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10172 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2327 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/types.py
--rw-r--r--   0        0        0     1019 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/utils.py
--rw-r--r--   0        0        0     2955 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/validator.py
--rw-r--r--   0        0        0    21592 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2228 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/environment.py
--rw-r--r--   0        0        0      237 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-04-19 18:35:50.440583 flow360-0.2.0b4/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-04-19 18:35:50.444583 flow360-0.2.0b4/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1354 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/exceptions.py
--rw-r--r--   0        0        0     5809 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/solver_version.py
--rw-r--r--   0        0        0     2377 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/user_config.py
--rw-r--r--   0        0        0       38 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-04-19 18:36:07.724608 flow360-0.2.0b4/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-25 14:33:37.416890 flow360-0.2.0b5/LICENSE
+-rw-r--r--   0        0        0     1493 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3029 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1466 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     8847 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      220 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/__init__.py
+-rw-r--r--   0        0        0    24217 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/constants.py
+-rw-r--r--   0        0        0    26899 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    21248 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     8093 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      220 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     5798 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     8584 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10172 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2349 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/types.py
+-rw-r--r--   0        0        0     1019 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/utils.py
+-rw-r--r--   0        0        0     3255 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/validator.py
+-rw-r--r--   0        0        0    21646 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2595 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/environment.py
+-rw-r--r--   0        0        0      237 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-04-25 14:33:37.420890 flow360-0.2.0b5/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-04-25 14:33:37.424890 flow360-0.2.0b5/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-04-25 14:33:37.428890 flow360-0.2.0b5/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1354 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/solver_version.py
+-rw-r--r--   0        0        0     2908 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/user_config.py
+-rw-r--r--   0        0        0       38 2023-04-25 14:33:37.432890 flow360-0.2.0b5/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-04-25 14:33:54.097131 flow360-0.2.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b5/PKG-INFO
```

### Comparing `flow360-0.2.0b4/LICENSE` & `flow360-0.2.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/__init__.py` & `flow360-0.2.0b5/flow360/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     SlipWall,
     SubsonicInflow,
     SubsonicOutflowMach,
     SubsonicOutflowPressure,
     TimeStepping,
     TimeSteppingCFL,
     TurbulenceModelSolver,
+    UnvalidatedFlow360Params,
     WallFunction,
 )
 from .component.meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from .component.surface_mesh import SurfaceMesh
 from .component.surface_mesh import SurfaceMeshList as MySurfaceMeshes
 from .component.volume_mesh import VolumeMesh
 from .component.volume_mesh import VolumeMeshList as MyVolumeMeshes
 from .environment import Env
+from .user_config import UserConfig
 from .version import __version__
 
 
 # pylint: disable=too-few-public-methods,invalid-name
 class turbulence:
     """turbulece models shortcut: eg. flow360.turbulence.SA"""
```

### Comparing `flow360-0.2.0b4/flow360/cli/app.py` & `flow360-0.2.0b5/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/cloud/http_util.py` & `flow360-0.2.0b5/flow360/cloud/http_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 from functools import wraps
 
 import requests
 
 from ..environment import Env
 from ..exceptions import AuthorisationError, WebError, WebNotFoundError
 from ..log import log
-from ..user_config import user_config
+from ..user_config import UserConfig
 from ..version import __version__
 from .security import api_key
 
 
 def api_key_auth(request):
     """
     Set the authentication.
     :param request:
     :return:
     """
     key = api_key()
     if not key:
         raise AuthorisationError(
-            f"API key not found for profile={user_config.profile}, please set it by commandline: flow360 configure."
+            f"API key not found for profile={UserConfig.profile}, please set it by commandline: flow360 configure."
         )
     request.headers["simcloud-api-key"] = key
     request.headers["flow360-python-version"] = __version__
+    if Env.impersonate:
+        request.headers["FLOW360ACCESSUSER"] = Env.impersonate
     return request
 
 
 def http_interceptor(func):
     """
     Intercept the response and raise an exception if the status code is not 200.
     :param func:
```

### Comparing `flow360-0.2.0b4/flow360/cloud/rest_api.py` & `flow360-0.2.0b5/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/cloud/s3_utils.py` & `flow360-0.2.0b5/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/component/case.py` & `flow360-0.2.0b5/flow360/component/case.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 """
 from __future__ import annotations
 
 import json
 from enum import Enum
 from typing import Iterator, List
 
-from pydantic import Field
+import pydantic as pd
 from pylab import show, subplots
 
 from ..cloud.rest_api import RestApi
 from ..cloud.s3_utils import CloudFileNotFoundError, S3TransferType
+from ..exceptions import ValidationError
 from ..log import log
-from .flow360_params.flow360_params import Flow360Params
+from .flow360_params.flow360_params import Flow360Params, UnvalidatedFlow360Params
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
+    Flow360Status,
     ResourceDraft,
     before_submit_only,
     is_object_cloud_resource,
 )
 from .utils import is_valid_uuid
 from .validator import Validator
 
@@ -30,41 +32,51 @@
     """
     Case Base component
     """
 
     _endpoint = "cases"
 
     def copy(
-        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+        self,
+        name: str = None,
+        params: Flow360Params = None,
+        solver_version: str = None,
+        tags: List[str] = None,
     ) -> CaseDraft:
         """
         Alias for retry case
         :param name:
         :param params:
         :param tags:
         :return:
         """
 
-        return self.retry(name, params, tags)
+        return self.retry(name, params, solver_version=solver_version, tags=tags)
 
     # pylint: disable=no-member
     def retry(
-        self, name: str = None, params: Flow360Params = None, tags: List[str] = None
+        self,
+        name: str = None,
+        params: Flow360Params = None,
+        solver_version: str = None,
+        tags: List[str] = None,
     ) -> CaseDraft:
         """
         Retry case
         :param name:
         :param params:
         :param tags:
         :return:
         """
 
         name = name or self.name or self.info.name
         params = params or self.params.copy(deep=True)
-        new_case = Case.create(name, params, other_case=self, tags=tags)
+        new_case = Case.create(
+            name, params, other_case=self, solver_version=solver_version, tags=tags
+        )
         return new_case
 
     def continuation(
         self, name: str = None, params: Flow360Params = None, tags: List[str] = None
     ) -> CaseDraft:
         """
         Alias for fork a case to continue simulation
@@ -94,17 +106,17 @@
 
 
 class CaseMeta(Flow360ResourceBaseModel):
     """
     CaseMeta data component
     """
 
-    id: str = Field(alias="caseId")
-    case_mesh_id: str = Field(alias="caseMeshId")
-    parent_id: str = Field(alias="parentId")
+    id: str = pd.Field(alias="caseId")
+    case_mesh_id: str = pd.Field(alias="caseMeshId")
+    parent_id: str = pd.Field(alias="parentId")
 
     def to_case(self) -> Case:
         """
         returns Case object from case meta info
         """
         return Case(self.id)
 
@@ -152,15 +164,15 @@
         return self._params
 
     @params.setter
     def params(self, value: Flow360Params):
         """
         sets case params (before submit only)
         """
-        if not isinstance(value, Flow360Params):
+        if not isinstance(value, Flow360Params) and not isinstance(value, UnvalidatedFlow360Params):
             raise ValueError("params are not of type Flow360Params.")
         self._params = value
 
     @property
     def name(self) -> str:
         """
         returns case name
@@ -185,15 +197,15 @@
     def volume_mesh_id(self, value):
         """
         sets volume mesh id
         """
         self._volume_mesh_id = value
 
     @before_submit_only
-    def submit(self) -> Case:
+    def submit(self, force_submit: bool = False) -> Case:
         """
         submits case to cloud for running
         """
         assert self.name
         assert self.volume_mesh_id or self.other_case or self.parent_id or self.parent_case
         assert self.params
 
@@ -214,15 +226,20 @@
             parent_id = self.parent_case.id
             volume_mesh_id = self.parent_case.volume_mesh_id
 
         volume_mesh_id = volume_mesh_id or self.other_case.volume_mesh_id
 
         is_valid_uuid(volume_mesh_id)
         is_valid_uuid(parent_id, ignore_none=True)
-        self.validator_api(self.params, volume_mesh_id=volume_mesh_id)
+        self.validator_api(
+            self.params,
+            volume_mesh_id=volume_mesh_id,
+            solver_version=self.solver_version,
+            raise_on_error=(not force_submit),
+        )
 
         data = {
             "name": self.name,
             "meshId": volume_mesh_id,
             "runtimeParams": self.params.to_flow360_json(),
             "tags": self.tags,
             "parentId": parent_id,
@@ -260,19 +277,30 @@
         is_valid_uuid(self.volume_mesh_id, ignore_none=True)
 
         if pre_submit_checks:
             is_object_cloud_resource(self.other_case)
             is_object_cloud_resource(self.parent_case)
 
     @classmethod
-    def validator_api(cls, params: Flow360Params, volume_mesh_id):
+    def validator_api(
+        cls,
+        params: Flow360Params,
+        volume_mesh_id,
+        solver_version: str = None,
+        raise_on_error: bool = True,
+    ):
         """
         validation api: validates case parameters before submitting
         """
-        return Validator.CASE.validate(params, mesh_id=volume_mesh_id)
+        return Validator.CASE.validate(
+            params,
+            mesh_id=volume_mesh_id,
+            solver_version=solver_version,
+            raise_on_error=raise_on_error,
+        )
 
 
 # pylint: disable=too-many-instance-attributes
 class Case(CaseBase, Flow360Resource):
     """
     Case component
     """
@@ -303,15 +331,24 @@
 
     @property
     def params(self) -> Flow360Params:
         """
         returns case params
         """
         if self._params is None:
-            self._params = Flow360Params(**json.loads(self.get(method="runtimeParams")["content"]))
+            raw_params = json.loads(self.get(method="runtimeParams")["content"])
+            try:
+                self._params = Flow360Params(**raw_params)
+            except pd.ValidationError as err:
+                if self.status is Flow360Status.ERROR:
+                    log.error(f"{err}")
+                    self._params = raw_params
+                else:
+                    raise ValidationError(f"{err}") from err
+
         return self._params
 
     @property
     def name(self) -> str:
         """
         returns case name
         """
@@ -426,15 +463,17 @@
         :return:
         """
 
         assert name
         assert volume_mesh_id or other_case or parent_id or parent_case
         assert params
 
-        if not isinstance(params, Flow360Params):
+        if not isinstance(params, Flow360Params) and not isinstance(
+            params, UnvalidatedFlow360Params
+        ):
             raise ValueError("params are not of type Flow360Params.")
 
         new_case = CaseDraft(
             name=name,
             volume_mesh_id=volume_mesh_id,
             params=params.copy(),
             parent_id=parent_id,
```

### Comparing `flow360-0.2.0b4/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b5/flow360/component/flow360_params/flow360_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 from abc import ABC
 from typing import Dict, List, Optional, Union
 
 import pydantic as pd
 from typing_extensions import Literal
 
 from ...exceptions import ConfigError, Flow360NotImplementedError, ValidationError
+from ...log import log
+from ...user_config import UserConfig
 from ..constants import constants
 from ..types import (
     Axis,
     BoundaryVelocityType,
     Coordinate,
     MomentLengthType,
+    NonNegativeFloat,
     Omega,
     PositiveFloat,
     PositiveInt,
     TimeStep,
     Velocity,
 )
 from ..utils import _get_value_or_none, beta_feature
-from .params_base import Flow360BaseModel, Flow360SortableBaseModel, export_to_flow360
+from .params_base import (
+    DeprecatedAlias,
+    Flow360BaseModel,
+    Flow360SortableBaseModel,
+    _self_named_property_validator,
+    export_to_flow360,
+)
 from .solvers import NavierStokesSolver, TurbulenceModelSolver
 
 
 # pylint: disable=invalid-name
 def get_time_non_dim_unit(mesh_unit_length, C_inf, extra_msg=""):
     """
     returns time non-dimensionalisation
@@ -412,17 +421,38 @@
 
 
 class TimeSteppingCFL(Flow360BaseModel):
     """
     CFL for time stepping component
     """
 
+    type: Optional[Literal["ramp", "adaptive"]] = pd.Field()
     initial: Optional[int] = pd.Field()
     final: Optional[int] = pd.Field()
     ramp_steps: Optional[int] = pd.Field(alias="rampSteps")
+    min: Optional[PositiveFloat] = pd.Field()
+    max: Optional[PositiveFloat] = pd.Field()
+    max_relative_change: Optional[PositiveFloat] = pd.Field(alias="maxRelativeChange")
+    convergence_limiting_factor: Optional[PositiveFloat] = pd.Field(
+        alias="convergenceLimitingFactor"
+    )
+    randomizer: Optional[Dict] = pd.Field()
+
+    @classmethod
+    def adaptive(cls):
+        """
+        returns default adaptive CFL settings
+        """
+        return cls(
+            type="adaptive",
+            min=0.1,
+            max=10000,
+            max_relative_change=1,
+            convergence_limiting_factor=0.25,
+        )
 
     @classmethod
     def default_steady(cls):
         """
         returns default steady CFL settings
         """
         return cls(initial=5, final=200, ramp_steps=40)
@@ -444,34 +474,14 @@
     physical_steps: Optional[PositiveInt] = pd.Field(alias="physicalSteps")
     max_pseudo_steps: Optional[PositiveInt] = pd.Field(alias="maxPseudoSteps")
     time_step_size: Optional[
         Union[pd.confloat(gt=0, allow_inf_nan=False), TimeStep, Literal["inf"]]
     ] = pd.Field(alias="timeStepSize", default="inf")
     CFL: Optional[TimeSteppingCFL] = pd.Field()
 
-    # pylint: disable=no-self-argument
-    @pd.root_validator(pre=True)
-    def handle_max_physical_steps(cls, values):
-        """
-        root validator to handle maxPhysicalSteps (deprecated) alias for physical_steps
-        """
-
-        max_physical_steps = values.get("maxPhysicalSteps", None)
-        physical_steps = values.get("physicalSteps", values.get("physical_steps", None))
-
-        if max_physical_steps is not None:
-            if physical_steps is not None:
-                allowed = ["maxPhysicalSteps", "physicalSteps"]
-                raise ValidationError(f"Only one of {allowed} can be used.")
-
-            values["physical_steps"] = max_physical_steps
-            values.pop("maxPhysicalSteps")
-
-        return values
-
     @classmethod
     def default_steady(cls):
         """
         returns default steady settings
         """
         return cls(
             physical_steps=1,
@@ -519,14 +529,18 @@
     @pd.validator("time_step_size", pre=True, always=True)
     def check_time_step_size(cls, value):
         """time step validator"""
         if isinstance(value, tuple):
             return TimeStep(v=value[0], unit=value[1])
         return value
 
+    # pylint: disable=missing-class-docstring,too-few-public-methods
+    class Config(Flow360BaseModel.Config):
+        deprecated_aliases = [DeprecatedAlias(name="physical_steps", deprecated="maxPhysicalSteps")]
+
 
 class _GenericBoundaryWrapper(Flow360BaseModel):
     v: BoundaryType
 
 
 class Boundaries(Flow360SortableBaseModel):
     """:class:`Boundaries` class for setting up Boundaries
@@ -557,22 +571,17 @@
         """Validator for boundary list section
 
         Raises
         ------
         ValidationError
             When boundary is incorrect
         """
-        for key, v in values.items():
-            try:
-                values[key] = _GenericBoundaryWrapper(v=v).v
-            except Exception as exc:
-                raise ValidationError(
-                    f"{v} (type={type(v)}) is not any of supported boundary types."
-                ) from exc
-        return values
+        return _self_named_property_validator(
+            values, _GenericBoundaryWrapper, msg="is not any of supported boundary types."
+        )
 
 
 class Geometry(Flow360BaseModel):
     """
     Geometry component
     """
 
@@ -611,32 +620,35 @@
             unit length in meters
         """
         in_meter = {"m": 1, "cm": 0.01, "mm": 0.001, "inch": 0.0254, "feet": 0.3048}
         return in_meter[unit]
 
     # pylint: disable=missing-class-docstring,too-few-public-methods
     class Config(Flow360BaseModel.Config):
-        exclude_on_flow360_export = {"mesh_unit", "mesh_unit_length"}
+        exclude_on_flow360_export = ["mesh_unit", "mesh_unit_length"]
+        allow_but_remove = ["meshName", "endianness"]
 
 
 class Freestream(Flow360BaseModel):
     """
     Freestream component
     """
 
     Reynolds: Optional[PositiveFloat] = pd.Field()
-    Mach: Optional[PositiveFloat] = pd.Field()
+    Mach: Optional[NonNegativeFloat] = pd.Field()
     MachRef: Optional[PositiveFloat] = pd.Field()
     mu_ref: Optional[PositiveFloat] = pd.Field(alias="muRef")
     temperature: PositiveFloat = pd.Field(alias="Temperature")
     density: Optional[PositiveFloat]
     speed: Optional[Union[Velocity, PositiveFloat]]
     alpha: Optional[float] = pd.Field(alias="alphaAngle")
     beta: Optional[float] = pd.Field(alias="betaAngle", default=0)
-    turbulentViscosityRatio: Optional[PositiveFloat]
+    turbulent_viscosity_ratio: Optional[NonNegativeFloat] = pd.Field(
+        alias="turbulentViscosityRatio"
+    )
 
     @pd.validator("speed", pre=True, always=True)
     def validate_speed(cls, v):
         """speed validator"""
         if isinstance(v, tuple):
             return Velocity(v=v[0], unit=v[1])
         return v
@@ -712,38 +724,43 @@
 
         if return_json:
             return self.json()
         return None
 
     # pylint: disable=missing-class-docstring,too-few-public-methods
     class Config(Flow360BaseModel.Config):
-        exclude_on_flow360_export = {"speed", "density"}
+        exclude_on_flow360_export = ["speed", "density"]
         require_one_of = ["Mach", "speed"]
 
 
 class Flow360Params(Flow360BaseModel):
     """
     Flow360 solver parameters
     """
 
     geometry: Optional[Geometry] = pd.Field()
     boundaries: Optional[Boundaries] = pd.Field()
+    initial_condition: Optional[Dict] = pd.Field(alias="initialCondition")
     time_stepping: Optional[TimeStepping] = pd.Field(alias="timeStepping", default=TimeStepping())
     sliding_interfaces: Optional[List[SlidingInterface]] = pd.Field(alias="slidingInterfaces")
     navier_stokes_solver: Optional[NavierStokesSolver] = pd.Field(alias="navierStokesSolver")
     turbulence_model_solver: Optional[TurbulenceModelSolver] = pd.Field(
         alias="turbulenceModelSolver"
     )
     transition_model_solver: Optional[Dict] = pd.Field(alias="transitionModelSolver")
     freestream: Optional[Freestream] = pd.Field()
-    bet_disks: Optional[List] = pd.Field(alias="betDisks")
-    actuator_disks: Optional[List] = pd.Field(alias="actuatorDisks")
+    bet_disks: Optional[List[Dict]] = pd.Field(alias="BETDisks")
+    actuator_disks: Optional[List[ActuatorDisk]] = pd.Field(alias="actuatorDisks")
+    porous_media: Optional[List[Dict]] = pd.Field(alias="porousMedia")
+    user_defined_dynamics: Optional[List[Dict]] = pd.Field(alias="userDefinedDynamics")
     surface_output: Optional[Dict] = pd.Field(alias="surfaceOutput")
     volume_output: Optional[Dict] = pd.Field(alias="volumeOutput")
     slice_output: Optional[Dict] = pd.Field(alias="sliceOutput")
+    iso_surface_output: Optional[Dict] = pd.Field(alias="isoSurfaceOutput")
+    monitor_output: Optional[Dict] = pd.Field(alias="monitorOutput")
 
     # pylint: disable=invalid-name
     def _get_non_dimensionalisation(self):
         mesh_unit_length, C_inf = None, None
         if self.geometry:
             mesh_unit_length = _get_value_or_none(self.geometry.get_mesh_unit_length)
         if self.freestream:
@@ -784,15 +801,33 @@
     @classmethod
     def default(cls, steady: bool = True, solver_version: str = None) -> Flow360Params:
         """
         return default case settings
         """
         raise Flow360NotImplementedError("Default flow360 params are not yet implemented.")
 
+    # pylint: disable=missing-class-docstring,too-few-public-methods
+    class Config(Flow360BaseModel.Config):
+        allow_but_remove = ["runControl", "testControl"]
+
 
 class Flow360MeshParams(Flow360BaseModel):
     """
     Flow360 mesh parameters
     """
 
     boundaries: MeshBoundary = pd.Field()
     sliding_interfaces: Optional[List[MeshSlidingInterface]] = pd.Field(alias="slidingInterfaces")
+
+
+class UnvalidatedFlow360Params(Flow360BaseModel):
+    def __init__(self, filename: str = None, **kwargs):
+        if UserConfig.do_validation:
+            raise ConfigError(
+                "This is DEV feature. To use it activate by: fl.UserConfig.disable_validation()."
+            )
+        log.warning("This is DEV feature, use it only when you know what you are doing.")
+        super().__init__(filename, **kwargs)
+
+    # pylint: disable=missing-class-docstring,too-few-public-methods
+    class Config(Flow360BaseModel.Config):
+        extra = "allow"
```

### Comparing `flow360-0.2.0b4/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b5/flow360/component/flow360_params/params_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import yaml
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from typing_extensions import Literal
 
 from ...exceptions import ConfigError, FileError, ValidationError
 from ...log import log
-from ..types import TYPE_TAG_STR
+from ..types import COMMENTS, TYPE_TAG_STR
 
 
 def json_dumps(value, *args, **kwargs):
     """custom json dump with sort_keys=True"""
     return json.dumps(value, sort_keys=True, *args, **kwargs)
 
 
@@ -77,22 +77,63 @@
             args[0].Config.will_export = False
             raise
         return value
 
     return wrapper_func
 
 
+def _self_named_property_validator(values: dict, validator: BaseModel, msg: str = "") -> dict:
+    """When model uses custom, user defined property names, for example boundary names.
+
+    Parameters
+    ----------
+    values : dict
+        pydantic root validator values
+    validator : BaseModel
+        pydantic BaseModel with field 'v' for validating entry of this class properites
+    msg : str, optional
+        Additional message to be displayed on error, by default ""
+
+    Returns
+    -------
+    dict
+        values to be passed to next pydantic root validator
+
+    Raises
+    ------
+    ValidationError
+        When validation fails
+    """
+    for key, v in values.items():
+        # allow for comments
+        if key == COMMENTS:
+            continue
+        try:
+            values[key] = validator(v=v).v
+        except Exception as exc:
+            raise ValidationError(f"{v} (type={type(v)}) {msg}") from exc
+    return values
+
+
+class DeprecatedAlias(BaseModel):
+    name: str
+    deprecated: str
+
+
 class Flow360BaseModel(BaseModel):
     """Base pydantic model that all Flow360 components inherit from.
     Defines configuration for handling data structures
     as well as methods for imporing, exporting, and hashing Flow360 objects.
     For more details on pydantic base models, see:
     `Pydantic Models <https://pydantic-docs.helpmanual.io/usage/models/>`_
     """
 
+    # comments is allowed property at every level
+    comments: Optional[Any] = pd.Field()
+
     def __init__(self, filename: str = None, **kwargs):
         if filename:
             obj = self.from_file(filename=filename)
             super().__init__(**obj.dict())
         else:
             super().__init__(**kwargs)
 
@@ -133,26 +174,75 @@
         }
         allow_mutation = True
         copy_on_model_validation = "none"
         underscore_attrs_are_private = True
         exclude_on_flow360_export: Optional[Any] = None
         will_export: Optional[bool] = False
         require_one_of: Optional[List[str]] = []
+        allow_but_remove: Optional[List[str]] = []
+        deprecated_aliases: Optional[List[DeprecatedAlias]] = []
 
     # pylint: disable=no-self-argument
-    @pd.root_validator(pre=True)
+    @pd.root_validator()
     def one_of(cls, values):
         """root validator for require one of"""
         if cls.Config.require_one_of:
             set_values = [key for key, v in values.items() if v is not None]
             intersection = list(set(set_values) & set(cls.Config.require_one_of))
             if len(intersection) == 0:
                 raise ConfigError(f"One of {cls.Config.require_one_of} is required.")
         return values
 
+    # pylint: disable=no-self-argument
+    @pd.root_validator(pre=True)
+    def allow_but_remove(cls, values):
+        """root validator for allow_but_remove, e.g., legacy properties that are no longer in use"""
+        if cls.Config.allow_but_remove:
+            for field in cls.Config.allow_but_remove:
+                values.pop(field, None)
+        return values
+
+    # pylint: disable=no-self-argument
+    @pd.root_validator(pre=True)
+    def handle_depracated_aliases(cls, values):
+        """
+        root validator to handle deprecated aliases
+        """
+        if cls.Config.deprecated_aliases:
+            for deprecated_alias in cls.Config.deprecated_aliases:
+                values = cls._handle_depracated_alias(values, deprecated_alias)
+        return values
+
+    @classmethod
+    def _get_field_alias(cls, field_name: str = None):
+        if field_name is not None:
+            alias = [field.alias for field in cls.__fields__.values() if field.name == field_name]
+            if len(alias) > 0:
+                return alias[0]
+        return None
+
+    @classmethod
+    def _handle_depracated_alias(cls, values, deprecated_alias: DeprecatedAlias = None):
+        deprecated_value = values.get(deprecated_alias.deprecated, None)
+        alias = cls._get_field_alias(field_name=deprecated_alias.name)
+        actual_value = values.get(deprecated_alias.name, values.get(alias, None))
+
+        if deprecated_value is not None:
+            if actual_value is not None and actual_value != deprecated_value:
+                allowed = [deprecated_alias.deprecated, deprecated_alias.name]
+                raise ValidationError(f"Only one of {allowed} can be used.")
+            if actual_value is None:
+                log.warning(
+                    f'"{deprecated_alias.deprecated}" is deprecated. Use "{deprecated_alias.name}" instead.'
+                )
+                values[deprecated_alias.name] = deprecated_value
+            values.pop(deprecated_alias.deprecated)
+
+        return values
+
     def copy(self, update=None, **kwargs) -> Flow360BaseModel:
         """Copy a Flow360BaseModel.  With ``deep=True`` as default."""
         if "deep" in kwargs and kwargs["deep"] is False:
             raise ValueError("Can't do shallow copy of component, set `deep=True` in copy().")
         kwargs.update({"deep": True})
         new_copy = BaseModel.copy(self, update=update, **kwargs)
         return self.validate(new_copy.dict())
```

### Comparing `flow360-0.2.0b4/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b5/flow360/component/flow360_params/solvers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Flow360 solvers parameters
 """
 from __future__ import annotations
 
 from enum import Enum
-from typing import Optional
+from typing import Dict, Optional
 
 import pydantic as pd
 from typing_extensions import Literal
 
 from ..types import NonNegativeInt, PositiveFloat, PositiveInt
-from .params_base import Flow360BaseModel
+from .params_base import DeprecatedAlias, Flow360BaseModel
 
 
 class GenericSolverSettings(Flow360BaseModel):
     """:class:`GenericSolverSettings` class"""
 
     absolute_tolerance: Optional[PositiveFloat] = pd.Field(alias="absoluteTolerance")
     relative_tolerance: Optional[float] = pd.Field(alias="relativeTolerance")
@@ -22,14 +22,19 @@
     update_jacobian_frequency: Optional[PositiveInt] = pd.Field(alias="updateJacobianFrequency")
     equation_eval_frequency: Optional[PositiveInt] = pd.Field(alias="equationEvalFrequency")
     max_force_jac_update_physical_steps: Optional[NonNegativeInt] = pd.Field(
         alias="maxForceJacUpdatePhysicalSteps"
     )
     order_of_accuracy: Optional[Literal[1, 2]] = pd.Field(alias="orderOfAccuracy")
     kappaMUSCL: Optional[pd.confloat(ge=-1, le=1)] = pd.Field()
+    randomizer: Optional[Dict] = pd.Field()
+
+    # pylint: disable=missing-class-docstring,too-few-public-methods
+    class Config(Flow360BaseModel.Config):
+        deprecated_aliases = [DeprecatedAlias(name="absolute_tolerance", deprecated="tolerance")]
 
 
 class NavierStokesSolver(GenericSolverSettings):
     """:class:`NavierStokesSolver` class for setting up Navier-Stokes solver
 
     Parameters
     ----------
@@ -82,14 +87,16 @@
     -------
     >>> ns = NavierStokesSolver(absolute_tolerance=1e-10)
     """
 
     CFL_multiplier: Optional[PositiveFloat] = pd.Field(alias="CFLMultiplier")
     limit_velocity: Optional[bool] = pd.Field(alias="limitVelocity")
     limit_pressure_density: Optional[bool] = pd.Field(alias="limitPressureDensity")
+    extra_dissipation: Optional[float] = pd.Field(alias="extraDissipation")
+    viscous_wave_speed_scale: Optional[float] = pd.Field(alias="viscousWaveSpeedScale")
 
 
 class TurbulenceModelModelType(str, Enum):
     """Turbulence model type"""
 
     SA = "SpalartAllmaras"
     SST = "kOmegaSST"
```

### Comparing `flow360-0.2.0b4/flow360/component/meshing/params.py` & `flow360-0.2.0b5/flow360/component/meshing/params.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 Flow360 meshing parameters
 """
 from typing import List, Optional, Union
 
 import pydantic as pd
 from typing_extensions import Literal
 
-from ...exceptions import ValidationError
-from ..flow360_params.params_base import Flow360BaseModel, Flow360SortableBaseModel
+from ..flow360_params.params_base import (
+    Flow360BaseModel,
+    Flow360SortableBaseModel,
+    _self_named_property_validator,
+)
 from ..types import Axis, Coordinate, NonNegativeFloat, PositiveFloat, Size
 
 
 class Aniso(Flow360BaseModel):
     """Aniso edge"""
 
     type = pd.Field("aniso", const=True)
@@ -65,22 +68,17 @@
         """Validator for edge list section
 
         Raises
         ------
         ValidationError
             When edge is incorrect
         """
-        for key, val in values.items():
-            try:
-                values[key] = _GenericEdgeWrapper(v=val).v
-            except Exception as exc:
-                raise ValidationError(
-                    f"{val} (type={type(val)}) is not any of supported edge types."
-                ) from exc
-        return values
+        return _self_named_property_validator(
+            values, _GenericEdgeWrapper, msg="is not any of supported edge types."
+        )
 
 
 class Face(Flow360BaseModel):
     """Face"""
 
     max_edge_length: PositiveFloat = pd.Field(alias="maxEdgeLength")
     adapt: Optional[bool] = pd.Field()
@@ -117,22 +115,18 @@
         """Validator for face list section
 
         Raises
         ------
         ValidationError
             When face is incorrect
         """
-        for key, val in values.items():
-            try:
-                values[key] = _GenericFaceWrapper(v=val).v
-            except Exception as exc:
-                raise ValidationError(
-                    f"{val} (type={type(val)}) is not any of supported face types."
-                ) from exc
-        return values
+
+        return _self_named_property_validator(
+            values, _GenericFaceWrapper, msg="is not any of supported face types."
+        )
 
 
 class SurfaceMeshingParams(Flow360BaseModel):
     """
     Flow360 Surface Meshing parameters
     """
```

### Comparing `flow360-0.2.0b4/flow360/component/resource_base.py` & `flow360-0.2.0b5/flow360/component/resource_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import wraps
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field
 
 from ..cloud.rest_api import RestApi
 from ..log import log
-from ..user_config import user_config
+from ..user_config import UserConfig
 
 
 class Flow360Status(Enum):
     """
     Flow360Status component
     """
 
@@ -118,15 +118,15 @@
 
     def __init__(self):
         # remove from traceback:
         # 1. This line (self.traceback)
         # 2. Call of this init
         self.traceback = traceback.format_stack()[:-2]
 
-        if not user_config.suppress_submit_warning():
+        if not UserConfig.suppress_submit_warning():
             log.warning(
                 f"""\
 Remeber to submit your {self.__class__.__name__} to cloud to have it processed.
 Please run .submit() after .create()
 To suppress this message run: flow360 configure --suppress-submit-warning"""
             )
             for line in self.traceback:
```

### Comparing `flow360-0.2.0b4/flow360/component/surface_mesh.py` & `flow360-0.2.0b5/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/component/types.py` & `flow360-0.2.0b5/flow360/component/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pydantic as pd
 from typing_extensions import Annotated, Literal
 
 from ..exceptions import ValidationError
 
 # type tag default name
 TYPE_TAG_STR = "_type"
+COMMENTS = "comments"
 
 
 def annotate_type(UnionType):  # pylint:disable=invalid-name
     """Annotated union type using TYPE_TAG_STR as discriminator."""
     return Annotated[UnionType, pd.Field(discriminator=TYPE_TAG_STR)]
```

### Comparing `flow360-0.2.0b4/flow360/component/utils.py` & `flow360-0.2.0b5/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/component/validator.py` & `flow360-0.2.0b5/flow360/component/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 from typing import Union
 
 from ..cloud.rest_api import RestApi
 from ..exceptions import ValidationError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
-from .flow360_params.flow360_params import Flow360Params
+from .flow360_params.flow360_params import Flow360Params, UnvalidatedFlow360Params
 from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 
 
 class Validator(Enum):
     """ ":class: Validator"""
 
     VOLUME_MESH = "VolumeMesh"
@@ -31,14 +31,15 @@
 
     # pylint: disable=anomalous-backslash-in-string
     def validate(
         self,
         params: Union[Flow360Params, SurfaceMeshingParams, VolumeMeshingParams],
         solver_version: str = None,
         mesh_id=None,
+        raise_on_error: bool = True,
     ):
         """API validator
 
         Parameters
         ----------
         params : Union[Flow360Params, SurfaceMeshingParams]
             flow360 parameters to validate
@@ -59,14 +60,15 @@
         ValidationError
             when validation API fails
         """
         if (
             not isinstance(params, Flow360Params)
             and not isinstance(params, SurfaceMeshingParams)
             and not isinstance(params, VolumeMeshingParams)
+            and not isinstance(params, UnvalidatedFlow360Params)
         ):
             raise FlValueError(
                 f"""
                 params must be instance of [Flow360Params, SurfaceMeshingParams, VolumeMeshingParams,
                 but {params}, type={type(params)} got.
                 """
             )
@@ -89,10 +91,13 @@
 
         if "success" in res and res["success"] is True:
             return res
 
         if "success" in res and res["success"] is False:
             if "validationError" in res and res["validationError"] is not None:
                 res_str = str(res).replace("[", "\[")
-                raise ValidationError(f"Error when validating: {res_str}")
+                if raise_on_error:
+                    raise ValidationError(f"Error when validating: {res_str}")
+                # pylint: disable=pointless-exception-statement
+                ValidationError(f"Error when validating: {res_str}")
 
         return None
```

### Comparing `flow360-0.2.0b4/flow360/component/volume_mesh.py` & `flow360-0.2.0b5/flow360/component/volume_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from .meshing.params import VolumeMeshingParams
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
+from .types import COMMENTS
 from .validator import Validator
 
 try:
     import h5py
 
     _H5PY_AVAILABLE = True
 except ImportError:
@@ -69,15 +70,15 @@
     ):
         return params.boundaries.no_slip_walls
 
     if isinstance(params, Flow360Params) and params.boundaries:
         return [
             wall_name
             for wall_name, wall in params.boundaries.dict().items()
-            if _GenericBoundaryWrapper(v=wall).v.type == NoSlipWall().type
+            if wall_name != COMMENTS and _GenericBoundaryWrapper(v=wall).v.type == NoSlipWall().type
         ]
 
     return []
 
 
 def get_boundries_from_sliding_interfaces(params: Union[Flow360Params, Flow360MeshParams]):
     """
```

### Comparing `flow360-0.2.0b4/flow360/environment.py` & `flow360-0.2.0b5/flow360/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Environment Setup
 """
 
 from pydantic import BaseModel
 
-from .user_config import user_config
+from .user_config import UserConfig
 
 
 class EnvironmentConfig(BaseModel):
     """
     Basic Configuration for definition environment.
     """
 
@@ -19,15 +19,15 @@
 
     def active(self):
         """
         Activate the particular environment.
         :return:
         """
         Env.set_current(self)
-        user_config.set_profile(self.apikey_profile)
+        UserConfig.set_profile(self.apikey_profile)
 
     def get_real_url(self, path: str):
         """
         Get the real url for the particular environment.
         :param path:
         :return:
         """
@@ -64,14 +64,15 @@
         Env.current.name == "dev"
     """
 
     def __init__(self):
         """
         Initialize the environment.
         """
+        self._impersonate = None
         self._current = prod
 
     @property
     def current(self):
         """
         Get the current environment.
         :return: EnvironmentConfig
@@ -106,9 +107,25 @@
         """
         Set the current environment.
         :param config:
         :return:
         """
         self._current = config
 
+    @property
+    def impersonate(self):
+        """
+        Get the impersonate environment.
+        :return:
+        """
+        return self._impersonate
+
+    @impersonate.setter
+    def impersonate(self, value):
+        self._impersonate = value
+
+    @impersonate.deleter
+    def impersonate(self):
+        self._impersonate = None
+
 
 Env = Environment()
```

### Comparing `flow360-0.2.0b4/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b5/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b5/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b5/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b5/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/base_test_case.py` & `flow360-0.2.0b5/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b5/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b5/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b5/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b5/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b5/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b5/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b5/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b5/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b5/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/exceptions.py` & `flow360-0.2.0b5/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/log.py` & `flow360-0.2.0b5/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/solver_version.py` & `flow360-0.2.0b5/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b4/flow360/user_config.py` & `flow360-0.2.0b5/flow360/user_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 
 home = os.path.expanduser("~")
 config_file = f"{home}/.flow360/config.toml"
 
 DEFAULT_PROFILE = "default"
 
 
-class UserConfig:
+class BasicUserConfig:
     """
     Basic User Configuration.
     """
 
     def __init__(self):
         self._read_config()
         self.set_profile(DEFAULT_PROFILE)
         self._check_env_profile()
         self._apikey = None
         self._check_env_apikey()
+        self._do_validation = True
 
     def _check_env_profile(self):
         simcloud_profile = os.environ.get("SIMCLOUD_PROFILE", None)
         if simcloud_profile is not None and simcloud_profile != self.profile:
             log.info(f"Found env variable SIMCLOUD_PROFILE={simcloud_profile}")
             self.set_profile(simcloud_profile)
 
@@ -81,9 +82,28 @@
         Returns
         -------
         bool
             whether to suppress submit warnings
         """
         return self.config.get("user", {}).get("config", {}).get("suppress_submit_warning", False)
 
+    @property
+    def do_validation(self):
+        """for handling user side validation (pydantic)
+
+        Returns
+        -------
+        bool
+            whether to do user side validation
+        """
+        return self._do_validation
+
+    def disable_validation(self):
+        """disable user side validation (pydantic)"""
+        self._do_validation = False
+
+    def enable_validation(self):
+        """enable user side validation (pydantic)"""
+        self._do_validation = True
+
 
-user_config = UserConfig()
+UserConfig = BasicUserConfig()
```

### Comparing `flow360-0.2.0b4/pyproject.toml` & `flow360-0.2.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b4"
+version = "v0.2.0b5"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b4/PKG-INFO` & `flow360-0.2.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b4
+Version: 0.2.0b5
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

