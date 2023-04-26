# Comparing `tmp/PyTrial-0.0.4.tar.gz` & `tmp/PyTrial-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTrial-0.0.4.tar", last modified: Fri Apr 21 19:26:22 2023, max compression
+gzip compressed data, was "dist/PyTrial-0.0.5.tar", last modified: Tue Apr 25 16:40:29 2023, max compression
```

## Comparing `PyTrial-0.0.4.tar` & `PyTrial-0.0.5.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.4/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PKG-INFO
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4711 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      264 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/top_level.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6009 2023-03-06 23:05:32.000000 PyTrial-0.0.4/README.md
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/data/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10898 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/drug_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/patient_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21943 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/site_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/trial_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/vocab_data.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/bert.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/drug.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/icd.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/causal/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/causal/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/confidence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/confidence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/dipole.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/raim.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/retain.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/rnn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/stagenet.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/mlp.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/xgboost.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8666 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5913 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/metrics.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/pgentropy.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/hint.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/mlp.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_structure.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/dataloader.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/module.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/spot.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/xgboost.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/compose.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/deepenroll.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/bm25.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/doc2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/trial2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/whiten_bert.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-04-19 17:00:00.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      136 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/eva.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/knn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-01-27 05:51:39.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/promptehr.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/synteg.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/copula_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/ct_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14680 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/med_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/tvae.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/check.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/mimic_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/parallel.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15561 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/utils/tabular_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-04-21 00:55:39.000000 PyTrial-0.0.4/pytrial/utils/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/trial_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-21 19:26:22.000000 PyTrial-0.0.4/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1186 2023-04-21 19:25:57.000000 PyTrial-0.0.4/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.5/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6746 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PKG-INFO
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6746 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4711 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      264 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/top_level.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6009 2023-03-06 23:05:32.000000 PyTrial-0.0.5/README.md
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-04-25 16:40:15.000000 PyTrial-0.0.5/pytrial/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/data/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10898 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/drug_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/patient_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21943 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/site_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/trial_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/vocab_data.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/bert.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/drug.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/icd.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/causal/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/causal/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/confidence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/confidence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8666 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5913 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/metrics.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/pgentropy.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/hint.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/mlp.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_structure.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/spot.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/xgboost.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/bm25.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-04-19 17:00:00.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      136 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/knn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-01-27 05:51:39.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15310 2023-04-25 16:39:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/med_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/check.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/mimic_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/parallel.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15561 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/utils/tabular_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-04-21 00:55:39.000000 PyTrial-0.0.5/pytrial/utils/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/trial_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-25 16:40:29.000000 PyTrial-0.0.5/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1271 2023-04-25 16:40:09.000000 PyTrial-0.0.5/setup.py
```

### Comparing `PyTrial-0.0.4/LICENSE` & `PyTrial-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/PKG-INFO` & `PyTrial-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
-Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun
+Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h2 align='center'>
     PyTrial
```

### Comparing `PyTrial-0.0.4/PyTrial.egg-info/PKG-INFO` & `PyTrial-0.0.5/PyTrial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
-Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun
+Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h2 align='center'>
     PyTrial
```

### Comparing `PyTrial-0.0.4/PyTrial.egg-info/SOURCES.txt` & `PyTrial-0.0.5/PyTrial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/README.md` & `PyTrial-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/demo_data.py` & `PyTrial-0.0.5/pytrial/data/demo_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/patient_data.py` & `PyTrial-0.0.5/pytrial/data/patient_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/site_data.py` & `PyTrial-0.0.5/pytrial/data/site_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/trial_data.py` & `PyTrial-0.0.5/pytrial/data/trial_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/utils.py` & `PyTrial-0.0.5/pytrial/data/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/data/vocab_data.py` & `PyTrial-0.0.5/pytrial/data/vocab_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/model_utils/bert.py` & `PyTrial-0.0.5/pytrial/model_utils/bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/model_utils/drug.py` & `PyTrial-0.0.5/pytrial/model_utils/drug.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/model_utils/icd.py` & `PyTrial-0.0.5/pytrial/model_utils/icd.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/data.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/losses.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/metrics.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/base.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/dipole.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/raim.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/retain.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/rnn.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/stagenet.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/base.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/mlp.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/transtab.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/xgboost.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/trainer.py` & `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/base.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/data.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/losses.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/metrics.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/pgentropy.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/pgentropy.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/site_selection/trainer.py` & `PyTrial-0.0.5/pytrial/tasks/site_selection/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/base.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/data.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/evaluation.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/hint.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/hint.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/logistic_regression.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/mlp.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_structure.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_structure.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_utils.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/dataloader.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/module.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/utils.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/spot.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/spot.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_outcome/xgboost.py` & `PyTrial-0.0.5/pytrial/tasks/trial_outcome/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/data.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/losses.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/base.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/compose.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/deepenroll.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/trainer.py` & `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/data.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/losses.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/metrics.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/models/base.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/models/doc2vec.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/models/trial2vec.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_search/models/whiten_bert.py` & `PyTrial-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/data.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/losses.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/base.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/eva.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/evaluation.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/knn.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/knn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/promptehr.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/rnn_gan.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/synteg.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/base.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/copula_gan.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/ct_gan.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/evaluation.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/med_gan.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/med_gan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import pdb
 import joblib
