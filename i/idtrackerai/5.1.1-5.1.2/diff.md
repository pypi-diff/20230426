# Comparing `tmp/idtrackerai-5.1.1.tar.gz` & `tmp/idtrackerai-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.1.1.tar", last modified: Wed Apr 26 09:36:19 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.2.tar", last modified: Wed Apr 26 11:46:31 2023, max compression
```

## Comparing `idtrackerai-5.1.1.tar` & `idtrackerai-5.1.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.1/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1597 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3079 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.149648 idtrackerai-5.1.1/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.149648 idtrackerai-5.1.1/src/idmatcherai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idmatcherai/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9092 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idmatcherai/main.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idmatcherai/matcher.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15527 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31677 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-04-24 13:20:28.000000 idtrackerai-5.1.1/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7524 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3144 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/crossings_detection.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5057 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.161648 idtrackerai-5.1.1/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-03-20 08:48:28.000000 idtrackerai-5.1.1/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    25591 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.165648 idtrackerai-5.1.1/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8913 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.165648 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15885 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    23986 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.165648 idtrackerai-5.1.1/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4271 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/network/evaluate.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/learners.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/train.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/network/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27568 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3599 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-26 09:35:16.000000 idtrackerai-5.1.1/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    36591 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-03-21 11:15:37.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/accumulation_manager_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/assigner.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/identification_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/identification_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/identity_transfer.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai/tracker/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/network/get_predictions.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/network/stop_training_criteria.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/network/trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1144 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2990 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12519 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    33060 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.153648 idtrackerai-5.1.1/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5669 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      371 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-04-26 09:36:19.000000 idtrackerai-5.1.1/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6097 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-04-12 07:40:32.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.169648 idtrackerai-5.1.1/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4975 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-04-24 13:20:28.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-04-24 13:20:28.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5405 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16140 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5827 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-03-20 08:48:29.000000 idtrackerai-5.1.1/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31781 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      425 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-03-21 11:17:49.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12940 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 09:36:19.173648 idtrackerai-5.1.1/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6020 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4866 2023-04-12 10:06:11.000000 idtrackerai-5.1.1/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2092 2023-04-26 09:35:10.000000 idtrackerai-5.1.1/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.2/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1597 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3079 2023-04-26 11:36:15.000000 idtrackerai-5.1.2/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9092 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15562 2023-04-26 11:34:40.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31737 2023-04-26 11:35:45.000000 idtrackerai-5.1.2/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7524 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3144 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossings_detection.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5057 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.683650 idtrackerai-5.1.2/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    25591 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8913 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15885 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    23986 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4271 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27568 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3634 2023-04-26 11:34:55.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-26 09:35:16.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    36591 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-03-21 11:15:37.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/assigner.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/identity_transfer.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/tracker/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/get_predictions.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/stop_training_criteria.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1144 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2990 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12519 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    33060 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5669 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      371 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6097 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-04-12 07:40:32.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4975 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5405 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16140 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5827 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31781 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      425 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12940 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6020 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4866 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2092 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.1/LICENSE` & `idtrackerai-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/PKG-INFO` & `idtrackerai-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.1
+Version: 5.1.2
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.1/README.md` & `idtrackerai-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/pyproject.toml` & `idtrackerai-5.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.1.1"
+version = "5.1.2"
 authors = [
     { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
```

### Comparing `idtrackerai-5.1.1/src/idmatcherai/main.py` & `idtrackerai-5.1.2/src/idmatcherai/main.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idmatcherai/matcher.py` & `idtrackerai-5.1.2/src/idmatcherai/matcher.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/__init__.py` & `idtrackerai-5.1.2/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.2/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.2/src/idtrackerai/animals_detection/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,17 @@
         )
 
     # Applying the mask
     if ROI_mask is not None:
         segmented_frame *= ROI_mask  # type: ignore
 
     # Extract blobs info
+    # TODO cv2.CHAIN_APPROX_TC89_L1
     contours = cv2.findContours(
-        segmented_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_TC89_L1
+        segmented_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
     )[0]
 
     # Filter contours by size
     areas = []
     good_contours = []
     for contour in contours:
         area = cv2.contourArea(contour)
```

### Comparing `idtrackerai-5.1.1/src/idtrackerai/blob.py` & `idtrackerai-5.1.2/src/idtrackerai/blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,45 +604,46 @@
         ] = masked_bbox_image
 
         M = cv2.getRotationMatrix2D(
             (diag, diag), self.orientation * 180 / np.pi - 45, 1
         )
 
         # old method
-        # id_img = cv2.warpAffine(
-        #     src=id_img,
-        #     M=M,
-        #     dsize=(diag + img_size2, diag + img_size2),
-        #     borderMode=cv2.BORDER_CONSTANT,
-        #     flags=cv2.INTER_CUBIC,
-        # )
-        # return id_img[-img_size:, -img_size:]
-
         id_img = cv2.warpAffine(
             src=id_img,
             M=M,
-            dsize=(diag + img_size, diag + img_size),
+            dsize=(diag + img_size2, diag + img_size2),
             borderMode=cv2.BORDER_CONSTANT,
             flags=cv2.INTER_CUBIC,
         )
