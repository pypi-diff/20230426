# Comparing `tmp/erroranalysis-0.4.2.tar.gz` & `tmp/erroranalysis-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erroranalysis-0.4.2.tar", last modified: Fri Mar 10 19:05:13 2023, max compression
+gzip compressed data, was "dist/erroranalysis-0.4.3.tar", last modified: Wed Apr 26 01:12:10 2023, max compression
```

## Comparing `erroranalysis-0.4.2.tar` & `erroranalysis-0.4.3.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/_internal/error_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/error_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/_internal/error_report/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/error_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/process_categoricals.py
--rw-r--r--   0 runner    (1001) docker     (123)    41699 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/_internal/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30887 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/analyzer/error_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis/report/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/report/error_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/erroranalysis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-10 19:05:12.000000 erroranalysis-0.4.2/erroranalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/erroranalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 19:05:12.000000 erroranalysis-0.4.2/erroranalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-10 19:05:12.000000 erroranalysis-0.4.2/erroranalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-10 19:05:12.000000 erroranalysis-0.4.2/erroranalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:05:13.000000 erroranalysis-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_error_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_pyspark_surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_root_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-03-10 19:04:28.000000 erroranalysis-0.4.2/tests/test_surrogate_error_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_report/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/error_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34348 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/process_categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/_internal/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32082 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/analyzer/error_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/ebm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/error_correlation_methods/gbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/report/error_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/erroranalysis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/erroranalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:12:10.000000 erroranalysis-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_error_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_pyspark_surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_root_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-26 01:11:21.000000 erroranalysis-0.4.3/tests/test_surrogate_error_tree.py
```

### Comparing `erroranalysis-0.4.2/LICENSE` & `erroranalysis-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/PKG-INFO` & `erroranalysis-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.4.2
+Version: 0.4.3
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Error Analysis SDK for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
 
 The error analysis sdk enables users to get a deeper understanding of machine learning model errors. When evaluating a machine learning model, aggregate accuracy is not sufficient and single-score evaluation may hide important conditions of inaccuracies. Use Error Analysis to identify cohorts with higher error rates and diagnose the root causes behind these errors.
 
 Highlights of the package include:
 
 - The error heatmap to investigate how one or two input features impact the error rate across cohorts
 - The decision tree surrogate model trained on errors to discover cohorts with high error rates across multiple features. Investigate indicators such as error rate, error coverage, and data representation for each discovered cohort.
```

### Comparing `erroranalysis-0.4.2/README.md` & `erroranalysis-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Error Analysis SDK for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
 
 The error analysis sdk enables users to get a deeper understanding of machine learning model errors. When evaluating a machine learning model, aggregate accuracy is not sufficient and single-score evaluation may hide important conditions of inaccuracies. Use Error Analysis to identify cohorts with higher error rates and diagnose the root causes behind these errors.
 
 Highlights of the package include:
 
 - The error heatmap to investigate how one or two input features impact the error rate across cohorts
 - The decision tree surrogate model trained on errors to discover cohorts with high error rates across multiple features. Investigate indicators such as error rate, error coverage, and data representation for each discovered cohort.
