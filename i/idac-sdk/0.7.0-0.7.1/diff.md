# Comparing `tmp/idac_sdk-0.7.0.tar.gz` & `tmp/idac_sdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idac_sdk-0.7.0.tar", last modified: Fri Sep 30 15:02:24 2022, max compression
+gzip compressed data, was "idac_sdk-0.7.1.tar", last modified: Tue Apr 25 16:27:54 2023, max compression
```

## Comparing `idac_sdk-0.7.0.tar` & `idac_sdk-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.382854 idac_sdk-0.7.0/
--rw-r--r--   0 vkumov     (501) staff       (20)      828 2022-09-30 15:02:24.382521 idac_sdk-0.7.0/PKG-INFO
--rw-r--r--   0 vkumov     (501) staff       (20)      126 2022-03-04 15:54:41.000000 idac_sdk-0.7.0/README.md
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.358669 idac_sdk-0.7.0/idac_sdk/
--rw-r--r--   0 vkumov     (501) staff       (20)      513 2022-04-20 11:23:12.000000 idac_sdk-0.7.0/idac_sdk/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)       22 2022-09-30 13:11:40.000000 idac_sdk-0.7.0/idac_sdk/_version.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.362391 idac_sdk-0.7.0/idac_sdk/asynced/
--rw-r--r--   0 vkumov     (501) staff       (20)       39 2022-04-21 13:26:08.000000 idac_sdk-0.7.0/idac_sdk/asynced/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3191 2022-04-21 13:18:14.000000 idac_sdk-0.7.0/idac_sdk/asynced/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)    13218 2022-09-30 14:07:20.000000 idac_sdk-0.7.0/idac_sdk/asynced/request.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.363715 idac_sdk-0.7.0/idac_sdk/base/
--rw-r--r--   0 vkumov     (501) staff       (20)      775 2022-04-21 15:57:46.000000 idac_sdk-0.7.0/idac_sdk/base/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)    10257 2022-04-21 13:16:40.000000 idac_sdk-0.7.0/idac_sdk/base/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)     6462 2022-09-30 14:15:09.000000 idac_sdk-0.7.0/idac_sdk/base/request.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.365600 idac_sdk-0.7.0/idac_sdk/cli/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 10:42:29.000000 idac_sdk-0.7.0/idac_sdk/cli/__init__.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.369756 idac_sdk-0.7.0/idac_sdk/cli/commands/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 14:57:36.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      971 2022-03-08 12:09:25.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/cleanup.py
--rw-r--r--   0 vkumov     (501) staff       (20)     4674 2022-03-18 16:42:32.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/config.py
--rw-r--r--   0 vkumov     (501) staff       (20)     5166 2022-09-30 14:31:38.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/create.py
--rw-r--r--   0 vkumov     (501) staff       (20)      854 2022-03-08 12:10:08.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/extend.py
--rw-r--r--   0 vkumov     (501) staff       (20)      754 2022-03-08 12:10:43.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/restart.py
--rw-r--r--   0 vkumov     (501) staff       (20)     1685 2022-03-22 16:48:08.000000 idac_sdk-0.7.0/idac_sdk/cli/commands/status.py
--rw-r--r--   0 vkumov     (501) staff       (20)      941 2022-03-08 12:49:55.000000 idac_sdk-0.7.0/idac_sdk/cli/idac.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.376115 idac_sdk-0.7.0/idac_sdk/cli/lib/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-01 14:23:45.000000 idac_sdk-0.7.0/idac_sdk/cli/lib/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2100 2022-03-18 16:42:32.000000 idac_sdk-0.7.0/idac_sdk/cli/lib/_controller_options.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2514 2022-09-30 14:54:39.000000 idac_sdk-0.7.0/idac_sdk/cli/lib/_helpers.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2563 2022-04-22 08:11:32.000000 idac_sdk-0.7.0/idac_sdk/cli/lib/_vpn_options.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.376629 idac_sdk-0.7.0/idac_sdk/config/
--rw-r--r--   0 vkumov     (501) staff       (20)     2219 2022-03-18 11:31:57.000000 idac_sdk-0.7.0/idac_sdk/config/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      832 2022-03-22 16:53:21.000000 idac_sdk-0.7.0/idac_sdk/errors.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.377315 idac_sdk-0.7.0/idac_sdk/lib/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-18 11:31:57.000000 idac_sdk-0.7.0/idac_sdk/lib/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      648 2022-09-30 14:30:13.000000 idac_sdk-0.7.0/idac_sdk/lib/_helpers.py
--rw-r--r--   0 vkumov     (501) staff       (20)      703 2022-04-21 12:26:37.000000 idac_sdk-0.7.0/idac_sdk/log.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.379610 idac_sdk-0.7.0/idac_sdk/models/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-02-15 16:51:03.000000 idac_sdk-0.7.0/idac_sdk/models/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      123 2022-03-18 16:42:32.000000 idac_sdk-0.7.0/idac_sdk/models/auth.py
--rw-r--r--   0 vkumov     (501) staff       (20)      435 2022-03-18 16:42:32.000000 idac_sdk-0.7.0/idac_sdk/models/config.py
--rw-r--r--   0 vkumov     (501) staff       (20)      460 2022-02-16 10:03:45.000000 idac_sdk-0.7.0/idac_sdk/models/new_request.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3344 2022-04-22 08:28:14.000000 idac_sdk-0.7.0/idac_sdk/models/request_state.py
--rw-r--r--   0 vkumov     (501) staff       (20)      758 2022-04-20 11:23:00.000000 idac_sdk-0.7.0/idac_sdk/models/vpn_config.py
--rw-r--r--   0 vkumov     (501) staff       (20)     6207 2022-09-30 13:38:55.000000 idac_sdk-0.7.0/idac_sdk/session_data.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.381991 idac_sdk-0.7.0/idac_sdk/synced/
--rw-r--r--   0 vkumov     (501) staff       (20)       38 2022-02-28 15:43:21.000000 idac_sdk-0.7.0/idac_sdk/synced/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3302 2022-04-21 13:17:55.000000 idac_sdk-0.7.0/idac_sdk/synced/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)    13042 2022-09-30 14:07:15.000000 idac_sdk-0.7.0/idac_sdk/synced/request.py
--rw-r--r--   0 vkumov     (501) staff       (20)      734 2022-03-18 11:31:57.000000 idac_sdk-0.7.0/idac_sdk/types.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2022-09-30 15:02:24.361180 idac_sdk-0.7.0/idac_sdk.egg-info/
--rw-r--r--   0 vkumov     (501) staff       (20)      828 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vkumov     (501) staff       (20)     1239 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vkumov     (501) staff       (20)        1 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vkumov     (501) staff       (20)       48 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/entry_points.txt
--rw-r--r--   0 vkumov     (501) staff       (20)      130 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/requires.txt
--rw-r--r--   0 vkumov     (501) staff       (20)        9 2022-09-30 15:02:24.000000 idac_sdk-0.7.0/idac_sdk.egg-info/top_level.txt
--rw-r--r--   0 vkumov     (501) staff       (20)       38 2022-09-30 15:02:24.382973 idac_sdk-0.7.0/setup.cfg
--rw-r--r--   0 vkumov     (501) staff       (20)     1711 2022-04-21 16:08:30.000000 idac_sdk-0.7.0/setup.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.739950 idac_sdk-0.7.1/
+-rw-r--r--   0 vkumov     (501) staff       (20)      828 2023-04-25 16:27:54.739635 idac_sdk-0.7.1/PKG-INFO
+-rw-r--r--   0 vkumov     (501) staff       (20)      126 2022-03-04 15:54:41.000000 idac_sdk-0.7.1/README.md
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.716168 idac_sdk-0.7.1/idac_sdk/
+-rw-r--r--   0 vkumov     (501) staff       (20)      513 2022-04-20 11:23:12.000000 idac_sdk-0.7.1/idac_sdk/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)       22 2023-04-25 16:27:24.000000 idac_sdk-0.7.1/idac_sdk/_version.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.721219 idac_sdk-0.7.1/idac_sdk/asynced/
+-rw-r--r--   0 vkumov     (501) staff       (20)       39 2022-04-21 13:26:08.000000 idac_sdk-0.7.1/idac_sdk/asynced/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     3191 2022-04-21 13:18:14.000000 idac_sdk-0.7.1/idac_sdk/asynced/controller.py
+-rw-r--r--   0 vkumov     (501) staff       (20)    13215 2023-04-25 16:25:48.000000 idac_sdk-0.7.1/idac_sdk/asynced/request.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.723011 idac_sdk-0.7.1/idac_sdk/base/
+-rw-r--r--   0 vkumov     (501) staff       (20)      775 2022-04-21 15:57:46.000000 idac_sdk-0.7.1/idac_sdk/base/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)    10216 2023-04-25 16:25:56.000000 idac_sdk-0.7.1/idac_sdk/base/controller.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     6462 2022-09-30 14:15:09.000000 idac_sdk-0.7.1/idac_sdk/base/request.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.724010 idac_sdk-0.7.1/idac_sdk/cli/
+-rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 10:42:29.000000 idac_sdk-0.7.1/idac_sdk/cli/__init__.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.728611 idac_sdk-0.7.1/idac_sdk/cli/commands/
+-rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 14:57:36.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      971 2022-03-08 12:09:25.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/cleanup.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     4674 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/config.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     5164 2023-04-25 16:26:02.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/create.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      854 2022-03-08 12:10:08.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/extend.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      754 2022-03-08 12:10:43.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/restart.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     1685 2022-03-22 16:48:08.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/status.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      941 2022-03-08 12:49:55.000000 idac_sdk-0.7.1/idac_sdk/cli/idac.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.731019 idac_sdk-0.7.1/idac_sdk/cli/lib/
+-rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-01 14:23:45.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     2100 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_controller_options.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     2512 2023-04-25 16:26:09.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_helpers.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     2563 2022-04-22 08:11:32.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_vpn_options.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.731744 idac_sdk-0.7.1/idac_sdk/config/
+-rw-r--r--   0 vkumov     (501) staff       (20)     2219 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/config/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      832 2022-03-22 16:53:21.000000 idac_sdk-0.7.1/idac_sdk/errors.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.733115 idac_sdk-0.7.1/idac_sdk/lib/
+-rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/lib/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      646 2023-04-25 16:26:14.000000 idac_sdk-0.7.1/idac_sdk/lib/_helpers.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      703 2022-04-21 12:26:37.000000 idac_sdk-0.7.1/idac_sdk/log.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.737072 idac_sdk-0.7.1/idac_sdk/models/
+-rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-02-15 16:51:03.000000 idac_sdk-0.7.1/idac_sdk/models/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      123 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/models/auth.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      435 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/models/config.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      460 2022-02-16 10:03:45.000000 idac_sdk-0.7.1/idac_sdk/models/new_request.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     3344 2022-04-22 08:28:14.000000 idac_sdk-0.7.1/idac_sdk/models/request_state.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      758 2022-04-20 11:23:00.000000 idac_sdk-0.7.1/idac_sdk/models/vpn_config.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     6204 2023-04-25 16:25:39.000000 idac_sdk-0.7.1/idac_sdk/session_data.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.739022 idac_sdk-0.7.1/idac_sdk/synced/
+-rw-r--r--   0 vkumov     (501) staff       (20)       38 2022-02-28 15:43:21.000000 idac_sdk-0.7.1/idac_sdk/synced/__init__.py
+-rw-r--r--   0 vkumov     (501) staff       (20)     3302 2022-04-21 13:17:55.000000 idac_sdk-0.7.1/idac_sdk/synced/controller.py
+-rw-r--r--   0 vkumov     (501) staff       (20)    13039 2023-04-25 16:26:20.000000 idac_sdk-0.7.1/idac_sdk/synced/request.py
+-rw-r--r--   0 vkumov     (501) staff       (20)      734 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/types.py
+drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.719439 idac_sdk-0.7.1/idac_sdk.egg-info/
+-rw-r--r--   0 vkumov     (501) staff       (20)      828 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vkumov     (501) staff       (20)     1239 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vkumov     (501) staff       (20)        1 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vkumov     (501) staff       (20)       48 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 vkumov     (501) staff       (20)      118 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/requires.txt
+-rw-r--r--   0 vkumov     (501) staff       (20)        9 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vkumov     (501) staff       (20)       38 2023-04-25 16:27:54.740059 idac_sdk-0.7.1/setup.cfg
+-rw-r--r--   0 vkumov     (501) staff       (20)     1688 2023-04-25 16:25:29.000000 idac_sdk-0.7.1/setup.py
```

### Comparing `idac_sdk-0.7.0/PKG-INFO` & `idac_sdk-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idac_sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `idac_sdk-0.7.0/idac_sdk/__init__.py` & `idac_sdk-0.7.1/idac_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/asynced/controller.py` & `idac_sdk-0.7.1/idac_sdk/asynced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/asynced/request.py` & `idac_sdk-0.7.1/idac_sdk/asynced/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from httpx import AsyncClient, Request
-import ujson
+import json
 import asyncio
 from typing import Dict, List, Optional, Tuple, Union
 
 from idac_sdk.base import (
     DEFAULT_WAIT_INTERVAL,
     DEFAULT_WAIT_TIMEOUT,
     REQUEST_ERROR_STATES,
@@ -129,15 +129,15 @@
                 r = await client.send(request=request)
                 logger.debug(f"Got response: {r.status_code} {r.reason_phrase}")
                 if r.status_code < 200 or r.status_code > 399:
                     r.raise_for_status()
 
                 json_body: dict
                 try:
-                    json_body = ujson.loads(r.text)
+                    json_body = json.loads(r.text)
                 except Exception as e:
                     logger.debug(f"Failed to parse JSON body: {e}")
                     if r.next_request:
                         self.raise_if_error(r.next_request.url)
                         logger.debug(f"Have next request, going there: {r.next_request.url}")
                         # update request and increase redirects counter
                         request = r.next_request
@@ -182,15 +182,15 @@
 
         async with AsyncClient() as client:
             client.headers.update({"User-Agent": self.user_agent})
             r = await client.request(method, api, headers=headers)
             if r.status_code < 200 or r.status_code > 399:
                 r.raise_for_status()
 
-            json_body: dict = ujson.loads(r.text)
+            json_body: dict = json.loads(r.text)
             return RequestState(**json_body)
 
     @check_controller
     async def restart(self) -> None:
         """Restarts request
 
         Raises:
```

