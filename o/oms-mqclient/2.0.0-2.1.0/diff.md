# Comparing `tmp/oms-mqclient-2.0.0.tar.gz` & `tmp/oms-mqclient-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.0.0.tar", last modified: Fri Apr 21 20:01:30 2023, max compression
+gzip compressed data, was "oms-mqclient-2.1.0.tar", last modified: Tue Apr 25 16:27:16 2023, max compression
```

## Comparing `oms-mqclient-2.0.0.tar` & `oms-mqclient-2.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2674 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-21 20:01:28.000000 oms-mqclient-2.0.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5676 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12343 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    12296 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15440 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    16965 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1118 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 20:01:30.000000 oms-mqclient-2.0.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2725 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.660924 oms-mqclient-2.0.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.664924 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    20680 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:01:30.668924 oms-mqclient-2.0.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-04-21 20:01:27.000000 oms-mqclient-2.0.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5808 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12421 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    12342 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15483 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    22378 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    33482 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.0.0/LICENSE` & `oms-mqclient-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/PKG-INFO` & `oms-mqclient-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.0.0/README.md` & `oms-mqclient-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/mqclient/__init__.py` & `oms-mqclient-2.1.0/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.0.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.1.0/mqclient/broker_client_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 TIMEOUT_MILLIS_DEFAULT = 1000  # milliseconds
 RETRY_DELAY = 1  # seconds
 TRY_ATTEMPTS = 3  # ex: 3 means 1 initial try and 2 retries
 
 
 class ConnectingFailedException(Exception):
-    """Raised when a `connect()` invocation fails."""
+    """Raised when a `connect()` fails."""
 
 
 class ClosingFailedException(Exception):
-    """Raised when a `close()` invocation fails."""
+    """Raised when a `close()` fails."""
 
 
 class AlreadyClosedException(ClosingFailedException):
-    """Raised when a `close()` invocation fails on an already closed interface."""
+    """Raised when a `close()` fails on an already closed interface."""
 
 
 class AckException(Exception):
     """Raised when there's a problem with acking."""
 
 
 class NackException(Exception):
@@ -86,15 +86,16 @@
         """Read and return dict from the `headers` field."""
         if not self._headers:
             self._headers = pickle.loads(self.payload)["headers"]
         return self._headers
 
     @staticmethod
     def serialize(data: Any, headers: Optional[Dict[str, Any]] = None) -> bytes:
