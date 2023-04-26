# Comparing `tmp/l3c-0.0.1.tar.gz` & `tmp/l3c-0.0.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l3c-0.0.1.tar", last modified: Thu Feb 23 11:03:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

