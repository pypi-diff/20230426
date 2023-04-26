# Comparing `tmp/questdb-connect-0.0.14.tar.gz` & `tmp/questdb-connect-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.14.tar", last modified: Tue Apr 25 13:27:32 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.15.tar", last modified: Wed Apr 26 14:18:50 2023, max compression
```

## Comparing `questdb-connect-0.0.14.tar` & `questdb-connect-0.0.15.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 13:27:32.861667 questdb-connect-0.0.14/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.14/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 13:27:32.861514 questdb-connect-0.0.14/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.14/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2372 2023-04-25 13:27:24.000000 questdb-connect-0.0.14/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-25 13:27:32.861703 questdb-connect-0.0.14/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 13:27:32.856912 questdb-connect-0.0.14/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 13:27:32.859420 questdb-connect-0.0.14/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.14/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9980 2023-04-25 13:13:49.000000 questdb-connect-0.0.14/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     8422 2023-04-24 09:39:15.000000 questdb-connect-0.0.14/src/questdb_connect/engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     7509 2023-04-25 13:25:22.000000 questdb-connect-0.0.14/src/questdb_connect/superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     9914 2023-04-25 09:41:56.000000 questdb-connect-0.0.14/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 13:27:32.860764 questdb-connect-0.0.14/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      488 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-25 13:27:32.000000 questdb-connect-0.0.14/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 13:27:32.861200 questdb-connect-0.0.14/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9785 2023-04-25 10:45:04.000000 questdb-connect-0.0.14/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3253 2023-04-25 10:27:32.000000 questdb-connect-0.0.14/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.449398 questdb-connect-0.0.15/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.15/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:18:50.449259 questdb-connect-0.0.15/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.15/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 13:30:53.000000 questdb-connect-0.0.15/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 14:18:50.449435 questdb-connect-0.0.15/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.444857 questdb-connect-0.0.15/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.447276 questdb-connect-0.0.15/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1355 2023-04-26 13:17:59.000000 questdb-connect-0.0.15/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9739 2023-04-26 14:03:15.000000 questdb-connect-0.0.15/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7941 2023-04-26 12:20:15.000000 questdb-connect-0.0.15/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7073 2023-04-26 14:04:36.000000 questdb-connect-0.0.15/src/questdb_connect/types.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5788 2023-04-26 13:30:18.000000 questdb-connect-0.0.15/src/questdb_connect/types_copy.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.448225 questdb-connect-0.0.15/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      522 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.448972 questdb-connect-0.0.15/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.15/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.15/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.15/tests/test_types.py
```

### Comparing `questdb-connect-0.0.14/LICENSE` & `questdb-connect-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.14/PKG-INFO` & `questdb-connect-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.14
+Version: 0.0.15
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.14/README.md` & `questdb-connect-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.14/pyproject.toml` & `questdb-connect-0.0.15/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.14"
+version = "0.0.15"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -35,15 +35,16 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
-    'apache-superset>=2.1.0'
+    'apache-superset>=2.1.0',
+    'sqlparse==0.4.3',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/questdb/questdb-connect/"
 "Bug Tracker" = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
@@ -73,7 +74,8 @@
 
 [tool.ruff.pylint]
 max-branches = 20
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
+"tests/test_superset.py" = ["S101"]
```

### Comparing `questdb-connect-0.0.14/src/questdb_connect/__init__.py` & `questdb-connect-0.0.15/src/questdb_connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import psycopg2
 
 # ===== DBAPI =====
+# https://peps.python.org/pep-0249/
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
 
 
 class Error(Exception):
```

### Comparing `questdb-connect-0.0.14/src/questdb_connect/dialect.py` & `questdb-connect-0.0.15/src/questdb_connect/dialect.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 #  limitations under the License.
 #
 import abc
 
 import sqlalchemy as sqla
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
+from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
-from questdb_connect import types
+from questdb_connect.types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
-
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
 
 def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
@@ -48,90 +48,75 @@
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
             table_name: str,
             ts_col_name: str = None,
-            partition_by: types.PartitionBy = types.PartitionBy.DAY,
+            partition_by: PartitionBy = PartitionBy.DAY,
             is_wal: bool = True
     ):
         Traversible.__init__(self)
         self.name = table_name
         self.ts_col_name = ts_col_name
         self.partition_by = partition_by
         self.is_wal = is_wal
         self.compiled = None
 
     def get_table_suffix(self):
         if self.compiled is None:
             self.compiled = ''
             has_ts = self.ts_col_name is not None
