# Comparing `tmp/dirigera-0.1.3.tar.gz` & `tmp/dirigera-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.3.tar", last modified: Sun Apr 23 09:34:51 2023, max compression
+gzip compressed data, was "dirigera-0.1.4.tar", last modified: Wed Apr 26 20:27:27 2023, max compression
```

## Comparing `dirigera-0.1.3.tar` & `dirigera-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 09:34:39.000000 dirigera-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-23 09:34:51.228526 dirigera-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-23 09:34:39.000000 dirigera-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-23 09:34:39.000000 dirigera-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:34:51.228526 dirigera-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:34:39.000000 dirigera-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.224526 dirigera-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.224526 dirigera-0.1.3/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/devices/light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-23 09:34:39.000000 dirigera-0.1.3/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 09:34:51.000000 dirigera-0.1.3/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:34:51.228526 dirigera-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-23 09:34:39.000000 dirigera-0.1.3/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-23 09:34:39.000000 dirigera-0.1.3/tests/test_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 20:27:18.000000 dirigera-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 20:27:27.418074 dirigera-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-26 20:27:18.000000 dirigera-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-26 20:27:18.000000 dirigera-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:27:27.418074 dirigera-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:27:18.000000 dirigera-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/devices/light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-26 20:27:18.000000 dirigera-0.1.4/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 20:27:27.000000 dirigera-0.1.4/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:27:27.418074 dirigera-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-26 20:27:18.000000 dirigera-0.1.4/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-26 20:27:18.000000 dirigera-0.1.4/tests/test_light.py
```

### Comparing `dirigera-0.1.3/LICENSE` & `dirigera-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.3/PKG-INFO` & `dirigera-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.3
+Version: 0.1.4
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,18 +23,23 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Leggin/dirigera
 Keywords: python,iot,smarthome,hub,lighting,ikea,tradfri,dirigera
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Dirigera Python Client
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
```

### Comparing `dirigera-0.1.3/README.md` & `dirigera-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.3/pyproject.toml` & `dirigera-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,32 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.3"
+version = "0.1.4"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
     "websocket-client >= 1.0.0",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.optional-dependencies]
 dev = ["black", "pytest"]
```

### Comparing `dirigera-0.1.3/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.4/src/dirigera/devices/environment_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Dict
 
 from .device import Device
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 @dataclass
 class EnvironmentSensor(Device):
@@ -14,15 +14,15 @@
     current_pm25: int
     max_measured_pm25: int
     min_measured_pm25: int
     voc_index: int
 
     def refresh(self) -> None:
         data = self.dirigera_client.get(route=f"/devices/{self.device_id}")
-        attributes: dict[str, Any] = data["attributes"]
+        attributes: Dict[str, Any] = data["attributes"]
         self.firmware_version = attributes["firmwareVersion"]
         self.current_temperature = attributes["currentTemperature"]
         self.current_rh = attributes["currentRH"]
         self.current_pm25 = attributes["currentPM25"]
         self.voc_index = attributes["vocIndex"]
         self.room_id = data["room"]["id"]
         self.room_name = data["room"]["name"]
