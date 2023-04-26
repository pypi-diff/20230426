# Comparing `tmp/pnap-tag-api-1.0.4.tar.gz` & `tmp/pnap-tag-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-tag-api-1.0.4.tar", last modified: Thu Mar  9 08:59:19 2023, max compression
+gzip compressed data, was "dist/pnap-tag-api-1.0.5.tar", last modified: Tue Apr 25 13:57:56 2023, max compression
```

## Comparing `pnap-tag-api-1.0.4.tar` & `pnap-tag-api-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     5493 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     7309 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api/
--rw-r--r--   0 runner    (1001) docker     (116)    17105 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14821 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    12409 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    14206 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (116)      346 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12342 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/delete_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    13002 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/resource_assignment.py
--rw-r--r--   0 runner    (1001) docker     (116)    13116 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/tag_update.py
--rw-r--r--   0 runner    (1001) docker     (116)    13116 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model/tag_create.py
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39968 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5619 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)    26581 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      213 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)      688 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83144 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      465 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/pnap_tag_api/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1774 2023-03-09 08:59:09.000000 pnap-tag-api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7309 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      728 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:59:19.000000 pnap-tag-api-1.0.4/pnap_tag_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)    26581 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14821 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83144 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14206 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12409 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13116 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/tag_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12342 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/delete_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13116 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/tag_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13002 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/model/resource_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17105 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39968 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/pnap_tag_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7309 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7309 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/pnap_tag_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:57:56.000000 pnap-tag-api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-04-25 13:57:44.000000 pnap-tag-api-1.0.5/setup.py
```

### Comparing `pnap-tag-api-1.0.4/README.md` & `pnap-tag-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/PKG-INFO` & `pnap-tag-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-tag-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tags API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-tag-api
```

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/configuration.py` & `pnap-tag-api-1.0.5/pnap_tag_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/rest.py` & `pnap-tag-api-1.0.5/pnap_tag_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/error.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/tag.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/tag.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/delete_result.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/delete_result.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/resource_assignment.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/resource_assignment.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/tag_update.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/tag_update.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model/tag_create.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model/tag_create.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/__init__.py` & `pnap-tag-api-1.0.5/pnap_tag_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/api_client.py` & `pnap-tag-api-1.0.5/pnap_tag_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/exceptions.py` & `pnap-tag-api-1.0.5/pnap_tag_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/api/tags_api.py` & `pnap-tag-api-1.0.5/pnap_tag_api/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/models/__init__.py` & `pnap-tag-api-1.0.5/pnap_tag_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api/model_utils.py` & `pnap-tag-api-1.0.5/pnap_tag_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/setup.py` & `pnap-tag-api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api.egg-info/PKG-INFO` & `pnap-tag-api-1.0.5/pnap_tag_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-tag-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tags API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-tag-api
```

### Comparing `pnap-tag-api-1.0.4/pnap_tag_api.egg-info/SOURCES.txt` & `pnap-tag-api-1.0.5/pnap_tag_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

