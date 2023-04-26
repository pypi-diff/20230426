# Comparing `tmp/starlette_cache-0.1.2.tar.gz` & `tmp/starlette_cache-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_cache-0.1.2.tar", last modified: Wed Apr 26 18:00:18 2023, max compression
+gzip compressed data, was "starlette_cache-0.1.3.tar", last modified: Wed Apr 26 18:08:07 2023, max compression
```

## Comparing `starlette_cache-0.1.2.tar` & `starlette_cache-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,18 @@
--rw-r--r--   0        0        0    11338 2023-04-13 07:55:12.541904 starlette_cache-0.1.2/LICENSE
--rw-r--r--   0        0        0     3164 2023-04-26 17:57:56.336553 starlette_cache-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542331 starlette_cache-0.1.2/examples/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542448 starlette_cache-0.1.2/examples/in_memory/__init__.py
--rw-r--r--   0        0        0     1625 2023-04-26 17:58:02.531701 starlette_cache-0.1.2/examples/in_memory/main.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542729 starlette_cache-0.1.2/examples/redis/__init__.py
--rw-r--r--   0        0        0      155 2023-04-26 17:57:56.337204 starlette_cache-0.1.2/examples/redis/index.html
--rw-r--r--   0        0        0     2317 2023-04-26 17:58:02.622627 starlette_cache-0.1.2/examples/redis/main.py
--rw-r--r--   0        0        0     1291 2023-04-26 18:00:18.080760 starlette_cache-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2399 2023-04-17 16:08:09.643766 starlette_cache-0.1.2/starlette_cache/__init__.py
--rw-r--r--   0        0        0      626 2023-04-17 16:08:09.696318 starlette_cache-0.1.2/starlette_cache/backends/__init__.py
--rw-r--r--   0        0        0     1629 2023-04-26 17:57:57.598056 starlette_cache-0.1.2/starlette_cache/backends/inmemory.py
--rw-r--r--   0        0        0      749 2023-04-26 17:58:02.800328 starlette_cache-0.1.2/starlette_cache/backends/memcached.py
--rw-r--r--   0        0        0     1383 2023-04-26 17:58:02.858598 starlette_cache-0.1.2/starlette_cache/backends/redis.py
--rw-r--r--   0        0        0      972 2023-04-15 20:23:14.571512 starlette_cache-0.1.2/starlette_cache/coder.py
--rw-r--r--   0        0        0     6849 2023-04-17 16:08:09.674597 starlette_cache-0.1.2/starlette_cache/decorator.py
--rw-r--r--   0        0        0      998 2023-04-22 10:16:05.582238 starlette_cache-0.1.2/starlette_cache/key_builder.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.544272 starlette_cache-0.1.2/starlette_cache/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.545730 starlette_cache-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      410 2023-04-16 04:19:35.458039 starlette_cache-0.1.2/tests/test_codecs.py
--rw-r--r--   0        0        0     2507 2023-04-16 04:19:35.469699 starlette_cache-0.1.2/tests/test_decorator.py
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 starlette_cache-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2876 2023-04-26 18:07:05.959336 starlette_cache-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542331 starlette_cache-0.1.3/examples/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542448 starlette_cache-0.1.3/examples/in_memory/__init__.py
+-rw-r--r--   0        0        0     1625 2023-04-26 17:58:02.531701 starlette_cache-0.1.3/examples/in_memory/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542729 starlette_cache-0.1.3/examples/redis/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-26 17:57:56.337204 starlette_cache-0.1.3/examples/redis/index.html
+-rw-r--r--   0        0        0     2317 2023-04-26 17:58:02.622627 starlette_cache-0.1.3/examples/redis/main.py
+-rw-r--r--   0        0        0     1313 2023-04-26 18:08:07.179689 starlette_cache-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2399 2023-04-17 16:08:09.643766 starlette_cache-0.1.3/starlette_cache/__init__.py
+-rw-r--r--   0        0        0      626 2023-04-17 16:08:09.696318 starlette_cache-0.1.3/starlette_cache/backends/__init__.py
+-rw-r--r--   0        0        0      972 2023-04-15 20:23:14.571512 starlette_cache-0.1.3/starlette_cache/coder.py
+-rw-r--r--   0        0        0     6849 2023-04-17 16:08:09.674597 starlette_cache-0.1.3/starlette_cache/decorator.py
+-rw-r--r--   0        0        0      998 2023-04-22 10:16:05.582238 starlette_cache-0.1.3/starlette_cache/key_builder.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.544272 starlette_cache-0.1.3/starlette_cache/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.545730 starlette_cache-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-16 04:19:35.458039 starlette_cache-0.1.3/tests/test_codecs.py
+-rw-r--r--   0        0        0     2507 2023-04-16 04:19:35.469699 starlette_cache-0.1.3/tests/test_decorator.py
+-rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 starlette_cache-0.1.3/PKG-INFO
```

### Comparing `starlette_cache-0.1.2/README.md` & `starlette_cache-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # starlette-cache
 
