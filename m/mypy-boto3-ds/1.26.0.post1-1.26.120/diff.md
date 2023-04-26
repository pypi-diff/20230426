# Comparing `tmp/mypy-boto3-ds-1.26.0.post1.tar.gz` & `tmp/mypy_boto3_ds-1.26.120-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ds-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

