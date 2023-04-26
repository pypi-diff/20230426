# Comparing `tmp/draco-ml-0.2.0.tar.gz` & `tmp/draco-ml-0.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/draco-ml-0.2.0.tar", last modified: Tue Apr 12 07:28:22 2022, max compression
+gzip compressed data, was "draco-ml-0.2.1.dev0.tar", last modified: Wed Apr 26 14:33:59 2023, max compression
```

## Comparing `draco-ml-0.2.0.tar` & `draco-ml-0.2.1.dev0.tar`

### file list

```diff
@@ -1,86 +1,72 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/
--rw-r--r--   0 sarah      (501) staff       (20)       94 2022-04-12 07:27:17.000000 draco-ml-0.2.0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8306 2022-04-12 07:27:17.000000 draco-ml-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3069 2022-04-12 07:28:18.000000 draco-ml-0.2.0/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2022-04-12 07:27:17.000000 draco-ml-0.2.0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      297 2022-04-12 07:27:17.000000 draco-ml-0.2.0/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)    14358 2022-04-12 07:28:22.000000 draco-ml-0.2.0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)    10460 2022-04-12 07:28:18.000000 draco-ml-0.2.0/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      606 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/Makefile
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/docs/advanced_usage/
--rw-r--r--   0 sarah      (501) staff       (20)     2501 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/advanced_usage/concepts.md
--rw-r--r--   0 sarah      (501) staff       (20)     2537 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/advanced_usage/csv.md
--rw-r--r--   0 sarah      (501) staff       (20)     3532 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/advanced_usage/docker.md
--rw-r--r--   0 sarah      (501) staff       (20)       28 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/authors.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5902 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)       33 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)     7263 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/images/Draco-200.png
--rw-r--r--   0 sarah      (501) staff       (20)    27132 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/images/Draco.png
--rw-r--r--   0 sarah      (501) staff       (20)   886153 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/images/dai-logo.png
--rw-r--r--   0 sarah      (501) staff       (20)      541 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      767 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/make.bat
--rw-r--r--   0 sarah      (501) staff       (20)       28 2022-04-12 07:27:17.000000 draco-ml-0.2.0/docs/readme.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/
--rw-r--r--   0 sarah      (501) staff       (20)      512 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    36486 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)     2103 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/db.py
--rw-r--r--   0 sarah      (501) staff       (20)     2925 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/demo.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/loaders/
--rw-r--r--   0 sarah      (501) staff       (20)       72 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/loaders/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     8858 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/loaders/csv.py
--rw-r--r--   0 sarah      (501) staff       (20)     2768 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/metrics.py
--rw-r--r--   0 sarah      (501) staff       (20)    23391 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipeline.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/
--rw-r--r--   0 sarah      (501) staff       (20)      764 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb.json
--rw-r--r--   0 sarah      (501) staff       (20)     1160 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_prob_with_double_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)     1364 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_prob_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     1332 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_prob_with_unstack_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)     1039 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_with_double_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)      768 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_with_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)     1243 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     1211 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb_with_unstack_normalization.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/double_lstm/
--rw-r--r--   0 sarah      (501) staff       (20)     2531 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     2731 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_prob.json
--rw-r--r--   0 sarah      (501) staff       (20)     3160 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     2960 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/dummy/
--rw-r--r--   0 sarah      (501) staff       (20)      440 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/dummy/dummy.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/lstm/
--rw-r--r--   0 sarah      (501) staff       (20)     2519 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/lstm/lstm.json
--rw-r--r--   0 sarah      (501) staff       (20)     2719 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/lstm/lstm_prob.json
--rw-r--r--   0 sarah      (501) staff       (20)     3148 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/lstm/lstm_prob_with_unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     2948 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/lstm/lstm_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/lstm_regressor/
--rw-r--r--   0 sarah      (501) staff       (20)     2517 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/lstm_regressor/lstm_regressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     2946 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/pipelines/preprocessing/
--rw-r--r--   0 sarah      (501) staff       (20)     1502 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/preprocessing/double_entity_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)      824 2022-04-12 07:28:19.000000 draco-ml-0.2.0/draco/pipelines/preprocessing/entity_dataframe.json
--rw-r--r--   0 sarah      (501) staff       (20)      597 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/preprocessing/entity_normalization.json
--rw-r--r--   0 sarah      (501) staff       (20)     1001 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/pipelines/preprocessing/unstack.json
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)      862 2022-04-12 07:28:18.000000 draco-ml-0.2.0/draco/primitives/mlblocks.MLPipeline.json
--rw-r--r--   0 sarah      (501) staff       (20)      918 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/primitives/numpy.take.json
--rw-r--r--   0 sarah      (501) staff       (20)     2232 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/primitives/xgboost.XGBClassifier:probabilities.json
--rw-r--r--   0 sarah      (501) staff       (20)     3852 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/results.py
--rw-r--r--   0 sarah      (501) staff       (20)     6143 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/targets.py
--rw-r--r--   0 sarah      (501) staff       (20)     1682 2022-04-12 07:27:17.000000 draco-ml-0.2.0/draco/utils.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/draco_ml.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    14358 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     2199 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)       88 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      813 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        6 2022-04-12 07:28:21.000000 draco-ml-0.2.0/draco_ml.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1018 2022-04-12 07:28:22.000000 draco-ml-0.2.0/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     2956 2022-04-12 07:28:19.000000 draco-ml-0.2.0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2022-04-12 07:28:22.000000 draco-ml-0.2.0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)     1882 2022-04-12 07:28:18.000000 draco-ml-0.2.0/tests/test_benchmark.py
--rw-r--r--   0 sarah      (501) staff       (20)     1218 2022-04-12 07:27:17.000000 draco-ml-0.2.0/tests/test_metrics.py
--rw-r--r--   0 sarah      (501) staff       (20)     2316 2022-04-12 07:28:18.000000 draco-ml-0.2.0/tests/test_pipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.012706 draco-ml-0.2.1.dev0/
+-rw-r--r--   0 sarah      (501) staff       (20)       94 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8306 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3069 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      297 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    14191 2023-04-26 14:33:59.013166 draco-ml-0.2.1.dev0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)    10324 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.968815 draco-ml-0.2.1.dev0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      606 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/Makefile
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.970767 draco-ml-0.2.1.dev0/docs/advanced_usage/
+-rw-r--r--   0 sarah      (501) staff       (20)     2501 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/concepts.md
+-rw-r--r--   0 sarah      (501) staff       (20)     2537 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/csv.md
+-rw-r--r--   0 sarah      (501) staff       (20)     3532 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/advanced_usage/docker.md
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/authors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5886 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.973358 draco-ml-0.2.1.dev0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)     7263 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/Draco-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)    27132 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/Draco.png
+-rw-r--r--   0 sarah      (501) staff       (20)   886153 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/images/dai-logo.png
+-rw-r--r--   0 sarah      (501) staff       (20)      541 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      767 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/make.bat
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/docs/readme.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.985453 draco-ml-0.2.1.dev0/draco/
+-rw-r--r--   0 sarah      (501) staff       (20)      517 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    36486 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2103 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/db.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2925 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/demo.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.987092 draco-ml-0.2.1.dev0/draco/loaders/
+-rw-r--r--   0 sarah      (501) staff       (20)       72 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/loaders/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     8858 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/loaders/csv.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2768 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/metrics.py
+-rw-r--r--   0 sarah      (501) staff       (20)    23386 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.955813 draco-ml-0.2.1.dev0/draco/pipelines/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.991727 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/
+-rw-r--r--   0 sarah      (501) staff       (20)     2516 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2716 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3302 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.992797 draco-ml-0.2.1.dev0/draco/pipelines/dummy/
+-rw-r--r--   0 sarah      (501) staff       (20)      166 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/dummy/dummy.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:58.997426 draco-ml-0.2.1.dev0/draco/pipelines/lstm/
+-rw-r--r--   0 sarah      (501) staff       (20)     2504 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2704 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3490 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob_with_unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3290 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.000169 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/
+-rw-r--r--   0 sarah      (501) staff       (20)     2502 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3286 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.003246 draco-ml-0.2.1.dev0/draco/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)      862 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/mlblocks.MLPipeline.json
+-rw-r--r--   0 sarah      (501) staff       (20)      918 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/numpy.take.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2232 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/primitives/xgboost.XGBClassifier:probabilities.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3852 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/results.py
+-rw-r--r--   0 sarah      (501) staff       (20)     6143 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/targets.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1682 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/draco/utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.008370 draco-ml-0.2.1.dev0/draco_ml.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    14191 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     1523 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       87 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      833 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        6 2023-04-26 14:33:58.000000 draco-ml-0.2.1.dev0/draco_ml.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1023 2023-04-26 14:33:59.015084 draco-ml-0.2.1.dev0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2999 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-26 14:33:59.011654 draco-ml-0.2.1.dev0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)     1860 2023-04-13 20:29:53.000000 draco-ml-0.2.1.dev0/tests/test_benchmark.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1218 2023-04-06 18:13:31.000000 draco-ml-0.2.1.dev0/tests/test_metrics.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2547 2023-04-25 20:17:28.000000 draco-ml-0.2.1.dev0/tests/test_pipeline.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `draco-ml-0.2.0/CONTRIBUTING.rst` & `draco-ml-0.2.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/HISTORY.md` & `draco-ml-0.2.1.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/LICENSE` & `draco-ml-0.2.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/PKG-INFO` & `draco-ml-0.2.1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: draco-ml
-Version: 0.2.0
-Summary: AutoML for Renewable Energy Industries.
+Version: 0.2.1.dev0
+Summary: AutoML for Time Series.
 Home-page: https://github.com/sintel-dev/Draco
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: wind machine learning draco
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -29,15 +28,15 @@
 </p>
 
 <p align="left">
 <img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2019/03/GreenGuard.png" alt="Draco" />
 </p>
 
 <p align="left">
-AutoML for Renewable Energy Industries.
+AutoML for Time Series.
 </p>
 
 
 [![PyPI Shield](https://img.shields.io/pypi/v/draco-ml.svg)](https://pypi.python.org/pypi/draco-ml)
 [![Tests](https://github.com/sintel-dev/Draco/workflows/Run%20Tests/badge.svg)](https://github.com/sintel-dev/Draco/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
 [![Downloads](https://pepy.tech/badge/draco-ml)](https://pepy.tech/project/draco-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Draco/master?filepath=tutorials)
@@ -50,15 +49,15 @@
 - License: [MIT](https://github.com/sintel-dev/Draco/blob/master/LICENSE)
 - Documentation: https://sintel-dev.github.io/Draco
 - Homepage: https://github.com/sintel-dev/Draco
 
 ## Overview
 
 The Draco project is a collection of end-to-end solutions for machine learning problems
-commonly found in monitoring wind energy production systems. Most tasks utilize sensor data
+commonly found in time series monitoring systems. Most tasks utilize sensor data
 emanating from monitoring systems. We utilize the foundational innovations developed for
 automation of machine Learning at Data to AI Lab at MIT.
 
 The salient aspects of this customized project are:
 
 * A set of ready to use, well tested pipelines for different machine learning tasks. These are
   vetted through testing across multiple publicly available datasets for the same task.
@@ -241,26 +240,25 @@
 pipelines = get_pipelines()
 ```
 
 The returned `pipeline` variable will be `list` containing the names of all the pipelines
 available in the Draco system:
 
 ```
-['dfs_xgb',
- 'dfs_xgb_with_unstack',
- 'dfs_xgb_with_normalization',
- 'dfs_xgb_with_unstack_normalization',
- 'dfs_xgb_prob_with_unstack_normalization']
+['lstm',
+ 'lstm_with_unstack',
+ 'double_lstm',
+ 'double_lstm_with_unstack']
 ```
 
 For the rest of this tutorial, we will select and use the pipeline
