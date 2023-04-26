# Comparing `tmp/pypaperless-0.0.7.tar.gz` & `tmp/pypaperless-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaperless-0.0.7.tar", last modified: Wed Apr  6 09:36:04 2022, max compression
+gzip compressed data, was "pypaperless-0.0.8.tar", last modified: Tue Apr 25 18:07:11 2023, max compression
```

## Comparing `pypaperless-0.0.7.tar` & `pypaperless-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:36:04.236787 pypaperless-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-06 09:35:50.000000 pypaperless-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-04-06 09:36:04.236787 pypaperless-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-04-06 09:35:50.000000 pypaperless-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:36:04.232787 pypaperless-0.0.7/pypaperless/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-04-06 09:35:50.000000 pypaperless-0.0.7/pypaperless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-04-06 09:35:50.000000 pypaperless-0.0.7/pypaperless/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     6896 2022-04-06 09:35:50.000000 pypaperless-0.0.7/pypaperless/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-04-06 09:35:50.000000 pypaperless-0.0.7/pypaperless/paperless.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:36:04.236787 pypaperless-0.0.7/pypaperless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-04-06 09:36:03.000000 pypaperless-0.0.7/pypaperless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-04-06 09:36:04.000000 pypaperless-0.0.7/pypaperless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 09:36:03.000000 pypaperless-0.0.7/pypaperless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-06 09:36:04.000000 pypaperless-0.0.7/pypaperless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-04-06 09:35:50.000000 pypaperless-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-06 09:36:04.236787 pypaperless-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-04-06 09:35:50.000000 pypaperless-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:07:11.509345 pypaperless-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 18:06:58.000000 pypaperless-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 18:07:11.509345 pypaperless-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-25 18:06:58.000000 pypaperless-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:07:11.509345 pypaperless-0.0.8/pypaperless/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 18:06:58.000000 pypaperless-0.0.8/pypaperless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-25 18:06:58.000000 pypaperless-0.0.8/pypaperless/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-25 18:06:58.000000 pypaperless-0.0.8/pypaperless/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-25 18:06:58.000000 pypaperless-0.0.8/pypaperless/paperless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:07:11.509345 pypaperless-0.0.8/pypaperless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 18:07:11.000000 pypaperless-0.0.8/pypaperless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 18:07:11.000000 pypaperless-0.0.8/pypaperless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:07:11.000000 pypaperless-0.0.8/pypaperless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 18:07:11.000000 pypaperless-0.0.8/pypaperless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 18:06:58.000000 pypaperless-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:07:11.509345 pypaperless-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-25 18:06:58.000000 pypaperless-0.0.8/setup.py
```

### Comparing `pypaperless-0.0.7/LICENSE` & `pypaperless-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypaperless-0.0.7/PKG-INFO` & `pypaperless-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pypaperless
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small API wrapper for paperless-ngx dms.
 Home-page: https://github.com/grdn1337/paperless-api
 Author: tbsch
 Author-email: info@tbsch.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/grdn1337/paperless-api/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,14 +26,15 @@
 ```python
 import asyncio
 import pypaperless
 
 
 async def main():
     api = pypaperless.PaperlessAPI("http://127.0.0.1:9120", "SUPER_SECRET_API_TOKEN_HERE")
+    # alternative: api = pypaperless.PaperlessAPI("http://127.0.0.1:9120", username="user", password="pass")
 
     correspondents = await api.get_correspondents()
 
     for data in correspondents:
         print(data.raw_data)
 
 asyncio.run(main())
@@ -44,10 +43,28 @@
 Same is possible for every other endpoint provided by the API, excepting logs.
 
 ```python
 doctypes = await api.get_document_types()
 tags = await api.get_tags()
 views = await api.get_saved_views()
 documents = await api.get_documents()
+tasks = await apt.get_tasks()
 ```
 
+Request a single item by id from an endpoint.
+```python
+doctype = await api.get_document_type(3)
+tag = await api.get_tag(6)
+document = await api.get_document(6)
+task = await api.get_task(123)
+by_task_id = await api.get_task_by_task_id("fdaa724b-xxxx-yyyy-aaf8-edc5c113c656")
+```
 
+Post a document to Paperless. Only the file is mandatory, title, creation date correspondent id, and document type id are optional. Tags are crurrently not supported.
+```python
+await api.post_document("./invoice.pdf",title="Invoice bedroom closet")
+```
+
+Search for a document and receive a list of results. Search syntax is the same as in Paperless: https://docs.paperless-ngx.com/usage/#basic-usage_searching.
+```python
+matching_documents = await api.search("bedroom*")
+```
```

### Comparing `pypaperless-0.0.7/pypaperless/auth.py` & `pypaperless-0.0.8/pypaperless/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from aiohttp import ClientSession, ClientResponse
-
+import base64
 
 class Auth:
     """Class to make authenticated requests."""
 
-    def __init__(self, endpoint: str, token: str):
+    token: str = ""
+    basic_auth: str = ""
+
+    def __init__(self, endpoint: str, token: str = None, username: str = None, password: str = None):
         """Initialize the auth."""
         self.basepath = endpoint
