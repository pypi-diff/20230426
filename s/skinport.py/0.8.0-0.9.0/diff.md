# Comparing `tmp/skinport.py-0.8.0.tar.gz` & `tmp/skinport.py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skinport.py-0.8.0.tar", last modified: Mon Apr 10 09:50:49 2023, max compression
+gzip compressed data, was "skinport.py-0.9.0.tar", last modified: Wed Apr 26 06:32:19 2023, max compression
```

## Comparing `skinport.py-0.8.0.tar` & `skinport.py-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.605711 skinport.py-0.8.0/
--rw-rw-rw-   0        0        0     1089 2022-02-12 03:07:11.000000 skinport.py-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     1821 2023-04-10 09:50:49.604210 skinport.py-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      806 2022-02-20 02:32:30.000000 skinport.py-0.8.0/README.md
--rw-rw-rw-   0        0        0       82 2022-02-13 10:52:31.000000 skinport.py-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 09:50:49.605711 skinport.py-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1635 2023-04-10 09:42:35.000000 skinport.py-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.572301 skinport.py-0.8.0/skinport/
--rw-rw-rw-   0        0        0      958 2023-04-10 09:48:24.000000 skinport.py-0.8.0/skinport/__init__.py
--rw-rw-rw-   0        0        0    12303 2023-04-10 09:39:20.000000 skinport.py-0.8.0/skinport/client.py
--rw-rw-rw-   0        0        0     1599 2023-04-10 09:36:05.000000 skinport.py-0.8.0/skinport/color.py
--rw-rw-rw-   0        0        0     2298 2022-03-15 20:46:37.000000 skinport.py-0.8.0/skinport/enums.py
--rw-rw-rw-   0        0        0     4387 2022-03-11 08:02:20.000000 skinport.py-0.8.0/skinport/errors.py
--rw-rw-rw-   0        0        0     4480 2023-04-10 09:35:57.000000 skinport.py-0.8.0/skinport/http.py
--rw-rw-rw-   0        0        0     8941 2022-03-11 08:02:20.000000 skinport.py-0.8.0/skinport/item.py
--rw-rw-rw-   0        0        0     3253 2023-04-10 09:36:08.000000 skinport.py-0.8.0/skinport/iterators.py
--rw-rw-rw-   0        0        0     3357 2023-04-10 09:34:15.000000 skinport.py-0.8.0/skinport/sale.py
--rw-rw-rw-   0        0        0    17553 2023-04-10 09:36:12.000000 skinport.py-0.8.0/skinport/salefeed.py
--rw-rw-rw-   0        0        0     6812 2022-02-18 09:14:40.000000 skinport.py-0.8.0/skinport/transaction.py
--rw-rw-rw-   0        0        0      380 2022-03-15 20:56:14.000000 skinport.py-0.8.0/skinport/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.591677 skinport.py-0.8.0/skinport.py.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-10 09:50:49.000000 skinport.py-0.8.0/skinport.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 09:50:49.602689 skinport.py-0.8.0/tests/
--rw-rw-rw-   0        0        0     1689 2023-04-10 09:37:31.000000 skinport.py-0.8.0/tests/test_client.py
--rw-rw-rw-   0        0        0      989 2022-03-10 18:28:07.000000 skinport.py-0.8.0/tests/test_color.py
--rw-rw-rw-   0        0        0     2833 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_item.py
--rw-rw-rw-   0        0        0     5034 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_sale.py
--rw-rw-rw-   0        0        0     3360 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_salefeed.py
--rw-rw-rw-   0        0        0     2556 2022-03-11 08:02:20.000000 skinport.py-0.8.0/tests/test_transaction.py
--rw-rw-rw-   0        0        0      561 2023-04-10 09:34:45.000000 skinport.py-0.8.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:32:19.475116 skinport.py-0.9.0/
+-rw-rw-rw-   0        0        0     1089 2022-02-12 03:07:11.000000 skinport.py-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1821 2023-04-26 06:32:19.474117 skinport.py-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2022-02-20 02:32:30.000000 skinport.py-0.9.0/README.md
+-rw-rw-rw-   0        0        0       82 2022-02-13 10:52:31.000000 skinport.py-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 06:32:19.475116 skinport.py-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-04-10 09:42:35.000000 skinport.py-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:32:19.441087 skinport.py-0.9.0/skinport/
+-rw-rw-rw-   0        0        0      958 2023-04-26 06:31:06.000000 skinport.py-0.9.0/skinport/__init__.py
+-rw-rw-rw-   0        0        0    12899 2023-04-26 06:29:26.000000 skinport.py-0.9.0/skinport/client.py
+-rw-rw-rw-   0        0        0     1599 2023-04-10 09:36:05.000000 skinport.py-0.9.0/skinport/color.py
+-rw-rw-rw-   0        0        0     2298 2022-03-15 20:46:37.000000 skinport.py-0.9.0/skinport/enums.py
+-rw-rw-rw-   0        0        0     4387 2022-03-11 08:02:20.000000 skinport.py-0.9.0/skinport/errors.py
+-rw-rw-rw-   0        0        0     4480 2023-04-10 09:35:57.000000 skinport.py-0.9.0/skinport/http.py
+-rw-rw-rw-   0        0        0     8941 2022-03-11 08:02:20.000000 skinport.py-0.9.0/skinport/item.py
+-rw-rw-rw-   0        0        0     3253 2023-04-10 09:36:08.000000 skinport.py-0.9.0/skinport/iterators.py
+-rw-rw-rw-   0        0        0     3357 2023-04-10 09:34:15.000000 skinport.py-0.9.0/skinport/sale.py
+-rw-rw-rw-   0        0        0    17553 2023-04-10 09:36:12.000000 skinport.py-0.9.0/skinport/salefeed.py
+-rw-rw-rw-   0        0        0     6812 2022-02-18 09:14:40.000000 skinport.py-0.9.0/skinport/transaction.py
+-rw-rw-rw-   0        0        0      380 2022-03-15 20:56:14.000000 skinport.py-0.9.0/skinport/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:32:19.462105 skinport.py-0.9.0/skinport.py.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-26 06:32:19.000000 skinport.py-0.9.0/skinport.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-04-26 06:32:19.000000 skinport.py-0.9.0/skinport.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 06:32:19.000000 skinport.py-0.9.0/skinport.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-26 06:32:19.000000 skinport.py-0.9.0/skinport.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 06:32:19.000000 skinport.py-0.9.0/skinport.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 06:32:19.473116 skinport.py-0.9.0/tests/
+-rw-rw-rw-   0        0        0     1689 2023-04-10 09:37:31.000000 skinport.py-0.9.0/tests/test_client.py
+-rw-rw-rw-   0        0        0      989 2022-03-10 18:28:07.000000 skinport.py-0.9.0/tests/test_color.py
+-rw-rw-rw-   0        0        0     2833 2022-03-11 08:02:20.000000 skinport.py-0.9.0/tests/test_item.py
+-rw-rw-rw-   0        0        0     5034 2022-03-11 08:02:20.000000 skinport.py-0.9.0/tests/test_sale.py
+-rw-rw-rw-   0        0        0     3360 2022-03-11 08:02:20.000000 skinport.py-0.9.0/tests/test_salefeed.py
+-rw-rw-rw-   0        0        0     2556 2022-03-11 08:02:20.000000 skinport.py-0.9.0/tests/test_transaction.py
+-rw-rw-rw-   0        0        0      561 2023-04-10 09:34:45.000000 skinport.py-0.9.0/tests/test_utils.py
```

### Comparing `skinport.py-0.8.0/LICENSE` & `skinport.py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/PKG-INFO` & `skinport.py-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skinport.py
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python wrapper for the Skinport API
 Home-page: https://github.com/PaxxPatriot/skinport.py
 Author: PaxxPatriot
 Author-email: skinport.py@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skinport.py-0.8.0/README.md` & `skinport.py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/setup.py` & `skinport.py-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/__init__.py` & `skinport.py-0.9.0/skinport/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 :copyright: (c) 2022 PaxxPatriot
 :license: MIT, see LICENSE for more details.
 """
 __title__ = "skinport"
 __author__ = "PaxxPatriot"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 PaxxPatriot"
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple
 
 from . import utils
@@ -32,10 +32,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: str
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=0, minor=8, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=0, minor=9, micro=0, releaselevel="final", serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `skinport.py-0.8.0/skinport/client.py` & `skinport.py-0.9.0/skinport/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         _log.info("Closing the event loop.")
         loop.close()
 
 
 class Client:
     def __init__(self):
         self.http: HTTPClient = HTTPClient()
-        self.ws: socketio.AsyncClient = socketio.AsyncClient()
-        self._closed = False
+        self.ws: socketio.AsyncClient = socketio.AsyncClient(logger=True, engineio_logger=True)
+        self._connected = False
 
     def set_auth(self, *, client_id: str, client_secret: str):
         self.http.set_auth(client_id, client_secret)
 
     def run(self, *args: Any, **kwargs: Any) -> None:
         """A blocking call that abstracts away the event loop
         initialisation from you.
