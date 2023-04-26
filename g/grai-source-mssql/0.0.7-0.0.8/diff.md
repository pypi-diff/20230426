# Comparing `tmp/grai_source_mssql-0.0.7.tar.gz` & `tmp/grai_source_mssql-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mssql-0.0.7.tar", max compression
+gzip compressed data, was "grai_source_mssql-0.0.8.tar", max compression
```

## Comparing `grai_source_mssql-0.0.7.tar` & `grai_source_mssql-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      685 2023-04-17 19:09:03.819395 grai_source_mssql-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.7/src/grai_source_mssql/__init__.py
--rw-r--r--   0        0        0     6355 2023-04-17 19:09:03.819560 grai_source_mssql-0.0.7/src/grai_source_mssql/adapters.py
--rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.7/src/grai_source_mssql/base.py
--rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.7/src/grai_source_mssql/loader.py
--rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.7/src/grai_source_mssql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.7/src/grai_source_mssql/package_definitions.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.7/setup.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      685 2023-04-26 17:55:43.262699 grai_source_mssql-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.8/src/grai_source_mssql/__init__.py
+-rw-r--r--   0        0        0     6461 2023-04-26 17:55:43.262901 grai_source_mssql-0.0.8/src/grai_source_mssql/adapters.py
+-rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.8/src/grai_source_mssql/base.py
+-rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.8/src/grai_source_mssql/loader.py
+-rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.8/src/grai_source_mssql/models.py
+-rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.8/src/grai_source_mssql/package_definitions.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.8/setup.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.8/PKG-INFO
```

### Comparing `grai_source_mssql-0.0.7/pyproject.toml` & `grai_source_mssql-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_mssql"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mssql", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_mssql-0.0.7/src/grai_source_mssql/adapters.py` & `grai_source_mssql-0.0.8/src/grai_source_mssql/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,33 +48,35 @@
             "data_type": current.data_type,
             "default_value": default_value,
             "is_nullable": None if current.is_nullable else False,  # Only not-nullable is definitive.
             "is_primary_key": current.column_constraint
             and current.column_constraint.value == ColumnConstraint.primary_key.value,
             "is_unique": current.column_constraint and current.column_constraint.value in UNIQUE_COLUMN_CONSTRAINTS,
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

### Comparing `grai_source_mssql-0.0.7/src/grai_source_mssql/base.py` & `grai_source_mssql-0.0.8/src/grai_source_mssql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.7/src/grai_source_mssql/loader.py` & `grai_source_mssql-0.0.8/src/grai_source_mssql/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.7/src/grai_source_mssql/models.py` & `grai_source_mssql-0.0.8/src/grai_source_mssql/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.7/setup.py` & `grai_source_mssql-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'grai-schemas>=0.1.8,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'pyodbc>=4.0.35,<5.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-mssql',
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

### Comparing `grai_source_mssql-0.0.7/PKG-INFO` & `grai_source_mssql-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-mssql
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

