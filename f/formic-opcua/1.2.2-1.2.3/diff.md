# Comparing `tmp/formic_opcua-1.2.2.tar.gz` & `tmp/formic_opcua-1.2.3.tar.gz`

## Comparing `formic_opcua-1.2.2.tar` & `formic_opcua-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/core/parse.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.2.3/PKG-INFO
```

### Comparing `formic_opcua-1.2.2/.pre-commit-config.yaml` & `formic_opcua-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/examples/opcua_client.py` & `formic_opcua-1.2.3/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.2.3/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.2.3/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.2.3/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.2.3/formic_opcua/client/async_opcua_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         except (KeyError, IndexError):
             logger.warning(f'Unable to get node {path} from client map {self._node_map}')
             return None
         try:
             value = await node.read_value()
             logger.info(f'Read value {value} from path {path}')
             return value
-        except ConnectionError as e:
+        except Exception as e:
             logger.warning(f'{e}')
             logger.warning(f'Unable to read node at {path}')
         return None
 
     async def read(self, path: str) -> Any:
         logger.info(f'Attempting to read path {path}.')
         if not self._has_connected:  # Read attempt has failed or client never connected.
```

### Comparing `formic_opcua-1.2.2/formic_opcua/client/opcua_client.py` & `formic_opcua-1.2.3/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/core/parse.py` & `formic_opcua-1.2.3/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/core/type_conversions.py` & `formic_opcua-1.2.3/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.2.3/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.2.3/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/formic_opcua/server/opcua_server.py` & `formic_opcua-1.2.3/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/hooks/add_issue_prefix.py` & `formic_opcua-1.2.3/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/tests/test_server_config.py` & `formic_opcua-1.2.3/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/.gitignore` & `formic_opcua-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.2.2/pyproject.toml` & `formic_opcua-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