-        """Return serialized representation of message payload as a bytes object.
+        """Return serialized representation of message payload as a bytes
+        object.
 
         Optionally include `headers` dict for internal information.
         """
         if not headers:
             headers = {}
 
         return pickle.dumps({"headers": headers, "data": data}, protocol=4)
@@ -125,17 +126,23 @@
         """Send a message on a queue."""
         raise NotImplementedError()
 
 
 class Sub(RawQueue):
     """Subscriber queue."""
 
+    @property
+    def prefetch(self) -> int:
+        """Get prefetch."""
+        return self._prefetch  # type: ignore[attr-defined, no-any-return]
+
     @staticmethod
     def _to_message(*args: Any) -> Optional[Message]:
-        """Convert broker_client-specific payload to standardized Message type."""
+        """Convert broker_client-specific payload to standardized Message
+        type."""
         raise NotImplementedError()
 
     async def get_message(
         self, timeout_millis: Optional[int] = TIMEOUT_MILLIS_DEFAULT
     ) -> Optional[Message]:
         """Get a single message from a queue."""
         raise NotImplementedError()
```

### Comparing `oms-mqclient-2.0.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.1.0/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.1.0/mqclient/broker_clients/apachepulsar.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         # https://pulsar.apache.org/assets/images/pulsar-subscription-types-664733b68c7124129ca7d0e04dedcb96.png
         inner_sub = PulsarSub(
             self.address,
             self.topic,
             BrokerClient.SUBSCRIPTION_NAME,
             self._auth_token,
             self.ack_timeout,
+            prefetch=1,
         )
         await inner_sub.connect()
         await inner_sub.close()
 
         self.producer = self.client.create_producer(self.topic)
         LOGGER.debug(log_msgs.CONNECTED_PUB)
 
@@ -143,20 +144,21 @@
     def __init__(
         self,
         address: str,
         topic: str,
         subscription_name: str,
         auth_token: str,
         ack_timeout: Optional[int],
+        prefetch: int,
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({address}; {topic})")
         super().__init__(address, topic, auth_token, ack_timeout)
         self.consumer: pulsar.Consumer = None
         self.subscription_name = subscription_name
-        self.prefetch = 1
+        self._prefetch = prefetch  # see `Sub.prefetch` property
 
     async def connect(self) -> None:
         """Connect to subscriber."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
         self.consumer = self.client.subscribe(
@@ -366,11 +368,11 @@
         """Create a subscription queue."""
         q = PulsarSub(  # pylint: disable=invalid-name
             address,
             name,
             BrokerClient.SUBSCRIPTION_NAME,
             auth_token,
             ack_timeout,
+            prefetch,
         )
-        q.prefetch = prefetch
         await q.connect()
         return q
```

### Comparing `oms-mqclient-2.0.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.1.0/mqclient/broker_clients/nats.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,19 +151,19 @@
     """Wrapper around queue with prefetch-queue, using JetStream.
 
     Extends:
         NATS
         Sub
     """
 
-    def __init__(self, endpoint: str, stream_id: str, subject: str):
+    def __init__(self, endpoint: str, stream_id: str, subject: str, prefetch: int):
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({endpoint}; {stream_id}; {subject})")
         super().__init__(endpoint, stream_id, subject)
         self._subscription: Optional[nats.js.JetStreamContext.PullSubscription] = None
-        self.prefetch = 1
+        self._prefetch = prefetch  # see `Sub.prefetch` property
 
     async def connect(self) -> None:
         """Set up sub (pull subscription)."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
         if not self.js:
             raise RuntimeError("JetStream is not connected.")
@@ -376,11 +376,11 @@
 
         # NOTE - `auth_token` is not used currently
         """
         q = NATSSub(  # pylint: disable=invalid-name
             address,
             name + "-stream",
             name + "-subject",
+            prefetch,
         )
-        q.prefetch = prefetch
         await q.connect()
         return q
```

### Comparing `oms-mqclient-2.0.0/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.1.0/mqclient/broker_clients/rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,19 +200,19 @@
     """Wrapper around queue with prefetch-queue QoS.
 
     Extends:
         RabbitMQ
         Sub
     """
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, prefetch: int, **kwargs: Any) -> None:
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({args}; {kwargs})")
         super().__init__(*args, **kwargs)
         self.consumer_id = None
-        self.prefetch = 1
+        self._prefetch = prefetch  # see `Sub.prefetch` property
 
     async def connect(self) -> None:
         """Set up connection, channel, and queue.
 
         Turn on prefetching.
         """
         LOGGER.debug(log_msgs.CONNECTING_SUB)
@@ -468,11 +468,10 @@
             address (str): address of queue
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         # pylint: disable=invalid-name
-        q = RabbitMQSub(address, name, auth_token, ack_timeout)
-        q.prefetch = prefetch
+        q = RabbitMQSub(address, name, auth_token, ack_timeout, prefetch=prefetch)
         await q.connect()
         return q
```

### Comparing `oms-mqclient-2.0.0/mqclient/log_msgs.py` & `oms-mqclient-2.1.0/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/mqclient/queue.py` & `oms-mqclient-2.1.0/mqclient/queue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """Queue class encapsulating a pub-sub messaging system."""
 
 import contextlib
 import logging
 import sys
 import types
 import uuid
-from typing import Any, AsyncGenerator, AsyncIterator, Dict, Optional, Type
+from typing import (
+    Any,
+    AsyncGenerator,
+    AsyncIterator,
+    Awaitable,
+    Callable,
+    Dict,
+    Optional,
+    Type,
+)
 
 from . import broker_client_manager
 from . import telemetry as wtt
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
 
 LOGGER = logging.getLogger("mqclient")
 
