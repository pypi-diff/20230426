# Comparing `tmp/squarecloud-api-2.0.1.tar.gz` & `tmp/squarecloud-api-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squarecloud-api-2.0.1.tar", last modified: Mon Jan 16 13:06:54 2023, max compression
+gzip compressed data, was "squarecloud-api-3.0.0.tar", last modified: Tue Apr 25 18:13:07 2023, max compression
```

## Comparing `squarecloud-api-2.0.1.tar` & `squarecloud-api-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-16 13:06:54.799427 squarecloud-api-2.0.1/
--rw-rw-rw-   0        0        0     1100 2022-09-15 13:56:18.000000 squarecloud-api-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1431 2023-01-16 13:06:54.799427 squarecloud-api-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1100 2023-01-16 11:56:58.000000 squarecloud-api-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-01-16 13:06:54.799427 squarecloud-api-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      644 2023-01-16 13:06:24.000000 squarecloud-api-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-16 13:06:54.783773 squarecloud-api-2.0.1/squarecloud/
--rw-rw-rw-   0        0        0      135 2023-01-15 14:59:14.000000 squarecloud-api-2.0.1/squarecloud/__init__.py
--rw-rw-rw-   0        0        0     7779 2023-01-16 12:55:15.000000 squarecloud-api-2.0.1/squarecloud/app.py
--rw-rw-rw-   0        0        0    14626 2023-01-15 22:48:57.000000 squarecloud-api-2.0.1/squarecloud/client.py
--rw-rw-rw-   0        0        0     1632 2023-01-15 17:07:34.000000 squarecloud-api-2.0.1/squarecloud/data.py
--rw-rw-rw-   0        0        0      841 2023-01-12 00:11:44.000000 squarecloud-api-2.0.1/squarecloud/errors.py
-drwxrwxrwx   0        0        0        0 2023-01-16 13:06:54.783773 squarecloud-api-2.0.1/squarecloud/http/
--rw-rw-rw-   0        0        0       80 2023-01-15 14:59:14.000000 squarecloud-api-2.0.1/squarecloud/http/__init__.py
--rw-rw-rw-   0        0        0     2827 2023-01-15 12:09:16.000000 squarecloud-api-2.0.1/squarecloud/http/endpoints.py
--rw-rw-rw-   0        0        0     8066 2023-01-15 17:10:07.000000 squarecloud-api-2.0.1/squarecloud/http/http_client.py
--rw-rw-rw-   0        0        0     2097 2023-01-15 21:56:11.000000 squarecloud-api-2.0.1/squarecloud/listener.py
--rw-rw-rw-   0        0        0     1531 2023-01-15 14:59:14.000000 squarecloud-api-2.0.1/squarecloud/logs.py
--rw-rw-rw-   0        0        0     1111 2023-01-14 14:55:48.000000 squarecloud-api-2.0.1/squarecloud/payloads.py
--rw-rw-rw-   0        0        0      459 2023-01-13 17:05:22.000000 squarecloud-api-2.0.1/squarecloud/square.py
-drwxrwxrwx   0        0        0        0 2023-01-16 13:06:54.799427 squarecloud-api-2.0.1/squarecloud_api.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-01-16 13:06:54.000000 squarecloud-api-2.0.1/squarecloud_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-01-16 13:06:54.000000 squarecloud-api-2.0.1/squarecloud_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-16 13:06:54.000000 squarecloud-api-2.0.1/squarecloud_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-01-16 13:06:54.000000 squarecloud-api-2.0.1/squarecloud_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-16 13:06:54.000000 squarecloud-api-2.0.1/squarecloud_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 18:13:07.135228 squarecloud-api-3.0.0/
+-rw-rw-rw-   0        0        0     1100 2022-09-15 13:56:18.000000 squarecloud-api-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-04-25 18:13:07.134231 squarecloud-api-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2023-04-25 18:10:48.000000 squarecloud-api-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 18:13:07.135228 squarecloud-api-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      644 2023-04-21 17:39:22.000000 squarecloud-api-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:13:06.941611 squarecloud-api-3.0.0/squarecloud/
+-rw-rw-rw-   0        0        0      135 2023-01-15 14:59:14.000000 squarecloud-api-3.0.0/squarecloud/__init__.py
+-rw-rw-rw-   0        0        0    11409 2023-04-25 17:06:44.000000 squarecloud-api-3.0.0/squarecloud/app.py
+-rw-rw-rw-   0        0        0    16806 2023-04-25 18:00:46.000000 squarecloud-api-3.0.0/squarecloud/client.py
+-rw-rw-rw-   0        0        0     2138 2023-04-24 16:39:47.000000 squarecloud-api-3.0.0/squarecloud/data.py
+-rw-rw-rw-   0        0        0      841 2023-01-12 00:11:44.000000 squarecloud-api-3.0.0/squarecloud/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:13:06.965555 squarecloud-api-3.0.0/squarecloud/http/
+-rw-rw-rw-   0        0        0       80 2023-01-15 14:59:14.000000 squarecloud-api-3.0.0/squarecloud/http/__init__.py
+-rw-rw-rw-   0        0        0     4894 2023-04-24 17:22:57.000000 squarecloud-api-3.0.0/squarecloud/http/endpoints.py
+-rw-rw-rw-   0        0        0     8964 2023-04-25 16:40:32.000000 squarecloud-api-3.0.0/squarecloud/http/http_client.py
+-rw-rw-rw-   0        0        0     2097 2023-01-15 21:56:11.000000 squarecloud-api-3.0.0/squarecloud/listener.py
+-rw-rw-rw-   0        0        0     1059 2023-04-19 13:56:14.000000 squarecloud-api-3.0.0/squarecloud/logs.py
+-rw-rw-rw-   0        0        0     1014 2023-04-24 16:29:39.000000 squarecloud-api-3.0.0/squarecloud/payloads.py
+-rw-rw-rw-   0        0        0      459 2023-04-19 18:40:12.000000 squarecloud-api-3.0.0/squarecloud/square.py
+drwxrwxrwx   0        0        0        0 2023-04-25 18:13:07.127248 squarecloud-api-3.0.0/squarecloud_api.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 18:13:06.000000 squarecloud-api-3.0.0/squarecloud_api.egg-info/top_level.txt
```

### Comparing `squarecloud-api-2.0.1/LICENSE` & `squarecloud-api-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squarecloud-api-2.0.1/PKG-INFO` & `squarecloud-api-3.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarecloud-api
-Version: 2.0.1
+Version: 3.0.0
 Summary: SquareCloud API wrapper
 Home-page: UNKNOWN
 Author: Robert Nogueira
 Author-email: robertlucasnogueira@gmail.com
 License: MIT License
 Keywords: squarecloud/api/python
 Platform: UNKNOWN
