# Comparing `tmp/esppy-0.1.1.tar.gz` & `tmp/esppy-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esppy-0.1.1.tar", last modified: Wed Apr 26 07:38:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

