# Comparing `tmp/tarvis-exchange-dydx-0.9.1.tar.gz` & `tmp/tarvis-exchange-dydx-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-dydx-0.9.1.tar", last modified: Thu Apr 20 20:30:46 2023, max compression
+gzip compressed data, was "tarvis-exchange-dydx-0.9.2.tar", last modified: Tue Apr 25 23:49:39 2023, max compression
```

## Comparing `tarvis-exchange-dydx-0.9.1.tar` & `tarvis-exchange-dydx-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 20:30:35.000000 tarvis-exchange-dydx-0.9.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      407 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-20 20:30:35.000000 tarvis-exchange-dydx-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-20 20:30:35.000000 tarvis-exchange-dydx-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/tarvis/exchange/dydx/
--rw-r--r--   0 root         (0) root         (0)     8775 2023-04-20 20:30:35.000000 tarvis-exchange-dydx-0.9.1/tarvis/exchange/dydx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2023-04-20 20:30:46.000000 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-20 20:30:46.000000 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:30:46.000000 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-20 20:30:46.000000 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 20:30:46.000000 tarvis-exchange-dydx-0.9.1/tarvis_exchange_dydx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:30:46.412884 tarvis-exchange-dydx-0.9.1/test/
--rw-r--r--   0 root         (0) root         (0)    12009 2023-04-20 20:30:35.000000 tarvis-exchange-dydx-0.9.1/test/test_exchange_dydx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:39.001985 tarvis-exchange-dydx-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-25 23:49:27.000000 tarvis-exchange-dydx-0.9.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-25 23:49:39.001985 tarvis-exchange-dydx-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 23:49:27.000000 tarvis-exchange-dydx-0.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 23:49:39.001985 tarvis-exchange-dydx-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-25 23:49:27.000000 tarvis-exchange-dydx-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:38.997985 tarvis-exchange-dydx-0.9.2/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:38.997985 tarvis-exchange-dydx-0.9.2/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:38.997985 tarvis-exchange-dydx-0.9.2/tarvis/exchange/dydx/
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-04-25 23:49:27.000000 tarvis-exchange-dydx-0.9.2/tarvis/exchange/dydx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:39.001985 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-25 23:49:38.000000 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      309 2023-04-25 23:49:38.000000 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 23:49:38.000000 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-25 23:49:38.000000 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 23:49:38.000000 tarvis-exchange-dydx-0.9.2/tarvis_exchange_dydx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:39.001985 tarvis-exchange-dydx-0.9.2/test/
+-rw-r--r--   0 root         (0) root         (0)    12009 2023-04-25 23:49:27.000000 tarvis-exchange-dydx-0.9.2/test/test_exchange_dydx.py
```

### Comparing `tarvis-exchange-dydx-0.9.1/LICENSE.txt` & `tarvis-exchange-dydx-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-dydx-0.9.1/setup.py` & `tarvis-exchange-dydx-0.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-dydx",
-    version="0.9.1",
+    version="0.9.2",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for dYdX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-dydx-0.9.1/tarvis/exchange/dydx/__init__.py` & `tarvis-exchange-dydx-0.9.2/tarvis/exchange/dydx/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-dydx-0.9.1/test/test_exchange_dydx.py` & `tarvis-exchange-dydx-0.9.2/test/test_exchange_dydx.py`

 * *Files identical despite different names*

