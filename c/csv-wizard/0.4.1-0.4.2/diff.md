# Comparing `tmp/csv-wizard-0.4.1.tar.gz` & `tmp/csv-wizard-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-wizard-0.4.1.tar", last modified: Wed Apr 26 12:54:58 2023, max compression
+gzip compressed data, was "csv-wizard-0.4.2.tar", last modified: Wed Apr 26 13:37:01 2023, max compression
```

## Comparing `csv-wizard-0.4.1.tar` & `csv-wizard-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-0.4.1/LICENSE
--rw-r--r--   0        0        0      528 2023-04-26 12:54:46.812982 csv-wizard-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9063 2023-04-26 12:18:53.685144 csv-wizard-0.4.1/README.md
--rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-0.4.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-0.4.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-0.4.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-0.4.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-0.4.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-0.4.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      602 2023-03-12 19:20:33.474055 csv-wizard-0.4.1/tests/blank_rows.csv
--rw-r--r--   0        0        0        0 2023-02-25 01:56:18.464794 csv-wizard-0.4.1/tests/empty.csv
--rw-r--r--   0        0        0    10763 2023-03-06 13:13:06.791537 csv-wizard-0.4.1/tests/everyone 246.csv
--rw-r--r--   0        0        0    10841 2023-03-06 13:01:51.287843 csv-wizard-0.4.1/tests/everyone 248.csv
--rw-r--r--   0        0        0      605 2023-02-25 02:31:25.668851 csv-wizard-0.4.1/tests/has_dups.csv
--rw-r--r--   0        0        0      221 2023-03-12 19:20:35.022067 csv-wizard-0.4.1/tests/small0.csv
--rw-r--r--   0        0        0      265 2023-03-12 19:08:47.060612 csv-wizard-0.4.1/tests/small1.csv
--rw-r--r--   0        0        0      689 2023-04-25 12:46:45.058770 csv-wizard-0.4.1/tests/test_divide.py
--rw-r--r--   0        0        0      261 2023-04-25 12:46:45.043745 csv-wizard-0.4.1/tests/test_encoding.py
--rw-r--r--   0        0        0      628 2023-04-25 12:48:02.485401 csv-wizard-0.4.1/tests/test_find_common_rows.py
--rw-r--r--   0        0        0      541 2023-04-25 12:46:45.073859 csv-wizard-0.4.1/tests/test_find_different_rows.py
--rw-r--r--   0        0        0      616 2023-04-25 12:48:02.522568 csv-wizard-0.4.1/tests/test_get_all_rows.py
--rw-r--r--   0        0        0      979 2023-04-25 12:48:02.541536 csv-wizard-0.4.1/tests/test_get_dialect.py
--rw-r--r--   0        0        0      846 2023-04-25 12:46:45.068689 csv-wizard-0.4.1/tests/test_get_duplicates.py
--rw-r--r--   0        0        0      431 2023-04-25 12:48:02.573957 csv-wizard-0.4.1/tests/test_get_headers.py
--rw-r--r--   0        0        0     1541 2023-04-25 12:48:02.592401 csv-wizard-0.4.1/tests/test_misc.py
--rw-r--r--   0        0        0      284 2023-04-25 12:48:02.609419 csv-wizard-0.4.1/tests/test_slice.py
--rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 csv-wizard-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-0.4.2/LICENSE
+-rw-r--r--   0        0        0      528 2023-04-26 13:36:44.013526 csv-wizard-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9063 2023-04-26 12:18:53.685144 csv-wizard-0.4.2/README.md
+-rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-0.4.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-0.4.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-0.4.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-0.4.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      602 2023-03-12 19:20:33.474055 csv-wizard-0.4.2/tests/blank_rows.csv
+-rw-r--r--   0        0        0        0 2023-02-25 01:56:18.464794 csv-wizard-0.4.2/tests/empty.csv
+-rw-r--r--   0        0        0    10763 2023-03-06 13:13:06.791537 csv-wizard-0.4.2/tests/everyone 246.csv
+-rw-r--r--   0        0        0    10841 2023-03-06 13:01:51.287843 csv-wizard-0.4.2/tests/everyone 248.csv
+-rw-r--r--   0        0        0      605 2023-02-25 02:31:25.668851 csv-wizard-0.4.2/tests/has_dups.csv
+-rw-r--r--   0        0        0      221 2023-03-12 19:20:35.022067 csv-wizard-0.4.2/tests/small0.csv
+-rw-r--r--   0        0        0      265 2023-03-12 19:08:47.060612 csv-wizard-0.4.2/tests/small1.csv
+-rw-r--r--   0        0        0      689 2023-04-25 12:46:45.058770 csv-wizard-0.4.2/tests/test_divide.py
+-rw-r--r--   0        0        0      261 2023-04-25 12:46:45.043745 csv-wizard-0.4.2/tests/test_encoding.py
+-rw-r--r--   0        0        0      628 2023-04-25 12:48:02.485401 csv-wizard-0.4.2/tests/test_find_common_rows.py
+-rw-r--r--   0        0        0      541 2023-04-25 12:46:45.073859 csv-wizard-0.4.2/tests/test_find_different_rows.py
+-rw-r--r--   0        0        0      616 2023-04-25 12:48:02.522568 csv-wizard-0.4.2/tests/test_get_all_rows.py
+-rw-r--r--   0        0        0      979 2023-04-25 12:48:02.541536 csv-wizard-0.4.2/tests/test_get_dialect.py
+-rw-r--r--   0        0        0      846 2023-04-25 12:46:45.068689 csv-wizard-0.4.2/tests/test_get_duplicates.py
+-rw-r--r--   0        0        0      431 2023-04-25 12:48:02.573957 csv-wizard-0.4.2/tests/test_get_headers.py
+-rw-r--r--   0        0        0     1541 2023-04-25 12:48:02.592401 csv-wizard-0.4.2/tests/test_misc.py
+-rw-r--r--   0        0        0      284 2023-04-25 12:48:02.609419 csv-wizard-0.4.2/tests/test_slice.py
+-rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 csv-wizard-0.4.2/PKG-INFO
```

### Comparing `csv-wizard-0.4.1/LICENSE` & `csv-wizard-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/pyproject.toml` & `csv-wizard-0.4.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "chardet>=5.1.0",
     "pytest>=7.2.1",