@@ -91,21 +100,21 @@
         return await self._broker_client.create_pub_queue(
             self._address,
             self._name,
             self._auth_token,
             self._ack_timeout,
         )
 
-    async def _create_sub_queue(self) -> Sub:
+    async def _create_sub_queue(self, prefetch_override: Optional[int] = None) -> Sub:
         """Wrap `self._broker_client.create_sub_queue()` with instance's
         config."""
         return await self._broker_client.create_sub_queue(
             self._address,
             self._name,
-            self._prefetch,
+            prefetch_override if prefetch_override else self._prefetch,
             self._auth_token,
             self._ack_timeout,
         )
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
         these=[
@@ -200,21 +209,23 @@
 
     def open_sub(self) -> "QueueSubResource":
         """Open a resource to receive messages from the queue as an iterator.
 
         This returns a context-manager/generator. Its iterator stops when no
         messages are received for `timeout` seconds. If an exception is raised
         (inside the context), the message is rejected, the context is exited,
-        and exception can be re-raised if configured by `except_errors`.
+        and exception is re-raised if configured by `except_errors`. The
+        connection is closed after the context manager exits.
+
         Multiple calls to `open_sub()` is okay, but reusing the returned
         instance is not.
 
         Example:
-            async with queue.open_sub() as stream:
-                async for msg in stream:
+            async with queue.open_sub() as sub:
+                async for msg in sub:
                     print(msg)
 
         Returns:
             QueueSubResource -- context manager and generator object
         """
         LOGGER.debug("Creating new QueueSubResource instance.")
         return QueueSubResource(self)
@@ -225,14 +236,100 @@
             "self._broker_client",
             "self._address",
             "self._name",
             "self._prefetch",
             "self.timeout",
         ]
     )
