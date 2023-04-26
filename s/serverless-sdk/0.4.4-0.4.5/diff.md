# Comparing `tmp/serverless-sdk-0.4.4.tar.gz` & `tmp/serverless-sdk-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-voyigiic/serverless-sdk-0.4.4.tar", last modified: Thu Apr 20 20:12:25 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-m7ky189x/serverless-sdk-0.4.5.tar", last modified: Wed Apr 26 15:20:43 2023, max compression
```

## Comparing `serverless-sdk-0.4.4.tar` & `serverless-sdk-0.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/sls_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:12:25.000000 serverless-sdk-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-20 20:12:04.000000 serverless-sdk-0.4.4/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/warning_captured_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.4/PKG-INFO` & `serverless-sdk-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.4
+Version: 0.4.5
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.4/README.md` & `serverless-sdk-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/pyproject.toml` & `serverless-sdk-0.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel>=0.38.4",
 ]
 
 [project]
 name = "serverless-sdk"
-version = "0.4.4"
+version = "0.4.5"
 description = "Serverless SDK for Python"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
@@ -26,14 +26,15 @@
     "black>=22.12",
     "flask>=2.2.3",
     "pytest>=7.2",
     "pytest-httpserver>=1.0.6",
     "requests>=2.28.2",
     "ruff>=0.0.199",
     "urllib3>=1.26.15",
+    "yarl~=1.8.0",
 ]
 [project.urls]
 changelog = "https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md"
 documentation = "https://github.com/serverless/console/tree/main/python/packages/sdk"
 homepage = "https://www.serverless.com/console"
 repository = "https://github.com/serverless/console"
```

### Comparing `serverless-sdk-0.4.4/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.5/serverless_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.4
+Version: 0.4.5
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.4/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.5/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/__init__.py` & `serverless-sdk-0.4.5/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/exceptions.py` & `serverless-sdk-0.4.5/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.5/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.5/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/error.py` & `serverless-sdk-0.4.5/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.5/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
 import time
 import contextvars
 import contextlib
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from ..error import report as report_error
 from .import_hook import ImportHook
 import sls_sdk
 from wrapt import wrap_function_wrapper, ObjectProxy
+import io
+from typing import Iterable
 
 SDK = sls_sdk.serverlessSdk
 _IGNORE_FOLLOWING_REQUEST = contextvars.ContextVar("ignore", default=False)
 
 
 def ignore_following_request():
     _IGNORE_FOLLOWING_REQUEST.set(True)
@@ -19,14 +22,34 @@
 def reset_ignore_following_request():
     _IGNORE_FOLLOWING_REQUEST.set(False)
 
 
 _HTTP_SPAN = contextvars.ContextVar("http-span", default=None)
 
 
+def _decode_body(body):
+    if isinstance(body, bytes):
+        return body.decode("utf-8")
+    elif isinstance(body, str):
+        return body
+    elif isinstance(body, io.IOBase):
+        if body.seekable():
+            current_position = body.tell()
+            try:
+                return body.read().decode("utf-8")
+            finally:
+                body.seek(current_position)
+        else:
+            return body.peek().decode("utf-8")
+    elif isinstance(body, Iterable):
+        return b"".join(body).decode("utf-8")
+    else:
+        return None
+
+
 class BaseInstrumenter:
     def __init__(self, target_module):
         self._import_hook = ImportHook(target_module)
         self._is_installed = False
         self._module = None
 
     def install(self, should_monitor_request_response):
@@ -49,38 +72,43 @@
 
     def _install(self, module):
         raise NotImplementedError
 
     def _uninstall(self, module):
         raise NotImplementedError
 
-
-class NativeAIOHTTPInstrumenter(BaseInstrumenter):
-    def __init__(self):
-        super().__init__("aiohttp")
-        self._original_init = None
-
     def _capture_request_body(self, trace_span, body):
         if not body:
             return
         if not self.should_monitor_request_response:
             return
-        if len(body) > SDK._maximum_body_byte_length:
+
+        decoded = _decode_body(body)
+        length = len(decoded)
+
+        if length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "INPUT_BODY_TOO_LARGE",
                 trace_span,
             )
             return
         try:
-            trace_span.input = body.decode("utf-8")
+            trace_span.input = decoded
         except Exception:
             pass
 
