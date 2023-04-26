# Comparing `tmp/audiconnectpy-1.3.1.tar.gz` & `tmp/audiconnectpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.1.tar", last modified: Tue Apr 25 06:27:56 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.2.tar", last modified: Wed Apr 26 06:33:49 2023, max compression
```

## Comparing `audiconnectpy-1.3.1.tar` & `audiconnectpy-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22748 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-25 06:27:55.000000 audiconnectpy-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22874 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30468 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 06:33:49.000000 audiconnectpy-1.3.2/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 06:33:48.000000 audiconnectpy-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:49.872015 audiconnectpy-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 06:33:37.000000 audiconnectpy-1.3.2/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.1/LICENSE` & `audiconnectpy-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/PKG-INFO` & `audiconnectpy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.1/README.md` & `audiconnectpy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/audiconnectpy/api.py` & `audiconnectpy-1.3.2/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/audiconnectpy/auth.py` & `audiconnectpy-1.3.2/audiconnectpy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,31 +126,34 @@
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
 
     async def get(self, url: str, **kwargs: Any) -> Any:
         """GET request."""
-        headers = kwargs.pop("headers", await self.async_get_headers(token_type="mbb"))
+        if (headers := kwargs.pop("headers", None)) is None:
+            headers = await self.async_get_headers(token_type="mbb")
         response = await self.request(METH_GET, url, headers=headers, **kwargs)
         return response
 
     async def put(self, url: str, data: Any = None, **kwargs: Any) -> Any:
         """PUT request."""
-        headers = kwargs.pop("headers", await self.async_get_headers(token_type="mbb"))
+        if (headers := kwargs.pop("headers", None)) is None:
+            headers = await self.async_get_headers(token_type="mbb")
         response = await self.request(
             METH_PUT, url, headers=headers, data=data, **kwargs
         )
         return response
 
     async def post(
         self, url: str, data: Any = None, use_json: bool = True, **kwargs: Any
     ) -> Any:
         """POST request."""
-        headers = kwargs.pop("headers", await self.async_get_headers(token_type="mbb"))
+        if (headers := kwargs.pop("headers", None)) is None:
+            headers = await self.async_get_headers(token_type="mbb")
         if use_json and data:
             data = json.dumps(data)
         response = await self.request(
             METH_POST, url, headers=headers, data=data, **kwargs
         )
         return response
 
@@ -418,15 +421,15 @@
 
         headers = await self.async_get_headers(token_type="mbb", headers=headers)
 
         return headers
 
     async def async_get_headers(
         self,
-        token_type: Literal["idk", "mbb", "audi", "no"] = "idk",
+        token_type: Literal["idk", "mbb", "audi"] | None = None,
         headers: dict[str, Any] | None = None,
         okhttp: bool = False,
         security_token: str | None = None,
     ) -> dict[str, str]:
         """Get simple headers."""
         defaults = {
             "Accept": "application/json",
```

### Comparing `audiconnectpy-1.3.1/audiconnectpy/models.py` & `audiconnectpy-1.3.2/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/audiconnectpy/services.py` & `audiconnectpy-1.3.2/audiconnectpy/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             f"{url}/bs/departuretimer/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/timer"
         )
         return data
 
     async def async_get_capabilities(self, vin: str) -> VehicleDataResponse:
         """Get capabilities."""
         url = "https://emea.bff.cariad.digital"
-        headers = await self._auth.async_get_headers()
+        headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(
             f"{url}/vehicle/v1/vehicles/{vin.upper()}/capabilities", headers=headers
         )
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_get_vehicle_information(self) -> Any:
         """Get vehicle information."""
@@ -238,43 +238,43 @@
             f"{url}/bs/rhf/v1/{self.brand}/{self.country}/configuration"
         )
         return data
 
     async def async_get_personal_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
-        headers = await self._auth.async_get_headers()
+        headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/personalData", headers=headers)
         return data
 
     async def async_get_real_car_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
-        headers = await self._auth.async_get_headers()
+        headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/realCarData", headers=headers)
         return data
 
     async def async_get_mbb_status(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
-        headers = await self._auth.async_get_headers()
+        headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/mbbStatusData", headers=headers)
         return data
 
     async def async_get_identity_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
-        headers = await self._auth.async_get_headers()
+        headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/identityData", headers=headers)
         return data
 
     # async def async_get_users(self, vin: str) -> Any:
     #     """Get users."""
     #     url = "https://userinformationservice.apps.emea.vwapps.io/iaa"
-    #     headers = await self._auth.async_get_headers()
+    #     headers = await self._auth.async_get_headers(token_type="idk")
     #     data = await self._auth.get(f"{url}/uic/v1/vin/{vin.upper()}/users", headers=headers)
     #     return data
 
     async def async_get_fences(self, vin: str) -> Any:
         """Get fences."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
@@ -309,14 +309,15 @@
     async def async_lock(self, vin: str, lock: bool) -> None:
         """Set lock."""
         # OpenHab "lock","unlock"
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
         data += f'<rluAction xmlns="http://audi.de/connect/rlu"><action>{"lock" if lock else "unlock"}</action></rluAction>'
         headers = await self._auth.async_get_headers(
+            token_type="idk",
             headers={
                 "Content-Type": "application/vnd.vwg.mbb.RemoteLockUnlock_v1_0_0+xml"
             },
             security_token=await self._async_get_security_token(
                 vin, "rlu_v1/operations/" + ("LOCK" if lock else "UNLOCK")
             ),
         )
```

### Comparing `audiconnectpy-1.3.1/audiconnectpy/util.py` & `audiconnectpy-1.3.2/audiconnectpy/util.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.2/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.1/pyproject.toml` & `audiconnectpy-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.1/setup.py` & `audiconnectpy-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.1",
+    version="1.3.2",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

