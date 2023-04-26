# Comparing `tmp/ipython_gpt-0.0.5.tar.gz` & `tmp/ipython_gpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython_gpt-0.0.5.tar", max compression
+gzip compressed data, was "ipython_gpt-0.0.6.tar", max compression
```

## Comparing `ipython_gpt-0.0.5.tar` & `ipython_gpt-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-19 07:57:04.045928 ipython_gpt-0.0.5/LICENSE
--rw-r--r--   0        0        0     4694 2023-04-22 11:45:10.284927 ipython_gpt-0.0.5/README.md
--rw-r--r--   0        0        0     1365 2023-04-23 14:07:15.071118 ipython_gpt-0.0.5/ipython_gpt/__init__.py
--rw-r--r--   0        0        0     2009 2023-04-23 14:07:15.071210 ipython_gpt-0.0.5/ipython_gpt/api_client.py
--rw-r--r--   0        0        0      791 2023-04-23 14:07:13.749778 ipython_gpt-0.0.5/ipython_gpt/displays.py
--rw-r--r--   0        0        0     5056 2023-04-23 14:07:15.077081 ipython_gpt-0.0.5/ipython_gpt/subcommands.py
--rw-r--r--   0        0        0     1123 2023-04-23 14:11:42.724604 ipython_gpt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 ipython_gpt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-19 07:57:04.045928 ipython_gpt-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4741 2023-04-26 08:18:35.900837 ipython_gpt-0.0.6/README.md
+-rw-r--r--   0        0        0     1365 2023-04-26 08:38:04.515720 ipython_gpt-0.0.6/ipython_gpt/__init__.py
+-rw-r--r--   0        0        0     2467 2023-04-26 08:40:44.657956 ipython_gpt-0.0.6/ipython_gpt/api_client.py
+-rw-r--r--   0        0        0      791 2023-04-23 14:07:13.749778 ipython_gpt-0.0.6/ipython_gpt/displays.py
+-rw-r--r--   0        0        0     5056 2023-04-26 08:37:29.822724 ipython_gpt-0.0.6/ipython_gpt/subcommands.py
+-rw-r--r--   0        0        0     1123 2023-04-26 08:41:11.925630 ipython_gpt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 ipython_gpt-0.0.6/PKG-INFO
```

### Comparing `ipython_gpt-0.0.5/LICENSE` & `ipython_gpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython_gpt-0.0.5/README.md` & `ipython_gpt-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # IPython ChatGPT extension
 
 [![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![prettier badge](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white)](https://github.com/prettier/prettier)
-[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)4
+[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![test](https://img.shields.io/github/actions/workflow/status/santiagobasulto/ipython-gpt/test.yaml?logo=github&logoColor=white)](https://github.com/santiagobasulto/ipython-gpt/actions/workflows/test.yaml)
 
-This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
+This (standalone, no external dependencies required) extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
 
 **Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality. Check [this issue](https://github.com/santiagobasulto/ipython-gpt/issues/4) for a rough "roadmap".
```

### Comparing `ipython_gpt-0.0.5/ipython_gpt/__init__.py` & `ipython_gpt-0.0.6/ipython_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `ipython_gpt-0.0.5/ipython_gpt/api_client.py` & `ipython_gpt-0.0.6/ipython_gpt/api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,31 @@
 
 
 class APIClientException(Exception):
     pass
 
 
 class APIResponseException(APIClientException):
-    def __init__(self, method, path, headers, query_params, body):
+    def __init__(self, method, path, response_status, response_body):
         self.method = method
         self.path = path
-        self.headers = headers
-        self.query_params = query_params
-        self.body = body
+        self.response_status = response_status
+        self.response_body = response_body
 
     def __str__(self):
-        return f"Failed API Request '{self.method} {self.path}'"
+        error_message = (
+            (self.response_body or {})
+            .get("error", {})
+            .get("message", "No response from API.")
+        )
+        return f"Failed API Request '{self.method} {self.path}'. Got {self.response_status}: {error_message}"
+
+
+class UnauthorizedAPIException(APIResponseException):
+    pass
 
 
 class OpenAIClient:
     def __init__(self, openai_api_key, api_version=DEFAULT_API_VERSION):
         self.openai_api_key = openai_api_key
         self.api_version = api_version
 
@@ -50,16 +58,20 @@
         path = f"/{self.api_version}" + path
         if query_params is not None:
             path += "?" + urllib.parse.urlencode(query_params)
 
         try:
             connection.request(method, path, body, headers)
             resp = connection.getresponse()
+            resp_body = resp.read()
 
+            # TODO: this might raise an exception for an invalid body
+            content = json.loads(resp_body.decode("utf-8"))
             if 200 <= resp.status < 300:
-                resp_body = resp.read()
-                if resp_body and len(resp_body) > 0:
-                    return json.loads(resp_body.decode("utf-8"))
-            else:
-                raise APIResponseException(method, path, headers, query_params, body)
+                return content
+            if resp.status == 401:
+                raise UnauthorizedAPIException(method, path, resp.status, content)
+
+            # Catch all exception for any other not known status
+            raise APIResponseException(method, path, resp.status, content)
         finally:
             connection.close()
```

### Comparing `ipython_gpt-0.0.5/ipython_gpt/displays.py` & `ipython_gpt-0.0.6/ipython_gpt/displays.py`

 * *Files identical despite different names*

### Comparing `ipython_gpt-0.0.5/ipython_gpt/subcommands.py` & `ipython_gpt-0.0.6/ipython_gpt/subcommands.py`

 * *Files identical despite different names*

### Comparing `ipython_gpt-0.0.5/pyproject.toml` & `ipython_gpt-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipython-gpt"
-version = "0.0.5"
+version = "0.0.6"
 description = "A Jupyter/IPython extension to use ChatGPT"
 authors = ["Santiago Basulto <santiago.basulto@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/santiagobasulto/ipython-gpt"
 repository = "https://github.com/santiagobasulto/ipython-gpt"
 keywords = ["ipython", "jupyter", "chatgpt", "openai"]
 classifiers = [
```

### Comparing `ipython_gpt-0.0.5/PKG-INFO` & `ipython_gpt-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-gpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Jupyter/IPython extension to use ChatGPT
 Home-page: https://github.com/santiagobasulto/ipython-gpt
 License: MIT
 Keywords: ipython,jupyter,chatgpt,openai
 Author: Santiago Basulto
 Author-email: santiago.basulto@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -23,18 +23,18 @@
 Project-URL: Repository, https://github.com/santiagobasulto/ipython-gpt
 Description-Content-Type: text/markdown
 
 # IPython ChatGPT extension
 
 [![Black badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![prettier badge](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white)](https://github.com/prettier/prettier)
-[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)4
+[![pre-commit](https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![test](https://img.shields.io/github/actions/workflow/status/santiagobasulto/ipython-gpt/test.yaml?logo=github&logoColor=white)](https://github.com/santiagobasulto/ipython-gpt/actions/workflows/test.yaml)
 
-This extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
+This (standalone, no external dependencies required) extension allows you to use ChatGPT directly from your Jupyter Notebook or IPython Shell ([Demo](https://github.com/santiagobasulto/ipython-gpt/blob/master/Demo.ipynb)).
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230454-44529ea4-920e-4294-9d61-550771a4a95e.png">
 
 <img width="900" alt="IPython GPT, a Jupyter/IPython interface for Chat GPT" src="https://user-images.githubusercontent.com/872296/232230492-9bc50342-9d78-4adb-8168-2f94fcbc3b73.png">
 
 **Important!** This is a very early and raw version, I have a lot of things to improve regarding code quality and missing functionality. Check [this issue](https://github.com/santiagobasulto/ipython-gpt/issues/4) for a rough "roadmap".
```

