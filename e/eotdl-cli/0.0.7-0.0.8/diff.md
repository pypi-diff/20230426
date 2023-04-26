# Comparing `tmp/eotdl_cli-0.0.7.tar.gz` & `tmp/eotdl_cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl_cli-0.0.7.tar", max compression
+gzip compressed data, was "eotdl_cli-0.0.8.tar", max compression
```

## Comparing `eotdl_cli-0.0.7.tar` & `eotdl_cli-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.7/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-25 09:43:24.394687 eotdl_cli-0.0.7/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1184 2023-04-25 09:43:34.326720 eotdl_cli-0.0.7/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      480 2023-04-25 09:41:49.358365 eotdl_cli-0.0.7/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.7/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     2527 2023-04-25 09:32:20.840458 eotdl_cli-0.0.7/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      603 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1072 2023-04-11 08:30:40.657793 eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      573 2023-04-25 09:44:06.534826 eotdl_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 eotdl_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-0.0.8/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.8/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-25 09:43:24.394687 eotdl_cli-0.0.8/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1184 2023-04-25 14:20:41.828930 eotdl_cli-0.0.8/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-25 09:46:47.051348 eotdl_cli-0.0.8/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.8/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-0.0.8/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-0.0.8/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     3499 2023-04-25 14:34:45.862185 eotdl_cli-0.0.8/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-0.0.8/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-0.0.8/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-0.0.8/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      726 2023-04-25 14:20:29.904830 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-25 13:29:34.233064 eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      573 2023-04-25 14:57:05.356199 eotdl_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 eotdl_cli-0.0.8/PKG-INFO
```

### Comparing `eotdl_cli-0.0.7/eotdl_cli/commands/auth.py` & `eotdl_cli-0.0.8/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/eotdl_cli/commands/datasets.py` & `eotdl_cli-0.0.8/eotdl_cli/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/eotdl_cli/src/repos/AuthRepo.py` & `eotdl_cli-0.0.8/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/eotdl_cli/src/usecases/auth/main.py` & `eotdl_cli-0.0.8/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/eotdl_cli/src/usecases/datasets/main.py` & `eotdl_cli-0.0.8/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-0.0.7/pyproject.toml` & `eotdl_cli-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl_cli-0.0.7/PKG-INFO` & `eotdl_cli-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

