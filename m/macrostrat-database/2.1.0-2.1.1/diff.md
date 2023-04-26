# Comparing `tmp/macrostrat_database-2.1.0.tar.gz` & `tmp/macrostrat_database-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.1.0.tar", max compression
+gzip compressed data, was "macrostrat_database-2.1.1.tar", max compression
```

## Comparing `macrostrat_database-2.1.0.tar` & `macrostrat_database-2.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.0/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4665 2023-04-11 04:58:29.434832 macrostrat_database-2.1.0/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.0/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.0/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.0/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.0/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0    12657 2023-04-25 21:07:24.145016 macrostrat_database-2.1.0/macrostrat/database/utils.py
--rw-r--r--   0        0        0      598 2023-04-25 21:08:52.862221 macrostrat_database-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.1/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4665 2023-04-11 04:58:29.434832 macrostrat_database-2.1.1/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.1/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.1/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.1/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.1/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0    12662 2023-04-25 21:41:15.569926 macrostrat_database-2.1.1/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      598 2023-04-25 21:41:39.945703 macrostrat_database-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.1/PKG-INFO
```

### Comparing `macrostrat_database-2.1.0/macrostrat/database/__init__.py` & `macrostrat_database-2.1.1/macrostrat/database/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/mapper/__init__.py` & `macrostrat_database-2.1.1/macrostrat/database/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/mapper/base.py` & `macrostrat_database-2.1.1/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/mapper/cache.py` & `macrostrat_database-2.1.1/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/mapper/utils.py` & `macrostrat_database-2.1.1/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/postgresql.py` & `macrostrat_database-2.1.1/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.0/macrostrat/database/utils.py` & `macrostrat_database-2.1.1/macrostrat/database/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         except (ProgrammingError, IntegrityError, InternalError) as err:
             _err = str(err.orig).strip()
             dim = "already exists" in _err
             if trans is not None:
                 trans.rollback()
             elif hasattr(connectable, "rollback"):
                 connectable.rollback()
-            pretty_print(sql, fg=None if dim else "red", dim=True)
+            pretty_print(sql_text, fg=None if dim else "red", dim=True)
             if dim:
                 _err = "  " + _err
             secho(_err, fg="red", dim=dim)
             log.error(err)
             if raise_errors:
                 raise err
```

### Comparing `macrostrat_database-2.1.0/pyproject.toml` & `macrostrat_database-2.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A SQLAlchemy-based database toolkit."
 name = "macrostrat.database"
 packages = [
   {include = "macrostrat"},
 ]
-version = "2.1.0"
+version = "2.1.1"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
```

### Comparing `macrostrat_database-2.1.0/PKG-INFO` & `macrostrat_database-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-database
-Version: 2.1.0
+Version: 2.1.1
 Summary: A SQLAlchemy-based database toolkit.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

