# Comparing `tmp/pnap-ip-api-1.1.3.tar.gz` & `tmp/pnap-ip-api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-ip-api-1.1.3.tar", last modified: Thu Mar  9 08:58:29 2023, max compression
+gzip compressed data, was "dist/pnap-ip-api-1.1.4.tar", last modified: Tue Apr 25 13:57:56 2023, max compression
```

## Comparing `pnap-ip-api-1.1.3.tar` & `pnap-ip-api-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (116)     5953 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     7800 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1676 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7800 2023-03-09 08:58:28.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:58:28.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-09 08:58:28.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      772 2023-03-09 08:58:28.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:58:28.000000 pnap-ip-api-1.1.3/pnap_ip_api.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api/
--rw-r--r--   0 runner    (1001) docker     (116)    16974 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14708 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    12234 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    13203 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/tag_assignment.py
--rw-r--r--   0 runner    (1001) docker     (116)    15729 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block.py
--rw-r--r--   0 runner    (1001) docker     (116)    12309 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/delete_ip_block_result.py
--rw-r--r--   0 runner    (1001) docker     (116)      345 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12992 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/tag_assignment_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    12000 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block_patch.py
--rw-r--r--   0 runner    (1001) docker     (116)    13858 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block_create.py
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39875 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5507 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      216 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    32415 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/api/ip_blocks_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)      786 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83031 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:29.000000 pnap-ip-api-1.1.3/pnap_ip_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      481 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:58:19.000000 pnap-ip-api-1.1.3/pnap_ip_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32415 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/api/ip_blocks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14708 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83031 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5507 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    12309 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/delete_ip_block_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12000 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block_patch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13203 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15729 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13858 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12992 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/model/tag_assignment_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16974 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39875 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/pnap_ip_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:57:56.000000 pnap-ip-api-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1676 2023-04-25 13:57:44.000000 pnap-ip-api-1.1.4/setup.py
```

### Comparing `pnap-ip-api-1.1.3/README.md` & `pnap-ip-api-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/PKG-INFO` & `pnap-ip-api-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-ip-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: IP Addresses API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-ip-api
```

### Comparing `pnap-ip-api-1.1.3/setup.py` & `pnap-ip-api-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api.egg-info/PKG-INFO` & `pnap-ip-api-1.1.4/pnap_ip_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-ip-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: IP Addresses API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-ip-api
```

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api.egg-info/SOURCES.txt` & `pnap-ip-api-1.1.4/pnap_ip_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/configuration.py` & `pnap-ip-api-1.1.4/pnap_ip_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/rest.py` & `pnap-ip-api-1.1.4/pnap_ip_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/error.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/tag_assignment.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/tag_assignment.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/delete_ip_block_result.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/delete_ip_block_result.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/tag_assignment_request.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/tag_assignment_request.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block_patch.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block_patch.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model/ip_block_create.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model/ip_block_create.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/__init__.py` & `pnap-ip-api-1.1.4/pnap_ip_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/api_client.py` & `pnap-ip-api-1.1.4/pnap_ip_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/exceptions.py` & `pnap-ip-api-1.1.4/pnap_ip_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/api/ip_blocks_api.py` & `pnap-ip-api-1.1.4/pnap_ip_api/api/ip_blocks_api.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/models/__init__.py` & `pnap-ip-api-1.1.4/pnap_ip_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-ip-api-1.1.3/pnap_ip_api/model_utils.py` & `pnap-ip-api-1.1.4/pnap_ip_api/model_utils.py`

 * *Files identical despite different names*

