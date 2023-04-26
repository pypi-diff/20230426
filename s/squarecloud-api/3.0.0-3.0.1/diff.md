# Comparing `tmp/squarecloud-api-3.0.0.tar.gz` & `tmp/squarecloud-api-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squarecloud-api-3.0.0.tar", last modified: Tue Apr 25 18:13:07 2023, max compression
+gzip compressed data, was "squarecloud-api-3.0.1.tar", last modified: Wed Apr 26 13:58:49 2023, max compression
```

## Comparing `squarecloud-api-3.0.0.tar` & `squarecloud-api-3.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:13:07.135228 squarecloud-api-3.0.0/
--rw-rw-rw-   0        0        0     1100 2022-09-15 13:56:18.000000 squarecloud-api-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     1725 2023-04-25 18:13:07.134231 squarecloud-api-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1394 2023-04-25 18:10:48.000000 squarecloud-api-3.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 18:13:07.135228 squarecloud-api-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      644 2023-04-21 17:39:22.000000 squarecloud-api-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:13:06.941611 squarecloud-api-3.0.0/squarecloud/
--rw-rw-rw-   0        0        0      135 2023-01-15 14:59:14.000000 squarecloud-api-3.0.0/squarecloud/__init__.py
--rw-rw-rw-   0        0        0    11409 2023-04-25 17:06:44.000000 squarecloud-api-3.0.0/squarecloud/app.py
--rw-rw-rw-   0        0        0    16806 2023-04-25 18:00:46.000000 squarecloud-api-3.0.0/squarecloud/client.py
--rw-rw-rw-   0        0        0     2138 2023-04-24 16:39:47.000000 squarecloud-api-3.0.0/squarecloud/data.py
--rw-rw-rw-   0        0        0      841 2023-01-12 00:11:44.000000 squarecloud-api-3.0.0/squarecloud/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:13:06.965555 squarecloud-api-3.0.0/squarecloud/http/
--rw-rw-rw-   0        0        0       80 2023-01-15 14:59:14.000000 squarecloud-api-3.0.0/squarecloud/http/__init__.py
--rw-rw-rw-   0        0        0     4894 2023-04-24 17:22:57.000000 squarecloud-api-3.0.0/squarecloud/http/endpoints.py
--rw-rw-rw-   0        0        0     8964 2023-04-25 16:40:32.000000 squarecloud-api-3.0.0/squarecloud/http/http_client.py
--rw-rw-rw-   0        0        0     2097 2023-01-15 21:56:11.000000 squarecloud-api-3.0.0/squarecloud/listener.py
--rw-rw-rw-   0        0        0     1059 2023-04-19 13:56:14.000000 squarecloud-api-3.0.0/squarecloud/logs.py
--rw-rw-rw-   0        0        0     1014 2023-04-24 16:29:39.000000 squarecloud-api-3.0.0/squarecloud/payloads.py
--rw-rw-rw-   0        0        0      459 2023-04-19 18:40:12.000000 squarecloud-api-3.0.0/squarecloud/square.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:13:07.127248 squarecloud-api-3.0.0/squarecloud_api.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 13:58:49.203170 squarecloud-api-3.0.1/
+-rw-rw-rw-   0        0        0     1100 2022-09-15 13:56:18.000000 squarecloud-api-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-04-26 13:58:49.202173 squarecloud-api-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2023-04-25 18:10:48.000000 squarecloud-api-3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 13:58:49.203170 squarecloud-api-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      644 2023-04-26 13:58:36.000000 squarecloud-api-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:58:49.111417 squarecloud-api-3.0.1/squarecloud/
+-rw-rw-rw-   0        0        0      135 2023-01-15 14:59:14.000000 squarecloud-api-3.0.1/squarecloud/__init__.py
+-rw-rw-rw-   0        0        0    11052 2023-04-25 18:55:49.000000 squarecloud-api-3.0.1/squarecloud/app.py
+-rw-rw-rw-   0        0        0    16822 2023-04-26 13:29:58.000000 squarecloud-api-3.0.1/squarecloud/client.py
+-rw-rw-rw-   0        0        0     2180 2023-04-26 13:56:48.000000 squarecloud-api-3.0.1/squarecloud/data.py
+-rw-rw-rw-   0        0        0      841 2023-01-12 00:11:44.000000 squarecloud-api-3.0.1/squarecloud/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:58:49.154301 squarecloud-api-3.0.1/squarecloud/http/
+-rw-rw-rw-   0        0        0       80 2023-01-15 14:59:14.000000 squarecloud-api-3.0.1/squarecloud/http/__init__.py
+-rw-rw-rw-   0        0        0     4894 2023-04-24 17:22:57.000000 squarecloud-api-3.0.1/squarecloud/http/endpoints.py
+-rw-rw-rw-   0        0        0     8964 2023-04-25 16:40:32.000000 squarecloud-api-3.0.1/squarecloud/http/http_client.py
+-rw-rw-rw-   0        0        0     2097 2023-01-15 21:56:11.000000 squarecloud-api-3.0.1/squarecloud/listener.py
+-rw-rw-rw-   0        0        0     1059 2023-04-19 13:56:14.000000 squarecloud-api-3.0.1/squarecloud/logs.py
+-rw-rw-rw-   0        0        0     1014 2023-04-24 16:29:39.000000 squarecloud-api-3.0.1/squarecloud/payloads.py
+-rw-rw-rw-   0        0        0      459 2023-04-19 18:40:12.000000 squarecloud-api-3.0.1/squarecloud/square.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:58:49.200178 squarecloud-api-3.0.1/squarecloud_api.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-04-26 13:58:48.000000 squarecloud-api-3.0.1/squarecloud_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-04-26 13:58:48.000000 squarecloud-api-3.0.1/squarecloud_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 13:58:48.000000 squarecloud-api-3.0.1/squarecloud_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-26 13:58:48.000000 squarecloud-api-3.0.1/squarecloud_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-26 13:58:48.000000 squarecloud-api-3.0.1/squarecloud_api.egg-info/top_level.txt
```

### Comparing `squarecloud-api-3.0.0/LICENSE` & `squarecloud-api-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/PKG-INFO` & `squarecloud-api-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarecloud-api
-Version: 3.0.0
+Version: 3.0.1
 Summary: SquareCloud API wrapper
 Home-page: UNKNOWN
 Author: Robert Nogueira
 Author-email: robertlucasnogueira@gmail.com
 License: MIT License
 Keywords: squarecloud/api/python
 Platform: UNKNOWN
