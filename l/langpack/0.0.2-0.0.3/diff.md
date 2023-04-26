# Comparing `tmp/langpack-0.0.2-py2.py3-none-any.whl.zip` & `tmp/langpack-0.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13028 bytes, number of entries: 12
+Zip file size: 13027 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 18:39 langpack/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Apr-21 03:47 langpack/app_template.py
 -rw-rw-r--  2.0 unx      611 b- defN 23-Apr-21 04:02 langpack/client_template.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Apr-20 22:07 langpack/index.html
 -rw-rw-r--  2.0 unx     7528 b- defN 23-Apr-21 05:17 langpack/tester.py
 -rw-rw-r--  2.0 unx    21745 b- defN 23-Apr-21 06:43 langpack/tools.py
 -rw-rw-r--  2.0 unx     7512 b- defN 23-Apr-24 16:47 langpack/utils.py
--rw-rw-r--  2.0 unx      871 b- defN 23-Apr-25 22:05 langpack-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-25 22:05 langpack-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       77 b- defN 23-Apr-25 22:05 langpack-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-25 22:05 langpack-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      934 b- defN 23-Apr-25 22:05 langpack-0.0.2.dist-info/RECORD
-12 files, 43041 bytes uncompressed, 11464 bytes compressed:  73.4%
+-rw-rw-r--  2.0 unx      871 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       77 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      934 b- defN 23-Apr-25 22:28 langpack-0.0.3.dist-info/RECORD
+12 files, 43041 bytes uncompressed, 11463 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langpack/tools.py
 Comment: 
 
 Filename: langpack/utils.py
 Comment: 
 
-Filename: langpack-0.0.2.dist-info/METADATA
+Filename: langpack-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: langpack-0.0.2.dist-info/WHEEL
+Filename: langpack-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: langpack-0.0.2.dist-info/entry_points.txt
+Filename: langpack-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: langpack-0.0.2.dist-info/top_level.txt
+Filename: langpack-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: langpack-0.0.2.dist-info/RECORD
+Filename: langpack-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `langpack-0.0.2.dist-info/METADATA` & `langpack-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langpack
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library to pakcage and deploy langugage model apps
 Home-page: UNKNOWN
 Author: Chuan Li
 Author-email: c@lambdalabs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: apify-client (==1.0.0)
```

## Comparing `langpack-0.0.2.dist-info/RECORD` & `langpack-0.0.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 langpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 langpack/app_template.py,sha256=Athx3xBnaw3twNdjtR_qbM37CRXj8-iL2e8CL0vjoaY,857
 langpack/client_template.py,sha256=76uiHaqX-YNpbl4yd62a-V1dXV5S0tcxbTXYOsGTQfI,611
 langpack/index.html,sha256=BQdpj0HZwhSfctr69ZeddzalBGHAp3WCb-LM6rkIzJM,2787
 langpack/tester.py,sha256=PoDgNQe_fis7y6ZsQOITTF6M1svBZ-Sp2cE5EqTRadU,7528
 langpack/tools.py,sha256=Yg6yrUoZ9fgNU7rMErYoTS5YCeP-m9adAkDZ5JvDeYY,21745
 langpack/utils.py,sha256=2fmcJwHpoSgnscrJ47ZFYXFToIEWazooo75VQNcbTP0,7512
-langpack-0.0.2.dist-info/METADATA,sha256=u8j7MGUR6Lc8fPz7DNs3UfepJfKwEKB47WmxVnYIj-Q,871
-langpack-0.0.2.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-langpack-0.0.2.dist-info/entry_points.txt,sha256=tr9PNRuctA7z6aoVqeR4pND15CtSHpq6v-Bmjfyipyw,77
-langpack-0.0.2.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
-langpack-0.0.2.dist-info/RECORD,,
+langpack-0.0.3.dist-info/METADATA,sha256=M_HUoqbnM00711-pDp14lkEkjb9H9eZw2kVGmo9YxWI,871
+langpack-0.0.3.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+langpack-0.0.3.dist-info/entry_points.txt,sha256=tr9PNRuctA7z6aoVqeR4pND15CtSHpq6v-Bmjfyipyw,77
+langpack-0.0.3.dist-info/top_level.txt,sha256=j92Fj-GurEfjdOLmRWAy5wdVGVoOFqkhz6grAYs19Yw,9
+langpack-0.0.3.dist-info/RECORD,,
```

