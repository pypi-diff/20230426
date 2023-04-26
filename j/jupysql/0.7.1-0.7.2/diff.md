# Comparing `tmp/jupysql-0.7.1.tar.gz` & `tmp/jupysql-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.1.tar", last modified: Wed Apr 19 17:09:32 2023, max compression
+gzip compressed data, was "jupysql-0.7.2.tar", last modified: Tue Apr 25 23:07:07 2023, max compression
```

## Comparing `jupysql-0.7.1.tar` & `jupysql-0.7.2.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.527426 jupysql-0.7.1/
--rw-r--r--   0 eduardo    (501) staff       (20)    11820 2023-03-30 15:02:40.000000 jupysql-0.7.1/LICENSE
--rw-r--r--   0 eduardo    (501) staff       (20)       52 2022-12-22 14:07:08.000000 jupysql-0.7.1/MANIFEST.in
--rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-19 17:09:32.527475 jupysql-0.7.1/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)     2354 2023-04-13 14:31:32.000000 jupysql-0.7.1/README.md
--rw-r--r--   0 eduardo    (501) staff       (20)      647 2023-04-12 23:36:02.000000 jupysql-0.7.1/pyproject.toml
--rw-r--r--   0 eduardo    (501) staff       (20)      120 2023-04-19 17:09:32.527664 jupysql-0.7.1/setup.cfg
--rw-r--r--   0 eduardo    (501) staff       (20)     2138 2023-04-19 17:04:46.000000 jupysql-0.7.1/setup.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.523170 jupysql-0.7.1/src/
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.524643 jupysql-0.7.1/src/jupysql.egg-info/
--rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)      796 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2022-12-22 14:07:34.000000 jupysql-0.7.1/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 eduardo    (501) staff       (20)      491 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        4 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.526406 jupysql-0.7.1/src/sql/
--rw-r--r--   0 eduardo    (501) staff       (20)      169 2023-04-19 17:09:29.000000 jupysql-0.7.1/src/sql/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)    10319 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/_testing.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2899 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/column_guesser.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2716 2023-04-12 23:36:02.000000 jupysql-0.7.1/src/sql/command.py
--rw-r--r--   0 eduardo    (501) staff       (20)    14312 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/connection.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.526866 jupysql-0.7.1/src/sql/ggplot/
--rw-r--r--   0 eduardo    (501) staff       (20)      248 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      446 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/aes.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1331 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.527320 jupysql-0.7.1/src/sql/ggplot/geom/
--rw-r--r--   0 eduardo    (501) staff       (20)      158 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      327 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 eduardo    (501) staff       (20)      463 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1060 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2412 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/ggplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     9231 2023-04-13 01:27:43.000000 jupysql-0.7.1/src/sql/inspect.py
--rw-r--r--   0 eduardo    (501) staff       (20)    14701 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/magic.py
--rw-r--r--   0 eduardo    (501) staff       (20)     8803 2023-04-19 17:04:46.000000 jupysql-0.7.1/src/sql/magic_cmd.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2516 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/magic_plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2923 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/parse.py
--rw-r--r--   0 eduardo    (501) staff       (20)    16880 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)    15767 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/run.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4868 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/store.py
--rw-r--r--   0 eduardo    (501) staff       (20)      326 2023-03-03 23:16:57.000000 jupysql-0.7.1/src/sql/telemetry.py
--rw-r--r--   0 eduardo    (501) staff       (20)     5096 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/util.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806642 jupysql-0.7.2/
+-rw-r--r--   0 eduardo    (501) staff       (20)    11820 2023-03-30 15:02:40.000000 jupysql-0.7.2/LICENSE
+-rw-r--r--   0 eduardo    (501) staff       (20)       52 2022-12-22 14:07:08.000000 jupysql-0.7.2/MANIFEST.in
+-rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-25 23:07:07.806695 jupysql-0.7.2/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)     2354 2023-04-13 14:31:32.000000 jupysql-0.7.2/README.md
+-rw-r--r--   0 eduardo    (501) staff       (20)      701 2023-04-21 22:29:05.000000 jupysql-0.7.2/pyproject.toml
+-rw-r--r--   0 eduardo    (501) staff       (20)      120 2023-04-25 23:07:07.806876 jupysql-0.7.2/setup.cfg
+-rw-r--r--   0 eduardo    (501) staff       (20)     2138 2023-04-19 17:04:46.000000 jupysql-0.7.2/setup.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.802612 jupysql-0.7.2/src/
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.803948 jupysql-0.7.2/src/jupysql.egg-info/
+-rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)      836 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        1 2022-12-22 14:07:34.000000 jupysql-0.7.2/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 eduardo    (501) staff       (20)      491 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        4 2023-04-25 23:07:07.000000 jupysql-0.7.2/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.805737 jupysql-0.7.2/src/sql/
+-rw-r--r--   0 eduardo    (501) staff       (20)      169 2023-04-25 23:07:06.000000 jupysql-0.7.2/src/sql/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      544 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/_patch.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    10319 2023-04-12 23:53:59.000000 jupysql-0.7.2/src/sql/_testing.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2899 2023-04-21 22:52:16.000000 jupysql-0.7.2/src/sql/column_guesser.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2963 2023-04-25 22:57:19.000000 jupysql-0.7.2/src/sql/command.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    17895 2023-04-25 22:57:19.000000 jupysql-0.7.2/src/sql/connection.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     1159 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/exceptions.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806131 jupysql-0.7.2/src/sql/ggplot/
+-rw-r--r--   0 eduardo    (501) staff       (20)      248 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      446 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/aes.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     1092 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-25 23:07:07.806533 jupysql-0.7.2/src/sql/ggplot/geom/
+-rw-r--r--   0 eduardo    (501) staff       (20)      158 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      327 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      463 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     1060 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2412 2023-03-30 15:02:40.000000 jupysql-0.7.2/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    10405 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/inspect.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    15400 2023-04-25 19:03:00.000000 jupysql-0.7.2/src/sql/magic.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     9161 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/magic_cmd.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2692 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/magic_plot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2923 2023-04-21 16:12:23.000000 jupysql-0.7.2/src/sql/parse.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    15764 2023-04-21 22:29:05.000000 jupysql-0.7.2/src/sql/plot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    16714 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/run.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     4949 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/store.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      326 2023-03-03 23:16:57.000000 jupysql-0.7.2/src/sql/telemetry.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     6923 2023-04-25 16:22:28.000000 jupysql-0.7.2/src/sql/util.py
```

### Comparing `jupysql-0.7.1/LICENSE` & `jupysql-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/PKG-INFO` & `jupysql-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.1
+Version: 0.7.2
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.1 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.2 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.1/README.md` & `jupysql-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/pyproject.toml` & `jupysql-0.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.pkgmt]
 github = "ploomber/jupysql"
 env_name = "jupysql"
 package_name = "sql"
 
 [tool.pkgmt.check_links]
 extensions = ["md", "rst", "py", "ipynb"]
