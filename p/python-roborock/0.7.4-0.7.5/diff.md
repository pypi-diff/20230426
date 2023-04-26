# Comparing `tmp/python_roborock-0.7.4.tar.gz` & `tmp/python_roborock-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.4.tar", max compression
+gzip compressed data, was "python_roborock-0.7.5.tar", max compression
```

## Comparing `python_roborock-0.7.4.tar` & `python_roborock-0.7.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-25 12:34:51.012619 python_roborock-0.7.4/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-25 12:34:51.012619 python_roborock-0.7.4/README.md
--rw-r--r--   0        0        0     1370 2023-04-25 12:34:52.060653 python_roborock-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/__init__.py
--rw-r--r--   0        0        0    19296 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/cloud_api.py
--rw-r--r--   0        0        0     4383 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/exceptions.py
--rw-r--r--   0        0        0     6178 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/roborock_message.py
--rw-r--r--   0        0        0    12103 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/typing.py
--rw-r--r--   0        0        0      754 2023-04-25 12:34:51.012619 python_roborock-0.7.4/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 17:53:40.403433 python_roborock-0.7.5/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-25 17:53:40.403433 python_roborock-0.7.5/README.md
+-rw-r--r--   0        0        0     1370 2023-04-25 17:53:41.199445 python_roborock-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-25 17:53:40.403433 python_roborock-0.7.5/roborock/__init__.py
+-rw-r--r--   0        0        0    19297 2023-04-25 17:53:40.403433 python_roborock-0.7.5/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-25 17:53:40.403433 python_roborock-0.7.5/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-25 17:53:40.403433 python_roborock-0.7.5/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4329 2023-04-25 17:53:40.403433 python_roborock-0.7.5/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9872 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/exceptions.py
+-rw-r--r--   0        0        0     6209 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12043 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/typing.py
+-rw-r--r--   0        0        0      767 2023-04-25 17:53:40.407433 python_roborock-0.7.5/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.5/PKG-INFO
```

### Comparing `python_roborock-0.7.4/LICENSE` & `python_roborock-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/README.md` & `python_roborock-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/pyproject.toml` & `python_roborock-0.7.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.4"
+version = "0.7.5"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.4/roborock/api.py` & `python_roborock-0.7.5/roborock/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Status,
     UserData,
     WashTowelMode,
 )
 from .exceptions import RoborockException, RoborockTimeout, VacuumError
 from .roborock_future import RoborockFuture
 from .roborock_message import RoborockMessage
-from .typing import RoborockCommand, DeviceProp, DockSummary
+from .typing import DeviceProp, DockSummary, RoborockCommand
 from .util import unpack_list
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
 SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
@@ -275,15 +275,15 @@
 
     async def get_prop(self, device_id: str) -> DeviceProp | None:
         [status, dnd_timer, clean_summary, consumable] = await asyncio.gather(
             *[
                 self.get_status(device_id),
                 self.get_dnd_timer(device_id),
                 self.get_clean_summary(device_id),
-                self.get_consumable(device_id)
+                self.get_consumable(device_id),
             ]
         )
         last_clean_record = None
         if clean_summary and clean_summary.records and len(clean_summary.records) > 0:
             last_clean_record = await self.get_clean_record(device_id, clean_summary.records[0])
         dock_summary = None
         if status and status.dock_type is not None and status.dock_type != RoborockDockTypeCode["0"]:
