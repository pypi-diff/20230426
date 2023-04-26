# Comparing `tmp/sending-0.2.2.tar.gz` & `tmp/sending-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sending-0.2.2.tar", max compression
+gzip compressed data, was "sending-0.3.0.tar", max compression
```

## Comparing `sending-0.2.2.tar` & `sending-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      873 2022-07-28 20:53:12.545286 sending-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2022-04-29 16:38:58.758613 sending-0.2.2/sending/__init__.py
--rw-r--r--   0        0        0     4749 2022-07-26 19:50:11.895466 sending-0.2.2/sending/backends/jupyter.py
--rw-r--r--   0        0        0     1320 2022-04-29 20:47:41.331714 sending-0.2.2/sending/backends/memory.py
--rw-r--r--   0        0        0     1252 2022-04-29 16:38:58.759009 sending-0.2.2/sending/backends/redis.py
--rw-r--r--   0        0        0    16185 2022-07-28 20:48:42.946944 sending-0.2.2/sending/base.py
--rw-r--r--   0        0        0      337 2022-04-29 16:38:58.759377 sending-0.2.2/sending/logging.py
--rw-r--r--   0        0        0      369 2022-07-22 22:07:48.992187 sending-0.2.2/sending/util.py
--rw-r--r--   0        0        0      721 2022-07-28 20:54:04.313681 sending-0.2.2/setup.py
--rw-r--r--   0        0        0      530 2022-07-28 20:54:04.313878 sending-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1280 2023-04-26 17:45:32.244905 sending-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-26 17:45:32.244905 sending-0.3.0/sending/__init__.py
+-rw-r--r--   0        0        0    10067 2023-04-26 17:45:32.248905 sending-0.3.0/sending/backends/jupyter.py
+-rw-r--r--   0        0        0     1581 2023-04-26 17:45:32.248905 sending-0.3.0/sending/backends/memory.py
+-rw-r--r--   0        0        0     1507 2023-04-26 17:45:32.248905 sending-0.3.0/sending/backends/redis.py
+-rw-r--r--   0        0        0    11403 2023-04-26 17:45:32.248905 sending-0.3.0/sending/backends/websocket.py
+-rw-r--r--   0        0        0    20386 2023-04-26 17:45:32.248905 sending-0.3.0/sending/base.py
+-rw-r--r--   0        0        0      337 2023-04-26 17:45:32.248905 sending-0.3.0/sending/logging.py
+-rw-r--r--   0        0        0      369 2023-04-26 17:45:32.248905 sending-0.3.0/sending/util.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 sending-0.3.0/PKG-INFO
```

### Comparing `sending-0.2.2/pyproject.toml` & `sending-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 [tool.poetry]
 name = "sending"
