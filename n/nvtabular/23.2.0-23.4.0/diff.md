# Comparing `tmp/nvtabular-23.2.0.tar.gz` & `tmp/nvtabular-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvtabular-23.2.0.tar", last modified: Mon Mar 13 19:39:18 2023, max compression
+gzip compressed data, was "nvtabular-23.4.0.tar", last modified: Wed Apr 26 19:16:38 2023, max compression
```

## Comparing `nvtabular-23.2.0.tar` & `nvtabular-23.4.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.828449 nvtabular-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-13 19:38:23.000000 nvtabular-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-13 19:38:23.000000 nvtabular-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-03-13 19:39:18.828449 nvtabular-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-13 19:38:23.000000 nvtabular-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.800449 nvtabular-23.2.0/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.808449 nvtabular-23.2.0/cpp/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-13 19:38:23.000000 nvtabular-23.2.0/cpp/nvtabular/__init__.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.812449 nvtabular-23.2.0/cpp/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-13 19:38:23.000000 nvtabular-23.2.0/cpp/nvtabular/inference/__init__.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-03-13 19:38:23.000000 nvtabular-23.2.0/cpp/nvtabular/inference/categorify.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-13 19:38:23.000000 nvtabular-23.2.0/cpp/nvtabular/inference/fill.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.804449 nvtabular-23.2.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.812449 nvtabular-23.2.0/merlin/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-13 19:38:23.000000 nvtabular-23.2.0/merlin/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.812449 nvtabular-23.2.0/merlin/transforms/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-13 19:38:23.000000 nvtabular-23.2.0/merlin/transforms/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.828449 nvtabular-23.2.0/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-13 19:39:18.828449 nvtabular-23.2.0/nvtabular/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.812449 nvtabular-23.2.0/nvtabular/framework_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/framework_utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/framework_utils/torch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/torch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/torch/layers/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/torch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/framework_utils/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/inference/triton/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/benchmarking_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.816449 nvtabular-23.2.0/nvtabular/inference/triton/model/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/model/model_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/triton/workflow_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.820449 nvtabular-23.2.0/nvtabular/inference/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/workflow/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/workflow/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/inference/workflow/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.820449 nvtabular-23.2.0/nvtabular/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/loader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.824449 nvtabular-23.2.0/nvtabular/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/add_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/categorify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10296 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/column_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/difference_lag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/drop_low_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/dropna.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/hashed_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/join_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/join_groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/lambdaop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/list_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/logop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/reduce_dtype_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/stat_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/target_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/ops/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.824449 nvtabular-23.2.0/nvtabular/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17129 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/tools/data_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/tools/dataset_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/tools/inspector_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.828449 nvtabular-23.2.0/nvtabular/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/workflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/workflow/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17047 2023-03-13 19:38:23.000000 nvtabular-23.2.0/nvtabular/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.812449 nvtabular-23.2.0/nvtabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-13 19:39:18.000000 nvtabular-23.2.0/nvtabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-13 19:38:23.000000 nvtabular-23.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:39:18.828449 nvtabular-23.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-13 19:38:23.000000 nvtabular-23.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-13 19:38:23.000000 nvtabular-23.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-13 19:38:23.000000 nvtabular-23.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:38:23.000000 nvtabular-23.2.0/requirements/gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-13 19:38:23.000000 nvtabular-23.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-13 19:39:18.828449 nvtabular-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-03-13 19:38:23.000000 nvtabular-23.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-03-13 19:38:23.000000 nvtabular-23.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 19:15:49.000000 nvtabular-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 19:15:49.000000 nvtabular-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 19:16:38.698010 nvtabular-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-26 19:15:49.000000 nvtabular-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.678010 nvtabular-23.4.0/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/cpp/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/__init__.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/cpp/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/__init__.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/categorify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/fill.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.678010 nvtabular-23.4.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/merlin/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 19:15:49.000000 nvtabular-23.4.0/merlin/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/merlin/transforms/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 19:15:49.000000 nvtabular-23.4.0/merlin/transforms/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/benchmarking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/triton/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/model/model_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/workflow_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/hugectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61346 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/categorify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/column_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/difference_lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/drop_low_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/dropna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/hashed_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/join_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/join_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/lambdaop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/list_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/logop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/reduce_dtype_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/stat_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/target_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/data_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/dataset_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/inspector_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17893 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 19:15:49.000000 nvtabular-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-26 19:16:38.698010 nvtabular-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-26 19:15:49.000000 nvtabular-23.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-04-26 19:15:49.000000 nvtabular-23.4.0/versioneer.py
```

### Comparing `nvtabular-23.2.0/LICENSE` & `nvtabular-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/PKG-INFO` & `nvtabular-23.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nvtabular-23.2.0/README.md` & `nvtabular-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/cpp/nvtabular/__init__.cc` & `nvtabular-23.4.0/cpp/nvtabular/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/cpp/nvtabular/inference/__init__.cc` & `nvtabular-23.4.0/cpp/nvtabular/inference/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/cpp/nvtabular/inference/categorify.cc` & `nvtabular-23.4.0/cpp/nvtabular/inference/categorify.cc`

 * *Files 5% similar despite different names*

```diff
@@ -89,25 +89,31 @@
               insert_int_mapping<double>(values);
               return;
             }
             break;
           case 'u':
             switch (dtype.itemsize())
             {
+            case 2:
+              insert_int_mapping<uint16_t>(values);
+              return;
             case 4:
               insert_int_mapping<uint32_t>(values);
               return;
             case 8:
               insert_int_mapping<uint64_t>(values);
               return;
             }
             break;
           case 'i':
             switch (dtype.itemsize())
             {
+            case 2:
+              insert_int_mapping<int16_t>(values);
+              return;
             case 4:
               insert_int_mapping<int32_t>(values);
               return;
             case 8:
               insert_int_mapping<int64_t>(values);
               return;
             }
