# Comparing `tmp/buenavista-0.2.0.tar.gz` & `tmp/buenavista-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buenavista-0.2.0.tar", last modified: Mon Apr  3 15:35:36 2023, max compression
+gzip compressed data, was "buenavista-0.2.1.tar", last modified: Tue Apr 25 23:03:11 2023, max compression
```

## Comparing `buenavista-0.2.0.tar` & `buenavista-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.920048 buenavista-0.2.0/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.2.0/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-03 15:35:36.919888 buenavista-0.2.0/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1566 2023-03-03 20:38:14.000000 buenavista-0.2.0/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.916564 buenavista-0.2.0/buenavista/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.2.0/buenavista/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.917680 buenavista-0.2.0/buenavista/backends/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.2.0/buenavista/backends/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     7044 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/backends/duckdb.py
--rw-r--r--   0 jwills     (501) staff       (20)     3384 2023-03-10 16:36:56.000000 buenavista-0.2.0/buenavista/backends/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     2486 2023-03-10 16:36:56.000000 buenavista-0.2.0/buenavista/bv_dialects.py
--rw-r--r--   0 jwills     (501) staff       (20)     3090 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/core.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.918654 buenavista-0.2.0/buenavista/examples/
--rw-r--r--   0 jwills     (501) staff       (20)     3540 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/examples/duckdb_http.py
--rw-r--r--   0 jwills     (501) staff       (20)     1218 2023-03-10 16:36:56.000000 buenavista-0.2.0/buenavista/examples/duckdb_postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.2.0/buenavista/examples/postgres_proxy.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.919455 buenavista-0.2.0/buenavista/http/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.2.0/buenavista/http/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/http/context.py
--rw-r--r--   0 jwills     (501) staff       (20)     4298 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/http/main.py
--rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.2.0/buenavista/http/schemas.py
--rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.2.0/buenavista/http/type_mapping.py
--rw-r--r--   0 jwills     (501) staff       (20)    18814 2023-03-25 04:03:13.000000 buenavista-0.2.0/buenavista/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-03 05:42:19.000000 buenavista-0.2.0/buenavista/rewrite.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-03 15:35:36.917230 buenavista-0.2.0/buenavista.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-03 15:35:36.000000 buenavista-0.2.0/buenavista.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      652 2023-04-03 15:35:36.000000 buenavista-0.2.0/buenavista.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-03 15:35:36.000000 buenavista-0.2.0/buenavista.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       83 2023-04-03 15:35:36.000000 buenavista-0.2.0/buenavista.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       11 2023-04-03 15:35:36.000000 buenavista-0.2.0/buenavista.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-03 15:35:36.920088 buenavista-0.2.0/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-03-09 18:25:32.000000 buenavista-0.2.0/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.916820 buenavista-0.2.1/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.2.1/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-25 23:03:11.916703 buenavista-0.2.1/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1566 2023-03-03 20:38:14.000000 buenavista-0.2.1/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.913102 buenavista-0.2.1/buenavista/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.2.1/buenavista/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.914506 buenavista-0.2.1/buenavista/backends/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.2.1/buenavista/backends/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7478 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/backends/duckdb.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3384 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/backends/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2486 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/bv_dialects.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3148 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/core.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.915330 buenavista-0.2.1/buenavista/examples/
+-rw-r--r--   0 jwills     (501) staff       (20)     3540 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/examples/duckdb_http.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1218 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/examples/duckdb_postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/examples/postgres_proxy.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.916458 buenavista-0.2.1/buenavista/http/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.2.1/buenavista/http/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/http/context.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4298 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/http/main.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.2.1/buenavista/http/schemas.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.2.1/buenavista/http/type_mapping.py
+-rw-r--r--   0 jwills     (501) staff       (20)    19000 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-25 17:26:47.000000 buenavista-0.2.1/buenavista/rewrite.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.914140 buenavista-0.2.1/buenavista.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      652 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       83 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       11 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-25 23:03:11.916856 buenavista-0.2.1/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-04-25 23:01:34.000000 buenavista-0.2.1/setup.py
```

### Comparing `buenavista-0.2.0/LICENSE` & `buenavista-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/PKG-INFO` & `buenavista-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.0
+Version: 0.2.1
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
```

### Comparing `buenavista-0.2.0/README.md` & `buenavista-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/backends/duckdb.py` & `buenavista-0.2.1/buenavista/backends/duckdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import logging
-import os
 import re
 from typing import Dict, Iterator, List, Optional, Tuple
 
-import duckdb
 import pyarrow as pa
+import sqlglot
 
 from buenavista.core import BVType, Connection, QueryResult, Session
 
 
 logger = logging.getLogger(__name__)
 
 
 def to_bvtype(t: pa.DataType) -> BVType:
-    if pa.types.is_boolean(t):
-        return BVType.BOOL
-    elif pa.types.is_int64(t):
+    if pa.types.is_int64(t):
         return BVType.BIGINT
     elif pa.types.is_integer(t):
         return BVType.INTEGER
     elif pa.types.is_string(t):
         return BVType.TEXT
     elif pa.types.is_date(t):
         return BVType.DATE
@@ -29,19 +26,30 @@
         return BVType.TIMESTAMP
     elif pa.types.is_floating(t):
         return BVType.FLOAT
     elif pa.types.is_decimal(t):
         return BVType.DECIMAL
     elif pa.types.is_binary(t):
         return BVType.BYTES