-ignore_substrings = ["d37ci6vzurychx.cloudfront.net", "https://bornsql.ca", "binder.ploomber.io"]
+ignore_substrings = ["d37ci6vzurychx.cloudfront.net", "https://bornsql.ca", "binder.ploomber.io", "127.0.0.1", "http://localhost", "https://localhost"]
 
 [tool.nbqa.addopts]
 flake8 = [
     # notebooks allow non-top imports
     "--extend-ignore=E402",
     # jupysql notebooks might have "undefined name" errors
     # due to the << operator
```

### Comparing `jupysql-0.7.1/setup.py` & `jupysql-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.2/src/jupysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.1
+Version: 0.7.2
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.1 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.2 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.1/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.2/src/jupysql.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 src/jupysql.egg-info/PKG-INFO
 src/jupysql.egg-info/SOURCES.txt
 src/jupysql.egg-info/dependency_links.txt
 src/jupysql.egg-info/not-zip-safe
 src/jupysql.egg-info/requires.txt
 src/jupysql.egg-info/top_level.txt
 src/sql/__init__.py
+src/sql/_patch.py
 src/sql/_testing.py
 src/sql/column_guesser.py
 src/sql/command.py
 src/sql/connection.py
+src/sql/exceptions.py
 src/sql/inspect.py
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
 src/sql/plot.py
 src/sql/run.py
```

### Comparing `jupysql-0.7.1/src/sql/_testing.py` & `jupysql-0.7.2/src/sql/_testing.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/sql/column_guesser.py` & `jupysql-0.7.2/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/sql/command.py` & `jupysql-0.7.2/src/sql/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,26 @@
 
     def __init__(self, magic, user_ns, line, cell) -> None:
         self.args = parse.magic_args(magic.execute, line)
         # self.args.line (everything that appears after %sql/%%sql in the first line)
         # is splited in tokens (delimited by spaces), this checks if we have one arg
         one_arg = len(self.args.line) == 1
 
+        is_custom_connection_ = (
+            Connection.is_custom_connection(user_ns.get(self.args.line[0], False))
+            if len(self.args.line) > 0
+            else False
+        )
+
         if (
             one_arg
             and self.args.line[0] in user_ns
-            and isinstance(user_ns[self.args.line[0]], Engine)
+            and (
+                isinstance(user_ns[self.args.line[0]], Engine) or is_custom_connection_
+            )
         ):
             line_for_command = []
             add_conn = True
         else:
             line_for_command = self.args.line
             add_conn = False
```

### Comparing `jupysql-0.7.1/src/sql/connection.py` & `jupysql-0.7.2/src/sql/connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import sqlalchemy
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import NoSuchModuleError
 from IPython.core.error import UsageError
 import difflib
 import sqlglot
 
+from sql.store import store
+from sql.telemetry import telemetry
+from sql import exceptions
+
 PLOOMBER_SUPPORT_LINK_STR = (
     "For technical support: https://ploomber.io/community"
     "\nDocumentation: https://jupysql.ploomber.io/en/latest/connecting.html"
 )
 IS_SQLALCHEMY_ONE = int(sqlalchemy.__version__.split(".")[0]) == 1
 
 # Check Full List: https://docs.sqlalchemy.org/en/20/dialects
@@ -188,18 +192,14 @@
     @classmethod
     def _error_invalid_connection_info(cls, e, connect_str):
         return UsageError(
             "An error happened while creating the connection: "
             f"{e}.{cls._suggest_fix(env_var=False, connect_str=connect_str)}"
         )
 
-    @classmethod
-    def _error_module_not_found(cls, e):
-        return ModuleNotFoundError("test")
-
     def __init__(self, engine, alias=None):
         self.url = engine.url
         self.name = self.assign_name(engine)
         self.dialect = self.url.get_dialect()
         self.session = engine.connect()
 
         if IS_SQLALCHEMY_ONE:
@@ -235,15 +235,15 @@
             else:
                 engine = sqlalchemy.create_engine(
                     connect_str,
                     connect_args=connect_args,
                 )
         except (ModuleNotFoundError, NoSuchModuleError) as e:
             suggestion_str = get_missing_package_suggestion_str(e)
-            raise UsageError(
+            raise exceptions.MissingPackageError(
                 "\n\n".join(
                     [
                         str(e),
                         suggestion_str,
                         PLOOMBER_SUPPORT_LINK_STR,
                     ]
                 )
@@ -261,18 +261,22 @@
         """
         Set the current database connection. This method is called from the magic to
         determine which connection to use (either use an existing one or open a new one)
         """
         connect_args = connect_args or {}
 
         if descriptor:
+            is_custom_connection_ = Connection.is_custom_connection(descriptor)
+
             if isinstance(descriptor, Connection):
                 cls.current = descriptor
             elif isinstance(descriptor, Engine):
                 cls.current = Connection(descriptor)
+            elif is_custom_connection_:
+                cls.current = CustomConnection(descriptor, alias=alias)
             else:
                 existing = rough_dict_get(cls.connections, descriptor)
 
                 # NOTE: I added one indentation level, otherwise
                 # the "existing" variable would not exist if
                 # passing an engine object as descriptor.
                 # Since I never saw this breaking, my guess
@@ -310,15 +314,19 @@
 
     @classmethod
     def connection_list(cls):
         """Returns the list of connections, appending '*' to the current one"""
         result = []
         for key in sorted(cls.connections):
             conn = cls.connections[key]
-            engine_url = conn.metadata.bind.url if IS_SQLALCHEMY_ONE else conn.url
+
+            if cls.is_custom_connection(conn):
+                engine_url = conn.url
+            else:
+                engine_url = conn.metadata.bind.url if IS_SQLALCHEMY_ONE else conn.url
 
             prefix = "* " if conn == cls.current else "  "
 
             if conn.alias:
                 repr_ = f"{prefix} ({conn.alias}) {engine_url!r}"
             else:
                 repr_ = f"{prefix} {engine_url!r}"
@@ -332,41 +340,74 @@
         if isinstance(descriptor, Connection):
             conn = descriptor
         else:
             conn = cls.connections.get(descriptor) or cls.connections.get(
                 descriptor.lower()
             )
         if not conn:
-            raise Exception(
+            raise exceptions.RuntimeError(
                 "Could not close connection because it was not found amongst these: %s"
-                % str(cls.connections.keys())
+                % str(list(cls.connections.keys()))
             )
 
         if descriptor in cls.connections:
             cls.connections.pop(descriptor)
         else:
             cls.connections.pop(
                 str(conn.metadata.bind.url) if IS_SQLALCHEMY_ONE else str(conn.url)
             )
             conn.session.close()
 
+    def is_custom_connection(conn=None) -> bool:
+        """
+        Checks if given connection is custom
+        """
+        is_custom_connection_ = False
+
+        if conn is None:
+            if not Connection.current:
+                raise exceptions.RuntimeError("No active connection")
+            else:
+                conn = Connection.current.session
+
+        if isinstance(conn, (CustomConnection, CustomSession)):
+            is_custom_connection_ = True
+        else:
+            # TODO: Better check when user passes a custom
+            # connection
+            if (
+                isinstance(
+                    conn, (sqlalchemy.engine.base.Connection, Connection, str, bool)
+                )
+                or conn.__class__.__name__ == "DataFrame"
+            ):
+                is_custom_connection_ = False
+            else:
+                is_custom_connection_ = True
+
+        return is_custom_connection_
+
     def _get_curr_sqlalchemy_connection_info(self):
         """Get the dialect, driver, and database server version info of current
         connected dialect
 
         Returns
         -------
         dict
             The dictionary which contains the SQLAlchemy-based dialect
             information, or None if there is no current connection.
         """
 
         if not self.session:
             return None
-        engine = self.metadata.bind if IS_SQLALCHEMY_ONE else self.session
+
+        try:
+            engine = self.metadata.bind if IS_SQLALCHEMY_ONE else self.session
+        except Exception:
+            engine = self.session
 
         return {
             "dialect": getattr(engine.dialect, "name", None),
             "driver": getattr(engine.dialect, "driver", None),
             "server_version_info": getattr(engine.dialect, "server_version_info", None),
         }
 
@@ -419,14 +460,17 @@
                 identifiers_ = sqlglot.Dialect.get_or_raise(
                     cur_dialect
                 ).Tokenizer.IDENTIFIERS
 
                 identifiers = [*set(identifiers + identifiers_)]
         except ValueError:
             pass
+        except AttributeError:
+            # this might be a custom connection..
+            pass
 
         return identifiers
 
     def _transpile_query(self, query):
         """Translate the given SQL clause that's compatible to current connected
         dialect by sqlglot
 
@@ -441,7 +485,88 @@
             SQL clause that's compatible to current connected dialect
         """
         write_dialect = self._get_curr_sqlglot_dialect()
         try:
             query = sqlglot.parse_one(query).sql(dialect=write_dialect)
         finally:
             return query
+
+    def _prepare_query(self, query, with_=None) -> str:
+        """
+        Returns a textual representation of a query based
+        on the current connection
+
+        Parameters
+        ----------
+        query : str
+            SQL query
+
+        with_ : string, default None
+            The key to use in with sql clause
+        """
+        if with_:
+            query = str(store.render(query, with_=with_))
+
+        query = self._transpile_query(query)
+
+        if self.is_custom_connection():
+            query = str(query)
+        else:
+            query = sqlalchemy.sql.text(query)
+
+        return query
+
+    def execute(self, query, with_=None):
+        """
+        Executes SQL query on a given connection
+        """
+        query = self._prepare_query(query, with_)
+        return self.session.execute(query)
+
+
+class CustomSession(sqlalchemy.engine.base.Connection):
+    """
+    Custom sql alchemy session
+    """
+
+    def __init__(self, connection, engine):
+        self.engine = engine
+        self.dialect = dict(
+            {
+                "name": connection.dialect,
+                "driver": connection.dialect,
+                "server_version_info": connection.dialect,
+            }
+        )
+
+    def execute(self, query):
+        cur = self.engine.cursor()
+        cur.execute(query)
+        return cur
+
+
+class CustomConnection(Connection):
+    """
+    Custom connection for unsupported drivers in sqlalchemy
+    """
+
+    @telemetry.log_call("CustomConnection", payload=True)
+    def __init__(self, payload, engine=None, alias=None):
+        try:
+            payload["engine"] = type(engine)
+        except Exception as e:
+            payload["engine_parsing_error"] = str(e)
+
+        if engine is None:
+            raise ValueError("Engine cannot be None")
+
+        connection_name_ = "custom_driver"
+        self.url = str(engine)
+        self.name = connection_name_
+        self.dialect = connection_name_
+        self.session = CustomSession(self, engine)
+
+        self.connections[alias or connection_name_] = self
+
+        self.connect_args = None
+        self.alias = alias
+        Connection.current = self
```

### Comparing `jupysql-0.7.1/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.2/src/sql/ggplot/facet_wrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 from jinja2 import Template
 import math
 import sql.connection
-from sql.store import store
 from sql.telemetry import telemetry
-import sqlalchemy
-
-
-def _run_query(query, with_=None, conn=None):
-    if not conn:
-        conn = sql.connection.Connection.current.session
-
-    if with_:
-        query = str(store.render(query, with_=with_))
-
-    return conn.execute(sqlalchemy.text(query)).fetchall()
 
 
 class facet:
     def __init__():
         pass
 
     def get_facet_values(self, table, column, with_):
@@ -25,15 +13,18 @@
             """
             SELECT
             distinct ({{column}})
             FROM "{{table}}"
             """
         )
         query = template.render(table=table, column=column)
-        values = _run_query(query, with_=with_)
+
+        conn = sql.connection.Connection.current
+
+        values = conn.execute(query, with_).fetchall()
         n_plots = len(values)
         n_cols = len(values) if len(values) < 3 else 3
         n_rows = math.ceil(n_plots / n_cols)
         return values, n_rows, n_cols
 
 
 class facet_wrap(facet):
```

### Comparing `jupysql-0.7.1/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.2/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/sql/ggplot/ggplot.py` & `jupysql-0.7.2/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/sql/inspect.py` & `jupysql-0.7.2/src/sql/inspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from sqlalchemy import inspect
 from prettytable import PrettyTable
 from ploomber_core.exceptions import modify_exceptions
 from sql.connection import Connection
 from sql.telemetry import telemetry
+from sql import exceptions
 import sql.run
 import math
 from sql import util
+from IPython.core.display import HTML
 
 
 def _get_inspector(conn):
     if conn:
         return inspect(conn)
 
     if not Connection.current:
-        raise RuntimeError("No active connection")
+        raise exceptions.RuntimeError("No active connection")
     else:
         return inspect(Connection.current.session)
 
 
 class DatabaseInspection:
     def __repr__(self) -> str:
         return self._table_txt
@@ -132,31 +134,36 @@
 
     def __init__(self, table_name, schema=None) -> None:
         util.is_table_exists(table_name, schema)
 
         if schema:
             table_name = f"{schema}.{table_name}"
 
-        columns = sql.run.raw_run(
+        columns_query_result = sql.run.raw_run(
             Connection.current, f"SELECT * FROM {table_name} WHERE 1=0"
-        ).keys()
+        )
+
+        if Connection.is_custom_connection():
+            columns = [i[0] for i in columns_query_result.description]
+        else:
+            columns = columns_query_result.keys()
 
         table_stats = dict({})
         columns_to_include_in_report = set()
 
         for column in columns:
             table_stats[column] = dict()
 
             # Note: index is reserved word in sqlite
             try:
                 result_col_freq_values = sql.run.raw_run(
                     Connection.current,
                     f"""SELECT DISTINCT {column} as top,
                     COUNT({column}) as frequency FROM {table_name}
-                    GROUP BY {column} ORDER BY Count({column}) Desc""",
+                    GROUP BY top ORDER BY frequency Desc""",
                 ).fetchall()
 
                 table_stats[column]["freq"] = result_col_freq_values[0][1]
                 table_stats[column]["top"] = result_col_freq_values[0][0]
 
                 columns_to_include_in_report.update(["freq", "top"])
 
@@ -166,27 +173,43 @@
             try:
                 # get all non None values, min, max and avg.
                 result_value_values = sql.run.raw_run(
                     Connection.current,
                     f"""
                     SELECT MIN({column}) AS min,
                     MAX({column}) AS max,
-                    COUNT(DISTINCT {column}) AS unique_count,
                     COUNT({column}) AS count
                     FROM {table_name}
                     WHERE {column} IS NOT NULL
                     """,
                 ).fetchall()
 
                 table_stats[column]["min"] = result_value_values[0][0]
                 table_stats[column]["max"] = result_value_values[0][1]
-                table_stats[column]["unique"] = result_value_values[0][2]
-                table_stats[column]["count"] = result_value_values[0][3]
+                table_stats[column]["count"] = result_value_values[0][2]
 
-                columns_to_include_in_report.update(["count", "unique", "min", "max"])
+                columns_to_include_in_report.update(["count", "min", "max"])
+
+            except Exception:
+                pass
+
+            try:
+                # get unique values
+                result_value_values = sql.run.raw_run(
+                    Connection.current,
+                    f"""
+                    SELECT
+                    COUNT(DISTINCT {column}) AS unique_count
+                    FROM {table_name}
+                    WHERE {column} IS NOT NULL
+                    """,
+                ).fetchall()
+                table_stats[column]["unique"] = result_value_values[0][0]
+
+                columns_to_include_in_report.update(["unique"])
 
             except Exception:
                 pass
 
             try:
                 results_avg = sql.run.raw_run(
                     Connection.current,
@@ -258,15 +281,32 @@
                 else:
                     value = ""
                 value = util.convert_to_scientific(value)
                 values.append(value)
 
             self._table.add_row(values)
 
-        self._table_html = self._table.get_html_string()
+        # Inject css to html to make first column sticky
+        sticky_column_css = """<style>
+ #profile-table td:first-child {
+  position: sticky;
+  left: 0;
+  background-color: var(--jp-cell-editor-background);
+}
+ #profile-table thead tr th:first-child {
+  position: sticky;
+  left: 0;
+  background-color: var(--jp-cell-editor-background);
+}
+            </style>"""
+        self._table_html = HTML(
+            sticky_column_css
+            + self._table.get_html_string(attributes={"id": "profile-table"})
+        ).__html__()
+
         self._table_txt = self._table.get_string()
 
 
 @telemetry.log_call()
 def get_table_names(schema=None):
     """Get table names for a given connection"""
     return Tables(schema)
```

### Comparing `jupysql-0.7.1/src/sql/magic.py` & `jupysql-0.7.2/src/sql/magic.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from sqlalchemy.exc import OperationalError, ProgrammingError, DatabaseError
 
 import warnings
 import sql.connection
 import sql.parse
 import sql.run
+from sql import exceptions
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
+from sql._patch import patch_ipython_usage_error
 from ploomber_core.dependencies import check_installed
 
 from traitlets.config.configurable import Configurable
 from traitlets import Bool, Int, Unicode, Dict, observe
 
 try:
     from pandas.core.frame import DataFrame, Series
-except ImportError:
+except ModuleNotFoundError:
     DataFrame = None
     Series = None
 
 from sql.telemetry import telemetry
 
 SUPPORT_INTERACTIVE_WIDGETS = ["Checkbox", "Text", "IntSlider", ""]
 
@@ -287,14 +289,15 @@
         user_ns = self.shell.user_ns.copy()
         user_ns.update(local_ns)
 
         command = SQLCommand(self, user_ns, line, cell)
         # args.line: contains the line after the magic with all options removed
 
         args = command.args
+
         # Create the interactive slider
         if args.interact and not is_interactive_mode:
             check_installed(["ipywidgets"], "--interactive argument")
             interactive_dict = {}
             for key in args.interact:
                 interactive_dict[key] = local_ns[key]
             print(
@@ -414,35 +417,59 @@
 
     legal_sql_identifier = re.compile(r"^[A-Za-z0-9#_$]+")
 
     @modify_exceptions
     def _persist_dataframe(self, raw, conn, user_ns, append=False, index=True):
         """Implements PERSIST, which writes a DataFrame to the RDBMS"""
         if not DataFrame:
-            raise ImportError("Must `pip install pandas` to use DataFrames")
+            raise exceptions.MissingPackageError(
+                "You must install pandas to persist results: pip install pandas"
+            )
 
         frame_name = raw.strip(";")
 
-        # Get the DataFrame from the user namespace
+        # invalid identifier
+        if not frame_name.isidentifier():
+            raise exceptions.UsageError(
+                f"Expected {frame_name!r} to be a pd.DataFrame but it's"
+                " not a valid identifier"
+            )
+
+        # missing argument
         if not frame_name:
-            raise SyntaxError("Syntax: %sql --persist <name_of_data_frame>")
-        try:
-            frame = eval(frame_name, user_ns)
-        except SyntaxError:
-            raise SyntaxError("Syntax: %sql --persist <name_of_data_frame>")
+            raise exceptions.UsageError(
+                "Missing argument: %sql --persist <name_of_data_frame>"
+            )
+
+        # undefined variable
+        if frame_name not in user_ns:
+            raise exceptions.UsageError(
+                f"Expected {frame_name!r} to be a pd.DataFrame but it's undefined"
+            )
+
+        frame = user_ns[frame_name]
+
         if not isinstance(frame, DataFrame) and not isinstance(frame, Series):
-            raise TypeError("%s is not a Pandas DataFrame or Series" % frame_name)
+            raise exceptions.TypeError(
+                f"{frame_name!r} is not a Pandas DataFrame or Series"
+            )
 
         # Make a suitable name for the resulting database table
         table_name = frame_name.lower()
         table_name = self.legal_sql_identifier.search(table_name).group(0)
 
         if_exists = "append" if append else "fail"
 
-        frame.to_sql(table_name, conn.session.engine, if_exists=if_exists, index=index)
+        try:
+            frame.to_sql(
+                table_name, conn.session.engine, if_exists=if_exists, index=index
+            )
+        except ValueError as e:
+            raise exceptions.ValueError(e) from e
+
         return "Persisted %s" % table_name
 
 
 def load_ipython_extension(ip):
     """Load the extension in IPython."""
 
     # this fails in both Firefox and Chrome for OS X.
@@ -451,9 +478,8 @@
     # js = "IPython.CodeCell.config_defaults.highlight_modes['magic_sql'] = {'reg':[/^%%sql/]};" # noqa
     # display_javascript(js, raw=True)
     ip.register_magics(SqlMagic)
     ip.register_magics(RenderMagic)
     ip.register_magics(SqlPlotMagic)
     ip.register_magics(SqlCmdMagic)
 
-
-# %%
+    patch_ipython_usage_error(ip)
```

### Comparing `jupysql-0.7.1/src/sql/magic_cmd.py` & `jupysql-0.7.2/src/sql/magic_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import sys
 import argparse
 
 from IPython.utils.process import arg_split
 from IPython.core.magic import Magics, line_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments
-from IPython.core.error import UsageError
 from sqlglot import select, condition
 from sqlalchemy import text
+from sql import util
 
 from prettytable import PrettyTable
 
 try:
     from traitlets.config.configurable import Configurable
-except ImportError:
+except ModuleNotFoundError:
     from IPython.config.configurable import Configurable
 
 import sql.connection
 from sql import inspect
 import sql.run
+from sql.util import sanitize_identifier
+from sql import exceptions
 
 
 class CmdParser(argparse.ArgumentParser):
     def exit(self, status=0, message=None):
         if message:
             self._print_message(message, sys.stderr)
 
     def error(self, message):
-        raise UsageError(message)
+        raise exceptions.UsageError(message)
 
 
 @magics_class
 class SqlCmdMagic(Magics, Configurable):
     """%sqlcmd magic"""
 
     @line_magic("sqlcmd")
@@ -38,42 +40,44 @@
     @argument("line", type=str, help="Command name")
     def _validate_execute_inputs(self, line):
         """
         Function to validate %sqlcmd inputs.
         Raises UsageError in case of an invalid input, executes command otherwise.
         """
 
+        # We relly on SQLAlchemy when inspecting tables
+        util.support_only_sql_alchemy_connection("%sqlcmd")
+
         AVAILABLE_SQLCMD_COMMANDS = ["tables", "columns", "test", "profile"]
 
         if line == "":
-            raise UsageError(
+            raise exceptions.UsageError(
                 "Missing argument for %sqlcmd. "
                 "Valid commands are: {}".format(", ".join(AVAILABLE_SQLCMD_COMMANDS))
             )
         else:
             split = arg_split(line)
             command, others = split[0].strip(), split[1:]
 
             if command in AVAILABLE_SQLCMD_COMMANDS:
                 return self.execute(command, others)
             else:
-                raise UsageError(
+                raise exceptions.UsageError(
                     f"%sqlcmd has no command: {command!r}. "
                     "Valid commands are: {}".format(
                         ", ".join(AVAILABLE_SQLCMD_COMMANDS)
                     )
                 )
 
     @argument("cmd_name", default="", type=str, help="Command name")
     @argument("others", default="", type=str, help="Other tags")
     def execute(self, cmd_name="", others="", cell="", local_ns=None):
         """
         Command
         """
-
         if cmd_name == "tables":
             parser = CmdParser()
 
             parser.add_argument(
                 "-s", "--schema", type=str, help="Schema name", required=False
             )
 
@@ -87,15 +91,17 @@
                 "-t", "--table", type=str, help="Table name", required=True
             )
             parser.add_argument(
                 "-s", "--schema", type=str, help="Schema name", required=False
             )
 
             args = parser.parse_args(others)
-            return inspect.get_columns(name=args.table, schema=args.schema)
+            return inspect.get_columns(
+                name=sanitize_identifier(args.table), schema=args.schema
+            )
         elif cmd_name == "test":
             parser = CmdParser()
 
             parser.add_argument(
                 "-t", "--table", type=str, help="Table name", required=True
             )
             parser.add_argument(
@@ -142,26 +148,26 @@
                 args.greater,
                 args.greater_or_equal,
                 args.less_than,
                 args.less_than_or_equal,
             ]
 
             if args.table and not any(COMPARATOR_ARGS):
-                raise UsageError("Please use a valid comparator.")
+                raise exceptions.UsageError("Please use a valid comparator.")
 
             if args.table and any(COMPARATOR_ARGS) and not args.column:
-                raise UsageError("Please pass a column to test.")
+                raise exceptions.UsageError("Please pass a column to test.")
 
             if args.greater and args.greater_or_equal:
-                return ValueError(
+                return exceptions.UsageError(
                     "You cannot use both greater and greater "
                     "than or equal to arguments at the same time."
                 )
             elif args.less_than and args.less_than_or_equal:
-                return ValueError(
+                return exceptions.UsageError(
                     "You cannot use both less and less than "
                     "or equal to arguments at the same time."
                 )
 
             conn = sql.connection.Connection.current.session
             result_dict = run_each_individually(args, conn)
 
@@ -170,15 +176,15 @@
                     if len(rows) > 1:
                         print(f"\n{comparator}:\n")
                         _pretty = PrettyTable()
                         _pretty.field_names = rows[0]
                         for row in rows[1:]:
                             _pretty.add_row(row)
                         print(_pretty)
-                raise UsageError(
+                raise exceptions.UsageError(
                     "The above values do not not match your test requirements."
                 )
             else:
                 return True
 
         elif cmd_name == "profile":
             parser = CmdParser()
@@ -212,15 +218,17 @@
         res = conn.execute(text(query)).fetchall()
         for column in column_data:
             columns.append(column[0])
         res = [columns, *res]
         return res
     except Exception as e:
         if "column" in str(e):
-            raise UsageError(f"Referenced column '{args.column}' not found!")
+            raise exceptions.UsageError(
+                f"Referenced column '{args.column}' not found!"
+            ) from e
 
 
 def run_each_individually(args, conn):
     base_query = select("*").from_(args.table)
 
     storage = {}
```

### Comparing `jupysql-0.7.1/src/sql/magic_plot.py` & `jupysql-0.7.2/src/sql/magic_plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     magics_class,
 )
 from IPython.core.magic_arguments import argument, magic_arguments
 from ploomber_core.exceptions import modify_exceptions
 
 try:
     from traitlets.config.configurable import Configurable
-except ImportError:
+except ModuleNotFoundError:
     from IPython.config.configurable import Configurable
 
 
 from sql import plot
 from sql.command import SQLPlotCommand
+from sql import exceptions
 from sql import util
 
 
 @magics_class
 class SqlPlotMagic(Magics, Configurable):
     """%sqlplot magic"""
 
@@ -60,35 +61,38 @@
 
         if len(cmd.args.column) == 1:
             column = cmd.args.column[0]
         else:
             column = cmd.args.column
 
         if not cmd.args.line:
-            raise ValueError(
-                "Missing the first argument, must be: 'histogram' or 'boxplot'"
+            raise exceptions.UsageError(
+                "Missing the first argument, must be: 'histogram' or 'boxplot'. "
+                "Example: %sqlplot histogram"
             )
 
-        if cmd.args.line[0] in {"box", "boxplot"}:
-            util.is_table_exists(cmd.args.table, with_=cmd.args.with_)
+        column = util.sanitize_identifier(column)
+        table = util.sanitize_identifier(cmd.args.table)
 
+        if cmd.args.line[0] in {"box", "boxplot"}:
+            util.is_table_exists(table, with_=cmd.args.with_)
             return plot.boxplot(
-                table=cmd.args.table,
+                table=table,
                 column=column,
                 with_=cmd.args.with_,
                 orient=cmd.args.orient,
                 conn=None,
             )
         elif cmd.args.line[0] in {"hist", "histogram"}:
-            util.is_table_exists(cmd.args.table, with_=cmd.args.with_)
+            util.is_table_exists(table, with_=cmd.args.with_)
 
             return plot.histogram(
-                table=cmd.args.table,
+                table=table,
                 column=column,
                 bins=cmd.args.bins,
                 with_=cmd.args.with_,
                 conn=None,
             )
         else:
-            raise ValueError(
+            raise exceptions.UsageError(
                 f"Unknown plot {cmd.args.line[0]!r}. Must be: 'histogram' or 'boxplot'"
             )
```

### Comparing `jupysql-0.7.1/src/sql/parse.py` & `jupysql-0.7.2/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.1/src/sql/plot.py` & `jupysql-0.7.2/src/sql/plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 """
 Plot using the SQL backend
 """
 from ploomber_core.dependencies import requires
 from ploomber_core.exceptions import modify_exceptions
 from jinja2 import Template
-import sqlalchemy
+
+from sql.util import flatten
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.colors import Normalize
 except ModuleNotFoundError:
     plt = None
     Normalize = None
 
 try:
     import numpy as np
 except ModuleNotFoundError:
     np = None
 
-from sql.store import store
 import sql.connection
 from sql.telemetry import telemetry
 import warnings
+from sql import util
 
 
 def _summary_stats(conn, table, column, with_=None):
+    """Compute percentiles and mean for boxplot"""
+
     if not conn:
         conn = sql.connection.Connection.current
-    """Compute percentiles and mean for boxplot"""
+
     template = Template(
         """
-SELECT
-percentile_disc(0.25) WITHIN GROUP (ORDER BY "{{column}}") AS q1,
-percentile_disc(0.50) WITHIN GROUP (ORDER BY "{{column}}") AS med,
-percentile_disc(0.75) WITHIN GROUP (ORDER BY "{{column}}") AS q3,
-AVG("{{column}}") AS mean,
-COUNT(*) AS N
-FROM "{{table}}"
+    SELECT
+    percentile_disc([0.25, 0.50, 0.75]) WITHIN GROUP \
+    (ORDER BY "{{column}}") AS percentiles,
+    AVG("{{column}}") AS mean,
+    COUNT(*) AS N
+    FROM "{{table}}"
 """
     )
-    query = template.render(table=table, column=column)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
+    query = template.render(table=table, column=column)
 
-    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
+    values = conn.execute(query, with_).fetchone()
     keys = ["q1", "med", "q3", "mean", "N"]
-    return {k: float(v) for k, v in zip(keys, values)}
+    return {k: float(v) for k, v in zip(keys, flatten(values))}
 
 
 def _whishi(conn, table, column, hival, with_=None):
     if not conn:
         conn = sql.connection.Connection.current
     template = Template(
         """
@@ -61,18 +61,15 @@
     WHERE "{{column}}" <= {{hival}}
 ) AS _whishi
 """
     )
 
     query = template.render(table=table, column=column, hival=hival)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-    query = conn._transpile_query(query)
-    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
+    values = conn.execute(query, with_).fetchone()
     keys = ["N", "wiskhi_max"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
 def _whislo(conn, table, column, loval, with_=None):
     if not conn:
         conn = sql.connection.Connection.current
@@ -85,18 +82,15 @@
     WHERE "{{column}}" >= {{loval}}
 ) AS _whislo
 """
     )
 
     query = template.render(table=table, column=column, loval=loval)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-    query = conn._transpile_query(query)
