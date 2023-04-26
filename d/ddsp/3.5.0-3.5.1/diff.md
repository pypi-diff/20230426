# Comparing `tmp/ddsp-3.5.0.tar.gz` & `tmp/ddsp-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddsp-3.5.0.tar", last modified: Tue Oct  4 01:01:47 2022, max compression
+gzip compressed data, was "dist/ddsp-3.5.1.tar", last modified: Wed Apr 26 18:27:36 2023, max compression
```

## Comparing `ddsp-3.5.0.tar` & `ddsp-3.5.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2022-10-04 01:01:47.000000 ddsp-3.5.0/setup.cfg
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13361 2022-10-04 01:01:46.000000 ddsp-3.5.0/README.md
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2022-10-04 01:01:47.000000 ddsp-3.5.0/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3172 2022-10-04 01:01:46.000000 ddsp-3.5.0/setup.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/effects_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/synths.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/colab/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/colab/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10038 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/colab/colab_utils.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/test_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/processors_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/core.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/spectral_ops.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/version.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/processors.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/spectral_ops_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/effects.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/losses_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10130 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/heuristics.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/models/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/inverse_synthesis.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/autoencoder_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/model.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/models/midi_autoencoder.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/metrics_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/eval_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/decoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/preprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/inference.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/nn_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/plotting.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/preprocessing_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/ddsp_run.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    19956 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/metrics.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/trainers.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/encoders.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/summaries.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/evaluators.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/models/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/models/vst/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/vst/vst_32k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/vst/vst_48k.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/vst/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/vst/vst.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/models/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/optimization/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/optimization/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/optimization/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/optimization/base_tpu.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/datasets/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/datasets/base.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/datasets/tfrecord.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/datasets/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/datasets/nsynth.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/eval/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/heuristic_power.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/heuristic.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/basic_f0_ld_twm.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/midi_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/basic_f0_ld.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/eval/basic.gin
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/papers/
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/__init__.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/finetune_model.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/ddsp_export.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/cloud.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/postprocessing.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/train_util.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/decoders_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    45842 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/nn.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/heuristics_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/docker/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/docker/task_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/docker/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/docker/ddsp_ai_platform.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/docker/task.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp/training/data_preparation/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/__init__.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/synthetic_data.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/training/cloud_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/core_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/losses.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/dags_test.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/dags.py
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2022-10-04 01:01:46.000000 ddsp-3.5.0/ddsp/synths_test.py
-drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      430 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/requires.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)     3282 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/SOURCES.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/PKG-INFO
--rw-r-----   0 jesseengel (399530) primarygroup (89939)      424 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/entry_points.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/dependency_links.txt
--rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2022-10-04 01:01:47.000000 ddsp-3.5.0/ddsp.egg-info/top_level.txt
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)       63 2023-04-26 18:27:36.000000 ddsp-3.5.1/setup.cfg
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13253 2023-04-26 18:27:33.000000 ddsp-3.5.1/README.md
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-26 18:27:36.000000 ddsp-3.5.1/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3269 2023-04-26 18:27:33.000000 ddsp-3.5.1/setup.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3873 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/effects_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11482 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/synths.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/colab/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/colab/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10035 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/colab/colab_utils.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1139 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/test_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      908 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3753 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/processors_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    63698 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/core.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19427 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/spectral_ops.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      794 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/version.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9610 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/processors.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11158 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/spectral_ops_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13484 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/effects.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3189 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/losses_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10127 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/heuristics.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/models/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11984 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/inverse_synthesis.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2482 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1594 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2834 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/autoencoder_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4715 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/model.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    23617 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/models/midi_autoencoder.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9529 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/metrics_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9122 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/eval_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9400 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/decoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8503 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/preprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    21779 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19583 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/inference.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8753 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/nn_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7919 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/plotting.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2292 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/preprocessing_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1182 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8700 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/ddsp_run.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    19956 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/metrics.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     6810 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/trainers.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    15113 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/encoders.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    16563 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/summaries.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     8307 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/evaluators.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/models/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst_32k.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2717 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst_48k.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2453 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/vst/vst.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1854 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1049 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/models/solo_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/optimization/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      416 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      116 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/optimization/base_tpu.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/datasets/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      224 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/base.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      351 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/tfrecord.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      475 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/datasets/nsynth.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/eval/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      176 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/heuristic_power.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      170 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/heuristic.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      158 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic_f0_ld_twm.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      150 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/midi_ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      138 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic_f0_ld.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      119 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/eval/basic.gin
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      217 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/tiny_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      221 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/nsynth_ae.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      267 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/solo_instrument.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/__init__.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     1881 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      582 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      730 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      472 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_model.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      679 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    12720 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/ddsp_export.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2885 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/cloud.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    13804 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/postprocessing.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    11770 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/train_util.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4177 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/decoders_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    45858 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/nn.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3010 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/heuristics_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/docker/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3441 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/task_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      640 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     9500 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/ddsp_ai_platform.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     5036 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/docker/task.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp/training/data_preparation/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     4406 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10303 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      692 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/__init__.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3852 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    10070 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/synthetic_data.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7832 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     2970 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/training/cloud_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    36651 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/core_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)    40636 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/losses.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3744 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/dags_test.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     7416 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/dags.py
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3736 2023-04-26 18:27:33.000000 ddsp-3.5.1/ddsp/synths_test.py
+drwxr-x---   0 jesseengel (399530) primarygroup (89939)        0 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      445 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/requires.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)     3282 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/SOURCES.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      658 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/PKG-INFO
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)      424 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/entry_points.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        1 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/dependency_links.txt
+-rw-r-----   0 jesseengel (399530) primarygroup (89939)        5 2023-04-26 18:27:36.000000 ddsp-3.5.1/ddsp.egg-info/top_level.txt
```

### Comparing `ddsp-3.5.0/README.md` & `ddsp-3.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 <img src="https://storage.googleapis.com/ddsp/github_images/ddsp_logo.png" width="200px" alt="logo"></img>
 </div>
 
 # DDSP: Differentiable Digital Signal Processing
 [![Build Status](https://github.com/magenta/ddsp/workflows/build/badge.svg)](https://github.com/magenta/ddsp/actions?query=workflow%3Abuild)
-[![Downloads](https://static.pepy.tech/personalized-badge/crepe?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/crepe)
+[![Downloads](https://static.pepy.tech/badge/ddsp)](https://pepy.tech/project/ddsp)
 
 [**Demos**](./ddsp/colab/demos)
 | [**Tutorials**](./ddsp/colab/tutorials)
 | [**Installation**](#Installation)
 | [**Overview**](#Overview)
 | [**Blog Post**](https://magenta.tensorflow.org/ddsp)
 | [**Papers**](./ddsp/training/gin/papers)
```

### Comparing `ddsp-3.5.0/PKG-INFO` & `ddsp-3.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.5.0
+Version: 3.5.1
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Provides-Extra: gcp
 Provides-Extra: data_preparation
 Provides-Extra: test
+Provides-Extra: gcp
```

### Comparing `ddsp-3.5.0/setup.py` & `ddsp-3.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,24 +36,25 @@
         '': ['*.gin'],
     },
     scripts=[],
     install_requires=[
         'absl-py',
         'cloudml-hypertune',
         'crepe<=0.0.12',
+        'dill<=0.3.4',
         'future',
         'gin-config>=0.3.0',
         'google-cloud-storage',
         'hmmlearn<=0.2.7',
         'librosa',
         'pydub',
-        'protobuf<=3.20.*',  # temporary fix for proto dependency bug
+        'protobuf<=3.20',  # temporary fix for proto dependency bug
         'mir_eval',
         'note_seq<0.0.4',
-        'numpy',
+        'numpy<1.24',
         'scipy',
         'six',
         'tensorflow',
         'tensorflow-addons',
         'tensorflowjs<3.19',
         'tensorflow-probability',
         'tensorflow-datasets',
@@ -67,23 +68,25 @@
         'data_preparation': [
             'apache_beam',
             # TODO(jesseengel): Remove versioning when beam import is fixed.
             'pyparsing<=2.4.7'
         ],
         'test': ['pytest', 'pylint!=2.5.0'],
     },
+    # pylint: disable=line-too-long
     entry_points={
         'console_scripts': [
             'ddsp_export = ddsp.training.ddsp_export:console_entry_point',
             'ddsp_run = ddsp.training.ddsp_run:console_entry_point',
             'ddsp_prepare_tfrecord = ddsp.training.data_preparation.ddsp_prepare_tfrecord:console_entry_point',
             'ddsp_generate_synthetic_dataset = ddsp.training.data_preparation.ddsp_generate_synthetic_dataset:console_entry_point',
             'ddsp_ai_platform = ddsp.training.docker.ddsp_ai_platform:console_entry_point',
         ],
     },
+    # pylint: enable=line-too-long
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
```

### Comparing `ddsp-3.5.0/ddsp/effects_test.py` & `ddsp-3.5.1/ddsp/effects_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/synths.py` & `ddsp-3.5.1/ddsp/synths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/colab/__init__.py` & `ddsp-3.5.1/ddsp/colab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/colab/colab_utils.py` & `ddsp-3.5.1/ddsp/colab/colab_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -227,15 +227,15 @@
   ## Computes mininmum adjustment distance.
   cost_diffs = np.abs(midi_diffs)
   cost_diffs = np.mean(weights * cost_diffs, axis=0)
 
   ## Computes mininmum "note" transitions.
   f0_at = f0_midi[mask_on][:, np.newaxis] - midi_diffs
   f0_at_diffs = np.diff(f0_at, axis=0)
-  deltas = (f0_at_diffs != 0.0).astype(np.float)
+  deltas = (f0_at_diffs != 0.0).astype(float)
   cost_deltas = np.mean(weights[:-1] * deltas, axis=0)
 
   # Tuning factor is minimum cost.
   norm = lambda x: (x - np.mean(x)) / np.std(x)
   cost = norm(cost_deltas) + norm(cost_diffs)
   return tuning_factors[np.argmin(cost)]
```

### Comparing `ddsp-3.5.0/ddsp/test_util.py` & `ddsp-3.5.1/ddsp/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/__init__.py` & `ddsp-3.5.1/ddsp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/processors_test.py` & `ddsp-3.5.1/ddsp/processors_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/core.py` & `ddsp-3.5.1/ddsp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/spectral_ops.py` & `ddsp-3.5.1/ddsp/spectral_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/version.py` & `ddsp-3.5.1/ddsp/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,8 +14,8 @@
 
 r"""Separate file for storing the current version of DDSP.
 
 Stored in a separate file so that setup.py can reference the version without
 pulling in all the dependencies in __init__.py.
 """
 
-__version__ = '3.5.0'
+__version__ = '3.5.1'
```

### Comparing `ddsp-3.5.0/ddsp/processors.py` & `ddsp-3.5.1/ddsp/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/spectral_ops_test.py` & `ddsp-3.5.1/ddsp/spectral_ops_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/effects.py` & `ddsp-3.5.1/ddsp/effects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/losses_test.py` & `ddsp-3.5.1/ddsp/losses_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/heuristics.py` & `ddsp-3.5.1/ddsp/training/heuristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -252,15 +252,15 @@
 @gin.register
 def strided_freq_change(controls,
                         frame_widths=(2, 4, 8, 16, 32),
                         pad_mode='front'):
   """Finds changes in f0 of >= 1 semitone across multiple strides."""
   f0 = np.squeeze(controls['f0_hz'].numpy())
   f0_midi = ddsp.core.hz_to_midi(f0)
-  transitions = np.ones(len(f0), dtype=np.bool)
+  transitions = np.ones(len(f0), dtype=bool)
   for frame_width in frame_widths:
     padded_f0 = pad_for_frame(
         f0_midi, mode=pad_mode, frame_width=frame_width, axis=0)
     frames = tf.signal.frame(padded_f0, frame_width, 1)
     semitone_changes = np.abs(frames[..., 0] - frames[..., -1]) > 0.75
 
     # only flip if other strides didn't find this transition
```

### Comparing `ddsp-3.5.0/ddsp/training/models/inverse_synthesis.py` & `ddsp-3.5.1/ddsp/training/models/inverse_synthesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/models/autoencoder.py` & `ddsp-3.5.1/ddsp/training/models/autoencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/models/__init__.py` & `ddsp-3.5.1/ddsp/training/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/models/autoencoder_test.py` & `ddsp-3.5.1/ddsp/training/models/autoencoder_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/models/model.py` & `ddsp-3.5.1/ddsp/training/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/models/midi_autoencoder.py` & `ddsp-3.5.1/ddsp/training/models/midi_autoencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/metrics_test.py` & `ddsp-3.5.1/ddsp/training/metrics_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/eval_util.py` & `ddsp-3.5.1/ddsp/training/eval_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/decoders.py` & `ddsp-3.5.1/ddsp/training/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/preprocessing.py` & `ddsp-3.5.1/ddsp/training/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data.py` & `ddsp-3.5.1/ddsp/training/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/inference.py` & `ddsp-3.5.1/ddsp/training/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/nn_test.py` & `ddsp-3.5.1/ddsp/training/nn_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/plotting.py` & `ddsp-3.5.1/ddsp/training/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/preprocessing_test.py` & `ddsp-3.5.1/ddsp/training/preprocessing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/__init__.py` & `ddsp-3.5.1/ddsp/training/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/ddsp_run.py` & `ddsp-3.5.1/ddsp/training/ddsp_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/metrics.py` & `ddsp-3.5.1/ddsp/training/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/trainers.py` & `ddsp-3.5.1/ddsp/training/trainers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/encoders.py` & `ddsp-3.5.1/ddsp/training/encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/summaries.py` & `ddsp-3.5.1/ddsp/training/summaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/evaluators.py` & `ddsp-3.5.1/ddsp/training/evaluators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/vst/vst_32k.gin` & `ddsp-3.5.1/ddsp/training/gin/models/vst/vst_32k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/vst/vst_48k.gin` & `ddsp-3.5.1/ddsp/training/gin/models/vst/vst_48k.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/vst/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/models/vst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/vst/vst.gin` & `ddsp-3.5.1/ddsp/training/gin/models/vst/vst.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/ae.gin` & `ddsp-3.5.1/ddsp/training/gin/models/ae.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/models/solo_instrument.gin` & `ddsp-3.5.1/ddsp/training/gin/models/solo_instrument.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/optimization/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/optimization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/datasets/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/eval/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/eval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/iclr2020/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/papers/iclr2020/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/papers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/icml2020/pretrain_model.gin` & `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_model.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/icml2020/__init__.py` & `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/icml2020/finetune_dataset.gin` & `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/finetune_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin` & `ddsp-3.5.1/ddsp/training/gin/papers/icml2020/pretrain_dataset.gin`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp/training/ddsp_export.py` & `ddsp-3.5.1/ddsp/training/ddsp_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/cloud.py` & `ddsp-3.5.1/ddsp/training/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/postprocessing.py` & `ddsp-3.5.1/ddsp/training/postprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/train_util.py` & `ddsp-3.5.1/ddsp/training/train_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/decoders_test.py` & `ddsp-3.5.1/ddsp/training/decoders_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/nn.py` & `ddsp-3.5.1/ddsp/training/nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 
 import inspect
 
 from ddsp import core
 from ddsp import losses
 import gin
 import tensorflow as tf
-import tensorflow_addons as tfa
+from tensorflow_addons.layers import SpectralNormalization
 import tensorflow_probability as tfp
 
 tfk = tf.keras
 tfkl = tfk.layers
 
 
 # False positive lint error on tf.split().
@@ -1098,15 +1098,15 @@
       layer = layer_class(ch,
                           (k, 1),
                           (stride, 1),
                           dilation_rate=(dilation, 1),
                           padding='same',
                           kernel_initializer=initializer)
       if spectral_norm:
-        return tfa.layers.SpectralNormalization(layer)
+        return SpectralNormalization(layer)
       else:
         return layer
 
     # Layer Factories.
     def dilated_conv(i):
       """Generates a dilated convolution layer, based on `i` depth in stack."""
       if dilation > 0:
```

### Comparing `ddsp-3.5.0/ddsp/training/heuristics_test.py` & `ddsp-3.5.1/ddsp/training/heuristics_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/docker/task_test.py` & `ddsp-3.5.1/ddsp/training/docker/task_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/docker/__init__.py` & `ddsp-3.5.1/ddsp/training/docker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/docker/ddsp_ai_platform.py` & `ddsp-3.5.1/ddsp/training/docker/ddsp_ai_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/docker/task.py` & `ddsp-3.5.1/ddsp/training/docker/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py` & `ddsp-3.5.1/ddsp/training/data_preparation/ddsp_generate_synthetic_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/prepare_tfrecord_lib.py` & `ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/__init__.py` & `ddsp-3.5.1/ddsp/training/data_preparation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py` & `ddsp-3.5.1/ddsp/training/data_preparation/ddsp_prepare_tfrecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/synthetic_data.py` & `ddsp-3.5.1/ddsp/training/data_preparation/synthetic_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py` & `ddsp-3.5.1/ddsp/training/data_preparation/prepare_tfrecord_lib_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/training/cloud_test.py` & `ddsp-3.5.1/ddsp/training/cloud_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/core_test.py` & `ddsp-3.5.1/ddsp/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/losses.py` & `ddsp-3.5.1/ddsp/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/dags_test.py` & `ddsp-3.5.1/ddsp/dags_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/dags.py` & `ddsp-3.5.1/ddsp/dags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp/synths_test.py` & `ddsp-3.5.1/ddsp/synths_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The DDSP Authors.
+# Copyright 2023 The DDSP Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ddsp-3.5.0/ddsp.egg-info/SOURCES.txt` & `ddsp-3.5.1/ddsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddsp-3.5.0/ddsp.egg-info/PKG-INFO` & `ddsp-3.5.1/ddsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ddsp
-Version: 3.5.0
+Version: 3.5.1
 Summary: Differentiable Digital Signal Processing 
 Home-page: http://github.com/magenta/ddsp
 Author: Google Inc.
 Author-email: no-reply@google.com
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: audio dsp signalprocessing machinelearning music
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Provides-Extra: gcp
 Provides-Extra: data_preparation
 Provides-Extra: test
+Provides-Extra: gcp
```