@@ -194,23 +200,27 @@
             case 8:
               return transform_int<double>(input);
             }
             break;
           case 'u':
             switch (itemsize)
             {
+            case 2:
+              return transform_int<uint16_t>(input);
             case 4:
               return transform_int<uint32_t>(input);
             case 8:
               return transform_int<uint64_t>(input);
             }
             break;
           case 'i':
             switch (itemsize)
             {
+            case 2:
+              return transform_int<int16_t>(input);
             case 4:
               return transform_int<int32_t>(input);
             case 8:
               return transform_int<int64_t>(input);
             }
             break;
           case 'b':
```

### Comparing `nvtabular-23.2.0/cpp/nvtabular/inference/fill.cc` & `nvtabular-23.4.0/cpp/nvtabular/inference/fill.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/merlin/transforms/__init__.py` & `nvtabular-23.4.0/merlin/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/merlin/transforms/ops/__init__.py` & `nvtabular-23.4.0/merlin/transforms/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/__init__.py` & `nvtabular-23.4.0/nvtabular/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/dispatch.py` & `nvtabular-23.4.0/nvtabular/dispatch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/__init__.py` & `nvtabular-23.4.0/nvtabular/framework_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/__init__.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/__init__.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/embedding.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/interaction.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/interaction.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py` & `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import gc
 
-import cudf
 import tensorflow as tf
-from cudf.core.column.lists import is_list_dtype
-from cudf.io.parquet import ParquetWriter
 from pandas_tfrecords.from_tfrecords import _get_feature_type, read_example
 from tqdm import tqdm
 
