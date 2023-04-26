# Comparing `tmp/autobricks-0.4.0.tar.gz` & `tmp/autobricks-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobricks-0.4.0.tar", last modified: Mon Apr 24 20:03:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

