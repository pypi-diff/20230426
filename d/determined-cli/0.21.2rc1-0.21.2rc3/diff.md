# Comparing `tmp/determined_cli-0.21.2rc1-py3-none-any.whl.zip` & `tmp/determined_cli-0.21.2rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1768 bytes, number of entries: 6
--rw-r--r--  2.0 unx      226 b- defN 23-Apr-20 16:40 determined_cli/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-20 16:40 determined_cli/__version__.py
--rw-r--r--  2.0 unx      414 b- defN 23-Apr-20 16:40 determined_cli-0.21.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 16:40 determined_cli-0.21.2rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-20 16:40 determined_cli-0.21.2rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      507 b- defN 23-Apr-20 16:40 determined_cli-0.21.2rc1.dist-info/RECORD
-6 files, 1281 bytes uncompressed, 836 bytes compressed:  34.7%
+Zip file size: 1767 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      226 b- defN 23-Apr-25 16:39 determined_cli/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-25 16:39 determined_cli/__version__.py
+-rw-r--r--  2.0 unx      414 b- defN 23-Apr-25 16:39 determined_cli-0.21.2rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:39 determined_cli-0.21.2rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-25 16:39 determined_cli-0.21.2rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      507 b- defN 23-Apr-25 16:39 determined_cli-0.21.2rc3.dist-info/RECORD
+6 files, 1281 bytes uncompressed, 835 bytes compressed:  34.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_cli/__init__.py
 Comment: 
 
 Filename: determined_cli/__version__.py
 Comment: 
 
-Filename: determined_cli-0.21.2rc1.dist-info/METADATA
+Filename: determined_cli-0.21.2rc3.dist-info/METADATA
 Comment: 
 
-Filename: determined_cli-0.21.2rc1.dist-info/WHEEL
+Filename: determined_cli-0.21.2rc3.dist-info/WHEEL
 Comment: 
 
-Filename: determined_cli-0.21.2rc1.dist-info/top_level.txt
+Filename: determined_cli-0.21.2rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_cli-0.21.2rc1.dist-info/RECORD
+Filename: determined_cli-0.21.2rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_cli/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.2-rc1"
+__version__ = "0.21.2-rc3"
```

