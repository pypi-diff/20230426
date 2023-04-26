# Comparing `tmp/codercore-1.9.0.tar.gz` & `tmp/codercore-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codercore-1.9.0.tar", last modified: Thu Mar 16 16:04:26 2023, max compression
+gzip compressed data, was "codercore-2.0.0.tar", last modified: Tue Apr 25 14:40:24 2023, max compression
```

## Comparing `codercore-1.9.0.tar` & `codercore-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.577226 codercore-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 16:04:26.577226 codercore-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-16 16:03:59.000000 codercore-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/schemas/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.577226 codercore-1.9.0/codercore/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-16 16:03:59.000000 codercore-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:04:26.577226 codercore-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.387995 codercore-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 14:40:24.387995 codercore-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 14:39:52.000000 codercore-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.383995 codercore-2.0.0/codercore/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.383995 codercore-2.0.0/codercore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.387995 codercore-2.0.0/codercore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.387995 codercore-2.0.0/codercore/lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/schemas/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.387995 codercore-2.0.0/codercore/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/test/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 14:39:52.000000 codercore-2.0.0/codercore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.383995 codercore-2.0.0/codercore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 14:40:24.000000 codercore-2.0.0/codercore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 14:40:24.000000 codercore-2.0.0/codercore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:40:24.000000 codercore-2.0.0/codercore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-25 14:40:24.000000 codercore-2.0.0/codercore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 14:40:24.000000 codercore-2.0.0/codercore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-25 14:39:52.000000 codercore-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:40:24.387995 codercore-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:40:24.387995 codercore-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 14:39:52.000000 codercore-2.0.0/tests/test_types.py
```

### Comparing `codercore-1.9.0/codercore/db/__init__.py` & `codercore-2.0.0/codercore/db/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import cache
 from typing import Callable, Optional, Type
 
 from asyncpg.connection import Connection
+from asyncstdlib.functools import cache as async_cache
 from google.cloud.sql.connector import IPTypes, create_async_connector
 from sqlalchemy.dialects.postgresql.asyncpg import (
     AsyncAdapt_asyncpg_connection,
     AsyncAdapt_asyncpg_dbapi,
 )
 from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 from sqlalchemy.orm import Session as Session_, sessionmaker as sessionmaker_
@@ -38,14 +39,15 @@
 
 def get_connection_url(
     driver: str, user: str, password: str, host: str, database: str
 ) -> str:
     return f"{driver}://{user}:{password}@{host}/{database}"
 
 
+@async_cache
 async def get_connection_with_auto_iam_creator(
     instance_connection_name: str,
     user: str,
     database: str,
 ) -> Callable[[], Connection]:
     connector = await create_async_connector()
```

### Comparing `codercore-1.9.0/codercore/lib/hash.py` & `codercore-2.0.0/codercore/lib/hash.py`

 * *Files identical despite different names*

### Comparing `codercore-1.9.0/codercore/lib/redis.py` & `codercore-2.0.0/codercore/lib/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,12 +79,12 @@
             formatted_key = key if isinstance(key, str) else key(*args, **kwargs)
             if (result := await connection.get(formatted_key)) is not None:
                 return deserialize(result)
             result = func(*args, **kwargs)
             if inspect.iscoroutine(result):
                 result = await result
             await connection.set(formatted_key, result, ex=ex)
-            return result
+            return deserialize(result)
 
         return wrapper
 
     return decorate
```

### Comparing `codercore-1.9.0/codercore/lib/settings.py` & `codercore-2.0.0/codercore/lib/settings.py`

 * *Files identical despite different names*

### Comparing `codercore-1.9.0/codercore/test/fixtures.py` & `codercore-2.0.0/codercore/test/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from collections.abc import AsyncIterator
+from typing import Awaitable, Callable
 
 from pytest import FixtureRequest
 from sqlalchemy import MetaData
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import sessionmaker as sessionmaker_
 from sqlalchemy.pool import NullPool
-from sqlalchemy_utils import database_exists, create_database, drop_database
+from sqlalchemy_utils import create_database, database_exists, drop_database
 
 from codercore.db import get_connection_url, sessionmaker
 from codercore.db.models import Base
-from codercore.lib.redis import connection, Redis
+from codercore.lib.redis import Redis, connection
 from codercore.lib.settings import EnvSettings
 
 
 def connection_settings(
     user: str,
     password: str,
     host: str,
@@ -66,12 +67,23 @@
             return
 
         drop_database(sync_db_connection_url)
 
     request.addfinalizer(cleanup)
 
 
-async def redis_connection(worker_id: str) -> AsyncIterator[Redis]:
-    redis = connection.__wrapped__(db=int(worker_id[2:]), **EnvSettings.redis)
-    yield redis
+async def redis_connection_maker(
+    worker_id: str,
+) -> AsyncIterator[Callable[[], Awaitable[Redis]]]:
+    async def redis_connection() -> Redis:
+        return connection.__wrapped__(db=int(worker_id[2:]), **EnvSettings.redis)
+
+    yield redis_connection
+    redis = await redis_connection()
     await redis.flushdb()
     await redis.close()
+
+
+async def redis_connection(
+    redis_connection_maker: Callable[[], Awaitable[Redis]]
+) -> Redis:
+    return await redis_connection_maker()
```

### Comparing `codercore-1.9.0/codercore/test/pydantic.py` & `codercore-2.0.0/codercore/test/pydantic.py`

 * *Files identical despite different names*

### Comparing `codercore-1.9.0/codercore.egg-info/SOURCES.txt` & `codercore-2.0.0/codercore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 codercore/__init__.py
+codercore/types.py
 codercore.egg-info/PKG-INFO
 codercore.egg-info/SOURCES.txt
 codercore.egg-info/dependency_links.txt
 codercore.egg-info/requires.txt
 codercore.egg-info/top_level.txt
 codercore/db/__init__.py
 codercore/db/models.py
@@ -13,8 +14,9 @@
 codercore/lib/redis.py
 codercore/lib/settings.py
 codercore/lib/version.py
 codercore/lib/schemas/__init__.py
 codercore/lib/schemas/pydantic.py
 codercore/test/__init__.py
 codercore/test/fixtures.py
-codercore/test/pydantic.py
+codercore/test/pydantic.py
+tests/test_types.py
```

### Comparing `codercore-1.9.0/pyproject.toml` & `codercore-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codercore"
-version = "1.9.0"
+version = "2.0.0"
 description = "codercore"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'asyncpg ~= 0.27',
+    'asyncstdlib ~= 3.10',
     'bcrypt ~= 4.0',
     'cloud-sql-python-connector[asyncpg] ~= 1.1',
     'psycopg2 ~= 2.9',
     'pydantic ~= 1.10',
     'pytest ~= 7.2',
     'redis ~= 4.3',
     'sqlalchemy[asyncio] ~= 1.4',
@@ -30,15 +31,15 @@
 dev = [
     'black ~= 22.10',
     'flake8 ~= 6.0',
     'isort ~= 5.11',
 ]
 
 [tool.bumpver]
-current_version = "1.9.0"
+current_version = "2.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