```

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/cohort_filter.py` & `erroranalysis-0.4.3/erroranalysis/_internal/cohort_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/constants.py` & `erroranalysis-0.4.3/erroranalysis/_internal/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,14 +92,17 @@
     RECALL_SCORE = 'recall_score'
     MACRO_RECALL_SCORE = 'macro_recall_score'
     MICRO_RECALL_SCORE = 'micro_recall_score'
     ERROR_RATE = 'error_rate'
     FALSE_POSITIVE_RATE = 'false_positive_rate'
     FALSE_NEGATIVE_RATE = 'false_negative_rate'
     SELECTION_RATE = 'selection_rate'
+    MEAN_AVERAGE_PRECISION = 'mean_average_precision'
+    AVERAGE_PRECISION = 'average_precision'
+    AVERAGE_RECALL = 'average_recall'
 
 
 class MetricKeys(str, Enum):
     """Provide keys for properties related to metrics.
     """
     METRIC_NAME = 'metricName'
     METRIC_VALUE = 'metricValue'
@@ -117,14 +120,24 @@
 class TreeNode(str, Enum):
     """Provide the tree node properties.
     """
     METRIC_NAME = MetricKeys.METRIC_NAME.value
     METRIC_VALUE = MetricKeys.METRIC_VALUE.value
 
 
+class ErrorCorrelationMethods(str, Enum):
+    """Provide the supported error correlation methods.
+
+    The supported methods are 'mutual_info', 'ebm' and 'gbm_shap'.
+    """
+    MUTUAL_INFO = 'mutual_info'
+    EBM = 'ebm'
+    GBM_SHAP = 'gbm_shap'
+
+
 metric_to_display_name = {
     Metrics.ACCURACY_SCORE: 'Accuracy score',
     Metrics.MEAN_PREDICTION: 'Mean prediction',
     Metrics.MEAN_ABSOLUTE_ERROR: 'Mean absolute error',
     Metrics.MEAN_SQUARED_ERROR: 'Mean squared error',
     Metrics.MEDIAN_ABSOLUTE_ERROR: 'Median absolute error',
     Metrics.R2_SCORE: 'R2 score',
```

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/matrix_filter.py` & `erroranalysis-0.4.3/erroranalysis/_internal/matrix_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/metrics.py` & `erroranalysis-0.4.3/erroranalysis/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/process_categoricals.py` & `erroranalysis-0.4.3/erroranalysis/_internal/process_categoricals.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/surrogate_error_tree.py` & `erroranalysis-0.4.3/erroranalysis/_internal/surrogate_error_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,14 @@
     :param min_child_samples: The minimal number of data required to
         create one leaf.
     :type min_child_samples: int
     :return: The extracted booster from the surrogate model and the
         scored dataset.
     :rtype: (Booster, pandas.DataFrame, (list[str], list[int]))
     """
-    row_index = filtered_df[ROW_INDEX]
     true_y = filtered_df[TRUE_Y]
     dropped_cols = [TRUE_Y, ROW_INDEX]
     if not is_model_analyzer:
         pred_y = filtered_df[PRED_Y]
         dropped_cols.append(PRED_Y)
     input_data = filtered_df.drop(columns=dropped_cols)
     is_pandas = isinstance(analyzer.dataset, pd.DataFrame)
@@ -326,15 +325,15 @@
                 process_categoricals(
                     all_feature_names=analyzer._feature_names,
                     categorical_features=analyzer._categorical_features,
                     dataset=input_data)
         else:
             string_indexed_data = analyzer.string_indexed_data
         for idx, c_i in enumerate(analyzer.categorical_indexes):
-            input_data[:, c_i] = string_indexed_data[row_index, idx]
+            input_data[:, c_i] = string_indexed_data[:, idx]
     dataset_sub_features = input_data[:, indexes]
 
     categorical_info = get_categorical_info(analyzer,
                                             dataset_sub_names)
     cat_ind_reindexed, categories_reindexed = categorical_info
 
     surrogate = create_surrogate_model(analyzer,
@@ -601,15 +600,15 @@
     :param tree: The tree to get the features from.
     :type tree: dict
     :return: The filtered DataFrame.
     :rtype: pandas.DataFrame
     """
     features = tree[CACHED_SUBTREE_FEATURES]
     features = features.union({PRED_Y, TRUE_Y, DIFF})
