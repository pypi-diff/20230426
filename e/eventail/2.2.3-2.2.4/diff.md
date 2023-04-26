# Comparing `tmp/eventail-2.2.3.tar.gz` & `tmp/eventail-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventail-2.2.3.tar", last modified: Tue Apr 11 14:54:35 2023, max compression
+gzip compressed data, was "eventail-2.2.4.tar", last modified: Tue Apr 25 14:19:04 2023, max compression
```

## Comparing `eventail-2.2.3.tar` & `eventail-2.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1079 2023-04-11 14:54:35.000000 eventail-2.2.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-04-11 14:54:35.000000 eventail-2.2.3/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-04-11 14:54:35.953250 eventail-2.2.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6154 2023-04-11 14:54:35.000000 eventail-2.2.3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/scripts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4202 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/inspect_queue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5376 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/monitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2108 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/publish_configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3098 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/publish_event.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5297 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/resurrect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-04-11 14:54:35.000000 eventail-2.2.3/scripts/send_command.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-11 14:54:35.953250 eventail-2.2.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1351 2023-04-11 14:54:35.000000 eventail-2.2.3/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.949250 eventail-2.2.3/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/aio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1181 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/aio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23411 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/aio/base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail/async_service/pika/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1242 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44831 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2811 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/async_service/pika/supervisor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3576 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/batch_processor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/gelf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/log_criticity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7806 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/sync_publisher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7622 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail/tmp_store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-11 14:54:35.953250 eventail-2.2.3/src/eventail.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6853 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-11 14:54:35.000000 eventail-2.2.3/src/eventail.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-04-25 14:19:03.000000 eventail-2.2.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-04-25 14:19:03.000000 eventail-2.2.4/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-04-25 14:19:04.365403 eventail-2.2.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6154 2023-04-25 14:19:03.000000 eventail-2.2.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.361403 eventail-2.2.4/scripts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4202 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/inspect_queue.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5358 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/monitor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2108 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/publish_configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/publish_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/resurrect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3447 2023-04-25 14:19:03.000000 eventail-2.2.4/scripts/send_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-25 14:19:04.365403 eventail-2.2.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1351 2023-04-25 14:19:03.000000 eventail-2.2.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.361403 eventail-2.2.4/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1121 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/aio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/aio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23412 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/aio/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail/async_service/pika/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    44831 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2811 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/async_service/pika/supervisor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3576 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/batch_processor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/gelf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/log_criticity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7806 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/sync_publisher.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7622 2023-04-25 14:19:03.000000 eventail-2.2.4/src/eventail/tmp_store.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-25 14:19:04.365403 eventail-2.2.4/src/eventail.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8234 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      820 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-25 14:19:04.000000 eventail-2.2.4/src/eventail.egg-info/top_level.txt
```

### Comparing `eventail-2.2.3/LICENSE` & `eventail-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/PKG-INFO` & `eventail-2.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: eventail
-Version: 2.2.3
-Summary: A base class and utilities for AM service architecture
-Home-page: https://github.com/allo-media/eventail
-Author: Allo-Media
-Author-email: dev@allo-media.fr
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: asyncio
-Provides-Extra: synchronous
-Provides-Extra: test
-License-File: LICENSE
-
 ![CircleCI](https://img.shields.io/circleci/build/github/allo-media/eventail)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eventail)
 ![PyPI - License](https://img.shields.io/pypi/l/eventail)
 
 # A python toolkit to develop services within the Allo-Media event-driven architecture, with debug utilities.
 
 ## Overview
@@ -190,9 +168,7 @@
   --count COUNT         Number of message to resurrect (default is 0 = all).
   --batch_size BATCH_SIZE
                         for more efficiency, if the messages are small, process them in batches of
                         this size (default is 1).
 
 ```
 
-
-
```

### Comparing `eventail-2.2.3/scripts/inspect_queue.py` & `eventail-2.2.4/scripts/inspect_queue.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/scripts/logger.py` & `eventail-2.2.4/scripts/logger.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/scripts/monitor.py` & `eventail-2.2.4/scripts/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,27 +132,27 @@
         description="Monitor selected Events and/or Commands on the given broker"
     )
     parser.add_argument("amqp_url", help="URL of the broker, including credentials")
     parser.add_argument(
         "--events",
         help="Event patterns to subscribe to (default to none)",
         nargs="*",
-        default=["none"],
+        default=[],
     )
     parser.add_argument(
         "--commands",
         help="Command patterns to subscribe to (default to none)",
         nargs="*",
-        default=["none"],
+        default=[],
     )
     parser.add_argument(
         "--configurations",
         help="Configuration patterns to subscribe to (default to none)",
         nargs="*",
-        default=["none"],
+        default=[],
     )
     parser.add_argument(
         "--save", action="store_true", help="save payloads in CBOR format."
     )
     args = parser.parse_args()
     monitor = Monitor(
         args.save,
```

### Comparing `eventail-2.2.3/scripts/publish_configuration.py` & `eventail-2.2.4/scripts/publish_configuration.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/scripts/publish_event.py` & `eventail-2.2.4/scripts/publish_event.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/scripts/resurrect.py` & `eventail-2.2.4/scripts/resurrect.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/scripts/send_command.py` & `eventail-2.2.4/scripts/send_command.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/setup.py` & `eventail-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="eventail",
-    version="2.2.3",
+    version="2.2.4",
     url="https://github.com/allo-media/eventail",
     author="Allo-Media",
     author_email="dev@allo-media.fr",
     description="A base class and utilities for AM service architecture",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `eventail-2.2.3/src/eventail/__init__.py` & `eventail-2.2.4/src/eventail/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/async_service/__init__.py` & `eventail-2.2.4/src/eventail/async_service/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/async_service/aio/__init__.py` & `eventail-2.2.4/src/eventail/async_service/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/async_service/aio/base.py` & `eventail-2.2.4/src/eventail/async_service/aio/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                     routing_key=routing_key,
                     mandatory=mandatory,
                     properties=spec.Basic.Properties(
                         delivery_mode=2,  # make message persistent
                         content_type=self._mime_type,
                         reply_to=reply_to,
                         correlation_id=correlation_id,
-                        headers=headers, # type: ignore
+                        headers=headers,  # type: ignore
                     ),
                 )
             except exceptions.DeliveryError as e:
                 # message was not delivered
                 # if it is returned as unroutable, raise a ValueError
                 if e.message is not None:
                     raise ValueError(404, f"{routing_key} is unroutable")
```

### Comparing `eventail-2.2.3/src/eventail/async_service/pika/__init__.py` & `eventail-2.2.4/src/eventail/async_service/pika/__init__.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/async_service/pika/base.py` & `eventail-2.2.4/src/eventail/async_service/pika/base.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/async_service/pika/supervisor.py` & `eventail-2.2.4/src/eventail/async_service/pika/supervisor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/batch_processor.py` & `eventail-2.2.4/src/eventail/batch_processor.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/gelf.py` & `eventail-2.2.4/src/eventail/gelf.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/log_criticity.py` & `eventail-2.2.4/src/eventail/log_criticity.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/sync_publisher.py` & `eventail-2.2.4/src/eventail/sync_publisher.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail/tmp_store.py` & `eventail-2.2.4/src/eventail/tmp_store.py`

 * *Files identical despite different names*

### Comparing `eventail-2.2.3/src/eventail.egg-info/PKG-INFO` & `eventail-2.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,195 @@
 Metadata-Version: 2.1
 Name: eventail
-Version: 2.2.3
+Version: 2.2.4
 Summary: A base class and utilities for AM service architecture
 Home-page: https://github.com/allo-media/eventail
 Author: Allo-Media
 Author-email: dev@allo-media.fr
 License: MIT
+Description: ![CircleCI](https://img.shields.io/circleci/build/github/allo-media/eventail)
+        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eventail)
+        ![PyPI - License](https://img.shields.io/pypi/l/eventail)
+        
+        # A python toolkit to develop services within the Allo-Media event-driven architecture, with debug utilities.
+        
+        ## Overview
+        
+        The Allo-Media event-driven service architecture is language and framework independent and is described in the following document:
+        
+        *Blog post coming soon…*
+        
+        ### eventail.async_service
+        
+        This package provides base classes for implementating fully asynchronous services conforming to this architecture on RabbitMQ.
+        To develop a service, just inherit one of the class (either `async_service.pika.Service` or `async_service.aio.Service` if you want async/await) and provide a concrete implementation of the abstract methods to code the specific behavior of your service.
+        
+        All the burden of communication, message safety, recovery, availability, load balancing and queue/exchange setup is taken care for you by this base class and RabbitMQ. It also provides a kind of supervisor to ensure automatic reconnection after a network failure.
+        
+        You just need to focus on the service logic you develop and then you can deploy as many instances of your service as you see fit, anywhere on the network, and the load will be automatically load-balanced between them.
+        
+        ### eventail.sync_publisher
+        
+        A kombu based synchronous Endpoint for publishing purposes only (events and logs). This is provided to help you port legacy applications to the EDA.
+        
+        ### Command line utilities
+        
+        This package also provide some debugging command line tools :
+        
+         - a logger that can target specific logs (service & criticity) through topic subscription;
+         - a utility to send events on the bus;
+         - a utility to send a command on the bus, wait for its result and display the outcome;
+         - a utility to monitor events and/or commands;
+         - a utility to inspect queues;
+         - and a utility to resurrect (replay) dead messages.
+        
+        ### Note about dead letters
+        
+        The base code  does not create the dead-letters exchange (DLX) for you, nor the dead-letter queues. It's good practice to do it once and configure the queues with a policy :
+        
+        ```
+        rabbitmqctl set_policy DLX ".*\.events|.*\.commands" '{"dead-letter-exchange":"am-dlx"}' --apply-to queues
+        ```
+        
+        Note that a policy applies to existing **and future** queues as well, so you don't have to reissue those commands each time a new service appears!
+        
+        ## Usage
+        
+        
+        ### API
+        
+        The API documentation is on [ReadTheDocs](https://eventail.readthedocs.io/).
+        
+        
+        ### Utilities
+        
+        Once installed (`pip install -e .`), these commands are in you virtualenv path:
+        
+        ```
+        logger.py --help
+        usage: logger.py [-h] [--filter [FILTER [FILTER ...]]] amqp_url
+        
+        Display selected logs in realtime on the given broker
+        
+        positional arguments:
+          amqp_url              URL of the broker, including credentials
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --filter [FILTER [FILTER ...]]
+                                Log patterns to subscribe to (default to all)
+        ```
+        
+        ```
+        usage: monitor.py [-h] [--events [EVENTS [EVENTS ...]]] [--commands [COMMANDS [COMMANDS ...]]] [--save]
+                          amqp_url
+        
+        Monitor selected Events and/or Commands on the given broker
+        
+        positional arguments:
+          amqp_url              URL of the broker, including credentials
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --events [EVENTS [EVENTS ...]]
+                                Event patterns to subscribe to (default to all)
+          --commands [COMMANDS [COMMANDS ...]]
+                                Command patterns to subscribe to (default to all)
+          --save                save payloads in CBOR format.
+        
+        ```
+        
+        ```
+        publish_event.py --help
+        usage: publish_event.py [-h] amqp_url event payload
+        
+        Publish an Event and its payload on the given broker
+        
+        positional arguments:
+          amqp_url    URL of the broker, including credentials
+          event       Event Name
+          payload     The path to the file containing the payload, in JSON or
+                      CBOR format (from file extension).
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        ```
+        usage: publish_configuration.py [-h] amqp_url event payload
+        
+        Publish a configuration event and its payload on the given broker
+        
+        positional arguments:
+          amqp_url    URL of the broker, including credentials
+          event       Configuration event name
+          payload     The path to the file containing the payload, in JSON or
+                      CBOR format (from file extension).
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        ```
+        send_command.py --help
+        usage: send_command.py [-h] amqp_url command payload
+        
+        Send a service command and its payload on the given broker and waits for its result.
+        
+        positional arguments:
+          amqp_url    URL of the broker, including credentials
+          command     Command in the form service.command
+          payload     The path to the file containing the payload, in JSON or
+                      CBOR format (from file extension).
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        ```
+        inspect_queue.py --help
+        usage: inspect_queue.py [-h] [--count COUNT] [--save] amqp_url queue
+        
+        Dump the content of a queue without consuming it.
+        
+        positional arguments:
+          amqp_url       URL of the broker, including credentials.
+          queue          Name of queue to inspect.
+        
+        optional arguments:
+          -h, --help     show this help message and exit
+          --count COUNT  Number of message to dump (default is 0 = all).
+          --save         save payloads in original format.
+        ```
+        
+        ```
+        resurrect.py --help
+        usage: resurrect.py [-h] [--count COUNT] [--batch_size BATCH_SIZE] amqp_url queue
+        
+        Resend dead letters.
+        
+        positional arguments:
+          amqp_url              URL of the broker, including credentials.
+          queue                 Name of dead-letter queue.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --count COUNT         Number of message to resurrect (default is 0 = all).
+          --batch_size BATCH_SIZE
+                                for more efficiency, if the messages are small, process them in batches of
+                                this size (default is 1).
+        
+        ```
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: synchronous
 Provides-Extra: test
-License-File: LICENSE
-
-![CircleCI](https://img.shields.io/circleci/build/github/allo-media/eventail)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eventail)
-![PyPI - License](https://img.shields.io/pypi/l/eventail)
-
-# A python toolkit to develop services within the Allo-Media event-driven architecture, with debug utilities.
-
-## Overview
-
-The Allo-Media event-driven service architecture is language and framework independent and is described in the following document:
-
-*Blog post coming soon…*
-
-### eventail.async_service
-
-This package provides base classes for implementating fully asynchronous services conforming to this architecture on RabbitMQ.
-To develop a service, just inherit one of the class (either `async_service.pika.Service` or `async_service.aio.Service` if you want async/await) and provide a concrete implementation of the abstract methods to code the specific behavior of your service.
-
-All the burden of communication, message safety, recovery, availability, load balancing and queue/exchange setup is taken care for you by this base class and RabbitMQ. It also provides a kind of supervisor to ensure automatic reconnection after a network failure.
-
-You just need to focus on the service logic you develop and then you can deploy as many instances of your service as you see fit, anywhere on the network, and the load will be automatically load-balanced between them.
-
-### eventail.sync_publisher
-
-A kombu based synchronous Endpoint for publishing purposes only (events and logs). This is provided to help you port legacy applications to the EDA.
-
-### Command line utilities
-
-This package also provide some debugging command line tools :
-
- - a logger that can target specific logs (service & criticity) through topic subscription;
- - a utility to send events on the bus;
- - a utility to send a command on the bus, wait for its result and display the outcome;
- - a utility to monitor events and/or commands;
- - a utility to inspect queues;
- - and a utility to resurrect (replay) dead messages.
-
-### Note about dead letters
-
-The base code  does not create the dead-letters exchange (DLX) for you, nor the dead-letter queues. It's good practice to do it once and configure the queues with a policy :
-
-```
-rabbitmqctl set_policy DLX ".*\.events|.*\.commands" '{"dead-letter-exchange":"am-dlx"}' --apply-to queues
-```
-
-Note that a policy applies to existing **and future** queues as well, so you don't have to reissue those commands each time a new service appears!
-
-## Usage
-
-
-### API
-
-The API documentation is on [ReadTheDocs](https://eventail.readthedocs.io/).
-
-
-### Utilities
-
-Once installed (`pip install -e .`), these commands are in you virtualenv path:
-
-```
-logger.py --help
-usage: logger.py [-h] [--filter [FILTER [FILTER ...]]] amqp_url
-
-Display selected logs in realtime on the given broker
-
-positional arguments:
-  amqp_url              URL of the broker, including credentials
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --filter [FILTER [FILTER ...]]
-                        Log patterns to subscribe to (default to all)
-```
-
-```
-usage: monitor.py [-h] [--events [EVENTS [EVENTS ...]]] [--commands [COMMANDS [COMMANDS ...]]] [--save]
-                  amqp_url
-
-Monitor selected Events and/or Commands on the given broker
-
-positional arguments:
-  amqp_url              URL of the broker, including credentials
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --events [EVENTS [EVENTS ...]]
-                        Event patterns to subscribe to (default to all)
-  --commands [COMMANDS [COMMANDS ...]]
-                        Command patterns to subscribe to (default to all)
-  --save                save payloads in CBOR format.
-
-```
-
-```
-publish_event.py --help
-usage: publish_event.py [-h] amqp_url event payload
-
-Publish an Event and its payload on the given broker
-
-positional arguments:
-  amqp_url    URL of the broker, including credentials
-  event       Event Name
-  payload     The path to the file containing the payload, in JSON or
-              CBOR format (from file extension).
-
-optional arguments:
-  -h, --help  show this help message and exit
-```
-
-```
-usage: publish_configuration.py [-h] amqp_url event payload
-
-Publish a configuration event and its payload on the given broker
-
-positional arguments:
-  amqp_url    URL of the broker, including credentials
-  event       Configuration event name
-  payload     The path to the file containing the payload, in JSON or
-              CBOR format (from file extension).
-
-optional arguments:
-  -h, --help  show this help message and exit
-```
-
-```
-send_command.py --help
-usage: send_command.py [-h] amqp_url command payload
-
-Send a service command and its payload on the given broker and waits for its result.
-
-positional arguments:
-  amqp_url    URL of the broker, including credentials
-  command     Command in the form service.command
-  payload     The path to the file containing the payload, in JSON or
-              CBOR format (from file extension).
-
-optional arguments:
-  -h, --help  show this help message and exit
-```
-
-```
-inspect_queue.py --help
-usage: inspect_queue.py [-h] [--count COUNT] [--save] amqp_url queue
-
-Dump the content of a queue without consuming it.
-
-positional arguments:
-  amqp_url       URL of the broker, including credentials.
-  queue          Name of queue to inspect.
-
-optional arguments:
-  -h, --help     show this help message and exit
-  --count COUNT  Number of message to dump (default is 0 = all).
-  --save         save payloads in original format.
-```
-
-```
-resurrect.py --help
-usage: resurrect.py [-h] [--count COUNT] [--batch_size BATCH_SIZE] amqp_url queue
-
-Resend dead letters.
-
-positional arguments:
-  amqp_url              URL of the broker, including credentials.
-  queue                 Name of dead-letter queue.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --count COUNT         Number of message to resurrect (default is 0 = all).
-  --batch_size BATCH_SIZE
-                        for more efficiency, if the messages are small, process them in batches of
-                        this size (default is 1).
-
-```
-
-
-
```

### Comparing `eventail-2.2.3/src/eventail.egg-info/SOURCES.txt` & `eventail-2.2.4/src/eventail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