-            is_partitioned = self.partition_by and self.partition_by != types.PartitionBy.NONE
+            is_partitioned = self.partition_by and self.partition_by != PartitionBy.NONE
             if has_ts:
                 self.compiled += f'TIMESTAMP({self.ts_col_name})'
             if is_partitioned:
                 if not has_ts:
-                    raise types.ArgumentError(None, 'Designated timestamp must be specified for partitioned table')
+                    raise ArgumentError(None, 'Designated timestamp must be specified for partitioned table')
                 self.compiled += f' PARTITION BY {self.partition_by.name}'
             if self.is_wal:
                 if not is_partitioned:
-                    raise types.ArgumentError(None, 'WAL table requires designated timestamp and partition by')
+                    raise ArgumentError(None, 'WAL table requires designated timestamp and partition by')
                 if self.is_wal:
                     self.compiled += ' WAL'
                 else:
                     self.compiled += ' BYPASS WAL'
         return self.compiled
 
     def _set_parent(self, parent, **_kwargs):
         parent.engine = self
 
 
 # ===== QUESTDB DIALECT TYPES =====
 
 
-_QUOTES = ("'", '"')
-
-
-def _quote_identifier(identifier: str):
-    if not identifier:
-        return None
-    first = 0
-    last = len(identifier)
-    if identifier[first] in _QUOTES:
-        first += 1
-    if identifier[last - 1] in _QUOTES:
-        last -= 1
-    return f"'{identifier[first:last]}'"
-
-
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
     """QuestDB's identifiers are better off with quotes"""
-    quote_identifier = staticmethod(_quote_identifier)
+    quote_identifier = staticmethod(quote_identifier)
 
     def _requires_quotes(self, _value):
         return True
 
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
     def visit_create_schema(self, create, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
 
     def visit_drop_schema(self, drop, **kw):
         raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
 
     def visit_create_table(self, create, **kw):
         table = create.element
-        create_table = f"CREATE TABLE '{table.fullname}' ("
+        create_table = f"CREATE TABLE {quote_identifier(table.fullname)} ("
         create_table += ', '.join([self.get_column_specification(c.element) for c in create.columns])
         return create_table + ') ' + table.engine.get_table_suffix()
 
     def get_column_specification(self, column: sqla.Column, **_):
-        if not isinstance(column.type, types.QDBTypeMixin):
-            raise types.ArgumentError('Column type is not a valid QuestDB type')
+        if not isinstance(column.type, QDBTypeMixin):
+            raise ArgumentError('Column type is not a valid QuestDB type')
         return column.type.column_spec(column.name)
 
 
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
@@ -158,37 +143,37 @@
     ):
         table_name = table.name
         result_set = self.bind.execute(f"tables() WHERE name = '{table_name}'")
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         table_attrs = result_set.first()
         col_ts_name = table_attrs['designatedTimestamp']
-        partition_by = types.PartitionBy[table_attrs['partitionBy']]
+        partition_by = PartitionBy[table_attrs['partitionBy']]
         is_wal = True if table_attrs['walEnabled'] else False
         for row in self.bind.execute(f"table_columns('{table_name}')"):
             col_name = row[0]
             if include_columns and col_name not in include_columns:
                 continue
             if exclude_columns and col_name in exclude_columns:
                 continue
-            col_type = types.resolve_type_from_name(row[1])
+            col_type = resolve_type_from_name(row[1])
             if col_ts_name and col_ts_name.upper() == col_name.upper():
                 table.append_column(sqla.Column(col_name, col_type, primary_key=True))
             else:
                 table.append_column(sqla.Column(col_name, col_type))
         table.engine = QDBTableEngine(table_name, col_ts_name, partition_by, is_wal)
         table.metadata = sqla.MetaData()
 
     def get_columns(self, table_name, schema=None, **kw):
         result_set = self.bind.execute(f"table_columns('{table_name}')")
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         return [{
             'name': row[0],
-            'type': types.resolve_type_from_name(row[1]),
+            'type': resolve_type_from_name(row[1]),
             'nullable': True,
             'autoincrement': False,
             'persisted': True
         } for row in result_set]
 
 
 # class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
