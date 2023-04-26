# Comparing `tmp/tonconnect-0.0.3.tar.gz` & `tmp/tonconnect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconnect-0.0.3.tar", last modified: Fri Apr 14 20:30:48 2023, max compression
+gzip compressed data, was "tonconnect-0.1.0.tar", last modified: Tue Apr 25 18:15:34 2023, max compression
```

## Comparing `tonconnect-0.0.3.tar` & `tonconnect-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.0.3/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1182 2023-04-12 09:12:00.350752 tonconnect-0.0.3/README.md
--rw-r--r--   0        0        0      288 2023-04-12 09:33:18.589470 tonconnect-0.0.3/examples/address.py
--rw-r--r--   0        0        0      552 2023-04-12 09:16:57.911646 tonconnect-0.0.3/examples/transactions.py
--rw-r--r--   0        0        0      541 2023-04-14 20:30:19.838032 tonconnect-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.0.3/tonconnect/__init__.py
--rw-r--r--   0        0        0      195 2023-04-12 07:18:49.859990 tonconnect-0.0.3/tonconnect/apps.py
--rw-r--r--   0        0        0     3709 2023-04-12 19:38:49.272910 tonconnect-0.0.3/tonconnect/bridge.py
--rw-r--r--   0        0        0     1368 2023-04-12 20:58:05.396250 tonconnect-0.0.3/tonconnect/connector.py
--rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.0.3/tonconnect/crypto.py
--rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.0.3/tonconnect/events.py
--rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.0.3/tonconnect/exceptions.py
--rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.0.3/tonconnect/options.py
--rw-r--r--   0        0        0     1745 2023-04-11 19:09:18.328616 tonconnect-0.0.3/tonconnect/requests.py
--rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.0.3/tonconnect/static.py
--rw-r--r--   0        0        0      299 2023-04-12 07:37:03.212040 tonconnect-0.0.3/tonconnect/url.py
--rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.0.3/tonconnect/utils.py
--rw-r--r--   0        0        0      361 2023-04-12 07:36:46.419499 tonconnect-0.0.3/tonconnect/wallet.py
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 tonconnect-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1783 2023-04-25 18:14:12.277674 tonconnect-0.1.0/README.md
+-rw-r--r--   0        0        0      288 2023-04-12 09:33:18.589470 tonconnect-0.1.0/examples/address.py
+-rw-r--r--   0        0        0      464 2023-04-25 17:58:46.142134 tonconnect-0.1.0/examples/async_address.py
+-rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.0/examples/transactions.py
+-rw-r--r--   0        0        0      556 2023-04-25 18:13:07.309181 tonconnect-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.0/tonconnect/__init__.py
+-rw-r--r--   0        0        0      261 2023-04-25 17:59:41.572138 tonconnect-0.1.0/tonconnect/apps.py
+-rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.0/tonconnect/bridge.py
+-rw-r--r--   0        0        0     2234 2023-04-25 17:51:46.989345 tonconnect-0.1.0/tonconnect/connector.py
+-rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.0/tonconnect/crypto.py
+-rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.1.0/tonconnect/events.py
+-rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.0/tonconnect/exceptions.py
+-rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.0/tonconnect/httpbridge.py
+-rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.0/tonconnect/options.py
+-rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.0/tonconnect/requests.py
+-rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.0/tonconnect/static.py
+-rw-r--r--   0        0        0      299 2023-04-12 07:37:03.212040 tonconnect-0.1.0/tonconnect/url.py
+-rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.0/tonconnect/utils.py
+-rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.0/tonconnect/wallet.py
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 tonconnect-0.1.0/PKG-INFO
```

### Comparing `tonconnect-0.0.3/LICENSE.md` & `tonconnect-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.3/README.md` & `tonconnect-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,30 +33,56 @@
 
 print(f'Universal connect url for Tonkeeper: {url}')
 
 address = connector.get_address()
 print(f'Successfuly connected {address}.')
 ```
 
+Example of asynchronous connecting wallet.
+
+```python
+import asyncio
+from tonconnect.connector import AsyncConnector
+
+
+async def main():
+    connector = AsyncConnector('https://tonclick.online/ton-connect.json')
+    url = await connector.connect('tonkeeper', 'test')
+
+    print(f'Universal connect url for Tonkeeper: {url}')
+
+    address = await connector.get_address()
+    print(f'Successfuly connected {address}.')
+
+
+if __name__ == '__main__':
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+```
+
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.0
+    * Async wrapper
+* 0.0.2 & 0.0.3
+    * pyproject.toml fix
 * 0.0.1
     * Initial Beta
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
 
 ## Donate
 
-If you liked the library, I will be glad to donate.
+If you like the library, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
 
 ## Acknowledgments
 
 * [ton-connect-docs](https://github.com/ton-blockchain/ton-connect)
 * [ton-connect-js-sdk](https://github.com/ton-connect/sdk)
```