-`dfs_xgb_with_unstack_normalization` as our template.
+`lstm_with_unstack` as our template.
 
 ```python3
-pipeline_name = 'dfs_xgb_with_unstack_normalization'
+pipeline_name = 'lstm_with_unstack'
 ```
 
 ## 3. Fitting the Pipeline
 
 Once we have loaded the data and selected the pipeline that we will use, we have to
 fit it.
 
@@ -412,9 +410,7 @@
 * initial collection of dfs and lstm based pipelines
 * optimized pipeline tuning
 * documentation and tutorials
 
 ### 0.1.0
 
 * First release on PyPI
-
-
```

### Comparing `draco-ml-0.2.0/README.md` & `draco-ml-0.2.1.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 </p>
 
 <p align="left">
 <img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2019/03/GreenGuard.png" alt="Draco" />
 </p>
 
 <p align="left">
-AutoML for Renewable Energy Industries.
+AutoML for Time Series.
 </p>
 
 
 [![PyPI Shield](https://img.shields.io/pypi/v/draco-ml.svg)](https://pypi.python.org/pypi/draco-ml)
 [![Tests](https://github.com/sintel-dev/Draco/workflows/Run%20Tests/badge.svg)](https://github.com/sintel-dev/Draco/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
 [![Downloads](https://pepy.tech/badge/draco-ml)](https://pepy.tech/project/draco-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Draco/master?filepath=tutorials)
@@ -25,15 +25,15 @@
 - License: [MIT](https://github.com/sintel-dev/Draco/blob/master/LICENSE)
 - Documentation: https://sintel-dev.github.io/Draco
 - Homepage: https://github.com/sintel-dev/Draco
 
 ## Overview
 
 The Draco project is a collection of end-to-end solutions for machine learning problems
-commonly found in monitoring wind energy production systems. Most tasks utilize sensor data
+commonly found in time series monitoring systems. Most tasks utilize sensor data
 emanating from monitoring systems. We utilize the foundational innovations developed for
 automation of machine Learning at Data to AI Lab at MIT.
 
 The salient aspects of this customized project are:
 
 * A set of ready to use, well tested pipelines for different machine learning tasks. These are
   vetted through testing across multiple publicly available datasets for the same task.
@@ -216,26 +216,25 @@
 pipelines = get_pipelines()
 ```
 
 The returned `pipeline` variable will be `list` containing the names of all the pipelines
 available in the Draco system:
 
 ```
-['dfs_xgb',
- 'dfs_xgb_with_unstack',
- 'dfs_xgb_with_normalization',
- 'dfs_xgb_with_unstack_normalization',
- 'dfs_xgb_prob_with_unstack_normalization']
+['lstm',
+ 'lstm_with_unstack',
+ 'double_lstm',
+ 'double_lstm_with_unstack']
 ```
 
 For the rest of this tutorial, we will select and use the pipeline
-`dfs_xgb_with_unstack_normalization` as our template.
+`lstm_with_unstack` as our template.
 
 ```python3
-pipeline_name = 'dfs_xgb_with_unstack_normalization'
+pipeline_name = 'lstm_with_unstack'
 ```
 
 ## 3. Fitting the Pipeline
 
 Once we have loaded the data and selected the pipeline that we will use, we have to
 fit it.
```

### Comparing `draco-ml-0.2.0/docs/Makefile` & `draco-ml-0.2.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/advanced_usage/concepts.md` & `draco-ml-0.2.1.dev0/docs/advanced_usage/concepts.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/advanced_usage/csv.md` & `draco-ml-0.2.1.dev0/docs/advanced_usage/csv.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/advanced_usage/docker.md` & `draco-ml-0.2.1.dev0/docs/advanced_usage/docker.md`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/conf.py` & `draco-ml-0.2.1.dev0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 # General information about the project.
 project = 'Draco'
 slug = 'draco'
 title = project + ' Documentation',
 copyright = '2018, MIT Data To AI Lab'
 author = 'MIT Data To AI Lab'
-description = 'AutoML for Renewable Energy Industries'
+description = 'AutoML for Time Series'
 user = 'sintel-dev'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
```

### Comparing `draco-ml-0.2.0/docs/images/Draco-200.png` & `draco-ml-0.2.1.dev0/docs/images/Draco-200.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/images/Draco.png` & `draco-ml-0.2.1.dev0/docs/images/Draco.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/images/dai-logo.png` & `draco-ml-0.2.1.dev0/docs/images/dai-logo.png`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/index.rst` & `draco-ml-0.2.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/docs/make.bat` & `draco-ml-0.2.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/benchmark.py` & `draco-ml-0.2.1.dev0/draco/benchmark.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/db.py` & `draco-ml-0.2.1.dev0/draco/db.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/demo.py` & `draco-ml-0.2.1.dev0/draco/demo.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/loaders/csv.py` & `draco-ml-0.2.1.dev0/draco/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/metrics.py` & `draco-ml-0.2.1.dev0/draco/metrics.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/pipeline.py` & `draco-ml-0.2.1.dev0/draco/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import keras
 import numpy as np
 from btb import BTBSession
 from btb.tuning import Tunable
 from mlblocks import MLPipeline
 from mlblocks.discovery import load_pipeline
-from mlprimitives.adapters.keras import Sequential
+from mlstars.adapters.keras import Sequential
 from sklearn.exceptions import NotFittedError
 from sklearn.model_selection import KFold, StratifiedKFold
 
 from draco.metrics import METRICS
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `draco-ml-0.2.0/draco/pipelines/dfs_xgb/dfs_xgb.json` & `draco-ml-0.2.1.dev0/draco/primitives/numpy.take.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('name', 'numpy.take'), ('contributors', ['Plamen Valentinov Kolev "*

 * *            "<plamen@csail.mit.edu>']), ('documentation', "*

 * *            "'https://docs.scipy.org/doc/numpy/reference/'), ('description', 'Take elements from "*

 * *            "an array along an axis.'), ('classifiers', OrderedDict([('type', 'postprocessor')])), "*

 * *            "('modalities', []), ('primitive', 'numpy.take'), ('produce', OrderedDict([('args', "*

 * *            "[OrderedDict([('name', 'y'), ('keyword', 'a'), […]*

```diff
@@ -1,29 +1,40 @@
 {
-    "init_params": {
-        "featuretools.dfs#1": {
-            "copy": true,
-            "encode": false,
-            "index": "turbine_id",
-            "max_depth": -1,
-            "n_jobs": 1,
-            "target_entity": "turbines",
-            "time_index": "cutoff_time",
-            "training_window": "1d",
-            "verbose": false
-        },
-        "mlblocks.MLPipeline#1": {
-            "pipeline": "preprocessing.entity_dataframe"
-        }
+    "classifiers": {
+        "type": "postprocessor"
     },
-    "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "dataframe": "readings"
+    "contributors": [
+        "Plamen Valentinov Kolev <plamen@csail.mit.edu>"
+    ],
+    "description": "Take elements from an array along an axis.",
+    "documentation": "https://docs.scipy.org/doc/numpy/reference/",
+    "hyperparameters": {
+        "fixed": {
+            "axis": {
+                "default": null,
+                "type": "int"
+            },
+            "indices": {
+                "default": 0,
+                "type": "int"
+            }
         }
     },
-    "primitives": [
-        "mlblocks.MLPipeline",
-        "featuretools.dfs",
-        "mlprimitives.custom.feature_extraction.CategoricalEncoder",
-        "xgboost.XGBClassifier"
-    ]
+    "modalities": [],
+    "name": "numpy.take",
+    "primitive": "numpy.take",
+    "produce": {
+        "args": [
+            {
+                "keyword": "a",
+                "name": "y",
+                "type": "ndarray"
+            }
+        ],
+        "output": [
+            {
+                "name": "y",
+                "type": "ndarray"
+            }
+        ]
+    }
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm.json` & `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9194444444444444%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', 'cutoff_time'), "*

 * *                  "('time_index', 'timestamp')]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1']}",*

 * * "'input_names'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('timeseries', 'readings')]), delete: "*

 * *               […]*

```diff
@@ -1,14 +1,14 @@
 {
     "init_params": {
         "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
             "epochs": 35,
             "verbose": false
         },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "pandas.DataFrame#1": {
             "columns": null,
             "index": null
@@ -29,15 +29,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
@@ -81,11 +81,11 @@
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
         "keras.Sequential.DoubleLSTMTimeSeriesClassifier"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_prob.json` & `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9244949494949495%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', 'cutoff_time'), "*

 * *                  "('time_index', 'timestamp')]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1']}",*

 * * "'input_names'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('timeseries', 'readings')]), delete: "*

 * *               […]*

```diff
@@ -2,15 +2,15 @@
     "init_params": {
         "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
             "classification": false,
             "epochs": 35,
             "loss": "keras.losses.binary_crossentropy",
             "verbose": false
         },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "numpy.take#1": {
             "axis": 1,
             "indices": 1
@@ -35,15 +35,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
@@ -87,12 +87,12 @@
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
         "keras.Sequential.DoubleLSTMTimeSeriesClassifier",
         "numpy.take"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json` & `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8623397435897436%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', 'cutoff_time'), "*

 * *                  "('time_index', 'timestamp')]), 'keras.Sequential.LSTMTimeSeriesClassifier#1': "*

 * *                  "OrderedDict([('epochs', 35), ('verbose', False), ('classification', False), "*

 * *                  "('loss', 'keras.losses.binary_crossentropy')]), delete: "*

 * *                  "['mlblocks.MLPipeline#1', "*

 * *               […]*

```diff
@@ -1,27 +1,16 @@
 {
     "init_params": {
-        "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
+        "keras.Sequential.LSTMTimeSeriesClassifier#1": {
             "classification": false,
             "epochs": 35,
             "loss": "keras.losses.binary_crossentropy",
             "verbose": false
         },
-        "mlblocks.MLPipeline#1": {
-            "input_names": {
-                "pandas.DataFrame.resample#1": {
-                    "X": "df"
-                },
-                "pandas.DataFrame.unstack#1": {
-                    "X": "readings"
-                }
-            },
-            "pipeline": "unstack"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "numpy.take#1": {
             "axis": 1,
             "indices": 1
@@ -46,18 +35,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "X": "readings"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
@@ -94,20 +80,19 @@
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
-        "mlblocks.MLPipeline",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
-        "keras.Sequential.DoubleLSTMTimeSeriesClassifier",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "keras.Sequential.LSTMTimeSeriesClassifier",
         "numpy.take"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/double_lstm/double_lstm_with_unstack.json` & `draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8535984848484849%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', 'cutoff_time'), "*

 * *                  "('time_index', 'timestamp')]), 'keras.Sequential.LSTMTimeSeriesRegressor#1': "*

 * *                  "OrderedDict([('epochs', 35), ('verbose', False)]), delete: "*

 * *                  "['mlblocks.MLPipeline#1', "*

 * *                  "'mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1', "*

 * *               […]*

```diff
@@ -1,25 +1,14 @@
 {
     "init_params": {
-        "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
+        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "epochs": 35,
             "verbose": false
         },
-        "mlblocks.MLPipeline#1": {
-            "input_names": {
-                "pandas.DataFrame.resample#1": {
-                    "X": "df"
-                },
-                "pandas.DataFrame.unstack#1": {
-                    "X": "readings"
-                }
-            },
-            "pipeline": "unstack"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "pandas.DataFrame#1": {
             "columns": null,
             "index": null
@@ -40,18 +29,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "X": "readings"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
@@ -88,19 +74,18 @@
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
-        "mlblocks.MLPipeline",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
-        "keras.Sequential.DoubleLSTMTimeSeriesClassifier"
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "keras.Sequential.LSTMTimeSeriesRegressor"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/lstm/lstm.json` & `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9194444444444444%*

 * *Differences: {"'init_params'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', 'cutoff_time'), "*

 * *                  "('time_index', 'timestamp')]), delete: "*

 * *                  "['mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1']}",*

 * * "'input_names'": "{'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('timeseries', 'readings')]), delete: "*

 * *               […]*

```diff
@@ -1,14 +1,14 @@
 {
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesClassifier#1": {
             "epochs": 35,
             "verbose": false
         },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "pandas.DataFrame#1": {
             "columns": null,
             "index": null
@@ -29,15 +29,15 @@
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
@@ -81,11 +81,11 @@
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
         "keras.Sequential.LSTMTimeSeriesClassifier"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/lstm/lstm_prob.json` & `draco-ml-0.2.1.dev0/draco/pipelines/lstm/lstm_prob_with_unstack.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8387029637029636%*

 * *Differences: {"'init_params'": "{'pandas.DataFrame.resample#1': OrderedDict([('rule', '3600s'), ('on', "*

 * *                  "'timestamp'), ('groupby', ['turbine_id', 'signal_id']), ('aggregation', "*

 * *                  "'mean'), ('reset_index', False)]), 'pandas.DataFrame.unstack#1': "*

 * *                  "OrderedDict([('level', 'signal_id'), ('reset_index', True)]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', […]*

```diff
@@ -2,15 +2,15 @@
     "init_params": {
         "keras.Sequential.LSTMTimeSeriesClassifier#1": {
             "classification": false,
             "epochs": 35,
             "loss": "keras.losses.binary_crossentropy",
             "verbose": false
         },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "numpy.take#1": {
             "axis": 1,
             "indices": 1
@@ -21,48 +21,68 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "aggregation": "mean",
+            "groupby": [
+                "turbine_id",
+                "signal_id"
+            ],
+            "on": "timestamp",
+            "reset_index": false,
+            "rule": "3600s"
+        },
         "pandas.DataFrame.set#1": {
             "key": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "key": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "level": "signal_id",
+            "reset_index": true
+        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#2": {
             "X": "readings"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
         "pandas.DataFrame.set#1": {
             "X": "readings",
             "value": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "X": "readings",
             "value": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
@@ -72,27 +92,35 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
+        "pandas.DataFrame.resample",
+        "pandas.DataFrame.unstack",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
         "keras.Sequential.LSTMTimeSeriesClassifier",
         "numpy.take"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/lstm/lstm_prob_with_unstack.json` & `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7913690476190477%*

 * *Differences: {"'init_params'": "{'pandas.DataFrame.resample#1': OrderedDict([('rule', '3600s'), ('on', "*

 * *                  "'timestamp'), ('groupby', ['turbine_id', 'signal_id']), ('aggregation', "*

 * *                  "'mean'), ('reset_index', False)]), 'pandas.DataFrame.unstack#1': "*

 * *                  "OrderedDict([('level', 'signal_id'), ('reset_index', True)]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', […]*

```diff
@@ -1,27 +1,16 @@
 {
     "init_params": {
-        "keras.Sequential.LSTMTimeSeriesClassifier#1": {
+        "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
             "classification": false,
             "epochs": 35,
             "loss": "keras.losses.binary_crossentropy",
             "verbose": false
         },
-        "mlblocks.MLPipeline#1": {
-            "input_names": {
-                "pandas.DataFrame.resample#1": {
-                    "X": "df"
-                },
-                "pandas.DataFrame.unstack#1": {
-                    "X": "readings"
-                }
-            },
-            "pipeline": "unstack"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "numpy.take#1": {
             "axis": 1,
             "indices": 1
@@ -32,51 +21,68 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "aggregation": "mean",
+            "groupby": [
+                "turbine_id",
+                "signal_id"
+            ],
+            "on": "timestamp",
+            "reset_index": false,
+            "rule": "3600s"
+        },
         "pandas.DataFrame.set#1": {
             "key": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "key": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "level": "signal_id",
+            "reset_index": true
+        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "X": "readings"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#2": {
             "X": "readings"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
         "pandas.DataFrame.set#1": {
             "X": "readings",
             "value": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "X": "readings",
             "value": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
@@ -86,28 +92,35 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
-        "mlblocks.MLPipeline",
+        "pandas.DataFrame.resample",
+        "pandas.DataFrame.unstack",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
-        "keras.Sequential.LSTMTimeSeriesClassifier",
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "keras.Sequential.DoubleLSTMTimeSeriesClassifier",
         "numpy.take"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/lstm/lstm_with_unstack.json` & `draco-ml-0.2.1.dev0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7823946886446888%*

 * *Differences: {"'init_params'": "{'pandas.DataFrame.resample#1': OrderedDict([('rule', '600s'), ('on', "*

 * *                  "'timestamp'), ('groupby', ['turbine_id', 'signal_id']), ('aggregation', "*

 * *                  "'mean'), ('reset_index', False)]), 'pandas.DataFrame.unstack#1': "*

 * *                  "OrderedDict([('level', 'signal_id'), ('reset_index', True)]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time',  […]*

```diff
@@ -1,76 +1,82 @@
 {
     "init_params": {
-        "keras.Sequential.LSTMTimeSeriesClassifier#1": {
+        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
             "epochs": 35,
-            "verbose": false
+            "verbose": true
         },
-        "mlblocks.MLPipeline#1": {
-            "input_names": {
-                "pandas.DataFrame.resample#1": {
-                    "X": "df"
-                },
-                "pandas.DataFrame.unstack#1": {
-                    "X": "readings"
-                }
-            },
-            "pipeline": "unstack"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "pandas.DataFrame#1": {
             "columns": null,
             "index": null
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "aggregation": "mean",
+            "groupby": [
+                "turbine_id",
+                "signal_id"
+            ],
+            "on": "timestamp",
+            "reset_index": false,
+            "rule": "600s"
+        },
         "pandas.DataFrame.set#1": {
             "key": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "key": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "level": "signal_id",
+            "reset_index": true
+        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "X": "readings"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#2": {
             "X": "readings"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
         "pandas.DataFrame.set#1": {
             "X": "readings",
             "value": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "X": "readings",
             "value": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
@@ -80,27 +86,34 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
-        "mlblocks.MLPipeline",
+        "pandas.DataFrame.resample",
+        "pandas.DataFrame.unstack",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
-        "keras.Sequential.LSTMTimeSeriesClassifier"
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "keras.Sequential.LSTMTimeSeriesRegressor"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json` & `draco-ml-0.2.1.dev0/draco/pipelines/double_lstm/double_lstm_with_unstack.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7823946886446888%*

 * *Differences: {"'init_params'": "{'pandas.DataFrame.resample#1': OrderedDict([('rule', '3600s'), ('on', "*

 * *                  "'timestamp'), ('groupby', ['turbine_id', 'signal_id']), ('aggregation', "*

 * *                  "'mean'), ('reset_index', False)]), 'pandas.DataFrame.unstack#1': "*

 * *                  "OrderedDict([('level', 'signal_id'), ('reset_index', True)]), "*

 * *                  "'mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1': "*

 * *                  "OrderedDict([('window_size', 24), ('cutoff_time', […]*

```diff
@@ -1,76 +1,82 @@
 {
     "init_params": {
-        "keras.Sequential.LSTMTimeSeriesRegressor#1": {
+        "keras.Sequential.DoubleLSTMTimeSeriesClassifier#1": {
             "epochs": 35,
             "verbose": false
         },
-        "mlblocks.MLPipeline#1": {
-            "input_names": {
-                "pandas.DataFrame.resample#1": {
-                    "X": "df"
-                },
-                "pandas.DataFrame.unstack#1": {
-                    "X": "readings"
-                }
-            },
-            "pipeline": "unstack"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "cutoff_time": "cutoff_time",
             "time_index": "timestamp",
             "window_size": 24
         },
         "pandas.DataFrame#1": {
             "columns": null,
             "index": null
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "aggregation": "mean",
+            "groupby": [
+                "turbine_id",
+                "signal_id"
+            ],
+            "on": "timestamp",
+            "reset_index": false,
+            "rule": "3600s"
+        },
         "pandas.DataFrame.set#1": {
             "key": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "key": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "level": "signal_id",
+            "reset_index": true
+        },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "feature_range": [
                 -1,
                 1
             ]
         }
     },
     "input_names": {
-        "mlblocks.MLPipeline#1": {
-            "X": "readings"
-        },
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences#1": {
             "timeseries": "readings"
         },
         "pandas.DataFrame#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#1": {
             "X": "readings"
         },
         "pandas.DataFrame.pop#2": {
             "X": "readings"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
         "pandas.DataFrame.set#1": {
             "X": "readings",
             "value": "turbine_id"
         },
         "pandas.DataFrame.set#2": {
             "X": "readings",
             "value": "timestamp"
         },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
@@ -80,27 +86,34 @@
         },
         "pandas.DataFrame.pop#1": {
             "item": "turbine_id"
         },
         "pandas.DataFrame.pop#2": {
             "item": "timestamp"
         },
+        "pandas.DataFrame.resample#1": {
+            "X": "readings"
+        },
+        "pandas.DataFrame.unstack#1": {
+            "X": "readings"
+        },
         "sklearn.impute.SimpleImputer#1": {
             "X": "readings"
         },
         "sklearn.preprocessing.MinMaxScaler#1": {
             "X": "readings"
         }
     },
     "primitives": [
-        "mlblocks.MLPipeline",
+        "pandas.DataFrame.resample",
+        "pandas.DataFrame.unstack",
         "pandas.DataFrame.pop",
         "pandas.DataFrame.pop",
         "sklearn.impute.SimpleImputer",
         "sklearn.preprocessing.MinMaxScaler",
         "pandas.DataFrame",
         "pandas.DataFrame.set",
         "pandas.DataFrame.set",
-        "mlprimitives.custom.timeseries_preprocessing.cutoff_window_sequences",
-        "keras.Sequential.LSTMTimeSeriesRegressor"
+        "mlstars.custom.timeseries_preprocessing.cutoff_window_sequences",
+        "keras.Sequential.DoubleLSTMTimeSeriesClassifier"
     ]
 }
```

### Comparing `draco-ml-0.2.0/draco/primitives/mlblocks.MLPipeline.json` & `draco-ml-0.2.1.dev0/draco/primitives/mlblocks.MLPipeline.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/primitives/xgboost.XGBClassifier:probabilities.json` & `draco-ml-0.2.1.dev0/draco/primitives/xgboost.XGBClassifier:probabilities.json`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/results.py` & `draco-ml-0.2.1.dev0/draco/results.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/targets.py` & `draco-ml-0.2.1.dev0/draco/targets.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco/utils.py` & `draco-ml-0.2.1.dev0/draco/utils.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/draco_ml.egg-info/PKG-INFO` & `draco-ml-0.2.1.dev0/draco_ml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: draco-ml
-Version: 0.2.0
-Summary: AutoML for Renewable Energy Industries.
+Version: 0.2.1.dev0
+Summary: AutoML for Time Series.
 Home-page: https://github.com/sintel-dev/Draco
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: wind machine learning draco
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -29,15 +28,15 @@
 </p>
 
 <p align="left">
 <img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2019/03/GreenGuard.png" alt="Draco" />
 </p>
 
 <p align="left">
-AutoML for Renewable Energy Industries.
+AutoML for Time Series.
 </p>
 
 
 [![PyPI Shield](https://img.shields.io/pypi/v/draco-ml.svg)](https://pypi.python.org/pypi/draco-ml)
 [![Tests](https://github.com/sintel-dev/Draco/workflows/Run%20Tests/badge.svg)](https://github.com/sintel-dev/Draco/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
 [![Downloads](https://pepy.tech/badge/draco-ml)](https://pepy.tech/project/draco-ml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sintel-dev/Draco/master?filepath=tutorials)
@@ -50,15 +49,15 @@
 - License: [MIT](https://github.com/sintel-dev/Draco/blob/master/LICENSE)
 - Documentation: https://sintel-dev.github.io/Draco
 - Homepage: https://github.com/sintel-dev/Draco
 
 ## Overview
 
 The Draco project is a collection of end-to-end solutions for machine learning problems
-commonly found in monitoring wind energy production systems. Most tasks utilize sensor data
+commonly found in time series monitoring systems. Most tasks utilize sensor data
 emanating from monitoring systems. We utilize the foundational innovations developed for
 automation of machine Learning at Data to AI Lab at MIT.
 
 The salient aspects of this customized project are:
 
 * A set of ready to use, well tested pipelines for different machine learning tasks. These are
   vetted through testing across multiple publicly available datasets for the same task.
@@ -241,26 +240,25 @@
 pipelines = get_pipelines()
 ```
 
 The returned `pipeline` variable will be `list` containing the names of all the pipelines
 available in the Draco system:
 
 ```
-['dfs_xgb',
- 'dfs_xgb_with_unstack',
- 'dfs_xgb_with_normalization',
- 'dfs_xgb_with_unstack_normalization',
- 'dfs_xgb_prob_with_unstack_normalization']
+['lstm',
+ 'lstm_with_unstack',
+ 'double_lstm',
+ 'double_lstm_with_unstack']
 ```
 
 For the rest of this tutorial, we will select and use the pipeline
-`dfs_xgb_with_unstack_normalization` as our template.
+`lstm_with_unstack` as our template.
 
 ```python3
-pipeline_name = 'dfs_xgb_with_unstack_normalization'
+pipeline_name = 'lstm_with_unstack'
 ```
 
 ## 3. Fitting the Pipeline
 
 Once we have loaded the data and selected the pipeline that we will use, we have to
 fit it.
 
@@ -412,9 +410,7 @@
 * initial collection of dfs and lstm based pipelines
 * optimized pipeline tuning
 * documentation and tutorials
 
 ### 0.1.0
 
 * First release on PyPI
-
-
```

### Comparing `draco-ml-0.2.0/draco_ml.egg-info/SOURCES.txt` & `draco-ml-0.2.1.dev0/draco_ml.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -27,37 +27,25 @@
 draco/metrics.py
 draco/pipeline.py
 draco/results.py
 draco/targets.py
 draco/utils.py
 draco/loaders/__init__.py
 draco/loaders/csv.py
-draco/pipelines/dfs_xgb/dfs_xgb.json
-draco/pipelines/dfs_xgb/dfs_xgb_prob_with_double_normalization.json
-draco/pipelines/dfs_xgb/dfs_xgb_prob_with_unstack.json
-draco/pipelines/dfs_xgb/dfs_xgb_prob_with_unstack_normalization.json
-draco/pipelines/dfs_xgb/dfs_xgb_with_double_normalization.json
-draco/pipelines/dfs_xgb/dfs_xgb_with_normalization.json
-draco/pipelines/dfs_xgb/dfs_xgb_with_unstack.json
-draco/pipelines/dfs_xgb/dfs_xgb_with_unstack_normalization.json
 draco/pipelines/double_lstm/double_lstm.json
 draco/pipelines/double_lstm/double_lstm_prob.json
 draco/pipelines/double_lstm/double_lstm_prob_with_unstack.json
 draco/pipelines/double_lstm/double_lstm_with_unstack.json
 draco/pipelines/dummy/dummy.json
 draco/pipelines/lstm/lstm.json
 draco/pipelines/lstm/lstm_prob.json
 draco/pipelines/lstm/lstm_prob_with_unstack.json
 draco/pipelines/lstm/lstm_with_unstack.json
 draco/pipelines/lstm_regressor/lstm_regressor.json
 draco/pipelines/lstm_regressor/lstm_regressor_with_unstack.json
-draco/pipelines/preprocessing/double_entity_normalization.json
-draco/pipelines/preprocessing/entity_dataframe.json
-draco/pipelines/preprocessing/entity_normalization.json
-draco/pipelines/preprocessing/unstack.json
 draco/primitives/mlblocks.MLPipeline.json
 draco/primitives/numpy.take.json
 draco/primitives/xgboost.XGBClassifier:probabilities.json
 draco_ml.egg-info/PKG-INFO
 draco_ml.egg-info/SOURCES.txt
 draco_ml.egg-info/dependency_links.txt
 draco_ml.egg-info/entry_points.txt
```

### Comparing `draco-ml-0.2.0/draco_ml.egg-info/requires.txt` & `draco-ml-0.2.1.dev0/draco_ml.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 baytune<0.5,>=0.4.0
-mlprimitives<0.4,>=0.3.2
+ml-stars>=0.1.0
 mlblocks<0.5,>=0.4.0
 pymongo<4,>=3.7.2
-scikit-learn>=0.21
+scikit-learn<1.2,>=0.21
 tqdm<4.50.0,>=4.36.1
 scipy<2,>=1.0.1
-numpy<1.21.0,>=1.16.0
+numpy<1.19,>=1.16.0
 pandas<2,>=1
 tensorflow<2.3,>=2
 partd<2,>=1.1.0
 fsspec<0.9,>=0.8.5
 dask<3,>=2.6.0
 tabulate<0.9,>=0.8.3
-xlsxwriter>=1.3.6<1.4
+xlsxwriter<1.4,>=1.3.6
+protobuf<4
+importlib-metadata<5
 
 [dev]
 bumpversion<0.6,>=0.5.3
 pip>=9.0.1
 watchdog<0.11,>=0.8.3
 m2r<0.3,>=0.2.0
 nbsphinx<0.7,>=0.5.0
@@ -26,19 +28,19 @@
 autodocsumm>=0.1.10
 markupsafe<2.1.0
 Jinja2<3,>=2
 flake8<4,>=3.7.7
 isort<5,>=4.3.4
 autoflake<2,>=1.1
 autopep8<2,>=1.4.3
+importlib-metadata<5
 twine<4,>=1.10.0
 wheel>=0.30.0
 coverage<6,>=4.5.1
 tox<4,>=2.9.1
-importlib-metadata<2,>=0.12
 pytest>=3.4.2
 pytest-cov>=2.6.0
 jupyter<2,>=1.0.0
 rundoc<0.5,>=0.4.3
 
 [test]
 pytest>=3.4.2
```

### Comparing `draco-ml-0.2.0/setup.cfg` & `draco-ml-0.2.1.dev0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `draco-ml-0.2.0/setup.py` & `draco-ml-0.2.1.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,31 @@
     with open('HISTORY.md', encoding='utf-8') as history_file:
         history = history_file.read()
 except IOError:
     history = ''
 
 install_requires = [
     'baytune>=0.4.0,<0.5',
-    'mlprimitives>=0.3.2,<0.4',
+    'ml-stars>=0.1.0',
     'mlblocks>=0.4.0,<0.5',
     'pymongo>=3.7.2,<4',
-    'scikit-learn>=0.21',
+    'scikit-learn>=0.21,<1.2',
     'tqdm<4.50.0,>=4.36.1',
     'scipy>=1.0.1,<2',
-    'numpy>=1.16.0,<1.21.0',
+    'numpy>=1.16.0,<1.19',
     'pandas>=1,<2',
     'tensorflow>=2,<2.3',
     'partd>=1.1.0,<2',
     'fsspec>=0.8.5,<0.9',
     'dask>=2.6.0,<3',
     'tabulate>=0.8.3,<0.9',
-    'xlsxwriter>=1.3.6<1.4',
+    'xlsxwriter>=1.3.6,<1.4',
+    # fix conflicts
+    'protobuf<4',
+    'importlib-metadata<5',
 ]
 
 setup_requires = [
     'pytest-runner>=2.11.1',
 ]
 
 tests_require = [
@@ -63,23 +66,23 @@
     # style check
     'flake8>=3.7.7,<4',
     'isort>=4.3.4,<5',
 
     # fix style issues
     'autoflake>=1.1,<2',
     'autopep8>=1.4.3,<2',
+    'importlib-metadata<5',
 
     # distribute on PyPI
     'twine>=1.10.0,<4',
     'wheel>=0.30.0',
 
     # Advanced testing
     'coverage>=4.5.1,<6',
     'tox>=2.9.1,<4',
-    'importlib-metadata<2,>=0.12',
 ]
 
 setup(
     author='MIT Data To AI Lab',
     author_email='dailabmit@gmail.com',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -87,15 +90,15 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description='AutoML for Renewable Energy Industries.',
+    description='AutoML for Time Series.',
     entry_points={
         'mlblocks': [
             'pipelines=draco:MLBLOCKS_PIPELINES',
             'primitives=draco:MLBLOCKS_PRIMITIVES'
         ],
     },
     extras_require={
@@ -111,10 +114,10 @@
     name='draco-ml',
     packages=find_packages(include=['draco', 'draco.*']),
     python_requires='>=3.6,<3.9',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/Draco',
-    version='0.2.0',
+    version='0.2.1.dev0',
     zip_safe=False,
 )
```

### Comparing `draco-ml-0.2.0/tests/test_benchmark.py` & `draco-ml-0.2.1.dev0/tests/test_benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from draco.benchmark import evaluate_templates
 from draco.demo import load_demo
 
 
 def test_predict():
     # setup
     templates = [
-        'dfs_xgb_prob_with_unstack_normalization'
+        'lstm_with_unstack'
     ]
 
     window_size_rule = [
         ('1d', '1h')
     ]
 
     target_times, readings = load_demo()
```

### Comparing `draco-ml-0.2.0/tests/test_metrics.py` & `draco-ml-0.2.1.dev0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `draco-ml-0.2.0/tests/test_pipeline.py` & `draco-ml-0.2.1.dev0/tests/test_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """Tests for `draco.pipeline` module."""
 from unittest import TestCase
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
+from mlblocks import MLPipeline
 
 from draco.pipeline import DracoPipeline, get_pipelines
 
 
 def test_get_pipelines():
     output = get_pipelines()
     assert isinstance(output, list)
@@ -24,14 +25,21 @@
 
 
 def test_get_pipelines_type_error():
     with pytest.raises(FileNotFoundError):
         get_pipelines(pipeline_type='does-not-exist')
 
 
+def test_loading_pipelines():
+    draco_pipelines = get_pipelines()
+    for pipeline in draco_pipelines:
+        mlpipeline = MLPipeline(pipeline)
+        assert isinstance(mlpipeline, MLPipeline)
+
+
 class TestDracoPipeline(TestCase):
 
     def _get_data(self):
         target_times = pd.DataFrame({
             'turbine_id': ['T001'],
             'cutoff_time': [pd.Timestamp('2010-01-01')],
             'target': [1]
```

