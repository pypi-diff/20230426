# Comparing `tmp/pnap-rancher-solution-api-1.0.4.tar.gz` & `tmp/pnap-rancher-solution-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-rancher-solution-api-1.0.4.tar", last modified: Thu Mar  9 08:59:07 2023, max compression
+gzip compressed data, was "dist/pnap-rancher-solution-api-1.0.5.tar", last modified: Tue Apr 25 13:58:00 2023, max compression
```

## Comparing `pnap-rancher-solution-api-1.0.4.tar` & `pnap-rancher-solution-api-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     5972 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     7849 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1700 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7849 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       26 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/
--rw-r--r--   0 runner    (1001) docker     (116)    17040 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14710 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    17483 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    15332 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    12250 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    11891 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node.py
--rw-r--r--   0 runner    (1001) docker     (116)    13565 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/ssh_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    12699 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_certificates.py
--rw-r--r--   0 runner    (1001) docker     (116)    15840 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)      359 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12326 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/delete_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    15017 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/workload_cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    14153 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)    15748 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node_pool_ssh_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    14962 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_config_certificates.py
--rw-r--r--   0 runner    (1001) docker     (116)    17064 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster_workload_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    13115 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1304 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39929 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5495 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      230 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    21128 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api/clusters_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)     1511 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83033 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:07.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      507 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:58:56.000000 pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     7849 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7849 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1304 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21128 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14710 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83033 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5495 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15332 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12250 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12699 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14153 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12326 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/delete_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13115 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15840 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15017 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/workload_cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14962 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_config_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17483 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster_workload_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15748 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node_pool_ssh_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13565 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/ssh_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11891 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17040 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39929 2023-04-25 13:57:45.000000 pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api_client.py
```

### Comparing `pnap-rancher-solution-api-1.0.4/README.md` & `pnap-rancher-solution-api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/PKG-INFO` & `pnap-rancher-solution-api-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-rancher-solution-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Rancher Solution API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-rancher-solution-api
```

### Comparing `pnap-rancher-solution-api-1.0.4/setup.py` & `pnap-rancher-solution-api-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/PKG-INFO` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-rancher-solution-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Rancher Solution API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-rancher-solution-api
```

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api.egg-info/SOURCES.txt` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/configuration.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/rest.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster_configuration.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_config.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_config.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/error.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/ssh_config.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_certificates.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_certificates.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/delete_result.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/delete_result.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/workload_cluster_config.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/workload_cluster_config.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node_pool.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node_pool.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/node_pool_ssh_config.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/node_pool_ssh_config.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_cluster_config_certificates.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_cluster_config_certificates.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/cluster_workload_configuration.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/cluster_workload_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model/rancher_server_metadata.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model/rancher_server_metadata.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/__init__.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api_client.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/exceptions.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/api/clusters_api.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/models/__init__.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-rancher-solution-api-1.0.4/pnap_rancher_solution_api/model_utils.py` & `pnap-rancher-solution-api-1.0.5/pnap_rancher_solution_api/model_utils.py`

 * *Files identical despite different names*