### Comparing `idac_sdk-0.7.0/idac_sdk/base/__init__.py` & `idac_sdk-0.7.1/idac_sdk/base/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/base/controller.py` & `idac_sdk-0.7.1/idac_sdk/base/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Optional, Tuple, Union
-import ujson
+import json
 import httpx
 from base64 import b64encode
 import warnings
 from operator import itemgetter
 from idac_sdk.lib._helpers import get_worker_hash
 from idac_sdk.models.auth import Auth
 
@@ -80,23 +80,18 @@
             raise IncorrectControllerURLError("Controller URL not provided")
 
         self.user_agent = user_agent if user_agent else DEFAULT_USER_AGENT
         self.api_version = api_version if api_version else cfg.defaults.api_version
 
         auth_type = auth_type if auth_type else IDACAuthType[cfg.defaults.auth.type]
         params: dict[str, str] = {}
-        if (
-            auth
-            and isinstance(auth, str)
-            and auth_type
-            not in [
+        if (auth and isinstance(auth, str) and auth_type not in [
                 IDACAuthType.DCLOUD_SESSION.name,
                 IDACAuthType.NONE.name,
-            ]
-        ):
+        ]):
             params = {"token": auth}
         elif auth_type == IDACAuthType.BASIC.name:
             if isinstance(auth, list):
                 params = {
                     "token": b64encode(bytes(f"{auth[0]}:{auth[1]}", "utf-8")).decode("utf-8")
                 }
         elif auth_type == IDACAuthType.WORKER.name:
