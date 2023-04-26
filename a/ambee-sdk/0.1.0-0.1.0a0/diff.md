# Comparing `tmp/ambee_sdk-0.1.0.tar.gz` & `tmp/ambee_sdk-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambee_sdk-0.1.0.tar", last modified: Tue Apr 25 21:59:18 2023, max compression
+gzip compressed data, was "ambee_sdk-0.1.0a0.tar", last modified: Mon Mar 20 14:25:18 2023, max compression
```

## Comparing `ambee_sdk-0.1.0.tar` & `ambee_sdk-0.1.0a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-04-25 21:59:18.485622 ambee_sdk-0.1.0/
--rwxr-xr-x   0 ambee      (501) staff       (20)     1062 2023-03-01 05:42:50.000000 ambee_sdk-0.1.0/LICENSE
--rw-r--r--   0 ambee      (501) staff       (20)     1617 2023-04-25 21:59:18.485517 ambee_sdk-0.1.0/PKG-INFO
--rwxr-xr-x   0 ambee      (501) staff       (20)     1145 2023-03-20 14:22:23.000000 ambee_sdk-0.1.0/README.md
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-04-25 21:59:18.484748 ambee_sdk-0.1.0/ambee_sdk/
--rwxr-xr-x   0 ambee      (501) staff       (20)       25 2023-03-02 06:32:50.000000 ambee_sdk-0.1.0/ambee_sdk/__init__.py
--rwxr-xr-x   0 ambee      (501) staff       (20)    43594 2023-04-25 21:58:20.000000 ambee_sdk-0.1.0/ambee_sdk/ambee_sdk.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-04-25 21:59:18.485376 ambee_sdk-0.1.0/ambee_sdk.egg-info/
--rwxr-xr-x   0 ambee      (501) staff       (20)     1617 2023-04-25 21:59:18.000000 ambee_sdk-0.1.0/ambee_sdk.egg-info/PKG-INFO
--rwxr-xr-x   0 ambee      (501) staff       (20)      235 2023-04-25 21:59:18.000000 ambee_sdk-0.1.0/ambee_sdk.egg-info/SOURCES.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)        1 2023-04-25 21:59:18.000000 ambee_sdk-0.1.0/ambee_sdk.egg-info/dependency_links.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)       26 2023-04-25 21:59:18.000000 ambee_sdk-0.1.0/ambee_sdk.egg-info/requires.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)       10 2023-04-25 21:59:18.000000 ambee_sdk-0.1.0/ambee_sdk.egg-info/top_level.txt
--rw-r--r--   0 ambee      (501) staff       (20)       38 2023-04-25 21:59:18.485662 ambee_sdk-0.1.0/setup.cfg
--rwxr-xr-x   0 ambee      (501) staff       (20)      938 2023-04-25 21:43:27.000000 ambee_sdk-0.1.0/setup.py
+drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)     1062 2023-03-01 05:42:50.000000 ambee_sdk-0.1.0a0/LICENSE
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)     1619 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/PKG-INFO
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)     1145 2023-03-20 14:22:23.000000 ambee_sdk-0.1.0a0/README.md
+drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/ambee_sdk/
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)       25 2023-03-02 06:32:50.000000 ambee_sdk-0.1.0a0/ambee_sdk/__init__.py
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)    43276 2023-03-09 08:26:46.000000 ambee_sdk-0.1.0a0/ambee_sdk/ambee_sdk.py
+drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)     1619 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)      235 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)        1 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)       26 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)       10 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)       38 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/setup.cfg
+-rw-rw-r--   0 ambee     (1000) ambee     (1000)      939 2023-03-09 04:15:39.000000 ambee_sdk-0.1.0a0/setup.py
```

### Comparing `ambee_sdk-0.1.0/LICENSE` & `ambee_sdk-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ambee_sdk-0.1.0/PKG-INFO` & `ambee_sdk-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambee_sdk
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Python SDK for Ambee's APIs
 Home-page: 
 Author: Ambee
 License: MIT
 Keywords: ambee climate environment pollen air-quality weather api sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ambee_sdk-0.1.0/README.md` & `ambee_sdk-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `ambee_sdk-0.1.0/ambee_sdk/ambee_sdk.py` & `ambee_sdk-0.1.0a0/ambee_sdk/ambee_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,17 +391,15 @@
                     print(response.status_code)
                     raise e
 
 
 class pollen(ambee):
     """Contains methods to fetch data from Pollen API"""
 
-    def get_latest(
-        self, by, lat=None, lng=None, place=None, speciesRisk=False, return_df=False
-    ):
+    def get_latest(self, by, lat=None, lng=None, place=None, return_df=False):
         """Retrives latest pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             lat (float/int/str, optional): Latitude. Defaults to None.
             lng (float/int/str, optional): Longitude. Defaults to None.
             place (str, optional): Placename. Defaults to None.
@@ -420,16 +418,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/latest/pollen/by-lat-lng?lat={}&lng={}&speciesRisk={}".format(
-                            lat, lng, speciesRisk
+                        "https://api.ambeedata.com/latest/pollen/by-lat-lng?lat={}&lng={}".format(
+                            lat, lng
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
@@ -447,16 +445,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/latest/pollen/by-place?place={}&speciesRisk={}".format(
-                            place, speciesRisk
+                        "https://api.ambeedata.com/latest/pollen/by-place?place={}".format(
+                            place
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
@@ -466,23 +464,15 @@
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
     def get_historical(
-        self,
-        by,
-        from_val,
-        to_val,
-        lat=None,
-        lng=None,
-        place=None,
-        speciesRisk=False,
-        return_df=False,
+        self, by, from_val, to_val, lat=None, lng=None, place=None, return_df=False
     ):
         """Retrives historical pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             from_val (str): Start timestamp for historical query
             to_val (_type_): End timestamp for historical query
@@ -504,16 +494,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/history/pollen/by-lat-lng?lat={}&lng={}&from={}&to={}&speciesRisk={}".format(
-                            lat, lng, from_val, to_val, speciesRisk
+                        "https://api.ambeedata.com/history/pollen/by-lat-lng?lat={}&lng={}&from={}&to={}".format(
+                            lat, lng, from_val, to_val
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
@@ -531,16 +521,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/history/pollen/by-place?place={}&from={}&to={}&speciesRisk={}".format(
-                            place, from_val, to_val, speciesRisk
+                        "https://api.ambeedata.com/history/pollen/by-place?place={}&from={}&to={}".format(
+                            place, from_val, to_val
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
@@ -549,17 +539,15 @@
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
-    def get_forecast(
-        self, by, lat=None, lng=None, place=None, speciesRisk=False, return_df=False
-    ):
+    def get_forecast(self, by, lat=None, lng=None, place=None, return_df=False):
         """Retrives forecasted pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             lat (float/int/str, optional): Latitude. Defaults to None.
             lng (float/int/str, optional): Longitude. Defaults to None.
             place (str, optional): Placename. Defaults to None.
@@ -578,16 +566,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/forecast/pollen/by-lat-lng?lat={}&lng={}&speciesRisk={}".format(
-                            lat, lng, speciesRisk
+                        "https://api.ambeedata.com/forecast/pollen/by-lat-lng?lat={}&lng={}".format(
+                            lat, lng
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
@@ -605,16 +593,16 @@
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     response = requests.get(
-                        "https://api.ambeedata.com/forecast/pollen/by-place?place={}&speciesRisk={}".format(
-                            place, speciesRisk
+                        "https://api.ambeedata.com/forecast/pollen/by-place?place={}".format(
+                            place
                         ),
                         headers=headers,
                     )
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
```

### Comparing `ambee_sdk-0.1.0/ambee_sdk.egg-info/PKG-INFO` & `ambee_sdk-0.1.0a0/ambee_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambee-sdk
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Python SDK for Ambee's APIs
 Home-page: 
 Author: Ambee
 License: MIT
 Keywords: ambee climate environment pollen air-quality weather api sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ambee_sdk-0.1.0/setup.py` & `ambee_sdk-0.1.0a0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name="ambee_sdk",
     packages=find_packages(include=["ambee_sdk"]),
-    version="0.1.0",
+    version="0.1.0a",
     author="Ambee",
     license="MIT",
     url='',
     description="Python SDK for Ambee's APIs",
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[ "requests", "pandas", "geopandas"
```

