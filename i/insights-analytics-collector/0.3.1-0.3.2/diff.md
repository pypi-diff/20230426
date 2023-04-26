# Comparing `tmp/insights-analytics-collector-0.3.1.tar.gz` & `tmp/insights-analytics-collector-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insights-analytics-collector-0.3.1.tar", last modified: Mon Apr 24 15:31:19 2023, max compression
+gzip compressed data, was "insights-analytics-collector-0.3.2.tar", last modified: Wed Apr 26 15:55:50 2023, max compression
```

## Comparing `insights-analytics-collector-0.3.1.tar` & `insights-analytics-collector-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.965939 insights-analytics-collector-0.3.1/insights_analytics_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_data_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/csv_file_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.965939 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module4_slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/test_gathering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/test_slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:50.199999 insights-analytics-collector-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-26 15:55:50.199999 insights-analytics-collector-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:50.195999 insights-analytics-collector-0.3.2/insights_analytics_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collection_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collection_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collection_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collection_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/csv_file_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/insights_analytics_collector/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:50.195999 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 15:55:50.000000 insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:55:50.199999 insights-analytics-collector-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:50.195999 insights-analytics-collector-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:50.199999 insights-analytics-collector-0.3.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/collector_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/collector_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/collector_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/collector_module4_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/test_gathering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-26 15:55:28.000000 insights-analytics-collector-0.3.2/tests/functional/test_slicing.py
```

### Comparing `insights-analytics-collector-0.3.1/LICENSE.md` & `insights-analytics-collector-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/PKG-INFO` & `insights-analytics-collector-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-analytics-collector
-Version: 0.3.1
+Version: 0.3.2
 Summary: Collector Package for Insights for AAP
 Home-page: https://github.com/RedHatInsights/insights-analytics-collector/
 Author: Martin Slemr
 Author-email: mslemr@redhat.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `insights-analytics-collector-0.3.1/README.md` & `insights-analytics-collector-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collection.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collection.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_csv.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collection_csv.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_data_status.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collection_data_status.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_json.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collection_json.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_manifest.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collection_manifest.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/collector.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/collector.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/csv_file_splitter.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/csv_file_splitter.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/decorators.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/decorators.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector/package.py` & `insights-analytics-collector-0.3.2/insights_analytics_collector/package.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/PKG-INFO` & `insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-analytics-collector
-Version: 0.3.1
+Version: 0.3.2
 Summary: Collector Package for Insights for AAP
 Home-page: https://github.com/RedHatInsights/insights-analytics-collector/
 Author: Martin Slemr
 Author-email: mslemr@redhat.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/SOURCES.txt` & `insights-analytics-collector-0.3.2/insights_analytics_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/setup.py` & `insights-analytics-collector-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 # We use the README as the long_description
 readme_path = os.path.join(os.path.dirname(__file__), "README.md")
 
 
 setup(
     name="insights-analytics-collector",
```

### Comparing `insights-analytics-collector-0.3.1/tests/functional/collector_module.py` & `insights-analytics-collector-0.3.2/tests/functional/collector_module.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/tests/functional/collector_module3.py` & `insights-analytics-collector-0.3.2/tests/functional/collector_module3.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/tests/functional/collector_module4_slicing.py` & `insights-analytics-collector-0.3.2/tests/functional/collector_module4_slicing.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/tests/functional/helpers.py` & `insights-analytics-collector-0.3.2/tests/functional/helpers.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/tests/functional/test_gathering.py` & `insights-analytics-collector-0.3.2/tests/functional/test_gathering.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.1/tests/functional/test_slicing.py` & `insights-analytics-collector-0.3.2/tests/functional/test_slicing.py`

 * *Files identical despite different names*

