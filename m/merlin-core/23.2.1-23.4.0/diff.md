# Comparing `tmp/merlin-core-23.2.1.tar.gz` & `tmp/merlin-core-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-core-23.2.1.tar", last modified: Fri Mar 10 09:44:39 2023, max compression
+gzip compressed data, was "merlin-core-23.4.0.tar", last modified: Wed Apr 26 16:36:00 2023, max compression
```

## Comparing `merlin-core-23.2.1.tar` & `merlin-core-23.4.0.tar`

### file list

```diff
@@ -1,82 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.483296 merlin-core-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-10 09:44:10.000000 merlin-core-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-10 09:44:10.000000 merlin-core-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-10 09:44:39.483296 merlin-core-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-10 09:44:10.000000 merlin-core-23.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.475296 merlin-core-23.2.1/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.483296 merlin-core-23.2.1/merlin/core/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-10 09:44:39.483296 merlin-core-23.2.1/merlin/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/core/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/core/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/core/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.479296 merlin-core-23.2.1/merlin/dag/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/dictarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22773 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.479296 merlin-core-23.2.1/merlin/dag/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/ops/concat_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/ops/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/ops/subset_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/ops/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.479296 merlin-core-23.2.1/merlin/dtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.479296 merlin-core-23.2.1/merlin/dtypes/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/cudf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/mappings/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/dtypes/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.479296 merlin-core-23.2.1/merlin/io/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/avro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/dataframe_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/dataframe_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51011 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/dataset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)    46743 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/io/writer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.483296 merlin-core-23.2.1/merlin/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.483296 merlin-core-23.2.1/merlin/schema/io/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/io/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/io/schema_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/io/tensorflow_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-10 09:44:10.000000 merlin-core-23.2.1/merlin/schema/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:44:39.483296 merlin-core-23.2.1/merlin_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-10 09:44:39.000000 merlin-core-23.2.1/merlin_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-10 09:44:10.000000 merlin-core-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-10 09:44:10.000000 merlin-core-23.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-10 09:44:10.000000 merlin-core-23.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-10 09:44:39.483296 merlin-core-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-10 09:44:10.000000 merlin-core-23.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-03-10 09:44:10.000000 merlin-core-23.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 16:35:32.000000 merlin-core-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 16:35:32.000000 merlin-core-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 16:36:00.535273 merlin-core-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-26 16:35:32.000000 merlin-core-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.527273 merlin-core-23.4.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/core/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/has_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/dictarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15397 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dag/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/concat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/subset_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dispatch/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dtypes/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/avro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataframe_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataframe_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53986 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/hugectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/writer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/schema/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/schema_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/tensorflow_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/cupy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/numpy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensor_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensor_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensorflow_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/torch_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-26 16:35:32.000000 merlin-core-23.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 16:35:32.000000 merlin-core-23.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 16:35:32.000000 merlin-core-23.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 16:36:00.535273 merlin-core-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 16:35:32.000000 merlin-core-23.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-04-26 16:35:32.000000 merlin-core-23.4.0/versioneer.py
```

### Comparing `merlin-core-23.2.1/LICENSE` & `merlin-core-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/PKG-INFO` & `merlin-core-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.2.1
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-core-23.2.1/README.md` & `merlin-core-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/core/__init__.py` & `merlin-core-23.4.0/merlin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/core/compat.py` & `merlin-core-23.4.0/merlin/core/has_gpu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import os
 
-try:
-    from numba import cuda  # pylint: disable=unused-import
-except ImportError:
-    cuda = None
+# pylint: disable=unused-import
+import os
 
 from dask.distributed.diagnostics import nvml
 
 
 def _get_gpu_count():
     """Get Number of GPU devices accounting for CUDA_VISIBLE_DEVICES environment variable"""
     # Using the `dask.distributed.diagnostics.nvml.device_get_count`
```

### Comparing `merlin-core-23.2.1/merlin/core/dispatch.py` & `merlin-core-23.4.0/merlin/core/dispatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,42 +20,38 @@
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
-from merlin.core.compat import HAS_GPU
+# unused HAS_GPU import is here for backwards compatibility
+from merlin.core.compat import HAS_GPU  # pylint: disable=unused-import # noqa: F401
+from merlin.core.compat import cudf
+from merlin.core.compat import cupy as cp
 from merlin.core.protocols import DataFrameLike, DictLike, SeriesLike
 
-cudf = None
-cp = None
 rmm = None
 
-if HAS_GPU:
+if cudf:
     try:
-        import cudf  # type: ignore[no-redef]
         import dask_cudf
         import rmm  # type: ignore[no-redef]
         from cudf.core.column import as_column, build_column
 
         try:
             # cudf >= 21.08
             from cudf.api.types import is_list_dtype as cudf_is_list_dtype
             from cudf.api.types import is_string_dtype as cudf_is_string_dtype
         except ImportError:
             # cudf < 21.08
             from cudf.utils.dtypes import is_list_dtype as cudf_is_list_dtype
             from cudf.utils.dtypes import is_string_dtype as cudf_is_string_dtype
     except ImportError:
         pass
-    try:
-        import cupy as cp  # type: ignore[no-redef]
-    except ImportError:
-        pass
 
 try:
     # Dask >= 2021.5.1
     from dask.dataframe.core import hash_object_dispatch
 except ImportError:
     # Dask < 2021.5.1
     from dask.dataframe.utils import hash_object_dispatch
@@ -73,27 +69,35 @@
                 return func(*args, **kwargs)
 
             return inner2
 
         return inner1
 
 
-if HAS_GPU and cudf:
+if cudf:
     DataFrameType = Union[pd.DataFrame, cudf.DataFrame]  # type: ignore
     SeriesType = Union[pd.Series, cudf.Series]  # type: ignore
 else:
     DataFrameType = pd.DataFrame  # type: ignore
     SeriesType = pd.Series  # type: ignore
 
 
 # Define mapping between non-nullable,
 # and nullable types in Pandas
 _PD_NULLABLE_MAP = {
+    "float32": "Float32",
+    "float64": "Float64",
+    "int8": "Int8",
+    "int16": "Int16",
     "int32": "Int32",
     "int64": "Int64",
+    "uint8": "UInt8",
+    "uint16": "UInt16",
+    "uint32": "UInt32",
+    "uint64": "UInt64",
 }
 
 
 class ExtData(enum.Enum):
     """Simple Enum to track external-data types"""
 
     DATASET = 0
@@ -120,56 +124,56 @@
             df = df.compute()
         return Dataset(df)
     return df
 
 
 def read_parquet_metadata(path):
     """Read parquet metadata from path"""
-    if HAS_GPU:
+    if cudf:
         return cudf.io.read_parquet_metadata(path)
     full_meta = pq.read_metadata(path)
     pf = pq.ParquetFile(path)
     return full_meta.num_rows, full_meta.num_row_groups, pf.schema.names
 
 
 def get_lib():
     """Dispatch to the appropriate library (cudf or pandas) for the current environment"""
-    return cudf if HAS_GPU else pd
+    return cudf if (cudf and HAS_GPU) else pd
 
 
 def reinitialize(managed_memory=False):
     if rmm:
         rmm.reinitialize(managed_memory=managed_memory)
     return
 
 
 def random_uniform(size):
     """Dispatch for numpy.random.RandomState"""
-    if HAS_GPU:
+    if cp:
         return cp.random.uniform(size=size)
     else:
         return np.random.uniform(size=size)
 
 
 def coo_matrix(data, row, col):
     """Dispatch for scipy.sparse.coo_matrix"""
-    if HAS_GPU:
+    if cp:
         return cp.sparse.coo_matrix((data, row, col))
     else:
         import scipy
 
         return scipy.sparse.coo_matrix((data, row, col))
 
 
 def is_dataframe_object(x):
     # Simple check if object is a cudf or pandas
     # DataFrame object
-    if not HAS_GPU:
-        return isinstance(x, pd.DataFrame)
-    return isinstance(x, (cudf.DataFrame, pd.DataFrame))
+    if cudf:
+        return isinstance(x, (cudf.DataFrame, pd.DataFrame))
+    return isinstance(x, pd.DataFrame)
 
 
 def nullable_series(data, like_df, dtype):
     # Return a Series containing the elements in `data`,
     # with a nullable version of `dtype`, using `like_df`
     # to infer the Series constructor
     if isinstance(like_df, pd.DataFrame):
@@ -178,17 +182,17 @@
         return like_df._constructor_sliced(data, dtype=_PD_NULLABLE_MAP.get(str(dtype), dtype))
     return like_df._constructor_sliced(data, dtype=dtype)
 
 
 def is_series_object(x):
     # Simple check if object is a cudf or pandas
     # Series object
-    if not HAS_GPU:
-        return isinstance(x, pd.Series)
-    return isinstance(x, (cudf.Series, pd.Series))
+    if cudf:
+        return isinstance(x, (cudf.Series, pd.Series))
+    return isinstance(x, pd.Series)
 
 
 def is_cpu_object(x):
     # Simple check if object is a cudf or pandas
     # DataFrame object
     return isinstance(x, (pd.DataFrame, pd.Series))
 
@@ -213,58 +217,94 @@
         if s.dtype == "object":
             s = s.str.htoi()
         return s.astype(dtype or np.int32)
 
 
 def random_state(seed, like_df=None):
     """Dispatch for numpy.random.RandomState"""
-    if not HAS_GPU or isinstance(like_df, (pd.DataFrame, pd.Series)):
+    if like_df is None:
+        return cp.random.RandomState(seed) if cp else np.random.RandomState(seed)
+    elif isinstance(like_df, (pd.DataFrame, pd.Series, pd.RangeIndex)):
         return np.random.RandomState(seed)
-    else:
+    elif cudf and isinstance(like_df, (cudf.DataFrame, cudf.Series, cudf.RangeIndex)):
         return cp.random.RandomState(seed)
+    else:
+        raise ValueError(
+            "Unsupported dataframe type: "
+            f"{type(like_df)}"
+            " Supported types: a DataFrame, Series, or RangeIndex (cudf or pandas)."
+        )
 
 
 def arange(size, like_df=None, dtype=None):
     """Dispatch for numpy.arange"""
-    if not HAS_GPU or isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series)):
+    if like_df is None:
+        return cp.arange(size, dtype=dtype) if cp else np.arange(size, dtype=dtype)
+    elif isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series, pd.RangeIndex)):
         return np.arange(size, dtype=dtype)
-    else:
+    elif cudf and isinstance(like_df, (cp.ndarray, cudf.DataFrame, cudf.Series, cudf.RangeIndex)):
         return cp.arange(size, dtype=dtype)
+    else:
+        raise ValueError(
+            "Unsupported dataframe type: "
+            f"{type(like_df)}"
+            " Expected either a pandas or cudf DataFrame or Series."
+        )
 
 
 def array(x, like_df=None, dtype=None):
     """Dispatch for numpy.array"""
-    if not HAS_GPU or isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series)):
+    if like_df is None:
+        return cp.array(x, dtype=dtype) if cp else np.array(x, dtype=dtype)
+    elif isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series, pd.RangeIndex)):
         return np.array(x, dtype=dtype)
-    else:
+    elif cudf and isinstance(like_df, (cp.ndarray, cudf.DataFrame, cudf.Series, cudf.RangeIndex)):
         return cp.array(x, dtype=dtype)
+    else:
+        raise ValueError(
+            "Unsupported dataframe type: "
+            f"{type(like_df)}"
+            " Expected either a pandas or cudf DataFrame or Series."
+        )
 
 
 def zeros(size, like_df=None, dtype=None):
     """Dispatch for numpy.array"""
