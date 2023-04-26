# Comparing `tmp/mlpj-0.2.tar.gz` & `tmp/mlpj-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpj-0.2.tar", last modified: Mon Apr 24 12:02:58 2023, max compression
+gzip compressed data, was "mlpj-0.2.1.tar", last modified: Tue Apr 25 16:54:59 2023, max compression
```

## Comparing `mlpj-0.2.tar` & `mlpj-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-24 12:02:58.810752 mlpj-0.2/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2/LICENSE
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1756 2023-04-24 12:02:58.807419 mlpj-0.2/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-24 12:02:58.807419 mlpj-0.2/mlpj/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       70 2023-04-23 11:58:11.000000 mlpj-0.2/mlpj/__init__.py
--rw-------   0 bruno     (1000) bruno     (1000)    30221 2023-04-23 10:31:40.000000 mlpj-0.2/mlpj/actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7743 2023-04-23 17:34:32.000000 mlpj-0.2/mlpj/ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1190 2023-04-22 15:20:30.000000 mlpj-0.2/mlpj/numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    23146 2023-04-23 16:17:57.000000 mlpj-0.2/mlpj/pandas_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    28573 2023-04-24 10:47:07.000000 mlpj-0.2/mlpj/plot_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)     7593 2023-04-23 16:30:36.000000 mlpj-0.2/mlpj/project_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     7345 2023-04-22 17:41:08.000000 mlpj-0.2/mlpj/python_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    18232 2023-04-23 11:06:21.000000 mlpj-0.2/mlpj/result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2/mlpj/result_template.html
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1598 2023-04-22 17:41:41.000000 mlpj-0.2/mlpj/timeseries_utils.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-24 12:02:58.807419 mlpj-0.2/mlpj.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1756 2023-04-24 12:02:58.000000 mlpj-0.2/mlpj.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      562 2023-04-24 12:02:58.000000 mlpj-0.2/mlpj.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-04-24 12:02:58.000000 mlpj-0.2/mlpj.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-04-24 12:02:58.000000 mlpj-0.2/mlpj.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-04-24 12:02:58.000000 mlpj-0.2/mlpj.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-04-24 12:02:58.810752 mlpj-0.2/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1221 2023-04-23 11:58:54.000000 mlpj-0.2/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-24 12:02:58.807419 mlpj-0.2/test/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    10983 2023-04-23 10:38:17.000000 mlpj-0.2/test/test_actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      483 2023-04-22 15:22:38.000000 mlpj-0.2/test/test_numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13448 2023-04-22 17:43:03.000000 mlpj-0.2/test/test_pandas_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3686 2023-04-22 16:30:49.000000 mlpj-0.2/test/test_python_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2978 2023-04-24 07:28:36.000000 mlpj-0.2/test/test_result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1515 2023-04-22 17:44:08.000000 mlpj-0.2/test/test_timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.610810 mlpj-0.2.1/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.1/LICENSE
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-25 16:54:59.610810 mlpj-0.2.1/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.1/README.md
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.607477 mlpj-0.2.1/mlpj/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-04-25 16:50:02.000000 mlpj-0.2.1/mlpj/__init__.py
+-rw-------   0 bruno     (1000) bruno     (1000)    30221 2023-04-23 10:31:40.000000 mlpj-0.2.1/mlpj/actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     7743 2023-04-23 17:34:32.000000 mlpj-0.2.1/mlpj/ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1190 2023-04-22 15:20:30.000000 mlpj-0.2.1/mlpj/numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    23146 2023-04-23 16:17:57.000000 mlpj-0.2.1/mlpj/pandas_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    28573 2023-04-24 10:47:07.000000 mlpj-0.2.1/mlpj/plot_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)     7593 2023-04-23 16:30:36.000000 mlpj-0.2.1/mlpj/project_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     7860 2023-04-25 16:48:41.000000 mlpj-0.2.1/mlpj/python_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    18232 2023-04-23 11:06:21.000000 mlpj-0.2.1/mlpj/result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.1/mlpj/result_template.html
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1630 2023-04-25 13:13:57.000000 mlpj-0.2.1/mlpj/timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.607477 mlpj-0.2.1/mlpj.egg-info/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      562 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/requires.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-04-25 16:54:59.000000 mlpj-0.2.1/mlpj.egg-info/top_level.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-04-25 16:54:59.610810 mlpj-0.2.1/setup.cfg
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1223 2023-04-25 16:49:37.000000 mlpj-0.2.1/setup.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-04-25 16:54:59.610810 mlpj-0.2.1/test/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    10983 2023-04-23 10:38:17.000000 mlpj-0.2.1/test/test_actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      483 2023-04-22 15:22:38.000000 mlpj-0.2.1/test/test_numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    13448 2023-04-22 17:43:03.000000 mlpj-0.2.1/test/test_pandas_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3686 2023-04-22 16:30:49.000000 mlpj-0.2.1/test/test_python_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2978 2023-04-24 07:28:36.000000 mlpj-0.2.1/test/test_result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1515 2023-04-22 17:44:08.000000 mlpj-0.2.1/test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2/LICENSE` & `mlpj-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/PKG-INFO` & `mlpj-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2
+Version: 0.2.1
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2/README.md` & `mlpj-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/actions_looper.py` & `mlpj-0.2.1/mlpj/actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/ml_utils.py` & `mlpj-0.2.1/mlpj/ml_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/numpy_utils.py` & `mlpj-0.2.1/mlpj/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/pandas_utils.py` & `mlpj-0.2.1/mlpj/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/plot_utils.py` & `mlpj-0.2.1/mlpj/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/project_utils.py` & `mlpj-0.2.1/mlpj/project_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/python_utils.py` & `mlpj-0.2.1/mlpj/python_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import os
 import sys
 import sqlite3
 import datetime
 import contextlib
 import tempfile
