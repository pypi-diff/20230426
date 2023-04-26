# Comparing `tmp/discovery-connectors-1.4.1.tar.gz` & `tmp/discovery-connectors-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-connectors-1.4.1.tar", last modified: Mon Apr 24 14:04:14 2023, max compression
+gzip compressed data, was "discovery-connectors-1.4.2.tar", last modified: Tue Apr 25 21:48:55 2023, max compression
```

## Comparing `discovery-connectors-1.4.1.tar` & `discovery-connectors-1.4.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.430725 discovery-connectors-1.4.1/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-24 14:04:14.430903 discovery-connectors-1.4.1/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.417939 discovery-connectors-1.4.1/discovery_connectors.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1019 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      197 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.418499 discovery-connectors-1.4.1/ds_connectors/
--rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/ds_connectors/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.423198 discovery-connectors-1.4.1/ds_connectors/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.1/ds_connectors/handlers/cortex_helpers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/hive_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mc_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5089 2023-04-24 14:03:48.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mongodb_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mysql_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/postgres_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/redis_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15587 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/s3_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.423872 discovery-connectors-1.4.1/ds_connectors/parsers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/parsers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/parsers/dsv.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-24 14:04:14.431527 discovery-connectors-1.4.1/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2354 2023-04-24 14:03:48.000000 discovery-connectors-1.4.1/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.411323 discovery-connectors-1.4.1/tests/
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.425118 discovery-connectors-1.4.1/tests/aws/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/aws/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/aws/s3_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.426004 discovery-connectors-1.4.1/tests/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.1/tests/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.427015 discovery-connectors-1.4.1/tests/managed_content/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.1/tests/managed_content/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.1/tests/managed_content/mc_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.428431 discovery-connectors-1.4.1/tests/mongodb/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/tests/mongodb/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8334 2023-04-24 14:02:17.000000 discovery-connectors-1.4.1/tests/mongodb/mongodb_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.429697 discovery-connectors-1.4.1/tests/mysql/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.1/tests/mysql/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8825 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/tests/mysql/mysql_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.430277 discovery-connectors-1.4.1/tests/po1/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/po1/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.200615 discovery-connectors-1.4.2/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-25 21:48:55.200808 discovery-connectors-1.4.2/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.188116 discovery-connectors-1.4.2/discovery_connectors.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-25 21:48:55.000000 discovery-connectors-1.4.2/discovery_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1023 2023-04-25 21:48:55.000000 discovery-connectors-1.4.2/discovery_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-25 21:48:55.000000 discovery-connectors-1.4.2/discovery_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      197 2023-04-25 21:48:55.000000 discovery-connectors-1.4.2/discovery_connectors.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-25 21:48:55.000000 discovery-connectors-1.4.2/discovery_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.188535 discovery-connectors-1.4.2/ds_connectors/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-24 14:04:41.000000 discovery-connectors-1.4.2/ds_connectors/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.194317 discovery-connectors-1.4.2/ds_connectors/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.2/ds_connectors/handlers/cortex_helpers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/handlers/hive_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.2/ds_connectors/handlers/mc_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5089 2023-04-24 14:03:48.000000 discovery-connectors-1.4.2/ds_connectors/handlers/mongodb_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.2/ds_connectors/handlers/mysql_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    16117 2023-04-25 21:47:33.000000 discovery-connectors-1.4.2/ds_connectors/handlers/old_s3_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/handlers/postgres_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/handlers/redis_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.195030 discovery-connectors-1.4.2/ds_connectors/parsers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/parsers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/ds_connectors/parsers/dsv.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-25 21:48:55.201456 discovery-connectors-1.4.2/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2354 2023-04-24 14:03:48.000000 discovery-connectors-1.4.2/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.184153 discovery-connectors-1.4.2/tests/
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.195751 discovery-connectors-1.4.2/tests/aws/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/tests/aws/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/tests/aws/s3_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.196303 discovery-connectors-1.4.2/tests/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.2/tests/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.196889 discovery-connectors-1.4.2/tests/managed_content/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.2/tests/managed_content/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.2/tests/managed_content/mc_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.197798 discovery-connectors-1.4.2/tests/mongodb/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-24 14:02:30.000000 discovery-connectors-1.4.2/tests/mongodb/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8334 2023-04-24 14:02:17.000000 discovery-connectors-1.4.2/tests/mongodb/mongodb_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.199134 discovery-connectors-1.4.2/tests/mysql/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.2/tests/mysql/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8825 2023-04-24 14:02:30.000000 discovery-connectors-1.4.2/tests/mysql/mysql_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-25 21:48:55.200079 discovery-connectors-1.4.2/tests/po1/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.2/tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.4.1/LICENSE.txt` & `discovery-connectors-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/PKG-INFO` & `discovery-connectors-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.1
+Version: 1.4.2
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.4.1/discovery_connectors.egg-info/PKG-INFO` & `discovery-connectors-1.4.2/discovery_connectors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.1
+Version: 1.4.2
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-connectors-1.4.1/discovery_connectors.egg-info/SOURCES.txt` & `discovery-connectors-1.4.2/discovery_connectors.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ds_connectors/__init__.py
 ds_connectors/handlers/__init__.py
 ds_connectors/handlers/cortex_helpers.py
 ds_connectors/handlers/hive_handlers.py
 ds_connectors/handlers/mc_handlers.py
 ds_connectors/handlers/mongodb_handlers.py
 ds_connectors/handlers/mysql_handlers.py