-    if not HAS_GPU or isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series)):
+    if like_df is None:
+        return cp.zeros(size, dtype=dtype) if cp else np.zeros(size, dtype=dtype)
+    elif isinstance(like_df, (np.ndarray, pd.DataFrame, pd.Series, cudf.RangeIndex)):
         return np.zeros(size, dtype=dtype)
-    else:
+    elif cudf and isinstance(like_df, (cp.ndarray, cudf.DataFrame, cudf.Series, cudf.RangeIndex)):
         return cp.zeros(size, dtype=dtype)
+    else:
+        raise ValueError(
+            "Unsupported dataframe type: "
+            f"{type(like_df)}"
+            " Expected either a pandas or cudf DataFrame or Series."
+        )
 
 
 def hash_series(ser):
     """Row-wise Series hash"""
-    if not HAS_GPU or isinstance(ser, pd.Series):
+    if isinstance(ser, pd.Series):
         # Using pandas hashing, which does not produce the
         # same result as cudf.Series.hash_values().  Do not
         # expect hash-based data transformations to be the
         # same on CPU and CPU.  TODO: Fix this (maybe use
         # murmurhash3 manually on CPU).
         return hash_object_dispatch(ser).values
-    else:
+    elif cudf and isinstance(ser, cudf.Series):
         if is_list_dtype(ser):
             return ser.list.leaves.hash_values()
         else:
             return ser.hash_values()
+    else:
+        raise ValueError(
+            "Unsupported series type: " f"{type(ser)}" " Expected either a pandas or cudf Series."
+        )
 
 
 def series_has_nulls(s):
     """Check if Series contains any null values"""
     if isinstance(s, pd.Series):
         return s.isnull().values.any()
     else:
@@ -297,28 +337,27 @@
     # adds detection when in merlin column
     if hasattr(ser, "is_list"):
         return ser[0].dtype
     return None
 
 
 def is_list_dtype(ser):
-    """Check if Series contains list elements"""
+    """Check if Series, dtype, or array contains or represents list elements"""
     # adds detection for merlin column
     if hasattr(ser, "is_list"):
         return ser.is_list
     if isinstance(ser, pd.Series):
         if not len(ser):  # pylint: disable=len-as-condition
             return False
         return pd.api.types.is_list_like(ser.values[0])
-    elif not HAS_GPU:
-        # either np.ndarray or a dtype
-        if isinstance(ser, np.ndarray):
-            ser = ser[0]
-        return pd.api.types.is_list_like(ser)
-    return cudf_is_list_dtype(ser)
+    elif cudf and isinstance(ser, (cudf.Series, cudf.ListDtype)):
+        return cudf_is_list_dtype(ser)
+    elif isinstance(ser, np.ndarray) or (cp and isinstance(ser, cp.ndarray)):
+        return len(ser.shape) > 1
+    return pd.api.types.is_list_like(ser)
 
 
 def is_string_dtype(dtype: np.dtype) -> bool:
     """Check if the dtype of obj is a string type
 
     Parameters
     ----------
@@ -326,26 +365,36 @@
         Potential string dtype to check
 
     Returns
     -------
     bool
         `True` if the dtype of `obj` is a string type
     """
-    if not HAS_GPU:
-        return pd.api.types.is_string_dtype(dtype)
-    else:
+    if cudf:
         return cudf_is_string_dtype(dtype)
+    return pd.api.types.is_string_dtype(dtype)
 
 
 def flatten_list_column_values(s):
     """returns a flattened list from a list column"""
-    if isinstance(s, pd.Series) or not cudf:
+    if isinstance(s, pd.Series):
         return pd.Series(itertools.chain(*s))
-    else:
+    elif cudf and isinstance(s, cudf.Series):
         return s.list.leaves
+    elif cp and isinstance(s, cp.ndarray):
+        return s.flatten()
+    elif isinstance(s, np.ndarray):
+        return s.flatten()
+    else:
+        raise ValueError(
+            "Unsupported series type: "
+            f"{type(s)} "
+            "Expected either a pandas or cuDF Series. "
+            "Or a NumPy or CuPy array"
+        )
 
 
 def flatten_list_column(s):
     """Flatten elements of a list-based column, and return as a DataFrame"""
     values = flatten_list_column_values(s)
     if isinstance(s, pd.Series) or not cudf:
         return pd.DataFrame({s.name: values})
@@ -376,29 +425,29 @@
 
 
 def read_parquet_dispatch(df: DataFrameLike) -> Callable:
     """Dispatch function for reading parquet files"""
     return read_dispatch(df=df, fmt="parquet")
 
 
-def read_dispatch(df: DataFrameLike = None, cpu=None, collection=False, fmt="parquet") -> Callable:
+def read_dispatch(
+    df: Union[DataFrameLike, str] = None, cpu=None, collection=False, fmt="parquet"
+) -> Callable:
     """Return the necessary read_parquet function to generate
     data of a specified type.
     """
-    if cpu or isinstance(df, pd.DataFrame) or not HAS_GPU:
+    if cpu or isinstance(df, pd.DataFrame):
         _mod = dd if collection else pd
+    elif cudf and isinstance(df, cudf.DataFrame):
+        _mod = dask_cudf if collection else cudf.io
     else:
         if collection:
-            _mod = dask_cudf
-        elif cudf is not None:
-            _mod = cudf.io
+            _mod = dask_cudf if cudf else dd
         else:
-            raise ValueError(
-                "Unable to load cudf. Please check your environment GPU and cudf available."
-            )
+            _mod = cudf.io if cudf else pd
     _attr = "read_csv" if fmt == "csv" else "read_parquet"
     return getattr(_mod, _attr)
 
 
 def parquet_writer_dispatch(df: DataFrameLike, path=None, **kwargs):
     """Return the necessary ParquetWriter class to write
     data of a specified type.
@@ -458,15 +507,15 @@
             children=(original._column.offsets, encoded),
         )
 
 
 def pull_apart_list(original, device=None):
     values = flatten_list_column_values(original)
     if isinstance(original, pd.Series):
-        offsets = pd.Series([0]).append(original.map(len).cumsum()).reset_index(drop=True)
+        offsets = pd.concat([pd.Series([0]), original.map(len).cumsum()]).reset_index(drop=True)
         if isinstance(offsets[0], list):
             offsets = pd.Series(offsets.reshape().flatten()).reset_index(drop=True)
     else:
         offsets = original._column.offsets
         elements = original._column.elements
         if isinstance(elements, cudf.core.column.lists.ListColumn):
             offsets = make_series(elements.offsets)[offsets]
@@ -481,23 +530,34 @@
         return x.to_arrow()
 
 
 def concat(objs, **kwargs):
     """dispatch function for concat"""
     if isinstance(objs[0], dd.DataFrame):
         return dd.multi.concat(objs)
-    elif isinstance(objs[0], (pd.DataFrame, pd.Series)) or not HAS_GPU:
+    elif isinstance(objs[0], (pd.DataFrame, pd.Series)):
         return pd.concat(objs, **kwargs)
-    else:
+    elif cudf and isinstance(objs[0], (cudf.DataFrame, cudf.Series)):
         return cudf.core.reshape.concat(objs, **kwargs)
+    else:
+        raise ValueError(
+            "Unsupported dataframe type: "
+            f"{type(objs[0])}"
+            " Expected a pandas, cudf, or dask DataFrame."
+        )
 
 
 def make_df(_like_df=None, device=None):
     """Return a DataFrame with the same dtype as `_like_df`"""
-    if not cudf or device == "cpu" or isinstance(_like_df, (pd.DataFrame, pd.Series)):
+    if (
+        not cudf
+        or device == "cpu"
+        or not HAS_GPU
+        or isinstance(_like_df, (pd.DataFrame, pd.Series))
+    ):
         # move to pandas need it on CPU (host memory)
         # can be a cudf, cupy or numpy Series
         if cudf and isinstance(_like_df, (cudf.DataFrame, cudf.Series)):
             # move to cpu
             return _like_df.to_pandas()
         if cp and isinstance(_like_df, cp.ndarray):
             return pd.DataFrame(_like_df.get())
@@ -580,15 +640,15 @@
             # Convert cudf-backed collection to pandas-backed collection
             return x.to_dask_dataframe()
         else:
             # Make sure _x is a pandas DataFrame
             _x = x if isinstance(x, pd.DataFrame) else x.to_pandas()
             # Output a collection if `to_collection=True`
             return dd.from_pandas(_x, sort=False, npartitions=npartitions) if to_collection else _x
-    else:
+    elif cudf and dask_cudf:
         if isinstance(x, dd.DataFrame):
             # If input is a Dask collection, convert to dask_cudf
             if isinstance(x, dask_cudf.DataFrame):
                 # Already a cudf-backed Dask collection
                 return x
             # Convert pandas-backed collection to cudf-backed collection
             return x.map_partitions(cudf.from_pandas)
@@ -603,34 +663,38 @@
                 _x = cudf.DataFrame.from_pandas(x)
             # Output a collection if `to_collection=True`
             return (
                 dask_cudf.from_cudf(_x, sort=False, npartitions=npartitions)
                 if to_collection
                 else _x
             )
+    else:
+        raise RuntimeError(
+            "Unable to move data to GPU. "
+            "cudf and dask_cudf are not available. "
+            "Make sure these packages are installed and can be imported in this environment. "
+        )
 
 
 def to_host(x):
     """Move cudf.DataFrame to host memory for caching.
 
     All other data will pass through unchanged.
     """
-    if not HAS_GPU or isinstance(x, (pd.DataFrame, dd.DataFrame)):
-        return x
-    else:
+    if cudf and isinstance(x, cudf.DataFrame):
         return x.to_arrow()
+    return x
 
 
 def from_host(x):
-    if not HAS_GPU:
-        return x
-    elif isinstance(x, cudf.DataFrame):
-        return x
-    else:
+    if isinstance(x, pd.DataFrame):
+        return cudf.DataFrame.from_pandas(x)
+    elif isinstance(x, pa.Table):
         return cudf.DataFrame.from_arrow(x)
+    return x
 
 
 def build_cudf_list_column(new_elements, new_offsets):
     """Method creates a List series from the corresponding elements and
     row_lengths
 
     Parameters
@@ -641,22 +705,22 @@
         The corresponding row lengths of the elements
 
     Returns
     -------
     cudf.Series
         The list column with corresponding elements and row_lengths as a series.
     """
-    if not HAS_GPU:
-        return []
-    return build_column(
-        None,
-        dtype=cudf.core.dtypes.ListDtype(new_elements.dtype),
-        size=new_offsets.size - 1,
-        children=(as_column(new_offsets), as_column(new_elements)),
-    )
+    if cudf:
+        return build_column(
+            None,
+            dtype=cudf.core.dtypes.ListDtype(new_elements.dtype),
+            size=new_offsets.size - 1,
+            children=(as_column(new_offsets), as_column(new_elements)),
+        )
+    return []
 
 
 def build_pandas_list_column(elements, row_lengths):
     """Method creates a List series from the corresponding elements and
     row_lengths
 
     Parameters
@@ -711,7 +775,19 @@
 
 
 def get_random_state():
     """get_random_state from either cupy or numpy."""
     if cp:
         return cp.random.get_random_state()
     return np.random.mtrand.RandomState()
+
+
+def df_from_dict(col_dict):
+    from merlin.table import TensorTable, df_from_tensor_table
+
+    return df_from_tensor_table(TensorTable(col_dict))
+
+
+def dict_from_df(df: DataFrameLike):
+    from merlin.table import tensor_table_from_df
+
+    return tensor_table_from_df(df).to_dict()
```

### Comparing `merlin-core-23.2.1/merlin/core/protocols.py` & `merlin-core-23.4.0/merlin/core/protocols.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/core/utils.py` & `merlin-core-23.4.0/merlin/core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,105 +26,19 @@
 
 import dask
 import distributed
 from dask.dataframe.optimize import optimize as dd_optimize
 from dask.distributed import Client, get_client
 from tqdm import tqdm
 