-        self.token = token
+        if token:
+            self.token = token
+        if username and password:
+            self.basic_auth = base64.b64encode(f"{username}:{password}".encode()).decode()
 
     async def request(self, session: ClientSession, method: str, path: str, **kwargs) -> ClientResponse:
         uri = f"{self.basepath}/{path}/"
         return await self.__request(session, method, uri, **kwargs)
 
     async def request_raw(self, session: ClientSession, method: str, uri: str, **kwargs) -> ClientResponse:
         return await self.__request(session, method, uri, **kwargs)
@@ -28,12 +34,15 @@
 
         if params is None:
             params = {}
         else:
             params = dict(params)
 
         params["format"] = "json"
-        headers["authorization"] = f"Token {self.token}"
+        if self.token:
+            headers["authorization"] = f"Token {self.token}"
+        else:
+            headers["authorization"] = f"Basic {self.basic_auth}"
 
         return await session.request(
             method, uri, **kwargs, headers=headers,
         )
```

### Comparing `pypaperless-0.0.7/pypaperless/model.py` & `pypaperless-0.0.8/pypaperless/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -258,7 +258,60 @@
         """Return the original_file_name."""
         return self.raw_data["original_file_name"]
 
     @property
     def archived_file_name(self) -> str:
         """Return the archived_file_name."""
         return self.raw_data["archived_file_name"]
+
+class Task:
+    """Class that represents a task object in the paperless API"""
+
+    def __init__(self, raw_data: dict, auth: Auth):
+        """Initialize a task object."""
+        self.raw_data = raw_data
+        self.auth = auth
+
+    @property
+    def task_id(self) -> str:
+        """Return the task id."""
+        return self.raw_data["task_id"]
+
+    @property
+    def task_file_name(self) -> str:
+        """Return the task file name."""
+        return self.raw_data["task_file_name"]
+
+    @property
+    def date_created(self) -> datetime:
+        """Return the creation date."""
+        return self.raw_data["date_created"]
+    
+    @property
+    def date_done(self) -> datetime:
+        """Return the finishing date."""
+        return self.raw_data["date_done"]
+
+    @property
+    def type(self) -> str:
+        """Return the type."""
+        return self.raw_data["type"]
+
+    @property
+    def status(self) -> str:
+        """Return the status."""
+        return self.raw_data["status"]
+
+    @property
+    def result(self) -> str:
+        """Return the result string."""
+        return self.raw_data["result"]
+
+    @property
+    def result(self) -> bool:
+        """Return if the task was acknowledged"""
+        return self.raw_data["acknowledged"]
+    
+    @property
+    def related_document(self) -> int:
+        """Return the related document id"""
+        return self.raw_data["related_document"]
```

### Comparing `pypaperless-0.0.7/pypaperless.egg-info/PKG-INFO` & `pypaperless-0.0.8/pypaperless.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pypaperless
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small API wrapper for paperless-ngx dms.
 Home-page: https://github.com/grdn1337/paperless-api
 Author: tbsch
 Author-email: info@tbsch.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/grdn1337/paperless-api/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,14 +26,15 @@
 ```python
 import asyncio
 import pypaperless
 
 
 async def main():
     api = pypaperless.PaperlessAPI("http://127.0.0.1:9120", "SUPER_SECRET_API_TOKEN_HERE")
+    # alternative: api = pypaperless.PaperlessAPI("http://127.0.0.1:9120", username="user", password="pass")
 
     correspondents = await api.get_correspondents()
 
     for data in correspondents:
         print(data.raw_data)
 
 asyncio.run(main())
@@ -44,10 +43,28 @@
 Same is possible for every other endpoint provided by the API, excepting logs.
 
 ```python
 doctypes = await api.get_document_types()
 tags = await api.get_tags()
 views = await api.get_saved_views()
 documents = await api.get_documents()
+tasks = await apt.get_tasks()
 ```
 
+Request a single item by id from an endpoint.
+```python
+doctype = await api.get_document_type(3)
+tag = await api.get_tag(6)
+document = await api.get_document(6)
+task = await api.get_task(123)
+by_task_id = await api.get_task_by_task_id("fdaa724b-xxxx-yyyy-aaf8-edc5c113c656")
+```
 
+Post a document to Paperless. Only the file is mandatory, title, creation date correspondent id, and document type id are optional. Tags are crurrently not supported.
+```python
+await api.post_document("./invoice.pdf",title="Invoice bedroom closet")
+```
+
+Search for a document and receive a list of results. Search syntax is the same as in Paperless: https://docs.paperless-ngx.com/usage/#basic-usage_searching.
+```python
+matching_documents = await api.search("bedroom*")
+```
```

### Comparing `pypaperless-0.0.7/setup.py` & `pypaperless-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypaperless",
-    version="0.0.7",
+    version="0.0.8",
     author="tbsch",
     author_email="info@tbsch.de",
     description="A small API wrapper for paperless-ngx dms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/grdn1337/paperless-api",
     project_urls={
```

