# Comparing `tmp/batchx-9.7.1.tar.gz` & `tmp/batchx-9.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchx-9.7.1.tar", last modified: Wed Apr 26 10:40:01 2023, max compression
+gzip compressed data, was "batchx-9.7.2.tar", last modified: Wed Apr 26 15:33:07 2023, max compression
```

## Comparing `batchx-9.7.1.tar` & `batchx-9.7.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.610843 batchx-9.7.1/
--rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:40:01.610843 batchx-9.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.7.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.602842 batchx-9.7.1/batchx/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/admin_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13599 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/admin_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5445 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/alert_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/alert_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6011 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/audit_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/audit_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7926 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/auth_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18170 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/auth_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/billing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48012 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/bx.py
--rw-r--r--   0 root         (0) root         (0)     5608 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3160 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/consumer_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/consumer_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/docker_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/docker_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/environment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5829 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/environment_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26134 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/filesystem_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28037 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/filesystem_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3893 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26939 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/image_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22798 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26615 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24930 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/log_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/log_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8460 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/organization_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16168 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/organization_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5606 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/picture_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/picture_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/profile_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/profile_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8419 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/provider_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/provider_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6509 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/tag_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9944 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/tag_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/token_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/token_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/user_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.610843 batchx-9.7.1/batchx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1226 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:40:01.610843 batchx-9.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.7.1/setup.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 10:40:00.000000 batchx-9.7.1/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:07.387352 batchx-9.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 15:33:07.387352 batchx-9.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.7.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.7.2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:07.387352 batchx-9.7.2/batchx/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/admin_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13599 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/admin_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/alert_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/alert_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/audit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/audit_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7926 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/auth_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18170 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/auth_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/billing_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48012 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/bx.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/consumer_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/consumer_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/docker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/docker_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/environment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/environment_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26131 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/filesystem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28037 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/filesystem_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26939 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22798 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26615 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24930 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/log_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/log_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8460 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/organization_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16168 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/organization_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5606 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/picture_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/picture_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/profile_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/profile_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/provider_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/provider_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6509 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/tag_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/tag_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/token_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/token_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-04-26 15:33:06.000000 batchx-9.7.2/batchx/user_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:33:07.387352 batchx-9.7.2/batchx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 15:33:07.000000 batchx-9.7.2/batchx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-04-26 15:33:07.000000 batchx-9.7.2/batchx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:33:07.000000 batchx-9.7.2/batchx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-26 15:33:07.000000 batchx-9.7.2/batchx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 15:33:07.000000 batchx-9.7.2/batchx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:33:07.387352 batchx-9.7.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.7.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 15:33:06.000000 batchx-9.7.2/version
```

### Comparing `batchx-9.7.1/PKG-INFO` & `batchx-9.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.1
+Version: 9.7.2
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.1/README.md` & `batchx-9.7.2/README.md`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/admin_pb2.py` & `batchx-9.7.2/batchx/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/admin_pb2_grpc.py` & `batchx-9.7.2/batchx/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/alert_pb2.py` & `batchx-9.7.2/batchx/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/alert_pb2_grpc.py` & `batchx-9.7.2/batchx/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/audit_pb2.py` & `batchx-9.7.2/batchx/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/audit_pb2_grpc.py` & `batchx-9.7.2/batchx/audit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/auth_pb2.py` & `batchx-9.7.2/batchx/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/auth_pb2_grpc.py` & `batchx-9.7.2/batchx/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/billing_pb2.py` & `batchx-9.7.2/batchx/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/billing_pb2_grpc.py` & `batchx-9.7.2/batchx/billing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/bx.py` & `batchx-9.7.2/batchx/bx.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/common_pb2.py` & `batchx-9.7.2/batchx/common_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/consumer_pb2.py` & `batchx-9.7.2/batchx/consumer_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/consumer_pb2_grpc.py` & `batchx-9.7.2/batchx/consumer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/docker_pb2.py` & `batchx-9.7.2/batchx/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/environment_pb2.py` & `batchx-9.7.2/batchx/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/environment_pb2_grpc.py` & `batchx-9.7.2/batchx/environment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/filesystem_pb2.py` & `batchx-9.7.2/batchx/filesystem_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from . import log_pb2 as log__pb2
 from . import tag_pb2 as tag__pb2
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"\xd9\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"\x16\n\x14ListS3BucketsRequest\"\xd6\x02\n\x15ListS3BucketsResponse\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12?\n\x06\x62ucket\x18\x02 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12\x42\n\x05users\x18\x03 \x03(\x0b\x32\x33.batchx.filesystem.ListS3BucketsResponse.UsersEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"A\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf8\r\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"\xd9\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"+\n\x14ListS3BucketsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\"\xc1\x02\n\x15ListS3BucketsResponse\x12?\n\x06\x62ucket\x18\x01 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12\x42\n\x05users\x18\x02 \x03(\x0b\x32\x33.batchx.filesystem.ListS3BucketsResponse.UsersEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"A\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf8\r\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'filesystem_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017io.batchx.protoB\017FilesystemProto'
@@ -77,16 +77,16 @@
   _ADDS3BUCKETREQUEST._serialized_start=76
   _ADDS3BUCKETREQUEST._serialized_end=293
   _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_start=212
   _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_end=293
   _ADDS3BUCKETRESPONSE._serialized_start=295
   _ADDS3BUCKETRESPONSE._serialized_end=316
   _LISTS3BUCKETSREQUEST._serialized_start=318
-  _LISTS3BUCKETSREQUEST._serialized_end=340
-  _LISTS3BUCKETSRESPONSE._serialized_start=343
+  _LISTS3BUCKETSREQUEST._serialized_end=361
+  _LISTS3BUCKETSRESPONSE._serialized_start=364
   _LISTS3BUCKETSRESPONSE._serialized_end=685
   _LISTS3BUCKETSRESPONSE_BUCKET._serialized_start=522
   _LISTS3BUCKETSRESPONSE_BUCKET._serialized_end=618
   _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_start=620
   _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_end=685
   _REMOVES3BUCKETREQUEST._serialized_start=687
   _REMOVES3BUCKETREQUEST._serialized_end=752
```