+ds_connectors/handlers/old_s3_handlers.py
 ds_connectors/handlers/postgres_handlers.py
 ds_connectors/handlers/redis_handlers.py
-ds_connectors/handlers/s3_handlers.py
 ds_connectors/parsers/__init__.py
 ds_connectors/parsers/dsv.py
 tests/aws/__init__.py
 tests/aws/s3_handler_test.py
 tests/handlers/__init__.py
 tests/managed_content/__init__.py
 tests/managed_content/mc_handler_test.py
```

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/cortex_helpers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/cortex_helpers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/hive_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/hive_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/mc_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/mc_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/mongodb_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/mongodb_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/mysql_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/mysql_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/postgres_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/postgres_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/redis_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/redis_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/ds_connectors/handlers/s3_handlers.py` & `discovery-connectors-1.4.2/ds_connectors/handlers/old_s3_handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-import threading
-from io import StringIO, BytesIO
-import pandas as pd
-import pickle
-import json
-import os
-
-from aistac.handlers.abstract_handlers import AbstractSourceHandler, ConnectorContract, AbstractPersistHandler, \
-    HandlerFactory
-
-__author__ = 'Darryl Oatridge'
-
-
-class S3SourceHandler(AbstractSourceHandler):
-    """ An Amazon AWS S3 source handler.
-
-        URI Format:
-            uri = 's3://<bucket>[/<path>]/<filename.ext>'
-
-        Restrictions:
-            - This does not use the AWS S3 Multipart Upload and is limited to 5GB files
-    """
-
-    def __init__(self, connector_contract: ConnectorContract):
-        """ initialise the Handler passing the connector_contract dictionary
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - region_name (optional) session region name
-            - profile_name (optional) session shared credentials file profile name
-        """
-        self.botocore = HandlerFactory.get_module('botocore.exceptions')
-        self.boto3 = HandlerFactory.get_module('boto3')
-        super().__init__(connector_contract)
-        cc_params = connector_contract.kwargs
-        cc_params.update(connector_contract.query)  # Update kwargs with those in the uri query
-        region_name = cc_params.pop('region_name', 'us-east-2')
-        aws_access_key_id = cc_params.pop('aws_access_key_id', os.environ.get('AWS_ACCESS_KEY_ID'))
-        aws_secret_access_key = cc_params.pop('aws_secret_access_key', os.environ.get('AWS_SECRET_ACCESS_KEY'))
-        aws_session_token = cc_params.pop('aws_session_token', os.environ.get('AWS_SESSION_TOKEN'))
-        profile_name = cc_params.pop('profile_name', None)
-        self._session = self.boto3.Session(region_name=region_name, aws_access_key_id=aws_access_key_id,
-                                           aws_secret_access_key=aws_secret_access_key, profile_name=profile_name,
-                                           aws_session_token=aws_session_token)
-        self._file_state = 0
-        self._changed_flag = True
-
-    def supported_types(self) -> list:
-        """ The source types supported with this module"""
-        return ['parquet', 'csv', 'tsv', 'txt', 'json', 'pickle']
-
-    def exists(self) -> bool:
-        """ Returns True is the file exists
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - s3_list_params: (optional) a dictionary of additional s3 parameters directly passed to 'list_objects_v2'
-
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The S3 Source Connector Contract has not been set correctly")
-        _cc = self.connector_contract
-        if not isinstance(_cc, ConnectorContract):
-            raise ValueError("The Python Source Connector Contract has not been set correctly")
-        cc_params = _cc.kwargs
-        cc_params.update(_cc.query)  # Update kwargs with those in the uri query
-        s3_list_params = cc_params.pop('s3_list_params', {})
-        if _cc.schema not in ['s3']:
-            raise ValueError("The Connector Contract Schema has not been set correctly.")
-        s3_client = self._session.client(_cc.schema)
-        response = s3_client.list_objects_v2(Bucket=_cc.netloc, **s3_list_params)
-        for obj in response.get('Contents', []):
-            if obj['Key'] == _cc.path[1:]:
-                return True
-        return False
-
-    def has_changed(self) -> bool:
-        """ returns if the file has been modified
-
-            - s3_get_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The S3 Source Connector Contract has not been set correctly")
-        _cc = self.connector_contract
-        if not isinstance(_cc, ConnectorContract):
-            raise ValueError("The Python Source Connector Contract has not been set correctly")
-        cc_params = _cc.kwargs
-        cc_params.update(_cc.query)  # Update kwargs with those in the uri query
-        # pop all the extra params
-        s3_get_params = cc_params.pop('s3_get_params', {})
-        if _cc.schema not in ['s3']:
-            raise ValueError("The Connector Contract Schema has not been set correctly.")
-        s3_client = self._session.client(_cc.schema)
-        try:
-            s3_object = s3_client.get_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_get_params)
-        except self.botocore.ClientError as e:
-            code = e.response["Error"]["Code"]
-            raise ConnectionError("Failed to retrieve the object from region '{}', bucket '{}' "
-                                  "Key '{}' with error code '{}'".format(self._session.region_name, _cc.netloc,
-                                                                         _cc.path[1:], code))
-        state = s3_object.get('LastModified', 0)
-        if state != self._file_state:
-            self._changed_flag = True
-            self._file_state = state
-        return self._changed_flag
-
-    def reset_changed(self, changed: bool = False):
-        """ manual reset to say the file has been seen. This is automatically called if the file is loaded"""
-        changed = changed if isinstance(changed, bool) else False
-        self._changed_flag = changed
-
-    def load_canonical(self, **kwargs) -> [pd.DataFrame, dict]:
-        """Loads the canonical dataset, returning a Pandas DataFrame. This method utilises the pandas
-        'pd.read_' methods and directly passes the kwargs to these methods.
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - file_type: (optional) the type of the source file. if not set, inferred from the file extension
-                            by default json files load as dict, to load as pandas use read_params '{as_dataframe: True}
-            - encoding: (optional) the encoding of the s3 object body. Default 'utf-8'
-            - s3_get_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
-            - read_params: (optional) value pair dict of parameters to pass to the read methods. Underlying
-                           read methods the parameters are passed to are all pandas 'read_*', e.g. pd.read_csv
-
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The S3 Source Connector Contract has not been set correctly")
-        _cc = self.connector_contract
-        if not isinstance(_cc, ConnectorContract):
-            raise ValueError("The Python Source Connector Contract has not been set correctly")
-        _, _, _ext = _cc.address.rpartition('.')
-        cc_params = _cc.kwargs
-        cc_params.update(_cc.query)  # Update kwargs with those in the uri query
-        cc_params.update(kwargs)     # Update with any passed though the call
-        # pop all the extra params
-        encoding = cc_params.pop('encoding', 'utf-8')
-        file_type = cc_params.pop('file_type', _ext if len(_ext) > 0 else 'pickle')
-        s3_get_params = cc_params.pop('s3_get_params', {})
-        read_params = cc_params.pop('read_params', {})
-        if file_type.lower() not in self.supported_types():
-            raise ValueError("The file type {} is not recognised. "
-                             "Set file_type parameter to a recognised source type".format(file_type))
-        # session
-        if _cc.schema not in ['s3']:
-            raise ValueError("The Connector Contract Schema has not been set correctly.")
-        s3_client = self._session.client(_cc.schema)
-        try:
-            s3_object = s3_client.get_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_get_params)
-        except self.botocore.ClientError as e:
-            code = e.response["Error"]["Code"]
-            raise ConnectionError("Failed to retrieve the object from region '{}', bucket '{}' "
-                                  "Key '{}' with error code '{}'".format(self._session.region_name, _cc.netloc,
-                                                                         _cc.path[1:], code))
-        resource_body = s3_object['Body'].read()
-        with threading.Lock():
-            if file_type.lower() in ['parquet', 'pq', 'pqt']:
-                return pd.read_parquet(BytesIO(resource_body), **read_params)
-            if file_type.lower() in ['csv', 'tsv', 'txt']:
-                return pd.read_csv(StringIO(resource_body.decode(encoding)), **read_params)
-            if file_type.lower() in ['json']:
-                as_dataframe = read_params.pop('as_dataframe', False)
-                if as_dataframe:
-                    return pd.read_json(StringIO(resource_body.decode(encoding)), **read_params)
-                return json.load(StringIO(resource_body.decode(encoding)), **read_params)
-            if file_type.lower() in ['pkl ', 'pickle']:
-                fix_imports = read_params.pop('fix_imports', True)
-                encoding = read_params.pop('encoding', 'ASCII')
-                errors = read_params.pop('errors', 'strict')
-                return pickle.loads(resource_body, fix_imports=fix_imports, encoding=encoding, errors=errors)
-        raise LookupError('The source format {} is not currently supported'.format(file_type))
-
-
-class S3PersistHandler(S3SourceHandler, AbstractPersistHandler):
-    """ An Amazon AWS S3 source handler.
-
-        URI Format:
-            uri = 's3://<bucket>[/<path>]/<filename.ext>'
-
-        Restrictions:
-            - This does not use the AWS S3 Multipart Upload and is limited to 5GB files
-    """
-
-    def persist_canonical(self, canonical: [pd.DataFrame, dict], **kwargs) -> bool:
-        """ persists either the canonical dataset.
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - file_type: (optional) the type of the source file. if not set, inferred from the file extension
-            - s3_put_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
-            - write_params: (optional) value pair dict of parameters to pass to the write methods - pandas.to_csv,
-                              pandas.to_json, pickle.dump and parquet.Table.from_pandas
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            return False
-        _uri = self.connector_contract.address
-        return self.backup_canonical(uri=_uri, canonical=canonical, **kwargs)
-
-    def backup_canonical(self, canonical: [pd.DataFrame, dict], uri: str, **kwargs) -> bool:
-        """ persists the canonical dataset as a backup to the specified URI resource. Note that only the
-        address is taken from the URI and all other attributes are taken from the ConnectorContract
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - file_type: (optional) the type of the source file. if not set, inferred from the file extension
-            - s3_put_params: (optional) value pair dict of parameters to pass to the Boto3 put_object method
-            - write_params: (optional) value pair dict of parameters to pass to the write methods - pandas.to_csv,
-                              pandas.to_json, pickle.dump and parquet.Table.from_pandas
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The S3 Source Connector Contract has not been set correctly")
-        _cc = self.connector_contract
-        if not isinstance(_cc, ConnectorContract):
-            raise ValueError("The Python Source Connector Contract has not been set correctly")
-        schema, bucket, path = _cc.parse_address_elements(uri=uri)
-        _, _, _ext = path.rpartition('.')
-        cc_params = kwargs if isinstance(kwargs, dict) else _cc.kwargs
-        cc_params.update(_cc.parse_query(uri=uri))
-        # pop all the extra params
-        s3_put_params = cc_params.pop('s3_put_params', _cc.kwargs.get('put_object_kw', {}))
-        write_params = cc_params.pop('write_params', _cc.kwargs.get('write_kw', {}))
-        file_type = cc_params.pop('file_type', _cc.kwargs.get('file_type', _ext if len(_ext) > 0 else 'pkl'))
-        if _cc.schema not in ['s3']:
-            raise ValueError("The Connector Contract Schema has not been set correctly.")
-        s3_client = self._session.client(_cc.schema)
-        # csv
-        if file_type.lower() in ['csv', 'tsv', 'txt']:
-            byte_obj = StringIO()
-            _mode = write_params.pop('mode', 'wb')
-            _index = write_params.pop('index', False)
-            with threading.Lock():
-                canonical.to_csv(byte_obj, mode=_mode, index=_index, **write_params)
-                s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj.getvalue(), **s3_put_params)
-        # pickle
-        elif file_type.lower() in ['pkl ', 'pickle']:
-            _protocol = write_params.pop('protocol', pickle.HIGHEST_PROTOCOL)
-            _fix_imports = write_params.pop('fix_imports', True)
-            with threading.Lock():
-                byte_obj = pickle.dumps(canonical, protocol=_protocol, fix_imports=_fix_imports)
-                s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj, **s3_put_params)
-        # json
-        elif file_type.lower() in ['json']:
-            byte_obj = StringIO()
-            with threading.Lock():
-                if isinstance(canonical, pd.DataFrame):
-                    canonical.to_json(byte_obj, **write_params)
-                    body = byte_obj.getvalue()
-                else:
-                    encode = write_params.pop('encode', 'UTF-8')
-                    body = (bytes(json.dumps(canonical, **s3_put_params).encode(encode)))
-                s3_client.put_object(Bucket=bucket, Key=path[1:], Body=body, **s3_put_params)
-        # parquet
-        elif file_type.lower() in ['parquet', 'pq', 'pqt']:
-            _index = write_params.pop('index', False)
-            byte_obj = BytesIO()
-            with threading.Lock():
-                # table = pa.Table.from_pandas(df=canonical, **write_params)
-                canonical.to_parquet(byte_obj, index=_index, **write_params)
-                s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj.getvalue(), **s3_put_params)
-        else:
-            raise LookupError('The source format {} is not currently supported for write'.format(file_type))
-        return True
-
-    def remove_canonical(self) -> bool:
-        """ removes the URI named resource
-
-        Extra Parameters in the ConnectorContract kwargs:
-            - s3_del_params: (optional) value pair dict of parameters to pass to the Boto3 delete_object method
-        """
-        if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The S3 Source Connector Contract has not been set correctly")
-        _cc = self.connector_contract
-        if not isinstance(_cc, ConnectorContract):
-            raise ValueError("The Python Source Connector Contract has not been set correctly")
-        cc_params = _cc.kwargs
-        cc_params.update(_cc.query)  # Update kwargs with those in the uri query
-        # pop all the extra params
-        s3_del_params = cc_params.pop('s3_put_params', _cc.kwargs.get('put_object_kw', {}))
-        if _cc.schema not in ['s3']:
-            raise ValueError("The Connector Contract Schema has not been set correctly.")
-        s3_client = self._session.client(_cc.schema)
-        response = s3_client.response = s3_client.delete_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_del_params)
-        if response.get('RequestCharged') is None:
-            return False
-        return True
+# import threading
+# from io import StringIO, BytesIO
+# import pandas as pd
+# import pickle
+# import json
+# import os
+#
+# from aistac.handlers.abstract_handlers import AbstractSourceHandler, ConnectorContract, AbstractPersistHandler, \
+#     HandlerFactory
+#
+# __author__ = 'Darryl Oatridge'
+#
+#
+# class S3SourceHandler(AbstractSourceHandler):
+#     """ An Amazon AWS S3 source handler.
+#
+#         URI Format:
+#             uri = 's3://<bucket>[/<path>]/<filename.ext>'
+#
+#         Restrictions:
+#             - This does not use the AWS S3 Multipart Upload and is limited to 5GB files
+#     """
+#
+#     def __init__(self, connector_contract: ConnectorContract):
+#         """ initialise the Handler passing the connector_contract dictionary
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - region_name (optional) session region name
+#             - profile_name (optional) session shared credentials file profile name
+#         """
+#         self.botocore = HandlerFactory.get_module('botocore.exceptions')
+#         self.boto3 = HandlerFactory.get_module('boto3')
+#         super().__init__(connector_contract)
+#         cc_params = connector_contract.kwargs
+#         cc_params.update(connector_contract.query)  # Update kwargs with those in the uri query
+#         region_name = cc_params.pop('region_name', 'us-east-2')
+#         aws_access_key_id = cc_params.pop('aws_access_key_id', os.environ.get('AWS_ACCESS_KEY_ID'))
+#         aws_secret_access_key = cc_params.pop('aws_secret_access_key', os.environ.get('AWS_SECRET_ACCESS_KEY'))
+#         aws_session_token = cc_params.pop('aws_session_token', os.environ.get('AWS_SESSION_TOKEN'))
+#         profile_name = cc_params.pop('profile_name', None)
+#         self._session = self.boto3.Session(region_name=region_name, aws_access_key_id=aws_access_key_id,
+#                                            aws_secret_access_key=aws_secret_access_key, profile_name=profile_name,
+#                                            aws_session_token=aws_session_token)
+#         self._file_state = 0
+#         self._changed_flag = True
+#
+#     def supported_types(self) -> list:
+#         """ The source types supported with this module"""
+#         return ['parquet', 'csv', 'tsv', 'txt', 'json', 'pickle']
+#
+#     def exists(self) -> bool:
+#         """ Returns True is the file exists
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - s3_list_params: (optional) a dictionary of additional s3 parameters directly passed to 'list_objects_v2'
+#
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             raise ValueError("The S3 Source Connector Contract has not been set correctly")
+#         _cc = self.connector_contract
+#         if not isinstance(_cc, ConnectorContract):
+#             raise ValueError("The Python Source Connector Contract has not been set correctly")
+#         cc_params = _cc.kwargs
+#         cc_params.update(_cc.query)  # Update kwargs with those in the uri query
+#         s3_list_params = cc_params.pop('s3_list_params', {})
+#         if _cc.schema not in ['s3']:
+#             raise ValueError("The Connector Contract Schema has not been set correctly.")
+#         s3_client = self._session.client(_cc.schema)
+#         response = s3_client.list_objects_v2(Bucket=_cc.netloc, **s3_list_params)
+#         for obj in response.get('Contents', []):
+#             if obj['Key'] == _cc.path[1:]:
+#                 return True
+#         return False
+#
+#     def has_changed(self) -> bool:
+#         """ returns if the file has been modified
+#
+#             - s3_get_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             raise ValueError("The S3 Source Connector Contract has not been set correctly")
+#         _cc = self.connector_contract
+#         if not isinstance(_cc, ConnectorContract):
+#             raise ValueError("The Python Source Connector Contract has not been set correctly")
+#         cc_params = _cc.kwargs
+#         cc_params.update(_cc.query)  # Update kwargs with those in the uri query
+#         # pop all the extra params
+#         s3_get_params = cc_params.pop('s3_get_params', {})
+#         if _cc.schema not in ['s3']:
+#             raise ValueError("The Connector Contract Schema has not been set correctly.")
+#         s3_client = self._session.client(_cc.schema)
+#         try:
+#             s3_object = s3_client.get_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_get_params)
+#         except self.botocore.ClientError as e:
+#             code = e.response["Error"]["Code"]
+#             raise ConnectionError("Failed to retrieve the object from region '{}', bucket '{}' "
+#                                   "Key '{}' with error code '{}'".format(self._session.region_name, _cc.netloc,
+#                                                                          _cc.path[1:], code))
+#         state = s3_object.get('LastModified', 0)
+#         if state != self._file_state:
+#             self._changed_flag = True
+#             self._file_state = state
+#         return self._changed_flag
+#
+#     def reset_changed(self, changed: bool = False):
+#         """ manual reset to say the file has been seen. This is automatically called if the file is loaded"""
+#         changed = changed if isinstance(changed, bool) else False
+#         self._changed_flag = changed
+#
+#     def load_canonical(self, **kwargs) -> [pd.DataFrame, dict]:
+#         """Loads the canonical dataset, returning a Pandas DataFrame. This method utilises the pandas
+#         'pd.read_' methods and directly passes the kwargs to these methods.
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - file_type: (optional) the type of the source file. if not set, inferred from the file extension
+#                             by default json files load as dict, to load as pandas use read_params '{as_dataframe: True}
+#             - encoding: (optional) the encoding of the s3 object body. Default 'utf-8'
+#             - s3_get_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
+#             - read_params: (optional) value pair dict of parameters to pass to the read methods. Underlying
+#                            read methods the parameters are passed to are all pandas 'read_*', e.g. pd.read_csv
+#
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             raise ValueError("The S3 Source Connector Contract has not been set correctly")
+#         _cc = self.connector_contract
+#         if not isinstance(_cc, ConnectorContract):
+#             raise ValueError("The Python Source Connector Contract has not been set correctly")
+#         _, _, _ext = _cc.address.rpartition('.')
+#         cc_params = _cc.kwargs
+#         cc_params.update(_cc.query)  # Update kwargs with those in the uri query
+#         cc_params.update(kwargs)     # Update with any passed though the call
+#         # pop all the extra params
+#         encoding = cc_params.pop('encoding', 'utf-8')
+#         file_type = cc_params.pop('file_type', _ext if len(_ext) > 0 else 'pickle')
+#         s3_get_params = cc_params.pop('s3_get_params', {})
+#         read_params = cc_params.pop('read_params', {})
+#         if file_type.lower() not in self.supported_types():
+#             raise ValueError("The file type {} is not recognised. "
+#                              "Set file_type parameter to a recognised source type".format(file_type))
+#         # session
+#         if _cc.schema not in ['s3']:
+#             raise ValueError("The Connector Contract Schema has not been set correctly.")
+#         s3_client = self._session.client(_cc.schema)
+#         try:
+#             s3_object = s3_client.get_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_get_params)
+#         except self.botocore.ClientError as e:
+#             code = e.response["Error"]["Code"]
+#             raise ConnectionError("Failed to retrieve the object from region '{}', bucket '{}' "
+#                                   "Key '{}' with error code '{}'".format(self._session.region_name, _cc.netloc,
+#                                                                          _cc.path[1:], code))
+#         resource_body = s3_object['Body'].read()
+#         with threading.Lock():
+#             if file_type.lower() in ['parquet', 'pq', 'pqt']:
+#                 return pd.read_parquet(BytesIO(resource_body), **read_params)
+#             if file_type.lower() in ['csv', 'tsv', 'txt']:
+#                 return pd.read_csv(StringIO(resource_body.decode(encoding)), **read_params)
+#             if file_type.lower() in ['json']:
+#                 as_dataframe = read_params.pop('as_dataframe', False)
+#                 if as_dataframe:
+#                     return pd.read_json(StringIO(resource_body.decode(encoding)), **read_params)
+#                 return json.load(StringIO(resource_body.decode(encoding)), **read_params)
+#             if file_type.lower() in ['pkl ', 'pickle']:
+#                 fix_imports = read_params.pop('fix_imports', True)
+#                 encoding = read_params.pop('encoding', 'ASCII')
+#                 errors = read_params.pop('errors', 'strict')
+#                 return pickle.loads(resource_body, fix_imports=fix_imports, encoding=encoding, errors=errors)
+#         raise LookupError('The source format {} is not currently supported'.format(file_type))
+#
+#
+# class S3PersistHandler(S3SourceHandler, AbstractPersistHandler):
+#     """ An Amazon AWS S3 source handler.
+#
+#         URI Format:
+#             uri = 's3://<bucket>[/<path>]/<filename.ext>'
+#
+#         Restrictions:
+#             - This does not use the AWS S3 Multipart Upload and is limited to 5GB files
+#     """
+#
+#     def persist_canonical(self, canonical: [pd.DataFrame, dict], **kwargs) -> bool:
+#         """ persists either the canonical dataset.
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - file_type: (optional) the type of the source file. if not set, inferred from the file extension
+#             - s3_put_params: (optional) a dictionary of additional s3 client parameters directly passed to 'get_object'
+#             - write_params: (optional) value pair dict of parameters to pass to the write methods - pandas.to_csv,
+#                               pandas.to_json, pickle.dump and parquet.Table.from_pandas
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             return False
+#         _uri = self.connector_contract.address
+#         return self.backup_canonical(uri=_uri, canonical=canonical, **kwargs)
+#
+#     def backup_canonical(self, canonical: [pd.DataFrame, dict], uri: str, **kwargs) -> bool:
+#         """ persists the canonical dataset as a backup to the specified URI resource. Note that only the
+#         address is taken from the URI and all other attributes are taken from the ConnectorContract
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - file_type: (optional) the type of the source file. if not set, inferred from the file extension
+#             - s3_put_params: (optional) value pair dict of parameters to pass to the Boto3 put_object method
+#             - write_params: (optional) value pair dict of parameters to pass to the write methods - pandas.to_csv,
+#                               pandas.to_json, pickle.dump and parquet.Table.from_pandas
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             raise ValueError("The S3 Source Connector Contract has not been set correctly")
+#         _cc = self.connector_contract
+#         if not isinstance(_cc, ConnectorContract):
+#             raise ValueError("The Python Source Connector Contract has not been set correctly")
+#         schema, bucket, path = _cc.parse_address_elements(uri=uri)
+#         _, _, _ext = path.rpartition('.')
+#         cc_params = kwargs if isinstance(kwargs, dict) else _cc.kwargs
+#         cc_params.update(_cc.parse_query(uri=uri))
+#         # pop all the extra params
+#         s3_put_params = cc_params.pop('s3_put_params', _cc.kwargs.get('put_object_kw', {}))
+#         write_params = cc_params.pop('write_params', _cc.kwargs.get('write_kw', {}))
+#         file_type = cc_params.pop('file_type', _cc.kwargs.get('file_type', _ext if len(_ext) > 0 else 'pkl'))
+#         if _cc.schema not in ['s3']:
+#             raise ValueError("The Connector Contract Schema has not been set correctly.")
+#         s3_client = self._session.client(_cc.schema)
+#         # csv
+#         if file_type.lower() in ['csv', 'tsv', 'txt']:
+#             byte_obj = StringIO()
+#             _mode = write_params.pop('mode', 'wb')
+#             _index = write_params.pop('index', False)
+#             with threading.Lock():
+#                 canonical.to_csv(byte_obj, mode=_mode, index=_index, **write_params)
+#                 s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj.getvalue(), **s3_put_params)
+#         # pickle
+#         elif file_type.lower() in ['pkl ', 'pickle']:
+#             _protocol = write_params.pop('protocol', pickle.HIGHEST_PROTOCOL)
+#             _fix_imports = write_params.pop('fix_imports', True)
+#             with threading.Lock():
+#                 byte_obj = pickle.dumps(canonical, protocol=_protocol, fix_imports=_fix_imports)
+#                 s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj, **s3_put_params)
+#         # json
+#         elif file_type.lower() in ['json']:
+#             byte_obj = StringIO()
+#             with threading.Lock():
+#                 if isinstance(canonical, pd.DataFrame):
+#                     canonical.to_json(byte_obj, **write_params)
+#                     body = byte_obj.getvalue()
+#                 else:
+#                     encode = write_params.pop('encode', 'UTF-8')
+#                     body = (bytes(json.dumps(canonical, **s3_put_params).encode(encode)))
+#                 s3_client.put_object(Bucket=bucket, Key=path[1:], Body=body, **s3_put_params)
+#         # parquet
+#         elif file_type.lower() in ['parquet', 'pq', 'pqt']:
+#             _index = write_params.pop('index', False)
+#             byte_obj = BytesIO()
+#             with threading.Lock():
+#                 # table = pa.Table.from_pandas(df=canonical, **write_params)
+#                 canonical.to_parquet(byte_obj, index=_index, **write_params)
+#                 s3_client.put_object(Bucket=bucket, Key=path[1:], Body=byte_obj.getvalue(), **s3_put_params)
+#         else:
+#             raise LookupError('The source format {} is not currently supported for write'.format(file_type))
+#         return True
+#
+#     def remove_canonical(self) -> bool:
+#         """ removes the URI named resource
+#
+#         Extra Parameters in the ConnectorContract kwargs:
+#             - s3_del_params: (optional) value pair dict of parameters to pass to the Boto3 delete_object method
+#         """
+#         if not isinstance(self.connector_contract, ConnectorContract):
+#             raise ValueError("The S3 Source Connector Contract has not been set correctly")
+#         _cc = self.connector_contract
+#         if not isinstance(_cc, ConnectorContract):
+#             raise ValueError("The Python Source Connector Contract has not been set correctly")
+#         cc_params = _cc.kwargs
+#         cc_params.update(_cc.query)  # Update kwargs with those in the uri query
+#         # pop all the extra params
+#         s3_del_params = cc_params.pop('s3_put_params', _cc.kwargs.get('put_object_kw', {}))
+#         if _cc.schema not in ['s3']:
+#             raise ValueError("The Connector Contract Schema has not been set correctly.")
+#         s3_client = self._session.client(_cc.schema)
+#         response = s3_client.response = s3_client.delete_object(Bucket=_cc.netloc, Key=_cc.path[1:], **s3_del_params)
+#         if response.get('RequestCharged') is None:
+#             return False
+#         return True
```

### Comparing `discovery-connectors-1.4.1/ds_connectors/parsers/dsv.py` & `discovery-connectors-1.4.2/ds_connectors/parsers/dsv.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/setup.py` & `discovery-connectors-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/tests/aws/s3_handler_test.py` & `discovery-connectors-1.4.2/tests/aws/s3_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/tests/managed_content/mc_handler_test.py` & `discovery-connectors-1.4.2/tests/managed_content/mc_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/tests/mongodb/mongodb_handler_test.py` & `discovery-connectors-1.4.2/tests/mongodb/mongodb_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.1/tests/mysql/mysql_handler_test.py` & `discovery-connectors-1.4.2/tests/mysql/mysql_handler_test.py`

 * *Files identical despite different names*