+    async def open_sub_manual_acking(
+        self,
+        ack_pending_limit: Optional[int] = None,
+    ) -> AsyncGenerator["ManualQueueSubResource", None]:
+        """Open a resource to receive messages from the queue as an iterator.
+
+        This returns a context-manager with an iterator function `iter_messages()`.
+        The iterator stops when no messages are received for `timeout` seconds.
+        Multiple calls to `open_sub()` is okay, but reusing the returned
+        instance is not.
+
+        The connection is closed after the context manager exits.
+
+        *Unlike `open_sub()`*, the caller is responsible for:
+            - All acking and/or nacking
+            - Any error handling
+
+        **NOTE: unless you need to parallelize your message processing,
+        use `open_sub()`**
+
+        Args:
+            ack_pending_limit (int, optional):
+                how many messages are expected to be pending before being
+                acked. If not given, the `self.prefetch` is used. If you
+                surpass this limit, the iterator will raise a
+                `TooManyMessagesPendingAckException`.
+
+        Examples:
+            async with queue.open_sub_manual_acking() as sub:
+                async for msg in sub.iter_messages():
+                    print(msg.data)
+                    sub.ack(msg)
+                    # if you choose not to nack on an error,
+                    # the broker will take longer to redeliver
+
+            async with queue.open_sub_manual_acking() as sub:
+                async for msg in sub.iter_messages():
+                    try:
+                        process_message(msg.data)
+                    except Exception:
+                        await sub.nack(msg)
+                    else:
+                        await sub.ack(msg)
+
+            async with queue.open_sub_manual_acking(ack_pending_limit=5) as sub:
+                pending = []
+                async for msg in sub.iter_messages():
+                    try:
+                        process_message(msg.data)
+                        pending.append(msg)
+                    except Exception:
+                        await sub.nack(msg)
+
+                    if len(pending) == 3:
+                        for msg in pending:
+                            await sub.ack(msg)
+                        pending = []
+
+                for msg in pending:
+                    await sub.ack(msg)
+
+        Returns:
+            ManualQueueSubResource -- context manager w/ iterator function
+        """
+        sub = await self._create_sub_queue(prefetch_override=ack_pending_limit)
+
+        try:
+            yield ManualQueueSubResource(
+                lambda: sub.get_message(self.timeout * 1000),
+                lambda msg: self._safe_ack(sub, msg),
+                lambda msg: self._safe_nack(sub, msg),
+                ack_pending_limit=sub.prefetch,
+            )
+        finally:
+            await sub.close()
+
+    @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
+    @wtt.spanned(
+        these=[
+            "self._broker_client",
+            "self._address",
+            "self._name",
+            "self._prefetch",
+            "self.timeout",
+        ]
+    )
     async def open_sub_one(self) -> AsyncIterator[Any]:
         """Open a context to receive a single messages from the queue.
 
         This is an async context manager. If an exception is raised
         (inside the context), the message is rejected, the context is
         exited, and exception can be re-raised if configured by
         `except_errors`.
@@ -295,30 +392,88 @@
         )
 
 
 class EmptyQueueException(Exception):
     """Raised when the queue is empty."""
 
 
+class TooManyMessagesPendingAckException(Exception):
+    """Raised when the ack-pending limit has been surpassed."""
+
+
 class QueuePubResource:
     """A manager class around `Pub.send_message()`."""
 
     def __init__(self, pub: Pub):
         self.pub = pub
 
     @wtt.spanned(kind=wtt.SpanKind.PRODUCER)
     async def send(self, data: Any) -> None:
         """Send a message."""
         msg_bytes = Message.serialize(data, headers=wtt.inject_links_carrier())
         LOGGER.info(f"Sending Message: {sys.getsizeof(msg_bytes)} bytes")
         await self.pub.send_message(msg_bytes)
 
 
+class ManualQueueSubResource:
+    """A manager class around `Sub.get_message()`."""
+
+    def __init__(
+        self,
+        get_message_function: Callable[[], Awaitable[Optional[Message]]],
+        ack_function: Callable[[Message], Awaitable[None]],
+        nack_function: Callable[[Message], Awaitable[None]],
+        ack_pending_limit: int,
+    ) -> None:
+        self._get_message = get_message_function
+        self._ack_function = ack_function
+        self._nack_function = nack_function
+        self._ack_pending = 0
+        self._ack_pending_limit = ack_pending_limit
+
+    async def iter_messages(self) -> AsyncIterator[Message]:
+        """Yield a message."""
+
+        @wtt.spanned(
+            kind=wtt.SpanKind.CONSUMER,
+            carrier="msg.headers",
+            carrier_relation=wtt.CarrierRelation.LINK,
+        )
+        def add_span_link(msg: Message) -> Message:
+            return msg
+
+        while True:
+            if self._ack_pending >= self._ack_pending_limit:
+                raise TooManyMessagesPendingAckException(
+                    f"{self._ack_pending} messages are pending ack/nack "
+                    f"(out of {self._ack_pending_limit} allowed)"
+                )
+
+            raw_msg = await self._get_message()
+            if not raw_msg:  # no message -> close and exit
+                return
+
+            msg = add_span_link(raw_msg)  # got a message -> link and proceed
+            LOGGER.info(f"Received Message: {_message_size_message(msg)}")
+            self._ack_pending += 1
+            yield msg
+
+    async def ack(self, msg: Message) -> None:
+        """Acknowledge the message."""
+        await self._ack_function(msg)
+        self._ack_pending -= 1
+
+    async def nack(self, msg: Message) -> None:
+        """Acknowledge the message."""
+        await self._nack_function(msg)
+        self._ack_pending -= 1
+
+
 class QueueSubResource:
-    """An async context manager wrapping `Sub.message_generator()`."""
+    """An async context-manager generator, wraps `Sub.message_generator()`."""
 
     RUNTIME_ERROR_CONTEXT_STRING = (
         "'QueueSubResource' object's runtime "
         "context has not been entered. Use 'async with ... as ...' syntax."
     )
 
     def __init__(self, queue: Queue) -> None:
```

### Comparing `oms-mqclient-2.0.0/mqclient/telemetry.py` & `oms-mqclient-2.1.0/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.1.0/oms_mqclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.0.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.1.0/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/setup.cfg` & `oms-mqclient-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 import logging
 from multiprocessing.dummy import Pool as ThreadPool
 from typing import Any, List
 
 import asyncstdlib as asl
 import pytest
-from mqclient.queue import Queue
+from mqclient.queue import Queue, TooManyMessagesPendingAckException
 
 from .utils import (
     DATA_LIST,
     _log_recv,
     _log_recv_multiple,
     _log_send,
     all_were_received,
@@ -21,16 +21,23 @@
 
 
 class PubSubQueue:
     """Integration test suite for Queue objects."""
 
     broker_client: str = ""
 
+    ###########################################################################
+    # tests 000 - 099:
+    #
+    # Testing scenarios with different numbers of sub and/or pubs
+    # to see no data loss
+    ###########################################################################
+
     @pytest.mark.asyncio
-    async def test_10(self, queue_name: str, auth_token: str) -> None:
+    async def test_010(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, one sub."""
         all_recvd: List[Any] = []
 
         pub_sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub_sub.open_pub() as p:
             await p.send(DATA_LIST[0])
             _log_send(DATA_LIST[0])
