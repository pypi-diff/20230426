# Comparing `tmp/rivian-python-client-0.1.9.tar.gz` & `tmp/rivian-python-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian-python-client-0.1.9.tar", max compression
+gzip compressed data, was "rivian-python-client-0.2.0.tar", max compression
```

## Comparing `rivian-python-client-0.1.9.tar` & `rivian-python-client-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      325 2023-02-10 02:57:09.893996 rivian-python-client-0.1.9/README.md
--rw-r--r--   0        0        0      555 2023-02-10 02:57:09.893996 rivian-python-client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      102 2023-02-10 02:57:09.893996 rivian-python-client-0.1.9/src/rivian/__init__.py
--rw-r--r--   0        0        0      519 2023-02-10 02:57:09.893996 rivian-python-client-0.1.9/src/rivian/exceptions.py
--rw-r--r--   0        0        0    21774 2023-02-10 02:57:09.893996 rivian-python-client-0.1.9/src/rivian/rivian.py
--rw-r--r--   0        0        0     1045 2023-02-10 02:57:36.376173 rivian-python-client-0.1.9/setup.py
--rw-r--r--   0        0        0      832 2023-02-10 02:57:36.376491 rivian-python-client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/README.md
+-rw-r--r--   0        0        0      555 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/src/rivian/__init__.py
+-rw-r--r--   0        0        0     2888 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/const.py
+-rw-r--r--   0        0        0      779 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/exceptions.py
+-rw-r--r--   0        0        0    24357 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/rivian.py
+-rw-r--r--   0        0        0     6962 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0     1045 2023-04-26 14:26:36.278962 rivian-python-client-0.2.0/setup.py
+-rw-r--r--   0        0        0      832 2023-04-26 14:26:36.279379 rivian-python-client-0.2.0/PKG-INFO
```

### Comparing `rivian-python-client-0.1.9/src/rivian/rivian.py` & `rivian-python-client-0.2.0/src/rivian/rivian.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,57 @@
 """Asynchronous Python client for the Rivian API."""
 from __future__ import annotations
 
-from typing import Any
-
 import asyncio
 import json
+import logging
 import socket
-import random
 import uuid
-
-import logging
+from collections.abc import Callable
+from typing import Any
 
 import aiohttp
 import async_timeout
-from yarl import URL
+from aiohttp import ClientRequest, ClientResponse, ClientWebSocketResponse
 
-from rivian.exceptions import *
+from .const import VEHICLE_STATE_PROPERTIES
+from .exceptions import (
+    RivianApiException,
+    RivianApiRateLimitError,
+    RivianDataError,
+    RivianExpiredTokenError,
+    RivianInvalidCredentials,
+    RivianInvalidOTP,
+    RivianTemporarilyLockedError,
+    RivianUnauthenticated,
+)
+from .ws_monitor import WebSocketMonitor
 
 _LOGGER = logging.getLogger(__name__)
 
 CESIUM_BASEPATH = "https://cesium.rivianservices.com/v2"
 AUTH_BASEPATH = "https://auth.rivianservices.com/auth/api/v1"
 GRAPHQL_BASEPATH = "https://rivian.com/api/gql"
 GRAPHQL_GATEWAY = GRAPHQL_BASEPATH + "/gateway/graphql"
 GRAPHQL_CHARGING = GRAPHQL_BASEPATH + "/chrg/user/graphql"
+GRAPHQL_WEBSOCKET = "wss://api.rivian.com/gql-consumer-subscriptions/graphql"
+
+APOLLO_CLIENT_NAME = "com.rivian.ios.consumer-apollo-ios"
 
 BASE_HEADERS = {
     "User-Agent": "RivianApp/707 CFNetwork/1237 Darwin/20.4.0",
     "Accept": "application/json",
     "Content-Type": "application/json",
-    "Apollographql-Client-Name": "com.rivian.ios.consumer-apollo-ios",
+    "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
 }
 
