# Comparing `tmp/cortex-python-6.3.1a1.tar.gz` & `tmp/cortex-python-6.3.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex-python-6.3.1a1.tar", last modified: Thu Feb 23 15:05:34 2023, max compression
+gzip compressed data, was "cortex-python-6.3.1a2.tar", last modified: Wed Apr 26 11:35:37 2023, max compression
```

## Comparing `cortex-python-6.3.1a1.tar` & `cortex-python-6.3.1a2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/
--rw-r--r--   0 root         (0) root         (0)      533 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11368 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4623 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3938 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.459992 cortex-python-6.3.1a1/cortex/
--rw-r--r--   0 root         (0) root         (0)      877 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/auth.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/camel.py
--rw-r--r--   0 root         (0) root         (0)    27148 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/client.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/connection.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/constant.py
--rw-r--r--   0 root         (0) root         (0)    10083 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/content.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/env.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/cortex/experiment/
--rw-r--r--   0 root         (0) root         (0)      675 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7794 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/experiment/local.py
--rw-r--r--   0 root         (0) root         (0)    10770 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/experiment/model.py
--rw-r--r--   0 root         (0) root         (0)    37404 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/experiment/remote.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/message.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/model.py
--rw-r--r--   0 root         (0) root         (0)    10071 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/properties.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/secrets.py
--rw-r--r--   0 root         (0) root         (0)    11589 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/serviceconnector.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/session.py
--rw-r--r--   0 root         (0) root         (0)     8521 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/skill.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/timer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/types.py
--rw-r--r--   0 root         (0) root         (0)     8390 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/utils.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/cortex/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/cortex_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4623 2023-02-23 15:05:34.000000 cortex-python-6.3.1a1/cortex_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-23 15:05:34.000000 cortex-python-6.3.1a1/cortex_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 15:05:34.000000 cortex-python-6.3.1a1/cortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      235 2023-02-23 15:05:34.000000 cortex-python-6.3.1a1/cortex_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-23 15:05:34.000000 cortex-python-6.3.1a1/cortex_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2171 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/test/
--rw-r--r--   0 root         (0) root         (0)      590 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 15:05:34.463992 cortex-python-6.3.1a1/test/unit/
--rw-r--r--   0 root         (0) root         (0)      590 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/authenticationclient_test.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/connectionclient_test.py
--rw-r--r--   0 root         (0) root         (0)     9001 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/cortex_test.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/environment_config_test.py
--rw-r--r--   0 root         (0) root         (0)     6849 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/experiment_test.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     8747 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/run_test.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/serviceconnector_test.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-23 15:03:15.000000 cortex-python-6.3.1a1/test/unit/sessionclient_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex/
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/camel.py
+-rw-r--r--   0 root         (0) root         (0)    27147 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/client.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/connection.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9662 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/content.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/env.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex/experiment/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7794 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/local.py
+-rw-r--r--   0 root         (0) root         (0)    10770 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/model.py
+-rw-r--r--   0 root         (0) root         (0)    37404 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/remote.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/message.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/model.py
+-rw-r--r--   0 root         (0) root         (0)    10071 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/properties.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/secrets.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/serviceconnector.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/session.py
+-rw-r--r--   0 root         (0) root         (0)     8521 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/skill.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/timer.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/types.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/test/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/test/unit/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/authenticationclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     4371 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/connectionclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     9014 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/cortex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/environment_config_test.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/experiment_test.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     8807 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/run_test.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/serviceconnector_test.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/sessionclient_test.py
```

### Comparing `cortex-python-6.3.1a1/CHANGELOG.md` & `cortex-python-6.3.1a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/LICENSE` & `cortex-python-6.3.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/PKG-INFO` & `cortex-python-6.3.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a1
+Version: 6.3.1a2
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a1/README.md` & `cortex-python-6.3.1a2/README.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/__init__.py` & `cortex-python-6.3.1a2/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/auth.py` & `cortex-python-6.3.1a2/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/camel.py` & `cortex-python-6.3.1a2/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/client.py` & `cortex-python-6.3.1a2/cortex/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         url: str,
         token: _Token = None,
         config: dict = None,
         project: str = None,
         version: int = VERSION,
         verify_ssl_cert: bool = False,
     ):
