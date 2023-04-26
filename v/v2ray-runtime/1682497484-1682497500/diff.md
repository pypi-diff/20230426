# Comparing `tmp/v2ray_runtime-1682497484.tar.gz` & `tmp/v2ray_runtime-1682497500-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2ray_runtime-1682497484.tar", last modified: Wed Apr 26 08:24:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

