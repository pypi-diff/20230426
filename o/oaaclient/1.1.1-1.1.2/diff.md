# Comparing `tmp/oaaclient-1.1.1.tar.gz` & `tmp/oaaclient-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaaclient-1.1.1.tar", last modified: Tue Mar 14 20:09:49 2023, max compression
+gzip compressed data, was "oaaclient-1.1.2.tar", last modified: Wed Apr 26 18:43:43 2023, max compression
```

## Comparing `oaaclient-1.1.1.tar` & `oaaclient-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:09:49.516167 oaaclient-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-14 20:09:30.000000 oaaclient-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-14 20:09:49.516167 oaaclient-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-14 20:09:30.000000 oaaclient-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:09:49.516167 oaaclient-1.1.1/oaaclient/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-14 20:09:30.000000 oaaclient-1.1.1/oaaclient/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37507 2023-03-14 20:09:30.000000 oaaclient-1.1.1/oaaclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-14 20:09:30.000000 oaaclient-1.1.1/oaaclient/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    89791 2023-03-14 20:09:30.000000 oaaclient-1.1.1/oaaclient/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-14 20:09:30.000000 oaaclient-1.1.1/oaaclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:09:49.516167 oaaclient-1.1.1/oaaclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 20:09:49.000000 oaaclient-1.1.1/oaaclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-14 20:09:30.000000 oaaclient-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 20:09:49.516167 oaaclient-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-14 20:09:30.000000 oaaclient-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:09:49.516167 oaaclient-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36240 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_custom_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_custom_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_payload_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_reprs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_template_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-03-14 20:09:30.000000 oaaclient-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.981456 oaaclient-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 18:43:20.000000 oaaclient-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-26 18:43:43.977456 oaaclient-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-26 18:43:20.000000 oaaclient-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/oaaclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39135 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90551 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-26 18:43:20.000000 oaaclient-1.1.2/oaaclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/oaaclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 18:43:43.000000 oaaclient-1.1.2/oaaclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-26 18:43:20.000000 oaaclient-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:43:43.981456 oaaclient-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 18:43:20.000000 oaaclient-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:43:43.977456 oaaclient-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36240 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_custom_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_custom_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_payload_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_reprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_template_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-26 18:43:20.000000 oaaclient-1.1.2/tests/test_utils.py
```

### Comparing `oaaclient-1.1.1/LICENSE` & `oaaclient-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/PKG-INFO` & `oaaclient-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.1
+Version: 1.1.2
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.1/README.md` & `oaaclient-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/oaaclient/client.py` & `oaaclient-1.1.2/oaaclient/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 
 import argparse
 import base64
 import gzip
 import json
 import logging
 import os
+import platform
 import re
 import socket
 import sys
 import urllib.parse
 from datetime import datetime
 from enum import Enum
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.exceptions import JSONDecodeError as RequestsJSONDecodeError
 from urllib3.util.retry import Retry
 
+from oaaclient import __version__ as OAACLIENT_VERSION
 import oaaclient.utils as oaautils
 from oaaclient.templates import CustomApplication, CustomIdPProvider
 
 PROVIDER_ICON_MAX_SIZE = 64_000
 
 log = logging.getLogger(__name__)
 
