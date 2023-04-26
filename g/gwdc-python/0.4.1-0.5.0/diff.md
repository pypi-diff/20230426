# Comparing `tmp/gwdc-python-0.4.1.tar.gz` & `tmp/gwdc_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdc-python-0.4.1.tar", max compression
+gzip compressed data, was "gwdc_python-0.5.0.tar", max compression
```

## Comparing `gwdc-python-0.4.1.tar` & `gwdc_python-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1076 2021-07-14 03:56:25.321182 gwdc-python-0.4.1/LICENSE
--rw-r--r--   0        0        0      195 2021-07-14 03:56:25.321182 gwdc-python-0.4.1/README.rst
--rw-r--r--   0        0        0       67 2022-03-30 04:37:54.864865 gwdc-python-0.4.1/gwdc_python/__init__.py
--rw-r--r--   0        0        0     1091 2022-06-23 04:56:34.805258 gwdc-python-0.4.1/gwdc_python/exceptions.py
--rw-r--r--   0        0        0       61 2022-05-24 05:38:08.345632 gwdc-python-0.4.1/gwdc_python/files/__init__.py
--rw-r--r--   0        0        0     3980 2022-05-24 05:38:08.345632 gwdc-python-0.4.1/gwdc_python/files/file_reference.py
--rw-r--r--   0        0        0     2598 2022-05-24 00:51:21.897363 gwdc-python-0.4.1/gwdc_python/files/filters.py
--rw-r--r--   0        0        0      659 2022-05-24 00:51:21.897363 gwdc-python-0.4.1/gwdc_python/files/identifiers.py
--rw-r--r--   0        0        0        0 2022-05-24 00:51:21.897363 gwdc-python-0.4.1/gwdc_python/files/tests/__init__.py
--rw-r--r--   0        0        0     4897 2022-05-24 00:51:21.897363 gwdc-python-0.4.1/gwdc_python/files/tests/test_file_reference.py
--rw-r--r--   0        0        0     4444 2022-05-24 00:51:21.897363 gwdc-python-0.4.1/gwdc_python/files/tests/test_filters.py
--rw-r--r--   0        0        0     3296 2022-05-24 00:51:21.901363 gwdc-python-0.4.1/gwdc_python/files/tests/test_identifiers.py
--rw-r--r--   0        0        0     4378 2022-06-23 04:56:34.805258 gwdc-python-0.4.1/gwdc_python/gwdc.py
--rw-r--r--   0        0        0      541 2022-06-08 01:43:57.767269 gwdc-python-0.4.1/gwdc_python/helpers.py
--rw-r--r--   0        0        0       26 2022-06-07 05:22:42.476139 gwdc-python-0.4.1/gwdc_python/jobs/__init__.py
--rw-r--r--   0        0        0     1421 2022-06-08 05:30:42.361873 gwdc-python-0.4.1/gwdc_python/jobs/base.py
--rw-r--r--   0        0        0     3298 2022-06-08 05:30:42.361873 gwdc-python-0.4.1/gwdc_python/jobs/meta.py
--rw-r--r--   0        0        0        0 2022-06-07 05:22:42.476139 gwdc-python-0.4.1/gwdc_python/jobs/tests/__init__.py
--rw-r--r--   0        0        0      789 2022-06-08 01:43:57.767269 gwdc-python-0.4.1/gwdc_python/jobs/tests/test_base.py
--rw-r--r--   0        0        0      830 2022-06-07 05:22:42.476139 gwdc-python-0.4.1/gwdc_python/jobs/tests/test_meta.py
--rw-r--r--   0        0        0      227 2022-06-08 01:43:57.767269 gwdc-python-0.4.1/gwdc_python/logger.py
--rw-r--r--   0        0        0        0 2021-06-22 05:11:59.641512 gwdc-python-0.4.1/gwdc_python/tests/__init__.py
--rw-r--r--   0        0        0     4022 2022-06-23 04:56:34.805258 gwdc-python-0.4.1/gwdc_python/tests/test_gwdc_python.py
--rw-r--r--   0        0        0      112 2022-06-08 01:43:57.767269 gwdc-python-0.4.1/gwdc_python/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-05-24 00:51:21.901363 gwdc-python-0.4.1/gwdc_python/utils/tests/__init__.py
--rw-r--r--   0        0        0     2244 2022-06-08 01:43:57.771269 gwdc-python-0.4.1/gwdc_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1337 2022-05-24 00:51:21.901363 gwdc-python-0.4.1/gwdc_python/utils/typed_list.py
--rw-r--r--   0        0        0     2709 2022-06-08 05:30:42.361873 gwdc-python-0.4.1/gwdc_python/utils/utils.py
--rw-r--r--   0        0        0      879 2022-06-23 04:56:34.805258 gwdc-python-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1308 2022-06-23 05:02:49.194150 gwdc-python-0.4.1/setup.py
--rw-r--r--   0        0        0     1210 2022-06-23 05:02:49.194418 gwdc-python-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-07-19 20:27:11.070554 gwdc_python-0.5.0/LICENSE
+-rw-r--r--   0        0        0      195 2021-07-19 20:27:11.070554 gwdc_python-0.5.0/README.rst
+-rw-r--r--   0        0        0       67 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/__init__.py
+-rw-r--r--   0        0        0     1091 2022-08-09 17:58:23.302425 gwdc_python-0.5.0/gwdc_python/exceptions.py
+-rw-r--r--   0        0        0       61 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/__init__.py
+-rw-r--r--   0        0        0     3980 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/file_reference.py
+-rw-r--r--   0        0        0     2598 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/filters.py
+-rw-r--r--   0        0        0      659 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/identifiers.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/__init__.py
+-rw-r--r--   0        0        0     4897 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_file_reference.py
+-rw-r--r--   0        0        0     4444 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_filters.py
+-rw-r--r--   0        0        0     3296 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_identifiers.py
+-rw-r--r--   0        0        0     4485 2023-04-26 01:47:22.282014 gwdc_python-0.5.0/gwdc_python/gwdc.py
+-rw-r--r--   0        0        0      541 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/helpers.py
+-rw-r--r--   0        0        0       26 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/__init__.py
+-rw-r--r--   0        0        0     1421 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/base.py
+-rw-r--r--   0        0        0     3298 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/meta.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/__init__.py
+-rw-r--r--   0        0        0      789 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/test_base.py
+-rw-r--r--   0        0        0      830 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/test_meta.py
+-rw-r--r--   0        0        0      227 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/logger.py
+-rw-r--r--   0        0        0        0 2021-06-30 01:51:45.372719 gwdc_python-0.5.0/gwdc_python/tests/__init__.py
+-rw-r--r--   0        0        0     5269 2023-04-26 01:46:57.208773 gwdc_python-0.5.0/gwdc_python/tests/test_gwdc_python.py
+-rw-r--r--   0        0        0      112 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2244 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1337 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/typed_list.py
+-rw-r--r--   0        0        0     2709 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/utils.py
+-rw-r--r--   0        0        0      879 2023-04-26 02:44:46.210050 gwdc_python-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 gwdc_python-0.5.0/setup.py
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gwdc_python-0.5.0/PKG-INFO
```

### Comparing `gwdc-python-0.4.1/LICENSE` & `gwdc_python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/exceptions.py` & `gwdc_python-0.5.0/gwdc_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/file_reference.py` & `gwdc_python-0.5.0/gwdc_python/files/file_reference.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/filters.py` & `gwdc_python-0.5.0/gwdc_python/files/filters.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/identifiers.py` & `gwdc_python-0.5.0/gwdc_python/files/identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/tests/test_file_reference.py` & `gwdc_python-0.5.0/gwdc_python/files/tests/test_file_reference.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/tests/test_filters.py` & `gwdc_python-0.5.0/gwdc_python/files/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/files/tests/test_identifiers.py` & `gwdc_python-0.5.0/gwdc_python/files/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/gwdc.py` & `gwdc_python-0.5.0/gwdc_python/gwdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,27 @@
 class GWDC:
     def __init__(self, token, auth_endpoint, endpoint, custom_error_handler=None):
         self.api_token = token
         self.auth_endpoint = auth_endpoint
         self.endpoint = endpoint
         if custom_error_handler:
             self._apply_custom_error_handler(custom_error_handler)