-from merlin.core.compat import HAS_GPU, cuda
+from merlin.core.compat import HAS_GPU, cuda, device_mem_size  # noqa pylint: disable=unused-import
 
 _merlin_dask_client = ContextVar("_merlin_dask_client", default="auto")
 
 
-try:
-    import psutil
-except ImportError:
-    psutil = None
-
-
-def pynvml_mem_size(kind="total", index=0):
-    """Get Memory Info for device.
-
-    Parameters
-    ----------
-    kind : str, optional
-        Either "free" or "total", by default "total"
-    index : int, optional
-        Device Index, by default 0
-
-    Returns
-    -------
-    int
-        Either free or total memory on device depending on the kind parameter.
-
-    Raises
-    ------
-    ValueError
-        When kind is not one of {"free", "total"}
-    """
-    import pynvml
-
-    pynvml.nvmlInit()
-    size = None
-    if kind == "free":
-        size = int(pynvml.nvmlDeviceGetMemoryInfo(pynvml.nvmlDeviceGetHandleByIndex(index)).free)
-    elif kind == "total":
-        size = int(pynvml.nvmlDeviceGetMemoryInfo(pynvml.nvmlDeviceGetHandleByIndex(index)).total)
-    else:
-        raise ValueError(f"{kind} not a supported option for device_mem_size.")
-    pynvml.nvmlShutdown()
-    return size
-
-
-def device_mem_size(kind="total", cpu=False):
-    """Get Memory Info for either CPU or GPU.
-
-    Parameters
-    ----------
-    kind : str, optional
-        Either "total" or "free", by default "total"
-    cpu : bool, optional
-        Specifies whether to check memory for CPU or GPU, by default False
-
-    Returns
-    -------
-    int
-        Free or total memory on device
-
-    Raises
-    ------
-    ValueError
-        When kind is provided with an unsupported value.
-    """
-    # Use psutil (if available) for cpu mode
-    if cpu and psutil:
-        if kind == "total":
-            return psutil.virtual_memory().total
-        elif kind == "free":
-            return psutil.virtual_memory().free
-    elif cpu:
-        warnings.warn("Please install psutil for full cpu=True support.")
-        # Assume 1GB of memory
-        return int(1e9)
-
-    if kind not in ["free", "total"]:
-        raise ValueError(f"{kind} not a supported option for device_mem_size.")
-    try:
-        if kind == "free":
-            return int(cuda.current_context().get_memory_info()[0])
-        else:
-            return int(cuda.current_context().get_memory_info()[1])
-    except NotImplementedError:
-        if kind == "free":
-            # Not using NVML "free" memory, because it will not include RMM-managed memory
-            warnings.warn("get_memory_info is not supported. Using total device memory from NVML.")
-        size = pynvml_mem_size(kind="total", index=0)
-        return size
-
-
 def get_rmm_size(size):
     return (size // 256) * 256
 
 
 def download_file(url, local_filename, unzip_files=True, redownload=True):
     """utility function to download a dataset file (movielens/criteo/rossmann etc)
     locally, displaying a progress bar during download"""
```

### Comparing `merlin-core-23.2.1/merlin/dag/__init__.py` & `merlin-core-23.4.0/merlin/dag/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/base_operator.py` & `merlin-core-23.4.0/merlin/dag/base_operator.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/dictarray.py` & `merlin-core-23.4.0/merlin/dag/dictarray.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/executors.py` & `merlin-core-23.4.0/merlin/dag/executors.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def transform(
         self,
         transformable,
         graph,
         output_dtypes=None,
         additional_columns=None,
         capture_dtypes=False,
-        validate_dtypes=True,
+        strict=False,
     ):
         """
         Transforms a single dataframe (possibly a partition of a Dask Dataframe)
         by applying the operators from a collection of Nodes
         """
         nodes = []
         if isinstance(graph, Graph):
@@ -62,194 +62,189 @@
             raise TypeError(
                 f"LocalExecutor detected unsupported type of input for graph: {type(graph)}."
                 " `graph` argument must be either a `Graph` object (preferred)"
                 " or a list of `Node` objects (deprecated, but supported for backward "
                 " compatibility.)"
             )
 
+        # There's usually only one node, but it's possibly to pass multiple nodes for `fit`
+        # If we have multiple, we concatenate their outputs into a single transformable
         output_data = None
-
         for node in nodes:
-            input_data = self._build_input_data(
-                node, transformable, capture_dtypes=capture_dtypes, validate_dtypes=validate_dtypes
-            )
-
-            if node.op:
-                transformed_data = self._transform_data(
-                    node, input_data, capture_dtypes=capture_dtypes, validate_dtypes=validate_dtypes
-                )
-            else:
-                transformed_data = input_data
-
+            transformed_data = self._execute_node(node, transformable, capture_dtypes, strict)
             output_data = self._combine_node_outputs(node, transformed_data, output_data)
 
+        # If there are any additional columns that weren't produced by one of the supplied nodes
+        # we grab them directly from the supplied input data. Normally this would happen on a
+        # per-node basis, but offers a safety net for the multi-node case
         if additional_columns:
             output_data = concat_columns(
                 [output_data, transformable[_get_unique(additional_columns)]]
             )
 
         return output_data
 
-    def _build_input_data(self, node, transformable, capture_dtypes=False, validate_dtypes=True):
-        """
-        Recurse through the graph executing parent and dependency operators
-        to form the input dataframe for each output node
-        Parameters
-        ----------
-        node : Node
-            Output node of the graph to execute
-        transformable : Transformable
-            Dataframe to run the graph ending with node on
-        capture_dtypes : bool, optional
-            Overrides the schema dtypes with the actual dtypes when True, by default False
-        Returns
-        -------
-        Transformable
-            The input DataFrame or DictArray formed from
-            the outputs of upstream parent/dependency nodes
-        """
-        node_input_cols = _get_unique(node.input_schema.column_names)
-        addl_input_cols = set(node.dependency_columns.names)
-
-        if node.parents_with_dependencies:
-            # If there are parents, collect their outputs
-            # to build the current node's input
-            input_data = None
-            seen_columns = None
-
-            for parent in node.parents_with_dependencies:
-                parent_output_cols = _get_unique(parent.output_schema.column_names)
-                parent_data = self.transform(
-                    transformable,
-                    [parent],
-                    capture_dtypes=capture_dtypes,
-                    validate_dtypes=validate_dtypes,
-                )
-                if input_data is None or not len(input_data):
-                    input_data = parent_data[parent_output_cols]
-                    seen_columns = set(parent_output_cols)
-                else:
-                    new_columns = set(parent_output_cols) - seen_columns
-                    if new_columns:
-                        input_data = concat_columns([input_data, parent_data[list(new_columns)]])
-                        seen_columns.update(new_columns)
-
-            # Check for additional input columns that aren't generated by parents
-            # and fetch them from the root DataFrame or DictArray
-            unseen_columns = set(node.input_schema.column_names) - seen_columns
-            addl_input_cols = addl_input_cols.union(unseen_columns)
+    def _execute_node(self, node, transformable, capture_dtypes=False, strict=False):
+        upstream_outputs = self._run_upstream_transforms(
+            node, transformable, capture_dtypes, strict
+        )
+        upstream_columns = self._append_addl_root_columns(node, transformable, upstream_outputs)
+        transform_input = self._merge_upstream_columns(upstream_columns)
+        transform_output = self._run_node_transform(node, transform_input, capture_dtypes, strict)
+        return transform_output
+
+    def _run_upstream_transforms(self, node, transformable, capture_dtypes=False, strict=False):
+        upstream_outputs = []
+
+        for upstream_node in node.parents_with_dependencies:
+            node_output = self._execute_node(
+                upstream_node,
+                transformable,
+                capture_dtypes=capture_dtypes,
+                strict=strict,
+            )
+            if node_output is not None and len(node_output) > 0:
+                upstream_outputs.append(node_output)
 
-            # TODO: Find a better way to remove dupes
-            addl_input_cols = addl_input_cols - set(input_data.columns)
+        return upstream_outputs
 
-            if addl_input_cols:
-                input_data = concat_columns([input_data, transformable[list(addl_input_cols)]])
-        else:
-            # If there are no parents, this is an input node,
-            # so pull columns directly from root data
-            addl_input_cols = list(addl_input_cols) if addl_input_cols else []
-            input_data = transformable[node_input_cols + addl_input_cols]
+    def _append_addl_root_columns(self, node, transformable, upstream_outputs):
+        node_input_cols = set(node.input_schema.column_names)
+        addl_input_cols = set(node.dependency_columns.names)
 
-        return input_data
+        already_present = set()
+        for upstream_tensors in upstream_outputs:
+            for col in node_input_cols:
+                if col in upstream_tensors:
+                    already_present.add(col)
+
+        root_columns = node_input_cols.union(addl_input_cols) - already_present
+
+        if root_columns:
+            upstream_outputs.append(transformable[list(root_columns)])
+
+        return upstream_outputs
+
+    def _merge_upstream_columns(self, upstream_outputs, merge_fn=concat_columns):
+        combined_outputs = None
+        seen_columns = set()
+        for upstream_output in upstream_outputs:
+            if combined_outputs is None or not len(combined_outputs):
+                combined_outputs = upstream_output
+                seen_columns = set(upstream_output.columns)
+            else:
+                new_columns = set(upstream_output.columns) - seen_columns
+                if new_columns:
+                    combined_outputs = merge_fn(
+                        [combined_outputs, upstream_output[list(new_columns)]]
+                    )
+                    seen_columns.update(new_columns)
+        return combined_outputs
 
-    def _transform_data(self, node, input_data, capture_dtypes=False, validate_dtypes=True):
+    def _run_node_transform(self, node, input_data, capture_dtypes=False, strict=False):
         """
         Run the transform represented by the final node in the graph
         and check output dtypes against the output schema
         Parameters
         ----------
         node : Node
             Output node of the graph to execute
         input_data : Transformable
             Dataframe to run the graph ending with node on
         capture_dtypes : bool, optional
             Overrides the schema dtypes with the actual dtypes when True, by default False
-        validate_dtypes : bool, optional
-            Checks the dtype of returned data against the schema, by default True
+        strict : bool, optional
+            Raises error if the dtype of returned data doesn't match the schema, by default False
         Returns
         -------
         Transformable
             The output DataFrame or DictArray formed by executing the final node's transform
         Raises
         ------
         TypeError
             If the transformed output columns don't have the same dtypes
-            as the output schema columns when validate_dtypes is True
+            as the output schema columns when `strict` is True
         RuntimeError
             If no DataFrame or DictArray is returned from the operator
         """
+        if not node.op:
+            return input_data
+
         try:
             # use input_columns to ensure correct grouping (subgroups)
             selection = node.input_columns.resolve(node.input_schema)
-            output_data = node.op.transform(selection, input_data)
+            transformed_data = node.op.transform(selection, input_data)
 
-            # Update or validate output_data dtypes
-            if capture_dtypes or validate_dtypes:
-                for col_name, output_col_schema in node.output_schema.column_schemas.items():
-                    col_series = output_data[col_name]
-                    output_data_dtype = col_series.dtype
-                    col_shape = output_col_schema.shape
-                    is_list = is_list_dtype(col_series)
-
-                    if is_list:
-                        output_data_dtype = list_val_dtype(col_series)
-
-                        if not col_shape.is_list or col_shape.is_unknown:
-                            col_shape = DefaultShapes.LIST
-
-                    # TODO: Add a utility that condenses the known methods of fetching dtypes
-                    # from series/arrays into a single function, so that Tensorflow specific
-                    # code doesn't leak into the executors
-                    if not hasattr(output_data_dtype, "as_numpy_dtype") and hasattr(
-                        col_series, "numpy"
-                    ):
-                        output_data_dtype = col_series[0].cpu().numpy().dtype
+            if transformed_data is None:
+                raise RuntimeError(f"Operator {node.op} didn't return a value during transform")
+            elif capture_dtypes:
+                self._capture_dtypes(node, transformed_data)
+            elif strict and len(transformed_data):
+                self._validate_dtypes(node, transformed_data)
 
-                    output_data_schema = output_col_schema.with_dtype(output_data_dtype).with_shape(
-                        col_shape
-                    )
+            return transformed_data
 
-                    if capture_dtypes:
-                        node.output_schema.column_schemas[col_name] = output_data_schema
-                    elif validate_dtypes and len(output_data):
-                        # Validate that the dtypes match but only if they both exist
-                        # (since schemas may not have all dtypes specified, especially
-                        # in the tests)
-                        output_schema_dtype = output_col_schema.dtype.without_shape
-                        output_data_dtype = md.dtype(output_data_dtype).without_shape
-                        if (
-                            output_schema_dtype
-                            and output_data_dtype
-                            and output_schema_dtype != md.string
-                            and output_schema_dtype != output_data_dtype
-                        ):
-                            raise TypeError(
-                                f"Dtype discrepancy detected for column {col_name}: "
-                                f"operator {node.op.label} reported dtype "
-                                f"`{output_schema_dtype}` but returned dtype "
-                                f"`{output_data_dtype}`."
-                            )
-        except Exception:
+        except Exception as exc:
             LOG.exception("Failed to transform operator %s", node.op)
-            raise
-        if output_data is None:
-            raise RuntimeError(f"Operator {node.op} didn't return a value during transform")
+            raise exc
 
-        return output_data
+    def _capture_dtypes(self, node, output_data):
+        for col_name, output_col_schema in node.output_schema.column_schemas.items():
+            output_data_schema = self._build_schema_from_data(
+                output_data, col_name, output_col_schema
+            )
+            node.output_schema.column_schemas[col_name] = output_data_schema
+
+    # TODO: Turn this into a function
+    def _build_schema_from_data(self, output_data, col_name, output_col_schema):
+        column = output_data[col_name]
+        column_dtype = column.dtype
+        col_shape = output_col_schema.shape
+        is_list = is_list_dtype(column)
+
+        if is_list:
+            column_dtype = list_val_dtype(column)
+
+            if not col_shape.is_list or col_shape.is_unknown:
+                col_shape = DefaultShapes.LIST
+
+        return output_col_schema.with_dtype(column_dtype).with_shape(col_shape)
+
+    # TODO: Turn this into a function
+    def _validate_dtypes(self, node, output_data):
+        for col_name, output_col_schema in node.output_schema.column_schemas.items():
+            # Validate that the dtypes match but only if they both exist
+            # (since schemas may not have all dtypes specified, especially
+            # in the tests)
+            output_schema_dtype = output_col_schema.dtype.without_shape
+            output_data_dtype = md.dtype(output_data.dtype).without_shape
+            if (
+                output_schema_dtype
+                and output_data_dtype
+                and output_schema_dtype != md.string
+                and output_schema_dtype != output_data_dtype
+            ):
+                raise TypeError(
+                    f"Dtype discrepancy detected for column {col_name}: "
+                    f"operator {node.op.label} reported dtype "
+                    f"`{output_schema_dtype}` but returned dtype "
+                    f"`{output_data_dtype}`."
+                )
 
-    def _combine_node_outputs(self, node, transformed_data, output):
+    # TODO: Turn this into a function
+    def _combine_node_outputs(self, node, transformed, output):
         node_output_cols = _get_unique(node.output_schema.column_names)
 
         # dask needs output to be in the same order defined as meta, reorder partitions here
         # this also selects columns (handling the case of removing columns from the output using
         # "-" overload)
         if output is None:
-            output = transformed_data[node_output_cols]
+            output = transformed[node_output_cols]
         else:
-            output = concat_columns([output, transformed_data[node_output_cols]])
+            output = concat_columns([output, transformed[node_output_cols]])
 
         return output
 
 
 class DaskExecutor:
     """
     An executor for running Merlin operator DAGs as distributed Dask jobs
@@ -263,15 +258,21 @@
             set_client_deprecated(client, "DaskExecutor")
 
     def __getstate__(self):
         # dask client objects aren't picklable - exclude from saved representation
         return {k: v for k, v in self.__dict__.items() if k != "client"}
 
     def transform(
-        self, ddf, graph, output_dtypes=None, additional_columns=None, capture_dtypes=False
+        self,
+        ddf,
+        graph,
+        output_dtypes=None,
+        additional_columns=None,
+        capture_dtypes=False,
+        strict=False,
     ):
         """
         Transforms all partitions of a Dask Dataframe by applying the operators
         from a collection of Nodes
         """
         nodes = []
         if isinstance(graph, Graph):
@@ -324,20 +325,21 @@
 
         return ensure_optimize_dataframe_graph(
             ddf=ddf.map_partitions(
                 self._executor.transform,
                 nodes,
                 additional_columns=additional_columns,
                 capture_dtypes=capture_dtypes,
+                strict=strict,
                 meta=output_dtypes,
                 enforce_metadata=False,
             )
         )
 
-    def fit(self, ddf, nodes):
+    def fit(self, ddf, nodes, strict=False):
         """Calculates statistics for a set of nodes on the input dataframe
 
         Parameters
         -----------
         ddf: dask.Dataframe
             The input dataframe to calculate statistics for. If there is a
             train/test split this should be the training dataset only.
@@ -356,14 +358,15 @@
             # apply transforms necessary for the inputs to the current column group, ignoring
             # the transforms from the statop itself
             transformed_ddf = self.transform(
                 ddf,
                 node.parents_with_dependencies,
                 additional_columns=addl_input_cols,
                 capture_dtypes=True,
+                strict=strict,
             )
 
             try:
                 stats.append(node.op.fit(node.input_columns, transformed_ddf))
             except Exception:
                 LOG.exception("Failed to fit operator %s", node.op)
                 raise
```

### Comparing `merlin-core-23.2.1/merlin/dag/graph.py` & `merlin-core-23.4.0/merlin/dag/graph.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/node.py` & `merlin-core-23.4.0/merlin/dag/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 
             if not source_col_schema:
                 raise ValueError(
                     f"Missing column '{col_name}' at the input to '{self.op.__class__.__name__}'."
                 )
 
             if strict_dtypes or not self.op.dynamic_dtypes:
-                if source_col_schema.dtype != col_schema.dtype:
+                if source_col_schema.dtype.without_shape != col_schema.dtype.without_shape:
                     raise ValueError(
                         f"Mismatched dtypes for column '{col_name}' provided to "
                         f"'{self.op.__class__.__name__}': "
                         f"ancestor nodes provided dtype '{source_col_schema.dtype}', "
                         f"expected dtype '{col_schema.dtype}'."
                     )
 
@@ -302,14 +302,17 @@
         -----------
         other: Node or str or list of str
 
         Returns
         -------
         Node
         """
+        if not other:
+            return self
+
         if isinstance(self.op, ConcatColumns):
             child = self
         else:
             # Create a child node
             child = type(self)()
             child.op = ConcatColumns(label="+")
             child.add_parent(self)
```

### Comparing `merlin-core-23.2.1/merlin/dag/ops/__init__.py` & `merlin-core-23.4.0/merlin/dag/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/ops/concat_columns.py` & `merlin-core-23.4.0/merlin/dag/ops/concat_columns.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/ops/selection.py` & `merlin-core-23.4.0/merlin/dag/ops/selection.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/ops/subset_columns.py` & `merlin-core-23.4.0/merlin/dag/ops/subset_columns.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/ops/subtraction.py` & `merlin-core-23.4.0/merlin/dag/ops/subtraction.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dag/selector.py` & `merlin-core-23.4.0/merlin/dag/selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     names: list of (str or tuple of str)
         The columns to select from the input Dataset. The elements of this list are strings
         indicating the column names in most cases, but can also be tuples of strings
         for feature crosses.
     subgroups, optional: list of ColumnSelector objects
         This provides an alternate syntax for grouping column names together (instead
         of nesting tuples inside the list of names)
+    tags : list of Tags
+        The columns to select from the input dataset based on Tags. Any column with
+        at-least-one of the tags provided will be considered.
     """
 
     def __init__(
         self,
         names: Union[str, List[str]] = None,
         subgroups: List["ColumnSelector"] = None,
         tags: List[Union[Tags, str]] = None,
```

### Comparing `merlin-core-23.2.1/merlin/dag/utils.py` & `merlin-core-23.4.0/merlin/dag/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/__init__.py` & `merlin-core-23.4.0/merlin/dtypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 
 # flake8: noqa
 from merlin.dtypes import mappings
 from merlin.dtypes.aliases import *
 from merlin.dtypes.base import DType
 from merlin.dtypes.registry import _dtype_registry
+from merlin.dtypes.shape import Dimension, Shape
 
 # Convenience alias for registering dtypes
 register = _dtype_registry.register
 
 
 def dtype(external_dtype):
     # If the supplied dtype is None, then there's not a default dtype we can
```

### Comparing `merlin-core-23.2.1/merlin/dtypes/aliases.py` & `merlin-core-23.4.0/merlin/dtypes/aliases.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/base.py` & `merlin-core-23.4.0/merlin/dtypes/base.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mapping.py` & `merlin-core-23.4.0/merlin/dtypes/mapping.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/__init__.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/cudf.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/cudf.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import numpy as np
 
+from merlin.core.compat import cudf
 from merlin.core.dispatch import is_string_dtype
 from merlin.dtypes.mapping import DTypeMapping, NumpyPreprocessor
 from merlin.dtypes.registry import _dtype_registry
 
 
 def cudf_translator(raw_dtype) -> np.dtype:
     """
@@ -37,21 +38,20 @@
     category_type = raw_dtype._categories.dtype
     if is_string_dtype(category_type):
         return np.dtype("str")
     else:
         return category_type
 
 
-try:
-    # We only want to register this mapping if cudf is available, even though
-    # the mapping itself doesn't use cudf (yet?)
-
-    import cudf  # pylint:disable=unused-import # noqa: F401
-
-    cudf_dtypes = DTypeMapping(
-        translator=NumpyPreprocessor("cudf", cudf_translator, attrs=["_categories"]),
-    )
-    _dtype_registry.register("cudf", cudf_dtypes)
-except ImportError as exc:
-    from warnings import warn
+if cudf:
+    try:
+        # We only want to register this mapping if cudf is available, even though
+        # the mapping itself doesn't use cudf (yet?)
+
+        cudf_dtypes = DTypeMapping(
+            translator=NumpyPreprocessor("cudf", cudf_translator, attrs=["_categories"]),
+        )
+        _dtype_registry.register("cudf", cudf_dtypes)
+    except ImportError as exc:
+        from warnings import warn
 
-    warn(f"cuDF dtype mappings did not load successfully due to an error: {exc.msg}")
+        warn(f"cuDF dtype mappings did not load successfully due to an error: {exc.msg}")
```

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/numpy.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/numpy.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/pandas.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/pandas.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/python.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/python.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/tf.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/tf.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/torch.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/mappings/triton.py` & `merlin-core-23.4.0/merlin/dtypes/mappings/triton.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/registry.py` & `merlin-core-23.4.0/merlin/dtypes/registry.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/dtypes/shape.py` & `merlin-core-23.4.0/merlin/dtypes/shape.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,42 @@
             raise ValueError("The minimum size of a dimension cannot be None. ")
 
         if self.min < 0:
             raise ValueError(
                 "The minimum size of a dimension must be non-negative. " f"Provided min: {self.min}"
             )
 
+        if self.min and not isinstance(self.min, int):
+            raise ValueError(
+                "The minimum size of a dimension must be an integer. "
+                f"Received a value of type '{type(self.min)}'"
+            )
+        if self.max and not isinstance(self.max, int):
+            raise ValueError(
+                "The maximum size of a dimension must be an integer. "
+                f"Received a value of type '{type(self.max)}'"
+            )
+
         if self.max and self.max < 0:
             raise ValueError(
                 "The maximum size of a dimension must be at least one. " f"Provided max: {self.max}"
             )
 
         if self.max and self.max < self.min:
             raise ValueError(
                 "The maximum size of a dimension must be at least as large as the minimum size. "
                 f"Provided min: {self.min} max: {self.max}"
             )
 
+    def __int__(self):
+        if self.min == self.max:
+            return self.max
+        else:
+            raise ValueError(f"Can't convert {self} without a fixed size to an integer.")
+
     @property
     def is_bounded(self):
         return self.max is not None
 
     @property
     def is_fixed(self):
         return self.is_bounded and self.min == self.max
@@ -125,14 +142,17 @@
             return True
 
         return self.dims == other.dims
 
     def __iter__(self):
         return self.dims
 
+    def __getitem__(self, index):
+        return self.dims[index]
+
     def with_dim(self, index, value):
         new_dims = list(self.dims)
         new_dims[index] = value
         return replace(self, dims=tuple(new_dims))
 
     def with_dim_min(self, index, value):
         return self.with_dim(index, self.dims[index].with_min(value))
@@ -166,12 +186,15 @@
 
     @property
     def is_ragged(self):
         return self.is_list and any(dim.min != dim.max for dim in self.dims[1:])
 
     @property
     def as_tuple(self):
-        return tuple(((dim.min, dim.max) for dim in self.dims)) if self.dims else None
+        if not self.dims:
+            return None
+
+        return tuple(((dim.min, dim.max) if dim.min != dim.max else dim.max for dim in self.dims))
 
     @property
     def is_unknown(self):
         return self.dims is None
```

### Comparing `merlin-core-23.2.1/merlin/io/__init__.py` & `merlin-core-23.4.0/merlin/io/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # flake8: noqa
 from merlin.io import dataframe_iter, dataset, shuffle
 from merlin.io.dataframe_iter import DataFrameIter
-from merlin.io.dataset import Dataset
+from merlin.io.dataset import MERLIN_METADATA_DIR_NAME, Dataset
 from merlin.io.shuffle import Shuffle, shuffle_df
```

### Comparing `merlin-core-23.2.1/merlin/io/avro.py` & `merlin-core-23.4.0/merlin/io/avro.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
 
-import cudf
 import uavro as ua
 from dask.base import tokenize
 from dask.dataframe.core import new_dd_object
 
+from merlin.core.compat import cudf
 from merlin.io.dataset_engine import DatasetEngine
 
 
 class AvroDatasetEngine(DatasetEngine):
     """AvroDatasetEngine
 
     Uses `uavro` to decompose dataset into groups of avro blocks.
```

### Comparing `merlin-core-23.2.1/merlin/io/csv.py` & `merlin-core-23.4.0/merlin/io/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import functools
 
 import dask.dataframe as dd
-
-try:
-    import dask_cudf
-except ImportError:
-    dask_cudf = None
-import numpy as np
 from dask.bytes import read_bytes
 from dask.utils import parse_bytes
 from fsspec.core import get_fs_token_paths
 from fsspec.utils import infer_compression
 
+from merlin.core.compat import dask_cudf
+from merlin.core.compat import numpy as np
 from merlin.io.dataset_engine import DatasetEngine
 
 
 class CSVDatasetEngine(DatasetEngine):
     """CSVDatasetEngine
 
     Thin wrapper around dask_cudf.read_csv.
```

### Comparing `merlin-core-23.2.1/merlin/io/dask.py` & `merlin-core-23.4.0/merlin/io/dask.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import collections
+import warnings
 
 import dask
 import pandas as pd
 from dask.base import tokenize
+from dask.blockwise import Blockwise
 from dask.dataframe.core import _concat, new_dd_object
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 
 from merlin.core.dispatch import annotate
 from merlin.core.utils import ensure_optimize_dataframe_graph, global_dask_client
 from merlin.io.shuffle import Shuffle
@@ -43,14 +45,17 @@
     """
 
     def __init__(self, full_graph, name, parts):
         self.name = name
         self.parts = parts
         self.subgraph = full_graph.cull({(self.name, part) for part in self.parts})
 
+    def __iter__(self):
+        return iter(self.parts)
+
     def __getitem__(self, part):
         key = (self.name, part)
         dsk = self.subgraph.cull({key})
         return dask.get(dsk, key)
 
 
 @annotate("write_output_partition", color="green", domain="merlin_python")
@@ -63,14 +68,15 @@
     cat_names,
     cont_names,
     label_names,
     output_format,
     num_threads,
     cpu,
     suffix,
+    row_group_size,
 ):
     df_size = len(df)
     out_files_per_proc = out_files_per_proc or 1
 
     # Get cached writer (or create/cache a new one)
     with get_worker_cache("writer") as writer_cache:
         writer = writer_cache.get(processed_path, None)
@@ -81,14 +87,16 @@
                 out_files_per_proc,
                 shuffle,
                 use_guid=True,
                 bytes_io=(shuffle == Shuffle.PER_WORKER),
                 num_threads=num_threads,
                 cpu=cpu,
                 suffix=suffix,
+                fs=fs,
+                row_group_size=row_group_size,
             )
             writer.set_col_names(labels=label_names, cats=cat_names, conts=cont_names)
             writer_cache[processed_path] = writer
 
         # Add data
         writer.add_data(df)
 
