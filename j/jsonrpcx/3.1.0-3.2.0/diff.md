# Comparing `tmp/jsonrpcx-3.1.0.tar.gz` & `tmp/jsonrpcx-3.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpcx-3.1.0.tar", last modified: Sun Jul  4 14:42:47 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

