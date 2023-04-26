# Comparing `tmp/stockpick-1.3.0.tar.gz` & `tmp/stockpick-1.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stockpick-1.3.0.tar", last modified: Thu Mar 23 10:53:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

