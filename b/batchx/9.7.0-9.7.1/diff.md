# Comparing `tmp/batchx-9.7.0.tar.gz` & `tmp/batchx-9.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchx-9.7.0.tar", last modified: Wed Apr 26 10:13:55 2023, max compression
+gzip compressed data, was "batchx-9.7.1.tar", last modified: Wed Apr 26 10:40:01 2023, max compression
```

## Comparing `batchx-9.7.0.tar` & `batchx-9.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:13:55.312791 batchx-9.7.0/
--rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:13:55.312791 batchx-9.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.7.0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:13:55.312791 batchx-9.7.0/batchx/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/admin_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13599 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/admin_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5445 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/alert_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/alert_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6011 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/audit_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/audit_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7926 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/auth_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18170 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/auth_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/billing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48012 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/bx.py
--rw-r--r--   0 root         (0) root         (0)     5608 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3160 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/consumer_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/consumer_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/docker_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/docker_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/environment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5829 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/environment_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26002 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/filesystem_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28037 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/filesystem_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3893 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26939 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/image_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22798 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26615 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24930 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/log_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/log_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8460 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/organization_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16168 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/organization_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5606 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/picture_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/picture_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/profile_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/profile_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8419 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/provider_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/provider_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6509 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/tag_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9944 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/tag_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/token_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/token_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-26 10:13:54.000000 batchx-9.7.0/batchx/user_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:13:55.312791 batchx-9.7.0/batchx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:13:55.000000 batchx-9.7.0/batchx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1226 2023-04-26 10:13:55.000000 batchx-9.7.0/batchx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:13:55.000000 batchx-9.7.0/batchx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-26 10:13:55.000000 batchx-9.7.0/batchx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 10:13:55.000000 batchx-9.7.0/batchx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:13:55.312791 batchx-9.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.7.0/setup.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 10:13:54.000000 batchx-9.7.0/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.610843 batchx-9.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:40:01.610843 batchx-9.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.7.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.7.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.602842 batchx-9.7.1/batchx/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/admin_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13599 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/admin_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/alert_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/alert_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/audit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/audit_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7926 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/auth_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18170 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/auth_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/billing_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48012 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/bx.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/consumer_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/consumer_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/docker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/docker_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/environment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/environment_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26134 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/filesystem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28037 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/filesystem_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26939 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22798 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26615 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24930 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/log_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/log_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8460 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/organization_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16168 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/organization_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5606 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/picture_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/picture_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/profile_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/profile_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/provider_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/provider_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6509 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/tag_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/tag_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/token_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/token_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-04-26 10:40:00.000000 batchx-9.7.1/batchx/user_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:01.610843 batchx-9.7.1/batchx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 10:40:01.000000 batchx-9.7.1/batchx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:40:01.610843 batchx-9.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.7.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 10:40:00.000000 batchx-9.7.1/version
```

### Comparing `batchx-9.7.0/PKG-INFO` & `batchx-9.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.0
+Version: 9.7.1
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.0/README.md` & `batchx-9.7.1/README.md`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/admin_pb2.py` & `batchx-9.7.1/batchx/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/admin_pb2_grpc.py` & `batchx-9.7.1/batchx/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/alert_pb2.py` & `batchx-9.7.1/batchx/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/alert_pb2_grpc.py` & `batchx-9.7.1/batchx/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/audit_pb2.py` & `batchx-9.7.1/batchx/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/audit_pb2_grpc.py` & `batchx-9.7.1/batchx/audit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/auth_pb2.py` & `batchx-9.7.1/batchx/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/auth_pb2_grpc.py` & `batchx-9.7.1/batchx/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/billing_pb2.py` & `batchx-9.7.1/batchx/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/billing_pb2_grpc.py` & `batchx-9.7.1/batchx/billing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/bx.py` & `batchx-9.7.1/batchx/bx.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/common_pb2.py` & `batchx-9.7.1/batchx/common_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/consumer_pb2.py` & `batchx-9.7.1/batchx/consumer_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/consumer_pb2_grpc.py` & `batchx-9.7.1/batchx/consumer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/docker_pb2.py` & `batchx-9.7.1/batchx/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/environment_pb2.py` & `batchx-9.7.1/batchx/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/environment_pb2_grpc.py` & `batchx-9.7.1/batchx/environment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/filesystem_pb2.py` & `batchx-9.7.1/batchx/filesystem_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from . import log_pb2 as log__pb2
 from . import tag_pb2 as tag__pb2
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"\xc4\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"\x16\n\x14ListS3BucketsRequest\"\xc1\x02\n\x15ListS3BucketsResponse\x12?\n\x06\x62ucket\x18\x01 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12\x42\n\x05users\x18\x02 \x03(\x0b\x32\x33.batchx.filesystem.ListS3BucketsResponse.UsersEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\",\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf8\r\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"\xd9\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"\x16\n\x14ListS3BucketsRequest\"\xd6\x02\n\x15ListS3BucketsResponse\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12?\n\x06\x62ucket\x18\x02 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12\x42\n\x05users\x18\x03 \x03(\x0b\x32\x33.batchx.filesystem.ListS3BucketsResponse.UsersEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"A\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf8\r\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'filesystem_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017io.batchx.protoB\017FilesystemProto'
@@ -68,146 +68,146 @@
   _FILESYSTEMSERVICE.methods_by_name['ShareFile']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['AddS3Bucket']._options = None
   _FILESYSTEMSERVICE.methods_by_name['AddS3Bucket']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['ListS3Buckets']._options = None
   _FILESYSTEMSERVICE.methods_by_name['ListS3Buckets']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['RemoveS3Bucket']._options = None
   _FILESYSTEMSERVICE.methods_by_name['RemoveS3Bucket']._serialized_options = b'\220\002\002'
-  _BLOBSTATUS._serialized_start=6998
-  _BLOBSTATUS._serialized_end=7118
+  _BLOBSTATUS._serialized_start=7061
+  _BLOBSTATUS._serialized_end=7181
   _ADDS3BUCKETREQUEST._serialized_start=76
-  _ADDS3BUCKETREQUEST._serialized_end=272
-  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_start=191
-  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_end=272
-  _ADDS3BUCKETRESPONSE._serialized_start=274
-  _ADDS3BUCKETRESPONSE._serialized_end=295
-  _LISTS3BUCKETSREQUEST._serialized_start=297
-  _LISTS3BUCKETSREQUEST._serialized_end=319
-  _LISTS3BUCKETSRESPONSE._serialized_start=322
-  _LISTS3BUCKETSRESPONSE._serialized_end=643
-  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_start=480
-  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_end=576
-  _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_start=578
-  _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_end=643
-  _REMOVES3BUCKETREQUEST._serialized_start=645
-  _REMOVES3BUCKETREQUEST._serialized_end=689
-  _REMOVES3BUCKETRESPONSE._serialized_start=691
-  _REMOVES3BUCKETRESPONSE._serialized_end=715
-  _SHAREFILEREQUEST._serialized_start=718
-  _SHAREFILEREQUEST._serialized_end=887
-  _SHAREFILEREQUEST_TYPE._serialized_start=857
-  _SHAREFILEREQUEST_TYPE._serialized_end=887
-  _SHAREFILERESPONSE._serialized_start=889
-  _SHAREFILERESPONSE._serialized_end=908
-  _SETBLOBSTATUSREQUEST._serialized_start=910
-  _SETBLOBSTATUSREQUEST._serialized_end=1016
-  _SETBLOBSTATUSRESPONSE._serialized_start=1018
-  _SETBLOBSTATUSRESPONSE._serialized_end=1041
-  _LISTBLOBPOINTERSREQUEST._serialized_start=1044
-  _LISTBLOBPOINTERSREQUEST._serialized_end=1729
-  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_start=1322
-  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_end=1485
-  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_start=1462
-  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_end=1485
-  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_start=1487
-  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_end=1566
-  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_start=1569
-  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_end=1729
-  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_start=1690
-  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_end=1729
-  _LISTBLOBPOINTERSRESPONSE._serialized_start=1732
-  _LISTBLOBPOINTERSRESPONSE._serialized_end=2001
-  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_start=1935
-  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_end=2001
-  _LISTBLOBSREQUEST._serialized_start=2004
-  _LISTBLOBSREQUEST._serialized_end=2888
-  _LISTBLOBSREQUEST_ORDER._serialized_start=2238
-  _LISTBLOBSREQUEST_ORDER._serialized_end=2439
-  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_start=2352
-  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_end=2439
-  _LISTBLOBSREQUEST_PAGINATION._serialized_start=2442
-  _LISTBLOBSREQUEST_PAGINATION._serialized_end=2600
-  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_start=2575
-  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_end=2600
-  _LISTBLOBSREQUEST_FILTERING._serialized_start=2603
-  _LISTBLOBSREQUEST_FILTERING._serialized_end=2888
-  _LISTBLOBSRESPONSE._serialized_start=2891
-  _LISTBLOBSRESPONSE._serialized_end=3143
-  _LISTBLOBSRESPONSE_USERSENTRY._serialized_start=578
-  _LISTBLOBSRESPONSE_USERSENTRY._serialized_end=643
-  _GETBLOBREQUEST._serialized_start=3145
-  _GETBLOBREQUEST._serialized_end=3198
-  _GETBLOBRESPONSE._serialized_start=3200
-  _GETBLOBRESPONSE._serialized_end=3256
-  _BLOB._serialized_start=3259
-  _BLOB._serialized_end=3646
-  _BLOB_METAINFO._serialized_start=3546
-  _BLOB_METAINFO._serialized_end=3646
-  _LISTFOLDERREQUEST._serialized_start=3649
-  _LISTFOLDERREQUEST._serialized_end=4699
-  _LISTFOLDERREQUEST_FILTERING._serialized_start=3946
-  _LISTFOLDERREQUEST_FILTERING._serialized_end=4324
-  _LISTFOLDERREQUEST_PAGINATION._serialized_start=4327
-  _LISTFOLDERREQUEST_PAGINATION._serialized_end=4484
-  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_start=1462
-  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_end=1485
-  _LISTFOLDERREQUEST_ORDER._serialized_start=4487
-  _LISTFOLDERREQUEST_ORDER._serialized_end=4699
-  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_start=4602
-  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_end=4699
-  _LISTFOLDERRESPONSE._serialized_start=4702
-  _LISTFOLDERRESPONSE._serialized_end=4965
-  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_start=1935
-  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_end=2001
-  _CREATEFOLDERREQUEST._serialized_start=4968
-  _CREATEFOLDERREQUEST._serialized_end=5146
-  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_start=5099
-  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_end=5146
-  _CREATEFOLDERRESPONSE._serialized_start=5148
-  _CREATEFOLDERRESPONSE._serialized_end=5170
-  _DELETEFOLDERREQUEST._serialized_start=5172
-  _DELETEFOLDERREQUEST._serialized_end=5228
-  _DELETEFOLDERRESPONSE._serialized_start=5230
-  _DELETEFOLDERRESPONSE._serialized_end=5252
-  _DELETEFILEREQUEST._serialized_start=5254
-  _DELETEFILEREQUEST._serialized_end=5308
-  _DELETEFILERESPONSE._serialized_start=5310
-  _DELETEFILERESPONSE._serialized_end=5366
-  _GETFILEREQUEST._serialized_start=5368
-  _GETFILEREQUEST._serialized_end=5419
-  _GETFILERESPONSE._serialized_start=5421
-  _GETFILERESPONSE._serialized_end=5519
-  _FILE._serialized_start=5522
-  _FILE._serialized_end=5878
-  _FILE_STATUS._serialized_start=5829
-  _FILE_STATUS._serialized_end=5878
-  _REPORTUPLOADSTATUSREQUEST._serialized_start=5880
-  _REPORTUPLOADSTATUSREQUEST._serialized_end=5966
-  _REPORTUPLOADSTATUSRESPONSE._serialized_start=5968
-  _REPORTUPLOADSTATUSRESPONSE._serialized_end=5996
-  _CANCELUPLOADREQUEST._serialized_start=5998
-  _CANCELUPLOADREQUEST._serialized_end=6054
-  _CANCELUPLOADRESPONSE._serialized_start=6056
-  _CANCELUPLOADRESPONSE._serialized_end=6078
-  _METADATA._serialized_start=6081
-  _METADATA._serialized_end=6313
-  _METADATA_USERDATAENTRY._serialized_start=5099
-  _METADATA_USERDATAENTRY._serialized_end=5146
-  _UPLOADPRESIGNEDREQUEST._serialized_start=6315
-  _UPLOADPRESIGNEDREQUEST._serialized_end=6421
-  _UPLOADPRESIGNEDRESPONSE._serialized_start=6424
-  _UPLOADPRESIGNEDRESPONSE._serialized_end=6584
-  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_start=6553
-  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_end=6576
-  _DOWNLOADPRESIGNEDREQUEST._serialized_start=6586
-  _DOWNLOADPRESIGNEDREQUEST._serialized_end=6690
-  _DOWNLOADPRESIGNEDRESPONSE._serialized_start=6692
-  _DOWNLOADPRESIGNEDRESPONSE._serialized_end=6779
-  _COPYREQUEST._serialized_start=6781
-  _COPYREQUEST._serialized_end=6892
-  _COMPLETEUPLOADREQUEST._serialized_start=6894
-  _COMPLETEUPLOADREQUEST._serialized_end=6970
-  _COMPLETEUPLOADRESPONSE._serialized_start=6972
-  _COMPLETEUPLOADRESPONSE._serialized_end=6996
-  _FILESYSTEMSERVICE._serialized_start=7121
-  _FILESYSTEMSERVICE._serialized_end=8905
+  _ADDS3BUCKETREQUEST._serialized_end=293
+  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_start=212
+  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_end=293
+  _ADDS3BUCKETRESPONSE._serialized_start=295
+  _ADDS3BUCKETRESPONSE._serialized_end=316
+  _LISTS3BUCKETSREQUEST._serialized_start=318
+  _LISTS3BUCKETSREQUEST._serialized_end=340
+  _LISTS3BUCKETSRESPONSE._serialized_start=343
+  _LISTS3BUCKETSRESPONSE._serialized_end=685
+  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_start=522
+  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_end=618
+  _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_start=620
+  _LISTS3BUCKETSRESPONSE_USERSENTRY._serialized_end=685
+  _REMOVES3BUCKETREQUEST._serialized_start=687
+  _REMOVES3BUCKETREQUEST._serialized_end=752
+  _REMOVES3BUCKETRESPONSE._serialized_start=754
+  _REMOVES3BUCKETRESPONSE._serialized_end=778
+  _SHAREFILEREQUEST._serialized_start=781
+  _SHAREFILEREQUEST._serialized_end=950
+  _SHAREFILEREQUEST_TYPE._serialized_start=920
+  _SHAREFILEREQUEST_TYPE._serialized_end=950
+  _SHAREFILERESPONSE._serialized_start=952
+  _SHAREFILERESPONSE._serialized_end=971
+  _SETBLOBSTATUSREQUEST._serialized_start=973
+  _SETBLOBSTATUSREQUEST._serialized_end=1079
+  _SETBLOBSTATUSRESPONSE._serialized_start=1081
+  _SETBLOBSTATUSRESPONSE._serialized_end=1104
+  _LISTBLOBPOINTERSREQUEST._serialized_start=1107
+  _LISTBLOBPOINTERSREQUEST._serialized_end=1792
+  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_start=1385
+  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_end=1548
+  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_start=1525
+  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_end=1548
+  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_start=1550
+  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_end=1629
+  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_start=1632
+  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_end=1792
+  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_start=1753
+  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_end=1792
+  _LISTBLOBPOINTERSRESPONSE._serialized_start=1795
+  _LISTBLOBPOINTERSRESPONSE._serialized_end=2064
+  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_start=1998
+  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_end=2064
+  _LISTBLOBSREQUEST._serialized_start=2067
+  _LISTBLOBSREQUEST._serialized_end=2951
+  _LISTBLOBSREQUEST_ORDER._serialized_start=2301
+  _LISTBLOBSREQUEST_ORDER._serialized_end=2502
+  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_start=2415
+  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_end=2502
+  _LISTBLOBSREQUEST_PAGINATION._serialized_start=2505
+  _LISTBLOBSREQUEST_PAGINATION._serialized_end=2663
+  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_start=2638
+  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_end=2663
+  _LISTBLOBSREQUEST_FILTERING._serialized_start=2666
+  _LISTBLOBSREQUEST_FILTERING._serialized_end=2951
+  _LISTBLOBSRESPONSE._serialized_start=2954
+  _LISTBLOBSRESPONSE._serialized_end=3206
+  _LISTBLOBSRESPONSE_USERSENTRY._serialized_start=620
+  _LISTBLOBSRESPONSE_USERSENTRY._serialized_end=685
+  _GETBLOBREQUEST._serialized_start=3208
+  _GETBLOBREQUEST._serialized_end=3261
+  _GETBLOBRESPONSE._serialized_start=3263
+  _GETBLOBRESPONSE._serialized_end=3319
+  _BLOB._serialized_start=3322
+  _BLOB._serialized_end=3709
+  _BLOB_METAINFO._serialized_start=3609
+  _BLOB_METAINFO._serialized_end=3709
+  _LISTFOLDERREQUEST._serialized_start=3712
+  _LISTFOLDERREQUEST._serialized_end=4762
+  _LISTFOLDERREQUEST_FILTERING._serialized_start=4009
+  _LISTFOLDERREQUEST_FILTERING._serialized_end=4387
+  _LISTFOLDERREQUEST_PAGINATION._serialized_start=4390
+  _LISTFOLDERREQUEST_PAGINATION._serialized_end=4547
+  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_start=1525
+  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_end=1548
+  _LISTFOLDERREQUEST_ORDER._serialized_start=4550
+  _LISTFOLDERREQUEST_ORDER._serialized_end=4762
+  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_start=4665
+  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_end=4762
+  _LISTFOLDERRESPONSE._serialized_start=4765
+  _LISTFOLDERRESPONSE._serialized_end=5028
+  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_start=1998
+  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_end=2064
+  _CREATEFOLDERREQUEST._serialized_start=5031
+  _CREATEFOLDERREQUEST._serialized_end=5209
+  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_start=5162
+  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_end=5209
+  _CREATEFOLDERRESPONSE._serialized_start=5211
+  _CREATEFOLDERRESPONSE._serialized_end=5233
+  _DELETEFOLDERREQUEST._serialized_start=5235
+  _DELETEFOLDERREQUEST._serialized_end=5291
+  _DELETEFOLDERRESPONSE._serialized_start=5293
+  _DELETEFOLDERRESPONSE._serialized_end=5315
+  _DELETEFILEREQUEST._serialized_start=5317
+  _DELETEFILEREQUEST._serialized_end=5371
+  _DELETEFILERESPONSE._serialized_start=5373
+  _DELETEFILERESPONSE._serialized_end=5429
+  _GETFILEREQUEST._serialized_start=5431
+  _GETFILEREQUEST._serialized_end=5482
+  _GETFILERESPONSE._serialized_start=5484
+  _GETFILERESPONSE._serialized_end=5582
+  _FILE._serialized_start=5585
+  _FILE._serialized_end=5941
+  _FILE_STATUS._serialized_start=5892
+  _FILE_STATUS._serialized_end=5941
+  _REPORTUPLOADSTATUSREQUEST._serialized_start=5943
+  _REPORTUPLOADSTATUSREQUEST._serialized_end=6029
+  _REPORTUPLOADSTATUSRESPONSE._serialized_start=6031
+  _REPORTUPLOADSTATUSRESPONSE._serialized_end=6059
+  _CANCELUPLOADREQUEST._serialized_start=6061
+  _CANCELUPLOADREQUEST._serialized_end=6117
+  _CANCELUPLOADRESPONSE._serialized_start=6119
+  _CANCELUPLOADRESPONSE._serialized_end=6141
+  _METADATA._serialized_start=6144
+  _METADATA._serialized_end=6376
+  _METADATA_USERDATAENTRY._serialized_start=5162
+  _METADATA_USERDATAENTRY._serialized_end=5209
+  _UPLOADPRESIGNEDREQUEST._serialized_start=6378
+  _UPLOADPRESIGNEDREQUEST._serialized_end=6484
+  _UPLOADPRESIGNEDRESPONSE._serialized_start=6487
+  _UPLOADPRESIGNEDRESPONSE._serialized_end=6647
+  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_start=6616
+  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_end=6639
+  _DOWNLOADPRESIGNEDREQUEST._serialized_start=6649
+  _DOWNLOADPRESIGNEDREQUEST._serialized_end=6753
+  _DOWNLOADPRESIGNEDRESPONSE._serialized_start=6755
+  _DOWNLOADPRESIGNEDRESPONSE._serialized_end=6842
+  _COPYREQUEST._serialized_start=6844
+  _COPYREQUEST._serialized_end=6955
+  _COMPLETEUPLOADREQUEST._serialized_start=6957
+  _COMPLETEUPLOADREQUEST._serialized_end=7033
+  _COMPLETEUPLOADRESPONSE._serialized_start=7035
+  _COMPLETEUPLOADRESPONSE._serialized_end=7059
+  _FILESYSTEMSERVICE._serialized_start=7184
+  _FILESYSTEMSERVICE._serialized_end=8968
 # @@protoc_insertion_point(module_scope)
```

