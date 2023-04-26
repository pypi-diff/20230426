# Comparing `tmp/easycheck_doiteasy-0.0.6.tar.gz` & `tmp/easycheck_doiteasy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.6.tar", last modified: Thu Apr 20 04:45:25 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.0.7.tar", last modified: Tue Apr 25 21:46:46 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.6.tar` & `easycheck_doiteasy-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-20 04:45:25.215160 easycheck_doiteasy-0.0.6/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.6/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-20 04:45:25.215160 easycheck_doiteasy-0.0.6/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.6/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-20 04:45:25.215160 easycheck_doiteasy-0.0.6/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     5157 2023-04-20 04:44:25.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-20 04:45:25.215160 easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-20 04:45:25.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-20 04:45:25.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-20 04:45:25.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-20 04:45:25.000000 easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.6/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-20 04:45:25.219159 easycheck_doiteasy-0.0.6/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.7/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.7/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.307144 easycheck_doiteasy-0.0.7/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     5254 2023-04-25 21:09:31.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-25 21:46:46.000000 easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.7/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-25 21:46:46.311144 easycheck_doiteasy-0.0.7/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.6/LICENSE.txt` & `easycheck_doiteasy-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.6/PKG-INFO` & `easycheck_doiteasy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.6/README.md` & `easycheck_doiteasy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.6/easycheck_doiteasy/easycheck_doiteasy.py` & `easycheck_doiteasy-0.0.7/easycheck_doiteasy/easycheck_doiteasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,26 @@
         self.ejecution_line_ids = []
         try:
             requests.post(url, data=data, headers=headers)
         except Exception as e:
             logging.error(e)
 
     
-    def send_subejecution(self, name, duration, start_datetime, end_datetime, total_register, successful):
+    def send_subejecution(self, name, duration, start_datetime, end_datetime, total_register, file_size, successful):
         """
         Sends execution data to an ejecution line API endpoint.
 
         Parameters:
         - name (str): The name of the execution.
         - duration (str): The duration of the execution in seconds.
         - start_datetime (str): The start datetime of the execution in ISO format (e.g. '2023-04-12T10:30:00Z').
         - end_datetime (str): The end datetime of the execution in ISO format (e.g. '2023-04-12T11:00:00Z').
         - destination (str): The destination of the execution.
         - total_register (int): The total number of registers processed during the execution.
+        - file_size (float): The size of the file
         - successful (bool): Whether the execution was successful or not.
         Returns:
         - None
         Raises:
         - This method may raise an exception if the HTTP request to the API endpoint fails for any reason. In this case, an error message will be logged.
         """    
         headers = {}
@@ -85,14 +86,15 @@
         url = f'{domain}{path}'
         data = {
             'name': name,
             'duration': duration,
             'start_datetime': start_datetime,
             'end_datetime': end_datetime,
             'total_register': total_register,
+            'file_size': file_size,
             'successful': successful,
             'register_token': self.token
         }
         try:
             res = requests.post(url, data=data, headers=headers)
             if res.status_code == 200:
                 self.ejecution_line_ids.append(res.json()['id'])
```

### Comparing `easycheck_doiteasy-0.0.6/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.0.7/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.6/setup.cfg` & `easycheck_doiteasy-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.6
+version = 0.0.7
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://etlcheck.com/
 project_urls =
```

