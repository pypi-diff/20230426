# Comparing `tmp/anonlink_client-0.1.8.tar.gz` & `tmp/anonlink_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonlink_client-0.1.8.tar", max compression
+gzip compressed data, was "anonlink_client-0.1.9.tar", max compression
```

## Comparing `anonlink_client-0.1.8.tar` & `anonlink_client-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1472 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0    10174 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/LICENSE
--rw-r--r--   0        0        0     2073 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/README.md
--rw-r--r--   0        0        0      201 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/__init__.py
--rw-r--r--   0        0        0    17701 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/cli.py
--rw-r--r--   0        0        0      253 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/data/blocking_schema.json
--rw-r--r--   0        0        0     1027 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/data/nvtr_schema.json
--rw-r--r--   0        0        0     1547 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/data/randomnames-schema.json
--rw-r--r--   0        0        0     2176 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/data/schema.json
--rw-r--r--   0        0        0     6757 2023-03-01 23:26:06.241126 anonlink_client-0.1.8/anonlinkclient/utils.py
--rw-r--r--   0        0        0     2024 2023-03-01 23:26:06.253126 anonlink_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 anonlink_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1513 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0    10174 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2073 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/README.md
+-rw-r--r--   0        0        0      201 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/__init__.py
+-rw-r--r--   0        0        0    17701 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/cli.py
+-rw-r--r--   0        0        0      253 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/data/blocking_schema.json
+-rw-r--r--   0        0        0     1027 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/data/nvtr_schema.json
+-rw-r--r--   0        0        0     1547 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/data/randomnames-schema.json
+-rw-r--r--   0        0        0     2176 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/data/schema.json
+-rw-r--r--   0        0        0     6757 2023-04-26 00:36:19.385877 anonlink_client-0.1.9/anonlinkclient/utils.py
+-rw-r--r--   0        0        0     2030 2023-04-26 00:36:19.397877 anonlink_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 anonlink_client-0.1.9/PKG-INFO
```

### Comparing `anonlink_client-0.1.8/CHANGELOG.md` & `anonlink_client-0.1.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Change Log
 
-## new version
+
+## 0.1.9
+
+- Update to much faster clkhash v0.18.0 #197
 
 ## 0.1.8
 - Support blocklib >= 0.1.8 #188
 
 ## 0.1.7
 - Support for Python 3.11 and latest clkhash version #184
```

### Comparing `anonlink_client-0.1.8/LICENSE` & `anonlink_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/README.md` & `anonlink_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/anonlinkclient/cli.py` & `anonlink_client-0.1.9/anonlinkclient/cli.py`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/anonlinkclient/data/nvtr_schema.json` & `anonlink_client-0.1.9/anonlinkclient/data/nvtr_schema.json`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/anonlinkclient/data/randomnames-schema.json` & `anonlink_client-0.1.9/anonlinkclient/data/randomnames-schema.json`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/anonlinkclient/data/schema.json` & `anonlink_client-0.1.9/anonlinkclient/data/schema.json`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/anonlinkclient/utils.py` & `anonlink_client-0.1.9/anonlinkclient/utils.py`

 * *Files identical despite different names*

### Comparing `anonlink_client-0.1.8/pyproject.toml` & `anonlink_client-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anonlink-client"
-version = "0.1.8"
+version = "0.1.9"
 description = "Client side tool for clkhash and blocklib"
 authors = [
     "Wilko Henecka <wilkohenecka@gmx.net>",
     "Brian Thorne <brian@hardbyte.nz>"
 ]
 readme = "README.md"
 packages = [{include = "anonlinkclient"}]
@@ -39,22 +39,23 @@
 anonlink = 'anonlinkclient.cli:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 bashplotlib = "^0.6"
 blocklib = "^0.1.8"
 click = ">=7.1.2,<9.0.0"
-clkhash = "^0.17"
+clkhash = "^0.18.0"
 jsonschema = ">=3.2,<5.0"
 requests = "^2.25.1"
 retrying="^1.3.3"
 minio = "^7.0.3"
 ijson="^3.1.4"
 pydantic = "^1.10.5"
 jupyter = "^1.0.0"
+anonlink = "^0.15.2"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 jupyter = "^1.0.0"
@@ -66,14 +67,13 @@
 pytest = "^6.2.5"
 pytest-cov = "^4.0.0"
 pytest-timeout="^1.4.2"
 nbval="^0.9.6"
 mock="^4.0.2"
 mypy = "^0.982"
 twine = "^4.0.1"
-anonlink="^0.15"
 pre-commit = "^2.20.0"
 recordlinkage = "^0.15"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `anonlink_client-0.1.8/PKG-INFO` & `anonlink_client-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonlink-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client side tool for clkhash and blocklib
 Home-page: https://github.com/data61/anonlink-client
 License: Apache-2.0
 Author: Wilko Henecka
 Author-email: wilkohenecka@gmx.net
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,18 +21,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
+Requires-Dist: anonlink (>=0.15.2,<0.16.0)
 Requires-Dist: bashplotlib (>=0.6,<0.7)
 Requires-Dist: blocklib (>=0.1.8,<0.2.0)
 Requires-Dist: click (>=7.1.2,<9.0.0)
-Requires-Dist: clkhash (>=0.17,<0.18)
+Requires-Dist: clkhash (>=0.18.0,<0.19.0)
 Requires-Dist: ijson (>=3.1.4,<4.0.0)
 Requires-Dist: jsonschema (>=3.2,<5.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: minio (>=7.0.3,<8.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
```