@@ -32,21 +32,21 @@
 ## Getting api key
 
 to get your api key/token just go to the [SquareCloud] website and
 register/login, after that go
 to `dashboard` > `my account` > `Regenerate API/CLI KEY` and copy the key.
 
 > ## [Documentation](docs/)
-> - [application](docs/application.md)
-> - [capture_listeners](docs/capture_listeners.md)
-> - [client](docs/client.md)
-> - [commit_and_upload](docs/commit_and_upload.md)
-> - [request_listeners](docs/request_listeners.md)
+> - [application](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/application.md)
+> - [capture_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/capture_listeners.md)
+> - [client](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/client.md)
+> - [commit_and_upload](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/commit_and_upload.md)
+> - [request_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/request_listeners.md)
 
-## Basict usage
+## Basic usage
 ```python
 import squarecloud as square
 import asyncio
 
 client = square.Client('API_KEY', debug=True)
 
 async def main():
```

### Comparing `squarecloud-api-2.0.1/README.md` & `squarecloud-api-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 ## Getting api key
 
 to get your api key/token just go to the [SquareCloud] website and
 register/login, after that go
 to `dashboard` > `my account` > `Regenerate API/CLI KEY` and copy the key.
 
 > ## [Documentation](docs/)
-> - [application](docs/application.md)
-> - [capture_listeners](docs/capture_listeners.md)
-> - [client](docs/client.md)
-> - [commit_and_upload](docs/commit_and_upload.md)
-> - [request_listeners](docs/request_listeners.md)
+> - [application](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/application.md)
+> - [capture_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/capture_listeners.md)
+> - [client](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/client.md)
+> - [commit_and_upload](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/commit_and_upload.md)
+> - [request_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/request_listeners.md)
 