@@ -132,14 +140,15 @@
     fs,
     cat_names,
     cont_names,
     label_names,
     output_format,
     num_threads,
     cpu,
+    row_group_size,
 ):
     # Logic copied from cudf/cudf/io/parquet.py
     data_cols = df.columns.drop(partition_cols)
     if len(data_cols) == 0:
         raise ValueError("No data left to save outside partition columns")
 
     # Partition the input data
@@ -148,14 +157,15 @@
         output_format,
         output_path,
         1,
         shuffle,
         num_threads=num_threads,
         cpu=cpu,
         fns=fns,
+        row_group_size=row_group_size,
     )
     writer.set_col_names(labels=label_names, cats=cat_names, conts=cont_names)
 
     # Add the partitioned data
     writer.add_data(dfs)
 
     # Return metadata and row-count in dict
@@ -172,32 +182,40 @@
     cat_names,
     cont_names,
     label_names,
     output_format,
     num_threads,
     cpu,
     suffix,
+    row_group_size,
 ):
     fns = fns if isinstance(fns, (tuple, list)) else (fns,)
     writer = writer_factory(
         output_format,
         output_path,
         len(fns),
         shuffle,
         bytes_io=(shuffle == Shuffle.PER_WORKER),
         num_threads=num_threads,
         cpu=cpu,
         fns=[fn + suffix for fn in fns],
+        fs=fs,
+        row_group_size=row_group_size,
     )
     writer.set_col_names(labels=label_names, cats=cat_names, conts=cont_names)
 
     # Add data
     num_rows = 0
