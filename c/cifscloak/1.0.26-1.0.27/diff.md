# Comparing `tmp/cifscloak-1.0.26.tar.gz` & `tmp/cifscloak-1.0.27-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cifscloak-1.0.26.tar", last modified: Thu Jun  9 20:29:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

