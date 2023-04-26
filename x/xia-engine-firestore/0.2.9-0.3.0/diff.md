# Comparing `tmp/xia_engine_firestore-0.2.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.3.0-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 155881 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Apr-26 10:17 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx   390144 b- defN 23-Apr-26 10:20 xia_engine_firestore/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/RECORD
-7 files, 391996 bytes uncompressed, 154715 bytes compressed:  60.5%
+Zip file size: 128411 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-26 18:55 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx   354544 b- defN 23-Apr-26 18:56 xia_engine_firestore/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-26 18:56 xia_engine_firestore-0.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      780 b- defN 23-Apr-26 18:56 xia_engine_firestore-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-26 18:56 xia_engine_firestore-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-26 18:56 xia_engine_firestore-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-26 18:56 xia_engine_firestore-0.3.0.dist-info/RECORD
+7 files, 356372 bytes uncompressed, 127239 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
-Filename: xia_engine_firestore/engine.cp39-win_amd64.pyd
+Filename: xia_engine_firestore/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_firestore-0.2.9.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.9.dist-info/METADATA
+Filename: xia_engine_firestore-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.2.9.dist-info/WHEEL
+Filename: xia_engine_firestore-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.2.9.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.9.dist-info/RECORD
+Filename: xia_engine_firestore-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.2.9"
+__version__ = "0.3.0"
```

## Comparing `xia_engine_firestore-0.2.9.dist-info/METADATA` & `xia_engine_firestore-0.3.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-firestore
-Version: 0.2.9
+Version: 0.3.0
 Summary: X-I-A Firestore Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.2.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.3.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: google-cloud-firestore
 Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-firestore.svg?color=blue
@@ -28,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install xia-engine-firestore
 
 
-
-
```

