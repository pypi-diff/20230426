# Comparing `tmp/Flask-DigestAuth-0.5.0.tar.gz` & `tmp/Flask-DigestAuth-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-DigestAuth-0.5.0.tar", last modified: Thu Jan  5 16:22:12 2023, max compression
+gzip compressed data, was "Flask-DigestAuth-0.6.0.tar", last modified: Wed Apr 26 15:41:19 2023, max compression
```

## Comparing `Flask-DigestAuth-0.5.0.tar` & `Flask-DigestAuth-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.5.0/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)      808 2022-12-06 14:02:16.000000 Flask-DigestAuth-0.5.0/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)    12007 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11281 2023-01-05 16:16:58.000000 Flask-DigestAuth-0.5.0/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.357505 Flask-DigestAuth-0.5.0/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2022-12-07 01:40:48.000000 Flask-DigestAuth-0.5.0/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2022-12-07 01:40:48.000000 Flask-DigestAuth-0.5.0/docs/make.bat
--rw-r--r--   0 imacat    (1000) users      (100)        6 2022-12-06 14:18:07.000000 Flask-DigestAuth-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.357505 Flask-DigestAuth-0.5.0/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.357505 Flask-DigestAuth-0.5.0/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2022-12-07 01:41:12.000000 Flask-DigestAuth-0.5.0/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.357505 Flask-DigestAuth-0.5.0/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2022-12-07 01:41:16.000000 Flask-DigestAuth-0.5.0/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1028 2023-01-05 16:20:40.000000 Flask-DigestAuth-0.5.0/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-01-05 16:16:58.000000 Flask-DigestAuth-0.5.0/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)      678 2022-12-07 10:03:38.000000 Flask-DigestAuth-0.5.0/docs/source/flask_digest_auth.rst
--rw-r--r--   0 imacat    (1000) users      (100)      902 2023-01-04 13:07:18.000000 Flask-DigestAuth-0.5.0/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-01-05 16:01:07.000000 Flask-DigestAuth-0.5.0/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       60 2022-12-07 07:56:42.000000 Flask-DigestAuth-0.5.0/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)      777 2022-11-23 20:56:29.000000 Flask-DigestAuth-0.5.0/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)      914 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.357505 Flask-DigestAuth-0.5.0/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)    12007 2023-01-05 16:22:12.000000 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)      714 2023-01-05 16:22:12.000000 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-01-05 16:22:12.000000 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       33 2023-01-05 16:22:12.000000 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       18 2023-01-05 16:22:12.000000 Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/src/flask_digest_auth/
--rw-r--r--   0 imacat    (1000) users      (100)      888 2022-12-06 13:20:21.000000 Flask-DigestAuth-0.5.0/src/flask_digest_auth/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     4099 2022-12-06 15:52:42.000000 Flask-DigestAuth-0.5.0/src/flask_digest_auth/algo.py
--rw-r--r--   0 imacat    (1000) users      (100)    17813 2023-01-05 15:49:57.000000 Flask-DigestAuth-0.5.0/src/flask_digest_auth/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     5521 2022-12-07 10:58:02.000000 Flask-DigestAuth-0.5.0/src/flask_digest_auth/test.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-01-05 16:22:12.361505 Flask-DigestAuth-0.5.0/tests/
--rw-r--r--   0 imacat    (1000) users      (100)     1952 2022-11-22 22:47:31.000000 Flask-DigestAuth-0.5.0/tests/test_algo.py
--rw-r--r--   0 imacat    (1000) users      (100)     7817 2023-01-05 16:01:07.000000 Flask-DigestAuth-0.5.0/tests/test_auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    10496 2023-01-05 16:01:07.000000 Flask-DigestAuth-0.5.0/tests/test_flask_login.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.199127 Flask-DigestAuth-0.6.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.6.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2787 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     2154 2023-04-26 15:40:40.000000 Flask-DigestAuth-0.6.0/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1071 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      678 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/flask_digest_auth.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      915 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       60 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1845 2023-04-26 15:30:27.000000 Flask-DigestAuth-0.6.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-26 15:41:19.199127 Flask-DigestAuth-0.6.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.191127 Flask-DigestAuth-0.6.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)      708 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       37 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       18 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/src/flask_digest_auth/
+-rw-r--r--   0 imacat    (1000) users      (100)      939 2023-04-26 15:35:16.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4103 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17722 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5538 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/test.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/tests/
+-rw-r--r--   0 imacat    (1000) users      (100)     1956 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7829 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10505 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_flask_login.py
```

### Comparing `Flask-DigestAuth-0.5.0/LICENSE` & `Flask-DigestAuth-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/MANIFEST.in` & `Flask-DigestAuth-0.6.0/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,11 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-include docs/*
-include docs/source/*
-include docs/source/_static/*
-include docs/source/_templates/*
-include tests/*
+recursive-include docs *
+recursive-exclude docs/build *
+recursive-include tests *
+recursive-exclude tests *.pyc
```

### Comparing `Flask-DigestAuth-0.5.0/docs/Makefile` & `Flask-DigestAuth-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/docs/make.bat` & `Flask-DigestAuth-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/docs/source/conf.py` & `Flask-DigestAuth-0.6.0/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('../../src/'))
+import flask_digest_auth
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Flask-DigestAuth'
 copyright = '2022-2023, imacat'
 author = 'imacat'
-release = '0.5.0'
+release = flask_digest_auth.VERSION
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ['_templates']
```

### Comparing `Flask-DigestAuth-0.5.0/docs/source/examples.rst` & `Flask-DigestAuth-0.6.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/docs/source/flask_digest_auth.rst` & `Flask-DigestAuth-0.6.0/docs/source/flask_digest_auth.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/docs/source/index.rst` & `Flask-DigestAuth-0.6.0/docs/source/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    intro
    flask_digest_auth
    examples
+   changelog
 
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `Flask-DigestAuth-0.5.0/docs/source/intro.rst` & `Flask-DigestAuth-0.6.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.5.0/src/Flask_DigestAuth.egg-info/SOURCES.txt` & `Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 docs/Makefile
 docs/make.bat
-docs/requirements.txt
+docs/source/changelog.rst
 docs/source/conf.py
 docs/source/examples.rst
 docs/source/flask_digest_auth.rst
 docs/source/index.rst
 docs/source/intro.rst
 docs/source/modules.rst
 docs/source/_static/.keep
```

### Comparing `Flask-DigestAuth-0.5.0/src/flask_digest_auth/__init__.py` & `Flask-DigestAuth-0.6.0/src/flask_digest_auth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 
 """The HTTP digest authentication.
 
 """
 from flask_digest_auth.algo import make_password_hash, calc_response
 from flask_digest_auth.auth import DigestAuth
 from flask_digest_auth.test import Client
+
+VERSION: str = "0.6.0"
+"""The package version."""
```

### Comparing `Flask-DigestAuth-0.5.0/src/flask_digest_auth/algo.py` & `Flask-DigestAuth-0.6.0/src/flask_digest_auth/algo.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 #  limitations under the License.
 
 """The algorithm.
 
 """
 from __future__ import annotations
 
-import typing as t
 from hashlib import md5
+from typing import Optional, Literal
 
 
 def make_password_hash(realm: str, username: str, password: str) -> str:
     """Calculates the password hash for the HTTP digest authentication.
     Use this function to set the password for the user.
 
     :Example:
@@ -40,18 +40,18 @@
     :return: The password hash for the HTTP digest authentication.
     """
     return md5(f"{username}:{realm}:{password}".encode("utf8")).hexdigest()
 
 
 def calc_response(
         method: str, uri: str, password_hash: str,
-        nonce: str, qop: t.Optional[t.Literal["auth", "auth-int"]] = None,
-        algorithm: t.Optional[t.Literal["MD5", "MD5-sess"]] = "MD5-sess",
-        cnonce: t.Optional[str] = None, nc: t.Optional[str] = None,
-        body: t.Optional[bytes] = None) -> str:
+        nonce: str, qop: Optional[Literal["auth", "auth-int"]] = None,
+        algorithm: Optional[Literal["MD5", "MD5-sess"]] = "MD5-sess",
+        cnonce: Optional[str] = None, nc: Optional[str] = None,
+        body: Optional[bytes] = None) -> str:
     """Calculates the response value of the HTTP digest authentication.
 
     :param method: The request method.
     :param uri: The request URI.
     :param password_hash: The password hash for the HTTP digest authentication.
     :param nonce: The nonce.
     :param qop: The quality of protection, either ``auth`` or ``auth-int``.
```

### Comparing `Flask-DigestAuth-0.5.0/src/flask_digest_auth/auth.py` & `Flask-DigestAuth-0.6.0/src/flask_digest_auth/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,60 +19,59 @@
 See `RFC 2617`_ HTTP Authentication: Basic and Digest Access Authentication
 
 .. _RFC 2617: https://www.rfc-editor.org/rfc/rfc2617
 """
 from __future__ import annotations
 
 import sys
-import typing as t
 from functools import wraps
 from secrets import token_urlsafe, randbits
+from typing import Any, Optional, Literal, Callable, List
 
 from flask import g, request, Response, session, abort, Flask, Request, \
     current_app
 from itsdangerous import URLSafeTimedSerializer, BadData
 from werkzeug.datastructures import Authorization
 
 from flask_digest_auth.algo import calc_response
 
 
 class DigestAuth:
     """The HTTP digest authentication."""
 
-    def __init__(self, realm: t.Optional[str] = None):
+    def __init__(self, realm: Optional[str] = None):
         """Constructs the HTTP digest authentication.
 
         :param realm: The realm.
         """
         self.__serializer: URLSafeTimedSerializer \
             = URLSafeTimedSerializer(token_urlsafe(32))
         """The serializer to generate and validate the nonce and opaque."""
         self.realm: str = "Login Required" if realm is None else realm
         """The realm.  Default is "Login Required"."""
-        self.algorithm: t.Optional[t.Literal["MD5", "MD5-sess"]] = None
+        self.algorithm: Optional[Literal["MD5", "MD5-sess"]] = None
         """The algorithm, either None, ``MD5``, or ``MD5-sess``.  Default is
         None."""
         self.use_opaque: bool = True
         """Whether to use an opaque.  Default is True."""
-        self.__domain: t.List[str] = []
+        self.__domain: List[str] = []
         """A list of directories that this username and password applies to.
         Default is empty."""
-        self.__qop: t.List[t.Literal["auth", "auth-int"]] \
-            = ["auth", "auth-int"]
+        self.__qop: List[Literal["auth", "auth-int"]] = ["auth", "auth-int"]
         """A list of supported quality of protection supported, either
         ``qop``, ``auth-int``, both, or empty.  Default is both."""
         self.__get_password_hash: BasePasswordHashGetter \
             = BasePasswordHashGetter()
         """The callback to return the password hash."""
         self.__get_user: BaseUserGetter = BaseUserGetter()
         """The callback to return the user."""
         self.__on_login: BaseOnLogInCallback = BaseOnLogInCallback()
         """The callback to run when the user logs in."""
 
-    def login_required(self, view) -> t.Callable:
+    def login_required(self, view) -> Callable:
         """The view decorator for the HTTP digest authentication.
 
         :Example:
 
         ::
 
             @app.get("/admin")
@@ -85,29 +84,29 @@
         :param view: The view.
         :return: The login-protected view.
         """
 
         class NoLogInException(Exception):
             """The exception thrown when the user is not authorized."""
 
-        def get_logged_in_user() -> t.Any:
+        def get_logged_in_user() -> Any:
             """Returns the currently logged-in user.
 
             :return: The currently logged-in user.
             :raise NoLogInException: When the user is not logged in.
             """
             if "user" not in session:
                 raise NoLogInException
-            user: t.Optional[t.Any] = self.__get_user(session["user"])
+            user: Optional[Any] = self.__get_user(session["user"])
             if user is None:
                 del session["user"]
                 raise NoLogInException
             return user
 
-        def auth_user(state: AuthState) -> t.Any:
+        def auth_user(state: AuthState) -> Any:
             """Authenticates a user.
 
             :param state: The authentication state.
             :return: The user.
             :raise UnauthorizedException: When the authentication fails.
             """
             authorization: Authorization = request.authorization
@@ -117,15 +116,15 @@
                 raise UnauthorizedException(
                     "Not an HTTP digest authorization")
             self.__authenticate(state)
             session["user"] = authorization.username
             return self.__get_user(authorization.username)
 
         @wraps(view)
-        def login_required_view(*args, **kwargs) -> t.Any:
+        def login_required_view(*args, **kwargs) -> Any:
             """The login-protected view.
 
             :param args: The positional arguments of the view.
             :param kwargs: The keyword arguments of the view.
             :return: The response.
             """
             try:
@@ -167,15 +166,15 @@
                     "Missing \"opaque\" in the Authorization header")
             try:
                 self.__serializer.loads(
                     authorization.opaque, salt="opaque", max_age=1800)
             except BadData:
                 raise UnauthorizedException("Invalid opaque")
             state.opaque = authorization.opaque
-        password_hash: t.Optional[str] \
+        password_hash: Optional[str] \
             = self.__get_password_hash(authorization.username)
         if password_hash is None:
             raise UnauthorizedException(
                 f"No such user \"{authorization.username}\"")
         expected: str = calc_response(
             method=request.method, uri=authorization.uri,
             password_hash=password_hash, nonce=authorization.nonce,
@@ -198,26 +197,26 @@
     def __make_response_header(self, state: AuthState) -> str:
         """Composes and returns the ``WWW-Authenticate`` response header.
 
         :param state: The authorization state.
         :return: The ``WWW-Authenticate`` response header.
         """
 
-        def get_opaque() -> t.Optional[str]:
+        def get_opaque() -> Optional[str]:
             """Returns the opaque value.
 
             :return: The opaque value.
             """
             if not self.use_opaque:
                 return None
             if state.opaque is not None:
                 return state.opaque
             return self.__serializer.dumps(randbits(32), salt="opaque")
 
-        opaque: t.Optional[str] = get_opaque()
+        opaque: Optional[str] = get_opaque()
         nonce: str = self.__serializer.dumps(
             randbits(32),
             salt="nonce" if opaque is None else f"nonce-{opaque}")
 
         header: str = f"Digest realm=\"{self.realm}\""
         if len(self.__domain) > 0:
             domain_list: str = ",".join(self.__domain)
@@ -230,15 +229,15 @@
         if self.algorithm is not None:
             header += f", algorithm=\"{self.algorithm}\""
         if len(self.__qop) > 0:
             qop_list: str = ",".join(self.__qop)
             header += f", qop=\"{qop_list}\""
         return header
 
-    def register_get_password(self, func: t.Callable[[str], t.Optional[str]])\
+    def register_get_password(self, func: Callable[[str], Optional[str]]) \
             -> None:
         """The decorator to register the callback to obtain the password hash.
 
         :Example:
 
         ::
 
@@ -252,26 +251,25 @@
         :return: None.
         """
 
         class PasswordHashGetter(BasePasswordHashGetter):
             """The base password hash getter."""
 
             @staticmethod
-            def __call__(username: str) -> t.Optional[str]:
+            def __call__(username: str) -> Optional[str]:
                 """Returns the password hash of a user.
 
                 :param username: The username.
                 :return: The password hash, or None if the user does not exist.
                 """
                 return func(username)
 
         self.__get_password_hash = PasswordHashGetter()
 
-    def register_get_user(self, func: t.Callable[[str], t.Optional[t.Any]])\
-            -> None:
+    def register_get_user(self, func: Callable[[str], Optional[Any]]) -> None:
         """The decorator to register the callback to obtain the user.
 
         :Example:
 
         ::
 
             @auth.register_get_user
@@ -283,25 +281,25 @@
         :return: None.
         """
 
         class UserGetter(BaseUserGetter):
             """The user getter."""
 
             @staticmethod
-            def __call__(username: str) -> t.Optional[t.Any]:
+            def __call__(username: str) -> Optional[Any]:
                 """Returns a user.
 
                 :param username: The username.
                 :return: The user, or None if the user does not exist.
                 """
                 return func(username)
 
         self.__get_user = UserGetter()
 
-    def register_on_login(self, func: t.Callable[[t.Any], None]) -> None:
+    def register_on_login(self, func: Callable[[Any], None]) -> None:
         """The decorator to register the callback to run when the user logs in.
 
         :Example:
 
         ::
 
             @auth.register_on_login
@@ -312,15 +310,15 @@
         :return: None.
         """
 
         class OnLogInCallback:
             """The callback when the user logs in."""
 
             @staticmethod
-            def __call__(user: t.Any) -> None:
+            def __call__(user: Any) -> None:
                 """Runs the callback when the user logs in.
 
                 :param user: The logged-in user.
                 :return: None.
                 """
                 func(user)
 
@@ -332,15 +330,14 @@
 
         :Example:
 
         ::
 
             app: flask = Flask(__name__)
             auth: DigestAuth = DigestAuth()
-            auth.realm = "My Admin"
             auth.init_app(app)
 
         :param app: The Flask application.
         :return: None.
         """
         app.extensions["digest_auth"] = self
         if "DIGEST_AUTH_REALM" in app.config:
@@ -363,15 +360,15 @@
                 response: Response = Response()
                 response.status = 401
                 response.headers["WWW-Authenticate"] \
                     = self.__make_response_header(state)
                 abort(response)
 
             @login_manager.request_loader
-            def load_user_from_request(req: Request) -> t.Optional[t.Any]:
+            def load_user_from_request(req: Request) -> Optional[Any]:
                 """Loads the user from the request header.
 
                 :param req: The request.
                 :return: The authenticated user, or None if the
                     authentication fails
                 """
                 request._digest_auth_state = AuthState()
@@ -424,17 +421,17 @@
     """The authentication state.  It keeps the status in the earlier
     authentication stage, so that the latter response stage knows how to
     response.
     """
 
     def __init__(self):
         """Constructs the authorization state."""
-        self.opaque: t.Optional[str] = None
+        self.opaque: Optional[str] = None
         """The opaque value specified by the client, if valid."""
-        self.stale: t.Optional[bool] = None
+        self.stale: Optional[bool] = None
         """The stale value, if there is a previous log in attempt."""
 
 
 class UnauthorizedException(Exception):
     """The exception thrown when the authentication fails."""
 
 
@@ -443,15 +440,15 @@
     or None if the user does not exist.  The default is to raise an
     :class:`UnboundLocalError` if the callback is not registered yet.
 
     See :meth:`flask_digest_auth.auth.DigestAuth.register_get_password`
     """
 
     @staticmethod
-    def __call__(username: str) -> t.Optional[str]:
+    def __call__(username: str) -> Optional[str]:
         """Returns the password hash of a user.
 
         :param username: The username.
         :return: The password hash, or None if the user does not exist.
         :raise UnboundLocalError: When the password hash getter function is
             not registered yet.
         """
@@ -464,15 +461,15 @@
     the user does not exist.  The default is to raise an
     :class:`UnboundLocalError` if the callback is not registered yet.
 
     See :meth:`flask_digest_auth.auth.DigestAuth.register_get_user`
     """
 
     @staticmethod
-    def __call__(username: str) -> t.Optional[t.Any]:
+    def __call__(username: str) -> Optional[Any]:
         """Returns a user.
 
         :param username: The username.
         :return: The user, or None if the user does not exist.
         :raise UnboundLocalError: When the user getter function is not
             registered yet.
         """
@@ -484,13 +481,13 @@
     """The base callback to run when the user logs in, given the logged-in
     user.  The default does nothing.
 
     See :meth:`flask_digest_auth.auth.DigestAuth.register_on_login`
     """
 
     @staticmethod
-    def __call__(user: t.Any) -> None:
+    def __call__(user: Any) -> None:
         """Runs the callback when the user logs in.
 
         :param user: The logged-in user.
         :return: None.
         """
```

### Comparing `Flask-DigestAuth-0.5.0/src/flask_digest_auth/test.py` & `Flask-DigestAuth-0.6.0/src/flask_digest_auth/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test client with HTTP digest authentication enabled.
 
 """
-import typing as t
 from secrets import token_urlsafe
+from typing import Optional, Literal, Tuple, Dict
 
 from flask import g
 from werkzeug.datastructures import Authorization, WWWAuthenticate
 from werkzeug.test import TestResponse, Client as WerkzeugClient
 
 from flask_digest_auth.algo import calc_response, make_password_hash
 
@@ -79,15 +79,15 @@
                     "/admin", digest_auth=(USERNAME, PASSWORD))
                 assert response.status_code == 200
 
     .. _unittest: https://docs.python.org/3/library/unittest.html
     .. _pytest: https://pytest.org
     """
 
-    def open(self, *args, digest_auth: t.Optional[t.Tuple[str, str]] = None,
+    def open(self, *args, digest_auth: Optional[Tuple[str, str]] = None,
              **kwargs) -> TestResponse:
         """Opens a request.
 
         :param args: The arguments.
         :param digest_auth: The (*username*, *password*) tuple for the HTTP
             digest authentication.
         :param kwargs: The keyword arguments.
@@ -113,35 +113,35 @@
 
         :param www_authenticate: The ``WWW-Authenticate`` response.
         :param uri: The request URI.
         :param username: The username.
         :param password: The password.
         :return: The request authorization.
         """
-        qop: t.Optional[t.Literal["auth", "auth-int"]] = None
+        qop: Optional[Literal["auth", "auth-int"]] = None
         if www_authenticate.qop is not None and "auth" in www_authenticate.qop:
             qop = "auth"
 
-        cnonce: t.Optional[str] = None
+        cnonce: Optional[str] = None
         if qop is not None or www_authenticate.algorithm == "MD5-sess":
             cnonce = token_urlsafe(8)
-        nc: t.Optional[str] = None
+        nc: Optional[str] = None
         count: int = 1
         if qop is not None:
             nc: str = hex(count)[2:].zfill(8)
 
         expected: str = calc_response(
             method="GET", uri=uri,
             password_hash=make_password_hash(www_authenticate.realm,
                                              username, password),
             nonce=www_authenticate.nonce, qop=qop,
             algorithm=www_authenticate.algorithm, cnonce=cnonce, nc=nc,
             body=None)
 
-        data: t.Dict[str, str] = {
+        data: Dict[str, str] = {
             "username": username, "realm": www_authenticate.realm,
             "nonce": www_authenticate.nonce, "uri": uri, "response": expected}
         if www_authenticate.algorithm is not None:
             data["algorithm"] = www_authenticate.algorithm
         if cnonce is not None:
             data["cnonce"] = cnonce
         if www_authenticate.opaque is not None:
```

### Comparing `Flask-DigestAuth-0.5.0/tests/test_algo.py` & `Flask-DigestAuth-0.6.0/tests/test_algo.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test case for the HTTP digest authentication algorithm.
 
 """
-import typing as t
 import unittest
+from typing import Optional, Literal
 
 from flask_digest_auth import make_password_hash, calc_response
 
 
 class AlgorithmTestCase(unittest.TestCase):
     """The test case for the HTTP digest authentication algorithm."""
 
@@ -35,17 +35,17 @@
         """
         realm: str = "testrealm@host.com"
         username: str = "Mufasa"
         password: str = "Circle Of Life"
         method: str = "GET"
         uri: str = "/dir/index.html"
         nonce: str = "dcd98b7102dd2f0e8b11d0f600bfb0c093"
-        qop: t.Optional[t.Literal["auth", "auth-int"]] = "auth"
-        algorithm: t.Optional[t.Literal["MD5", "MD5-sess"]] = None
-        cnonce: t.Optional[str] = "0a4f113b"
-        nc: t.Optional[str] = "00000001"
-        body: t.Optional[bytes] = None
+        qop: Optional[Literal["auth", "auth-int"]] = "auth"
+        algorithm: Optional[Literal["MD5", "MD5-sess"]] = None
+        cnonce: Optional[str] = "0a4f113b"
+        nc: Optional[str] = "00000001"
+        body: Optional[bytes] = None
 
         password_hash: str = make_password_hash(realm, username, password)
         response: str = calc_response(method, uri, password_hash, nonce, qop,
                                       algorithm, cnonce, nc, body)
         self.assertEqual(response, "6629fae49393a05397450978507c4ef1")
```

### Comparing `Flask-DigestAuth-0.5.0/tests/test_auth.py` & `Flask-DigestAuth-0.6.0/tests/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test case for the HTTP digest authentication.
 
 """
-import typing as t
 from secrets import token_urlsafe
+from typing import Any, Optional, Dict
 
 from flask import Response, Flask, g, redirect, request
 from flask_testing import TestCase
 from werkzeug.datastructures import WWWAuthenticate, Authorization
 
 from flask_digest_auth import DigestAuth, make_password_hash, Client
 
@@ -62,28 +62,28 @@
             "DIGEST_AUTH_REALM": _REALM,
         })
         app.test_client_class = Client
 
         auth: DigestAuth = DigestAuth()
         auth.init_app(app)
         self.user: User = User(_USERNAME, _PASSWORD)
-        user_db: t.Dict[str, User] = {_USERNAME: self.user}
+        user_db: Dict[str, User] = {_USERNAME: self.user}
 
         @auth.register_get_password
-        def get_password_hash(username: str) -> t.Optional[str]:
+        def get_password_hash(username: str) -> Optional[str]:
             """Returns the password hash of a user.
 
             :param username: The username.
             :return: The password hash, or None if the user does not exist.
             """
             return user_db[username].password_hash if username in user_db \
                 else None
 
         @auth.register_get_user
-        def get_user(username: str) -> t.Optional[t.Any]:
+        def get_user(username: str) -> Optional[Any]:
             """Returns a user.
 
             :param username: The username.
             :return: The user, or None if the user does not exist.
             """
             return user_db[username] if username in user_db else None
```

### Comparing `Flask-DigestAuth-0.5.0/tests/test_flask_login.py` & `Flask-DigestAuth-0.6.0/tests/test_flask_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test case for the Flask-Login integration.
 
 """
-import typing as t
 from secrets import token_urlsafe
+from typing import Optional, Dict
 
 from flask import Response, Flask, g, redirect, request
 from flask_testing import TestCase
 from werkzeug.datastructures import WWWAuthenticate, Authorization
 
 from flask_digest_auth import DigestAuth, make_password_hash, Client
 
@@ -93,18 +93,18 @@
         login_manager: flask_login.LoginManager = flask_login.LoginManager()
         login_manager.init_app(app)
 
         auth: DigestAuth = DigestAuth()
         auth.init_app(app)
 
         self.user: User = User(_USERNAME, _PASSWORD)
-        user_db: t.Dict[str, User] = {_USERNAME: self.user}
+        user_db: Dict[str, User] = {_USERNAME: self.user}
 
         @auth.register_get_password
-        def get_password_hash(username: str) -> t.Optional[str]:
+        def get_password_hash(username: str) -> Optional[str]:
             """Returns the password hash of a user.
 
             :param username: The username.
             :return: The password hash, or None if the user does not exist.
             """
             return user_db[username].password_hash if username in user_db \
                 else None
@@ -115,15 +115,15 @@
 
             :param user: The logged-in user.
             :return: None.
             """
             user.visits = user.visits + 1
 
         @login_manager.user_loader
-        def load_user(user_id: str) -> t.Optional[User]:
+        def load_user(user_id: str) -> Optional[User]:
             """Loads a user.
 
             :param user_id: The username.
             :return: The user, or None if the user does not exist.
             """
             return user_db[user_id] if user_id in user_db else None
```

