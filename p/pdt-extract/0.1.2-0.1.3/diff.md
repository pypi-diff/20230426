# Comparing `tmp/pdt_extract-0.1.2-py3-none-any.whl.zip` & `tmp/pdt_extract-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 1526 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      640 b- defN 23-Apr-26 18:37 pdt_extract-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 18:37 pdt_extract-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-26 18:37 pdt_extract-0.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-26 18:37 pdt_extract-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      411 b- defN 23-Apr-26 18:37 pdt_extract-0.1.2.dist-info/RECORD
-5 files, 1191 bytes uncompressed, 748 bytes compressed:  37.2%
+Zip file size: 8573 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    11413 b- defN 23-Apr-25 23:53 pdt_canny.py
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-26 19:26 pdt_extract/__init__.py
+-rw-rw-rw-  2.0 fat    11416 b- defN 23-Apr-26 19:26 pdt_extract/pdt_extract.py
+-rw-rw-rw-  2.0 fat      640 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      545 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/RECORD
+7 files, 24192 bytes uncompressed, 7609 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: pdt_extract-0.1.2.dist-info/METADATA
+Filename: pdt_canny.py
 Comment: 
 
-Filename: pdt_extract-0.1.2.dist-info/WHEEL
+Filename: pdt_extract/__init__.py
 Comment: 
 
-Filename: pdt_extract-0.1.2.dist-info/entry_points.txt
+Filename: pdt_extract/pdt_extract.py
 Comment: 
 
-Filename: pdt_extract-0.1.2.dist-info/top_level.txt
+Filename: pdt_extract-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pdt_extract-0.1.2.dist-info/RECORD
+Filename: pdt_extract-0.1.3.dist-info/WHEEL
+Comment: 
+
+Filename: pdt_extract-0.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: pdt_extract-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pdt_extract-0.1.2.dist-info/METADATA` & `pdt_extract-0.1.3.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdt-extract
-Version: 0.1.2
+Version: 0.1.3
 Summary: Perform edge profile and characteristic feature extraction from images of pendant drops
 Home-page: https://github.com/DmitriLyalikov/pdt-canny-edge-detector
 Author: Dmitri Lyalikov
 Author-email: Dlyalikov01@manhattan.edu
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 Requires-Dist: imageio
```

