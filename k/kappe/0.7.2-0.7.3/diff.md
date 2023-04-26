# Comparing `tmp/kappe-0.7.2.tar.gz` & `tmp/kappe-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappe-0.7.2.tar", last modified: Sun Mar 26 10:24:46 2023, max compression
+gzip compressed data, was "kappe-0.7.3.tar", last modified: Wed Apr 26 09:47:42 2023, max compression
```

## Comparing `kappe-0.7.2.tar` & `kappe-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.450689 kappe-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 10:24:37.000000 kappe-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-26 10:24:46.450689 kappe-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-26 10:24:37.000000 kappe-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-26 10:24:37.000000 kappe-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 10:24:46.450689 kappe-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.446689 kappe-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.446689 kappe-0.7.2/src/kappe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/kappe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.450689 kappe-0.7.2/src/kappe/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/module/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/module/qos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/module/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/module/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.450689 kappe-0.7.2/src/kappe/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.450689 kappe-0.7.2/src/kappe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/utils/msg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/utils/pointcloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-26 10:24:37.000000 kappe-0.7.2/src/kappe/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 10:24:46.450689 kappe-0.7.2/src/kappe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 10:24:46.000000 kappe-0.7.2/src/kappe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.110287 kappe-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 09:47:29.000000 kappe-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-26 09:47:42.110287 kappe-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-26 09:47:29.000000 kappe-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-26 09:47:29.000000 kappe-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:47:42.110287 kappe-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.098287 kappe-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.102287 kappe-0.7.3/src/kappe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/kappe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/module/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.110287 kappe-0.7.3/src/kappe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/msg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 09:47:29.000000 kappe-0.7.3/src/kappe/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:47:42.106287 kappe-0.7.3/src/kappe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 09:47:42.000000 kappe-0.7.3/src/kappe.egg-info/top_level.txt
```

### Comparing `kappe-0.7.2/pyproject.toml` & `kappe-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/convert.py` & `kappe-0.7.3/src/kappe/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from kappe import __version__
 from kappe.module.pointcloud import point_cloud
 from kappe.module.tf import tf_remove
 from kappe.module.timing import fix_ros1_time, time_offset
 from kappe.plugin import ConverterPlugin, load_plugin
 from kappe.settings import Settings
