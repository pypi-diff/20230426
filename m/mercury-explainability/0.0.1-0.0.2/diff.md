# Comparing `tmp/mercury-explainability-0.0.1.tar.gz` & `tmp/mercury-explainability-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-explainability-0.0.1.tar", last modified: Mon Apr 24 14:16:00 2023, max compression
+gzip compressed data, was "mercury-explainability-0.0.2.tar", last modified: Tue Apr 25 15:11:04 2023, max compression
```

## Comparing `mercury-explainability-0.0.1.tar` & `mercury-explainability-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.503444 mercury-explainability-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-24 14:16:00.503444 mercury-explainability-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.495444 mercury-explainability-0.0.1/mercury/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.495444 mercury-explainability-0.0.1/mercury/explainability/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.499444 mercury-explainability-0.0.1/mercury/explainability/explainers/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/_dummy_alibi_explainers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.499444 mercury-explainability-0.0.1/mercury/explainability/explainers/_tree_splitters/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/_tree_splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/_tree_splitters/cut_finder.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/ale.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/cf_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/clustering_tree_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/counter_fact_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/counter_fact_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15804 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explainers/shuffle_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.503444 mercury-explainability-0.0.1/mercury/explainability/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/clustering_tree_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/counter_factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/explanations/shuffle_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/mercury/explainability/pyspark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:16:00.503444 mercury-explainability-0.0.1/mercury_explainability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-24 14:16:00.000000 mercury-explainability-0.0.1/mercury_explainability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-24 14:16:00.000000 mercury-explainability-0.0.1/mercury_explainability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:16:00.000000 mercury-explainability-0.0.1/mercury_explainability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-24 14:16:00.000000 mercury-explainability-0.0.1/mercury_explainability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 14:16:00.000000 mercury-explainability-0.0.1/mercury_explainability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:16:00.503444 mercury-explainability-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 14:15:44.000000 mercury-explainability-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.111666 mercury-explainability-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 15:11:04.111666 mercury-explainability-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.095666 mercury-explainability-0.0.2/mercury/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.099665 mercury-explainability-0.0.2/mercury/explainability/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.103665 mercury-explainability-0.0.2/mercury/explainability/explainers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/_dummy_alibi_explainers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.107666 mercury-explainability-0.0.2/mercury/explainability/explainers/_tree_splitters/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/_tree_splitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/_tree_splitters/cut_finder.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/ale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/cf_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/clustering_tree_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/counter_fact_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30833 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/counter_fact_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explainers/shuffle_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.107666 mercury-explainability-0.0.2/mercury/explainability/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/clustering_tree_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/counter_factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/explanations/shuffle_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/mercury/explainability/pyspark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:11:04.111666 mercury-explainability-0.0.2/mercury_explainability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-25 15:11:04.000000 mercury-explainability-0.0.2/mercury_explainability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-25 15:11:04.000000 mercury-explainability-0.0.2/mercury_explainability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:11:04.000000 mercury-explainability-0.0.2/mercury_explainability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 15:11:04.000000 mercury-explainability-0.0.2/mercury_explainability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 15:11:04.000000 mercury-explainability-0.0.2/mercury_explainability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:11:04.111666 mercury-explainability-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-25 15:10:45.000000 mercury-explainability-0.0.2/setup.py
```

### Comparing `mercury-explainability-0.0.1/LICENSE` & `mercury-explainability-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/PKG-INFO` & `mercury-explainability-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-explainability
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mercury's explainability is a library with implementations of different state-of-the-art methods in the field of explainability
 Author-email: Mercury Team <mercury.group@bbva.com>
 Project-URL: Homepage, https://github.com/BBVA/mercury-explainability
 Project-URL: Bug Tracker, https://github.com/BBVA/mercury-explainability/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # mercury-explainability
 
 [![](https://github.com/BBVA/mercury-explainability/actions/workflows/test.yml/badge.svg)](https://github.com/BBVA/mercury-explainability)
-![](https://img.shields.io/badge/latest-0.0.1-blue)
+![](https://img.shields.io/badge/latest-0.0.2-blue)
 
 ***mercury-explainability*** is a library with implementations of different state-of-the-art methods in the field of explainability. They are designed to work efficiently and to be easily integrated with the main Machine Learning frameworks.
 
 ## Mercury project at BBVA
 
 Mercury is a collaborative library that was developed by the Advanced Analytics community at BBVA. Originally, it was created as an [InnerSource](https://en.wikipedia.org/wiki/Inner_source) project but after some time, we decided to release certain parts of the project as Open Source.
 That's the case with the `mercury-explainability` package.
```

### Comparing `mercury-explainability-0.0.1/README.md` & `mercury-explainability-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # mercury-explainability
 
 [![](https://github.com/BBVA/mercury-explainability/actions/workflows/test.yml/badge.svg)](https://github.com/BBVA/mercury-explainability)
-![](https://img.shields.io/badge/latest-0.0.1-blue)
+![](https://img.shields.io/badge/latest-0.0.2-blue)
 
 ***mercury-explainability*** is a library with implementations of different state-of-the-art methods in the field of explainability. They are designed to work efficiently and to be easily integrated with the main Machine Learning frameworks.
 
 ## Mercury project at BBVA
 
 Mercury is a collaborative library that was developed by the Advanced Analytics community at BBVA. Originally, it was created as an [InnerSource](https://en.wikipedia.org/wiki/Inner_source) project but after some time, we decided to release certain parts of the project as Open Source.
 That's the case with the `mercury-explainability` package.
```

### Comparing `mercury-explainability-0.0.1/mercury/explainability/__init__.py` & `mercury-explainability-0.0.2/mercury/explainability/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 from .explainers.counter_fact_basic import CounterFactualExplainerBasic
 from .explainers.shuffle_importance import ShuffleImportanceExplainer
 from .explainers.explainer import MercuryExplainer
 from .explainers.partial_dependence import PartialDependenceExplainer
 from .explanations.anchors import AnchorsWithImportanceExplanation
 from .explanations.counter_factual import CounterfactualWithImportanceExplanation
```

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/__init__.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/_dummy_alibi_explainers.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/_dummy_alibi_explainers.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/_tree_splitters/cut_finder.pyx` & `mercury-explainability-0.0.2/mercury/explainability/explainers/_tree_splitters/cut_finder.pyx`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/ale.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/ale.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/anchors.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/anchors.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/cf_strategies.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/cf_strategies.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/clustering_tree_explainer.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/clustering_tree_explainer.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/counter_fact_basic.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/counter_fact_basic.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/counter_fact_importance.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/counter_fact_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as TP
 import numpy as np
 import pandas as pd
 import tensorflow as tf
+tf.compat.v1.disable_eager_execution()
 
 from abc import ABC
 from .explainer import MercuryExplainer
 
 from mercury.explainability.explanations.counter_factual import (
     CounterfactualWithImportanceExplanation
 )
```

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/explainer.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/explainer.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/partial_dependence.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/partial_dependence.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,14 @@
         self.resolution = resolution
 
         if type(quantiles) == float:
             self.compute_quantiles = (quantiles, 1 - quantiles)
         else:
             self.compute_quantiles = quantiles
 
-        # Pyspark names of float and integer datatypes
-        self.__float_typenames = set(["FloatType", "DoubleType", "DecimalType"])
-        self.__int_typenames = set(["FloatType", "DoubleType", "LongType", "IntegerType", "ShortType", "ByteType"])
-
     def explain(self,
             features: TP.Union["pandas.DataFrame", "pyspark.sql.DataFrame"],  # noqa: F821
             ignore_feats: TP.List[str] = None,
             categoricals: TP.List[str] = None)->PartialDependenceExplanation:
         """
         This method will compute the partial dependences for a ML model.
         This explainer also contains a distributed (pyspark) implementation which
@@ -203,35 +199,48 @@
         Returns:
             Dictionary with the partial dependences of each selected feature
             and whether that feature is categorical or not.
         """
         from pyspark.sql.functions import col
         from pyspark.sql import functions as sqlf
 
+        from pyspark.sql.types import (
+            FloatType,
+            DoubleType,
+            DecimalType,
+            LongType,
+            IntegerType,
+            ShortType,
+            ByteType
+        )
+
+        # Pyspark names of float and integer datatypes
+        float_pyspark_types = (FloatType, DoubleType, DecimalType)
+        int_pyspark_types = (FloatType, DoubleType, LongType, IntegerType, ShortType, ByteType)
+
         data = {}
 
         # Calculate unique values for disjoint set of columns from categoricals
         cols_to_check = [n for n in feat_names if n not in categoricals]
         # Calculate all statistics at once to save collects
         num_distinct_values = features.agg(
             *(sqlf.countDistinct(col(c)).alias(c) for c in cols_to_check)
         ).collect()[0]
-        datatypes = {c: str(features.schema[c].dataType) for c in features.columns}
         minimums = features.select([sqlf.min(c).alias(c) for c in features.columns]).collect()[0]
         maximums = features.select([sqlf.max(c).alias(c) for c in features.columns]).collect()[0]
 
         for colname in feat_names:
             start = time.time()
 
             data[colname] = {}
             # Determine whether this column is discrete, real or categorical
             is_categorical = False
-            if datatypes[colname] in self.__float_typenames and colname not in categoricals:
+            if isinstance(features.schema[colname].dataType, float_pyspark_types) and colname not in categoricals:
                 grid = np.linspace(minimums[colname], maximums[colname])
-            elif datatypes[colname] in self.__int_typenames \
+            elif isinstance(features.schema[colname].dataType, int_pyspark_types) \
                     and num_distinct_values[colname] > self._max_categorical_values:
                 step_size = max(
                     1, np.abs((maximums[colname] - minimums[colname]) // self.resolution)
                 )
                 grid = np.arange(minimums[colname], maximums[colname], step=step_size)
             else:
                 grid = features.select(colname).distinct().rdd.flatMap(lambda x: x).collect()
```

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explainers/shuffle_importance.py` & `mercury-explainability-0.0.2/mercury/explainability/explainers/shuffle_importance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Union, Callable
 from .explainer import MercuryExplainer
 from ..explanations.shuffle_importance import FeatureImportanceExplanation
 
 
 import numpy as np
 import pandas as pd
-import pyspark
 from sklearn.preprocessing import MinMaxScaler
 
 
 class ShuffleImportanceExplainer(MercuryExplainer):
     """
     This explainer estimates the feature importance of each predictor for a
     given black-box model. The used strategy consists on random shuffling one
@@ -59,22 +58,22 @@
         ...     return my_evaluator.evaluate(model_out)
         >>> explainer = ShuffleImportanceExplainer(my_inference_function)
         >>> explanation = explainer.explain(features, target_colname)
         >>> explanation.plot()
         ```
     """
     def __init__(self,
-                 eval_fn: Callable[[Union["pd.DataFrame", "pyspark.sql.DataFrame"], Union["np.ndarray", str]], float],
+                 eval_fn: Callable[[Union["pd.DataFrame", "pyspark.sql.DataFrame"], Union["np.ndarray", str]], float],  # noqa: F821
                  normalize: bool = True
         ):
         self.eval_fn = eval_fn
         self.normalize = normalize
 
     def explain(self,
-                predictors: Union["pd.DataFrame", "pyspark.sql.DataFrame"],
+                predictors: Union["pd.DataFrame", "pyspark.sql.DataFrame"],  # noqa: F821
                 target: Union["np.ndarray", str]
         ) -> FeatureImportanceExplanation:
         """
         Explains the model given the data.
 
         Args:
             predictors (Union[pandas.DataFrame, pyspark.sql.DataFrame]):
```

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explanations/anchors.py` & `mercury-explainability-0.0.2/mercury/explainability/explanations/anchors.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explanations/clustering_tree_explanation.py` & `mercury-explainability-0.0.2/mercury/explainability/explanations/clustering_tree_explanation.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explanations/counter_factual.py` & `mercury-explainability-0.0.2/mercury/explainability/explanations/counter_factual.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explanations/partial_dependence.py` & `mercury-explainability-0.0.2/mercury/explainability/explanations/partial_dependence.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/explanations/shuffle_importance.py` & `mercury-explainability-0.0.2/mercury/explainability/explanations/shuffle_importance.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury/explainability/pyspark_utils.py` & `mercury-explainability-0.0.2/mercury/explainability/pyspark_utils.py`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/mercury_explainability.egg-info/PKG-INFO` & `mercury-explainability-0.0.2/mercury_explainability.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-explainability
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mercury's explainability is a library with implementations of different state-of-the-art methods in the field of explainability
 Author-email: Mercury Team <mercury.group@bbva.com>
 Project-URL: Homepage, https://github.com/BBVA/mercury-explainability
 Project-URL: Bug Tracker, https://github.com/BBVA/mercury-explainability/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # mercury-explainability
 
 [![](https://github.com/BBVA/mercury-explainability/actions/workflows/test.yml/badge.svg)](https://github.com/BBVA/mercury-explainability)
-![](https://img.shields.io/badge/latest-0.0.1-blue)
+![](https://img.shields.io/badge/latest-0.0.2-blue)
 
 ***mercury-explainability*** is a library with implementations of different state-of-the-art methods in the field of explainability. They are designed to work efficiently and to be easily integrated with the main Machine Learning frameworks.
 
 ## Mercury project at BBVA
 
 Mercury is a collaborative library that was developed by the Advanced Analytics community at BBVA. Originally, it was created as an [InnerSource](https://en.wikipedia.org/wiki/Inner_source) project but after some time, we decided to release certain parts of the project as Open Source.
 That's the case with the `mercury-explainability` package.
```

### Comparing `mercury-explainability-0.0.1/mercury_explainability.egg-info/SOURCES.txt` & `mercury-explainability-0.0.2/mercury_explainability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-explainability-0.0.1/pyproject.toml` & `mercury-explainability-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "numpy", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mercury-explainability"
 license = {file = "LICENSE.txt"}
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mercury Team", email="mercury.group@bbva.com" },
 ]
 description = "Mercury's explainability is a library with implementations of different state-of-the-art methods in the field of explainability"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

