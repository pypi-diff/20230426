# Comparing `tmp/mlflow_hf_transformers-0.3.tar.gz` & `tmp/mlflow_hf_transformers-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_hf_transformers-0.3.tar", last modified: Mon Jan 16 15:36:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

