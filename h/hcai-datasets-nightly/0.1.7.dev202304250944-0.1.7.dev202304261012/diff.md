# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202304250944.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202304261012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304250944.tar", last modified: Tue Apr 25 09:44:45 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304261012.tar", last modified: Wed Apr 26 10:12:38 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202304250944.tar` & `hcai-datasets-nightly-0.1.7.dev202304261012.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10746 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.976669 hcai-datasets-nightly-0.1.7.dev202304261012/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-26 10:12:38.976669 hcai-datasets-nightly-0.1.7.dev202304261012/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.968669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.968669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.968669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.968669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-26 10:12:26.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20593 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23409 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10997 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.972669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 10:12:38.976669 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-26 10:12:38.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-26 10:12:38.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 10:12:38.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-26 10:12:38.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-26 10:12:38.000000 hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 10:12:38.976669 hcai-datasets-nightly-0.1.7.dev202304261012/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-26 10:12:27.000000 hcai-datasets-nightly-0.1.7.dev202304261012/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304261012/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304250944
+Version: 0.1.7.dev202304261012
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/README.md` & `hcai-datasets-nightly-0.1.7.dev202304261012/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,24 +79,24 @@
         self.annotator = annotator
         self.left_context_ms = ndu.parse_time_string_to_ms(left_context)
         self.right_context_ms = ndu.parse_time_string_to_ms(right_context)
         self.frame_size_ms = (
             ndu.parse_time_string_to_ms(frame_size) if frame_size else None
         )
 
-
         if self.frame_size_ms == 0:
-            print("WARNING: Frame size 0 is invalid. Returning whole session as sample.")
+            print(
+                "WARNING: Frame size 0 is invalid. Returning whole session as sample."
+            )
             self.frame_size_ms = None
 
         self.stride_ms = (
             ndu.parse_time_string_to_ms(stride) if stride else self.frame_size_ms
         )
 
-
         self.start_ms = ndu.parse_time_string_to_ms(start)
         if not self.start_ms:
             self.start_ms = 0
 
         self.end_ms = ndu.parse_time_string_to_ms(end)
         if not self.end_ms:
             self.end_ms = float("inf")
@@ -276,14 +276,16 @@
                 sample_data_path = os.path.join(
                     self.nova_data_dir,
                     self.dataset,
                     self.sessions[0],
                     sample_stream_name,
                 )
                 dtype = nt.string_to_enum(nt.DataTypes, data_stream["type"])
+                window_size = (self.left_context_ms + self.frame_size_ms + self.right_context_ms) / (1 / data_stream["sr"])
+                # TODO
                 try:
                     if dtype == nt.DataTypes.VIDEO:
                         data = VideoData(
                             role=role,
                             name=data_stream["name"],
                             file_ext=data_stream["fileExt"],
                             sr=data_stream["sr"],
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -473,14 +473,50 @@
                     f"Unexpected error uploading annotations for {database} - {session} - {scheme} - {annotator}. Upload failed."
                 )
                 return ""
             else:
                 anno_id = success.inserted_id
         return anno_id
 
+    def set_data_streams(self, database: str, file_name: str, file_ext: str, stream_type: str,  is_valid:bool, sr: float, dimlabels: list):
+
+        # check if datastream already exists
+        mongo_stream = self.get_docs_by_prop(
+            file_name, "name", database, self.STREAM_COLLECTION
+        )
+        if mongo_stream:
+            print(f"INFO: Stream {file_name} already exists in database. Skip adding stream.")
+            return
+
+        # build doc
+        mongo_steam_doc = {
+            "name" : file_name,
+            "fileExt" : file_ext,
+            "type" : stream_type,
+            "isValid" : is_valid,
+            "sr" : sr,
+            "dimlabels": dimlabels
+        }
+
+        # insert datastream
+        success = self.insert_doc_by_prop(
+            doc=mongo_steam_doc,
+            database=database,
+            collection=self.STREAM_COLLECTION,
+        )
+
+
+        if not success.acknowledged:
+            warnings.warn(f"Unexpected error adding stream for {database} - {file_name}.{file_ext}. Upload failed.")
+            return ""
+        else:
+            stream_id = success.inserted_id
+
+        return stream_id
+
     def get_mongo_scheme(self, scheme, database):
         mongo_scheme = self.get_docs_by_prop(scheme, "name", database, self.SCHEME_COLLECTION)
         if not mongo_scheme:
             warnings.warn(f"Unknown scheme {scheme} found")
             return ""
 
         return mongo_scheme
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         name: str = "",
         file_ext: str = "stream",
         sr: int = 0,
         data_type: nt.DataTypes = None,
         is_valid: bool = True,
         sample_data_path: str = "",
         lazy_loading: bool = False,
+        n_samples_per_window: int = 1
     ):
         """
 
         Args:
             role ():
             name ():
             file_ext ():
@@ -45,14 +46,15 @@
         self.lazy_loading = lazy_loading
         self.data_type = data_type
 
         # Set when populate_meta_info is called
         self.sample_data_shape = None
         self.np_data_type = None
         self.meta_loaded = False
+        self.n_frames_per_window = n_samples_per_window
 
         # Set when open_file_reader is called
         self.file_path = None
         self.file_reader = None
         self.dur = sys.maxsize
 
         if sample_data_path:
@@ -250,14 +252,22 @@
         }
 
     def get_sample_hook(self, frame_start_ms: int, frame_end_ms: int):
         try:
             self.data_stream_opend()
             start_frame = milli_seconds_to_frame(self.sr, frame_start_ms)
             end_frame = milli_seconds_to_frame(self.sr, frame_end_ms)
+
+            # rounding error
+            #if start_frame == end_frame:
+            #    end_frame += 1
+            #elif end_frame - start_frame > 1:
+
+
+
             return self.file_reader.data[start_frame:end_frame]
         except RuntimeError:
             print(
                 "Could not get chunk {}-{} from data stream {}".format(
                     frame_start_ms, frame_end_ms, merge_role_key(self.role, self.name)
                 )
             )
@@ -284,26 +294,27 @@
 
 
 ##########################
 # General helper functions
 ##########################
 
 
-def frame_to_seconds(sr: int, frame: int) -> float:
-    return frame / sr
+#def frame_to_seconds(sr: int, frame: int) -> float:
+#    return frame / sr
 
 
 def seconds_to_frame(sr: int, time_s: float) -> int:
     return round(time_s * sr)
 
 
 def milli_seconds_to_frame(sr: int, time_ms: int) -> int:
     return seconds_to_frame(sr=sr, time_s=time_ms / 1000)
 
 
+
 def parse_time_string_to_ms(frame: Union[str, int, float]) -> int:
     # if frame is specified milliseconds as string
     if str(frame).endswith("ms"):
         try:
             return int(frame[:-2])
         except ValueError:
             raise ValueError(
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304250944
+Version: 0.1.7.dev202304261012
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202304261012/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304250944/setup.py` & `hcai-datasets-nightly-0.1.7.dev202304261012/setup.py`

 * *Files identical despite different names*

