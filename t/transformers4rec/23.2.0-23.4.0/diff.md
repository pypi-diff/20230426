# Comparing `tmp/transformers4rec-23.2.0.tar.gz` & `tmp/transformers4rec-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers4rec-23.2.0.tar", last modified: Wed Mar  8 16:31:50 2023, max compression
+gzip compressed data, was "transformers4rec-23.4.0.tar", last modified: Wed Apr 26 21:12:08 2023, max compression
```

## Comparing `transformers4rec-23.2.0.tar` & `transformers4rec-23.4.0.tar`

### file list

```diff
@@ -1,191 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.723504 transformers4rec-23.2.0/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    60300 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/DP_DDP_perf.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/nlp_x_recsys.png
--rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/preproc_data_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/sequential_rec.png
--rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/_images/transformers4rec_metaarchitecture.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.727504 transformers4rec-23.2.0/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.727504 transformers4rec-23.2.0/merlin_standard_lib/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/proto/schema_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/schema/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/merlin_standard_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/utils/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/utils/embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/merlin_standard_lib/utils/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/dataloader.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/tests/assets/data_schema/
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/assets/data_schema/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/assets/data_schema/data_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/assets/data_schema/data_seq.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/assets/data_schema/data_seq_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/assets/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/config/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/config/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/config/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.731504 transformers4rec-23.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.735504 transformers4rec-23.2.0/tests/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.735504 transformers4rec-23.2.0/tests/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/testing/tabular_data/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/data/testing/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.739504 transformers4rec-23.2.0/tests/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.739504 transformers4rec-23.2.0/tests/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/merlin_standard_lib/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/merlin_standard_lib/schema/test_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.743504 transformers4rec-23.2.0/tests/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.743504 transformers4rec-23.2.0/tests/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/block/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/block/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/block/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/features/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/features/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/features/test_sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/features/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/model/test_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/model/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/tabular/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/tabular/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/tabular/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_dataloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_ranking_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/torch/utils/test_schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/unit/test_getting_started_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/unit/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.747504 transformers4rec-23.2.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/transformers4rec/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/transformers4rec/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.751504 transformers4rec-23.2.0/transformers4rec/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/config/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/config/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.755504 transformers4rec-23.2.0/transformers4rec/data/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.755504 transformers4rec-23.2.0/transformers4rec/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.759504 transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.759504 transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/data/yoochoose.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.763504 transformers4rec-23.2.0/transformers4rec/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.763504 transformers4rec-23.2.0/transformers4rec/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/block/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/block/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/block/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.771504 transformers4rec-23.2.0/transformers4rec/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/features/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35957 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/masking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.771504 transformers4rec-23.2.0/transformers4rec/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29443 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17068 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/model/prediction_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/ranking_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.771504 transformers4rec-23.2.0/transformers4rec/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/tabular/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/tabular/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/tabular/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    34011 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/transformers4rec/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/utils/examples_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/utils/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/torch/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.775504 transformers4rec-23.2.0/transformers4rec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/transformers4rec/utils/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:31:50.751504 transformers4rec-23.2.0/transformers4rec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-03-08 16:31:50.000000 transformers4rec-23.2.0/transformers4rec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-03-08 16:31:50.000000 transformers4rec-23.2.0/transformers4rec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:31:50.000000 transformers4rec-23.2.0/transformers4rec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-08 16:31:50.000000 transformers4rec-23.2.0/transformers4rec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-08 16:31:50.000000 transformers4rec-23.2.0/transformers4rec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-03-08 16:24:31.000000 transformers4rec-23.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    60445 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/DP_DDP_perf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/nlp_x_recsys.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/preproc_data_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/sequential_rec.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/transformers4rec_metaarchitecture.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/proto/schema_bp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/utils/embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/base_external.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/base_merlin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.621868 transformers4rec-23.4.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/integration/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/integration/notebooks/test_getting_started_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/integration/notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/assets/data_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/test_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_dataloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_ranking_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/test_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/yoochoose.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35959 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/masking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30310 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/prediction_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/ranking_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35065 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/examples_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/versioneer.py
```

### Comparing `transformers4rec-23.2.0/.pre-commit-config.yaml` & `transformers4rec-23.4.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 repos:
       - repo: https://github.com/timothycrosley/isort
-        rev: 5.10.1
+        rev: 5.12.0
         hooks:
         - id: isort
           additional_dependencies: [toml]
       - repo: https://github.com/python/black
-        rev: 22.8.0
+        rev: 23.1.0
         hooks:
         - id: black
       - repo: https://github.com/pycqa/flake8
-        rev: 3.9.2
+        rev: 6.0.0
         hooks:
         - id: flake8
       - repo: https://github.com/pre-commit/mirrors-mypy
-        rev: 'v0.991'
+        rev: 'v1.0.1'
         hooks:
           - id: mypy
             language_version: python3
             args: [--non-interactive, --install-types]
       - repo: https://github.com/codespell-project/codespell
-        rev: v2.2.1
+        rev: v2.2.2
         hooks:
         - id: codespell
 #      - repo: https://github.com/mgedmin/check-manifest
 #        rev: "0.46"
 #        hooks:
 #          - id: check-manifest
 #            args: [--ignore, "*source*"]
```

### Comparing `transformers4rec-23.2.0/CLA.md` & `transformers4rec-23.4.0/CLA.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/CONTRIBUTING.md` & `transformers4rec-23.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/LICENSE` & `transformers4rec-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/MANIFEST.in` & `transformers4rec-23.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/PKG-INFO` & `transformers4rec-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers4rec
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: pytorch
 Provides-Extra: nvtabular
-Provides-Extra: dataloader
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
```

### Comparing `transformers4rec-23.2.0/README.md` & `transformers4rec-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/_images/nlp_x_recsys.png` & `transformers4rec-23.4.0/_images/nlp_x_recsys.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/_images/pipeline.png` & `transformers4rec-23.4.0/_images/pipeline.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/_images/preproc_data_example.png` & `transformers4rec-23.4.0/_images/preproc_data_example.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/_images/sequential_rec.png` & `transformers4rec-23.4.0/_images/sequential_rec.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/_images/transformers4rec_metaarchitecture.png` & `transformers4rec-23.4.0/_images/transformers4rec_metaarchitecture.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/proto/__init__.py` & `transformers4rec-23.4.0/merlin_standard_lib/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/proto/schema_bp.py` & `transformers4rec-23.4.0/merlin_standard_lib/proto/schema_bp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.4.0/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/schema/schema.py` & `transformers4rec-23.4.0/merlin_standard_lib/schema/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,32 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-
 import collections
+import json
 import os
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, TypeVar, Union
 
-from ..utils import proto_utils
-from .tag import TagsType
+from google.protobuf import json_format, text_format
+from google.protobuf.message import Message as ProtoMessage
+from merlin.models.utils import schema_utils as mm_schema_utils
+from merlin.schema import Schema as CoreSchema
+from merlin.schema import Tags, TagSet, TagsType
+from merlin.schema.io import proto_utils
 
 try:
     from functools import cached_property  # type: ignore
 except ImportError:
     # polyfill cached_property for python <= 3.7 (using lru_cache which was introduced in python3.2)
     from functools import lru_cache
 
     cached_property = lambda func: property(lru_cache()(func))  # type: ignore  # noqa
 
 import betterproto  # noqa
+from betterproto import Message as BetterProtoMessage
 
 from ..proto.schema_bp import *  # noqa
 from ..proto.schema_bp import (
     Annotation,
     Feature,
     FeatureType,
     FixedShape,
@@ -41,14 +45,16 @@
     FloatDomain,
     IntDomain,
     ValueCount,
     ValueCountList,
     _Schema,
 )
 
+ProtoMessageType = TypeVar("ProtoMessageType", bound=BetterProtoMessage)
+
 
 def _parse_shape_and_value_count(shape, value_count) -> Dict[str, Any]:
     output: Dict[str, Union[ValueCount, ValueCountList, FixedShape]] = {}
     if shape:
         output["shape"] = FixedShape([FixedShapeDim(d) for d in shape])
 
     if value_count:
@@ -70,19 +76,19 @@
         num_items: int,
         shape: Optional[Union[Tuple[int, ...], List[int]]] = None,
         value_count: Optional[Union[ValueCount, ValueCountList]] = None,
         min_index: int = 0,
         tags: Optional[TagsType] = None,
         **kwargs,
     ) -> "ColumnSchema":
-        _tags: List[str] = [str(t) for t in tags] if tags else []
+        _tags: List[str] = [t.value for t in TagSet(tags or [])]
 
         extra = _parse_shape_and_value_count(shape, value_count)
         int_domain = IntDomain(name=name, min=min_index, max=num_items, is_categorical=True)
-        _tags = list(set(_tags + ["categorical"]))
+        _tags = list(set(_tags + [Tags.CATEGORICAL.value]))
         extra["type"] = FeatureType.INT
 
         return cls(name=name, int_domain=int_domain, **extra, **kwargs).with_tags(_tags)
 
     @classmethod
     def create_continuous(
         cls,
@@ -94,15 +100,15 @@
         disallow_inf: bool = False,
         is_embedding: bool = False,
         shape: Optional[Union[Tuple[int, ...], List[int]]] = None,
         value_count: Optional[Union[ValueCount, ValueCountList]] = None,
         tags: Optional[TagsType] = None,
         **kwargs,
     ) -> "ColumnSchema":
-        _tags: List[str] = [str(t) for t in tags] if tags else []
+        _tags: List[str] = [t.value for t in TagSet(tags or [])]
 
         extra = _parse_shape_and_value_count(shape, value_count)
         if min_value is not None and max_value is not None:
             if is_float:
                 extra["float_domain"] = FloatDomain(
                     name=name,
                     min=float(min_value),
@@ -112,15 +118,15 @@
                     is_embedding=is_embedding,
                 )
             else:
                 extra["int_domain"] = IntDomain(
                     name=name, min=int(min_value), max=int(max_value), is_categorical=False
                 )
         extra["type"] = FeatureType.FLOAT if is_float else FeatureType.INT
-        _tags = list(set(_tags + ["continuous"]))
+        _tags = list(set(_tags + [Tags.CONTINUOUS.value]))
 
         return cls(name=name, **extra, **kwargs).with_tags(_tags)
 
     def copy(self, **kwargs) -> "ColumnSchema":
         return proto_utils.copy_better_proto_message(self, **kwargs)
 
     def with_name(self, name: str):
@@ -135,29 +141,27 @@
             output.annotation = Annotation(tag=tags)
 
         return output
 
     def with_tags_based_on_properties(
         self, using_value_count=True, using_domain=True
     ) -> "ColumnSchema":
-        from .tag import Tag
-
         extra_tags = []
 
         if using_value_count and proto_utils.has_field(self, "value_count"):
-            extra_tags.append(str(Tag.LIST))
+            extra_tags.append(str(Tags.LIST))
 
         if using_domain and proto_utils.has_field(self, "int_domain"):
             if self.int_domain.is_categorical:
-                extra_tags.append(str(Tag.CATEGORICAL))
+                extra_tags.append(str(Tags.CATEGORICAL))
             else:
-                extra_tags.append(str(Tag.CONTINUOUS))
+                extra_tags.append(str(Tags.CONTINUOUS))
 
         if using_domain and proto_utils.has_field(self, "float_domain"):
-            extra_tags.append(str(Tag.CONTINUOUS))
+            extra_tags.append(str(Tags.CONTINUOUS))
 
         return self.with_tags(extra_tags) if extra_tags else self.copy()
 
     def with_properties(self, properties: Dict[str, Union[str, int, float]]) -> "ColumnSchema":
         output = self.copy()
         if output.annotation:
             if len(output.annotation.extra_metadata) > 0:
@@ -297,22 +301,25 @@
 
         return output
 
     def select_by_tag(self, to_select) -> "Schema":
         if not isinstance(to_select, (list, tuple)) and not callable(to_select):
             to_select = [to_select]
 
-        def collection_filter_fn(column_tags):
-            return all(x in column_tags for x in to_select)
+        if callable(to_select):
+            return self._filter_column_schemas(to_select, lambda x: False, lambda x: x.tags)
+        else:
+            # Schema.tags always returns a List[str] with the tag values, so if the user wants to
+            # filter using the Tags Enum, we need to convert those to their string value
+            to_select = [tag.value if isinstance(tag, Tags) else tag for tag in to_select]
 
-        output: Schema = self._filter_column_schemas(
-            to_select, collection_filter_fn, lambda x: x.tags
-        )
+            def collection_filter_fn(column_names: List[str]):
+                return all(x in column_names for x in to_select)
 
-        return output
+            return self._filter_column_schemas(to_select, collection_filter_fn, lambda x: x.tags)
 
     def remove_by_tag(self, to_remove) -> "Schema":
         if not isinstance(to_remove, (list, tuple)) and not callable(to_remove):
             to_remove = [to_remove]
 
         def collection_filter_fn(column_tags):
             return all(x in column_tags for x in to_remove)
@@ -358,33 +365,25 @@
         selected_schemas = []
         for column_schema in self.column_schemas:
             if self._check_column_schema(column_schema, filter_fn, negate=negate):
                 selected_schemas.append(column_schema)
 
         return Schema(selected_schemas)
 
-    def categorical_cardinalities(self) -> Dict[str, int]:
-        outputs = {}
-        for col in self:
-            if col.int_domain and col.int_domain.is_categorical:
-                outputs[col.name] = col.int_domain.max + 1
-
-        return outputs
-
     @property
     def column_names(self) -> List[str]:
         return [f.name for f in self.feature]
 
     @property
     def column_schemas(self) -> Sequence[ColumnSchema]:
         return self.feature
 
     @cached_property
     def item_id_column_name(self):
-        item_id_col = self.select_by_tag("item_id")
+        item_id_col = self.select_by_tag(Tags.ITEM_ID)
         if len(item_id_col.column_names) == 0:
             raise ValueError("There is no column tagged as item id.")
 
         return item_id_col.column_names[0]
 
     def from_json(self, value: Union[str, bytes]) -> "Schema":
         if os.path.isfile(value):
@@ -397,15 +396,15 @@
         from tensorflow_metadata.proto.v0 import schema_pb2
 
         return proto_utils.better_proto_to_proto_text(self, schema_pb2.Schema())
 
     def from_proto_text(self, path_or_proto_text: str) -> "Schema":
         from tensorflow_metadata.proto.v0 import schema_pb2
 
-        return proto_utils.proto_text_to_better_proto(self, path_or_proto_text, schema_pb2.Schema())
+        return _proto_text_to_better_proto(self, path_or_proto_text, schema_pb2.Schema())
 
     def copy(self, **kwargs) -> "Schema":
         return proto_utils.copy_better_proto_message(self, **kwargs)
 
     def add(self, other, allow_overlap=True) -> "Schema":
         if isinstance(other, str):
             other = Schema.create([other])
@@ -504,7 +503,41 @@
         result = Schema(self.column_schemas)
 
         for key in other.column_schemas:
             if key in self.column_schemas:
                 result.column_schemas.pop(key, None)
 
         return result
+
+
+def _proto_text_to_better_proto(
+    better_proto_message: ProtoMessageType, path_proto_text: str, message: ProtoMessage
+) -> ProtoMessageType:
+    proto_text = path_proto_text
+    if os.path.isfile(proto_text):
+        with open(path_proto_text, "r") as f:
+            proto_text = f.read()
+
+    proto = text_format.Parse(proto_text, message)
+
+    # This is a hack because as of now we can't parse the Any representation.
+    # TODO: Fix this.
+    d = json_format.MessageToDict(proto)
+    for f in d["feature"]:
+        if "extraMetadata" in f["annotation"]:  # type: ignore
+            extra_metadata = f["annotation"].pop("extraMetadata")  # type: ignore
+            f["annotation"]["comment"] = [json.dumps(extra_metadata[0]["value"])]  # type: ignore
+    json_str = json_format.MessageToJson(json_format.ParseDict(d, message))
+
+    return better_proto_message.__class__().from_json(json_str)
+
+
+def categorical_cardinalities(schema) -> Dict[str, int]:
+    if isinstance(schema, CoreSchema):
+        return mm_schema_utils.categorical_cardinalities(schema)
+
+    outputs = {}
+    for col in schema:
+        if col.int_domain and col.int_domain.is_categorical:
+            outputs[col.name] = col.int_domain.max + 1
+
+    return outputs
```

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/utils/__init__.py` & `transformers4rec-23.4.0/merlin_standard_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/merlin_standard_lib/utils/embedding_utils.py` & `transformers4rec-23.4.0/merlin_standard_lib/utils/embedding_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import math
 
-from merlin_standard_lib import Schema
+from merlin_standard_lib import Schema, categorical_cardinalities
 
 
 def get_embedding_sizes_from_schema(schema: Schema, multiplier: float = 2.0):
-    cardinalities = schema.categorical_cardinalities()
+    cardinalities = categorical_cardinalities(schema)
 
     return {
         key: get_embedding_size_from_cardinality(val, multiplier)
         for key, val in cardinalities.items()
     }
```

### Comparing `transformers4rec-23.2.0/mypy.ini` & `transformers4rec-23.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/setup.cfg` & `transformers4rec-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/setup.py` & `transformers4rec-23.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 def read_requirements(filename):
     base = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(base, filename), "rb", "utf-8") as f:
         lineiter = (line.strip() for line in f)
         return [line for line in lineiter if line and not line.startswith("#")]
 
 