-        self._obtain_access_token()
+
+        if self.api_token:
+            self._obtain_access_token()
 
     def _apply_custom_error_handler(self, custom_error_handler):
         self._obtain_access_token = custom_error_handler(self._obtain_access_token)
         self._refresh_access_token = custom_error_handler(self._refresh_access_token)
         self.request = custom_error_handler(self.request)
 
-    def _request(self, endpoint, query, variables=None, headers={}, method="POST"):
+    def _request(self, endpoint, query, variables=None, headers=None, method="POST"):
+        if headers is None:
+            headers = {}
+
         variables = camelize(variables)
         variables, files, files_map = split_variables_dict(variables)
 
         if files:
             operations = {
                 "query": query,
                 "variables": variables,
@@ -115,12 +120,12 @@
         )
         self.jwt_token = data["refresh_token"]["token"]
         self.refresh_token = data["refresh_token"]["refresh_token"]
 
     @handle_request_errors
     def request(self, query, variables=None, headers=None, authorize=True):
 
-        all_headers = {'Authorization': 'JWT ' + self.jwt_token} if authorize else {}
+        all_headers = {'Authorization': 'JWT ' + self.jwt_token} if authorize and self.api_token else {}
         if headers is not None:
             all_headers = {**all_headers, **headers}
 
         return self._request(endpoint=self.endpoint, query=query, variables=variables, headers=all_headers)