-version = "0.2.2"
+version = "0.3.0"
 description = "Library for pub/sub usage within an async application"
 authors = ["Nicholas Wold <nick@nicholaswold.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 aioredis = {extras = ["hiredis"], version = "^2.0.0", optional = true}
 jupyter_client = {version = "^7.3.0", optional = true}
+ipykernel = {version = "^6.15.1", optional = true}
+websockets = {version = "^10.3", optional = true}
 
 [tool.poetry.extras]
 redis = ["aioredis"]
-jupyter = ["jupyter_client"]
+jupyter = ["jupyter_client", "ipykernel"]
+websockets = ["websockets"]
+all = ["aioredis", "jupyter_client", "ipykernel", "websockets"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.7.0"
 black = "^22.3.0"
-flake8 = "^4.0.1"
-pytest-asyncio = "^0.18.3"
+flake8 = "^5.0.4"
+pytest-asyncio = "^0.19"
 isort = "^5.10.1"
-nox = "^2022.1.7"
+nox = "^2022.8.7"
+managed-service-fixtures = "^0.1.4"
+nox-poetry = "^1.0.1"
+pytest-cov = "^3.0.0"
+uvicorn = "^0.18.2"
+fastapi = "^0.79.0"
+httpx = "^0.23.0"
+structlog = "^22.1.0"
+pytest-timeout = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-markers = ["redis", "jupyter"]
 asyncio_mode = "auto"
+filterwarnings = ["ignore::DeprecationWarning"]
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 line_length = 100
 multi_line_output = 3
```

### Comparing `sending-0.2.2/sending/base.py` & `sending-0.3.0/sending/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-"""This module defines an abstract PubSubManager class that must be used when
-   implementing custom managers or other features."""
+"""Publish Subscribe Managers and PubSub sessions.
+
+This module defines an abstract `AbstractPubSubManager` class that must be
+subclassed when implementing custom managers or other features.
+
+This module also implements a `DetachedPubSubSession` that receives messages
+only for topics which it has a subscription.
+
+The module also implements a more robust `PubSubSession`, a subclass of
+`DetachedPubSubSession, which receives messages from topics that it or its
+parent have a subscription.
+"""
 import abc
 import asyncio
 import enum
+import traceback
 from collections import defaultdict, namedtuple
 from functools import partial, wraps
-from typing import Callable, Coroutine, Dict, List, Set
+from typing import Callable, Dict, List, Optional, Set
 from uuid import UUID, uuid4
 
 from .logging import logger
 from .util import ensure_async
 
 QueuedMessage = namedtuple("QueuedMessage", ["topic", "contents", "session_id"])
 Callback = namedtuple("Callback", ["method", "predicate", "qualname"])
@@ -17,23 +28,26 @@
 __not_in_a_session__ = object()
 
 # Reserved name for system events sent by the library
 SYSTEM_TOPIC = "__sending__"
 
 
 class SystemEvents(enum.Enum):
-    # Umbrella event for disconnects caused by circumstances out of the user's control.
-    # Could be a network error, or something like ZMQ's MAXMSGSIZE flag forcibly disconnecting
-    # the peer.
+    """System events related to the pub/sub manager
+
+    We've forcibly disconnected from the pub/sub server. This is for situations
+    where the underlying backend has forced a disconnect without the user
+    asking. ZMQ `MAXMSGSIZE` cycling connections is a good example.
+    """
+
     FORCED_DISCONNECT = enum.auto()
 
 
 class AbstractPubSubManager(abc.ABC):
-    """
-    Manages the publish-subscribe workflow.
+    """A manager for the publish-subscribe workflow.
 
     This abstract class provides a common base class for a publish-subscribe
     workflow and the management of components in the workflow.
 
     The manager keeps track of message queues and workers that serve clients
     subscribed to a publisher's feed of messages.
     """
@@ -47,40 +61,92 @@
 
         self.poll_workers: List[asyncio.Task] = []
         self.subscribed_topics_by_session: Dict[str, Set] = defaultdict(set)
 
         self.callbacks_by_id: Dict[UUID, Callback] = {}
         self.callback_ids_by_session: Dict[UUID, Set[UUID]] = defaultdict(set)
 
-        self.inbound_message_hook: Coroutine = None
-        self.outbound_message_hook: Coroutine = None
+        # Allow these hooks to be defined within the class or attached to an instance
+        if not hasattr(self, "inbound_message_hook"):
+            # Called by _inbound_worker when picking up a message from inbound queue
+            # Primarily used for deserializing messages from the wire
+            # Will get one argument: incoming "raw" message content over the wire
+            self.inbound_message_hook: Optional[Callable] = None
+        if not hasattr(self, "outbound_message_hook"):
+            # Called by _outbound_worker before pushing a message to _publish
+            # Primarily used for serializing messages going out over the wire
+            # Will get one argument, the QueuedMessage.contents coming out of .send()
+            self.outbound_message_hook: Optional[Callable] = None
+        if not hasattr(self, "context_hook"):
+            # Called at .initialize() and then within the while True loop for
+            # each worker. Should be used to set structlog.contextvars.bind_contextvars.
+            # Takes no arguments
+            self.context_hook: Optional[Callable] = None
+        if not hasattr(self, "callback_hook"):
+            # Called when the inbound worker is about to pass a QueuedMessage.contents
+            # into a callback. Primarily used for logging the QueuedMessage.topic as
+            # contextvars in the callback logging. Can be removed if we begin passing
+            # kwargs / full QueuedMessage to callbacks.
+            # Takses two arguments: the QueuedMessage and the Callback
+            self.callback_hook: Optional[Callable] = None
 
     async def initialize(
         self,
         *,
         queue_size=0,
         inbound_workers=1,
         outbound_workers=1,
         poll_workers=1,
+        enable_polling=True,
     ):
-        """Initialize a pub-sub channel, specifically its queues and workers."""
+        """Initialize a pub-sub channel, specifically its queues and workers.
+
+        `enable_polling` if set to True, the default, will start the poll
+        workers. If `enable_polling` is False, it will only start the inbound
+        and outbound workers and not start the poll worker. The False setting
+        is useful if you're writing tests and don't want a connection to
+        external IO to be started.
+
+        ```
+        mgr = SomeBackend()
+        publish = mocker.patch.object(mgr, "_publish")
+
+        @mgr.callback(on_topic="test-topic")
+        def echo(msg: str):
+            mgr.send(topic_name="test-topic", message=msg)
+
+        await mgr.initialize(enable_polling=False)
+        mgr.schedule_for_delivery(topic="test-topic", contents="echo test")
+        await asyncio.sleep(0.01)
+        publish.assert_called_once_with(
+            QueuedMessage(topic="test-topic, contents="echo test", session_id=None)
+        )
+        ```
+        """
+        if self.context_hook:
+            await self.context_hook()
         self.outbound_queue = asyncio.Queue(queue_size)
         self.inbound_queue = asyncio.Queue(queue_size)
 
         for i in range(outbound_workers):
             self.outbound_workers.append(asyncio.create_task(self._outbound_worker()))
 
         for i in range(inbound_workers):
             self.inbound_workers.append(asyncio.create_task(self._inbound_worker()))
 
-        for i in range(poll_workers):
-            self.poll_workers.append(asyncio.create_task(self._poll_loop()))
+        if enable_polling:
+            for i in range(poll_workers):
+                self.poll_workers.append(asyncio.create_task(self._poll_loop()))
 
     async def shutdown(self, now=False):
-        """Shut down a pub-sub channel and its related queues and workers"""
+        """Shut down a pub-sub channel and its related queues and workers.
+
+        The `now` parameter will drain queues gracefully if set to the default
+        False. If set to True, the queues are cleared and set to None.
+        """
         if not now:
             await self._drain_queues()
 
         self.inbound_queue = None
 
         self.outbound_queue = None
 
@@ -104,14 +170,15 @@
         self.inbound_workers.clear()
         self.poll_workers.clear()
         self.subscribed_topics_by_session.clear()
         self.callbacks_by_id.clear()
         self.callback_ids_by_session.clear()
 
     async def _drain_queues(self):
+        """Private method which waits for queues to clear."""
         await self.inbound_queue.join()
         await self.outbound_queue.join()
 
     def send(self, topic_name: str, message):
         """Sends a message to a specific topic's queue."""
         self.outbound_queue.put_nowait(QueuedMessage(topic_name, message, None))
 
@@ -224,22 +291,27 @@
 
             if _session_id is not None:
                 self.callback_ids_by_session[_session_id].remove(cb_id)
 
     async def _outbound_worker(self):
         while True:
             message = await self.outbound_queue.get()
+            if self.context_hook:
+                await self.context_hook()
             try:
                 if self.outbound_message_hook is not None:
                     coro = ensure_async(self.outbound_message_hook)
                     message = message._replace(contents=await coro(message.contents))
                 logger.debug(f"Sending message to topic: {message.topic}")
                 await self._publish(message)
-            except Exception:
-                logger.exception("Uncaught exception found while publishing message")
+            except Exception as e:
+                tb_str = traceback.format_exception(etype=type(e), value=e, tb=e.__traceback__)
+                logger.exception(
+                    "Uncaught exception found while publishing message", exc_info="".join(tb_str)
+                )
             finally:
                 self.outbound_queue.task_done()
 
     @abc.abstractmethod
     async def _publish(self, message: QueuedMessage):
         """The action needed to publish the message to the backend pubsub
         implementation.
@@ -247,30 +319,35 @@
         This will only be called by the outbound worker.
         """
         pass
 
     async def _inbound_worker(self):
         while True:
             message = await self.inbound_queue.get()
-
+            if self.context_hook:
+                await self.context_hook()
             try:
                 if self.inbound_message_hook is not None and message.topic is not SYSTEM_TOPIC:
                     coro = ensure_async(self.inbound_message_hook)
                     message = message._replace(contents=await coro(message.contents))
 
                 if message.session_id is None:
                     callback_ids = list(self.callbacks_by_id.keys())
                 else:
                     callback_ids = self.callback_ids_by_session[message.session_id]
 
                 await asyncio.gather(
                     *[self._delegate_to_callback(message, cb_id) for cb_id in callback_ids]
                 )
-            except Exception:
-                logger.exception("Uncaught exception found while processing inbound message")
+            except Exception as e:
+                tb_str = traceback.format_exception(etype=type(e), value=e, tb=e.__traceback__)
+                logger.exception(
+                    "Uncaught exception found while processing inbound message",
+                    exc_info="".join(tb_str),
+                )
             finally:
                 self.inbound_queue.task_done()
 
     async def _delegate_to_callback(self, message: QueuedMessage, callback_id: UUID):
         cb = self.callbacks_by_id.get(callback_id)
         if cb is not None:
             try:
@@ -280,62 +357,72 @@
                 if cb.predicate is None or await cb.predicate(
                     message.topic, message.contents, system_event=system_event
                 ):
                     logger.debug(f"Delegating to callback: '{cb.qualname}'")
                     # TODO(nick): I would love to have a set of kwargs that are passed around
                     # for callbacks + predicates that you opt-in to. That would be a bit easier
                     # to document and access.
+                    if self.callback_hook:
+                        await self.callback_hook(message, cb)
                     await cb.method(message.contents)
                 else:
                     logger.debug(
                         f"Skipping callback '{cb.qualname}' because predicate returned False"
                     )
-            except Exception:
-                logger.exception("Uncaught exception encountered while delegating to callback")
+            except Exception as e:
+                tb_str = traceback.format_exception(etype=type(e), value=e, tb=e.__traceback__)
+                logger.exception(
+                    "Uncaught exception encountered while delegating to callback",
+                    exc_info="".join(tb_str),
+                )
 
     async def _poll_loop(self):
         while True:
+            if self.context_hook:
+                await self.context_hook()
             try:
                 await self._poll()
             except Exception:
                 logger.exception("Uncaught exception encountered while polling backend")
             finally:
                 await asyncio.sleep(0)
 
     @abc.abstractmethod
     async def _poll(self):
         pass
 
     def schedule_for_delivery(self, topic, contents, _session_id=None):
         """Use contents to create and queue a message for the topic's feed."""
+        logger.debug(f"Scheduling message for delivery on topic: {topic}")
         message = QueuedMessage(topic, contents, _session_id)
         self.inbound_queue.put_nowait(message)
 
     def get_detached_session(self):
         """Get a new session for callbacks and subscriptions that won't receive
         global messages from this parent.
         """
         return DetachedPubSubSession(self)
 
     def get_session(self):
         """Get a new session for callbacks and subscriptions."""
         return PubSubSession(self)
 
     def _emit_system_event(self, topic: str, event: SystemEvents):
+        logger.debug(f"Emitting system event: {event}")
         self.schedule_for_delivery(SYSTEM_TOPIC, {"event": event, "topic": topic})
 
 
 class DetachedPubSubSession:
-    """A session that does not receive messages for topics other than what it has explicitly
-    subscribed to.
+    """A session that receives messages from subscribed topics.
 
-    It still relies on the parent as the centralized queuing mechanism for processing inbound
-    and outbound messages, but it ensures total isolation for what messages get passed down to
-    the session's callbacks. This is helpful if you don't want to have a separate polling process
-    for each session.
+    It still relies on the parent PubSubManager as the centralized queuing
+    mechanism for processing inbound and outbound messages. It also ensures
+    total isolation for what messages get passed down to the session's callbacks
+    (detached from its parent's subscriptions). This is helpful when a separate
+    polling process is needed for each session.
     """
 
     def __init__(self, parent: AbstractPubSubManager) -> None:
         self.id: str = str(uuid4())
         self.parent: AbstractPubSubManager = parent
         self._unregister_callbacks_by_id: Dict[str, Callable] = {}
 
@@ -402,17 +489,17 @@
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.stop()
 
 
 class PubSubSession(DetachedPubSubSession):
-    """A holder for callbacks and topic subscriptions. Also receives messages from topics
-    subscribed to by the parent manager.
+    """A holder for callbacks and topic subscriptions.
 
+    Also receives messages from topics subscribed to by the parent manager.
     This is helpful if you have a global topic that all sessions should subscribe to
     automatically without client input.
     """
 
     @property
     def subscribed_topics(self) -> Set[str]:
         all_session_topics = self.parent.subscribed_topics_by_session[__not_in_a_session__]
```

