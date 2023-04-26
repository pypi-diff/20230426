# Comparing `tmp/oidc_client-0.2.3.tar.gz` & `tmp/oidc_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_client-0.2.3.tar", max compression
+gzip compressed data, was "oidc_client-0.2.4.tar", max compression
```

## Comparing `oidc_client-0.2.3.tar` & `oidc_client-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1085 2023-04-24 00:12:01.040127 oidc_client-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     1069 2023-04-24 00:12:01.040127 oidc_client-0.2.3/README.md
--rw-r--r--   0        0        0      541 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/__main__.py
--rw-r--r--   0        0        0     5028 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/cli.py
--rw-r--r--   0        0        0     3717 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/config.py
--rw-r--r--   0        0        0      925 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/error.py
--rw-r--r--   0        0        0      215 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/index.html
--rw-r--r--   0        0        0     1748 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2023-04-24 00:12:01.040127 oidc_client-0.2.3/oidc_client/localhost.key
--rw-r--r--   0        0        0     8471 2023-04-24 00:12:01.041127 oidc_client-0.2.3/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2023-04-24 00:12:01.041127 oidc_client-0.2.3/oidc_client/pkce.py
--rw-r--r--   0        0        0      556 2023-04-24 00:12:01.041127 oidc_client-0.2.3/oidc_client/tls.py
--rw-r--r--   0        0        0     1328 2023-04-24 00:12:01.041127 oidc_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-26 13:38:00.178439 oidc_client-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-04-26 13:38:00.178439 oidc_client-0.2.4/README.md
+-rw-r--r--   0        0        0      541 2023-04-26 13:38:00.178439 oidc_client-0.2.4/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-26 13:38:00.178439 oidc_client-0.2.4/oidc_client/__main__.py
+-rw-r--r--   0        0        0     5028 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/cli.py
+-rw-r--r--   0        0        0     3717 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/config.py
+-rw-r--r--   0        0        0      925 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/error.py
+-rw-r--r--   0        0        0      264 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/index.html
+-rw-r--r--   0        0        0     1748 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/localhost.key
+-rw-r--r--   0        0        0     8651 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/pkce.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/py.typed
+-rw-r--r--   0        0        0      556 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/tls.py
+-rw-r--r--   0        0        0     1328 2023-04-26 13:38:00.179439 oidc_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.4/PKG-INFO
```

### Comparing `oidc_client-0.2.3/LICENSE.md` & `oidc_client-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/README.md` & `oidc_client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/__init__.py` & `oidc_client-0.2.4/oidc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/cli.py` & `oidc_client-0.2.4/oidc_client/cli.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/config.py` & `oidc_client-0.2.4/oidc_client/config.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/discovery.py` & `oidc_client-0.2.4/oidc_client/discovery.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/lib.py` & `oidc_client-0.2.4/oidc_client/lib.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/localhost.crt` & `oidc_client-0.2.4/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/localhost.key` & `oidc_client-0.2.4/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/oauth.py` & `oidc_client-0.2.4/oidc_client/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 import json
 import random
 import string
 import webbrowser
 from dataclasses import dataclass, fields
 from http import HTTPStatus
 from http.server import BaseHTTPRequestHandler, HTTPServer
+from importlib import metadata
 from importlib.resources import files
 from socket import socket
+from string import Template
 from typing import cast
 from urllib.error import HTTPError
 from urllib.parse import parse_qs, urlencode, urlparse
 from urllib.request import Request, urlopen
 
 from .error import AuthorizationError, RedirectionError
 from .pkce import PKCESecret
@@ -81,15 +83,19 @@
             return
 
         self.send_response(HTTPStatus.OK)
         self.send_header("Connection", "close")
         self.send_header("Content-type", "text/html;utf-8")
         self.end_headers()
 
-        self.wfile.write(files(__package__).joinpath("index.html").read_bytes())
+        self.wfile.write(
+            Template(files(__package__).joinpath("index.html").read_text())
+            .safe_substitute(version=metadata.version(__package__))
+            .encode()
+        )
 
 
 class RedirectionServer(HTTPServer):
     """OAuth 2.1 authorization code flow (with PKCE) HTTP server."""
 
     def __init__(
         self,
```

### Comparing `oidc_client-0.2.3/oidc_client/pkce.py` & `oidc_client-0.2.4/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/oidc_client/tls.py` & `oidc_client-0.2.4/oidc_client/tls.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.3/pyproject.toml` & `oidc_client-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.2.3"
+version = "0.2.4"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
```

### Comparing `oidc_client-0.2.3/PKG-INFO` & `oidc_client-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