### Comparing `batchx-9.7.1/batchx/filesystem_pb2_grpc.py` & `batchx-9.7.2/batchx/filesystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/health_pb2.py` & `batchx-9.7.2/batchx/health_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/health_pb2_grpc.py` & `batchx-9.7.2/batchx/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/image_pb2.py` & `batchx-9.7.2/batchx/image_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/image_pb2_grpc.py` & `batchx-9.7.2/batchx/image_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/job_pb2.py` & `batchx-9.7.2/batchx/job_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/job_pb2_grpc.py` & `batchx-9.7.2/batchx/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/log_pb2.py` & `batchx-9.7.2/batchx/log_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/organization_pb2.py` & `batchx-9.7.2/batchx/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/organization_pb2_grpc.py` & `batchx-9.7.2/batchx/organization_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/picture_pb2.py` & `batchx-9.7.2/batchx/picture_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/picture_pb2_grpc.py` & `batchx-9.7.2/batchx/picture_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/profile_pb2.py` & `batchx-9.7.2/batchx/profile_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/provider_pb2.py` & `batchx-9.7.2/batchx/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/provider_pb2_grpc.py` & `batchx-9.7.2/batchx/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/tag_pb2.py` & `batchx-9.7.2/batchx/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/tag_pb2_grpc.py` & `batchx-9.7.2/batchx/tag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/token_pb2.py` & `batchx-9.7.2/batchx/token_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/token_pb2_grpc.py` & `batchx-9.7.2/batchx/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/user_pb2.py` & `batchx-9.7.2/batchx/user_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx/user_pb2_grpc.py` & `batchx-9.7.2/batchx/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/batchx.egg-info/PKG-INFO` & `batchx-9.7.2/batchx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.1
+Version: 9.7.2
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.1/batchx.egg-info/SOURCES.txt` & `batchx-9.7.2/batchx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchx-9.7.1/setup.py` & `batchx-9.7.2/setup.py`

 * *Files identical despite different names*