-## Basict usage
+## Basic usage
 ```python
 import squarecloud as square
 import asyncio
 
 client = square.Client('API_KEY', debug=True)
 
 async def main():
```

### Comparing `squarecloud-api-2.0.1/setup.py` & `squarecloud-api-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(name=r'squarecloud-api',
-      version='2.0.1',
+      version='3.0.0',
       license='MIT License',
       author='Robert Nogueira',
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email='robertlucasnogueira@gmail.com',
       keywords='squarecloud/api/python',
       description='SquareCloud API wrapper',
```

### Comparing `squarecloud-api-2.0.1/squarecloud/client.py` & `squarecloud-api-3.0.0/squarecloud/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """This module is a wrapper for using the SquareCloud API"""
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
+from io import BytesIO
 from typing import List, Literal, Any, Callable
 
 from .app import Application
 from .data import (
     AppData,
     StatusData,
     UserData,
     LogsData,
     BackupData,
-    FullLogsData,
-    UploadData
+    UploadData, FileInfo, StatisticsData
 )
 from .errors import ApplicationNotFound, InvalidFile, SquareException
 from .http import HTTPClient, Response
 from .http.endpoints import Endpoint
 from .listener import ListenerManager, Listener
 from .logs import logger
 from .payloads import (
     UserPayload,
     StatusPayload,
     LogsPayload,
     BackupPayload,
-    FullLogsPayload,
     UploadPayload,
 )
 from .square import File
 
 
 class AbstractClient(ABC):
     """Abstract client class"""
@@ -45,15 +44,16 @@
         display_name: str,
         main: str,
         memory: int,
         version: Literal['recommended', 'latest'],
         avatar: str | None = None,
         description: str | None = None,
         subdomain: str | None = None,
-        start: str | None = None
+        start: str | None = None,
+        auto_restart: bool | None = None,
 ):
     """
     Creates a config file (squarecloud.app)
     Args:
 
         display_name: name of your application
         main: name of your main file
@@ -75,14 +75,15 @@
         'MAIN': main,
         'MEMORY': memory,
         'VERSION': version,
         'AVATAR': avatar,
         'DESCRIPTION': description,
         'SUBDOMAIN': subdomain,
         'START': start,
+        'AUTORESTART': auto_restart,
     }
     for key, value in optionals.items():
         if value is not None:
             string: str = f'{key}={value}\n'
             content += string
     with open(f'./{path}/squarecloud.app', 'w', encoding='utf-8') as file:
         file.write(content)
@@ -122,54 +123,54 @@
             if not self._listener.get_request_listener(endpoint):
                 return self._listener.add_request_listener(endpoint, func)
             raise SquareException(
                 f'Already exists an capture_listener for {endpoint}')
 
         return wrapper
 
-    async def me(self, avoid_listener: bool = False) -> UserData:
+    async def me(self, **kwargs) -> UserData:
         """Get your information
 
         Args:
             avoid_listener: whether to avoid the request listener
 
         Returns:
             UserData
         """
         response: Response = await self._http.fetch_user_info()
         payload: UserPayload = response.response
         user_data: UserData = UserData(**payload['user'])
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return user_data
 
     async def user_info(self, user_id: int | None = None,
-                        avoid_listener: bool = False) -> UserData:
+                        **kwargs) -> UserData:
         """
         Get user information
         Args:
             user_id: user ID
             avoid_listener: whether to avoid the request listener
 
         Returns:
             UserData
         """
         response: Response = await self._http.fetch_user_info(user_id=user_id)
         payload: UserPayload = response.response
         user_data: UserData = UserData(**payload['user'])
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return user_data
 
     async def get_logs(self, app_id: str,
-                       avoid_listener: bool = False) -> LogsData:
+                       **kwargs) -> LogsData:
         """
         Get logs for an application
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
 
