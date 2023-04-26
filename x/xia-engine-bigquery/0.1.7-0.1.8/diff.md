# Comparing `tmp/xia_engine_bigquery-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_bigquery-0.1.8-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 471127 bytes, number of entries: 9
--rw-r--r--  2.0 unx      361 b- defN 23-Apr-23 10:43 xia_engine_bigquery/__init__.py
--rw-r--r--  2.0 unx   626688 b- defN 23-Apr-23 10:50 xia_engine_bigquery/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   299520 b- defN 23-Apr-23 10:51 xia_engine_bigquery/proto.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   294912 b- defN 23-Apr-23 10:49 xia_engine_bigquery/schema.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 10:51 xia_engine_bigquery-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      886 b- defN 23-Apr-23 10:51 xia_engine_bigquery-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 10:51 xia_engine_bigquery-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-23 10:51 xia_engine_bigquery-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      846 b- defN 23-Apr-23 10:51 xia_engine_bigquery-0.1.7.dist-info/RECORD
-9 files, 1223484 bytes uncompressed, 469645 bytes compressed:  61.6%
+Zip file size: 384848 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      361 b- defN 23-Apr-26 20:17 xia_engine_bigquery/__init__.py
+-rw-r--r--  2.0 unx   542736 b- defN 23-Apr-26 20:17 xia_engine_bigquery/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx   268808 b- defN 23-Apr-26 20:17 xia_engine_bigquery/proto.cpython-310-darwin.so
+-rw-r--r--  2.0 unx   269568 b- defN 23-Apr-26 20:18 xia_engine_bigquery/schema.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-26 20:18 xia_engine_bigquery-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      849 b- defN 23-Apr-26 20:18 xia_engine_bigquery-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-26 20:18 xia_engine_bigquery-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-26 20:18 xia_engine_bigquery-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      856 b- defN 23-Apr-26 20:18 xia_engine_bigquery-0.1.8.dist-info/RECORD
+9 files, 1083458 bytes uncompressed, 383348 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_engine_bigquery/__init__.py
 Comment: 
 
-Filename: xia_engine_bigquery/engine.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_bigquery/proto.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/proto.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_bigquery/schema.cp39-win_amd64.pyd
+Filename: xia_engine_bigquery/schema.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.7.dist-info/LICENSE.txt
+Filename: xia_engine_bigquery-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.7.dist-info/METADATA
+Filename: xia_engine_bigquery-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.7.dist-info/WHEEL
+Filename: xia_engine_bigquery-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.7.dist-info/top_level.txt
+Filename: xia_engine_bigquery-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.7.dist-info/RECORD
+Filename: xia_engine_bigquery-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_bigquery/__init__.py

```diff
@@ -5,8 +5,8 @@
 
 __all__ = [
     "DocToProto",
     "DocToSchema",
     "BigqueryWriteEngine", "BigqueryStreamEngine", "BigqueryAppendOnlyEngine"
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_engine_bigquery-0.1.7.dist-info/METADATA` & `xia_engine_bigquery-0.1.8.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-bigquery
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A Document Engine on Bigquery
-Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: protobuf
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery-storage
 Requires-Dist: xia-engine
@@ -30,9 +28,7 @@
 =============================
 
 Install the package::
 
     pip install xia-engine-bigquery
 
 
-
-
```