```

### Comparing `gwdc-python-0.4.1/gwdc_python/helpers.py` & `gwdc_python-0.5.0/gwdc_python/helpers.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/jobs/base.py` & `gwdc_python-0.5.0/gwdc_python/jobs/base.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/jobs/meta.py` & `gwdc_python-0.5.0/gwdc_python/jobs/meta.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/jobs/tests/test_base.py` & `gwdc_python-0.5.0/gwdc_python/jobs/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/jobs/tests/test_meta.py` & `gwdc_python-0.5.0/gwdc_python/jobs/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/tests/test_gwdc_python.py` & `gwdc_python-0.5.0/gwdc_python/tests/test_gwdc_python.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,21 +44,27 @@
     errors = [{"message": 'Signature has expired'}]
     return {"text": json.dumps({"errors": errors})}
 
 
 # Set up GWDC class with specified responses
 @pytest.fixture
 def setup_gwdc(requests_mock):
-    def _setup_gwdc(auth_responses=[], responses=[], error_handler=None):
+    def _setup_gwdc(auth_responses=None, responses=None, error_handler=None, token='mock_token'):
+        if responses is None:
+            responses = []
+
+        if auth_responses is None:
+            auth_responses = []
+
         auth_response_list = [response() for response in auth_responses]
         response_list = [response() for response in responses]
         requests_mock.post('https://gwcloud.org.au/auth/graphql', auth_response_list)
         requests_mock.post('https://gwcloud.org.au/bilby/graphql', response_list)
         return GWDC(
-            token='mock_token',
+            token=token,
             auth_endpoint='https://gwcloud.org.au/auth/graphql',
             endpoint='https://gwcloud.org.au/bilby/graphql',
             custom_error_handler=error_handler
         )
     return _setup_gwdc
 
 
@@ -86,15 +92,15 @@
     )
     gwdc._refresh_access_token()
     assert gwdc.jwt_token == "mock_jwt_token_new"
     assert gwdc.refresh_token == "mock_refresh_token_new"
 
 
 # Test that a token will be automatically refreshed if it has expired
