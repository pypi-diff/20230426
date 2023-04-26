# Comparing `tmp/pymavlog-0.1.2.tar.gz` & `tmp/pymavlog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.1.2.tar", max compression
+gzip compressed data, was "pymavlog-0.2.0.tar", max compression
```

## Comparing `pymavlog-0.1.2.tar` & `pymavlog-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-26 07:41:51.286790 pymavlog-0.1.2/LICENSE
--rw-r--r--   0        0        0     1657 2023-04-26 07:41:51.286790 pymavlog-0.1.2/README.md
--rw-r--r--   0        0        0      176 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/__init__.py
--rw-r--r--   0        0        0     5976 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-04-26 07:41:51.286790 pymavlog-0.1.2/pymavlog/helpers.py
--rw-r--r--   0        0        0     1072 2023-04-26 07:42:04.966868 pymavlog-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 pymavlog-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-26 16:08:11.867424 pymavlog-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1890 2023-04-26 16:08:11.867424 pymavlog-0.2.0/README.md
+-rw-r--r--   0        0        0      196 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/__init__.py
+-rw-r--r--   0        0        0     8808 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-04-26 16:08:34.587891 pymavlog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 pymavlog-0.2.0/PKG-INFO
```

### Comparing `pymavlog-0.1.2/LICENSE` & `pymavlog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymavlog-0.1.2/README.md` & `pymavlog-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ```bash
 make tests
 ```
 
 ## Usage
 
-The main class of the package is `MavLog`, which parses the log file messages in-memory as NumPy arrays. You can parse a file like:
+Mavlink log files are parsed using `MavLog`, which iterates through the logged messages and saves them in-memory as NumPy arrays. You can parse a file like:
 
 ```python
 from pymavlog import MavLog
 
 
 filepath = "foo/bar.bin"
 mavlog = MavLog("foo/bar.bin")
@@ -74,8 +74,17 @@
 
 and do some calculations, for example calculating the average value:
 
 ```python
 avg_gyr_x = imu_messages["GyrX"].mean()
 ```
 
-More info in the docs (TBD).
+Pymavlog also supports telemetry log files. You can read a tlog file `.tlog` in a similar way as binary log files, like:
+
+```python
+from pymavlog import MavTLog
+
+
+filepath = "foo/bar.tlog"
+tlog = MavTLog("foo/bar.tlog")
+tlog.parse()
+```
```

### Comparing `pymavlog-0.1.2/pymavlog/core.py` & `pymavlog-0.2.0/pymavlog/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 import typing as t
 from datetime import datetime
 
 import numpy as np
 from pymavlink import mavutil
 from pymavlink.DFReader import DFFormat, DFMessage
+from pymavlink.dialects.v20.ardupilotmega import MAVLink_message
 
 from .errors import EmptyLogError, InvalidFormatError
 
 
 class MavLinkMessageSeries(object):
     """
     Class that represents a timeseries of MavLink messages
     """
 