+base = read_requirements("requirements/base_external.txt")
+base += read_requirements("requirements/base_merlin.txt")
+
 requirements = {
-    "base": read_requirements("requirements/base.txt"),
+    "base": base,
     "pytorch": read_requirements("requirements/pytorch.txt"),
     "nvtabular": read_requirements("requirements/nvtabular.txt"),
-    "dataloader": read_requirements("requirements/dataloader.txt"),
     "docs": read_requirements("requirements/docs.txt"),
     "dev": read_requirements("requirements/dev.txt"),
 }
 
 setup(
     name="transformers4rec",
     version=versioneer.get_version(),
```

### Comparing `transformers4rec-23.2.0/tests/__init__.py` & `transformers4rec-23.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/assets/data_schema/data.parquet` & `transformers4rec-23.4.0/tests/unit/assets/data_schema/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/assets/data_schema/data_schema.pbtxt` & `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/assets/data_schema/data_seq.parquet` & `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/assets/data_schema/data_seq_schema.pbtxt` & `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/assets/schema.pbtxt` & `transformers4rec-23.4.0/tests/unit/assets/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/config/__init__.py` & `transformers4rec-23.4.0/tests/unit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/config/test_schema.py` & `transformers4rec-23.4.0/tests/unit/config/test_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,46 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import pytest
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag
+from merlin_standard_lib import categorical_cardinalities
 from merlin_standard_lib.utils.embedding_utils import get_embedding_sizes_from_schema
 
 
 def test_schema_from_yoochoose_schema(yoochoose_schema):
     assert len(yoochoose_schema.column_names) == 22
-    assert len(yoochoose_schema.select_by_tag(Tag.CONTINUOUS).column_schemas) == 11
-    assert len(yoochoose_schema.select_by_tag(Tag.CATEGORICAL).column_schemas) == 3
+    assert len(yoochoose_schema.select_by_tag(Tags.CONTINUOUS).column_schemas) == 11
+    assert len(yoochoose_schema.select_by_tag(Tags.CATEGORICAL).column_schemas) == 3
 
 
 def test_schema_cardinalities(yoochoose_schema):
     schema = yoochoose_schema
-    assert schema.categorical_cardinalities() == {
+    assert categorical_cardinalities(schema) == {
         "item_id/list": schema.select_by_name("item_id/list").feature[0].int_domain.max + 1,
         "category/list": schema.select_by_name("category/list").feature[0].int_domain.max + 1,
         "user_country": schema.select_by_name("user_country").feature[0].int_domain.max + 1,
     }
 
 
 @pytest.mark.xfail
 def test_schema_embedding_sizes_nvt(yoochoose_schema):
     pytest.importorskip("nvtabular")
     schema = yoochoose_schema
-    assert schema.categorical_cardinalities() == {"item_id/list": 51996, "category/list": 332}
+    assert categorical_cardinalities(schema) == {"item_id/list": 51996, "category/list": 332}
     embedding_sizes = schema.embedding_sizes_nvt(minimum_size=16, maximum_size=512)
     assert embedding_sizes == {"item_id/list": 512, "category/list": 41, "user_country": 16}
 
 
 def test_schema_embedding_sizes(yoochoose_schema):
     schema = yoochoose_schema.remove_by_name("session_id")
 
-    assert schema.categorical_cardinalities() == {
+    assert categorical_cardinalities(schema) == {
         "category/list": 333,
         "item_id/list": 51997,
         "user_country": 63,
     }
     embedding_sizes = get_embedding_sizes_from_schema(schema, multiplier=3.0)
     assert embedding_sizes == {"item_id/list": 46, "category/list": 13, "user_country": 9}
```

### Comparing `transformers4rec-23.2.0/tests/config/test_trainer.py` & `transformers4rec-23.4.0/tests/unit/config/test_trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/config/test_transformer.py` & `transformers4rec-23.4.0/tests/unit/config/test_transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/conftest.py` & `transformers4rec-23.4.0/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,26 +12,43 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from __future__ import absolute_import
 
-import importlib
 from pathlib import Path
 
+import numpy as np
 import pytest
+from merlin.datasets.synthetic import generate_data
+from merlin.io import Dataset
+from merlin.schema.io.tensorflow_metadata import TensorflowMetadata
 
 from merlin_standard_lib import Schema
 from transformers4rec.data import tabular_sequence_testing_data, tabular_testing_data
 
 REPO_ROOT = Path(__file__).parent.parent
 
 
 @pytest.fixture
+def ecommerce_data() -> Dataset:
+    np.random.seed(0)
+    return generate_data("e-commerce", num_rows=100)
+
+
+@pytest.fixture
+def testing_data() -> Dataset:
+    data = generate_data("testing", num_rows=100)
+    data.schema = data.schema.without(["session_id", "session_start", "day_idx"])
+
+    return data
+
+
+@pytest.fixture
 def yoochoose_path_file() -> str:
     return tabular_sequence_testing_data.path
 
 
 @pytest.fixture
 def yoochoose_schema_file() -> str:
     return tabular_sequence_testing_data.schema_path
@@ -53,10 +70,38 @@
 
 
 @pytest.fixture
 def tabular_schema() -> Schema:
     return tabular_testing_data.schema.remove_by_name(["session_id", "session_start", "day_idx"])
 
 
-torch = importlib.util.find_spec("torch")
-if torch is not None:
-    from tests.torch.conftest import *  # noqa
+@pytest.fixture
+def tabular_core_schema(tabular_schema):
+    return TensorflowMetadata.from_json(tabular_schema.to_json()).to_merlin_schema()
+
+
+def parametrize_schemas(name):
+    if name == "tabular":
+        schema = tabular_testing_data.schema.remove_by_name(
+            ["session_id", "session_start", "day_idx"]
+        )
+    elif name == "yoochoose":
+        schema = tabular_sequence_testing_data.schema
+
+    return pytest.mark.parametrize(
+        "schema",
+        [
+            pytest.param(schema, id="merlin-standard-lib"),
+            pytest.param(
+                TensorflowMetadata.from_json(schema.to_json()).to_merlin_schema(),
+                id="merlin-core",
+            ),
+        ],
+    )
+
+
+try:
+    import torchmetrics  # noqa
+
+    from tests.unit.torch._conftest import *  # noqa
+except ModuleNotFoundError:
+    pass
```

### Comparing `transformers4rec-23.2.0/tests/data/test_preprocessing.py` & `transformers4rec-23.4.0/tests/unit/utils/test_data_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import numpy as np
-import pytest
 
-from merlin_standard_lib import ColumnSchema, Schema, Tag
-from transformers4rec.data import preprocessing
-from transformers4rec.data.synthetic import (
-    generate_item_interactions,
-    synthetic_ecommerce_data_schema,
-)
+from transformers4rec.utils import data_utils
 
-pd = pytest.importorskip("pandas")
+np.random.seed(0)
 
 
-def test_remove_consecutive_interactions():
-    np.random.seed(0)
+def test_remove_consecutive_interactions(testing_data):
+    df = testing_data.compute()
+    df["session_id"] = np.random.randint(0, 3, len(df))
 
-    schema = synthetic_ecommerce_data_schema.remove_by_name("item_recency")
-    schema += Schema([ColumnSchema.create_continuous("timestamp", tags=[Tag.SESSION])])
+    # generate repeated interactions
+    repeated = 3
+    rows = []
+    for _ in range(repeated):
+        new_row = [123, 42, 0.151773, 10, -2.336, 0.819, 0.025, 0.944, 0.051, [2, 3, 12], 0, 1]
+        rows.append(new_row)
+    to_add = type(df)(rows, columns=df.columns)
+    df = df.append(to_add, ignore_index=True)
 
-    interactions_df = generate_item_interactions(500, schema)
-    filtered_df = preprocessing.remove_consecutive_interactions(interactions_df.copy())
+    filtered = data_utils.remove_consecutive_interactions(
+        df.copy(), timestamp_col="event_timestamp"
+    )
 
-    assert len(filtered_df) < len(interactions_df)
-    assert len(filtered_df) == 499
-    assert len(list(filtered_df.columns)) == len(list(interactions_df.columns))
+    assert len(filtered) < len(df)
+    assert len(list(filtered.columns)) == len(list(df.columns))
 
 
-def test_add_item_first_seen_col_to_df():
-    schema = synthetic_ecommerce_data_schema.remove_by_name("item_recency")
-    schema += Schema([ColumnSchema.create_continuous("timestamp", tags=[Tag.SESSION])])
+def test_add_item_first_seen_col_to_df(testing_data):
+    df = data_utils.add_item_first_seen_col_to_df(
+        testing_data.compute(), timestamp_column="event_timestamp"
+    )
 
-    df = preprocessing.add_item_first_seen_col_to_df(generate_item_interactions(500, schema))
-
-    assert len(list(df.columns)) == len(schema) + 1
-    assert isinstance(df["item_ts_first"], pd.Series)
+    assert len(list(df.columns)) == len(testing_data.schema) + 1
+    assert len(df["item_ts_first"]) == 100
+    assert str(df["item_ts_first"].dtype) == "int64"
 
 
 # TODO: Add test for session_aggregator when nvtabular 21.09 is released
```

### Comparing `transformers4rec-23.2.0/tests/data/test_synthetic.py` & `transformers4rec-23.4.0/tests/unit/data/test_synthetic.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 
 
 def test_generate_item_interactions():
     data = generate_item_interactions(500, synthetic_ecommerce_data_schema)
 
     assert isinstance(data, pd.DataFrame)
     assert len(data) == 500
-    assert list(data.columns) == [
-        "session_id",
-        "item_id",
-        "day",
-        "purchase",
-        "price",
-        "category",
-        "item_recency",
-    ]
+    print(sorted(list(data.columns)))
+    assert sorted(list(data.columns)) == sorted(
+        [
+            "session_id",
+            "item_id",
+            "day",
+            "purchase",
+            "price",
+            "category",
+            "item_recency",
+        ]
+    )
     expected_dtypes = {
         "session_id": "int64",
         "item_id": "int64",
         "day": "int64",
         "purchase": "int64",
         "price": "float64",
         "category": "int64",
         "item_recency": "float64",
     }
-
-    assert all(val == expected_dtypes[key] for key, val in dict(data.dtypes).items())
+    for key, val in dict(data.dtypes).items():
+        assert val == expected_dtypes[key]
```

### Comparing `transformers4rec-23.2.0/tests/data/testing/tabular_data/test_dataset.py` & `transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/data/testing/test_dataset.py` & `transformers4rec-23.4.0/tests/unit/data/testing/test_dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/merlin_standard_lib/__init__.py` & `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/merlin_standard_lib/schema/test_schema.py` & `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 
+from merlin_standard_lib import categorical_cardinalities
 from merlin_standard_lib.schema import schema
 
 
 def test_column_proto_txt():
     col = schema.ColumnSchema(name="qa")
 
     assert col.to_proto_text() == 'name: "qa"\n'
@@ -56,15 +57,15 @@
 
 
 def test_column_schema_categorical_with_shape():
     col = schema.ColumnSchema.create_categorical("cat_1", 1000, shape=(1,))
 
     assert col.shape.dim[0].size == 1
 
-    assert schema.Schema([col]).categorical_cardinalities() == dict(cat_1=1000 + 1)
+    assert categorical_cardinalities(schema.Schema([col])) == dict(cat_1=1000 + 1)
 
 
 def test_column_schema_categorical_with_value_count():
     col = schema.ColumnSchema.create_categorical(
         "cat_1", 1000, value_count=schema.ValueCount(0, 100)
     )
```

### Comparing `transformers4rec-23.2.0/tests/merlin_standard_lib/schema/test_tag.py` & `transformers4rec-23.4.0/transformers4rec/torch/typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 # Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -9,18 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from merlin_standard_lib import Tag
+import typing
+from typing import Dict
 
+import torch
 
-def test_tag_equality():
-    assert Tag.CATEGORICAL == "categorical"
-    assert Tag.CONTINUOUS == "continuous"
-    assert Tag.ITEM_ID == "item_id"
+# TODO: Make this more generic and work with multi-hot features
+TabularData = Dict[str, torch.Tensor]
+TensorOrTabularData = typing.Union[torch.Tensor, TabularData]
 
 
-def test_tag_to_str():
-    assert str(Tag.CATEGORICAL) == "categorical"
+__all__ = [
+    "TabularData",
+    "TensorOrTabularData",
+]
```

### Comparing `transformers4rec-23.2.0/tests/torch/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/block/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/block/test_base.py` & `transformers4rec-23.4.0/tests/unit/torch/block/test_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,54 +10,53 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import pytest
+import torch
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_base_block(torch_tabular_features):
     block = torch_tabular_features >> tr.MLPBlock([64, 32])
 
     embedding_block = block.get_children_by_class_name(list(block), "EmbeddingFeatures")[0]
 
     assert isinstance(embedding_block, tr.EmbeddingFeatures)
 
 
 def test_sequential_block(torch_tabular_features):
     block = tr.SequentialBlock(
         torch_tabular_features,
         tr.MLPBlock([64, 32]),
-        tr.Block(pytorch.nn.Dropout(0.5), [None, 32]),
+        tr.Block(torch.nn.Dropout(0.5), [None, 32]),
     )
 
     output_size = block.output_size()
     assert list(output_size) == [-1, 32]
 
     embedding_block = block.get_children_by_class_name(list(block), "EmbeddingFeatures")[0]
     assert isinstance(embedding_block, tr.EmbeddingFeatures)
 
 
 def test_sequential_block_with_output_size(torch_tabular_features):
     block = tr.SequentialBlock(
         torch_tabular_features,
         tr.MLPBlock([64, 32]),
-        pytorch.nn.Dropout(0.5),
+        torch.nn.Dropout(0.5),
         output_size=[None, 32],
     )
 
     output_size = block.output_size()
     assert list(output_size) == [None, 32]
 
 
 def test_sequential(torch_tabular_features):
     inputs = torch_tabular_features
-    block = pytorch.nn.Sequential(*tr.build_blocks(inputs, tr.MLPBlock([64, 32])))
-    block2 = pytorch.nn.Sequential(inputs, tr.MLPBlock([64, 32]).to_module(inputs))
+    block = torch.nn.Sequential(*tr.build_blocks(inputs, tr.MLPBlock([64, 32])))
+    block2 = torch.nn.Sequential(inputs, tr.MLPBlock([64, 32]).to_module(inputs))
 
-    assert isinstance(block, pytorch.nn.Sequential)
-    assert isinstance(block2, pytorch.nn.Sequential)
+    assert isinstance(block, torch.nn.Sequential)
+    assert isinstance(block2, torch.nn.Sequential)
```

### Comparing `transformers4rec-23.2.0/tests/torch/block/test_mlp.py` & `transformers4rec-23.4.0/tests/unit/torch/block/test_mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import pytest
-
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_mlp_block(tabular_schema, torch_tabular_data):
     tab_module = tr.TabularFeatures.from_schema(
         tabular_schema, max_sequence_length=20, aggregation="concat"
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/block/test_transformer.py` & `transformers4rec-23.4.0/tests/unit/torch/block/test_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
 
+import transformers4rec.torch as tr
 from transformers4rec.config import transformer as tconf
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
-
-
 config_classes = [
     tconf.XLNetConfig,
     tconf.LongformerConfig,
     tconf.GPT2Config,
     tconf.BertConfig,
     tconf.RobertaConfig,
     tconf.TransfoXLConfig,
@@ -36,15 +34,14 @@
 lm_tasks = list(tr.masking.masking_registry.keys())
 lm_tasks.remove("permutation")
 
 
 # Test output of XLNet with different masking tasks using SequentialBlock
 @pytest.mark.parametrize("task", lm_tasks)
 def test_transformer_block(yoochoose_schema, torch_yoochoose_like, task):
-
     col_group = yoochoose_schema
     tab_module = tr.TabularSequenceFeatures.from_schema(
         col_group,
         max_sequence_length=20,
         aggregation="concat",
         masking=task,
     )
@@ -63,15 +60,14 @@
 
     assert outputs.ndim == 3
     assert outputs.shape[-1] == 64
 
 
 # Test output of XLNet with permutation language model using SequentialBlock
 def test_xlnet_with_plm(yoochoose_schema, torch_yoochoose_like):
-
     col_group = yoochoose_schema
     tab_module = tr.TabularSequenceFeatures.from_schema(
         col_group,
         max_sequence_length=20,
         aggregation="concat",
         d_output=64,
         masking="permutation",
@@ -133,15 +129,15 @@
         d_output=64,
         masking="causal",
     )
 
     transformer_model = transformer_body.build(d_model=64, n_head=4, n_layer=2, total_seq_length=20)
     model = tr.TransformerBlock(transformer=transformer_model)
 
-    block = pytorch.nn.Sequential(tab_module, model)
+    block = torch.nn.Sequential(tab_module, model)
 
     outputs = block(torch_yoochoose_like)
 
     assert outputs.ndim == 3
     assert outputs.shape[-1] == 64
 
 
@@ -156,15 +152,15 @@
         masking="causal",
     )
 
     model = tr.TransformerBlock.from_registry(
         transformer="reformer", d_model=64, n_head=4, n_layer=2, total_seq_length=20
     )
 
-    block = pytorch.nn.Sequential(tab_module, model)
+    block = torch.nn.Sequential(tab_module, model)
 
     outputs = block(torch_yoochoose_like)
 
     assert outputs.ndim == 3
     # 2 * hidden_size because Reformer uses reversible resnet layers
     assert outputs.shape[-1] == 64 * 2
```

### Comparing `transformers4rec-23.2.0/tests/torch/conftest.py` & `transformers4rec-23.4.0/tests/unit/torch/_conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,106 +10,105 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import numpy as np
 import pytest
+import torch
 
-pytorch = pytest.importorskip("torch")
-np = pytest.importorskip("numpy")
-tr = pytest.importorskip("transformers4rec.torch")
-schema_utils = pytest.importorskip("transformers4rec.torch.utils.schema_utils")
+import transformers4rec.torch as tr
 
 NUM_EXAMPLES = 1000
 MAX_CARDINALITY = 100
 
 
 @pytest.fixture
 def torch_con_features():
     features = {}
     keys = [f"con_{f}" for f in "abcdef"]
 
     for key in keys:
-        features[key] = pytorch.rand((NUM_EXAMPLES, 1))
+        features[key] = torch.rand((NUM_EXAMPLES, 1))
 
     return features
 
 
 @pytest.fixture
 def torch_cat_features():
     features = {}
     keys = [f"cat_{f}" for f in "abcdef"]
 
     for key in keys:
-        features[key] = pytorch.randint(MAX_CARDINALITY, (NUM_EXAMPLES,))
+        features[key] = torch.randint(MAX_CARDINALITY, (NUM_EXAMPLES,))
 
     return features
 
 
 @pytest.fixture
 def torch_masking_inputs():
     # fixed parameters for tests
     NUM_EXAMPLES = 20
     MAX_LEN = 10
     PAD_TOKEN = 0
     hidden_dim = 16
     features = {}
     # generate random tensors for test
-    features["input_tensor"] = pytorch.tensor(
+    features["input_tensor"] = torch.tensor(
         np.random.uniform(0, 1, (NUM_EXAMPLES, MAX_LEN, hidden_dim))
     )
     # create sequences
-    labels = pytorch.tensor(np.random.randint(1, MAX_CARDINALITY, (NUM_EXAMPLES, MAX_LEN)))
+    labels = torch.tensor(np.random.randint(1, MAX_CARDINALITY, (NUM_EXAMPLES, MAX_LEN)))
     # replace last 2 items by zeros to mimic padding
     labels[:, MAX_LEN - 2 :] = 0
     features["labels"] = labels
     features["padding_idx"] = PAD_TOKEN
     features["vocab_size"] = MAX_CARDINALITY
 
     return features
 
 
 @pytest.fixture
 def torch_seq_prediction_head_inputs():
     ITEM_DIM = 128
     POS_EXAMPLE = 25
     features = {}
-    features["seq_model_output"] = pytorch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, ITEM_DIM)))
-    features["item_embedding_table"] = pytorch.nn.Embedding(MAX_CARDINALITY, ITEM_DIM)
-    features["labels_all"] = pytorch.tensor(np.random.randint(1, MAX_CARDINALITY, (POS_EXAMPLE,)))
+    features["seq_model_output"] = torch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, ITEM_DIM)))
+    features["item_embedding_table"] = torch.nn.Embedding(MAX_CARDINALITY, ITEM_DIM)
+    features["labels_all"] = torch.tensor(np.random.randint(1, MAX_CARDINALITY, (POS_EXAMPLE,)))
     features["vocab_size"] = MAX_CARDINALITY
     features["item_dim"] = ITEM_DIM
     return features
 
 
 @pytest.fixture
 def torch_ranking_metrics_inputs():
     POS_EXAMPLE = 30
     VOCAB_SIZE = 40
     features = {}
-    features["scores"] = pytorch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, VOCAB_SIZE)))
-    features["ks"] = pytorch.LongTensor([1, 2, 3, 5, 10, 20])
-    features["labels_one_hot"] = pytorch.LongTensor(
+    features["scores"] = torch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, VOCAB_SIZE)))
+    features["ks"] = [1, 2, 3, 5, 10, 20]
+    features["labels_one_hot"] = torch.LongTensor(
         np.random.choice(a=[0, 1], size=(POS_EXAMPLE, VOCAB_SIZE))
     )
 
-    features["labels"] = pytorch.tensor(np.random.randint(1, VOCAB_SIZE, (POS_EXAMPLE,)))
+    features["labels"] = torch.tensor(np.random.randint(1, VOCAB_SIZE, (POS_EXAMPLE,)))
     return features
 
 
 @pytest.fixture
 def torch_seq_prediction_head_link_to_block():
     ITEM_DIM = 64
     POS_EXAMPLE = 25
     features = {}
