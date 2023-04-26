# Comparing `tmp/red2df-1.0.4.tar.gz` & `tmp/red2df-1.1.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red2df-1.0.4.tar", last modified: Tue Jun 21 09:06:50 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