-    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
+    values = conn.execute(query, with_).fetchone()
     keys = ["N", "wisklo_min"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
 def _percentile(conn, table, column, pct, with_=None):
     if not conn:
         conn = sql.connection.Connection.current.session
@@ -105,47 +99,42 @@
 SELECT
 percentile_disc({{pct}}) WITHIN GROUP (ORDER BY "{{column}}") AS pct,
 FROM "{{table}}"
 """
     )
     query = template.render(table=table, column=column, pct=pct)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-    query = conn._transpile_query(query)
-    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()[0]
+    values = conn.execute(query, with_).fetchone()[0]
     return values
 
 
 def _between(conn, table, column, whislo, whishi, with_=None):
     template = Template(
         """
 SELECT "{{column}}"
 FROM "{{table}}"
 WHERE "{{column}}" < {{whislo}}
 OR  "{{column}}" > {{whishi}}
 """
     )
     query = template.render(table=table, column=column, whislo=whislo, whishi=whishi)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-    query = conn._transpile_query(query)
-    results = [
-        float(n[0]) for n in conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
-    ]
+    results = [float(n[0]) for n in conn.execute(query, with_).fetchall()]
     return results
 
 
 # https://github.com/matplotlib/matplotlib/blob/b5ac96a8980fdb9e59c9fb649e0714d776e26701/lib/matplotlib/cbook/__init__.py
 @modify_exceptions
 def _boxplot_stats(conn, table, column, whis=1.5, autorange=False, with_=None):
+    """Compute statistics required to create a boxplot"""
     if not conn:
         conn = sql.connection.Connection.current
-    """Compute statistics required to create a boxplot"""
+
+    # calculating stats might fail on other DBs (percentile_disc)
+    util.support_only_sql_alchemy_connection("boxplot")
 
     def _compute_conf_interval(N, med, iqr):
         notch_min = med - 1.57 * iqr / np.sqrt(N)
         notch_max = med + 1.57 * iqr / np.sqrt(N)
 
         return notch_min, notch_max
 
@@ -293,18 +282,15 @@
 """
     if use_backticks:
         template_ = template_.replace('"', "`")
 
     template = Template(template_)
     query = template.render(table=table, column=column)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-    query = con._transpile_query(query)
-    min_, max_ = con.session.execute(sqlalchemy.sql.text(query)).fetchone()
+    min_, max_ = con.execute(query, with_).fetchone()
     return min_, max_
 
 
 def _are_numeric_values(*values):
     return all([isinstance(value, (int, float)) for value in values])
 
 
@@ -377,15 +363,14 @@
     **Plot multiple columns from the same table**:
 
     .. plot:: ../examples/plot_histogram_many.py
     """
     if not conn:
         conn = sql.connection.Connection.current
 
-    print("Current conn: ", conn)
     ax = ax or plt.gca()
     payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
     if category:
         if isinstance(column, list):
             if len(column) > 1:
                 raise ValueError(
                     f"""Columns given : {column}.
@@ -515,52 +500,49 @@
             )
 
         range_ = max_ - min_
         bin_size = range_ / bins
 
         template_ = """
             select
-            floor("{{column}}"/{{bin_size}})*{{bin_size}},
+            floor("{{column}}"/{{bin_size}})*{{bin_size}} as bin,
             count(*) as count
             from "{{table}}"
             {{filter_query}}
-            group by 1
-            order by 1;
+            group by bin
+            order by bin;
             """
 
         if use_backticks:
             template_ = template_.replace('"', "`")
 
         template = Template(template_)
 
         query = template.render(
             table=table, column=column, bin_size=bin_size, filter_query=filter_query
         )
     else:
         template_ = """
         select
-            "{{column}}", count ({{column}})
+            "{{column}}" as col, count ({{column}})
         from "{{table}}"
         {{filter_query}}
-        group by 1
-        order by 1;
+        group by col
+        order by col;
         """
 
         if use_backticks:
             template_ = template_.replace('"', "`")
 
         template = Template(template_)
 
         query = template.render(table=table, column=column, filter_query=filter_query)
 
