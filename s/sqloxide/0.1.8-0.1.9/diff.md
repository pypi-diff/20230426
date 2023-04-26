# Comparing `tmp/sqloxide-0.1.8-cp39-cp39-win_amd64.whl.zip` & `tmp/sqloxide-0.1.9-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 266380 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       58 b- defN 21-Jan-16 20:12 sqloxide/__init__.py
--rw-rw-rw-  2.0 fat   706560 b- defN 21-Jan-16 20:16 sqloxide/sqloxide.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1088 b- defN 21-Jan-16 20:16 sqloxide-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5486 b- defN 21-Jan-16 20:16 sqloxide-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      105 b- defN 21-Jan-16 20:16 sqloxide-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 21-Jan-16 20:16 sqloxide-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      561 b- defN 21-Jan-16 20:16 sqloxide-0.1.8.dist-info/RECORD
-7 files, 713867 bytes uncompressed, 265386 bytes compressed:  62.8%
+Zip file size: 285599 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       58 b- defN 21-Feb-16 15:14 sqloxide/__init__.py
+-rw-rw-rw-  2.0 fat   768512 b- defN 21-Feb-16 15:17 sqloxide/sqloxide.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1088 b- defN 21-Feb-16 15:17 sqloxide-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5246 b- defN 21-Feb-16 15:17 sqloxide-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      105 b- defN 21-Feb-16 15:17 sqloxide-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 21-Feb-16 15:17 sqloxide-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      561 b- defN 21-Feb-16 15:17 sqloxide-0.1.9.dist-info/RECORD
+7 files, 775579 bytes uncompressed, 284605 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqloxide/__init__.py
 Comment: 
 
 Filename: sqloxide/sqloxide.cp39-win_amd64.pyd
 Comment: 
 
-Filename: sqloxide-0.1.8.dist-info/LICENSE
+Filename: sqloxide-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: sqloxide-0.1.8.dist-info/METADATA
+Filename: sqloxide-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: sqloxide-0.1.8.dist-info/WHEEL
+Filename: sqloxide-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: sqloxide-0.1.8.dist-info/top_level.txt
+Filename: sqloxide-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sqloxide-0.1.8.dist-info/RECORD
+Filename: sqloxide-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sqloxide-0.1.8.dist-info/LICENSE` & `sqloxide-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sqloxide-0.1.8.dist-info/METADATA` & `sqloxide-0.1.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: sqloxide
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python bindings for sqlparser-rs
 Home-page: https://github.com/wseaton/sqloxide
 Author: Will Eaton
 Author-email: me@wseaton.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6.0,<4.0
 Description-Content-Type: text/markdown
 
 # sqloxide
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/wseaton/sqloxide/CI) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqloxide)
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/wseaton/sqloxide/CI)
 
 `sqloxide` wraps rust bindings for [sqlparser-rs](https://github.com/ballista-compute/sqlparser-rs) into a python package using `pyO3`.
 
-This package is currently in an *alpha* state, and while the upstream rust crate it wraps is pretty mature, I wouldn't use this in any production code yet ðŸ˜‰
-
 The original goal of this project was to have a very fast, efficient, and accurate SQL parser I could use for building data lineage graphs across large code bases (think hundreds of auto-generated .sql files). Most existing sql parsing approaches for python are either very slow or not accurate (especially in regards to deeply nested queries, sub-selects and/or table aliases).
 
 ## Installation
 
 The project provides `manylinux2014` wheels on pypi so it should be compatible with most linux distributions. Native wheels are also now available for OSX and Windows.
 
 To install from pypi:
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

