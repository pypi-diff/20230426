# Comparing `tmp/fastapi_sql-0.1.0.tar.gz` & `tmp/fastapi_sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_sql-0.1.1.tar", max compression
```

## Comparing `fastapi_sql-0.1.0.tar` & `fastapi_sql-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1193 2023-04-26 14:38:45.068241 fastapi_sql-0.1.0/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.0/fastapi_sql/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-26 14:38:45.068357 fastapi_sql-0.1.0/fastapi_sql/exeptions.py
--rw-r--r--   0        0        0     2024 2023-04-26 14:38:45.068738 fastapi_sql-0.1.0/fastapi_sql/model.py
--rw-r--r--   0        0        0      339 2023-04-26 15:00:12.814030 fastapi_sql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 fastapi_sql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-04-26 16:25:20.232468 fastapi_sql-0.1.1/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.1/fastapi_sql/exceptions.py
+-rw-r--r--   0        0        0      919 2023-04-26 16:21:35.866852 fastapi_sql-0.1.1/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     2037 2023-04-26 15:59:18.170588 fastapi_sql-0.1.1/fastapi_sql/model.py
+-rw-r--r--   0        0        0      359 2023-04-26 16:01:43.615418 fastapi_sql-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.1/PKG-INFO
```

### Comparing `fastapi_sql-0.1.0/fastapi_sql/__init__.py` & `fastapi_sql-0.1.1/fastapi_sql/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import Any
 
 from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession, async_sessionmaker,
                                     create_async_engine)
-from sqlalchemy import *
+from sqlalchemy import MetaData, Table, Column, Integer, Text, String, DateTime, Date, select
+from sqlalchemy.sql import Select
 from .model import Model
-from .exeptions import *
+from .exceptions import *
+from .migrate import Migration
 
 
 class SQLAlchemy:
     __engine__: AsyncEngine
     session: AsyncSession
     __metadata__: MetaData
+    migration: Migration
     
     Model = Model
     Table = Table
     
     Column = Column
     Integer = Integer
     Text = Text
@@ -29,13 +32,14 @@
         self.__sessionmaker__ = async_sessionmaker(
                     bind=self.__engine__, 
                     autoflush=session_options.get('session_autoflush', True),
                     expire_on_commit=session_options.get('expire_on_commit', True)
         )
         self.session = self.__sessionmaker__()
         self.__metadata__ = Model.metadata
+        self.migration = Migration(kwargs.get('migration_options', {}))
         
     def create_all(self):
         self.__metadata__.create_all(bind=self.__engine__)
         
-        
-        
+    def select(self, cls: type[Model]) -> Select[Any]:
+        return select(cls)
```

### Comparing `fastapi_sql-0.1.0/fastapi_sql/model.py` & `fastapi_sql-0.1.1/fastapi_sql/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from sqlalchemy.orm import DeclarativeBase
 from re import sub
 
+from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta, declared_attr
+
+
 class _Base(DeclarativeBase):
     '''Declarative base'''
 
 class Model(_Base):
     def __init__(cls, name: str, bases: tuple[type, ...], d: dict[str, t.Any], **kwargs: t.Any):
         if should_set_tablename(cls):
             cls.__tablename__ = camel_to_snake_case(cls.__name__)
@@ -26,29 +28,29 @@
     -   If a name is found, it should be used if the class is a mixin, otherwise one
         should be generated.
     -   Abstract models should not have one generated.
     Later, ``__table_cls__`` will determine if the model looks like single or
     joined-table inheritance. If no primary key is found, the name will be unset.
     """
     if cls.__dict__.get("__abstract__", False) or not any(
-        isinstance(b, sa.orm.DeclarativeMeta) for b in cls.__mro__[1:]
+        isinstance(b, DeclarativeMeta) for b in cls.__mro__[1:]
     ):
         return False
 
     for base in cls.__mro__:
         if "__tablename__" not in base.__dict__:
             continue
 
-        if isinstance(base.__dict__["__tablename__"], sa.orm.declared_attr):
+        if isinstance(base.__dict__["__tablename__"], declared_attr):
             return False
 
         return not (
             base is cls
             or base.__dict__.get("__abstract__", False)
-            or not isinstance(base, sa.orm.DeclarativeMeta)
+            or not isinstance(base, DeclarativeMeta)
         )
 
     return True
 
 def camel_to_snake_case(name: str) -> str:
     '''Convert a ``CamelCase`` name to ``snake_case``.'''
     name = sub(r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))", r"_\1", name)
```

### Comparing `fastapi_sql-0.1.0/PKG-INFO` & `fastapi_sql-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.10,<3.0.0)
+Requires-Dist: alembic (>=1.10.4,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
```

