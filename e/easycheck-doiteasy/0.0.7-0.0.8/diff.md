# Comparing `tmp/easycheck_doiteasy-0.0.7.tar.gz` & `tmp/easycheck_doiteasy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.7.tar", last modified: Tue Apr 25 21:46:46 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.0.8.tar", last modified: Wed Apr 26 19:29:08 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.7.tar` & `easycheck_doiteasy-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.7/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.7/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.307144 easycheck_doiteasy-0.0.7/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     5254 2023-04-25 21:09:31.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.7/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 19:29:08.955849 easycheck_doiteasy-0.0.8/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.8/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 19:29:08.955849 easycheck_doiteasy-0.0.8/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.8/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 19:29:08.955849 easycheck_doiteasy-0.0.8/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     5375 2023-04-26 16:18:51.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 19:29:08.955849 easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 19:29:08.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-26 19:29:08.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-26 19:29:08.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-26 19:29:08.000000 easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.8/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-26 19:29:08.955849 easycheck_doiteasy-0.0.8/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.7/LICENSE.txt` & `easycheck_doiteasy-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.7/PKG-INFO` & `easycheck_doiteasy-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.7/README.md` & `easycheck_doiteasy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.7/easycheck_doiteasy/easycheck_doiteasy.py` & `easycheck_doiteasy-0.0.8/easycheck_doiteasy/easycheck_doiteasy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import timedelta, datetime
 import requests
 import os
 import logging
 logging = logging.getLogger(__name__)
 
 
 
@@ -17,15 +18,15 @@
         domain (str): The default domain URL for API calls.
         """
         self.token = token
         self.domain = 'https://etlcheck.com'
         self.ejecution_line_ids = []
 
 
-    def send_ejecution(self, name, duration, start_datetime, end_datetime, destination, total_register, successful):
+    def send_ejecution(self, name: str, duration: timedelta, start_datetime: datetime, end_datetime: datetime, destination: str, total_register: int, successful: bool):
         """
         Sends execution data to a specified API endpoint.
 
         Parameters:
         - name (str): The name of the execution.
         - duration (str): The duration of the execution in seconds.
         - start_datetime (str): The start datetime of the execution in ISO format (e.g. '2023-04-12T10:30:00Z').
@@ -58,44 +59,44 @@
         self.ejecution_line_ids = []
         try:
             requests.post(url, data=data, headers=headers)
         except Exception as e:
             logging.error(e)
 
     
-    def send_subejecution(self, name, duration, start_datetime, end_datetime, total_register, file_size, successful):
+    def send_subejecution(self, name: str, duration: float, start_datetime: str, end_datetime: str, total_register: int, file_size: int, successful: bool, state: str): 
         """
-        Sends execution data to an ejecution line API endpoint.
-
-        Parameters:
-        - name (str): The name of the execution.
-        - duration (str): The duration of the execution in seconds.
-        - start_datetime (str): The start datetime of the execution in ISO format (e.g. '2023-04-12T10:30:00Z').
-        - end_datetime (str): The end datetime of the execution in ISO format (e.g. '2023-04-12T11:00:00Z').
-        - destination (str): The destination of the execution.
-        - total_register (int): The total number of registers processed during the execution.
-        - file_size (float): The size of the file
-        - successful (bool): Whether the execution was successful or not.
+        Sends the subexecution details to the API endpoint.
+        Args:
+            name (str): The name of the subexecution.
+            duration (float): The duration of the subexecution in seconds.
+            start_datetime (str): The start datetime of the subexecution in ISO format.
+            end_datetime (str): The end datetime of the subexecution in ISO format.
+            total_register (int): The total number of records processed.
+            file_size (int): The size of the input file in bytes.
+            successful (bool): True if the subexecution was successful, False otherwise.
+            state (str): The current state of the subexecution. Possible values are "init", "processing", and "completed".
         Returns:
-        - None
+            None
         Raises:
-        - This method may raise an exception if the HTTP request to the API endpoint fails for any reason. In this case, an error message will be logged.
-        """    
+            Exception: If there is an error while sending the subexecution details.
+        """
         headers = {}
         domain = self.domain
         path = '/api/base/ejecution_line/send/'
         url = f'{domain}{path}'
         data = {
             'name': name,
             'duration': duration,
             'start_datetime': start_datetime,
             'end_datetime': end_datetime,
             'total_register': total_register,
             'file_size': file_size,
             'successful': successful,
+            'state': state,
             'register_token': self.token
         }
         try:
             res = requests.post(url, data=data, headers=headers)
             if res.status_code == 200:
                 self.ejecution_line_ids.append(res.json()['id'])
         except Exception as e:
```

### Comparing `easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.0.8/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.7/setup.cfg` & `easycheck_doiteasy-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.7
+version = 0.0.8
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://etlcheck.com/
 project_urls =
```

