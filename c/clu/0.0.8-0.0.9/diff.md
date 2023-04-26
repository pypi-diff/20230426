# Comparing `tmp/clu-0.0.8.tar.gz` & `tmp/clu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clu-0.0.8.tar", last modified: Fri Dec 16 16:33:49 2022, max compression
+gzip compressed data, was "clu-0.0.9.tar", last modified: Wed Apr 26 07:34:01 2023, max compression
```

## Comparing `clu-0.0.8.tar` & `clu-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-16 16:33:37.000000 clu-0.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-16 16:33:37.000000 clu-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2022-12-16 16:33:49.621310 clu-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-12-16 16:33:37.000000 clu-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-16 16:33:37.000000 clu-0.0.8/clu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2022-12-16 16:33:37.000000 clu-0.0.8/clu/asynclib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2022-12-16 16:33:37.000000 clu-0.0.8/clu/asynclib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2022-12-16 16:33:37.000000 clu-0.0.8/clu/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2022-12-16 16:33:37.000000 clu-0.0.8/clu/checkpoint_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu/data/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-16 16:33:37.000000 clu-0.0.8/clu/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2022-12-16 16:33:37.000000 clu-0.0.8/clu/data/dataset_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2022-12-16 16:33:37.000000 clu-0.0.8/clu/data/dataset_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24010 2022-12-16 16:33:37.000000 clu-0.0.8/clu/deterministic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2022-12-16 16:33:37.000000 clu-0.0.8/clu/deterministic_data_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-16 16:33:37.000000 clu-0.0.8/clu/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2022-12-16 16:33:37.000000 clu-0.0.8/clu/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2022-12-16 16:33:37.000000 clu-0.0.8/clu/internal/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu/metric_writers/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/async_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/async_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/logging_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/logging_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/multi_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/multi_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/summary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/summary_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/torch_tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/torch_tensorboard_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metric_writers/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25753 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2022-12-16 16:33:37.000000 clu-0.0.8/clu/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2022-12-16 16:33:37.000000 clu-0.0.8/clu/parameter_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-12-16 16:33:37.000000 clu-0.0.8/clu/parameter_overview_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2022-12-16 16:33:37.000000 clu-0.0.8/clu/periodic_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2022-12-16 16:33:37.000000 clu-0.0.8/clu/periodic_actions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-16 16:33:37.000000 clu-0.0.8/clu/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2022-12-16 16:33:37.000000 clu-0.0.8/clu/platform/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-16 16:33:37.000000 clu-0.0.8/clu/platform/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2022-12-16 16:33:37.000000 clu-0.0.8/clu/preprocess_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2022-12-16 16:33:37.000000 clu-0.0.8/clu/preprocess_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2022-12-16 16:33:37.000000 clu-0.0.8/clu/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2022-12-16 16:33:37.000000 clu-0.0.8/clu/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:33:49.621310 clu-0.0.8/clu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2022-12-16 16:33:49.000000 clu-0.0.8/clu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-16 16:33:49.000000 clu-0.0.8/clu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 16:33:49.000000 clu-0.0.8/clu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-16 16:33:49.000000 clu-0.0.8/clu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-16 16:33:49.000000 clu-0.0.8/clu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 16:33:49.621310 clu-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2022-12-16 16:33:37.000000 clu-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 07:33:48.000000 clu-0.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 07:33:48.000000 clu-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-26 07:34:01.849789 clu-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 07:33:48.000000 clu-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 07:33:48.000000 clu-0.0.9/clu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-26 07:33:48.000000 clu-0.0.9/clu/asynclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-26 07:33:48.000000 clu-0.0.9/clu/asynclib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21322 2023-04-26 07:33:48.000000 clu-0.0.9/clu/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-04-26 07:33:48.000000 clu-0.0.9/clu/checkpoint_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-26 07:33:48.000000 clu-0.0.9/clu/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-04-26 07:33:48.000000 clu-0.0.9/clu/data/dataset_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 07:33:48.000000 clu-0.0.9/clu/data/dataset_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-04-26 07:33:48.000000 clu-0.0.9/clu/deterministic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-04-26 07:33:48.000000 clu-0.0.9/clu/deterministic_data_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 07:33:48.000000 clu-0.0.9/clu/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-26 07:33:48.000000 clu-0.0.9/clu/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-26 07:33:48.000000 clu-0.0.9/clu/internal/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu/metric_writers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/async_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/async_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/logging_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/logging_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/multi_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/multi_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/summary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/summary_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/torch_tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/torch_tensorboard_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metric_writers/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29218 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-04-26 07:33:48.000000 clu-0.0.9/clu/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-26 07:33:48.000000 clu-0.0.9/clu/parameter_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-26 07:33:48.000000 clu-0.0.9/clu/parameter_overview_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-04-26 07:33:48.000000 clu-0.0.9/clu/periodic_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-26 07:33:48.000000 clu-0.0.9/clu/periodic_actions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 07:33:48.000000 clu-0.0.9/clu/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-26 07:33:48.000000 clu-0.0.9/clu/platform/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-26 07:33:48.000000 clu-0.0.9/clu/platform/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-04-26 07:33:48.000000 clu-0.0.9/clu/preprocess_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-26 07:33:48.000000 clu-0.0.9/clu/preprocess_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-26 07:33:48.000000 clu-0.0.9/clu/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 07:33:48.000000 clu-0.0.9/clu/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:34:01.849789 clu-0.0.9/clu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-26 07:34:01.000000 clu-0.0.9/clu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 07:34:01.000000 clu-0.0.9/clu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:34:01.000000 clu-0.0.9/clu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-26 07:34:01.000000 clu-0.0.9/clu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 07:34:01.000000 clu-0.0.9/clu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:34:01.849789 clu-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-26 07:33:48.000000 clu-0.0.9/setup.py
```

### Comparing `clu-0.0.8/LICENSE` & `clu-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clu-0.0.8/PKG-INFO` & `clu-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of libraries for ML training loops in JAX.
 Home-page: http://github.com/google/CommonLoopUtils
 Author: Common Loop Utils Authors
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: JAX machine learning
 Classifier: Development Status :: 4 - Beta