-    if with_:
-        query = str(store.render(query, with_=with_))
+    data = conn.execute(query, with_).fetchall()
 
-    query = conn._transpile_query(query)
-    data = conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
     bin_, height = zip(*data)
 
     if bin_[0] is None:
         raise ValueError("Data contains NULLs")
 
     return bin_, height, bin_size
 
@@ -578,44 +560,36 @@
 ):
     """Compute the corresponding heights of each bin based on the category"""
     if not conn:
         conn = sql.connection.Connection.current
 
     cases = []
     for bin in bins:
-        case = f'SUM(CASE WHEN floor = {bin} THEN count ELSE 0 END) AS "{bin}",'
+        case = f'SUM(CASE WHEN FLOOR({column}/{bin_size})*{bin_size} = {bin} \
+                 THEN 1 ELSE 0 END) AS "{bin}",'
         cases.append(case)
 
     cases = " ".join(cases)
 
     filter_query = f"WHERE {facet['key']} == '{facet['value']}'" if facet else ""
 
     template = Template(
         """
         SELECT {{category}},
         {{cases}}
-        FROM (
-        SELECT FLOOR("{{column}}"/{{bin_size}})*{{bin_size}} AS floor,
-        {{category}}, COUNT(*) as count
         FROM "{{table}}"
-        GROUP BY floor, {{category}}
         {{filter_query}}
-        ) AS subquery
         GROUP BY {{category}};
         """
     )
     query = template.render(
         table=table,
         column=column,
         bin_size=bin_size,
         category=category,
         filter_query=filter_query,
         cases=cases,
     )
 