+        return id_img[-img_size:, -img_size:]
 
-        # we build the offset like this to have the minimal ones on the
-        # beginning of the array and be preferably selected by max()
-        origins = [0]
-        for offset in range(img_size2 // 2):
-            origins.extend((diag - img_size2 + offset, diag - img_size2 - offset))
-
-        origin = max(
-            origins,
-            key=lambda origin: np.count_nonzero(
-                id_img[origin : origin + img_size, origin : origin + img_size]
-            ),
-        )
+        # TODO proposed future method
+        # id_img = cv2.warpAffine(
+        #     src=id_img,
+        #     M=M,
+        #     dsize=(diag + img_size, diag + img_size),
+        #     borderMode=cv2.BORDER_CONSTANT,
+        #     flags=cv2.INTER_CUBIC,
+        # )
+
+        # # we build the offset like this to have the minimal ones on the
+        # # beginning of the array and be preferably selected by max()
+        # origins = [0]
+        # for offset in range(img_size2 // 2):
+        #     origins.extend((diag - img_size2 + offset, diag - img_size2 - offset))
+
+        # origin = max(
+        #     origins,
+        #     key=lambda origin: np.count_nonzero(
+        #         id_img[origin : origin + img_size, origin : origin + img_size]
+        #     ),
+        # )
 
-        return id_img[origin : origin + img_size, origin : origin + img_size]
+        # return id_img[origin : origin + img_size, origin : origin + img_size]
 
     def get_bbox_mask(self) -> np.ndarray:
         base = np.zeros(
             (
                 self.bbox_in_frame_coordinates[1][1]
                 - self.bbox_in_frame_coordinates[0][1]
                 + 2,  # 2 bbox_image_pads
```

### Comparing `idtrackerai-5.1.1/src/idtrackerai/constants.toml` & `idtrackerai-5.1.2/src/idtrackerai/constants.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/crossing_detector.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/crossings_detection.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossings_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/model_area.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py` & `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.2/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.2/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/fragment.py` & `idtrackerai-5.1.2/src/idtrackerai/fragment.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.2/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.2/src/idtrackerai/globalfragment.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.2/src/idtrackerai/list_of_blobs.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.2/src/idtrackerai/list_of_fragments.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.2/src/idtrackerai/list_of_global_fragments.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/evaluate.py` & `idtrackerai-5.1.2/src/idtrackerai/network/evaluate.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/learners.py` & `idtrackerai-5.1.2/src/idtrackerai/network/learners.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/models.py` & `idtrackerai-5.1.2/src/idtrackerai/network/models.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/network_params.py` & `idtrackerai-5.1.2/src/idtrackerai/network/network_params.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/train.py` & `idtrackerai-5.1.2/src/idtrackerai/network/train.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/network/utils.py` & `idtrackerai-5.1.2/src/idtrackerai/network/utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/erosion.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     segmented_eroded_frame = cv2.erode(
         src=segmented_frame,
         kernel=np.ones(video.erosion_kernel_size, np.uint8),
         iterations=1,
     )
 
     # Extract blobs info
+    # TODO cv2.CHAIN_APPROX_TC89_L1
     contours = cv2.findContours(
-        segmented_eroded_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_TC89_L1
+        segmented_eroded_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
     )[0]
 
     return [
         Blob(contour, frame_number=frame_number, pixels_are_from_eroded_blob=True)
         for contour in contours
     ]
```

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/postprocess/trajectories_to_csv.py` & `idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/accumulation_manager_utils.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/assigner.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/assigner.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/identification_dataloader.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataloader.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/dataset/identification_dataset.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/identity_transfer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/network/get_predictions.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/network/get_predictions.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/network/stop_training_criteria.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/network/stop_training_criteria.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/network/trainer.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/network/trainer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/pre_trainer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.2/src/idtrackerai/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.2/src/idtrackerai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.2/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.2/src/idtrackerai/utils/confparams.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.2/src/idtrackerai/utils/init_logger.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.2/src/idtrackerai/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai/video.py` & `idtrackerai-5.1.2/src/idtrackerai/video.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.2/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.1
+Version: 5.1.2
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.1/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.2/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/__init__.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/themes.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/themes.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.2/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.2/src/idtrackerai_start_app/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.2/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validation_GUI.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.2/src/idtrackerai_video/general_video.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_video/individual_videos.py` & `idtrackerai-5.1.2/src/idtrackerai_video/individual_videos.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.1/src/idtrackerai_video/main.py` & `idtrackerai-5.1.2/src/idtrackerai_video/main.py`

 * *Files identical despite different names*

