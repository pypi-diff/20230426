# Comparing `tmp/nycu_tdx_py-0.1.3.tar.gz` & `tmp/nycu_tdx_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nycu_tdx_py-0.1.3.tar", last modified: Wed Apr 26 16:05:31 2023, max compression
+gzip compressed data, was "nycu_tdx_py-0.1.4.tar", last modified: Wed Apr 26 16:06:50 2023, max compression
```

## Comparing `nycu_tdx_py-0.1.3.tar` & `nycu_tdx_py-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:05:31.856229 nycu_tdx_py-0.1.3/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:05:31.857229 nycu_tdx_py-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.3/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-26 16:05:31.857229 nycu_tdx_py-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-04-26 16:05:04.000000 nycu_tdx_py-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:05:31.845229 nycu_tdx_py-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 16:05:31.849228 nycu_tdx_py-0.1.3/src/example_publish_pypi_medium/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.3/src/example_publish_pypi_medium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:05:31.850229 nycu_tdx_py-0.1.3/src/example_publish_pypi_medium/example/
--rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.3/src/example_publish_pypi_medium/example/__init__.py
--rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.3/src/example_publish_pypi_medium/example/custom_sklearn.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:05:31.856229 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-26 16:05:31.000000 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-26 16:05:31.000000 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:05:31.000000 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 16:05:31.000000 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-26 16:05:31.000000 nycu_tdx_py-0.1.3/src/nycu_tdx_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:06:50.487611 nycu_tdx_py-0.1.4/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:06:50.487611 nycu_tdx_py-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-26 15:03:33.000000 nycu_tdx_py-0.1.4/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-26 16:06:50.488638 nycu_tdx_py-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-04-26 16:06:45.000000 nycu_tdx_py-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:06:50.470868 nycu_tdx_py-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 16:06:50.476621 nycu_tdx_py-0.1.4/src/example_publish_pypi_medium/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.4/src/example_publish_pypi_medium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:06:50.478610 nycu_tdx_py-0.1.4/src/example_publish_pypi_medium/example/
+-rw-rw-rw-   0        0        0        0 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.4/src/example_publish_pypi_medium/example/__init__.py
+-rw-rw-rw-   0        0        0       75 2022-01-08 23:56:05.000000 nycu_tdx_py-0.1.4/src/example_publish_pypi_medium/example/custom_sklearn.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:06:50.486609 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-26 16:06:50.000000 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-26 16:06:50.000000 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:06:50.000000 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-26 16:06:50.000000 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-26 16:06:50.000000 nycu_tdx_py-0.1.4/src/nycu_tdx_py.egg-info/top_level.txt
```