-    return df[features]
+    return df[list(features)]
 
 
 def cache_subtree_features(tree, feature_names, parent=None):
     """Caches the features of the subtree on each of the tree nodes.
 
     :param tree: The current node in the tree to cache the features on.
     :type tree: dict
```

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/utils.py` & `erroranalysis-0.4.3/erroranalysis/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/_internal/version_checker.py` & `erroranalysis-0.4.3/erroranalysis/_internal/version_checker.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis/analyzer/error_analyzer.py` & `erroranalysis-0.4.3/erroranalysis/analyzer/error_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 from abc import ABC, abstractmethod
 
 import numpy as np
 import pandas as pd
 from sklearn.feature_selection import (mutual_info_classif,
                                        mutual_info_regression)
 
-from erroranalysis._internal.constants import (MatrixParams, Metrics,
+from erroranalysis._internal.constants import (ErrorCorrelationMethods,
+                                               MatrixParams, Metrics,
                                                ModelTask, RootKeys,
                                                metric_to_display_name)
 from erroranalysis._internal.matrix_filter import \
     compute_matrix as _compute_matrix
 from erroranalysis._internal.matrix_filter import \
     compute_matrix_on_dataset as _compute_matrix_on_dataset
 from erroranalysis._internal.metrics import metric_to_func
 from erroranalysis._internal.process_categoricals import process_categoricals
 from erroranalysis._internal.surrogate_error_tree import \
     compute_error_tree as _compute_error_tree
 from erroranalysis._internal.surrogate_error_tree import \
     compute_error_tree_on_dataset as _compute_error_tree_on_dataset
 from erroranalysis._internal.utils import generate_random_unique_indexes
 from erroranalysis._internal.version_checker import check_pandas_version
+from erroranalysis.error_correlation_methods import (
+    compute_ebm_global_importance, compute_gbm_global_importance)
 from erroranalysis.report import ErrorReport
 
 BIN_THRESHOLD = MatrixParams.BIN_THRESHOLD
 IMPORTANCES_THRESHOLD = 50000
 ROOT_COVERAGE = 100
+MUTUAL_INFO = ErrorCorrelationMethods.MUTUAL_INFO.value
 
 
 class BaseAnalyzer(ABC):
     """BaseAnalyzer Class, used by ModelAnalyzer and PredictionsAnalyzer.
 
     BaseAnalyzer class is the common base class for the ModelAnalyzer
     and PredictionsAnalyzer classes.
@@ -368,15 +372,16 @@
 
     def create_error_report(self,
                             filter_features=None,
                             max_depth=None,
                             num_leaves=None,
                             min_child_samples=None,
                             compute_importances=False,
-                            compute_root_stats=False):
+                            compute_root_stats=False,
+                            error_correlation_method=MUTUAL_INFO):
         """Creates the error analysis ErrorReport.
 
         The ErrorReport contains the importances, heatmap and tree view json.
 
         :param filter_features: One or two features to compute the heatmap.
         :type filter_features: list
         :param max_depth: The maximum depth of the surrogate tree trained
@@ -405,33 +410,35 @@
         matrix = None
         if filter_features:
             matrix = self.compute_matrix(filter_features,
                                          None,
                                          None)
         importances = None
         if compute_importances:
-            importances = self.compute_importances()
+            importances = self.compute_importances(error_correlation_method)
         root_stats = None
         if compute_root_stats:
             root_stats = self.compute_root_stats()
         return ErrorReport(tree, matrix,
                            tree_features=self.feature_names,
                            matrix_features=filter_features,
                            importances=importances,
                            root_stats=root_stats)
 
-    def compute_importances(self):
+    def compute_importances(self, error_correlation_method=MUTUAL_INFO):
         """Compute the importances or correlation between features and error.
 
         Computes the feature importances or the correlation between
         each of the features in the dataset and the error from the label
         and prediction columns.  Uses mutual information, specifically
         uses the scikit-learn methods mutual_info_classif for classification
         and mutual_info_regression for regression tasks.
 
