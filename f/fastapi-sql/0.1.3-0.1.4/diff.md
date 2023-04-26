# Comparing `tmp/fastapi_sql-0.1.3.tar.gz` & `tmp/fastapi_sql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.1.3.tar", max compression
+gzip compressed data, was "fastapi_sql-0.1.4.tar", max compression
```

## Comparing `fastapi_sql-0.1.3.tar` & `fastapi_sql-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1488 2023-04-26 16:25:20.232468 fastapi_sql-0.1.3/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.3/fastapi_sql/exceptions.py
--rw-r--r--   0        0        0      919 2023-04-26 16:21:35.866852 fastapi_sql-0.1.3/fastapi_sql/migrate.py
--rw-r--r--   0        0        0      537 2023-04-26 16:49:31.615839 fastapi_sql-0.1.3/fastapi_sql/model.py
--rw-r--r--   0        0        0      359 2023-04-26 16:50:07.474069 fastapi_sql-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1533 2023-04-26 16:55:01.586780 fastapi_sql-0.1.4/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.4/fastapi_sql/exceptions.py
+-rw-r--r--   0        0        0      933 2023-04-26 16:52:03.910855 fastapi_sql-0.1.4/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0      537 2023-04-26 16:49:31.615839 fastapi_sql-0.1.4/fastapi_sql/model.py
+-rw-r--r--   0        0        0      359 2023-04-26 16:51:40.067367 fastapi_sql-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.4/PKG-INFO
```

### Comparing `fastapi_sql-0.1.3/fastapi_sql/__init__.py` & `fastapi_sql-0.1.4/fastapi_sql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         self.__sessionmaker__ = async_sessionmaker(
                     bind=self.__engine__, 
                     autoflush=session_options.get('session_autoflush', True),
                     expire_on_commit=session_options.get('expire_on_commit', True)
         )
         self.session = self.__sessionmaker__()
         self.__metadata__ = Model.metadata
-        self.migration = Migration(kwargs.get('migration_options', {}))
+        if kwargs.get('migrate', False):
+            self.migration = Migration(kwargs.get('migration_options', {}))
         
     def create_all(self):
         self.__metadata__.create_all(bind=self.__engine__)
         
     def select(self, cls: type[Model]) -> Select[Any]:
         return select(cls)
```

### Comparing `fastapi_sql-0.1.3/fastapi_sql/migrate.py` & `fastapi_sql-0.1.4/fastapi_sql/migrate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from alembic.config import main
 from typing import Any
 
 class Migration:
     def __init__(self, init_options: 'dict[str,Any]' = {}):
-        argv = ['init']
+        argv = ['init', 'migrations']
         argv.extend(init_options)
         main(argv)
         
     def migrate(self, options: 'dict[str,Any]' = {}):
         argv = ['migrate']
         argv.extend(options)
         main(argv)
```

### Comparing `fastapi_sql-0.1.3/fastapi_sql/model.py` & `fastapi_sql-0.1.4/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.3/PKG-INFO` & `fastapi_sql-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