@@ -33,17 +33,17 @@
 
         data = [{"attributes": {"customName": name}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
         self.custom_name = name
 
 
 def dict_to_environment_sensor(
-    data: dict[str, Any], dirigera_client: AbstractSmartHomeHub
+    data: Dict[str, Any], dirigera_client: AbstractSmartHomeHub
 ):
-    attributes: dict[str, Any] = data["attributes"]
+    attributes: Dict[str, Any] = data["attributes"]
     return EnvironmentSensor(
         dirigera_client=dirigera_client,
         device_id=data["id"],
         is_reachable=data["isReachable"],
         custom_name=attributes["customName"],
         firmware_version=attributes.get("firmwareVersion"),
         hardware_version=attributes.get("hardwareVersion"),
```

### Comparing `dirigera-0.1.3/src/dirigera/devices/light.py` & `dirigera-0.1.4/src/dirigera/devices/light.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any
+from typing import Any, Optional, Dict
 
 from .device import Device
 
 from ..hub.abstract_smart_home_hub import AbstractSmartHomeHub
 
 
 class StartupEnum(Enum):
@@ -15,25 +15,25 @@
 
 
 @dataclass
 class Light(Device):
     dirigera_client: AbstractSmartHomeHub
     is_reachable: bool
     is_on: bool
-    startup_on_off: StartupEnum | None
-    light_level: int | None
-    color_temp: int | None
-    color_temp_min: int | None
-    color_temp_max: int | None
-    color_hue: int | None
-    color_saturation: float | None
+    startup_on_off: Optional[StartupEnum]
+    light_level: Optional[int]
+    color_temp: Optional[int]
+    color_temp_min: Optional[int]
+    color_temp_max: Optional[int]
+    color_hue: Optional[int]
+    color_saturation: Optional[float]
 
     def refresh(self) -> None:
         data = self.dirigera_client.get(route=f"/devices/{self.device_id}")
-        attributes: dict[str, Any] = data["attributes"]
+        attributes: Dict[str, Any] = data["attributes"]
         self.device_id = data["id"]
         self.is_reachable = data["isReachable"]
         self.custom_name = attributes["customName"]
         self.is_on = attributes["isOn"]
         self.startup_on_off = attributes.get("startupOnOff")
         self.light_level = attributes.get("lightLevel")
         self.color_temp = attributes.get("colorTemperature")
@@ -115,16 +115,16 @@
         When set to START_TOGGLE, a sequence of power-off -> power-on, will toggle the lamp state
         """
         data = [{"attributes": {"startupOnOff": behaviour}}]
         self.dirigera_client.patch(route=f"/devices/{self.device_id}", data=data)
         self.startup_on_off = behaviour
 
 
-def dict_to_light(data: dict[str, Any], dirigera_client: AbstractSmartHomeHub):
-    attributes: dict[str, Any] = data["attributes"]
+def dict_to_light(data: Dict[str, Any], dirigera_client: AbstractSmartHomeHub):
+    attributes: Dict[str, Any] = data["attributes"]
 
     return Light(
         dirigera_client=dirigera_client,
         device_id=data["id"],
         is_reachable=data["isReachable"],
         custom_name=attributes["customName"],
         is_on=attributes["isOn"],
```

### Comparing `dirigera-0.1.3/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.4/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import abc
-from typing import Any
+from typing import Any, Dict, List
 
 
 class AbstractSmartHomeHub(abc.ABC):
     @abc.abstractmethod
-    def patch(self, route: str, data: dict[str, Any]) -> dict[str, Any]:
+    def patch(self, route: str, data: Dict[str, Any]) -> Dict[str, Any]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def get(self, route: str) -> dict[str, Any]:
+    def get(self, route: str) -> Dict[str, Any]:
         raise NotImplementedError
 
 
 class FakeDirigeraHub(AbstractSmartHomeHub):
     def __init__(self) -> None:
-        self.patch_actions: list = []
-        self.get_actions: list = []
+        self.patch_actions: List = []
+        self.get_actions: List = []
 
-    def patch(self, route: str, data: dict[str, Any]) -> dict[str, Any]:
+    def patch(self, route: str, data: Dict[str, Any]) -> Dict[str, Any]:
         self.patch_actions.append({"route": route, "data": data})
 
-    def get(self, route: str) -> dict[str, Any]:
+    def get(self, route: str) -> Dict[str, Any]:
         self.get_actions.append({"route": route})
```

### Comparing `dirigera-0.1.3/src/dirigera/hub/auth.py` & `dirigera-0.1.4/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.3/src/dirigera/hub/hub.py` & `dirigera-0.1.4/src/dirigera/hub/hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ssl
-from typing import Any
+from typing import Any, Dict, List
 import requests
 import websocket
 from urllib3.exceptions import InsecureRequestWarning
 
 from .abstract_smart_home_hub import AbstractSmartHomeHub
 from ..devices.light import Light, dict_to_light
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
@@ -35,22 +35,22 @@
         self.token = token
 
     def headers(self):
         return {"Authorization": f"Bearer {self.token}"}
 
     def create_event_listener(
         self,
-        on_open: Any | None = None,
-        on_message: Any | None = None,
-        on_error: Any | None = None,
-        on_close: Any | None = None,
-        on_ping: Any | None = None,
-        on_pong: Any | None = None,
-        on_data: Any | None = None,
-        on_cont_message: Any | None = None,
+        on_open: Any = None,
+        on_message: Any = None,
+        on_error: Any = None,
+        on_close: Any = None,
+        on_ping: Any = None,
+        on_pong: Any = None,
+        on_data: Any = None,
+        on_cont_message: Any = None,
     ):
         wsapp = websocket.WebSocketApp(
             self.websocket_base_url,
             header={"Authorization": f"Bearer {self.token}"},
             on_open=on_open,
             on_message=on_message,
             on_error=on_error,
@@ -59,36 +59,36 @@
             on_pong=on_pong,
             on_data=on_data,
             on_cont_message=on_cont_message,
         )
 
         wsapp.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
 
-    def patch(self, route: str, data: dict[str, Any]) -> dict[str, Any]:
+    def patch(self, route: str, data: Dict[str, Any]) -> Dict[str, Any]:
         response = requests.patch(
             f"{self.api_base_url}{route}",
             headers=self.headers(),
             json=data,
             timeout=10,
             verify=False,
         )
         response.raise_for_status()
         return response.text
 
-    def get(self, route: str) -> dict[str, Any]:
+    def get(self, route: str) -> Dict[str, Any]:
         response = requests.get(
             f"{self.api_base_url}{route}",
             headers=self.headers(),
             timeout=10,
             verify=False,
         )
         response.raise_for_status()
         return response.json()
 
-    def get_lights(self) -> list[Light]:
+    def get_lights(self) -> List[Light]:
         """
         Fetches all lights registered in the Hub
         """
         devices = self.get("/devices")
         lights = list(filter(lambda x: x["type"] == "light", devices))
         return [dict_to_light(light, self) for light in lights]
 
@@ -98,15 +98,15 @@
         """
         lights = self.get_lights()
         lights = list(filter(lambda x: x.custom_name == lamp_name, lights))
         if len(lights) == 0:
             raise AssertionError(f"No light found with name {lamp_name}")
         return lights[0]
 
-    def get_environment_sensors(self) -> list[EnvironmentSensor]:
+    def get_environment_sensors(self) -> List[EnvironmentSensor]:
         """
         Fetches all environment sensors registered in the Hub
         """
         devices = self.get("/devices")
         sensors = list(
             filter(lambda x: x["deviceType"] == "environmentSensor", devices)
         )
```

### Comparing `dirigera-0.1.3/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.4/src/dirigera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.3
+Version: 0.1.4
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,18 +23,23 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/Leggin/dirigera
 Keywords: python,iot,smarthome,hub,lighting,ikea,tradfri,dirigera
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Dirigera Python Client
 ![Test](https://github.com/Leggin/dirigera/actions/workflows/tests.yml/badge.svg)
 ![Pypi](https://img.shields.io/pypi/v/dirigera)
```

### Comparing `dirigera-0.1.3/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.4/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.3/tests/test_environment_sensor.py` & `dirigera-0.1.4/tests/test_environment_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Dict
 import pytest
 from src.dirigera.hub.abstract_smart_home_hub import FakeDirigeraHub
 from src.dirigera.devices.environment_sensor import (
     EnvironmentSensor,
     dict_to_environment_sensor,
 )
 
@@ -67,15 +68,15 @@
     fake_sensor.set_name(new_name)
     action = fake_client.patch_actions.pop()
     assert action["route"] == f"/devices/{fake_sensor.device_id}"
     assert action["data"] == [{"attributes": {"customName": new_name}}]
     assert fake_sensor.custom_name == new_name
 
 
-def test_dict_to_sensor(fake_client: FakeDirigeraHub, sensor_dict: dict):
+def test_dict_to_sensor(fake_client: FakeDirigeraHub, sensor_dict: Dict):
     sensor = dict_to_environment_sensor(sensor_dict, fake_client)
     assert sensor.device_id == sensor_dict["id"]
     assert sensor.is_reachable == sensor_dict["isReachable"]
     assert sensor.custom_name == sensor_dict["attributes"]["customName"]
     assert sensor.firmware_version == sensor_dict["attributes"]["firmwareVersion"]
     assert sensor.hardware_version == sensor_dict["attributes"]["hardwareVersion"]
     assert sensor.model == sensor_dict["attributes"]["model"]
```

### Comparing `dirigera-0.1.3/tests/test_light.py` & `dirigera-0.1.4/tests/test_light.py`

 * *Files identical despite different names*

