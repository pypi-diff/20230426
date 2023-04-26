# Comparing `tmp/mergepdf-0.0.3-py3-none-any.whl.zip` & `tmp/mergepdf-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3236 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1132 b- defN 80-Jan-01 00:00 mergepdf/__init__.py
+Zip file size: 6260 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 mergepdf/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 mergepdf/__main__.py
-?rw-r--r--  2.0 unx       42 b- defN 16-Jan-01 00:00 mergepdf-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1070 b- defN 80-Jan-01 00:00 mergepdf-0.0.3.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 mergepdf-0.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1329 b- defN 16-Jan-01 00:00 mergepdf-0.0.3.dist-info/METADATA
-?rw-r--r--  2.0 unx      546 b- defN 16-Jan-01 00:00 mergepdf-0.0.3.dist-info/RECORD
-7 files, 4229 bytes uncompressed, 2268 bytes compressed:  46.4%
+-rw-r--r--  2.0 unx    10763 b- defN 80-Jan-01 00:00 mergepdf-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mergepdf-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mergepdf-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx     1300 b- defN 80-Jan-01 00:00 mergepdf-0.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx      547 b- defN 16-Jan-01 00:00 mergepdf-0.1.0.dist-info/RECORD
+7 files, 13797 bytes uncompressed, 5292 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mergepdf/__init__.py
 Comment: 
 
 Filename: mergepdf/__main__.py
 Comment: 
 
-Filename: mergepdf-0.0.3.dist-info/entry_points.txt
+Filename: mergepdf-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: mergepdf-0.0.3.dist-info/LICENSE
+Filename: mergepdf-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: mergepdf-0.0.3.dist-info/WHEEL
+Filename: mergepdf-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mergepdf-0.0.3.dist-info/METADATA
+Filename: mergepdf-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: mergepdf-0.0.3.dist-info/RECORD
+Filename: mergepdf-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mergepdf/__init__.py

```diff
@@ -1,30 +1,26 @@
 import argparse
 import pathlib
 
 import PyPDF2
 
-# see pyproject.toml
-__version__ = "0.0.2"
-__author__ = "Saito Tsutomu <tsutomu7@hotmail.co.jp>"
-
 
 def mergepdf(input_dir, output_file, sorted_key):
     """Merge PDF files."""
-    lst = list(map(str, pathlib.Path(input_dir).rglob("*.pdf")))
+    lst = sorted(map(str, pathlib.Path(input_dir).rglob("*.pdf")))
     key = eval(f"lambda s: f'{sorted_key}'") if sorted_key else None
     if key:
         lst = sorted(lst, key=key)
         print(lst)
     try:
-        merger = PyPDF2.PdfFileMerger()
+        merger = PyPDF2.PdfMerger()
         merger.strict = False
         print("Including")
         for file in lst:
-            merger.append(file, import_bookmarks=False)
+            merger.append(file, import_outline=False)
             print(f' {file}{(" as " + key(file)) if key else ""}')
         merger.write(output_file)
     finally:
         merger.close()
         print(f"Output {output_file}")
```

## Comparing `mergepdf-0.0.3.dist-info/METADATA` & `mergepdf-0.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: mergepdf
-Version: 0.0.3
+Version: 0.1.0
 Summary: `mergepdf` is a package for merge PDF files.
 Home-page: https://github.com/SaitoTsutomu/mergepdf
-License: MIT
+License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: PyPDF2 (>=1.26.0,<2.0.0)
+Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
 Description-Content-Type: text/x-rst
 
 `mergepdf` is a package for merge PDF files.
 ::
 
    $ mergepdf -h
    usage: mergepdf [-h] [-i INPUT_DIR] [-o OUTPUT_FILE] [-k SORTED_KEY]
```

