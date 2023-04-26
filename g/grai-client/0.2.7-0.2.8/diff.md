# Comparing `tmp/grai_client-0.2.7.tar.gz` & `tmp/grai_client-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.2.7.tar", max compression
+gzip compressed data, was "grai_client-0.2.8.tar", max compression
```

## Comparing `grai_client-0.2.7.tar` & `grai_client-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      771 2023-04-17 19:08:37.025212 grai_client-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       78 2023-02-13 20:16:22.660883 grai_client-0.2.7/src/grai_client/__init__.py
--rw-r--r--   0        0        0     1344 2023-02-13 20:16:22.661185 grai_client-0.2.7/src/grai_client/authentication.py
--rw-r--r--   0        0        0      210 2023-02-13 20:16:22.661271 grai_client-0.2.7/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0     8706 2023-04-17 19:08:37.025349 grai_client-0.2.7/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0      286 2023-04-17 19:08:37.025448 grai_client-0.2.7/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     2640 2023-04-17 19:08:37.025545 grai_client-0.2.7/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.2.7/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     2514 2023-04-17 19:08:37.025648 grai_client-0.2.7/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0      931 2023-04-17 19:08:37.025740 grai_client-0.2.7/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0     7796 2023-04-17 19:08:37.025852 grai_client-0.2.7/src/grai_client/endpoints/v1/get.py
--rw-r--r--   0        0        0     1780 2023-04-17 19:08:37.025956 grai_client-0.2.7/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     1338 2023-04-17 19:08:37.026055 grai_client-0.2.7/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0      976 2023-03-13 20:23:41.240223 grai_client-0.2.7/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0      948 2023-04-17 19:08:37.026173 grai_client-0.2.7/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.2.7/src/grai_client/py.typed
--rw-r--r--   0        0        0       58 2023-02-13 20:16:22.662870 grai_client-0.2.7/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0      218 2023-02-13 20:16:22.662940 grai_client-0.2.7/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      329 2023-02-13 20:16:22.663042 grai_client-0.2.7/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0      111 2023-02-13 20:16:22.663106 grai_client-0.2.7/src/grai_client/schemas/workspace.py
--rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.2.7/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     2907 2023-02-13 20:16:22.663262 grai_client-0.2.7/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     1375 2023-02-13 20:16:22.663339 grai_client-0.2.7/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.2.7/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      529 2023-04-10 17:14:23.662254 grai_client-0.2.7/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 grai_client-0.2.7/setup.py
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 grai_client-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      773 2023-04-26 15:32:49.411692 grai_client-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-02-13 20:16:22.660883 grai_client-0.2.8/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-26 15:19:51.604530 grai_client-0.2.8/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      210 2023-02-13 20:16:22.661271 grai_client-0.2.8/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     8706 2023-04-17 19:21:38.334922 grai_client-0.2.8/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0      286 2023-04-17 19:21:38.335020 grai_client-0.2.8/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     2640 2023-04-17 19:21:38.335218 grai_client-0.2.8/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.2.8/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     2514 2023-04-17 19:21:38.335366 grai_client-0.2.8/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0      931 2023-04-17 19:21:38.335480 grai_client-0.2.8/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0     7796 2023-04-17 19:21:38.335700 grai_client-0.2.8/src/grai_client/endpoints/v1/get.py
+-rw-r--r--   0        0        0     1780 2023-04-17 19:21:38.335803 grai_client-0.2.8/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     1338 2023-04-17 19:21:38.335909 grai_client-0.2.8/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0      976 2023-03-13 20:23:41.240223 grai_client-0.2.8/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0      948 2023-04-17 19:21:38.336104 grai_client-0.2.8/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.2.8/src/grai_client/py.typed
+-rw-r--r--   0        0        0       58 2023-02-13 20:16:22.662870 grai_client-0.2.8/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0      218 2023-02-13 20:16:22.662940 grai_client-0.2.8/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      329 2023-02-13 20:16:22.663042 grai_client-0.2.8/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0      111 2023-02-13 20:16:22.663106 grai_client-0.2.8/src/grai_client/schemas/workspace.py
+-rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.2.8/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     2907 2023-02-13 20:16:22.663262 grai_client-0.2.8/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     1375 2023-04-26 15:19:45.800736 grai_client-0.2.8/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.2.8/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-26 00:38:08.539486 grai_client-0.2.8/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 grai_client-0.2.8/setup.py
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 grai_client-0.2.8/PKG-INFO
```

### Comparing `grai_client-0.2.7/pyproject.toml` & `grai_client-0.2.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 requests = "^2.28.1"
-multimethod = "1.9"
+multimethod = "^1.9"
 orjson = "^3.8.3"
 pyyaml = "^6.0"
-grai-schemas = "^0.1.8"
+grai-schemas = "^0.1.11"
 httpx = "^0.23.3"
 brotli = "^1.0.9"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.971"
 isort = "^5.10.1"
 black = "^22.6.0"
```

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/client.py` & `grai_client-0.2.8/src/grai_client/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/utilities.py` & `grai_client-0.2.8/src/grai_client/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/client.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/get.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/get.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/post.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/post.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/url.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.2.8/src/grai_client/endpoints/v1/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/testing/schema.py` & `grai_client-0.2.8/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/src/grai_client/update.py` & `grai_client-0.2.8/src/grai_client/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional, TypeVar
 
 from grai_schemas.base import Edge, Node
-from grai_schemas.utilities import merge_models
+from grai_schemas.utilities import merge, merge_models
 
 from grai_client.endpoints.client import BaseClient
 
 T = TypeVar("T", Node, Edge)
 
 
 def deactivate(items: List[T]) -> List[T]:
@@ -28,12 +28,12 @@
     new_item_keys = item_map.keys() - current_item_map.keys()
     deactivated_item_keys = current_item_map.keys() - item_map.keys()
     updated_item_keys = item_map.keys() - new_item_keys
 
     deactivated_items = deactivate([current_item_map[k] for k in deactivated_item_keys])
     new_items: List[T] = [item_map[k] for k in new_item_keys]
     updated_items = [
-        merge_models(item_map[k], current_item_map[k]) for k in updated_item_keys if item_map[k] != current_item_map[k]
+        merge(item_map[k], current_item_map[k]) for k in updated_item_keys if item_map[k] != current_item_map[k]
     ]
     # client.patch(deactivated_items)
     client.patch(updated_items)
     client.post(new_items)
```

### Comparing `grai_client-0.2.7/src/grai_client/utilities/tests.py` & `grai_client-0.2.8/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.2.7/setup.py` & `grai_client-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
  'grai_client.utilities']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['brotli>=1.0.9,<2.0.0',
- 'grai-schemas>=0.1.8,<0.2.0',
+ 'grai-schemas>=0.1.11,<0.2.0',
  'httpx>=0.23.3,<0.24.0',
- 'multimethod==1.9',
+ 'multimethod>=1.9,<2.0',
  'orjson>=3.8.3,<4.0.0',
  'pydantic>=1.9.1,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-client',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_client-0.2.7/PKG-INFO` & `grai_client-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
-Requires-Dist: grai-schemas (>=0.1.8,<0.2.0)
+Requires-Dist: grai-schemas (>=0.1.11,<0.2.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: multimethod (==1.9)
+Requires-Dist: multimethod (>=1.9,<2.0)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