@@ -257,16 +252,17 @@
 
     def drop_auth(self) -> None:
         """Resets Auth"""
         if self.auth and self.auth.params and "token" in self.auth.params:
             del self.auth.params["token"]
 
     def get_auth_token_pre(
-        self, creds: str = "", datacenter: str = ""
-    ) -> Union[str, Tuple[str, dict[str, str], dict[str, str]]]:
+            self,
+            creds: str = "",
+            datacenter: str = "") -> Union[str, Tuple[str, dict[str, str], dict[str, str]]]:
         if not self.auth:
             raise NoAuth("No Auth defined")
 
         logger.debug("Getting auth")
         if self.auth and self.auth.params and "token" in self.auth.params:
             return self.auth.params["token"]
 
@@ -289,14 +285,14 @@
         if response.status_code == 404:
             # old controller, no support for auth/token API, ignore :)
             logger.debug("Looks like controller doesn't support authentication. Ignoring")
             if use_as_auth:
                 self.auth.params["token"] = "empty_token"
             return "empty_token"
         response.raise_for_status()
-        json_body = ujson.loads(response.text)
+        json_body = json.loads(response.text)
         if isinstance(json_body, dict) and json_body.get("token", None):
             if use_as_auth:
                 logger.debug("Saving token for future authentications")
                 self.auth.params["token"] = json_body["token"]
             return json_body["token"]
         raise NoAuthTokenInResponse("Didn't receive auth token from controller")
