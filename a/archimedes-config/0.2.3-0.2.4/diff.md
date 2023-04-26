# Comparing `tmp/archimedes_config-0.2.3.tar.gz` & `tmp/archimedes_config-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_config-0.2.3.tar", max compression
+gzip compressed data, was "archimedes_config-0.2.4.tar", max compression
```

## Comparing `archimedes_config-0.2.3.tar` & `archimedes_config-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/__init__.py
--rw-r--r--   0        0        0     7834 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/arckeyl.py
--rw-r--r--   0        0        0    13575 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/config_manager.py
--rw-r--r--   0        0        0     2308 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/keyvault_client.py
--rw-r--r--   0        0        0     1242 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/keyvault_config_manager.py
--rw-r--r--   0        0        0     1311 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/utils/path_utils.py
--rw-r--r--   0        0        0     3898 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/utils/util.py
--rw-r--r--   0        0        0      673 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/workflows/add_secrets.py
--rw-r--r--   0        0        0      965 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/workflows/lock_secrets.py
--rw-r--r--   0        0        0     2127 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/workflows/secret_creation.py
--rw-r--r--   0        0        0      944 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/workflows/unlock_secrets.py
--rw-r--r--   0        0        0     4126 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/archimedes_config/workflows/workflow_base.py
--rw-r--r--   0        0        0      753 2023-03-30 12:25:05.351456 archimedes_config-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      188 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/__init__.py
+-rw-r--r--   0        0        0     7834 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/arckeyl.py
+-rw-r--r--   0        0        0    13575 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/config_manager.py
+-rw-r--r--   0        0        0     2308 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/keyvault_client.py
+-rw-r--r--   0        0        0     1242 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/keyvault_config_manager.py
+-rw-r--r--   0        0        0     1311 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/utils/path_utils.py
+-rw-r--r--   0        0        0     3898 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/utils/util.py
+-rw-r--r--   0        0        0      673 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/add_secrets.py
+-rw-r--r--   0        0        0      965 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/lock_secrets.py
+-rw-r--r--   0        0        0     2127 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/secret_creation.py
+-rw-r--r--   0        0        0      944 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/unlock_secrets.py
+-rw-r--r--   0        0        0     4126 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/archimedes_config/workflows/workflow_base.py
+-rw-r--r--   0        0        0      753 2023-04-26 14:18:28.347622 archimedes_config-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.2.4/PKG-INFO
```

### Comparing `archimedes_config-0.2.3/archimedes_config/arckeyl.py` & `archimedes_config-0.2.4/archimedes_config/arckeyl.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/config_manager.py` & `archimedes_config-0.2.4/archimedes_config/config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/keyvault_client.py` & `archimedes_config-0.2.4/archimedes_config/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/keyvault_config_manager.py` & `archimedes_config-0.2.4/archimedes_config/keyvault_config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/utils/path_utils.py` & `archimedes_config-0.2.4/archimedes_config/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/utils/util.py` & `archimedes_config-0.2.4/archimedes_config/utils/util.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/workflows/add_secrets.py` & `archimedes_config-0.2.4/archimedes_config/workflows/add_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/workflows/lock_secrets.py` & `archimedes_config-0.2.4/archimedes_config/workflows/lock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/workflows/secret_creation.py` & `archimedes_config-0.2.4/archimedes_config/workflows/secret_creation.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/workflows/unlock_secrets.py` & `archimedes_config-0.2.4/archimedes_config/workflows/unlock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/archimedes_config/workflows/workflow_base.py` & `archimedes_config-0.2.4/archimedes_config/workflows/workflow_base.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.2.3/pyproject.toml` & `archimedes_config-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archimedes-config"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["BigyaPradhan <bigya.pradhan@optimeering.com>"]
 packages = [{include = "archimedes_config"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 cryptography = "^39.0.1"
```

### Comparing `archimedes_config-0.2.3/PKG-INFO` & `archimedes_config-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archimedes-config
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: BigyaPradhan
 Author-email: bigya.pradhan@optimeering.com
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

