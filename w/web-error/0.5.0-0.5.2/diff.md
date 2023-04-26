# Comparing `tmp/web_error-0.5.0.tar.gz` & `tmp/web_error-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_error-0.5.0.tar", max compression
+gzip compressed data, was "web_error-0.5.2.tar", max compression
```

## Comparing `web_error-0.5.0.tar` & `web_error-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.0/LICENSE
--rw-r--r--   0        0        0     3068 2023-02-19 13:50:24.308619 web_error-0.5.0/README.md
--rw-r--r--   0        0        0     1772 2023-02-19 13:50:24.307619 web_error-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-02-19 13:50:24.308619 web_error-0.5.0/web_error/__init__.py
--rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.0/web_error/constant.py
--rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.0/web_error/error.py
--rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.0/web_error/handler/__init__.py
--rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.0/web_error/handler/aiohttp.py
--rw-r--r--   0        0        0     1731 2023-02-19 13:21:46.864564 web_error-0.5.0/web_error/handler/fastapi.py
--rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.0/web_error/handler/flask.py
--rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.0/web_error/handler/pyramid.py
--rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.0/web_error/handler/starlette.py
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 web_error-0.5.0/setup.py
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3068 2023-04-25 17:11:29.892937 web_error-0.5.2/README.md
+-rw-r--r--   0        0        0     1772 2023-04-25 17:11:29.892937 web_error-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-25 17:11:29.892937 web_error-0.5.2/web_error/__init__.py
+-rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.2/web_error/constant.py
+-rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.2/web_error/error.py
+-rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.2/web_error/handler/__init__.py
+-rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.2/web_error/handler/aiohttp.py
+-rw-r--r--   0        0        0     2521 2023-04-25 17:03:40.700398 web_error-0.5.2/web_error/handler/fastapi.py
+-rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.2/web_error/handler/flask.py
+-rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.2/web_error/handler/pyramid.py
+-rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.2/web_error/handler/starlette.py
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 web_error-0.5.2/setup.py
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.2/PKG-INFO
```

### Comparing `web_error-0.5.0/LICENSE` & `web_error-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web_error-0.5.0/README.md` & `web_error-0.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Web Errors v0.5.0
+# Web Errors v0.5.2
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
 ![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
```

### Comparing `web_error-0.5.0/pyproject.toml` & `web_error-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web_error"
-version = "0.5.0"
+version = "0.5.2"
 description = "Web based error utils"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/web-error/"
 homepage="https://github.com/EdgyEdgemond/web-error/"
 readme = "README.md"
```

### Comparing `web_error-0.5.0/web_error/error.py` & `web_error-0.5.2/web_error/error.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.0/web_error/handler/aiohttp.py` & `web_error-0.5.2/web_error/handler/aiohttp.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.0/web_error/handler/fastapi.py` & `web_error-0.5.2/web_error/handler/pyramid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,54 @@
-import json
 import logging
-from typing import List, Optional
+from typing import Dict
 
-from fastapi.exceptions import RequestValidationError
-from starlette.exceptions import HTTPException
+from pyramid.httpexceptions import HTTPException
+from pyramid.request import Request  # noqa: TCH002
+from pyramid.view import view_config
 
 from web_error import constant
 from web_error.error import HttpException
-from web_error.handler import starlette
 
 logger = logging.getLogger(__name__)
 
 
-def exception_handler(request: starlette.Request, exc: Exception) -> starlette.JSONResponse:  # noqa: ARG001
+@view_config(context=HTTPException, renderer="json")
+def pyramid_handler(exc: HTTPException, request: Request) -> Dict:
+    status = exc.code
+    response = {
+        "message": exc.explanation,
+        "debug_message": exc.detail,
+        "code": None,
+    }
+
+    if "predicate mismatch" in exc.detail and "request_method" in exc.detail:
+        status = 405
+        response["message"] = "Request method not allowed."
+
+    if status >= constant.SERVER_ERROR:
+        logger.exception(exc.explanation)
+
+    request.response.status = status
+    return response
+
+
+@view_config(context=Exception, renderer="json")
+def exception_handler(exc: Exception, request: Request) -> Dict:
+    # If the view has two formal arguments, the first is the context.
+    # The context is always available as ``request.context`` too.
     status = constant.SERVER_ERROR
     message = "Unhandled exception occurred."
     response = {
         "message": message,
         "debug_message": str(exc),
         "code": None,
     }
 
-    if isinstance(exc, HTTPException):
-        response["message"] = exc.detail
-        status = exc.status_code
-
-    if isinstance(exc, RequestValidationError):
-        response["message"] = "Request validation error."
-        response["debug_message"] = json.loads(exc.json())
-        status = 422
-
     if isinstance(exc, HttpException):
         response = exc.marshal()
         status = exc.status
 
     if status >= constant.SERVER_ERROR:
-        logger.exception(message, exc_info=(type(exc), exc, exc.__traceback__))
+        logger.exception(message)
 
-    return starlette.JSONResponse(
-        status_code=status,
-        content=response,
-    )
-
-
-def generate_handler_with_cors(
-    allow_origins: Optional[List[str]] = None,
-    allow_credentials: bool = True,
-    allow_methods: Optional[List[str]] = None,
-    allow_headers: Optional[List[str]] = None,
-) -> starlette.JSONResponse:
-    return starlette.generate_handler_with_cors(
-        allow_origins=allow_origins,
-        allow_credentials=allow_credentials,
-        allow_methods=allow_methods,
-        allow_headers=allow_headers,
-        _exception_handler=exception_handler,
-    )
+    request.response.status = status
+    return response
```

### Comparing `web_error-0.5.0/web_error/handler/flask.py` & `web_error-0.5.2/web_error/handler/flask.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.0/web_error/handler/starlette.py` & `web_error-0.5.2/web_error/handler/starlette.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.0/setup.py` & `web_error-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['web_error', 'web_error.handler']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'web-error',
-    'version': '0.5.0',
+    'version': '0.5.2',
     'description': 'Web based error utils',
-    'long_description': '# Web Errors v0.5.0\n[![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)\n![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)\n![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)\n[![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)\n\n`web_error` is a set of exceptions and handlers for use in web apis to support easy error management and responses\n\nEach exception easily marshals to JSON for use in api errors. Handlers for different web frameworks are provided.\n\n\n## Errors\n\nThe base `web_error.error.HttpException` accepts a `message`, `debug_message`, `code` and `status` (default 500)\n\nAnd will render a response with status as the status code:\n\n```json\n{\n    "code": "code",\n    "message": "message",\n    "debug_message": "debug_message",\n}\n```\n\nSome convenience Exceptions are provided, to create custom error subclass these\nand define `message` and `code` attributes.\n\n* `web_error.error.ServerException` provides status 500 errors\n* `web_error.error.BadRequestException` provides status 400 errors\n* `web_error.error.UnauthorisedException` provides status 401 errors\n* `web_error.error.NotFoundException` provides status 404 errors\n\n### Custom Errors\n\nSubclassing the convenience classes provide a simple way to consistently raise the same error\nand message.\n\nCode is an optional attribute to provide a unique value to parse in a frontend/client instead of\nmatching against messages.\n\n```python\nfrom web_error.error import NotFoundException\n\n\nclass UserNotFoundError(NotFoundException):\n    message = "User not found."\n    code = "E001"\n```\n\n\n## FastAPI\n\nInclude the `exception_handler` in your app.\n\n```python\n    exception_handler = web_error.handler.fastapi.exception_handler\n\n    return FastAPI(\n        exception_handlers={\n            Exception: exception_handler,\n            RequestValidationError: exception_handler,\n            HTTPException: exception_handler,\n        },\n    )\n```\n## Pyramid\n\nInclude the pyramid exception handlers in your config.\n\n```python\ndef main(global_config, **config_blob):\n    config = Configurator(settings=config_blob)\n\n    ...\n\n    config.scan("web_error.handler.pyramid")\n\n    return config.make_wsgi_app()\n```\n\nThis will handle all unexpected errors, and any app specific errors.\n\n```python\n@view_config(route_name="test", renderer="json")\ndef test(request):\n    raise UserNotFoundError("debug message")\n```\n\n\n## Flask\n\nRegister the error handler with your application\n\n```python\napp.register_error_handler(Exception, web_error.handler.flask.exception_handler)\n```\n\n## Aiohttp\n\nDecorate your views with the error handler.\n\n```python\n@web_error.handler.aiohttp.view_error_handler\nasync def user(self):\n    raise UserNotFoundError("debug message")\n```\n',
+    'long_description': '# Web Errors v0.5.2\n[![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)\n[![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)\n![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)\n![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)\n[![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)\n\n`web_error` is a set of exceptions and handlers for use in web apis to support easy error management and responses\n\nEach exception easily marshals to JSON for use in api errors. Handlers for different web frameworks are provided.\n\n\n## Errors\n\nThe base `web_error.error.HttpException` accepts a `message`, `debug_message`, `code` and `status` (default 500)\n\nAnd will render a response with status as the status code:\n\n```json\n{\n    "code": "code",\n    "message": "message",\n    "debug_message": "debug_message",\n}\n```\n\nSome convenience Exceptions are provided, to create custom error subclass these\nand define `message` and `code` attributes.\n\n* `web_error.error.ServerException` provides status 500 errors\n* `web_error.error.BadRequestException` provides status 400 errors\n* `web_error.error.UnauthorisedException` provides status 401 errors\n* `web_error.error.NotFoundException` provides status 404 errors\n\n### Custom Errors\n\nSubclassing the convenience classes provide a simple way to consistently raise the same error\nand message.\n\nCode is an optional attribute to provide a unique value to parse in a frontend/client instead of\nmatching against messages.\n\n```python\nfrom web_error.error import NotFoundException\n\n\nclass UserNotFoundError(NotFoundException):\n    message = "User not found."\n    code = "E001"\n```\n\n\n## FastAPI\n\nInclude the `exception_handler` in your app.\n\n```python\n    exception_handler = web_error.handler.fastapi.exception_handler\n\n    return FastAPI(\n        exception_handlers={\n            Exception: exception_handler,\n            RequestValidationError: exception_handler,\n            HTTPException: exception_handler,\n        },\n    )\n```\n## Pyramid\n\nInclude the pyramid exception handlers in your config.\n\n```python\ndef main(global_config, **config_blob):\n    config = Configurator(settings=config_blob)\n\n    ...\n\n    config.scan("web_error.handler.pyramid")\n\n    return config.make_wsgi_app()\n```\n\nThis will handle all unexpected errors, and any app specific errors.\n\n```python\n@view_config(route_name="test", renderer="json")\ndef test(request):\n    raise UserNotFoundError("debug message")\n```\n\n\n## Flask\n\nRegister the error handler with your application\n\n```python\napp.register_error_handler(Exception, web_error.handler.flask.exception_handler)\n```\n\n## Aiohttp\n\nDecorate your views with the error handler.\n\n```python\n@web_error.handler.aiohttp.view_error_handler\nasync def user(self):\n    raise UserNotFoundError("debug message")\n```\n',
     'author': 'Daniel Edgecombe',
     'author_email': 'edgy.edgemond@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/EdgyEdgemond/web-error/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `web_error-0.5.0/PKG-INFO` & `web_error-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-error
-Version: 0.5.0
+Version: 0.5.2
 Summary: Web based error utils
 Home-page: https://github.com/EdgyEdgemond/web-error/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/EdgyEdgemond/web-error/
 Description-Content-Type: text/markdown
 
-# Web Errors v0.5.0
+# Web Errors v0.5.2
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
 ![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
```

