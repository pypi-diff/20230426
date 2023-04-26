# Comparing `tmp/legion-utils-0.3.0.tar.gz` & `tmp/legion-utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-utils-0.3.0.tar", last modified: Sun Apr 23 03:35:41 2023, max compression
+gzip compressed data, was "legion-utils-0.3.1.tar", last modified: Tue Apr 25 23:43:30 2023, max compression
```

## Comparing `legion-utils-0.3.0.tar` & `legion-utils-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:58.357856 legion-utils-0.3.0/LICENSE
--rw-r--r--   0        0        0     2573 2022-11-16 02:41:58.357856 legion-utils-0.3.0/README.md
--rw-r--r--   0        0        0      671 2022-11-16 02:41:58.357856 legion-utils-0.3.0/legion_utils/__init__.py
--rw-r--r--   0        0        0    12649 2023-04-10 23:53:37.883526 legion-utils-0.3.0/legion_utils/core.py
--rw-r--r--   0        0        0      893 2023-04-23 03:31:02.035016 legion-utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      454 2023-04-17 01:19:20.049718 legion-utils-0.3.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     5565 2023-04-17 01:27:37.589477 legion-utils-0.3.0/tests/integration/test_alert.py
--rw-r--r--   0        0        0     2104 2023-04-17 01:25:04.130604 legion-utils-0.3.0/tests/integration/utils.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    18292 2023-04-17 01:01:57.259012 legion-utils-0.3.0/tests/unit/test_alert_data.py
--rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 legion-utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:58.357856 legion-utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2573 2022-11-16 02:41:58.357856 legion-utils-0.3.1/README.md
+-rw-r--r--   0        0        0      671 2022-11-16 02:41:58.357856 legion-utils-0.3.1/legion_utils/__init__.py
+-rw-r--r--   0        0        0    14781 2023-04-25 23:43:26.225395 legion-utils-0.3.1/legion_utils/core.py
+-rw-r--r--   0        0        0        0 2023-04-25 23:43:26.225395 legion-utils-0.3.1/legion_utils/py.typed
+-rw-r--r--   0        0        0      893 2023-04-25 23:43:26.225395 legion-utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-17 01:19:20.049718 legion-utils-0.3.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     5565 2023-04-17 01:27:37.589477 legion-utils-0.3.1/tests/integration/test_alert.py
+-rw-r--r--   0        0        0     2104 2023-04-17 01:25:04.130604 legion-utils-0.3.1/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:58.357856 legion-utils-0.3.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    20103 2023-04-25 23:43:26.225395 legion-utils-0.3.1/tests/unit/test_alert_data.py
+-rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 legion-utils-0.3.1/PKG-INFO
```

### Comparing `legion-utils-0.3.0/LICENSE` & `legion-utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.0/README.md` & `legion-utils-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.0/legion_utils/__init__.py` & `legion-utils-0.3.1/legion_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.0/legion_utils/core.py` & `legion-utils-0.3.1/legion_utils/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import IntEnum
 from pprint import pformat
 from re import match
+from socket import gethostname
 from typing import Dict, Any, Optional, Union, List
 
 from robotnikmq import Topic, Message, RobotnikConfig
 from typeguard import typechecked
 
 
 @typechecked
@@ -51,37 +52,72 @@
             return Priority.CRITICAL
     if isinstance(candidate, int):
         return Priority(candidate)
     raise ValueError(f'"{candidate}" cannot be mapped to a valid priority')
 
 
 class NotificationMsg:
+    """This is the default message type from which all other types inherit. It
+       has the most basic and essential properties of a Legion message. Most of
+       the properties are Optional because they're not necessary for a message
+       type of "Notification". You probably should not be using this type
+       directly without setting the priorities and TTLs that you want.
+    """
     @typechecked
     def __init__(
         self,
         contents: Dict[str, Any],
         alert_key: Union[str, List[str], None] = None,
         desc: Optional[str] = None,
         ttl: Optional[int] = None,
         priority: Optional[Priority] = None,
     ):
-        self.contents = contents
+        default_contents: Dict[str, Any] = {'msg_src': gethostname()}
+        self.contents = {**default_contents, **contents}
         self.alert_key = (
             "[" + "][".join(alert_key) + "]"
             if isinstance(alert_key, List)
             else alert_key
         )
         self.desc = desc
         self.ttl = ttl
         self.priority = priority or Priority.INFO
 
+    @property
+    def msg_src(self) -> Optional[str]:
+        """Returns the value of the msg_src property, which is typically the
+           hostname of the machine that generated the message, however, this
+           value can be overridden by settings it in the contents dict.
+
+        Returns:
+            Optional[str]: returns the string stored in contents['msg_src'] if
+                           its present in the contents dict or None if its not.
+        """
+        return self.contents.get('msg_src')
+
     @typechecked
     def broadcast(
         self, exchange: str, route: str, config: Optional[RobotnikConfig] = None
     ) -> None:
+        """Broadcasts the message to a given exchange and route, with an
+           optional Robotnik configuration which can be used to broadcast the
+           message to a wholly different set of servers than the one that would
+           normally be used by the RobotnikMQ library.
+
+        Args:
+            exchange (str): The topic exchange to broadcast to. See:
+                            https://www.rabbitmq.com/tutorials/amqp-concepts.html#exchanges
+            route (str): The routing key for the message. See:
+                         https://www.rabbitmq.com/tutorials/tutorial-four-python.html
+            config (Optional[RobotnikConfig], optional): An optional configuration that can be used
+                                                         to publish the message to a completely
+                                                         different set of RabbitMQ servers than what
+                                                         would otherwise be used by RobotnikMQ by
+                                                         default. Defaults to None.
+        """
         broadcast_msg(exchange, route, self, config)
 
 
 @typechecked
 class InfoMsg(NotificationMsg):
     def __init__(self, contents: Dict[str, Any], ttl: Optional[int] = None):
         super().__init__(contents=contents, ttl=ttl, priority=Priority.INFO)
```

### Comparing `legion-utils-0.3.0/pyproject.toml` & `legion-utils-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "legion-utils"
-version = "0.3.0"
+version = "0.3.1"
 description = "Utilities for Legion Reporters and Monitors"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "robotnikmq>=0.7.0",
 ]
```

### Comparing `legion-utils-0.3.0/tests/integration/test_alert.py` & `legion-utils-0.3.1/tests/integration/test_alert.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.0/tests/integration/utils.py` & `legion-utils-0.3.1/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `legion-utils-0.3.0/PKG-INFO` & `legion-utils-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legion-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Utilities for Legion Reporters and Monitors
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >=3.8.3,<4.0
 Description-Content-Type: text/markdown
 
 # Legion Utils
```

