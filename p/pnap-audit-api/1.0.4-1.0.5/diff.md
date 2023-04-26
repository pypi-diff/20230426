# Comparing `tmp/pnap-audit-api-1.0.4.tar.gz` & `tmp/pnap-audit-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-audit-api-1.0.4.tar", last modified: Thu Mar  9 08:51:06 2023, max compression
+gzip compressed data, was "dist/pnap-audit-api-1.0.5.tar", last modified: Tue Apr 25 13:57:59 2023, max compression
```

## Comparing `pnap-audit-api-1.0.4.tar` & `pnap-audit-api-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     5356 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     7128 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api/
--rw-r--r--   0 runner    (1001) docker     (116)    16924 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14648 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    12571 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/event.py
--rw-r--r--   0 runner    (1001) docker     (116)    12177 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    11499 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/headers.py
--rw-r--r--   0 runner    (1001) docker     (116)      348 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12515 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/user_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    12200 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11965 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/api_action_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    11897 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14687 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model/api_action.py
--rw-r--r--   0 runner    (1001) docker     (116)     1154 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39813 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5444 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      217 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8136 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/api/events_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)      518 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    82971 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      477 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/pnap_audit_api/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1613 2023-03-09 08:50:50.000000 pnap-audit-api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:51:06.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7128 2023-03-09 08:51:05.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:51:05.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2023-03-09 08:51:05.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      834 2023-03-09 08:51:05.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:51:05.000000 pnap-audit-api-1.0.4/pnap_audit_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     7128 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7128 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8136 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14648 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82971 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:59.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/api_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12177 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11499 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/headers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12571 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11965 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/api_action_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11897 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12200 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/model/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16924 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39813 2023-04-25 13:57:44.000000 pnap-audit-api-1.0.5/pnap_audit_api/api_client.py
```

### Comparing `pnap-audit-api-1.0.4/README.md` & `pnap-audit-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/PKG-INFO` & `pnap-audit-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-audit-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Audit Log API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-audit-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-audit-api Version: 1.0.4 Summary: Audit Log
+Metadata-Version: 2.1 Name: pnap-audit-api Version: 1.0.5 Summary: Audit Log
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 audit-api The Audit Logs API lets you read audit log entries and track API
 calls or activities in the Bare Metal Cloud Portal.
 
  Knowledge base articles to help you can be found here
```

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/configuration.py` & `pnap-audit-api-1.0.5/pnap_audit_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/rest.py` & `pnap-audit-api-1.0.5/pnap_audit_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/event.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/event.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/error.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/headers.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/headers.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/user_info.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/user_info.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/request.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/request.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/api_action_all_of.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/api_action_all_of.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/response.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/response.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model/api_action.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model/api_action.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/__init__.py` & `pnap-audit-api-1.0.5/pnap_audit_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/api_client.py` & `pnap-audit-api-1.0.5/pnap_audit_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/exceptions.py` & `pnap-audit-api-1.0.5/pnap_audit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/api/events_api.py` & `pnap-audit-api-1.0.5/pnap_audit_api/api/events_api.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/models/__init__.py` & `pnap-audit-api-1.0.5/pnap_audit_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api/model_utils.py` & `pnap-audit-api-1.0.5/pnap_audit_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/setup.py` & `pnap-audit-api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api.egg-info/PKG-INFO` & `pnap-audit-api-1.0.5/pnap_audit_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-audit-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Audit Log API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-audit-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-audit-api Version: 1.0.4 Summary: Audit Log
+Metadata-Version: 2.1 Name: pnap-audit-api Version: 1.0.5 Summary: Audit Log
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 audit-api The Audit Logs API lets you read audit log entries and track API
 calls or activities in the Bare Metal Cloud Portal.
 
  Knowledge base articles to help you can be found here
```

### Comparing `pnap-audit-api-1.0.4/pnap_audit_api.egg-info/SOURCES.txt` & `pnap-audit-api-1.0.5/pnap_audit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

