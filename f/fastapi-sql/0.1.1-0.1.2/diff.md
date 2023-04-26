# Comparing `tmp/fastapi_sql-0.1.1.tar.gz` & `tmp/fastapi_sql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_sql-0.1.2.tar", max compression
```

## Comparing `fastapi_sql-0.1.1.tar` & `fastapi_sql-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1488 2023-04-26 16:25:20.232468 fastapi_sql-0.1.1/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.1/fastapi_sql/exceptions.py
--rw-r--r--   0        0        0      919 2023-04-26 16:21:35.866852 fastapi_sql-0.1.1/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     2037 2023-04-26 15:59:18.170588 fastapi_sql-0.1.1/fastapi_sql/model.py
--rw-r--r--   0        0        0      359 2023-04-26 16:01:43.615418 fastapi_sql-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-04-26 16:25:20.232468 fastapi_sql-0.1.2/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-26 14:38:45.038024 fastapi_sql-0.1.2/fastapi_sql/exceptions.py
+-rw-r--r--   0        0        0      919 2023-04-26 16:21:35.866852 fastapi_sql-0.1.2/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0      451 2023-04-26 16:44:45.417912 fastapi_sql-0.1.2/fastapi_sql/model.py
+-rw-r--r--   0        0        0      359 2023-04-26 16:42:13.555086 fastapi_sql-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 fastapi_sql-0.1.2/PKG-INFO
```

### Comparing `fastapi_sql-0.1.1/fastapi_sql/__init__.py` & `fastapi_sql-0.1.2/fastapi_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.1/fastapi_sql/migrate.py` & `fastapi_sql-0.1.2/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.1.1/PKG-INFO` & `fastapi_sql-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