+
+class NativeAIOHTTPInstrumenter(BaseInstrumenter):
+    def __init__(self):
+        super().__init__("aiohttp")
+        self._original_init = None
+
     async def _capture_response_body(self, trace_span, response):
+        # response is a aiohttp.ClientResponse object
         if not self.should_monitor_request_response:
             return
         if (
             response.content_length
             and response.content_length > SDK._maximum_body_byte_length
         ):
             SDK._report_notice(
@@ -88,15 +116,15 @@
                 "OUTPUT_BODY_TOO_LARGE",
                 trace_span,
             )
             return
         try:
             response_body = await response.read()
             if response_body:
-                trace_span.output = response_body.decode("utf-8")
+                trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     async def _on_request_start(self, session, trace_config_ctx, params):
         if hasattr(session, "_sls_ignore") and session._sls_ignore:
             return
         trace_config_ctx.start_time = time.perf_counter_ns()
@@ -190,14 +218,16 @@
 class NativeHTTPInstrumenter(BaseInstrumenter):
     def __init__(self):
         super().__init__("http.client")
         self._original_request = None
         self._original_getresponse = None
 
     def _instrumented_request(self):
+        # See https://docs.python.org/3/library/http.client.html#http.client.HTTPConnection.request
+        # for the signature of the request method
         def _func(_self, method, url, body=None, headers={}, *, encode_chunked=False):
             _self._sls_ignore = (
                 _IGNORE_FOLLOWING_REQUEST.get() or _DISABLE_NATIVE_INSTRUMENTATION.get()
             )
 
             if _self._sls_ignore:
                 return self._original_request(
@@ -240,32 +270,17 @@
                 trace_span.tags["http.error_code"] = ex.__class__.__name__
                 if trace_span.end_time is None:
                     trace_span.close()
                 raise
 
         return _func
 
-    def _capture_request_body(self, trace_span, body):
-        if not body:
-            return
-        if not self.should_monitor_request_response:
-            return
-        if len(body) > SDK._maximum_body_byte_length:
-            SDK._report_notice(
-                "Large body excluded",
-                "INPUT_BODY_TOO_LARGE",
-                trace_span,
-            )
-            return
-        try:
-            trace_span.input = body.decode("utf-8")
-        except Exception:
-            pass
-
     def _instrumented_getresponse(self):
+        # See https://docs.python.org/3/library/http.client.html#http.client.HTTPConnection.getresponse
+        # for the signature of the getresponse method
         def _func(_self, *args, **kwargs):
             trace_span = _HTTP_SPAN.get()
             if _self._sls_ignore or not trace_span:
                 return self._original_getresponse(_self, *args, **kwargs)
 
             try:
                 response = self._original_getresponse(_self, *args, **kwargs)
@@ -287,15 +302,15 @@
                 "OUTPUT_BODY_TOO_LARGE",
                 trace_span,
             )
             return
         try:
             response_body = response.peek()
             if response_body:
-                trace_span.output = response_body.decode("utf-8")
+                trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     def _install(self, module):
         self._module = module
         self._original_request = self._module.HTTPConnection.request
         self._original_getresponse = self._module.HTTPConnection.getresponse
@@ -375,46 +390,29 @@
         except Exception as ex:
             trace_span.tags["http.error_code"] = ex.__class__.__name__
             raise
         finally:
             if trace_span.end_time is None:
                 trace_span.close()
 
-    def _capture_request_body(self, trace_span, body):
-        if not body:
-            return
-        if not self.should_monitor_request_response:
-            return
-        if len(body) > SDK._maximum_body_byte_length:
-            SDK._report_notice(
-                "Large body excluded",
-                "INPUT_BODY_TOO_LARGE",
-                trace_span,
-            )
-            return
-        try:
-            trace_span.input = body.decode("utf-8")
-        except Exception:
-            pass
-
     def _capture_response_body(self, trace_span, response):
         if not self.should_monitor_request_response:
             return
         response_body = response.data
         response_length = int(response.headers.get("Content-Length", 0))
         if response_length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "OUTPUT_BODY_TOO_LARGE",
                 trace_span,
             )
             return
         try:
             if response_body:
