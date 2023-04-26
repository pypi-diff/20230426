# Comparing `tmp/elliptic_sdk-0.0.2.tar.gz` & `tmp/elliptic_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elliptic_sdk-0.0.2.tar", max compression
+gzip compressed data, was "elliptic_sdk-0.0.3.tar", max compression
```

## Comparing `elliptic_sdk-0.0.2.tar` & `elliptic_sdk-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0       21 2023-04-19 13:32:23.004077 elliptic_sdk-0.0.2/elliptic_sdk/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-19 14:15:46.386875 elliptic_sdk-0.0.2/elliptic_sdk/aml.py
--rw-r--r--   0        0        0      165 2023-04-19 13:47:35.835487 elliptic_sdk-0.0.2/elliptic_sdk/enums.py
--rw-r--r--   0        0        0     1479 2023-04-26 10:56:28.366239 elliptic_sdk-0.0.2/elliptic_sdk/schemas.py
--rw-r--r--   0        0        0      310 2023-04-19 13:30:59.908133 elliptic_sdk-0.0.2/elliptic_sdk/settings.py
--rw-r--r--   0        0        0      615 2023-04-19 14:32:26.250874 elliptic_sdk-0.0.2/elliptic_sdk/test_aml.py
--rw-r--r--   0        0        0      440 2023-04-26 10:57:43.463966 elliptic_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.3/LICENSE
+-rw-r--r--   0        0        0       21 2023-04-19 13:32:23.004077 elliptic_sdk-0.0.3/elliptic_sdk/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-19 14:15:46.386875 elliptic_sdk-0.0.3/elliptic_sdk/aml.py
+-rw-r--r--   0        0        0      165 2023-04-19 13:47:35.835487 elliptic_sdk-0.0.3/elliptic_sdk/enums.py
+-rw-r--r--   0        0        0     1479 2023-04-26 10:56:28.366239 elliptic_sdk-0.0.3/elliptic_sdk/schemas.py
+-rw-r--r--   0        0        0      310 2023-04-19 13:30:59.908133 elliptic_sdk-0.0.3/elliptic_sdk/settings.py
+-rw-r--r--   0        0        0     1044 2023-04-26 11:29:27.668205 elliptic_sdk-0.0.3/elliptic_sdk/test_aml.py
+-rw-r--r--   0        0        0      440 2023-04-26 11:29:54.300864 elliptic_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.3/PKG-INFO
```

### Comparing `elliptic_sdk-0.0.2/LICENSE` & `elliptic_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.2/elliptic_sdk/aml.py` & `elliptic_sdk-0.0.3/elliptic_sdk/aml.py`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.2/elliptic_sdk/schemas.py` & `elliptic_sdk-0.0.3/elliptic_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.2/PKG-INFO` & `elliptic_sdk-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elliptic-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Elliptic SDK
 Author: Olexandr Shalakhin
 Author-email: olexandr@shalakhin.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