```

### Comparing `python_roborock-0.7.4/roborock/cli.py` & `python_roborock-0.7.5/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/cloud_api.py` & `python_roborock-0.7.5/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/code_mappings.py` & `python_roborock-0.7.5/roborock/code_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,22 +148,15 @@
         38: "water empty",
         39: "waste water tank full",
     },
 )
 
 RoborockDockTypeCode = create_code_enum(
     "RoborockDockTypeCode",
-    {
-        0: "no_dock",
-        1: "unknown",
-        2: "unknown",
-        3: "empty_wash_fill_dock",
-        4: "unknown",
-        5: "auto_empty_dock_pure"
-    },
+    {0: "no_dock", 1: "unknown", 2: "unknown", 3: "empty_wash_fill_dock", 4: "unknown", 5: "auto_empty_dock_pure"},
 )
 
 RoborockDockDustCollectionModeCode = create_code_enum(
     "RoborockDockDustCollectionModeCode",
     {
         0: "smart",
         1: "light",
```

### Comparing `python_roborock-0.7.4/roborock/containers.py` & `python_roborock-0.7.5/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/exceptions.py` & `python_roborock-0.7.5/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/local_api.py` & `python_roborock-0.7.5/roborock/local_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
-from asyncio import Transport
+from asyncio import Transport, BaseTransport
 from typing import Callable, Mapping, Optional
 
 import async_timeout
 
 from .api import QUEUE_TIMEOUT, SPECIAL_COMMANDS, RoborockClient
 from .containers import RoborockLocalDeviceInfo
 from .exceptions import CommandVacuumError, RoborockConnectionException, RoborockException
@@ -136,15 +136,15 @@
         return self.transport and self.transport.is_reading()
 
     async def connect(self):
         try:
             if not self.is_connected():
                 async with async_timeout.timeout(self.timeout):
                     _LOGGER.info(f"Connecting to {self.ip}")
-                    self.transport, _ = await self.loop.create_connection(lambda: self, self.ip, 58867)
+                    self.transport, _ = await self.loop.create_connection(lambda: self, self.ip, 58867)  # type: ignore
         except Exception as e:
             raise RoborockConnectionException(f"Failed connecting to {self.ip}") from e
 
     def disconnect(self):
         if self.transport:
             self.transport.close()
```

### Comparing `python_roborock-0.7.4/roborock/roborock_future.py` & `python_roborock-0.7.5/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/roborock_message.py` & `python_roborock-0.7.5/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.4/roborock/typing.py` & `python_roborock-0.7.5/roborock/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     CleanSummary,
     Consumable,
     DNDTimer,
     DustCollectionMode,
     SmartWashParams,
     Status,
     WashTowelMode,
-    MultiMapsList,
 )
 
 
 class RoborockCommand(str, Enum):
     GET_PROP = "get_prop"
     GET_MAP_V1 = "get_map_v1"
     GET_STATUS = "get_status"
@@ -191,24 +190,23 @@
     RoborockCommand.GET_ROOM_MAPPING: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.NAME_SEGMENT: CommandInfo(prefix=b"\x00\x00\x027"),
     RoborockCommand.SET_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00\x97"),
     RoborockCommand.GET_HOMESEC_CONNECT_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.START_CAMERA_PREVIEW: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_TURN_SERVER: CommandInfo(prefix=b"\x00\x00\x00\x77"),
     RoborockCommand.GET_DEVICE_ICE: CommandInfo(prefix=b"\x00\x00\x00\x77"),
-    # TODO discover prefix for following commands
-    # RoborockCommand.APP_GET_DRYER_SETTING: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.APP_SET_DRYER_SETTING: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.GET_DUST_COLLECTION_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.SET_DUST_COLLECTION_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.GET_SMART_WASH_PARAMS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.SET_SMART_WASH_PARAMS: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.GET_WASH_TOWEL_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.SET_WASH_TOWEL_MODE: CommandInfo(prefix=b'\x00\x00\x00w'),
-    # RoborockCommand.START_WASH_THEN_CHARGE: CommandInfo(prefix=b'\x00\x00\x00w'),
+    RoborockCommand.GET_DUST_COLLECTION_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.APP_GET_DRYER_SETTING: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.APP_SET_DRYER_SETTING: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_DUST_COLLECTION_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_SMART_WASH_PARAMS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_SMART_WASH_PARAMS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_WASH_TOWEL_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.SET_WASH_TOWEL_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.START_WASH_THEN_CHARGE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
 }
 
 
 @dataclass
 class DockSummary:
     dust_collection_mode: Optional[DustCollectionMode] = None
     wash_towel_mode: Optional[WashTowelMode] = None
```

### Comparing `python_roborock-0.7.4/roborock/util.py` & `python_roborock-0.7.5/roborock/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from asyncio import AbstractEventLoop
-from typing import TypeVar
+from typing import Optional, TypeVar
 
 T = TypeVar("T")
 
 
-def unpack_list(value: list[T], size: int) -> list[T | None]:
+def unpack_list(value: list[T], size: int) -> list[Optional[T]]:
     return (value + [None] * size)[:size]
 
 
 def get_running_loop_or_create_one() -> AbstractEventLoop:
     try:
         loop = asyncio.get_event_loop()
     except RuntimeError:
```

### Comparing `python_roborock-0.7.4/PKG-INFO` & `python_roborock-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.4
+Version: 0.7.5
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.4 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.7.5 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

