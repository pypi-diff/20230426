# Comparing `tmp/databasez-0.2.1.tar.gz` & `tmp/databasez-0.2.2.tar.gz`

## Comparing `databasez-0.2.1.tar` & `databasez-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/__init__.py
--rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/core.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/importer.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/interfaces.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/py.typed
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/testclient.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/__init__.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/aiopg.py
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/asyncmy.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/mssql.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/mysql.py
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/postgres.py
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/common/__init__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/common/records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/compilers/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/compilers/psycopg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/dialects/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.2.1/databasez/backends/dialects/psycopg.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.2.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.2.1/README.md
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 databasez-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 databasez-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/__init__.py
+-rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/core.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/importer.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/interfaces.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/py.typed
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/testclient.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/__init__.py
+-rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/aiopg.py
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/asyncmy.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/mssql.py
+-rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/mysql.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/postgres.py
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/common/__init__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/common/records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/compilers/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/compilers/psycopg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/dialects/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/dialects/psycopg.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.2.2/README.md
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 databasez-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 databasez-0.2.2/PKG-INFO
```

### Comparing `databasez-0.2.1/databasez/core.py` & `databasez-0.2.2/databasez/core.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/databasez/importer.py` & `databasez-0.2.2/databasez/importer.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/databasez/interfaces.py` & `databasez-0.2.2/databasez/interfaces.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/databasez/testclient.py` & `databasez-0.2.2/databasez/testclient.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/databasez/backends/aiopg.py` & `databasez-0.2.2/databasez/backends/aiopg.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,16 @@
         assert self._connection is None, "Connection is already acquired"
         assert self._database._pool is not None, "DatabaseBackend is not running"
         self._connection = await self._database._pool.acquire()
 
     async def release(self) -> None:
         assert self._connection is not None, "Connection is not acquired"
         assert self._database._pool is not None, "DatabaseBackend is not running"
-        await self._database._pool.release(self._connection)
-        self._connection = None
+        connection, self._connection = self._connection, None
+        await self._database._pool.release(connection)
 
     async def fetch_all(self, query: ClauseElement) -> typing.List[RecordInterface]:
         assert self._connection is not None, "Connection is not acquired"
         query_str, args, result_columns, context = self._compile(query)
         column_maps = create_column_maps(result_columns)
         dialect = self._dialect
```

### Comparing `databasez-0.2.1/databasez/backends/asyncmy.py` & `databasez-0.2.2/databasez/backends/asyncmy.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
             autocommit=True,
             **kwargs,
         )
 
     async def disconnect(self) -> None:
         assert self._pool is not None, "DatabaseBackend is not running"
         self._pool.close()
-        await self._pool.wait_closed()
-        self._pool = None
+        pool, self._pool = self._pool, None
+        await pool.wait_closed()
 
     def connection(self) -> "AsyncMyConnection":
         return AsyncMyConnection(self, self._dialect)
 
 
 class CompilationContext:
     def __init__(self, context: ExecutionContext):
```

### Comparing `databasez-0.2.1/databasez/backends/mssql.py` & `databasez-0.2.2/databasez/backends/mssql.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             dsn=dsn,
             **kwargs,
         )
 
     async def disconnect(self) -> None:
         assert self._pool is not None, "DatabaseBackend is not running"
         self._pool.close()
-        await self._pool.wait_closed()
-        self._pool = None
+        pool, self._pool = self._pool, None
+        await pool.wait_closed()
 
     def connection(self) -> "MSSQLConnection":
         return MSSQLConnection(self, self._dialect)
 
 
 class CompilationContext:
     def __init__(self, context: ExecutionContext):
```

### Comparing `databasez-0.2.1/databasez/backends/mysql.py` & `databasez-0.2.2/databasez/backends/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
             autocommit=True,
             **kwargs,
         )
 
     async def disconnect(self) -> None:
         assert self._pool is not None, "DatabaseBackend is not running"
         self._pool.close()
-        await self._pool.wait_closed()
-        self._pool = None
+        pool, self._pool = self._pool, None
+        await pool.wait_closed()
 
     def connection(self) -> "MySQLConnection":
         return MySQLConnection(self, self._dialect)
 
 
 class CompilationContext:
     def __init__(self, context: ExecutionContext):
```

### Comparing `databasez-0.2.1/databasez/backends/postgres.py` & `databasez-0.2.2/databasez/backends/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         assert self._connection is None, "Connection is already acquired"
         assert self._database._pool is not None, "DatabaseBackend is not running"
         self._connection = await self._database._pool.acquire()
 
     async def release(self) -> None:
         assert self._connection is not None, "Connection is not acquired"
         assert self._database._pool is not None, "DatabaseBackend is not running"
-        self._connection = await self._database._pool.release(self._connection)
-        self._connection = None
+        connection, self._connection = self._connection, None
+        self._connection = await self._database._pool.release(connection)
 
     async def fetch_all(self, query: ClauseElement) -> typing.List[RecordInterface]:
         assert self._connection is not None, "Connection is not acquired"
         query_str, args, result_columns = self._compile(query)
         rows = await self._connection.fetch(query_str, *args)
         dialect = self._dialect
         column_maps = create_column_maps(result_columns)
```

### Comparing `databasez-0.2.1/databasez/backends/sqlite.py` & `databasez-0.2.2/databasez/backends/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
     async def acquire(self) -> None:
         assert self._connection is None, "Connection is already acquired"
         self._connection = await self._pool.acquire()
 
     async def release(self) -> None:
         assert self._connection is not None, "Connection is not acquired"
-        await self._pool.release(self._connection)
-        self._connection = None
+        connection, self._connection = self._connection, None
+        await self._pool.release(connection)
 
     async def fetch_all(self, query: ClauseElement) -> typing.List[Record]:
         assert self._connection is not None, "Connection is not acquired"
         query_str, args, result_columns, context = self._compile(query)
         column_maps = create_column_maps(result_columns)
         dialect = self._dialect
```

### Comparing `databasez-0.2.1/databasez/backends/common/records.py` & `databasez-0.2.2/databasez/backends/common/records.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/databasez/backends/dialects/psycopg.py` & `databasez-0.2.2/databasez/backends/dialects/psycopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/LICENSE.md` & `databasez-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/README.md` & `databasez-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/pyproject.toml` & `databasez-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databasez-0.2.1/PKG-INFO` & `databasez-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databasez
-Version: 0.2.1
+Version: 0.2.2
 Summary: Async database support for Python.
 Project-URL: Homepage, https://github.com/dymmond/databasez
 Project-URL: Documentation, https://databasez.dymmond.com/
 Project-URL: Changelog, https://databasez.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/databasez
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
```

