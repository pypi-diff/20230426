# Comparing `tmp/govqa-0.1.0-py3-none-any.whl.zip` & `tmp/govqa-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,8 @@
-Zip file size: 1350 bytes, number of entries: 4
--rw-r--r--  2.0 unx      905 b- defN 23-Apr-07 15:25 govqa-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 15:25 govqa-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-07 15:25 govqa-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      288 b- defN 23-Apr-07 15:25 govqa-0.1.0.dist-info/RECORD
-4 files, 1286 bytes uncompressed, 784 bytes compressed:  39.0%
+Zip file size: 3887 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-25 13:46 govqa/__init__.py
+-rw-r--r--  2.0 unx     6756 b- defN 23-Apr-25 13:46 govqa/base.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Apr-25 13:46 govqa-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 13:46 govqa-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-25 13:46 govqa-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      430 b- defN 23-Apr-25 13:46 govqa-0.1.1.dist-info/RECORD
+6 files, 8211 bytes uncompressed, 3109 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
-Filename: govqa-0.1.0.dist-info/METADATA
+Filename: govqa/__init__.py
 Comment: 
 
-Filename: govqa-0.1.0.dist-info/WHEEL
+Filename: govqa/base.py
 Comment: 
 
-Filename: govqa-0.1.0.dist-info/top_level.txt
+Filename: govqa-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: govqa-0.1.0.dist-info/RECORD
+Filename: govqa-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: govqa-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: govqa-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `govqa-0.1.0.dist-info/METADATA` & `govqa-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govqa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interact with GovQA, a public records request management platform owned by Granicus
 Home-page: https://datamade.us
 Author: DataMade
 Author-email: info@datamade.us
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

