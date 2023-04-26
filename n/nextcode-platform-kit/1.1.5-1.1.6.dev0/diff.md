# Comparing `tmp/nextcode-platform-kit-1.1.5.tar.gz` & `tmp/nextcode-platform-kit-1.1.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nextcode-platform-kit-1.1.5.tar", last modified: Fri Mar 18 15:11:52 2022, max compression
+gzip compressed data, was "nextcode-platform-kit-1.1.6.dev0.tar", last modified: Wed Apr 26 15:35:48 2023, max compression
```

## Comparing `nextcode-platform-kit-1.1.5.tar` & `nextcode-platform-kit-1.1.6.dev0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/
--rw-r--r--   0 root         (0) root         (0)      951 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/platkit/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/platkit/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      416 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6141 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/platkit/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/endpoints/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     8561 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/flasksetup.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/librarypatches.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/testcase.py
--rw-rw-rw-   0 root         (0) root         (0)     5879 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/logsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/platkit/middleware/
--rw-rw-rw-   0 root         (0) root         (0)     3713 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/middleware/logstash_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/middleware/reverse_proxied.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/platkit/models/
--rw-rw-rw-   0 root         (0) root         (0)     1041 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/models/responses.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/csautils.py
--rw-rw-rw-   0 root         (0) root         (0)    13691 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/platkit/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3958 2022-03-18 15:11:26.000000 nextcode-platform-kit-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      951 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      197 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-18 15:11:51.000000 nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-18 15:11:52.000000 nextcode-platform-kit-1.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.560858 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:35:47.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.564858 nextcode-platform-kit-1.1.6.dev0/platkit/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-26 15:35:48.000000 nextcode-platform-kit-1.1.6.dev0/platkit/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/csautils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.565858 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8561 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/flasksetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/librarypatches.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/logsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.566858 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/logstash_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/middleware/reverse_proxied.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:35:48.567858 nextcode-platform-kit-1.1.6.dev0/platkit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/models/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/testcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/platkit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:35:48.568858 nextcode-platform-kit-1.1.6.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-26 15:35:17.000000 nextcode-platform-kit-1.1.6.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nextcode-platform-kit-1.1.5/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.5
+Version: 1.1.6.dev0
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-
-UNKNOWN
-
```

### Comparing `nextcode-platform-kit-1.1.5/platkit/cli.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/cli.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/endpoints/auth.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/flasksetup.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/flasksetup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 """
 
 from http import HTTPStatus
 import logging
 import time
 
 from flask import request, current_app, make_response, jsonify, Blueprint
-from flask_restx import abort, Model
+from flask_restx import abort, Model, Api
 from flask_httpauth import HTTPTokenAuth
 from werkzeug.utils import find_modules, import_string
 from werkzeug.exceptions import HTTPException
 from werkzeug.middleware.proxy_fix import ProxyFix
 from flask import Flask
 
 import sentry_sdk
 from sentry_sdk.integrations.flask import FlaskIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 from sentry_sdk.integrations.sqlalchemy import SqlalchemyIntegration
-from platkit.librarypatches import PatchedApi as Api
 from platkit.exceptions import InvalidUsage
-from platkit.utils import CustomJSONEncoder
+from platkit.utils import CustomJSONProvider
 from platkit import logsetup
 from platkit.config import Config
 from platkit.middleware.reverse_proxied import ReverseProxied
 from platkit.prometheus import metrics
 from platkit.cli import setup_commands
 
 log = logging.getLogger("platkit")
@@ -135,15 +134,16 @@
 
 def setup_base_app(app, build_info=None):
     print('setup_base_app')
     auth = HTTPTokenAuth("Bearer")
     app.auth = auth
 
     # Datetime fix
-    app.json_encoder = CustomJSONEncoder
+    app.json_provider_class = CustomJSONProvider
+    app.json = CustomJSONProvider(app)
 
     @app.errorhandler(500)
     @app.errorhandler(503)
     @app.errorhandler(409)
     @app.errorhandler(405)
     @app.errorhandler(404)
     @app.errorhandler(403)
```

### Comparing `nextcode-platform-kit-1.1.5/platkit/librarypatches.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/librarypatches.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,14 @@
 import re
 import os
 from flask import make_response
 from flask.json import dumps
 import flask_restx
 
 
-# monkeypatch the Api class to remove hard-coded '/' rules so that we can put something that
-# is not swagger into the root. Hopefully this will be solved in flask_restx at some point
-# https://github.com/noirbizarre/flask-restx/issues/247
-class PatchedApi(flask_restx.Api):
-    def _register_doc(self, app_or_blueprint):
-        if self._add_specs and self._doc:
-            app_or_blueprint.add_url_rule(self._doc, "doc", self.render_doc)
-
-    @property
-    def base_path(self):
-        return ""
-
-
 # Remove Flask restx exception handlers so that we can use our own
 # Otherwise we cannot have custom structured error messages from the Api
 def patched_init_app(self, app):
     self._register_specs(self.blueprint or app)
     self._register_doc(self.blueprint or app)
 
     if len(self.resources) > 0:
```

### Comparing `nextcode-platform-kit-1.1.5/platkit/testcase.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/testcase.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/utils.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 #!/usr/bin/env python
+from __future__ import annotations
 
 import os
 import logging
 from unittest import mock
 from datetime import date
 from http import HTTPStatus
 
 import yaml
+import json
 from pathlib import Path
 from decouple import AutoConfig
 from cryptography.hazmat.primitives.serialization import load_pem_public_key
 from cryptography.hazmat.backends import default_backend
 
 from flask import current_app, url_for
-from flask.json import JSONEncoder
+from flask.json.provider import JSONProvider
 from flask_restx import abort
 
 log = logging.getLogger(__name__)
 
 
-class CustomJSONEncoder(JSONEncoder):
+class CustomJSONEncoder(json.JSONEncoder):
     """Extend the JSON encoder to treat date-time objects as strict
     rfc3339 types.
     """
 
     def default(self, obj):  # pylint: disable=E0202
         # This fixes endless recursion in unittests
         if isinstance(obj, mock.MagicMock):
             return dict(obj)
         if isinstance(obj, date):
             return obj.isoformat() + "Z"
         # backwards-compatibility fix for models
         elif hasattr(obj, "as_dict"):
             return obj.as_dict()
         else:
-            return JSONEncoder.default(self, obj)
+            return json.JSONEncoder.default(self, obj)
+
+
+class CustomJSONProvider(JSONProvider):
+    def dumps(self, obj, **kwargs):
+        return json.dumps(obj, **kwargs, cls=CustomJSONEncoder)
+
+    def loads(self, s: str | bytes, **kwargs):
+        return json.loads(s, **kwargs)
 
 
 def get_build_info(root_path):
     """Return build info from package yaml file called .build_info.yml which is generated from the
     build process and at the very least return the version from the package..
     """
     directory = os.path.dirname(root_path)
```

### Comparing `nextcode-platform-kit-1.1.5/platkit/logsetup.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/logsetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/middleware/logstash_formatter.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/middleware/logstash_formatter.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/middleware/reverse_proxied.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/middleware/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/config.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/config.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/models/responses.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/models/responses.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/csautils.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/csautils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/platkit/auth.py` & `nextcode-platform-kit-1.1.6.dev0/platkit/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 def unpack_user_jwt():
     """Decodes and returns the auth jwt from the request if any"""
     current_user = None
     try:
         if request.headers.get("Authorization"):
             token = request.headers.get("Authorization").split("Bearer ")[1]
-            current_user = jwt.decode(token, algorithms=["RS256"], verify=False)
+            current_user = jwt.decode(token, algorithms=["RS256"], options={'verify_signature': False})
     except Exception:
         pass
     return current_user
 
 
 def get_private_key():
     """