+LOCATION_TEMPLATE = "{ latitude longitude timeStamp }"
+VALUE_TEMPLATE = "{ timeStamp value }"
+TEMPLATE_MAP = {"gnssLocation": LOCATION_TEMPLATE}
+
 
 class Rivian:
     """Main class for the Rivian API Client"""
 
     def __init__(
         self,
         client_id: str,
@@ -44,33 +60,37 @@
         session: aiohttp.client.ClientSession | None = None,
     ) -> None:
         self._session = session
         self._close_session = False
         self._session_token = ""
         self._access_token = ""
         self._refresh_token = ""
+        self._csrf_token = ""
         self._app_session_token = ""
         self._user_session_token = ""
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.request_timeout = request_timeout
 
         self._otp_needed = False
         self._otp_token = ""
 
+        self._ws_monitor: WebSocketMonitor | None = None
+        self._subscriptions: dict[str, str] = {}
+
     async def authenticate(
         self,
         username: str,
         password: str,
-    ) -> ClientRequest:
+    ) -> ClientResponse | dict[str, str]:
         """Authenticate against the Rivian API with Username and Password"""
         url = url = AUTH_BASEPATH + "/token/auth"
 
-        headers = dict()
+        headers = {}
         headers.update(BASE_HEADERS)
 
         json_data = {
             "grant_type": "password",
             "username": username,
             "client_id": self.client_id,
             "client_secret": self.client_secret,
@@ -336,21 +356,21 @@
         username: str,
         password: str,
     ) -> dict[str, Any]:
         """Authenticate against the Rivian GraphQL API with Username and Password"""
 
         url = GRAPHQL_GATEWAY
 
