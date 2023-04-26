# Comparing `tmp/starlette_cache-0.1.1.tar.gz` & `tmp/starlette_cache-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_cache-0.1.1.tar", last modified: Sun Apr 16 15:36:59 2023, max compression
+gzip compressed data, was "starlette_cache-0.1.2.tar", last modified: Wed Apr 26 18:00:18 2023, max compression
```

## Comparing `starlette_cache-0.1.1.tar` & `starlette_cache-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11338 2023-04-13 07:55:12.541904 starlette_cache-0.1.1/LICENSE
--rw-r--r--   0        0        0     3165 2023-04-16 15:30:03.059476 starlette_cache-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542331 starlette_cache-0.1.1/examples/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542448 starlette_cache-0.1.1/examples/in_memory/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-16 04:19:35.480823 starlette_cache-0.1.1/examples/in_memory/main.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542729 starlette_cache-0.1.1/examples/redis/__init__.py
--rw-r--r--   0        0        0      154 2023-04-13 07:55:12.542843 starlette_cache-0.1.1/examples/redis/index.html
--rw-r--r--   0        0        0     2301 2023-04-16 04:19:35.475056 starlette_cache-0.1.1/examples/redis/main.py
--rw-r--r--   0        0        0     1311 2023-04-16 15:36:59.928462 starlette_cache-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2354 2023-04-16 04:19:32.481038 starlette_cache-0.1.1/starlette_cache/__init__.py
--rw-r--r--   0        0        0      628 2023-04-16 04:15:59.790112 starlette_cache-0.1.1/starlette_cache/backends/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-16 04:19:32.487149 starlette_cache-0.1.1/starlette_cache/backends/inmemory.py
--rw-r--r--   0        0        0      768 2023-04-16 04:19:35.462985 starlette_cache-0.1.1/starlette_cache/backends/memcached.py
--rw-r--r--   0        0        0     1375 2023-04-16 04:19:32.462355 starlette_cache-0.1.1/starlette_cache/backends/redis.py
--rw-r--r--   0        0        0      972 2023-04-15 20:23:14.571512 starlette_cache-0.1.1/starlette_cache/coder.py
--rw-r--r--   0        0        0     6790 2023-04-16 04:19:32.455772 starlette_cache-0.1.1/starlette_cache/decorator.py
--rw-r--r--   0        0        0      601 2023-04-15 22:16:18.665503 starlette_cache-0.1.1/starlette_cache/key_builder.py
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.544272 starlette_cache-0.1.1/starlette_cache/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 07:55:12.545730 starlette_cache-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      410 2023-04-16 04:19:35.458039 starlette_cache-0.1.1/tests/test_codecs.py
--rw-r--r--   0        0        0     2507 2023-04-16 04:19:35.469699 starlette_cache-0.1.1/tests/test_decorator.py
--rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 starlette_cache-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-04-13 07:55:12.541904 starlette_cache-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3164 2023-04-26 17:57:56.336553 starlette_cache-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542331 starlette_cache-0.1.2/examples/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542448 starlette_cache-0.1.2/examples/in_memory/__init__.py
+-rw-r--r--   0        0        0     1625 2023-04-26 17:58:02.531701 starlette_cache-0.1.2/examples/in_memory/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.542729 starlette_cache-0.1.2/examples/redis/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-26 17:57:56.337204 starlette_cache-0.1.2/examples/redis/index.html
+-rw-r--r--   0        0        0     2317 2023-04-26 17:58:02.622627 starlette_cache-0.1.2/examples/redis/main.py
+-rw-r--r--   0        0        0     1291 2023-04-26 18:00:18.080760 starlette_cache-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2399 2023-04-17 16:08:09.643766 starlette_cache-0.1.2/starlette_cache/__init__.py
+-rw-r--r--   0        0        0      626 2023-04-17 16:08:09.696318 starlette_cache-0.1.2/starlette_cache/backends/__init__.py
+-rw-r--r--   0        0        0     1629 2023-04-26 17:57:57.598056 starlette_cache-0.1.2/starlette_cache/backends/inmemory.py
+-rw-r--r--   0        0        0      749 2023-04-26 17:58:02.800328 starlette_cache-0.1.2/starlette_cache/backends/memcached.py
+-rw-r--r--   0        0        0     1383 2023-04-26 17:58:02.858598 starlette_cache-0.1.2/starlette_cache/backends/redis.py
+-rw-r--r--   0        0        0      972 2023-04-15 20:23:14.571512 starlette_cache-0.1.2/starlette_cache/coder.py
+-rw-r--r--   0        0        0     6849 2023-04-17 16:08:09.674597 starlette_cache-0.1.2/starlette_cache/decorator.py
+-rw-r--r--   0        0        0      998 2023-04-22 10:16:05.582238 starlette_cache-0.1.2/starlette_cache/key_builder.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.544272 starlette_cache-0.1.2/starlette_cache/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 07:55:12.545730 starlette_cache-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-16 04:19:35.458039 starlette_cache-0.1.2/tests/test_codecs.py
+-rw-r--r--   0        0        0     2507 2023-04-16 04:19:35.469699 starlette_cache-0.1.2/tests/test_decorator.py
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 starlette_cache-0.1.2/PKG-INFO
```

### Comparing `starlette_cache-0.1.1/LICENSE` & `starlette_cache-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.1/README.md` & `starlette_cache-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,7 @@
 
 `InMemoryBackend` store cache data in memory and use lazy delete, which mean if you don't access it after cached, it
 will not delete automatically.
 
 ## Tests and coverage
 
 ## Acknowlegdments
