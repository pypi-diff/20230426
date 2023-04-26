# Comparing `tmp/oidc_client-0.2.4.tar.gz` & `tmp/oidc_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_client-0.2.4.tar", max compression
+gzip compressed data, was "oidc_client-0.2.5.tar", max compression
```

## Comparing `oidc_client-0.2.4.tar` & `oidc_client-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1085 2023-04-26 13:38:00.178439 oidc_client-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     1069 2023-04-26 13:38:00.178439 oidc_client-0.2.4/README.md
--rw-r--r--   0        0        0      541 2023-04-26 13:38:00.178439 oidc_client-0.2.4/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-26 13:38:00.178439 oidc_client-0.2.4/oidc_client/__main__.py
--rw-r--r--   0        0        0     5028 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/cli.py
--rw-r--r--   0        0        0     3717 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/config.py
--rw-r--r--   0        0        0      925 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/error.py
--rw-r--r--   0        0        0      264 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/index.html
--rw-r--r--   0        0        0     1748 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/localhost.key
--rw-r--r--   0        0        0     8651 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/pkce.py
--rw-r--r--   0        0        0        0 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/py.typed
--rw-r--r--   0        0        0      556 2023-04-26 13:38:00.179439 oidc_client-0.2.4/oidc_client/tls.py
--rw-r--r--   0        0        0     1328 2023-04-26 13:38:00.179439 oidc_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-26 15:38:59.194940 oidc_client-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-04-26 15:38:59.194940 oidc_client-0.2.5/README.md
+-rw-r--r--   0        0        0      541 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/__main__.py
+-rw-r--r--   0        0        0     5028 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/cli.py
+-rw-r--r--   0        0        0     3717 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/config.py
+-rw-r--r--   0        0        0      925 2023-04-26 15:38:59.194940 oidc_client-0.2.5/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/error.py
+-rw-r--r--   0        0        0      264 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/index.html
+-rw-r--r--   0        0        0     1748 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/localhost.key
+-rw-r--r--   0        0        0     8651 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/pkce.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/py.typed
+-rw-r--r--   0        0        0      556 2023-04-26 15:38:59.195940 oidc_client-0.2.5/oidc_client/tls.py
+-rw-r--r--   0        0        0     1325 2023-04-26 15:38:59.195940 oidc_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 oidc_client-0.2.5/PKG-INFO
```

### Comparing `oidc_client-0.2.4/LICENSE.md` & `oidc_client-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/README.md` & `oidc_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/__init__.py` & `oidc_client-0.2.5/oidc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/cli.py` & `oidc_client-0.2.5/oidc_client/cli.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/config.py` & `oidc_client-0.2.5/oidc_client/config.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/discovery.py` & `oidc_client-0.2.5/oidc_client/discovery.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/lib.py` & `oidc_client-0.2.5/oidc_client/lib.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/localhost.crt` & `oidc_client-0.2.5/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/localhost.key` & `oidc_client-0.2.5/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/oauth.py` & `oidc_client-0.2.5/oidc_client/oauth.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/pkce.py` & `oidc_client-0.2.5/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/oidc_client/tls.py` & `oidc_client-0.2.5/oidc_client/tls.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.2.4/pyproject.toml` & `oidc_client-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.2.4"
+version = "0.2.5"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
@@ -15,16 +15,16 @@
 authors = ["Loris Zinsou <lzinsou@proton.me>"]
 
 [tool.poetry.scripts]
 oidc = "oidc_client.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-toml = { version = "^0.10.2", allow-prereleases = true, python = "<3.11" }
-StrEnum = { version = "^0.4.10", allow-prereleases = true, python = "<3.11" }
+toml = { version = ">=0.10", allow-prereleases = true, python = "<3.11" }
+StrEnum = { version = ">=0.4", allow-prereleases = true, python = "<3.11" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 mypy = "^1.2.0"
 isort = "^5.12.0"
 black = "^23.3.0"
```

### Comparing `oidc_client-0.2.4/PKG-INFO` & `oidc_client-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: StrEnum (>=0.4.10,<0.5.0) ; python_version < "3.11"
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; python_version < "3.11"
+Requires-Dist: StrEnum (>=0.4) ; python_version < "3.11"
+Requires-Dist: toml (>=0.10) ; python_version < "3.11"
 Project-URL: Repository, https://gitlab.com/lzinsou/oidc-client
 Description-Content-Type: text/markdown
 
 OIDC Client
 ===========
 
 A pure-Python OpenID Connect client supporting OAuth 2.1 authorization flows, built for Python 3.10+ with minimal dependencies.
```