-        headers = dict()
+        headers = {}
         headers.update(BASE_HEADERS)
         headers.update(
             {
                 "Csrf-Token": self._csrf_token,
                 "A-Sess": self._app_session_token,
-                "Apollographql-Client-Name": "com.rivian.ios.consumer-apollo-ios",
+                "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
                 "Dc-Cid": f"m-ios-{uuid.uuid4()}",
             }
         )
 
         graphql_json = {
             "operationName": "Login",
             "query": "mutation Login($email: String!, $password: String!) {\n  login(email: $email, password: $password) {\n    __typename\n    ... on MobileLoginResponse {\n      __typename\n      accessToken\n      refreshToken\n      userSessionToken\n    }\n    ... on MobileMFALoginResponse {\n      __typename\n      otpToken\n    }\n  }\n}",
@@ -380,15 +400,15 @@
 
         headers = dict()
         headers.update(BASE_HEADERS)
         headers.update(
             {
                 "Csrf-Token": self._csrf_token,
                 "A-Sess": self._app_session_token,
-                "Apollographql-Client-Name": "com.rivian.ios.consumer-apollo-ios",
+                "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
             }
         )
 
         graphql_json = {
             "operationName": "LoginWithOTP",
             "query": "mutation LoginWithOTP($email: String!, $otpCode: String!, $otpToken: String!) {\n  loginWithOTP(email: $email, otpCode: $otpCode, otpToken: $otpToken) {\n    __typename\n    ... on MobileLoginResponse {\n      __typename\n      accessToken\n      refreshToken\n      userSessionToken\n    }\n  }\n}",
             "variables": {
@@ -446,39 +466,26 @@
             "operationName": "getRegisteredWallboxes",
             "query": "query getRegisteredWallboxes {\n  getRegisteredWallboxes {\n    __typename\n    wallboxId\n    userId\n    wifiId\n    name\n    linked\n    latitude\n    longitude\n    chargingStatus\n    power\n    currentVoltage\n    currentAmps\n    softwareVersion\n    model\n    serialNumber\n    maxAmps\n    maxVoltage\n    maxPower\n  }\n}",
             "variables": None,
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
-    async def get_vehicle_state(
-        self, vin: str, properties: dict[str]
-    ) -> ClientResponse:
+    async def get_vehicle_state(self, vin: str, properties: set[str]) -> ClientResponse:
         """get vehicle state (graphql)"""
         url = GRAPHQL_GATEWAY
 
-        headers = dict()
+        headers = {}
         headers.update(BASE_HEADERS)
         headers.update(
             {"A-Sess": self._app_session_token, "U-Sess": self._user_session_token}
         )
 
-        graphql_query = "query GetVehicleState($vehicleID: String!) {\n  vehicleState(id: $vehicleID) {\n    "
-        gnss_attribute_template = (
-            "{\n      latitude\n      longitude\n      timeStamp\n    }\n"
-        )
-        generic_sensor_template = "{\n      timeStamp\n      value\n    }\n"
-
-        for key in properties:
-            template = generic_sensor_template
-            if key == "gnssLocation":
-                template = gnss_attribute_template
-
-            graphql_query += f"{key} {template}"
-        graphql_query += "}"
+        graphql_query = "query GetVehicleState($vehicleID: String!) {\n  vehicleState(id: $vehicleID) "
+        graphql_query += self._build_vehicle_state_fragment(properties)
         graphql_query += "}"
 
         graphql_json = {
             "operationName": "GetVehicleState",
             "query": graphql_query,
             "variables": {"vehicleID": vin},
         }
@@ -520,14 +527,66 @@
             "operationName": "getLiveSessionData",
             "query": graphql_query,
             "variables": {"userId": user_id, "vehicleId": vin},
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
+    async def subscribe_for_vehicle_updates(
+        self,
+        vin: str,
+        properties: set[str] | None = None,
+        callback: Callable = None,
+    ) -> Callable | None:
+        """Open a web socket connection to receive updates."""
+        if not properties:
+            properties = VEHICLE_STATE_PROPERTIES
+
+        try:
+            await self._ws_connect()
+            async with async_timeout.timeout(self.request_timeout):
+                await self._ws_monitor.connection_ack.wait()
+            payload = {
+                "operationName": "VehicleState",
+                "query": f"subscription VehicleState($vehicleID: String!) {{ vehicleState(id: $vehicleID) {self._build_vehicle_state_fragment(properties)} }}",
+                "variables": {"vehicleID": vin},
+            }
+            unsubscribe = await self._ws_monitor.start_subscription(payload, callback)
+            _LOGGER.debug("%s subscribed to updates", vin)
+            return unsubscribe
+        except Exception as ex:  # pylint: disable=broad-except
+            _LOGGER.error(ex)
+
+    async def _ws_connect(self) -> ClientWebSocketResponse:
+        """Initiate a websocket connection."""
+
+        async def connection_init(websocket: ClientWebSocketResponse) -> None:
+            await websocket.send_json(
+                {
+                    "payload": {
+                        "client-name": APOLLO_CLIENT_NAME,
+                        "client-version": "1.13.0-1494",
+                        "dc-cid": f"m-ios-{uuid.uuid4()}",
+                        "u-sess": self._user_session_token,
+                    },
+                    "type": "connection_init",
+                }
+            )
+
+        if not self._ws_monitor:
+            self._ws_monitor = WebSocketMonitor(
+                self, GRAPHQL_WEBSOCKET, connection_init
+            )
+        ws_monitor = self._ws_monitor
+        if ws_monitor.websocket is None or ws_monitor.websocket.closed:
+            await ws_monitor.new_connection(True)
+        if ws_monitor.monitor is None or ws_monitor.monitor.done():
+            await ws_monitor.start_monitor()
+        return ws_monitor.websocket
+
     async def __graphql_query(self, headers: dict(str, str), url: str, body: str):
         """execute and return arbitrary graphql query"""
         if self._session is None:
             self._session = aiohttp.ClientSession()
             self._close_session = True
 
         try:
@@ -535,79 +594,70 @@
                 response = await self._session.request(
                     "POST",
                     url,
                     json=body,
                     headers=headers,
                 )
         except asyncio.TimeoutError as exception:
-            raise Exception(
+            raise RivianApiException(
                 "Timeout occurred while connecting to Rivian API."
             ) from exception
         except (aiohttp.ClientError, socket.gaierror) as exception:
-            raise Exception(
+            raise RivianApiException(
                 "Error occurred while communicating with Rivian."
             ) from exception
 
         try:
             response_json = await response.json()
-            if "errors" in response_json:
-                for e in response_json["errors"]:
-                    extensions = e["extensions"]
-                    if extensions["code"] == "UNAUTHENTICATED":
+            if errors := response_json.get("errors"):
+                for error in errors:
+                    extensions = error["extensions"]
+                    if (code := extensions["code"]) == "UNAUTHENTICATED":
                         raise RivianUnauthenticated(
-                            response.status,
-                            response_json,
-                            headers,
-                            body,
+                            response.status, response_json, headers, body
                         )
-                    elif extensions["code"] == "DATA_ERROR":
+                    if code == "DATA_ERROR":
                         raise RivianDataError(
-                            response.status,
-                            response_json,
-                            headers,
-                            body,
+                            response.status, response_json, headers, body
                         )
-                    elif extensions["code"] == "BAD_CURRENT_PASSWORD":
+                    if code == "BAD_CURRENT_PASSWORD":
                         raise RivianInvalidCredentials(
-                            response.status,
-                            response_json,
-                            headers,
-                            body,
+                            response.status, response_json, headers, body
                         )
-                    elif (
-                        extensions["code"] == "BAD_USER_INPUT"
+                    if (
+                        code == "BAD_USER_INPUT"
                         and extensions["reason"] == "INVALID_OTP"
                     ):
                         raise RivianInvalidOTP(
-                            response.status,
-                            response_json,
-                            headers,
-                            body,
+                            response.status, response_json, headers, body
                         )
-                    elif extensions["code"] == "SESSION_MANAGER_ERROR":
+                    if code == "SESSION_MANAGER_ERROR":
                         raise RivianTemporarilyLockedError(
-                            response.status,
-                            response_json,
-                            headers,
-                            body,
+                            response.status, response_json, headers, body
                         )
-                raise Exception(
+                    if code == "RATE_LIMIT":
+                        raise RivianApiRateLimitError(
+                            response.status, response_json, headers, body
+                        )
+                raise RivianApiException(
                     "Error occurred while reading the graphql response from Rivian.",
                     response.status,
                     response_json,
                     headers,
                     body,
                 )
         except Exception as exception:
             raise exception
 
         return response
 
     async def close(self) -> None:
         """Close open client session."""
+        if self._ws_monitor:
+            await self._ws_monitor.close()
         if self._session and self._close_session:
             await self._session.close()
 
     async def __aenter__(self) -> Rivian:
         """Async enter.
         Returns:
             The Rivian object.
@@ -616,7 +666,12 @@
 
     async def __aexit__(self, *_exc_info) -> None:
         """Async exit.
         Args:
             _exc_info: Exec type.
         """
         await self.close()
+
+    def _build_vehicle_state_fragment(self, properties: set[str]) -> str:
+        """Build GraphQL vehicle state fragment from properties."""
+        frag = " ".join(f"{p} {TEMPLATE_MAP.get(p,VALUE_TEMPLATE)}" for p in properties)
+        return f"{{ {frag} }}"
```

### Comparing `rivian-python-client-0.1.9/setup.py` & `rivian-python-client-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0.0', 'yarl>=1.6.0']
 
 setup_kwargs = {
     'name': 'rivian-python-client',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Rivian API Client (Unofficial)',
     'long_description': '# Python: Rivian API Client\n\nCurrently a Work In Progress\n\n## Dependencies\n\n[Poetry](https://python-poetry.org/docs/)\n\n```\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\n## Setup\n\nInstall project dependencies into the poetry virtual environment.\n\n```\npoetry install\n```\n\n## Run Tests\n\n```\npoetry run pytest\n```\n',
     'author': 'Brian Retterer',
     'author_email': 'bretterer@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `rivian-python-client-0.1.9/PKG-INFO` & `rivian-python-client-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