-
```

### Comparing `starlette_cache-0.1.1/examples/in_memory/main.py` & `starlette_cache-0.1.2/examples/in_memory/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,26 +51,26 @@
 @app.get("/kwargs")
 async def get_kwargs(name: str):
     return await func_kwargs(name, name=name)
 
 
 @app.get("/sync-me")
 @cache(namespace="test")
-def sync_me():
+def sync_me() -> int:
     # as per the fastapi docs, this sync function is wrapped in a thread,
     # thereby converted to async. fastapi-cache does the same.
     return 42
 
 
 @app.get("/cache_response_obj")
 @cache(namespace="test", expire=5)
 async def cache_response_obj():
     return JSONResponse({"a": 1})
 
 
 @app.on_event("startup")
-async def startup():
+async def startup() -> None:
     FastAPICache.init(InMemoryBackend())
 
 
 if __name__ == "__main__":
     uvicorn.run("main:app", debug=True, reload=True)
```

### Comparing `starlette_cache-0.1.1/examples/redis/main.py` & `starlette_cache-0.1.2/examples/redis/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pendulum
 import redis.asyncio as redis
 import uvicorn
 from redis.asyncio.connection import ConnectionPool
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
-from starlette_cache import FastAPICache
+from starlette_cache import StarletteCache
 from starlette_cache.backends.redis import RedisBackend
 from starlette_cache.coder import PickleCoder
 from starlette_cache.decorator import cache
 
 app = FastAPI()
 
 app.mount(path="/static", app=StaticFiles(directory="./"), name="static")
@@ -34,15 +34,15 @@
 @cache(namespace="test", expire=10)
 async def index():
     return dict(ret=await get_ret())
 
 
 @app.get("/clear")
 async def clear():
-    return await FastAPICache.clear(namespace="test")
+    return await StarletteCache.clear(namespace="test")
 
 
 @app.get("/date")
 @cache(namespace="test", expire=10)
 async def get_data(request: Request, response: Response):
     return pendulum.today()
 
@@ -74,15 +74,15 @@
 @app.get("/cache_response_obj")
 @cache(namespace="test", expire=5)
 async def cache_response_obj():
     return JSONResponse({"a": 1})
 
 
 @app.on_event("startup")
-async def startup():
+async def startup() -> None:
     pool = ConnectionPool.from_url(url="redis://redis")
     r = redis.Redis(connection_pool=pool)