```

### Comparing `idac_sdk-0.7.0/idac_sdk/base/request.py` & `idac_sdk-0.7.1/idac_sdk/base/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/cleanup.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/config.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/create.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncclick as click
-import ujson
+import json
 from jsonpath_ng import parse
 
 from idac_sdk import (
     IDACRequestAsync,
     IDACRequestType,
     SessionData,
 )
@@ -176,8 +176,8 @@
     with click.open_file(file, "w") as f:
         if out_path:
             for o in out_path:
                 jsonpath_expr = parse(o)
                 for match in jsonpath_expr.find(state_dict):
                     f.write(f"{match.value}\n")
         else:
-            f.write(ujson.dumps(state_dict))
+            f.write(json.dumps(state_dict))
```

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/extend.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/extend.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/restart.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/restart.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/commands/status.py` & `idac_sdk-0.7.1/idac_sdk/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/idac.py` & `idac_sdk-0.7.1/idac_sdk/cli/idac.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/lib/_controller_options.py` & `idac_sdk-0.7.1/idac_sdk/cli/lib/_controller_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/lib/_helpers.py` & `idac_sdk-0.7.1/idac_sdk/cli/lib/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ujson
+import json
 import platform
 from typing import List
 import asyncclick as click
 import logging
 from httpx import URL
 
 from idac_sdk.log import logger
@@ -55,15 +55,15 @@
         return parsed
 
     return None
 
 
 def parse_json(ctx, param, raw: str):
     if raw is not None:
-        return ujson.loads(raw)
+        return json.loads(raw)
 
 
 DEFAULT_OUTPUT_UNIX = r"/dcloud/idac_sdk.out"
 DEFAULT_OUTPUT_WIN = r"c:\dcloud\idac_sdk.out"
 
 
 def default_output(ctx, param, raw: str):
```

