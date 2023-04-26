# Comparing `tmp/findmyorder-0.0.9.tar.gz` & `tmp/findmyorder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-0.0.9.tar", max compression
+gzip compressed data, was "findmyorder-1.0.0.tar", max compression
```

## Comparing `findmyorder-0.0.9.tar` & `findmyorder-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-23 14:03:54.167185 findmyorder-0.0.9/LICENSE
--rw-r--r--   0        0        0     1426 2023-04-23 14:03:54.167185 findmyorder-0.0.9/README.md
--rw-r--r--   0        0        0      103 2023-04-23 14:03:54.923196 findmyorder-0.0.9/findmyorder/__init__.py
--rw-r--r--   0        0        0      219 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/config.py
--rw-r--r--   0        0        0      206 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/core.toml
--rw-r--r--   0        0        0     2578 2023-04-23 14:03:54.167185 findmyorder-0.0.9/findmyorder/main.py
--rw-r--r--   0        0        0      962 2023-04-23 14:03:54.923196 findmyorder-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 findmyorder-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-26 15:01:19.233066 findmyorder-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1426 2023-04-26 15:01:19.233066 findmyorder-1.0.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-26 15:01:19.961066 findmyorder-1.0.0/findmyorder/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/config.py
+-rw-r--r--   0        0        0      120 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3112 2023-04-26 15:01:19.233066 findmyorder-1.0.0/findmyorder/main.py
+-rw-r--r--   0        0        0     1194 2023-04-26 15:01:19.961066 findmyorder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 findmyorder-1.0.0/PKG-INFO
```

### Comparing `findmyorder-0.0.9/LICENSE` & `findmyorder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.9/README.md` & `findmyorder-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-0.0.9/pyproject.toml` & `findmyorder-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "0.0.9"
+version = "1.0.0"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
@@ -12,21 +12,35 @@
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 asyncio = "*"
+dynaconf = "*"
+pyparsing = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.pytest.ini_options]
+testpaths = "tests/"
+python_classes = [
+  "Test*",
+  "*Test"
+]
+log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
+log_level = "DEBUG"
+pythonpath = [
+  "."
+]
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `findmyorder-0.0.9/PKG-INFO` & `findmyorder-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 0.0.9
+Version: 1.0.0
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
+Requires-Dist: dynaconf
+Requires-Dist: pyparsing
 Project-URL: Changelog, https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/findmyorder/issues
 Project-URL: Support, https://github.com/mraniki/findmyorder/discussions
 Description-Content-Type: text/markdown
 
 # Find my order.
```