```

### Comparing `questdb-connect-0.0.14/src/questdb_connect/engine.py` & `questdb-connect-0.0.15/src/questdb_connect/superset_engine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,178 @@
+#
+#     ___                  _   ____  ____
+#    / _ \ _   _  ___  ___| |_|  _ \| __ )
+#   | | | | | | |/ _ \/ __| __| | | |  _ \
+#   | |_| | |_| |  __/\__ \ |_| |_| | |_) |
+#    \__\_\\__,_|\___||___/\__|____/|____/
+#
+#  Copyright (c) 2014-2019 Appsicle
+#  Copyright (c) 2019-2023 QuestDB
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#  http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+#
 import logging
-
+import re
 from datetime import datetime
-from typing import Dict, List, Optional, Type
-
-from flask import current_app
-from flask_babel import gettext as __
-from marshmallow import Schema, fields
-from marshmallow.validate import Range
-from sqlalchemy.engine.url import URL, make_url
-from sqlalchemy.sql.type_api import TypeEngine
-from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersType, BasicParametersMixin
-from superset.db_engine_specs.exceptions import SupersetDBAPIDatabaseError
-from superset.errors import SupersetError, SupersetErrorType, ErrorLevel
-from superset.utils.core import ColumnSpec, GenericDataType
-from superset.utils.network import is_hostname_valid, is_port_open
-from superset.models.core import Database
-
-from clickhouse_connect import driver_name
-from clickhouse_connect.common import set_setting
-from clickhouse_connect.driver import default_port
-from clickhouse_connect.cc_sqlalchemy.datatypes.base import sqla_type_from_name
-from clickhouse_connect.cc_superset.datatypes import configure_types
-from clickhouse_connect.driver.exceptions import ClickHouseError
+from typing import Any, Dict, Optional, Tuple
 
-logger = logging.getLogger(__name__)
+from sqlalchemy.types import TypeEngine
+from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
+from superset.utils import core as utils
+from superset.utils.core import GenericDataType
 
-configure_types()
-set_setting('product_name', f"superset/{current_app.config.get('VERSION_STRING', 'dev')}")
+import questdb_connect.dialect as qdbcd
+from questdb_connect import types
 
-
-class ClickHouseParametersSchema(Schema):
-    username = fields.String(allow_none=True, description=__('Username'))
-    password = fields.String(allow_none=True, description=__('Password'))
-    host = fields.String(required=True, description=__('Hostname or IP address'))
-    port = fields.Integer(allow_none=True, description=__('Database port'), validate=Range(min=0, max=65535), )
-    database = fields.String(allow_none=True, description=__('Database name'))
-    encryption = fields.Boolean(default=True, description=__('Use an encrypted connection to the database'))
-    query = fields.Dict(keys=fields.Str(), values=fields.Raw(), description=__('Additional parameters'))
+logger = logging.getLogger(__name__)
 
 
-class ClickHouseEngineSpec(BaseEngineSpec, BasicParametersMixin):
-    """
-    See :py:class:`superset.db_engine_specs.base.BaseEngineSpec`
-    """
+# https://superset.apache.org/docs/databases/installing-database-drivers
+# Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
+# https://preset.io/blog/building-database-connector/
 
-    engine = driver_name
-    engine_name = 'ClickHouse Connect'
 
