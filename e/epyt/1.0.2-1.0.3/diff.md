# Comparing `tmp/epyt-1.0.2.tar.gz` & `tmp/epyt-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyt-1.0.2.tar", last modified: Mon Nov 28 15:22:40 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

