# Comparing `tmp/firefly_exchange_client-0.2.2.tar.gz` & `tmp/firefly_exchange_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.2.2.tar", last modified: Fri Apr  7 20:13:11 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.2.3.tar", last modified: Wed Apr 26 08:22:20 2023, max compression
```

## Comparing `firefly_exchange_client-0.2.2.tar` & `firefly_exchange_client-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.049288 firefly_exchange_client-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.049288 firefly_exchange_client-0.2.2/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    32136 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-07 20:12:59.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:13:11.053288 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 20:13:11.000000 firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.000588 firefly_exchange_client-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32136 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-26 08:22:11.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:22:20.004588 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-26 08:22:20.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 08:22:19.000000 firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.2.2/LICENSE` & `firefly_exchange_client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/PKG-INFO` & `firefly_exchange_client-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.2/README.md` & `firefly_exchange_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/pyproject.toml` & `firefly_exchange_client-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.2.2"
+version = "0.2.3"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/api_service.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/constants.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/interfaces.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/sockets.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,65 +76,68 @@
             Inputs:
                 - symbol: market symbol of market user wants global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.connection_established:
                 raise Exception("Socket connection is established, invoke socket.open()")
 
-            sio.emit('SUBSCRIBE',[
+            resp = sio.call('SUBSCRIBE',[
             {
                 "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
                 "p": symbol.value,
             },
             ])
-            return True
+            return resp["success"]
         except Exception as e:
             print("Error: ", e)
             return False
 
     async def unsubscribe_global_updates_by_symbol(self,symbol: MARKET_SYMBOLS):
         """
             Allows user to unsubscribe to global updates for the desired symbol.
                 Inputs:
                     - symbol: market symbol of market user wants to remove global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.connection_established:
                 return False 
             
-            sio.emit('UNSUBSCRIBE', [
+            resp = sio.call('UNSUBSCRIBE', [
             {
                 "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
                 "p": symbol.value,
             },
             ])
-            return True
-        except:
+
+            return resp["success"]
+        except Exception as e:
+            print(e);
             return False
 
     async def subscribe_user_update_by_token(self, parent_account: str=None, user_token: str=None):
         """
             Allows user to subscribe to their account updates.
             Inputs:
                 - parent_account(str): address of parent account. Only whitelisted 
                   sub-account can listen to its parent account position updates
                 - token(str): auth token generated when onboarding on firefly
         """
         try:
             if not self.connection_established:
                 return False
               
-            sio.emit("SUBSCRIBE", [
+            resp = sio.call("SUBSCRIBE", [
             {
                 "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
                 'pa': parent_account,
                 "t": self.token if user_token == None else user_token,
             },
             ])
-            return True
+
+            return resp["success"]
         except Exception as e:
             print(e);
             return False
 
     async def unsubscribe_user_update_by_token(self, parent_account: str=None, user_token:str=None): 
         """
             Allows user to unsubscribe to their account updates.
@@ -142,20 +145,20 @@
                 - parent_account(str): address of parent account. Only for sub-accounts
                 - token: auth token generated when onboarding on firefly
         """
         try:
             if not self.connection_established:
                 return False
               
-            sio.emit("UNSUBSCRIBE", [
+            resp = sio.call("UNSUBSCRIBE", [
             {
                 "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
                 'pa': parent_account,
                 "t": self.token if user_token == None else user_token,
             },
             ])
-            return True
+            return resp["success"]
         except:
             return False
```

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.2.2/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.2.3/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