-                trace_span.output = response_body.decode("utf-8")
+                trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     def _install(self, module):
         self._module = module
         wrap_function_wrapper(
             module.connectionpool.HTTPConnectionPool,
```

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/name.py` & `serverless-sdk-0.4.5/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.5/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.5/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.5/sls_sdk/lib/trace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 from __future__ import annotations
 from collections.abc import Iterable
 import logging
 import time
+import threading
 from typing import List, Optional, Callable
 from contextvars import ContextVar
 from backports.cached_property import cached_property  # available in Python >=3.8
 from typing_extensions import Final, Self
 import json
+from .instrumentation.import_hook import ImportHook
 from .timing import to_protobuf_epoch_timestamp
 from ..base import Nanoseconds, TraceId
 from ..exceptions import (
     ClosureOnClosedSpan,
     FutureSpanStartTime,
     InvalidType,
     UnreachableTrace,
     PastSpanEndTime,
     FutureSpanEndTime,
 )
 from .emitter import event_emitter
 from .id import generate_id
 from .name import get_resource_name
 from .tags import Tags, convert_tags_to_protobuf
+from wrapt import wrap_function_wrapper
 
 logger = logging.getLogger(__name__)
 
 
 __all__: Final[List[str]] = [
     "TraceSpan",
 ]
 
 
 TraceSpanContext = ContextVar[Optional["TraceSpan"]]
 
+_CONTEXT: Final[TraceSpanContext] = ContextVar("ctx", default=None)
 
-ctx: Final[TraceSpanContext] = ContextVar("ctx", default=None)
 root_span: Optional[TraceSpan] = None
 
 
+def _install_thread_hook(threading_module):
+    # Implementation of item 2 in `resolve_current_span`
+    def _thread_ctor_wrapper(actual_start, instance, args, kwargs):
+        if not hasattr(instance, "_parent_span"):
+            instance._parent_span = _CONTEXT.get() or root_span
+        result = actual_start(*args, **kwargs)
+        return result
+
+    wrap_function_wrapper(threading_module.Thread, "start", _thread_ctor_wrapper)
+
+
+_import_hook = ImportHook("threading")
+_import_hook.enable(_install_thread_hook)
+
+
 class TraceSpan:
     parent_span: Self
     name: str
     start_time: Nanoseconds
     end_time: Optional[Nanoseconds] = None
     _input: Optional[str] = None
     _output: Optional[str] = None
@@ -65,24 +83,38 @@
         self.sub_spans = []
 
         self._set_start_time(start_time)
         self._set_tags(tags)
         self._set_spans(immediate_descendants)
         self._on_close_by_root = on_close_by_root
 
+    def __str__(self):
+        parent = self.parent_span.name if self.parent_span else None
+        return f"{self.name} (parent={parent} - id={self.id})"
+
+    def __repr__(self):
+        return self.__str__()
+
     @staticmethod
     def resolve_current_span() -> Optional[TraceSpan]:
-        global root_span, ctx
-        span = ctx.get(None)
-
-        return span or root_span or None
+        # Current span is resolved in the following order:
+        # 1. Current context, this covers spans in async contexts
+        # 2. Current thread, this covers spans in threads
+        # 3. Root span, fallback to root if no other span can be resolved
+        # 4. None, if no span can be resolved
+        return (
+            _CONTEXT.get()
+            or getattr(threading.current_thread(), "_parent_span", None)
+            or root_span
+            or None
+        )
 
     def _set_spans(self, immediate_descendants: Optional[List[str]]):
         self._set_span_hierarchy()
-        self._set_ctx()
+        _CONTEXT.set(self)
         if immediate_descendants and len(immediate_descendants) > 0:
             TraceSpan(
                 immediate_descendants.pop(0),
                 start_time=self.start_time,
                 immediate_descendants=immediate_descendants,
             )
 
@@ -98,18 +130,14 @@
             self.parent_span = TraceSpan.resolve_current_span()
             while self.parent_span.end_time:
                 self.parent_span = self.parent_span.parent_span or root_span
 
         if self.parent_span:
             self.parent_span.sub_spans.append(self)
 
-    def _set_ctx(self, override: Optional[TraceSpan] = None):
-        global ctx
-        ctx.set(override or self)
-
     def _set_name(self, name):
         self.name = get_resource_name(name)
 
     def _set_tags(self, tags: Optional[Tags]):
         self.tags = Tags()
         self.custom_tags = Tags()
 
@@ -164,15 +192,14 @@
     def input(self, value: str):
         if value is not None and not isinstance(value, str):
             raise InvalidType("`input` must be a string.")
 
         self._input = value
 
     def close(self, end_time: Optional[Nanoseconds] = None):
-        global root_span, ctx
         default: Nanoseconds = time.perf_counter_ns()
         target_end_time = end_time
 
         if self.end_time is not None:
             raise ClosureOnClosedSpan(
                 f"Cannot close span ({self.name}): Span already closed"
             )
@@ -201,31 +228,32 @@
 
             if left_over_spans:
                 spans = ", ".join([s.name for s in left_over_spans])
                 logger.error(
                     "Serverless SDK Warning: Following trace spans didn't end before"
                     + f" end of lambda invocation: {spans}"
                 )
-            self._set_ctx()
+            _CONTEXT.set(self)
         else:
             # if this is not the root span and context points to this
             # then we need to reset the context to the first open ancestor span
-            if self is ctx.get(None):
+            current = _CONTEXT.get()
+            if self is current:
                 current = self.parent_span
                 found = False
                 # loop through ancestors
                 while current:
                     if not current.end_time:
                         # break at the first open ancestor and store it in the context
-                        self._set_ctx(current)
+                        _CONTEXT.set(current)
                         found = True
                         break
                     current = current.parent_span
                 if not found:
-                    self._set_ctx(root_span)
+                    _CONTEXT.set(root_span)
 
         event_emitter.emit("trace-span-close", self)
         return self
 
     def to_protobuf_dict(self):
         result = {
             "id": self.id,
```

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.5/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.5/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.4/tests/test_thread_safety.py` & `serverless-sdk-0.4.5/tests/test_thread_safety.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 from time import sleep
-import concurrent.futures
 import asyncio
 import random
 import pytest
 from pytest_httpserver import HTTPServer
 from werkzeug.wrappers import Request, Response
 
 SMALL_REQUEST_PAYLOAD = b"a"
 SMALL_RESPONSE_PAYLOAD = b"r"
 
 
 def print_spans(root, length=100):
+    print("\n")
     # normalize start and end times within [0, length]
     offset = root.start_time
     for span in root.spans:
         span.end_time -= offset
         span.start_time -= offset
     scale = root.end_time
     for span in root.spans:
@@ -24,30 +24,32 @@
 
     for span in root.spans:
         beginning = " " * span.start_time
         middle = "*" * (span.end_time - span.start_time)
         print(f"{span.name.ljust(20, ' ')}: {beginning}{middle}")
 
 
-def test_overlapping_spans_multithreaded(sdk):
+def test_overlapping_spans_multithreaded(instrumented_sdk):
     # given
+    import concurrent.futures
+
     parallelism = 10
 
     def _create_span_and_sleep(index):
         sleep(0.01 * index)
-        span = sdk._create_trace_span(f"child{index}")
+        span = instrumented_sdk._create_trace_span(f"child{index}")
         span.index = index
         sleep(0.01 * index)
-        inner_span = sdk._create_trace_span(f"grandchild{index}")
+        inner_span = instrumented_sdk._create_trace_span(f"grandchild{index}")
         sleep(0.01 * index)
         inner_span.close()
         sleep(0.01 * index)
         span.close()
 
-    root_span = sdk._create_trace_span("root")
+    root_span = instrumented_sdk._create_trace_span("root")
 
     # when
     with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
         futures = [
             executor.submit(_create_span_and_sleep, i) for i in range(parallelism)
         ]
         for future in concurrent.futures.as_completed(futures):
@@ -64,29 +66,29 @@
         assert sub_span.parent_span is root_span
         assert sub_span.name == f"child{idx}"
         assert len(sub_span.sub_spans) == 1
         assert sub_span.sub_spans[0].name == f"grandchild{idx}"
         assert sub_span.sub_spans[0].parent_span is sub_span
 
 
-def test_overlapping_spans_async(sdk):
+def test_overlapping_spans_async(instrumented_sdk):
     # given
     parallelism = 10
 
     async def _create_span_and_sleep(index):
         await asyncio.sleep(0.05)
-        span = sdk._create_trace_span(f"child{index}")
+        span = instrumented_sdk._create_trace_span(f"child{index}")
         await asyncio.sleep(0.05)
-        inner_span = sdk._create_trace_span(f"grandchild{index}")
+        inner_span = instrumented_sdk._create_trace_span(f"grandchild{index}")
         await asyncio.sleep(0.05)
         inner_span.close()
         await asyncio.sleep(0.05)
         span.close()
 
-    root_span = sdk._create_trace_span("root")
+    root_span = instrumented_sdk._create_trace_span("root")
 
     # when
     async def _run():
         await asyncio.gather(*[_create_span_and_sleep(i) for i in range(parallelism)])
 
     asyncio.run(_run())
 
@@ -101,37 +103,41 @@
         assert sub_span.parent_span is root_span
         assert sub_span.name == f"child{idx}"
         assert len(sub_span.sub_spans) == 1
         assert sub_span.sub_spans[0].name == f"grandchild{idx}"
         assert sub_span.sub_spans[0].parent_span is sub_span
 
 
-def test_overlapping_spans_async_with_multithreading(sdk):
+def test_overlapping_spans_async_with_multithreading(instrumented_sdk):
     # given
+    import concurrent.futures
+
     parallelism = 5
 
     async def _create_span_and_sleep(thread_index, async_index):
         await asyncio.sleep(0.05)
-        span = sdk._create_trace_span(f"thread{thread_index}.async{async_index}")
+        span = instrumented_sdk._create_trace_span(
+            f"thread{thread_index}.async{async_index}"
+        )
         span.index = thread_index * 100 + async_index + 1
         await asyncio.sleep(0.05)
-        inner_span = sdk._create_trace_span(
+        inner_span = instrumented_sdk._create_trace_span(
             f"thread{thread_index}.async{async_index}.child"
         )
         await asyncio.sleep(0.05)
         inner_span.close()
         await asyncio.sleep(0.05)
         span.close()
 
-    root_span = sdk._create_trace_span("root")
+    root_span = instrumented_sdk._create_trace_span("root")
 
     # when
     async def _run(thread_index):
         await asyncio.sleep(0.1)
-        span = sdk._create_trace_span(f"thread{thread_index}")
+        span = instrumented_sdk._create_trace_span(f"thread{thread_index}")
         span.index = thread_index * 100
         await asyncio.gather(
             *[_create_span_and_sleep(thread_index, i) for i in range(parallelism)]
         )
         await asyncio.sleep(0.1)
         span.close()
 
@@ -155,38 +161,42 @@
         assert len(sub_span.sub_spans) == parallelism
         for sub_idx, sub_sub_span in enumerate(sub_span.sub_spans):
             assert sub_sub_span.parent_span is sub_span
             assert sub_sub_span.name == f"thread{idx}.async{sub_idx}"
             assert len(sub_sub_span.sub_spans) == 1
 
 
-def test_overlapping_spans_async_with_multithreading_large_scale(sdk):
+def test_overlapping_spans_async_with_multithreading_large_scale(instrumented_sdk):
     # given
+    import concurrent.futures
+
     parallelism = 10
     scale = 1000
 
     async def _create_span_and_sleep(thread_index, async_index):
         await asyncio.sleep(0)
-        span = sdk._create_trace_span(f"thread{thread_index}.async{async_index}")
+        span = instrumented_sdk._create_trace_span(
+            f"thread{thread_index}.async{async_index}"
+        )
         span.index = thread_index * scale * 10 + async_index + 1
         await asyncio.sleep(0)
-        inner_span = sdk._create_trace_span(
+        inner_span = instrumented_sdk._create_trace_span(
             f"thread{thread_index}.async{async_index}.child"
         )
         await asyncio.sleep(0)
         inner_span.close()
         await asyncio.sleep(0)
         span.close()
 
-    root_span = sdk._create_trace_span("root")
+    root_span = instrumented_sdk._create_trace_span("root")
 
     # when
     async def _run(thread_index):
         await asyncio.sleep(0.1)
-        span = sdk._create_trace_span(f"thread{thread_index}")
+        span = instrumented_sdk._create_trace_span(f"thread{thread_index}")
         span.index = thread_index * scale * 10
         await asyncio.gather(
             *[_create_span_and_sleep(thread_index, i) for i in range(scale)]
         )
         await asyncio.sleep(0.1)
         span.close()
 
@@ -211,34 +221,36 @@
         for sub_idx, sub_sub_span in enumerate(sub_span.sub_spans):
             assert sub_sub_span.parent_span is sub_span
             assert sub_sub_span.name == f"thread{idx}.async{sub_idx}"
             assert len(sub_sub_span.sub_spans) == 1
 
 
 @pytest.mark.parametrize("is_error", [True, False])
-def test_captured_events_async_with_multithreading(sdk, is_error):
+def test_captured_events_async_with_multithreading(instrumented_sdk, is_error):
     # given
+    import concurrent.futures
+
     parallelism = 5
     scale = 100
     captured_events = []
 
     def _captured_event_handler(captured_event):
         captured_events.append(captured_event)
 
-    sdk._event_emitter.on("captured-event", _captured_event_handler)
+    instrumented_sdk._event_emitter.on("captured-event", _captured_event_handler)
 
     async def _create_captured_event_and_sleep(thread_index, async_index):
         await asyncio.sleep(0)
         if is_error:
-            sdk.capture_error(
+            instrumented_sdk.capture_error(
                 Exception("Captured error"),
                 tags={"threadIndex": thread_index, "asyncIndex": async_index},
             )
         else:
-            sdk.capture_warning(
+            instrumented_sdk.capture_warning(
                 "Captured warning",
                 tags={"threadIndex": thread_index, "asyncIndex": async_index},
             )
 
     # when
     async def _run(thread_index):
         await asyncio.sleep(0.1 + random.random() * 0.1)
@@ -265,67 +277,73 @@
         ]
         assert len(events) == scale
         events = sorted(events, key=lambda event: event.custom_tags["asyncIndex"])
         for async_index in range(scale):
             assert events[async_index].custom_tags["asyncIndex"] == async_index
 
 
-def test_set_tag_multithreaded(sdk):
+def test_set_tag_multithreaded(instrumented_sdk):
     # given
+    import concurrent.futures
+
     parallelism = 10
     scale = 10000
 
     def _set_tag_and_sleep(thread_index):
         sleep(0.05)
         for i in range(scale):
             unique_value = thread_index * scale * 10 + i
-            sdk.set_tag(f"tag{unique_value}", unique_value)
+            instrumented_sdk.set_tag(f"tag{unique_value}", unique_value)
 
     # when
     with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
         futures = [executor.submit(_set_tag_and_sleep, i) for i in range(parallelism)]
         for future in concurrent.futures.as_completed(futures):
             assert future.exception() is None
 
     # then
-    assert len(sdk._custom_tags) == parallelism * scale
+    assert len(instrumented_sdk._custom_tags) == parallelism * scale
 
     # given
     def _del_tag_and_sleep(thread_index):
         sleep(0.05)
         for i in range(scale):
             unique_value = thread_index * scale * 10 + i
-            del sdk._custom_tags[f"tag{unique_value}"]
+            del instrumented_sdk._custom_tags[f"tag{unique_value}"]
 
     # when
     with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
         futures = [executor.submit(_del_tag_and_sleep, i) for i in range(parallelism)]
         for future in concurrent.futures.as_completed(futures):
             assert future.exception() is None
 
     # then
-    assert len(sdk._custom_tags) == 0
+    assert len(instrumented_sdk._custom_tags) == 0
 
 
 @pytest.mark.parametrize(
     "request_body,response_body",
     [
         (SMALL_REQUEST_PAYLOAD, SMALL_RESPONSE_PAYLOAD),
     ],
 )
 def test_instrument_requests_multithreaded(
     instrumented_sdk, httpserver: HTTPServer, request_body, response_body
 ):
     # given
+    import concurrent.futures
+
     def handler(request: Request):
         return Response(response_body)
 
     httpserver.expect_request("/foo/bar").respond_with_handler(handler)
 
     root = instrumented_sdk._create_trace_span("rootspan")
+    assert len(root.spans) == 1
+
     parallelism = 5
 
     # when
     import requests
 
     def _run():
         requests.get(
@@ -353,7 +371,136 @@
                     "http.path": "/foo/bar",
                     "http.query_parameter_names": ["baz"],
                     "http.status_code": 200,
                 }
             ).items()
         )
         assert "User-Agent" in span.tags["http.request_header_names"]
+
+
+def test_overlapping_spans_multithreaded_hierarchy_plain(instrumented_sdk):
+    # given
+    import threading
+
+    def _create_grandchild_span():
+        span = instrumented_sdk._create_trace_span("grandchild")
+        span.close()
+
+    def _create_child_span():
+        span = instrumented_sdk._create_trace_span("child")
+        thread = threading.Thread(target=_create_grandchild_span)
+        thread.start()
+        thread.join()
+
+        span.close()
+
+    root_span = instrumented_sdk._create_trace_span("root")
+
+    # when
+    thread = threading.Thread(target=_create_child_span)
+    thread.start()
+    thread.join()
+
+    root_span.close()
+
+    # then
+    assert len(root_span.spans) == 3
+    (root, child, grandchild) = root_span.spans
+    assert root.name == "root"
+    assert child.name == "child"
+    assert grandchild.name == "grandchild"
+    assert root.parent_span is None
+    assert child.parent_span == root
+    assert grandchild.parent_span == child
+
+
+def test_overlapping_spans_multithreaded_hierarchy_thread_pool_executor(
+    instrumented_sdk,
+):
+    # given
+    import concurrent.futures
+
+    def _create_grandchild_span(parent_index, index):
+        span = instrumented_sdk._create_trace_span(
+            f"child{parent_index}grandchild{index}"
+        )
+        span.close()
+
+    def _create_child_span(index):
+        span = instrumented_sdk._create_trace_span(f"child{index}")
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
+            futures = [
+                executor.submit(_create_grandchild_span, index, i) for i in range(2)
+            ]
+            for future in concurrent.futures.as_completed(futures):
+                assert future.exception() is None
+
+        span.close()
+
+    root_span = instrumented_sdk._create_trace_span("root")
+
+    # when
+    with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
+        futures = [executor.submit(_create_child_span, i) for i in range(2)]
+        for future in concurrent.futures.as_completed(futures):
+            assert future.exception() is None
+
+    root_span.close()
+
+    # then
+    assert len(root_span.spans) == 7
+    root = [span for span in root_span.spans if span.name == "root"][0]
+    child0 = [span for span in root_span.spans if span.name == "child0"][0]
+    child1 = [span for span in root_span.spans if span.name == "child1"][0]
+    child0grandchild0 = [
+        span for span in root_span.spans if span.name == "child0grandchild0"
+    ][0]
+    child0grandchild1 = [
+        span for span in root_span.spans if span.name == "child0grandchild1"
+    ][0]
+    child1grandchild0 = [
+        span for span in root_span.spans if span.name == "child1grandchild0"
+    ][0]
+    child1grandchild1 = [
+        span for span in root_span.spans if span.name == "child1grandchild1"
+    ][0]
+    assert root.parent_span is None
+    assert child0.parent_span is root
+    assert child1.parent_span is root
+    assert child0grandchild0.parent_span is child0
+    assert child0grandchild1.parent_span is child0
+    assert child1grandchild0.parent_span is child1
+    assert child1grandchild1.parent_span is child1
+
+
+def test_overlapping_spans_async_hierarchy(instrumented_sdk):
+    # given
+    async def _create_child_span():
+        span = instrumented_sdk._create_trace_span("child")
+
+        async def _create_grandchild_span():
+            span = instrumented_sdk._create_trace_span("grandchild")
+            span.close()
+
+        await _create_grandchild_span()
+        span.close()
+
+    root_span = instrumented_sdk._create_trace_span("root")
+
+    # when
+    async def _run():
+        await _create_child_span()
+
+    asyncio.run(_run())
+
+    root_span.close()
+
+    # then
+    assert len(root_span.spans) == 3
+    (root, child, grandchild) = root_span.spans
+    assert root.name == "root"
+    assert child.name == "child"
+    assert grandchild.name == "grandchild"
+    assert root.parent_span is None
+    assert child.parent_span == root
+    assert grandchild.parent_span == child
```

