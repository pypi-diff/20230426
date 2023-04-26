# Comparing `tmp/grai_source_bigquery-0.0.3.tar.gz` & `tmp/grai_source_bigquery-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.0.3.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.0.4.tar", max compression
```

## Comparing `grai_source_bigquery-0.0.3.tar` & `grai_source_bigquery-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      738 2023-04-17 19:09:03.810095 grai_source_bigquery-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.3/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     6553 2023-04-17 19:09:03.810266 grai_source_bigquery-0.0.3/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.3/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.3/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     4778 2023-04-13 22:32:27.123660 grai_source_bigquery-0.0.3/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.3/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.3/setup.py
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-04-26 17:55:43.260206 grai_source_bigquery-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.4/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     6659 2023-04-26 17:55:43.260599 grai_source_bigquery-0.0.4/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.4/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.4/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     4778 2023-04-13 22:32:27.123660 grai_source_bigquery-0.0.4/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.4/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.4/setup.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.4/PKG-INFO
```

### Comparing `grai_source_bigquery-0.0.3/pyproject.toml` & `grai_source_bigquery-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_bigquery-0.0.3/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.0.4/src/grai_source_bigquery/adapters.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,32 +48,34 @@
         "node_attributes": {
             "data_type": current.data_type,
             "default_value": default_value,
             "is_nullable": None if current.is_nullable else False,  # Only not-nullable is definitive.
             # "is_primary_key": current.is_pk, # This is getting a default value right now
             # "is_unique": # Not support in BQ
         },
+        "tags": [config.metadata_id],
     }
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     data = {
         "version": version,
         "node_type": NodeTypeLabels.table.value,
         "node_attributes": {},
+        "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
-    data = {"version": version}
+    data = {"version": version, "tags": [config.metadata_id]}
 
     if isinstance(current.source, TableID):
         if isinstance(current.destination, ColumnID):
             data["edge_type"] = EdgeTypeLabels.table_to_column.value
             return TableToColumnMetadata(**data)
         elif isinstance(current.destination, TableID):
             data["edge_type"] = EdgeTypeLabels.table_to_table.value
```

### Comparing `grai_source_bigquery-0.0.3/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.0.4/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.3/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.0.4/src/grai_source_bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.3/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.0.4/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.3/setup.py` & `grai_source_bigquery-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'grai-schemas>=0.1.9,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'setuptools>=67.1.0,<68.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-bigquery',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': 'None',
     'author': 'Edward Louth',
     'author_email': 'edward@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_bigquery-0.0.3/PKG-INFO` & `grai_source_bigquery-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