@@ -177,228 +178,205 @@
             LogData
         """
         response: Response | None = await self._http.fetch_logs(app_id)
         if not response:
             return LogsData(logs=None)
         payload: LogsPayload = response.response
         logs_data: LogsData = LogsData(**payload)
-        if not avoid_listener:
-            endpoint: Endpoint = response.route.endpoint
-            await self._listener.on_request(endpoint=endpoint,
-                                            response=response)
-        return logs_data
-
-    async def full_logs(self, app_id: str,
-                        avoid_listener: bool = False) -> FullLogsData:
-        """
-        Get logs for an application'
-
-        Args:
-            app_id: the application ID
-            avoid_listener: whether to avoid the request listener
-
-        Returns:
-            FullLogsData
-        """
-        response: Response = await self._http.fetch_logs_complete(app_id)
-        payload: FullLogsPayload = response.response
-        logs_data: FullLogsData = FullLogsData(**payload)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return logs_data
 
     async def app_status(self, app_id: str,
-                         avoid_listener: bool = False) -> StatusData:
+                         **kwargs) -> StatusData:
         """
         Get an application status
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
 
         Returns:
             StatusData
         """
         response: Response = await self._http.fetch_app_status(app_id)
         payload: StatusPayload = response.response
         status: StatusData = StatusData(**payload)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return status
 
     async def start_app(self, app_id: str,
-                        avoid_listener: bool = False) -> Response:
+                        **kwargs) -> Response:
         """
         Start an application
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
         Returns:
             Response
         """
 
         response: Response = await self._http.start_application(app_id)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return response
 
     async def stop_app(self, app_id: str,
-                       avoid_listener: bool = False) -> Response:
+                       **kwargs) -> Response:
         """
         Stop an application
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
         Returns:
             Response
         """
         response: Response = await self._http.stop_application(app_id)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return response
 
     async def restart_app(self, app_id: str,
-                          avoid_listener: bool = False) -> Response:
+                          **kwargs) -> Response:
         """
         Restart an application
 
         Args:
             avoid_listener: whether to avoid the request listener
             app_id: the application ID
         Returns:
             Response
         """
         response: Response = await self._http.restart_application(app_id)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return response
 
     async def backup(self, app_id: str,
-                     avoid_listener: bool = False) -> BackupData:
+                     **kwargs) -> BackupData:
         """
         Backup an application
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
         Returns:
             Backup
         """
         response: Response = await self._http.backup(app_id)
         payload: BackupPayload = response.response
         backup: BackupData = BackupData(**payload)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return backup
 
     async def delete_app(self, app_id: str,
-                         avoid_listener: bool = False) -> Response:
+                         **kwargs) -> Response:
         """
         Delete an application
 
         Args:
             app_id: the application ID
             avoid_listener: whether to avoid the request listener
         Returns:
             Response
         """
         response: Response = await self._http.delete_application(app_id)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return response
 
     async def commit(self, app_id: str, file: File,
-                     avoid_listener: bool = False) -> Response:
+                     **kwargs) -> Response:
         """
         Commit an application
 
         Args:
             app_id: the application ID
             file: the file object to be committed
             avoid_listener: whether to avoid the request listener
         Returns:
             Response
         """
         response: Response = await self._http.commit(app_id, file)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         return response
 
     async def app(self, app_id: str,
-                  avoid_listener: bool = False) -> Application:
+                  **kwargs) -> Application:
         """
         Get an application
 
         Args:
             avoid_listener: whether to avoid the request listener
             app_id: the application ID
         Returns:
             Application
         """
         response: Response = await self._http.fetch_user_info()
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         payload: UserPayload = response.response
         app_data = list(filter(lambda application: application['id'] == app_id,
                                payload['applications']))
         if not app_data:
             raise ApplicationNotFound
         app_data = app_data.pop()
         app: Application = Application(
             client=self, http=self._http,
-            data=AppData(**app_data))  # type: ignore
+            **app_data)  # type: ignore
         return app
 
     async def all_apps(
-            self, avoid_listener: bool = False) -> List[Application]:
+            self, **kwargs) -> List[Application]:
         """
         Get a list of your applications
 
         Args:
             avoid_listener: whether to avoid the request listener
 
         Returns:
             List[Application]
         """
         response: Response = await self._http.fetch_user_info()
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
         payload: UserPayload = response.response
-        apps_data: List[AppData] = [
-            AppData(**app_data) for app_data in  # type: ignore
-            payload['applications']]
+        apps_data: list = payload['applications']
         apps: List[Application] = [
-            Application(client=self, http=self._http, data=data) for data
+            Application(client=self, http=self._http, **data) for data
             in apps_data]
         return apps
 
     async def upload_app(self, file: File,
-                         avoid_listener: bool = False) -> UploadData:
+                         **kwargs) -> UploadData:
         """
         Upload an application
 
         Args:
             file: the file to be uploaded
             avoid_listener:whether to avoid the request listener
 
