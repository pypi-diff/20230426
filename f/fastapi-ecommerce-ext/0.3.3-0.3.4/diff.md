# Comparing `tmp/fastapi_ecommerce_ext-0.3.3.tar.gz` & `tmp/fastapi_ecommerce_ext-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.3.3.tar", last modified: Fri Apr 21 03:31:07 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.3.4.tar", last modified: Wed Apr 26 15:53:58 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.3.3.tar` & `fastapi_ecommerce_ext-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.804811 fastapi_ecommerce_ext-0.3.3/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      382 2023-04-21 03:31:07.804811 fastapi_ecommerce_ext-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.791811 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.803812 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-21 03:31:05.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     2663 2023-04-21 03:21:49.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.800811 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      382 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 03:31:07.805811 fastapi_ecommerce_ext-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-21 03:31:05.000000 fastapi_ecommerce_ext-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:53:58.366038 fastapi_ecommerce_ext-0.3.4/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      382 2023-04-26 15:53:58.366038 fastapi_ecommerce_ext-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 15:53:58.355067 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:53:58.365126 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-21 03:31:05.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     2667 2023-04-26 15:53:56.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:53:58.362126 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      382 2023-04-26 15:53:58.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-26 15:53:58.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:53:58.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-26 15:53:58.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 15:53:58.000000 fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-26 15:53:58.367043 fastapi_ecommerce_ext-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-26 15:53:56.000000 fastapi_ecommerce_ext-0.3.4/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.3.3/LICENSE.txt` & `fastapi_ecommerce_ext-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.3.4/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,22 @@
         try:
             await self.log_before_response(request)
             st = time.time()
             response = await call_next(request)
             elapsed = f"{time.time() - st:0.10f} sec"
             response.headers.append("X-Response-Time", elapsed)
         except Exception as e:
-            if request.app.debug:
-                logger.exception(e)
             response = JSONResponse(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 content={"detail": f"{e.__class__.__name__} - {e.args}"},
                 media_type="application/json",
             )
-            return await self.log_after_response(request, response)
+            if request.app.debug:
+                logger.exception(e)
+                return await self.log_after_response(request, response)
         return response
 
     @staticmethod
     def log_format(request: Request):
         return f"{request.client.host}:{request.client.port} - {request.method} {request.url}"
 
     async def log_before_response(self, request: Request):
```

### Comparing `fastapi_ecommerce_ext-0.3.3/setup.py` & `fastapi_ecommerce_ext-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "0.3.3"
+version = "0.3.4"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```

