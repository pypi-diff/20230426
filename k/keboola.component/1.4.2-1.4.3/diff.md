# Comparing `tmp/keboola.component-1.4.2.tar.gz` & `tmp/keboola.component-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keboola.component-1.4.2.tar", last modified: Fri Mar 24 10:02:05 2023, max compression
+gzip compressed data, was "keboola.component-1.4.3.tar", last modified: Tue Apr 25 15:06:47 2023, max compression
```

## Comparing `keboola.component-1.4.2.tar` & `keboola.component-1.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:02:05.250983 keboola.component-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-24 10:01:41.000000 keboola.component-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-03-24 10:02:05.250983 keboola.component-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-03-24 10:01:41.000000 keboola.component-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:02:05.250983 keboola.component-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-24 10:01:41.000000 keboola.component-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:02:05.246983 keboola.component-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:02:05.246983 keboola.component-1.4.2/src/keboola/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:02:05.250983 keboola.component-1.4.2/src/keboola/component/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    40791 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    47209 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/sync_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-24 10:01:41.000000 keboola.component-1.4.2/src/keboola/component/table_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:02:05.250983 keboola.component-1.4.2/src/keboola.component.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 10:02:05.000000 keboola.component-1.4.2/src/keboola.component.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:06:47.513751 keboola.component-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 15:06:30.000000 keboola.component-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-04-25 15:06:47.513751 keboola.component-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-04-25 15:06:30.000000 keboola.component-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:06:47.513751 keboola.component-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 15:06:30.000000 keboola.component-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:06:47.509751 keboola.component-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:06:47.509751 keboola.component-1.4.3/src/keboola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:06:47.513751 keboola.component-1.4.3/src/keboola/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40791 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47209 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/sync_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-25 15:06:30.000000 keboola.component-1.4.3/src/keboola/component/table_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:06:47.509751 keboola.component-1.4.3/src/keboola.component.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 15:06:47.000000 keboola.component-1.4.3/src/keboola.component.egg-info/top_level.txt
```

### Comparing `keboola.component-1.4.2/LICENSE` & `keboola.component-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/PKG-INFO` & `keboola.component-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.component
-Version: 1.4.2
+Version: 1.4.3
 Summary: General library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-component
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Project-URL: Documentation, https://keboola.github.io/python-component/interface.html
 Project-URL: Component Template project, https://bitbucket.org/kds_consulting_team/cookiecutter-python-component
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keboola.component-1.4.2/README.md` & `keboola.component-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/setup.py` & `keboola.component-1.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 project_urls = {
     'Documentation': 'https://keboola.github.io/python-component/interface.html',
     'Component Template project': 'https://bitbucket.org/kds_consulting_team/cookiecutter-python-component'
 }
 
 setuptools.setup(
     name="keboola.component",
-    version="1.4.2",
+    version="1.4.3",
     author="Keboola KDS Team",
     project_urls=project_urls,
     setup_requires=['pytest-runner', 'flake8'],
     tests_require=['pytest'],
     install_requires=[
         'pygelf',
         'pytz',
```

### Comparing `keboola.component-1.4.2/src/keboola/component/base.py` & `keboola.component-1.4.3/src/keboola/component/base.py`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/src/keboola/component/dao.py` & `keboola.component-1.4.3/src/keboola/component/dao.py`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/src/keboola/component/interface.py` & `keboola.component-1.4.3/src/keboola/component/interface.py`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/src/keboola/component/sync_actions.py` & `keboola.component-1.4.3/src/keboola/component/sync_actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,27 +59,27 @@
 
     def __post_init__(self):
         self.label = self.label or self.value
         # special case of element SyncActionResult with no status. (all other must contain {"status":true}
         self.status = None
 
 
-def process_sync_action_result(result: Union[None, dict, SyncActionResult, List[SyncActionResult]]) -> str:
+def process_sync_action_result(result: Union[None, List[dict], dict, SyncActionResult, List[SyncActionResult]]) -> str:
     """
     Converts Sync Action result into valid string (expected by Sync Action).
     Args:
         result: Union[None, SyncActionResult, List[SyncActionResult]]
 
     Returns: str: Valid string representation of the Sync action result.
 
     """
     if isinstance(result, SyncActionResult):
         result_str = str(result)
     elif isinstance(result, list):
-        result_str = f'[{", ".join([str(r) for r in result])}]'
+        result_str = f'[{", ".join([json.dumps(r) if isinstance(r, dict) else str(r) for r in result])}]'
     elif result is None:
         result_str = json.dumps({'status': 'success'})
     elif isinstance(result, dict):
         # for backward compatibility
         result_str = json.dumps(result)
     else:
         raise ValueError("Result of sync action must be either None or an instance of SyncActionResult "
```

### Comparing `keboola.component-1.4.2/src/keboola/component/table_schema.py` & `keboola.component-1.4.3/src/keboola/component/table_schema.py`

 * *Files identical despite different names*

### Comparing `keboola.component-1.4.2/src/keboola.component.egg-info/PKG-INFO` & `keboola.component-1.4.3/src/keboola.component.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.component
-Version: 1.4.2
+Version: 1.4.3
 Summary: General library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-component
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Project-URL: Documentation, https://keboola.github.io/python-component/interface.html
 Project-URL: Component Template project, https://bitbucket.org/kds_consulting_team/cookiecutter-python-component
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keboola.component-1.4.2/src/keboola.component.egg-info/SOURCES.txt` & `keboola.component-1.4.3/src/keboola.component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