+from merlin.core.compat import cudf
+
+if cudf:
+    from cudf.core.column.lists import is_list_dtype
+    from cudf.io.parquet import ParquetWriter
+
 
 def convert_tfrecords_to_parquet(
     filenames, output_dir, compression_type="", chunks=100000, convert_lists=False
 ):
     """
     Converts tfrecord files to parquet file format
```

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/torch/__init__.py` & `nvtabular-23.4.0/nvtabular/framework_utils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/torch/layers/__init__.py` & `nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/torch/layers/embeddings.py` & `nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/torch/models.py` & `nvtabular-23.4.0/nvtabular/framework_utils/torch/models.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/framework_utils/torch/utils.py` & `nvtabular-23.4.0/nvtabular/framework_utils/torch/utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/graph.py` & `nvtabular-23.4.0/nvtabular/graph.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/__init__.py` & `nvtabular-23.4.0/nvtabular/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/__init__.py` & `nvtabular-23.4.0/nvtabular/inference/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/benchmarking_tools.py` & `nvtabular-23.4.0/nvtabular/inference/triton/benchmarking_tools.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/data_conversions.py` & `nvtabular-23.4.0/nvtabular/inference/triton/data_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,24 @@
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 # OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import itertools
 
-try:
-    import cudf
-    import cupy as cp
-except ImportError:
-    cudf = cp = None
-
-import numpy as np
 import pandas as pd
 
+from merlin.core.compat import cudf
+from merlin.core.compat import cupy as cp
+from merlin.core.compat import numpy as np
 from merlin.core.dispatch import build_cudf_list_column, is_list_dtype
 from merlin.dag import Supports
 
+xp = cp or np
+
 
 def convert_format(tensors, kind, target_kind):
     """Converts data from format 'kind' to one of the formats specified in 'target_kind'
     This allows us to convert data to/from dataframe representations for operators that
     only support certain reprentations
     """
 
@@ -50,23 +48,23 @@
     # as tuples of (values, offsets) tensors in this case - but have to do work at
     # each step in terms of converting.
     if kind & target_kind:
         return tensors, kind
 
     elif target_kind & Supports.GPU_DICT_ARRAY:
         if kind == Supports.CPU_DICT_ARRAY:
-            return _convert_array(tensors, cp.array), Supports.GPU_DICT_ARRAY
+            return _convert_array(tensors, xp.array), Supports.GPU_DICT_ARRAY
         elif kind == Supports.CPU_DATAFRAME:
             return _pandas_to_array(tensors, False), Supports.GPU_DICT_ARRAY
         elif kind == Supports.GPU_DATAFRAME:
             return _cudf_to_array(tensors, False), Supports.GPU_DICT_ARRAY
 
     elif target_kind & Supports.CPU_DICT_ARRAY:
         if kind == Supports.GPU_DICT_ARRAY:
-            return _convert_array(tensors, cp.asnumpy), Supports.CPU_DICT_ARRAY
+            return _convert_array(tensors, xp.asnumpy), Supports.CPU_DICT_ARRAY
         elif kind == Supports.CPU_DATAFRAME:
             return _pandas_to_array(tensors, True), Supports.CPU_DICT_ARRAY
         elif kind == Supports.GPU_DATAFRAME:
             return _cudf_to_array(tensors, True), Supports.CPU_DICT_ARRAY
 
     elif target_kind & Supports.GPU_DATAFRAME:
         if kind == Supports.CPU_DATAFRAME:
@@ -75,15 +73,15 @@
 
     elif target_kind & Supports.CPU_DATAFRAME:
         if kind == Supports.GPU_DATAFRAME:
             return tensors.to_pandas(), Supports.CPU_DATAFRAME
         elif kind == Supports.CPU_DICT_ARRAY:
             return _array_to_pandas(tensors), Supports.CPU_DATAFRAME
         elif kind == Supports.GPU_DICT_ARRAY:
-            return _array_to_pandas(_convert_array(tensors, cp.asnumpy)), Supports.CPU_DATAFRAME
+            return _array_to_pandas(_convert_array(tensors, xp.asnumpy)), Supports.CPU_DATAFRAME
 
     raise ValueError("unsupported target for converting tensors", target_kind)
 
 
 def _convert_array(tensors, converter):
     output = {}
     for name, tensor in tensors.items():
@@ -112,29 +110,29 @@
             output[name] = build_cudf_list_column(tensor[0], tensor[1].astype("int32"))
         else:
             output[name] = tensor
     return output
 
 
 def _pandas_to_array(df, cpu=True):
-    array_type = np.array if cpu else cp.array
+    array_type = np.array if cpu else xp.array
 
     output = {}
     for name in df.columns:
         col = df[name]
         if pd.api.types.is_list_like(col.values[0]):
             offsets = pd.Series([0]).append(col.map(len).cumsum()).values
             if not cpu:
-                offsets = cp.array(offsets)
+                offsets = xp.array(offsets)
             values = array_type(list(itertools.chain(*col)))
             output[name] = (values, offsets)
         else:
             values = col.values
             if not cpu:
-                values = cp.array(values)
+                values = xp.array(values)
             output[name] = values
 
     return output
 
 
 def _cudf_to_array(df, cpu=True):
     output = {}
```

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/ensemble.py` & `nvtabular-23.4.0/nvtabular/inference/triton/ensemble.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/model/__init__.py` & `nvtabular-23.4.0/nvtabular/inference/triton/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/model/model_pt.py` & `nvtabular-23.4.0/nvtabular/inference/triton/model/model_pt.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
                     input_dict[name] = torch.tensor(
                         _convert_tensor(pb_utils.get_input_tensor_by_name(request, name)),
                         dtype=dtype,
                     ).cuda()
 
                 # Sparse inputs have a special format
                 for name, dtype in self.sparse_inputs.items():
-
                     # Get __values and __nnzs
                     input_val = _convert_tensor(
                         pb_utils.get_input_tensor_by_name(request, name + sparse_value_marker)
                     )
                     input_nnzs = _convert_tensor(
                         pb_utils.get_input_tensor_by_name(request, name + sparse_nnzs_marker)
                     )
```

### Comparing `nvtabular-23.2.0/nvtabular/inference/triton/workflow_model.py` & `nvtabular-23.4.0/nvtabular/inference/triton/workflow_model.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/workflow/__init__.py` & `nvtabular-23.4.0/nvtabular/inference/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/workflow/base.py` & `nvtabular-23.4.0/nvtabular/inference/workflow/base.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/workflow/hugectr.py` & `nvtabular-23.4.0/nvtabular/inference/workflow/hugectr.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         rows = max(len(tensors[name]) for name in columns)
         d = self._convert_to_np(columns, tensors, dtype, rows)
         return d.reshape(1, len(columns) * rows)
 
     def get_offsets(self, workflow, categorical_cols):
         embeddings = get_embedding_sizes(workflow)
         if embeddings is None:
-            raise Exception("embeddings cannot be None")
+            raise ValueError("embeddings cannot be None")
         else:
             offsets = {}
             curr_offset = 0
             for name in categorical_cols:
                 offsets[name] = curr_offset
                 curr_offset += embeddings[name][0]
             return offsets
```

### Comparing `nvtabular-23.2.0/nvtabular/inference/workflow/pytorch.py` & `nvtabular-23.4.0/nvtabular/inference/workflow/pytorch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/inference/workflow/tensorflow.py` & `nvtabular-23.4.0/nvtabular/inference/workflow/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/io.py` & `nvtabular-23.4.0/nvtabular/io.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/loader/__init__.py` & `nvtabular-23.4.0/nvtabular/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/loader/backend.py` & `nvtabular-23.4.0/nvtabular/loader/backend.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/loader/tensorflow.py` & `nvtabular-23.4.0/nvtabular/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/loader/tf_utils.py` & `nvtabular-23.4.0/nvtabular/loader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/loader/torch.py` & `nvtabular-23.4.0/nvtabular/loader/torch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/__init__.py` & `nvtabular-23.4.0/nvtabular/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/add_metadata.py` & `nvtabular-23.4.0/nvtabular/ops/add_metadata.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/bucketize.py` & `nvtabular-23.4.0/nvtabular/ops/bucketize.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/categorify.py` & `nvtabular-23.4.0/nvtabular/ops/categorify.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,14 @@
         num_buckets=None,
         vocabs=None,
         max_size=0,
         start_index=0,
         single_table=False,
         cardinality_memory_limit=None,
     ):
-
         # We need to handle three types of encoding here:
         #
         #   (1) Conventional encoding. There are no multi-column groups. So,
         #       each categorical column is separately transformed into a new
         #       "encoded" column (1-to-1).  The unique values are calculated
         #       separately for each column.
         #
@@ -928,15 +927,14 @@
     # Loop over dfs and append to file
     # TODO: For high-cardinality columns, should support
     #       Dask-based to_parquet call here (but would need to
     #       support directory reading within dependent ops)
     n_writes = 0
     for df in dfs:
         if len(df):
-
             if options.on_host and not is_cpu_object(df):
                 # Use pyarrow - df is already a pyarrow table
                 if pwriter is None:
                     pwriter = pq.ParquetWriter(path, df.schema, compression=None)
                 pwriter.write_table(df)
             else:
                 # df is a cudf or pandas DataFrame
@@ -1053,14 +1051,16 @@
             df = _combo_encode(df, name_size_multi, col_selector, options)
         else:
             # Using (default) "joint" encoding
             df = _joint_encode(df, col_selector, options)
 
         df.to_parquet(path, index=False, compression=None)
     else:
+        if hasattr(df, "convert_dtypes"):
+            df = df.convert_dtypes()
         df_null = type(df)({c: [None] for c in col_selector.names})
         for c in col_selector.names:
             df_null[c] = df_null[c].astype(df[c].dtype)
         df_null.to_parquet(path, index=False, compression=None)
 
     del df
     return path
```

### Comparing `nvtabular-23.2.0/nvtabular/ops/clip.py` & `nvtabular-23.4.0/nvtabular/ops/clip.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/column_similarity.py` & `nvtabular-23.4.0/nvtabular/ops/column_similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-try:
-    import cupy
-    import cupy.sparse
-except ImportError:
-    cupy = None
-
 import numba
-import numpy
 import pandas as pd
 import scipy.sparse
 
-try:
-    from cupyx.scipy.sparse import coo_matrix
-except ImportError:
-    from scipy.sparse import coo_matrix
-
+from merlin.core.compat import cuda, cupy, numpy
 from merlin.core.dispatch import DataFrameType, annotate
 from merlin.schema import Schema, Tags
 from nvtabular.ops.operator import ColumnSelector, Operator
 
+if cupy:
+    from cupyx.scipy.sparse import coo_matrix
+else:
+    from scipy.sparse import coo_matrix
+
 
 class ColumnSimilarity(Operator):
     """Calculates the similarity between two columns using tf-idf, cosine or
     inner product as the distance metric. For each row, this calculates the distance
     between the two columns by looking up features for those columns in a sparse matrix,
     and then computing the distance between the rows of the feature matrices.
 