@@ -50,15 +57,15 @@
                 print(f"{i}: `{d}`")
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
-    async def test_11(self, queue_name: str, auth_token: str) -> None:
+    async def test_011(self, queue_name: str, auth_token: str) -> None:
         """Test an individual pub and an individual sub."""
         all_recvd: List[Any] = []
 
         pub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub.open_pub() as p:
             await p.send(DATA_LIST[0])
             _log_send(DATA_LIST[0])
@@ -79,15 +86,15 @@
                 print(f"{i}: `{d}`")
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
-    async def test_12(self, queue_name: str, auth_token: str) -> None:
+    async def test_012(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, two subs (one subscribed to wrong queue)."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             await p.send(DATA_LIST[0])
@@ -103,15 +110,15 @@
         ).open_sub_one() as d:
             all_recvd.append(_log_recv(d))
             assert d == DATA_LIST[0]
 
         assert all_were_received(all_recvd, [DATA_LIST[0]])
 
     @pytest.mark.asyncio
-    async def test_20(self, queue_name: str, auth_token: str) -> None:
+    async def test_020(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         # for each send, create and receive message via a new sub
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
@@ -123,15 +130,15 @@
                     self.broker_client, name=queue_name, auth_token=auth_token
                 ).open_sub_one() as d:
                     all_recvd.append(_log_recv(d))
                     assert d == data
 
         assert all_were_received(all_recvd)
 
-    async def _test_21(self, queue_name: str, num_subs: int, auth_token: str) -> None:
+    async def _test_021(self, queue_name: str, num_subs: int, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending)."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for data in DATA_LIST:
@@ -151,39 +158,39 @@
         with ThreadPool(num_subs) as pool:
             received_data = pool.map(start_recv_thread, range(num_subs))
         all_recvd.extend(item for sublist in received_data for item in sublist)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_21_fewer(self, queue_name: str, auth_token: str) -> None:
