# Comparing `tmp/nycu_tdx_py-0.1.5.tar.gz` & `tmp/nycu_tdx_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nycu_tdx_py-0.1.5.tar", last modified: Wed Apr 26 16:15:45 2023, max compression
+gzip compressed data, was "nycu_tdx_py-0.1.6.tar", last modified: Wed Apr 26 16:17:46 2023, max compression
```

## Comparing `nycu_tdx_py-0.1.5.tar` & `nycu_tdx_py-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:15:45.737398 nycu_tdx_py-0.1.5/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:15:45.737398 nycu_tdx_py-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-26 16:15:45.738399 nycu_tdx_py-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-04-26 16:15:20.000000 nycu_tdx_py-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:15:45.718733 nycu_tdx_py-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 16:15:45.722732 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:15:45.728236 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/example/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/example/__init__.py
--rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/example/custom_sklearn.py
--rw-rw-rw-   0        0        0     1140 2023-04-26 16:15:04.000000 nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/example/get_token.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:15:45.736398 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:15:45.000000 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-04-26 16:15:45.000000 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:15:45.000000 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 16:15:45.000000 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-26 16:15:45.000000 nycu_tdx_py-0.1.5/src/nycu_tdx_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.354111 nycu_tdx_py-0.1.6/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:17:46.354111 nycu_tdx_py-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.6/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-26 16:17:46.355129 nycu_tdx_py-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-04-26 16:17:13.000000 nycu_tdx_py-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.338950 nycu_tdx_py-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.344982 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.348100 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/__init__.py
+-rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/custom_sklearn.py
+-rw-rw-rw-   0        0        0     1140 2023-04-26 16:15:04.000000 nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/get_token.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:17:46.353110 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-26 16:17:46.000000 nycu_tdx_py-0.1.6/src/nycu_tdx_py.egg-info/top_level.txt
```

### Comparing `nycu_tdx_py-0.1.5/src/example_publish_pypi_medium/example/get_token.py` & `nycu_tdx_py-0.1.6/src/example_publish_pypi_medium/example/get_token.py`

 * *Files identical despite different names*

