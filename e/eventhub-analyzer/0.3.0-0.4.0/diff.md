# Comparing `tmp/eventhub_analyzer-0.3.0.tar.gz` & `tmp/eventhub_analyzer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhub_analyzer-0.3.0.tar", max compression
+gzip compressed data, was "eventhub_analyzer-0.4.0.tar", max compression
```

## Comparing `eventhub_analyzer-0.3.0.tar` & `eventhub_analyzer-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       21 2023-01-31 13:48:25.910746 eventhub_analyzer-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.3.0/eventhub_analyzer/__init__.py
--rw-r--r--   0        0        0     6972 2023-01-31 13:53:10.620535 eventhub_analyzer-0.3.0/eventhub_analyzer/main.py
--rw-r--r--   0        0        0      533 2023-01-31 13:54:47.511783 eventhub_analyzer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 eventhub_analyzer-0.3.0/setup.py
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 eventhub_analyzer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1933 2023-02-15 17:11:16.847513 eventhub_analyzer-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.4.0/eventhub_analyzer/__init__.py
+-rw-r--r--   0        0        0    12354 2023-02-22 15:59:56.060035 eventhub_analyzer-0.4.0/eventhub_analyzer/main.py
+-rw-r--r--   0        0        0      626 2023-04-26 09:23:50.328721 eventhub_analyzer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 eventhub_analyzer-0.4.0/setup.py
+-rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 eventhub_analyzer-0.4.0/PKG-INFO
```

### Comparing `eventhub_analyzer-0.3.0/pyproject.toml` & `eventhub_analyzer-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "eventhub-analyzer"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Stefan Hudelmaier <stefan.hudelmaier@device-insight.com>"]
 readme = "README.md"
 packages = [{include = "eventhub_analyzer"}]
+repository = "https://github.com/deviceinsight/eventhub-analyzer"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 azure-storage-blob = "^12.14.1"
 python-dotenv = "^0.21.1"
 jsonpickle = "^3.0.1"
 texttable = "^1.6.7"
 click = "^8.1.3"
+azure-eventhub = "^5.11.1"
 
 [tool.poetry.scripts]
 eventhub-analyzer = "eventhub_analyzer.main:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

