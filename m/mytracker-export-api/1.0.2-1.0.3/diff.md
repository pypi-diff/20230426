# Comparing `tmp/mytracker_export_api-1.0.2.tar.gz` & `tmp/mytracker_export_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytracker_export_api-1.0.2.tar", last modified: Mon Jan 23 14:16:53 2023, max compression
+gzip compressed data, was "mytracker_export_api-1.0.3.tar", last modified: Wed Apr 26 16:17:07 2023, max compression
```

## Comparing `mytracker_export_api-1.0.2.tar` & `mytracker_export_api-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.609394 mytracker_export_api-1.0.2/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1835 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/.gitignore
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/LICENSE
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-01-23 14:16:53.609079 mytracker_export_api-1.0.2/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.2/README.md
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.599724 mytracker_export_api-1.0.2/examples/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     6778 2022-07-01 11:29:52.000000 mytracker_export_api-1.0.2/examples/raw_data.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     5503 2022-07-01 11:30:17.000000 mytracker_export_api-1.0.2/examples/report.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1863 2022-06-29 15:28:06.000000 mytracker_export_api-1.0.2/examples/segment.ipynb
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.603331 mytracker_export_api-1.0.2/mytracker_export_api/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/mytracker_export_api/__init__.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/mytracker_export_api/exceptions.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)    16244 2023-01-23 14:04:08.000000 mytracker_export_api-1.0.2/mytracker_export_api/mytracker.py
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.608578 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      487 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/SOURCES.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/dependency_links.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/not-zip-safe
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       31 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/requires.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/top_level.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       31 2022-08-25 14:45:19.000000 mytracker_export_api-1.0.2/requirements.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-01-23 14:16:53.609508 mytracker_export_api-1.0.2/setup.cfg
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-01-23 11:11:22.000000 mytracker_export_api-1.0.2/setup.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-04-26 16:17:07.661303 mytracker_export_api-1.0.3/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.3/LICENSE
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-04-26 16:17:07.660825 mytracker_export_api-1.0.3/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.3/README.md
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-04-26 16:17:07.652769 mytracker_export_api-1.0.3/mytracker_export_api/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.3/mytracker_export_api/__init__.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.3/mytracker_export_api/exceptions.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)    17251 2023-04-26 16:12:20.000000 mytracker_export_api-1.0.3/mytracker_export_api/mytracker.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-04-26 16:17:07.660066 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      390 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/SOURCES.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/dependency_links.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/not-zip-safe
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       47 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/requires.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-04-26 16:17:07.000000 mytracker_export_api-1.0.3/mytracker_export_api.egg-info/top_level.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-04-26 16:17:07.661500 mytracker_export_api-1.0.3/setup.cfg
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-04-26 16:12:10.000000 mytracker_export_api-1.0.3/setup.py
```

### Comparing `mytracker_export_api-1.0.2/LICENSE` & `mytracker_export_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/PKG-INFO` & `mytracker_export_api-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker_export_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.2/README.md` & `mytracker_export_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/mytracker_export_api/mytracker.py` & `mytracker_export_api-1.0.3/mytracker_export_api/mytracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import hashlib
 import hmac
 import base64
 import time
 import requests
+import ssl
+import warnings
 import pandas as pd
-from binascii import b2a_base64
 from urllib.parse import urlencode, quote_plus
-from urllib.request import ProxyHandler, build_opener, install_opener, urlopen 
+from urllib.request import ProxyHandler, build_opener, install_opener, urlopen
+from urllib3.exceptions import InsecureRequestWarning
 from .exceptions import MyTrackerError
 
 
 class MyTracker:
     
     METHOD_GET = 'GET'
     METHOD_POST = 'POST'
@@ -20,36 +22,43 @@
     CANCEL_RAW_DATA_URL = 'https://tracker.my.com/api/raw/v1/export/cancel.json'
     
     CREATE_REPORT_URL = 'https://tracker.my.com/api/report/v1/file/create.json'
     GET_REPORT_URL = 'https://tracker.my.com/api/report/v1/file/get.json'
     
     CREATE_SEGMENT_URL = 'https://tracker.my.com/api/segment/v1/export/create.json'
     GET_SEGMENT_URL = 'https://tracker.my.com/api/segment/v1/export/get.json'
