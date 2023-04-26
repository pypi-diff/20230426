# Comparing `tmp/timeexecution-7.0.2.tar.gz` & `tmp/timeexecution-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeexecution-7.0.2.tar", last modified: Tue Feb  7 11:06:05 2023, max compression
+gzip compressed data, was "timeexecution-7.0.3.tar", last modified: Wed Feb  8 14:15:55 2023, max compression
```

## Comparing `timeexecution-7.0.2.tar` & `timeexecution-7.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.431583 timeexecution-7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.427583 timeexecution-7.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.427583 timeexecution-7.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-07 11:05:51.000000 timeexecution-7.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-02-07 11:05:51.000000 timeexecution-7.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-07 11:05:51.000000 timeexecution-7.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-07 11:05:51.000000 timeexecution-7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-07 11:05:51.000000 timeexecution-7.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-02-07 11:06:05.431583 timeexecution-7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-02-07 11:05:51.000000 timeexecution-7.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-07 11:05:51.000000 timeexecution-7.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-07 11:05:51.000000 timeexecution-7.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-07 11:06:05.431583 timeexecution-7.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-02-07 11:05:51.000000 timeexecution-7.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.427583 timeexecution-7.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/dummy_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/test_base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/test_decorator_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tests/test_threaded_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.427583 timeexecution-7.0.2/time_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.431583 timeexecution-7.0.2/time_execution/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/backends/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/backends/threaded.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-02-07 11:05:51.000000 timeexecution-7.0.2/time_execution/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:06:05.431583 timeexecution-7.0.2/timeexecution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-07 11:06:05.000000 timeexecution-7.0.2/timeexecution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-07 11:05:51.000000 timeexecution-7.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.000142 timeexecution-7.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-02-08 14:15:42.000000 timeexecution-7.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-02-08 14:15:42.000000 timeexecution-7.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-08 14:15:42.000000 timeexecution-7.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-08 14:15:42.000000 timeexecution-7.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-08 14:15:42.000000 timeexecution-7.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-02-08 14:15:55.004143 timeexecution-7.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-02-08 14:15:42.000000 timeexecution-7.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-08 14:15:42.000000 timeexecution-7.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-08 14:15:42.000000 timeexecution-7.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-08 14:15:55.004143 timeexecution-7.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-02-08 14:15:42.000000 timeexecution-7.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/dummy_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/test_decorator_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tests/test_threaded_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/time_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/time_execution/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/backends/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/backends/threaded.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-02-08 14:15:42.000000 timeexecution-7.0.3/time_execution/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 14:15:55.004143 timeexecution-7.0.3/timeexecution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-02-08 14:15:54.000000 timeexecution-7.0.3/timeexecution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-08 14:15:55.000000 timeexecution-7.0.3/timeexecution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 14:15:54.000000 timeexecution-7.0.3/timeexecution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 14:15:54.000000 timeexecution-7.0.3/timeexecution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-08 14:15:54.000000 timeexecution-7.0.3/timeexecution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 14:15:54.000000 timeexecution-7.0.3/timeexecution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-08 14:15:42.000000 timeexecution-7.0.3/tox.ini
```

### Comparing `timeexecution-7.0.2/.editorconfig` & `timeexecution-7.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/.gitchangelog.rc` & `timeexecution-7.0.3/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/.github/workflows/publish.yml` & `timeexecution-7.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/.github/workflows/tests.yml` & `timeexecution-7.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/.gitignore` & `timeexecution-7.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/CHANGELOG.md` & `timeexecution-7.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/LICENSE` & `timeexecution-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/Makefile` & `timeexecution-7.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/PKG-INFO` & `timeexecution-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeexecution
-Version: 7.0.2
+Version: 7.0.3
 Summary: Python project
 Home-page: https://github.com/kpn/py-timeexecution
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `timeexecution-7.0.2/README.md` & `timeexecution-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/pyproject.toml` & `timeexecution-7.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/setup.py` & `timeexecution-7.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/tests/test_decorator_async.py` & `timeexecution-7.0.3/tests/test_decorator_async.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/tests/test_elasticsearch.py` & `timeexecution-7.0.3/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/tests/test_hooks.py` & `timeexecution-7.0.3/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/tests/test_threaded_backend.py` & `timeexecution-7.0.3/tests/test_threaded_backend.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/time_execution/backends/elasticsearch.py` & `timeexecution-7.0.3/time_execution/backends/elasticsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,11 +65,16 @@
             metrics (list): data with mappings to send to elasticsearch
         """
         actions = []
         index = self.get_index()
         for metric in metrics:
             actions.append({"index": {"_index": index}})
             actions.append(metric)
+
+        bulk_params = {"operations": actions}
+        if self.pipeline:
+            bulk_params["pipeline"] = self.pipeline
+
         try:
-            self.client.bulk(operations=actions)
+            self.client.bulk(**bulk_params)
         except TransportError as exc:
             logger.warning("bulk_write metrics %r failure %r", metrics, exc)
```

### Comparing `timeexecution-7.0.2/time_execution/backends/threaded.py` & `timeexecution-7.0.3/time_execution/backends/threaded.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/time_execution/decorator.py` & `timeexecution-7.0.3/time_execution/decorator.py`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/timeexecution.egg-info/PKG-INFO` & `timeexecution-7.0.3/timeexecution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeexecution
-Version: 7.0.2
+Version: 7.0.3
 Summary: Python project
 Home-page: https://github.com/kpn/py-timeexecution
 Author: KPN DE Platform
 Author-email: de-platform@kpn.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `timeexecution-7.0.2/timeexecution.egg-info/SOURCES.txt` & `timeexecution-7.0.3/timeexecution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeexecution-7.0.2/tox.ini` & `timeexecution-7.0.3/tox.ini`

 * *Files identical despite different names*

