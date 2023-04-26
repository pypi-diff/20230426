# Comparing `tmp/synthea-rdf-0.1.5.tar.gz` & `tmp/synthea_rdf-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthea-rdf-0.1.5.tar", last modified: Sun Apr 23 05:55:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

