# Comparing `tmp/whitson_tool_helper-0.0.6.tar.gz` & `tmp/whitson_tool_helper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.0.6.tar", last modified: Tue Apr 25 15:33:19 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.0.7.tar", last modified: Tue Apr 25 15:46:13 2023, max compression
```

## Comparing `whitson_tool_helper-0.0.6.tar` & `whitson_tool_helper-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      561 2023-04-25 15:33:10.000000 whitson_tool_helper-0.0.6/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/src/whitson_tool_helper/
--rw-rw-r--   0 markus    (1000) markus    (1000)      148 2023-04-25 15:24:46.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/__init__.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/
--rw-rw-r--   0 markus    (1000) markus    (1000)      126 2023-04-25 15:33:02.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2882 2023-04-25 14:55:41.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/consumer.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     1445 2023-04-25 14:55:41.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/producer.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/timeout.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      198 2023-04-25 14:55:41.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper/whitson_exceptions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:33:19.272898 whitson_tool_helper-0.0.6/src/whitson_tool_helper.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-04-25 15:33:19.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      448 2023-04-25 15:33:19.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-25 15:33:19.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-04-25 15:33:19.000000 whitson_tool_helper-0.0.6/src/whitson_tool_helper.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      561 2023-04-25 15:46:04.000000 whitson_tool_helper-0.0.7/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/src/whitson_tool_helper/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      148 2023-04-25 15:24:46.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/__init__.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      126 2023-04-25 15:33:02.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2891 2023-04-25 15:45:29.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/consumer.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1445 2023-04-25 14:55:41.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/producer.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/timeout.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      198 2023-04-25 14:55:41.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper/whitson_exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-25 15:46:13.036944 whitson_tool_helper-0.0.7/src/whitson_tool_helper.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-04-25 15:46:13.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      448 2023-04-25 15:46:13.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-25 15:46:13.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-04-25 15:46:13.000000 whitson_tool_helper-0.0.7/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.0.6/pyproject.toml` & `whitson_tool_helper-0.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 requires-python = ">=3.11"
```

### Comparing `whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/consumer.py` & `whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import concurrent.futures.thread
 from google.cloud import pubsub_v1 as pubsub
 import google.api_core.exceptions
 from google.cloud.pubsub_v1.subscriber.message import Message
 import logging
 import json
 import traceback
 
@@ -57,15 +56,16 @@
                 except Exception as e:
                     logger.error(e)
                     logger.error(traceback.format_exc())
                     logger.warning(f"ACKING UNPROCESSED MESSAGE: {msg.message_id}")
                 else:
                     logger.info(f"ACKING MESSAGE: {msg.message_id}")
                 self.subscriber.acknowledge(
-                    self.subscription_path, [received_message.ack_id]
+                    subscription=self.subscription_path,
+                    ack_ids=[received_message.ack_id],
                 )
 
     def process_msg(self, msg: Message):
         try:
             logger.debug(f"Received PubSub message (id: {msg.message_id})")
             data = json.loads(msg.data.decode("utf8")) if self.decode_json else msg
             logger.debug(data)
```

### Comparing `whitson_tool_helper-0.0.6/src/whitson_tool_helper/pubsub/producer.py` & `whitson_tool_helper-0.0.7/src/whitson_tool_helper/pubsub/producer.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.0.6/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.0.7/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