### Comparing `tonconnect-0.0.3/examples/transactions.py` & `tonconnect-0.1.0/examples/transactions.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 url = connector.connect('tonkeeper', 'test')
 
 print(f'Universal connect url for Tonkeeper: {url}')
 
 address = connector.get_address()
 print(f'Successfuly connected {address}.')
 
-request = SendRequest(connector.wallet.bridge.next_id(), [SendMessage('address', 1)], time.time() + 1000, -239, 'address')
-connector.bridge.send_request(request)
+request = SendRequest(connector.wallet.bridge.next_id(), [SendMessage('0:0000000000000000000000000000000000000000000000000000000000000000', 0.000000001), SendMessage('0:0000000000000000000000000000000000000000000000000000000000000000', 0.000000001)], time.time() + 900, -239, '0:a0a61c7cad32343ee9309a0a55aa23e0aa0b93ba3850b1c83687b8e0738534b7')
+print(connector.bridge.send_request(request))
```

### Comparing `tonconnect-0.0.3/pyproject.toml` & `tonconnect-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "tonconnect"
 description = "TON Connect - Python library for using TON Connect 2."
 readme = "README.md"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
     {name = "Vlad100"}
 ]
 dependencies = [
     "pynacl",
     "requests",
-    "tonsdk"
+    "tonsdk",
+    "aiohttp"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ClickoTON-Foundation/tonconnect"
 Documentation = "https://github.com/ClickoTON-Foundation/tonconnect"
 Repository = "https://github.com/ClickoTON-Foundation/tonconnect/"
```

### Comparing `tonconnect-0.0.3/tonconnect/crypto.py` & `tonconnect-0.1.0/tonconnect/crypto.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.3/tonconnect/events.py` & `tonconnect-0.1.0/tonconnect/events.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.0.3/tonconnect/requests.py` & `tonconnect-0.1.0/tonconnect/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     
     def get_params(self):
         return {}
     
     def to_dict(self):
         params = self.get_params()
         
-        result = {'method': self.method, 'params': params, 'id': str(self.id)}
+        result = {'method': self.method, 'params': params, 'id': self.id}
         return result
 
 class SendMessage():
     def __init__(self, address: str, amount: int, payload: str = None, state_init: str = None):
         self.address = address
-        self.amount = amount * (10 ** 9)
+        self.amount = round(amount * (10 ** 9))
         self.payload = payload
         self.state_init = state_init
     
     def to_dict(self):
         result = {'address': self.address, 'amount': str(self.amount)}
         
         if self.payload is not None:
@@ -32,24 +32,23 @@
         
         return result
 
 class SendRequest(Request):
     def __init__(self, id: int, messages: list[SendMessage], valid_until: int = None, network: int = None, from_address: str = None):
         super().__init__('sendTransaction', id)
         
-        self.valid_until = round(valid_until * 1000)
+        self.valid_until = round(valid_until) * 1000
         self.network = network
         self.from_address = from_address
         self.messages = messages
     
     def get_params(self):
         params = {'messages': [message.to_dict() for message in self.messages]}
         
         if self.valid_until is not None:
-            params['valid_until'] = str(self.valid_until)
+            params['valid_until'] = self.valid_until
         if self.network is not None:
             params['network'] = str(self.network)
         if self.from_address is not None:
             params['from'] = self.from_address
         
         return [json.dumps(params)]
-
```

### Comparing `tonconnect-0.0.3/PKG-INFO` & `tonconnect-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: tonconnect
-Version: 0.0.3
+Version: 0.1.0
 Summary: TON Connect - Python library for using TON Connect 2.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: tonsdk
+Requires-Dist: aiohttp
 Project-URL: Documentation, https://github.com/ClickoTON-Foundation/tonconnect
 Project-URL: Homepage, https://github.com/ClickoTON-Foundation/tonconnect
 Project-URL: Repository, https://github.com/ClickoTON-Foundation/tonconnect/
 
 # TON Connect for Python
 
 Library for connecting TON Connect to Python apps.
@@ -46,30 +47,56 @@
 
 print(f'Universal connect url for Tonkeeper: {url}')
 
 address = connector.get_address()
 print(f'Successfuly connected {address}.')
 ```
 
+Example of asynchronous connecting wallet.
+
+```python
+import asyncio
+from tonconnect.connector import AsyncConnector
+
+
+async def main():
+    connector = AsyncConnector('https://tonclick.online/ton-connect.json')
+    url = await connector.connect('tonkeeper', 'test')
+
+    print(f'Universal connect url for Tonkeeper: {url}')
+
+    address = await connector.get_address()
+    print(f'Successfuly connected {address}.')
+
+
+if __name__ == '__main__':
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+```
+
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.0
+    * Async wrapper
+* 0.0.2 & 0.0.3
+    * pyproject.toml fix
 * 0.0.1
     * Initial Beta
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
 
 ## Donate
 
-If you liked the library, I will be glad to donate.
+If you like the library, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
 
 ## Acknowledgments
 
 * [ton-connect-docs](https://github.com/ton-blockchain/ton-connect)
 * [ton-connect-js-sdk](https://github.com/ton-connect/sdk)
```