-    FastAPICache.init(RedisBackend(r), prefix="fastapi-cache")
+    StarletteCache.init(RedisBackend(r), prefix="starlette-cache")
 
 
 if __name__ == "__main__":
     uvicorn.run("main:app", debug=True, reload=True)
```

### Comparing `starlette_cache-0.1.1/pyproject.toml` & `starlette_cache-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 [tool.pdm.dev-dependencies]
 dev = [
-    "httpx>=0.24.0",
-    "pytest>=7.3.1",
-    "black>=23.3.0",
-    "coverage>=7.2.3",
-    "ruff>=0.0.261",
-    "mypy>=1.2.0",
+    "crackerjack>=0.1.7",
+    "pre-commit>=3.2.2",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
+fix = true
+show-fixes = true
+show-source = true
 
 [tool.ruff.isort]
-split-on-trailing-comma = true
-force-wrap-aliases = true
-combine-as-imports = true
+force-single-line = true
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
 strict = true
-
-[tool.deptry]
+pretty = true
 
 [tool.refurb]
+enable_all = true
+
+[tool.pytype]
+inputs = [
+    "package_name",
+]
 
 [project]
 name = "starlette-cache"
-version = "0.1.1"
+version = "0.1.2"
 description = "Cache for Starlette"
-authors = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
 dependencies = [
     "starlette>=0.26.1",
     "uvicorn>=0.21.1",
     "redis>=4.5.4",
     "aiomcache>=0.8.1",
     "pendulum>=2.1.2",
     "aiohttp>=3.8.4",
     "typing-extensions>=4.5.0",
     "msgspec>=0.14.1",
-    "starlette-async-jinja>=0.1.0",
-    "acb>=0.1.1",
+    "acb>=0.1.4",
+    "starlette-async-jinja>=0.1.1",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
+authors = [
+    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
+]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
 homepage = "https://github.com/lesleslie/starlette-cache"
 documentation = "https://github.com/lesleslie/starlette-cache"
```

### Comparing `starlette_cache-0.1.1/starlette_cache/__init__.py` & `starlette_cache-0.1.2/starlette_cache/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import Callable, Optional, Type
+from typing import Callable
+from typing import Optional
+from typing import Type
 
 from backends import Backend
-from coder import Coder, JsonCoder
+from coder import Coder
+from coder import JsonCoder
 from key_builder import default_key_builder
 
 
 class StarletteCache:
     _backend: Optional[Backend] = None
     _prefix: Optional[str] = None
     _expire: Optional[int] = None
@@ -70,14 +73,14 @@
 
     @classmethod
     def get_enable(cls) -> bool:
         return cls._enable
 
     @classmethod
     async def clear(
-            cls, namespace: Optional[str] = None, key: Optional[str] = None
+        cls, namespace: Optional[str] = None, key: Optional[str] = None
     ) -> int:
         assert (
-                cls._backend and cls._prefix is not None
+            cls._backend and cls._prefix is not None
         ), "You must call init first!"  # nosec: B101
         namespace = cls._prefix + (":" + namespace if namespace else "")
         return await cls._backend.clear(namespace, key)
```

### Comparing `starlette_cache-0.1.1/starlette_cache/backends/__init__.py` & `starlette_cache-0.1.2/starlette_cache/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 
-class BaseCache(ABC):
+class Backend(ABC):
     @abstractmethod
     async def get_with_ttl(self, key: str) -> t.Tuple[int, t.Optional[str]]:
         raise NotImplementedError
 
     @abstractmethod
     async def get(self, key: str) -> t.Optional[str]:
         raise NotImplementedError
```

### Comparing `starlette_cache-0.1.1/starlette_cache/backends/inmemory.py` & `starlette_cache-0.1.2/starlette_cache/backends/inmemory.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             return None
 
     async def set(self, key: str, value: str, expire: Optional[int] = None) -> None:
         async with self._lock:
             self._store[key] = Value(value, self._now + (expire or 0))
 
     async def clear(
-            self, namespace: Optional[str] = None, key: Optional[str] = None
+        self, namespace: Optional[str] = None, key: Optional[str] = None
     ) -> int:
         count = 0
         if namespace:
             keys = list(self._store.keys())
             for key in keys:
                 if key.startswith(namespace):
                     del self._store[key]
```

### Comparing `starlette_cache-0.1.1/starlette_cache/backends/memcached.py` & `starlette_cache-0.1.2/starlette_cache/backends/memcached.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from typing import Optional, Tuple
 
 from aiomcache import Client
 from . import Backend
 
 
 class MemcachedBackend(Backend):
-    def __init__(self, mcache: Client):
+    def __init__(self, mcache: Client) -> None:
         self.mcache = mcache
 
     async def get_with_ttl(self, key: str) -> Tuple[int, Optional[str]]:
         return 3600, await self.mcache.get(key.encode())
-    
-    
+
     async def get(self, key: str) -> Optional[str]:
         return await self.mcache.get(key, key.encode())
-    
-    
+
     async def set(self, key: str, value: str, expire: Optional[int] = None) -> None:
         await self.mcache.set(key.encode(), value.encode(), exptime=expire or 0)
-    
-    
+
     async def clear(
         self, namespace: Optional[str] = None, key: Optional[str] = None
     ) -> int:
         raise NotImplementedError
```

### Comparing `starlette_cache-0.1.1/starlette_cache/backends/redis.py` & `starlette_cache-0.1.2/starlette_cache/backends/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Tuple
 
 from redis.asyncio.client import AbstractRedis as AioRedis
 from redis.asyncio import RedisCluster as AioRedisCluster
 
 
 class RedisBackend(AioRedis):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.redis = redis
         self.is_cluster = isinstance(redis, AioRedisCluster)
 
     async def get_with_ttl(self, key: str) -> Tuple[int, str]:
         async with self.redis.pipeline(transaction=not self.is_cluster) as pipe:
             return await pipe.ttl(key).get(key).execute()
```

### Comparing `starlette_cache-0.1.1/starlette_cache/coder.py` & `starlette_cache-0.1.2/starlette_cache/coder.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.1/starlette_cache/decorator.py` & `starlette_cache-0.1.2/starlette_cache/decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import inspect
 import logging
 import sys
 from functools import wraps
-from typing import Any, Awaitable, Callable, Optional, Type, TypeVar
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import Optional
+from typing import Type
+from typing import TypeVar
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
 
-from fastapi.concurrency import run_in_threadpool
+from starlette.concurrency import run_in_threadpool
 from starlette.requests import Request
 from starlette.responses import Response
 
-from starlette_cache import FastAPICache
+from starlette_cache import StarletteCache
 from starlette_cache.coder import Coder
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 def cache(
-        expire: Optional[int] = None,
-        coder: Optional[Type[Coder]] = None,
+    expire: Optional[int] = None,
+    coder: Optional[Type[Coder]] = None,
     key_builder: Optional[Callable[..., Any]] = None,
     namespace: Optional[str] = "",
 ) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]:
     """
     cache all function
     :param namespace:
     :param expire:
@@ -37,21 +42,29 @@
 
     :return:
     """
 
     def wrapper(func: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]:
         signature = inspect.signature(func)
         request_param = next(
-    (param for param in signature.parameters.values() if param.annotation is Request),
-    None,
-)
+            (
+                param
+                for param in signature.parameters.values()
+                if param.annotation is Request
+            ),
+            None,
+        )
         response_param = next(
-    (param for param in signature.parameters.values() if param.annotation is Response),
-    None,
-)
+            (
+                param
+                for param in signature.parameters.values()
+                if param.annotation is Response
+            ),
+            None,
+        )
         parameters = []
         extra_params = []
         for p in signature.parameters.values():
             if p.kind <= inspect.Parameter.KEYWORD_ONLY:
                 parameters.append(p)
             else:
                 extra_params.append(p)