-    if with_:
-        query = str(store.render(query, with_=with_))
-
-    query = conn._transpile_query(query)
-    data = conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
+    data = conn.execute(query, with_).fetchall()
 
     return data
```

### Comparing `jupysql-0.7.1/src/sql/run.py` & `jupysql-0.7.2/src/sql/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from functools import reduce
 from io import StringIO
 import html
 
 import prettytable
 import sqlalchemy
 import sqlparse
-import sql.connection
+from sql.connection import Connection
+from sql import exceptions
 from .column_guesser import ColumnGuesserMixin
 
 try:
     from pgspecial.main import PGSpecial
-except ImportError:
+except ModuleNotFoundError:
     PGSpecial = None
 from sqlalchemy.orm import Session
 
 from sql.telemetry import telemetry
 import logging
 import warnings
+from collections.abc import Iterable
 
 
 def unduplicate_field_names(field_names):
     """Append a number to duplicate field names to make them unique."""
     res = []
     for k in field_names:
         if k in res:
@@ -104,30 +106,45 @@
 
     Can access rows listwise, or by string value of leftmost column.
     """
 
     def __init__(self, sqlaproxy, config):
         self.config = config
         self.keys = {}
-        if sqlaproxy.returns_rows:
-            self.keys = sqlaproxy.keys()
-            if isinstance(config.autolimit, int) and config.autolimit > 0:
-                list.__init__(self, sqlaproxy.fetchmany(size=config.autolimit))
-            else:
-                list.__init__(self, sqlaproxy.fetchall())
-            self.field_names = unduplicate_field_names(self.keys)
 
-            _style = None
-            if isinstance(config.style, str):
-                _style = prettytable.__dict__[config.style.upper()]
+        is_sql_alchemy_results = not hasattr(sqlaproxy, "description")
+
+        list.__init__(self, [])
+        self.pretty = None
 
-            self.pretty = PrettyTable(self.field_names, style=_style)
+        if is_sql_alchemy_results:
+            should_try_fetch_results = sqlaproxy.returns_rows
         else:
-            list.__init__(self, [])
-            self.pretty = None
+            should_try_fetch_results = True
+
+        if should_try_fetch_results:
+            if is_sql_alchemy_results:
+                self.keys = sqlaproxy.keys()
+            elif isinstance(sqlaproxy.description, Iterable):
+                self.keys = [i[0] for i in sqlaproxy.description]
+            else:
+                self.keys = []
+
+            if len(self.keys) > 0:
+                if isinstance(config.autolimit, int) and config.autolimit > 0:
+                    list.__init__(self, sqlaproxy.fetchmany(size=config.autolimit))
+                else:
+                    list.__init__(self, sqlaproxy.fetchall())
+                self.field_names = unduplicate_field_names(self.keys)
+
+                _style = None
+                if isinstance(config.style, str):
+                    _style = prettytable.__dict__[config.style.upper()]
+
+                self.pretty = PrettyTable(self.field_names, style=_style)
 
     def _repr_html_(self):
         _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
         if self.pretty:
             self.pretty.add_rows(self)
             result = self.pretty.get_html_string()
             # to create clickable links
@@ -177,15 +194,15 @@
     def DataFrame(self, payload):
         "Returns a Pandas DataFrame instance built from the result set."
         import pandas as pd
 
         frame = pd.DataFrame(self, columns=(self and self.keys) or [])
         payload[
             "connection_info"
-        ] = sql.connection.Connection.current._get_curr_sqlalchemy_connection_info()
+        ] = Connection.current._get_curr_sqlalchemy_connection_info()
         return frame
 
     @telemetry.log_call("polars-data-frame")
     def PolarsDataFrame(self, **polars_dataframe_kwargs):
         "Returns a Polars DataFrame instance built from the result set."
         import polars as pl
 
@@ -406,15 +423,16 @@
     """Checks if driver is pytds"""
     return "pytds" in str(dialect)
 
 
 def handle_postgres_special(conn, statement):
     """Execute a PostgreSQL special statement using PGSpecial module."""
     if not PGSpecial:
-        raise ImportError("pgspecial not installed")
+        raise exceptions.MissingPackageError("pgspecial not installed")
+
     pgspecial = PGSpecial()
     _, cur, headers, _ = pgspecial.execute(conn.session.connection.cursor(), statement)[
         0
     ]
     return FakeResultProxy(cur, headers)
 
 
@@ -459,24 +477,33 @@
         # returning only when sql is empty string
         return "Connected: %s" % conn.name
 
     for statement in sqlparse.split(sql):
         first_word = sql.strip().split()[0].lower()
         manual_commit = False
         if first_word == "begin":
-            raise ValueError("ipython_sql does not support transactions")
+            raise exceptions.RuntimeError("JupySQL does not support transactions")
         if first_word.startswith("\\") and is_postgres_or_redshift(conn.dialect):
             result = handle_postgres_special(conn, statement)
         else:
             txt = sqlalchemy.sql.text(statement)
             manual_commit = set_autocommit(conn, config)
-            result = conn.session.execute(txt)
+
+            is_custom_connection = Connection.is_custom_connection(conn)
+            if is_custom_connection:
+                txt_ = str(txt)
+            else:
+                txt_ = txt
+            # stringify txt to avoid TypeError:
+            # Boolean value of this clause is not defined
+            result = conn.session.execute(txt_)
         _commit(conn=conn, config=config, manual_commit=manual_commit)
         if result and config.feedback:
-            print(interpret_rowcount(result.rowcount))
+            if hasattr(result, "rowcount"):
+                print(interpret_rowcount(result.rowcount))
 
     resultset = ResultSet(result, config)
     return select_df_type(resultset, config)
 
 
 def raw_run(conn, sql):
     return conn.session.execute(sqlalchemy.sql.text(sql))
```

### Comparing `jupysql-0.7.1/src/sql/store.py` & `jupysql-0.7.2/src/sql/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Iterator, Iterable
 from collections.abc import MutableMapping
 from jinja2 import Template
 from ploomber_core.exceptions import modify_exceptions
 import sql.connection
-from IPython.core.error import UsageError
 import warnings
 import difflib
 
+from sql import exceptions
+
 
 class SQLStore(MutableMapping):
     """Stores SQL scripts to render large queries with CTEs
 
     Notes
     -----
     .. versionadded:: 0.4.3