@@ -204,23 +198,25 @@
     # pylint: disable=not-an-iterable
     for i in numba.prange(len(a)):
         output[i] = _inner_product_cpu(
             a[i], a_indptr, a_indices, a_data, b[i], b_indptr, b_indices, b_data
         )
 
 
-@numba.cuda.jit
-def _row_wise_inner_product_gpu(
-    a, a_indptr, a_indices, a_data, b, b_indptr, b_indices, b_data, output
-):
-    i = numba.cuda.grid(1)
-    if i < a.size:
-        output[i] = _inner_product_gpu(
-            a[i], a_indptr, a_indices, a_data, b[i], b_indptr, b_indices, b_data
-        )
+if cuda:
+
+    @numba.cuda.jit
+    def _row_wise_inner_product_gpu(
+        a, a_indptr, a_indices, a_data, b, b_indptr, b_indices, b_data, output
+    ):
+        i = numba.cuda.grid(1)
+        if i < a.size:
+            output[i] = _inner_product_gpu(
+                a[i], a_indptr, a_indices, a_data, b[i], b_indptr, b_indices, b_data
+            )
 
 
 def _inner_product(a, a_indptr, a_indices, a_data, b, b_indptr, b_indices, b_data):
     # adapted from scipy:
     # https://github.com/scipy/scipy/blob/312b706c1d98980ed140adae943d41f9f7dc08f5/scipy/sparse/sparsetools/csr.h#L780-L854
     a_pos, a_end = a_indptr[a], a_indptr[a + 1]
     b_pos, b_end = b_indptr[b], b_indptr[b + 1]