@@ -23,19 +23,19 @@
 
 This repository contains common functionality for writing ML training loops. The
 goal is to make trainings loops short and readable (but moving common tasks to
 small libraries) without removing the flexibility required for research.
 
 To get started, check out this Colab:
 
-https://colab.research.google.com/github/google/CommonLoopUtils/blob/master/clu_synopsis.ipynb
+https://colab.research.google.com/github/google/CommonLoopUtils/blob/main/clu_synopsis.ipynb
 
 If you're looking for usage examples, see:
 
-https://github.com/google/flax/tree/master/examples
+https://github.com/google/flax/tree/main/examples
 
 You can also find answers to common questions about CLU on Flax Github
 discussions page:
 
 https://github.com/google/flax/discussions
 
 Note: As this point we are not accepting contributions. Please fork the
```

### Comparing `clu-0.0.8/README.md` & `clu-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 This repository contains common functionality for writing ML training loops. The
 goal is to make trainings loops short and readable (but moving common tasks to
 small libraries) without removing the flexibility required for research.
 
 To get started, check out this Colab:
 
-https://colab.research.google.com/github/google/CommonLoopUtils/blob/master/clu_synopsis.ipynb
+https://colab.research.google.com/github/google/CommonLoopUtils/blob/main/clu_synopsis.ipynb
 
 If you're looking for usage examples, see:
 
-https://github.com/google/flax/tree/master/examples
+https://github.com/google/flax/tree/main/examples
 
 You can also find answers to common questions about CLU on Flax Github
 discussions page:
 
 https://github.com/google/flax/discussions
 
 Note: As this point we are not accepting contributions. Please fork the
```

### Comparing `clu-0.0.8/clu/__init__.py` & `clu-0.0.9/clu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/asynclib.py` & `clu-0.0.9/clu/asynclib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/asynclib_test.py` & `clu-0.0.9/clu/asynclib_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/checkpoint.py` & `clu-0.0.9/clu/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -72,15 +72,15 @@
 
 T = TypeVar("T")
 SCHEME_RE = re.compile("^(?P<scheme>[a-z][a-z0-9.+-]+://)?(?P<path>.*)", re.I)
 
 
 def safe_normpath(path: str) -> str:
   """Normalizes path safely to get around `gfile.glob()` limitations."""
