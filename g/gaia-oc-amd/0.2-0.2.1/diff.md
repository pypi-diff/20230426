# Comparing `tmp/gaia_oc_amd-0.2.tar.gz` & `tmp/gaia_oc_amd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gaia_oc_amd-0.2.tar", last modified: Sun Apr 23 10:29:40 2023, max compression
+gzip compressed data, was "dist/gaia_oc_amd-0.2.1.tar", last modified: Wed Apr 26 16:29:31 2023, max compression
```

## Comparing `gaia_oc_amd-0.2.tar` & `gaia_oc_amd-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1806 2022-12-01 11:23:02.000000 gaia_oc_amd-0.2/.gitignore
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1068 2022-07-06 16:30:37.000000 gaia_oc_amd-0.2/LICENSE
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6382 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/PKG-INFO
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     5218 2023-04-23 09:11:14.000000 gaia_oc_amd-0.2/README.md
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.655057 gaia_oc_amd-0.2/examples/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)  4588424 2023-04-23 09:25:22.000000 gaia_oc_amd-0.2/examples/quick_tutorial.ipynb
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)  8914197 2023-04-23 10:02:23.000000 gaia_oc_amd-0.2/examples/tutorial.ipynb
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.651057 gaia_oc_amd-0.2/gaia_oc_amd/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      324 2022-12-01 20:07:40.000000 gaia_oc_amd-0.2/gaia_oc_amd/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    25142 2023-04-22 15:39:34.000000 gaia_oc_amd-0.2/gaia_oc_amd/build_sets.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.651057 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-30 11:26:29.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8247 2023-04-21 08:26:38.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/diagnostics.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8844 2023-04-22 09:52:52.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/membership_probability.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.651057 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     3160 2022-11-12 10:58:20.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/hyper_parameters
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   161836 2022-11-12 11:59:59.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/model_parameters
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11795 2023-04-22 16:24:44.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/hyper_parameters
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   162537 2023-04-22 21:15:28.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/model_parameters
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    27873 2023-04-21 15:20:30.000000 gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/visualization.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      745 2022-12-02 16:14:46.000000 gaia_oc_amd-0.2/gaia_oc_amd/create_gaia_credentials_file.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1573 2022-11-08 12:39:43.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/LogErrVsMagSpline.csv
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-29 15:24:28.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     5044 2023-04-21 07:57:47.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/candidate_selection.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11288 2023-04-21 11:22:40.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/cluster.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6433 2023-04-22 16:09:51.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/cone_preprocessing.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    17474 2023-04-22 16:13:02.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/datasets.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8687 2023-04-21 08:52:43.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/features.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8434 2023-04-20 20:13:28.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/isochrone_preprocessing.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9228 2023-04-22 15:36:00.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/query.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2737 2023-04-20 19:47:37.000000 gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/source_sets.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4808 2022-12-02 15:51:10.000000 gaia_oc_amd-0.2/gaia_oc_amd/download_startup_data.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    19208 2023-04-23 09:19:57.000000 gaia_oc_amd-0.2/gaia_oc_amd/evaluate_clusters.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11338 2023-04-22 15:42:27.000000 gaia_oc_amd-0.2/gaia_oc_amd/io.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.655057 gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-29 15:39:17.000000 gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    10291 2022-09-24 13:22:46.000000 gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/deepsets_zaheer.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    10302 2023-04-23 08:57:36.000000 gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/training.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12041 2023-04-22 16:19:02.000000 gaia_oc_amd-0.2/gaia_oc_amd/train_deep_sets_model.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      970 2023-04-21 08:26:38.000000 gaia_oc_amd-0.2/gaia_oc_amd/utils.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-23 10:29:40.651057 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6382 2023-04-23 10:29:40.000000 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/PKG-INFO
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2651 2023-04-23 10:29:40.000000 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/SOURCES.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        1 2023-04-23 10:29:40.000000 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/dependency_links.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      156 2023-04-23 10:29:40.000000 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/requires.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       12 2023-04-23 10:29:40.000000 gaia_oc_amd-0.2/gaia_oc_amd.egg-info/top_level.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      155 2023-04-22 10:10:33.000000 gaia_oc_amd-0.2/requirements.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       38 2023-04-23 10:29:40.663057 gaia_oc_amd-0.2/setup.cfg
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1470 2023-04-23 10:29:26.000000 gaia_oc_amd-0.2/setup.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1806 2022-12-01 11:23:02.000000 gaia_oc_amd-0.2.1/.gitignore
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1068 2022-07-06 16:30:37.000000 gaia_oc_amd-0.2.1/LICENSE
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6387 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     5221 2023-04-23 10:38:28.000000 gaia_oc_amd-0.2.1/README.md
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.481644 gaia_oc_amd-0.2.1/examples/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)  4588424 2023-04-23 09:25:22.000000 gaia_oc_amd-0.2.1/examples/quick_tutorial.ipynb
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)  8914197 2023-04-23 10:02:23.000000 gaia_oc_amd-0.2.1/examples/tutorial.ipynb
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.473644 gaia_oc_amd-0.2.1/gaia_oc_amd/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      324 2022-12-01 20:07:40.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    25142 2023-04-22 15:39:34.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/build_sets.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.473644 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-30 11:26:29.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8247 2023-04-21 08:26:38.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/diagnostics.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8844 2023-04-22 09:52:52.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/membership_probability.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.469644 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     3160 2022-11-12 10:58:20.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/hyper_parameters
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   161836 2022-11-12 11:59:59.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/model_parameters
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11795 2023-04-22 16:24:44.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/hyper_parameters
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   162537 2023-04-22 21:15:28.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/model_parameters
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    27895 2023-04-26 15:08:14.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/visualization.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      745 2022-12-02 16:14:46.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/create_gaia_credentials_file.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1573 2022-11-08 12:39:43.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/LogErrVsMagSpline.csv
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-29 15:24:28.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     5044 2023-04-21 07:57:47.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/candidate_selection.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11288 2023-04-21 11:22:40.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/cluster.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6433 2023-04-22 16:09:51.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/cone_preprocessing.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    17474 2023-04-22 16:13:02.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/datasets.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8687 2023-04-21 08:52:43.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/features.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     8434 2023-04-20 20:13:28.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/isochrone_preprocessing.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9228 2023-04-22 15:36:00.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/query.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2737 2023-04-20 19:47:37.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/source_sets.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4808 2022-12-02 15:51:10.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/download_startup_data.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    19208 2023-04-23 09:19:57.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/evaluate_clusters.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11338 2023-04-22 15:42:27.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/io.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.473644 gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2022-06-29 15:39:17.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    10291 2022-09-24 13:22:46.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/deepsets_zaheer.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    10302 2023-04-23 08:57:36.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/training.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12041 2023-04-22 16:19:02.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/train_deep_sets_model.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      970 2023-04-21 08:26:38.000000 gaia_oc_amd-0.2.1/gaia_oc_amd/utils.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-04-26 16:29:31.473644 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     6387 2023-04-26 16:29:31.000000 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2651 2023-04-26 16:29:31.000000 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        1 2023-04-26 16:29:31.000000 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      144 2023-04-26 16:29:31.000000 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/requires.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       12 2023-04-26 16:29:31.000000 gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/top_level.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      143 2023-04-26 16:26:36.000000 gaia_oc_amd-0.2.1/requirements.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       38 2023-04-26 16:29:31.489645 gaia_oc_amd-0.2.1/setup.cfg
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1472 2023-04-26 16:21:38.000000 gaia_oc_amd-0.2.1/setup.py
```

### Comparing `gaia_oc_amd-0.2/.gitignore` & `gaia_oc_amd-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/LICENSE` & `gaia_oc_amd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/PKG-INFO` & `gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: gaia_oc_amd
-Version: 0.2
+Name: gaia-oc-amd
+Version: 0.2.1
 Summary: Machine learning tool for the determination of new members of open clusters using Gaia data.
 Home-page: https://github.com/MGJvanGroeningen/gaia_oc_amd
 Author: Matthijs G. J. van Groeningen
 Author-email: matthijsvangroeningen@gmail.com
 License: UNKNOWN
 Description: # Open Cluster Automatic Membership Determination with Gaia data
