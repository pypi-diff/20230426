# Comparing `tmp/veta-0.7.4.tar.gz` & `tmp/veta-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veta-0.7.4.tar", last modified: Wed Feb  8 17:09:41 2023, max compression
+gzip compressed data, was "veta-0.7.5.tar", last modified: Wed Apr 26 18:07:21 2023, max compression
```

## Comparing `veta-0.7.4.tar` & `veta-0.7.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.698674 veta-0.7.4/
--rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.4/.gitignore
--rw-r--r--   0 pbarbosa   (503) staff       (20)      600 2023-01-13 02:44:49.000000 veta-0.7.4/Dockerfile
--rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.4/LICENSE
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-02-08 17:09:41.698158 veta-0.7.4/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34853 2022-12-29 20:23:55.000000 veta-0.7.4/README.md
--rw-r--r--   0 pbarbosa   (503) staff       (20)      484 2022-12-30 18:52:40.000000 veta-0.7.4/conda_environment.yml
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-02-08 17:08:39.000000 veta-0.7.4/pyproject.toml
--rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-02-08 17:09:41.698783 veta-0.7.4/setup.cfg
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.628853 veta-0.7.4/src/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.4/src/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    24705 2023-01-13 02:22:43.000000 veta-0.7.4/src/base.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22309 2023-01-13 02:18:40.000000 veta-0.7.4/src/benchmark.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.630208 veta-0.7.4/src/config/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.4/src/config/__init__.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.668954 veta-0.7.4/src/config/example_imgs/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/.gitkeep
--rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/benchmark_af.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/benchmark_dist.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.4/src/config/example_imgs/benchmark_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.4/src/config/example_imgs/benchmark_thresholds.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/heatmap.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/inspect_ratios.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.4/src/config/example_imgs/inspect_ratios2.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/logo.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/ml_fi.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/ml_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/pearson_corr.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.4/src/config/example_imgs/per_bin_score.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.4/src/config/example_imgs/per_bin_score_split_ss.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.4/src/config/example_imgs/roc_analysis.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.4/src/config/example_imgs/roc_curves.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1356 2022-12-29 18:11:14.000000 veta-0.7.4/src/config/tools_config.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)    14414 2022-12-29 18:11:14.000000 veta-0.7.4/src/interrogate.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.676932 veta-0.7.4/src/plots/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.4/src/plots/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    23298 2023-02-08 17:08:39.000000 veta-0.7.4/src/plots/plots_benchmark_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     8780 2022-12-29 18:52:15.000000 veta-0.7.4/src/plots/plots_interrogate_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15452 2023-02-08 17:08:39.000000 veta-0.7.4/src/plots/plots_intronic_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.4/src/plots/plots_machine_learning.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.4/src/plots/plots_threshold_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.4/src/plots/plots_utils.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.686341 veta-0.7.4/src/predictions/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.4/src/predictions/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2022-07-06 23:37:56.000000 veta-0.7.4/src/predictions/apply.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     9437 2022-12-29 18:11:14.000000 veta-0.7.4/src/predictions/filters.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    16825 2022-12-30 18:52:40.000000 veta-0.7.4/src/predictions/introns.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    21103 2022-12-29 18:11:14.000000 veta-0.7.4/src/predictions/metapredictions.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2022-08-25 13:25:47.000000 veta-0.7.4/src/predictions/metrics.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2022-12-29 18:11:14.000000 veta-0.7.4/src/predictions/thresholds.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.4/src/predictions/utils_classifiers.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.693485 veta-0.7.4/src/preprocessing/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.4/src/preprocessing/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.4/src/preprocessing/clinvar.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2022-10-07 22:13:57.000000 veta-0.7.4/src/preprocessing/location.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.4/src/preprocessing/osutils.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.4/src/preprocessing/tables.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22626 2022-12-29 18:11:14.000000 veta-0.7.4/src/preprocessing/utils_tools.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.4/src/preprocessing/vcf.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-02-08 17:09:41.696967 veta-0.7.4/src/veta.egg-info/
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/SOURCES.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/dependency_links.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/entry_points.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/requires.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-02-08 17:09:41.000000 veta-0.7.4/src/veta.egg-info/top_level.txt
--rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.4/src/veta.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.579820 veta-0.7.5/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.5/.gitignore
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      600 2023-01-13 02:44:49.000000 veta-0.7.5/Dockerfile
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.5/LICENSE
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-04-26 18:07:21.578540 veta-0.7.5/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    34853 2022-12-29 20:23:55.000000 veta-0.7.5/README.md
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      484 2022-12-30 18:52:40.000000 veta-0.7.5/conda_environment.yml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-04-26 18:03:35.000000 veta-0.7.5/pyproject.toml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-04-26 18:07:21.579936 veta-0.7.5/setup.cfg
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.514575 veta-0.7.5/src/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.5/src/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    24705 2023-01-13 02:22:43.000000 veta-0.7.5/src/base.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22309 2023-01-13 02:18:40.000000 veta-0.7.5/src/benchmark.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.515547 veta-0.7.5/src/config/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.5/src/config/__init__.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.551976 veta-0.7.5/src/config/example_imgs/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/.gitkeep
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/benchmark_af.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/benchmark_dist.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.5/src/config/example_imgs/benchmark_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.5/src/config/example_imgs/benchmark_thresholds.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/heatmap.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/inspect_ratios.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.5/src/config/example_imgs/inspect_ratios2.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/logo.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/ml_fi.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/ml_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/pearson_corr.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.5/src/config/example_imgs/per_bin_score.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.5/src/config/example_imgs/per_bin_score_split_ss.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.5/src/config/example_imgs/roc_analysis.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.5/src/config/example_imgs/roc_curves.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1352 2023-04-26 18:03:35.000000 veta-0.7.5/src/config/tools_config.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    14414 2022-12-29 18:11:14.000000 veta-0.7.5/src/interrogate.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.562353 veta-0.7.5/src/plots/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.5/src/plots/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    23298 2023-02-08 17:08:39.000000 veta-0.7.5/src/plots/plots_benchmark_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     8780 2022-12-29 18:52:15.000000 veta-0.7.5/src/plots/plots_interrogate_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15452 2023-02-08 17:08:39.000000 veta-0.7.5/src/plots/plots_intronic_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.5/src/plots/plots_machine_learning.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.5/src/plots/plots_threshold_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.5/src/plots/plots_utils.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.568582 veta-0.7.5/src/predictions/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.5/src/predictions/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2022-07-06 23:37:56.000000 veta-0.7.5/src/predictions/apply.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     9437 2022-12-29 18:11:14.000000 veta-0.7.5/src/predictions/filters.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    16825 2022-12-30 18:52:40.000000 veta-0.7.5/src/predictions/introns.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    21103 2022-12-29 18:11:14.000000 veta-0.7.5/src/predictions/metapredictions.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2022-08-25 13:25:47.000000 veta-0.7.5/src/predictions/metrics.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2022-12-29 18:11:14.000000 veta-0.7.5/src/predictions/thresholds.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.5/src/predictions/utils_classifiers.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.574597 veta-0.7.5/src/preprocessing/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.5/src/preprocessing/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.5/src/preprocessing/clinvar.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2022-10-07 22:13:57.000000 veta-0.7.5/src/preprocessing/location.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.5/src/preprocessing/osutils.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.5/src/preprocessing/tables.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22626 2022-12-29 18:11:14.000000 veta-0.7.5/src/preprocessing/utils_tools.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.5/src/preprocessing/vcf.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-26 18:07:21.577853 veta-0.7.5/src/veta.egg-info/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/SOURCES.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/dependency_links.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/entry_points.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/requires.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-04-26 18:07:21.000000 veta-0.7.5/src/veta.egg-info/top_level.txt
+-rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.5/src/veta.py
```

### Comparing `veta-0.7.4/Dockerfile` & `veta-0.7.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/LICENSE` & `veta-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/PKG-INFO` & `veta-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.4
+Version: 0.7.5
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
```

### Comparing `veta-0.7.4/README.md` & `veta-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/pyproject.toml` & `veta-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "veta"
 description = "Simple variant prediction evaluation"
 authors = [
     {name = "Pedro Barbosa", email = "psbpedrobarbosa@gmail.com"},
 ]
 