-Starlette fork of Starlette Cache with the fastapi_cache dependency removed.
+Starlette fork of Starlette Cache was originally a fork of fastapi-cache with the fastapi-cache dependency removed.
+It is now being completed rebuilt around cashews with starlette-async-jinja support.
 
 
+Stay tuned...
+
 ## Introduction
 
-`fastapi-cache` is a tool to cache fastapi response and function result, with backends support `redis`, `memcache`,
-and `dynamodb`.
+
 
 ## Features
 
-- Support `redis`, `memcache`, `dynamodb`, and `in-memory` backends.
-- Easily integration with `fastapi`.
-- Support http cache like `ETag` and `Cache-Control`.
+
 
 ## Requirements
 
-- `asyncio` environment.
-- `redis` if use `RedisBackend`.
-- `memcache` if use `MemcacheBackend`.
-- `aiobotocore` if use `DynamoBackend`.
 
 ## Install
 
 ```shell
 > pdm add startlette-cache
 ```
```

### Comparing `starlette_cache-0.1.2/examples/in_memory/main.py` & `starlette_cache-0.1.3/examples/in_memory/main.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/examples/redis/main.py` & `starlette_cache-0.1.3/examples/redis/main.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/pyproject.toml` & `starlette_cache-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,28 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "starlette-cache"
-version = "0.1.2"
+version = "0.1.3"
 description = "Cache for Starlette"
 dependencies = [
     "starlette>=0.26.1",
     "uvicorn>=0.21.1",
     "redis>=4.5.4",
     "aiomcache>=0.8.1",
     "pendulum>=2.1.2",
     "aiohttp>=3.8.4",
     "typing-extensions>=4.5.0",
     "msgspec>=0.14.1",
     "acb>=0.1.4",
     "starlette-async-jinja>=0.1.1",
+    "cashews>=6.0.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `starlette_cache-0.1.2/starlette_cache/__init__.py` & `starlette_cache-0.1.3/starlette_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/starlette_cache/backends/__init__.py` & `starlette_cache-0.1.3/starlette_cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/starlette_cache/coder.py` & `starlette_cache-0.1.3/starlette_cache/coder.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/starlette_cache/decorator.py` & `starlette_cache-0.1.3/starlette_cache/decorator.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/starlette_cache/key_builder.py` & `starlette_cache-0.1.3/starlette_cache/key_builder.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/tests/test_decorator.py` & `starlette_cache-0.1.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.2/PKG-INFO` & `starlette_cache-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-cache
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cache for Starlette
 Home-page: https://github.com/lesleslie/starlette-cache
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/starlette-cache
 Project-URL: Documentation, https://github.com/lesleslie/starlette-cache
 Project-URL: Repository, https://github.com/lesleslie/starlette-cache
@@ -15,38 +15,35 @@
 Requires-Dist: aiomcache>=0.8.1
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: msgspec>=0.14.1
 Requires-Dist: acb>=0.1.4
 Requires-Dist: starlette-async-jinja>=0.1.1
+Requires-Dist: cashews>=6.0.2
 Description-Content-Type: text/markdown
 
 # starlette-cache
 
-Starlette fork of Starlette Cache with the fastapi_cache dependency removed.
+Starlette fork of Starlette Cache was originally a fork of fastapi-cache with the fastapi-cache dependency removed.
+It is now being completed rebuilt around cashews with starlette-async-jinja support.
 
 
+Stay tuned...
+
 ## Introduction
 
-`fastapi-cache` is a tool to cache fastapi response and function result, with backends support `redis`, `memcache`,
-and `dynamodb`.
+
 
 ## Features
 
-- Support `redis`, `memcache`, `dynamodb`, and `in-memory` backends.
-- Easily integration with `fastapi`.
-- Support http cache like `ETag` and `Cache-Control`.
+
 
 ## Requirements
 
-- `asyncio` environment.
-- `redis` if use `RedisBackend`.
-- `memcache` if use `MemcacheBackend`.
-- `aiobotocore` if use `DynamoBackend`.
 
 ## Install
 
 ```shell
 > pdm add startlette-cache
 ```
```

