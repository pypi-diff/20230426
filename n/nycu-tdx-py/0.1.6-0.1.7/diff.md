# Comparing `tmp/nycu_tdx_py-0.1.6.tar.gz` & `tmp/nycu_tdx_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nycu_tdx_py-0.1.6.tar", last modified: Wed Apr 26 16:17:46 2023, max compression
+gzip compressed data, was "nycu_tdx_py-0.1.7.tar", last modified: Wed Apr 26 16:32:26 2023, max compression
```

## Comparing `nycu_tdx_py-0.1.6.tar` & `nycu_tdx_py-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.354111 nycu_tdx_py-0.1.6/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:17:46.354111 nycu_tdx_py-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.6/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-26 16:17:46.355129 nycu_tdx_py-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-04-26 16:17:13.000000 nycu_tdx_py-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.338950 nycu_tdx_py-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.344982 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.348100 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/__init__.py
--rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/custom_sklearn.py
--rw-rw-rw-   0        0        0     1140 2023-04-26 16:15:04.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/get_token.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.353110 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:32:26.701529 nycu_tdx_py-0.1.7/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:32:26.702532 nycu_tdx_py-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.7/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-26 16:32:26.704535 nycu_tdx_py-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-04-26 16:32:01.000000 nycu_tdx_py-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:32:26.667533 nycu_tdx_py-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 16:32:26.678528 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:32:26.684531 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/example/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/example/__init__.py
+-rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/example/custom_sklearn.py
+-rw-rw-rw-   0        0        0     1237 2023-04-26 16:29:23.000000 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/example/nycutdx.py
+-rw-rw-rw-   0        0        0     1237 2023-04-26 16:29:23.000000 nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/nycutdx.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:32:26.700533 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:32:26.000000 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-04-26 16:32:26.000000 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:32:26.000000 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 16:32:26.000000 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-26 16:32:26.000000 nycu_tdx_py-0.1.7/src/nycu_tdx_py.egg-info/top_level.txt
```

### Comparing `nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/get_token.py` & `nycu_tdx_py-0.1.7/src/example_publish_pypi_medium/example/nycutdx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import requests
 
 def get_token(app_id, app_key):
+    auth_url="https://tdx.transportdata.tw/auth/realms/TDXConnect/protocol/openid-connect/token"
     class Auth():
         def __init__(self, app_id, app_key):
             self.app_id = app_id
             self.app_key = app_key
 
         def get_auth_header(self):
             content_type = 'application/x-www-form-urlencoded'
```