### Comparing `idac_sdk-0.7.0/idac_sdk/cli/lib/_vpn_options.py` & `idac_sdk-0.7.1/idac_sdk/cli/lib/_vpn_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/config/__init__.py` & `idac_sdk-0.7.1/idac_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/errors.py` & `idac_sdk-0.7.1/idac_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/lib/_helpers.py` & `idac_sdk-0.7.1/idac_sdk/lib/_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from base64 import b64encode
 from functools import cache
 import hashlib
 import secrets
 from time import time
-import ujson
+import json
 
 
 def get_worker_hash(client_id: str, secret: str) -> str:
     timestamp = time.time()
     nonce = secrets.token_urlsafe()
     token_payload = {
         'client_id': client_id,
         'timestamp': timestamp,
         'access_token': hash_token(f"{secret}.{timestamp}.{nonce}"),
         'nonce': nonce
     }
-    return ujson.dumps(token_payload)
+    return json.dumps(token_payload)
 
 
 @cache
 def hash_token(payload: str) -> str:
     hasher = hashlib.sha3_256()
     hasher.update(payload.encode())
     digest = b64encode(hasher.digest()).decode()
```

### Comparing `idac_sdk-0.7.0/idac_sdk/log.py` & `idac_sdk-0.7.1/idac_sdk/log.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/models/request_state.py` & `idac_sdk-0.7.1/idac_sdk/models/request_state.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/models/vpn_config.py` & `idac_sdk-0.7.1/idac_sdk/models/vpn_config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/session_data.py` & `idac_sdk-0.7.1/idac_sdk/session_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 import os.path
 from warnings import warn
 import xmltodict