-def test_gwdc_request(setup_gwdc):
+def test_gwdc_request(setup_gwdc, requests_mock):
     gwdc = setup_gwdc(
         auth_responses=[access_token_response, refresh_token_response],
         responses=[access_token_expired, request_test_response]
     )
     assert gwdc.jwt_token == "mock_jwt_token"
     assert gwdc.refresh_token == "mock_refresh_token"
     response = gwdc.request(
@@ -104,14 +110,17 @@
             }
         """
     )
     assert gwdc.jwt_token == "mock_jwt_token_new"
     assert gwdc.refresh_token == "mock_refresh_token_new"
     assert response["test_response"] == "mock_response"
 
+    # Authorization should have been provided in the headers
+    assert "Authorization" in requests_mock.request_history[-1].headers
+
 
 # Test that GWDC will allow the custom error handler to intercept raised errors
 def test_gwdc_custom_error_handling_token(setup_gwdc):
     class TestException(Exception):
         pass
 
     def custom_error_handler(f):
@@ -123,7 +132,43 @@
         return wrapper
 
     with pytest.raises(TestException):
         setup_gwdc(
             auth_responses=[api_token_incorrect],
             error_handler=custom_error_handler
         )
+
+
+# Test that creating an instance without a token works
+def test_gwdc_no_token(setup_gwdc, requests_mock):
+    try:
+        setup_gwdc(
+            auth_responses=[],
+            responses=[],
+            token=""
+        )
+    except json.decoder.JSONDecodeError:
+        pytest.fail("Unexpected error when creating GWDC without a token")
+
+    assert requests_mock.call_count == 0
+
+
+# Test that requests still work correctly without providing a token
+def test_gwdc_request_no_token(setup_gwdc, requests_mock):
+    gwdc = setup_gwdc(
+        auth_responses=[],
+        responses=[request_test_response],
+        token=""
+    )
+
+    response = gwdc.request(
+        query="""
+            query {
+                testResponse
+            }
+        """
+    )
+
+    assert response["test_response"] == "mock_response"
+
+    # Authorization should not have been provided in the headers
+    assert "Authorization" not in requests_mock.request_history[0].headers
```

### Comparing `gwdc-python-0.4.1/gwdc_python/utils/tests/test_utils.py` & `gwdc_python-0.5.0/gwdc_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/utils/typed_list.py` & `gwdc_python-0.5.0/gwdc_python/utils/typed_list.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/gwdc_python/utils/utils.py` & `gwdc_python-0.5.0/gwdc_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwdc-python-0.4.1/pyproject.toml` & `gwdc_python-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwdc-python"
-version = "0.4.1"
+version = "0.5.0"
 description = "API for GWDC modules"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwdc_python"
 include = ["LICENSE",]
 
@@ -19,15 +19,15 @@
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 pyhumps = "^3.7.1"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.3"
 requests-mock = "^1.8.0"
 pyflakes = "^2.3.1"
 flake8 = "^3.9.2"
 coverage = "^5.5"
 pytest-cov = "^2.12.1"
 pytest-mock = "^3.7.0"
```

### Comparing `gwdc-python-0.4.1/setup.py` & `gwdc_python-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,21 @@
  'tqdm>=4.61.2,<5.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'gwdc-python',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'API for GWDC modules',
     'long_description': 'GWDC Python API\n===============\n\nThis package handles requests for the GWDC modules. Presently, it primarily handles the requests for `gwcloud-python <https://pypi.org/project/gwcloud-python/>`_.',
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/gravitationalwavedc/gwdc_python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `gwdc-python-0.4.1/PKG-INFO` & `gwdc_python-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: gwdc-python
-Version: 0.4.1
+Version: 0.5.0
 Summary: API for GWDC modules
 Home-page: https://github.com/gravitationalwavedc/gwdc_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.0.2,<5.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.0.2,<5.0.0) ; extra == "docs"
 Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.1,<4.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
 Project-URL: Repository, https://github.com/gravitationalwavedc/gwdc_python
 Description-Content-Type: text/x-rst
 
 GWDC Python API
 ===============
```