-    default_driver = 'connect'
-    time_secondary_columns = True
+class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
+    engine = 'questdb'
+    engine_name = 'QuestDB Connect'
+    default_driver = "psycopg2"
+    encryption_parameters = {"sslmode": "prefer"}
+    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
-    _function_names = []
-
+    time_secondary_columns = True
+    max_column_name_length = 120
     _time_grain_expressions = {
         None: '{col}',
-        'PT1M': 'toStartOfMinute(toDateTime({col}))',
-        'PT5M': 'toStartOfFiveMinutes(toDateTime({col}))',
-        'PT10M': 'toStartOfTenMinutes(toDateTime({col}))',
-        'PT15M': 'toStartOfFifteenMinutes(toDateTime({col}))',
-        'PT30M': 'toDateTime(intDiv(toUInt32(toDateTime({col})), 1800)*1800)',
-        'PT1H': 'toStartOfHour(toDateTime({col}))',
-        'P1D': 'toStartOfDay(toDateTime({col}))',
-        'P1W': 'toMonday(toDateTime({col}))',
-        'P1M': 'toStartOfMonth(toDateTime({col}))',
-        'P3M': 'toStartOfQuarter(toDateTime({col}))',
-        'P1Y': 'toStartOfYear(toDateTime({col}))',
+        'PT1S': "date_trunc('second', {col})",
+        'PT5S': "date_trunc('second', {col}) + 5000000",
+        'PT30S': "date_trunc('second', {col}) + 30000000",
+        'PT1M': "date_trunc('minute', {col})",
+        'PT5M': "date_trunc('minute', {col}) + 300000000",
+        'PT10M': "date_trunc('minute', {col}) + 600000000",
+        'PT15M': "date_trunc('minute', {col}) + 900000000",
+        'PT30M': "date_trunc('minute', {col}) + 1800000000",
+        'PT1H': "date_trunc('hour', {col})",
+        'PT6H': "date_trunc('hour', {col})",
+        'PT1D': "date_trunc('day', {col})",
+        'P1W': "date_trunc('week', {col})",
+        'P1M': "date_trunc('month', {col})",
+        'P1Y': "date_trunc('year', {col})",
+        'P3M': "date_trunc('quarter', {col})",
     }