@@ -407,16 +385,76 @@
         """
         if not isinstance(file, File):
             raise InvalidFile(
                 f'you need provide an {File.__name__} object')
         if file.name.split('.')[-1] != 'zip':
             raise InvalidFile('the file must be a .zip file')
         response: Response = await self._http.upload(file)
-        if not avoid_listener:
+        if not kwargs.get('avoid_listener'):
             endpoint: Endpoint = response.route.endpoint
             await self._listener.on_request(endpoint=endpoint,
                                             response=response)
-        payload: UploadPayload = response.app
+        payload: UploadPayload = response.response.get('app')
         app: UploadData = UploadData(**payload)
         endpoint: Endpoint = response.route.endpoint
         await self._listener.on_request(endpoint=endpoint, response=response)
         return app
+
+    async def app_files_list(self, app_id: str, path: str, **kwargs):
+        response: Response = await self._http.fetch_app_files_list(app_id,
+                                                                   path)
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+
+        if not response.response[0]:  # type ignore
+            return
+        return [FileInfo(**data) for data in response.response]
+
+    async def read_app_file(self, app_id: str, path: str, **kwargs):
+        response: Response = await self._http.read_app_file(app_id, path)
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+        if response.response:
+            return BytesIO(bytes(response.response.get('data')))
+
+    async def create_app_file(self, app_id: str, file: File,
+                              path: str, **kwargs):
+        if not isinstance(file, File):
+            raise SquareException(
+                'the file must be an string or a squarecloud.File object')
+        file_bytes = list(file.bytes.read())
+        response: Response = await self._http.create_app_file(app_id,
+                                                              file_bytes, path)
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+        file.bytes.close()
+
+    async def delete_app_file(self, app_id: str, path: str, **kwargs):
+        response: Response = await self._http.file_delete(app_id, path)
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+        return response
+
+    async def statistics(self, **kwargs):
+        response: Response = await self._http.get_statistics()
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+        data = response.response['statistics']
+        return StatisticsData(**data)
+
+    async def app_data(self, app_id: str, **kwargs):
+        response: Response = await self._http.get_app_data(app_id)
+        if not kwargs.get('avoid_listener'):
+            endpoint: Endpoint = response.route.endpoint
+            await self._listener.on_request(endpoint=endpoint,
+                                            response=response)
+        return AppData(**response.response.get('app'))
```

### Comparing `squarecloud-api-2.0.1/squarecloud/data.py` & `squarecloud-api-3.0.0/squarecloud/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,21 +30,41 @@
     time: int | None = None
 
 
 @dataclass
 class AppData:
     """application data class"""
     id: str
-    tag: str
+    name: str
+    desc: str
+    avatar: str
+    owner: str
+    cluster: Literal[
+        'florida-ds1-1',
+        'florida-ds1-2',
+        'florida-ds1-3',
+        'florida-ds1-free-1'
+    ]
+    cpu: int
     ram: int
-    lang: Literal['javascript', 'typescript', 'python', 'java']
-    type: Literal['free', 'paid']
+    language: Literal[
+        'javascript',
+        'typescript',
+        'python',
+        'java',
+        'rust',
+        'go',
+        'static',
+        'dynamic',
+    ]
     cluster: Literal['free-', 'florida-1']
+    domain: str | None
+    custom: str | None
     isWebsite: bool
-    avatar: str
+    gitIntegration: bool
 
 
 @dataclass
 class UserData:
     """user data class"""
     id: int
     tag: str
@@ -60,28 +80,39 @@
     logs: str | None
 
     def __eq__(self, other):
         return isinstance(other, LogsData) and self.logs == other.logs
 
 
 @dataclass
-class FullLogsData:
-    """complete logs data class"""
-    logs: str
-
-
-@dataclass
 class BackupData:
     """backup data class"""
     downloadURL: str
 
 
 @dataclass
 class UploadData:
     id: str
     tag: str
-    description: str
+    description: str | None
     language: str
     avatar: str
     subdomain: str | None
     ram: int
     cpu: int
+
+
+@dataclass
+class FileInfo:
+    type: Literal['file', 'directory']
+    name: str
+    size: int
+    lastModified: int
+
+
+@dataclass
+class StatisticsData:
+    users: int
+    apps: int
+    websites: int
+    ping: int
+    time: int
```

### Comparing `squarecloud-api-2.0.1/squarecloud/errors.py` & `squarecloud-api-3.0.0/squarecloud/errors.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-2.0.1/squarecloud/http/http_client.py` & `squarecloud-api-3.0.0/squarecloud/http/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Literal
 
 import aiohttp
 
 from .endpoints import Endpoint, Router
+from ..data import AppData
 from ..errors import (
     NotFoundError,
     RequestError,
     BadRequestError,
     AuthenticationFailure
 )
 from ..logs import logger
@@ -22,42 +23,39 @@
     def __init__(self, data: RawResponseData, route: Router) -> None:
         self.data = data
         self.route: Router = route
         self.status: Literal['success', 'error'] = data.get('status')
         self.code: int = data.get('code')
         self.message: str = data.get('message')
         self.response: dict[str, Any] = data.get('response')
-        self.app: dict[str, Any] = data.get('app')
 
     def __repr__(self):
         return f'{Response.__name__}({self.status})'
 
 
 class HTTPClient:
     """A client that handles requests and responses"""
 
     def __init__(self, api_key: str) -> None:
         self.api_key = api_key
         self.__session = aiohttp.ClientSession
 
-    async def request(self, route: Router, **kwargs) -> Response | None:
+    async def request(self, route: Router,
+                      **kwargs) -> Response | None | bytes:
         """
         Sends a request to the Square API and returns the response.
 
         Args:
             route: the route to send a request
         Returns:
             RawResponseData
         """
         headers = {'Authorization': self.api_key}
 
-        if route.method == 'POST':
-            kwargs['skip_auto_headers'] = {'Content-Type'}
         if route.endpoint in (Endpoint.commit(), Endpoint.upload()):
-            del kwargs['skip_auto_headers']
             file = kwargs.pop('file')
             form = aiohttp.FormData()
             form.add_field('file', file.bytes, filename=file.name)
             kwargs['data'] = form
         async with self.__session(headers=headers) as session:
             async with session.request(url=route.url, method=route.method,
                                        **kwargs) as resp:
@@ -67,16 +65,16 @@
                     'status': data.get('status'),
                     'route': route.url,
                     'code': data.get('code'),
                     'request_message': data.get('message', '')
                 }
                 match status_code:
                     case 200:
-                        extra.pop('code')
                         logger.debug(msg='request to route: ', extra=extra)
+                        extra.pop('code')
                         response: Response = Response(data=data, route=route)
                     case 404:
                         logger.debug(msg='request to route: ', extra=extra)
                         msg = f'route [{route.endpoint.name}] returned 404, [{data.get("code")}]'
                         if route.endpoint == Endpoint.logs():
                             return
                         raise NotFoundError(msg)
@@ -134,28 +132,14 @@
         Returns:
             Response
         """
         route: Router = Router(Endpoint.logs(), app_id=app_id)
         response: Response = await self.request(route)
         return response
 
