# Comparing `tmp/foursight_cgap-3.4.0.5b52.tar.gz` & `tmp/foursight_cgap-3.4.0.5b53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.4.0.5b52.tar", max compression
+gzip compressed data, was "foursight_cgap-3.4.0.5b53.tar", max compression
```

## Comparing `foursight_cgap-3.4.0.5b52.tar` & `foursight_cgap-3.4.0.5b53.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.4.0.5b52/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-08 19:59:00.537811 foursight_cgap-3.4.0.5b52/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-16 14:13:10.875303 foursight_cgap-3.4.0.5b52/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2022-11-08 19:59:00.538833 foursight_cgap-3.4.0.5b52/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4648 2023-04-14 03:05:49.302363 foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17006 2023-04-14 03:05:49.302857 foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2023-04-14 03:05:49.303368 foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2022-11-08 19:59:00.539793 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2022-11-08 19:59:00.540026 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2023-04-14 03:05:49.303951 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2023-04-14 03:05:49.304237 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-04-14 03:05:49.304663 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2022-11-08 19:59:00.540455 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2022-11-08 19:59:00.540531 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2022-11-08 19:59:00.540609 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13183 2022-11-08 19:59:00.540858 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2022-11-08 19:59:00.540938 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2022-11-08 19:59:00.541029 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2022-11-08 19:59:00.541252 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2022-11-08 19:59:00.541379 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-04-14 03:05:49.304998 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2023-04-14 03:05:49.305563 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58825 2023-04-14 03:05:49.306426 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58247 2023-04-14 03:05:49.307575 foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2022-11-08 19:59:00.542779 foursight_cgap-3.4.0.5b52/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      616 2022-11-08 19:59:00.542892 foursight_cgap-3.4.0.5b52/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      315 2023-04-14 03:05:49.308031 foursight_cgap-3.4.0.5b52/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1045 2023-04-26 14:21:10.580105 foursight_cgap-3.4.0.5b52/pyproject.toml
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 foursight_cgap-3.4.0.5b52/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.4.0.5b53/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-08 19:59:00.537811 foursight_cgap-3.4.0.5b53/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1038 2023-04-16 14:13:10.875303 foursight_cgap-3.4.0.5b53/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2022-11-08 19:59:00.538833 foursight_cgap-3.4.0.5b53/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4648 2023-04-14 03:05:49.302363 foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17006 2023-04-14 03:05:49.302857 foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-04-14 03:05:49.303368 foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2022-11-08 19:59:00.539793 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2022-11-08 19:59:00.540026 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2023-04-14 03:05:49.303951 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2023-04-14 03:05:49.304237 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-04-14 03:05:49.304663 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2022-11-08 19:59:00.540455 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2022-11-08 19:59:00.540531 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2022-11-08 19:59:00.540609 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13183 2022-11-08 19:59:00.540858 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2022-11-08 19:59:00.540938 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2022-11-08 19:59:00.541029 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2022-11-08 19:59:00.541252 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2022-11-08 19:59:00.541379 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-04-14 03:05:49.304998 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2023-04-14 03:05:49.305563 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58825 2023-04-14 03:05:49.306426 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58247 2023-04-14 03:05:49.307575 foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2022-11-08 19:59:00.542779 foursight_cgap-3.4.0.5b53/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      616 2022-11-08 19:59:00.542892 foursight_cgap-3.4.0.5b53/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      315 2023-04-14 03:05:49.308031 foursight_cgap-3.4.0.5b53/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1127 2023-04-26 14:23:29.622732 foursight_cgap-3.4.0.5b53/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 foursight_cgap-3.4.0.5b53/PKG-INFO
```

### Comparing `foursight_cgap-3.4.0.5b52/LICENSE.txt` & `foursight_cgap-3.4.0.5b53/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/app_utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/buckets.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_schedules.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_setup.json` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/deploy.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/chalicelib_cgap/package.py` & `foursight_cgap-3.4.0.5b53/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.4.0.5b52/pyproject.toml` & `foursight_cgap-3.4.0.5b53/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "3.4.0.5b52"
+version = "3.4.0.5b53"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
 
@@ -31,10 +31,13 @@
 pytest = "5.1.2"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.21.6"
 pytest-cov = "2.7.1"
 flaky = "3.6.1"
 
+[tool.poetry.scripts]
+publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `foursight_cgap-3.4.0.5b52/PKG-INFO` & `foursight_cgap-3.4.0.5b53/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 3.4.0.5b52
+Version: 3.4.0.5b53
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