```

### Comparing `squarecloud-api-3.0.0/README.md` & `squarecloud-api-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/setup.py` & `squarecloud-api-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(name=r'squarecloud-api',
-      version='3.0.0',
+      version='3.0.1',
       license='MIT License',
       author='Robert Nogueira',
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email='robertlucasnogueira@gmail.com',
       keywords='squarecloud/api/python',
       description='SquareCloud API wrapper',
```

### Comparing `squarecloud-api-3.0.0/squarecloud/app.py` & `squarecloud-api-3.0.1/squarecloud/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,7 @@
     async def delete_file(self, path: str, **kwargs):
         response: Response = await self.client.delete_app_file(self.id, path)
         if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = Endpoint.files_delete()
             await self._listener.on_capture(endpoint=endpoint,
                                             response=response)
         return response
-
-    async def data(self, **kwargs):
-        response: AppData = await self.client.app_data(self.id)
-        if not kwargs.get('avoid_listener'):
-            endpoint: Endpoint = Endpoint.app_data()
-            await self._listener.on_capture(endpoint=endpoint,
-                                            response=response)
-        return response
```

### Comparing `squarecloud-api-3.0.0/squarecloud/client.py` & `squarecloud-api-3.0.1/squarecloud/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def create_config_file(
         path: str,
         display_name: str,
         main: str,
         memory: int,
-        version: Literal['recommended', 'latest'],
+        version: Literal['recommended', 'latest'] = 'recommended',
         avatar: str | None = None,
         description: str | None = None,
         subdomain: str | None = None,
         start: str | None = None,
         auto_restart: bool | None = None,
 ):
     """
```

### Comparing `squarecloud-api-3.0.0/squarecloud/data.py` & `squarecloud-api-3.0.1/squarecloud/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,35 +53,35 @@
         'java',
         'rust',
         'go',
         'static',
         'dynamic',
     ]
     cluster: Literal['free-', 'florida-1']
-    domain: str | None
-    custom: str | None
     isWebsite: bool
     gitIntegration: bool
+    domain: str | None = None
+    custom: str | None = None
 
 
 @dataclass
 class UserData:
     """user data class"""
     id: int
     tag: str
     locale: str
-    email: str | None
     plan: PlanData
     blocklist: bool
+    email: str | None = None
 
 
 @dataclass
 class LogsData:
     """logs data class"""
-    logs: str | None
+    logs: str | None = None
 
     def __eq__(self, other):
         return isinstance(other, LogsData) and self.logs == other.logs
 
 
 @dataclass
 class BackupData:
@@ -89,20 +89,20 @@
     downloadURL: str
 
 
 @dataclass
 class UploadData:
     id: str
     tag: str
-    description: str | None
     language: str
     avatar: str
-    subdomain: str | None
     ram: int
     cpu: int
+    subdomain: str | None = None
+    description: str | None = None
 
 
 @dataclass
 class FileInfo:
     type: Literal['file', 'directory']
     name: str
     size: int
```

### Comparing `squarecloud-api-3.0.0/squarecloud/errors.py` & `squarecloud-api-3.0.1/squarecloud/errors.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud/http/endpoints.py` & `squarecloud-api-3.0.1/squarecloud/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud/http/http_client.py` & `squarecloud-api-3.0.1/squarecloud/http/http_client.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud/listener.py` & `squarecloud-api-3.0.1/squarecloud/listener.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud/logs.py` & `squarecloud-api-3.0.1/squarecloud/logs.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud/payloads.py` & `squarecloud-api-3.0.1/squarecloud/payloads.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-3.0.0/squarecloud_api.egg-info/PKG-INFO` & `squarecloud-api-3.0.1/squarecloud_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarecloud-api
-Version: 3.0.0
+Version: 3.0.1
 Summary: SquareCloud API wrapper
 Home-page: UNKNOWN
 Author: Robert Nogueira
 Author-email: robertlucasnogueira@gmail.com
 License: MIT License
 Keywords: squarecloud/api/python
 Platform: UNKNOWN
```

