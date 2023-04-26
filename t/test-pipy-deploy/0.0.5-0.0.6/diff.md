# Comparing `tmp/test-pipy-deploy-0.0.5.tar.gz` & `tmp/test-pipy-deploy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-pipy-deploy-0.0.5.tar", last modified: Wed Apr 26 14:59:50 2023, max compression
+gzip compressed data, was "test-pipy-deploy-0.0.6.tar", last modified: Wed Apr 26 15:01:57 2023, max compression
```

## Comparing `test-pipy-deploy-0.0.5.tar` & `test-pipy-deploy-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:59:50.012267 test-pipy-deploy-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 14:59:30.000000 test-pipy-deploy-0.0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:59:50.016267 test-pipy-deploy-0.0.5/test_pipy_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 14:59:49.000000 test-pipy-deploy-0.0.5/test_pipy_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 14:59:50.000000 test-pipy-deploy-0.0.5/test_pipy_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:59:49.000000 test-pipy-deploy-0.0.5/test_pipy_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 14:59:50.000000 test-pipy-deploy-0.0.5/test_pipy_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 15:01:40.000000 test-pipy-deploy-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:57.460621 test-pipy-deploy-0.0.6/test_pipy_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 15:01:57.000000 test-pipy-deploy-0.0.6/test_pipy_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 15:01:57.000000 test-pipy-deploy-0.0.6/test_pipy_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:57.000000 test-pipy-deploy-0.0.6/test_pipy_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 15:01:57.000000 test-pipy-deploy-0.0.6/test_pipy_deploy.egg-info/top_level.txt
```

### Comparing `test-pipy-deploy-0.0.5/.github/workflows/pipy_deployment.yaml` & `test-pipy-deploy-0.0.6/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `test-pipy-deploy-0.0.5/LICENSE` & `test-pipy-deploy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `test-pipy-deploy-0.0.5/pyproject.toml` & `test-pipy-deploy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

