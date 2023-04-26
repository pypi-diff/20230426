# Comparing `tmp/pydbtools-5.5.3.tar.gz` & `tmp/pydbtools-5.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbtools-5.5.3.tar", max compression
+gzip compressed data, was "pydbtools-5.5.4.tar", max compression
```

## Comparing `pydbtools-5.5.3.tar` & `pydbtools-5.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9632 2023-03-06 18:39:44.542284 pydbtools-5.5.3/README.md
--rw-r--r--   0        0        0      855 2023-03-06 18:39:44.546284 pydbtools-5.5.3/pydbtools/__init__.py
--rw-r--r--   0        0        0     1130 2023-03-06 18:39:44.546284 pydbtools-5.5.3/pydbtools/_sql_render.py
--rw-r--r--   0        0        0    23104 2023-03-06 18:39:44.546284 pydbtools-5.5.3/pydbtools/_wrangler.py
--rw-r--r--   0        0        0     6391 2023-03-06 18:39:44.546284 pydbtools-5.5.3/pydbtools/utils.py
--rw-r--r--   0        0        0      647 2023-03-06 18:39:44.546284 pydbtools-5.5.3/pyproject.toml
--rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 pydbtools-5.5.3/PKG-INFO
+-rw-r--r--   0        0        0     9632 2023-04-26 15:04:22.979736 pydbtools-5.5.4/README.md
+-rw-r--r--   0        0        0      855 2023-04-26 15:04:22.983736 pydbtools-5.5.4/pydbtools/__init__.py
+-rw-r--r--   0        0        0     1130 2023-04-26 15:04:22.983736 pydbtools-5.5.4/pydbtools/_sql_render.py
+-rw-r--r--   0        0        0    23104 2023-04-26 15:04:22.983736 pydbtools-5.5.4/pydbtools/_wrangler.py
+-rw-r--r--   0        0        0     6421 2023-04-26 15:04:22.983736 pydbtools-5.5.4/pydbtools/utils.py
+-rw-r--r--   0        0        0      647 2023-04-26 15:04:22.983736 pydbtools-5.5.4/pyproject.toml
+-rw-r--r--   0        0        0    10475 1970-01-01 00:00:00.000000 pydbtools-5.5.4/PKG-INFO
```

### Comparing `pydbtools-5.5.3/README.md` & `pydbtools-5.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.3/pydbtools/__init__.py` & `pydbtools-5.5.4/pydbtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     create_table,
 )
 
 from ._sql_render import get_sql_from_file, render_sql_template  # noqa: F401
 
 from .utils import s3_path_join  # noqa: F401
 
-__version__ = "5.5.3"
+__version__ = "5.5.4"
```

### Comparing `pydbtools-5.5.3/pydbtools/_sql_render.py` & `pydbtools-5.5.4/pydbtools/_sql_render.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.3/pydbtools/_wrangler.py` & `pydbtools-5.5.4/pydbtools/_wrangler.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.3/pydbtools/utils.py` & `pydbtools-5.5.4/pydbtools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     if out_path[-1] != "/":
         out_path += "/"
 
     return (sts_resp["UserId"], out_path)
 
 
 def get_database_name_from_userid(user_id: str) -> str:
-    unique_db_name = user_id.split(":")[-1].split("-", 1)[-1].replace("-", "_")
+    unique_db_name = "".join(
+        x for x in user_id.split(":")[-1].split("@", 1)[0] if x.isalnum()
+    )
     unique_db_name = temp_database_name_prefix + unique_db_name
     return unique_db_name
 
 
 def get_database_name_from_sql(sql: str) -> str:
     """
     Obtains database name from SQL query for use
```

### Comparing `pydbtools-5.5.3/pyproject.toml` & `pydbtools-5.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool]
 [tool.poetry]
 name = "pydbtools"
-version = "5.5.3"
+version = "5.5.4"
 description = "A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler."
 license = "MIT"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11" # wrangler dependency
 boto3 = ">=1.7.4"
-sqlparse = "^0.4.1"
-awswrangler = "^2.12.0"
+sqlparse = "^0.4.4"
+awswrangler = "^2.15.0"
 pyarrow = ">=5.0.0"
 Jinja2 = ">=3.1.0"
 sql-metadata = "^2.3.0"
 arrow-pd-parser = "^1.3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.1"
```

### Comparing `pydbtools-5.5.3/PKG-INFO` & `pydbtools-5.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pydbtools
-Version: 5.5.3
+Version: 5.5.4
 Summary: A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler.
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.0)
 Requires-Dist: arrow-pd-parser (>=1.3.7,<2.0.0)
-Requires-Dist: awswrangler (>=2.12.0,<3.0.0)
+Requires-Dist: awswrangler (>=2.15.0,<3.0.0)
 Requires-Dist: boto3 (>=1.7.4)
 Requires-Dist: pyarrow (>=5.0.0)
 Requires-Dist: sql-metadata (>=2.3.0,<3.0.0)
-Requires-Dist: sqlparse (>=0.4.1,<0.5.0)
+Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Description-Content-Type: text/markdown
 
 # pydbtools
 
 A package that is used to run SQL queries speficially configured for the Analytical Platform. This packages uses AWS Wrangler's Athena module but adds additional functionality (like Jinja templating, creating temporary tables) and alters some configuration to our specification. 
 
 ## Installation
```

