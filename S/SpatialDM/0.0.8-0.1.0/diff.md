# Comparing `tmp/SpatialDM-0.0.8.tar.gz` & `tmp/SpatialDM-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpatialDM-0.0.8.tar", last modified: Tue Mar 14 12:12:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