-    for part in subgraph.parts:
-        table = subgraph[part]
+    for part in subgraph:
+        if isinstance(subgraph, list):
+            # Partition is already a DataFrame object
+            table = part
+        else:
+            # Extract partition from the DaskSubgraph
+            table = subgraph[part]
         writer.add_data(table)
         num_rows += len(table)
         del table
 
     # Return metadata and row-count in dict
     return writer.close()
 
@@ -246,20 +264,29 @@
     cat_names,
     cont_names,
     label_names,
     output_format,
     num_threads,
     cpu,
     suffix="",
+    row_group_size=None,
     partition_on=None,
     schema=None,
 ):
     # Construct graph for Dask-based dataset write
     token = tokenize(
-        ddf, shuffle, out_files_per_proc, cat_names, cont_names, label_names, suffix, partition_on
+        ddf,
+        shuffle,
+        out_files_per_proc,
+        cat_names,
+        cont_names,
+        label_names,
+        suffix,
+        partition_on,
+        row_group_size,
     )
     name = "write-processed-" + token
     write_name = name + "-partition" + token
 
     # Check that the data is in the correct place
     assert isinstance(ddf._meta, pd.DataFrame) is cpu
 
@@ -280,30 +307,61 @@
                 fs,
                 cat_names,
                 cont_names,
                 label_names,
                 output_format,
                 num_threads,
                 cpu,
+                row_group_size,
             )
         dsk[name] = (
             _write_metadata_files,
             task_list,
             output_path,
             output_format,
             cpu,
             schema,
         )
     elif file_partition_map is not None:
         # Use specified mapping of data to output files
         cached_writers = False
         full_graph = ddf.dask
+
+        # Check if we need to use conventional task scheduling,
+        # or if the partition-file mapping is dangerous
+        use_tasks = False
+        all_blockwise = all(isinstance(layer, Blockwise) for layer in full_graph.layers.values())
+        if not all_blockwise:
+            if all(len(v) == 1 for v in file_partition_map.values()):
+                # Use conventional task scheduling if we have a 1:1
+                # mapping between partitions and output files
+                use_tasks = True
+            else:
+                # We don't have all Blockwise layers, so this
+                # write operation may cause pain
+                warnings.warn(
+                    "Using the 'subgraph' approach to execute a graph "
+                    "with non-trivial dependencies. This may cause memory "
+                    "errors if there is not a 1:1 mapping between Dask "
+                    "partitions and output files. Please consider using "
+                    "defaults for `output_files` and `out_files_per_proc`."
+                )
+
         for fns, parts in file_partition_map.items():
             # Isolate subgraph for this output file
