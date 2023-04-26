# Comparing `tmp/chopper-0.5.0.tar.gz` & `tmp/chopper-0.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chopper-0.5.0.tar", last modified: Thu Jul  7 14:41:06 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