@@ -239,15 +235,15 @@
             b_pos += 1
 
     return similarity
 
 
 # JIT the _inner_product function to run on both CPU/GPU using numba
 _inner_product_cpu = numba.njit(inline="always")(_inner_product)
-_inner_product_gpu = numba.cuda.jit(device=True, inline=True)(_inner_product)
+_inner_product_gpu = numba.cuda.jit(device=True, inline=True)(_inner_product) if cuda else None
 
 
 def _convert_features(features, metric, on_device):
     if on_device:
         # take a shallow copy to avoid mutating the input, but keep gpu
         # memory as low as possible. (also convert to coo_matrix if passed
         # a CSR etc)
```

### Comparing `nvtabular-23.2.0/nvtabular/ops/data_stats.py` & `nvtabular-23.4.0/nvtabular/ops/data_stats.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/difference_lag.py` & `nvtabular-23.4.0/nvtabular/ops/difference_lag.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/drop_low_cardinality.py` & `nvtabular-23.4.0/nvtabular/ops/drop_low_cardinality.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/dropna.py` & `nvtabular-23.4.0/nvtabular/ops/dropna.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/fill.py` & `nvtabular-23.4.0/nvtabular/ops/fill.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/filter.py` & `nvtabular-23.4.0/nvtabular/ops/filter.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/groupby.py` & `nvtabular-23.4.0/nvtabular/ops/groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,14 @@
         for _v in v:
             if isinstance(_v, str):
                 _agg_cols.append(name_sep.join([k, _v]))
     return _agg_cols
 
 
 def _apply_aggs(_df, groupby_cols, _list_aggs, _conv_aggs, name_sep="_", ascending=True):