+        :param error_correlation_method: Method to compute error correlation.
+        :type error_correlation_method: str
         :return: The computed importances or correlation between the
             features and error.
         :rtype: list[float]
         """
         input_data = self.dataset
         diff = self.get_diff()
         if isinstance(self.dataset, pd.DataFrame):
@@ -447,46 +454,58 @@
         num_rows = input_data.shape[0]
         if num_rows > IMPORTANCES_THRESHOLD:
             indexes = generate_random_unique_indexes(num_rows,
                                                      IMPORTANCES_THRESHOLD)
             input_data = input_data[indexes]
             diff = diff[indexes]
         try:
-            importances = self._compute_mutual_info(input_data, diff)
+            importances = self._compute_error_correlation(
+                input_data, diff, error_correlation_method)
         except ValueError:
             # Impute input_data if it contains NaNs, infinity or a value too
             # large for dtype('float64')
             input_data = np.nan_to_num(input_data)
-            importances = self._compute_mutual_info(input_data, diff)
+            importances = self._compute_error_correlation(
+                input_data, diff, error_correlation_method)
         return importances
 
-    def _compute_mutual_info(self, input_data, diff):
-        """Compute the mutual information between the features and error.
+    def _compute_error_correlation(self, input_data, diff,
+                                   error_correlation_method):
+        """Compute the correlation between the features and error.
 
-        :param input_data: The input data to compute the mutual information
+        :param input_data: The input data to compute the error correlation
             on.
         :type input_data: numpy.ndarray
         :param diff: The difference between the label and prediction
             columns.
         :type diff: numpy.ndarray
-        :return: The computed mutual information between the features and
+        :param error_correlation_method: Method to compute error correlation.
+        :type error_correlation_method: str
+        :return: The computed error correlation between the features and
             error.
         :rtype: list[float]
         """
         # if only one row, replicate it to avoid exception
         if input_data.shape[0] == 1:
             input_data = np.concatenate((input_data, input_data))
             diff = np.concatenate((diff, diff))
-        n_neighbors = min(3, input_data.shape[0] - 1)
-        if self._model_task == ModelTask.CLASSIFICATION:
-            return mutual_info_classif(
-                input_data, diff, n_neighbors=n_neighbors).tolist()
+        if error_correlation_method == ErrorCorrelationMethods.MUTUAL_INFO:
+            n_neighbors = min(3, input_data.shape[0] - 1)
+            if self._model_task == ModelTask.CLASSIFICATION:
+                return mutual_info_classif(
+                    input_data, diff, n_neighbors=n_neighbors).tolist()
+            else:
+                return mutual_info_regression(
+                    input_data, diff, n_neighbors=n_neighbors).tolist()
+        elif error_correlation_method == ErrorCorrelationMethods.EBM:
+            return compute_ebm_global_importance(
+                input_data, diff, self._model_task)
         else:
-            return mutual_info_regression(
-                input_data, diff, n_neighbors=n_neighbors).tolist()
+            return compute_gbm_global_importance(
+                input_data, diff, self._model_task, self._categorical_indexes)
 
     def compute_root_stats(self):
         """Compute the root all data statistics.
 
         :return: The computed root statistics.
         :rtype: dict
         """
```

### Comparing `erroranalysis-0.4.2/erroranalysis/report/error_report.py` & `erroranalysis-0.4.3/erroranalysis/report/error_report.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/erroranalysis.egg-info/PKG-INFO` & `erroranalysis-0.4.3/erroranalysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.4.2
+Version: 0.4.3
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Error Analysis SDK for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
 
 The error analysis sdk enables users to get a deeper understanding of machine learning model errors. When evaluating a machine learning model, aggregate accuracy is not sufficient and single-score evaluation may hide important conditions of inaccuracies. Use Error Analysis to identify cohorts with higher error rates and diagnose the root causes behind these errors.
 
 Highlights of the package include:
 
 - The error heatmap to investigate how one or two input features impact the error rate across cohorts
 - The decision tree surrogate model trained on errors to discover cohorts with high error rates across multiple features. Investigate indicators such as error rate, error coverage, and data representation for each discovered cohort.
