# Comparing `tmp/pandasflow-0.4.0.tar.gz` & `tmp/pandasflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.4.0.tar", last modified: Wed Apr 26 14:27:14 2023, max compression
+gzip compressed data, was "pandasflow-0.4.1.tar", last modified: Wed Apr 26 15:03:27 2023, max compression
```

## Comparing `pandasflow-0.4.0.tar` & `pandasflow-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.955346 pandasflow-0.4.0/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.0/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-26 14:27:14.956345 pandasflow-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.946770 pandasflow-0.4.0/pandasflow/
--rw-rw-rw-   0        0        0      268 2023-04-26 14:27:11.000000 pandasflow-0.4.0/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.948767 pandasflow-0.4.0/pandasflow/dev/
--rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.0/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.0/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      479 2023-04-25 13:49:33.000000 pandasflow-0.4.0/pandasflow/get_import.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.951197 pandasflow-0.4.0/pandasflow/metrics/
--rw-rw-rw-   0        0        0      120 2023-04-26 14:24:20.000000 pandasflow-0.4.0/pandasflow/metrics/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-04-26 14:26:38.000000 pandasflow-0.4.0/pandasflow/metrics/lloss_up.py
--rw-rw-rw-   0        0        0      341 2023-04-26 14:17:55.000000 pandasflow-0.4.0/pandasflow/metrics/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.0/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.951197 pandasflow-0.4.0/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.0/pandasflow/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.953765 pandasflow-0.4.0/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.0/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.0/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.0/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.948767 pandasflow-0.4.0/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-26 14:27:14.000000 pandasflow-0.4.0/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 14:27:14.956345 pandasflow-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 14:27:14.955346 pandasflow-0.4.0/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.0/test/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.0/test/split_tt_test.py
--rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.0/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.4.0/test/test_get_column_name.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.521613 pandasflow-0.4.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.4.1/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-26 15:03:27.521613 pandasflow-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-25 14:18:16.000000 pandasflow-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.510642 pandasflow-0.4.1/pandasflow/
+-rw-rw-rw-   0        0        0      296 2023-04-26 15:02:39.000000 pandasflow-0.4.1/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.513634 pandasflow-0.4.1/pandasflow/dev/
+-rw-rw-rw-   0        0        0       62 2023-04-26 14:24:20.000000 pandasflow-0.4.1/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-04-26 14:21:40.000000 pandasflow-0.4.1/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      413 2023-04-26 15:02:39.000000 pandasflow-0.4.1/pandasflow/get_import.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.515629 pandasflow-0.4.1/pandasflow/metrics/
+-rw-rw-rw-   0        0        0      120 2023-04-26 14:24:20.000000 pandasflow-0.4.1/pandasflow/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-04-26 14:55:46.000000 pandasflow-0.4.1/pandasflow/metrics/lloss_up.py
+-rw-rw-rw-   0        0        0      393 2023-04-26 14:59:27.000000 pandasflow-0.4.1/pandasflow/metrics/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.4.1/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.516626 pandasflow-0.4.1/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.4.1/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.517624 pandasflow-0.4.1/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.4.1/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.4.1/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.4.1/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.512637 pandasflow-0.4.1/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-26 15:03:27.000000 pandasflow-0.4.1/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2023-04-26 15:03:27.000000 pandasflow-0.4.1/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:03:27.000000 pandasflow-0.4.1/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-26 15:03:27.000000 pandasflow-0.4.1/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 15:03:27.000000 pandasflow-0.4.1/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:03:27.521613 pandasflow-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:03:27.520621 pandasflow-0.4.1/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.4.1/test/__init__.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.4.1/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.4.1/test/test_get_column_name.py
+-rw-rw-rw-   0        0        0      608 2023-04-26 14:57:04.000000 pandasflow-0.4.1/test/test_lloss_up.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 14:30:22.000000 pandasflow-0.4.1/test/test_mean_error.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.4.1/test/test_split_tt.py
```

### Comparing `pandasflow-0.4.0/LICENCE` & `pandasflow-0.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/PKG-INFO` & `pandasflow-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.0/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.4.1/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/pandasflow/reset_mi.py` & `pandasflow-0.4.1/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/pandasflow/split/train_test.py` & `pandasflow-0.4.1/pandasflow/split/train_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/pandasflow/split/train_valid_test.py` & `pandasflow-0.4.1/pandasflow/split/train_valid_test.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.4.1/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.4.0/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.4.1/pandasflow.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,12 @@
 pandasflow/metrics/lloss_up.py
 pandasflow/metrics/mean_error.py
 pandasflow/services/__init__.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
-test/split_tt_test.py
 test/split_tvt_test.py
-test/test_get_column_name.py
+test/test_get_column_name.py
+test/test_lloss_up.py
+test/test_mean_error.py
+test/test_split_tt.py
```

### Comparing `pandasflow-0.4.0/setup.py` & `pandasflow-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.4.0/test/split_tvt_test.py` & `pandasflow-0.4.1/test/split_tvt_test.py`

 * *Files identical despite different names*