-
-    sqlalchemy_uri_placeholder = 'clickhousedb://user:password@host[:port][/dbname][?secure=value&=value...]'
-    parameters_schema = ClickHouseParametersSchema()
-    encryption_parameters = {'secure': 'true'}
+    _default_column_type_mappings = (
+        (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
+        (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
+        (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
+        (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
+        (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
+        (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
+        (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
+        (re.compile("^DOUBLE'", re.IGNORECASE), types.Double, GenericDataType.NUMERIC),
+        (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol, GenericDataType.STRING),
+        (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
+        (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
+        (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
+        (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
+        (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
+        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING),
+    )
+
+    @classmethod
+    def build_sqlalchemy_uri(
+            cls,
+            parameters: BasicParametersType,
+            encrypted_extra: Optional[Dict[str, str]] = None
+    ) -> str:
+        return qdbcd.connection_uri(
+            parameters.get("host"),
+            int(parameters.get("port")),
+            parameters.get("username"),
+            parameters.get("password"),
+            parameters.get("database"))
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
-        return '{col}'
-
-    @classmethod
-    def get_dbapi_exception_mapping(cls) -> Dict[Type[Exception], Type[Exception]]:
-        return {}
-
-    @classmethod
-    def get_dbapi_mapped_exception(cls, exception: Exception) -> Exception:
-        new_exception = cls.get_dbapi_exception_mapping().get(type(exception))
-        if new_exception == SupersetDBAPIDatabaseError:
-            return SupersetDBAPIDatabaseError('Connection failed')
-        if not new_exception:
-            return exception
-        return new_exception(str(exception))
+        """SQL expression that converts epoch (seconds) to datetime that can be used in a
+        query. The reference column should be denoted as `{col}` in the return
+        expression, e.g. "FROM_UNIXTIME({col})"
+        :return: SQL Expression
+        """
+        return '{col} * 1000000'
 
     @classmethod
     def convert_dttm(cls, target_type: str, dttm: datetime, *_args, **_kwargs) -> Optional[str]:
-        if target_type.upper() == 'DATE':
-            return f"'{dttm.date().isoformat()}'"
-        if target_type.upper() == 'DATETIME':
-            return f"""'{dttm.isoformat(sep=" ", timespec="seconds")}'"""
+        """Convert a Python `datetime` object to a SQL expression.
+        :param target_type: The target type of expression
+        :param dttm: The datetime object
+        :param db_extra: The database extra object
+        :return: The SQL expression
+        """
+        type_u = target_type.upper()
+        if type_u == 'DATE':
+            return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
+        if type_u in ('DATETIME', 'TIMESTAMP'):
+            dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
+            return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
-    def get_function_names(cls, database: Database) -> List[str]:
-        if cls._function_names:
-            return cls._function_names
-        try:
-            names = database.get_df(
-                'SELECT name FROM system.functions UNION ALL ' +
-                'SELECT name FROM system.table_functions LIMIT 10000')['name'].tolist()
-            cls._function_names = names
-            return names
-        except ClickHouseError:
-            logger.exception('Error retrieving system.functions')
-            return []
-
-    @classmethod
-    def get_datatype(cls, type_code: str) -> str:
+    def get_datatype(cls, type_code: Any) -> Optional[str]:
+        """Change column type code from cursor description to string representation.
+        :param type_code: Type code from cursor description
+        :return: String representation of type code
+        """
+        logger.info('QUEST get_datatype(type_code: %s)', type_code)
         return type_code
 
     @classmethod
-    def get_column_spec(cls, native_type: Optional[str], *_args, **_kwargs) -> Optional[ColumnSpec]:
-        if not native_type:
+    def get_column_types(
+            cls,
+            column_type: Optional[str],
+    ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
+        if not column_type:
             return None
-        sqla_type = sqla_type_from_name(native_type)
-        generic_type = sqla_type.generic_type
-        return ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
+        logger.info('QUEST get_column_types(column_type: %s)', column_type)
+        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
+            matching_name = regex.match(column_type)
+            if matching_name:
+                return types.resolve_type_from_name(sqla_type.__visit_name__), generic_type
+        return None
 
     @classmethod
-    def get_sqla_column_type(cls, column_type: Optional[str], *_args, **_kwargs):
-        if column_type is None:
+    def get_column_spec(
+            cls,
+            native_type: Optional[str],
+            db_extra: Optional[Dict[str, Any]] = None,
+            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+    ) -> Optional[utils.ColumnSpec]:
+        if not native_type:
             return None
-        sqla_type = sqla_type_from_name(column_type)
-        return sqla_type, sqla_type.generic_type
+        logger.info('QUEST get_column_spec(native_type: %s)', native_type)
+        sqla_type = types.resolve_type_from_name(native_type)
+        name_u = sqla_type.__visit_name__
+        generic_type = None
+        if name_u == 'BOOLEAN':
+            generic_type = GenericDataType.BOOLEAN
+        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
+            generic_type = GenericDataType.NUMERIC
+        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
+            generic_type = GenericDataType.STRING
+        elif name_u in ('DATE', 'TIMESTAMP'):
+            generic_type = GenericDataType.TEMPORAL
+        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+            generic_type = GenericDataType.STRING
+        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
 
     @classmethod
     def column_datatype_to_string(cls, sqla_column_type: TypeEngine, *_args):
+        logger.info('QUEST column_datatype_to_string(sqla_column_type: %s)', sqla_column_type)
         return sqla_column_type.compile()
-
-    @classmethod
-    def build_sqlalchemy_uri(cls, parameters: BasicParametersType, *_args):
-        url_params = parameters.copy()
-        if url_params.get('encryption'):
-            query = parameters.get('query', {}).copy()
-            query.update(cls.encryption_parameters)
-            url_params['query'] = query
-        if not url_params.get('database'):
-            url_params['database'] = '__default__'
-        url_params.pop('encryption', None)
-        return str(URL(f'{cls.engine}+{cls.default_driver}', **url_params))
-
-    @classmethod
-    def get_parameters_from_uri(cls, uri: str, *_args, **_kwargs) -> BasicParametersType:
-        url = make_url(uri)
-        query = url.query
-        if 'secure' in query:
-            encryption = url.query.get('secure') == 'true'
-            query.pop('secure')
-        else:
-            encryption = False
-        return BasicParametersType(
-            username=url.username,
-            password=url.password,
-            host=url.host,
-            port=url.port,
-            database=None if url.database == '__default__' else url.database,
-            query=dict(query),
-            encryption=encryption)
-
-    @classmethod
-    # pylint: disable=arguments-renamed
-    def validate_parameters(cls, properties) -> List[SupersetError]:
-        # The newest versions of superset send a "properties" object with a parameters key, instead of just
-        # the parameters, so we hack to be compatible
-        parameters = properties.get('parameters', properties)
-        host = parameters.get('host', None)
-        if not host:
-            return [SupersetError(
-                'Hostname is required',
-                SupersetErrorType.CONNECTION_MISSING_PARAMETERS_ERROR,
-                ErrorLevel.WARNING,
-                {'missing': ['host']},
-            )]
-        if not is_hostname_valid(host):
-            return [SupersetError(
-                "The hostname provided can't be resolved.",
-                SupersetErrorType.CONNECTION_INVALID_HOSTNAME_ERROR,
-                ErrorLevel.ERROR,
-                {'invalid': ['host']},
-            )]
-        port = parameters.get('port')
-        if port is None:
-            port = default_port('http', parameters.get('encryption', False))
-        try:
-            port = int(port)
-        except (ValueError, TypeError):
-            port = -1
-        if port <= 0 or port >= 65535:
-            return [SupersetError(
-                'Port must be a valid integer between 0 and 65535 (inclusive).',
-                SupersetErrorType.CONNECTION_INVALID_PORT_ERROR,
-                ErrorLevel.ERROR,
-                {'invalid': ['port']})]
-        if not is_port_open(host, port):
-            return [SupersetError(
-                'The port is closed.',
-                SupersetErrorType.CONNECTION_PORT_CLOSED_ERROR,
-                ErrorLevel.ERROR,
-                {'invalid': ['port']})]
-        return []
```

### Comparing `questdb-connect-0.0.14/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.15/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.14
+Version: 0.0.15
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.14/tests/test_dialect.py` & `questdb-connect-0.0.15/tests/test_dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     with test_engine.connect() as conn:
         assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME)
         assert not test_engine.dialect.has_table(conn, 'scorchio')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
         expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                     "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                     "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                     "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                     "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                    "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                     "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
         stmt1 = sqla.insert(test_model).values(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=13,
             col_long=14,
@@ -122,35 +122,35 @@
         ('col_double', types.Double(), False),
         ('col_symbol', types.Symbol(), False),
         ('col_string', types.String(), False),
         ('col_char', types.Char(), False),
         ('col_uuid', types.UUID(), False),
         ('col_date', types.Date(), False),
         ('col_ts', types.Timestamp(), True),
-        ('col_geohash', types.geohash_type(40)(), False),
+        ('col_geohash', types.GeohashInt(), False),
         ('col_long256', types.Long256(), False)
     ])
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
     expected = ("(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     try:
         for idx in range(num_rows):
             session.add(test_model(
                 col_boolean=True,
                 col_byte=8,
                 col_short=12,
@@ -178,23 +178,23 @@
 def test_bulk_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
     expected = ("(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 1, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                 "(True, 8, 12, 2, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
-                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
+                "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                 "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')")
     models = [
         test_model(
             col_boolean=True,
             col_byte=8,
             col_short=12,
             col_int=idx,
```

### Comparing `questdb-connect-0.0.14/tests/test_types.py` & `questdb-connect-0.0.15/tests/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 #
 import re
 
 from questdb_connect import types
 
 
 def test_resolve_type_from_name():
-    for type_class in types.basic_type_classes:
+    for type_class in types.QUESTDB_TYPES:
         resolved_class = types.resolve_type_from_name(type_class.__visit_name__)
         assert type_class.__visit_name__ == resolved_class.__visit_name__
         assert isinstance(type_class(), resolved_class)
         assert isinstance(resolved_class(), type_class)
 
     for n in range(1, 61):
         g_name = types.geohash_type_name(n)
         g_class = types.resolve_type_from_name(g_name)
-        assert isinstance(g_class(), types.geohash_type(n))
+        assert isinstance(g_class(), types.geohash_class(n))
 
 
 def test_superset_default_mappings():
     default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte),
@@ -51,23 +51,23 @@
         (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol),
         (re.compile("^STRING", re.IGNORECASE), types.String),
         (re.compile("^UUID", re.IGNORECASE), types.UUID),
         (re.compile("^CHAR", re.IGNORECASE), types.Char),
         (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp),
         (re.compile("^DATE", re.IGNORECASE), types.Date)
     )
-    for type_class in types.basic_type_classes:
+    for type_class in types.QUESTDB_TYPES:
         for pattern, _expected_type in default_column_type_mappings:
             matching_name = pattern.match(type_class.__visit_name__)
             if matching_name:
                 resolved_class = types.resolve_type_from_name(matching_name.group(0))
                 assert type_class.__visit_name__ == resolved_class.__visit_name__
                 assert isinstance(type_class(), resolved_class)
                 assert isinstance(resolved_class(), type_class)
                 break
     geohash_pattern = re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE)
     for n in range(1, 61):
         g_name = types.geohash_type_name(n)
         matching_name = geohash_pattern.match(g_name).group(0)
         assert matching_name == g_name
         g_class = types.resolve_type_from_name(g_name)
-        assert isinstance(g_class(), types.geohash_type(n))
+        assert isinstance(g_class(), types.geohash_class(n))
```

