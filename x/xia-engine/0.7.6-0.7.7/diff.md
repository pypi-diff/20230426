# Comparing `tmp/xia_engine-0.7.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.7.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1219744 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1383 b- defN 23-Apr-26 05:04 xia_engine/__init__.py
--rw-r--r--  2.0 unx   438784 b- defN 23-Apr-26 05:09 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   594432 b- defN 23-Apr-26 05:08 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   762880 b- defN 23-Apr-26 05:14 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   702976 b- defN 23-Apr-26 05:12 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   262144 b- defN 23-Apr-26 05:15 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   462848 b- defN 23-Apr-26 05:11 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 05:15 xia_engine-0.7.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      745 b- defN 23-Apr-26 05:15 xia_engine-0.7.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 05:15 xia_engine-0.7.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 05:15 xia_engine-0.7.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-26 05:15 xia_engine-0.7.6.dist-info/RECORD
-12 files, 3227506 bytes uncompressed, 1217978 bytes compressed:  62.3%
+Zip file size: 1241469 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1383 b- defN 23-Apr-26 09:36 xia_engine/__init__.py
+-rw-r--r--  2.0 unx   458240 b- defN 23-Apr-26 09:41 xia_engine/acl.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   594432 b- defN 23-Apr-26 09:40 xia_engine/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   779776 b- defN 23-Apr-26 09:46 xia_engine/document.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   720896 b- defN 23-Apr-26 09:44 xia_engine/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   262144 b- defN 23-Apr-26 09:47 xia_engine/exception.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   462848 b- defN 23-Apr-26 09:42 xia_engine/fields.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 09:47 xia_engine-0.7.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-26 09:47 xia_engine-0.7.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 09:47 xia_engine-0.7.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 09:47 xia_engine-0.7.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-26 09:47 xia_engine-0.7.7.dist-info/RECORD
+12 files, 3281778 bytes uncompressed, 1239703 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine/fields.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine-0.7.6.dist-info/LICENSE.txt
+Filename: xia_engine-0.7.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.7.6.dist-info/METADATA
+Filename: xia_engine-0.7.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.7.6.dist-info/WHEEL
+Filename: xia_engine-0.7.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.7.6.dist-info/top_level.txt
+Filename: xia_engine-0.7.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.7.6.dist-info/RECORD
+Filename: xia_engine-0.7.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
```

## Comparing `xia_engine-0.7.6.dist-info/METADATA` & `xia_engine-0.7.7.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.7.6
+Version: 0.7.7
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.7.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.7.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine-0.7.6.dist-info/RECORD` & `xia_engine-0.7.7.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_engine/__init__.py,sha256=_z_kqq1ZO2NdvtWFFUVFdNyk7g1p7MvsU3UEFeEB73A,1383
-xia_engine/acl.cp39-win_amd64.pyd,sha256=WqzKvKAcTgA3F0A7goVQwhO6ZAtRHW9qywUa-RjeCMY,438784
-xia_engine/base.cp39-win_amd64.pyd,sha256=cRE_UqoSFGMUrIuVyRk3AcfFC4dhCZYrrFLB2J9Ue-A,594432
-xia_engine/document.cp39-win_amd64.pyd,sha256=AfUQTmctJ2WTor9qQl1BcBwRfiFXqZLtr3hH1ukAOG0,762880
-xia_engine/engine.cp39-win_amd64.pyd,sha256=4prCZaPItRkuamDDdrlvXMaAC2DZkAH2QH4CHObVV_g,702976
-xia_engine/exception.cp39-win_amd64.pyd,sha256=7ubtZIe1Cf8eFylexIp1qpw5P1yw1y84ODbMB4bbbjY,262144
-xia_engine/fields.cp39-win_amd64.pyd,sha256=eUZnHEvpgQqPArwund-JQGAt5mCpz_EXIBsKbo1Ofvk,462848
-xia_engine-0.7.6.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine-0.7.6.dist-info/METADATA,sha256=-qAFenWpaw4WDCnvhdWNjvaUPhN2cEDMGpWauDJyKBk,745
-xia_engine-0.7.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine-0.7.6.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
-xia_engine-0.7.6.dist-info/RECORD,,
+xia_engine/__init__.py,sha256=s9WCxuOzHhIGM1TwsYPGdNl6CMjyfgDOU5vOWpOffTQ,1383
+xia_engine/acl.cp39-win_amd64.pyd,sha256=IyfG7JSiajDAhL3CnyNvNQl5g1KDzYk2nwP2zamR0Uk,458240
+xia_engine/base.cp39-win_amd64.pyd,sha256=UyeF2imsgDWlCRzmIWS_m-vosrMc4XPYMe8X7U-DdQU,594432
+xia_engine/document.cp39-win_amd64.pyd,sha256=VrMMmQJsSH2HydEmxnxMcDdTpAn2p7Y0NXni-mxvM88,779776
+xia_engine/engine.cp39-win_amd64.pyd,sha256=53wg9oJuAmbZeYvgU0H2_hB3eZICTSbuqSnGK7HrN-0,720896
+xia_engine/exception.cp39-win_amd64.pyd,sha256=1YEe4qpbSsBQ-dOReSQ0CraAVc4MOeg71fend1zHIYA,262144
+xia_engine/fields.cp39-win_amd64.pyd,sha256=e00H4r7Yl70GDa9632emjxmfoCQ7B3GZNHPqCd0W6OY,462848
+xia_engine-0.7.7.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine-0.7.7.dist-info/METADATA,sha256=F8KGuQJCXRfD1M3S-D8J0EG1S9ZH1Ck3BUx06x2-hjA,745
+xia_engine-0.7.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine-0.7.7.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
+xia_engine-0.7.7.dist-info/RECORD,,
```