-version = "0.7.4"
+version = "0.7.5"
 readme = "README.md"
 requires-python = "~=3.8"
 dependencies = [
     "matplotlib==3.5.1",
     "numpy==1.23.5",
     "pandas==1.4.2",
     "seaborn==0.11.2",
```

### Comparing `veta-0.7.4/src/base.py` & `veta-0.7.5/src/base.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/benchmark.py` & `veta-0.7.5/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/benchmark_af.png` & `veta-0.7.5/src/config/example_imgs/benchmark_af.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/benchmark_dist.png` & `veta-0.7.5/src/config/example_imgs/benchmark_dist.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/benchmark_performance.png` & `veta-0.7.5/src/config/example_imgs/benchmark_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/benchmark_thresholds.png` & `veta-0.7.5/src/config/example_imgs/benchmark_thresholds.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/heatmap.png` & `veta-0.7.5/src/config/example_imgs/heatmap.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/inspect_ratios.png` & `veta-0.7.5/src/config/example_imgs/inspect_ratios.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/inspect_ratios2.png` & `veta-0.7.5/src/config/example_imgs/inspect_ratios2.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/logo.png` & `veta-0.7.5/src/config/example_imgs/logo.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/ml_fi.png` & `veta-0.7.5/src/config/example_imgs/ml_fi.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/ml_performance.png` & `veta-0.7.5/src/config/example_imgs/ml_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/pearson_corr.png` & `veta-0.7.5/src/config/example_imgs/pearson_corr.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/per_bin_score.png` & `veta-0.7.5/src/config/example_imgs/per_bin_score.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/per_bin_score_split_ss.png` & `veta-0.7.5/src/config/example_imgs/per_bin_score_split_ss.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/roc_analysis.png` & `veta-0.7.5/src/config/example_imgs/roc_analysis.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/example_imgs/roc_curves.png` & `veta-0.7.5/src/config/example_imgs/roc_curves.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/config/tools_config.txt` & `veta-0.7.5/src/config/tools_config.txt`

 * *Files 8% similar despite different names*

```diff
@@ -63,9 +63,9 @@
 ConSpliceML	ConSpliceML
 MMSplice	mmsplice_deltaPSI
 kipoiSplice4	kipoisplice_4
 CI-SpliceAI	CI-SpliceAI
 Pangolin	Pangolin
 SPiP	SPiP
 MLCsplice	MLCsplice
-AbSplice-DNA      AbSplice_DNA
-LaBranchoR	labranchoR
+AbSplice-DNA	AbSplice_DNA
+LaBranchoR	labranchoR
```

### Comparing `veta-0.7.4/src/interrogate.py` & `veta-0.7.5/src/interrogate.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_benchmark_mode.py` & `veta-0.7.5/src/plots/plots_benchmark_mode.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_interrogate_mode.py` & `veta-0.7.5/src/plots/plots_interrogate_mode.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_intronic_analysis.py` & `veta-0.7.5/src/plots/plots_intronic_analysis.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_machine_learning.py` & `veta-0.7.5/src/plots/plots_machine_learning.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_threshold_analysis.py` & `veta-0.7.5/src/plots/plots_threshold_analysis.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/plots/plots_utils.py` & `veta-0.7.5/src/plots/plots_utils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/apply.py` & `veta-0.7.5/src/predictions/apply.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/filters.py` & `veta-0.7.5/src/predictions/filters.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/introns.py` & `veta-0.7.5/src/predictions/introns.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/metapredictions.py` & `veta-0.7.5/src/predictions/metapredictions.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/metrics.py` & `veta-0.7.5/src/predictions/metrics.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/thresholds.py` & `veta-0.7.5/src/predictions/thresholds.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/predictions/utils_classifiers.py` & `veta-0.7.5/src/predictions/utils_classifiers.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/clinvar.py` & `veta-0.7.5/src/preprocessing/clinvar.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/location.py` & `veta-0.7.5/src/preprocessing/location.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/osutils.py` & `veta-0.7.5/src/preprocessing/osutils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/tables.py` & `veta-0.7.5/src/preprocessing/tables.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/utils_tools.py` & `veta-0.7.5/src/preprocessing/utils_tools.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/preprocessing/vcf.py` & `veta-0.7.5/src/preprocessing/vcf.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/veta.egg-info/PKG-INFO` & `veta-0.7.5/src/veta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.4
+Version: 0.7.5
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
```

### Comparing `veta-0.7.4/src/veta.egg-info/SOURCES.txt` & `veta-0.7.5/src/veta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veta-0.7.4/src/veta.py` & `veta-0.7.5/src/veta.py`

 * *Files identical despite different names*