-            subgraph = DaskSubgraph(full_graph, ddf._name, parts)
+            if use_tasks and len(parts) == 1:
+                # If there is only one input partition for this
+                # file, then we don't need to create a subgraph.
+                # We can just use conventional task scheduling
+                subgraph = [(ddf._name, parts[0])]
+            else:
+                # Otherwise, we need a subgraph to avoid
+                # materializing multiple input partitions on the
+                # same worker at once (likely to cause OOM errors)
+                subgraph = DaskSubgraph(full_graph, ddf._name, parts)
             task_list.append((write_name, str(fns)))
             dsk[task_list[-1]] = (
                 _write_subgraph,
                 subgraph,
                 fns,
                 output_path,
                 shuffle,
@@ -311,14 +369,15 @@
                 cat_names,
                 cont_names,
                 label_names,
                 output_format,
                 num_threads,
                 cpu,
                 suffix,
+                row_group_size,
             )
         dsk[name] = (
             _write_metadata_files,
             task_list,
             output_path,
             output_format,
             cpu,
@@ -338,14 +397,15 @@
                 cat_names,
                 cont_names,
                 label_names,
                 output_format,
                 num_threads,
                 cpu,
                 suffix,
+                row_group_size,
             )
             task_list.append(key)
         dsk[name] = (lambda x: x, task_list)
 
     graph = ensure_optimize_dataframe_graph(
         dsk=HighLevelGraph.from_collections(name, dsk, dependencies=[ddf]),
         keys=[name],
```

### Comparing `merlin-core-23.2.1/merlin/io/dataframe_engine.py` & `merlin-core-23.4.0/merlin/io/dataframe_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-try:
-    import cudf
-    import dask_cudf
-except ImportError:
-    cudf = None
 from dask.dataframe.core import new_dd_object
 from dask.highlevelgraph import HighLevelGraph
 
+from merlin.core.compat import cudf, dask_cudf
 from merlin.io.dataset_engine import DatasetEngine
 
 
 class DataFrameDatasetEngine(DatasetEngine):
     """DataFrameDatasetEngine allows NVT to interact with a dask_cudf.DataFrame object
     in the same way as a dataset on disk.
     """
```

### Comparing `merlin-core-23.2.1/merlin/io/dataframe_iter.py` & `merlin-core-23.4.0/merlin/io/dataframe_iter.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/io/dataset.py` & `merlin-core-23.4.0/merlin/io/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,37 +26,34 @@
 from dask.base import tokenize
 from dask.dataframe.core import new_dd_object
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import natural_sort_key, parse_bytes
 from fsspec.core import get_fs_token_paths
 from fsspec.utils import stringify_path
 
+from merlin.core.compat import HAS_GPU, cudf, device_mem_size
 from merlin.core.dispatch import (
     convert_data,
     hex_to_int,
     is_dataframe_object,
     is_list_dtype,
     list_val_dtype,
 )
-from merlin.core.utils import device_mem_size, global_dask_client, set_client_deprecated
+from merlin.core.utils import global_dask_client, set_client_deprecated
 from merlin.dtypes.shape import DefaultShapes
 from merlin.io.csv import CSVDatasetEngine
 from merlin.io.dask import _ddf_to_dataset, _simple_shuffle
 from merlin.io.dataframe_engine import DataFrameDatasetEngine
 from merlin.io.dataframe_iter import DataFrameIter
 from merlin.io.parquet import ParquetDatasetEngine
 from merlin.io.shuffle import _check_shuffle_arg
 from merlin.schema import ColumnSchema, Schema
 from merlin.schema.io.tensorflow_metadata import TensorflowMetadata
 
-try:
-    import cudf
-except ImportError:
-    cudf = None
-
+MERLIN_METADATA_DIR_NAME = ".merlin"
 LOG = logging.getLogger("merlin")
 
 
 class Dataset:
     """Universal external-data wrapper for NVTabular
 
     The NVTabular `Workflow` and `DataLoader`-related APIs require all
@@ -237,18 +234,31 @@
 
         self.dtypes = dtypes
         self.schema = schema
 
         # Cache for "real" (sampled) metadata
         self._real_meta = {}
 
-        # Check if we are keeping data in cpu memory
+        # Check if we are keeping data in host or gpu device memory
         self.cpu = cpu
-        if not self.cpu:
-            self.cpu = cudf is None
+        if self.cpu is False:
+            if not HAS_GPU:
+                raise RuntimeError(
+                    "Cannot initialize Dataset on GPU. "
+                    "No devices detected (with pynvml). "
+                    "Check that pynvml can be initialized. "
+                )
+            if cudf is None:
+                raise RuntimeError(
+                    "Cannot initialize Dataset on GPU. "
+                    "cudf package not found. "
+                    "Check that cudf is installed in this environment and can be imported.  "
+                )
+        if self.cpu is None:
+            self.cpu = cudf is None or not HAS_GPU
 
         # Keep track of base dataset (optional)
         self.base_dataset = base_dataset or self
 
         # For now, lets warn the user that "cpu mode" is experimental
         if self.cpu:
             warnings.warn(
@@ -335,18 +345,36 @@
                 path_or_source = [Path(path_or_source)]
             if isinstance(path_or_source, list) and isinstance(path_or_source[0], (str, Path)):
                 # list of paths to files
                 schema_path = Path(path_or_source[0])
                 if schema_path.is_file():
                     schema_path = schema_path.parent
 
-                if (schema_path / "schema.pbtxt").exists():
+                pbtxt_deprecated_warning = (
+                    "Found schema.pbtxt. Loading schema automatically from "
+                    "schema.pbtxt is deprecated and will be removed in the "
+                    "future. Re-run workflow to generate .merlin/schema.json."
+                )
+
+                if (schema_path / MERLIN_METADATA_DIR_NAME / "schema.json").exists():
+                    schema = TensorflowMetadata.from_json_file(
+                        schema_path / MERLIN_METADATA_DIR_NAME
+                    )
+                    self.schema = schema.to_merlin_schema()
+                elif (schema_path.parent / MERLIN_METADATA_DIR_NAME / "schema.json").exists():
+                    schema = TensorflowMetadata.from_json_file(
+                        schema_path.parent / MERLIN_METADATA_DIR_NAME
+                    )
+                    self.schema = schema.to_merlin_schema()
+                elif (schema_path / "schema.pbtxt").exists():
+                    warnings.warn(pbtxt_deprecated_warning, DeprecationWarning)
                     schema = TensorflowMetadata.from_proto_text_file(schema_path)
                     self.schema = schema.to_merlin_schema()
                 elif (schema_path.parent / "schema.pbtxt").exists():
+                    warnings.warn(pbtxt_deprecated_warning, DeprecationWarning)
                     schema = TensorflowMetadata.from_proto_text_file(schema_path.parent)
                     self.schema = schema.to_merlin_schema()
                 else:
                     self.infer_schema()
             else:
                 # df with no schema
                 self.infer_schema()
@@ -541,14 +569,15 @@
             self.to_ddf()
             .clear_divisions()
             .repartition(
                 npartitions=npartitions,
                 partition_size=partition_size,
             ),
             schema=self.schema,
+            cpu=self.cpu,
         )
 
     @classmethod
     def merge(cls, left, right, **kwargs):
         """Merge two Dataset objects
 
         Produces a new Dataset object. If the ``cpu`` Dataset attributes
@@ -658,14 +687,15 @@
     def to_parquet(
         self,
         output_path,
         shuffle=None,
         preserve_files=False,
         output_files=None,
         out_files_per_proc=None,
+        row_group_size=None,
         num_threads=0,
         dtypes=None,
         cats=None,
         conts=None,
         labels=None,
         suffix=".parquet",
         partition_on=None,
@@ -701,26 +731,34 @@
             Whether to preserve the original file-to-partition mapping of
             the base dataset. This option requires `method="subgraph"`, and is
             only available if the base dataset is known, and if it corresponds
             to csv or parquet format. If True, the `out_files_per_proc` option
             will be ignored. Default is False.
         output_files : dict, list or int
             The total number of desired output files. This option requires
-            `method="subgraph"`, and the default value will be the number of Dask
-            workers, multiplied by `out_files_per_proc`. For further output-file
+            `method="subgraph"`. When `out_files_per_proc=None`, the default
+            is the number of underlying Dask partitions. When `out_files_per_proc`
+            is set to an integer, the default is the product of that integer and
+            the total number of workers in the Dask cluster. For further output-file
             control, this argument may also be used to pass a dictionary mapping
             the output file names to partition indices, or a list of desired
             output-file names.
         out_files_per_proc : integer
             Number of output files that each process will use to shuffle an input
             partition. Default is 1. If `method="worker"`, the total number of output
             files will always be the total number of Dask workers, multiplied by this
             argument. If `method="subgraph"`, the total number of files is determined
             by `output_files` (and `out_files_per_proc` must be 1 if a dictionary is
             specified).
+        row_group_size : integer
+            Maximum number of rows to include in each Parquet row-group. By default,
+            the maximum row-group size will be chosen by the backend Parquet engine
+            (cudf or pyarrow). Note that cudf currently prohibits this value from
+            being less than `5000` rows. If smaller row-groups are necessary, try
+            calling `to_cpu()` before writing to disk.
         num_threads : integer
             Number of IO threads to use for writing the output dataset.
             For `0` (default), no dedicated IO threads will be used.
         dtypes : dict
             Dictionary containing desired datatypes for output columns.
             Keys are column names, values are datatypes.
         suffix : str or False
@@ -747,14 +785,15 @@
             specifying `method="worker"`.
         write_hugectr_keyset : bool, optional
             Whether to write a HugeCTR keyset output file ("_hugectr.keyset").
             Writing this file can be very slow, and should only be done if you
             are planning to ingest the output data with HugeCTR. Default is False.
         """
 
+        preserve_partitions = False
         if partition_on:
             # Check that the user is not expecting a specific output-file
             # count/structure that is not supported
             if output_files:
                 raise ValueError("`output_files` not supported when `partition_on` is used.")
             if out_files_per_proc:
                 raise ValueError("`out_files_per_proc` not supported when `partition_on` is used.")
@@ -770,35 +809,44 @@
             if method == "worker":
                 if output_files or preserve_files:
                     raise ValueError("output_files and preserve_files require `method='subgraph'`")
                 output_files = False
             elif preserve_files and output_files:
                 raise ValueError("Cannot specify both preserve_files and output_files.")
             elif not (output_files or preserve_files):
-                # Default "subgraph" behavior - Set output_files to the
-                # total umber of workers, multiplied by out_files_per_proc
-                try:
-                    nworkers = len(global_dask_client().cluster.workers)
-                except AttributeError:
-                    nworkers = 1
-                output_files = nworkers * (out_files_per_proc or 1)
+                if out_files_per_proc:
+                    # Default "subgraph" behavior - Set output_files to the
+                    # total umber of workers, multiplied by out_files_per_proc
+                    try:
+                        nworkers = len(global_dask_client().cluster.workers)
+                    except AttributeError:
+                        nworkers = 1
+                    output_files = nworkers * out_files_per_proc
+                else:
+                    # Preserve original Dask partitions if output_files,
+                    # preserve_files AND out_files_per_proc are all None
+                    preserve_partitions = True
 
         # Replace None/False suffix argument with ""
         suffix = suffix or ""
 
         # Check shuffle argument
         shuffle = _check_shuffle_arg(shuffle)
 
         if isinstance(output_files, dict) or (not output_files and preserve_files):
             # Do not shuffle partitions if we are preserving files or
             # if a specific file-partition mapping is already specified
             ddf = self.to_ddf()
         else:
             ddf = self.to_ddf(shuffle=shuffle)
 
+        # Check if partitions should be preserved
+        if preserve_partitions:
+            output_files = ddf.npartitions
+
         # Deal with `method=="subgraph"`.
         # Convert `output_files` argument to a dict mapping
         if output_files:
             #   NOTES on `output_files`:
             #
             # - If a list of file names is specified, a contiguous range of
             #   output partitions will be mapped to each file. The same
@@ -889,28 +937,32 @@
                     split_fn = fn.split(".")
                     if split_fn[-1] in ("parquet", "avro", "orc", "csv"):
                         output_files[".".join(split_fn[:-1]) + suffix] = rgs
                     else:
                         output_files[fn + suffix] = rgs
             suffix = ""  # Don't add a suffix later - Names already include it
 
-        schema = Schema({**self.schema.column_schemas})
+        schema = self.schema.copy()
 
         if dtypes:
             _meta = _set_dtypes(ddf._meta, dtypes)
             ddf = ddf.map_partitions(_set_dtypes, dtypes, meta=_meta)
             for col_name, col_dtype in dtypes.items():
                 schema[col_name] = schema[col_name].with_dtype(col_dtype)
 
         fs = get_fs_token_paths(output_path)[0]
-        fs.mkdirs(output_path, exist_ok=True)
+        fs.mkdirs(str(output_path), exist_ok=True)
 
         tf_metadata = TensorflowMetadata.from_merlin_schema(schema)
         tf_metadata.to_proto_text_file(output_path)
 
+        metadata_path = fs.sep.join([str(output_path), MERLIN_METADATA_DIR_NAME])
+        fs.mkdirs(metadata_path, exist_ok=True)
+        tf_metadata.to_json_file(metadata_path)
+
         # Output dask_cudf DataFrame to dataset
         _ddf_to_dataset(
             ddf,
             fs,
             output_path,
             shuffle,
             output_files,
@@ -918,14 +970,15 @@
             cats or [],
             conts or [],
             labels or [],
             "parquet",
             num_threads,
             self.cpu,
             suffix=suffix,
+            row_group_size=row_group_size,
             partition_on=partition_on,
             schema=schema if write_hugectr_keyset else None,
         )
 
     def to_hugectr(
         self,
         output_path,
```

### Comparing `merlin-core-23.2.1/merlin/io/dataset_engine.py` & `merlin-core-23.4.0/merlin/io/dataset_engine.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/io/fsspec_utils.py` & `merlin-core-23.4.0/merlin/io/fsspec_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 from pyarrow import parquet as pq
 
 if Version(fsspec.__version__) > Version("2021.11.0"):
     import fsspec.parquet as fsspec_parquet
 else:
     fsspec_parquet = None
 
-try:
-    import cudf
+from merlin.core.compat import cudf
+
+if cudf:
     from cudf.core.column import as_column, build_categorical_column
 
     if fsspec_parquet and (Version(cudf.__version__) < Version("21.12.0")):
         # This version of cudf does not support
         # reads from python-file objects. Avoid
         # using the `fsspec.parquet` module
         fsspec_parquet = None
-except ImportError:
-    cudf = None
+
 
 #
 # Parquet-Specific Utilities
 #
 
 
 def _optimized_read_partition_remote(
```

### Comparing `merlin-core-23.2.1/merlin/io/hugectr.py` & `merlin-core-23.4.0/merlin/io/hugectr.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/io/parquet.py` & `merlin-core-23.4.0/merlin/io/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 import threading
 import warnings
 from collections import defaultdict
 from uuid import uuid4
 
 from packaging.version import Version
 
-try:
-    import cudf
+from merlin.core.compat import cudf
+
+if cudf:
     import dask_cudf
     from cudf.io.parquet import ParquetWriter as pwriter_cudf
     from dask_cudf.io.parquet import CudfEngine
-except ImportError:
-    cudf = None
+
 import dask
 import dask.dataframe as dd
 import fsspec
 import pandas as pd
 import pyarrow as pa
 import pyarrow.dataset as pa_ds
 import toolz as tlz
@@ -1038,19 +1038,21 @@
             if self.shuffle == Shuffle.PER_WORKER:
                 df = shuffle_df(df)
             md[path] = self._to_parquet(df, path)
         return md
 
 
 class GPUParquetWriter(BaseParquetWriter):
-    def __init__(self, out_dir, **kwargs):
+    def __init__(self, out_dir, row_group_size=None, **kwargs):
         super().__init__(out_dir, **kwargs)
         # Passing index=False when creating ParquetWriter
         # to avoid bug: https://github.com/rapidsai/cudf/issues/7011
         self.pwriter_kwargs = {"compression": None, "index": False}
+        if row_group_size:
+            self.pwriter_kwargs.update({"row_group_size_rows": row_group_size})
 
     @property
     def _pwriter(self):
         return pwriter_cudf
 
     def _read_parquet(self, source):
         return cudf.io.read_parquet(source)
@@ -1079,31 +1081,32 @@
             md_dict[fn] = writer.close(metadata_file_path=fn)
         for f in self.data_files:
             f.close()
         return md_dict
 
 
 class CPUParquetWriter(BaseParquetWriter):
-    def __init__(self, out_dir, **kwargs):
+    def __init__(self, out_dir, row_group_size=None, **kwargs):
         super().__init__(out_dir, **kwargs)
         self.md_collectors = {}
         self.pwriter_kwargs = {"compression": None}
+        self._row_group_size = row_group_size
 
     @property
     def _pwriter(self):
         return pwriter_pyarrow
 
     def _read_parquet(self, source):
         return pd.read_parquet(source, engine="pyarrow")
 
     def _get_row_group_size(self, df):
         # Make sure our `row_group_size` argument (which corresponds
         # to the number of rows in each row-group) will produce
         # row-groups ~128MB in size.
-        if not hasattr(self, "_row_group_size"):
+        if self._row_group_size is None:
             row_size = df.memory_usage(deep=True).sum() / max(len(df), 1)
             self._row_group_size = math.ceil(128_000_000 / row_size)
         return self._row_group_size
 
     def _to_parquet(self, df, sink):
         md = []
         df.to_parquet(
```

### Comparing `merlin-core-23.2.1/merlin/io/shuffle.py` & `merlin-core-23.4.0/merlin/io/shuffle.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 #
 import enum
 import warnings
 
 import pandas as pd
 from packaging.version import Version
 
-_IGNORE_INDEX_SUPPORTED = Version(pd.__version__) >= Version("1.3.0")
+from merlin.core.compat import cudf
 
-try:
-    import cudf
+_IGNORE_INDEX_SUPPORTED = Version(pd.__version__) >= Version("1.3.0")
 
-    _CUDF_IGNORE_INDEX_SUPPORTED = Version(cudf.__version__) >= Version("22.04.0")
-except ImportError:
-    _CUDF_IGNORE_INDEX_SUPPORTED = None
+if cudf:
+    try:
+        _CUDF_IGNORE_INDEX_SUPPORTED = Version(cudf.__version__) >= Version("22.04.0")
+    except ImportError:
+        _CUDF_IGNORE_INDEX_SUPPORTED = None
 
 
 class Shuffle(enum.Enum):
     PER_PARTITION = 0
     PER_WORKER = 1
     FULL = 2
```

### Comparing `merlin-core-23.2.1/merlin/io/writer.py` & `merlin-core-23.4.0/merlin/io/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,18 @@
 #
 import json
 import math
 import queue
 import threading
 from typing import Optional
 
-try:
-    import cupy as cp
-except ImportError:
-    cp = None
-
 import numpy as np
 from fsspec.core import get_fs_token_paths
 
+from merlin.core.compat import cupy as cp
 from merlin.core.dispatch import annotate
 from merlin.io.shuffle import shuffle_df
 
 
 class Writer:
     def add_data(self, df):
         raise NotImplementedError()
```

### Comparing `merlin-core-23.2.1/merlin/io/writer_factory.py` & `merlin-core-23.4.0/merlin/io/writer_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,38 +26,42 @@
     shuffle,
     use_guid=False,
     bytes_io=False,
     num_threads=0,
     cpu=False,
     fns=None,
     suffix=None,
+    fs=None,
+    **kwargs,  # Format-specific arguments
 ):
     if output_format is None:
         return None
 
-    writer_cls, fs = _writer_cls_factory(output_format, output_path, cpu=cpu)
+    writer_cls, fs = _writer_cls_factory(output_format, output_path, cpu=cpu, fs=fs)
     return writer_cls(
         output_path,
         num_out_files=out_files_per_proc,
         shuffle=shuffle,
         fs=fs,
         use_guid=use_guid,
         bytes_io=bytes_io,
         num_threads=num_threads,
         cpu=cpu,
         fns=fns,
         suffix=suffix,
+        **kwargs,  # Format-specific arguments
     )
 
 
-def _writer_cls_factory(output_format, output_path, cpu=None):
+def _writer_cls_factory(output_format, output_path, cpu=None, fs=None):
     if output_format == "parquet" and cpu:
         writer_cls = CPUParquetWriter
     elif output_format == "parquet":
         writer_cls = GPUParquetWriter
     elif output_format == "hugectr":
         writer_cls = HugeCTRWriter
     else:
         raise ValueError("Output format not yet supported.")
 
-    fs = get_fs_token_paths(output_path)[0]
+    if fs is None:
+        fs = get_fs_token_paths(output_path)[0]
     return writer_cls, fs
```

### Comparing `merlin-core-23.2.1/merlin/schema/__init__.py` & `merlin-core-23.4.0/merlin/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/schema/io/__init__.py` & `merlin-core-23.4.0/merlin/schema/io/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/schema/io/proto_utils.py` & `merlin-core-23.4.0/merlin/schema/io/proto_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/schema/io/schema_bp.py` & `merlin-core-23.4.0/merlin/schema/io/schema_bp.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/merlin/schema/io/tensorflow_metadata.py` & `merlin-core-23.4.0/merlin/schema/io/tensorflow_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 DOMAIN_ATTRS = {FeatureType.INT: "int_domain", FeatureType.FLOAT: "float_domain"}
 FEATURE_TYPES = {
     "int": FeatureType.INT,
     "uint": FeatureType.INT,
     "float": FeatureType.FLOAT,
 }
+SCHEMA_PBTXT_FILE_NAME = "schema.pbtxt"
+SCHEMA_JSON_FILE_NAME = "schema.json"
 
 
 class TensorflowMetadata:
     """
     Reads and writes Merlin schemas as `tensorflow-metadata` Protobuf and JSON files
 
     See https://github.com/tensorflow/metadata for details on this metadata serialization format
@@ -60,28 +62,35 @@
             Schema object parsed from JSON
 
         """
         schema = ProtoSchema().from_json(json)
         return TensorflowMetadata(schema)
 
     @classmethod
-    def from_json_file(cls, path: os.PathLike) -> "TensorflowMetadata":
+    def from_json_file(
+        cls, path: os.PathLike, file_name=SCHEMA_JSON_FILE_NAME
+    ) -> "TensorflowMetadata":
         """Create a TensorflowMetadata schema object from a JSON file
 
         Parameters
         ----------
         path : str
             Path to the JSON file to parse
+        file_name : str
+            Name of the schema file. Defaults to "schema.json".
 
         Returns
         -------
         TensorflowMetadata
             Schema object parsed from JSON file
 
         """
+        path = pathlib.Path(path)
+        if path.is_dir():
+            path = path / file_name
         return cls.from_json(_read_file(path))
 
     @classmethod
     def from_proto_text(cls, proto_text: str) -> "TensorflowMetadata":
         """Create a TensorflowMetadata schema object from a Protobuf text string
 
         Parameters
@@ -101,15 +110,15 @@
             ProtoSchema(), proto_text, schema_pb2.Schema()
         )
 
         return TensorflowMetadata(schema)
 
     @classmethod
     def from_proto_text_file(
-        cls, path: os.PathLike, file_name="schema.pbtxt"
+        cls, path: os.PathLike, file_name=SCHEMA_PBTXT_FILE_NAME
     ) -> "TensorflowMetadata":
         """Create a TensorflowMetadata schema object from a Protobuf text file
 
         Parameters
         ----------
         path : str
             Path to the directory containing the Protobuf text file to parse
@@ -134,24 +143,23 @@
             Generated Proto text string
 
         """
         from tensorflow_metadata.proto.v0 import schema_pb2
 
         return proto_utils.better_proto_to_proto_text(self.proto_schema, schema_pb2.Schema())
 
-    def to_proto_text_file(self, path: str, file_name="schema.pbtxt"):
+    def to_proto_text_file(self, path: str, file_name=SCHEMA_PBTXT_FILE_NAME):
         """Write this TensorflowMetadata schema object to a file as a Proto text string
 
         Parameters
         ----------
         path : str
             Path to the directory containing the Protobuf text file
         file_name : str
             Name of the output file. Defaults to "schema.pbtxt".
-        path: str :
 
         """
         _write_file(self.to_proto_text(), path, file_name)
 
     def copy(self, **kwargs) -> "TensorflowMetadata":
         """Create a copy of this TensorflowMetadata schema object
 
@@ -217,14 +225,27 @@
         -------
         str
             Schema converted to a JSON string
 
         """
         return self.proto_schema.to_json()
 
+    def to_json_file(self, path: str, file_name=SCHEMA_JSON_FILE_NAME):
+        """Write this TensorflowMetadata schema object to a file as a JSON
+
+        Parameters
+        ----------
+        path : str
+            Path to the directory containing the JSON text file
+        file_name : str
+            Name of the output file. Defaults to "schema.json".
+
+        """
+        _write_file(self.to_json(), path, file_name)
+
 
 def _pb_int_domain(column_schema):
     domain = column_schema.properties.get("domain")
     if domain is None:
         return None
 
     return IntDomain(
@@ -248,15 +269,17 @@
     )
 
 
 def _pb_extra_metadata(column_schema):
     properties = {
         k: v for k, v in column_schema.properties.items() if k not in ("domain", "value_count")
     }
-    properties["_dims"] = list(list(dim) for dim in column_schema.shape.as_tuple or [])
+    properties["_dims"] = list(
+        list(dim) if isinstance(dim, tuple) else dim for dim in column_schema.shape.as_tuple or []
+    )
     properties["is_list"] = column_schema.is_list
     properties["is_ragged"] = column_schema.is_ragged
     if column_schema.dtype.element_size:
         properties["dtype_item_size"] = column_schema.dtype.element_size
     return schema_bp.Any().from_dict(properties)
 
 
@@ -392,16 +415,23 @@
             dtype = md.float64
     elif feature.type == FeatureType.BYTES:
         dtype = md.string
 
     dims_list = properties.pop("_dims", None)
 
     if dims_list:
-        dims_tuple = tuple(tuple(dim) for dim in dims_list)
-        dtype = dtype.with_shape(dims_tuple)
+        dims = []
+        for dim in dims_list:
+            if isinstance(dim, list):
+                dims.append(tuple(int(d) if isinstance(d, float) else d for d in dim))
+            elif dim is not None:
+                dims.append(int(dim))
+            else:
+                dims.append(dim)
+        dtype = dtype.with_shape(tuple(dims))
 
         # If we found dims, avoid overwriting that shape with one inferred from counts or flags
         properties.pop("value_count", None)
         properties.pop("is_list", None)
         properties.pop("is_ragged", None)
 
     return dtype
```

### Comparing `merlin-core-23.2.1/merlin/schema/schema.py` & `merlin-core-23.4.0/merlin/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,18 +103,21 @@
 
         # Update the shape and propagate out to flags and value counts
         dtype = dtype.with_shape(new_shape)
         object.__setattr__(self, "dtype", dtype)
         object.__setattr__(self, "is_list", dtype.shape.is_list)
         object.__setattr__(self, "is_ragged", dtype.shape.is_ragged)
 
+        properties = {**self.properties}
+
         if new_shape.dims is not None and len(new_shape.dims) > 1:
             value_counts = {"min": new_shape.dims[1].min, "max": new_shape.dims[1].max}
-            properties = {**self.properties, **{"value_count": value_counts}}
-            object.__setattr__(self, "properties", properties)
+            properties = {**properties, **{"value_count": value_counts}}
+
+        object.__setattr__(self, "properties", properties)
 
     def _shape_from_flags(self, is_list):
         return Shape(((0, None), (0, None))) if is_list else None
 
     def _shape_from_counts(self, value_count):
         return Shape(((0, None), (value_count.min or 0, value_count.max)))
 
@@ -132,15 +135,15 @@
 
         Returns
         -------
         ColumnSchema
             Copied object with new column name
 
         """
-        return replace(self, name=name)
+        return self._replace(name=name)
 
     def with_tags(self, tags: Union[str, Tags]) -> "ColumnSchema":
         """Create a copy of this ColumnSchema object with different column tags
 
         Parameters
         ----------
         tags : Union[str, Tags]
@@ -148,15 +151,15 @@
 
         Returns
         -------
         ColumnSchema
             Copied object with new column tags
 
         """
-        return replace(self, tags=self.tags.override(tags))  # type: ignore
+        return self._replace(tags=self.tags.override(tags))  # type: ignore
 
     def with_properties(self, properties: dict) -> "ColumnSchema":
         """Create a copy of this ColumnSchema object with different column properties
 
         Parameters
         ----------
         properties : dict
@@ -178,24 +181,22 @@
 
         # Using new dictionary to avoid passing old ref to new schema
         new_properties = {**self.properties, **properties}
 
         value_counts = properties.get("value_count", {})
 
         if value_counts:
-            return replace(
-                self,
+            return self._replace(
                 properties=new_properties,
                 dtype=self.dtype.without_shape,
                 is_list=None,
                 is_ragged=None,
             )
         else:
-            return replace(
-                self,
+            return self._replace(
                 properties=new_properties,
             )
 
     def with_dtype(self, dtype, is_list: bool = None, is_ragged: bool = None) -> "ColumnSchema":
         """Create a copy of this ColumnSchema object with different column dtype
 
         Parameters
@@ -218,16 +219,16 @@
         new_dtype = md.dtype(dtype).with_shape(self.shape)
 
         properties = self.properties.copy()
         if is_list is not None or is_ragged is not None:
             properties.pop("value_count", None)
             new_dtype = new_dtype.without_shape
 
-        return replace(
-            self, dtype=new_dtype, properties=properties, is_list=is_list, is_ragged=is_ragged
+        return self._replace(
+            dtype=new_dtype, properties=properties, is_list=is_list, is_ragged=is_ragged
         )
 
     def with_shape(self, shape: Union[Tuple, Shape]) -> "ColumnSchema":
         """
         Create a copy of this object with a new shape
 
         Parameters
@@ -244,16 +245,15 @@
         ------
         TypeError
             If value is not either a tuple or a Shape
         """
         dims = Shape(shape).as_tuple
         properties = self.properties.copy()
         properties.pop("value_count", None)
-        return replace(
-            self,
+        return self._replace(
             dims=dims,
             properties=properties,
             is_list=None,
             is_ragged=None,
         )
 
     @property
@@ -283,14 +283,21 @@
         return self.name
 
     def _domain(self) -> Optional[Domain]:
         """ """
         domain = self.properties.get("domain")
         return Domain(**domain) if domain else None
 
+    def _replace(self, *args, **kwargs):
+        if "dims" not in kwargs and not (
+            "properties" in kwargs and "value_count" in kwargs["properties"]
+        ):
+            kwargs["dims"] = self.shape.as_tuple
+        return replace(self, *args, **kwargs)
+
     def _validate_shape_info(self, shape, value_counts, is_list, is_ragged):
         value_counts = value_counts or {}
 
         min_count = value_counts.get("min", None)
         max_count = value_counts.get("max", None)
         ragged_counts = min_count != max_count
 
@@ -415,35 +422,51 @@
                 schema = schema.excluding_by_tag(selector.tags)
 
         return schema
 
     def apply_inverse(self, selector) -> "Schema":
         return self.excluding(selector)
 
-    def select_by_tag(self, tags: Union[Union[str, Tags], List[Union[str, Tags]]]) -> "Schema":
-        """Select matching columns from this Schema object using a list of tags
+    def select_by_tag(
+        self,
+        tags: Union[Union[str, Tags], List[Union[str, Tags]]],
+        pred_fn=None,
+    ) -> "Schema":
+        """Select columns from this Schema that match ANY of the supplied tags.
 
         Parameters
         ----------
         tags : List[Union[str, Tags]] :
             List of tags that describes which columns match
+        pred_fn : `any` or `all`
+            Predicate function that decides if the column should be selected.
+            Receives iterable of bool values indicating whether each
+            of the provided tags is present on a column schema.
+            Returning True selects this column, False will not return that column.
 
         Returns
         -------
         Schema
             New object containing only the ColumnSchemas of selected columns
 
         """
+        pred_fn = pred_fn or any
+
         if not isinstance(tags, (list, tuple)):
             tags = [tags]
 
         selected_schemas = {}
 
+        normalized_tags = [
+            Tags._value2member_map_.get(tag.lower(), tag) if isinstance(tag, str) else tag
+            for tag in tags
+        ]
+
         for _, column_schema in self.column_schemas.items():
-            if any(x in column_schema.tags for x in tags):
+            if pred_fn(x in column_schema.tags for x in normalized_tags):
                 selected_schemas[column_schema.name] = column_schema
 
         return Schema(selected_schemas)
 
     def excluding_by_tag(self, tags) -> "Schema":
         if not isinstance(tags, (list, tuple)):
             tags = [tags]
@@ -635,14 +658,18 @@
     def __sub__(self, other):
         if other is None:
             return self
 
         if not isinstance(other, Schema):
             raise TypeError(f"unsupported operand type(s) for -: 'Schema' and {type(other)}")
 
-        result = Schema({**self.column_schemas})
+        result = self.copy()
 
         for key in other.column_schemas.keys():
             if key in self.column_schemas.keys():
                 result.column_schemas.pop(key, None)
 
         return result
+
+    def copy(self) -> "Schema":
+        """Return a copy of the schema"""
+        return Schema({**self.column_schemas})
```

### Comparing `merlin-core-23.2.1/merlin/schema/tags.py` & `merlin-core-23.4.0/merlin/schema/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     CATEGORICAL = "categorical"
     CONTINUOUS = "continuous"
     LIST = "list"
     SEQUENCE = "sequence"
     TEXT = "text"
     TOKENIZED = "tokenized"
     TIME = "time"
+    EMBEDDING = "embedding"
 
     # Feature context
     ID = "id"
     USER = "user"
     ITEM = "item"
     SESSION = "session"
     CONTEXT = "context"
```

### Comparing `merlin-core-23.2.1/merlin_core.egg-info/PKG-INFO` & `merlin-core-23.4.0/merlin_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.2.1
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-core-23.2.1/merlin_core.egg-info/SOURCES.txt` & `merlin-core-23.4.0/merlin_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 merlin/core/__init__.py
 merlin/core/_version.py
-merlin/core/compat.py
 merlin/core/dispatch.py
+merlin/core/has_gpu.py
 merlin/core/protocols.py
 merlin/core/utils.py
+merlin/core/compat/__init__.py
+merlin/core/compat/tensorflow.py
+merlin/core/compat/torch.py
 merlin/dag/__init__.py
 merlin/dag/base_operator.py
 merlin/dag/dictarray.py
 merlin/dag/executors.py
 merlin/dag/graph.py
 merlin/dag/node.py
 merlin/dag/selector.py
 merlin/dag/utils.py
 merlin/dag/ops/__init__.py
 merlin/dag/ops/concat_columns.py
 merlin/dag/ops/selection.py
 merlin/dag/ops/subset_columns.py
 merlin/dag/ops/subtraction.py
+merlin/dispatch/lazy.py
 merlin/dtypes/__init__.py
 merlin/dtypes/aliases.py
 merlin/dtypes/base.py
 merlin/dtypes/mapping.py
 merlin/dtypes/registry.py
 merlin/dtypes/shape.py
 merlin/dtypes/mappings/__init__.py
@@ -58,13 +62,21 @@
 merlin/schema/__init__.py
 merlin/schema/schema.py
 merlin/schema/tags.py
 merlin/schema/io/__init__.py
 merlin/schema/io/proto_utils.py
 merlin/schema/io/schema_bp.py
 merlin/schema/io/tensorflow_metadata.py
+merlin/table/__init__.py
+merlin/table/conversions.py
+merlin/table/cupy_column.py
+merlin/table/numpy_column.py
+merlin/table/tensor_column.py
+merlin/table/tensor_table.py
+merlin/table/tensorflow_column.py
+merlin/table/torch_column.py
 merlin_core.egg-info/PKG-INFO
 merlin_core.egg-info/SOURCES.txt
 merlin_core.egg-info/dependency_links.txt
 merlin_core.egg-info/not-zip-safe
 merlin_core.egg-info/requires.txt
 merlin_core.egg-info/top_level.txt
```

### Comparing `merlin-core-23.2.1/pyproject.toml` & `merlin-core-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/setup.cfg` & `merlin-core-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/setup.py` & `merlin-core-23.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.2.1/versioneer.py` & `merlin-core-23.4.0/versioneer.py`

 * *Files identical despite different names*