-
         self._token = token
         self._config = config
         self._project = project
         self._url = url
         self._version = version
         self._verify_ssl_cert = verify_ssl_cert
```

### Comparing `cortex-python-6.3.1a1/cortex/connection.py` & `cortex-python-6.3.1a2/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/constant.py` & `cortex-python-6.3.1a2/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/content.py` & `cortex-python-6.3.1a2/cortex/content.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from io import BytesIO, StringIO, FileIO
 from typing import Union, List
 from urllib3.response import HTTPResponse
 
 
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from requests.exceptions import HTTPError
-import tenacity
 
 from .serviceconnector import _Client
 from .utils import (
     raise_for_status_with_detail,
     get_logger,
 )
 
@@ -68,29 +67,30 @@
         :type retries: int, optional
         :return: a dict with the response to request upload.
         :rtype: dict
 
         .. NOTE: This method uses a multi-part form request; to upload very large files, use `uploadStreaming` instead.
         .. seealso: uploadStreaming()
         """  # pylint: disable=line-too-long
-        res = tenacity.Retrying(
-            stop=tenacity.stop_after_attempt(retries + 1),
-            retry=tenacity.retry_if_exception(
-                ManagedContentClient._http_request_retry_predicate,
-            ),
-        )
-        return res.wraps(self._upload)(key, stream_name, stream, content_type)
+        return self._upload(key, stream_name, stream, content_type, retries)
 
-    def _upload(self, key: str, stream_name: str, stream: object, content_type: str):
+    def _upload(
+        self,
+        key: str,
+        stream_name: str,
+        stream: object,
+        content_type: str,
+        retries: int = 1,
+    ):
         uri = self.URIs["content"].format(projectId=self._project())
         fields = {"key": key, "content": (stream_name, stream, content_type)}
         data = MultipartEncoder(fields=fields)
         headers = {"Content-Type": data.content_type}
-        res = self._serviceconnector.request(
-            "POST", uri=uri, body=data, headers=headers
+        res = self._serviceconnector.request_with_retry(
+            "POST", uri=uri, body=data, headers=headers, retries=retries
         )
         raise_for_status_with_detail(res)
         return res.json()
 
     @staticmethod
     def _get_source_files(source):
         source_regex = os.path.join(source, "**/*")
@@ -143,52 +143,44 @@
         :param content_type: The type of the file to store (e.g., `text/csv`), defaults to "application/octet-stream"
         :type content_type: str, optional
         :param retries: Number of times to retry a failed request from a retryable response., defaults to 1
         :type retries: int, optional
         :return: A dict with the response to request upload.
         :rtype: dict
         """  # pylint: disable=line-too-long
-        res = tenacity.Retrying(
-            stop=tenacity.stop_after_attempt(retries + 1),
-            retry=tenacity.retry_if_exception(
-                ManagedContentClient._http_request_retry_predicate
-            ),
-        )
-        return res.wraps(self._upload_streaming)(key, stream, content_type)
+        return self._upload_streaming(key, stream, content_type, retries)
 
-    def _upload_streaming(self, key: str, stream: object, content_type: str):
+    def _upload_streaming(
+        self, key: str, stream: object, content_type: str, retries: int = 1
+    ):
         uri = self._make_content_uri(key)
         headers = {"Content-Type": content_type}