+    elif pa.types.is_boolean(t):
+        return BVType.BOOL
     elif pa.types.is_interval(t):
         return BVType.INTERVAL
-    elif pa.types.is_list(t) or pa.types.is_struct(t) or pa.types.is_map(t):
+    elif pa.types.is_list(t):
+        field_type = t.field(0).type
+        if pa.types.is_integer(field_type):
+            return BVType.INTEGERARRAY
+        elif pa.types.is_string(field_type):
+            return BVType.STRINGARRAY
+        else:
+            # TODO: detailed nested types
+            return BVType.ARRAY
+    elif pa.types.is_struct(t) or pa.types.is_map(t):
         # TODO: support detailed nested types
-        return BVType.TEXT
+        return BVType.JSON
     else:
         return BVType.UNKNOWN
 
 
 class RecordBatchIterator(Iterator[List[Optional[str]]]):
     def __init__(self, rbr: pa.RecordBatchReader):
         self.rbr = rbr
@@ -173,15 +181,21 @@
         return sql
 
     def in_transaction(self) -> bool:
         return self.in_txn
 
     def execute_sql(self, sql: str, params=None) -> QueryResult:
         status = ""
-        lsql = sql.lower()
+        try:
+            lsql = sqlglot.parse_one(sql).sql(comments=False)
+        except:
+            # TODO: log this
+            lsql = sql
+
+        lsql = lsql.lower()
         if self.in_txn:
             if "commit" in lsql:
                 self.in_txn = False
                 status = "COMMIT"
             elif "rollback" in lsql:
                 self.in_txn = False
                 status = "ROLLBACK"
```

### Comparing `buenavista-0.2.0/buenavista/backends/postgres.py` & `buenavista-0.2.1/buenavista/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/bv_dialects.py` & `buenavista-0.2.1/buenavista/bv_dialects.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/core.py` & `buenavista-0.2.1/buenavista/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     INTERVAL = 7
     JSON = 8
     DECIMAL = 9
     TEXT = 10
     TIME = 11
     TIMESTAMP = 12
     UNKNOWN = 13
+    ARRAY = 14
+    INTEGERARRAY = 15
+    STRINGARRAY = 16
 
 
 class QueryResult:
     """The BV representation of a result of a query."""
 
     def has_results(self) -> bool:
         raise NotImplementedError
```

### Comparing `buenavista-0.2.0/buenavista/examples/duckdb_http.py` & `buenavista-0.2.1/buenavista/examples/duckdb_http.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/examples/duckdb_postgres.py` & `buenavista-0.2.1/buenavista/examples/duckdb_postgres.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/http/context.py` & `buenavista-0.2.1/buenavista/http/context.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/http/main.py` & `buenavista-0.2.1/buenavista/http/main.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/http/schemas.py` & `buenavista-0.2.1/buenavista/http/schemas.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/http/type_mapping.py` & `buenavista-0.2.1/buenavista/http/type_mapping.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista/postgres.py` & `buenavista-0.2.1/buenavista/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import io
 import json
 import logging
 import os
 import random
-import re
 import socketserver
 import struct
 from typing import Dict, List, Optional
 
 from .core import BVType, Connection, Extension, Session, QueryResult
 from .rewrite import Rewriter
 
@@ -57,26 +56,29 @@
     SYNC = b"S"
     TERMINATE = b"X"
 
 
 PG_UNKNOWN = (705, str)
 BVTYPE_TO_PGTYPE = {
     BVType.NULL: (-1, lambda v: None),
+    BVType.ARRAY: (2277, lambda v: "{" + ",".join(v) + "}"),
     BVType.BIGINT: (20, str),
     BVType.BOOL: (16, lambda v: "true" if v else "false"),
     BVType.BYTES: (17, lambda v: "\\x" + v.hex()),
     BVType.DATE: (1082, lambda v: v.isoformat()),
+    BVType.DECIMAL: (1700, str),
     BVType.FLOAT: (701, str),
     BVType.INTEGER: (23, str),
+    BVType.INTEGERARRAY: (1007, lambda v: "{" + ",".join(v) + "}"),
     BVType.INTERVAL: (
         1186,
         lambda v: f"{v.days} days {v.seconds} seconds {v.microseconds} microseconds",
     ),
     BVType.JSON: (114, lambda v: json.dumps(v)),
-    BVType.DECIMAL: (1700, str),
+    BVType.STRINGARRAY: (1009, lambda v: "{" + ",".join(v) + "}"),
     BVType.TEXT: (25, str),
     BVType.TIME: (1083, lambda v: v.isoformat()),
     BVType.TIMESTAMP: (1114, lambda v: v.isoformat().replace("T", " ")),
 }
 
 
 class BVBuffer(object):
```

### Comparing `buenavista-0.2.0/buenavista/rewrite.py` & `buenavista-0.2.1/buenavista/rewrite.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/buenavista.egg-info/PKG-INFO` & `buenavista-0.2.1/buenavista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.0
+Version: 0.2.1
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
```

### Comparing `buenavista-0.2.0/buenavista.egg-info/SOURCES.txt` & `buenavista-0.2.1/buenavista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.0/setup.py` & `buenavista-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "buenavista"
-package_version = "0.2.0"
+package_version = "0.2.1"
 
 description = """Programmable Presto and Postgres Proxies"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