+    async def test_021_fewer(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Fewer subs than messages.
         """
-        await self._test_21(queue_name, len(DATA_LIST) // 2, auth_token)
+        await self._test_021(queue_name, len(DATA_LIST) // 2, auth_token)
 
     @pytest.mark.asyncio
-    async def test_21_same(self, queue_name: str, auth_token: str) -> None:
+    async def test_021_same(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Same number of subs as messages.
         """
-        await self._test_21(queue_name, len(DATA_LIST), auth_token)
+        await self._test_021(queue_name, len(DATA_LIST), auth_token)
 
     @pytest.mark.asyncio
-    async def test_21_more(self, queue_name: str, auth_token: str) -> None:
+    async def test_021_more(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         More subs than messages.
         """
-        await self._test_21(queue_name, len(DATA_LIST) ** 2, auth_token)
+        await self._test_021(queue_name, len(DATA_LIST) ** 2, auth_token)
 
     @pytest.mark.asyncio
-    async def test_22(self, queue_name: str, auth_token: str) -> None:
+    async def test_022(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Use the same number of subs as number of messages.
         """
         all_recvd: List[Any] = []
 
         async with Queue(
@@ -205,15 +212,15 @@
 
         with ThreadPool(len(DATA_LIST)) as pool:
             all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_23(self, queue_name: str, auth_token: str) -> None:
+    async def test_023(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, and too many subs.
 
         More subs than messages with `open_sub_one()` will raise an
         exception.
         """
         all_recvd: List[Any] = []
 
@@ -240,15 +247,15 @@
         # Extra Sub
         with pytest.raises(Exception):
             await recv_thread(-1)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_30(self, queue_name: str, auth_token: str) -> None:
+    async def test_030(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
 
         for data in DATA_LIST:
             async with Queue(
@@ -265,15 +272,15 @@
 
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_31(self, queue_name: str, auth_token: str) -> None:
+    async def test_031(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, unordered (front-loaded sending)."""
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
             async with Queue(
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_pub() as p:
@@ -285,15 +292,15 @@
         async with sub.open_sub() as gen:
             received_data = [m async for m in gen]
         all_recvd.extend(_log_recv_multiple(received_data))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_40(self, queue_name: str, auth_token: str) -> None:
+    async def test_040(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, ordered/alternatingly.
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -311,15 +318,15 @@
 
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_41(self, queue_name: str, auth_token: str) -> None:
+    async def test_041(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -334,15 +341,15 @@
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_42(self, queue_name: str, auth_token: str) -> None:
+    async def test_042(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the more pubs than subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -357,15 +364,15 @@
                 sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
             async with sub.open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_43(self, queue_name: str, auth_token: str) -> None:
+    async def test_043(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the fewer pubs than subs.
         """
         all_recvd: List[Any] = []
 
         for data_pairs in [DATA_LIST[i : i + 2] for i in range(0, len(DATA_LIST), 2)]:
@@ -381,15 +388,15 @@
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_50(self, queue_name: str, auth_token: str) -> None:
+    async def test_050(self, queue_name: str, auth_token: str) -> None:
         """Test_20 with variable prefetching.
 
         One pub, multiple subs.
         """
         all_recvd: List[Any] = []
 
         async with Queue(
@@ -410,15 +417,15 @@
                     async with sub.open_sub_one() as d:
                         all_recvd.append(_log_recv(d))
                         assert d == data
 
         assert all_were_received(all_recvd, DATA_LIST * ((len(DATA_LIST) * 2) - 1))
 
     @pytest.mark.asyncio
-    async def test_51(self, queue_name: str, auth_token: str) -> None:
+    async def test_051(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, with prefetching.
 
         Prefetching should have no visible affect.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -443,16 +450,22 @@
         sub2.timeout = 1
         async with sub2.open_sub() as gen:
             async for _, d in asl.enumerate(gen):
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
+    ###########################################################################
+    # tests 100 - 199:
+    #
+    # Tests for open_sub()
+    ###########################################################################
+
     @pytest.mark.asyncio
-    async def test_60(self, queue_name: str, auth_token: str) -> None:
+    async def test_100(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() fail and recovery, with multiple open_sub()
         calls."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
@@ -485,15 +498,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
         assert reused
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_61(self, queue_name: str, auth_token: str) -> None:
+    async def test_101(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() fail and recovery, with error propagation."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
@@ -530,15 +543,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
         assert reused
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
-    async def test_70_fail(self, queue_name: str, auth_token: str) -> None:
+    async def test_110__fail(self, queue_name: str, auth_token: str) -> None:
         """Failure-test open_sub() with reusing a 'QueueSubResource'
         instance."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
@@ -556,15 +569,15 @@
 
         # continue where we left off
         with pytest.raises(RuntimeError):
             async with recv_gen as gen:
                 assert 0  # we should never get here
 
     @pytest.mark.asyncio
-    async def test_80_break(self, queue_name: str, auth_token: str) -> None:
+    async def test_120_break(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() with a `break` statement."""
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for d in DATA_LIST:
                 await p.send(d)
                 _log_send(d)
@@ -584,7 +597,325 @@
         # continue where we left off
         async with sub.open_sub() as gen:
             async for i, d in asl.enumerate(gen):
                 print(f"{i}: `{d}`")
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
+
+    ###########################################################################
+    # tests 200 - 299:
+    #
+    # Tests for open_sub_manual_acking()
+    ###########################################################################
+
+    @pytest.mark.asyncio
+    async def test_200__ideal(self, queue_name: str, auth_token: str) -> None:
+        """Test open_sub_manual_acking() ideal scenario."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking() as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                print(f"{i}: `{msg.data}`")
+                all_recvd.append(_log_recv(msg.data))
+                # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                await gen.ack(msg)
+
+        print(all_recvd)
+        assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    async def test_210__immediate_recovery(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() fail and immediate recovery, with
+        nacking."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        class TestException(Exception):  # pylint: disable=C0115
+            pass
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking() as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                try:
+                    # DO WORK!
+                    print(f"{i}: `{msg.data}`")
+                    if i == 2:
+                        raise TestException()
+                    all_recvd.append(_log_recv(msg.data))
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                except Exception:
+                    await gen.nack(msg)
+                else:
+                    await gen.ack(msg)
+
+        print(all_recvd)
+        assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    async def test_220__posthoc_recovery(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() fail and post-hoc recovery, with
+        nacking."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        class TestException(Exception):  # pylint: disable=C0115
+            pass
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        excepted = False
+        sub.timeout = 1
+        # sub.except_errors = False  # has no effect
+        async with sub.open_sub_manual_acking() as gen:
+            try:
+                async for i, msg in asl.enumerate(gen.iter_messages()):
+                    print(f"{i}: `{msg.data}`")
+                    if i == 2:
+                        raise TestException()
+                    all_recvd.append(_log_recv(msg.data))
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    await gen.ack(msg)
+            except TestException:
+                excepted = True
+                await gen.nack(msg)
+        assert excepted
+
+        logging.warning("Round 2!")
+
+        # continue where we left off
+        posthoc = False
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking() as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                print(f"{i}: `{msg.data}`")
+                posthoc = True
+                all_recvd.append(_log_recv(msg.data))
+                # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                await gen.ack(msg)
+        assert posthoc
+        print(all_recvd)
+        assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    async def test_221__posthoc_recovery__fail(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() fail, post-hoc recovery, then fail.
+
+        Final fail is due to not nacking.
+        """
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        class TestException(Exception):  # pylint: disable=C0115
+            pass
+
+        errored_msg = None
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        excepted = False
+        async with sub.open_sub_manual_acking() as gen:
+            try:
+                async for i, msg in asl.enumerate(gen.iter_messages()):
+                    print(f"{i}: `{msg.data}`")
+                    if i == 2:
+                        errored_msg = msg.data
+                        raise TestException()
+                    all_recvd.append(_log_recv(msg.data))
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    await gen.ack(msg)
+            except TestException:
+                excepted = True
+                # await gen.nack(msg)  # no acking
+        assert excepted
+
+        logging.warning("Round 2!")
+
+        # continue where we left off
+        posthoc = False
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking() as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                print(f"{i}: `{msg.data}`")
+                posthoc = True
+                all_recvd.append(_log_recv(msg.data))
+                # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                await gen.ack(msg)
+        assert posthoc
+
+        # Either all the messages have been gotten (re-opening the connection took longer enough)
+        # OR it hasn't been long enough to redeliver un-acked/nacked message
+        # This is difficult to test -- all we can tell is if it is one of these scenarios
+        print(all_recvd)
+        assert all_were_received(all_recvd) or (
+            all_were_received(all_recvd + [errored_msg])
+        )
+
+    @pytest.mark.asyncio
+    async def test_230__fail_bad_usage(self, queue_name: str, auth_token: str) -> None:
+        """Failure-test open_sub_manual_acking() with reusing a
+        'QueueSubResource' instance."""
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        recv_gen = sub.open_sub_manual_acking()
+        async with recv_gen as gen:
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                print(f"{i}: `{msg.data}`")
+                # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                await gen.ack(msg)
+
+        logging.warning("Round 2!")
+
+        # continue where we left off
+        with pytest.raises((AttributeError, RuntimeError)):
+            # AttributeError: '_AsyncGeneratorContextManager' object has no attribute 'args'
+            # RuntimeError: generator didn't yield
+            async with recv_gen as gen:
+                assert 0  # we should never get here
+
+    @pytest.mark.asyncio
+    async def test_240__delayed_mixed_acking_nacking(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() fail and immediate recovery with
+        multi-tasking, with mixed acking and nacking."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        class TestException(Exception):  # pylint: disable=C0115
+            pass
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        async with sub.open_sub_manual_acking(ack_pending_limit=len(DATA_LIST)) as gen:
+            pending = []
+            async for i, msg in asl.enumerate(gen.iter_messages()):
+                try:
+                    # DO WORK!
+                    print(f"{i}: `{msg.data}`")
+                    if i % 3 == 0:  # nack every 1/3
+                        raise TestException()
+                    all_recvd.append(_log_recv(msg.data))
+                    pending.append(msg)
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    if i % 2 == 0:  # ack every 1/2
+                        await gen.ack(msg)
+                        pending.remove(msg)
+                except Exception:
+                    await gen.nack(msg)
+
+            for msg in pending:  # messages with index not %2 nor %3, (1,5,7,...)
+                await gen.ack(msg)
+
+        print(all_recvd)
+        assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    async def test_250__delayed_acking__fail(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() w/ delayed acking AND surpass
+        `ack_pending_limit`."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        ack_pending_limit = len(DATA_LIST) // 2
+        async with sub.open_sub_manual_acking(ack_pending_limit) as gen:
+            messages = []
+            with pytest.raises(TooManyMessagesPendingAckException):
+                async for i, msg in asl.enumerate(gen.iter_messages()):
+                    print(f"{i}: `{msg.data}`")
+                    all_recvd.append(_log_recv(msg.data))
+                    messages.append(msg)
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    assert gen._ack_pending == i + 1
+
+        print(all_recvd)
+        assert not all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    async def test_251__no_nacking__fail(
+        self, queue_name: str, auth_token: str
+    ) -> None:
+        """Test open_sub_manual_acking() w/ delayed acking AND surpass
+        `ack_pending_limit`."""
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for d in DATA_LIST:
+                await p.send(d)
+                _log_send(d)
+
+        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
+        sub.timeout = 1
+        ack_pending_limit = len(DATA_LIST) // 2
+        async with sub.open_sub_manual_acking(ack_pending_limit) as gen:
+            messages = []
+            with pytest.raises(TooManyMessagesPendingAckException):
+                async for i, msg in asl.enumerate(gen.iter_messages()):
+                    print(f"{i}: `{msg.data}`")
+                    all_recvd.append(_log_recv(msg.data))
+                    messages.append(msg)
+                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
+                    if i % 2 == 0:
+                        pass  # eventually enough "passes" causes a TooManyMessagesPendingAckException
+                    else:
+                        await gen.ack(msg)
+                    assert gen._ack_pending == (i // 2) + 1
+
+        print(all_recvd)
+        assert not all_were_received(all_recvd)
```

### Comparing `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/integrate/conftest.py` & `oms-mqclient-2.1.0/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/integrate/test_nats.py` & `oms-mqclient-2.1.0/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.1.0/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.1.0/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.1.0/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.0.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.1.0/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