-from kappe.utils.msg_def import get_msg_def
+from kappe.utils.msg_def import get_message_definition
 from kappe.utils.types import McapROSMessage
 
 logger = logging.getLogger(__name__)
 
 
 def generate_qos(config: dict) -> str:
     qos_default = {
@@ -77,17 +77,15 @@
         self.f_writer = output_path.open('wb')
 
         self.reader = make_reader(self.f_reader)
         self.writer = McapWriter(self.f_writer)
 
         self.mcap_header = self.reader.get_header()
         if self.mcap_header.profile == Profile.ROS1 and self.config.msg_folder is None:
-            logger.error("""msg_folder is required for ROS1 mcap!
-You can get common message definitions from:
-git clone --depth=1 --branch=humble https://github.com/ros2/common_interfaces.git msgs""")
+            logger.error('msg_folder is required for ROS1 mcap! See README for more information')
 
         summ = self.reader.get_summary()
 
         if summ is None:
             raise ValueError('Unindexed mcap!')
 
         self.summary: Summary = summ
@@ -122,15 +120,15 @@
                 schema_def = self.config.msg_schema.definition[schema_name]
             elif schema.encoding == SchemaEncoding.ROS1 or \
                     schema_name in self.config.msg_schema.mapping:
                 # if schema is not defined in the config, and it is a ROS1 schema or
                 # or scheme name is mapped, try to get the schema definition
                 # from ROS or disk
 
-                new_data = get_msg_def(schema_name, self.config.msg_folder)
+                new_data = get_message_definition(schema_name, self.config.msg_folder)
 
                 if new_data is not None:
                     schema_def = new_data
                 else:
                     logger.warning(
                         'Schema "%s" not found, skipping.', schema.name)
                     continue
@@ -141,15 +139,15 @@
         # Register schemas for converters
         for conv_list in self.plugin_conv.values():
             for conv, _out_topic in conv_list:
                 out_schema = conv.output_schema
                 if out_schema in self.schema_list:
                     continue
 
-                new_data = get_msg_def(out_schema, self.config.msg_folder)
+                new_data = get_message_definition(out_schema, self.config.msg_folder)
 
                 if new_data is None:
                     raise ValueError(
                         f'Converter: Output schema "{out_schema}" not found')
                 self.schema_list[out_schema] = self.writer.register_msgdef(
                     out_schema, new_data)
```

### Comparing `kappe-0.7.2/src/kappe/cut.py` & `kappe-0.7.3/src/kappe/cut.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,17 +120,15 @@
     for schema, channel, message in reader.iter_messages(
         topics=['/tf_static'],
     ):
         tf_static_msgs.append(message.data)
         tf_static_schema = schema
         tf_static_channel = channel
 
-    if tf_static_schema is None:
-        raise ValueError('Could not find /tf_static topic in file')
-    if tf_static_channel is None:
+    if tf_static_schema is None or tf_static_channel is None:
         raise ValueError('Could not find /tf_static topic in file')
 
     return tf_static_schema, tf_static_channel, tf_static_msgs
 
 
 def cutter_split(input_file: Path, output: Path, settings: CutSettings) -> None:
     """Cut a file into multiple files."""
```

### Comparing `kappe-0.7.2/src/kappe/kappe.py` & `kappe-0.7.3/src/kappe/kappe.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/module/pointcloud.py` & `kappe-0.7.3/src/kappe/module/pointcloud.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/module/qos.py` & `kappe-0.7.3/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/module/tf.py` & `kappe-0.7.3/src/kappe/module/tf.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/module/timing.py` & `kappe-0.7.3/src/kappe/module/timing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 from types import SimpleNamespace
 from typing import Any
 
 from mcap_ros1._vendor.genpy.rostime import Duration as ROS1Duration
 from mcap_ros1._vendor.genpy.rostime import Time as ROS1Time
 from pydantic import BaseModel, Extra
 
 from kappe.utils.types import McapROSMessage
 
+logger = logging.getLogger(__name__)
+
 # TODO: move to utils, make more generic
 TimeMsg = type(
     'builtin_interfaces/Time',
     (SimpleNamespace,),
     {
         '__name__': 'builtin_interfaces/Time',
-        '__slots__': ['secs', 'nsecs'],
+        '__slots__': ['sec', 'nanosec'],
     },
 )
 
 
 class SettingTimeOffset(BaseModel, extra=Extra.forbid):
     """
     Time offset settings.
@@ -29,40 +32,62 @@
     """
 
     sec: int = 0
     nanosec: int = 0
     pub_time: bool | None
 
 
-def time_offset(cfg: SettingTimeOffset, msg: McapROSMessage):
-    """Apply time offset to the message."""
+def time_offset_stamp(cfg: SettingTimeOffset, publish_time_ns: int, stamp: TimeMsg):
     pub_time = cfg.pub_time
     off_sec = cfg.sec
     off_nanosec = cfg.nanosec
 
     if pub_time is True:
-        header_sec = msg.publish_time_ns // 1e9
-        header_nanosec = msg.publish_time_ns % int(1e9)
+        header_sec = publish_time_ns // 1e9
+        header_nanosec = publish_time_ns % int(1e9)
     else:
-        header_sec = int(msg.ros_msg.header.stamp.sec)
-        header_nanosec = int(msg.ros_msg.header.stamp.nanosec)
+        header_sec = int(stamp.sec)
+        header_nanosec = int(stamp.nanosec)
 
     header_nanosec += off_nanosec
 
     # handle nanosec under & overflow
     if header_nanosec < 0:
         header_nanosec += int(1e9)
         header_sec -= 1
     elif header_nanosec >= int(1e9):
         header_nanosec -= int(1e9)
         header_sec += 1
 
-    header = msg.ros_msg.header
-    header.stamp.nanosec = header_nanosec
-    header.stamp.sec = header_sec + off_sec
+    stamp.nanosec = header_nanosec
+    stamp.sec = header_sec + off_sec
+
+
+def time_offset_rec(cfg: SettingTimeOffset, publish_time_ns: int, msg: Any):
+    if not hasattr(msg, '__slots__'):
+        return
+
+    for slot in msg.__slots__:
+        attr = getattr(msg, slot)
+
+        if isinstance(attr, list):
+            for i in attr:
+                time_offset_rec(cfg, publish_time_ns, i)
+
+        if 'mcap_ros2._dynamic.Time' in str(type(attr)):
+            time_offset_stamp(cfg, publish_time_ns, attr)
+        else:
+            time_offset_rec(cfg, publish_time_ns, attr)
+
+
+def time_offset(cfg: SettingTimeOffset, msg: McapROSMessage):
+    """Apply time offset to the message."""
+    if not hasattr(msg, '__slots__'):
+        return
+    time_offset_rec(cfg, msg.publish_time_ns, msg.ros_msg)
 
 
 def fix_ros1_time(msg: Any):
     """
     Fix ROS1 time and duration types, recursively inplace.
 
     secs -> sec
@@ -74,13 +99,13 @@
     for slot in msg.__slots__:
         attr = getattr(msg, slot)
 
         if isinstance(attr, list):
             for i in attr:
                 fix_ros1_time(i)
 
-        elif isinstance(attr, (ROS1Time, ROS1Duration)):
+        elif isinstance(attr, ROS1Time | ROS1Duration):
             time = TimeMsg()
-            time.secs = attr.secs
-            time.nsecs = attr.nsecs
+            time.sec = attr.secs
+            time.nanosec = attr.nsecs
 
             setattr(msg, slot, time)
```

### Comparing `kappe-0.7.2/src/kappe/plugin.py` & `kappe-0.7.3/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/plugins/image.py` & `kappe-0.7.3/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/settings.py` & `kappe-0.7.3/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe/utils/msg_def.py` & `kappe-0.7.3/src/kappe/utils/msg_def.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,97 +11,105 @@
     from rosidl_runtime_py.utilities import get_message
 except ImportError:
     logger.debug('rosidl_runtime_py not found')
     get_interface_path = None
     get_message = None
 
 
-def get_msg_def_ros(msg: str) -> str | None:
+def get_msg_def_ros(msg: str) -> tuple[str, list[str]] | None:
     if get_message is None or get_interface_path is None:
         return None
 
-    text = ''
     fields = get_message(msg).get_fields_and_field_types()
 
+    dependencies = []
     for type_name in fields.values():
         # primitive
         if '/' not in type_name:
             continue
 
+        # builtin_interfaces are expected to be known by the parser
         if type_name.startswith('builtin_interfaces/'):
             continue
 
-        ret = get_msg_def_ros(type_name)
-        if ret is None:
-            logger.error('Failed to find definition for %s', type_name)
-            return None
-
-        text += ret
-
-    text += '========================================\n'
-    text += f'MSG: {msg}\n'
-
-    if '/msg/' not in msg:
-        split = msg.split('/')
-        msg = '/'.join([split[0], 'msg', *split[1:]])
+        dependencies.append(type_name)
 
     with Path(get_interface_path(msg)).open(encoding='utf-8') as msg_file:
-        text += msg_file.read()
+        text = msg_file.read()
 
-    return text
+    return text, dependencies
 
 
-def get_msg_def_disk(msg: str, folder: Path) -> str | None:
-    pkg_name = msg.split('/')[0]
-    msg_name = msg.split('/')[-1]
+"""
+    Returns message definition and its dependencies
+"""
+
+
+def get_msg_def_disk(msg_type: str, folder: Path) -> tuple[str, list[str]] | None:
+    pkg_name = msg_type.split('/')[0]
+    msg_name = msg_type.split('/')[-1]
 
     # TODO: make 'msg' optional?
     # TODO: how to handle multiple matches?
     msg_path = list(folder.glob(f'**/{pkg_name}/msg/{msg_name}.msg'))
     if len(msg_path) == 0:
         return None
 
     msg_path = msg_path[0]
 
-    if not msg_path.exists():
-        return None
-
-    text = ''
     with msg_path.open(encoding='utf-8') as msg_file:
         msg_text = msg_file.read()
 
-    text += f'MSG: {msg}\n'
-    text += msg_text
-    text += '\n'
-    text += '=' * 40 + '\n'
-
+    dependencies = []
     msg_def = ros2_parser.parse_message_string(pkg_name, msg_name, msg_text)
     for field in msg_def.fields:
         f_type = field.type
         if field.type.is_primitive_type():
             continue
 
+        # builtin_interfaces are expected to be known by the parser
         if f_type.pkg_name == 'builtin_interfaces':
             continue
 
-        field_text = get_msg_def_disk(f'{f_type.pkg_name}/{f_type.type}', folder)
-        if field_text is None:
-            logger.error(
-                'Failed to find definition for %s/%s',
-                f_type.pkg_name,
-                f_type.type)
-            return None
-        text += field_text
+        dependencies.append(f'{f_type.pkg_name}/{f_type.type}')
+
+    return (msg_text, dependencies)
 
-    return text
 
+def get_msg_def(msg_type: str, folder: Path | None = None) -> tuple[str, list[str]] | None:
+    ret = get_msg_def_ros(msg_type)
+    if ret is None and folder is not None:
+        return get_msg_def_disk(msg_type, folder)
 
-def get_msg_def(msg: str, folder: Path | None = None) -> str | None:
-    new_data = None
+    return ret
 
-    new_data = get_msg_def_ros(msg)
 
-    if new_data is None and folder is not None:
-        # use ./msgs/ to get the message definition
-        return get_msg_def_disk(msg, folder)
+def get_message_definition(msg_type: str, folder: Path | None = None) -> str | None:
+    msg_def = get_msg_def(msg_type, folder)
+    if msg_def is None:
+        return None
+
+    msg_text, dependencies = msg_def
+    added_types = set()
+    while len(dependencies) > 0:
+        for dep in dependencies:
+            if dep in added_types:
+                continue
+
+            msg_def = get_msg_def(dep, folder)
+            if msg_def is None:
+                return None
+
+            dep_text, dep_dep = msg_def
+
+            msg_text += '=' * 40 + '\n'
+            msg_text += f'MSG: {dep}\n'
+            msg_text += dep_text
+            added_types.add(dep)
+            dependencies.extend(dep_dep)
+
+        # remove added types
+        for added in added_types:
+            if added in dependencies:
+                dependencies.remove(added)
 
-    return new_data
+    return msg_text
```

### Comparing `kappe-0.7.2/src/kappe/utils/pointcloud2.py` & `kappe-0.7.3/src/kappe/utils/pointcloud2.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     field_names: list[str] = []
     field_offsets: list[int] = []
     field_datatypes: list[str] = []
     for i, field in enumerate(fields):
         # Datatype as numpy datatype
         datatype = _DATATYPES[field.datatype]
         # Name field
-        name = f'{DUMMY_FIELD_PREFIX}_{i}' if field.name == '' else field.name
+        name = f'{DUMMY_FIELD_PREFIX}_{i}' if not field.name else field.name
         # Handle fields with count > 1 by creating subfields with a suffix consisting
         # of '_' followed by the subfield counter [0 -> (count - 1)]
         assert field.count > 0, "Can't process fields with count = 0."
         for a in range(field.count):
             # Add suffix if we have multiple subfields
             subfield_name = f'{name}_{a}' if field.count > 1 else name
             assert subfield_name not in field_names, 'Duplicate field names are not allowed!'
```

### Comparing `kappe-0.7.2/src/kappe/utils/settings.py` & `kappe-0.7.3/src/kappe/utils/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.7.2/src/kappe.egg-info/SOURCES.txt` & `kappe-0.7.3/src/kappe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

