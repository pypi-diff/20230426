# Comparing `tmp/grai_source_flat_file-0.0.7.tar.gz` & `tmp/grai_source_flat_file-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_flat_file-0.0.7.tar", max compression
+gzip compressed data, was "grai_source_flat_file-0.0.8.tar", max compression
```

## Comparing `grai_source_flat_file-0.0.7.tar` & `grai_source_flat_file-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      713 2023-04-17 19:09:03.818104 grai_source_flat_file-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.7/src/grai_source_flat_file/__init__.py
--rw-r--r--   0        0        0     4323 2023-04-17 19:09:03.818263 grai_source_flat_file-0.0.7/src/grai_source_flat_file/adapters.py
--rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.7/src/grai_source_flat_file/base.py
--rw-r--r--   0        0        0     2029 2023-04-17 19:09:03.818417 grai_source_flat_file-0.0.7/src/grai_source_flat_file/loader.py
--rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.7/src/grai_source_flat_file/models.py
--rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.7/src/grai_source_flat_file/package_definitions.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.7/setup.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      713 2023-04-26 17:55:43.262066 grai_source_flat_file-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.8/src/grai_source_flat_file/__init__.py
+-rw-r--r--   0        0        0     4437 2023-04-26 17:55:43.262318 grai_source_flat_file-0.0.8/src/grai_source_flat_file/adapters.py
+-rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.8/src/grai_source_flat_file/base.py
+-rw-r--r--   0        0        0     2029 2023-04-17 19:49:39.123184 grai_source_flat_file-0.0.8/src/grai_source_flat_file/loader.py
+-rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.8/src/grai_source_flat_file/models.py
+-rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.8/src/grai_source_flat_file/package_definitions.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.8/setup.py
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.8/PKG-INFO
```

### Comparing `grai_source_flat_file-0.0.7/pyproject.toml` & `grai_source_flat_file-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_flat_file"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_flat_file", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_flat_file-0.0.7/src/grai_source_flat_file/adapters.py` & `grai_source_flat_file-0.0.8/src/grai_source_flat_file/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,37 @@
     data = {
         "version": version,
         "node_type": NodeTypeLabels.column.value,
         "node_attributes": {
             "data_type": current.data_type,
             "is_nullable": current.is_nullable,
         },
+        "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_node(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     data = {
         "version": version,
         "node_type": NodeTypeLabels.table.value,
         "node_attributes": {},
+        "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> TableToColumnMetadata:
     data = {
         "version": version,
+        "tags": [config.metadata_id],
     }
     return TableToColumnMetadata(edge_type=EdgeTypeLabels.table_to_column.value, **data)
 
 
 @multimethod
 def build_app_metadata(current: Any, desired: Any) -> None:
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
```

### Comparing `grai_source_flat_file-0.0.7/src/grai_source_flat_file/base.py` & `grai_source_flat_file-0.0.8/src/grai_source_flat_file/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.7/src/grai_source_flat_file/loader.py` & `grai_source_flat_file-0.0.8/src/grai_source_flat_file/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.7/src/grai_source_flat_file/models.py` & `grai_source_flat_file-0.0.8/src/grai_source_flat_file/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.7/setup.py` & `grai_source_flat_file-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'grai-schemas>=0.1.10,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pandas>=1.4.4,<2.0.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-flat-file',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_flat_file-0.0.7/PKG-INFO` & `grai_source_flat_file-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-flat-file
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