@@ -79,17 +92,14 @@
         @wraps(func)
         async def inner(*args: P.args, **kwargs: P.kwargs) -> R:
             nonlocal coder
             nonlocal expire
             nonlocal key_builder
 
             async def ensure_async_func(*args: P.args, **kwargs: P.kwargs) -> R:
-                """Run cached sync functions in thread pool just like FastAPI."""
-                # if the wrapped function does NOT have request or response in its function signature,
-                # make sure we don't pass them in as keyword arguments
                 if not request_param:
                     kwargs.pop("request", None)
                 if not response_param:
                     kwargs.pop("response", None)
 
                 if inspect.iscoroutinefunction(func):
                     # async, return as is.
@@ -101,21 +111,24 @@
                     # sync, wrap in thread and return async
                     # see above why we have to await even although caller also awaits.
                     return await run_in_threadpool(func, *args, **kwargs)
 
             copy_kwargs = kwargs.copy()
             request: Optional[Request] = copy_kwargs.pop("request", None)
             response: Optional[Response] = copy_kwargs.pop("response", None)
-            if (request and request.headers.get("Cache-Control") in ("no-store", "no-cache"))or not FastAPICache.get_enable():
+            if (
+                request
+                and request.headers.get("Cache-Control") in ("no-store", "no-cache")
+            ) or not StarletteCache.get_enable():
                 return await ensure_async_func(*args, **kwargs)
 