@@ -72,23 +74,25 @@
 
 class OAAConnectionError(OAAClientError):
     """ Error with API Connection"""
 
 class OAAClient():
     """Class for OAA API Connection and Management.
 
-    Utilities for OAA-related operations with Veza API calls. Manages custom providers and datasources, and can push OAA
+    Utilities for OAA-related operations with Veza API calls. Manages custom providers and data sources, and can push OAA
     payloads from JSON or template objects.
 
+    Connection url and API key can be automatically loaded from OS environment values if set. To utilize environment variables
+    initialize OAAClient without providing a URL or API key value and set the `VEZA_URL` and `VEZA_API_KEY` OS environment variables.
+
     Args:
-        url (str): URL for Veza instance.
-        api_key (str): Veza API key.
+        url (str, optional): URL for Veza instance.
+        api_key (str, optional): Veza API key.
         username (str, optional): Not used (legacy). Defaults to None.
         token (str, optional): Legacy parameter name for API key. Defaults to None.
-        skip_validation (bool, optional): Skip test API call to validate host and credentials. Defaults to False.
 
     Attributes:
         url (str): URL of the Veza instance to connect to
         api_key (str): Veza API key
         enable_compression (bool): Enable or disable compression of the OAA payload during push, defaults to enabled (True)
 
     Raises:
@@ -105,17 +109,20 @@
     # platform defined allowed characters for use unless otherwise allowed defined
     ALLOWED_CHARACTERS = r"^[ @#$%&*:()!,a-zA-Z0-9_'\"=.-]*$"
 
     # default number of entities to get when requesting a page size.
     # Must be passed with params for API call when calling paging APIs `params={"page_size": self.DEFAULT_PAGE_LENGTH}`
     DEFAULT_PAGE_SIZE = 250
 
-    def __init__(self, url:str, api_key: str = None, username: str = None, token: str = None):
-        if not url:
-            raise ValueError("Must provide url argument")
+    def __init__(self, url:str = None, api_key: str = None, username: str = None, token: str = None):
+
+        if not url and "VEZA_URL" in os.environ:
+            url = os.getenv("VEZA_URL", "")
+        elif not url:
+            raise ValueError("Must provide Veza URL")
 
         if not re.match(r"^https:\/\/.*", url):
             self.url = f"https://{url}"
         else:
             self.url = url
         self.url = self.url.rstrip("/")
 
@@ -126,16 +133,20 @@
         if unsafe_https.lower() == "true":
             self.verify_ssl = False
 
         self.username = username
 
         if api_key:
             self.api_key = api_key
-        else:
+        elif token:
             self.api_key = token
+        elif "VEZA_API_KEY" in os.environ:
+            self.api_key = os.getenv("VEZA_API_KEY", "")
+        else:
+            raise ValueError("Must provide Veza API key")
 
         if not self.url:
             raise OAAClientError("MISSING_URL", "URL cannot be None")
         if not self.api_key:
             raise OAAClientError("MISSING_AUTH", "API key cannot be None")
 
         # enable payload compression by default, connection object property can be set to False to disable
@@ -151,14 +162,16 @@
 
         retry_policy = OAARetry(backoff_max=self.DEFAULT_RETRY_MAX_BACKOFF, total=retry_count, backoff_factor=self.DEFAULT_RETRY_BACKOFF_FACTOR, status_forcelist=[429, 500, 502, 503, 504])
         adapter = HTTPAdapter(max_retries=retry_policy)
         self._http_adapter = requests.Session()
         self._http_adapter.mount("https://", adapter)
         self._http_adapter.mount("http://", adapter)
 
+        self.update_user_agent()
+
         # test connection
         self._test_connection()
 
     def get_provider_list(self) -> list[dict]:
         """Return list of Providers.
 
         Returns:
@@ -769,15 +782,18 @@
             OAAClientError: For errors connecting to or returned by the Veza tenant
 
         Returns:
             dict: Veza API JSON response as dictionary
         """
 
         response = None
-        headers = {"authorization": f"Bearer {self.api_key}"}
+
+        headers = {}
+        headers["authorization"] = f"Bearer {self.api_key}"
+        headers["user-agent"] = self._user_agent
         api_timeout = 300
         api_path = api_path.lstrip("/")
 
         if params:
             params_str = urllib.parse.urlencode(params)
         else:
             params_str = None
@@ -805,14 +821,18 @@
                 result = {}
                 code = "ERROR"
                 if response.reason:
                     message = f"Error reason: {response.reason}"
                 else:
                     message = "Unknown error, response is not JSON"
 
+            log.debug(f"Error returned by Veza API: {e.response.status_code} {message} {e.response.url} request_id: {request_id} timestamp {timestamp}")
+            for d in details:
+                log.debug(d)
+
             raise OAAResponseError(code, message, status_code=e.response.status_code, details=details, timestamp=timestamp, request_id=request_id)
         except requests.exceptions.JSONDecodeError as e:
             # HTTP response reports success but response does not decode to JSON
             if response:
                 status_code = response.status_code
             else:
                 status_code = None
@@ -851,14 +871,37 @@
         except OAAResponseError as e:
             log.debug("API returned error during API connection test")
             raise e
         except OAAConnectionError as e:
             log.debug("Unable to connect during API connection test")
             raise e
 
+    def update_user_agent(self, extra: str = "") -> None:
+        """Updates the User-Agent string passed with all API calls
+
+        Generates a User-Agent with the oaaclient version, Python version and platform information.
+
+        The optional `extra` string will be appended if provided.
+
+        Args:
+            extra (str, optional): Additional information to append to User-Agent string. Defaults to "".
+        """
+
+        python_version = platform.python_version()
+        os_name = platform.system()
+        os_version = platform.release()
+
+        self._user_agent = f"oaaclient/{OAACLIENT_VERSION} python/{python_version} {os_name}/{os_version};"
+        if extra:
+            self._user_agent += f" {extra}"
+
+        log.debug(f"User-Agent {self._user_agent}")
+
+        return
+
 class OAARetry(Retry):
     """Super class for urllib3.util.retry
 
     Super class to allow modifying the default max backoff time from 120 seconds
     to our own value
 
     Args:
