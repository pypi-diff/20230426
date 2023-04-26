# Comparing `tmp/sqlmesh-0.6.1.tar.gz` & `tmp/sqlmesh-0.6.2.dev2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.6.1.tar", last modified: Wed Apr 26 18:54:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