```

### Comparing `erroranalysis-0.4.2/erroranalysis.egg-info/SOURCES.txt` & `erroranalysis-0.4.3/erroranalysis.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 erroranalysis/_internal/surrogate_error_tree.py
 erroranalysis/_internal/utils.py
 erroranalysis/_internal/version_checker.py
 erroranalysis/_internal/error_analyzer/__init__.py
 erroranalysis/_internal/error_report/__init__.py
 erroranalysis/analyzer/__init__.py
 erroranalysis/analyzer/error_analyzer.py
+erroranalysis/error_correlation_methods/__init__.py
+erroranalysis/error_correlation_methods/ebm.py
+erroranalysis/error_correlation_methods/gbm.py
 erroranalysis/report/__init__.py
 erroranalysis/report/error_report.py
 tests/test_cohort_filter.py
 tests/test_error_report.py
 tests/test_importances.py
 tests/test_matrix_filter.py
 tests/test_metrics.py
```

### Comparing `erroranalysis-0.4.2/setup.py` & `erroranalysis-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,13 @@
     python_requires='>=3.6',
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ]
 )
```

### Comparing `erroranalysis-0.4.2/tests/test_cohort_filter.py` & `erroranalysis-0.4.3/tests/test_cohort_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/tests/test_error_report.py` & `erroranalysis-0.4.3/tests/test_error_report.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/tests/test_importances.py` & `erroranalysis-0.4.3/tests/test_root_stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,118 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-import time
-
-import numpy as np
 import pytest
-from common_utils import replicate_dataset
 
-from erroranalysis._internal.constants import ModelTask
+from erroranalysis._internal.constants import (Metrics, RootKeys,
+                                               metric_to_display_name)
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
+from erroranalysis._internal.metrics import metric_to_func
 from rai_test_utils.datasets.tabular import (
     create_binary_classification_dataset, create_cancer_data,
     create_housing_data, create_iris_data, create_simple_titanic_data)
-from rai_test_utils.models.lightgbm import create_lightgbm_classifier
 from rai_test_utils.models.model_utils import (create_models_classification,
                                                create_models_regression)
-from rai_test_utils.models.sklearn import (
-    create_sklearn_random_forest_classifier,
-    create_sklearn_random_forest_regressor, create_titanic_pipeline)
+from rai_test_utils.models.sklearn import create_titanic_pipeline
 
 TOL = 1e-10
-NUM_SAMPLE_ROWS = 100
-DEFAULT_SAMPLE_COLS = 20
 
 
-class TestImportances(object):
+class TestRootStats(object):
 
-    def test_importances_iris(self):
+    @pytest.mark.parametrize('metric', [Metrics.ERROR_RATE,
+                                        Metrics.MACRO_PRECISION_SCORE,
+                                        Metrics.MICRO_PRECISION_SCORE,
+                                        Metrics.MACRO_RECALL_SCORE,
+                                        Metrics.MICRO_RECALL_SCORE,
+                                        Metrics.MACRO_F1_SCORE,
+                                        Metrics.MICRO_F1_SCORE,
+                                        Metrics.ACCURACY_SCORE])
+    def test_importances_iris(self, metric):
         X_train, X_test, y_train, y_test, feature_names, _ = create_iris_data()
 
         models = create_models_classification(X_train, y_train)
 
         for model in models:
             categorical_features = []
             run_error_analyzer(model, X_test, y_test, feature_names,
-                               categorical_features)
+                               categorical_features, metric)
 
-    def test_importances_cancer(self):
+    @pytest.mark.parametrize('metric', [Metrics.ERROR_RATE,
+                                        Metrics.PRECISION_SCORE,
+                                        Metrics.RECALL_SCORE,
+                                        Metrics.ACCURACY_SCORE,
+                                        Metrics.F1_SCORE])
+    def test_importances_cancer(self, metric):
         X_train, X_test, y_train, y_test, feature_names, _ = \
             create_cancer_data()
 
         models = create_models_classification(X_train, y_train)
 
         for model in models:
             categorical_features = []
             run_error_analyzer(model, X_test, y_test, feature_names,
-                               categorical_features)
+                               categorical_features, metric)
 