```

### Comparing `oaaclient-1.1.1/oaaclient/structures.py` & `oaaclient-1.1.2/oaaclient/structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/oaaclient/templates.py` & `oaaclient-1.1.2/oaaclient/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,16 +370,16 @@
 
         return self.idp_identities[name]
 
     def add_tag(self, key: str, value: str = "") -> None:
         """ Add a tag to the Application
 
         Args:
-            key (str): Name for the tag
-            value (str, optional): String value for tag. Defaults to "".
+            key (str): Key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
+            value (str, optional): Value for Tag, will appear in Veza as `key:value`. Must be letters, numbers, whitespace and the special characters @,._- only. Defaults to "".
         """
 
         tag = Tag(key=key, value=value)
         if tag not in self.tags:
             self.tags.append(tag)
 
     def set_property(self, property_name: str, property_value: any) -> None:
@@ -603,16 +603,16 @@
         """ No longer supported, access should be added through identity (local_user, local_group, idp) """
         raise Exception("No longer supported: Add access via identity")
 
     def add_tag(self, key: str, value: str = "") -> None:
         """ Add a new tag to resource.
 
         Args:
-            key (str): Name for the tag.
-            value (str, optional): String value for tag. Defaults to "".
+            key (str): Key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
+            value (str, optional): Value for Tag, will appear in Veza as `key:value`. Must be letters, numbers, whitespace and the special characters @,._- only. Defaults to "".
         """
         tag = Tag(key=key, value=value)
         if tag not in self.tags:
             self.tags.append(tag)
 
     def set_property(self, property_name: str, property_value: any) -> None:
         """ Set the value for a custom property on a resource or sub-resource.
@@ -779,16 +779,16 @@
 
         return response
 
     def add_tag(self, key: str, value: str = "") -> None:
         """ Add a new tag to identity.
 
         Args:
-            key (str): Name for the tag
-            value (str, optional): String value for tag. Defaults to "".
+            key (str): Key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
+            value (str, optional): Value for Tag, will appear in Veza as `key:value`. Must be letters, numbers, whitespace and the special characters @,._- only. Defaults to "".
         """
 
         tag = Tag(key=key, value=value)
         if tag not in self.tags:
             self.tags.append(tag)
 
     def set_property(self, property_name: str, property_value: any) -> None:
@@ -1121,21 +1121,21 @@
         """
         role = str(role)
 
         if (self.unique_id and self.unique_id == role) or (self.unique_id is None and self.name == role):
             raise OAATemplateException("Cannot add role to self")
 
         self.roles = append_helper(self.roles, role)
-        
+
     def add_tag(self, key: str, value: str = "") -> None:
         """ Add a new tag to role.
 
         Args:
-            key (str): Name for the tag
-            value (str, optional): String value for tag. Defaults to "".
+            key (str): Key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
+            value (str, optional): Value for Tag, will appear in Veza as `key:value`. Must be letters, numbers, whitespace and the special characters @,._- only. Defaults to "".
         """
 
         tag = Tag(key=key, value=value)
         if tag not in self.tags:
             self.tags.append(tag)
 
     def set_property(self, property_name: str, property_value: any) -> None:
