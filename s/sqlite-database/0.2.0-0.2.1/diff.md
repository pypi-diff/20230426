# Comparing `tmp/sqlite_database-0.2.0.tar.gz` & `tmp/sqlite_database-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_database-0.2.0.tar", last modified: Wed Apr 26 05:41:34 2023, max compression
+gzip compressed data, was "sqlite_database-0.2.1.tar", last modified: Wed Apr 26 06:19:30 2023, max compression
```

## Comparing `sqlite_database-0.2.0.tar` & `sqlite_database-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.005612 sqlite_database-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.001612 sqlite_database-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.001612 sqlite_database-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.001612 sqlite_database-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/Features.md
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/History.md
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-26 05:41:34.005612 sqlite_database-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/pylint.toml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-26 05:41:34.009611 sqlite_database-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.005612 sqlite_database-0.2.0/sqlite_database/
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/sqlite_database/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.005612 sqlite_database-0.2.0/sqlite_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-26 05:41:33.000000 sqlite_database-0.2.0/sqlite_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 05:41:33.000000 sqlite_database-0.2.0/sqlite_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:41:33.000000 sqlite_database-0.2.0/sqlite_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 05:41:33.000000 sqlite_database-0.2.0/sqlite_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:41:33.000000 sqlite_database-0.2.0/sqlite_database.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:34.005612 sqlite_database-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-26 05:41:17.000000 sqlite_database-0.2.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.013416 sqlite_database-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/Features.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/History.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/pylint.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/sqlite_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/sqlite_database/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/sqlite_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 06:19:30.000000 sqlite_database-0.2.1/sqlite_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:29.000000 sqlite_database-0.2.1/sqlite_database.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:30.017416 sqlite_database-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-04-26 06:19:12.000000 sqlite_database-0.2.1/tests/test_database.py
```

### Comparing `sqlite_database-0.2.0/.github/workflows/pylint.yml` & `sqlite_database-0.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/.github/workflows/python-app.yml` & `sqlite_database-0.2.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/.github/workflows/python-publish.yml` & `sqlite_database-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/.gitignore` & `sqlite_database-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/Features.md` & `sqlite_database-0.2.1/Features.md`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/History.md` & `sqlite_database-0.2.1/History.md`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/LICENSE` & `sqlite_database-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/PKG-INFO` & `sqlite_database-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlite_database
-Version: 0.2.0
+Version: 0.2.1
 Summary: A weird wrapper for SQLite Connection
-Home-page: https://github.com/RimuEirnarn/sqlite_wrapper
+Home-page: https://github.com/RimuEirnarn/sqlite_database
 Author: RimuEirnarn
 Author-email: rimuru720@proton.me
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/RimuEirnarn/sqlite_database
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `sqlite_database-0.2.0/README.md` & `sqlite_database-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/pylint.toml` & `sqlite_database-0.2.1/pylint.toml`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/setup.cfg` & `sqlite_database-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = sqlite_database
 version = attr: sqlite_database.__version__
 license_files = LICENSE
-url = https://github.com/RimuEirnarn/sqlite_wrapper
+url = https://github.com/RimuEirnarn/sqlite_database
 author = RimuEirnarn
 author_email = rimuru720@proton.me
 description = A weird wrapper for SQLite Connection
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Source Code = https://github.com/RimuEirnarn/sqlite_database
```

### Comparing `sqlite_database-0.2.0/sqlite_database/__init__.py` & `sqlite_database-0.2.1/sqlite_database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,10 +170,10 @@
 
     @property
     def sql(self):
         """SQL Connection"""
         return self._database
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __all__ = ["Database", "Table", "op",
            "Column", "null", 'AttrDict', 'text', 'integer', 'real', 'blob']
```

### Comparing `sqlite_database-0.2.0/sqlite_database/_debug.py` & `sqlite_database-0.2.1/sqlite_database/_debug.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/_utils.py` & `sqlite_database-0.2.1/sqlite_database/_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/column.py` & `sqlite_database-0.2.1/sqlite_database/column.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/csv.py` & `sqlite_database-0.2.1/sqlite_database/csv.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/errors.py` & `sqlite_database-0.2.1/sqlite_database/errors.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/locals.py` & `sqlite_database-0.2.1/sqlite_database/locals.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/operators.py` & `sqlite_database-0.2.1/sqlite_database/operators.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/query_builder.py` & `sqlite_database-0.2.1/sqlite_database/query_builder.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/signature.py` & `sqlite_database-0.2.1/sqlite_database/signature.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/table.py` & `sqlite_database-0.2.1/sqlite_database/table.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database/typings.py` & `sqlite_database-0.2.1/sqlite_database/typings.py`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/sqlite_database.egg-info/PKG-INFO` & `sqlite_database-0.2.1/sqlite_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlite-database
-Version: 0.2.0
+Version: 0.2.1
 Summary: A weird wrapper for SQLite Connection
-Home-page: https://github.com/RimuEirnarn/sqlite_wrapper
+Home-page: https://github.com/RimuEirnarn/sqlite_database
 Author: RimuEirnarn
 Author-email: rimuru720@proton.me
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/RimuEirnarn/sqlite_database
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `sqlite_database-0.2.0/sqlite_database.egg-info/SOURCES.txt` & `sqlite_database-0.2.1/sqlite_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlite_database-0.2.0/tests/test_database.py` & `sqlite_database-0.2.1/tests/test_database.py`

 * *Files identical despite different names*