+    "build>=0.10.0",
+    "twine>=4.0.2",
 ]
 
 [project]
 name = "csv_wizard"
-version = "0.4.1"
+version = "0.4.2"
 description = "Handy extension to Python csv standard library package"
 authors = [
     { name = "liquidsnake", email = "bentsoft365@gmail.com" },
 ]
 dependencies = [
     "chardet>=5.1.0",
-    "build>=0.10.0",
-    "twine>=4.0.2",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `csv-wizard-0.4.1/README.md` & `csv-wizard-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/blank_rows.csv` & `csv-wizard-0.4.2/tests/blank_rows.csv`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/everyone 246.csv` & `csv-wizard-0.4.2/tests/everyone 246.csv`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/everyone 248.csv` & `csv-wizard-0.4.2/tests/everyone 248.csv`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/has_dups.csv` & `csv-wizard-0.4.2/tests/has_dups.csv`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_divide.py` & `csv-wizard-0.4.2/tests/test_divide.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_find_common_rows.py` & `csv-wizard-0.4.2/tests/test_find_common_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_find_different_rows.py` & `csv-wizard-0.4.2/tests/test_find_different_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_get_all_rows.py` & `csv-wizard-0.4.2/tests/test_get_all_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_get_dialect.py` & `csv-wizard-0.4.2/tests/test_get_dialect.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_get_duplicates.py` & `csv-wizard-0.4.2/tests/test_get_duplicates.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/tests/test_misc.py` & `csv-wizard-0.4.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-0.4.1/PKG-INFO` & `csv-wizard-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv_wizard
-Version: 0.4.1
+Version: 0.4.2
 Summary: Handy extension to Python csv standard library package
 License: MIT
 Author-email: liquidsnake <bentsoft365@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # CSV Divider
```