-    def test_importances_binary_classification(self):
+    @pytest.mark.parametrize('metric', [Metrics.ERROR_RATE,
+                                        Metrics.PRECISION_SCORE,
+                                        Metrics.RECALL_SCORE,
+                                        Metrics.ACCURACY_SCORE,
+                                        Metrics.F1_SCORE])
+    def test_importances_binary_classification(self, metric):
         X_train, y_train, X_test, y_test, _ = \
             create_binary_classification_dataset()
         feature_names = list(X_train.columns)
         models = create_models_classification(X_train, y_train)
 
         for model in models:
             categorical_features = []
             run_error_analyzer(model, X_test, y_test, feature_names,
-                               categorical_features)
+                               categorical_features, metric=metric)
 
     def test_importances_titanic(self):
         X_train, X_test, y_train, y_test, numeric, categorical = \
             create_simple_titanic_data()
         feature_names = categorical + numeric
         clf = create_titanic_pipeline(X_train, y_train)
         categorical_features = categorical
         run_error_analyzer(clf, X_test, y_test, feature_names,
                            categorical_features)
 
-    def test_importances_housing(self):
+    @pytest.mark.parametrize('metric', [Metrics.MEAN_SQUARED_ERROR,
+                                        Metrics.MEAN_ABSOLUTE_ERROR])
+    def test_importances_housing(self, metric):
         X_train, X_test, y_train, y_test, feature_names = \
             create_housing_data()
         models = create_models_regression(X_train, y_train)
 
         for model in models:
             categorical_features = []
             run_error_analyzer(model, X_test, y_test, feature_names,
-                               categorical_features)
-
-    def test_large_data_importances(self):
-        # mutual information can be very costly for large number of rows
-        # hence, assert we downsample to compute importances for large data
-        X_train, y_train, X_test, y_test, _ = \
-            create_binary_classification_dataset(NUM_SAMPLE_ROWS)
-        feature_names = list(X_train.columns)
-        model = create_sklearn_random_forest_regressor(X_train, y_train)
-        X_test, y_test = replicate_dataset(X_test, y_test)
-        assert X_test.shape[0] > 1000000
-        t0 = time.time()
-        categorical_features = []
-        model_analyzer = ModelAnalyzer(model, X_test, y_test,
-                                       feature_names,
-                                       categorical_features)
-        model_analyzer.compute_importances()
-        t1 = time.time()
-        execution_time = t1 - t0
-        print(execution_time)
-        # assert we don't take too long and downsample the dataset
-        # note execution time is in seconds
-        assert execution_time < 20
-
-    @pytest.mark.parametrize('num_rows', [1, 2, 3, 4])
-    def test_small_data_importances(self, num_rows):
-        # validate we can run on very few rows
-        X_train, y_train, X_test, y_test, _ = \
-            create_binary_classification_dataset(NUM_SAMPLE_ROWS)
-        feature_names = list(X_train.columns)
-        model = create_sklearn_random_forest_classifier(X_train, y_train)
-        X_test = X_test[:num_rows]
-        y_test = y_test[:num_rows]
-        categorical_features = []
-        model_analyzer = ModelAnalyzer(model, X_test, y_test,
-                                       feature_names,
-                                       categorical_features)
-        scores = model_analyzer.compute_importances()
-        assert len(scores) == DEFAULT_SAMPLE_COLS
-
-    def test_importances_missings(self):
-        X_train, X_test, y_train, y_test, feature_names, _ = create_iris_data()
-
-        # add missing values to X_test
-        for i in range(5, 10):
-            X_test.iloc[i, 0] = np.nan
-            X_test.iloc[i + 5, 2] = np.nan
-
-        model = create_lightgbm_classifier(X_train, y_train)
-
-        categorical_features = []
-        run_error_analyzer(model, X_test, y_test, feature_names,
-                           categorical_features)
+                               categorical_features, metric)
 
 
 def run_error_analyzer(model, X_test, y_test, feature_names,
-                       categorical_features):
+                       categorical_features, metric=Metrics.ERROR_RATE):
     model_analyzer = ModelAnalyzer(model, X_test, y_test,
                                    feature_names,
-                                   categorical_features)
-    scores = model_analyzer.compute_importances()
-    if model_analyzer.model_task == ModelTask.CLASSIFICATION:
-        diff = model.predict(model_analyzer.dataset) != model_analyzer.true_y
-    else:
-        diff = model.predict(model_analyzer.dataset) - model_analyzer.true_y
-    assert isinstance(scores, list)
-    assert len(scores) == len(feature_names)
-    # If model predicted perfectly, assert all scores are zeros
-    if not any(diff):
-        assert all(abs(score - 0) < TOL for score in scores)
+                                   categorical_features,
+                                   metric=metric)
+    root_stats = model_analyzer.compute_root_stats()
+    metric_name = metric_to_display_name[metric]
+
+    total = len(X_test)
+
+    assert root_stats[RootKeys.METRIC_NAME] == metric_name
+    assert root_stats[RootKeys.TOTAL_SIZE] == total
+    assert root_stats[RootKeys.ERROR_COVERAGE] == 100
+
+    if metric == Metrics.ERROR_RATE:
+        diff = model_analyzer.get_diff()
+        error = sum(diff)
+        metric_value = (error / total) * 100
     else:
