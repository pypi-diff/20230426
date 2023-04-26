# Comparing `tmp/embody_ble-1.1.5.tar.gz` & `tmp/embody_ble-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody_ble-1.1.5.tar", max compression
+gzip compressed data, was "embody_ble-1.1.6.tar", max compression
```

## Comparing `embody_ble-1.1.5.tar` & `embody_ble-1.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-17 13:48:58.718535 embody_ble-1.1.5/LICENSE
--rw-r--r--   0        0        0     4413 2023-03-17 13:48:58.718535 embody_ble-1.1.5/README.md
--rw-r--r--   0        0        0     2134 2023-03-17 13:49:10.562843 embody_ble-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      249 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/__init__.py
--rw-r--r--   0        0        0      226 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/__main__.py
--rw-r--r--   0        0        0     7024 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/cli.py
--rw-r--r--   0        0        0    17796 2023-03-17 13:49:10.562843 embody_ble-1.1.5/src/embodyble/embodyble.py
--rw-r--r--   0        0        0      150 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/exceptions.py
--rw-r--r--   0        0        0     1089 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/listeners.py
--rw-r--r--   0        0        0        0 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/py.typed
--rw-r--r--   0        0        0    24909 2023-03-17 13:48:58.718535 embody_ble-1.1.5/src/embodyble/reporting.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 embody_ble-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-26 06:47:17.657046 embody_ble-1.1.6/LICENSE
+-rw-r--r--   0        0        0     4413 2023-04-26 06:47:17.657046 embody_ble-1.1.6/README.md
+-rw-r--r--   0        0        0     2134 2023-04-26 06:47:31.001087 embody_ble-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/__init__.py
+-rw-r--r--   0        0        0      226 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/__main__.py
+-rw-r--r--   0        0        0     7024 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/cli.py
+-rw-r--r--   0        0        0    17921 2023-04-26 06:47:31.001087 embody_ble-1.1.6/src/embodyble/embodyble.py
+-rw-r--r--   0        0        0      150 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/exceptions.py
+-rw-r--r--   0        0        0     1089 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/listeners.py
+-rw-r--r--   0        0        0        0 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/py.typed
+-rw-r--r--   0        0        0    24909 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/reporting.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 embody_ble-1.1.6/PKG-INFO
```

### Comparing `embody_ble-1.1.5/LICENSE` & `embody_ble-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.5/README.md` & `embody_ble-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.5/pyproject.toml` & `embody_ble-1.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-ble"
-version = "1.1.5"
+version = "1.1.6"
 description = "Communicate with the EmBody device over BLE (bluetooth)"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-ble"
 repository = "https://github.com/aidee-health/embody-ble"
 documentation = "https://github.com/aidee-health/embody-ble"
```

### Comparing `embody_ble-1.1.5/src/embodyble/cli.py` & `embody_ble-1.1.6/src/embodyble/cli.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.5/src/embodyble/embodyble.py` & `embody_ble-1.1.6/src/embodyble/embodyble.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from concurrent.futures import ThreadPoolExecutor
 from threading import Thread
 from typing import Optional
 
 from bleak import BleakClient
 from bleak import BleakGATTCharacteristic
 from bleak import BleakScanner
-from embodycodec import attributes
 from embodycodec import codec
 from embodyserial import embodyserial
+from embodyserial.helpers import EmbodySendHelper
+from packaging import version
 
 from .exceptions import EmbodyBleError
 from .listeners import BleMessageListener
 from .listeners import ConnectionListener
 from .listeners import MessageListener
 from .listeners import ResponseMessageListener
 
@@ -201,25 +202,19 @@
         if self.__reader:
             self.__reader.stop()
 
     @staticmethod
     def __find_name_from_serial_port() -> str:
         """Request serial no from EmBody device."""
         comm = embodyserial.EmbodySerial()
-        response = comm.send(
-            msg=codec.GetAttribute(attributes.SerialNoAttribute.attribute_id), timeout=5
-        )
-        if not response or not isinstance(response, codec.GetAttributeResponse):
-            raise EmbodyBleError(
-                "Unable to find connected EmBody device on any serial port or no response received"
-            )
-        device_name = (
-            "G3_"
-            + response.value.value.to_bytes(8, "big", signed=True).hex()[-4:].upper()
-        )
+        send_helper = EmbodySendHelper(comm)
+        serial_no = send_helper.get_serial_no()
+        firmware_version = version.parse(send_helper.get_firmware_version())
+        prefix = "G3_" if firmware_version < version.parse("5.4.0") else "EmBody_"
+        device_name = prefix + serial_no[-4:].upper()
         comm.shutdown()
         return device_name
 
     def list_available_devices(self, timeout=3) -> list[str]:
         """List available devices filtered by NUS service."""
         return asyncio.run_coroutine_threadsafe(
             self.__list_available_devices(timeout), self.__loop
@@ -228,15 +223,22 @@
     async def __list_available_devices(self, timeout=3) -> list[str]:
         """List available devices filtered by NUS service."""
         scanner = BleakScanner()
         await scanner.start()
         await asyncio.sleep(timeout)
         await scanner.stop()
         devices = scanner.discovered_devices
-        return [d.name for d in devices if d.name and d.name.startswith("G3_")]
+        return [d.name for d in devices if EmbodyBle.is_embody_ble_device(d.name)]
+
+    @staticmethod
+    def is_embody_ble_device(device_name: Optional[str]) -> bool:
+        """Check if the device name is an EmBody device."""
+        return device_name is not None and device_name.lower().startswith(
+            tuple(["g3", "embody"])
+        )
 
     def add_message_listener(self, listener: MessageListener) -> None:
         self.__message_listeners.append(listener)
 
     def add_ble_message_listener(self, listener: BleMessageListener) -> None:
         self.__ble_message_listeners.append(listener)
```

### Comparing `embody_ble-1.1.5/src/embodyble/listeners.py` & `embody_ble-1.1.6/src/embodyble/listeners.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.5/src/embodyble/reporting.py` & `embody_ble-1.1.6/src/embodyble/reporting.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.5/PKG-INFO` & `embody_ble-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embody-ble
-Version: 1.1.5
+Version: 1.1.6
 Summary: Communicate with the EmBody device over BLE (bluetooth)
 Home-page: https://github.com/aidee-health/embody-ble
 License: MIT
 Author: Aidee Health AS
 Author-email: hello@aidee.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

