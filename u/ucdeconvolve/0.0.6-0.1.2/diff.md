# Comparing `tmp/ucdeconvolve-0.0.6.tar.gz` & `tmp/ucdeconvolve-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdeconvolve-0.0.6.tar", last modified: Mon Jan 30 18:05:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