-  d = SCHEME_RE.match(path).groupdict()
+  d = SCHEME_RE.match(path).groupdict()  # pytype: disable=attribute-error  # re-none
   return (d["scheme"] or "") + os.path.normpath(d["path"])
 
 
 def load_state_dict(base_directory) -> Dict[str, Any]:
   """Restores `state` as dictionary from the latest checkpoint.
 
   Synopsis:
```

### Comparing `clu-0.0.8/clu/checkpoint_test.py` & `clu-0.0.9/clu/checkpoint_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/data/__init__.py` & `clu-0.0.9/clu/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/data/dataset_iterator.py` & `clu-0.0.9/clu/data/dataset_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/data/dataset_iterator_test.py` & `clu-0.0.9/clu/data/dataset_iterator_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/deterministic_data.py` & `clu-0.0.9/clu/deterministic_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/deterministic_data_test.py` & `clu-0.0.9/clu/deterministic_data_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/internal/__init__.py` & `clu-0.0.9/clu/internal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/internal/utils.py` & `clu-0.0.9/clu/internal/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/internal/utils_test.py` & `clu-0.0.9/clu/internal/utils_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/__init__.py` & `clu-0.0.9/clu/metric_writers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/async_writer.py` & `clu-0.0.9/clu/metric_writers/async_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/async_writer_test.py` & `clu-0.0.9/clu/metric_writers/async_writer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/interface.py` & `clu-0.0.9/clu/metric_writers/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/logging_writer.py` & `clu-0.0.9/clu/metric_writers/logging_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -38,15 +38,15 @@
       values: Mapping[str, Array],
       metadata: Optional[Mapping[str, Any]] = None):
     logging.info("[%d]%s Got raw tensors: %s.", step, self._collection_str,
                  {k: v.shape for k, v in values.items()})
 
   def write_scalars(self, step: int, scalars: Mapping[str, Scalar]):
     values = [
-        f"{k}={v:.6f}" if isinstance(v, float) else f"{k}={v}"
+        f"{k}={v:.6g}" if isinstance(v, float) else f"{k}={v}"
         for k, v in sorted(scalars.items())
     ]
     logging.info("[%d]%s %s", step, self._collection_str, ", ".join(values))
 
   def write_images(self, step: int, images: Mapping[str, Array]):
     logging.info("[%d]%s Got images: %s.", step, self._collection_str,
                  {k: v.shape for k, v in images.items()})
```

### Comparing `clu-0.0.8/clu/metric_writers/logging_writer_test.py` & `clu-0.0.9/clu/metric_writers/logging_writer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,18 +24,18 @@
   def setUp(self):
     super().setUp()
     self.writer = logging_writer.LoggingWriter()
 
   def test_write_scalars(self):
     with self.assertLogs(level="INFO") as logs:
       self.writer.write_scalars(0, {"a": 3, "b": 0.15})
-      self.writer.write_scalars(2, {"a": 5, "b": 0.007})
+      self.writer.write_scalars(2, {"a": 0.0000005, "b": 0.007})
     self.assertEqual(
         logs.output,
-        ["INFO:absl:[0] a=3, b=0.150000", "INFO:absl:[2] a=5, b=0.007000"])
+        ["INFO:absl:[0] a=3, b=0.15", "INFO:absl:[2] a=5e-07, b=0.007"])
 
   def test_write_images(self):
     images = np.zeros((2, 28, 28, 3))
     with self.assertLogs(level="INFO") as logs:
       self.writer.write_images(4, {"input_images": images})
     self.assertEqual(
         logs.output,
@@ -100,15 +100,15 @@
           },
           num_buckets={
               "a": 2,
           })
       writer.write_hparams({"learning_rate": 0.1})
 
     self.assertEqual(logs.output, [
-        "INFO:absl:[0] collection=train a=3, b=0.150000",
+        "INFO:absl:[0] collection=train a=3, b=0.15",
         "INFO:absl:[4] collection=train Got images: {'input_images': (2, 28, 28, 3)}.",
         "INFO:absl:[4] collection=train Got texts: {'samples': 'bla'}.",
         "INFO:absl:[4] collection=train Histogram for 'a' = {[-0.1, 0.1): 1, [0.1, 0.3]: 2}",
         "INFO:absl:[Hyperparameters] collection=train {'learning_rate': 0.1}",
     ])
```

### Comparing `clu-0.0.8/clu/metric_writers/multi_writer.py` & `clu-0.0.9/clu/metric_writers/multi_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/multi_writer_test.py` & `clu-0.0.9/clu/metric_writers/multi_writer_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/summary_writer.py` & `clu-0.0.9/clu/metric_writers/summary_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/summary_writer_test.py` & `clu-0.0.9/clu/metric_writers/summary_writer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/torch_tensorboard_writer.py` & `clu-0.0.9/clu/metric_writers/torch_tensorboard_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/torch_tensorboard_writer_test.py` & `clu-0.0.9/clu/metric_writers/torch_tensorboard_writer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metric_writers/utils.py` & `clu-0.0.9/clu/metric_writers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,15 +60,15 @@
 
   Args:
     writer: MetricWriter object
     step: Step at which the arrays were generated.
     metrics: Mapping from name to clu.values.Value object.
   """
   writes = collections.defaultdict(dict)
