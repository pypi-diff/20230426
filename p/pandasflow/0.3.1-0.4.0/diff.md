# Comparing `tmp/pandasflow-0.3.1.tar.gz` & `tmp/pandasflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.3.1.tar", last modified: Sat Apr 22 18:32:10 2023, max compression
+gzip compressed data, was "pandasflow-0.4.0.tar", last modified: Wed Apr 26 14:27:14 2023, max compression
```

## Comparing `pandasflow-0.3.1.tar` & `pandasflow-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.184682 pandasflow-0.3.1/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.3.1/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-22 18:32:10.184682 pandasflow-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.177371 pandasflow-0.3.1/pandasflow/
--rw-rw-rw-   0        0        0      284 2023-04-22 18:31:51.000000 pandasflow-0.3.1/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.180692 pandasflow-0.3.1/pandasflow/dev/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.3.1/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.3.1/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.3.1/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.3.1/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.3.1/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.181689 pandasflow-0.3.1/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.3.1/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.182687 pandasflow-0.3.1/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.3.1/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.3.1/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.3.1/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.180692 pandasflow-0.3.1/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 18:32:10.185679 pandasflow-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.184682 pandasflow-0.3.1/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.3.1/test/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.3.1/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.3.1/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.3.1/test/test_get_column_name.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.955346 pandasflow-0.4.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.0/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-26 14:27:14.956345 pandasflow-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.946770 pandasflow-0.4.0/pandasflow/
+-rw-rw-rw-   0        0        0      268 2023-04-26 14:27:11.000000 pandasflow-0.4.0/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.948767 pandasflow-0.4.0/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.0/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.0/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      479 2023-04-25 13:49:33.000000 pandasflow-0.4.0/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.951197 pandasflow-0.4.0/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      120 2023-04-26 14:24:20.000000 pandasflow-0.4.0/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-04-26 14:26:38.000000 pandasflow-0.4.0/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      341 2023-04-26 14:17:55.000000 pandasflow-0.4.0/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.0/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.951197 pandasflow-0.4.0/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.0/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.953765 pandasflow-0.4.0/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.0/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.0/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.0/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.948767 pandasflow-0.4.0/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:27:14.956345 pandasflow-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.955346 pandasflow-0.4.0/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.0/test/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.0/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.0/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.4.0/test/test_get_column_name.py
```

### Comparing `pandasflow-0.3.1/LICENCE` & `pandasflow-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.1/PKG-INFO` & `pandasflow-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.3.1
+Version: 0.4.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.3.1/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.0/pandasflow/dev/err_mean_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandasflow as pdf
 import seaborn as sns
 
 
 def err_mean_diff(df, index_col, dark=True, color='red'):
 	CM = sns.dark_palette(color, as_cmap=True) if dark else sns.light_palette(color, as_cmap=True)
 	
-	t = df.groupby(index_col)[['error', 'error_abs']].agg(['count', 'mean'])
+	t = df.groupby(index_col)[['metrics', 'error_abs']].agg(['count', 'mean'])
 	t = pdf.reset_mi(t)
 	t = t.drop(['error_abs_count'], axis=1)
 	t = t.rename({'error_count': 'count'}, axis=1)
 	t['error_mean_diff'] = t['error_abs_mean'] - df['error_abs'].mean()
 	t = t.rename({'error_count': 'count'}, axis=1)
 	t['test_mean_error'] = df['error_abs'].mean()
```

### Comparing `pandasflow-0.3.1/pandasflow/reset_mi.py` & `pandasflow-0.4.0/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.1/pandasflow/split/train_test.py` & `pandasflow-0.4.0/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.1/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.0/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.1/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.0/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.3.1
+Version: 0.4.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.3.1/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.0/pandasflow.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENCE
 README.md
 setup.cfg
 setup.py
 pandasflow/__init__.py
 pandasflow/get_import.py
-pandasflow/mean_error.py
 pandasflow/reset_mi.py
 pandasflow.egg-info/PKG-INFO
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
+pandasflow/metrics/__init__.py
+pandasflow/metrics/lloss_up.py
+pandasflow/metrics/mean_error.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
 test/split_tt_test.py
 test/split_tvt_test.py
```

### Comparing `pandasflow-0.3.1/setup.py` & `pandasflow-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.1/test/split_tvt_test.py` & `pandasflow-0.4.0/test/split_tvt_test.py`

 * *Files identical despite different names*