-    
-    
-    def __init__(self, api_user_id, api_secret_key, proxies=None):
+
+    def __init__(self, api_user_id, api_secret_key, proxies=None, ssl_verify=True):
         '''
         MyTracker class initialization. 
 
         -----------
         Parameters:
             api_user_id (int): API User ID
             api_secret_key (str): API Secret Key
             proxies (dict, optional): dictionary mapping protocol to the URL of the proxy
+            ssl_verify (bool, optional): SSL/TLS certificate check flag
 
         Example:
             proxies = {
                'http': 'http://proxy.example.com:8080',
                'https': 'http://secureproxy.example.com:8090',
             }
         '''
         
         self.api_user_id = api_user_id
         self.api_secret_key = api_secret_key
         self.proxies = proxies
+        self.ssl_verify = ssl_verify
+        self.urllib_context = None
+
+        if not ssl_verify:
+            self.urllib_context = ssl.create_default_context()
+            self.urllib_context.check_hostname = False
+            self.urllib_context.verify_mode = ssl.CERT_NONE
     
     def _get_signature(self, url, method, data='') -> str:
         ''' Getting a signature. '''
         
         base_string = '&'.join([method.upper(), quote_plus(url, safe='~'), quote_plus(data, safe='~')])
         signature = base64.b64encode(hmac.new(bytes(self.api_secret_key, 'UTF-8'), 
                                               bytes(base_string, 'UTF-8'), 
@@ -59,18 +68,22 @@
 
     def _send_request(self, url, method, headers=None):
         ''' Sending a request. '''
         
         if not headers:
             headers = {}
         headers['Authorization'] = self._get_signature(url, method)
-        if method.upper() == 'GET':
-            return requests.get(url=url, headers=headers, proxies=self.proxies)
-        elif method.upper() == 'POST':
-            return requests.post(url=url, headers=headers, proxies=self.proxies)
+
+        with warnings.catch_warnings():
+            if not self.ssl_verify:
+                warnings.simplefilter('ignore', InsecureRequestWarning)
+            if method.upper() == 'GET':
+                return requests.get(url=url, headers=headers, proxies=self.proxies, verify=self.ssl_verify)
+            elif method.upper() == 'POST':
+                return requests.post(url=url, headers=headers, proxies=self.proxies, verify=self.ssl_verify)
     
     def create_export(self, create_params, url):
         ''' 
         Data export request. 
 
         -----------
         Parameters:
@@ -188,18 +201,20 @@
                 self.cancel_raw_data_export(get_params['idRawExport'])
                 raise MyTrackerError(f'The program was interrupted. The request was canceled.')
             
             if get_response['code'] == 200:
                 if get_response['data']['status'] == 'Success!':
                     if return_df is True:
                         raw_data = []
-                        install_opener(build_opener(ProxyHandler(self.proxies)))
                         for file in get_response['data']['files']:
                             link = file['link']
-                            with urlopen(link, timeout=10) as f:
+                            opener = build_opener(ProxyHandler(self.proxies))
+                            opener.addheaders = [('Authorization', self._get_signature(url=link, method=self.METHOD_GET))]
+                            install_opener(opener)
+                            with urlopen(link, timeout=10, context=self.urllib_context) as f:
                                 raw_file = pd.read_csv(f, compression='gzip')
                             raw_data.append(raw_file)
                         raw_data = pd.concat(raw_data, ignore_index=True)
                         break
                     elif return_df is False:
                         return dict(get_response)
                     else:
@@ -299,16 +314,18 @@
         while True:
             get_response = self.get_export(get_params, url=self.GET_REPORT_URL)
             
             if get_response['code'] == 200:
                 if get_response['data']['status'] == 'Success!':
                     if return_df is True:
                         link = get_response['data']['files'][0]['link']
-                        install_opener(build_opener(ProxyHandler(self.proxies)))
-                        with urlopen(link, timeout=10) as file:
+                        opener = build_opener(ProxyHandler(self.proxies))
+                        opener.addheaders = [('Authorization', self._get_signature(url=link, method=self.METHOD_GET))]
+                        install_opener(opener)
+                        with urlopen(link, timeout=10, context=self.urllib_context) as file:
                             report = pd.read_csv(file, compression='gzip')
                         break
                     elif return_df is False:
                         return dict(get_response)
                     else:
                         raise MyTrackerError('Parameter return_df must be True or False.')
```

### Comparing `mytracker_export_api-1.0.2/mytracker_export_api.egg-info/PKG-INFO` & `mytracker_export_api-1.0.3/mytracker_export_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker-export-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.2/setup.py` & `mytracker_export_api-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mytracker_export_api',
-    version='1.0.2',
+    version='1.0.3',
     description='Python wrapper for MyTracker Export API.',
     packages=['mytracker_export_api'],
     author='Artyom Novopolsky',
     author_email='a.novopolsky@corp.mail.ru',
     install_requires=open('requirements.txt').read().splitlines(),
     python_requires='>=3.6.1',
     long_description=open('README.md').read(),
```