@@ -39,23 +40,23 @@
         self._data = dict()
 
     def __setitem__(self, key: str, value: str) -> None:
         self._data[key] = value
 
     def __getitem__(self, key) -> str:
         if not self._data:
-            raise UsageError("No saved SQL")
+            raise exceptions.UsageError("No saved SQL")
         if key not in self._data:
             matches = difflib.get_close_matches(key, self._data)
             error = f'"{key}" is not a valid snippet identifier.'
             if matches:
-                raise UsageError(error + f' Did you mean "{matches[0]}"?')
+                raise exceptions.UsageError(error + f' Did you mean "{matches[0]}"?')
             else:
                 valid = ", ".join(f'"{key}"' for key in self._data.keys())
-                raise UsageError(error + f" Valid identifiers are {valid}.")
+                raise exceptions.UsageError(error + f" Valid identifiers are {valid}.")
         return self._data[key]
 
     def __iter__(self) -> Iterator[str]:
         for key in self._data:
             yield key
 
     def __len__(self) -> int:
@@ -67,20 +68,22 @@
     def render(self, query, with_=None):
         # TODO: if with is false, WITH should not appear
         return SQLQuery(self, query, with_)
 
     @modify_exceptions
     def store(self, key, query, with_=None):
         if "-" in key:
-            raise UsageError(
-                "Using hyphens in save argument isn't allowed."
-                " Please use dashes(-) instead"
+            raise exceptions.UsageError(
+                "Using hyphens (-) in save argument isn't allowed."
+                " Please use underscores (_) instead"
             )
         if with_ and key in with_:
-            raise ValueError(f"Script name ({key!r}) cannot appear in with_ argument")
+            raise exceptions.UsageError(
+                f"Script name ({key!r}) cannot appear in with_ argument"
+            )
 
         self._data[key] = SQLQuery(self, query, with_)
 
 
 class SQLQuery:
     """Holds queries and renders them"""
```

### Comparing `jupysql-0.7.1/src/sql/util.py` & `jupysql-0.7.2/src/sql/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 from sql import inspect
 import difflib
-import sql.run
 from sql.connection import Connection
 from sql.store import store
+from sql import exceptions
+
+SINGLE_QUOTE = "'"
+DOUBLE_QUOTE = '"'
+
+
+def sanitize_identifier(identifier):
+    if (identifier[0] == SINGLE_QUOTE and identifier[-1] == SINGLE_QUOTE) or (
+        identifier[0] == DOUBLE_QUOTE and identifier[-1] == DOUBLE_QUOTE
+    ):
+        return identifier[1:-1]
+    else:
+        return identifier
 
 
 def convert_to_scientific(value):
     """
     Converts value to scientific notation if necessary
 
     Parameters
@@ -62,38 +74,46 @@
     ignore_error: bool, default False
         Avoid raising a ValueError
     """
     if table is None:
         if ignore_error:
             return False
         else:
-            raise ValueError("Table cannot be None")
+            raise exceptions.UsageError("Table cannot be None")
     if not Connection.current:
-        raise RuntimeError("No active connection")
+        raise exceptions.RuntimeError("No active connection")
     if not conn:
         conn = Connection.current
 
     table = strip_multiple_chars(table, "\"'")
 
     if schema:
         table_ = f"{schema}.{table}"
     else:
         table_ = table
 
     _is_exist = _is_table_exists(table_, with_, conn)
 
     if not _is_exist:
         if not ignore_error:
+            try_find_suggestions = not Connection.is_custom_connection(conn)
             expected = []
-            existing_schemas = inspect.get_schema_names()
+            existing_schemas = []
+            existing_tables = []
+
+            if try_find_suggestions:
+                existing_schemas = inspect.get_schema_names()
+
             if schema and schema not in existing_schemas:
                 expected = existing_schemas
                 invalid_input = schema
             else:
-                existing_tables = _get_list_of_existing_tables()
+                if try_find_suggestions:
+                    existing_tables = _get_list_of_existing_tables()
+
                 expected = existing_tables
                 invalid_input = table
 
             if schema:
                 err_message = (
                     f"There is no table with name {table!r} in schema {schema!r}"
                 )
@@ -114,15 +134,15 @@
                 suggestions = difflib.get_close_matches(invalid_input, expected)
 
                 if len(suggestions) > 0:
                     _suggestions_string = pretty_print(suggestions, last_delimiter="or")
                     suggestions_message = f"\nDid you mean : {_suggestions_string}"
                     err_message = f"{err_message}{suggestions_message}"
 
-            raise ValueError(err_message)
+            raise exceptions.TableNotFoundError(err_message)
 
     return _is_exist
 
 
 def _get_list_of_existing_tables() -> list:
     """
     Returns a list of table names for a given connection
@@ -162,26 +182,71 @@
 
 def _is_table_exists(table: str, with_: str, conn) -> bool:
     """
     Runs a SQL query to check if table exists
     """
     if not conn:
         conn = Connection.current
+
     identifiers = conn.get_curr_identifiers()
+
     if with_:
         return table in list(store)
     else:
         for iden in identifiers:
             if isinstance(iden, tuple):
                 query = "SELECT * FROM {0}{1}{2} WHERE 1=0".format(
                     iden[0], table, iden[1]
                 )
             else:
                 query = "SELECT * FROM {0}{1}{0} WHERE 1=0".format(iden, table)
             try:
-                query = conn._transpile_query(query)
-                sql.run.raw_run(conn, query)
+                conn.execute(query)
                 return True
             except Exception:
                 pass
 
     return False
+
+
+def flatten(src, ltypes=(list, tuple)):
+    """The flatten function creates a new tuple / list
+    with all sub-tuple / sub-list elements concatenated into it recursively
+
+    Parameters
+    ----------
+    src : tuple / list
+        Source tuple / list with all sub-tuple / sub-list elements
+    ltypes : tuple, optional
+        sub element's data type, by default (list, tuple)
+
+    Returns
+    -------
+    tuple / list
+        Flatten tuple / list
+    """
+    ltype = type(src)
+    # Create a process list to handle flatten elements
+    process_list = list(src)
+    i = 0
+    while i < len(process_list):
+        while isinstance(process_list[i], ltypes):
+            if not process_list[i]:
+                process_list.pop(i)
+                i -= 1
+                break
+            else:
+                process_list[i : i + 1] = process_list[i]
+        i += 1
+
+    # If input src data type is tuple, return tuple
+    if not isinstance(process_list, ltype):
+        return tuple(process_list)
+    return process_list
+
+
+def support_only_sql_alchemy_connection(command):
+    """
+    Throws a sql.exceptions.RuntimeError if connection is not SQLAlchemy
+    """
+    if Connection.is_custom_connection():
+        raise exceptions.RuntimeError(f"{command} is not supported for a custom engine")
```

