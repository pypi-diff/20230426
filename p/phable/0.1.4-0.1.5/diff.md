# Comparing `tmp/phable-0.1.4.tar.gz` & `tmp/phable-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phable-0.1.4.tar", max compression
+gzip compressed data, was "phable-0.1.5.tar", max compression
```

## Comparing `phable-0.1.4.tar` & `phable-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.4/LICENSE
--rw-r--r--   0        0        0      646 2023-03-19 01:51:40.173953 phable-0.1.4/README.rst
--rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.4/phable/__init__.py
--rw-r--r--   0        0        0    11158 2023-03-19 18:33:00.065921 phable-0.1.4/phable/scram.py
--rw-r--r--   0        0        0     1046 2023-03-19 00:43:52.432294 phable-0.1.4/phable/session.py
--rw-r--r--   0        0        0     2896 2023-03-19 00:44:05.387065 phable-0.1.4/phable/utils.py
--rw-r--r--   0        0        0      411 2023-03-22 22:53:45.134987 phable-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 phable-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2645 2023-04-25 15:37:14.606164 phable-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.5/phable/__init__.py
+-rw-r--r--   0        0        0     3111 2023-04-25 15:37:14.606725 phable-0.1.5/phable/http.py
+-rw-r--r--   0        0        0     5203 2023-04-25 15:37:14.607113 phable-0.1.5/phable/json_parser.py
+-rw-r--r--   0        0        0     3266 2023-04-25 15:37:14.607396 phable-0.1.5/phable/kinds.py
+-rw-r--r--   0        0        0     3251 2023-04-25 15:37:14.607665 phable-0.1.5/phable/phable.py
+-rw-r--r--   0        0        0    16671 2023-04-25 15:37:14.607992 phable-0.1.5/phable/scram.py
+-rw-r--r--   0        0        0      721 2023-04-25 15:48:21.586998 phable-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 phable-0.1.5/PKG-INFO
```

### Comparing `phable-0.1.4/LICENSE` & `phable-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phable-0.1.4/phable/utils.py` & `phable-0.1.5/phable/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import json
+import logging
 import ssl
-import typing
 import urllib.error
 import urllib.parse
 import urllib.request
 from email.message import Message
+from typing import Any, NamedTuple, Optional
 
+logger = logging.getLogger(__name__)
 
-class Response(typing.NamedTuple):
+
+class Response(NamedTuple):
     """Container for HTTP response."""
 
     body: str
     headers: Message
     status: int
     error_count: int = 0
 
-    def json(self) -> typing.Any:
+    def json(self) -> Any:
         """
         Decode body's JSON.
         Returns:
             Pythonic representation of the JSON object
         """
         try:
             output = json.loads(self.body)
         except json.JSONDecodeError:
             output = ""
         return output
 
 
 def request(
     url: str,
-    data: dict = None,
-    params: dict = None,
-    headers: dict = None,
+    data: Optional[dict[str, Any]] = None,
+    params: Optional[dict[str, Any]] = None,
+    headers: Optional[dict[str, Any]] = None,
     method: str = "GET",
     data_as_json: bool = True,
     error_count: int = 0,
 ) -> Response:
     """
     Perform HTTP request.
     Args:
@@ -69,14 +72,15 @@
     if params:
         url += "?" + urllib.parse.urlencode(params, doseq=True, safe="/")
 
     if data:
         if data_as_json:
             request_data = json.dumps(data).encode()
             headers["Content-Type"] = "application/json; charset=UTF-8"
+            logger.critical(f"Here is the request data:\n{request_data}")
         else:
             request_data = urllib.parse.urlencode(data).encode()
 
     httprequest = urllib.request.Request(
         url, data=request_data, headers=headers, method=method
     )
 
@@ -95,8 +99,8 @@
         response = Response(
             body=str(e.reason),
             headers=e.headers,
             status=e.code,
             error_count=error_count + 1,
         )
 
-    return response
+    return response  # .json()
```