-        res = self._serviceconnector.request(
-            "POST", uri=uri, body=stream, headers=headers
+        res = self._serviceconnector.request_with_retry(
+            "POST", uri=uri, body=stream, headers=headers, retries=retries
         )
         raise_for_status_with_detail(res)
         return res.json()
 
     def download(self, key: str, retries: int = 1) -> HTTPResponse:
         """Download a file from managed content (S3 like blob store).
 
         :param key: The path of the file to retrieve.
         :type key: str
         :param retries: Number of times to retry a failed request from a response., defaults to 1
         :type retries: int, optional
         :return: A HTTPResponse object
         :rtype: :py:class:`urllib3.response.HTTPResponse`
         """
-        res = tenacity.Retrying(
-            stop=tenacity.stop_after_attempt(retries + 1),
-            retry=tenacity.retry_if_exception(
-                ManagedContentClient._http_request_retry_predicate
-            ),
-        )
-        return res.wraps(self._download)(key)
+        return self._download(key, retries)
 
-    def _download(self, key: str):
+    def _download(self, key: str, retries: int = 1):
         uri = self._make_content_uri(key)
-        res = self._serviceconnector.request("GET", uri=uri, stream=True)
+        res = self._serviceconnector.request_with_retry(
+            "GET", uri=uri, stream=True, retries=retries
+        )
         raise_for_status_with_detail(res)
         return res.raw
 
     def exists(self, key: str) -> bool:
         """Check that a file from managed content (S3) exists.
 
         :param key: The path of the file to check.
@@ -205,15 +197,15 @@
 
         :param key: The path of the file to delete
         :type key: str
         :return: A boolean indicating whether the file exists or not.
         :rtype: dict
         """
         uri = self._make_content_uri(key)
-        res = self._serviceconnector.request("DELETE", uri=uri)
+        res = self._serviceconnector.request_with_retry("DELETE", uri=uri, retries=1)
         raise_for_status_with_detail(res)
         return res.json()
 
     def list(self, prefix: str = None, limit: int = -1, skip: int = -1) -> List[dict]:
         """List objects in a project's managed content store
 
         :param prefix:  The key prefix to filter objects with, defaults to None
@@ -229,15 +221,17 @@
         query = {}
         if prefix is not None:
             query["filter"] = prefix
         if limit > 0:
             query["limit"] = limit
         if skip > 0:
             query["skip"] = skip
-        res = self._serviceconnector.request("GET", uri=uri, params=query)
+        res = self._serviceconnector.request_with_retry(
+            "GET", uri=uri, params=query, retries=1
+        )
         raise_for_status_with_detail(res)
         return res.json()
 
     ## Private ##
 
     @staticmethod
     def _http_request_retry_predicate(exception: Exception) -> bool:
```

### Comparing `cortex-python-6.3.1a1/cortex/env.py` & `cortex-python-6.3.1a2/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/exceptions.py` & `cortex-python-6.3.1a2/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/experiment/__init__.py` & `cortex-python-6.3.1a2/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/experiment/local.py` & `cortex-python-6.3.1a2/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/experiment/model.py` & `cortex-python-6.3.1a2/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/experiment/remote.py` & `cortex-python-6.3.1a2/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/message.py` & `cortex-python-6.3.1a2/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/model.py` & `cortex-python-6.3.1a2/cortex/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/properties.py` & `cortex-python-6.3.1a2/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/secrets.py` & `cortex-python-6.3.1a2/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/serviceconnector.py` & `cortex-python-6.3.1a2/cortex/serviceconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,53 +84,54 @@
             body=data,
             headers=headers_to_send,
             allow_redirects=False,
             verify=self.verify_ssl_cert,
         )
 
     def request_with_retry(
-        self, method, uri, body=None, headers=None, debug=False, **kwargs
+        self, method, uri, body=None, headers=None, debug=False, retries=2, **kwargs
     ):
         """
         Sends a request to the specified URI. Auto retry with backoff on 50x errors
 
         :param method: HTTP method to send to the service.
         :param uri: Path to extend service URL.
         :param body: Data to send as the post body to the service.
         :param headers: HTTP headers for this post.
         :param debug: Enable debug True|False (default: False)
+        :param retries: defaults to 2
         :param kwargs: Additional key-value pairs to pass to the request method.
         :return: :class:`Response <Response>` object
         """
         headers_to_send = self._construct_headers(headers)
         url = self._construct_url(uri)
         if debug:
             log.debug("START {} {}".format("GET", uri))
-        res = ServiceConnector.requests_retry_session().request(
+        res = ServiceConnector.requests_retry_session(retries=retries).request(
             method,
             url,
             data=body,
             allow_redirects=False,
             headers=headers_to_send,
             verify=self.verify_ssl_cert,
             **kwargs,
         )
         if debug:
             log.debug("  END {} {}".format("GET", uri))
         return res
 
     def request(
         self,
-        method,
-        uri,
-        body=None,
-        headers=None,
-        debug=False,
-        is_internal_url=False,
-        **kwargs,
+        method: str,
+        uri: str,
+        body: object = None,
+        headers: object = None,
+        debug: bool = False,
+        is_internal_url: bool = False,
+        **kwargs: dict,
     ):
         """
         Sends a request to the specified URI.
 
         :param method: HTTP method to send to the service.
         :param uri: Path to extend service URL.
         :param body: Data to send as the post body to the service.
```

### Comparing `cortex-python-6.3.1a1/cortex/session.py` & `cortex-python-6.3.1a2/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/skill.py` & `cortex-python-6.3.1a2/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/timer.py` & `cortex-python-6.3.1a2/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/types.py` & `cortex-python-6.3.1a2/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex/utils.py` & `cortex-python-6.3.1a2/cortex/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 import json
 import base64
 import hashlib
 import logging
 import urllib.parse
 from collections import namedtuple
-import datetime
+from datetime import datetime, timedelta, timezone
 from pathlib import Path
+
 import python_jwt as py_jwt
 import jwcrypto.jwk as jwkLib
 from requests.exceptions import HTTPError
-from tenacity import RetryCallState
+from requests import request
 from .exceptions import BadTokenException, AuthenticationHeaderError
 
 
 def md5sum(file_name, blocksize=65536):
     """
     Computes md5sum on a fileself.
 
@@ -136,32 +137,53 @@
     try:
         decode_JWT(token)
         return token
     except py_jwt._JWTError:  # pylint: disable=protected-access
         return generate_token(config)
 
 
+def _get_fabric_info(config: dict):
+    uri = config.get("url") + "/fabric/v4/info"
+    headers = {"Content-Type": "application/json"}
+    return request("GET", uri, headers=headers).json()
+
+
+def _get_fabric_server_ts(config: dict):
+    return _get_fabric_info(config).get("serverTs")
+
+
 def generate_token(config, validity=2):
     """
     Use the Personal Access Token (JWK) obtained from Cortex's console
     to generate JWTs to access cortex services..
     """
     try:
+        server_ts = int(
+            _get_fabric_server_ts(config) / 1000
+        )  # fabric info returns serverTs in milliseconds
         key = jwkLib.JWK.from_json(json.dumps(config.get("jwk")))
         token_payload = {
             "iss": config.get("issuer"),
             "aud": config.get("audience"),
             "sub": config.get("username"),
+            "iat": server_ts / 1000,
         }
+
+        server_ts_dt = datetime.fromtimestamp(server_ts, tz=timezone.utc)
+
+        expiry = server_ts_dt + timedelta(minutes=validity)
+
         token = py_jwt.generate_jwt(
             claims=token_payload,
             priv_key=key,
             algorithm="EdDSA",
-            lifetime=datetime.timedelta(minutes=validity),
-            other_headers={"kid": key.thumbprint()},
+            expires=expiry,
+            other_headers={
+                "kid": key.thumbprint(),
+            },
         )
         return token
     except Exception as err:
         gen_token_msg = (
             "Unable to generate a JWT token, " "check PAT config or cortex profile: {}"
         ).format(err)
         raise BadTokenException(gen_token_msg) from err
@@ -247,28 +269,7 @@
     """
     parse a given string and apply common encoding/substitution rules
     :param string: the string to parse
     :return:
     """
     # Replaces special characters like / with %2F (URL encoding)
     return urllib.parse.quote(string, safe="")
-
-
-def generic_retry_before_handler(retry_state: RetryCallState):
-    """Helper to track the status of retries using tenacity
-
-    :param retry_state: This is passed in by tenacity
-    :type retry_state: :class:`tenacity.RetryCallState`
-    """
-    if retry_state.attempt_number < 1:
-        loglevel = logging.INFO
-    else:
-        loglevel = logging.WARNING
-
-    log_message(
-        msg=(
-            f"Retrying {retry_state.fn}: attempt {retry_state.attempt_number} "
-            f"ended with: {retry_state.outcome}"
-        ),
-        log=get_logger("http_status"),
-        level=loglevel,
-    )
```

### Comparing `cortex-python-6.3.1a1/cortex/viz.py` & `cortex-python-6.3.1a2/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/cortex_python.egg-info/PKG-INFO` & `cortex-python-6.3.1a2/cortex_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a1
+Version: 6.3.1a2
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a1/cortex_python.egg-info/SOURCES.txt` & `cortex-python-6.3.1a2/cortex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/setup.py` & `cortex-python-6.3.1a2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,18 @@
     },
     platforms=["any"],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "requests>=2.12.4,<3",
         "requests-toolbelt>=0.8.0",
-        "python-jwt>=3.3.0,<4.0",
-        "pyyaml>=5.3.1,<6",
+        "pyyaml>=5.3.1",
+        "python-dateutil>=2.8.0,<3",
+        "python-jwt>=3.3.5,<4.0",
         "cuid>=0.3,<1",
-        "tenacity>=8.0,<9.0",
         "dill>=0.2.8.2",
     ],
     extras_require={
         "viz": ["matplotlib>=2.2.2,<3", "seaborn>=0.9.0,<0.10", "pandas"],
         "jupyter": ["ipython>=6.4.0,<7", "maya>=0.5.0", "jinja2"],
     },
     tests_require=["mocket>=3.9.0,<4.0", "pytest>=7.2.1,<8"],
```

### Comparing `cortex-python-6.3.1a1/test/__init__.py` & `cortex-python-6.3.1a2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/test/unit/__init__.py` & `cortex-python-6.3.1a2/test/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/test/unit/authenticationclient_test.py` & `cortex-python-6.3.1a2/test/unit/authenticationclient_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,33 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import unittest
 
+from mocket import mocketize
+
 from cortex.auth import AuthenticationClient
 from cortex.utils import decode_JWT, verify_JWT
-from .fixtures import mock_pat_config, mock_api_endpoint
+from .fixtures import mock_pat_config, mock_api_endpoint, register_mock_fabric_info
 
 
 class TestAuthenticationClient(unittest.TestCase):
     def setUp(self):
+        register_mock_fabric_info()
         self.ac = AuthenticationClient()
 
+    @mocketize
     def test_contructor_with_args(self):
         # This client doesn't need parameters, but allow them for backward compat
         ac = AuthenticationClient(mock_api_endpoint(), 4)
         jwt = ac.fetch_auth_token(mock_pat_config())
 
+    @mocketize
     def test_fetch_auth_token(self):
         # setup
         # uri = self.ac.URIs['authenticate'].format(projectId='cogscale')
         # url = self.ac._serviceconnector._construct_url(uri)
         body = mock_pat_config()
         # Entry.single_register(Entry.POST,
         #                       url,
@@ -41,11 +46,12 @@
         # execute
         # todo mock this call?..
         token = self.ac.fetch_auth_token(body)
         # test
         decodedbody = decode_JWT(token)
         self.assertEqual(body["issuer"], decodedbody[1]["iss"])
 
+    @mocketize
     def test_expired_token(self):
         # Shouldn't fail to validate expired token WITHIN the python lib, this is responsibiltiy of auth proxy...
         exp_token = "eyJhbGciOiJFZERTQSIsImtpZCI6IkhwVy15YTdGU1U3eVYtYWx6eWV3UFBEd1BlRmdya2kwVlFQS2JoNEo0UHciLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJjb3J0ZXgiLCJleHAiOjE2MzAzNDgxOTYsImlhdCI6MTYzMDM0ODE2NiwiaXNzIjoiY29nbml0aXZlc2NhbGUuY29tIiwianRpIjoiU0dkRjVidG1fUXlYcjZhMVRrOU9oZyIsIm5iZiI6MTYzMDM0ODE2Niwic3ViIjoiNzFhOGZhYWMtOWRmYi00MjhkLWE5MGMtMGI1MzQ4MWI4NjY1In0.pB7hvEcIMV1Qt6GTGPGcKbS1zhidPMJ-luV-KBOaHrwgCh2jDOQdve2Sv5RqmNa6Jkk-Bxh-1g4XG8CxGGSqAQ"
         verify_JWT(exp_token)
```

### Comparing `cortex-python-6.3.1a1/test/unit/connectionclient_test.py` & `cortex-python-6.3.1a2/test/unit/connectionclient_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,24 @@
 from mocket.mockhttp import Entry
 from mocket import mocketize
 
 from cortex.connection import ConnectionClient
 from cortex.content import ManagedContentClient
 from cortex import Cortex
 
-from .fixtures import john_doe_token
+from .fixtures import john_doe_token, mock_api_endpoint, mock_project
 
+projectId = mock_project()
+url = mock_api_endpoint()
 TOKEN = john_doe_token()
-projectId = "cogscale"
-url = "http://127.0.0.1:123"
-
-# params similar to those passed from
-params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
 
 
 class TestConnectionClient(unittest.TestCase):
     def setUp(self):
+        params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
         self.cc = ConnectionClient(url, token=TOKEN, project=projectId)
         self.mc = ManagedContentClient(url, token=TOKEN, project=projectId)
         self.client = Cortex.from_message(params)
         self.mcFromClient = ManagedContentClient(self.client)
 
     @mocketize
     def test_save_connection(self):
```

### Comparing `cortex-python-6.3.1a1/test/unit/cortex_test.py` & `cortex-python-6.3.1a2/test/unit/cortex_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 from cortex.experiment import ExperimentClient, Experiment
 from cortex.model import ModelClient, Model
 from cortex.secrets import SecretsClient, Secret
 from cortex.session import SessionClient, Session
 from cortex.types import TypeClient, Type
 from cortex.skill import SkillClient, Skill
 
-from .fixtures import john_doe_subject, john_doe_token
+from .fixtures import john_doe_subject, john_doe_token, mock_api_endpoint
 
 token = john_doe_token()
-api_endpoint = "https://api.test.cortex"
+api_endpoint = mock_api_endpoint()
 api_version = 4
 
 
 class TestCortex(unittest.TestCase):
     def test_client(self):
         account = "unittest"
         cortex = Cortex.client(
```

### Comparing `cortex-python-6.3.1a1/test/unit/environment_config_test.py` & `cortex-python-6.3.1a2/test/unit/environment_config_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a1/test/unit/experiment_test.py` & `cortex-python-6.3.1a2/test/unit/experiment_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 import os
 
 from cortex import Cortex
 from cortex.experiment import ExperimentClient, Experiment
 
 from mocket.mockhttp import Entry
 from mocket import mocketize
-from .fixtures import mock_pat_config, build_mock_url, mock_api_endpoint
+from .fixtures import mock_api_endpoint, mock_project
 from .fixtures import john_doe_token
 
 import dill
 
-# PROJECT = 'expproj'
 TOKEN = john_doe_token()
-projectId = "cogscale"
-url = "http://127.0.0.1:123"
+projectId = mock_project()
+url = mock_api_endpoint()
 params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
 
 
 class TestExperiment(unittest.TestCase):
     """
     Test experiment checks experiment functionality
     """
```

### Comparing `cortex-python-6.3.1a1/test/unit/run_test.py` & `cortex-python-6.3.1a2/test/unit/run_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,33 @@
 from mocket import mocketize
 
 from pytest import raises
 from requests.exceptions import HTTPError
 
 from cortex import Cortex
 from cortex.experiment import ExperimentClient, RemoteRun, Experiment
-from .fixtures import mock_pat_config, build_mock_url, mock_api_endpoint
+from .fixtures import build_mock_url, mock_api_endpoint, mock_project, john_doe_token
 
-PROJECT = "runproj"
+PROJECT = mock_project()
+TOKEN = john_doe_token()
+url = mock_api_endpoint()
 
 
 class TestRun(unittest.TestCase):
     """
     Test experiment checks experiment functionality
     """
 
     RUN_EXP_NAME = "unittest-exp"
     RUN_ID = "000001"
 
     def setUp(self):
+        params = {"token": TOKEN, "projectId": PROJECT, "apiEndpoint": url}
         self.local = Cortex.local()
-        self.cortex = Cortex.client(
-            api_endpoint=mock_api_endpoint(), config=mock_pat_config(), project=PROJECT
-        )
+        self.cortex = Cortex.from_message(params)
 
         # register mock for getting an experiment from the client
         uri = ExperimentClient.URIs["experiment"].format(
             experimentName=self.RUN_EXP_NAME, projectId=PROJECT
         )
         returns = {"name": self.RUN_EXP_NAME}
         Entry.single_register(
```

### Comparing `cortex-python-6.3.1a1/test/unit/serviceconnector_test.py` & `cortex-python-6.3.1a2/test/unit/serviceconnector_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,41 +12,43 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import json
 from mocket.mockhttp import Entry
-from test.unit import fixtures
 from mocket import mocketize
 import requests
 from cortex import __version__
 from cortex.serviceconnector import ServiceConnector
 
-URL = "http://1.2.3.4:80"
+from .fixtures import mock_api_endpoint, john_doe_token
+
+URL = mock_api_endpoint()
 VERSION = 4
+TOKEN = john_doe_token()
 
 
 def test__init__():
-    s = ServiceConnector(URL, VERSION, config=fixtures.mock_pat_config())
+    s = ServiceConnector(URL, VERSION, token=TOKEN)
 
     assert s.url == URL
     assert s.version == VERSION
 
 
 def test__construct_url():
-    sc = ServiceConnector(URL, VERSION, config=fixtures.mock_pat_config())
+    sc = ServiceConnector(URL, VERSION, token=TOKEN)
     r = sc._construct_url("abc")
-    expect = "http://1.2.3.4:80/fabric/v4/{}".format("abc")
+    expect = "http://127.0.0.1:8000/fabric/v4/{}".format("abc")
     assert r == expect
 
 
 @mocketize
 def test_request():
-    sc = ServiceConnector(URL, VERSION, config=fixtures.mock_pat_config())
+    sc = ServiceConnector(URL, VERSION, token=TOKEN)
     path = "models/events"
     url = sc._construct_url(path)
     body = {"handle": 123}
     useragentfragment = f"cortex-python/{__version__}"
     Entry.single_register(Entry.POST, url, status=200, body=json.dumps(body))
     r = sc.request("POST", path, body)
```

### Comparing `cortex-python-6.3.1a1/test/unit/sessionclient_test.py` & `cortex-python-6.3.1a2/test/unit/sessionclient_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import json
 import unittest
 import uuid
-from test.unit import fixtures
 from mocket.mockhttp import Entry
 from mocket import mocketize
 
 from cortex.session import SessionClient
 from cortex import Cortex
 
-TOKEN = fixtures.john_doe_token()
-projectId = "cogscale"
-url = "http://127.0.0.1:123"
-params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
+from .fixtures import john_doe_token, mock_api_endpoint, mock_project
+
+projectId = mock_project()
+url = mock_api_endpoint()
+TOKEN = john_doe_token()
 
 
 class TestSessionClient(unittest.TestCase):
     def setUp(self):
+        params = {"token": TOKEN, "projectId": projectId, "apiEndpoint": url}
         self.client = SessionClient(Cortex.from_message(params))
         self.session_id = str(uuid.uuid4())
 
     def register_entry(self, verb, uri, body):
         url = self.client._serviceconnector._construct_url(uri)
         Entry.single_register(verb, url, status=200, body=json.dumps(body))
```