-    features["seq_model_output"] = pytorch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, ITEM_DIM)))
-    features["item_embedding_table"] = pytorch.nn.Embedding(MAX_CARDINALITY, ITEM_DIM)
-    features["labels_all"] = pytorch.tensor(np.random.randint(1, MAX_CARDINALITY, (POS_EXAMPLE,)))
+    features["seq_model_output"] = torch.tensor(np.random.uniform(0, 1, (POS_EXAMPLE, ITEM_DIM)))
+    features["item_embedding_table"] = torch.nn.Embedding(MAX_CARDINALITY, ITEM_DIM)
+    features["labels_all"] = torch.tensor(np.random.randint(1, MAX_CARDINALITY, (POS_EXAMPLE,)))
     features["vocab_size"] = MAX_CARDINALITY
     features["item_dim"] = ITEM_DIM
     features["config"] = {
         "item": {
             "dtype": "categorical",
             "cardinality": MAX_CARDINALITY,
             "tags": ["categorical", "item"],
```

### Comparing `transformers4rec-23.2.0/tests/torch/features/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/features/test_continuous.py` & `transformers4rec-23.4.0/tests/unit/torch/features/test_continuous.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import pytest
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag
-
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_continuous_features(torch_con_features):
     features = ["con_a", "con_b"]
     con = tr.ContinuousFeatures(features)(torch_con_features)
 
     assert list(con.keys()) == features
 
 
 def test_continuous_features_yoochoose(yoochoose_schema, torch_yoochoose_like):
     schema = yoochoose_schema
-    cont_cols = schema.select_by_tag(Tag.CONTINUOUS)
+    cont_cols = schema.select_by_tag(Tags.CONTINUOUS)
 
     con = tr.ContinuousFeatures.from_schema(cont_cols)
     outputs = con(torch_yoochoose_like)
 
     assert set(outputs.keys()) == set(cont_cols.column_names)
```

### Comparing `transformers4rec-23.2.0/tests/torch/features/test_embedding.py` & `transformers4rec-23.4.0/tests/unit/torch/features/test_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 # limitations under the License.
 #
 
 from functools import partial
 
 import numpy as np
 import pytest
+import torch
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag
-
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_embedding_features(torch_cat_features):
     dim = 15
     feature_config = {
         f: tr.FeatureConfig(tr.TableConfig(100, dim, name=f)) for f in torch_cat_features.keys()
     }
@@ -49,15 +48,15 @@
     )
     assert all([emb.detach().numpy().std() > 0.5 for emb in embeddings.values()])
 
 
 def test_embedding_features_custom_init(torch_cat_features):
     MEAN = 1.0
     STD = 0.05
-    emb_initializer = partial(pytorch.nn.init.normal_, mean=MEAN, std=STD)
+    emb_initializer = partial(torch.nn.init.normal_, mean=MEAN, std=STD)
     feature_config = {
         f: tr.FeatureConfig(tr.TableConfig(100, dim=15, name=f, initializer=emb_initializer))
         for f in torch_cat_features.keys()
     }
     embeddings = tr.EmbeddingFeatures(feature_config)(torch_cat_features)
 
     assert list(embeddings.keys()) == list(feature_config.keys())
@@ -72,29 +71,28 @@
 def test_table_config_invalid_embedding_initializer():
     with pytest.raises(ValueError) as excinfo:
         tr.TableConfig(100, dim=15, initializer="INVALID INITIALIZER")
     assert "initializer must be callable if specified" in str(excinfo.value)
 
 
 def test_embedding_features_yoochoose(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
-
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
     emb_module = tr.EmbeddingFeatures.from_schema(schema)
     embeddings = emb_module(torch_yoochoose_like)
 
     assert list(embeddings.keys()) == schema.column_names
     assert all(emb.shape[-1] == 64 for emb in embeddings.values())
     assert emb_module.item_id == "item_id/list"
 
     max_value = schema.select_by_name("item_id/list").feature[0].int_domain.max
     assert emb_module.item_embedding_table.num_embeddings == max_value + 1
 
 
 def test_embedding_features_yoochoose_custom_dims(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
 
     emb_module = tr.EmbeddingFeatures.from_schema(
         schema, embedding_dims={"item_id/list": 100}, embedding_dim_default=64
     )
 
     assert emb_module.embedding_tables["item_id/list"].weight.shape[1] == 100
     assert emb_module.embedding_tables["category/list"].weight.shape[1] == 64
@@ -102,15 +100,15 @@
     embeddings = emb_module(torch_yoochoose_like)
 
     assert embeddings["item_id/list"].shape[1] == 100
     assert embeddings["category/list"].shape[1] == 64
 
 
 def test_embedding_features_yoochoose_infer_embedding_sizes(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
 
     emb_module = tr.EmbeddingFeatures.from_schema(
         schema, infer_embedding_sizes=True, infer_embedding_sizes_multiplier=3.0
     )
 
     assert emb_module.embedding_tables["item_id/list"].weight.shape[1] == 46
     assert emb_module.embedding_tables["category/list"].weight.shape[1] == 13
@@ -124,21 +122,21 @@
 def test_embedding_features_yoochoose_custom_initializers(yoochoose_schema, torch_yoochoose_like):
     ITEM_MEAN = 1.0
     ITEM_STD = 0.05
 
     CATEGORY_MEAN = 2.0
     CATEGORY_STD = 0.1
 
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
     emb_module = tr.EmbeddingFeatures.from_schema(
         schema,
         layer_norm=False,
         embeddings_initializers={
-            "item_id/list": partial(pytorch.nn.init.normal_, mean=ITEM_MEAN, std=ITEM_STD),
-            "category/list": partial(pytorch.nn.init.normal_, mean=CATEGORY_MEAN, std=CATEGORY_STD),
+            "item_id/list": partial(torch.nn.init.normal_, mean=ITEM_MEAN, std=ITEM_STD),
+            "category/list": partial(torch.nn.init.normal_, mean=CATEGORY_MEAN, std=CATEGORY_STD),
         },
     )
 
     embeddings = emb_module(torch_yoochoose_like)
 
     assert embeddings["item_id/list"].detach().numpy().mean() == pytest.approx(ITEM_MEAN, abs=0.1)
     assert embeddings["item_id/list"].detach().numpy().std() == pytest.approx(ITEM_STD, abs=0.1)
@@ -155,15 +153,15 @@
 def test_pre_trained_embeddings_initializer(yoochoose_schema, torch_yoochoose_like, trainable):
     item_id_cardinality = (
         yoochoose_schema.select_by_name("item_id/list").feature[0].int_domain.max + 1
     )
     embedding_dim = 64
     pre_trained_item_embeddings = np.random.rand(item_id_cardinality, embedding_dim)
 
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
     emb_module = tr.EmbeddingFeatures.from_schema(
         schema,
         embedding_dims={"item_id/list": embedding_dim},
         embeddings_initializers={
             "item_id/list": tr.PretrainedEmbeddingsInitializer(
                 pre_trained_item_embeddings, trainable=trainable
             ),
@@ -194,64 +192,64 @@
 
 
 def test_soft_embedding():
     embeddings_dim = 16
     num_embeddings = 64
 
     soft_embedding = tr.SoftEmbedding(num_embeddings, embeddings_dim)
-    assert soft_embedding.embedding_table.weight.shape == pytorch.Size(
+    assert soft_embedding.embedding_table.weight.shape == torch.Size(
         [num_embeddings, embeddings_dim]
     ), "Internal soft embedding table does not have the expected shape"
 
     batch_size = 10
     seq_length = 20
-    cont_feature_inputs = pytorch.rand((batch_size, seq_length))
+    cont_feature_inputs = torch.rand((batch_size, seq_length))
     output = soft_embedding(cont_feature_inputs)
 
-    assert output.shape == pytorch.Size(
+    assert output.shape == torch.Size(
         [batch_size, seq_length, embeddings_dim]
     ), "Soft embedding output has not the expected shape"
 
     # Checking the default embedding initialization
     assert output.detach().numpy().mean() == pytest.approx(0.0, abs=0.2)
     assert output.detach().numpy().std() == pytest.approx(0.05, abs=0.2)
 
 
 def test_soft_embedding_with_custom_init():
     embeddings_dim = 16
     num_embeddings = 64
 
     INIT_MEAN = 1.0
     INIT_STD = 0.05
-    emb_initializer = partial(pytorch.nn.init.normal_, mean=INIT_MEAN, std=INIT_STD)
+    emb_initializer = partial(torch.nn.init.normal_, mean=INIT_MEAN, std=INIT_STD)
     soft_embedding = tr.SoftEmbedding(
         num_embeddings, embeddings_dim, emb_initializer=emb_initializer
     )
-    assert soft_embedding.embedding_table.weight.shape == pytorch.Size(
+    assert soft_embedding.embedding_table.weight.shape == torch.Size(
         [num_embeddings, embeddings_dim]
     ), "Internal soft embedding table does not have the expected shape"
 
     batch_size = 10
     seq_length = 20
-    cont_feature_inputs = pytorch.rand((batch_size, seq_length))
+    cont_feature_inputs = torch.rand((batch_size, seq_length))
     output = soft_embedding(cont_feature_inputs)
 
-    assert output.shape == pytorch.Size(
+    assert output.shape == torch.Size(
         [batch_size, seq_length, embeddings_dim]
     ), "Soft embedding output has not the expected shape"
 
     assert output.detach().numpy().mean() == pytest.approx(INIT_MEAN, abs=0.1)
     assert output.detach().numpy().std() == pytest.approx(INIT_STD, abs=0.1)
 
 
 def test_soft_continuous_features(torch_con_features):
     dim = 16
     num_embeddings = 64
 
-    emb_initializer = partial(pytorch.nn.init.normal_, mean=1.0, std=0.05)
+    emb_initializer = partial(torch.nn.init.normal_, mean=1.0, std=0.05)
 
     feature_config = {
         f: tr.FeatureConfig(
             tr.TableConfig(num_embeddings, dim, initializer=emb_initializer, name=f)
         )
         for f in torch_con_features.keys()
     }
@@ -264,16 +262,16 @@
         [list(v.shape) == list(torch_con_features[k].shape) + [dim] for k, v in output.items()]
     )
 
 
 def test_layer_norm_features():
     ln = tr.TabularLayerNorm(features_dim={"a": 100, "b": 200})
     inputs = {
-        "a": pytorch.tensor(np.random.uniform(1.0, 4.0, (500, 100)), dtype=pytorch.float32),
-        "b": pytorch.tensor(np.random.uniform(2.0, 10.0, (500, 200)), dtype=pytorch.float32),
+        "a": torch.tensor(np.random.uniform(1.0, 4.0, (500, 100)), dtype=torch.float32),
+        "b": torch.tensor(np.random.uniform(2.0, 10.0, (500, 200)), dtype=torch.float32),
     }
 
     outputs = ln(inputs)
 
     assert all(
         [val.detach().numpy().mean() == pytest.approx(0.0, abs=0.1) for val in outputs.values()]
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/features/test_sequential.py` & `transformers4rec-23.4.0/tests/unit/torch/features/test_sequential.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,108 +11,114 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+from merlin.schema import Schema as CoreSchema
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag
+import transformers4rec.torch as tr
+from tests.conftest import parametrize_schemas
 
-tr = pytest.importorskip("transformers4rec.torch")
 
-
-def test_sequential_and_non_seq_embedding_features(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+@parametrize_schemas("yoochoose")
+def test_sequential_and_non_seq_embedding_features(schema, torch_yoochoose_like):
+    schema = schema.select_by_tag(Tags.CATEGORICAL)
     emb_module = tr.SequenceEmbeddingFeatures.from_schema(schema)
 
     outputs = emb_module(torch_yoochoose_like)
 
-    assert list(outputs.keys()) == schema.select_by_tag(Tag.CATEGORICAL).column_names
+    assert list(outputs.keys()) == schema.select_by_tag(Tags.CATEGORICAL).column_names
 
     seq_features = ["item_id/list", "category/list"]
     non_seq_features = ["user_country"]
 
     for fname in seq_features:
         assert list(outputs[fname].shape) == [100, 20, 64]
 
     for fname in non_seq_features:
         assert list(outputs[fname].shape) == [100, 64]
 
 
-def test_sequential_tabular_features(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features(schema, torch_yoochoose_like):
     tab_module = tr.TabularSequenceFeatures.from_schema(schema)
 
     outputs = tab_module(torch_yoochoose_like)
 
-    tag_select = lambda tags: any(t in [Tag.CONTINUOUS, Tag.CATEGORICAL] for t in tags)  # noqa
-    cols = schema.select_by_tag(tag_select).column_names
+    cols = [
+        c.name
+        for c in list(
+            schema.select_by_tag(Tags.CONTINUOUS) + schema.select_by_tag(Tags.CATEGORICAL)
+        )
+    ]
 
     assert set(outputs.keys()) == set(cols)
 
 
-def test_sequential_tabular_features_with_feature_modules_kwargs(
-    yoochoose_schema, torch_yoochoose_like
-):
-    schema = yoochoose_schema
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features_with_feature_modules_kwargs(schema, torch_yoochoose_like):
     EMB_DIM = 200
     tab_module = tr.TabularSequenceFeatures.from_schema(
         schema,
         embedding_dim_default=EMB_DIM,
     )
 
     outputs = tab_module(torch_yoochoose_like)
 
     assert set(outputs.keys()) == set(
-        schema.select_by_tag(Tag.CONTINUOUS).column_names
-        + schema.select_by_tag(Tag.CATEGORICAL).column_names
+        schema.select_by_tag(Tags.CONTINUOUS).column_names
+        + schema.select_by_tag(Tags.CATEGORICAL).column_names
     )
 
-    categ_features = schema.select_by_tag(Tag.CATEGORICAL).column_names
+    categ_features = schema.select_by_tag(Tags.CATEGORICAL).column_names
     assert all(v.shape[-1] == EMB_DIM for k, v in outputs.items() if k in categ_features)
 
 
-def test_sequential_tabular_features_with_projection(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features_with_projection(schema, torch_yoochoose_like):
     tab_module = tr.TabularSequenceFeatures.from_schema(
         schema, max_sequence_length=20, continuous_projection=64
     )
-    continuous_feature_names = schema.select_by_tag(Tag.CONTINUOUS).column_names
+    continuous_feature_names = schema.select_by_tag(Tags.CONTINUOUS).column_names
 
     outputs = tab_module(torch_yoochoose_like)
 
     assert len(set(continuous_feature_names).intersection(set(outputs.keys()))) == 0
     assert "continuous_projection" in outputs
     assert list(outputs["continuous_projection"].shape)[1:] == [20, 64]
 
 
-def test_sequential_tabular_features_with_masking(yoochoose_schema, torch_yoochoose_like):
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features_with_masking(schema, torch_yoochoose_like):
     input_module = tr.TabularSequenceFeatures.from_schema(
-        yoochoose_schema,
+        schema,
         max_sequence_length=20,
         continuous_projection=64,
         d_output=100,
         masking="causal",
     )
 
     outputs = input_module(torch_yoochoose_like)
 
     assert outputs.ndim == 3
     assert outputs.shape[-1] == 100
     assert outputs.shape[1] == 20
 
 
-def test_sequential_tabular_features_ignore_masking(yoochoose_schema, torch_yoochoose_like):
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features_ignore_masking(schema, torch_yoochoose_like):
     import numpy as np
 
     from transformers4rec.torch.masking import CausalLanguageModeling, MaskedLanguageModeling
 
     input_module = tr.TabularSequenceFeatures.from_schema(
-        yoochoose_schema,
+        schema,
         max_sequence_length=20,
         continuous_projection=64,
         d_output=100,
         aggregation="concat",
     )
     output_wo_masking = input_module(torch_yoochoose_like, training=False).detach().cpu().numpy()
 
@@ -135,25 +141,24 @@
     output_eval_masking = (
         input_module(torch_yoochoose_like, training=False, testing=True).detach().cpu().numpy()
     )
     # MLM extends the inputs with one position during inference
     assert output_inference_masking.shape[1] == output_eval_masking.shape[1] + 1
 
 
-def test_tabular_features_yoochoose_direct(yoochoose_schema, torch_yoochoose_like):
-    continuous_module = tr.ContinuousFeatures.from_schema(yoochoose_schema, tags=["continuous"])
-    categorical_module = tr.SequenceEmbeddingFeatures.from_schema(
-        yoochoose_schema, tags=["categorical"]
-    )
+@parametrize_schemas("yoochoose")
+def test_tabular_features_yoochoose_direct(schema, torch_yoochoose_like):
+    continuous_module = tr.ContinuousFeatures.from_schema(schema, tags=Tags.CONTINUOUS)
+    categorical_module = tr.SequenceEmbeddingFeatures.from_schema(schema, tags=Tags.CATEGORICAL)
 
     tab_seq_features = tr.TabularSequenceFeatures(
         continuous_module=continuous_module,
         categorical_module=categorical_module,
         aggregation="concat",
-        schema=yoochoose_schema,
+        schema=schema,
     )
     outputs = tab_seq_features(torch_yoochoose_like)
 
     assert (
         len(
             set(categorical_module.schema.column_names).difference(
                 set(tab_seq_features.schema.column_names)
@@ -168,20 +173,24 @@
             )
         )
         == 0
     )
     assert len(outputs.shape) == 3
 
 
-def test_sequential_tabular_features_with_masking_no_itemid(yoochoose_schema):
+@parametrize_schemas("yoochoose")
+def test_sequential_tabular_features_with_masking_no_itemid(schema):
     with pytest.raises(ValueError) as excinfo:
-        yoochoose_schema = yoochoose_schema.remove_by_name("item_id/list")
+        if isinstance(schema, CoreSchema):
+            schema = schema.excluding_by_name("item_id/list")
+        else:
+            schema = schema.remove_by_name("item_id/list")
 
         tr.TabularSequenceFeatures.from_schema(
-            yoochoose_schema,
+            schema,
             max_sequence_length=20,
             continuous_projection=64,
             d_output=100,
             masking="causal",
         )
 
     assert "For masking a categorical_module is required including an item_id" in str(excinfo.value)
@@ -197,14 +206,14 @@
             projection=tr.MLPBlock([64]),
             masking="causal",
         )
 
     assert "You cannot specify both d_output and projection at the same time" in str(excinfo.value)
 
 
-def test_sequential_and_non_sequential_tabular_features(yoochoose_schema, torch_yoochoose_like):
-    schema = yoochoose_schema
+@parametrize_schemas("yoochoose")
+def test_sequential_and_non_sequential_tabular_features(schema, torch_yoochoose_like):
     tab_module = tr.TabularSequenceFeatures.from_schema(schema, aggregation="concat")
 
     outputs = tab_module(torch_yoochoose_like)
 
     assert list(outputs.shape) == [100, 20, 203]
```

### Comparing `transformers4rec-23.2.0/tests/torch/features/test_tabular.py` & `transformers4rec-23.4.0/tests/unit/torch/features/test_tabular.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,76 +10,73 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import pytest
 
-from merlin_standard_lib import Tag
+from merlin.schema import Tags
 
-tr = pytest.importorskip("transformers4rec.torch")
-torch_utils = pytest.importorskip("transformers4rec.torch.utils.torch_utils")
+import transformers4rec.torch as tr
+from tests.conftest import parametrize_schemas
 
 
-def test_tabular_features(tabular_schema, torch_tabular_data):
-    schema = tabular_schema
+@parametrize_schemas("tabular")
+def test_tabular_features(schema, torch_tabular_data):
     tab_module = tr.TabularFeatures.from_schema(schema)
 
     outputs = tab_module(torch_tabular_data)
 
     assert set(outputs.keys()) == set(
-        schema.select_by_tag(Tag.CONTINUOUS).column_names
-        + schema.select_by_tag(Tag.CATEGORICAL).column_names
+        schema.select_by_tag(Tags.CONTINUOUS).column_names
+        + schema.select_by_tag(Tags.CATEGORICAL).column_names
     )
 
 
-def test_tabular_features_embeddings_options(tabular_schema, torch_tabular_data):
-    schema = tabular_schema
-
+@parametrize_schemas("tabular")
+def test_tabular_features_embeddings_options(schema, torch_tabular_data):
     EMB_DIM = 100
     tab_module = tr.TabularFeatures.from_schema(schema, embedding_dim_default=EMB_DIM)
 
     outputs = tab_module(torch_tabular_data)
 
-    categ_features = schema.select_by_tag(Tag.CATEGORICAL).column_names
+    categ_features = schema.select_by_tag(Tags.CATEGORICAL).column_names
     assert all(v.shape[-1] == EMB_DIM for k, v in outputs.items() if k in categ_features)
 
 
-def test_tabular_features_with_projection(tabular_schema, torch_tabular_data):
-    schema = tabular_schema
+@parametrize_schemas("tabular")
+def test_tabular_features_with_projection(schema, torch_tabular_data):
     tab_module = tr.TabularFeatures.from_schema(schema, continuous_projection=64)
 
     outputs = tab_module(torch_tabular_data)
 
-    continuous_feature_names = schema.select_by_tag(Tag.CONTINUOUS).column_names
+    continuous_feature_names = schema.select_by_tag(Tags.CONTINUOUS).column_names
 
     assert len(set(continuous_feature_names).intersection(set(outputs.keys()))) == 0
     assert "continuous_projection" in outputs
     assert list(outputs["continuous_projection"].shape)[1] == 64
 
 
-def test_tabular_features_soft_encoding(tabular_schema, torch_tabular_data):
-    schema = tabular_schema
-
+@parametrize_schemas("tabular")
+def test_tabular_features_soft_encoding(schema, torch_tabular_data):
     emb_cardinality = 10
     emb_dim = 8
     tab_module = tr.TabularFeatures.from_schema(
         schema,
         continuous_soft_embeddings=True,
         soft_embedding_cardinality_default=emb_cardinality,
         soft_embedding_dim_default=emb_dim,
     )
 
     outputs = tab_module(torch_tabular_data)
 
     assert (
         list(outputs.keys())
-        == schema.select_by_tag(Tag.CONTINUOUS).column_names
-        + schema.select_by_tag(Tag.CATEGORICAL).column_names
+        == schema.select_by_tag(Tags.CONTINUOUS).column_names
+        + schema.select_by_tag(Tags.CATEGORICAL).column_names
     )
 
     assert all(
         list(outputs[col_name].shape) == list(torch_tabular_data[col_name].shape) + [emb_dim]
-        for col_name in schema.select_by_tag(Tag.CONTINUOUS).column_names
+        for col_name in schema.select_by_tag(Tags.CONTINUOUS).column_names
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/model/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/model/test_head.py` & `transformers4rec-23.4.0/tests/unit/torch/model/test_head.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 # fixed parameters for tests
 METRICS = [
     tr.ranking_metric.NDCGAt(top_ks=[2, 5, 10], labels_onehot=True),
     tr.ranking_metric.AvgPrecisionAt(top_ks=[2, 5, 10], labels_onehot=True),
 ]
 
 
 @pytest.mark.parametrize("task", [tr.BinaryClassificationTask, tr.RegressionTask])
 def test_simple_heads(torch_tabular_features, torch_tabular_data, task):
-    targets = {"target": pytorch.randint(2, (100,)).float()}
+    targets = {"target": torch.randint(2, (100,)).float()}
 
     body = tr.SequentialBlock(torch_tabular_features, tr.MLPBlock([64]))
     head = task("target").to_head(body, torch_tabular_features)
 
     body_out = body(torch_tabular_data)
     loss = head(body_out, targets=targets, training=True)["loss"]
 
@@ -43,17 +43,17 @@
 @pytest.mark.parametrize("task_block", [None, tr.MLPBlock([32]), tr.MLPBlock([32]).build([-1, 64])])
 @pytest.mark.parametrize("summary", [None, "last", "first", "mean", "cls_index"])
 def test_simple_heads_on_sequence(
     torch_yoochoose_tabular_transformer_features, torch_yoochoose_like, task, task_block, summary
 ):
     inputs = torch_yoochoose_tabular_transformer_features
     if summary:
-        targets = {"target": pytorch.randint(2, (100,)).float()}
+        targets = {"target": torch.randint(2, (100,)).float()}
     else:
-        targets = {"target": pytorch.randint(2, (2000,)).float()}
+        targets = {"target": torch.randint(2, (100, 20)).float()}
 
     body = tr.SequentialBlock(inputs, tr.MLPBlock([64]))
     head = task("target", task_block=task_block, summary_type=summary).to_head(body, inputs)
 
     body_out = body(torch_yoochoose_like)
     loss = head(body_out, targets=targets, training=True)["loss"]
 
@@ -67,43 +67,43 @@
         tr.MLPBlock([32]),
         tr.MLPBlock([32]).build([-1, 64]),
         dict(classification=tr.MLPBlock([16]), regression=tr.MLPBlock([20])),
     ],
 )
 def test_head_with_multiple_tasks(torch_tabular_features, torch_tabular_data, task_blocks):
     targets = {
-        "classification": pytorch.randint(2, (100,)).float(),
-        "regression": pytorch.randint(2, (100,)).float(),
+        "classification": torch.randint(2, (100,)).float(),
+        "regression": torch.randint(2, (100,)).float(),
     }
 
     body = tr.SequentialBlock(torch_tabular_features, tr.MLPBlock([64]))
     tasks = [
         tr.BinaryClassificationTask("classification", task_name="classification"),
         tr.RegressionTask("regression", task_name="regression"),
     ]
     # TODO: how to get targets with no dataloader?
     head = tr.Head(body, tasks, task_blocks=task_blocks)
-    optimizer = pytorch.optim.Adam(head.parameters())
+    optimizer = torch.optim.Adam(head.parameters())
 
-    with pytorch.set_grad_enabled(mode=True):
+    with torch.set_grad_enabled(mode=True):
         body_out = body(torch_tabular_data)
         output = head(body_out, targets=targets, training=True)
         loss = output["loss"]
         metrics = head.calculate_metrics(output["predictions"], targets=output["labels"])
 
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
 
     assert loss.min() >= 0 and loss.max() <= 1
     assert len(metrics.keys()) == 4
     if task_blocks:
         assert head.task_blocks["classification"][0] != head.task_blocks["regression"][0]
 
-        assert not pytorch.equal(
+        assert not torch.equal(
             head.task_blocks["classification"][0][0].weight,
             head.task_blocks["regression"][0][0].weight,
         )
 
 
 def test_item_prediction_head(torch_yoochoose_tabular_transformer_features, torch_yoochoose_like):
     input_module = torch_yoochoose_tabular_transformer_features
@@ -142,15 +142,15 @@
     body = tr.SequentialBlock(input_module, tr.MLPBlock([64]))
     head = tr.Head(body, tr.NextItemPredictionTask(weight_tying=weight_tying), inputs=input_module)
 
     body_outputs = body(torch_yoochoose_like, testing=True)
 
     trg_flat = input_module.masking.masked_targets.flatten()
     non_pad_mask = trg_flat != input_module.masking.padding_idx
-    labels_all = pytorch.masked_select(trg_flat, non_pad_mask)
+    labels_all = torch.masked_select(trg_flat, non_pad_mask)
 
     output = head.prediction_task_dict["next-item"](
         inputs=body_outputs,
         targets=labels_all,
         testing=True,
     )
     loss = output["loss"]
@@ -182,26 +182,26 @@
         param in outputs
         for param in ["loss", "labels", "predictions", "pred_metadata", "model_outputs"]
     ]
 
 
 def test_head_not_inferring_output_size_body(torch_tabular_features):
     with pytest.raises(ValueError) as excinfo:
-        body = tr.SequentialBlock(torch_tabular_features, pytorch.nn.Dropout(0.5))
+        body = tr.SequentialBlock(torch_tabular_features, torch.nn.Dropout(0.5))
         tr.Head(
             body,
             tr.BinaryClassificationTask(),
         )
 
         assert "Can't infer output-size of the body" in str(excinfo.value)
 
 
 def test_item_prediction_head_with_wrong_body(torch_tabular_features):
     with pytest.raises(ValueError) as excinfo:
-        body = tr.SequentialBlock(torch_tabular_features, pytorch.nn.Dropout(0.5))
+        body = tr.SequentialBlock(torch_tabular_features, torch.nn.Dropout(0.5))
         tr.Head(
             body,
             tr.NextItemPredictionTask(),
         )
 
         assert "NextItemPredictionTask needs a 3-dim vector as input, found:" in str(excinfo.value)
 
@@ -210,15 +210,15 @@
     torch_yoochoose_tabular_transformer_features, torch_yoochoose_like
 ):
     input_module = torch_yoochoose_tabular_transformer_features
 
     body = tr.SequentialBlock(
         input_module,
         tr.MLPBlock([64]),
-        pytorch.nn.GRU(input_size=64, hidden_size=64, num_layers=2),
+        torch.nn.GRU(input_size=64, hidden_size=64, num_layers=2),
         output_size=[None, 20, 64],
     )
     head = tr.Head(
         body,
         tr.NextItemPredictionTask(weight_tying=True),
         inputs=input_module,
     )
@@ -233,15 +233,15 @@
     torch_yoochoose_tabular_transformer_features, torch_yoochoose_like
 ):
     input_module = torch_yoochoose_tabular_transformer_features
 
     body = tr.SequentialBlock(
         input_module,
         tr.MLPBlock([64]),
-        tr.Block(pytorch.nn.GRU(input_size=64, hidden_size=64, num_layers=2), [None, 20, 64]),
+        tr.Block(torch.nn.GRU(input_size=64, hidden_size=64, num_layers=2), [None, 20, 64]),
     )
     head = tr.Head(
         body,
         tr.NextItemPredictionTask(weight_tying=True),
         inputs=input_module,
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/model/test_model.py` & `transformers4rec-23.4.0/tests/unit/torch/model/test_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,25 @@
 import os
 import tempfile
 
 import pytest
 import torch
 from merlin.schema import Schema as Core_Schema
 
+import transformers4rec.torch as tr
 from transformers4rec.config import transformer as tconf
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
-
-if pytorch.cuda.is_available():
+if torch.cuda.is_available():
     devices = ["cpu", "cuda"]
 else:
     devices = ["cpu"]
 
 
 def test_simple_model(torch_tabular_features, torch_tabular_data):
-    targets = {"target": pytorch.randint(2, (100,)).float()}
+    targets = {"target": torch.randint(2, (100,)).float()}
 
     inputs = torch_tabular_features
     body = tr.SequentialBlock(inputs, tr.MLPBlock([64]))
     model = tr.BinaryClassificationTask("target").to_model(body, inputs)
 
     dataset = [(torch_tabular_data, targets)]
     losses = model.fit(dataset, num_epochs=5)
@@ -53,14 +51,50 @@
 
     # assert list(metrics.keys()) == ["precision", "recall", "accuracy"]
     assert len(metrics) == 3
     assert len(losses) == 5
     assert all(loss.min() >= 0 and loss.max() <= 1 for loss in losses)
 
 
+def test_sequential_prediction_model_with_ragged_inputs(torch_yoochoose_like, yoochoose_schema):
+    input_module = tr.TabularSequenceFeatures.from_schema(
+        yoochoose_schema,
+        max_sequence_length=20,
+        d_output=64,
+        masking="causal",
+    )
+    prediction_task = tr.NextItemPredictionTask(weight_tying=True)
+    transformer_config = tconf.XLNetConfig.build(
+        d_model=64, n_head=8, n_layer=2, total_seq_length=20
+    )
+    model = transformer_config.to_torch_model(input_module, prediction_task)
+
+    _ = model(torch_yoochoose_like)
+
+    model.eval()
+
+    inference_inputs = tr.data.tabular_sequence_testing_data.torch_synthetic_data(
+        num_rows=10, min_session_length=1, max_session_length=4, ragged=True
+    )
+    inference_inputs_2 = tr.data.tabular_sequence_testing_data.torch_synthetic_data(
+        num_rows=20, min_session_length=1, max_session_length=10, ragged=True
+    )
+    model_output = model(inference_inputs)
+
+    # if the model is traced with ragged inputs it can only be called with ragged inputs
+    # if the model is traced with padded inputs it can only be called with padded inputs
+    traced_model = torch.jit.trace(model, inference_inputs, strict=False)
+    traced_model_output = traced_model(inference_inputs)
+    assert torch.equal(model_output, traced_model_output)
+
+    model_output = model(inference_inputs_2)
+    traced_model_output = traced_model(inference_inputs_2)
+    assert torch.equal(model_output, traced_model_output)
+
+
 @pytest.mark.parametrize("task", [tr.BinaryClassificationTask, tr.RegressionTask])
 def test_sequential_prediction_model(
     torch_yoochoose_tabular_transformer_features, torch_yoochoose_like, task
 ):
     inputs = torch_yoochoose_tabular_transformer_features
 
     transformer_config = tconf.XLNetConfig.build(
@@ -71,34 +105,84 @@
     head_1 = tr.Head(
         body,
         tr.NextItemPredictionTask(weight_tying=True),
         inputs=inputs,
     )
     head_2 = task("target", summary_type="mean").to_head(body, inputs)
 
-    bc_targets = pytorch.randint(2, (100,)).float()
+    bc_targets = torch.randint(2, (100,)).float()
 
     model = tr.Model(head_1, head_2)
     output = model(torch_yoochoose_like, training=True, targets=bc_targets)
 
     assert isinstance(output, dict)
     assert len(list(output.keys())) == 3
     assert len(list(output["predictions"])) == 2
     assert set(list(output.keys())) == set(["loss", "labels", "predictions"])
 
+    # test inference inputs with only one item
+    inference_inputs = tr.data.tabular_sequence_testing_data.torch_synthetic_data(
+        num_rows=10, min_session_length=1, max_session_length=1
+    )
+    _ = model(inference_inputs)
+
+
+def test_sequential_binary_classification_model(
+    torch_yoochoose_tabular_transformer_features,
+    torch_yoochoose_like,
+):
+    bs, max_len = 100, 20
+    wrong_target = {"target": torch.randint(2, (bs,)).float()}
+    targets = {"sequential_target": torch.randint(2, (bs, max_len)).float()}
+
+    inputs = torch_yoochoose_tabular_transformer_features
+    transformer_config = tconf.XLNetConfig.build(
+        d_model=64, n_head=4, n_layer=2, total_seq_length=max_len
+    )
+    body = tr.SequentialBlock(inputs, tr.MLPBlock([64]), tr.TransformerBlock(transformer_config))
+
+    with pytest.raises(ValueError) as excinfo:
+        head = tr.Head(
+            body,
+            tr.BinaryClassificationTask("target", summary_type=None),
+            inputs=inputs,
+        )
+        model = tr.Model(head)
+        dataset = [(torch_yoochoose_like, wrong_target)]
+        losses = model.fit(dataset, num_epochs=1)
+    assert "If `summary_type==None`, targets are expected to be a 2D tensor" in str(excinfo.value)
+
+    head = tr.Head(
+        body,
+        tr.BinaryClassificationTask("sequential_target", summary_type=None),
+        inputs=inputs,
+    )
+    model = tr.Model(head)
+
+    dataset = [(torch_yoochoose_like, targets)]
+    losses = model.fit(dataset, num_epochs=5)
+    metrics = model.evaluate(dataset, mode="eval")
+
+    assert len(metrics) == 3
+    assert len(losses) == 5
+    assert all(loss.min() >= 0 and loss.max() <= 1 for loss in losses)
+
+    predictions = model(torch_yoochoose_like)
+    assert predictions.shape == (bs, max_len)
+
 
 def test_model_with_multiple_heads_and_tasks(
     yoochoose_schema,
     torch_yoochoose_tabular_transformer_features,
     torch_yoochoose_like,
 ):
     # Tabular classification and regression tasks
     targets = {
-        "classification": pytorch.randint(2, (100,)).float(),
-        "regression": pytorch.randint(2, (100,)).float(),
+        "classification": torch.randint(2, (100,)).float(),
+        "regression": torch.randint(2, (100,)).float(),
     }
 
     non_sequential_features_schema = yoochoose_schema.select_by_name(["user_age", "user_country"])
 
     tabular_features = tr.TabularFeatures.from_schema(
         non_sequential_features_schema,
         max_sequence_length=20,
@@ -111,16 +195,16 @@
         tr.BinaryClassificationTask("classification"),
         tr.RegressionTask("regression"),
     ]
     head_1 = tr.Head(body, tasks)
 
     # Session-based classification and regression tasks
     targets_2 = {
-        "classification_session": pytorch.randint(2, (100,)).float(),
-        "regression_session": pytorch.randint(2, (100,)).float(),
+        "classification_session": torch.randint(2, (100,)).float(),
+        "regression_session": torch.randint(2, (100,)).float(),
     }
     transformer_config = tconf.XLNetConfig.build(
         d_model=64, n_head=4, n_layer=2, total_seq_length=20
     )
     body_2 = tr.SequentialBlock(
         torch_yoochoose_tabular_transformer_features,
         tr.MLPBlock([64]),
@@ -286,14 +370,29 @@
         masking="mlm",
     )
     task = tr.NextItemPredictionTask(weight_tying=True)
     model = transformer_config.to_torch_model(input_module, task)
     assert model(torch_yoochoose_like, training=True)
 
 
+def test_with_next_item_pred_sampled_softmax(torch_yoochoose_like, yoochoose_schema):
+    d_model = 32
+    transformer_config = tconf.XLNetConfig.build(d_model, 4, 2, 20)
+    input_module = tr.TabularSequenceFeatures.from_schema(
+        yoochoose_schema,
+        max_sequence_length=20,
+        continuous_projection=64,
+        d_output=32,
+        masking="mlm",
+    )
+    task = tr.NextItemPredictionTask(weight_tying=True, sampled_softmax=True, max_n_samples=1000)
+    model = transformer_config.to_torch_model(input_module, task)
+    assert model(torch_yoochoose_like, training=True)
+
+
 @pytest.mark.parametrize("masking", ["causal", "mlm", "plm", "rtd"])
 def test_output_shape_mode_eval(torch_yoochoose_like, yoochoose_schema, masking):
     input_module = tr.TabularSequenceFeatures.from_schema(
         yoochoose_schema,
         max_sequence_length=20,
         d_output=64,
         masking=masking,
```

### Comparing `transformers4rec-23.2.0/tests/torch/tabular/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/tabular/test_aggregation.py` & `transformers4rec-23.4.0/tests/unit/torch/tabular/test_aggregation.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag
-
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_concat_aggregation_yoochoose(tabular_schema, torch_tabular_data):
     schema = tabular_schema
     tab_module = tr.features.tabular.TabularFeatures.from_schema(schema)
 
     block = tab_module >> tr.ConcatFeatures()
@@ -45,16 +44,16 @@
     assert out.shape[2] == 4
 
 
 def test_element_wise_sum_features_different_shapes():
     with pytest.raises(ValueError) as excinfo:
         element_wise_op = tr.ElementwiseSum()
         input = {
-            "item_id/list": pytorch.rand(10, 20),
-            "category/list": pytorch.rand(10, 25),
+            "item_id/list": torch.rand(10, 20),
+            "category/list": torch.rand(10, 25),
         }
         element_wise_op(input)
     assert "shapes of all input features are not equal" in str(excinfo.value)
 
 
 def test_element_wise_sum_aggregation_yoochoose(tabular_schema, torch_tabular_data):
     schema = tabular_schema
@@ -72,29 +71,29 @@
         element_wise_op = tr.ElementwiseSumItemMulti()
         element_wise_op(None)
     assert "requires a schema" in str(excinfo.value)
 
 
 def test_element_wise_sum_item_multi_col_group_no_item_id(yoochoose_schema):
     with pytest.raises(ValueError) as excinfo:
-        categ_schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+        categ_schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
         # Remove the item id from col_group
         categ_schema = categ_schema.remove_by_name("item_id/list")
         element_wise_op = tr.ElementwiseSumItemMulti(categ_schema)
         element_wise_op(None)
     assert "no column tagged as item id" in str(excinfo.value)
 
 
 def test_element_wise_sum_item_multi_features_different_shapes(yoochoose_schema):
     with pytest.raises(ValueError) as excinfo:
-        categ_schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+        categ_schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
         element_wise_op = tr.ElementwiseSumItemMulti(categ_schema)
         input = {
-            "item_id/list": pytorch.rand(10, 20),
-            "category/list": pytorch.rand(10, 25),
+            "item_id/list": torch.rand(10, 20),
+            "category/list": torch.rand(10, 25),
         }
         element_wise_op(input)
     assert "shapes of all input features are not equal" in str(excinfo.value)
 
 
 def test_element_wise_sum_item_multi_aggregation_yoochoose(yoochoose_schema, torch_yoochoose_like):
     schema = yoochoose_schema
@@ -106,15 +105,15 @@
 
     assert out.shape[-1] == 64
 
 
 def test_element_wise_sum_item_multi_aggregation_registry_yoochoose(
     yoochoose_schema, torch_yoochoose_like
 ):
-    categ_schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    categ_schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
 
     tab_module = tr.TabularSequenceFeatures.from_schema(
         categ_schema, aggregation="element-wise-sum-item-multi"
     )
 
     out = tab_module(torch_yoochoose_like)
```

### Comparing `transformers4rec-23.2.0/tests/torch/tabular/test_tabular.py` & `transformers4rec-23.4.0/tests/unit/torch/tabular/test_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 import torch
 
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 if torch.cuda.is_available():
     devices = ["cpu", "cuda"]
 else:
     devices = ["cpu"]
```

### Comparing `transformers4rec-23.2.0/tests/torch/tabular/test_transformations.py` & `transformers4rec-23.4.0/tests/unit/torch/tabular/test_transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
+from merlin.schema import Tags
 
-from merlin_standard_lib import Tag, schema
-
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
+from merlin_standard_lib import schema
 
 
 @pytest.mark.parametrize("replacement_prob", [0.1, 0.3, 0.5, 0.7])
 def test_stochastic_swap_noise(replacement_prob):
     NUM_SEQS = 100
     SEQ_LENGTH = 80
     PAD_TOKEN = 0
 
     # Creating some input sequences with padding in the end
     # (to emulate sessions with different lengths)
     seq_inputs = {
-        "categ_seq_feat": pytorch.tril(
-            pytorch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH)), 1
+        "categ_seq_feat": torch.tril(
+            torch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH)), 1
         ),
-        "cont_seq_feat": pytorch.tril(pytorch.rand((NUM_SEQS, SEQ_LENGTH)), 1),
-        "categ_non_seq_feat": pytorch.randint(low=1, high=100, size=(NUM_SEQS,)),
+        "cont_seq_feat": torch.tril(torch.rand((NUM_SEQS, SEQ_LENGTH)), 1),
+        "categ_non_seq_feat": torch.randint(low=1, high=100, size=(NUM_SEQS,)),
     }
 
     ssn = tr.StochasticSwapNoise(pad_token=PAD_TOKEN, replacement_prob=replacement_prob)
     out_features_ssn = ssn(seq_inputs, input_mask=seq_inputs["categ_seq_feat"] != PAD_TOKEN)
 
     for fname in seq_inputs:
         replaced_mask = out_features_ssn[fname] != seq_inputs[fname]
-        replaced_mask_non_padded = pytorch.masked_select(
+        replaced_mask_non_padded = torch.masked_select(
             replaced_mask, seq_inputs[fname] != PAD_TOKEN
         )
         replacement_rate = replaced_mask_non_padded.float().mean()
         assert replacement_rate == pytest.approx(replacement_prob, abs=0.15)
 
 
 @pytest.mark.parametrize("replacement_prob", [0.1, 0.3, 0.5, 0.7])
@@ -55,29 +55,29 @@
     NUM_SEQS = 100
     SEQ_LENGTH = 80
     PAD_TOKEN = 0
 
     # Creating some input sequences with padding in the end
     # (to emulate sessions with different lengths)
     seq_inputs = {
-        "categ_seq_feat": pytorch.tril(
-            pytorch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH)), 1
+        "categ_seq_feat": torch.tril(
+            torch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH)), 1
         ),
-        "cont_seq_feat": pytorch.tril(pytorch.rand((NUM_SEQS, SEQ_LENGTH)), 1),
-        "categ_non_seq_feat": pytorch.randint(low=1, high=100, size=(NUM_SEQS,)),
+        "cont_seq_feat": torch.tril(torch.rand((NUM_SEQS, SEQ_LENGTH)), 1),
+        "categ_non_seq_feat": torch.randint(low=1, high=100, size=(NUM_SEQS,)),
     }
 
     ssn = tr.StochasticSwapNoise(pad_token=PAD_TOKEN, replacement_prob=replacement_prob)
     # Set the eval mode and checks that swap noise is not applied on eval
     ssn.eval()
     out_features_ssn = ssn(seq_inputs, input_mask=seq_inputs["categ_seq_feat"] != PAD_TOKEN)
 
     for fname in seq_inputs:
         replaced_mask = out_features_ssn[fname] == seq_inputs[fname]
-        assert pytorch.all(replaced_mask)
+        assert torch.all(replaced_mask)
 
 
 @pytest.mark.parametrize("replacement_prob", [0.1, 0.3, 0.5, 0.7])
 def test_stochastic_swap_noise_with_tabular_features(
     yoochoose_schema, torch_yoochoose_like, replacement_prob
 ):
     PAD_TOKEN = 0
@@ -95,15 +95,15 @@
         replaced_mask = out_features_ssn[fname] != out_features[fname]
 
         # Ignoring padding items to compute the mean replacement rate
         feat_non_padding_mask = inputs[fname] != PAD_TOKEN
         # For embedding features it is necessary to expand the mask
         if len(replaced_mask.shape) > len(feat_non_padding_mask.shape):
             feat_non_padding_mask = feat_non_padding_mask.unsqueeze(-1)
-        replaced_mask_non_padded = pytorch.masked_select(replaced_mask, feat_non_padding_mask)
+        replaced_mask_non_padded = torch.masked_select(replaced_mask, feat_non_padding_mask)
         replacement_rate = replaced_mask_non_padded.float().mean()
         assert replacement_rate == pytest.approx(replacement_prob, abs=0.15)
 
 
 @pytest.mark.parametrize("replacement_prob", [0.1, 0.3, 0.5, 0.7])
 def test_stochastic_swap_noise_with_tabular_features_from_schema(
     yoochoose_schema, torch_yoochoose_like, replacement_prob
@@ -130,22 +130,22 @@
         replaced_mask = out_features_ssn[fname] != out_features[fname]
 
         # Ignoring padding items to compute the mean replacement rate
         feat_non_padding_mask = inputs[fname] != PAD_TOKEN
         # For embedding features it is necessary to expand the mask
         if len(replaced_mask.shape) > len(feat_non_padding_mask.shape):
             feat_non_padding_mask = feat_non_padding_mask.unsqueeze(-1)
-        replaced_mask_non_padded = pytorch.masked_select(replaced_mask, feat_non_padding_mask)
+        replaced_mask_non_padded = torch.masked_select(replaced_mask, feat_non_padding_mask)
         replacement_rate = replaced_mask_non_padded.float().mean()
         assert replacement_rate == pytest.approx(replacement_prob, abs=0.20)
 
 
 @pytest.mark.parametrize("layer_norm", ["layer-norm", tr.TabularLayerNorm()])
 def test_layer_norm(yoochoose_schema, torch_yoochoose_like, layer_norm):
-    schema = yoochoose_schema.select_by_tag(Tag.CATEGORICAL)
+    schema = yoochoose_schema.select_by_tag(Tags.CATEGORICAL)
 
     emb_module = tr.EmbeddingFeatures.from_schema(
         schema, embedding_dims={"item_id/list": 100}, embedding_dim_default=64, post=layer_norm
     )
 
     out = emb_module(torch_yoochoose_like)
 
@@ -172,47 +172,46 @@
         ]
     )
 
     layer_norm = tr.TabularLayerNorm()
     tab_module = tr.TabularSequenceFeatures.from_schema(schema, post=layer_norm)
     out_features = tab_module(inputs)
 
-    assert pytorch.all(
+    assert torch.all(
         out_features["timestamp/weekday/sin/list"]
         == inputs["timestamp/weekday/sin/list"].unsqueeze(-1)
     )
-    assert pytorch.all(
+    assert torch.all(
         out_features["timestamp/weekday/cos/list"]
         == inputs["timestamp/weekday/cos/list"].unsqueeze(-1)
     )
 
     # Check if layer norm was applied to categ features
     assert out_features["item_id/list"].mean(axis=-1).mean().item() == pytest.approx(0.0, abs=0.02)
     assert out_features["item_id/list"].std(axis=-1).mean().item() == pytest.approx(1.0, abs=0.02)
     assert out_features["category/list"].mean(axis=-1).mean().item() == pytest.approx(0.0, abs=0.02)
     assert out_features["category/list"].std(axis=-1).mean().item() == pytest.approx(1.0, abs=0.02)
 
 
 def test_stochastic_swap_noise_raise_exception_not_2d_item_id():
-
     s = schema.Schema(
         [
             schema.ColumnSchema.create_categorical(
-                "item_id_feat", num_items=1000, tags=[Tag.ITEM_ID.value]
+                "item_id_feat", num_items=1000, tags=[Tags.ITEM_ID]
             ),
         ]
     )
 
     NUM_SEQS = 100
     SEQ_LENGTH = 80
     PAD_TOKEN = 0
 
     seq_inputs = {
-        "item_id_feat": pytorch.tril(
-            pytorch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH, 64)), 1
+        "item_id_feat": torch.tril(
+            torch.randint(low=1, high=100, size=(NUM_SEQS, SEQ_LENGTH, 64)), 1
         ),
     }
 
     ssn = tr.StochasticSwapNoise(pad_token=PAD_TOKEN, replacement_prob=0.3, schema=s)
 
     with pytest.raises(ValueError) as excinfo:
         ssn(seq_inputs)
@@ -224,16 +223,16 @@
 def test_dropout_transformation():
     NUM_SEQS = 100
     SEQ_LENGTH = 80
 
     DROPOUT_RATE = 0.3
 
     inputs = {
-        "embedded_feat": pytorch.rand((NUM_SEQS, SEQ_LENGTH, 10)),
-        "continuous_feat": pytorch.rand((NUM_SEQS, SEQ_LENGTH)),
+        "embedded_feat": torch.rand((NUM_SEQS, SEQ_LENGTH, 10)),
+        "continuous_feat": torch.rand((NUM_SEQS, SEQ_LENGTH)),
     }
 
     input_dropout = tr.TabularDropout(dropout_rate=DROPOUT_RATE)
     out_features = input_dropout(inputs)
 
     for fname in inputs:
         input_zeros_rate = (inputs[fname] == 0.0).float().mean()
@@ -250,15 +249,15 @@
     out_features = tab_module(inputs)
 
     input_dropout = tr.TabularDropout(dropout_rate=DROPOUT_RATE)
     out_features_dropout = tab_module(inputs, post=input_dropout)
 
     for fname in out_features:
         mask_prev_not_zeros = out_features[fname] != 0.0
-        out_features_dropout_ignoring_zeroes = pytorch.masked_select(
+        out_features_dropout_ignoring_zeroes = torch.masked_select(
             out_features_dropout[fname], mask_prev_not_zeros
         )
         output_dropout_zeros_rate = (out_features_dropout_ignoring_zeroes == 0.0).float().mean()
         assert output_dropout_zeros_rate == pytest.approx(DROPOUT_RATE, abs=0.2)
 
 
 def test_input_dropout_with_tabular_features_post_from_squema(
@@ -283,12 +282,12 @@
 
     input_dropout = tr.TabularDropout(dropout_rate=DROPOUT_RATE)
     tab_module_dropout = tr.TabularSequenceFeatures.from_schema(schema, post=input_dropout)
     out_features_dropout = tab_module_dropout(inputs)
 
     for fname in out_features:
         mask_prev_not_zeros = out_features[fname] != 0.0
-        out_features_dropout_ignoring_zeroes = pytorch.masked_select(
+        out_features_dropout_ignoring_zeroes = torch.masked_select(
             out_features_dropout[fname], mask_prev_not_zeros
         )
         output_dropout_zeros_rate = (out_features_dropout_ignoring_zeroes == 0.0).float().mean()
         assert output_dropout_zeros_rate == pytest.approx(DROPOUT_RATE, abs=0.1)
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_dataloader_utils.py` & `transformers4rec-23.4.0/tests/unit/torch/test_dataloader_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
 
-torch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_pyarrow_load(yoochoose_schema, yoochoose_path_file):
     pytest.importorskip("pyarrow")
     max_sequence_length = 20
     batch_size = 16
     loader = tr.utils.data_utils.PyarrowDataLoader.from_schema(
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_experimental.py` & `transformers4rec-23.4.0/tests/unit/torch/test_experimental.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 
+import transformers4rec.torch as tr
 from transformers4rec.config import transformer as tconf
 from transformers4rec.torch.experimental import PostContextFusion
 
-tr = pytest.importorskip("transformers4rec.torch")
-pytorch = pytest.importorskip("torch")
-
 
 @pytest.mark.parametrize("fusion_aggregation", ["concat", "elementwise-mul", "elementwise-sum"])
 def test_post_fusion_context_block(yoochoose_schema, torch_yoochoose_like, fusion_aggregation):
-
     tab_module = tr.TabularSequenceFeatures.from_schema(
         yoochoose_schema,
         max_sequence_length=20,
         aggregation="concat",
         d_output=64,
         masking="causal",
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_masking.py` & `transformers4rec-23.4.0/tests/unit/torch/test_masking.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import numpy as np
 import pytest
+import torch
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 # fixed parameters for tests
 lm_tasks = list(tr.masking.masking_registry.keys())
 
 
 # Test output shapes
 @pytest.mark.parametrize("task", lm_tasks)
@@ -43,17 +42,17 @@
     hidden_dim = torch_masking_inputs["input_tensor"].size(2)
     lm = tr.masking.masking_registry[task](
         hidden_dim, padding_idx=torch_masking_inputs["padding_idx"]
     )
     lm.compute_masked_targets(torch_masking_inputs["labels"], training=False)
     # get non padded last items
     non_padded_mask = torch_masking_inputs["labels"] != torch_masking_inputs["padding_idx"]
-    rows_ids = pytorch.arange(
+    rows_ids = torch.arange(
         torch_masking_inputs["labels"].size(0),
-        dtype=pytorch.long,
+        dtype=torch.long,
         device=torch_masking_inputs["labels"].device,
     )
     last_item_sessions = non_padded_mask.sum(axis=1) - 1
     last_labels = torch_masking_inputs["labels"][rows_ids, last_item_sessions].flatten().numpy()
     # get the last labels from output
     trgt_pad = lm.masked_targets != torch_masking_inputs["padding_idx"]
     out_last = lm.masked_targets[trgt_pad].flatten().numpy()
@@ -96,17 +95,17 @@
         hidden_dim,
         padding_idx=torch_masking_inputs["padding_idx"],
         train_on_last_item_seq_only=True,
     )
     lm.compute_masked_targets(torch_masking_inputs["labels"], training=True)
     # get non padded last items
     non_padded_mask = torch_masking_inputs["labels"] != torch_masking_inputs["padding_idx"]
-    rows_ids = pytorch.arange(
+    rows_ids = torch.arange(
         torch_masking_inputs["labels"].size(0),
-        dtype=pytorch.long,
+        dtype=torch.long,
         device=torch_masking_inputs["labels"].device,
     )
     last_item_sessions = non_padded_mask.sum(axis=1) - 1
     last_labels = torch_masking_inputs["labels"][rows_ids, last_item_sessions].flatten().numpy()
     # last labels from output
     trgt_pad = lm.masked_targets != torch_masking_inputs["padding_idx"]
     out_last = lm.masked_targets[trgt_pad].flatten().numpy()
@@ -170,17 +169,15 @@
     )
     masking_info = lm.compute_masked_targets(torch_masking_inputs["labels"], training=True)
     trg_flat = masking_info.targets.flatten()
     non_pad_mask = trg_flat != torch_masking_inputs["padding_idx"]
     # Nb of pos items
     pos_items = non_pad_mask.sum()
     # generate random logits
-    logits = pytorch.tensor(
-        np.random.uniform(0, 1, (pos_items, torch_masking_inputs["vocab_size"]))
-    )
+    logits = torch.tensor(np.random.uniform(0, 1, (pos_items, torch_masking_inputs["vocab_size"])))
     corrupted_inputs, discriminator_labels, _ = lm.get_fake_tokens(
         torch_masking_inputs["labels"], trg_flat, logits
     )
     replacement_mask = discriminator_labels != 0
     assert all(lm.mask_schema[replacement_mask] == 1)
 
 
@@ -193,15 +190,15 @@
     masking_info = lm.compute_masked_targets(torch_masking_inputs["labels"], training=True)
 
     trg_flat = masking_info.targets.flatten()
     non_pad_mask = trg_flat != torch_masking_inputs["padding_idx"]
     # Nb of pos items
     pos_items = non_pad_mask.sum()
     # generate random logits
-    logits = pytorch.tensor(np.random.uniform(0, 1, (pos_items, pos_items)))
+    logits = torch.tensor(np.random.uniform(0, 1, (pos_items, pos_items)))
     corrupted_inputs, discriminator_labels, updates = lm.get_fake_tokens(
         torch_masking_inputs["labels"], trg_flat, logits
     )
     replacement_mask = discriminator_labels != 0
     assert set(corrupted_inputs[replacement_mask].numpy()).issubset(trg_flat[non_pad_mask].numpy())
 
 
@@ -213,22 +210,22 @@
     )
     masking_info = lm.compute_masked_targets(torch_masking_inputs["labels"], training=True)
     trg_flat = masking_info.targets.flatten()
     non_pad_mask = trg_flat != torch_masking_inputs["padding_idx"]
     # Nb of pos items
     pos_items = non_pad_mask.sum()
     # generate random logits
-    logits = pytorch.tensor(np.random.uniform(0, 1, (pos_items, pos_items)))
+    logits = torch.tensor(np.random.uniform(0, 1, (pos_items, pos_items)))
     updates = lm.sample_from_softmax(logits)
     assert updates.size(0) == pos_items
 
 
 @pytest.mark.parametrize("mode", [True, False])
 def test_masked_positions(torch_masking_inputs, mode):
     hidden_dim = torch_masking_inputs["input_tensor"].size(2)
     lm = tr.masking.ReplacementLanguageModeling(
         hidden_dim, padding_idx=torch_masking_inputs["padding_idx"], sample_from_batch=True
     )
     masking_info = lm.compute_masked_targets(torch_masking_inputs["labels"], training=mode)
 
-    targets = pytorch.masked_select(masking_info.targets, masking_info.schema)
+    targets = torch.masked_select(masking_info.targets, masking_info.schema)
     assert all(targets != torch_masking_inputs["padding_idx"])
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_public_api.py` & `transformers4rec-23.4.0/tests/unit/torch/test_public_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 transformer_config_names = [
     "AlbertConfig",
     "ElectraConfig",
     "GPT2Config",
     "LongformerConfig",
     "ReformerConfig",
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_ranking_metrics.py` & `transformers4rec-23.4.0/tests/unit/torch/test_ranking_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 import torch
 
+import transformers4rec.torch as tr
 from transformers4rec.torch.ranking_metric import MeanReciprocalRankAt
 
-tr = pytest.importorskip("transformers4rec.torch")
-
 # fixed parameters for tests
 list_metrics = list(tr.ranking_metric.ranking_metrics_registry.keys())
 
 
 # Test length of output equal to number of cutoffs
 @pytest.mark.parametrize("metric", list_metrics)
 def test_avg_precision_at(torch_ranking_metrics_inputs, metric):
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_readme.py` & `transformers4rec-23.4.0/tests/unit/torch/test_readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import pytest
-
-tr = pytest.importorskip("transformers4rec.torch")
+import transformers4rec.torch as tr
 
 
 def test_readme_quick_start_example_pytorch():
     schema: tr.Schema = tr.data.tabular_sequence_testing_data.schema
     # Or read schema from disk: tr.Schema().from_json(SCHEMA_PATH)
     max_sequence_length, d_model = 20, 64
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_torchscript.py` & `transformers4rec-23.4.0/tests/unit/torch/test_torchscript.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import pytest
+import torch
 
+import transformers4rec.torch as tr
 from transformers4rec.config import transformer as tconf
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
-
 
 def test_torchsciprt_not_strict(torch_yoochoose_like, yoochoose_schema):
-
     input_module = tr.TabularSequenceFeatures.from_schema(
         yoochoose_schema,
         max_sequence_length=20,
         d_output=64,
         masking="causal",
     )
     prediction_task = tr.NextItemPredictionTask(weight_tying=True)
@@ -20,13 +17,12 @@
     )
     model = transformer_config.to_torch_model(input_module, prediction_task)
 
     _ = model(torch_yoochoose_like, training=False)
 
     model.eval()
 
-    traced_model = pytorch.jit.trace(model, torch_yoochoose_like, strict=False)
-    assert isinstance(traced_model, pytorch.jit.TopLevelTracedModule)
-    assert pytorch.allclose(
-        model(torch_yoochoose_like),
-        traced_model(torch_yoochoose_like),
+    traced_model = torch.jit.trace(model, torch_yoochoose_like, strict=False)
+    assert isinstance(traced_model, torch.jit.TopLevelTracedModule)
+    assert torch.allclose(
+        model(torch_yoochoose_like), traced_model(torch_yoochoose_like), rtol=1e-02
     )
```

### Comparing `transformers4rec-23.2.0/tests/torch/test_trainer.py` & `transformers4rec-23.4.0/tests/unit/torch/test_trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 # limitations under the License.
 #
 
 import os
 import tempfile
 
 import pytest
+import torch
+from merlin.schema import Schema
 
+import transformers4rec.torch as tr
 from transformers4rec.config import trainer
 from transformers4rec.config import transformer as tconf
 
-pytorch = pytest.importorskip("torch")
-tr = pytest.importorskip("transformers4rec.torch")
-
 
 @pytest.mark.parametrize("batch_size", [16, 32])
 def test_set_train_eval_loaders_attributes(
     torch_yoochoose_like, torch_yoochoose_next_item_prediction_model, batch_size
 ):
-    train_loader = pytorch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size)
+    train_loader = torch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size)
     train_loader._batch_size = batch_size
-    eval_loader = pytorch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size // 2)
+    eval_loader = torch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size // 2)
     eval_loader._batch_size = batch_size // 2
-    test_loader = pytorch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size // 2)
+    test_loader = torch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size // 2)
     test_loader._batch_size = batch_size // 2
 
     args = trainer.T4RecTrainingArguments(
         output_dir=".",
         max_steps=5,
         max_sequence_length=20,
         per_device_train_batch_size=batch_size,
@@ -54,31 +54,34 @@
 
     assert recsys_trainer.get_train_dataloader() == train_loader
     assert recsys_trainer.get_eval_dataloader() == eval_loader
     assert recsys_trainer.get_test_dataloader() == test_loader
 
 
 @pytest.mark.parametrize("batch_size", [16, 32])
-def test_set_train_eval_loaders_pyarrow(torch_yoochoose_next_item_prediction_model, batch_size):
-
+@pytest.mark.parametrize("schema_type", ["msl", "core"])
+def test_set_train_eval_loaders_pyarrow(
+    torch_yoochoose_next_item_prediction_model, batch_size, schema_type
+):
     data = tr.data.tabular_sequence_testing_data
+    schema = data.schema if schema_type == "msl" else data.merlin_schema
     args = trainer.T4RecTrainingArguments(
         output_dir=".",
         max_steps=5,
         num_train_epochs=1,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size // 2,
         data_loader_engine="pyarrow",
         fp16=False,
         no_cuda=True,
     )
     resys_trainer = tr.Trainer(
         model=torch_yoochoose_next_item_prediction_model,
         args=args,
-        schema=data.schema,
+        schema=schema,
         train_dataset_or_path=data.path,
         eval_dataset_or_path=data.path,
     )
 
     assert resys_trainer.get_train_dataloader().batch_size == batch_size
     assert resys_trainer.get_eval_dataloader().batch_size == batch_size // 2
 
@@ -137,15 +140,16 @@
     )
 
     recsys_trainer.reset_lr_scheduler()
     result = recsys_trainer.train()
     assert result
 
 
-def test_trainer_eval_loop(torch_yoochoose_next_item_prediction_model):
+@pytest.mark.parametrize("schema_type", ["msl", "core"])
+def test_trainer_eval_loop(torch_yoochoose_next_item_prediction_model, schema_type):
     pytest.importorskip("pyarrow")
     batch_size = 16
     args = trainer.T4RecTrainingArguments(
         output_dir=".",
         max_steps=5,
         num_train_epochs=1,
         per_device_train_batch_size=batch_size,
@@ -155,18 +159,19 @@
         fp16=False,
         no_cuda=True,
         report_to=[],
         debug=["r"],
     )
 
     data = tr.data.tabular_sequence_testing_data
+    schema = data.schema if schema_type == "msl" else data.merlin_schema
     recsys_trainer = tr.Trainer(
         model=torch_yoochoose_next_item_prediction_model,
         args=args,
-        schema=data.schema,
+        schema=schema,
         train_dataset_or_path=data.path,
         eval_dataset_or_path=data.path,
         test_dataset_or_path=data.path,
         compute_metrics=True,
     )
 
     eval_metrics = recsys_trainer.evaluate(eval_dataset=data.path, metric_key_prefix="eval")
@@ -349,14 +354,16 @@
         max_sequence_length=20,
         d_output=64,
         masking="mlm",
     )
     transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
     model = transformer_config.to_torch_model(inputs, task)
 
+    assert isinstance(model.input_schema, Schema)
+
     args = trainer.T4RecTrainingArguments(
         output_dir=".",
         max_steps=5,
         num_train_epochs=1,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size // 2,
         data_loader_engine="merlin_dataloader",
@@ -381,20 +388,109 @@
     predictions = recsys_trainer.predict(data.path)
 
     assert isinstance(eval_metrics, dict)
     assert set(default_metric).issubset(set(eval_metrics.keys()))
     assert eval_metrics["eval_/loss"] is not None
 
     assert predictions is not None
+    # 1000 is the total samples in the testing data
+    if isinstance(task, tr.NextItemPredictionTask):
+        assert predictions.predictions.shape == (1000, task.target_dim)
+    else:
+        assert predictions.predictions.shape == (1000,)
 
 
-def test_trainer_with_multiple_tasks():
+# This is broken out as a separate test since combining it leads to strange errors
+@pytest.mark.parametrize(
+    "task_and_metrics",
+    [
+        (
+            tr.NextItemPredictionTask(weight_tying=True),
+            [
+                "eval_/next-item/ndcg_at_10",
+                "eval_/next-item/ndcg_at_20",
+                "eval_/next-item/avg_precision_at_10",
+                "eval_/next-item/avg_precision_at_20",
+                "eval_/next-item/recall_at_10",
+                "eval_/next-item/recall_at_20",
+            ],
+        ),
+        (
+            tr.BinaryClassificationTask("click", summary_type="mean"),
+            [
+                "eval_/click/binary_classification_task/binary_accuracy",
+                "eval_/click/binary_classification_task/binary_precision",
+                "eval_/click/binary_classification_task/binary_recall",
+            ],
+        ),
+        (
+            tr.RegressionTask("play_percentage", summary_type="mean"),
+            [
+                "eval_/play_percentage/regression_task/mean_squared_error",
+            ],
+        ),
+    ],
+)
+def test_trainer_music_streaming_core_schema(task_and_metrics):
     data = tr.data.music_streaming_testing_data
-    schema = data.schema
+    schema = data.merlin_schema
     batch_size = 16
+    task, default_metric = task_and_metrics
+
+    inputs = tr.TabularSequenceFeatures.from_schema(
+        schema,
+        max_sequence_length=20,
+        d_output=64,
+        masking="mlm",
+    )
+    transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
+    model = transformer_config.to_torch_model(inputs, task)
+
+    assert isinstance(model.input_schema, Schema)
+
+    args = trainer.T4RecTrainingArguments(
+        output_dir=".",
+        max_steps=5,
+        num_train_epochs=1,
+        per_device_train_batch_size=batch_size,
+        per_device_eval_batch_size=batch_size // 2,
+        data_loader_engine="merlin_dataloader",
+        max_sequence_length=20,
+        fp16=False,
+        report_to=[],
+        debug=["r"],
+    )
+
+    recsys_trainer = tr.Trainer(
+        model=model,
+        args=args,
+        schema=schema,
+        train_dataset_or_path=data.path,
+        eval_dataset_or_path=data.path,
+        test_dataset_or_path=data.path,
+        compute_metrics=True,
+    )
+
+    recsys_trainer.train()
+    eval_metrics = recsys_trainer.evaluate(eval_dataset=data.path, metric_key_prefix="eval")
+    predictions = recsys_trainer.predict(data.path)
+
+    assert isinstance(eval_metrics, dict)
+    assert set(default_metric).issubset(set(eval_metrics.keys()))
+    assert eval_metrics["eval_/loss"] is not None
+
+    assert predictions is not None
+
+
+@pytest.mark.parametrize("schema_type", ["msl", "core"])
+def test_trainer_with_multiple_tasks(schema_type):
+    data = tr.data.music_streaming_testing_data
+    schema = data.schema if schema_type == "msl" else data.merlin_schema
+    batch_size = 16
+    predict_top_k = 20
     tasks = [
         tr.NextItemPredictionTask(weight_tying=True),
         tr.BinaryClassificationTask("click", summary_type="mean"),
         tr.RegressionTask("play_percentage", summary_type="mean"),
     ]
     inputs = tr.TabularSequenceFeatures.from_schema(
         schema,
@@ -415,15 +511,15 @@
         output_dir=".",
         max_steps=5,
         num_train_epochs=1,
         per_device_train_batch_size=batch_size,
         per_device_eval_batch_size=batch_size // 2,
         data_loader_engine="merlin_dataloader",
         max_sequence_length=20,
-        predict_top_k=20,
+        predict_top_k=predict_top_k,
         fp16=False,
         report_to=[],
         debug=["r"],
     )
 
     recsys_trainer = tr.Trainer(
         model=model,
@@ -453,7 +549,52 @@
     ]
 
     assert isinstance(eval_metrics, dict)
     assert set(default_metrics).issubset(set(eval_metrics.keys()))
     assert eval_metrics["eval_/loss"] is not None
 
     assert predictions is not None
+    assert predictions.predictions["next-item"][0].shape == (1000, predict_top_k)
+    assert predictions.predictions["play_percentage/regression_task"].shape == (1000,)
+    assert predictions.predictions["click/binary_classification_task"].shape == (1000,)
+
+
+def test_trainer_trop_k_with_wrong_task():
+    data = tr.data.music_streaming_testing_data
+    schema = data.schema
+    batch_size = 16
+    predict_top_k = 20
+
+    task = tr.BinaryClassificationTask("click", summary_type="mean")
+    inputs = tr.TabularSequenceFeatures.from_schema(
+        schema,
+        max_sequence_length=20,
+        d_output=64,
+    )
+    transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
+    model = transformer_config.to_torch_model(inputs, task)
+
+    args = trainer.T4RecTrainingArguments(
+        output_dir=".",
+        num_train_epochs=1,
+        per_device_train_batch_size=batch_size,
+        per_device_eval_batch_size=batch_size // 2,
+        data_loader_engine="merlin_dataloader",
+        max_sequence_length=20,
+        predict_top_k=predict_top_k,
+        report_to=[],
+        debug=["r"],
+    )
+
+    recsys_trainer = tr.Trainer(
+        model=model,
+        args=args,
+        schema=schema,
+        train_dataset_or_path=data.path,
+        eval_dataset_or_path=data.path,
+        test_dataset_or_path=data.path,
+        compute_metrics=True,
+    )
+    with pytest.raises(AssertionError) as excinfo:
+        recsys_trainer.predict(data.path)
+
+    assert "Top-k prediction is specific to NextItemPredictionTask" in str(excinfo.value)
```

### Comparing `transformers4rec-23.2.0/tests/torch/utils/__init__.py` & `transformers4rec-23.4.0/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/torch/utils/test_schema_utils.py` & `transformers4rec-23.4.0/tests/unit/torch/utils/test_schema_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,52 +10,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import torch
+from merlin.schema import Tags
 
-import pytest
-
-from merlin_standard_lib import ColumnSchema, Schema, Tag
+from merlin_standard_lib import ColumnSchema, Schema
 from merlin_standard_lib.schema.schema import ValueCount
-
-schema_utils = pytest.importorskip("transformers4rec.torch.utils.schema_utils")
-pytorch = pytest.importorskip("torch")
+from transformers4rec.torch.utils import schema_utils
 
 
 def test_random_data_from_simple_schema():
     s = Schema(
         [
             ColumnSchema.create_categorical(
                 "item_id",
                 num_items=1000,
-                tags=[Tag.ITEM_ID, Tag.LIST],
+                tags=[Tags.ITEM_ID, Tags.LIST],
                 value_count=ValueCount(1, 50),
             ),
             ColumnSchema.create_categorical(
-                "session_cat", num_items=1000, tags=[Tag.LIST], value_count=ValueCount(1, 50)
+                "session_cat", num_items=1000, tags=[Tags.LIST], value_count=ValueCount(1, 50)
             ),
             ColumnSchema.create_continuous(
-                "session_con", tags=[Tag.LIST], value_count=ValueCount(1, 50)
+                "session_con", tags=[Tags.LIST], value_count=ValueCount(1, 50)
             ),
             ColumnSchema.create_categorical("context_cat", num_items=1000),
         ]
     )
 
     random_data = schema_utils.random_data_from_schema(s, 100, max_session_length=50)
 
     assert random_data["context_cat"].shape == (100,)
-    assert random_data["session_con"].dtype == pytorch.float32
-    for val in s.select_by_tag(Tag.LIST).filter_columns_from_dict(random_data).values():
+    assert random_data["session_con"].dtype == torch.float32
+    for val in s.select_by_tag(Tags.LIST).filter_columns_from_dict(random_data).values():
         assert val.shape == (100, 50)
 
-    for val in s.select_by_tag(Tag.CATEGORICAL).filter_columns_from_dict(random_data).values():
-        assert val.dtype == pytorch.int64
+    for val in s.select_by_tag(Tags.CATEGORICAL).filter_columns_from_dict(random_data).values():
+        assert val.dtype == torch.int64
         assert val.max() < 1000
 
 
 def test_random_data_from_schema_with_embeddings():
     def create_emb(name):
         return ColumnSchema.create_continuous(name, shape=(100,), is_embedding=True)
```

### Comparing `transformers4rec-23.2.0/tests/unit/test_notebooks.py` & `transformers4rec-23.4.0/tests/integration/notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tests/utils/__init__.py` & `transformers4rec-23.4.0/transformers4rec/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/tox.ini` & `transformers4rec-23.4.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 ; For all tests that run in Github Actions, see
 ; .github/workflows/cpu-ci.yml for the workflow definition.
 
 [tox]
-envlist = python3.8,test-gpu,test-cpu
+envlist = python3.8,test-gpu,test-cpu,test-gpu-integration,test-cpu-integration
 
 [testenv]
 commands =
-    pip install --upgrade pip
-    pip install .
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
+    pip install --upgrade pip    
+    pip install -r requirements/base_external.txt -r requirements/pytorch.txt
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/models.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
+    pip install . --no-deps
 
 [testenv:test-cpu]
 ; Runs in: Github Actions
-; Runs all CPU-based tests. NOTE: if you are using an M1 mac, this will fail. You need to
+; Runs all CPU-based unit tests. NOTE: if you are using an M1 mac, this will fail. You need to
+; change the tensorflow dependency to `tensorflow-macos` in requirements/test-cpu.txt.
+deps = -rrequirements/test.txt
+commands =
+    {[testenv]commands}
+
+    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests/unit
+
+[testenv:test-cpu-integration]
+; Runs in: Github Actions
+; Runs all CPU-based NOTEBOOK tests. NOTE: if you are using an M1 mac, this will fail. You need to
 ; change the tensorflow dependency to `tensorflow-macos` in requirements/test-cpu.txt.
 deps = -rrequirements/test.txt
 commands =
     {[testenv]commands}
 
-    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests
+    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests/integration
 
 [testenv:test-gpu]
 sitepackages=true
 ; Runs in: Internal Jenkins
 ; Runs GPU-based tests.
 ; The jenkins jobs run on an image based on merlin-hugectr. This will include all cudf configuration
 ; and other gpu-specific libraries that we can enxpect will always exist. Thus, we don't need
@@ -33,15 +45,31 @@
 setenv = 
     TF_GPU_ALLOCATOR=cuda_malloc_async
 deps =
     -rrequirements/test.txt
 commands =
     {[testenv]commands}
 
-    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests
+    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests/unit
+
+[testenv:test-gpu-integration]
+sitepackages=true
+setenv = 
+    TF_GPU_ALLOCATOR=cuda_malloc_async
+deps =
+    -rrequirements/test.txt   
+commands =
+    ; install latest Merlin libraries from source
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/systems.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/models.git@{posargs:main}
+
+    python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests/integration
 
 [testenv:docs]
 ; Runs in: Github Actions
 ; Generates documentation with sphinx. There are other steps in the Github Actions workflow
 ; to publish the documentation on release.
 changedir = {toxinidir}
 deps = -rrequirements/docs.txt
```

### Comparing `transformers4rec-23.2.0/transformers4rec/__init__.py` & `transformers4rec-23.4.0/transformers4rec/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/config/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/config/schema.py` & `transformers4rec-23.4.0/transformers4rec/config/schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/config/trainer.py` & `transformers4rec-23.4.0/transformers4rec/config/trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/config/transformer.py` & `transformers4rec-23.4.0/transformers4rec/config/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import transformers
-
-from merlin_standard_lib import Registry
+from merlin.models.utils.registry import Registry
 
 transformer_registry: Registry = Registry("transformers")
 
 
 class T4RecConfig:
     def to_huggingface_torch_model(self):
         model_cls = transformers.MODEL_MAPPING[self.transformers_config_cls]
```

### Comparing `transformers4rec-23.2.0/transformers4rec/data/__init__.py` & `transformers4rec-23.4.0/transformers4rec/data/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/dataset.py` & `transformers4rec-23.4.0/transformers4rec/data/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 # limitations under the License.
 #
 
 
 import os
 from typing import Optional
 
+from merlin.schema import Schema as CoreSchema
+from merlin.schema.io.tensorflow_metadata import TensorflowMetadata
+
 from merlin_standard_lib import Schema
 
 
 class Dataset:
     def __init__(self, schema_path: str):
         self.schema_path = schema_path
         if self.schema_path.endswith(".pb") or self.schema_path.endswith(".pbtxt"):
@@ -29,25 +32,30 @@
         else:
             self._schema = Schema().from_json(self.schema_path)
 
     @property
     def schema(self) -> Schema:
         return self._schema
 
+    @property
+    def merlin_schema(self) -> CoreSchema:
+        return TensorflowMetadata.from_json(self.schema.to_json()).to_merlin_schema()
+
     def torch_synthetic_data(
-        self, num_rows=100, min_session_length=5, max_session_length=20, device=None
+        self, num_rows=100, min_session_length=5, max_session_length=20, device=None, ragged=False
     ):
         from transformers4rec.torch.utils import schema_utils
 
         return schema_utils.random_data_from_schema(
             self.schema,
             num_rows=num_rows,
             min_session_length=min_session_length,
             max_session_length=max_session_length,
             device=device,
+            ragged=ragged,
         )
 
     def tf_synthetic_data(self, num_rows=100, min_session_length=5, max_session_length=20):
         from transformers4rec.tf.utils import schema_utils
 
         return schema_utils.random_data_from_schema(
             self.schema,
```

### Comparing `transformers4rec-23.2.0/transformers4rec/data/preprocessing.py` & `transformers4rec-23.4.0/transformers4rec/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         except ImportError:
             raise ValueError(
                 "Rapids is necessary for running function in gpu, please install: " "dask_cudf."
             )
         data = dask_cudf.from_cudf(data, npartitions=3)
 
     # get item and session features
-    item_features = schema.select_by_tag(["item"]).feature
+    item_features = schema.select_by_tag(["item"]).first
     session_feat = schema.select_by_tag(["session"]).column_names
     groupby_dict = {k.name: ["list"] for k in item_features}
     for col in session_feat:
         groupby_dict[col] = ["first"]
 
     # retrieve session_id column
     session_column = schema.select_by_tag(["session_id"]).feature
```

### Comparing `transformers4rec-23.2.0/transformers4rec/data/synthetic.py` & `transformers4rec-23.4.0/transformers4rec/data/synthetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 
 import numpy as np
 import pandas as pd
+from merlin.schema import Tags
+from merlin.schema.io.proto_utils import has_field
 
 import merlin_standard_lib as msl
-from merlin_standard_lib import Schema, Tag
-from merlin_standard_lib.utils.proto_utils import has_field
+from merlin_standard_lib import Schema
 
 LOG = logging.getLogger("transformers4rec")
 
 
 def generate_session_interactions(
     num_interactions: int,
     schema: Schema,
@@ -40,30 +41,30 @@
     >>> import merlin_standard_lib as msl
     >>> s = msl.Schema(
         [
             msl.ColumnSchema.create_categorical("session_id", num_items=5000, tags=['session_id']),
             msl.ColumnSchema.create_categorical(
                 "item_id",
                 num_items=10000,
-                tags=[Tag.ITEM_ID, Tag.LIST],
+                tags=[Tags.ITEM_ID, Tags.LIST],
                 value_count=msl.schema.ValueCount(1, 20),
             ),
             msl.ColumnSchema.create_categorical(
                 "category", num_items=100,
-                tags=[Tag.LIST, Tag.ITEM], value_count=msl.schema.ValueCount(1, 20)
+                tags=[Tags.LIST, Tags.ITEM], value_count=msl.schema.ValueCount(1, 20)
             ),
             msl.ColumnSchema.create_continuous(
                 "item_recency", min_value=0, max_value=1,
-                tags=[Tag.LIST, Tag.ITEM], value_count=msl.schema.ValueCount(1, 20)
+                tags=[Tags.LIST, Tags.ITEM], value_count=msl.schema.ValueCount(1, 20)
             ),
             msl.ColumnSchema.create_categorical("day", num_items=11, tags=['session']),
             msl.ColumnSchema.create_categorical(
-                "purchase", num_items=3, tags=['session', Tag.BINARY_CLASSIFICATION]),
+                "purchase", num_items=3, tags=['session', Tags.BINARY_CLASSIFICATION]),
             msl.ColumnSchema.create_continuous(
-                "price", min_value=0, max_value=1 , tags=['session', Tag.REGRESSION])
+                "price", min_value=0, max_value=1 , tags=['session', Tags.REGRESSION])
         ]
     )
     >>> generate_session_interactions(100000, s, 30, 5, 'gpu')
     """
     from transformers4rec.data.preprocessing import session_aggregator  # type: ignore
 
     data = generate_item_interactions(num_interactions, schema)
@@ -77,49 +78,49 @@
 
 def generate_item_interactions(num_interactions: int, schema: Schema) -> pd.DataFrame:
     """
     Util function to generate synthetic data for session-based item-interactions
     from a schema object. It supports the generation of session and item features.
     The schema should include a few tags:
 
-    - `Tag.SESSION` for features related to sessions
-    - `Tag.SESSION_ID` to tag the session-id feature
-    - `Tag.ITEM` for features related to item interactions.
+    - `Tags.SESSION` for features related to sessions
+    - `Tags.SESSION_ID` to tag the session-id feature
+    - `Tags.ITEM` for features related to item interactions.
 
     Parameters:
     ----------
     num_interactions: int
         number of interaction rows to generate.
     schema: Schema
         schema object describing the columns to generate.
 
     Returns
     -------
     data: pd.DataFrame
         Pandas dataframe with synthetic generated data.
     """
-    session_col = schema.select_by_tag(Tag.SESSION_ID).feature[0]
+    session_col = schema.select_by_tag([Tags.SESSION_ID.value]).feature[0]
     data = pd.DataFrame(
         np.random.randint(1, session_col.int_domain.max, num_interactions),
         columns=[session_col.name],
     ).astype(np.int64)
 
-    item_id_col = schema.select_by_tag(Tag.ITEM_ID).feature[0]
+    item_id_col = schema.select_by_tag([Tags.ITEM_ID.value]).feature[0]
     data[item_id_col.name] = np.clip(
         np.random.lognormal(3.0, 1.0, num_interactions).astype(np.int32),
         1,
         item_id_col.int_domain.max,
     ).astype(np.int64)
 
     # get session cols
-    session_features = schema.select_by_tag(Tag.SESSION).feature
+    session_features = schema.select_by_tag(Tags.SESSION.value).feature
     for feature in session_features:
         is_int_feature = has_field(feature, "int_domain")
         if is_int_feature:
-            if Tag.BINARY_CLASSIFICATION.value in feature.tags:
+            if Tags.BINARY_CLASSIFICATION.value in feature.tags:
                 mapping_feature = dict(
                     zip(
                         data[session_col.name].unique(),
                         np.random.choice(a=[0, 1], size=(data[session_col.name].nunique())),
                     )
                 )
                 data[feature.name] = data[session_col.name].map(mapping_feature)
@@ -144,15 +145,15 @@
                         size=(data[session_col.name].nunique()),
                     ),
                 )
             )
             data[feature.name] = data[session_col.name].map(mapping_feature)
 
     # get item-id cols
-    items_features = schema.select_by_tag(Tag.ITEM).feature
+    items_features = schema.select_by_tag(Tags.ITEM.value).feature
     for feature in items_features:
         is_int_feature = has_field(feature, "int_domain")
         if is_int_feature:
             data[feature.name] = pd.cut(
                 data[item_id_col.name],
                 bins=feature.int_domain.max - 1,
                 labels=np.arange(1, feature.int_domain.max),
@@ -167,32 +168,32 @@
 
 synthetic_ecommerce_data_schema = Schema(
     [
         msl.ColumnSchema.create_categorical("session_id", num_items=5000, tags=["session_id"]),
         msl.ColumnSchema.create_categorical(
             "item_id",
             num_items=10000,
-            tags=[Tag.ITEM_ID, Tag.LIST],
+            tags=[Tags.ITEM_ID, Tags.LIST],
             value_count=msl.schema.ValueCount(1, 20),
         ),
         msl.ColumnSchema.create_categorical(
             "category",
             num_items=100,
-            tags=[Tag.LIST, Tag.ITEM],
+            tags=[Tags.LIST, Tags.ITEM],
             value_count=msl.schema.ValueCount(1, 20),
         ),
         msl.ColumnSchema.create_continuous(
             "item_recency",
             min_value=0,
             max_value=1,
-            tags=[Tag.LIST, Tag.ITEM],
+            tags=[Tags.LIST, Tags.ITEM],
             value_count=msl.schema.ValueCount(1, 20),
         ),
-        msl.ColumnSchema.create_categorical("day", num_items=11, tags=[Tag.SESSION]),
+        msl.ColumnSchema.create_categorical("day", num_items=11, tags=[Tags.SESSION]),
         msl.ColumnSchema.create_categorical(
-            "purchase", num_items=3, tags=[Tag.SESSION, Tag.BINARY_CLASSIFICATION]
+            "purchase", num_items=3, tags=[Tags.SESSION, Tags.BINARY_CLASSIFICATION]
         ),
         msl.ColumnSchema.create_continuous(
-            "price", min_value=0, max_value=1, tags=[Tag.SESSION, Tag.REGRESSION]
+            "price", min_value=0, max_value=1, tags=[Tags.SESSION, Tags.REGRESSION]
         ),
     ]
 )
```

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/data.parquet` & `transformers4rec-23.4.0/transformers4rec/data/testing/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/dataset.py` & `transformers4rec-23.4.0/transformers4rec/data/testing/dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/data.parquet` & `transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/music_streaming/schema.json` & `transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/schema.json` & `transformers4rec-23.4.0/transformers4rec/data/testing/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/data.parquet` & `transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/testing/tabular_data/schema.json` & `transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/data/yoochoose.py` & `transformers4rec-23.4.0/transformers4rec/data/yoochoose.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     device: str, default: "gpu"
         Device to use for processing clicks.
 
     Returns
     -------
     Union[cudf.DataFrame, pandas.DataFrame]
     """
-    from .preprocessing import (  # type: ignore
+    from ..utils.data_utils import (  # type: ignore
         add_item_first_seen_col_to_df,
         remove_consecutive_interactions,
     )
 
     if device == "gpu":
         import cudf
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from merlin_standard_lib import Schema, Tag
+from merlin_standard_lib import Schema
 
 from .. import data
 from ..config.schema import requires_schema
 from ..config.trainer import T4RecTrainingArguments
 from ..config.transformer import (
     AlbertConfig,
     ElectraConfig,
@@ -71,15 +71,14 @@
     TabularTransformation,
 )
 from .tabular.transformations import StochasticSwapNoise, TabularDropout, TabularLayerNorm
 from .trainer import Trainer  # type: ignore
 
 __all__ = [
     "Schema",
-    "Tag",
     "ranking_metric",
     "requires_schema",
     "T4RecConfig",
     "GPT2Config",
     "XLNetConfig",
     "TransfoXLConfig",
     "LongformerConfig",
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/block/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/block/base.py` & `transformers4rec-23.4.0/transformers4rec/torch/block/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 import abc
 import inspect
 import logging
 from collections import OrderedDict
 from typing import List, Optional, Union
 
 import torch
+from merlin.models.utils.misc_utils import filter_kwargs
 from torch.nn import Module
 
-from merlin_standard_lib.utils.misc_utils import filter_kwargs
-
 from ..utils import torch_utils
 
 LOG = logging.getLogger("transformers4rec")
 
 
 class BlockBase(torch_utils.OutputSizeMixin, torch.nn.Module, metaclass=abc.ABCMeta):
     def to_model(self, prediction_task_or_head, inputs=None, **kwargs):
@@ -57,16 +56,16 @@
 
 class Block(BlockBase):
     def __init__(self, module: torch.nn.Module, output_size: Union[List[int], torch.Size]):
         super().__init__()
         self.module = module
         self._output_size = output_size
 
-    def forward(self, inputs):
-        return self.module(inputs)
+    def forward(self, inputs, **kwargs):
+        return self.module(inputs, **kwargs)
 
     def forward_output_size(self, input_size):
         if self._output_size[0] is None:
             batch_size = torch_utils.calculate_batch_size_from_input_size(input_size)
 
             return [batch_size] + self._output_size[1:]
 
@@ -140,15 +139,15 @@
         return right_shift_block(other, self)
 
     def forward(self, input, training=False, testing=False, **kwargs):
         # from transformers4rec.torch import TabularSequenceFeatures
 
         for i, module in enumerate(self):
             if i == len(self) - 1:
-                filtered_kwargs = filter_kwargs(kwargs, module, filter_positional_or_keyword=False)
+                filtered_kwargs = filter_kwargs(kwargs, module, cascade_kwargs_if_possible=True)
                 input = module(input, **filtered_kwargs)
 
             elif "training" in inspect.signature(module.forward).parameters:
                 if "testing" in inspect.signature(module.forward).parameters:
                     input = module(input, training=training, testing=testing)
                 else:
                     input = module(input, training=training)
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/block/mlp.py` & `transformers4rec-23.4.0/transformers4rec/torch/block/mlp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/block/transformer.py` & `transformers4rec-23.4.0/transformers4rec/torch/block/transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/experimental.py` & `transformers4rec-23.4.0/transformers4rec/torch/experimental.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/text.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/base.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/continuous.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/continuous.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from typing import List, Optional
 
 import torch
+from merlin.models.utils.doc_utils import docstring_parameter
 
 from merlin_standard_lib import Schema
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
 
 from ..tabular.base import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     FilterFeatures,
     TabularAggregationType,
     TabularTransformationType,
 )
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/embedding.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # limitations under the License.
 #
 
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Text, Union
 
 import torch
+from merlin.models.utils.doc_utils import docstring_parameter
+from merlin.schema import Tags, TagsType
 
-from merlin_standard_lib import Schema, Tag
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
+from merlin_standard_lib import Schema, categorical_cardinalities
 from merlin_standard_lib.utils.embedding_utils import get_embedding_sizes_from_schema
 
 from ..tabular.base import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     FilterFeatures,
     TabularAggregationType,
     TabularTransformationType,
@@ -103,15 +104,15 @@
         schema: Schema,
         embedding_dims: Optional[Dict[str, int]] = None,
         embedding_dim_default: int = 64,
         infer_embedding_sizes: bool = False,
         infer_embedding_sizes_multiplier: float = 2.0,
         embeddings_initializers: Optional[Dict[str, Callable[[Any], None]]] = None,
         combiner: str = "mean",
-        tags: Optional[Union[Tag, list, str]] = None,
+        tags: Optional[TagsType] = None,
         item_id: Optional[str] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         aggregation=None,
         pre=None,
         post=None,
         **kwargs,
@@ -154,16 +155,22 @@
             Returns the ``EmbeddingFeatures`` for the dataset schema
         """
         # TODO: propagate item-id from ITEM_ID tag
 
         if tags:
             schema = schema.select_by_tag(tags)
 
-        if not item_id and schema.select_by_tag(["item_id"]).column_names:
-            item_id = schema.select_by_tag(["item_id"]).column_names[0]
+        _item_id = schema.select_by_tag(Tags.ITEM_ID)
+        if not item_id and len(_item_id) > 0:
+            if len(_item_id) > 1:
+                raise ValueError(
+                    "Multiple columns with tag ITEM_ID found. "
+                    "Please specify the item_id column name."
+                )
+            item_id = list(_item_id)[0].name
 
         embedding_dims = embedding_dims or {}
 
         if infer_embedding_sizes:
             embedding_dims_infered = get_embedding_sizes_from_schema(
                 schema, infer_embedding_sizes_multiplier
             )
@@ -172,15 +179,15 @@
                 **embedding_dims,
                 **{k: v for k, v in embedding_dims_infered.items() if k not in embedding_dims},
             }
 
         embeddings_initializers = embeddings_initializers or {}
 
         emb_config = {}
-        cardinalities = schema.categorical_cardinalities()
+        cardinalities = categorical_cardinalities(schema)
         for key, cardinality in cardinalities.items():
             embedding_size = embedding_dims.get(key, embedding_dim_default)
             embedding_initializer = embeddings_initializers.get(key, None)
             emb_config[key] = (cardinality, embedding_size, embedding_initializer)
 
         feature_config: Dict[str, FeatureConfig] = {}
         for name, (vocab_size, dim, emb_initilizer) in emb_config.items():
@@ -300,15 +307,15 @@
         soft_embedding_cardinalities: Optional[Dict[str, int]] = None,
         soft_embedding_cardinality_default: int = 10,
         soft_embedding_dims: Optional[Dict[str, int]] = None,
         soft_embedding_dim_default: int = 8,
         embeddings_initializers: Optional[Dict[str, Callable[[Any], None]]] = None,
         layer_norm: bool = True,
         combiner: str = "mean",
-        tags: Optional[Union[Tag, list, str]] = None,
+        tags: Optional[TagsType] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         **kwargs,
     ) -> Optional["SoftEmbeddingFeatures"]:
         """
         Instantitates ``SoftEmbeddingFeatures`` from a ``DatasetSchema``.
 
@@ -349,15 +356,15 @@
             schema = schema.select_by_tag(tags)
 
         soft_embedding_cardinalities = soft_embedding_cardinalities or {}
         soft_embedding_dims = soft_embedding_dims or {}
         embeddings_initializers = embeddings_initializers or {}
 
         sizes = {}
-        cardinalities = schema.categorical_cardinalities()
+        cardinalities = categorical_cardinalities(schema)
         for col_name in schema.column_names:
             # If this is NOT a categorical feature
             if col_name not in cardinalities:
                 embedding_size = soft_embedding_dims.get(col_name, soft_embedding_dim_default)
                 cardinality = soft_embedding_cardinalities.get(
                     col_name, soft_embedding_cardinality_default
                 )
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/sequence.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from typing import Dict, List, Optional, Tuple, Union
 
 import torch
+from merlin.models.utils.doc_utils import docstring_parameter
+from merlin.schema import Tags, TagsType
 
-from merlin_standard_lib import Schema, Tag
-from merlin_standard_lib.schema.tag import TagsType
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
+from merlin_standard_lib import Schema
 
 from ..block.base import BlockOrModule, BuildableBlock, SequentialBlock
 from ..block.mlp import MLPBlock
 from ..masking import MaskSequence, masking_registry
 from ..tabular.base import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     AsTabular,
@@ -137,16 +137,16 @@
         self.projection_module = projection_module
         self.set_masking(masking)
 
     @classmethod
     def from_schema(  # type: ignore
         cls,
         schema: Schema,
-        continuous_tags: Optional[Union[TagsType, Tuple[Tag]]] = (Tag.CONTINUOUS,),
-        categorical_tags: Optional[Union[TagsType, Tuple[Tag]]] = (Tag.CATEGORICAL,),
+        continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
+        categorical_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CATEGORICAL,),
         aggregation: Optional[str] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         continuous_projection: Optional[Union[List[int], int]] = None,
         continuous_soft_embeddings: bool = False,
         projection: Optional[Union[torch.nn.Module, BuildableBlock]] = None,
         d_output: Optional[int] = None,
@@ -155,18 +155,18 @@
     ) -> "TabularSequenceFeatures":
         """Instantiates ``TabularFeatures`` from a ``DatasetSchema``
 
         Parameters
         ----------
         schema : DatasetSchema
             Dataset schema
-        continuous_tags : Optional[Union[DefaultTags, list, str]], optional
-            Tags to filter the continuous features, by default Tag.CONTINUOUS
-        categorical_tags : Optional[Union[DefaultTags, list, str]], optional
-            Tags to filter the categorical features, by default Tag.CATEGORICAL
+        continuous_tags : Optional[Union[TagsType, Tuple[Tags]]], optional
+            Tags to filter the continuous features, by default Tags.CONTINUOUS
+        categorical_tags : Optional[Union[TagsType, Tuple[Tags]]], optional
+            Tags to filter the categorical features, by default Tags.CATEGORICAL
         aggregation : Optional[str], optional
             Feature aggregation option, by default None
         automatic_build : bool, optional
             Automatically infers input size from features, by default True
         max_sequence_length : Optional[int], optional
             Maximum sequence length for list features by default None
         continuous_projection : Optional[Union[List[int], int]], optional
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/tabular.py` & `transformers4rec-23.4.0/transformers4rec/torch/features/tabular.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from typing import List, Optional, Tuple, Type, Union
 
-from merlin_standard_lib import Schema, Tag
-from merlin_standard_lib.schema.tag import TagsType
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
+from merlin.models.utils.doc_utils import docstring_parameter
+from merlin.schema import Tags, TagsType
+
+from merlin_standard_lib import Schema
 
 from ..block.base import SequentialBlock
 from ..block.mlp import MLPBlock
 from ..tabular.base import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     AsTabular,
     MergeTabular,
@@ -114,33 +115,33 @@
 
         return self
 
     @classmethod
     def from_schema(  # type: ignore
         cls,
         schema: Schema,
-        continuous_tags: Optional[Union[TagsType, Tuple[Tag]]] = (Tag.CONTINUOUS,),
-        categorical_tags: Optional[Union[TagsType, Tuple[Tag]]] = (Tag.CATEGORICAL,),
+        continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
+        categorical_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CATEGORICAL,),
         aggregation: Optional[str] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         continuous_projection: Optional[Union[List[int], int]] = None,
         continuous_soft_embeddings: bool = False,
         **kwargs,
     ) -> "TabularFeatures":
         """Instantiates ``TabularFeatures`` from a ``DatasetSchema``
 
         Parameters
         ----------
         schema : DatasetSchema
             Dataset schema
-        continuous_tags : Optional[Union[DefaultTags, list, str]], optional
-            Tags to filter the continuous features, by default Tag.CONTINUOUS
-        categorical_tags : Optional[Union[DefaultTags, list, str]], optional
-            Tags to filter the categorical features, by default Tag.CATEGORICAL
+        continuous_tags : Optional[Union[TagsType, Tuple[Tags]]], optional
+            Tags to filter the continuous features, by default Tags.CONTINUOUS
+        categorical_tags : Optional[Union[TagsType, Tuple[Tags]]], optional
+            Tags to filter the categorical features, by default Tags.CATEGORICAL
         aggregation : Optional[str], optional
             Feature aggregation option, by default None
         automatic_build : bool, optional
             Automatically infers input size from features, by default True
         max_sequence_length : Optional[int], optional
             Maximum sequence length for list features by default None
         continuous_projection : Optional[Union[List[int], int]], optional
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/features/text.py` & `transformers4rec-23.4.0/transformers4rec/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/masking.py` & `transformers4rec-23.4.0/transformers4rec/torch/masking.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Tuple
 
 import torch
+from merlin.models.utils.doc_utils import docstring_parameter
+from merlin.models.utils.registry import Registry
 from torch import nn
 
-from merlin_standard_lib import Registry
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
-
 from .utils.torch_utils import OutputSizeMixin
 
 masking_registry = Registry("torch.masking")
 
 
 @dataclass
 class MaskingInfo:
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/model/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/model/base.py` & `transformers4rec-23.4.0/transformers4rec/torch/model/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,36 +20,37 @@
 from collections import defaultdict
 from types import SimpleNamespace
 from typing import Callable, Dict, Iterable, List, Optional, Type, Union, cast
 
 import numpy as np
 import torch
 import torchmetrics as tm
+from merlin.models.utils.registry import camelcase_to_snakecase
 from merlin.schema import ColumnSchema
 from merlin.schema import Schema as Core_Schema
+from merlin.schema import Tags
 from tqdm import tqdm
 from transformers.modeling_utils import SequenceSummary
 
-from merlin_standard_lib import Schema, Tag
-from merlin_standard_lib.registry import camelcase_to_snakecase
+from merlin_standard_lib import Schema
 
 from ..block.base import BlockBase, BlockOrModule, BlockType
 from ..features.base import InputBlock
 from ..features.sequence import TabularFeaturesType
-from ..typing import TabularData, TensorOrTabularData
+from ..typing import TabularData
+from ..utils.padding import pad_inputs
 from ..utils.torch_utils import LossMixin, MetricsMixin
 
 
 def name_fn(name, inp):
     return "/".join([name, inp]) if name else None
 
 
 class PredictionTask(torch.nn.Module, LossMixin, MetricsMixin):
     """Individual prediction-task of a model.
-
     Parameters
     ----------
     loss: torch.nn.Module
         The loss to use during training of this task.
     metrics: torch.nn.Module
         The metrics to calculate during training & evaluation.
     target_name: str, optional
@@ -104,15 +105,14 @@
         device=None,
         task_block: Optional[BlockType] = None,
         pre=None,
     ):
         """
         The method will be called when block is converted to a model,
         i.e when linked to prediction head.
-
         Parameters
         ----------
         block:
             the model block to link with head
         device:
             set the device for the metrics and layers of the task
         """
@@ -162,14 +162,21 @@
 
         if self.pre:
             x = self.pre(x)  # type: ignore
 
         if training or testing:
             # add support of computing the loss inside the forward
             # and return a dictionary as standard output
+            if self.summary_type is None:
+                if targets.dim() != 2:
+                    raise ValueError(
+                        "If `summary_type==None`, targets are expected to be a 2D tensor, "
+                        f"but got a tensor with shape {targets.shape}"
+                    )
+
             loss = self.loss(x, target=targets)
             return {"loss": loss, "labels": targets, "predictions": x}
 
         return x
 
     @property
     def task_name(self):
@@ -187,15 +194,14 @@
         self.metrics = torch.nn.ModuleList(metrics)
 
     def calculate_metrics(  # type: ignore
         self,
         predictions: torch.Tensor,
         targets: torch.Tensor,
     ) -> Dict[str, torch.Tensor]:
-
         outputs = {}
 
         predictions = self.forward_to_prediction_fn(cast(torch.Tensor, predictions))
 
         from .prediction_task import BinaryClassificationTask
 
         for metric in self.metrics:
@@ -220,15 +226,14 @@
 
     def to_model(self, body, inputs=None, **kwargs) -> "Model":
         return Model(Head(body, self, inputs=inputs, **kwargs), **kwargs)
 
 
 class Head(torch.nn.Module, LossMixin, MetricsMixin):
     """Head of a Model, a head has a single body but could have multiple prediction-tasks.
-
     Parameters
     ----------
     body: Block
         TODO
     prediction_tasks: Union[List[PredictionTask], PredictionTask], optional
         TODO
     task_blocks
@@ -265,15 +270,14 @@
             for task, val in zip(cast(List[PredictionTask], prediction_tasks), task_weights):
                 self._task_weights[task.task_name] = val
 
         self.build(inputs=inputs, task_blocks=task_blocks)
 
     def build(self, inputs=None, device=None, task_blocks=None):
         """Build each prediction task that's part of the head.
-
         Parameters
         ----------
         body
         inputs
         device
         task_blocks
         """
@@ -302,40 +306,38 @@
         body: BlockBase,
         task_blocks: Optional[Union[BlockType, Dict[str, BlockType]]] = None,
         task_weight_dict: Optional[Dict[str, float]] = None,
         loss_reduction: str = "mean",
         inputs: Optional[TabularFeaturesType] = None,
     ) -> "Head":
         """Instantiate a Head from a Schema through tagged targets.
-
         Parameters
         ----------
         schema: DatasetSchema
             Schema to use for inferring all targets based on the tags.
         body
         task_blocks
         task_weight_dict
         loss_reduction
         inputs
-
         Returns
         -------
         Head
         """
         task_weight_dict = task_weight_dict or {}
         tasks: List[PredictionTask] = []
         task_weights = []
 
         from .prediction_task import BinaryClassificationTask, RegressionTask
 
-        for binary_target in schema.select_by_tag(Tag.BINARY_CLASSIFICATION).column_names:
+        for binary_target in schema.select_by_tag([Tags.BINARY, Tags.CLASSIFICATION]).column_names:
             tasks.append(BinaryClassificationTask(binary_target))
             task_weights.append(task_weight_dict.get(binary_target, 1.0))
 
-        for regression_target in schema.select_by_tag(Tag.REGRESSION).column_names:
+        for regression_target in schema.select_by_tag(Tags.REGRESSION).column_names:
             tasks.append(RegressionTask(regression_target))
             task_weights.append(task_weight_dict.get(regression_target, 1.0))
 
         # TODO: Add multi-class classification here. Figure out how to get number of classes
 
         return cls(
             body,
@@ -344,20 +346,18 @@
             task_weights=task_weights,
             loss_reduction=loss_reduction,
             inputs=inputs,
         )
 
     def pop_labels(self, inputs: TabularData) -> TabularData:
         """Pop the labels from the different prediction_tasks from the inputs.
-
         Parameters
         ----------
         inputs: TabularData
             Input dictionary containing all targets.
-
         Returns
         -------
         TabularData
         """
         outputs = {}
         for name in self.prediction_task_dict.keys():
             outputs[name] = inputs.pop(name)
@@ -384,16 +384,15 @@
             predictions = {}
             for name, task in self.prediction_task_dict.items():
                 if isinstance(targets, dict):
                     label = targets.get(task.target_name, None)
                 else:
                     label = targets
                 if label is not None:
-                    # Remove dimension `1` as merlin dataloader returns tensors of shape (-1, 1)
-                    label = torch.squeeze(label.float(), -1)
+                    label = label.float()
                 task_output = task(
                     body_outputs, targets=label, training=training, testing=testing, **kwargs
                 )
                 labels[name] = task_output["labels"]
                 predictions[name] = task_output["predictions"]
                 losses.append(task_output["loss"] * self._task_weights[name])
             loss_tensor = torch.stack(losses)
@@ -409,15 +408,14 @@
 
     def calculate_metrics(  # type: ignore
         self,
         predictions: Union[torch.Tensor, TabularData],
         targets: Union[torch.Tensor, TabularData],
     ) -> Dict[str, Union[Dict[str, torch.Tensor], torch.Tensor]]:
         """Calculate metrics of the task(s) set in the Head instance.
-
         Parameters
         ----------
         predictions: Union[torch.Tensor, TabularData]
             The predictions tensors to use for calculate metrics.
             They can be either a torch.Tensor if a single task is used or
             a dictionary of torch.Tensor if multiple tasks are used. In the
             second case, the dictionary is indexed by the tasks names.
@@ -464,15 +462,14 @@
 
     @property
     def task_blocks(self) -> Dict[str, Optional[BlockOrModule]]:
         return {name: task.task_block for name, task in self.prediction_task_dict.items()}
 
     def to_model(self, **kwargs) -> "Model":
         """Convert the head to a Model.
-
         Returns
         -------
         Model
         """
 
         return Model(self, **kwargs)
 
@@ -481,29 +478,32 @@
     def __init__(
         self,
         *head: Head,
         head_weights: Optional[List[float]] = None,
         head_reduction: str = "mean",
         optimizer: Type[torch.optim.Optimizer] = torch.optim.Adam,
         name: str = None,
+        max_sequence_length: Optional[int] = None,
     ):
         """Model class that can aggregate one or multiple heads.
-
         Parameters
         ----------
         head: Head
             One or more heads of the model.
         head_weights: List[float], optional
             Weight-value to use for each head.
         head_reduction: str, optional
             How to reduce the losses into a single tensor when multiple heads are used.
         optimizer: Type[torch.optim.Optimizer]
             Optimizer-class to use during fitting
         name: str, optional
             Name of the model.
+        max_sequence_length : int, optional
+            The maximum sequence length supported by the model.
+            Used to truncate sequence inputs longer than this value.
         """
         if head_weights:
             if not isinstance(head_weights, list):
                 raise ValueError("`head_weights` must be a list")
             if not len(head_weights) == len(head):
                 raise ValueError(
                     "`head_weights` needs to have the same length " "as the number of heads"
@@ -512,25 +512,24 @@
         super().__init__()
 
         self.name = name
         self.heads = torch.nn.ModuleList(head)
         self.head_weights = head_weights or [1.0] * len(head)
         self.head_reduction = head_reduction
         self.optimizer = optimizer
+        self.max_sequence_length = max_sequence_length
 
-    def forward(
-        self, inputs: TensorOrTabularData, targets=None, training=False, testing=False, **kwargs
-    ):
+    def forward(self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs):
         # Convert inputs to float32 which is the default type, expected by PyTorch
         for name, val in inputs.items():
             if torch.is_floating_point(val):
                 inputs[name] = val.to(torch.float32)
-        # Squeeze second dimension `1` of non-list inputs
-        for name, val in inputs.items():
-            inputs[name] = torch.squeeze(val, -1)
+
+        # pad ragged inputs
+        inputs = pad_inputs(inputs, self.max_sequence_length)
 
         if isinstance(targets, dict) and len(targets) == 0:
             # `pyarrow`` dataloader is returning {} instead of None
             # TODO remove this code when `PyarraowDataLoader` is dropped
             targets = None
 
         # TODO: Optimize this
@@ -576,15 +575,14 @@
 
     def calculate_metrics(  # type: ignore
         self,
         predictions: Union[torch.Tensor, TabularData],
         targets: Union[torch.Tensor, TabularData],
     ) -> Dict[str, Union[Dict[str, torch.Tensor], torch.Tensor]]:
         """Calculate metrics of the task(s) set in the Head instance.
-
         Parameters
         ----------
         predictions: Union[torch.Tensor, TabularData]
             The predictions tensors returned by the model.
             They can be either a torch.Tensor if a single task is used or
             a dictionary of torch.Tensor if multiple heads/tasks are used. In the
             second case, the dictionary is indexed by the tasks names.
@@ -725,72 +723,79 @@
     @property
     def input_schema(self):
         # return the input schema given by the model
         # loop over the heads to get input schemas
         schemas = []
         for head in self.heads:
             schemas.append(head.body.inputs.schema)
+        if all(isinstance(s, Core_Schema) for s in schemas):
+            return sum(schemas, Core_Schema())
+
         model_schema = sum(schemas, Schema())
 
         # TODO: rework T4R to use Merlin Schemas.
         # In the meantime, we convert model_schema to merlin core schema
         core_schema = Core_Schema()
         for column in model_schema:
             name = column.name
 
             dtype = {0: np.float32, 2: np.int64, 3: np.float32}[column.type]
             tags = column.tags
-            is_list = column.value_count.max > 0
+            dims = None
+            if column.value_count.max > 0:
+                dims = (None, (column.value_count.min, column.value_count.max))
             int_domain = {"min": column.int_domain.min, "max": column.int_domain.max}
             properties = {
                 "int_domain": int_domain,
             }
 
             col_schema = ColumnSchema(
-                name,
-                dtype=dtype,
-                tags=tags,
-                properties=properties,
-                is_list=is_list,
-                is_ragged=False,
+                name, dtype=dtype, tags=tags, properties=properties, dims=dims
             )
             core_schema[name] = col_schema
         return core_schema
 
     @property
     def output_schema(self):
         from .prediction_task import BinaryClassificationTask, RegressionTask
 
         # if the model has one head with one task, the output is a tensor
         # if multiple heads and/or multiple prediction task, the output is a dictionary
         output_cols = []
         for head in self.heads:
+            dims = None
             for name, task in head.prediction_task_dict.items():
                 target_dim = task.target_dim
                 int_domain = {"min": target_dim, "max": target_dim}
                 if (
                     isinstance(task, (BinaryClassificationTask, RegressionTask))
                     and not task.summary_type
                 ):
-                    is_list = True
+                    dims = (None, (1, None))
+                elif (
+                    isinstance(task, (BinaryClassificationTask, RegressionTask))
+                    and task.summary_type
+                ):
+                    dims = (None,)
                 else:
-                    is_list = False
+                    dims = (None, task.target_dim)
                 properties = {
                     "int_domain": int_domain,
                 }
-                col_schema = ColumnSchema(
-                    name, dtype=np.float32, properties=properties, is_list=is_list, is_ragged=False
-                )
+                col_schema = ColumnSchema(name, dtype=np.float32, properties=properties, dims=dims)
                 output_cols.append(col_schema)
 
         return Core_Schema(output_cols)
 
+    @property
+    def prediction_tasks(self):
+        return [task for head in self.heads for task in list(head.prediction_task_dict.values())]
+
     def save(self, path: Union[str, os.PathLike], model_name="t4rec_model_class"):
         """Saves the model to f"{export_path}/{model_name}.pkl" using `cloudpickle`
-
         Parameters
         ----------
         path : Union[str, os.PathLike]
             Path to the directory where the T4Rec model should be saved.
         model_name : str, optional
            the name given to the pickle file storing the T4Rec model,
             by default 't4rec_model_class'
@@ -807,15 +812,14 @@
         export_path = export_path / model_name
         with open(export_path, "wb") as out:
             cloudpickle.dump(self, out)
 
     @classmethod
     def load(cls, path: Union[str, os.PathLike], model_name="t4rec_model_class") -> "Model":
         """Loads a T4Rec model that was saved with `model.save()`.
-
         Parameters
         ----------
         path : Union[str, os.PathLike]
             Path to the directory where the T4Rec model is saved.
         model_name : str, optional
            the name given to the pickle file storing the T4Rec model,
             by default 't4rec_model_class'.
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/model/prediction_task.py` & `transformers4rec-23.4.0/transformers4rec/torch/model/prediction_task.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import logging
-from typing import Dict, Iterable, Optional
+from math import sqrt
+from typing import Dict, Iterable, Optional, Sequence, Tuple
 
 import torch
 import torchmetrics as tm
 
 from ..block.base import Block, BuildableBlock, SequentialBlock
 from ..block.mlp import MLPBlock
 from ..masking import MaskedLanguageModeling
@@ -32,15 +33,15 @@
 
 
 class BinaryClassificationPrepareBlock(BuildableBlock):
     def build(self, input_size) -> SequentialBlock:
         return SequentialBlock(
             torch.nn.Linear(input_size[-1], 1, bias=False),
             torch.nn.Sigmoid(),
-            LambdaModule(lambda x: x.view(-1)),
+            LambdaModule(lambda x: torch.squeeze(x, -1)),
             output_size=[
                 None,
             ],
         )
 
 
 class BinaryClassificationTask(PredictionTask):
@@ -153,15 +154,15 @@
         )
 
 
 class RegressionPrepareBlock(BuildableBlock):
     def build(self, input_size) -> SequentialBlock:
         return SequentialBlock(
             torch.nn.Linear(input_size[-1], 1),
-            LambdaModule(lambda x: x.view(-1)),
+            LambdaModule(lambda x: torch.squeeze(x, -1)),
             output_size=[
                 None,
             ],
         )
 
 
 class RegressionTask(PredictionTask):
@@ -211,39 +212,47 @@
     softmax_temperature: float
         Softmax temperature, used to reduce model overconfidence, so that softmax(logits / T).
         Value 1.0 reduces to regular softmax.
     padding_idx: int
         pad token id.
     target_dim: int
         vocabulary size of item ids
+    sampled_softmax: Optional[bool]
+        Enables sampled softmax. By default False
+    max_n_samples: Optional[int]
+        Number of samples for sampled softmax. By default 100
     """
 
     DEFAULT_METRICS = (
         # default metrics suppose labels are int encoded
         NDCGAt(top_ks=[10, 20], labels_onehot=True),
         AvgPrecisionAt(top_ks=[10, 20], labels_onehot=True),
         RecallAt(top_ks=[10, 20], labels_onehot=True),
     )
 
     def __init__(
         self,
-        loss: torch.nn.Module = torch.nn.NLLLoss(ignore_index=0),
+        loss: torch.nn.Module = torch.nn.CrossEntropyLoss(),
         metrics: Iterable[tm.Metric] = DEFAULT_METRICS,
         task_block: Optional[BlockType] = None,
         task_name: str = "next-item",
         weight_tying: bool = False,
         softmax_temperature: float = 1,
         padding_idx: int = 0,
         target_dim: int = None,
+        sampled_softmax: Optional[bool] = False,
+        max_n_samples: Optional[int] = 100,
     ):
         super().__init__(loss=loss, metrics=metrics, task_block=task_block, task_name=task_name)
         self.softmax_temperature = softmax_temperature
         self.weight_tying = weight_tying
         self.padding_idx = padding_idx
         self.target_dim = target_dim
+        self.sampled_softmax = sampled_softmax
+        self.max_n_samples = max_n_samples
 
         self.item_embedding_table = None
         self.masking = None
 
     def build(self, body, input_size, device=None, inputs=None, task_block=None, pre=None):
         """Build method, this is called by the `Head`."""
         if not len(input_size) == 3 or isinstance(input_size, dict):
@@ -282,14 +291,17 @@
             )
         self.padding_idx = self.masking.padding_idx
         pre = NextItemPredictionPrepareBlock(
             target_dim=self.target_dim,
             weight_tying=self.weight_tying,
             item_embedding_table=self.item_embedding_table,
             softmax_temperature=self.softmax_temperature,
+            sampled_softmax=self.sampled_softmax,
+            max_n_samples=self.max_n_samples,
+            min_id=self.padding_idx + 1,
         )
         super().build(
             body, input_size, device=device, inputs=inputs, task_block=task_block, pre=pre
         )
 
     def forward(self, inputs: torch.Tensor, targets=None, training=False, testing=False, **kwargs):
         if isinstance(inputs, (tuple, list)):
@@ -300,41 +312,41 @@
             x = self.task_block(x)  # type: ignore
 
         # Retrieve labels from masking
         if training or testing:
             labels = self.masking.masked_targets  # type: ignore
             trg_flat = labels.flatten()
             non_pad_mask = trg_flat != self.padding_idx
-            labels_all = torch.masked_select(trg_flat, non_pad_mask)
+            labels_all = torch.masked_select(trg_flat, non_pad_mask).long()
             # remove padded items, keep only masked positions
             x = self.remove_pad_3d(x, non_pad_mask)
-            x = self.pre(x)  # type: ignore
-            loss = self.loss(x, labels_all)
+            y = labels_all
+            x, y = self.pre(x, targets=y, training=training, testing=testing)  # type: ignore
+
+            loss = self.loss(x, y)
             return {
                 "loss": loss,
-                "labels": labels_all,
+                "labels": y,
                 "predictions": x,
-                # "pred_metadata": {},
-                # "model_outputs": [],
             }
         else:
             # Get the hidden position to use for predicting the next item
             labels = self.embeddings.item_seq
             non_pad_mask = labels != self.padding_idx
             rows_ids = torch.arange(labels.size(0), dtype=torch.long, device=labels.device)
             if isinstance(self.masking, MaskedLanguageModeling):
                 last_item_sessions = non_pad_mask.sum(dim=1)
             else:
                 last_item_sessions = non_pad_mask.sum(dim=1) - 1
             x = x[rows_ids, last_item_sessions]
 
-        # Compute predictions probs
-        x = self.pre(x)  # type: ignore
+            # Compute predictions probs
+            x, _ = self.pre(x)  # type: ignore
 
-        return x
+            return x
 
     def remove_pad_3d(self, inp_tensor, non_pad_mask):
         # inp_tensor: (n_batch x seqlen x emb_dim)
         inp_tensor = inp_tensor.flatten(end_dim=1)
         inp_tensor_fl = torch.masked_select(
             inp_tensor, non_pad_mask.unsqueeze(1).expand_as(inp_tensor)
         )
@@ -373,29 +385,38 @@
 class NextItemPredictionPrepareBlock(BuildableBlock):
     def __init__(
         self,
         target_dim: int,
         weight_tying: bool = False,
         item_embedding_table: Optional[torch.nn.Module] = None,
         softmax_temperature: float = 0,
+        sampled_softmax: Optional[bool] = False,
+        max_n_samples: Optional[int] = 100,
+        min_id: Optional[int] = 0,
     ):
         super().__init__()
         self.target_dim = target_dim
         self.weight_tying = weight_tying
         self.item_embedding_table = item_embedding_table
         self.softmax_temperature = softmax_temperature
+        self.sampled_softmax = sampled_softmax
+        self.max_n_samples = max_n_samples
+        self.min_id = min_id
 
     def build(self, input_size) -> Block:
         return Block(
             _NextItemPredictionTask(
                 input_size,
                 self.target_dim,
                 self.weight_tying,
                 self.item_embedding_table,
                 self.softmax_temperature,
+                self.sampled_softmax,
+                self.max_n_samples,
+                self.min_id,
             ),
             [-1, self.target_dim],
         )
 
 
 class _NextItemPredictionTask(torch.nn.Module):
     """Predict the interacted item-id probabilities.
@@ -413,54 +434,258 @@
         weight_tying: bool
             The item id embedding table weights are shared with the prediction network layer.
         item_embedding_table: torch.nn.Module
             Module that's used to store the embedding table for the item.
         softmax_temperature: float
             Softmax temperature, used to reduce model overconfidence, so that softmax(logits / T).
             Value 1.0 reduces to regular softmax.
+        sampled_softmax: Optional[bool]
+            Enables sampled softmax. By default False
+        max_n_samples: Optional[int]
+            Number of samples for sampled softmax. By default 100
+        min_id : Optional[int]
+            The minimum value of the range for the log-uniform sampling. By default 0.
     """
 
     def __init__(
         self,
-        input_size: int,
+        input_size: Sequence,
         target_dim: int,
         weight_tying: bool = False,
         item_embedding_table: Optional[torch.nn.Module] = None,
         softmax_temperature: float = 0,
+        sampled_softmax: Optional[bool] = False,
+        max_n_samples: Optional[int] = 100,
+        min_id: Optional[int] = 0,
     ):
         super().__init__()
         self.input_size = input_size
         self.target_dim = target_dim
         self.weight_tying = weight_tying
         self.item_embedding_table = item_embedding_table
         self.softmax_temperature = softmax_temperature
-        self.log_softmax = torch.nn.LogSoftmax(dim=-1)
+        self.sampled_softmax = sampled_softmax
 
-        if self.weight_tying:
-            self.output_layer_bias = torch.nn.Parameter(torch.Tensor(self.target_dim))
-            torch.nn.init.zeros_(self.output_layer_bias)
-        else:
-            self.output_layer = torch.nn.Linear(
-                self.input_size[-1], self.target_dim  # type: ignore
+        if not self.weight_tying:
+            self.output_layer = torch.nn.Parameter(torch.empty(self.target_dim, input_size[-1]))
+            torch.nn.init.kaiming_uniform_(self.output_layer, a=sqrt(5))
+
+        if self.sampled_softmax:
+            self.sampler = LogUniformSampler(
+                max_n_samples=max_n_samples,
+                max_id=target_dim,
+                min_id=min_id,
+                unique_sampling=True,
             )
 
-    def forward(self, inputs: torch.Tensor) -> torch.Tensor:
+    def forward(
+        self,
+        inputs: torch.Tensor,
+        targets: Optional[torch.Tensor] = None,
+        training=False,
+        testing=False,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
         if self.weight_tying:
-            logits = torch.nn.functional.linear(
-                inputs,
-                weight=self.item_embedding_table.weight,  # type: ignore
-                bias=self.output_layer_bias,
-            )
+            output_weights = self.item_embedding_table.weight
+        else:
+            output_weights = self.output_layer
+
+        if self.sampled_softmax and training:
+            logits, targets = self.sampled(inputs, targets, output_weights)
         else:
-            logits = self.output_layer(inputs)
+            logits = inputs @ output_weights.t()
 
         if self.softmax_temperature:
             # Softmax temperature to reduce model overconfidence
             # and better calibrate probs and accuracy
             logits = torch.div(logits, self.softmax_temperature)
 
-        predictions = self.log_softmax(logits)
+        return logits, targets
+
+    def sampled(self, inputs, targets, output_weights):
+        """Returns logits using sampled softmax"""
+        neg_samples, targets_probs, samples_probs = self.sampler.sample(targets)
 
-        return predictions
+        positive_weights = output_weights[targets]
+        negative_weights = output_weights[neg_samples]
+
+        positive_scores = (inputs * positive_weights).sum(dim=-1, keepdim=True)
+        negative_scores = inputs @ negative_weights.t()
+
+        # logQ correction, to not overpenalize popular items for being sampled
+        # more often as negatives
+        epsilon = 1e-16
+        positive_scores -= torch.unsqueeze(torch.log(targets_probs + epsilon), dim=-1)
+        negative_scores -= torch.unsqueeze(torch.log(samples_probs + epsilon), dim=0)
+
+        # Remove accidental matches
+        accidental_hits = torch.unsqueeze(targets, -1) == torch.unsqueeze(neg_samples, 0)
+        negative_scores[accidental_hits] = torch.finfo(torch.float16).min / 100.0
+
+        logits = torch.cat([positive_scores, negative_scores], axis=1)
+        new_targets = torch.zeros(logits.shape[0], dtype=torch.int64, device=targets.device)
+
+        return logits, new_targets
 
     def _get_name(self) -> str:
         return "NextItemPredictionTask"
+
+
+class LogUniformSampler(torch.nn.Module):
+    def __init__(
+        self,
+        max_n_samples: int,
+        max_id: int,
+        min_id: Optional[int] = 0,
+        unique_sampling: bool = True,
+        n_samples_multiplier_before_unique: int = 2,
+    ):
+        """LogUniformSampler samples negative samples based on a log-uniform distribution.
+        `P(class) = (log(class + 2) - log(class + 1)) / log(max_id + 1)`
+
+        This implementation is based on to:
+        https://github.com/kimiyoung/transformer-xl/blob/master/pytorch/utils/log_uniform_sampler.py
+        TensorFlow Reference:
+        https://github.com/tensorflow/tensorflow/blob/r1.10/tensorflow/python/ops/candidate_sampling_ops.py
+
+        LogUniformSampler assumes item ids are sorted decreasingly by their frequency.
+
+        if `unique_sampling==True`, then only unique sampled items will be returned.
+        The actual # samples will vary from run to run if `unique_sampling==True`,
+        as sampling without replacement (`torch.multinomial(..., replacement=False)`) is slow,
+        so we use `torch.multinomial(..., replacement=True).unique()` which doesn't guarantee
+        the same number of unique sampled items. You can try to increase
+        n_samples_multiplier_before_unique to increase the chances to have more
+        unique samples in that case.
+
+        Parameters
+        ----------
+        max_n_samples : int
+            The maximum desired number of negative samples. The number of samples might be
+            smaller than that if `unique_sampling==True`, as explained above.
+        max_id : int
+            The maximum value of the range for the log-uniform distribution.
+        min_id : Optional[int]
+            The minimum value of the range for the log-uniform sampling. By default 0.
+        unique_sampling : bool
+            Whether to return unique samples. By default True
+        n_samples_multiplier_before_unique : int
+            If unique_sampling=True, it is not guaranteed that the number of returned
+            samples will be equal to max_n_samples, as explained above.
+            You can increase n_samples_multiplier_before_unique to maximize
+            chances that a larger number of unique samples is returned.
+        """
+        super().__init__()
+
+        if max_id <= 0:
+            raise ValueError("max_id must be a positive integer.")
+        if max_n_samples <= 0:
+            raise ValueError("n_sample must be a positive integer.")
+
+        self.max_id = max_id
+        self.unique_sampling = unique_sampling
+        self.max_n_samples = max_n_samples
+        self.n_sample = max_n_samples
+        if self.unique_sampling:
+            self.n_sample = int(self.n_sample * n_samples_multiplier_before_unique)
+
+        with torch.no_grad():
+            dist = self.get_log_uniform_distr(max_id, min_id)
+            self.register_buffer("dist", dist)
+            unique_sampling_dist = self.get_unique_sampling_distr(dist, self.n_sample)
+            self.register_buffer("unique_sampling_dist", unique_sampling_dist)
+
+    def get_log_uniform_distr(self, max_id: int, min_id: int = 0) -> torch.Tensor:
+        """Approximates the items frequency distribution with log-uniform probability distribution
+        with P(class) = (log(class + 2) - log(class + 1)) / log(max_id + 1).
+        It assumes item ids are sorted decreasingly by their frequency.
+
+        Parameters
+        ----------
+        max_id : int
+            Maximum discrete value for sampling (e.g. cardinality of the item id)
+
+        Returns
+        -------
+        torch.Tensor
+            Returns the log uniform probability distribution
+        """
+        log_indices = torch.arange(1.0, max_id - min_id + 2.0, 1.0).log_()
+        probs = (log_indices[1:] - log_indices[:-1]) / log_indices[-1]
+        if min_id > 0:
+            probs = torch.cat([torch.zeros([min_id], dtype=probs.dtype), probs], axis=0)
+        return probs
+
+    def get_unique_sampling_distr(self, dist, n_sample):
+        """Returns the probability that each item is sampled at least once
+        given the specified number of trials. This is meant to be used when
+        self.unique_sampling == True.
+        That probability can be approximated by by 1 - (1 - p)^n
+        and we use a numerically stable version: -expm1(num_tries * log1p(-p))
+        """
+        return (-(-dist.double().log1p_() * n_sample).expm1_()).float()
+
+    def sample(self, labels: torch.Tensor):
+        """Sample negative samples and calculate their probabilities.
+
+        If `unique_sampling==True`, then only unique sampled items will be returned.
+        The actual # samples will vary from run to run if `unique_sampling==True`,
+        as sampling without replacement (`torch.multinomial(..., replacement=False)`) is slow,
+        so we use `torch.multinomial(..., replacement=True).unique()`
+        which doesn't guarantee the same number of unique sampled items.
+        You can try to increase n_samples_multiplier_before_unique
+        to increase the chances to have more unique samples in that case.
+
+        Parameters
+        ----------
+        labels : torch.Tensor, dtype=torch.long, shape=(batch_size,)
+            The input labels for which negative samples should be generated.
+
+        Returns
+        -------
+        neg_samples : torch.Tensor, dtype=torch.long, shape=(n_samples,)
+            The unique negative samples drawn from the log-uniform distribution.
+        true_probs : torch.Tensor, dtype=torch.float32, shape=(batch_size,)
+            The probabilities of the input labels according
+            to the log-uniform distribution (depends on self.unique_sampling choice).
+        samp_log_probs : torch.Tensor, dtype=torch.float32, shape=(n_samples,)
+            The probabilities of the sampled negatives according
+            to the log-uniform distribution (depends on self.unique_sampling choice).
+        """
+
+        if not torch.is_tensor(labels):
+            raise TypeError("Labels must be a torch.Tensor.")
+        if labels.dtype != torch.long:
+            raise ValueError("Labels must be a tensor of dtype long.")
+        if labels.dim() > 2 or (labels.dim() == 2 and min(labels.shape) > 1):
+            raise ValueError(
+                "Labels must be a 1-dimensional tensor or a 2-dimensional tensor"
+                "with one of the dimensions equal to 1."
+            )
+        if labels.size(0) == 0:
+            raise ValueError("Labels must not be an empty tensor.")
+        if (labels < 0).any() or (labels > self.max_id).any():
+            raise ValueError("All label values must be within the range [0, max_id].")
+
+        n_tries = self.n_sample
+
+        with torch.no_grad():
+            neg_samples = torch.multinomial(self.dist, n_tries, replacement=True).unique()[
+                : self.max_n_samples
+            ]
+
+            device = labels.device
+            neg_samples = neg_samples.to(device)
+
+            if self.unique_sampling:
+                dist = self.unique_sampling_dist
+            else:
+                dist = self.dist
+
+            true_probs = dist[labels]
+            samples_probs = dist[neg_samples]
+
+            return neg_samples, true_probs, samples_probs
+
+    def forward(self, labels):
+        return self.sample(labels)
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/ranking_metric.py` & `transformers4rec-23.4.0/transformers4rec/torch/ranking_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 #
 
 # Adapted from source code: https://github.com/karlhigley/ranking-metrics-torch
 from abc import abstractmethod
 
 import torch
 import torchmetrics as tm
+from merlin.models.utils.registry import Registry
 from torchmetrics.utilities.data import dim_zero_cat
 
-from merlin_standard_lib import Registry
-
 from .utils import torch_utils
 
 ranking_metrics_registry = Registry.class_registry("torch.ranking_metrics")
 
 
 class RankingMetric(tm.Metric):
     """
@@ -47,15 +46,15 @@
         # Store the mean of the batch metrics (for each cut-off at topk)
         self.add_state("metric_mean", default=[], dist_reduce_fx="cat")
 
     def update(self, preds: torch.Tensor, target: torch.Tensor, **kwargs):  # type: ignore
         # Computing the metrics at different cut-offs
         if self.labels_onehot:
             target = torch_utils.tranform_label_to_onehot(target, preds.size(-1))
-        metric = self._metric(torch.LongTensor(self.top_ks), preds.view(-1, preds.size(-1)), target)
+        metric = self._metric(self.top_ks, preds.view(-1, preds.size(-1)), target)
         self.metric_mean.append(metric)  # type: ignore
 
     def compute(self):
         # Computing the mean of the batch metrics (for each cut-off at topk)
         return dim_zero_cat(self.metric_mean).mean(0)
 
     @abstractmethod
@@ -168,17 +167,17 @@
         """
         ks, scores, labels = torch_utils.check_inputs(ks, scores, labels)
         topk_scores, _, topk_labels = torch_utils.extract_topk(ks, scores, labels)
         avg_precisions = torch_utils.create_output_placeholder(scores, ks)
 
         # Compute average precisions at K
         num_relevant = torch.sum(labels, dim=1)
-        max_k = ks.max().item()
+        max_k = max(ks)
 
-        precisions = self.precision_at(1 + torch.arange(max_k), topk_scores, topk_labels)
+        precisions = self.precision_at(list(range(1, max_k + 1)), topk_scores, topk_labels)
         rel_precisions = precisions * topk_labels
 
         for index, k in enumerate(ks):
             total_prec = rel_precisions[:, : int(k)].sum(dim=1)
             avg_precisions[:, index] = total_prec / num_relevant.clamp(min=1, max=k).to(
                 dtype=torch.float32, device=scores.device
             )  # Ensuring type is double, because it can be float if --fp16
@@ -211,17 +210,15 @@
             list of discounted cumulative gains at cutoffs
         """
         ks, scores, labels = torch_utils.check_inputs(ks, scores, labels)
         topk_scores, topk_indices, topk_labels = torch_utils.extract_topk(ks, scores, labels)
         dcgs = torch_utils.create_output_placeholder(scores, ks)
 
         # Compute discounts
-        discount_positions = torch.arange(ks.max().item()).to(
-            device=scores.device, dtype=torch.float32
-        )
+        discount_positions = torch.arange(max(ks)).to(device=scores.device, dtype=torch.float32)
 
         discount_log_base = torch.log(
             torch.Tensor([log_base]).to(device=scores.device, dtype=torch.float32)
         ).item()
 
         discounts = 1 / (torch.log(discount_positions + 2) / discount_log_base)
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/tabular/__init__.py` & `transformers4rec-23.4.0/transformers4rec/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/tabular/aggregation.py` & `transformers4rec-23.4.0/transformers4rec/torch/tabular/aggregation.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/tabular/base.py` & `transformers4rec-23.4.0/transformers4rec/torch/tabular/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from abc import ABC
+from copy import deepcopy
 from functools import reduce
 from typing import Dict, List, Optional, Tuple, Union
 
 import torch
+from merlin.models.utils.doc_utils import docstring_parameter
+from merlin.models.utils.registry import Registry
 
-from merlin_standard_lib import Registry, Schema
-from merlin_standard_lib.utils.doc_utils import docstring_parameter
+from merlin_standard_lib import Schema
 
 from ..block.base import BlockBase, SequentialBlock, right_shift_block
 from ..typing import TabularData, TensorOrTabularData
 from ..utils.torch_utils import OutputSizeMixin, calculate_batch_size_from_input_size
 
 tabular_transformation_registry: Registry = Registry.class_registry("torch.tabular_transformations")
 tabular_aggregation_registry: Registry = Registry.class_registry("torch.tabular_aggregations")
@@ -181,15 +183,15 @@
         tags
         kwargs
 
         Returns
         -------
         Optional[TabularModule]
         """
-        schema_copy = schema.copy()
+        schema_copy = deepcopy(schema)
         if tags:
             schema_copy = schema_copy.select_by_tag(tags)
 
         if not schema_copy.column_schemas:
             return None
 
         return cls.from_features(schema_copy.column_names, schema=schema_copy, **kwargs)
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/tabular/transformations.py` & `transformers4rec-23.4.0/transformers4rec/torch/tabular/transformations.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/trainer.py` & `transformers4rec-23.4.0/transformers4rec/torch/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR, EvalLoopOutput, SchedulerType
 from transformers.utils import logging
 
 from merlin_standard_lib import Schema
 
 from ..config.trainer import T4RecTrainingArguments
 from .model.base import Model
+from .model.prediction_task import NextItemPredictionTask
 from .utils.data_utils import T4RecDataLoader
 from .utils.torch_utils import nested_concat, nested_detach, nested_numpify, nested_truncate
 
 logger = logging.get_logger(__name__)
 
 
 class Trainer(BaseTrainer):
@@ -96,15 +97,14 @@
         eval_dataloader: Optional[DataLoader] = None,
         test_dataloader: Optional[DataLoader] = None,
         callbacks: Optional[List[TrainerCallback]] = [],
         compute_metrics=None,
         incremental_logging: bool = False,
         **kwargs,
     ):
-
         mock_dataset = DatasetMock()
 
         self.incremental_logging = incremental_logging
         if self.incremental_logging:
             self.past_global_steps = 0
             incremental_logging_callback = IncrementalLoggingCallback(self)
             callbacks.append(incremental_logging_callback)
@@ -124,44 +124,45 @@
         self.test_dataset_or_path = test_dataset_or_path
         self.train_dataloader = train_dataloader
         self.eval_dataloader = eval_dataloader
         self.test_dataloader = test_dataloader
         self.schema = schema
         self.incremental_logging = incremental_logging
 
+        # Set global_rank and global_size if DDP is used
+        if self.args.local_rank != -1:
+            self.device = self.local_rank = self.args.local_rank
+            self.global_size = self.args.world_size
+        else:
+            self.device = self.local_rank = None
+            self.global_size = None
+
     def get_train_dataloader(self):
         """
         Set the train dataloader to use by Trainer.
         It supports user defined data-loader set as an attribute in the constructor.
         When the attribute is None, The data-loader is defined using train_dataset
         and the `data_loader_engine` specified in Training Arguments.
         """
         if self.train_dataloader is not None:
             return self.train_dataloader
 
         assert self.schema is not None, "schema is required to generate Train Dataloader"
 
-        # Set global_rank and global_size if DDP is used
-        if self.args.local_rank != -1:
-            local_rank = self.args.local_rank
-            global_size = self.args.world_size
-        else:
-            local_rank = None
-            global_size = None
-
         return T4RecDataLoader.parse(self.args.data_loader_engine).from_schema(
             self.schema,
             self.train_dataset_or_path,
             self.args.per_device_train_batch_size,
             max_sequence_length=self.args.max_sequence_length,
             drop_last=self.args.dataloader_drop_last,
             shuffle=True,
             shuffle_buffer_size=self.args.shuffle_buffer_size,
-            global_rank=local_rank,
-            global_size=global_size,
+            global_rank=self.local_rank,
+            global_size=self.global_size,
+            device=self.device,
         )
 
     def get_eval_dataloader(self, eval_dataset=None):
         """
         Set the eval dataloader to use by Trainer.
         It supports user defined data-loader set as an attribute in the constructor.
         When the attribute is None, The data-loader is defined using eval_dataset
@@ -170,22 +171,26 @@
         if self.eval_dataloader is not None:
             return self.eval_dataloader
 
         if eval_dataset is None and self.eval_dataset is None:
             raise ValueError("Trainer: evaluation requires an eval_dataset.")
         eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
         assert self.schema is not None, "schema is required to generate Eval Dataloader"
+
         return T4RecDataLoader.parse(self.args.data_loader_engine).from_schema(
             self.schema,
             self.eval_dataset_or_path,
             self.args.per_device_eval_batch_size,
             max_sequence_length=self.args.max_sequence_length,
             drop_last=self.args.dataloader_drop_last,
             shuffle=False,
             shuffle_buffer_size=self.args.shuffle_buffer_size,
+            global_rank=self.local_rank,
+            global_size=self.global_size,
+            device=self.device,
         )
 
     def get_test_dataloader(self, test_dataset=None):
         """
         Set the test dataloader to use by Trainer.
         It supports user defined data-loader set as an attribute in the constructor.
         When the attribute is None, The data-loader is defined using test_dataset
@@ -202,14 +207,17 @@
             self.schema,
             test_dataset,
             self.args.per_device_eval_batch_size,
             max_sequence_length=self.args.max_sequence_length,
             drop_last=self.args.dataloader_drop_last,
             shuffle=False,
             shuffle_buffer_size=self.args.shuffle_buffer_size,
+            global_rank=self.local_rank,
+            global_size=self.global_size,
+            device=self.device,
         )
 
     def num_examples(self, dataloader: DataLoader):
         """
         Overriding :obj:`Trainer.num_examples()` method because
         the data loaders for this project do not return the dataset size,
         but the number of steps. So we estimate the dataset size here
@@ -348,15 +356,15 @@
         to provide more flexibility to unpack results from the model,
         like returning labels that are not exactly one input feature
         model
         """
         inputs = self._prepare_inputs(inputs)
         inputs, targets = inputs
         with torch.no_grad():
-            if self.use_amp:
+            if self._use_cuda_amp:
                 with autocast():
                     outputs = model(inputs, targets=targets, training=training, testing=testing)
             else:
                 outputs = model(inputs, targets=targets, training=training, testing=testing)
 
         if testing:
             loss = outputs["loss"].mean().detach()
@@ -375,14 +383,26 @@
         #    for k, v in outputs.items()
         #    if k not in ignore_keys + ["loss", "predictions", "labels"]
         # }
         other_outputs = None
 
         return (loss, predictions, labels, other_outputs)
 
+    @property
+    def _use_cuda_amp(self):
+        """
+        Check for CUDA AMP that is compatible with versions of the
+        transformers package before and after version 4.20 (which
+        renamed the property `use_amp` to `use_cuda_amp`)
+        """
+        try:
+            return self.use_cuda_amp
+        except AttributeError:
+            return self.use_amp
+
     def evaluation_loop(
         self,
         dataloader: DataLoader,
         description: str,
         prediction_loss_only: Optional[bool] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: Optional[str] = "eval",
@@ -434,15 +454,15 @@
             raise ValueError("dataset must implement __len__")
 
         batch_size = dataloader._batch_size
 
         logger.info("***** Running %s *****", description)
         logger.info("  Batch size = %d", batch_size)
 
-        preds_item_ids_scores_host: Union[torch.Tensor, List[torch.Tensor]] = None
+        preds_host: Union[torch.Tensor, List[torch.Tensor], Dict[str, torch.Tensor]] = None
         labels_host: Union[torch.Tensor, List[torch.Tensor]] = None
 
         if metric_key_prefix == "train" and self.args.eval_steps_on_train_set:
             num_examples = self.args.eval_steps_on_train_set * batch_size
         else:
             num_examples = self.num_examples(dataloader)
 
@@ -451,19 +471,19 @@
         model.eval()
 
         self.callback_handler.eval_dataloader = dataloader
 
         # Initialize containers
         # losses/preds/labels on GPU/TPU (accumulated for eval_accumulation_steps)
         losses_host = None
-        preds_item_ids_scores_host = None
+        preds_host = None
         labels_host = None
         # losses/preds/labels on CPU (final containers)
         all_losses = None
-        all_preds_item_ids_scores = None
+        all_preds = None
         all_labels = None
         # Will be useful when we have an iterable dataset so don't know its length.
         observed_num_examples = 0
 
         # Iterate over dataloader
         for step, inputs in enumerate(dataloader):
             # Update the observed num examples
@@ -505,44 +525,60 @@
                 labels = self._nested_gather(labels)
                 labels_host = (
                     labels
                     if labels_host is None
                     else nested_concat(labels_host, labels, padding_index=0)
                 )
             if preds is not None and self.args.predict_top_k > 0:
+                # get outputs of next-item scores
                 if isinstance(preds, dict):
-                    assert (
-                        "next-item" in preds
-                    ), "Top-k prediction is specific to NextItemPredictionTask"
-                    preds = preds["next-item"]
+                    assert any(
+                        isinstance(x, NextItemPredictionTask) for x in model.prediction_tasks
+                    ), "Top-k prediction is specific to NextItemPredictionTask, "
+                    "Please ensure `self.args.predict_top_k == 0` "
+                    pred_next_item = preds["next-item"]
+                else:
+                    assert isinstance(
+                        model.prediction_tasks[0], NextItemPredictionTask
+                    ), "Top-k prediction is specific to NextItemPredictionTask, "
+                    "Please ensure `self.args.predict_top_k == 0` "
+                    pred_next_item = preds
+
                 preds_sorted_item_scores, preds_sorted_item_ids = torch.topk(
-                    preds, k=self.args.predict_top_k, dim=-1
+                    pred_next_item, k=self.args.predict_top_k, dim=-1
                 )
                 self._maybe_log_predictions(
                     labels,
                     preds_sorted_item_ids,
                     preds_sorted_item_scores,
                     # outputs["pred_metadata"],
                     metrics_results_detailed,
                     metric_key_prefix,
                 )
                 # The output predictions will be a tuple with the ranked top-n item ids,
                 # and item recommendation scores
-                preds_item_ids_scores = (
-                    preds_sorted_item_ids,
-                    preds_sorted_item_scores,
-                )
-                preds_item_ids_scores_host = (
-                    preds_item_ids_scores
-                    if preds_item_ids_scores_host is None
-                    else nested_concat(
-                        preds_item_ids_scores_host,
-                        preds_item_ids_scores,
+                if isinstance(preds, dict):
+                    preds["next-item"] = (
+                        preds_sorted_item_ids,
+                        preds_sorted_item_scores,
+                    )
+                else:
+                    preds = (
+                        preds_sorted_item_ids,
+                        preds_sorted_item_scores,
                     )
+
+            preds_host = (
+                preds
+                if preds_host is None
+                else nested_concat(
+                    preds_host,
+                    preds,
                 )
+            )
 
             self.control = self.callback_handler.on_prediction_step(
                 self.args, self.state, self.control
             )
 
             # Gather all tensors and put them back on the CPU
             # if we have done enough accumulation steps.
@@ -560,27 +596,27 @@
                 if labels_host is not None:
                     labels = nested_numpify(labels_host)
                     all_labels = (
                         labels
                         if all_labels is None
                         else nested_concat(all_labels, labels, padding_index=0)
                     )
-                if preds_item_ids_scores_host is not None:
-                    preds_item_ids_scores = nested_numpify(preds_item_ids_scores_host)
-                    all_preds_item_ids_scores = (
-                        preds_item_ids_scores
-                        if all_preds_item_ids_scores is None
+                if preds_host is not None:
+                    preds = nested_numpify(preds_host)
+                    all_preds = (
+                        preds
+                        if all_preds is None
                         else nested_concat(
-                            all_preds_item_ids_scores,
-                            preds_item_ids_scores,
+                            all_preds,
+                            preds,
                         )
                     )
 
                 # Set back to None to begin a new accumulation
-                losses_host, preds_item_ids_scores_host, labels_host = None, None, None
+                losses_host, preds_host, labels_host = None, None, None
 
         if self.args.past_index and hasattr(self, "_past"):
             # Clean the state at the end of the evaluation loop
             delattr(self, "_past")
 
         # Gather all remaining tensors and put them back on the CPU
         if losses_host is not None:
@@ -589,35 +625,35 @@
                 losses if all_losses is None else np.concatenate((all_losses, losses), axis=0)
             )
         if labels_host is not None:
             labels = nested_numpify(labels_host)
             all_labels = (
                 labels if all_labels is None else nested_concat(all_labels, labels, padding_index=0)
             )
-        if preds_item_ids_scores_host is not None:
-            preds_item_ids_scores = nested_numpify(preds_item_ids_scores_host)
-            all_preds_item_ids_scores = (
-                preds_item_ids_scores
-                if all_preds_item_ids_scores is None
+        if preds_host is not None:
+            preds_host = nested_numpify(preds_host)
+            all_preds = (
+                preds_host
+                if all_preds is None
                 else nested_concat(
-                    all_preds_item_ids_scores,
-                    preds_item_ids_scores,
+                    all_preds,
+                    preds_host,
                 )
             )
         # Get Number of samples :
         # the data loaders for this project do not return the dataset size,
         num_samples = observed_num_examples
 
         # Number of losses has been rounded to a multiple of batch_size
         # and in a distributed training, the number of
         # samplers has been rounded to a multiple of batch_size, so we truncate.
         if all_losses is not None:
             all_losses = all_losses[:num_samples]
-        if all_preds_item_ids_scores is not None:
-            all_preds_item_ids_scores = nested_truncate(all_preds_item_ids_scores, num_samples)
+        if all_preds is not None:
+            all_preds = nested_truncate(all_preds, num_samples)
         if all_labels is not None:
             all_labels = nested_truncate(all_labels, num_samples)
 
         # Get metrics :
         metrics = {}
         # Computing the metrics results as the average of all steps
         if self.compute_metrics and testing:
@@ -628,15 +664,15 @@
 
             metrics = {**metrics, **streaming_metrics_results_flattened}
 
         if testing:
             metrics[f"{metric_key_prefix}_/loss"] = all_losses.mean().item()
 
         return EvalLoopOutput(
-            predictions=all_preds_item_ids_scores,
+            predictions=all_preds,
             label_ids=all_labels,
             metrics=metrics,
             num_samples=num_examples,
         )
 
     def _save_model_and_checkpoint(self, save_model_class=False):
         """
@@ -699,15 +735,15 @@
         rng_file = os.path.join(checkpoint_path, "rng_state.pth")
         checkpoint_rng_state = torch.load(rng_file)
         random.setstate(checkpoint_rng_state["python"])
         np.random.set_state(checkpoint_rng_state["numpy"])
         torch.random.set_rng_state(checkpoint_rng_state["cpu"])
         torch.cuda.random.set_rng_state_all(checkpoint_rng_state["cuda"])
         # Restoring AMP scaler
-        if self.use_amp:
+        if self._use_cuda_amp:
             self.scaler.load_state_dict(torch.load(os.path.join(checkpoint_path, "scaler.pt")))
 
     @property
     def log_predictions_callback(self) -> Callable:
         return self.__log_predictions_callback
 
     @log_predictions_callback.setter
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/utils/__init__.py` & `transformers4rec-23.4.0/transformers4rec/types.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/utils/data_utils.py` & `transformers4rec-23.4.0/transformers4rec/torch/utils/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 import logging
 import warnings
 from abc import ABC
 
 import numpy as np
 import torch
 from merlin.dataloader.torch import Loader
+from merlin.models.utils.misc_utils import validate_dataset
+from merlin.models.utils.registry import Registry
+from merlin.schema import Tags
 from torch.utils.data import DataLoader as PyTorchDataLoader
 from torch.utils.data import Dataset, IterableDataset
 
-from merlin_standard_lib import Registry, Schema, Tag
-from merlin_standard_lib.utils.misc_utils import _augment_schema, validate_dataset
+from merlin_standard_lib import Schema
+from transformers4rec.torch.utils.padding import pad_batch
 
 from ...utils import dependencies
 
 logger = logging.getLogger(__name__)
 
 dataloader_registry: Registry = Registry("torch.dataloader_loader")
 
@@ -155,20 +158,20 @@
             batch_size: int
                 batch size of Dataloader.
             max_sequence_length: int
                 The maximum length of list features.
             """
 
             categorical_features = (
-                categorical_features or schema.select_by_tag(Tag.CATEGORICAL).column_names
+                categorical_features or schema.select_by_tag(Tags.CATEGORICAL).column_names
             )
             continuous_features = (
-                continuous_features or schema.select_by_tag(Tag.CONTINUOUS).column_names
+                continuous_features or schema.select_by_tag(Tags.CONTINUOUS).column_names
             )
-            targets = targets or schema.select_by_tag(Tag.TARGETS).column_names
+            targets = targets or schema.select_by_tag(Tags.TARGET).column_names
 
             cols_to_read = categorical_features + continuous_features + targets
 
             return cls(
                 paths_or_dataset,
                 batch_size,
                 max_sequence_length,
@@ -316,18 +319,14 @@
         self.max_sequence_length = max_sequence_length
         self.drop_last = drop_last
 
         reader_kwargs = reader_kwargs or {}
         reader_kwargs["row_groups_per_part"] = row_groups_per_part
         self.set_dataset(buffer_size, engine, reader_kwargs)
 
-        self.dataset.schema = _augment_schema(
-            self.dataset.schema, cats, conts, labels, sparse_names, sparse_max, sparse_as_dense
-        )
-
         if (global_rank is not None) and (self.dataset.npartitions < global_size):
             logger.warning(
                 "UserWarning: User is advised to repartition the parquet file before training "
                 "so npartitions>=global_size. Cudf or pandas can be used for repartitioning "
                 "eg. pdf.to_parquet('file.parquet',row_group_size=N_ROWS/NPARTITIONS) for pandas "
                 "or gdf.to_parquet('file.parquet',row_group_size_rows=N_ROWS/NPARTITIONS) for cudf "
                 "so that npartitions=nr_rows/row_group_size. Also ensure npartitions is divisible "
@@ -338,36 +337,76 @@
         if (global_rank is not None) and (self.dataset.npartitions % global_size != 0):
             logger.warning(
                 f"UserWarning: User is advised to set the number of partitions"
                 f" ({self.dataset.npartitions}) divisible by the number of available"
                 f" GPUs ({global_size}). This will divide the work equally among GPUs"
                 " for DDP training and ensure optimal performance."
             )
+
+        self.dataset.schema = self._augment_schema(
+            self.dataset.schema, cats=cats, conts=conts, labels=labels
+        )
+
         loader = Loader(
             self.dataset,
             self.batch_size,
             shuffle,
             seed_fn=seed_fn,
             parts_per_chunk=parts_per_chunk,
             device=device,
             global_size=global_size,
             global_rank=global_rank,
             drop_last=drop_last,
-        )
+        ).map(self._get_pad_fn(sparse_max))
 
         DLDataLoader.__init__(
             self,
             loader,
             collate_fn=collate_fn,
             batch_size=self.batch_size,
             drop_last=self.drop_last,
         )
         self.schema = schema
         self.max_sequence_length = max_sequence_length
 
+    @staticmethod
+    def _get_pad_fn(padding_lengths):
+        def pad_fn(x, y):
+            new_x = pad_batch(x, padding_lengths)
+            if y is not None and isinstance(y, dict):
+                new_y = pad_batch(y, padding_lengths)
+            else:
+                new_y = y
+            return new_x, new_y
+
+        return pad_fn
+
+    @staticmethod
+    def _augment_schema(
+        schema,
+        cats=None,
+        conts=None,
+        labels=None,
+    ):
+        cats = cats or []
+        conts = conts or []
+        labels = labels or []
+
+        schema = schema.select_by_name(conts + cats + labels)
+
+        labels = [labels] if isinstance(labels, str) else labels
+        for label in labels:
+            schema[label] = schema[label].with_tags(Tags.TARGET)
+        for label in cats:
+            schema[label] = schema[label].with_tags(Tags.CATEGORICAL)
+        for label in conts:
+            schema[label] = schema[label].with_tags(Tags.CONTINUOUS)
+
+        return schema
+
     def set_dataset(self, buffer_size, engine, reader_kwargs):
         dataset = validate_dataset(
             self.paths_or_dataset,
             self.batch_size,
             buffer_size,
             engine,
             reader_kwargs,
@@ -402,22 +441,22 @@
                 Path to paquet data of Dataset object.
             batch_size: int
                 batch size of Dataloader.
             max_sequence_length: int
                 The maximum length of list features.
         """
         categorical_features = (
-            categorical_features or schema.select_by_tag(Tag.CATEGORICAL).column_names
+            categorical_features or schema.select_by_tag(Tags.CATEGORICAL).column_names
         )
         continuous_features = (
-            continuous_features or schema.select_by_tag(Tag.CONTINUOUS).column_names
+            continuous_features or schema.select_by_tag(Tags.CONTINUOUS).column_names
         )
-        targets = targets or schema.select_by_tag(Tag.TARGETS).column_names
+        targets = targets or schema.select_by_tag(Tags.TARGET).column_names
         schema = schema.select_by_name(categorical_features + continuous_features + targets)
-        sparse_names = sparse_names or schema.select_by_tag(Tag.LIST).column_names
+        sparse_names = sparse_names or schema.select_by_tag(Tags.LIST).column_names
         sparse_max = sparse_max or {name: max_sequence_length for name in sparse_names}
         loader = cls(
             paths_or_dataset,
             batch_size=batch_size,
             max_sequence_length=max_sequence_length,
             labels=targets,
             cats=categorical_features,
@@ -470,15 +509,14 @@
 class ShuffleDataset(IterableDataset):
     def __init__(self, dataset, buffer_size):
         super().__init__()
         self.dataset = dataset
         self.buffer_size = buffer_size
 
     def __iter__(self):
-
         logger.info("[SHUFFLE] INITIALIZING BUFFER_SIZE: {}".format(self.buffer_size))
 
         raise StopIteration()
         # TODO define The shuffle method for pyarrow dataloader
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/utils/examples_utils.py` & `transformers4rec-23.4.0/transformers4rec/torch/utils/examples_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/utils/schema_utils.py` & `transformers4rec-23.4.0/transformers4rec/torch/utils/schema_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 # limitations under the License.
 #
 
 import random
 from typing import Any, Dict, Optional
 
 import torch
+from merlin.schema.io.proto_utils import has_field
 
 from merlin_standard_lib import Schema
-from merlin_standard_lib.utils.proto_utils import has_field
 
 from ..typing import TabularData
 
 
 def random_data_from_schema(
     schema: Schema,
     num_rows: int,
     max_session_length: Optional[int] = None,
     min_session_length: int = 5,
     device=None,
+    ragged=False,
 ) -> TabularData:
     data: Dict[str, Any] = {}
 
     for i in range(num_rows):
         session_length = None
         if max_session_length:
             session_length = random.randint(min_session_length, max_session_length)
@@ -83,21 +84,26 @@
             else:
                 data[feature.name] = row
 
     outputs: TabularData = {}
     for key, val in data.items():
         if isinstance(val, tuple):
             offsets = [0]
-            for length in val[1][:-1]:
-                offsets.append(offsets[-1] + length)
-            vals = (val[0], torch.tensor(offsets, device=device).unsqueeze(dim=1))
-            values, offsets, diff_offsets, num_rows = _pull_values_offsets(vals, device=device)
-            indices = _get_indices(offsets, diff_offsets, device=device)
-            seq_limit = max_session_length or val[1][0]
-            outputs[key] = _get_sparse_tensor(values, indices, num_rows, seq_limit)
+            for row_length in val[1]:
+                offsets.append(offsets[-1] + row_length)
+
+            if ragged:
+                outputs[f"{key}__values"] = val[0]
+                outputs[f"{key}__offsets"] = torch.tensor(offsets, device=device)
+            else:
+                vals = (val[0], torch.tensor(offsets[:-1], device=device).unsqueeze(dim=1))
+                values, offsets, diff_offsets, num_rows = _pull_values_offsets(vals, device=device)
+                indices = _get_indices(offsets, diff_offsets, device=device)
+                seq_limit = max_session_length or val[1][0]
+                outputs[key] = _get_sparse_tensor(values, indices, num_rows, seq_limit)
         else:
             outputs[key] = data[key]
 
     return outputs
 
 
 def _pull_values_offsets(values_offset, device=None):
```

### Comparing `transformers4rec-23.2.0/transformers4rec/torch/utils/torch_utils.py` & `transformers4rec-23.4.0/transformers4rec/torch/utils/torch_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 import abc
 from collections.abc import Mapping
 from dataclasses import dataclass
 from typing import Dict, Optional, Union
 
 import numpy as np
 import torch
+from merlin.schema import Schema as CoreSchema
+from merlin.schema.io.proto_utils import has_field
 
 from merlin_standard_lib import Schema
-from merlin_standard_lib.utils.proto_utils import has_field
+from merlin_standard_lib.schema.schema import ColumnSchema
 
 from ...config.schema import SchemaMixin
 from ..typing import TabularData
 
 
 class OutputSizeMixin(SchemaMixin, abc.ABC):
     def build(self, input_size, schema=None, **kwargs):
@@ -133,58 +135,80 @@
 def check_gpu(module):
     try:
         return next(module.parameters()).is_cuda
     except StopIteration:
         return False
 
 
+def _has_field(col_schema, field_name):
+    if isinstance(col_schema, ColumnSchema):
+        return has_field(col_schema, field_name)
+
+    return getattr(col_schema, field_name, None)
+
+
+def _get_size_from_shape(col_schema, batch_size) -> torch.Size:
+    shape = [batch_size]
+
+    if isinstance(col_schema, ColumnSchema):
+        if has_field(col_schema, "shape"):
+            shape += [d.size for d in col_schema.shape.dim]
+    elif col_schema.shape.dims is not None:
+        if len(col_schema.shape.dims) == 1 and col_schema.shape.dims[0].max is None:
+            return torch.Size(shape)
+        raise NotImplementedError("TODO: support shape.dims")
+
+    return torch.Size(shape)
+
+
 def get_output_sizes_from_schema(schema: Schema, batch_size=-1, max_sequence_length=None):
     sizes = {}
-    for feature in schema.feature:
+
+    features = schema if isinstance(schema, CoreSchema) else schema.feature
+
+    for feature in features:
         name = feature.name
         # Sequential or multi-hot feature
-        if has_field(feature, "value_count"):
+        if _has_field(feature, "value_count"):
             sizes[name] = torch.Size(
                 [
                     batch_size,
                     max_sequence_length if max_sequence_length else feature.value_count.max,
                 ]
             )
-        elif has_field(feature, "shape"):
-            sizes[name] = torch.Size([batch_size] + [d.size for d in feature.shape.dim])
         else:
-            sizes[name] = torch.Size([batch_size])
+            sizes[name] = _get_size_from_shape(feature, batch_size)
 
     return sizes
 
 
 def calculate_batch_size_from_input_size(input_size):
     if isinstance(input_size, dict):
         input_size = [i for i in input_size.values() if isinstance(i, torch.Size)][0]
 
     return input_size[0]
 
 
 def check_inputs(ks, scores, labels):
-    if len(ks.shape) > 1:
-        raise ValueError("ks should be a 1-dimensional tensor")
+    if not (isinstance(ks, (list, tuple)) and len(ks) >= 1):
+        raise ValueError("ks should be a list or tuple with at least one element")
 
     if len(scores.shape) != 2:
         raise ValueError("scores must be a 2-dimensional tensor")
 
     if len(labels.shape) != 2:
         raise ValueError("labels must be a 2-dimensional tensor")
 
     if scores.shape != labels.shape:
         raise ValueError("scores and labels must be the same shape")
 
     return (
-        ks.to(dtype=torch.int32, device=scores.device),
+        ks,
         scores,
-        labels,  # .to(dtype=torch.float32, device=scores.device),
+        labels,
     )
 
 
 def extract_topk(ks, scores, labels):
     max_k = int(max(ks))
     topk_scores, topk_indices = torch.topk(scores, max_k)
     topk_labels = torch.gather(labels, 1, topk_indices)
@@ -238,15 +262,16 @@
     elif isinstance(tensors, np.ndarray):
         return numpy_pad_and_concatenate(tensors, new_tensors, padding_index=padding_index)
     else:
         raise TypeError(f"Unsupported type for concatenation: got {type(tensors)}")
 
 
 def torch_pad_and_concatenate(tensor1, tensor2, padding_index=-100):
-    """Concatenates `tensor1` and `tensor2` on first axis, applying padding on the second if necessary.
+    """Concatenates `tensor1` and `tensor2` on first axis, applying padding on the second as needed
+
     #TODO this method was copied from the latest version of HF transformers library to support
     dict outputs. So we should remove it when T4Rec is updated to use the latest version
     """
     tensor1 = atleast_1d(tensor1)
     tensor2 = atleast_1d(tensor2)
 
     if len(tensor1.shape) == 1 or tensor1.shape[1] == tensor2.shape[1]:
```

### Comparing `transformers4rec-23.2.0/transformers4rec/types.py` & `transformers4rec-23.4.0/transformers4rec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec/utils/__init__.py` & `transformers4rec-23.4.0/tests/unit/torch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+import pytest
+
+pytest.importorskip("torch")
```

### Comparing `transformers4rec-23.2.0/transformers4rec/utils/dependencies.py` & `transformers4rec-23.4.0/transformers4rec/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.2.0/transformers4rec.egg-info/PKG-INFO` & `transformers4rec-23.4.0/transformers4rec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers4rec
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: pytorch
 Provides-Extra: nvtabular
-Provides-Extra: dataloader
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
```

### Comparing `transformers4rec-23.2.0/versioneer.py` & `transformers4rec-23.4.0/versioneer.py`

 * *Files identical despite different names*

