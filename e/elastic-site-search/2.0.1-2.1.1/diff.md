# Comparing `tmp/elastic-site-search-2.0.1.tar.gz` & `tmp/elastic-site-search-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elastic-site-search-2.0.1.tar", last modified: Mon Sep 16 20:41:53 2019, max compression
+gzip compressed data, was "dist/elastic-site-search-2.1.1.tar", last modified: Tue Apr 25 20:18:36 2023, max compression
```

## Comparing `elastic-site-search-2.0.1.tar` & `elastic-site-search-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jasonstoltzfus   (501) staff       (20)        0 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)    19903 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/PKG-INFO
-drwxr-xr-x   0 jasonstoltzfus   (501) staff       (20)        0 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search/
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)       18 2019-09-16 20:37:01.000000 elastic-site-search-2.0.1/elastic_site_search/version.py
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)    12863 2019-09-16 20:35:51.000000 elastic-site-search-2.0.1/elastic_site_search/client.py
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)       79 2019-08-19 20:02:51.000000 elastic-site-search-2.0.1/elastic_site_search/__init__.py
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)    15162 2019-08-19 20:02:51.000000 elastic-site-search-2.0.1/README.md
--rwxr-xr-x   0 jasonstoltzfus   (501) staff       (20)     1540 2019-08-19 20:02:51.000000 elastic-site-search-2.0.1/setup.py
-drwxr-xr-x   0 jasonstoltzfus   (501) staff       (20)        0 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)    19903 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/PKG-INFO
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)      335 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/SOURCES.txt
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)       12 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/requires.txt
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)       20 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/top_level.txt
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)        1 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/elastic_site_search.egg-info/dependency_links.txt
--rw-r--r--   0 jasonstoltzfus   (501) staff       (20)       67 2019-09-16 20:41:53.000000 elastic-site-search-2.0.1/setup.cfg
+drwxr-xr-x   0 klimmarkelov   (501) staff       (20)        0 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)    19903 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/PKG-INFO
+drwxr-xr-x   0 klimmarkelov   (501) staff       (20)        0 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search/
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)       18 2023-04-25 20:14:02.000000 elastic-site-search-2.1.1/elastic_site_search/version.py
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)    12846 2023-04-25 20:14:02.000000 elastic-site-search-2.1.1/elastic_site_search/client.py
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)       79 2023-04-25 20:14:02.000000 elastic-site-search-2.1.1/elastic_site_search/__init__.py
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)    15162 2023-04-25 20:14:02.000000 elastic-site-search-2.1.1/README.md
+-rwxr-xr-x   0 klimmarkelov   (501) staff       (20)     1529 2023-04-25 20:14:02.000000 elastic-site-search-2.1.1/setup.py
+drwxr-xr-x   0 klimmarkelov   (501) staff       (20)        0 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)    19903 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/PKG-INFO
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)      335 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/SOURCES.txt
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)        4 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/requires.txt
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)       20 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/top_level.txt
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)        1 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/elastic_site_search.egg-info/dependency_links.txt
+-rw-r--r--   0 klimmarkelov   (501) staff       (20)       67 2023-04-25 20:18:36.000000 elastic-site-search-2.1.1/setup.cfg
```

### Comparing `elastic-site-search-2.0.1/PKG-INFO` & `elastic-site-search-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic-site-search
-Version: 2.0.1
+Version: 2.1.1
 Summary: Elastic Site Search API Client for Python
 Home-page: https://github.com/elastic/site-search-python
 Author: Elastic
 Author-email: support@elastic.co
 License: Apache 2.0
 Description: <p align="center"><img src="https://github.com/elastic/site-search-python/blob/master/logo-site-search.png?raw=true" alt="Elastic Site Search Logo"></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elastic-site-search Version: 2.0.1 Summary: Elastic
+Metadata-Version: 2.1 Name: elastic-site-search Version: 2.1.1 Summary: Elastic
 Site Search API Client for Python Home-page: https://github.com/elastic/site-
 search-python Author: Elastic Author-email: support@elastic.co License: Apache
 2.0 Description:
                           [Elastic Site Search Logo]
                        [CircleCI_build] [GitHub_release]
 > A first-party Python client for the [Elastic Site Search API](https://
 elastic.co/products/site-search). ## Contents + [Getting started](#getting-