-  histogram_num_buckets = collections.defaultdict(dict)
+  histogram_num_buckets = collections.defaultdict(int)
   for k, v in metrics.items():
     if isinstance(v, values.Summary):
       writes[(writer.write_summaries, frozenset({"metadata": v.metadata
                                                 }.items()))][k] = v.value
     elif _is_scalar(v):
       if isinstance(v, values.Scalar):
         writes[(writer.write_scalars, frozenset())][k] = v.value
@@ -88,15 +88,15 @@
               frozenset({"sample_rate": v.sample_rate}.items()))][k] = v.value
     else:
       raise ValueError("Metric: ", k, " has unsupported value: ", v)
 
   for (fn, extra_args), vals in writes.items():
     if fn == writer.write_histograms:
       # for write_histograms, the num_buckets arg is a Dict indexed by name
-      fn(step, vals, num_buckets=histogram_num_buckets)
+      writer.write_histograms(step, vals, num_buckets=histogram_num_buckets)
     else:
       fn(step, vals, **dict(extra_args))
 
 
 def create_default_writer(
     logdir: Optional[epath.PathLike] = None,
     *,
```

### Comparing `clu-0.0.8/clu/metric_writers/utils_test.py` & `clu-0.0.9/clu/metric_writers/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/metrics.py` & `clu-0.0.9/clu/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -77,15 +77,15 @@
   if a.shape != b.shape:
     raise ValueError(f"Expected same shape: {a.shape} != {b.shape}")
 
 
 class Metric:
   """Interface for computing metrics from intermediate values.
 
-  Refer to `Collection` for computing multipel metrics at the same time.
+  Refer to `Collection` for computing multiple metrics at the same time.
 
   Synopsis:
 
     import jax.numpy as jnp
     import flax
 
     @flax.struct.dataclass
@@ -118,42 +118,58 @@
     """Creates a `Metric` from model outputs."""
     raise NotImplementedError("Must override from_model_output()")
 
   def merge(self, other: "Metric") -> "Metric":
     """Returns `Metric` that is the accumulation of `self` and `other`.
 
     Args:
-      other: A `Metric` whose inermediate values should be accumulated onto the
+      other: A `Metric` whose intermediate values should be accumulated onto the
         values of `self`. Note that in a distributed setting, `other` will
         typically be the output of a `jax.lax` parallel operator and thus have a
         dimension added to the dataclass returned by `.from_model_output()`.
 
     Returns:
       A new `Metric` that accumulates the value from both `self` and `other`.
     """
     raise NotImplementedError("Must override merge()")
 
+  def merge_reduce(self, other: "Metric") -> "Metric":
+    return self.merge(other)
+
   def compute(self) -> jnp.array:
     """Computes final metrics from intermediate values."""
     raise NotImplementedError("Must override compute()")
 
   @classmethod
   def empty(cls) -> "Metric":
     """Returns an empty instance (i.e. `.merge(Metric.empty())` is a no-op)."""
     raise NotImplementedError("Must override empty()")
 
   def compute_value(self) -> clu.values.Value:
     """Wraps compute() and returns a values.Value."""
     return clu.values.Scalar(self.compute())
 
   def reduce(self) -> "Metric":
-    """Reduces the metric along it first axis by calling `merge()`."""
+    """Reduces the metric along it first axis by calling `reduce_merge()`.
+
+    This function primary use case is to aggregate metrics collected across
+    multiple devices, rather than "merging" metrics across multiple steps.
+
+    In many cases these have the same semantics (such as `Average`), but
+    in some such as LastValue's batch averaging, reduction across devices is
+    averaging, while reduction across steps is taking the last value.
+
+    See `Collection.reduce`, for usage patterns.
+
+    Returns:
+      reduced metric.
+    """
 
     def reduce_step(reduced: Metric, metric: Metric) -> Tuple[Metric, None]:
-      return reduced.merge(metric), None
+      return reduced.merge_reduce(metric), None
 
     first = jax.tree_map(lambda x: x[0], self)
     remainder = jax.tree_map(lambda x: x[1:], self)
     # TODO(b/160868467) Verify this adds no significant computational cost.
     return jax.lax.scan(reduce_step, first, remainder)[0]
 
   @classmethod
@@ -541,15 +557,40 @@
     """Returns `Collection` that is the accumulation of `self` and `other`."""
     return type(self)(**{
         metric_name: metric.merge(getattr(other, metric_name))
         for metric_name, metric in vars(self).items()
     })
 
   def reduce(self) -> "Collection":
-    """Reduces the collection by calling `Metric.reduce()` on each metric."""
+    """Reduces the collection by calling `Metric.reduce()` on each metric.
+
+    The primary use case is to reduce collection that was gathered
+    from  multiple devices into one collection: For instance inside pmap
+
+    ```
+      col = jax.lax.all_gather(col, axis_name='foo').reduce()
+    ```
+    or, if computed directly from model_outputs:
+
+    ```
+      col = col.merge(col.gather_from_model_output(**outputs)))
+    ```
+
+    will sync collections across all devices to create a replicated collection
+    that include statistics from all devices.
+    Outside pmap, this metric can then be safely unreplicated using for
+    `collection.unreplicate()`.
+
+    If `collection.unreplicate()` is called without gathering it will only
+    contain the statistics from the first device, which is rarely a desired
+    behavior.
+
+    Returns:
+      Reduced collection.
+    """
     return type(self)(**{
         metric_name: metric.reduce()
         for metric_name, metric in vars(self).items()
     })
 
   def compute(self) -> Dict[str, jnp.array]:
     """Returns a dictionary mapping metric field name to `Metric.compute()`."""
@@ -566,44 +607,98 @@
     return {
         metric_name: metric.compute_value()
         for metric_name, metric in vars(self).items()
         if metric_name != "_reduction_counter"
     }
 
   def unreplicate(self) -> "Collection":
-    """Short-hand for `flax.jax_utils.unreplicate(self)`."""
+    """Short-hand for `flax.jax_utils.unreplicate(self)`.
+
+    The collection should be gathered and `reduce`d inside pmap,
+    using `gather_from_model_output` or all_gather / reduce for this
+    function to return correct values. See `Collection.reduce` for details.
+
+    Returns:
+      Unreplicated collection
+    """
     return flax.jax_utils.unreplicate(self)
 
 
 @flax.struct.dataclass
 class LastValue(Metric):
-  """Keeps the last average batch value.
+  """Keeps the last average global batch value.
 
-  This is useful to log values like the learning rate.
+  This is useful to log values such as learning rate and losses during training.
+
+  This class mirrors Average, because it needs to maintain total/count
+  in cases when batch is distributed across multiple devices and need
+  to be averaged later. However, we don't inherit from Average to
+  maintain backward compatibility in case of isinstance(metric, Average)
+  check.  For backward compatibility this class can be initialized using the
+  keyword `LastValue(value=10)`  or  `total` and `count`.
   """
+  total: jnp.array
+  count: jnp.array
 
-  value: jnp.array
+  def __init__(self, total: Optional[jnp.array] = None,
+               count: Optional[jnp.array] = None,
+               value: Optional[jnp.array] = None,
+               ):
+    """Constructor which supports keyword argument value as initializer.
+
+    If  "value" is provided, then  "total" should *not* be provided.
+
+    Args:
+      total: Total value.
+      count: Count of examples, 1 if not provided
+      value: Value, if provided, will be assumed to be "count" of values.
+    """
+    count = count if count is not None else jnp.array(1, dtype=jnp.int32)
+    if value is not None:
+      if total is not None:
+        raise ValueError("Only one of 'total' and 'value' should be None. "
+                         f'Got {total}, {value}')
+      total = value * count
+    object.__setattr__(self, "total", total)
+    object.__setattr__(self, "count", count)
 
   @classmethod
   def empty(cls):
-    return cls(value=jnp.array(jnp.nan, jnp.float32))
+    return cls(jnp.array(0, jnp.float32), count=jnp.array(0, jnp.int32))
 
   @classmethod
   def from_model_output(cls,
                         value: jnp.array,
                         mask: Optional[jnp.array] = None,
                         **_) -> Metric:
     if mask is None:
       mask = jnp.ones((value.shape or [()])[0])
-    return cls(jnp.where(mask, value, jnp.zeros_like(value)).sum() / mask.sum())
+    return cls(
+        total=jnp.where(mask, value, jnp.zeros_like(value)).sum(),
+        count=mask.sum().astype(jnp.int32),
+    )
 
   def merge(self, other: "LastValue") -> "LastValue":
     _assert_same_shape(self.value, other.value)
     return other
 
+  def merge_reduce(self, other: "LastValue") -> "LastValue":
+    # We need to average during reduction
+    _assert_same_shape(self.total, other.total)
+    return type(self)(
+        total=self.total + other.total,
+        count=self.count + other.count,
+    )
+
+  @property
+  def value(self) -> jnp.array:
+    # Explicitly allow NaN division as it is part of normal computation here.
+    with jax.debug_nans(False):
+      return self.total / self.count
+
   def compute(self) -> Any:
     return self.value
 
 
 @flax.struct.dataclass
 class Average(Metric):
   """Computes the average of a scalar or a batch of tensors.
```

### Comparing `clu-0.0.8/clu/metrics_test.py` & `clu-0.0.9/clu/metrics_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -90,14 +90,24 @@
         "train_accuracy": 0.75,
         "learning_rate": 0.01,
     }
     self.results_masked = {
         "train_accuracy": 0.5,
         "learning_rate": 0.01,
     }
+    self.results_gather = {
+        "train_accuracy": 0.75,
+        "learning_rate": 0.015,  # Gathering averages distributed batches.
+    }
+
+    self.results_gather_masked = {
+        "train_accuracy": 0.5,
+        "learning_rate": 0.015,  # Gathering averages distributed batches.
+    }
+
     # Stack all values. Can for example be used in a pmap().
     self.model_outputs_stacked = jax.tree_map(lambda *args: jnp.stack(args),
                                               *self.model_outputs)
     self.model_outputs_masked_stacked = jax.tree_map(
         lambda *args: jnp.stack(args), *self.model_outputs_masked)
 
   def make_compute_metric(self, metric_class, reduce, jit=True):
@@ -129,19 +139,52 @@
           metric = metric.merge(update)
       return metric.compute()
 
     if jit:
       compute_metric = jax.jit(compute_metric)
     return compute_metric
 
-  def test_metric_reduce(self):
+  def test_metric_last_value_reduce(self):
     metric1 = metrics.LastValue.from_model_output(jnp.array([1, 2]))
     metric2 = metrics.LastValue.from_model_output(jnp.array([3, 4]))
+    metric3 = metrics.LastValue.from_model_output(jnp.array([3, 4]),
+                                                  jnp.array([0, 0]))
     metric12 = jax.tree_map(lambda *args: jnp.stack(args), metric1, metric2)
-    chex.assert_trees_all_equal(metric12.reduce().compute(), metric2.compute())
+    metric21 = jax.tree_map(lambda *args: jnp.stack(args), metric2, metric1)
+    self.assertEqual(metric12.reduce().value, 2.5)
+
+    chex.assert_trees_all_equal(metric12.reduce().compute(),
+                                metric21.reduce().compute())
+
+    metric13 = jax.tree_map(lambda *args: jnp.stack(args), metric1, metric3)
+    metric31 = jax.tree_map(lambda *args: jnp.stack(args), metric1, metric3)
+    self.assertEqual(metric13.reduce().value, 1.5)
+    chex.assert_trees_all_equal(metric13.reduce().compute(),
+                                metric31.reduce().compute())
+
+  def test_metric_last_value(self):
+    metric0 = metrics.LastValue.from_model_output(jnp.array([]))
+    metric1 = metrics.LastValue.from_model_output(jnp.array([1, 2]))
+    metric2 = metrics.LastValue.from_model_output(jnp.array([3, 4]))
+    np.testing.assert_equal(metric0.value, jnp.array(np.nan))
+    with jax.debug_nans(True):
+      # Verify that metrics is computable even under strict NaN checking.
+      _ = metric0.value
+    metric01 = metric0.merge(metric1)
+    self.assertEqual(metric01.value, 1.5)
+    metric12 = metric1.merge(metric2)
+    self.assertEqual(metric1.value, 1.5)
+    self.assertEqual(metric12.value, 3.5)
+    chex.assert_trees_all_equal(metric12.compute(), metric2.compute())
+
+  def test_metric_last_value_legacy_kwarg_value(self):
+    metric = metrics.LastValue(value=2.0)
+    self.assertEqual(metric.total, 2.0)
+    metric = metrics.LastValue(value=2.0, count=3)
+    self.assertEqual(metric.total, 6.0)
 
   def test_from_fun_with_single_output(self):
 
     def accuracy(*, logits, labels, **_):
       return (logits.argmax(axis=-1) == labels).astype(jnp.float32)
 
     chex.assert_trees_all_close(
@@ -339,31 +382,31 @@
 
   @parameterized.named_parameters(
       ("", False),
       ("_masked", True),
   )
   @mock.patch("jax.lax.all_gather")
   def test_collection_gather(self, masked, all_gather_mock):
-
+    model_outputs = self.model_outputs_masked if masked else self.model_outputs
     collections = [
         Collection.single_from_model_output(**model_output)
-        for model_output in (
-            self.model_outputs_masked if masked else self.model_outputs)
+        for model_output in (model_outputs)
+
     ]
     all_gather_mock.return_value = jax.tree_map(lambda *args: jnp.stack(args),
                                                 *collections)
 
     def compute_collection(model_outputs):
       collection = Collection.gather_from_model_output(**model_outputs[0])
       return collection.compute()
 
-    chex.assert_trees_all_close(
-        jax.jit(compute_collection)(
-            self.model_outputs_masked if masked else self.model_outputs),
-        self.results_masked if masked else self.results)
+    observed = jax.jit(compute_collection)(model_outputs)
+
+    expectation = self.results_gather_masked if masked else self.results_gather
+    chex.assert_trees_all_close(observed, expectation)
 
   @parameterized.named_parameters(
       ("", False),
       ("_masked", True),
   )
   def test_collection_gather_pmap(self, masked):
 
@@ -372,15 +415,15 @@
       return Collection.gather_from_model_output(**model_outputs)
 
     if jax.local_device_count() > 1:
       chex.assert_trees_all_close(
           compute_collection(
               self.model_outputs_masked_stacked if masked else self
               .model_outputs_stacked).unreplicate().compute(),
-          self.results_masked if masked else self.results)
+          self.results_gather_masked if masked else self.results_gather)
 
   def test_collection_asserts_replication(self):
     collections = [
         Collection.single_from_model_output(**model_output)
         for model_output in self.model_outputs
     ]
     collection = jax.tree_map(lambda *args: jnp.stack(args), *collections)
```

### Comparing `clu-0.0.8/clu/parameter_overview.py` & `clu-0.0.9/clu/parameter_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -223,15 +223,15 @@
   | FC_1/weights:0 | (63612, 1024) | 65,138,688 |
   | FC_1/biases:0  |       (1024,) |      1,024 |
   | FC_2/weights:0 |    (1024, 32) |     32,768 |
   | FC_2/biases:0  |         (32,) |         32 |
   +----------------+---------------+------------+
   Total: 65,172,512
   """
-  if isinstance(params, (dict, flax.core.FrozenDict)):
+  if include_stats and isinstance(params, (dict, flax.core.FrozenDict)):
     params = jax.tree_map(np.asarray, params)
   rows = get_parameter_rows(params, include_stats=include_stats)
   total_weights = count_parameters(params)
   RowType = ParamRowWithStats if include_stats else ParamRow
   # Pass in `column_names` to enable rendering empty tables.
   column_names = [field.name for field in dataclasses.fields(RowType)]
   table = make_table(rows, max_lines=max_lines, column_names=column_names)
```

### Comparing `clu-0.0.8/clu/parameter_overview_test.py` & `clu-0.0.9/clu/parameter_overview_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/periodic_actions.py` & `clu-0.0.9/clu/periodic_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/periodic_actions_test.py` & `clu-0.0.9/clu/periodic_actions_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/platform/__init__.py` & `clu-0.0.9/clu/platform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/platform/interface.py` & `clu-0.0.9/clu/platform/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/platform/local.py` & `clu-0.0.9/clu/platform/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/preprocess_spec.py` & `clu-0.0.9/clu/preprocess_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/preprocess_spec_test.py` & `clu-0.0.9/clu/preprocess_spec_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/profiler.py` & `clu-0.0.9/clu/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu/values.py` & `clu-0.0.9/clu/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `clu-0.0.8/clu.egg-info/PKG-INFO` & `clu-0.0.9/clu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of libraries for ML training loops in JAX.
 Home-page: http://github.com/google/CommonLoopUtils
 Author: Common Loop Utils Authors
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: JAX machine learning
 Classifier: Development Status :: 4 - Beta
@@ -23,19 +23,19 @@
 
 This repository contains common functionality for writing ML training loops. The
 goal is to make trainings loops short and readable (but moving common tasks to
 small libraries) without removing the flexibility required for research.
 
 To get started, check out this Colab:
 
-https://colab.research.google.com/github/google/CommonLoopUtils/blob/master/clu_synopsis.ipynb
+https://colab.research.google.com/github/google/CommonLoopUtils/blob/main/clu_synopsis.ipynb
 
 If you're looking for usage examples, see:
 
-https://github.com/google/flax/tree/master/examples
+https://github.com/google/flax/tree/main/examples
 
 You can also find answers to common questions about CLU on Flax Github
 discussions page:
 
 https://github.com/google/flax/discussions
 
 Note: As this point we are not accepting contributions. Please fork the
```

### Comparing `clu-0.0.8/clu.egg-info/SOURCES.txt` & `clu-0.0.9/clu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clu-0.0.8/setup.py` & `clu-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The CLU Authors.
+# Copyright 2023 The CLU Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,23 +22,24 @@
 from setuptools import find_packages
 from setuptools import setup
 
 tests_require = [
     "pytest",
     "tensorflow",
     "tensorflow_datasets",
-    "torch>=1.2.0",
+    # Temporarily disabling torch-2.0.0 since this fails Github actions.
+    "torch>=1.13.0,!=2.0.0",
 ]
 pytorch_require = [
-    "torch>=1.2.0",
+    "torch>=1.13.0",
 ]
 
 setup(
     name="clu",
-    version="0.0.8",
+    version="0.0.9",
     description=("Set of libraries for ML training loops in JAX."),
     author="Common Loop Utils Authors",
     author_email="no-reply@google.com",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/google/CommonLoopUtils",
     license="Apache 2.0",
```

