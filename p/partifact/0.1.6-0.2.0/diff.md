# Comparing `tmp/partifact-0.1.6.tar.gz` & `tmp/partifact-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partifact-0.1.6.tar", max compression
+gzip compressed data, was "partifact-0.2.0.tar", max compression
```

## Comparing `partifact-0.1.6.tar` & `partifact-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2021-11-10 09:35:16.513389 partifact-0.1.6/LICENSE
--rw-r--r--   0        0        0     2192 2023-04-24 18:59:12.451630 partifact-0.1.6/README.md
--rw-r--r--   0        0        0        0 2021-11-10 09:35:16.513765 partifact-0.1.6/partifact/__init__.py
--rw-r--r--   0        0        0     1450 2021-11-10 09:35:16.513940 partifact-0.1.6/partifact/auth_token.py
--rw-r--r--   0        0        0     3698 2023-04-24 18:55:45.224275 partifact-0.1.6/partifact/config.py
--rw-r--r--   0        0        0     1065 2021-11-10 09:35:16.514487 partifact-0.1.6/partifact/main.py
--rw-r--r--   0        0        0     2067 2021-11-10 09:35:16.514669 partifact-0.1.6/partifact/shell_commands.py
--rw-r--r--   0        0        0     1234 2023-04-24 18:58:35.107010 partifact-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 partifact-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-25 13:42:14.150572 partifact-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2192 2023-04-25 13:42:14.150572 partifact-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 13:42:14.150572 partifact-0.2.0/partifact/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-25 13:42:14.150572 partifact-0.2.0/partifact/auth_token.py
+-rw-r--r--   0        0        0     3698 2023-04-25 13:42:14.150572 partifact-0.2.0/partifact/config.py
+-rw-r--r--   0        0        0     1065 2023-04-25 13:42:14.150572 partifact-0.2.0/partifact/main.py
+-rw-r--r--   0        0        0     2067 2023-04-25 13:42:14.150572 partifact-0.2.0/partifact/shell_commands.py
+-rw-r--r--   0        0        0     1294 2023-04-25 13:42:14.150572 partifact-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 partifact-0.2.0/PKG-INFO
```

### Comparing `partifact-0.1.6/LICENSE` & `partifact-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/README.md` & `partifact-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/partifact/auth_token.py` & `partifact-0.2.0/partifact/auth_token.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/partifact/config.py` & `partifact-0.2.0/partifact/config.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/partifact/main.py` & `partifact-0.2.0/partifact/main.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/partifact/shell_commands.py` & `partifact-0.2.0/partifact/shell_commands.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.6/pyproject.toml` & `partifact-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "partifact"
-version = "0.1.6"
-description = ""
+version = "0.2.0"
+description = "CodeArtifact utilties for Poetry"
 authors = ["David Steiner <david_j_steiner@yahoo.co.nz>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Validus-Risk-Management/partifact"
 
 [tool.poetry.scripts]
 partifact = "partifact.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 boto3 = "^1.15"
 tomlkit = ">=0.7.0,<1.0.0"
-typer = "^0.3.2"
+typer = "^0.7.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^3.9.0"
 flake8-absolute-import = "^1.0"
 flake8-blind-except = "^0.2.0"
 flake8-breakpoint = "^1.1.0"
 flake8-bugbear = "^21.4.3"
 flake8-builtins = "^1.5.3"
@@ -34,16 +34,17 @@
 flake8-pytest-style = "^1.5.0"
 flake8-simplify = "^0.14.1"
 isort = "^5.12.0"
 mypy = "^0.910"
 pep8-naming = "^0.12.1"
 pre-commit = "^2.14.0"
 pyfakefs = "^4.5.0"
-pytest = "^6.2.4"
+pytest = "^7.2.0"
 pytest-mock = "^3.6.1"
+pytest-cov = "^4.0.0"
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 exclude = "tests/"
 
 [tool.isort]
```

### Comparing `partifact-0.1.6/PKG-INFO` & `partifact-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: partifact
-Version: 0.1.6
-Summary: 
+Version: 0.2.0
+Summary: CodeArtifact utilties for Poetry
 Home-page: https://github.com/Validus-Risk-Management/partifact
 License: MIT
 Author: David Steiner
 Author-email: david_j_steiner@yahoo.co.nz
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.15,<2.0)
 Requires-Dist: tomlkit (>=0.7.0,<1.0.0)
-Requires-Dist: typer (>=0.3.2,<0.4.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # partifact
 
 partifact is a tool to help with configuring and authenticating CodeArtifact as a repository for [Poetry](https://github.com/python-poetry/poetry) and [pip](https://pip.pypa.io/en/stable/).
 
 [AWS CLI](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/login.html) offers functionality to configure CodeArtifact for pip.
```