```

### Comparing `elastic-site-search-2.0.1/elastic_site_search/client.py` & `elastic-site-search-2.1.1/elastic_site_search/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import unicode_literals
 
 import base64
 import time
 import hashlib
 
-import anyjson
+import json
 from six.moves.urllib_parse import urlunparse, urlencode
 
 try:
     # VCRpy only works when `httplib` is imported directly on Python 2.x
     import httplib
 except ImportError:
     import http.client as httplib
@@ -157,15 +157,15 @@
 
   def sso_url(self, user_id):
     timestamp = self._get_timestamp()
     params = {'user_id': user_id, 'client_id': self.client_id, 'timestamp': timestamp, 'token': self._sso_token(user_id, timestamp)}
     return urlunparse(('https', 'swiftype.com', '/sso', '', urlencode(params), ''))
 
   def _sso_token(self, user_id, timestamp):
-    return hashlib.sha1((
+    return hashlib.sha256((
         '%s:%s:%s' % (user_id, self.client_secret, timestamp)
     ).encode('utf-8')).hexdigest()
 
   def _get_timestamp(self):
     return int(time.time())
 
   def __search_path(self, engine_id): return 'engines/%s/search' % (engine_id)
@@ -234,25 +234,25 @@
         raise HttpException(401, 'Authorization required.')
 
     full_path = self.__base_path + path + '.json'
     query = urlencode(params, True)
     if query:
       full_path += '?' + query
 
-    body = anyjson.serialize(data) if data else ''
+    body = json.dumps(data) if data else ''
 
     connection = httplib.HTTPConnection(self.__host)
     connection.request(method, full_path, body, headers)
 
     response = connection.getresponse()
     response.body = response.read()
     if (response.status // 100 == 2):
         if response.body:
             try:
-                response.body = anyjson.deserialize(response.body.decode('utf-8'))
+                response.body = json.loads(response.body.decode('utf-8'))
             except ValueError as e:
                 raise InvalidResponseFromServer('The JSON response could not be parsed: %s.\n%s' % (e, response.body))
             ret = {'status': response.status, 'body':response.body }
         else:
             ret = {'status': response.status }
     elif response.status == 401:
         raise HttpException( response.status, 'Authorization required.')
```

### Comparing `elastic-site-search-2.0.1/README.md` & `elastic-site-search-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `elastic-site-search-2.0.1/setup.py` & `elastic-site-search-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     license = 'Apache 2.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Elastic',
     author_email = 'support@elastic.co',
     url = 'https://github.com/elastic/site-search-python',
     packages = find_packages(exclude=['tests', 'fixtures']),
-    install_requires = ["anyjson", "six"],
+    install_requires = ["six"],
     tests_require=['nose', 'vcrpy', 'mock', 'unittest2'],
     test_suite='nose.collector',
     classifiers = [
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
```

### Comparing `elastic-site-search-2.0.1/elastic_site_search.egg-info/PKG-INFO` & `elastic-site-search-2.1.1/elastic_site_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic-site-search
-Version: 2.0.1
+Version: 2.1.1
 Summary: Elastic Site Search API Client for Python
 Home-page: https://github.com/elastic/site-search-python
 Author: Elastic
 Author-email: support@elastic.co
 License: Apache 2.0
 Description: <p align="center"><img src="https://github.com/elastic/site-search-python/blob/master/logo-site-search.png?raw=true" alt="Elastic Site Search Logo"></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elastic-site-search Version: 2.0.1 Summary: Elastic
+Metadata-Version: 2.1 Name: elastic-site-search Version: 2.1.1 Summary: Elastic
 Site Search API Client for Python Home-page: https://github.com/elastic/site-
 search-python Author: Elastic Author-email: support@elastic.co License: Apache
 2.0 Description:
                           [Elastic Site Search Logo]
                        [CircleCI_build] [GitHub_release]
 > A first-party Python client for the [Elastic Site Search API](https://
 elastic.co/products/site-search). ## Contents + [Getting started](#getting-
```

