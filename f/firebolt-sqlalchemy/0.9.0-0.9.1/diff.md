# Comparing `tmp/firebolt_sqlalchemy-0.9.0.tar.gz` & `tmp/firebolt_sqlalchemy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firebolt-sqlalchemy/firebolt-sqlalchemy/dist/.tmp-c0s8ia3l/firebolt_sqlalchemy-0.9.0.tar", last modified: Tue Apr 25 14:53:53 2023, max compression
+gzip compressed data, was "/home/runner/work/firebolt-sqlalchemy/firebolt-sqlalchemy/dist/.tmp-3t_hrdk5/firebolt_sqlalchemy-0.9.1.tar", last modified: Tue Apr 25 16:56:59 2023, max compression
```

## Comparing `firebolt_sqlalchemy-0.9.0.tar` & `firebolt_sqlalchemy-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-25 14:53:32.000000 firebolt_sqlalchemy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-25 14:53:32.000000 firebolt_sqlalchemy-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 14:53:32.000000 firebolt_sqlalchemy-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_db/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 14:53:44.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-25 14:53:32.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_db/firebolt_async_dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-04-25 14:53:32.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_db/firebolt_dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 14:53:53.000000 firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-25 16:56:33.000000 firebolt_sqlalchemy-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-25 16:56:33.000000 firebolt_sqlalchemy-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 16:56:33.000000 firebolt_sqlalchemy-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_db/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 16:56:47.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-25 16:56:33.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_db/firebolt_async_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-04-25 16:56:33.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_db/firebolt_dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 16:56:58.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 16:56:59.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:56:58.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 16:56:58.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-25 16:56:58.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 16:56:58.000000 firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/top_level.txt
```

### Comparing `firebolt_sqlalchemy-0.9.0/LICENSE` & `firebolt_sqlalchemy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-0.9.0/PKG-INFO` & `firebolt_sqlalchemy-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt_sqlalchemy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sqlalchemy adapter for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sqlalchemy
 Download-URL: https://github.com/firebolt-db/firebolt-sqlalchemy/archive/refs/tags/0.0.9.tar.gz
 Author: Firebolt
 Author-email: pypi@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sqlalchemy
```

### Comparing `firebolt_sqlalchemy-0.9.0/README.md` & `firebolt_sqlalchemy-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-0.9.0/setup.cfg` & `firebolt_sqlalchemy-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-0.9.0/src/firebolt_db/firebolt_async_dialect.py` & `firebolt_sqlalchemy-0.9.1/src/firebolt_db/firebolt_async_dialect.py`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-0.9.0/src/firebolt_db/firebolt_dialect.py` & `firebolt_sqlalchemy-0.9.1/src/firebolt_db/firebolt_dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,38 +11,39 @@
 from sqlalchemy.engine import ExecutionContext, default
 from sqlalchemy.engine.url import URL
 from sqlalchemy.sql import compiler, text
 from sqlalchemy.types import (
     ARRAY,
     BIGINT,
     BOOLEAN,
-    CHAR,
     DATE,
     DATETIME,
-    FLOAT,
     INTEGER,
+    NUMERIC,
+    REAL,
+    TEXT,
     TIMESTAMP,
-    VARCHAR,
 )
 
 
 class BYTEA(sqltypes.LargeBinary):
     __visit_name__ = "BYTEA"
 
 
 # Firebolt data types compatibility with sqlalchemy.sql.types
 type_map = {
-    "char": CHAR,
-    "text": VARCHAR,
-    "varchar": VARCHAR,
-    "string": VARCHAR,
-    "float": FLOAT,
-    "double": FLOAT,
-    "double precision": FLOAT,
-    "real": FLOAT,
+    "text": TEXT,
+    "varchar": TEXT,
+    "string": TEXT,
+    "float": REAL,
+    "double": REAL,
+    "double precision": REAL,
+    "numeric": NUMERIC,
+    "decimal": NUMERIC,
+    "real": REAL,
     "boolean": BOOLEAN,
     "int": INTEGER,
     "integer": INTEGER,
     "bigint": BIGINT,
     "long": BIGINT,
     "timestamp": TIMESTAMP,
     "timestamptz": TIMESTAMP,
@@ -72,15 +73,15 @@
     else:
         # Strip complex type info e.g. DECIMAL(8,23) -> DECIMAL
         fb_type = fb_type[: fb_type.find("(")] if "(" in fb_type else fb_type
         result = type_map.get(fb_type, DEFAULT_TYPE)  # type: ignore
     return result
 
 
-DEFAULT_TYPE = VARCHAR
+DEFAULT_TYPE = TEXT
 
 
 class UniversalSet(set):
     def __contains__(self, item: Any) -> bool:
         return True
```

### Comparing `firebolt_sqlalchemy-0.9.0/src/firebolt_sqlalchemy.egg-info/PKG-INFO` & `firebolt_sqlalchemy-0.9.1/src/firebolt_sqlalchemy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt-sqlalchemy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Sqlalchemy adapter for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sqlalchemy
 Download-URL: https://github.com/firebolt-db/firebolt-sqlalchemy/archive/refs/tags/0.0.9.tar.gz
 Author: Firebolt
 Author-email: pypi@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sqlalchemy
```

