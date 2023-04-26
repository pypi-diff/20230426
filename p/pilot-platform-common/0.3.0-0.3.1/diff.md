# Comparing `tmp/pilot-platform-common-0.3.0.tar.gz` & `tmp/pilot-platform-common-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.3.0.tar", last modified: Thu Mar 30 14:21:16 2023, max compression
+gzip compressed data, was "pilot-platform-common-0.3.1.tar", last modified: Tue Apr 25 16:58:14 2023, max compression
```

## Comparing `pilot-platform-common-0.3.0.tar` & `pilot-platform-common-0.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/geid/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/jwt_handler/jwt_handler_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/lineage/entity_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     8976 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/lineage/lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/lineage/lineage_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/logger/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/logger/logger_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/models/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.017858 pilot-platform-common-0.3.0/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/permissions/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/common/project/
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/common/vault/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-03-30 14:21:15.000000 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-03-30 14:21:16.000000 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:21:15.000000 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-03-30 14:21:15.000000 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-30 14:21:15.000000 pilot-platform-common-0.3.0/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7606 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:21:16.021858 pilot-platform-common-0.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_lineage_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_logger_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-03-30 14:20:21.000000 pilot-platform-common-0.3.0/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/jwt_handler/jwt_handler_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/entity_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8976 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/lineage/lineage_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logger/logger_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.688696 pilot-platform-common-0.3.1/common/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16665 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3264 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/permissions/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 16:58:14.000000 pilot-platform-common-0.3.1/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7606 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 16:58:14.692695 pilot-platform-common-0.3.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_lineage_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_logger_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-04-25 16:57:18.000000 pilot-platform-common-0.3.1/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.3.0/PKG-INFO` & `pilot-platform-common-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.3.0/README.md` & `pilot-platform-common-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/__init__.py` & `pilot-platform-common-0.3.1/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/geid/geid_client.py` & `pilot-platform-common-0.3.1/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-0.3.1/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/lineage/entity_object.py` & `pilot-platform-common-0.3.1/common/lineage/entity_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/lineage/lineage_client.py` & `pilot-platform-common-0.3.1/common/lineage/lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/lineage/lineage_object.py` & `pilot-platform-common-0.3.1/common/lineage/lineage_object.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/logger/formatter.py` & `pilot-platform-common-0.3.1/common/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/logger/logger_factory.py` & `pilot-platform-common-0.3.1/common/logger/logger_factory.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/logging/logging.py` & `pilot-platform-common-0.3.1/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/models/config_center_policy.py` & `pilot-platform-common-0.3.1/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.3.1/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.3.1/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.3.1/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/permissions/permissions.py` & `pilot-platform-common-0.3.1/common/permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/project/project_client.py` & `pilot-platform-common-0.3.1/common/project/project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/project/project_exceptions.py` & `pilot-platform-common-0.3.1/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/common/vault/vault_client.py` & `pilot-platform-common-0.3.1/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.3.1/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Research
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.3.0/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.3.1/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/pyproject.toml` & `pilot-platform-common-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "common"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Indoc Research"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dotenv = ">=0.19.1"
 aioredis = "^2.0.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
 aioboto3 = "^9.6.0"
 xmltodict = "^0.13.0"
 minio = "^7.1.8"
 httpx = "^0.23.0"
 pyjwt = "2.6.0"
-starlette = "^0.19.1"
+starlette = "^0.25.0"
 cryptography = "39.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-asyncio = "0.20.3"
 pytest-cov = "4.0.0"
 pytest-httpx = "0.21.3"
```

### Comparing `pilot-platform-common-0.3.0/setup.py` & `pilot-platform-common-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.3.0',
+    version='0.3.1',
     author='Indoc Research',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
@@ -28,15 +28,15 @@
         'httpx==0.23.0',
         'aioredis>=2.0.0,<3.0.0',
         'aioboto3==9.6.0',
         'xmltodict==0.13.0',
         'minio==7.1.8',
         'python-json-logger==2.0.2',
         'pyjwt==2.6.0',
-        'starlette>=0.19.1,<0.24.0',
+        'starlette>=0.25.0,<0.27.0',
         'cryptography==39.0.0',
     ],
     include_package_data=True,
     package_data={
         '': ['*.crt'],
     },
 )
```

### Comparing `pilot-platform-common-0.3.0/tests/conftest.py` & `pilot-platform-common-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_formatter.py` & `pilot-platform-common-0.3.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_jwt_handler.py` & `pilot-platform-common-0.3.1/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_lineage_client.py` & `pilot-platform-common-0.3.1/tests/test_lineage_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_logger_factory.py` & `pilot-platform-common-0.3.1/tests/test_logger_factory.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_logging.py` & `pilot-platform-common-0.3.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_permissions.py` & `pilot-platform-common-0.3.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_project_client.py` & `pilot-platform-common-0.3.1/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.3.0/tests/test_vault_client.py` & `pilot-platform-common-0.3.1/tests/test_vault_client.py`

 * *Files identical despite different names*

