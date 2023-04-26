# Comparing `tmp/schoolware_api-1.0.1.tar.gz` & `tmp/schoolware_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.0.1.tar", last modified: Wed Apr 26 09:03:58 2023, max compression
+gzip compressed data, was "schoolware_api-1.0.2.tar", last modified: Wed Apr 26 09:09:16 2023, max compression
```

## Comparing `schoolware_api-1.0.1.tar` & `schoolware_api-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:57.998378 schoolware_api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 09:03:57.994377 schoolware_api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-26 09:03:43.000000 schoolware_api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 09:03:43.000000 schoolware_api-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:57.994377 schoolware_api-1.0.1/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:43.000000 schoolware_api-1.0.1/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-26 09:03:43.000000 schoolware_api-1.0.1/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:03:57.994377 schoolware_api-1.0.1/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 09:03:57.000000 schoolware_api-1.0.1/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 09:03:57.000000 schoolware_api-1.0.1/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:03:57.000000 schoolware_api-1.0.1/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 09:03:57.000000 schoolware_api-1.0.1/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 09:03:57.000000 schoolware_api-1.0.1/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:03:57.998378 schoolware_api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 09:03:43.000000 schoolware_api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/setup.py
```

### Comparing `schoolware_api-1.0.1/PKG-INFO` & `schoolware_api-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,16 @@
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
+### only microsoft login supported for now
+
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | bg | background procces to keep token valid
```

### Comparing `schoolware_api-1.0.1/README.md` & `schoolware_api-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
+### only microsoft login supported for now
+
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | bg | background procces to keep token valid
```

### Comparing `schoolware_api-1.0.1/pyproject.toml` & `schoolware_api-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.0.1/schoolware_api/schoolware_api.py` & `schoolware_api-1.0.2/schoolware_api/schoolware_api.py`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.0.1/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.0.2/schoolware_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,16 @@
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
 
+### only microsoft login supported for now
+
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | bg | background procces to keep token valid
```

