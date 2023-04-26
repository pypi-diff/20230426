# Comparing `tmp/fusion-platform-python-sdk-1.6.6.tar.gz` & `tmp/fusion-platform-python-sdk-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.6.6.tar", last modified: Tue Mar 28 14:01:15 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.6.7.tar", last modified: Tue Apr 25 06:53:21 2023, max compression
```

## Comparing `fusion-platform-python-sdk-1.6.6.tar` & `fusion-platform-python-sdk-1.6.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-03-28 14:01:15.243063 fusion-platform-python-sdk-1.6.6/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.6.6/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.6.6/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-03-28 14:01:15.242781 fusion-platform-python-sdk-1.6.6/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.6.6/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-03-28 14:01:15.228723 fusion-platform-python-sdk-1.6.6/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-03-28 14:01:12.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-03-28 14:01:15.230645 fusion-platform-python-sdk-1.6.6/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1547331 2023-02-08 14:50:52.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-03-28 14:01:15.240286 fusion-platform-python-sdk-1.6.6/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    30748 2023-01-13 10:46:35.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12611 2022-06-27 13:48:00.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    37551 2023-01-27 11:38:30.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2495 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8037 2022-07-15 08:38:26.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3264 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10365 2022-06-16 08:00:49.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9709 2022-08-19 10:03:50.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-03-28 14:01:13.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7233 2023-03-28 14:01:12.000000 fusion-platform-python-sdk-1.6.6/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-03-28 14:01:15.242341 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-03-28 14:01:15.000000 fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-03-28 14:01:15.243165 fusion-platform-python-sdk-1.6.6/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-03-28 14:01:12.000000 fusion-platform-python-sdk-1.6.6/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-04-25 06:53:21.241762 fusion-platform-python-sdk-1.6.7/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.6.7/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.6.7/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-04-25 06:53:21.241490 fusion-platform-python-sdk-1.6.7/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2022-09-01 10:14:11.000000 fusion-platform-python-sdk-1.6.7/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-04-25 06:53:21.226105 fusion-platform-python-sdk-1.6.7/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     6806 2023-04-25 06:53:18.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-04-25 06:53:21.228158 fusion-platform-python-sdk-1.6.7/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1547331 2023-02-08 14:50:52.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-02-15 10:52:50.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-04-25 06:53:21.238923 fusion-platform-python-sdk-1.6.7/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    30748 2023-01-13 10:46:35.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12611 2022-06-27 13:48:00.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    37970 2023-04-25 06:29:47.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2495 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8125 2023-04-25 06:39:57.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3264 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10365 2022-06-16 08:00:49.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9709 2022-08-19 10:03:50.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-04-25 06:53:19.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7233 2023-04-25 06:53:18.000000 fusion-platform-python-sdk-1.6.7/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-04-25 06:53:21.241034 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1704 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-04-25 06:53:21.000000 fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-04-25 06:53:21.241871 fusion-platform-python-sdk-1.6.7/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-04-25 06:53:18.000000 fusion-platform-python-sdk-1.6.7/setup.py
```

### Comparing `fusion-platform-python-sdk-1.6.6/LICENSE.txt` & `fusion-platform-python-sdk-1.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/PKG-INFO` & `fusion-platform-python-sdk-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.6.6/README.md` & `fusion-platform-python-sdk-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.6.6'
-__version_date__ = '2023-03-28T14:01:12Z'
+__version__ = '1.6.7'
+__version_date__ = '2023-04-25T06:53:18Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
```

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/base.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.6.7/fusion_platform/fusion_platform_sdk.pdf`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/glasgow.geojson` & `fusion-platform-python-sdk-1.6.7/fusion_platform/glasgow.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/lake_district.geojson` & `fusion-platform-python-sdk-1.6.7/fusion_platform/lake_district.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/model.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/organisation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,26 +407,37 @@
         Attempts to execute the created process in the Fusion Platform<sup>&reg;</sup>. Optionally waits for the next execution to start, and then for it to complete.
 
         Args:
             wait: Optionally wait for the next execution to start and complete? Default False.
 
         Raises:
             RequestError: if the execute fails.
-            ModelError: if the execution fails.
+            ModelError: if any execution fails.
         """
         # Send the request and load the resulting model.
         self._send_and_load(self._get_path(self.__class__._PATH_EXECUTE), method=Session.METHOD_POST)
 
         if wait:
             # If we are waiting for the execution to complete, wait for the next execution to start...
             self.wait_for_next_execution()
 
-            # ...and for all the executions to complete.
+            # ...and for all the executions to complete. Note that we wait for all executions to complete, even if at least one has failed.
+            exception = None
+
             for execution in self.executions:
-                execution.check_complete(wait=wait)
+                try:
+                    execution.check_complete(wait=wait)
+                except ModelError as e:
+                    # Keep the first exception raised.
+                    if exception is None:
+                        exception = e
+
+            # Raise any exception.
+            if exception is not None:
+                raise exception
 
     @property
     def executions(self):
         """
         Provides an iterator through the process's executions.
 
         Returns:
```

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 
             # See if the execution has completed.
             self._logger.debug('checking for execution %s to complete: %f', self.id, self.progress)
             complete = self.progress >= 100
 
             # Raise an exception if the execution failed.
             if complete and not self.success:
+                self._logger.error(i18n.t('models.process_execution.execution_failed'))
                 raise ModelError(i18n.t('models.process_execution.execution_failed'))
 
             if complete:
                 self._logger.debug('execution %s is complete', self.id)
 
             if (not wait) or complete:
                 break
```

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/service.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/session.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.6.7/fusion_platform/translations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.6.6
+Version: 1.6.7
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.6.6/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.6.7/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.6.6/setup.py` & `fusion-platform-python-sdk-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.6.6',
+    version='1.6.7',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
```

