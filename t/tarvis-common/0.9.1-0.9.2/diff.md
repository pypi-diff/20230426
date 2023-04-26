# Comparing `tmp/tarvis-common-0.9.1.tar.gz` & `tmp/tarvis-common-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.1.tar", last modified: Thu Apr 20 20:27:00 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.2.tar", last modified: Tue Apr 25 22:43:33 2023, max compression
```

## Comparing `tarvis-common-0.9.1.tar` & `tarvis-common-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.011965 tarvis-common-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-20 20:27:00.011965 tarvis-common-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:27:00.011965 tarvis-common-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.003964 tarvis-common-0.9.1/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1288 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     5792 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6201 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.007964 tarvis-common-0.9.1/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)     8247 2023-04-20 20:26:50.000000 tarvis-common-0.9.1/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:27:00.011965 tarvis-common-0.9.1/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-20 20:26:59.000000 tarvis-common-0.9.1/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-04-20 20:26:59.000000 tarvis-common-0.9.1/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:26:59.000000 tarvis-common-0.9.1/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2023-04-20 20:26:59.000000 tarvis-common-0.9.1/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 20:26:59.000000 tarvis-common-0.9.1/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.413471 tarvis-common-0.9.2/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     5797 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)     8247 2023-04-25 22:43:24.000000 tarvis-common-0.9.2/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 22:43:33.417472 tarvis-common-0.9.2/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 22:43:33.000000 tarvis-common-0.9.2/tarvis_common.egg-info/top_level.txt
```

### Comparing `tarvis-common-0.9.1/LICENSE.txt` & `tarvis-common-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/setup.py` & `tarvis-common-0.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.1",
+    version="0.9.2",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.1/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.2/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.2/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.2/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.2/tarvis/common/logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     try:
         with io.open(_GCP_CLIENT_CREDENTIALS_FILE, "r") as credentials_file:
             credentials = json.load(credentials_file)
             client_email = credentials["client_email"]
             logging_client = client_email.split("@")[0]
             _gcp_extra = {"logging_client": logging_client}
     except:
-        logging.error(f"Missing or invalid {_GCP_CLIENT_CREDENTIALS_FILE}")
+        logging.critical(f'Missing or invalid "{_GCP_CLIENT_CREDENTIALS_FILE}"')
         raise
 
     # noinspection PyPackageRequirements
     import google.cloud.logging
 
     client = google.cloud.logging.Client()
     client.setup_logging()
```

### Comparing `tarvis-common-0.9.1/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.2/tarvis/common/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.2/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/time/__init__.py` & `tarvis-common-0.9.2/tarvis/common/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.2/tarvis/common/trading/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.1/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.2/tarvis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

