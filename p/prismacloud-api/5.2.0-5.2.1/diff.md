# Comparing `tmp/prismacloud-api-5.2.0.tar.gz` & `tmp/prismacloud-api-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-api-5.2.0.tar", last modified: Fri Feb 10 21:10:21 2023, max compression
+gzip compressed data, was "prismacloud-api-5.2.1.tar", last modified: Wed Apr 26 13:56:02 2023, max compression
```

## Comparing `prismacloud-api-5.2.0.tar` & `prismacloud-api-5.2.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.539994 prismacloud-api-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.527993 prismacloud-api-5.2.0/prismacloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.531993 prismacloud-api-5.2.0/prismacloud/api/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.531993 prismacloud-api-5.2.0/prismacloud/api/cspm/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cspm/_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cspm/_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cspm/cspm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/prismacloud/api/cwpp/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_defenders.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/cwpp/cwpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pc_lib_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pc_lib_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/prismacloud/api/pccs/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_checkov_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/pccs/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/prismacloud/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/prismacloud_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-02-10 21:10:21.000000 prismacloud-api-5.2.0/prismacloud_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-10 21:10:21.000000 prismacloud-api-5.2.0/prismacloud_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 21:10:21.000000 prismacloud-api-5.2.0/prismacloud_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-10 21:10:21.000000 prismacloud-api-5.2.0/prismacloud_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-10 21:10:21.000000 prismacloud-api-5.2.0/prismacloud_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.531993 prismacloud-api-5.2.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/scripts/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 21:10:21.539994 prismacloud-api-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:10:21.535994 prismacloud-api-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-10 21:10:01.000000 prismacloud-api-5.2.0/tests/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.970949 prismacloud-api-5.2.1/prismacloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.974949 prismacloud-api-5.2.1/prismacloud/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.974949 prismacloud-api-5.2.1/prismacloud/api/cspm/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cspm/_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cspm/_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cspm/cspm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.978949 prismacloud-api-5.2.1/prismacloud/api/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/cwpp/cwpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pc_lib_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pc_lib_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.978949 prismacloud-api-5.2.1/prismacloud/api/pccs/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_checkov_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/pccs/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/prismacloud/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/prismacloud_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-26 13:56:02.000000 prismacloud-api-5.2.1/prismacloud_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 13:56:02.000000 prismacloud-api-5.2.1/prismacloud_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:56:02.000000 prismacloud-api-5.2.1/prismacloud_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 13:56:02.000000 prismacloud-api-5.2.1/prismacloud_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 13:56:02.000000 prismacloud-api-5.2.1/prismacloud_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.970949 prismacloud-api-5.2.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/scripts/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:02.982949 prismacloud-api-5.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-26 13:55:30.000000 prismacloud-api-5.2.1/tests/unit.py
```

### Comparing `prismacloud-api-5.2.0/LICENSE` & `prismacloud-api-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/PKG-INFO` & `prismacloud-api-5.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.0
+Version: 5.2.1
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.0/README.md` & `prismacloud-api-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cspm/_endpoints.py` & `prismacloud-api-5.2.1/prismacloud/api/cspm/_endpoints.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cspm/_extended.py` & `prismacloud-api-5.2.1/prismacloud/api/cspm/_extended.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cspm/cspm.py` & `prismacloud-api-5.2.1/prismacloud/api/cspm/cspm.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/__init__.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .cwpp         import *
 from ._audits      import *
 from ._cloud       import *
 from ._collections import *
 from ._containers  import *
 from ._credentials import *
 from ._defenders   import *
+from ._feeds       import *
 from ._hosts       import *
 from ._images      import *
 from ._logs        import *
 from ._policies    import *
 from ._registry    import *
 from ._scans       import *
 from ._settings    import *
```

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_audits.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_cloud.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_collections.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_collections.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_containers.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_credentials.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_credentials.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_defenders.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_hosts.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_images.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_logs.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_policies.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_registry.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_scans.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_settings.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_settings.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_stats.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/_tags.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/_tags.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/cwpp/cwpp.py` & `prismacloud-api-5.2.1/prismacloud/api/cwpp/cwpp.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pc_lib_api.py` & `prismacloud-api-5.2.1/prismacloud/api/pc_lib_api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pc_lib_utility.py` & `prismacloud-api-5.2.1/prismacloud/api/pc_lib_utility.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pccs/__init__.py` & `prismacloud-api-5.2.1/prismacloud/api/pccs/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pccs/_errors.py` & `prismacloud-api-5.2.1/prismacloud/api/pccs/_errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,7 +15,16 @@
         return self.execute_code_security('GET', 'code/api/v1/errors/gitBlameAuthors', query_params=query_params)
 
     def fix_or_suppress_scan_results(self, criteria):
         return self.execute_code_security('POST', 'code/api/v1/errors/submitActions', body_params=criteria)
 
     def fixed_resource_code(self, criteria):
         return self.execute_code_security('POST', 'code/api/v1/errors/getFixedCode', body_params=criteria)
+
+    def resources_list(self, body_params=None):
+        return self.execute_code_security('POST', 'code/api/v2/errors/branch_scan/resources', body_params=body_params)
+
+    def policies_list(self, resource_uuid, body_params=None):
+        return self.execute_code_security('POST', 'code/api/v2/errors/branch_scan/resources/%s/policies' % resource_uuid, body_params=body_params)
+
+    def vulnerabilities_list(self, resource_uuid, query_params):
+        return self.execute_code_security('GET', 'code/api/v2/summaries/resource/%s/Vulnerabilities' % resource_uuid, query_params=query_params)
```

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pccs/_repositories.py` & `prismacloud-api-5.2.1/prismacloud/api/pccs/_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pccs/_suppressions.py` & `prismacloud-api-5.2.1/prismacloud/api/pccs/_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud/api/pccs/pccs.py` & `prismacloud-api-5.2.1/prismacloud/api/pccs/pccs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/prismacloud_api.egg-info/PKG-INFO` & `prismacloud-api-5.2.1/prismacloud_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-api
-Version: 5.2.0
+Version: 5.2.1
 Summary: Prisma Cloud API SDK for Python
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-api-python
 Author: Tom Kishel
 Author-email: tkishel@paloaltonetworks.com
 Keywords: prisma cloud api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prismacloud-api-5.2.0/prismacloud_api.egg-info/SOURCES.txt` & `prismacloud-api-5.2.1/prismacloud_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 prismacloud/api/cwpp/__init__.py
 prismacloud/api/cwpp/_audits.py
 prismacloud/api/cwpp/_cloud.py
 prismacloud/api/cwpp/_collections.py
 prismacloud/api/cwpp/_containers.py
 prismacloud/api/cwpp/_credentials.py
 prismacloud/api/cwpp/_defenders.py
+prismacloud/api/cwpp/_feeds.py
 prismacloud/api/cwpp/_hosts.py
 prismacloud/api/cwpp/_images.py
 prismacloud/api/cwpp/_logs.py
 prismacloud/api/cwpp/_policies.py
 prismacloud/api/cwpp/_registry.py
 prismacloud/api/cwpp/_scans.py
 prismacloud/api/cwpp/_settings.py
```

### Comparing `prismacloud-api-5.2.0/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py` & `prismacloud-api-5.2.1/scripts/examples/pcs_vuln_container_with_cve_2022_22965.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/setup.py` & `prismacloud-api-5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `prismacloud-api-5.2.0/tests/unit.py` & `prismacloud-api-5.2.1/tests/unit.py`

 * *Files identical despite different names*