-import ujson
+import json
 from typing import Any, Dict, Literal, Optional, Union
 from deepmerge import always_merger
 
 from idac_sdk.errors import (
     BadXmlFileError,
     IncorrectSessionData,
     SessionDataFileNotFoundError,
@@ -112,15 +112,15 @@
             else:
                 warn(f"session.xml not found by path '{file}'.", SessionDataFileNotFoundWarning)
                 return
 
         d = None
         with open(file, "r") as file_handle:
             d = xmltodict.parse(file_handle.read())
-            d = ujson.loads(ujson.dumps(d))
+            d = json.loads(json.dumps(d))
 
         if isinstance(d, dict):
             if "session" in d:
                 new_data = NewRequest(**d["session"])
             else:
                 new_data = NewRequest(**d)
```

### Comparing `idac_sdk-0.7.0/idac_sdk/synced/controller.py` & `idac_sdk-0.7.1/idac_sdk/synced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk/synced/request.py` & `idac_sdk-0.7.1/idac_sdk/synced/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from httpx import Client, Request
-import ujson
+import json
 from typing import Dict, List, Optional, Tuple, Union
 
 from idac_sdk.base import (
     DEFAULT_MAX_TRIES,
     DEFAULT_WAIT_INTERVAL,
     REQUEST_ERROR_STATES,
     REQUEST_GOOD_STATES,
@@ -126,15 +126,15 @@
                 r = client.send(request=request)
                 logger.debug(f"Got response: {r.status_code} {r.reason_phrase}")
                 if r.status_code < 200 or r.status_code > 399:
                     r.raise_for_status()
 
                 json_body: dict
                 try:
-                    json_body = ujson.loads(r.text)
+                    json_body = json.loads(r.text)
                 except Exception as e:
                     logger.debug(f"Failed to parse JSON body: {e}")
                     if r.next_request:
                         self.raise_if_error(r.next_request.url)
                         logger.debug(f"Have next request, going there: {r.next_request.url}")
                         # update request and increase redirects counter
                         request = r.next_request
@@ -179,15 +179,15 @@
 
         with Client() as client:
             client.headers.update({"User-Agent": self.user_agent})
             r = client.request(method, api, headers=headers)
             if r.status_code < 200 or r.status_code > 399:
                 r.raise_for_status()
 
-            json_body: dict = ujson.loads(r.text)
+            json_body: dict = json.loads(r.text)
             return RequestState(**json_body)
 
     @check_controller
     def restart(self) -> None:
         """Restarts request
 
         Raises:
```

### Comparing `idac_sdk-0.7.0/idac_sdk/types.py` & `idac_sdk-0.7.1/idac_sdk/types.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/idac_sdk.egg-info/PKG-INFO` & `idac_sdk-0.7.1/idac_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idac-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `idac_sdk-0.7.0/idac_sdk.egg-info/SOURCES.txt` & `idac_sdk-0.7.1/idac_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.0/setup.py` & `idac_sdk-0.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     keywords="idac sdk",
     url="https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python",
     packages=find_packages(include=["idac_sdk", "idac_sdk.*", "tests"]),
     long_description=read("README.md"),
     install_requires=[
         "asyncclick>=8.0.3.2",
         "httpx>=0.22.0",
-        "ujson>=1.35",
         "xmltodict>=0.12.0",
         "pydantic>=1.9.0",
         "deepmerge>=1.0.1",
         "PyYAML>=5.4.1",
         "jsonpath-ng>=1.5.3",
     ],
     python_requires=">=3.7",
```