+    MSG_TYPES = {
+        "uint8_t": int,
+        "uint16_t": int,
+        "uint32_t": int,
+        "uint64_t": int,
+        "int8_t": int,
+        "int16_t": int,
+        "int32_t": int,
+        "int64_t": int,
+        "float": float,
+        "char": str,
+    }
+
     def __init__(
         self,
         name: str,
         columns: t.List[str],
         types: t.List[type],
         column_alias: t.Dict[str, str] = {},
         msg_id: int = 1,
@@ -26,25 +40,28 @@
         self.id = msg_id
         self._to_datetime = convert_to_datetime
         self._column_alias = column_alias
 
         if len(columns) != len(types):
             raise InvalidFormatError("columns and types must have the same length")
 
-        self._columns = columns
-        self._types = types
+        self._columns = ["timestamp"]
+        if self._to_datetime:
+            self._types = [datetime]
+        else:
+            self._types = [float]
+
+        self._columns.extend(columns)
+        self._types.extend(types)
         self._fields: t.Dict[str, t.List[datetime | int | float]] = {}
+
         self.__set_series()
 
-    def __set_series(
-        self,
-    ):
-        for idx, c in enumerate(self._columns):
-            if c == "TimeUS":
-                self._types[idx] = datetime
+    def __set_series(self):
+        for c in self._columns:
             self._fields[self._column_alias.get(c, c)] = []
 
     @classmethod
     def from_df_format(
         cls,
         fmt: DFFormat,
         column_alias: t.Dict[str, str] = {},
@@ -56,14 +73,34 @@
             columns=fmt.columns,
             types=fmt.msg_types,
             column_alias=column_alias,
             msg_id=msg_id,
             convert_to_datetime=convert_to_datetime,
         )
 
+    @classmethod
+    def from_message(
+        cls,
+        msg: MAVLink_message,
+        column_alias: t.Dict[str, str] = {},
+        msg_id: int = 1,
+        convert_to_datetime: bool = False,
+    ):
+        msg_types = list(map(lambda x: cls.MSG_TYPES[x], msg.fieldtypes))
+        columns = msg.get_fieldnames()
+        name = msg.msgname
+        return cls(
+            name=name,
+            columns=columns,
+            types=msg_types,
+            column_alias=column_alias,
+            msg_id=msg_id,
+            convert_to_datetime=convert_to_datetime,
+        )
+
     @property
     def fields(self) -> t.Dict[str, np.ndarray]:
         """
         The timeseries fields as a numpy array
         """
         fields_np = {}
         for idx, c in enumerate(self._columns):
@@ -76,52 +113,54 @@
     @property
     def raw_fields(self) -> t.Dict[str, list]:
         """
         The timeseries fields as a python list
         """
         return self._fields
 
-    def append_message(self, message: dict) -> None:
-        msg_type = message["mavpackettype"]
+    def append_message(self, message: DFMessage) -> None:
+        msg_dict = message.to_dict()
+        msg_type = msg_dict["mavpackettype"]
 
         if msg_type != self.name:
             raise ValueError(f"Invalid message type, got {msg_type}, expected {self.name}")
 
-        message.pop("mavpackettype")
+        timestamp = getattr(message, "_timestamp", None)
 
-        for k, v in message.items():
-            if k == "TimeUS" and self._to_datetime:
-                self._fields[self._column_alias.get(k, k)].append(datetime.fromtimestamp(v))
+        msg_dict.pop("mavpackettype")
+
+        if timestamp:
+            if self._to_datetime:
+                self._fields["timestamp"].append(datetime.fromtimestamp(timestamp))
             else:
-                self._fields[self._column_alias.get(k, k)].append(v)
+                self._fields["timestamp"].append(timestamp)
+
+        for k, v in msg_dict.items():
+            self._fields[self._column_alias.get(k, k)].append(v)
 
 
-class MavLog(object):
+class MavLogBase(object):
     def __init__(
         self,
         filepath: str,
         messages_to_ignore: t.List[str] = ["FMT", "FMTU"],
         types: t.List[str] = None,
         to_datetime: bool = False,
         map_columns: t.Dict[str, str] = {},
     ):
         self._messages_ignore = messages_to_ignore
         self._mlog: mavutil.mavserial = mavutil.mavlink_connection(filepath)
 
         self._parsed_data: t.Dict[str, MavLinkMessageSeries] = {}
-        self._start_timestamp = 0
-        self._end_timestamp = 0
         self._msg_count = 0
         self._to_datetime = to_datetime
         self._map_columns = map_columns
         self._start_timestamp = None
         self._end_timestamp = None
 
-        self.__set_parsed_data(types)
-
     @property
     def parsed_data(self) -> t.Dict[str, MavLinkMessageSeries]:
         return self._parsed_data
 
     @property
     def message_count(self) -> int:
         return self._msg_count
@@ -140,31 +179,14 @@
     @property
     def end_timestamp(self) -> t.Union[float, datetime]:
         if self._to_datetime:
             return datetime.fromtimestamp(self._end_timestamp)
         else:
             return self._end_timestamp
 
-    def __set_parsed_data(self, types: t.List[str]):
-        self._types = []
-        for name, msg_id in self._mlog.name_to_id.items():
-            fmt = self._mlog.formats[msg_id]
-
-            msg_not_in_types = (types is not None) and (name not in types)
-            ignore_type = (name in self._messages_ignore) or msg_not_in_types
-            if ignore_type:
-                continue
-
-            self._types.append(fmt.name)
-            self._parsed_data[name] = MavLinkMessageSeries.from_df_format(
-                fmt, self._map_columns, msg_id, self._to_datetime
-            )
-        if not self._types:
-            raise EmptyLogError("The log contains no message types")
-
     def parse(self):
         """
         Parses the log file in-memory
         """
         message: DFMessage
 
         while True:
@@ -174,25 +196,21 @@
                 break
 
             if message.get_type() not in self._types:
                 continue
 
             message: DFMessage
 
-            msg_dict = message.to_dict()
-
-            self._parsed_data[message.get_type()].append_message(msg_dict)
-
-            try:
-                self._end_timestamp = msg_dict["TimeUS"]
-                if self._msg_count == 0 or not self._start_timestamp:
-                    self._start_timestamp = msg_dict["TimeUS"]
-            except KeyError:
-                pass
+            timestamp = getattr(message, "_timestamp", None)
+            if timestamp is not None:
+                self._end_timestamp = timestamp
+            if timestamp is not None and (self._msg_count == 0 or not self._start_timestamp):
+                self._start_timestamp = timestamp
 
+            self._parsed_data[message.get_type()].append_message(message)
             self._msg_count += 1
 
     def get(self, key: str):
         """
         Returns a MavLinkMessageSeries object for the given key
 
         ----
@@ -203,7 +221,87 @@
 
         ----
         Returns
         ----
             MavLinkMessageSeries
         """
         return self._parsed_data.get(key)
+
+
+class MavLog(MavLogBase):
+    """
+    A Mavlink binary log object
+    """
+
+    def __init__(
+        self,
+        filepath: str,
+        messages_to_ignore: t.List[str] = ["FMT", "FMTU"],
+        types: t.List[str] = None,
+        to_datetime: bool = False,
+        map_columns: t.Dict[str, str] = {},
+    ):
+        super().__init__(
+            filepath=filepath,
+            messages_to_ignore=messages_to_ignore,
+            types=types,
+            to_datetime=to_datetime,
+            map_columns=map_columns,
+        )
+
+        self.__set_parsed_data(types)
+
+    def __set_parsed_data(self, types: t.List[str]):
+        self._types = []
+        for name, msg_id in self._mlog.name_to_id.items():
+            fmt = self._mlog.formats[msg_id]
+            msg_not_in_types = (types is not None) and (name not in types)
+            ignore_type = (name in self._messages_ignore) or msg_not_in_types
+            if ignore_type:
+                continue
+
+            self._types.append(fmt.name)
+            self._parsed_data[name] = MavLinkMessageSeries.from_df_format(
+                fmt, self._map_columns, msg_id, self._to_datetime
+            )
+        if not self._types:
+            raise EmptyLogError("The log contains no message types")
+
+
+class MavTLog(MavLogBase):
+    """
+    A MavLink Telemetry log object
+    """
+
+    def __init__(
+        self,
+        filepath: str,
+        messages_to_ignore: t.List[str] = ["HEARTBEAT", "MAV"],
+        types: t.List[str] = None,
+        to_datetime: bool = False,
+        map_columns: t.Dict[str, str] = {},
+    ):
+        super().__init__(
+            filepath=filepath,
+            messages_to_ignore=messages_to_ignore,
+            types=types,
+            to_datetime=to_datetime,
+            map_columns=map_columns,
+        )
+
+        self.__set_parsed_data(types)
+
+    def __set_parsed_data(self, types: t.List[str]):
+        self._types = []
+        for name, msg_id in self._mlog.name_to_id.items():
+            msg = self._mlog.messages.get(name)
+            msg_not_in_types = (types is not None) and (name not in types)
+            ignore_type = (name in self._messages_ignore) or msg_not_in_types
+            if ignore_type:
+                continue
+
+            self._types.append(name)
+            self._parsed_data[name] = MavLinkMessageSeries.from_message(
+                msg, self._map_columns, msg_id, self._to_datetime
+            )
+        if not self._types:
+            raise EmptyLogError("The log contains no message types")
```

### Comparing `pymavlog-0.1.2/pyproject.toml` & `pymavlog-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymavlog"
-version = "0.1.2"
+version = "0.2.0"
 description = "A lightweight python library to parse MavLink log files"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Ricardo Martinez <rik@rmargar.net>"
 ]
 classifiers = [
```

### Comparing `pymavlog-0.1.2/PKG-INFO` & `pymavlog-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.1.2
+Version: 0.2.0
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -79,15 +79,15 @@
 
 ```bash
 make tests
 ```
 
 ## Usage
 
-The main class of the package is `MavLog`, which parses the log file messages in-memory as NumPy arrays. You can parse a file like:
+Mavlink log files are parsed using `MavLog`, which iterates through the logged messages and saves them in-memory as NumPy arrays. You can parse a file like:
 
 ```python
 from pymavlog import MavLog
 
 
 filepath = "foo/bar.bin"
 mavlog = MavLog("foo/bar.bin")
@@ -102,9 +102,18 @@
 
 and do some calculations, for example calculating the average value:
 
 ```python
 avg_gyr_x = imu_messages["GyrX"].mean()
 ```
 
-More info in the docs (TBD).
+Pymavlog also supports telemetry log files. You can read a tlog file `.tlog` in a similar way as binary log files, like:
+
+```python
+from pymavlog import MavTLog
+
+
+filepath = "foo/bar.tlog"
+tlog = MavTLog("foo/bar.tlog")
+tlog.parse()
+```
```