+import logging
 
 
 def all_except(seq, omissions):
     """All entries of a list except the one mentioned in `omissions`.
 
     Args:
         seq (seq): sequence of objects
@@ -276,7 +277,25 @@
     """Today in ISO date format
 
     Returns:
         str: in ISO date format
     """
     return datetime.date.today().isoformat()
 
+
+def create_console_logger(module, level=logging.DEBUG):
+    """Create a default console logger for a given module.
+
+    Args:
+        module (str): module name
+        level (int): logging level
+    Returns:
+        `logging.Logger`
+    """
+    logger = logging.getLogger(module)
+    logger.setLevel(level)
+    handler = logging.StreamHandler()
+    handler.setFormatter(
+        logging.Formatter("%(asctime)s %(name)s %(levelname)s: %(message)s"))
+    logger.addHandler(handler)
+
+    return logger
```

### Comparing `mlpj-0.2/mlpj/result_display.py` & `mlpj-0.2.1/mlpj/result_display.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/result_template.html` & `mlpj-0.2.1/mlpj/result_template.html`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/mlpj/timeseries_utils.py` & `mlpj-0.2.1/mlpj/timeseries_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """
 import pandas as pd
 
 from . import python_utils as pu
 
 
 def remove_last_n_days(df, datetime_colname, n_days):
-    """Remove the last n_days days from the dataframe.
+    """Remove the data later than `n_days` before today from the dataframe.
 
     Args:
         df (`pd.DataFrame`): input dataframe
         datetime_colname (str): column name containing pd-datetime values
-        n_days (int): number of days (prior to today) to remove
+        n_days (int): Data up to the date this many days ago will be kept.
     Returns:
         `pd.DataFrame`: filtered dataframe
     """
     last_day = pu.n_days_ago(n_days)
     return df[df[datetime_colname] <= pd.to_datetime(last_day)]
```

### Comparing `mlpj-0.2/mlpj.egg-info/PKG-INFO` & `mlpj-0.2.1/mlpj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpj
-Version: 0.2
+Version: 0.2.1
 Summary: Tools for machine learning projects
 Home-page: https://github.com/bdanielby/mlpj
 Author: Bruno Daniel
 License: MIT
 Project-URL: Homepage, https://github.com/bdanielby/mlpj
 Project-URL: Source, https://github.com/bdanielby/mlpj
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlpj-0.2/mlpj.egg-info/SOURCES.txt` & `mlpj-0.2.1/mlpj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/setup.py` & `mlpj-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 github_url = 'https://github.com/bdanielby/mlpj'
 
 setup(
     name='mlpj',
-    version='0.2',
+    version='0.2.1',
     description='Tools for machine learning projects',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url=github_url,
     author='Bruno Daniel',
     license='MIT',
     packages=['mlpj'],
```

### Comparing `mlpj-0.2/test/test_actions_looper.py` & `mlpj-0.2.1/test/test_actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/test/test_pandas_utils.py` & `mlpj-0.2.1/test/test_pandas_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/test/test_python_utils.py` & `mlpj-0.2.1/test/test_python_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/test/test_result_display.py` & `mlpj-0.2.1/test/test_result_display.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2/test/test_timeseries_utils.py` & `mlpj-0.2.1/test/test_timeseries_utils.py`

 * *Files identical despite different names*