### Comparing `batchx-9.7.0/batchx/filesystem_pb2_grpc.py` & `batchx-9.7.1/batchx/filesystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/health_pb2.py` & `batchx-9.7.1/batchx/health_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/health_pb2_grpc.py` & `batchx-9.7.1/batchx/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/image_pb2.py` & `batchx-9.7.1/batchx/image_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/image_pb2_grpc.py` & `batchx-9.7.1/batchx/image_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/job_pb2.py` & `batchx-9.7.1/batchx/job_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/job_pb2_grpc.py` & `batchx-9.7.1/batchx/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/log_pb2.py` & `batchx-9.7.1/batchx/log_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/organization_pb2.py` & `batchx-9.7.1/batchx/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/organization_pb2_grpc.py` & `batchx-9.7.1/batchx/organization_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/picture_pb2.py` & `batchx-9.7.1/batchx/picture_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/picture_pb2_grpc.py` & `batchx-9.7.1/batchx/picture_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/profile_pb2.py` & `batchx-9.7.1/batchx/profile_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/provider_pb2.py` & `batchx-9.7.1/batchx/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/provider_pb2_grpc.py` & `batchx-9.7.1/batchx/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/tag_pb2.py` & `batchx-9.7.1/batchx/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/tag_pb2_grpc.py` & `batchx-9.7.1/batchx/tag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/token_pb2.py` & `batchx-9.7.1/batchx/token_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/token_pb2_grpc.py` & `batchx-9.7.1/batchx/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/user_pb2.py` & `batchx-9.7.1/batchx/user_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx/user_pb2_grpc.py` & `batchx-9.7.1/batchx/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/batchx.egg-info/PKG-INFO` & `batchx-9.7.1/batchx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.0
+Version: 9.7.1
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.0/batchx.egg-info/SOURCES.txt` & `batchx-9.7.1/batchx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchx-9.7.0/setup.py` & `batchx-9.7.1/setup.py`

 * *Files identical despite different names*