-            coder = coder or FastAPICache.get_coder()
-            expire = expire or FastAPICache.get_expire()
-            key_builder = key_builder or FastAPICache.get_key_builder()
-            backend = FastAPICache.get_backend()
+            coder = coder or StarletteCache.get_coder()
+            expire = expire or StarletteCache.get_expire()
+            key_builder = key_builder or StarletteCache.get_key_builder()
+            backend = StarletteCache.get_backend()
 
             if inspect.iscoroutinefunction(key_builder):
                 cache_key = await key_builder(
                     func,
                     namespace,
                     request=request,
                     response=response,
```

### Comparing `starlette_cache-0.1.1/starlette_cache/key_builder.py` & `starlette_cache-0.1.2/starlette_cache/key_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from typing import Callable, Optional
 
 from starlette.requests import Request
 from starlette.responses import Response
-from acb.hash import hash
+from acb import hash
 from . import StarletteCache
 
 
+def key_name(self, name: AsyncPath | str, prefix: str = None) -> str:
+    prefix = prefix if prefix else self.prefix
+    if isinstance(name, str):
+        if name.startswith(f"{prefix}:"):
+            return name
+        return f"{prefix}:{hash.blake2b([name])}"
+    parent = name.parent if "base" in name.parts else name.parent.parent
+    return f"{prefix}:{hash.blake2b([parent.stem, name.stem])}"
+
+
 def default_key_builder(
     func: Callable,
     namespace: Optional[str] = "",
     request: Optional[Request] = None,
     response: Optional[Response] = None,
     args: Optional[tuple] = None,
     kwargs: Optional[dict] = None,
```

### Comparing `starlette_cache-0.1.1/tests/test_decorator.py` & `starlette_cache-0.1.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `starlette_cache-0.1.1/PKG-INFO` & `starlette_cache-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-cache
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cache for Starlette
 Home-page: https://github.com/lesleslie/starlette-cache
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/starlette-cache
 Project-URL: Documentation, https://github.com/lesleslie/starlette-cache
 Project-URL: Repository, https://github.com/lesleslie/starlette-cache
@@ -13,16 +13,16 @@
 Requires-Dist: uvicorn>=0.21.1
 Requires-Dist: redis>=4.5.4
 Requires-Dist: aiomcache>=0.8.1
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: msgspec>=0.14.1
-Requires-Dist: starlette-async-jinja>=0.1.0
-Requires-Dist: acb>=0.1.1
+Requires-Dist: acb>=0.1.4
+Requires-Dist: starlette-async-jinja>=0.1.1
 Description-Content-Type: text/markdown
 
 # starlette-cache
 
 Starlette fork of Starlette Cache with the fastapi_cache dependency removed.
 
 
@@ -145,8 +145,7 @@
 
 `InMemoryBackend` store cache data in memory and use lazy delete, which mean if you don't access it after cached, it
 will not delete automatically.
 
 ## Tests and coverage
 
 ## Acknowlegdments
-
```