@@ -108,15 +108,15 @@
         except NotImplementedError:
             pass
 
         async def runner():
             try:
                 await self.connect(*args, **kwargs)
             finally:
-                if not self._closed:
+                if self._connected:
                     await self.close()
 
         def stop_loop_on_completion(f):
             loop.stop()
 
         future = asyncio.ensure_future(runner(), loop=loop)
         future.add_done_callback(stop_loop_on_completion)
@@ -182,44 +182,58 @@
             The currency for pricing.
             Defaults to ``EUR``.
         locale: :class:`Locale`
             Whether or not to show only tradable items.
             Defaults to ``en``.
         """
         # Get parameters for the sale feed
+        if self._connected:
+            _log.info("Client is already connected. Closing the existing connection.")
+            await self.close()
+
+        try:
+            self.ws.on("*", self.catch_all)
+            self.ws.on("connect", lambda: asyncio.ensure_future(self.on_connect(**kwargs)))
+            await self.ws.connect("https://skinport.com", transports=["websocket"])
+            self._connected = True
+            await self.ws.wait()
+        except asyncio.TimeoutError:
+            _log.info("Connection timed out.")
+            await self.close()
+            self._connected = False
+        except socketio.exceptions.ConnectionError:
+            _log.warning("Client is already connected. Skipping connection attempt.")
+
+
+    async def on_connect(self, **kwargs: Any) -> None:
+            _log.info("Connected to Skinport. Emitting saleFeedJoin event...")
+            await self._emit_sale_feed_join(kwargs)
+
+    async def _emit_sale_feed_join(self, kwargs: Dict[str, Any]) -> None:
         app_id = kwargs.get("app_id", AppID.csgo)
         currency = kwargs.get("currency", Currency.eur)
         locale = kwargs.get("locale", Locale.en)
-
-        while not self._closed:
-            try:
-                self.ws.on("*", self.catch_all)
-                await self.ws.connect("https://skinport.com", transports=["websocket"])
-                await self.ws.emit(
-                    "saleFeedJoin",
-                    {
-                        "currency": currency.value,
-                        "locale": locale.value,
-                        "appid": app_id.value,
-                    },
-                )
-                await self.ws.wait()
-            except asyncio.TimeoutError:
-                _log.info("Connection timed out.")
-                await self.close()
-                await asyncio.sleep(5)  # Sleep 5 seconds to handle connection closing
-
+        await self.ws.emit(
+            "saleFeedJoin",
+            {
+                "currency": currency.value,
+                "locale": locale.value,
+                "appid": app_id.value,
+            },
+        )
+        await self.ws.wait()
+        
     async def close(self) -> None:
         """*coroutine*
         Closes the `aiohttp.ClientSession`.
         """
-        if self._closed:
+        if not self._connected:
             return
 
-        self._closed = True
+        self._connected = False
         if self.ws.eio.http is not None:
             await self.ws.eio.http.close()
         await self.http.close()
 
     @cached(cache=TTLCache(maxsize=128, ttl=300))
     async def get_items(
         self,
```

### Comparing `skinport.py-0.8.0/skinport/color.py` & `skinport.py-0.9.0/skinport/color.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/enums.py` & `skinport.py-0.9.0/skinport/enums.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/errors.py` & `skinport.py-0.9.0/skinport/errors.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/http.py` & `skinport.py-0.9.0/skinport/http.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/item.py` & `skinport.py-0.9.0/skinport/item.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/iterators.py` & `skinport.py-0.9.0/skinport/iterators.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/sale.py` & `skinport.py-0.9.0/skinport/sale.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/salefeed.py` & `skinport.py-0.9.0/skinport/salefeed.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport/transaction.py` & `skinport.py-0.9.0/skinport/transaction.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/skinport.py.egg-info/PKG-INFO` & `skinport.py-0.9.0/skinport.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skinport.py
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python wrapper for the Skinport API
 Home-page: https://github.com/PaxxPatriot/skinport.py
 Author: PaxxPatriot
 Author-email: skinport.py@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skinport.py-0.8.0/skinport.py.egg-info/SOURCES.txt` & `skinport.py-0.9.0/skinport.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_client.py` & `skinport.py-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_color.py` & `skinport.py-0.9.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_item.py` & `skinport.py-0.9.0/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_sale.py` & `skinport.py-0.9.0/tests/test_sale.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_salefeed.py` & `skinport.py-0.9.0/tests/test_salefeed.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_transaction.py` & `skinport.py-0.9.0/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `skinport.py-0.8.0/tests/test_utils.py` & `skinport.py-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