@@ -145,28 +145,27 @@
 
     return payload
 
 
 def encode_token(payload):
     algorithm = "RS256"
     private_key = get_private_key()
-    token = jwt.encode(payload, private_key, algorithm=algorithm).decode("utf-8")
+    token = jwt.encode(payload, private_key, algorithm=algorithm)
 
     return token
 
 
 def validate_self_issued_jwt(token):
     # verify that the private key matches our public key
     try:
         jwt.decode(
             token,
             get_public_key(),
             algorithms=["RS256"],
-            verify=True,
-            options={"verify_exp": False, "verify_aud": False},
+            options={"verify_exp": False, "verify_aud": False, 'verify_signature': True},
         )
     except Exception as e:
         abort(HTTPStatus.INTERNAL_SERVER_ERROR, message="Could not decode token: %s" % repr(e))
 
 
 def get_auth_payload(user_name, client_id="api-key-client", roles=None):
     """Create a valid token and put into authentication payload similar to OpenID connect payloads.
@@ -179,15 +178,15 @@
     return auth_payload
 
 
 def get_auth_payload_from_refresh_token(user_name, refresh_token):
     """Generates token pairs from a refresh token, for development
     """
     try:
-        payload = jwt.decode(refresh_token.encode("UTF-8"), verify=False)
+        payload = jwt.decode(refresh_token.encode("UTF-8"), algorithms=["RS256"], options={'verify_signature': False})
     except Exception as e:
         abort(HTTPStatus.BAD_REQUEST, message="Refresh token is invalid: %s" % repr(e))
     access_token = create_development_jwt_token(user_name, payload["aud"], "Bearer", 5 * 60)
 
     auth_payload = {"access_token": access_token, "refresh_token": refresh_token}
 
     return auth_payload
@@ -254,22 +253,22 @@
             abort(HTTPStatus.UNAUTHORIZED, message="please log-in")
 
     if not data_secure:
 
         try:
             # This manipulation is to test the integrity of the token.
             # ! this payload is insecure and will not be used outside of this test
-            data_unsecure = jwt.decode(token, algorithms=["RS256"], verify=False)
+            data_unsecure = jwt.decode(token,  algorithms=["RS256"], options={'verify_signature': False})
             aud = data_unsecure.get("aud")
         except jwt.InvalidTokenError:
             abort(HTTPStatus.UNAUTHORIZED, message="Token is indecipherable")
 
         try:
             # Token verification with public key - secure
-            data_secure = jwt.decode(token, public_key, algorithms=["RS256"], verify=True, audience=aud)
+            data_secure = jwt.decode(token, public_key, audience=aud, algorithms=["RS256"], options={'verify_signature': True})
         except jwt.ExpiredSignatureError:
             abort(HTTPStatus.UNAUTHORIZED, message="Token has expired. Please re-authenticate.")
         except jwt.InvalidTokenError as kex:
             if "Signature verification failed" in str(kex):
                 log.error(
                     "In all likelyhood we have a wrong public key for keycloak server "
                     "or the user is using a token for another keycloak server. "
```

### Comparing `nextcode-platform-kit-1.1.5/setup.py` & `nextcode-platform-kit-1.1.6.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/README.md` & `nextcode-platform-kit-1.1.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.5
+Version: 1.1.6.dev0
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-
-UNKNOWN
-
```

### Comparing `nextcode-platform-kit-1.1.5/nextcode_platform_kit.egg-info/SOURCES.txt` & `nextcode-platform-kit-1.1.6.dev0/nextcode_platform_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

