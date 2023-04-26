# Comparing `tmp/nycu_tdx_py-0.1.1.tar.gz` & `tmp/nycu_tdx_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nycu_tdx_py-0.1.1.tar", last modified: Wed Apr 26 15:10:38 2023, max compression
+gzip compressed data, was "nycu_tdx_py-0.1.2.tar", last modified: Wed Apr 26 15:58:42 2023, max compression
```

## Comparing `nycu_tdx_py-0.1.1.tar` & `nycu_tdx_py-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:10:38.524573 nycu_tdx_py-0.1.1/
--rw-rw-rw-   0        0        0      219 2023-04-26 15:10:38.524573 nycu_tdx_py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-26 15:10:38.526058 nycu_tdx_py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-04-26 15:10:18.000000 nycu_tdx_py-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:10:38.509574 nycu_tdx_py-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:10:38.513574 nycu_tdx_py-0.1.1/src/example_publish_pypi_medium/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.1/src/example_publish_pypi_medium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:10:38.515573 nycu_tdx_py-0.1.1/src/example_publish_pypi_medium/example/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.1/src/example_publish_pypi_medium/example/__init__.py
--rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.1/src/example_publish_pypi_medium/example/custom_sklearn.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:10:38.523574 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-26 15:10:38.000000 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-26 15:10:38.000000 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:10:38.000000 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 15:10:38.000000 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-26 15:10:38.000000 nycu_tdx_py-0.1.1/src/nycu_tdx_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 15:58:42.680590 nycu_tdx_py-0.1.2/
+-rw-rw-rw-   0        0        0      219 2023-04-26 15:58:42.680590 nycu_tdx_py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-26 15:58:42.681606 nycu_tdx_py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-04-26 15:57:44.000000 nycu_tdx_py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:58:42.662154 nycu_tdx_py-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:58:42.667596 nycu_tdx_py-0.1.2/src/example_publish_pypi_medium/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.2/src/example_publish_pypi_medium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:58:42.669583 nycu_tdx_py-0.1.2/src/example_publish_pypi_medium/example/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.2/src/example_publish_pypi_medium/example/__init__.py
+-rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.2/src/example_publish_pypi_medium/example/custom_sklearn.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:58:42.679607 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-26 15:58:42.000000 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-26 15:58:42.000000 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:58:42.000000 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 15:58:42.000000 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-26 15:58:42.000000 nycu_tdx_py-0.1.2/src/nycu_tdx_py.egg-info/top_level.txt
```

