# Comparing `tmp/hydev-1.2.0.tar.gz` & `tmp/hydev-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydev-1.2.0.tar", max compression
+gzip compressed data, was "hydev-1.3.0.tar", max compression
```

## Comparing `hydev-1.2.0.tar` & `hydev-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      252 2023-02-27 08:27:16.470934 hydev-1.2.0/LICENSE
--rw-r--r--   0        0        0     2503 2023-03-22 13:31:27.162653 hydev-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       35 2022-12-21 17:54:52.089197 hydev-1.2.0/src/hydev/__init__.py
--rw-r--r--   0        0        0     1779 2022-12-21 17:54:52.089197 hydev-1.2.0/src/hydev/common_pyproject.toml
--rw-r--r--   0        0        0     7535 2022-12-21 17:54:52.089197 hydev-1.2.0/src/hydev/main.py
--rw-r--r--   0        0        0     2920 2023-03-22 13:29:08.269945 hydev-1.2.0/src/hydev/utils.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 hydev-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2023-02-27 08:27:16.470934 hydev-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2501 2023-04-26 15:25:30.929894 hydev-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2022-12-21 17:54:52.089197 hydev-1.3.0/src/hydev/__init__.py
+-rw-r--r--   0        0        0     1779 2022-12-21 17:54:52.089197 hydev-1.3.0/src/hydev/common_pyproject.toml
+-rw-r--r--   0        0        0     7535 2022-12-21 17:54:52.089197 hydev-1.3.0/src/hydev/main.py
+-rw-r--r--   0        0        0     2920 2023-03-22 13:29:08.269945 hydev-1.3.0/src/hydev/utils.py
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 hydev-1.3.0/PKG-INFO
```

### Comparing `hydev-1.2.0/pyproject.toml` & `hydev-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydev"
-version = "1.2.0"
+version = "1.3.0"
 description = "Common tooling and configuration for pythonic development"
 authors = ["hoverhell <hoverhell@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 hydautoflake = "hydev.main:Autoflake.run_cli"
 hydblack = "hydev.main:Black.run_cli"
@@ -20,52 +20,52 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 # Libs
 click = "^8.1.3"
 pyyaml = "^6.0"
 toml = "^0.10.2"
 # Tooling
-poetry = "^1.4.1"
-pre-commit = "^3.2.0"
+poetry = "^1.4.2"
+pre-commit = "^3.2.2"
 # Debug conveniences
 coloredlogs = "^15.0.1"
 ipdb = "^0.13.13"
 # Formatting
 autoflake = "^1.7.8"
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
 # `flake8`
 flake8 = "^5.0.4"
 flake8-broken-line = "^0.6.0"
 flake8-debugger = "^4.1.2"
 flake8-mock-x2 = "^0.4.1"
 flake8-print = "^5.0.0"
 flake8-pytest-style = "^1.7.2"
 flake8-use-fstring = "^1.4"
 # `mypy`
-mypy = "^1.1.1"
+mypy = "^1.2.0"
 # `pytest`
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-blockage = "^0.2.4"
 pytest-cov = "^4.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-env = "^0.8.1"
 pytest-timeout = "^2.1.0"
 # `django`
 django-coverage-plugin = {version = "^3.0.0", optional = true}
-django-debug-toolbar = {version = "^3.8.1", optional = true}
+django-debug-toolbar = {version = "^4.0.0", optional = true}
 django-extra-checks = {version = "^0.13.3", optional = true}
 django-migration-linter = {version = "^4.1.0", optional = true}
 django-querycount = {version = "^0.8.3", optional = true}
 django-split-settings = {version = "^1.2.0", optional = true}
-django-stubs = {version = "^1.15.0", optional = true}
-django-stubs-ext = {version = "^0.7.0", optional = true}
+django-stubs = {version = "^1.16.0", optional = true}
+django-stubs-ext = {version = "^0.8.0", optional = true}
 django-test-migrations = {version = "^1.2.0", optional = true}
-flake8-django = {version = "^1.1.5", optional = true}
+flake8-django = {version = "^1.2", optional = true}
 pytest-django = {version = "^4.5.2", optional = true}
 # ...
 poetry-plugin-up = "^0.3.0"
 
 [tool.poetry.extras]
 django = [
   "django-coverage-plugin",
```

### Comparing `hydev-1.2.0/src/hydev/common_pyproject.toml` & `hydev-1.3.0/src/hydev/common_pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydev-1.2.0/src/hydev/main.py` & `hydev-1.3.0/src/hydev/main.py`

 * *Files identical despite different names*

### Comparing `hydev-1.2.0/src/hydev/utils.py` & `hydev-1.3.0/src/hydev/utils.py`

 * *Files identical despite different names*

### Comparing `hydev-1.2.0/PKG-INFO` & `hydev-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: hydev
-Version: 1.2.0
+Version: 1.3.0
 Summary: Common tooling and configuration for pythonic development
 License: MIT
 Author: hoverhell
 Author-email: hoverhell@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: django
 Requires-Dist: autoflake (>=1.7.8,<2.0.0)
-Requires-Dist: black (>=23.1.0,<24.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: django-coverage-plugin (>=3.0.0,<4.0.0) ; extra == "django"
-Requires-Dist: django-debug-toolbar (>=3.8.1,<4.0.0) ; extra == "django"
+Requires-Dist: django-debug-toolbar (>=4.0.0,<5.0.0) ; extra == "django"
 Requires-Dist: django-extra-checks (>=0.13.3,<0.14.0) ; extra == "django"
 Requires-Dist: django-migration-linter (>=4.1.0,<5.0.0) ; extra == "django"
 Requires-Dist: django-querycount (>=0.8.3,<0.9.0) ; extra == "django"
 Requires-Dist: django-split-settings (>=1.2.0,<2.0.0) ; extra == "django"
-Requires-Dist: django-stubs (>=1.15.0,<2.0.0) ; extra == "django"
-Requires-Dist: django-stubs-ext (>=0.7.0,<0.8.0) ; extra == "django"
+Requires-Dist: django-stubs (>=1.16.0,<2.0.0) ; extra == "django"
+Requires-Dist: django-stubs-ext (>=0.8.0,<0.9.0) ; extra == "django"
 Requires-Dist: django-test-migrations (>=1.2.0,<2.0.0) ; extra == "django"
 Requires-Dist: flake8 (>=5.0.4,<6.0.0)
 Requires-Dist: flake8-broken-line (>=0.6.0,<0.7.0)
 Requires-Dist: flake8-debugger (>=4.1.2,<5.0.0)
-Requires-Dist: flake8-django (>=1.1.5,<2.0.0) ; extra == "django"
+Requires-Dist: flake8-django (>=1.2,<2.0) ; extra == "django"
 Requires-Dist: flake8-mock-x2 (>=0.4.1,<0.5.0)
 Requires-Dist: flake8-print (>=5.0.0,<6.0.0)
 Requires-Dist: flake8-pytest-style (>=1.7.2,<2.0.0)
 Requires-Dist: flake8-use-fstring (>=1.4,<2.0)
 Requires-Dist: ipdb (>=0.13.13,<0.14.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
-Requires-Dist: mypy (>=1.1.1,<2.0.0)
-Requires-Dist: poetry (>=1.4.1,<2.0.0)
+Requires-Dist: mypy (>=1.2.0,<2.0.0)
+Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Requires-Dist: poetry-plugin-up (>=0.3.0,<0.4.0)
-Requires-Dist: pre-commit (>=3.2.0,<4.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
+Requires-Dist: pre-commit (>=3.2.2,<4.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: pytest-blockage (>=0.2.4,<0.3.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-deadfixtures (>=2.2.1,<3.0.0)
 Requires-Dist: pytest-django (>=4.5.2,<5.0.0) ; extra == "django"
 Requires-Dist: pytest-env (>=0.8.1,<0.9.0)
 Requires-Dist: pytest-timeout (>=2.1.0,<3.0.0)
```