@@ -1458,15 +1458,15 @@
             OAATemplateException: Name contains invalid characters or does not start with a letter
         """
 
         if not isinstance(name, str):
             raise OAATemplateException("Property name must be a string")
 
         if not re.match(r"^[a-z][a-z_]*$", name.lower()):
-            raise OAATemplateException("Lower-cased property name must match the pattern: ^[a-z][a-z_]*$'")
+            raise OAATemplateException(f"Lower-cased property name must match the pattern: ^[a-z][a-z_]*$': {name}")
 
         return
 
 
 ###############################################################################
 # Custom IdP Provider
 ###############################################################################
@@ -2025,33 +2025,33 @@
             raise OAATemplateException("property_type must be type OAAPropertyType enum")
 
 
 ###############################################################################
 # Shared models
 ###############################################################################
 class Tag():
-    """ Veza tag data model.
+    """ Veza Tag data model.
 
     Args:
         key (str): key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
-        value (str, optional): Value for tag, will appear in Veza as `key:value`. Must be letters, numbers or _ (underscore) only.
+        value (str, optional): Value for tag, will appear in Veza as `key:value`. Must be letters, numbers, whitespace and the special characters @,._- only.
 
     Attributes:
         key (str): key for tag, aka name. Must be present and must be letters, numbers or _ (underscore) only.
         value (str): Value for tag, will appear in Veza as `key:value`. Must be letters, numbers and the special characters @,._ only.
     """
 
     def __init__(self, key: str, value: str = "") -> None:
         self.key = str(key)
         self.value = str(value)
 
-        if not re.match(r"^[\w\d\s_]+$", self.key):
-            raise OAATemplateException(f"Invalid characters in tag key {self.key}: may only contain letters, numbers, whitespace and _ (underscore)")
+        if not re.match(r"^[\w\d_]+$", self.key):
+            raise OAATemplateException(f"Invalid characters in tag key. Key '{self.key}'. Key may only contain letters, numbers, and _ (underscore)")
         if self.value != "" and not re.match(r"^[\w\d\s_,@\.-]+$", self.value):
-            raise OAATemplateException(f"Invalid characters in tag value {self.value}: may only contain letters, numbers, whitespace and the special characters @,._-")
+            raise OAATemplateException(f"Invalid characters in tag value. Value '{self.value}'. Value may only contain letters, numbers, whitespace and the special characters @,._-")
 
     def __str__(self) -> str:
         if self.value:
             return f"Tag {self.key}:{self.value}"
         else:
             return f"Tag {self.key}"
```

### Comparing `oaaclient-1.1.1/oaaclient/utils.py` & `oaaclient-1.1.2/oaaclient/utils.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/oaaclient.egg-info/PKG-INFO` & `oaaclient-1.1.2/oaaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaaclient
-Version: 1.1.1
+Version: 1.1.2
 Summary: Veza Open Authorization API (OAA) SDK
 Author-email: "Veza Technologies Inc." <oaa_dev@veza.com>
 License: MIT
 Project-URL: homepage, https://github.com/veza/oaaclient-py
 Project-URL: repository, https://github.com/veza/oaaclient-py
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `oaaclient-1.1.1/oaaclient.egg-info/SOURCES.txt` & `oaaclient-1.1.2/oaaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/pyproject.toml` & `oaaclient-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_client.py` & `oaaclient-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_commands.py` & `oaaclient-1.1.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_custom_application.py` & `oaaclient-1.1.2/tests/test_custom_application.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_custom_idp.py` & `oaaclient-1.1.2/tests/test_custom_idp.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_payload_push.py` & `oaaclient-1.1.2/tests/test_payload_push.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_reprs.py` & `oaaclient-1.1.2/tests/test_reprs.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_structures.py` & `oaaclient-1.1.2/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `oaaclient-1.1.1/tests/test_tags.py` & `oaaclient-1.1.2/tests/test_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     assert new_tag is not None
     assert new_tag.key == "test"
     assert new_tag.value == "value"
 
 
 def test_tag_characters():
 
-    good_tag = Tag("lettér 123_", "letter.123@something.com,characters456@blah.com and space")
-    assert good_tag.key == "lettér 123_"
+    good_tag = Tag("lettér123_", "letter.123@something.com,characters456@blah.com and space")
+    assert good_tag.key == "lettér123_"
     assert good_tag.value == "letter.123@something.com,characters456@blah.com and space"
 
     with pytest.raises(OAATemplateException) as e:
         Tag("illegal:value!")
 
     assert e is not None
     assert "Invalid characters in tag key" in e.value.message
```

### Comparing `oaaclient-1.1.1/tests/test_utils.py` & `oaaclient-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