-        This repository presents automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
+        This repository presents an automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
         
         The research paper related to this work can be found [here](https://arxiv.org/abs/2303.08474).
         
         ## Python environment setup
         
         This code is available as a PyPI package and can be installed with
```

### Comparing `gaia_oc_amd-0.2/README.md` & `gaia_oc_amd-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Open Cluster Automatic Membership Determination with Gaia data
-This repository presents automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
+This repository presents an automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
 
 The research paper related to this work can be found [here](https://arxiv.org/abs/2303.08474).
 
 ## Python environment setup
 
 This code is available as a PyPI package and can be installed with
```

### Comparing `gaia_oc_amd-0.2/examples/quick_tutorial.ipynb` & `gaia_oc_amd-0.2.1/examples/quick_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/examples/tutorial.ipynb` & `gaia_oc_amd-0.2.1/examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/build_sets.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/build_sets.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/diagnostics.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/diagnostics.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/membership_probability.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/membership_probability.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/hyper_parameters` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/hyper_parameters`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/model_parameters` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v01/model_parameters`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/hyper_parameters` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/hyper_parameters`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/model_parameters` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/pretrained_models/DS10_v02/model_parameters`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/candidate_evaluation/visualization.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/candidate_evaluation/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
             plot_zero_error_boundaries(ax, x, y, cluster)
 
         if source_show_features is not None:
             plot_features(ax, x, y, source_show_features, cluster)
 
         if y == 'phot_g_mean_mag':
             if show_isochrone and cluster is not None and cluster.isochrone is not None:
-                ax.plot(cluster.isochrone[colour], cluster.isochrone['phot_g_mean_mag'],
+                ax.plot(cluster.isochrone[colour].to_numpy(), cluster.isochrone['phot_g_mean_mag'].to_numpy(),
                         label='isochrone', zorder=1)
             ax.invert_yaxis()
             legend_loc = 'best'
         else:
             legend_loc = 'upper left'
 
         ax.set_xlabel(labels[x], fontsize=axis_label_size)
```

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/create_gaia_credentials_file.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/create_gaia_credentials_file.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/LogErrVsMagSpline.csv` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/LogErrVsMagSpline.csv`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/candidate_selection.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/candidate_selection.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/cluster.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/cluster.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/cone_preprocessing.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/cone_preprocessing.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/datasets.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/datasets.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/features.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/features.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/isochrone_preprocessing.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/isochrone_preprocessing.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/query.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/query.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/data_preparation/source_sets.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/data_preparation/source_sets.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/download_startup_data.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/download_startup_data.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/evaluate_clusters.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/evaluate_clusters.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/io.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/io.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/deepsets_zaheer.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/deepsets_zaheer.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/machine_learning/training.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/machine_learning/training.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/train_deep_sets_model.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/train_deep_sets_model.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd/utils.py` & `gaia_oc_amd-0.2.1/gaia_oc_amd/utils.py`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd.egg-info/PKG-INFO` & `gaia_oc_amd-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: gaia-oc-amd
-Version: 0.2
+Name: gaia_oc_amd
+Version: 0.2.1
 Summary: Machine learning tool for the determination of new members of open clusters using Gaia data.
 Home-page: https://github.com/MGJvanGroeningen/gaia_oc_amd
 Author: Matthijs G. J. van Groeningen
 Author-email: matthijsvangroeningen@gmail.com
 License: UNKNOWN
 Description: # Open Cluster Automatic Membership Determination with Gaia data
-        This repository presents automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
+        This repository presents an automatic procedure for determining new members of open clusters. We use a neural network architecture to find additional members of an open cluster based on already established probable members. To train our model, we use astrometric and photometric data of stars obtained with the Gaia space telescope. The repository contains code for downloading and preparing datasets, for training the model and for the visualization of some results. 
         
         The research paper related to this work can be found [here](https://arxiv.org/abs/2303.08474).
         
         ## Python environment setup
         
         This code is available as a PyPI package and can be installed with
```

### Comparing `gaia_oc_amd-0.2/gaia_oc_amd.egg-info/SOURCES.txt` & `gaia_oc_amd-0.2.1/gaia_oc_amd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaia_oc_amd-0.2/setup.py` & `gaia_oc_amd-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(name='gaia_oc_amd',
-      version='0.2',
+      version='0.2.1',
       description='Machine learning tool for the determination of new members of open clusters using Gaia data.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/MGJvanGroeningen/gaia_oc_amd",
       author='Matthijs G. J. van Groeningen',
       author_email='matthijsvangroeningen@gmail.com',
       package_dir={'': './'},
```