-        assert any(score != 0 for score in scores)
+        metric_func = metric_to_func[metric]
+        metric_value = metric_func(model_analyzer.pred_y,
+                                   model_analyzer.true_y)
+
+    assert root_stats[RootKeys.METRIC_VALUE] == metric_value
```

### Comparing `erroranalysis-0.4.2/tests/test_matrix_filter.py` & `erroranalysis-0.4.3/tests/test_matrix_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/tests/test_metrics.py` & `erroranalysis-0.4.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/tests/test_pyspark_surrogate_error_tree.py` & `erroranalysis-0.4.3/tests/test_pyspark_surrogate_error_tree.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.4.2/tests/test_surrogate_error_tree.py` & `erroranalysis-0.4.3/tests/test_surrogate_error_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,20 +62,32 @@
                                analyzer_type)
 
     @pytest.mark.parametrize('analyzer_type', [AnalyzerType.MODEL,
                                                AnalyzerType.PREDICTIONS])
     def test_surrogate_error_tree_int_categorical(self, analyzer_type):
         X_train, X_test, y_train, y_test, categorical_features = \
             create_adult_census_data()
-
         model = create_kneighbors_classifier(X_train, y_train)
 
         run_error_analyzer(model, X_test, y_test, list(X_train.columns),
                            analyzer_type, categorical_features)
 
+    @pytest.mark.parametrize('analyzer_type', [AnalyzerType.MODEL,
+                                               AnalyzerType.PREDICTIONS])
+    def test_surrogate_error_tree_categorical_filtered(self, analyzer_type):
+        X_train, X_test, y_train, y_test, categorical_features = \
+            create_adult_census_data()
+        model = create_kneighbors_classifier(X_train, y_train)
+        filters = [{'arg': [40],
+                    'column': 'Age',
+                    'method': 'less and equal'}]
+        run_error_analyzer(model, X_test, y_test, list(X_train.columns),
+                           analyzer_type, categorical_features,
+                           filters=filters)
+
     def test_large_data_surrogate_error_tree(self):
         # validate tree trains quickly for large data
         X_train, y_train, X_test, y_test, _ = \
             create_binary_classification_dataset(100)
         feature_names = list(X_train.columns)
         model = create_sklearn_random_forest_regressor(X_train, y_train)
         X_test, y_test = replicate_dataset(X_test, y_test)
```

