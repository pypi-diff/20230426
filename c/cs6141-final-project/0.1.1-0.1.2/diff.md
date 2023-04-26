# Comparing `tmp/cs6141_final_project-0.1.1.tar.gz` & `tmp/cs6141_final_project-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs6141_final_project-0.1.1.tar", max compression
+gzip compressed data, was "cs6141_final_project-0.1.2.tar", max compression
```

## Comparing `cs6141_final_project-0.1.1.tar` & `cs6141_final_project-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4234 2023-04-25 20:26:00.022925 cs6141_final_project-0.1.1/README.md
--rw-r--r--   0        0        0     1091 2023-04-26 21:39:09.563092 cs6141_final_project-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/base/__init__.py
--rw-r--r--   0        0        0       35 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/base/base.py
--rw-r--r--   0        0        0       23 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/builder/__init__.py
--rw-r--r--   0        0        0    10965 2023-04-26 21:22:40.453297 cs6141_final_project-0.1.1/src/final_project/builder/builder.py
--rw-r--r--   0        0        0        0 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/generate_sql/__init__.py
--rw-r--r--   0        0        0     2221 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/generate_sql/create_ddl.py
--rw-r--r--   0        0        0     3045 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/generate_sql/old_upload.py
--rw-r--r--   0        0        0      631 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/generate_sql/test_sql.py
--rw-r--r--   0        0        0     1620 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/generate_sql/upload_sql.py
--rw-r--r--   0        0        0       22 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.1/src/final_project/loader/__init__.py
--rw-r--r--   0        0        0     9897 2023-04-26 21:21:49.557029 cs6141_final_project-0.1.1/src/final_project/loader/loader.py
--rw-r--r--   0        0        0       49 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.1/src/final_project/models/__init__.py
--rw-r--r--   0        0        0    15001 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.1/src/final_project/models/feed_forward.py
--rw-r--r--   0        0        0     4274 2023-04-26 21:21:49.557029 cs6141_final_project-0.1.1/src/final_project/models/models.py
--rw-r--r--   0        0        0       20 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.1/src/final_project/plots/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.1/src/final_project/plots/plots.py
--rw-r--r--   0        0        0       19 2023-04-26 16:10:32.921471 cs6141_final_project-0.1.1/src/final_project/roc/__init__.py
--rw-r--r--   0        0        0      224 2023-04-26 17:43:30.444656 cs6141_final_project-0.1.1/src/final_project/roc/roc.py
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 cs6141_final_project-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4234 2023-04-25 20:26:00.022925 cs6141_final_project-0.1.2/README.md
+-rw-r--r--   0        0        0     1091 2023-04-26 21:43:09.306066 cs6141_final_project-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/base/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/base/base.py
+-rw-r--r--   0        0        0       23 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/builder/__init__.py
+-rw-r--r--   0        0        0    10965 2023-04-26 21:22:40.453297 cs6141_final_project-0.1.2/src/final_project/builder/builder.py
+-rw-r--r--   0        0        0        0 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/generate_sql/__init__.py
+-rw-r--r--   0        0        0     2221 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/generate_sql/create_ddl.py
+-rw-r--r--   0        0        0     3045 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/generate_sql/old_upload.py
+-rw-r--r--   0        0        0      631 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/generate_sql/test_sql.py
+-rw-r--r--   0        0        0     1620 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/generate_sql/upload_sql.py
+-rw-r--r--   0        0        0       22 2023-04-25 20:26:00.318924 cs6141_final_project-0.1.2/src/final_project/loader/__init__.py
+-rw-r--r--   0        0        0     9897 2023-04-26 21:21:49.557029 cs6141_final_project-0.1.2/src/final_project/loader/loader.py
+-rw-r--r--   0        0        0       49 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.2/src/final_project/models/__init__.py
+-rw-r--r--   0        0        0    15001 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.2/src/final_project/models/feed_forward.py
+-rw-r--r--   0        0        0     4274 2023-04-26 21:21:49.557029 cs6141_final_project-0.1.2/src/final_project/models/models.py
+-rw-r--r--   0        0        0       20 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.2/src/final_project/plots/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-26 21:21:43.545001 cs6141_final_project-0.1.2/src/final_project/plots/plots.py
+-rw-r--r--   0        0        0       19 2023-04-26 16:10:32.921471 cs6141_final_project-0.1.2/src/final_project/roc/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-26 17:43:30.444656 cs6141_final_project-0.1.2/src/final_project/roc/roc.py
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 cs6141_final_project-0.1.2/PKG-INFO
```

### Comparing `cs6141_final_project-0.1.1/README.md` & `cs6141_final_project-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/pyproject.toml` & `cs6141_final_project-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cs6141-final-project"
-version = "0.1.1"
+version = "0.1.2"
 description = "To infinity, and beyond!"
 authors = [
     "Daniel Blum <blum.da@northeastern.edu>",
     "Matt Greene <greene.matthew@northeastern.edu>",
     "Bram Ziltzer <ziltzer.b@northeastern.edu>",
 ]
 readme = "README.md"
@@ -15,22 +15,22 @@
 black = {extras = ["jupyter"], version = "^23.3.0"}
 pandas = "^1.5.3"
 psycopg2-binary = "^2.9.5"
 python-dotenv = "^1.0.0"
 sqlalchemy = "^2.0.7"
 pyyaml = "^6.0"
 jupyterlab = "^3.6.3"
-numpy = "^1.24.3"
 scikit-learn = "^1.2.2"
 kaggle = "^1.5.13"
 tqdm = "^4.65.0"
 matplotlib = "^3.7.1"
 torch = "^2.0.0"
 tabulate = "^0.9.0"
 seaborn = "^0.12.2"
+numpy = "^1.23.5"
 
 
 [tool.black]
 line-length = 79
 exclude = '''
 /(
     \.eggs
```

### Comparing `cs6141_final_project-0.1.1/src/final_project/builder/builder.py` & `cs6141_final_project-0.1.2/src/final_project/builder/builder.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/generate_sql/create_ddl.py` & `cs6141_final_project-0.1.2/src/final_project/generate_sql/create_ddl.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/generate_sql/old_upload.py` & `cs6141_final_project-0.1.2/src/final_project/generate_sql/old_upload.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/generate_sql/test_sql.py` & `cs6141_final_project-0.1.2/src/final_project/generate_sql/test_sql.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/generate_sql/upload_sql.py` & `cs6141_final_project-0.1.2/src/final_project/generate_sql/upload_sql.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/loader/loader.py` & `cs6141_final_project-0.1.2/src/final_project/loader/loader.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/models/feed_forward.py` & `cs6141_final_project-0.1.2/src/final_project/models/feed_forward.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/models/models.py` & `cs6141_final_project-0.1.2/src/final_project/models/models.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/src/final_project/plots/plots.py` & `cs6141_final_project-0.1.2/src/final_project/plots/plots.py`

 * *Files identical despite different names*

### Comparing `cs6141_final_project-0.1.1/PKG-INFO` & `cs6141_final_project-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cs6141-final-project
-Version: 0.1.1
+Version: 0.1.2
 Summary: To infinity, and beyond!
 Author: Daniel Blum
 Author-email: blum.da@northeastern.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
 Requires-Dist: jupyterlab (>=3.6.3,<4.0.0)
 Requires-Dist: kaggle (>=1.5.13,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sqlalchemy (>=2.0.7,<3.0.0)
```

