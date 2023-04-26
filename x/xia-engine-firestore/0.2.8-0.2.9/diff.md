# Comparing `tmp/xia_engine_firestore-0.2.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.2.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 148576 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Apr-23 09:19 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx   370688 b- defN 23-Apr-23 09:22 xia_engine_firestore/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-23 09:22 xia_engine_firestore-0.2.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Apr-23 09:22 xia_engine_firestore-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-23 09:22 xia_engine_firestore-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-23 09:22 xia_engine_firestore-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-23 09:22 xia_engine_firestore-0.2.8.dist-info/RECORD
-7 files, 372540 bytes uncompressed, 147410 bytes compressed:  60.4%
+Zip file size: 155881 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-26 10:17 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx   390144 b- defN 23-Apr-26 10:20 xia_engine_firestore/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      817 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-Apr-26 10:20 xia_engine_firestore-0.2.9.dist-info/RECORD
+7 files, 391996 bytes uncompressed, 154715 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
 Filename: xia_engine_firestore/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_firestore-0.2.8.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.2.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.8.dist-info/METADATA
+Filename: xia_engine_firestore-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.2.8.dist-info/WHEEL
+Filename: xia_engine_firestore-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.2.8.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.2.8.dist-info/RECORD
+Filename: xia_engine_firestore-0.2.9.dist-info/RECORD
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
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
```

## Comparing `xia_engine_firestore-0.2.8.dist-info/METADATA` & `xia_engine_firestore-0.2.9.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-firestore
-Version: 0.2.8
+Version: 0.2.9
 Summary: X-I-A Firestore Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.2.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.2.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_firestore-0.2.8.dist-info/RECORD` & `xia_engine_firestore-0.2.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_firestore/__init__.py,sha256=6VkvyjtYD37GaaIYI5TjyTCJZCSMZepknVf-NRrrp4E,117
-xia_engine_firestore/engine.cp39-win_amd64.pyd,sha256=5ItII18TR5-43KahOU1y5uF_ZvvJJ5qzXKRxXkiIdvY,370688
-xia_engine_firestore-0.2.8.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine_firestore-0.2.8.dist-info/METADATA,sha256=nNOFXBKULXg0KDrrxVn2lHDjj2LeG2tfsiHmFeQOAtY,817
-xia_engine_firestore-0.2.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_firestore-0.2.8.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
-xia_engine_firestore-0.2.8.dist-info/RECORD,,
+xia_engine_firestore/__init__.py,sha256=iXseMT6Z1dDgyurFxPWX9wCH-2El5cBf4Dnm_K_28is,117
+xia_engine_firestore/engine.cp39-win_amd64.pyd,sha256=1KHYG_vpYaAcbgnD19nsRztnJ5YQGFam-qkI1lS6AS4,390144
+xia_engine_firestore-0.2.9.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_firestore-0.2.9.dist-info/METADATA,sha256=m2Hdw3UK7Cl5P0cmoDSNBwU7leieGTAOCROwOhG3ing,817
+xia_engine_firestore-0.2.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_firestore-0.2.9.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
+xia_engine_firestore-0.2.9.dist-info/RECORD,,
```