-
     # Apply conventional aggs
     _columns = list(set(groupby_cols) | set(_conv_aggs) | set(_list_aggs))
     df = _df[_columns].groupby(groupby_cols).agg(_conv_aggs).reset_index()
 
     df.columns = [
         name_sep.join([n for n in name if n != ""]) for name in df.columns.to_flat_index()
     ]
```

### Comparing `nvtabular-23.2.0/nvtabular/ops/hash_bucket.py` & `nvtabular-23.4.0/nvtabular/ops/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/hashed_cross.py` & `nvtabular-23.4.0/nvtabular/ops/hashed_cross.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/join_external.py` & `nvtabular-23.4.0/nvtabular/ops/join_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 
-try:
-    import cudf
-except ImportError:
-    cudf = None
-
 import dask.dataframe as dd
 import pandas as pd
 
+from merlin.core.compat import cudf
 from merlin.core.dispatch import (
     DataFrameType,
     ExtData,
     arange,
     convert_data,
     create_merlin_dataset,
     detect_format,
@@ -115,15 +111,14 @@
             raise ValueError("Only left join is currently supported.")
         if not isinstance(self.kind_ext, ExtData):
             raise ValueError("kind_ext option not recognized.")
         super().__init__()
 
     @property
     def _ext(self):
-
         if self._ext_cache is not None:
             # Return cached result if present
             return convert_data(self._ext_cache, cpu=self.cpu)
 
         # Use Dataset.to_ddf
         _dataset = self.df_ext
         if self.cpu:
```

### Comparing `nvtabular-23.2.0/nvtabular/ops/join_groupby.py` & `nvtabular-23.4.0/nvtabular/ops/join_groupby.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/lambdaop.py` & `nvtabular-23.4.0/nvtabular/ops/lambdaop.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/list_slice.py` & `nvtabular-23.4.0/nvtabular/ops/list_slice.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/logop.py` & `nvtabular-23.4.0/nvtabular/ops/logop.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/moments.py` & `nvtabular-23.4.0/nvtabular/ops/moments.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 
 from merlin.core.dispatch import flatten_list_column_values, is_list_dtype
 
 
 def _custom_moments(ddf, split_every=32):
-
     # Build custom task graph to gather stat moments
     dsk = {}
     token = tokenize(ddf)
     tree_reduce_name = "chunkwise-moments-" + token
     result_name = "global-moments-" + token
     for p in range(ddf.npartitions):
         # Gather necessary statstics on each partition.
@@ -41,15 +40,14 @@
     widths = [parts]
     while parts > 1:
         parts = math.ceil(parts / split_every)
         widths.append(parts)
     height = len(widths)
     for depth in range(1, height):
         for group in range(widths[depth]):
-
             p_max = widths[depth - 1]
             lstart = split_every * group
             lstop = min(lstart + split_every, p_max)
             node_list = [(tree_reduce_name, p, depth - 1) for p in range(lstart, lstop)]
 
             dsk[(tree_reduce_name, group, depth)] = (
                 _tree_node_moments,
```

### Comparing `nvtabular-23.2.0/nvtabular/ops/normalize.py` & `nvtabular-23.4.0/nvtabular/ops/normalize.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/operator.py` & `nvtabular-23.4.0/nvtabular/ops/operator.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/reduce_dtype_size.py` & `nvtabular-23.4.0/nvtabular/ops/reduce_dtype_size.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/rename.py` & `nvtabular-23.4.0/nvtabular/ops/rename.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/stat_operator.py` & `nvtabular-23.4.0/nvtabular/ops/stat_operator.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/target_encoding.py` & `nvtabular-23.4.0/nvtabular/ops/target_encoding.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/ops/value_counts.py` & `nvtabular-23.4.0/nvtabular/ops/value_counts.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/tools/__init__.py` & `nvtabular-23.4.0/nvtabular/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/tools/data_gen.py` & `nvtabular-23.4.0/nvtabular/tools/data_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,33 @@
 #
 
 import os
 import random
 import string
 
 import numpy as np
-import pandas as pd
 import psutil
-
-try:
-    import cupy
-except ImportError:
-    cupy = np
-
-try:
-    import cudf
-except ImportError:
-    cudf = pd
-
 from scipy import stats
 from scipy.stats import powerlaw, uniform
 
+from merlin.core.compat import cupy
 from merlin.core.dispatch import (
     HAS_GPU,
     concat,
     create_multihot_col,
     is_list_dtype,
     make_df,
     make_series,
     pull_apart_list,
 )
 from merlin.core.utils import device_mem_size
 from merlin.io import Dataset
 
+xp = cupy or np
+
 
 class UniformDistro:
     def create_col(self, num_rows, dtype=np.float32, min_val=0, max_val=1):
         ser = make_df(np.random.uniform(min_val, max_val, size=num_rows))[0]
         ser = ser.astype(dtype)
         return ser
 
@@ -60,17 +51,17 @@
 class PowerLawDistro:
     def __init__(self, alpha=0.1):
         self.alpha = alpha
 
     def create_col(self, num_rows, dtype=np.float32, min_val=0, max_val=1):
         gamma = 1 - self.alpha
         # range 1.0 - 2.0 to avoid using 0, which represents unknown, null, None
-        ser = make_df(cupy.random.uniform(0.0, 1.0, size=num_rows))[0]
-        factor = cupy.power(max_val, gamma) - cupy.power(min_val, gamma)
-        ser = (ser * factor.item()) + cupy.power(min_val, gamma).item()
+        ser = make_df(xp.random.uniform(0.0, 1.0, size=num_rows))[0]
+        factor = xp.power(max_val, gamma) - xp.power(min_val, gamma)
+        ser = (ser * factor.item()) + xp.power(min_val, gamma).item()
         exp = 1.0 / gamma
         ser = ser.pow(exp)
         # replace zeroes saved for unknown
         # add in nulls if requested
         # select indexes
         return ser.astype(dtype)
 
@@ -122,22 +113,24 @@
             ser = None
             if col.multi_min and col.multi_max:
                 if HAS_GPU:
                     ser = dist.create_col(
                         col_size + 1, dtype=np.long, min_val=col.multi_min, max_val=col.multi_max
                     )
                     ser = make_series(np.ceil(ser)).astype(ser.dtype)
+                    _cumsum = xp.cumsum
                 else:
                     ser = dist.create_col(
                         col_size + 1, dtype=np.long, min_val=col.multi_min, max_val=col.multi_max
                     )
                     ser = make_df(np.ceil(ser))[0]
+                    _cumsum = np.cumsum
                 # sum returns numpy dtype
                 col_size = int(ser.sum())
-                offs = make_df(cupy.cumsum(ser.values))[0]
+                offs = make_df(_cumsum(ser.values))[0]
                 offs = offs.astype("int32")
             if HAS_GPU:
                 ser = dist.create_col(
                     col_size, dtype=np.long, min_val=col.min_val, max_val=col.cardinality
                 )
                 ser = make_series(np.ceil(ser)).astype(ser.dtype)
             else:
@@ -370,18 +363,18 @@
                 return rep
         return None
 
     def permutate_index(self, ser):
         name = ser.name
         ser.name = "ind"
         ind = ser.drop_duplicates().values
-        ind_random = cupy.random.permutation(ind)
-        df_map = cudf.DataFrame({"ind": ind, "ind_random": ind_random})
+        ind_random = xp.random.permutation(ind)
+        df_map = make_df({"ind": ind, "ind_random": ind_random})
         if not HAS_GPU:
-            ser = cudf.DataFrame(ser)
+            ser = make_df(ser)
         ser = ser.merge(df_map, how="left", left_on="ind", right_on="ind")["ind_random"]
         ser.name = name
         return ser
 
 
 DISTRO_TYPES = {"powerlaw": PowerLawDistro, "uniform": UniformDistro}
```

### Comparing `nvtabular-23.2.0/nvtabular/tools/dataset_inspector.py` & `nvtabular-23.4.0/nvtabular/tools/dataset_inspector.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/tools/inspector_script.py` & `nvtabular-23.4.0/nvtabular/tools/inspector_script.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/utils.py` & `nvtabular-23.4.0/nvtabular/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 # pylint: disable=wildcard-import,unused-import,unused-wildcard-import
 import warnings
 
 # Re-export classes/modules from the core library for backwards compatibility
-from merlin.core.utils import *  # noqa
+from merlin.core.compat import *  # noqa
 
 warnings.warn(
     "The `nvtabular.utils` module has moved to `merlin.core.utils`. "
     "Support for importing from `nvtabular.utils` is deprecated, "
     "and will be removed in a future version. Please update "
     "your imports to refer to `merlin.core.utils`.",
     DeprecationWarning,
```

### Comparing `nvtabular-23.2.0/nvtabular/worker.py` & `nvtabular-23.4.0/nvtabular/worker.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/workflow/__init__.py` & `nvtabular-23.4.0/nvtabular/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/workflow/node.py` & `nvtabular-23.4.0/nvtabular/workflow/node.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/nvtabular/workflow/workflow.py` & `nvtabular-23.4.0/nvtabular/workflow/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,25 +17,22 @@
 import inspect
 import json
 import logging
 import sys
 import time
 import types
 import warnings
+from functools import singledispatchmethod
 from typing import TYPE_CHECKING, Optional
 
 import cloudpickle
 import fsspec
-
-try:
-    import cudf
-except ImportError:
-    cudf = None
 import pandas as pd
 
+from merlin.core.compat import cudf
 from merlin.dag import Graph
 from merlin.dag.executors import DaskExecutor, LocalExecutor
 from merlin.dag.node import iter_nodes
 from merlin.io import Dataset
 from merlin.schema import Schema
 from nvtabular.ops import LambdaOp, StatOperator
 from nvtabular.workflow.node import WorkflowNode
@@ -74,36 +71,65 @@
         The last node in the graph of operators this workflow should apply
     """
 
     def __init__(self, output_node: WorkflowNode, client: Optional["distributed.Client"] = None):
         self.graph = Graph(output_node)
         self.executor = DaskExecutor(client)
 
-    def transform(self, dataset: Dataset) -> Dataset:
-        """Transforms the dataset by applying the graph of operators to it. Requires the ``fit``
-        method to have already been called, or calculated statistics to be loaded from disk
-
-        This method returns a Dataset object, with the transformations lazily loaded. None
-        of the actual computation will happen until the produced Dataset is consumed, or
-        written out to disk.
+    @singledispatchmethod
+    def transform(self, data):
+        """Transforms the data by applying the graph of operators to it.
+
+        Requires the ``fit`` method to have already been called, or
+        using a Workflow that has already beeen fit and re-loaded from
+        disk (using the ``load`` method).
+
+        This method returns data of the same type.
+
+        In the case of a `Dataset`. The computation is lazy. It won't
+        happen until the produced Dataset is consumed, or written out
+        to disk. e.g. with a `dataset.compute()`.
 
         Parameters
         -----------
-        dataset: Dataset
-            Input dataset to transform
+        data: Union[Dataset, DataFrameType]
+            Input Dataset or DataFrame to transform
 
         Returns
         -------
-        Dataset
-            Transformed Dataset with the workflow graph applied to it
+        Dataset or DataFrame
+            Transformed Dataset or DataFrame with the workflow graph applied to it
+
+        Raises
+        ------
+        NotImplementedError
+            If passed an unsupoprted data type to transform.
+
         """
+        raise NotImplementedError(
+            f"Workflow.transform received an unsupported type: {type(data)} "
+            "Supported types are a `merlin.io.Dataset` or DataFrame (pandas or cudf)"
+        )
+
+    @transform.register
+    def _(self, dataset: Dataset) -> Dataset:
         return self._transform_impl(dataset)
 
+    @transform.register
+    def _(self, dataframe: pd.DataFrame) -> pd.DataFrame:
+        return self._transform_df(dataframe)
+
+    if cudf:
+
+        @transform.register
+        def _(self, dataframe: cudf.DataFrame) -> cudf.DataFrame:
+            return self._transform_df(dataframe)
+
     def fit_schema(self, input_schema: Schema):
-        """Fits the schema onto the workflow, computing the Schema for each node in the Workflow Graph
+        """Computes input and output schemas for each node in the Workflow graph
 
         Parameters
         ----------
         input_schema : Schema
             The input schema to use
 
         Returns
```

### Comparing `nvtabular-23.2.0/nvtabular.egg-info/PKG-INFO` & `nvtabular-23.4.0/nvtabular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nvtabular-23.2.0/nvtabular.egg-info/SOURCES.txt` & `nvtabular-23.4.0/nvtabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/pyproject.toml` & `nvtabular-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/requirements/test.txt` & `nvtabular-23.4.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/setup.cfg` & `nvtabular-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/setup.py` & `nvtabular-23.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.2.0/versioneer.py` & `nvtabular-23.4.0/versioneer.py`

 * *Files identical despite different names*

