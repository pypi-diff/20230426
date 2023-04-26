# Comparing `tmp/grai_source_redshift-0.0.3.tar.gz` & `tmp/grai_source_redshift-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.3.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.0.4.tar", max compression
```

## Comparing `grai_source_redshift-0.0.3.tar` & `grai_source_redshift-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      775 2023-04-25 00:54:43.259686 grai_source_redshift-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      145 2023-04-19 18:45:33.558481 grai_source_redshift-0.0.3/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     6562 2023-04-24 23:00:41.807746 grai_source_redshift-0.0.3/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1185 2023-04-25 00:59:25.399992 grai_source_redshift-0.0.3/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     7181 2023-04-25 00:57:39.596347 grai_source_redshift-0.0.3/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     4369 2023-04-24 21:21:13.073883 grai_source_redshift-0.0.3/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      186 2023-04-20 05:30:43.838248 grai_source_redshift-0.0.3/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.3/setup.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      777 2023-04-26 17:55:43.265533 grai_source_redshift-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-04-25 21:23:43.339413 grai_source_redshift-0.0.4/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     6668 2023-04-26 17:55:43.265767 grai_source_redshift-0.0.4/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1185 2023-04-25 21:23:43.339552 grai_source_redshift-0.0.4/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     7181 2023-04-25 21:23:43.339626 grai_source_redshift-0.0.4/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     4369 2023-04-25 21:23:43.339688 grai_source_redshift-0.0.4/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      186 2023-04-25 21:23:43.339739 grai_source_redshift-0.0.4/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.4/setup.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.4/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.3/pyproject.toml` & `grai_source_redshift-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  [tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 [tool.poetry.dependencies]
@@ -19,17 +19,17 @@
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 types-psycopg2 = "^2.9.18"
 pytest = "^7.2.0"
 
-   [tool.isort]
+    [tool.isort]
 profile = "black"
 known_first_party = "grai_source_redshift"
 
-   [tool.black]
+    [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grai_source_redshift-0.0.3/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.0.4/src/grai_source_redshift/adapters.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,33 +49,35 @@
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

### Comparing `grai_source_redshift-0.0.3/src/grai_source_redshift/base.py` & `grai_source_redshift-0.0.4/src/grai_source_redshift/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.3/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.0.4/src/grai_source_redshift/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.3/src/grai_source_redshift/models.py` & `grai_source_redshift-0.0.4/src/grai_source_redshift/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.3/setup.py` & `grai_source_redshift-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'grai-schemas>=0.1.5,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic[dotenv]>=1.10.7,<2.0.0',
  'redshift-connector>=2.0.910,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-redshift',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_redshift-0.0.3/PKG-INFO` & `grai_source_redshift-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