-    async def fetch_logs_complete(self, app_id: str) -> Response:
-        """
-        Make a request for LOGS_COMPLETE route
-
-        Args:
-            app_id:
-
-        Returns:
-            Response
-        """
-        route: Router = Router(Endpoint.full_logs(), app_id=app_id)
-        response: Response = await self.request(route)
-        return response
-
     async def start_application(self, app_id: str) -> Response:
         """
         Make a request for START route
 
         Args:
             app_id: the application ID
 
@@ -209,15 +193,15 @@
 
     async def delete_application(self, app_id: str) -> Response:
         """
         Make a request for DELETE route
         Args:
             app_id: the application ID
         """
-        route: Router = Router(Endpoint.delete(), app_id=app_id)
+        route: Router = Router(Endpoint.delete_app(), app_id=app_id)
         response: Response = await self.request(route)
         return response
 
     async def commit(self, app_id: str, file: File) -> Response:
         """
         Make a request for COMMIT route
         Args:
@@ -239,7 +223,39 @@
 
         Returns:
             Response
         """
         route: Router = Router(Endpoint.upload())
         response: Response = await self.request(route, file=file)
         return response
+
+    async def fetch_app_files_list(self, app_id: str, path: str):
+        route: Router = Router(Endpoint.files_list(), app_id=app_id, path=path)
+        response = await self.request(route)
+        return response
+
+    async def read_app_file(self, app_id: str, path: str):
+        route: Router = Router(Endpoint.files_read(), app_id=app_id, path=path)
+        response = await self.request(route)
+        return response
+
+    async def create_app_file(self, app_id: str, file: list[bytes], path: str):
+        route: Router = Router(Endpoint.files_create(), app_id=app_id)
+        response: Response = await self.request(route, json={'buffer': file,
+                                                             'path': path})
+        return response
+
+    async def file_delete(self, app_id: str, path: str):
+        route: Router = Router(Endpoint.files_delete(), app_id=app_id,
+                               path=path)
+        response: Response = await self.request(route)
+        return response
+
+    async def get_statistics(self):
+        route: Router = Router(Endpoint.statistics())
+        response: Response = await self.request(route)
+        return response
+
+    async def get_app_data(self, app_id: str):
+        route: Router = Router(Endpoint('APP_DATA'), app_id=app_id)
+        response: Response = await self.request(route)
+        return response
```

### Comparing `squarecloud-api-2.0.1/squarecloud/listener.py` & `squarecloud-api-3.0.0/squarecloud/listener.py`

 * *Files identical despite different names*

### Comparing `squarecloud-api-2.0.1/squarecloud/logs.py` & `squarecloud-api-3.0.0/squarecloud/logs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,36 @@
-"""custom logger"""
+"""Custom logger"""
+
 import logging
 
+# Define constants for color codes
+GREEN = '\033[0;32m'
+PURPLE = '\033[0;35m'
+RED = '\033[0;31m'
+END = '\033[m'
+
 # logging config
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
 
 
-class CustomFormatter(logging.Formatter):
-    """a custom logging formatter"""
-    green = '\033[0;32m'
-    purple = '\033[0;35m'
-    red = '\033[0;31m'
-    end = '\033[m'
+class CustomLogFormatter(logging.Formatter):
+    """A custom logging formatter"""
 
-    FORMAT_SUCCESS = f'{green}[%(levelname)s] %(status)s %(message)s %(route)s %(request_message)s {end}'
-    FORMAT_ERROR = f'{red}[%(levelname)s]  %(status)s %(message)s %(route)s, error: %(code)s{end}'
+    FORMAT_SUCCESS = f'{GREEN}[%(levelname)s] %(status)s %(message)s %(route)s %(request_message)s {END}'
+    FORMAT_ERROR = f'{RED}[%(levelname)s]  %(status)s %(message)s %(route)s, error: %(code)s{END}'
 
     def format(self, record: logging.LogRecord) -> str:
-        match record.status:
-            case 'success':
-                format_body = self.FORMAT_SUCCESS
-            case _:
-                format_body = self.FORMAT_ERROR
-        # formats_level = {
-        #     logging.INFO: self.purple + format_body + self.end,
-        #     logging.DEBUG: self.green + format_body + self.end,
-        #     logging.ERROR: self.red + format_body + self.end,
-        #     logging.CRITICAL: self.red + format_body + self.end,
-        #     logging.WARN: self.red + format_body + self.end,
-        # }
-        # log_fmt = formats_level.get(record.levelno)
-        # log_fmt = self.purple + format_body + self.end
+        if record.status == 'success':
+            format_body = self.FORMAT_SUCCESS
+        else:
+            format_body = self.FORMAT_ERROR
+        # log_fmt = PURPLE + format_body + END
         formatter = logging.Formatter(
             '\033[0;35m [%(asctime)s]: \033[m ' + format_body)
         return formatter.format(record)
 
 
 # console handler
 _ch = logging.StreamHandler()
 _ch.setLevel(logging.DEBUG)
-_ch.setFormatter(CustomFormatter())
+_ch.setFormatter(CustomLogFormatter())
 logger.addHandler(_ch)
```

### Comparing `squarecloud-api-2.0.1/squarecloud/payloads.py` & `squarecloud-api-3.0.0/squarecloud/payloads.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,32 +13,27 @@
     error: Optional[str]
     app: Optional[Dict[str, Any]]
 
 
 class UserPayload(RawResponseData):
     """user payload"""
     user: Dict[str, Any]
-    applications: Dict[str, Any]
+    applications: list[dict[str, Any]]
 
 
 class LogsPayload(RawResponseData):
     """logs payload"""
     logs: Dict[str, Any]
 
 
 class BackupPayload(RawResponseData):
     """backup payload"""
     backup: Dict[str, Any]
 
 
-class FullLogsPayload(RawResponseData):
-    """complete logs payload"""
-    url: Dict[str, Any]
-
-
 class StatusPayload(RawResponseData):
     """status payload"""
     # pylint: disable=invalid-name
     app_status: Dict[str, Any]
 
 
 class StopPayload(RawResponseData):
```

### Comparing `squarecloud-api-2.0.1/squarecloud_api.egg-info/PKG-INFO` & `squarecloud-api-3.0.0/squarecloud_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squarecloud-api
-Version: 2.0.1
+Version: 3.0.0
 Summary: SquareCloud API wrapper
 Home-page: UNKNOWN
 Author: Robert Nogueira
 Author-email: robertlucasnogueira@gmail.com
 License: MIT License
 Keywords: squarecloud/api/python
 Platform: UNKNOWN
@@ -32,21 +32,21 @@
 ## Getting api key
 
 to get your api key/token just go to the [SquareCloud] website and
 register/login, after that go
 to `dashboard` > `my account` > `Regenerate API/CLI KEY` and copy the key.
 
 > ## [Documentation](docs/)
-> - [application](docs/application.md)
-> - [capture_listeners](docs/capture_listeners.md)
-> - [client](docs/client.md)
-> - [commit_and_upload](docs/commit_and_upload.md)
-> - [request_listeners](docs/request_listeners.md)
+> - [application](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/application.md)
+> - [capture_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/capture_listeners.md)
+> - [client](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/client.md)
+> - [commit_and_upload](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/commit_and_upload.md)
+> - [request_listeners](https://github.com/squarecloudofc/wrapper-api-py/blob/main/docs/request_listeners.md)
 
-## Basict usage
+## Basic usage
 ```python
 import squarecloud as square
 import asyncio
 
 client = square.Client('API_KEY', debug=True)
 
 async def main():
```

