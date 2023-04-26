# Comparing `tmp/determined_common-0.21.2rc1-py3-none-any.whl.zip` & `tmp/determined_common-0.21.2rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1813 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-20 16:40 determined_common/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-20 16:40 determined_common/__version__.py
--rw-r--r--  2.0 unx      417 b- defN 23-Apr-20 16:40 determined_common-0.21.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 16:40 determined_common-0.21.2rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-20 16:40 determined_common-0.21.2rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-20 16:40 determined_common-0.21.2rc1.dist-info/RECORD
-6 files, 1314 bytes uncompressed, 845 bytes compressed:  35.7%
+Zip file size: 1815 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-25 16:39 determined_common/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-25 16:39 determined_common/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-25 16:39 determined_common-0.21.2rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:39 determined_common-0.21.2rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-25 16:39 determined_common-0.21.2rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-25 16:39 determined_common-0.21.2rc3.dist-info/RECORD
+6 files, 1314 bytes uncompressed, 847 bytes compressed:  35.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_common/__init__.py
 Comment: 
 
 Filename: determined_common/__version__.py
 Comment: 
 
-Filename: determined_common-0.21.2rc1.dist-info/METADATA
+Filename: determined_common-0.21.2rc3.dist-info/METADATA
 Comment: 
 
-Filename: determined_common-0.21.2rc1.dist-info/WHEEL
+Filename: determined_common-0.21.2rc3.dist-info/WHEEL
 Comment: 
 
-Filename: determined_common-0.21.2rc1.dist-info/top_level.txt
+Filename: determined_common-0.21.2rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_common-0.21.2rc1.dist-info/RECORD
+Filename: determined_common-0.21.2rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_common/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.2-rc1"
+__version__ = "0.21.2-rc3"
```

## Comparing `determined_common-0.21.2rc1.dist-info/RECORD` & `determined_common-0.21.2rc3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_common/__init__.py,sha256=cHo0m87BOaQx-d4abum7tAeKV_ukSvs3xkABM7R76OM,235
-determined_common/__version__.py,sha256=v8errfpJ1jIFbo5yuHdWwU0hD-X0S1Q-G8Ut3xcPq2k,27
-determined_common-0.21.2rc1.dist-info/METADATA,sha256=YdJwk8AcQ5qTaKQpqaZFEBRhyFEjU331KTtx_Tpu9J8,417
-determined_common-0.21.2rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-determined_common-0.21.2rc1.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
-determined_common-0.21.2rc1.dist-info/RECORD,,
+determined_common/__version__.py,sha256=Xcv8cCtpX71oudQtnyMEVzGWcEMsi-_JoUR7gihVHWQ,27
+determined_common-0.21.2rc3.dist-info/METADATA,sha256=WpQo-N9W7QwNQIgdbva3nlsFc3yKuZJS94Fgf2VSl9Y,417
+determined_common-0.21.2rc3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined_common-0.21.2rc3.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
+determined_common-0.21.2rc3.dist-info/RECORD,,
```