+import warnings
 
 import numpy as np
 import pandas as pd
 import torch
 from torch import nn
 from torch.nn import BatchNorm1d, Linear, Module, Sequential
 from torch.nn.functional import cross_entropy, mse_loss, sigmoid
@@ -175,15 +176,15 @@
                 self.output_info.append(
                     (len(v), 'softmax')
                 )
 
     def fit(self, data):
         data_val = data.df.values
         dataset = TensorDataset(torch.from_numpy(data_val.astype('float32')).to(self.device))
-        loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=True, drop_last=True)
+        loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=True, drop_last=False)
         
         self._get_metadata(data)
         
         # data_dim = self.transformer.output_dim
         data_dim = data_val.shape[1]
         encoder = Encoder(data_dim, self.compress_dims, self.embedding_dim).to(self.device)
         self.decoder = Decoder(self.embedding_dim, self.compress_dims, data_dim).to(self.device)
@@ -212,17 +213,31 @@
             list(self.generator.parameters()) + list(self.decoder.parameters()),
             weight_decay=self.l2scale
         )
         optimizerD = Adam(discriminator.parameters(), weight_decay=self.l2scale)
 
         mean = torch.zeros(self.batch_size, self.random_dim, device=self.device)
         std = mean + 1
+        bs_larger_than_n_sample = False
         for i in range(self.epochs):
             n_d = 2
             n_g = 1
+            
+            if len(loader) < n_d:
+                # batch size is larger than all samples
+                # so we have to update discriminator each iteration
+                bs_larger_than_n_sample = True
+                warnings.warn(
+                    f"""
+                    Batch size is larger than all samples.
+                    Discriminator will be updated each iteration instead of each {n_d} iterations.
+                    Consider using a smaller batch size.
+                    """
+                )
+            
             for id_, data in enumerate(loader):
                 real = data[0].to(self.device)
                 noise = torch.normal(mean=mean, std=std)
                 emb = self.generator(noise)
                 fake = self.decoder(emb, self.output_info)
 
                 optimizerD.zero_grad()
@@ -230,15 +245,15 @@
                 y_fake = discriminator(fake)
                 real_loss = -(torch.log(y_real + 1e-4).mean())
                 fake_loss = (torch.log(1.0 - y_fake + 1e-4).mean())
                 loss_d = real_loss - fake_loss
                 loss_d.backward()
                 optimizerD.step()
 
-                if i % n_d == 0:
+                if id_ % n_d == 0 or bs_larger_than_n_sample:
                     for _ in range(n_g):
                         noise = torch.normal(mean=mean, std=std)
                         emb = self.generator(noise)
                         fake = self.decoder(emb, self.output_info)
                         optimizerG.zero_grad()
                         y_fake = discriminator(fake)
                         loss_g = -(torch.log(y_fake + 1e-4).mean())
```

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/tvae.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/tasks/trial_simulation/trainer.py` & `PyTrial-0.0.5/pytrial/tasks/trial_simulation/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/check.py` & `PyTrial-0.0.5/pytrial/utils/check.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/mimic_utils.py` & `PyTrial-0.0.5/pytrial/utils/mimic_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/parallel.py` & `PyTrial-0.0.5/pytrial/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/tabular_utils.py` & `PyTrial-0.0.5/pytrial/utils/tabular_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/trainer.py` & `PyTrial-0.0.5/pytrial/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/pytrial/utils/trial_utils.py` & `PyTrial-0.0.5/pytrial/utils/trial_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.4/setup.py` & `PyTrial-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'PyTrial',
-    version = '0.0.4',
-    author = 'Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun',
+    version = '0.0.5',
+    author = 'Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun',
     author_email = 'zifengw2@illinois.edu',
     description = 'PyTrial: A Python Package for Artificial Intelligence in Drug Development',
     url = 'https://github.com/RyanWangZf/pytrial',
     keywords=['drug development', 'clinical trial', 'artificial intelligence', 'deep learning', 'machine learning'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=['test']),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
 )
```

