# Comparing `tmp/eo-grow-1.4.0.tar.gz` & `tmp/eo_grow-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-grow-1.4.0.tar", last modified: Thu Jan 26 10:13:31 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `eo-grow-1.4.0.tar` & `eo_grow-1.5.0.tar`

### file list

```diff
@@ -1,81 +1,60 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.650194 eo-grow-1.4.0/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1069 2022-01-27 12:06:46.000000 eo-grow-1.4.0/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       84 2022-05-04 07:29:08.000000 eo-grow-1.4.0/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7642 2023-01-26 10:13:31.650194 eo-grow-1.4.0/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5623 2023-01-26 10:07:33.000000 eo-grow-1.4.0/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.562193 eo-grow-1.4.0/eo_grow.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7642 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1749 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      253 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/entry_points.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2022-01-27 12:24:26.000000 eo-grow-1.4.0/eo_grow.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      656 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        7 2023-01-26 10:13:31.000000 eo-grow-1.4.0/eo_grow.egg-info/top_level.txt
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.566193 eo-grow-1.4.0/eogrow/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       69 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9945 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/cli.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.578194 eo-grow-1.4.0/eogrow/core/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       52 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/__init__.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.586194 eo-grow-1.4.0/eogrow/core/area/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      181 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/area/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6610 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/area/base.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5685 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/area/batch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2224 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/area/custom_grid.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3742 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/area/utm.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1411 2022-06-14 13:16:31.000000 eo-grow-1.4.0/eogrow/core/base.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9013 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/config.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    15788 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/logging.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12115 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/pipeline.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4226 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/schemas.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4266 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/core/storage.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.614194 eo-grow-1.4.0/eogrow/pipelines/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       45 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    11436 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/batch_to_eopatch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9603 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/byoc.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    14294 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/download.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    11443 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/download_batch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16365 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/export_maps.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    11218 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/features.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4994 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/import_tiff.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6434 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/merge_samples.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9191 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/prediction.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    11029 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/rasterize.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    12616 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/sampling.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9200 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/split_grid.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     6891 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/testing.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    10619 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/training.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5306 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/pipelines/zipmap.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        0 2022-05-04 07:29:08.000000 eo-grow-1.4.0/eogrow/py.typed
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.622194 eo-grow-1.4.0/eogrow/tasks/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       55 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     5466 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/batch_to_eopatch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1930 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/common.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     9064 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/features.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8162 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/prediction.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    11090 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/spatial.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4086 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/tasks/testing.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1110 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/types.py
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-01-26 10:13:31.650194 eo-grow-1.4.0/eogrow/utils/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       50 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/__init__.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      516 2022-10-24 10:06:48.000000 eo-grow-1.4.0/eogrow/utils/batch.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1266 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/eopatch_list.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2688 2022-11-17 09:47:49.000000 eo-grow-1.4.0/eogrow/utils/export.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2285 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/filter.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8729 2022-11-17 09:47:49.000000 eo-grow-1.4.0/eogrow/utils/fs.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2691 2022-11-17 09:47:49.000000 eo-grow-1.4.0/eogrow/utils/general.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1340 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/grid.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      971 2022-11-17 09:47:49.000000 eo-grow-1.4.0/eogrow/utils/logging.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     7092 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/map.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3569 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/meta.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      993 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/ray.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16547 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/testing.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      316 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/types.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     8857 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/validators.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2053 2022-10-24 10:06:48.000000 eo-grow-1.4.0/eogrow/utils/vector.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1145 2023-01-26 10:07:33.000000 eo-grow-1.4.0/eogrow/utils/zipmap.py
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1003 2023-01-26 10:07:33.000000 eo-grow-1.4.0/pyproject.toml
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      199 2023-01-26 10:07:33.000000 eo-grow-1.4.0/requirements-dev.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       76 2022-10-24 10:06:48.000000 eo-grow-1.4.0/requirements-docs.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      366 2023-01-26 10:07:33.000000 eo-grow-1.4.0/requirements.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-01-26 10:13:31.650194 eo-grow-1.4.0/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     3169 2022-10-24 10:06:48.000000 eo-grow-1.4.0/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/__init__.py
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/py.typed
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/types.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/base.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/config.py
+-rw-r--r--   0        0        0    16771 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/logging.py
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/pipeline.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/schemas.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/storage.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/__init__.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/base.py
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/batch.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/custom_grid.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/utm.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/__init__.py
+-rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/batch_to_eopatch.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/byoc.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/download.py
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/download_batch.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/export_maps.py
+-rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/features.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/import_tiff.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/import_vector.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/merge_samples.py
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/prediction.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/rasterize.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/sampling.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/split_grid.py
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/testing.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/training.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/zipmap.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/__init__.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/batch_to_eopatch.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/common.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/features.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/prediction.py
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/spatial.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/testing.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/batch.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/eopatch_list.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/filter.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/fs.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/general.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/grid.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/logging.py
+-rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/map.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/meta.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/ray.py
+-rw-r--r--   0        0        0    16448 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/testing.py
+-rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/validators.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/vector.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/zipmap.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eo_grow-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 eo_grow-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eo_grow-1.5.0/README.md
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10156 2020-02-02 00:00:00.000000 eo_grow-1.5.0/PKG-INFO
```

### Comparing `eo-grow-1.4.0/LICENSE` & `eo_grow-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/README.md` & `eo_grow-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 - `eogrow-validate <config>` only performs validation of the `<config>` file.
 - `eogrow-test <config>` initializes the pipeline/object but does not run it. Useful for testing if managers are set correctly or for generating area-split grids.
 - `eogrow-ray <cluster> <config>` executes the pipeline defined in `<config>` on the active Ray cluster defined by the `<cluster>` file.
 - `eogrow-template <import path> <template>` generates a template config for the object specified by the `<import path>` and saves it to the `<template>` file (or outputs it directly if `<template>` is not provided).
 
 ## Documentation
 
+For more information on the package visit [readthedocs](https://eo-grow.readthedocs.io/en/latest/).
+
 Explanatory examples can be found [here](https://github.com/sentinel-hub/eo-grow/tree/main/examples).
 
 More details on the config language used by **`eo-grow`** can be found [here](https://github.com/sentinel-hub/eo-grow/tree/main/docs/source/config-language.md).
 
 
 ## Questions and Issues
```

### Comparing `eo-grow-1.4.0/eogrow/cli.py` & `eo_grow-1.5.0/eogrow/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Implements the command line interface for `eo-grow`."""
 import json
 import os
 import re
 import subprocess
+from tempfile import NamedTemporaryFile
 from typing import Optional, Tuple
 
 import click
 
-from .core.config import collect_configs_from_path, decode_config_list, encode_config_list, interpret_config_from_dict
+from .core.config import collect_configs_from_path, interpret_config_from_dict
 from .core.schemas import build_schema_template
 from .pipelines.testing import TestPipeline
 from .utils.general import jsonify
 from .utils.meta import collect_schema, import_object, load_pipeline_class
+from .utils.ray import generate_cluster_config_path, start_cluster_if_needed
 
 variables_option = click.option(
     "-v",
     "--variable",
     "cli_variables",
     multiple=True,
     type=str,
@@ -30,246 +32,224 @@
     help=(
         "One or more indices of EOPatches. If given, a pipeline will run only for those EOPatches. "
         "Example: -t 0 -t 42 will run the pipeline for EOPatches with indices 0 and 42."
     ),
 )
 
 
-class EOGrowCli:
-    """A command line interface class for `eo-grow`
+@click.command()
+@click.argument("config_path", type=click.Path())
+@variables_option
+@test_patches_option
+def run_pipeline(config_path: str, cli_variables: Tuple[str], test_patches: Tuple[int]) -> None:
+    """Execute eo-grow pipeline using CLI.
+
+    \b
+    Example:
+        eogrow config_files/config.json
+    """
 
-    It is designed to be transferable to other packages based on `eo-grow`.
+    raw_configs = collect_configs_from_path(config_path)
+    cli_variable_mapping = dict(_parse_cli_variable(cli_var) for cli_var in cli_variables)
 
-    Note: It looks that click doesn't allow implementing CLI in a proper class structure, therefore here we are using
-    class variable to store the list of packages (https://github.com/pallets/click/issues/601).
+    pipelines = []
+    for raw_config in raw_configs:
+        config = interpret_config_from_dict(raw_config, cli_variable_mapping)
+        if test_patches:
+            config["test_subset"] = list(test_patches)
+
+        pipelines.append(load_pipeline_class(config).from_raw_config(config))
+
+    for pipeline in pipelines:
+        pipeline.run()
+
+
+@click.command()
+@click.argument("cluster_yaml", type=click.Path())
+@click.argument("config_path", type=click.Path())
+@click.option(
+    "--start", "start_cluster", is_flag=True, type=bool, help="Starts the cluster if it is not currently running."
+)
+@click.option(
+    "--stop",
+    "stop_cluster",
+    is_flag=True,
+    type=bool,
+    help=(
+        "Stops the cluster if after running the pipeline. In order for this to work got to AWS console "
+        "-> IAM -> Roles -> select ray-autoscaler-v1 role and attach IAMReadOnlyAccess policy."
+    ),
+)
+@click.option(
+    "--screen",
+    "use_screen",
+    is_flag=True,
+    type=bool,
+    help=(
+        "Run the cluster in a detached mode using screen software. Use Ctrl+A+D to detach any time, "
+        "even when running a pipeline or a Jupyter notebook. Use Ctrl+D to terminate the remote screen."
+    ),
+)
+@click.option(
+    "--tmux",
+    "use_tmux",
+    is_flag=True,
+    type=bool,
+    help="Run the cluster in a detached mode using tmux software. Use Ctrl+B and d to detach.",
+)
+@variables_option
+@test_patches_option
+def run_pipeline_on_cluster(
+    config_path: str,
+    cluster_yaml: str,
+    start_cluster: bool,
+    stop_cluster: bool,
+    use_screen: bool,
+    use_tmux: bool,
+    cli_variables: Tuple[str],
+    test_patches: Tuple[int],
+) -> None:
+    """Command for running an eo-grow pipeline on a remote Ray cluster of AWS EC2 instances. The provided config is
+    fully constructed and uploaded to the cluster head in the `~/.synced_configs/` directory, where it is then
+    executed. A custom suffix is added to distinguish runs which use the same config multiple times.
+
+    \b
+    Example:
+        eogrow-ray cluster.yaml config_files/config.json
     """
+    if start_cluster:
+        start_cluster_if_needed(cluster_yaml)
 
-    _command_namespace = "eogrow"
+    if stop_cluster and (use_screen or use_tmux):
+        raise NotImplementedError("It is not clear how to combine stop flag with either screen or tmux flag")
 
-    def __init__(self, command_namespace: Optional[str] = None):
-        """
-        :param command_namespace: A namespace for calling CLI, e.g. command_namespace='eogrow' if you call commands
-            "eogrow config.json".
-        """
-        if command_namespace:
-            EOGrowCli._command_namespace = command_namespace
-
-    @staticmethod
-    @click.command()
-    @click.argument("config_filename_or_string", type=click.Path())
-    @variables_option
-    @test_patches_option
-    @click.option(
-        "-e",
-        "--encoding",
-        "encoding",
-        is_flag=True,
-        type=bool,
-        help="The string passed to method is treated as an encoded config instead of filename.",
-    )
-    def main(
-        config_filename_or_string: str, cli_variables: Tuple[str], test_patches: Tuple[int], encoding: bool
-    ) -> None:
-        """Execute eo-grow pipeline using CLI.
-
-        \b
-        Example:
-            eogrow config_files/config.json
-        """
-        if encoding:
-            raw_configs = decode_config_list(config_filename_or_string)
-        else:
-            raw_configs = collect_configs_from_path(config_filename_or_string)
-
-        cli_variable_mapping = dict(_parse_cli_variable(cli_var) for cli_var in cli_variables)
-        pipelines = []
-        for raw_config in raw_configs:
-            config = interpret_config_from_dict(raw_config, cli_variable_mapping)
-            if test_patches:
-                config["test_subset"] = list(test_patches)
-
-            pipelines.append(load_pipeline_class(config).from_raw_config(config))
-
-        for pipeline in pipelines:
-            pipeline.run()
-
-    @staticmethod
-    @click.command()
-    @click.argument("cluster_yaml", type=click.Path())
-    @click.argument("config_filename", type=click.Path())
-    @click.option(
-        "--start", "start_cluster", is_flag=True, type=bool, help="Starts the cluster if it is not currently running."
-    )
-    @click.option(
-        "--stop",
-        "stop_cluster",
-        is_flag=True,
-        type=bool,
-        help=(
-            "Stops the cluster if after running the pipeline. In order for this to work got to AWS console "
-            "-> IAM -> Roles -> select ray-autoscaler-v1 role and attach IAMReadOnlyAccess policy."
-        ),
-    )
-    @click.option(
-        "--screen",
-        "use_screen",
-        is_flag=True,
-        type=bool,
-        help=(
-            "Run the cluster in a detached mode using screen software. Use Ctrl+A+D to detach any time, "
-            "even when running a pipeline or a Jupyter notebook. Use Ctrl+D to terminate the remote screen."
-        ),
-    )
-    @click.option(
-        "--tmux",
-        "use_tmux",
-        is_flag=True,
-        type=bool,
-        help="Run the cluster in a detached mode using tmux software. Use Ctrl+B and d to detach.",
-    )
-    @variables_option
-    @test_patches_option
-    def ray(
-        config_filename: str,
-        cluster_yaml: str,
-        start_cluster: bool,
-        stop_cluster: bool,
-        use_screen: bool,
-        use_tmux: bool,
-        cli_variables: Tuple[str],
-        test_patches: Tuple[int],
-    ) -> None:
-        """Command for running an eo-grow pipeline on a remote Ray cluster of AWS EC2 instances
-
-        \b
-        Example:
-            eogrow-ray cluster.yaml config_files/config.json
-        """
-        if stop_cluster and (use_screen or use_tmux):
-            raise NotImplementedError("It is not clear how to combine stop flag with either screen or tmux flag")
-
-        configs = collect_configs_from_path(config_filename)
-        encoded_configs = encode_config_list(configs)
-        cmd = (
-            f"{EOGrowCli._command_namespace} -e {encoded_configs}"
-            + "".join(f' -v "{cli_var_spec}"' for cli_var_spec in cli_variables)  # noqa B028
-            + "".join(f" -t {patch_index}" for patch_index in test_patches)
-            + ("; " if stop_cluster else "")  # Otherwise, ray will incorrectly prepare a command for stopping a cluster
+    raw_configs = [interpret_config_from_dict(config) for config in collect_configs_from_path(config_path)]
+    remote_path = generate_cluster_config_path(config_path)
+
+    with NamedTemporaryFile(mode="w", delete=True, suffix=".json") as local_path:
+        json.dump(raw_configs, local_path)
+        subprocess.run(f"ray rsync_up {cluster_yaml} {local_path.name!r} {remote_path!r}", shell=True)
+
+    cmd = (
+        f"eogrow {remote_path}"
+        + "".join(f' -v "{cli_var_spec}"' for cli_var_spec in cli_variables)  # noqa B028
+        + "".join(f" -t {patch_index}" for patch_index in test_patches)
+        + ("; " if stop_cluster else "")  # Otherwise, ray will incorrectly prepare a command for stopping a cluster
+    )
+    flag_info = [("stop", stop_cluster), ("screen", use_screen), ("tmux", use_tmux)]
+    exec_flags = " ".join(f"--{flag_name}" for flag_name, use_flag in flag_info if use_flag)
+
+    subprocess.run(f"ray exec {exec_flags} {cluster_yaml} {cmd!r}", shell=True)  # noqa B028
+
+
+@click.command()
+@click.argument("import_path", type=str)
+@click.argument("template_path", type=click.Path(), required=False)
+@click.option(
+    "-f",
+    "--force",
+    "force_override",
+    is_flag=True,
+    type=bool,
+    help=(
+        "In case a template path is provided and a file in the path already exists this flag is used to force "
+        "override it."
+    ),
+)
+@click.option(
+    "--template-format",
+    "template_format",
+    type=click.Choice(["minimal", "open-api"], case_sensitive=False),
+    help="Specifies which template format to use. The default is `minimal`",
+    default="minimal",
+)
+@click.option(
+    "--required-only",
+    "required_only",
+    is_flag=True,
+    type=bool,
+    help="If provided it will only include required fields in the template. Only for `minimal` template format",
+)
+@click.option(
+    "--add-descriptions",
+    "add_descriptions",
+    is_flag=True,
+    type=bool,
+    help="Adds descriptions to template. Only for `minimal` template format",
+)
+def make_template(
+    import_path: str,
+    template_path: Optional[str],
+    force_override: bool,
+    template_format: str,
+    required_only: bool,
+    add_descriptions: bool,
+) -> None:
+    """Command for creating a config template for an eo-grow pipeline
+
+    \b
+    Examples:
+        - save template to file:
+            eogrow-template eogrow.pipelines.download.DownloadPipeline config_files/download.json
+        - print template to command line:
+            eogrow-template eogrow.pipelines.download.DownloadPipeline
+    """
+    if not force_override and template_path and os.path.isfile(template_path):
+        raise FileExistsError(f"File {template_path} already exists. You can use -f to force override it.")
+
+    class_with_schema = import_object(import_path)
+    schema = collect_schema(class_with_schema)
+
+    if template_format == "open-api":
+        template = schema.schema()
+    else:
+        template = build_schema_template(
+            schema,
+            pipeline_import_path=import_path,
+            required_only=required_only,
+            add_descriptions=add_descriptions,
         )
-        flag_info = [("start", start_cluster), ("stop", stop_cluster), ("screen", use_screen), ("tmux", use_tmux)]
-        exec_flags = " ".join(f"--{flag_name}" for flag_name, use_flag in flag_info if use_flag)
 
-        subprocess.call(f"ray exec {exec_flags} {cluster_yaml} '{cmd}'", shell=True)  # noqa B028
+    if template_path:
+        with open(template_path, "w") as file:
+            json.dump(template, file, indent=2, default=jsonify)
+    else:
+        click.echo(json.dumps(template, indent=2, default=jsonify))
 
-    @staticmethod
-    @click.command()
-    @click.argument("import_path", type=str)
-    @click.argument("template_path", type=click.Path(), required=False)
-    @click.option(
-        "-f",
-        "--force",
-        "force_override",
-        is_flag=True,
-        type=bool,
-        help=(
-            "In case a template path is provided and a file in the path already exists this flag is used to force "
-            "override it."
-        ),
-    )
-    @click.option(
-        "--template-format",
-        "template_format",
-        type=click.Choice(["minimal", "open-api"], case_sensitive=False),
-        help="Specifies which template format to use. The default is `minimal`",
-        default="minimal",
-    )
-    @click.option(
-        "--required-only",
-        "required_only",
-        is_flag=True,
-        type=bool,
-        help="If provided it will only include required fields in the template. Only for `minimal` template format",
-    )
-    @click.option(
-        "--add-descriptions",
-        "add_descriptions",
-        is_flag=True,
-        type=bool,
-        help="Adds descriptions to template. Only for `minimal` template format",
-    )
-    def make_template(
-        import_path: str,
-        template_path: Optional[str],
-        force_override: bool,
-        template_format: str,
-        required_only: bool,
-        add_descriptions: bool,
-    ) -> None:
-        """Command for creating a config template for an eo-grow pipeline
-
-        \b
-        Examples:
-            - save template to file:
-                eogrow-template eogrow.pipelines.download.DownloadPipeline config_files/download.json
-            - print template to command line:
-                eogrow-template eogrow.pipelines.download.DownloadPipeline
-        """
-        if not force_override and template_path and os.path.isfile(template_path):
-            raise FileExistsError(f"File {template_path} already exists. You can use -f to force override it.")
-
-        object_with_schema = import_object(import_path)
-        schema = collect_schema(object_with_schema)
-
-        if template_format == "open-api":
-            template = schema.schema()
-        else:
-            template = build_schema_template(
-                schema,
-                pipeline_import_path=import_path,
-                required_only=required_only,
-                add_descriptions=add_descriptions,
-            )
-
-        if template_path:
-            with open(template_path, "w") as file:
-                json.dump(template, file, indent=2, default=jsonify)
-        else:
-            click.echo(json.dumps(template, indent=2, default=jsonify))
-
-    @staticmethod
-    @click.command()
-    @click.argument("config_filename", type=click.Path())
-    def validate_config(config_filename: str) -> None:
-        """Validate config without running a pipeline.
-
-        \b
-        Example:
-            eogrow-validate config_files/config.json
-        """
-        for config in collect_configs_from_path(config_filename):
-            raw_config = interpret_config_from_dict(config)
-            load_pipeline_class(config).Schema.parse_obj(raw_config)
-
-        click.echo("Config validation succeeded!")
-
-    @staticmethod
-    @click.command()
-    @click.argument("config_filename", type=click.Path())
-    def run_test_pipeline(config_filename: str) -> None:
-        """Runs a test pipeline that only makes sure the managers work correctly. This can be used to select best
-        area manager parameters.
-
-        \b
-        Example:
-            eogrow-test any_pipeline_config.json
-        """
-        for crude_config in collect_configs_from_path(config_filename):
-            raw_config = interpret_config_from_dict(crude_config)
-            pipeline = TestPipeline.with_defaults(raw_config)
-            pipeline.run()
+
+@click.command()
+@click.argument("config_path", type=click.Path())
+def validate_config(config_path: str) -> None:
+    """Validate config without running a pipeline.
+
+    \b
+    Example:
+        eogrow-validate config_files/config.json
+    """
+    for config in collect_configs_from_path(config_path):
+        raw_config = interpret_config_from_dict(config)
+        load_pipeline_class(config).Schema.parse_obj(raw_config)
+
+    click.echo("Config validation succeeded!")
+
+
+@click.command()
+@click.argument("config_path", type=click.Path())
+def run_test_pipeline(config_path: str) -> None:
+    """Runs a test pipeline that only makes sure the managers work correctly. This can be used to select best
+    area manager parameters.
+
+    \b
+    Example:
+        eogrow-test any_pipeline_config.json
+    """
+    for crude_config in collect_configs_from_path(config_path):
+        raw_config = interpret_config_from_dict(crude_config)
+        pipeline = TestPipeline.with_defaults(raw_config)
+        pipeline.run()
 
 
 def _parse_cli_variable(mapping_str: str) -> Tuple[str, str]:
     """Checks that the input is of shape `name:value` and then splits it into a tuple"""
     match = re.match(r"(?P<name>.+?):(?P<value>.+)", mapping_str)
     if match is None:
         raise ValueError(f'CLI variable input {mapping_str} is not of form `"name:value"`')
```

### Comparing `eo-grow-1.4.0/eogrow/core/area/base.py` & `eo_grow-1.5.0/eogrow/core/area/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Implementation of the base AreaManager."""
 import logging
+import warnings
 from abc import ABCMeta, abstractmethod
 from typing import Dict, Literal, Optional
 
 import fiona
 import fs
 import geopandas as gpd
 import shapely.ops
 from pydantic import Field
 
+from eolearn.core.exceptions import EODeprecationWarning
 from sentinelhub import CRS, BBox, Geometry
 
-from ...types import PatchList
+from ...types import PatchList, RawSchemaDict
 from ...utils.eopatch_list import load_names
 from ...utils.fs import LocalFile
 from ..base import EOGrowObject
 from ..schemas import BaseSchema, ManagerSchema
 from ..storage import StorageManager
 
 LOGGER = logging.getLogger(__name__)
@@ -27,14 +29,31 @@
         description="Buffer that will be applied to AOI geometry. Buffer has to be in the same units as AOI CRS.",
     )
     simplification_factor: Optional[float] = Field(
         description="Tolerance factor (in CRS units) for simplifying the buffered area geometry before splitting it.",
     )
 
 
+def area_schema_deprecation(cls: type, value: Optional[str], values: RawSchemaDict) -> str:
+    """Warns and reconfigures when `area` is used instead of `geometry_filename`."""
+    if values.get("area") is not None:
+        warnings.warn(
+            (
+                "Use `geometry_filename` to provide the file (e.g., geojson, gpkg) with AoI. The `area` parameter is"
+                " deprecated, and extra parameters like `buffer` and `simplification_factor` are no longer available;"
+                " users should prepare the AoI geometry by themselves."
+            ),
+            EODeprecationWarning,
+            stacklevel=2,
+        )
+        return values["area"].filename
+    assert value is not None, "Specify the `geometry_filename` parameter."
+    return value
+
+
 class PatchListSchema(BaseSchema):
     input_folder_key: str = Field(description="The storage manager key pointing to the folder containing the file.")
     filename: str = Field(description="A JSON file containing a list of EOPatch names.", regex=r"^.+\.(json|JSON)$")
 
 
 class BaseAreaManager(EOGrowObject, metaclass=ABCMeta):
     """A manager for the AOI and how it is split into EOPatches"""
@@ -68,18 +87,18 @@
         definitions. EOPatch names are stored in a column with identifier `self.NAME_COLUMN`.
 
         :return: A dictionary of GeoDataFrames that defines how the area is split into EOPatches.
         """
         grid_path = fs.path.combine(self.storage.get_cache_folder(), self.get_grid_cache_filename())
 
         if self.storage.filesystem.exists(grid_path):
-            return self._load_grid(grid_path)
-
-        grid = self._create_grid()
-        self._save_grid(grid, grid_path)
+            grid = self._load_grid(grid_path)
+        else:
+            grid = self._create_grid()
+            self._save_grid(grid, grid_path)
 
         if filtered and self.config.patch_names is not None:
             folder_path = self.storage.get_folder(self.config.patch_names.input_folder_key)
             patch_names_path = fs.path.join(folder_path, self.config.patch_names.filename)
             relevant_patch_names = set(load_names(self.storage.filesystem, patch_names_path))
 
             for crs, geoms in grid.items():
@@ -144,26 +163,14 @@
             for _, row in grid.iterrows():
                 named_bboxes.append((row.eopatch_name, BBox(row.geometry.bounds, crs=crs)))
 
         return named_bboxes
 
 
 def get_geometry_from_file(
-    filesystem: fs.base.FS,
-    file_path: str,
-    buffer: Optional[float],
-    simplification_factor: Optional[float],
-    geopandas_engine: Literal["fiona", "pyogrio"] = "fiona",
+    filesystem: fs.base.FS, file_path: str, geopandas_engine: Literal["fiona", "pyogrio"] = "fiona"
 ) -> Geometry:
     """Provides a single geometry object of entire AOI"""
     with LocalFile(file_path, mode="r", filesystem=filesystem) as local_file:
         area_df = gpd.read_file(local_file.path, engine=geopandas_engine)
-
-    area_shape = shapely.ops.unary_union(area_df.geometry)
-
-    if buffer is not None:
-        area_shape = area_shape.buffer(buffer)
-
-    if simplification_factor is not None:
-        area_shape = area_shape.simplify(simplification_factor, preserve_topology=True)
-
-    return Geometry(area_shape, CRS(area_df.crs))
+        area_shape = shapely.ops.unary_union(area_df.geometry)
+        return Geometry(area_shape, CRS(area_df.crs))
```

### Comparing `eo-grow-1.4.0/eogrow/core/area/batch.py` & `eo_grow-1.5.0/eogrow/core/area/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 import fs
 import geopandas as gpd
 from geopandas import GeoDataFrame
 from pydantic import Field
 
 from sentinelhub import CRS, BatchRequest, BatchRequestStatus, BatchSplitter, Geometry, SentinelHubBatch
 
+from ...utils.validators import field_validator
 from ..storage import StorageManager
-from .base import AreaSchema, BaseAreaManager, get_geometry_from_file
+from .base import AreaSchema, BaseAreaManager, area_schema_deprecation, get_geometry_from_file
 
 LOGGER = logging.getLogger(__name__)
 
 
 class MissingBatchIdError(ValueError):
     """Exception that is triggered if ID of a Sentinel Hub batch job is missing."""
 
 
 class BatchAreaManager(BaseAreaManager):
-    """Area manager that splits grid per UTM zones"""
+    """Area manager that splits the area according to the Sentinel Hub Batch tiling grids."""
 
     class Schema(BaseAreaManager.Schema):
-        area: AreaSchema
+        area: Optional[AreaSchema] = Field(description="DEPRECATED, use `geometry_filename` instead.")
+        geometry_filename: str = Field(  # type:ignore[assignment]
+            None, description="Name of the file that defines the AoI geometry, located in the input data folder."
+        )
         tiling_grid_id: int = Field(
             description="An id of one of the tiling grids predefined at Sentinel Hub Batch service."
         )
         resolution: float = Field(
             description=(
                 "Resolution of downloaded imagery in meters. Resolution options are predefined at Sentinel Hub Batch"
                 " service for a chosen tiling_grid_id."
@@ -39,29 +43,29 @@
         batch_id: Optional[str] = Field(
             description=(
                 "ID of the batch job that defines the AOI. Not required when using BatchDownloadPipeline,"
                 " which generates a new batch job with the given AOI parameters."
             ),
         )
 
+        _warn_and_adapt_old_config = field_validator("geometry_filename", area_schema_deprecation, pre=True)
+
     config: Schema
 
     def __init__(self, config: Schema, storage: StorageManager):
         super().__init__(config, storage)
         # We provide a way to inject a Batch ID after initialization if no ID was given in the config
         # This is meant to be used only in the BatchDownloadPipeline to force caching
         self._injected_batch_id: Optional[str] = None
 
     def get_area_geometry(self, *, crs: CRS = CRS.WGS84) -> Geometry:
-        file_path = fs.path.join(self.storage.get_input_data_folder(), self.config.area.filename)
+        file_path = fs.path.join(self.storage.get_input_data_folder(), self.config.geometry_filename)
         return get_geometry_from_file(
             filesystem=self.storage.filesystem,
             file_path=file_path,
-            buffer=self.config.area.buffer,
-            simplification_factor=self.config.area.simplification_factor,
             geopandas_engine=self.storage.config.geopandas_backend,
         ).transform(crs)
 
     def _create_grid(self) -> Dict[CRS, GeoDataFrame]:
         """Uses BatchSplitter to create a grid for the selected batch job."""
         batch_id = self.config.batch_id or self._injected_batch_id
 
@@ -113,15 +117,15 @@
         if batch_request.tiling_grid != expected_tiling_grid_params:
             raise ValueError(
                 f"Tiling grid parameters in config are {expected_tiling_grid_params} but given batch "
                 f"request has parameters {batch_request.tiling_grid}"
             )
 
     def get_grid_cache_filename(self) -> str:
-        input_filename = fs.path.basename(self.config.area.filename)
+        input_filename = fs.path.basename(self.config.geometry_filename)
         input_filename = input_filename.rsplit(".", 1)[0]
 
         raw_params = [
             input_filename,
             self.config.tiling_grid_id,
             self.config.resolution,
             self.config.tile_buffer_x,
```

### Comparing `eo-grow-1.4.0/eogrow/core/area/custom_grid.py` & `eo_grow-1.5.0/eogrow/core/area/custom_grid.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/core/area/utm.py` & `eo_grow-1.5.0/eogrow/core/area/utm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 """Area manager implementation for automated UTM CRS grids."""
 
 import logging
 from collections import defaultdict
-from typing import Dict
+from typing import Dict, Optional
 
 import fs
 import geopandas as gpd
 from geopandas import GeoDataFrame
 from pydantic import Field
 
 from sentinelhub import CRS, Geometry, UtmZoneSplitter
 
+from ...utils.validators import field_validator
 from ..schemas import BaseSchema
-from .base import AreaSchema, BaseAreaManager, get_geometry_from_file
+from .base import AreaSchema, BaseAreaManager, area_schema_deprecation, get_geometry_from_file
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PatchSchema(BaseSchema):
     size_x: int = Field(description="A width of each EOPatch in meters")
     size_y: int = Field(description="A height of each EOPatch in meters")
     buffer_x: float = Field(0, description="Number of meters by which to increase the tile size to left and right.")
     buffer_y: float = Field(0, description="Number of meters by which to increase the tile size to up and down.")
 
 
 class UtmZoneAreaManager(BaseAreaManager):
-    """Area manager that splits grid per UTM zones"""
+    """Area manager that splits the area per UTM zone"""
 
     class Schema(BaseAreaManager.Schema):
-        area: AreaSchema
+        area: Optional[AreaSchema] = Field(description="DEPRECATED, use `geometry_filename` instead.")
+        geometry_filename: str = Field(  # type:ignore[assignment]
+            None, description="Name of the file that defines the AoI geometry, located in the input data folder."
+        )
         patch: PatchSchema
 
         offset_x: float = Field(0, description="An offset of tiling grid in horizontal dimension")
         offset_y: float = Field(0, description="An offset of tiling grid in vertical dimension")
 
+        _warn_and_adapt_old_config = field_validator("geometry_filename", area_schema_deprecation, pre=True)
+
     config: Schema
 
     def get_area_geometry(self, *, crs: CRS = CRS.WGS84) -> Geometry:
-        file_path = fs.path.join(self.storage.get_input_data_folder(), self.config.area.filename)
+        file_path = fs.path.join(self.storage.get_input_data_folder(), self.config.geometry_filename)
         return get_geometry_from_file(
             filesystem=self.storage.filesystem,
             file_path=file_path,
-            buffer=self.config.area.buffer,
-            simplification_factor=self.config.area.simplification_factor,
             geopandas_engine=self.storage.config.geopandas_backend,
         ).transform(crs)
 
     def _create_grid(self) -> Dict[CRS, GeoDataFrame]:
         """Uses UtmZoneSplitter to create a grid"""
         area_geometry = self.get_area_geometry()
         LOGGER.info("Splitting area geometry into UTM zone grid")
@@ -74,15 +78,15 @@
         for crs, named_bbox_geoms in crs_to_patches.items():
             names, geoms = zip(*named_bbox_geoms)
             grid[crs] = gpd.GeoDataFrame({self.NAME_COLUMN: names}, geometry=list(geoms), crs=crs.pyproj_crs())
 
         return grid
 
     def get_grid_cache_filename(self) -> str:
-        input_filename = fs.path.basename(self.config.area.filename)
+        input_filename = fs.path.basename(self.config.geometry_filename)
         input_filename = input_filename.rsplit(".", 1)[0]
 
         raw_params = [
             input_filename,
             self.config.patch.size_x,
             self.config.patch.size_y,
             self.config.patch.buffer_x,
```

### Comparing `eo-grow-1.4.0/eogrow/core/base.py` & `eo_grow-1.5.0/eogrow/core/base.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/core/config.py` & `eo_grow-1.5.0/eogrow/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 """Implements functions that transform raw dictionaries/JSON files according to the config language of eo-grow."""
-import base64
 import copy
-import json
 import os
 import re
 from functools import reduce
 from typing import Any, Callable, Dict, List, NewType, Optional, Set, cast
 
 import fs.path
 import rapidjson
 
 from eolearn.core.utils.fs import get_base_filesystem_and_path, get_full_path, join_path
 
-from ..utils.general import jsonify
 from ..utils.meta import get_os_import_path
 
 CrudeConfig = NewType("CrudeConfig", dict)
 RawConfig = NewType("RawConfig", dict)
 
 
-def encode_config_list(configs: List[CrudeConfig]) -> str:
-    """Dumps a list of configs into a json and the encodes it with base64
-
-    :return: A base64-encoded string
-    """
-    json_string = json.dumps(configs, default=jsonify)
-    return base64.b64encode(json_string.encode()).decode()
-
-
-def decode_config_list(encoded_config_list: str) -> List[CrudeConfig]:
-    """Provides a list of config objects by decoding a base64-encoded string."""
-    decoded_string = base64.b64decode(encoded_config_list.encode()).decode()
-    decoded_list = json.loads(decoded_string)
-    if not isinstance(decoded_list, list):
-        raise ValueError(f"Encoding does not represent a list of configs. Got {type(decoded_list)}.")
-    return decoded_list
-
-
 def collect_configs_from_path(path: str, used_config_paths: Optional[Set[str]] = None) -> List[CrudeConfig]:
     """Loads and builds a list of config dictionaries defined by the parameters stored in files
 
     This function performs the 1st stage of language interpretation as described in
     eo-grow/documentation/config-language.md`.
 
     :param path: A full path where a config file is located
```

### Comparing `eo-grow-1.4.0/eogrow/core/logging.py` & `eo_grow-1.5.0/eogrow/core/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Implementation of LoggingManager and different handlers used for logging."""
 import contextlib
 import json
 import logging
 import sys
 import time
-from logging import FileHandler, Filter, Formatter, Handler, LogRecord, StreamHandler
-from typing import Any, List, Optional, Sequence, Union
+from logging import FileHandler, Filter, Formatter, Handler, LogRecord
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
+import colorlog
 import fs
 from fs.base import FS
 from fs.errors import FilesystemClosed
 from pydantic import Field
 
 from eolearn.core.utils.fs import join_path, unpickle_fs
 
@@ -20,14 +21,16 @@
 from ..utils.logging import get_instance_info
 from ..utils.meta import get_package_versions
 from .base import EOGrowObject
 from .config import RawConfig
 from .schemas import ManagerSchema
 from .storage import StorageManager
 
+DEFAULT_PACKAGES_TOKEN = "..."  # fix docs if this is changed!
+
 
 class LoggingManager(EOGrowObject):
     """A class that manages logging specifics"""
 
     class Schema(ManagerSchema):
         save_logs: bool = Field(
             False,
@@ -39,41 +42,45 @@
         include_logs_to_report: bool = Field(
             False,
             description=(
                 "If log files should be parsed into an EOExecution report file or just linked. When working "
                 "with larger number of EOPatches the recommended option is False."
             ),
         )
-        eoexecution_ignore_packages: Optional[List[str]] = Field(
+        eoexecution_ignore_packages: Tuple[str] = Field(
+            (DEFAULT_PACKAGES_TOKEN,),
             description=(
-                "Names of packages which logs will not be written to EOExecution log files. The default null value "
-                "means that a default list of packages will be used."
-            )
+                "Names of packages for which the logs will not be written to EOExecution log files. You can reference"
+                ' the defaults with "...", for example, adding another package can be done with ["...", "some_package"]'
+            ),
         )
 
-        pipeline_ignore_packages: Optional[List[str]] = Field(
+        pipeline_ignore_packages: Tuple[str] = Field(
+            (DEFAULT_PACKAGES_TOKEN,),
             description=(
-                "Names of packages which logs will not be written to the main pipeline log file. The default null "
-                "value means that a default list of packages will be used."
-            )
+                "Names of packages for which the logs will not be written to the main pipeline log file. You can"
+                ' reference the defaults with "...", for example, adding another package can be done with'
+                ' ["...", "some_package"]'
+            ),
         )
         pipeline_logs_backup_interval: float = Field(
             60,
             description=(
                 "When working with a remote storage this parameter defines a minimal number of seconds between "
                 "two consecutive times when pipeline log file will be copied into the remote storage."
             ),
         )
 
         show_logs: bool = Field(False, description="Shows basic pipeline execution logs at stdout.")
-        stdout_log_packages: Optional[List[str]] = Field(
+        stdout_log_packages: Tuple[str] = Field(
+            (DEFAULT_PACKAGES_TOKEN,),
             description=(
-                "Names of packages which logs will be written to stdout. The default null value means that a default "
-                "list of packages will be used."
-            )
+                "Names of packages for which the logs will be written to stdout. You can reference the defaults with"
+                ' "...", for example, adding another package can be done with ["...", "package_to_display"]'
+            ),
         )
 
         capture_warnings: bool = Field(
             True,
             description=(
                 "If warnings should be treated as logs and with save_logs=True written into log files instead of "
                 "being printed in stderr."
@@ -143,28 +150,31 @@
             logs_filename,
             filesystem=self.storage.filesystem,
             backup_interval=self.config.pipeline_logs_backup_interval,
             encoding="utf-8",
         )
 
         formatter = Formatter(
-            "%(levelname)s %(asctime)s %(name)s:%(lineno)d:\n\t%(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+            "%(levelname)s [%(asctime)s] %(name)s:%(lineno)d:\n\t%(message)s", datefmt="%Y-%m-%d %H:%M:%S"
         )
         file_handler.setFormatter(formatter)
 
         file_handler.addFilter(LogFileFilter(ignore_packages=self.config.pipeline_ignore_packages))
 
         return file_handler
 
     def _create_stdout_handler(self) -> Handler:
         """Creates a logging handler to write logs into a standard output."""
-        stdout_handler = StreamHandler(sys.stdout)
+        stdout_handler = colorlog.StreamHandler(sys.stdout)
         stdout_handler.setLevel(logging.INFO)
 
-        formatter = Formatter("%(levelname)s %(name)s:%(lineno)d: %(message)s")
+        formatter = colorlog.ColoredFormatter(
+            "%(log_color)s %(levelname)s %(cyan)s[%(asctime)s] %(light_blue)s%(name)s:%(lineno)d: %(white)s%(message)s",
+            datefmt="%H:%M:%S",
+        )
         stdout_handler.setFormatter(formatter)
 
         stdout_handler.addFilter(StdoutFilter(log_packages=self.config.stdout_log_packages))
 
         return stdout_handler
 
     def stop_logging(self, handlers: List[Handler]) -> None:
@@ -325,21 +335,21 @@
     DEFAULT_LOG_PACKAGES = (
         "eogrow",
         "__main__",
         "root",
         "sentinelhub.api.batch",
     )
 
-    def __init__(self, *args: Any, log_packages: Optional[Sequence[str]] = None, **kwargs: Any):
+    def __init__(self, *args: Any, log_packages: Sequence[str], **kwargs: Any):
         """
         :param log_packages: Names of packages which logs to include.
         """
         super().__init__(*args, **kwargs)
 
-        self.log_packages = self.DEFAULT_LOG_PACKAGES if log_packages is None else log_packages
+        self.log_packages = _parse_packages(log_packages, self.DEFAULT_LOG_PACKAGES)
 
     def filter(self, record: LogRecord) -> bool:
         """Shows only logs from eo-grow type packages and high-importance logs"""
         return any(package_name in record.name for package_name in self.log_packages)
 
 
 class LogFileFilter(Filter):
@@ -353,21 +363,21 @@
         "fiona",
         "rasterio",
         "graphviz",
         "urllib3",
         "boto3",
     )
 
-    def __init__(self, *args: Any, ignore_packages: Optional[Sequence[str]] = None, **kwargs: Any):
+    def __init__(self, *args: Any, ignore_packages: Sequence[str], **kwargs: Any):
         """
         :param ignore_packages: Names of packages which logs will be ignored.
         """
         super().__init__(*args, **kwargs)
 
-        self.ignore_packages = self.DEFAULT_IGNORE_PACKAGES if ignore_packages is None else tuple(ignore_packages)
+        self.ignore_packages = _parse_packages(ignore_packages, self.DEFAULT_IGNORE_PACKAGES)
 
     def filter(self, record: LogRecord) -> bool:
         """Shows everything from the main thread and process except logs from packages that are on the ignore list.
         Those packages send a lot of useless logs.
         """
         if record.name.startswith(self.ignore_packages):
             return False
@@ -385,18 +395,31 @@
         "rasterio",
         "numba",
         "fiona.ogrext",
         "fiona.env",
         "fiona._env",
     )
 
-    def __init__(self, ignore_packages: Optional[Sequence[str]] = None, *args: Any, **kwargs: Any):
+    def __init__(self, *args: Any, ignore_packages: Sequence[str], **kwargs: Any):
         """
         :param ignore_packages: Names of packages which logs will be ignored.
         """
         super().__init__(*args, **kwargs)
 
-        self.ignore_packages = self.DEFAULT_IGNORE_PACKAGES if ignore_packages is None else tuple(ignore_packages)
+        self.ignore_packages = _parse_packages(ignore_packages, self.DEFAULT_IGNORE_PACKAGES)
 
     def filter(self, record: LogRecord) -> bool:
         """Ignores logs from certain low-level packages"""
         return not record.name.startswith(self.ignore_packages)
+
+
+def _parse_packages(log_packages: Sequence[str], default_packages: Sequence[str]) -> Tuple[str, ...]:
+    """Builds a tuple of unique package names to be logged/ignored. If the placeholder for default packages is
+    present, those are added as well.
+
+    Since many handlers use the `startswith` method we return a tuple (a better alternative is frozenset).
+    """
+    unique_packages = set(log_packages)
+    if DEFAULT_PACKAGES_TOKEN in unique_packages:
+        unique_packages.remove(DEFAULT_PACKAGES_TOKEN)
+        unique_packages.update(default_packages)
+    return tuple(unique_packages)
```

### Comparing `eo-grow-1.4.0/eogrow/core/pipeline.py` & `eo_grow-1.5.0/eogrow/core/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Implementation of the base Pipeline class."""
-import datetime as dt
 import logging
 import time
 import uuid
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 from eolearn.core import CreateEOPatchTask, EOExecutor, EONode, EOWorkflow, LoadTask, SaveTask, WorkflowResults
 from eolearn.core.extra.ray import RayExecutor
 
 from ..types import ExecKwargs, PatchList, ProcessingType
+from ..utils.general import current_timestamp
 from ..utils.meta import import_object
 from ..utils.ray import handle_ray_connection
 from .area.base import BaseAreaManager
 from .base import EOGrowObject
 from .config import RawConfig
 from .logging import EOExecutionFilter, EOExecutionHandler, LoggingManager
 from .schemas import ManagerSchema, PipelineSchema
@@ -27,15 +27,15 @@
     """A base class for execution of processing procedures which may or may not include running EOWorkflows, running
     EOExecutions, creating maps, etc.
 
     The functionalities of this class are:
         - collecting input arguments (either from command line or as an initialization parameter) and parsing them
         - preparing a list of patches
         - preparing execution arguments
-        - monitoring the pipeline and reporting
+        - running the pipeline, monitoring, and reporting
     """
 
     class Schema(PipelineSchema):
         """Configuration schema, describing input parameters and their types."""
 
     config: Schema
 
@@ -52,14 +52,18 @@
 
         self.storage: StorageManager = self._load_manager(config.storage)
         self.sh_config = self.storage.sh_config
 
         self.area_manager: BaseAreaManager = self._load_manager(config.area, storage=self.storage)
         self.logging_manager: LoggingManager = self._load_manager(config.logging, storage=self.storage)
 
+    @property
+    def _pipeline_name(self) -> str:
+        return self.config.pipeline_name or self.__class__.__name__
+
     @classmethod
     def from_raw_config(cls: Type[Self], config: RawConfig, *args: Any, **kwargs: Any) -> Self:
         """Creates an object from a dictionary by constructing a validated config and use it to create the object."""
         validated_config = cls.Schema.parse_obj(config)
         if "raw_config" not in kwargs:
             kwargs["raw_config"] = config
         return cls(validated_config, *args, **kwargs)
@@ -80,15 +84,15 @@
             raise ValueError("Unable to load manager, field `manager` specifying it's class is missing.")
         manager_class = import_object(manager_config.manager)
         manager = manager_class(manager_config, **manager_params)
         return manager
 
     def get_pipeline_execution_name(self, pipeline_timestamp: str) -> str:
         """Returns the full name of the pipeline execution"""
-        return f"{pipeline_timestamp}-{self.__class__.__name__}-{self.pipeline_id}"
+        return f"{pipeline_timestamp}-{self._pipeline_name}-{self.pipeline_id}"
 
     def get_patch_list(self) -> PatchList:
         """Method which at the initialization prepares the list of EOPatches which will be used"""
         patch_list = self.area_manager.get_patch_list()
 
         if self.config.test_subset is not None:
             LOGGER.info("Filtering according to `test_subset` parameter.")
@@ -205,28 +209,28 @@
             executor.make_report(include_logs=self.logging_manager.config.include_logs_to_report)
             LOGGER.info("Saved EOExecution report to %s", executor.get_report_path(full_path=True))
 
         return successful, failed, execution_results
 
     def run(self) -> None:
         """The main method for pipeline execution. It sets up logging and runs the pipeline procedure."""
-        timestamp = dt.datetime.utcnow().strftime("%Y-%m-%dT%H-%M-%SZ")
+        timestamp = current_timestamp()
         self.current_execution_name = self.get_pipeline_execution_name(timestamp)
 
         handlers = self.logging_manager.start_logging(self.current_execution_name)
         try:
             self.logging_manager.update_pipeline_report(
                 pipeline_execution_name=self.current_execution_name,
                 pipeline_config=self.config,
                 pipeline_raw_config=self._raw_config,
                 pipeline_id=self.pipeline_id,
                 pipeline_timestamp=timestamp,
             )
 
-            LOGGER.info("Running %s", self.__class__.__name__)
+            LOGGER.info("Running %s", self._pipeline_name)
 
             pipeline_start = time.time()
             finished, failed = self.run_procedure()
             elapsed_time = time.time() - pipeline_start
 
             if failed:
                 LOGGER.info(
```

### Comparing `eo-grow-1.4.0/eogrow/core/schemas.py` & `eo_grow-1.5.0/eogrow/core/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     manager: Optional[ImportPath] = Field(description="An import path to this specific manager.")
 
 
 class PipelineSchema(BaseSchema):
     """Base schema of the Pipeline class."""
 
     pipeline: Optional[ImportPath] = Field(description="Import path to an implementation of Pipeline class.")
+    pipeline_name: Optional[str] = Field(
+        description="Custom pipeline name for easier identification in logs. By default the class name is used."
+    )
 
     storage: ManagerSchema = Field(description="A schema of an implementation of StorageManager class")
     validate_storage = field_validator("storage", validate_manager, pre=True)
 
     area: ManagerSchema = Field(description="A schema of an implementation of AreaManager class")
     validate_area = field_validator("area", validate_manager, pre=True)
```

### Comparing `eo-grow-1.4.0/eogrow/core/storage.py` & `eo_grow-1.5.0/eogrow/core/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Implementation of the StorageManager class for handling project storage."""
-from typing import Dict, Literal, Optional
+from typing import Any, Dict, Literal, Optional
 
 import fs
-from fs.base import FS
 from pydantic import BaseSettings, Field
 
+import sentinelhub
 from eolearn.core.utils.fs import get_aws_credentials, get_filesystem, is_s3_path
 from sentinelhub import SHConfig
 
-from ..types import AwsAclType
 from .base import EOGrowObject
 from .schemas import ManagerSchema
 
 
 class StorageManager(EOGrowObject):
     PRESET_FOLDERS: Dict[str, str] = {"logs": "logs", "input_data": "input-data", "cache": "cache"}
 
@@ -26,19 +25,16 @@
         aws_profile: Optional[str] = Field(
             env="AWS_PROFILE",
             description=(
                 "The AWS profile with credentials needed to access the S3 buckets. In case the profile isn't specified"
                 " with a parameter it can be read from an environmental variable."
             ),
         )
-        aws_acl: Optional[AwsAclType] = Field(
-            description=(
-                "An optional parameter to specify under what kind of access control list (ACL) objects should be saved"
-                " to an AWS S3 bucket."
-            )
+        filesystem_kwargs: Dict[str, Any] = Field(
+            default_factory=dict, description="Optional kwargs to be passed on to FS specs."
         )
         structure: Dict[str, str] = Field(
             default_factory=dict,
             description="A flat key: value store mapping each key to a path in the project.",
         )
         geopandas_backend: Literal["fiona", "pyogrio"] = Field(
             "fiona", description="Which backend is used for IO operations when using geopandas."
@@ -54,34 +50,28 @@
         super().__init__(config)
 
         for folder_key, folder_path in self.PRESET_FOLDERS.items():
             if folder_key not in self.config.structure:
                 self.config.structure[folder_key] = folder_path
 
         self.sh_config = self._prepare_sh_config()
-        self.filesystem = self._prepare_filesystem()
+        self.filesystem = get_filesystem(
+            self.config.project_folder, create=True, config=self.sh_config, **self.config.filesystem_kwargs
+        )
 
     def _prepare_sh_config(self) -> SHConfig:
         """Prepares an instance of `SHConfig` containing AWS credentials. In case given AWS profile doesn't exist it
         will show a warning and return a config without AWS credentials."""
-        sh_config = SHConfig(hide_credentials=True)
+        sh_config = SHConfig(hide_credentials=True) if sentinelhub.__version__ < "3.9.0" else SHConfig()
 
-        if self.is_on_aws() and self.config.aws_profile:
+        if self.is_on_s3() and self.config.aws_profile:
             sh_config = get_aws_credentials(aws_profile=self.config.aws_profile, config=sh_config)
 
         return sh_config
 
-    def _prepare_filesystem(self) -> FS:
-        """Prepares a filesystem object with the configuration parameters."""
-        fs_kwargs: Dict[str, str] = {}
-        if is_s3_path(self.config.project_folder) and self.config.aws_acl:
-            fs_kwargs["acl"] = self.config.aws_acl
-
-        return get_filesystem(self.config.project_folder, create=True, config=self.sh_config, **fs_kwargs)
-
     def get_folder(self, key: str, full_path: bool = False) -> str:
         """Returns the path associated with the given key in the structure config."""
         folder_path = self.config.structure[key]
         self.filesystem.makedirs(folder_path, recreate=True)
 
         if full_path:
             return fs.path.combine(self.config.project_folder, folder_path)
@@ -95,10 +85,10 @@
         """Returns the path associated with the cache key."""
         return self.get_folder("cache", full_path=full_path)
 
     def get_input_data_folder(self, full_path: bool = False) -> str:
         """Returns the path associated with the input_data key."""
         return self.get_folder("input_data", full_path=full_path)
 
-    def is_on_aws(self) -> bool:
+    def is_on_s3(self) -> bool:
         """Returns True if the project_folder is on S3, False otherwise."""
         return is_s3_path(self.config.project_folder)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/batch_to_eopatch.py` & `eo_grow-1.5.0/eogrow/pipelines/batch_to_eopatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Pipeline for conversion of batch results to EOPatches."""
 from typing import Any, List, Optional
 
 import numpy as np
-from pydantic import Field, root_validator
+from pydantic import Field, validator
 
 from eolearn.core import (
+    CreateEOPatchTask,
     EONode,
     EOWorkflow,
     FeatureType,
     MergeEOPatchesTask,
     MergeFeatureTask,
     OverwritePermission,
     RemoveFeatureTask,
@@ -19,15 +20,15 @@
 from eolearn.io import ImportFromTiffTask
 
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..tasks.batch_to_eopatch import DeleteFilesTask, FixImportedTimeDependentFeatureTask, LoadUserDataTask
 from ..types import ExecKwargs, Feature, FeatureSpec, PatchList, RawSchemaDict
 from ..utils.filter import get_patches_with_missing_features
-from ..utils.validators import optional_field_validator, parse_dtype
+from ..utils.validators import ensure_storage_key_presence, optional_field_validator, parse_dtype
 
 
 class FeatureMappingSchema(BaseSchema):
     """Defines a mapping between 1 or more batch outputs into an EOPatch feature"""
 
     batch_files: List[str] = Field(
         description=(
@@ -40,43 +41,46 @@
     dtype: Optional[np.dtype] = Field(description="Dtype of the output feature.")
     _parse_dtype = optional_field_validator("dtype", parse_dtype, pre=True)
 
 
 class BatchToEOPatchPipeline(Pipeline):
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(description="Storage manager key pointing to the path with Batch results")
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         output_folder_key: str = Field(description="Storage manager key pointing to where the EOPatches are saved")
-
-        mapping: List[FeatureMappingSchema] = Field(
-            description="A list of mapping from batch files into EOPatch features."
-        )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
 
         userdata_feature_name: Optional[str] = Field(
             description="A name of META_INFO feature in which userdata.json would be stored."
         )
         userdata_timestamp_reader: Optional[str] = Field(
             description=(
                 "Either an import path to a utility function or a Python code describing how to read "
                 "dates from userdata dictionary."
             ),
             example="\"[info['date'] for info in json.loads(userdata['metadata'])]\"",
         )
+
+        mapping: List[FeatureMappingSchema] = Field(
+            description="A list of mapping from batch files into EOPatch features."
+        )
+
+        @validator("mapping")
+        def check_nonempty_input(cls, value: list, values: RawSchemaDict) -> list:
+            if not value:
+                params = "userdata_feature_name", "userdata_timestamp_reader"
+                assert any(
+                    values.get(param) is not None for param in params
+                ), "At least one of `userdata_feature_name`, `userdata_timestamp_reader`, or `mapping` has to be set."
+            return value
+
         remove_batch_data: bool = Field(
             True, description="Whether to remove the raw batch data after the conversion is complete"
         )
 
-        @root_validator
-        def check_something_is_converted(cls, values: RawSchemaDict) -> RawSchemaDict:
-            """Check that the pipeline has something to do."""
-            params = "userdata_feature_name", "userdata_timestamp_reader", "mapping"
-            assert any(
-                values.get(param) is not None for param in params
-            ), "At least one of `userdata_feature_name`, `userdata_timestamp_reader`, or `mapping` has to be set."
-            return values
-
     config: Schema
 
     def __init__(self, *args: Any, **kwargs: Any):
         """Additionally sets some basic parameters calculated from config parameters"""
         super().__init__(*args, **kwargs)
 
         self._input_folder = self.storage.get_folder(self.config.input_folder_key)
@@ -100,47 +104,42 @@
         features: List[FeatureSpec] = [FeatureType.BBOX]
         features.extend(feature_mapping.feature for feature_mapping in self.config.mapping)
 
         if self.config.userdata_feature_name:
             features.append(FeatureType.META_INFO)
 
         if self.config.userdata_timestamp_reader:
-            features.append(FeatureType.TIMESTAMP)
+            features.append(FeatureType.TIMESTAMPS)
 
         return features
 
     def build_workflow(self) -> EOWorkflow:
         """Builds the workflow"""
-        userdata_node = None
+        metadata_node = EONode(CreateEOPatchTask(), name="Establish BBox")
         if self._has_userdata:
-            userdata_node = EONode(
+            metadata_node = EONode(
                 LoadUserDataTask(
                     path=self._input_folder,
                     filesystem=self.storage.filesystem,
                     userdata_feature_name=self.config.userdata_feature_name,
                     userdata_timestamp_reader=self.config.userdata_timestamp_reader,
-                )
+                ),
+                inputs=[metadata_node],
             )
 
         mapping_nodes = [
-            self._get_tiff_mapping_node(feature_mapping, userdata_node) for feature_mapping in self.config.mapping
+            self._get_tiff_mapping_node(feature_mapping, metadata_node) for feature_mapping in self.config.mapping
         ]
 
-        last_node = userdata_node
+        last_node = metadata_node
         if len(mapping_nodes) == 1:
             last_node = mapping_nodes[0]
         elif len(mapping_nodes) > 1:
             last_node = EONode(MergeEOPatchesTask(), inputs=mapping_nodes)
 
-        if last_node is None:
-            raise ValueError(
-                "At least one of `userdata_feature_name`, `userdata_timestamp_reader`, or `mapping` has to be set in"
-                " the config. This should have been caught in the validation phase, please report issue."
-            )
-
         processing_node = self.get_processing_node(last_node)
 
         save_task = SaveTask(
             path=self.storage.get_folder(self.config.output_folder_key),
             filesystem=self.storage.filesystem,
             features=self._get_output_features(),
             compress_level=1,
@@ -161,15 +160,15 @@
 
     def _get_tiff_mapping_node(self, mapping: FeatureMappingSchema, previous_node: Optional[EONode]) -> EONode:
         """Prepares tasks and dependencies that convert tiff files into an EOPatch feature"""
         if not all(batch_file.endswith(".tif") for batch_file in mapping.batch_files):
             raise ValueError(f"All batch files should end with .tif but found {mapping.batch_files}")
 
         feature_type, feature_name = mapping.feature
-        if not (feature_type.is_spatial() and feature_type.is_raster()):
+        if not (feature_type.is_image()):
             raise ValueError(f"Tiffs can only be read into spatial raster feature types, but {feature_type} was given.")
 
         tmp_features = []
         end_nodes = []
         for batch_file in mapping.batch_files:
             feature = feature_type, batch_file.replace(".tif", "_tmp")
             tmp_features.append(feature)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/byoc.py` & `eo_grow-1.5.0/eogrow/pipelines/byoc.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 from eogrow.core.config import RawConfig
 
 from ..core.pipeline import Pipeline
 from ..types import JsonDict
 from ..utils.validators import (
     ensure_defined_together,
     ensure_exactly_one_defined,
+    ensure_storage_key_presence,
     optional_field_validator,
     parse_data_collection,
 )
 from .export_maps import TIMESTAMP_FORMAT
 
 LOGGER = logging.getLogger(__name__)
 
 
 class IngestByocTilesPipeline(Pipeline):
     """Ingests .tiff files to a BYOC collection. Based on `ExportMapsPipeline` output for timeless features."""
 
     class Schema(Pipeline.Schema):
         byoc_tile_folder_key: str
+        _ensure_byoc_tile_folder_key = ensure_storage_key_presence("byoc_tile_folder_key")
+
         file_glob_pattern: str = Field("**/*.tiff", description="Pattern used to obtain the TIFF files to use")
 
         new_collection_name: Optional[str] = Field(description="Used for defining a new BYOC collection.")
         existing_collection: Optional[DataCollection] = Field(description="Used when updating and reingesting.")
         _parse_byoc_collection = optional_field_validator("existing_collection", parse_data_collection, pre=True)
         _ensure_exclusion = ensure_exactly_one_defined("new_collection_name", "existing_collection")
 
@@ -59,24 +62,26 @@
             if is_temporal and value is None:
                 return None
             if not is_temporal and value is not None:
                 return datetime.datetime.fromisoformat(value)
             raise AssertionError("Sensing time should be set for timeless BYOC collections.")
 
         cover_geometry_folder_key: Optional[str] = Field(description="Folder for supplying a custom cover geometry.")
+        _ensure_cover_geometry_folder_key = ensure_storage_key_presence("cover_geometry_folder_key")
+
         cover_geometry: Optional[str] = Field(description="Specifies a geometry file describing the cover geometry.")
         _ensure_cover_geometry = ensure_defined_together("cover_geometry_folder_key", "cover_geometry")
 
         reingest_existing: bool = Field(False, description="Whether to reingest or skip already ingested tiles.")
 
     config: Schema
 
     def __init__(self, config: Schema, raw_config: Optional[RawConfig] = None):
         super().__init__(config, raw_config)
-        if not self.storage.is_on_aws():
+        if not self.storage.is_on_s3():
             raise ValueError("Can only ingest for projects based on S3 storage.")
         project_folder = self.storage.config.project_folder
         self.bucket_name = project_folder.replace("s3://", "").split("/")[0]
         self._cover_geometry_df: Optional[gpd.GeoDataFrame] = None
 
     def get_byoc_collection(self, byoc_client: SentinelHubBYOC) -> JsonDict:
         """Obtains information about the existing collection or creates a new one."""
@@ -135,15 +140,15 @@
 
     def _get_tile_cover_geometry(self, tiff_path: str) -> Geometry:
         """Get geometry of the tile by intersecting the tiff geometry with the general cover geometry."""
         full_path = f"s3://{self.bucket_name}/" + tiff_path
         with rasterio.open(full_path) as tiff_data:
             tiff_bounds = tiff_data.bounds
             tiff_crs = CRS(tiff_data.crs.to_epsg())
-        tiff_poly = BBox([tiff_bounds.left, tiff_bounds.bottom, tiff_bounds.right, tiff_bounds.top], tiff_crs).geometry
+        tiff_poly = BBox((tiff_bounds.left, tiff_bounds.bottom, tiff_bounds.right, tiff_bounds.top), tiff_crs).geometry
 
         cover_poly = self._get_cover_geometry(tiff_crs)
         final_poly = tiff_poly.intersection(cover_poly) if cover_poly else tiff_poly
         return Geometry(final_poly, crs=tiff_crs)
 
     def _get_cover_geometry(self, crs: CRS) -> Optional[Geometry]:
         """Lazy-loads the cover geometry of whole area, reprojecting (and combining) in desired CRS on call."""
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/download.py` & `eo_grow-1.5.0/eogrow/pipelines/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..types import ExecKwargs, Feature, FeatureSpec, PatchList, ProcessingType, TimePeriod
 from ..utils.filter import get_patches_with_missing_features
 from ..utils.validators import (
     ensure_exactly_one_defined,
+    ensure_storage_key_presence,
     field_validator,
     optional_field_validator,
     parse_data_collection,
     parse_dtype,
     parse_time_period,
 )
 
@@ -72,14 +73,15 @@
 class BaseDownloadPipeline(Pipeline, metaclass=abc.ABCMeta):
     """Base pipeline for downloading satellite data"""
 
     class Schema(Pipeline.Schema):
         output_folder_key: str = Field(
             description="Storage manager key pointing to the path where downloaded EOPatches will be saved."
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
 
         compress_level: int = Field(1, description="Level of compression used in saving EOPatches")
         threads_per_worker: Optional[int] = Field(
             description=(
                 "Maximum number of parallel threads used during download by each worker. If set to None it will use "
                 "5 * N threads, where N is the number of CPUs on the machine"
             ),
@@ -246,15 +248,15 @@
 
     config: Schema
 
     def _get_output_features(self) -> List[FeatureSpec]:
         features: List[FeatureSpec] = [
             (FeatureType.DATA, self.config.bands_feature_name),
             FeatureType.BBOX,
-            FeatureType.TIMESTAMP,
+            FeatureType.TIMESTAMPS,
         ]
         features.extend(self.config.additional_data)
         return features
 
     def _get_download_node(self, session_loader: SessionLoaderType) -> EONode:
         time_diff = None if self.config.time_difference is None else dt.timedelta(minutes=self.config.time_difference)
         bands_dtype = np.uint16 if self.config.use_dn else np.float32
@@ -296,15 +298,15 @@
     class Schema(BaseDownloadPipeline.Schema, CommonDownloadFields, TimeDependantFields):
         features: List[Feature] = Field(description="Features to construct from the evalscript")
         evalscript_path: str
 
     config: Schema
 
     def _get_output_features(self) -> List[FeatureSpec]:
-        features: List[FeatureSpec] = [FeatureType.BBOX, FeatureType.TIMESTAMP]
+        features: List[FeatureSpec] = [FeatureType.BBOX, FeatureType.TIMESTAMPS]
         features.extend(self.config.features)
         return features
 
     def _get_download_node(self, session_loader: SessionLoaderType) -> EONode:
         evalscript = read_data(self.config.evalscript_path, data_format=MimeType.TXT)
         time_diff = None if self.config.time_difference is None else dt.timedelta(minutes=self.config.time_difference)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/download_batch.py` & `eo_grow-1.5.0/eogrow/pipelines/download_batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,21 @@
     read_data,
 )
 
 from ..core.area.batch import BatchAreaManager
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..types import TimePeriod
-from ..utils.validators import field_validator, optional_field_validator, parse_data_collection, parse_time_period
+from ..utils.validators import (
+    ensure_storage_key_presence,
+    field_validator,
+    optional_field_validator,
+    parse_data_collection,
+    parse_time_period,
+)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class InputDataSchema(BaseSchema):
     """Parameter structure for a single data collection used in a batch request."""
 
@@ -61,14 +67,15 @@
 
     class Schema(Pipeline.Schema):
         area: BatchAreaManager.Schema
 
         output_folder_key: str = Field(
             description="Storage manager key pointing to the path where batch results will be saved."
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
 
         inputs: List[InputDataSchema]
         evalscript_path: str
 
         tiff_outputs: List[str] = Field(default_factory=list, description="Names of TIFF outputs of a batch job")
         save_userdata: bool = Field(
             False, description="A flag indicating if userdata.json should also be one of the results of the batch job."
@@ -197,15 +204,15 @@
                 for input_config in self.config.inputs
             ],
             responses=responses,
             geometry=geometry,
         )
 
         data_folder = self.storage.get_folder(self.config.output_folder_key, full_path=True).rstrip("/")
-        if not self.storage.is_on_aws():
+        if not self.storage.is_on_s3():
             raise ValueError(f"The data folder path should be on s3 bucket, got {data_folder}")
 
         return self.batch_client.create(
             sentinelhub_request,
             tiling_grid=SentinelHubBatch.tiling_grid(
                 grid_id=self.config.area.tiling_grid_id,
                 resolution=self.config.area.resolution,
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/export_maps.py` & `eo_grow-1.5.0/eogrow/pipelines/export_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,32 +24,35 @@
 
 from eogrow.core.config import RawConfig
 
 from ..core.pipeline import Pipeline
 from ..types import ExecKwargs, Feature, PatchList
 from ..utils.eopatch_list import group_by_crs
 from ..utils.map import CogifyResamplingOptions, WarpResamplingOptions, cogify_inplace, extract_bands, merge_tiffs
+from ..utils.validators import ensure_storage_key_presence
 
 LOGGER = logging.getLogger(__name__)
 
 TIMESTAMP_FORMAT = "%Y-%m-%dT%H-%M-%S"
 
 
 class ExportMapsPipeline(Pipeline):
     """Pipeline to export a feature into a tiff map"""
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(
             description="The storage manager key pointing to the input folder for the export maps pipeline."
         )
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         output_folder_key: str = Field(
             description=(
                 "The storage manager key pointing to the output folder for the maps in the export maps pipeline."
             )
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
 
         feature: Feature
         map_name: Optional[str] = Field(regex=r".+\." + MimeType.TIFF.extension + r"?\b")  # noqa
         map_dtype: Literal["int8", "int16", "uint8", "uint16", "float32"]
         no_data_value: Optional[float] = Field(description="No data value to be passed to GeoTIFFs")
         scale_factor: Optional[float] = Field(description="Feature will be multiplied by this value at export")
         band_indices: Optional[List[int]] = Field(
@@ -201,15 +204,15 @@
         return exec_args
 
     def _prepare_files(self, geotiff_paths: List[str]) -> Tuple[FS, List[str]]:
         """Returns a filesystem and appropriate paths to the geotiffs to use in the pipeline.
 
         If required files are copied locally and a temporary filesystem object is returned.
         """
-        make_local_copies = self.storage.is_on_aws() or self.config.force_local_copies
+        make_local_copies = self.storage.is_on_s3() or self.config.force_local_copies
 
         if not make_local_copies:
             return self.storage.filesystem, geotiff_paths
 
         temp_fs = TempFS(identifier="_merge_maps_temp")
         temp_geotiff_paths = [fs.path.basename(path) for path in geotiff_paths]
 
@@ -263,18 +266,18 @@
         parallelize(filesystem.remove, geotiff_paths, workers=None, multiprocess=False)
 
         return time_to_tiffs_map
 
     def _extract_num_bands_and_timestamps(self, eopatch_name: str) -> Tuple[int, List[dt.datetime]]:
         """Loads an eopatch to get information about number of bands and the timestamps."""
         path = fs.path.join(self.storage.get_folder(self.config.input_folder_key), eopatch_name)
-        patch = EOPatch.load(path, (FeatureType.TIMESTAMP, self.config.feature), filesystem=self.storage.filesystem)
+        patch = EOPatch.load(path, (FeatureType.TIMESTAMPS, self.config.feature), filesystem=self.storage.filesystem)
         if self.config.band_indices is not None:
-            return len(self.config.band_indices), patch.timestamp
-        return patch[self.config.feature].shape[-1], patch.timestamp
+            return len(self.config.band_indices), patch.timestamps
+        return patch[self.config.feature].shape[-1], patch.timestamps
 
     @staticmethod
     def _execute_split_jobs(jobs: List["SplitTiffsJob"]) -> None:
         """Executes all the jobs for a specific tiff. This prevents parallel processes fighting over IO to a tiff."""
         for job in jobs:
             extract_bands(job.input_path, job.output_path, job.bands)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/features.py` & `eo_grow-1.5.0/eogrow/pipelines/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,21 @@
     MedianMosaickingTask,
     MosaickingTask,
     ValidDataFractionPredicate,
     join_valid_and_cloud_masks,
 )
 from ..types import Feature, FeatureSpec, PatchList, TimePeriod
 from ..utils.filter import get_patches_with_missing_features
-from ..utils.validators import field_validator, optional_field_validator, parse_dtype, parse_time_period
+from ..utils.validators import (
+    ensure_storage_key_presence,
+    field_validator,
+    optional_field_validator,
+    parse_dtype,
+    parse_time_period,
+)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ValidityFiltering(BaseSchema):
     cloud_mask_feature_name: Optional[str] = Field(
         description="Name of cloud mask to enable additional filtering by cloud"
@@ -48,17 +54,19 @@
 class FeaturesPipeline(Pipeline):
     """A pipeline to calculate and prepare features for ML"""
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(
             description="The storage manager key pointing to the input folder for the features pipeline."
         )
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         output_folder_key: str = Field(
             description="The storage manager key pointing to the output folder for the features pipeline."
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
 
         bands_feature_name: str = Field(description="Name of data feature containing band data")
 
         data_preparation: ValidityFiltering
 
         ndis: Dict[str, Tuple[int, int]] = Field(
             default_factory=dict,
@@ -85,15 +93,15 @@
             self._get_output_features(),
         )
 
         return filtered_patch_list
 
     def _get_output_features(self) -> List[FeatureSpec]:
         """Lists all features that are to be saved upon the pipeline completion"""
-        return [(FeatureType.DATA, self.config.output_feature_name), FeatureType.BBOX, FeatureType.TIMESTAMP]
+        return [(FeatureType.DATA, self.config.output_feature_name), FeatureType.BBOX, FeatureType.TIMESTAMPS]
 
     def _get_bands_feature(self) -> Feature:
         return FeatureType.DATA, self.config.bands_feature_name
 
     def _get_valid_data_feature(self) -> Feature:
         return FeatureType.MASK, self.config.data_preparation.valid_data_feature_name
 
@@ -266,11 +274,11 @@
             mosaicking_task = MedianMosaickingTask(
                 self._get_bands_feature(),
                 (start_date, end_date, self.config.mosaicking.n_mosaics),
                 self._get_valid_data_feature(),
             )
         mosaicking_node = EONode(mosaicking_task, inputs=[previous_node])
         return EONode(
-            CopyTask(features=[self._get_bands_feature(), FeatureType.BBOX, FeatureType.TIMESTAMP]),
+            CopyTask(features=[self._get_bands_feature(), FeatureType.BBOX, FeatureType.TIMESTAMPS]),
             inputs=[mosaicking_node],
             name="Remove non-mosaicked features",
         )
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/import_tiff.py` & `eo_grow-1.5.0/eogrow/pipelines/import_tiff.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from eolearn.features.utils import ResizeLib, ResizeMethod, ResizeParam
 from eolearn.io import ImportFromTiffTask
 
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..types import Feature, PatchList
 from ..utils.filter import get_patches_with_missing_features
-from ..utils.validators import optional_field_validator, parse_dtype
+from ..utils.validators import ensure_storage_key_presence, optional_field_validator, parse_dtype
 
 
 class ResizeSchema(BaseSchema):
     """How to resize the tiff data after adding it to EOPatches."""
 
     resize_type: ResizeParam = Field(
         description=(
@@ -33,18 +33,21 @@
     method: ResizeMethod = ResizeMethod.LINEAR
     library: ResizeLib = ResizeLib.PIL
 
 
 class ImportTiffPipeline(Pipeline):
     class Schema(Pipeline.Schema):
         output_folder_key: str = Field(description="The storage manager key of the output folder.")
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
         tiff_folder_key: str = Field(
             "input_data",
             description="The storage manager key of the folder containing the tiff. Defaults to the input-data folder.",
         )
+        _ensure_tiff_folder_key = ensure_storage_key_presence("tiff_folder_key")
         input_filename: str = Field(description="Name of tiff file to import.")
         output_feature: Feature = Field(description="Feature containing the imported tiff information.")
         no_data_value: float = Field(
             np.nan, description="Value assigned to undefined pixels, e.g. outside of given input image."
         )
         dtype: Optional[np.dtype] = Field(description="Custom dtype for the imported feature.")
         _parse_dtype = optional_field_validator("dtype", parse_dtype, pre=True)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/merge_samples.py` & `eo_grow-1.5.0/eogrow/pipelines/merge_samples.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 from pydantic import Field
 
 from eolearn.core import EOPatch, EOWorkflow, FeatureType, LoadTask, OutputTask, linearly_connect_tasks
 from eolearn.core.utils.fs import get_full_path
 
 from ..core.pipeline import Pipeline
 from ..types import Feature, FeatureSpec
+from ..utils.validators import ensure_storage_key_presence
 
 LOGGER = logging.getLogger(__name__)
 
 
 class MergeSamplesPipeline(Pipeline):
     """Pipeline to merge sampled data into joined numpy arrays"""
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(
             description="The storage manager key pointing to the input folder for the merge samples."
         )
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         output_folder_key: str = Field(
             description="The storage manager key pointing to the output folder for the merge samples pipeline."
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
         features_to_merge: List[Feature] = Field(
             description="Dictionary of all features for which samples are to be merged."
         )
         include_timestamp: bool = Field(False, description="Whether to also prepare an array of merged timestamps.")
         id_filename: Optional[str] = Field(
             description=(
                 "Filename of array holding patch ID of concatenated features. The patch ID is the index of the patch in"
@@ -59,15 +63,15 @@
 
         self.merge_and_save_features(result_patches, patch_names=successful)
 
         return successful, failed
 
     def build_workflow(self) -> EOWorkflow:
         """Creates a workflow that outputs the requested features"""
-        features_to_load: List[FeatureSpec] = [FeatureType.TIMESTAMP] if self.config.include_timestamp else []
+        features_to_load: List[FeatureSpec] = [FeatureType.TIMESTAMPS] if self.config.include_timestamp else []
         features_to_load.extend(self.config.features_to_merge)
         load_task = LoadTask(
             self.storage.get_folder(self.config.input_folder_key),
             filesystem=self.storage.filesystem,
             features=features_to_load,
         )
         output_task = OutputTask(name=self._OUTPUT_NAME)
@@ -93,16 +97,16 @@
 
         if patch_sample_nums is None:
             raise ValueError("Need at least one feature to merge.")
 
         if self.config.include_timestamp:
             arrays = []
             for patch, sample_num in zip(patches, patch_sample_nums):
-                arrays.append(np.tile(np.array(patch.timestamp), (sample_num, 1)))
-                patch.timestamp = []
+                arrays.append(np.tile(np.array(patch.timestamps), (sample_num, 1)))
+                patch.timestamps = []
 
             self._save_array(np.concatenate(arrays, axis=0), "TIMESTAMPS")
 
         if self.config.id_filename:
             LOGGER.info("Started merging EOPatch ids")
             patch_id_arrays = [
                 np.ones(sample_num, dtype=np.uint32) * patch_id for patch_id, sample_num in enumerate(patch_sample_nums)
@@ -113,16 +117,16 @@
 
     @staticmethod
     def _collect_and_remove_feature(patch: EOPatch, feature: Feature) -> np.ndarray:
         """Collects a feature from an EOPatch and removes it from EOPatch to conserve overall memory"""
         feature_array = patch[feature]
         feature_type, _ = feature
 
-        if feature_type is FeatureType.TIMESTAMP:
-            patch.timestamp = []
+        if feature_type is FeatureType.TIMESTAMPS:
+            patch.timestamps = []
             return np.array(feature_array)
 
         del patch[feature]
 
         axis = feature_type.ndim() - 2  # type: ignore[operator]
         feature_array = np.squeeze(feature_array, axis=axis)
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/prediction.py` & `eo_grow-1.5.0/eogrow/pipelines/prediction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 """Implements a base prediction pipeline and a LGBM specialized classification and regression pipelines."""
 import abc
 from typing import List, Optional, Tuple
 
 import fs
 import numpy as np
-from pydantic import Field, root_validator
+from pydantic import Field
 
 from eolearn.core import EONode, EOWorkflow, FeatureType, LoadTask, MergeEOPatchesTask, OverwritePermission, SaveTask
 
 from ..core.pipeline import Pipeline
 from ..tasks.prediction import ClassificationPredictionTask, RegressionPredictionTask
-from ..types import Feature, FeatureSpec, PatchList, RawSchemaDict
+from ..types import Feature, FeatureSpec, PatchList
 from ..utils.filter import get_patches_with_missing_features
-from ..utils.validators import optional_field_validator, parse_dtype
+from ..utils.validators import (
+    ensure_defined_together,
+    ensure_storage_key_presence,
+    optional_field_validator,
+    parse_dtype,
+)
 
 
 class BasePredictionPipeline(Pipeline, metaclass=abc.ABCMeta):
     """Pipeline to load a model and run prediction on EOPatches"""
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(
             description="The storage manager key pointing to the input folder of the model input data."
         )
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         input_features: List[Feature] = Field(
             description=(
                 "List of features of form `[(feature_type, feature_name)]` specifying which features are model input in"
                 " the correct order"
             )
         )
 
         output_folder_key: str = Field(
             description="The storage manager key pointing to the output folder for the prediction pipeline."
         )
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
         dtype: Optional[np.dtype] = Field(
             description="Casts the result to desired type. Uses predictor output type by default."
         )
         _parse_dtype = optional_field_validator("dtype", parse_dtype, pre=True)
 
-        prediction_mask_folder_key: Optional[str]
         prediction_mask_feature_name: Optional[str] = Field(
             description="Name of `MASK_TIMELESS` feature which defines which areas will be predicted"
         )
+        prediction_mask_folder_key: Optional[str]
+        _ensure_mask_feature_key = ensure_defined_together("prediction_mask_feature_name", "prediction_mask_folder_key")
 
         model_folder_key: str = Field(
             description="The storage manager key pointing to the folder of the model used in the prediction pipeline."
         )
+        _ensure_model_folder_key = ensure_storage_key_presence("model_folder_key")
         compress_level: int = Field(1, description="Level of compression used in saving EOPatches")
 
-        @root_validator
-        def validate_prediction_mask(cls, values: RawSchemaDict) -> RawSchemaDict:
-            """If prediction mask is defined then also its input folder has to be defined."""
-            is_mask_defined = values.get("prediction_mask_feature_name") is not None
-            is_folder_defined = values.get("prediction_mask_folder_key") is not None
-
-            if is_mask_defined:
-                assert (
-                    is_folder_defined
-                ), "Parameter prediction_mask_feature_name is defined but prediction_mask_folder_key is not."
-
-            return values
-
     config: Schema
 
     @abc.abstractmethod
     def _get_output_features(self) -> List[FeatureSpec]:
         """Lists all features that are to be saved upon the pipeline completion"""
 
     @property
@@ -95,15 +92,15 @@
 
     def _get_data_preparation_node(self) -> EONode:
         """Returns nodes containing for loading and preparing the data as well as the endpoint tasks"""
         features_load_node = EONode(
             LoadTask(
                 self.storage.get_folder(self.config.input_folder_key),
                 filesystem=self.storage.filesystem,
-                features=[FeatureType.BBOX, FeatureType.TIMESTAMP, *self.config.input_features],
+                features=[FeatureType.BBOX, FeatureType.TIMESTAMPS, *self.config.input_features],
             )
         )
 
         if not self.config.prediction_mask_folder_key:
             return features_load_node
 
         mask_load_node = EONode(
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/rasterize.py` & `eo_grow-1.5.0/eogrow/pipelines/rasterize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,159 @@
 """Implements a pipeline for rasterizing vector datasets."""
 import logging
 import os
 import uuid
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import fiona
 import fs
 import geopandas as gpd
 import numpy as np
-from pydantic import Field
+from pydantic import Field, validator
 
-from eolearn.core import (
-    CreateEOPatchTask,
-    EONode,
-    EOWorkflow,
-    FeatureType,
-    LoadTask,
-    MergeEOPatchesTask,
-    OverwritePermission,
-    SaveTask,
-)
+from eolearn.core import CreateEOPatchTask, EONode, EOWorkflow, FeatureType, LoadTask, OverwritePermission, SaveTask
 from eolearn.geometry import VectorToRasterTask
 from eolearn.io import VectorImportTask
+from sentinelhub import CRS
 
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..types import Feature, FeatureSpec, PatchList
 from ..utils.filter import get_patches_with_missing_features
 from ..utils.fs import LocalFile
-from ..utils.validators import ensure_exactly_one_defined, field_validator, parse_dtype
+from ..utils.validators import ensure_exactly_one_defined, ensure_storage_key_presence, field_validator, parse_dtype
 from ..utils.vector import concat_gdf
 
 LOGGER = logging.getLogger(__name__)
 
 
-class VectorColumnSchema(BaseSchema):
-    """Parameter structure for individual feature / dataset column to be rasterized"""
-
-    value: Optional[float] = Field(
-        description="Value to use for all rasterized polygons. Use either this or `values_column`."
-    )
-    values_column: Optional[str] = Field(
-        description=(
-            "GeoPandas dataframe column name from which to read values for geometries. Use either this or `value`."
-        )
-    )
-    output_feature: Feature = Field(description="Output feature of rasterization.")
-    polygon_buffer: float = Field(0, description="The size of polygon buffering to be applied before rasterization.")
-    resolution: Optional[float] = Field(
-        description="Rendering resolution in meters. Cannot be used with `raster_shape`."
-    )
-    raster_shape: Optional[Tuple[int, int]] = Field(
-        description="Shape of resulting raster image. Cannot be used with `resolution`."
-    )
-    overlap_value: Optional[int] = Field(description="Value to write over the areas where polygons overlap.")
-    dtype: np.dtype = Field(np.dtype("int32"), description="Numpy dtype of the output feature.")
-    _parse_dtype = field_validator("dtype", parse_dtype, pre=True)
-    no_data_value: int = Field(0, description="The no_data_value argument to be passed to VectorToRasterTask")
-
-    _check_value_values_column = ensure_exactly_one_defined("value", "values_column")
-    _check_shape_resolution = ensure_exactly_one_defined("raster_shape", "resolution")
-
-
 class Preprocessing(BaseSchema):
     reproject_crs: Optional[int] = Field(
         description=(
-            "An EPSG code of a CRS in which vector_input data will be reprojected once loaded. This parameter "
-            "is mandatory if vector_input contains multiple layers in different CRS"
+            "An EPSG code of a CRS in which vector_input data will be reprojected once loaded. Mandatory if"
+            " the input vector contains multiple layers in different CRS."
         ),
     )
 
 
 class RasterizePipeline(Pipeline):
     """A pipeline module for rasterizing vector datasets."""
 
     class Schema(Pipeline.Schema):
-        input_folder_key: str = Field(
-            description="The storage manager key pointing to the input folder for the rasterization pipeline."
+        input_folder_key: str = Field(description="The storage manager key pointing to the input folder.")
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
+        output_folder_key: str = Field(description="The storage manager key pointing to the output folder.")
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
+        vector_input: Union[Feature, str] = Field(description="An input filename or a feature containing vector data.")
+        output_feature: Feature = Field(description="A feature which should contain the newly rasterized data.")
+
+        raster_value: Optional[float] = Field(
+            description="Value to be used for all rasterized polygons. Cannot be used with `raster_values_column`."
         )
-        output_folder_key: str = Field(
-            description="The storage manager key pointing to the output folder for the rasterization pipeline pipeline."
+        raster_values_column: Optional[str] = Field(
+            description=(
+                "GeoPandas column for reading per-geometry rasterization values. Cannot be used with `raster_value`."
+            )
         )
-        vector_input: Union[Feature, str] = Field(
-            description="A filename in the input_data folder or a feature containing vector data."
+        _check_raster_value_values_column = ensure_exactly_one_defined("raster_value", "raster_values_column")
+
+        resolution: Optional[float] = Field(
+            description="Rendering resolution in meters. Cannot be used with `raster_shape`."
         )
-        dataset_layer: Optional[str] = Field(
-            description="Name of a layer with data to be rasterized in a multi-layer file."
+        raster_shape: Optional[Tuple[int, int]] = Field(
+            description="Shape of resulting raster image. Cannot be used with `resolution`."
         )
-        columns: List[VectorColumnSchema]
+        _check_shape_resolution = ensure_exactly_one_defined("resolution", "raster_shape")
+
+        dtype: np.dtype = Field(np.dtype("int32"), description="Numpy dtype of the output feature.")
+        _parse_dtype = field_validator("dtype", parse_dtype, pre=True)
+
         preprocess_dataset: Optional[Preprocessing] = Field(
-            description=(
-                "Parameters used by self.preprocess_dataset method. If set to `None` it skips the dataframe preprocess"
-                " step."
-            )
+            description="Parameters used by `self.preprocess_dataset` method. Skipped if set to `None`."
         )
+        dataset_layer: Optional[str] = Field(
+            description="In case of multi-layer files, name of the layer with data to be rasterized."
+        )
+        polygon_buffer: float = Field(
+            0, description="The size of polygon buffering to be applied before rasterization."
+        )
+        overlap_value: Optional[float] = Field(description="Value to write over the areas where polygons overlap.")
+        no_data_value: int = Field(0, description="The no_data_value argument to be passed to VectorToRasterTask")
         compress_level: int = Field(1, description="Level of compression used in saving EOPatches")
 
+        @validator("vector_input")
+        def _check_vector_input(cls, vector_input: Union[Feature, str]) -> Union[Feature, str]:
+            if isinstance(vector_input, str):
+                assert vector_input.lower().endswith(
+                    (".geojson", ".shp", ".gpkg", ".gdb")
+                ), f"Input file path {vector_input} should be a GeoJSON, Shapefile, GeoPackage or GeoDataBase."
+            else:
+                assert vector_input[0].is_vector(), "Only vector-like input features are allowed!"
+            return vector_input
+
+        @validator("output_feature")
+        def _check_temporal_nature_match(cls, output_feature: Feature, values: Dict[str, Any]) -> Feature:
+            assert output_feature[0].is_image(), "Only image-like output features are allowed!"
+
+            vector_input = values.get("vector_input")
+            if vector_input and not isinstance(vector_input, str):
+                assert (
+                    vector_input[0].is_temporal() == output_feature[0].is_temporal()
+                ), "Temporal natures of the vector input and the raster output must match!"
+            return output_feature
+
     config: Schema
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
         self.filename: Optional[str] = None
+        self.vector_feature: Feature
 
-        if len({c.output_feature[0].is_temporal() for c in self.config.columns}) != 1:
-            raise ValueError("All output features have to be either temporal or timeless!")
-
-        if isinstance(self.config.vector_input, str):
-            self.filename = self._parse_input_file(self.config.vector_input)
-            output_is_temporal = self.config.columns[0].output_feature[0].is_temporal()
-            feature_type = FeatureType.VECTOR if output_is_temporal else FeatureType.VECTOR_TIMELESS
-            self.vector_feature = feature_type, f"TEMP_{uuid.uuid4().hex}"
-        else:
+        if not isinstance(self.config.vector_input, str):
             self.vector_feature = self.config.vector_input
+        else:
+            ftype = FeatureType.VECTOR if self._is_temporal(self.config.output_feature) else FeatureType.VECTOR_TIMELESS
+            self.filename = self.config.vector_input
+            self.vector_feature = (ftype, f"TEMP_{uuid.uuid4().hex}")
 
     def filter_patch_list(self, patch_list: PatchList) -> PatchList:
         filtered_patch_list = get_patches_with_missing_features(
             self.storage.filesystem,
             self.storage.get_folder(self.config.output_folder_key),
             patch_list,
             self._get_output_features(),
         )
 
         return filtered_patch_list
 
     def run_procedure(self) -> Tuple[List[str], List[str]]:
         if self.filename is not None and self.config.preprocess_dataset is not None:
             self.run_dataset_preprocessing(self.filename, self.config.preprocess_dataset)
+
         return super().run_procedure()
 
     def run_dataset_preprocessing(self, filename: str, preprocess_config: Preprocessing) -> None:
         """Loads datasets, applies preprocessing steps and saves them to a cache folder"""
         LOGGER.info("Preprocessing dataset %s", filename)
         gpd_engine = self.storage.config.geopandas_backend
 
         file_path = fs.path.combine(self.storage.get_input_data_folder(), filename)
         with LocalFile(file_path, mode="r", filesystem=self.storage.filesystem) as local_file:
             dataset_layers = [
                 gpd.read_file(local_file.path, layer=layer, encoding="utf-8", engine=gpd_engine)
                 for layer in fiona.listlayers(local_file.path)
             ]
 
-        dataset_gdf = concat_gdf(dataset_layers, reproject_crs=preprocess_config.reproject_crs)
-
+        reproject_crs = None if preprocess_config.reproject_crs is None else CRS(preprocess_config.reproject_crs)
+        dataset_gdf = concat_gdf(dataset_layers, reproject_crs=reproject_crs)
         dataset_gdf = self.preprocess_dataset(dataset_gdf)
-
         dataset_path = self._get_dataset_path(filename)
+
         with LocalFile(dataset_path, mode="w", filesystem=self.storage.filesystem) as local_file:
             dataset_gdf.to_file(local_file.path, encoding="utf-8", driver="GPKG", engine=gpd_engine)
 
     def build_workflow(self) -> EOWorkflow:
         """Creates workflow that is divided into the following sub-parts:
 
         1. loading data,
@@ -158,32 +162,33 @@
         4. postprocessing steps,
         5. saving results
         """
         if self.filename is not None:
             create_node = EONode(CreateEOPatchTask())
             path = self._get_dataset_path(self.filename)
             import_task = VectorImportTask(
-                self.vector_feature,
+                feature=self.vector_feature,
                 path=path,
                 filesystem=self.storage.filesystem,
                 layer=self.config.dataset_layer,
             )
             data_preparation_node = EONode(import_task, inputs=[create_node])
         else:
+            features = [self.vector_feature, FeatureType.BBOX]
+            if self._is_temporal(self.vector_feature):
+                features.append(FeatureType.TIMESTAMPS)
             input_task = LoadTask(
                 self.storage.get_folder(self.config.input_folder_key),
                 filesystem=self.storage.filesystem,
-                features=[self.vector_feature, FeatureType.BBOX],
+                features=features,
             )
             data_preparation_node = EONode(input_task)
 
         preprocess_node = self.get_prerasterization_node(data_preparation_node)
-
         rasterization_node = self.get_rasterization_node(preprocess_node)
-
         postprocess_node = self.get_postrasterization_node(rasterization_node)
 
         save_task = SaveTask(
             self.storage.get_folder(self.config.output_folder_key),
             filesystem=self.storage.filesystem,
             features=self._get_output_features(),
             overwrite_permission=OverwritePermission.OVERWRITE_FEATURES,
@@ -200,57 +205,50 @@
     def get_prerasterization_node(self, previous_node: EONode) -> EONode:  # pylint: disable=no-self-use
         """Builds node with tasks to be applied after loading vector feature but before rasterization"""
         return previous_node
 
     def get_rasterization_node(self, previous_node: EONode) -> EONode:
         """Builds nodes containing rasterization tasks"""
 
-        rasterization_nodes = [
-            EONode(
-                inputs=[previous_node],
-                task=VectorToRasterTask(
-                    vector_input=self.vector_feature,
-                    raster_feature=column.output_feature,
-                    values_column=column.values_column,
-                    values=column.value,
-                    buffer=column.polygon_buffer,
-                    raster_resolution=column.resolution,
-                    raster_shape=column.raster_shape,
-                    raster_dtype=np.dtype(column.dtype),
-                    no_data_value=column.no_data_value,
-                    overlap_value=column.overlap_value,
-                ),
-            )
-            for column in self.config.columns
-        ]
-
-        if len(rasterization_nodes) == 1:
-            return rasterization_nodes[0]
-        return EONode(MergeEOPatchesTask(), inputs=rasterization_nodes)
+        return EONode(
+            inputs=[previous_node],
+            task=VectorToRasterTask(
+                vector_input=self.vector_feature,
+                raster_feature=self.config.output_feature,
+                values_column=self.config.raster_values_column,
+                values=self.config.raster_value,
+                buffer=self.config.polygon_buffer,
+                raster_resolution=self.config.resolution,
+                raster_shape=self.config.raster_shape,
+                raster_dtype=np.dtype(self.config.dtype),
+                no_data_value=self.config.no_data_value,
+                overlap_value=self.config.overlap_value,
+            ),
+        )
 
     def get_postrasterization_node(self, previous_node: EONode) -> EONode:  # pylint: disable=no-self-use
         """Builds node with tasks to be applied after rasterization"""
         return previous_node
 
-    @staticmethod
-    def _parse_input_file(value: str) -> str:
-        """Checks if given name ends with one of the supported file extensions"""
-        if not value.lower().endswith((".geojson", ".shp", ".gpkg", ".gdb")):
-            raise ValueError(f"Input file path {value} should be a GeoJSON, Shapefile, GeoPackage or GeoDataBase.")
-        return value
-
     def _get_dataset_path(self, filename: str) -> str:
         """Provides a path from where dataset should be loaded into the workflow"""
         if self.config.preprocess_dataset is not None:
             folder = self.storage.get_cache_folder()
             filename = f"preprocessed_{filename}"
             filename = (os.path.splitext(filename))[0] + ".gpkg"
         else:
             folder = self.storage.get_input_data_folder()
 
         return fs.path.combine(folder, filename)
 
     def _get_output_features(self) -> List[FeatureSpec]:
         """Lists all features that are to be saved upon the pipeline completion"""
-        features: List[FeatureSpec] = [FeatureType.BBOX]
-        features.extend(column.output_feature for column in self.config.columns)
+        features: List[FeatureSpec] = [self.config.output_feature, FeatureType.BBOX]
+        if self._is_temporal(self.config.output_feature):
+            features.append(FeatureType.TIMESTAMPS)
+
         return features
+
+    @staticmethod
+    def _is_temporal(feature: Feature) -> bool:
+        f_type, _ = feature
+        return f_type.is_temporal()
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/sampling.py` & `eo_grow-1.5.0/eogrow/pipelines/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import numpy as np
 from pydantic import Field
 
 from eolearn.core import EONode, EOWorkflow, FeatureType, LoadTask, MergeEOPatchesTask, OverwritePermission, SaveTask
 from eolearn.geometry import MorphologicalOperations, MorphologicalStructFactory
 from eolearn.ml_tools import BlockSamplingTask, FractionSamplingTask, GridSamplingTask
 
-from eogrow.utils.validators import ensure_exactly_one_defined
+from eogrow.utils.validators import ensure_exactly_one_defined, ensure_storage_key_presence
 
 from ..core.pipeline import Pipeline
 from ..tasks.common import ClassFilterTask
 from ..types import ExecKwargs, Feature, FeatureSpec, PatchList
 from ..utils.filter import get_patches_with_missing_features
 
 
 class BaseSamplingPipeline(Pipeline, metaclass=abc.ABCMeta):
     """Pipeline to run sampling on EOPatches"""
 
     class Schema(Pipeline.Schema):
         output_folder_key: str = Field(description="The storage manager key pointing to the pipeline output folder.")
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
         apply_to: Dict[str, Dict[FeatureType, List[str]]] = Field(
             description=(
                 "A dictionary defining which features to sample, its structure is "
                 "{folder_key: {feature_type: [feature_name]}}"
             ),
         )
         mask_of_samples_name: Optional[str] = Field(
@@ -90,15 +92,15 @@
                     raise ValueError(f"Only spatial features can be sampled, but found {feature_type}: {feature_names}")
 
                 for feature_name in feature_names:
                     load_features.append((feature_type, feature_name))
 
             load_features.append(FeatureType.BBOX)
             if any(FeatureType(feature_type).is_temporal() for feature_type in features):
-                load_features.append(FeatureType.TIMESTAMP)
+                load_features.append(FeatureType.TIMESTAMPS)
 
             load_task = LoadTask(
                 self.storage.get_folder(folder_name),
                 filesystem=self.storage.filesystem,
                 lazy_loading=True,
                 features=load_features,
             )
@@ -144,15 +146,15 @@
             output_features.append((feature_type, sampled_feature_name))
 
         mask_of_samples_feature = self._get_mask_of_samples_feature()
         if mask_of_samples_feature:
             output_features.append(mask_of_samples_feature)
 
         if any(feature_type.is_temporal() for feature_type, _, _ in features_to_sample):
-            output_features.append(FeatureType.TIMESTAMP)
+            output_features.append(FeatureType.TIMESTAMPS)
         return output_features
 
 
 class BaseRandomSamplingPipeline(BaseSamplingPipeline, metaclass=abc.ABCMeta):  # noqa B024
     """A base class for all sampling pipeline that work on random selection of samples"""
 
     class Schema(BaseSamplingPipeline.Schema):
@@ -250,15 +252,15 @@
         fraction_of_samples: Optional[float] = Field(
             description=(
                 "A percentage of samples to be sampled. Exactly one of parameters fraction_of_samples and "
                 "number_of_samples has to be given."
             )
         )
 
-        _check_fraction_number = ensure_exactly_one_defined("fraction_of_samples", "number_of_samples")
+        _check_fraction_number = ensure_exactly_one_defined("number_of_samples", "fraction_of_samples")
 
     config: Schema
 
     def _get_sampling_node(self, previous_node: EONode) -> EONode:
         """Prepare the sampling task"""
         amount: float = self.config.fraction_of_samples or self.config.number_of_samples  # type: ignore[assignment]
         task = BlockSamplingTask(
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/split_grid.py` & `eo_grow-1.5.0/eogrow/pipelines/split_grid.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from collections import defaultdict
 from typing import Dict, List, Literal, Tuple, Union
 
 import fs
 import geopandas as gpd
 from pydantic import Field
 
-from eolearn.core import EONode, EOWorkflow, FeatureType, LoadTask, OverwritePermission, SaveTask
+from eolearn.core import EONode, EOWorkflow, FeatureType, LoadTask, OverwritePermission
 from sentinelhub import CRS, BBox
 from sentinelhub.geometry import Geometry
 
 from ..core.area.batch import BatchAreaManager
 from ..core.area.utm import UtmZoneAreaManager
 from ..core.pipeline import Pipeline
+from ..tasks.common import SkippableSaveTask
 from ..tasks.spatial import SpatialSliceTask
 from ..types import ExecKwargs, Feature, FeatureSpec
 from ..utils.fs import LocalFile
 from ..utils.grid import split_bbox
+from ..utils.validators import ensure_storage_key_presence
 
 LOGGER = logging.getLogger(__name__)
 
 NamedBBox = Tuple[str, BBox]
 
 
 class SplitGridPipeline(Pipeline):
@@ -32,20 +34,25 @@
     The name of the column with eopatch names is `eopatch_name`.
     """
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(
             description="A storage manager key pointing to the folder where the data will be loaded from."
         )
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         eopatch_output_folder_key: str = Field(
             description="A storage manager key pointing to the folder where the data will be saved."
         )
+        _ensure_eopatch_output_folder_key = ensure_storage_key_presence("eopatch_output_folder_key")
+
         grid_output_folder_key: str = Field(
             description="A storage manager key of where to save the resulting split grid."
         )
+        _ensure_grid_output_folder_key = ensure_storage_key_presence("grid_output_folder_key")
+
         subsplit_grid_filename: str = Field(
             description="Filename of new grid, which can be used in `CustomAreaManager`.", regex=r"^.+\.gpkg$"
         )
         features: List[Feature] = Field(description="Which features will be loaded and adapted to new grid.")
         raise_misaligned: bool = Field(
             True,
             description="Raise an error if spatially splitting the EOPatch produces misalignments.",
@@ -140,15 +147,15 @@
 
         processing_nodes = []
         output_path = self.storage.get_folder(self.config.eopatch_output_folder_key)
         for _ in range(self.config.split_x * self.config.split_y):
             slice_task = SpatialSliceTask(features, raise_misaligned=self.config.raise_misaligned)
             slice_node = EONode(slice_task, inputs=[load_node])
 
-            save_task = SaveTask(
+            save_task = SkippableSaveTask(
                 output_path,
                 filesystem=self.storage.filesystem,
                 features=features,
                 overwrite_permission=OverwritePermission.OVERWRITE_FEATURES,
             )
             save_node = EONode(save_task, inputs=[slice_node])
             processing_nodes.append(save_node)
@@ -156,36 +163,36 @@
         return EOWorkflow.from_endnodes(*processing_nodes)
 
     def get_execution_arguments(  # type: ignore[override]
         self, workflow: EOWorkflow, bbox_splits: List[Tuple[NamedBBox, List[NamedBBox]]]
     ) -> ExecKwargs:
         nodes = workflow.get_nodes()
         load_node = nodes[0]
-        save_nodes = [node for node in nodes if isinstance(node.task, SaveTask)]
+        save_nodes = [node for node in nodes if isinstance(node.task, SkippableSaveTask)]
         slice_nodes = [save_node.inputs[0] for save_node in save_nodes]
 
         exec_args: ExecKwargs = {}
         for (orig_name, _), split_bboxes in bbox_splits:
             patch_args: Dict[EONode, Dict[str, object]] = {load_node: dict(eopatch_folder=orig_name)}
             # Since some bboxes might get filtered out, the remaining slice and save nodes should get None arguments
             split_bboxes_iter = it.chain(split_bboxes, it.repeat((None, None)))
 
             for slice_node, save_node, (subbox_name, subbox) in zip(slice_nodes, save_nodes, split_bboxes_iter):
-                patch_args[slice_node] = dict(bbox=subbox)
+                patch_args[slice_node] = dict(bbox=subbox, skip=(subbox is None))
                 patch_args[save_node] = dict(eopatch_folder=subbox_name)
 
             exec_args[orig_name] = patch_args
 
         return exec_args
 
     def _get_features(self) -> List[FeatureSpec]:
         """Provides features that will be transformed by the pipeline."""
         meta_features = [FeatureType.BBOX]
         if any(f_type.is_temporal() for f_type, _ in self.config.features):
-            meta_features += [FeatureType.TIMESTAMP]
+            meta_features += [FeatureType.TIMESTAMPS]
 
         return self.config.features + meta_features
 
     def save_new_grid(self, bbox_splits: List[Tuple[NamedBBox, List[NamedBBox]]]) -> None:
         """Organizes BBoxes into multiple GeoDataFrames that are then saved as layers of a GPKG file."""
         crs_groups = defaultdict(list)
         for _, new_bboxes in bbox_splits:
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/testing.py` & `eo_grow-1.5.0/eogrow/pipelines/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from eolearn.core import CreateEOPatchTask, EONode, EOWorkflow, MergeEOPatchesTask, OverwritePermission, SaveTask
 
 from ..core.config import RawConfig, recursive_config_join
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
 from ..tasks.testing import DummyRasterFeatureTask, DummyTimestampFeatureTask
 from ..types import ExecKwargs, Feature, PatchList, TimePeriod
-from ..utils.validators import field_validator, parse_dtype, parse_time_period
+from ..utils.validators import ensure_storage_key_presence, field_validator, parse_dtype, parse_time_period
 
 Self = TypeVar("Self", bound="TestPipeline")
 LOGGER = logging.getLogger(__name__)
 
 
 class TestPipeline(Pipeline):
     """Pipeline that just tests if all managers works correctly. It can be used to check if area manager creates a
@@ -82,14 +82,16 @@
 
 
 class DummyDataPipeline(Pipeline):
     """Pipeline for generating dummy data."""
 
     class Schema(Pipeline.Schema):
         output_folder_key: str = Field(description="The storage manager key pointing to the pipeline output folder.")
+        _ensure_output_folder_key = ensure_storage_key_presence("output_folder_key")
+
         seed: Optional[int] = Field(description="A randomness seed.")
 
         raster_features: List[RasterFeatureSchema] = Field(
             default_factory=list, description="A list of raster features to be generated."
         )
         timestamp_feature: Optional[TimestampFeatureSchema]
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/training.py` & `eo_grow-1.5.0/eogrow/pipelines/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     recall_score,
 )
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 
 from ..core.pipeline import Pipeline
 from ..core.schemas import BaseSchema
+from ..utils.validators import ensure_storage_key_presence
 
 LOGGER = logging.getLogger(__name__)
 
 
 class RandomTrainTestSplitSchema(BaseSchema):
     random_state: int = Field(
         42,
@@ -41,17 +42,19 @@
 
     This class has a few abstract methods which have to be implemented. But in general all public methods are designed
     in a way that you can override them in a child class
     """
 
     class Schema(Pipeline.Schema):
         input_folder_key: str = Field(description="The storage manager key pointing to the model training data.")
+        _ensure_input_folder_key = ensure_storage_key_presence("input_folder_key")
         model_folder_key: str = Field(
             description="The storage manager key pointing to the folder where the model will be saved."
         )
+        _ensure_model_folder_key = ensure_storage_key_presence("model_folder_key")
 
         train_features: List[str] = Field(
             description="A list of feature filenames to join into training features in the given order."
         )
 
         train_reference: str = Field(description="Name of file where the reference data is stored.")
```

### Comparing `eo-grow-1.4.0/eogrow/pipelines/zipmap.py` & `eo_grow-1.5.0/eogrow/pipelines/zipmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from ..utils.meta import import_object
 
 LOGGER = logging.getLogger(__name__)
 
 
 class InputFeatureSchema(BaseSchema):
     feature: Feature = Field(description="Which features to load from folder.")
-    folder_key: str = Field("The storage manager key pointing to the folder from which to load data.")
+    folder_key: str = Field(description="The storage manager key pointing to the folder from which to load data.")
     include_bbox_and_timestamp = Field(
         True,
         description="Auto loads BBOX and (if the features is temporal) TIMESTAMP.",
     )
 
 
 class ZipMapPipeline(Pipeline):
@@ -88,15 +88,15 @@
         for input_feature in self.config.input_features:
             features_to_load = load_schema[input_feature.folder_key]
             features_to_load.add(input_feature.feature)
 
             if input_feature.include_bbox_and_timestamp:
                 features_to_load.add(FeatureType.BBOX)
                 if input_feature.feature[0].is_temporal():
-                    features_to_load.add(FeatureType.TIMESTAMP)
+                    features_to_load.add(FeatureType.TIMESTAMPS)
 
         load_nodes = []
         for folder_key, features in load_schema.items():
             folder_path = self.storage.get_folder(folder_key, full_path=True)
             load_nodes.append(
                 EONode(LoadTask(folder_path, config=self.sh_config, features=list(features), lazy_loading=True))
             )
@@ -120,14 +120,14 @@
 
         mapping_node = self.get_zipmap_node(merge_node)
 
         save_path = self.storage.get_folder(self.config.output_folder_key, full_path=True)
         save_task = SaveTask(
             save_path,
             config=self.sh_config,
-            features=[self.config.output_feature, FeatureType.BBOX, FeatureType.TIMESTAMP],
+            features=[self.config.output_feature, FeatureType.BBOX, FeatureType.TIMESTAMPS],
             compress_level=self.config.compress_level,
             overwrite_permission=OverwritePermission.OVERWRITE_FEATURES,
         )
         save_node = EONode(save_task, inputs=[mapping_node])
 
         return EOWorkflow.from_endnodes(save_node)
```

### Comparing `eo-grow-1.4.0/eogrow/tasks/batch_to_eopatch.py` & `eo_grow-1.5.0/eogrow/tasks/batch_to_eopatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         userdata = self._load_userdata_file(folder)
 
         if self.userdata_feature_name:
             eopatch.meta_info[self.userdata_feature_name] = userdata
 
         if self.userdata_timestamp_reader:
-            eopatch.timestamp = self._parse_timestamps(userdata, self.userdata_timestamp_reader)
+            eopatch.timestamps = self._parse_timestamps(userdata, self.userdata_timestamp_reader)
 
         return eopatch
 
 
 class FixImportedTimeDependentFeatureTask(EOTask):
     """Fixes a time-dependent feature that has been imported as a timeless feature from batch results.
 
@@ -95,23 +95,23 @@
         """Fixes a feature in the given EOPatch"""
         data = eopatch[self.input_feature]
         del eopatch[self.input_feature]
 
         data = data[np.newaxis, ...]
         data = np.swapaxes(data, 0, -1)
 
-        if eopatch.timestamp:
-            timeframe_num = len(eopatch.timestamp)
+        if eopatch.timestamps:
+            timeframe_num = len(eopatch.timestamps)
             if data.shape[0] != timeframe_num:  # Handling a case where data would contain some empty timeframes
                 data = data[:timeframe_num, ...]
 
-            order_mask = np.argsort(eopatch.timestamp)  # type: ignore[arg-type]
+            order_mask = np.argsort(eopatch.timestamps)  # type: ignore[arg-type]
             is_strictly_increasing = (np.diff(order_mask) > 0).all()
             if not is_strictly_increasing:
-                eopatch.timestamp = sorted(eopatch.timestamp)
+                eopatch.timestamps = sorted(eopatch.timestamps)
                 data = data[order_mask]
 
         eopatch[self.output_feature] = data
         return eopatch
 
 
 class DeleteFilesTask(EOTask):
```

### Comparing `eo-grow-1.4.0/eogrow/tasks/common.py` & `eo_grow-1.5.0/eogrow/tasks/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Common tasks shared between pipelines."""
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 
-from eolearn.core import EOPatch, EOTask
+from eolearn.core import EOPatch, EOTask, SaveTask
+from eolearn.core.utils.parsing import parse_renamed_feature
 from eolearn.geometry import MorphologicalOperations
 
 from ..types import Feature
 
 
 class ClassFilterTask(EOTask):
     """Run class specific morphological operation."""
@@ -24,15 +25,15 @@
         :param feature: Feature to be modified
         :param labels: List of labels to be considered for morphological operation
         :param morph_operation: Type of morphological operation ot perform
         :param struct_elem: Structured element to be used. Taken from `ml_tools.MorphologicalStructFactory`
         """
         self.feature_name: Optional[str]
         self.new_feature_name: Optional[str]
-        self.renamed_feature = self.parse_renamed_feature(feature)
+        self.renamed_feature = parse_renamed_feature(feature)
         self.labels = labels
 
         if isinstance(morph_operation, MorphologicalOperations):
             self.morph_operation = MorphologicalOperations.get_operation(morph_operation)
         else:
             self.morph_operation = morph_operation
         self.struct_elem = struct_elem
@@ -45,7 +46,16 @@
             label_mask = np.squeeze((mask == label), axis=-1)
             mask_mod = self.morph_operation(label_mask, self.struct_elem) * label
             mask_mod = mask_mod[..., np.newaxis]
             mask[mask == label] = mask_mod[mask == label]
 
         eopatch[(feature_type, new_feature_name)] = mask
         return eopatch
+
+
+class SkippableSaveTask(SaveTask):
+    """Same as `SaveTask` but can be skipped if the `eopatch_folder` is set to `None`."""
+
+    def execute(self, eopatch: EOPatch, *, eopatch_folder: Optional[str] = "") -> EOPatch:
+        if eopatch_folder is None:
+            return eopatch
+        return super().execute(eopatch, eopatch_folder=eopatch_folder)
```

### Comparing `eo-grow-1.4.0/eogrow/tasks/features.py` & `eo_grow-1.5.0/eogrow/tasks/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import abc
 from datetime import date, datetime, time, timedelta
 from typing import List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from eolearn.core import EOPatch, EOTask, FeatureType, MapFeatureTask
+from eolearn.core.utils.parsing import parse_renamed_feature
 
 from ..types import Feature
 
 
 def join_valid_and_cloud_masks(valid_mask: np.ndarray, cloud_mask: np.ndarray) -> np.ndarray:
     """Used to zip together information about valid data and clouds into a combined validity mask"""
     return valid_mask.astype(bool) & (cloud_mask == 0)
@@ -43,15 +44,15 @@
     def __init__(
         self,
         feature: Feature,
         dates: Union[List[date], Tuple[date, date, int]],
         valid_mask: Optional[Feature] = None,
         ndvi_feature: Optional[Feature] = None,
     ):
-        self.parsed_feature = self.parse_renamed_feature(feature, allowed_feature_types={FeatureType.DATA})
+        self.parsed_feature = parse_renamed_feature(feature, allowed_feature_types={FeatureType.DATA})
         self.valid_mask_type, self.valid_mask_name = None, None
         if valid_mask is not None:
             self.valid_mask_type, self.valid_mask_name = self.parse_feature(
                 valid_mask, allowed_feature_types={FeatureType.MASK}
             )
         self.ndvi_feature_type, self.ndvi_feature_name = None, None
         if ndvi_feature is not None:
@@ -113,18 +114,18 @@
         """Computes mosaic"""
         return np.array([self._compute_single_mosaic(eopatch, idate) for idate in range(1, len(self.dates))])
 
     def execute(self, eopatch: EOPatch) -> EOPatch:
         """Compute mosaic for given dates"""
         feature_type, _, new_feature_name = self.parsed_feature
 
-        eopatch.timestamp = [ts.replace(tzinfo=None) for ts in eopatch.timestamp]
+        eopatch.timestamps = [ts.replace(tzinfo=None) for ts in eopatch.timestamps]
         eopatch[(feature_type, new_feature_name)] = self.compute_mosaic(eopatch)
 
-        eopatch.timestamp = list(self.compute_mosaic_dates())
+        eopatch.timestamps = list(self.compute_mosaic_dates())
 
         return eopatch
 
 
 class MaxNDVIMosaickingTask(MosaickingTask):
     """
     Task to create mosaics of data based on the max NDVI value between provided dates
@@ -137,15 +138,15 @@
         ndvi_feature: Feature,
         valid_mask: Optional[Feature] = None,
     ):
         super().__init__(feature, dates, ndvi_feature=ndvi_feature, valid_mask=valid_mask)
 
     def _compute_single_mosaic(self, eopatch: EOPatch, idate: int) -> np.ndarray:
         """Compute single mosaic using values of the max NDVI"""
-        array = self._find_time_indices(eopatch.timestamp, idate)
+        array = self._find_time_indices(eopatch.timestamps, idate)
         feature_type, feature_name, _ = self.parsed_feature
         feat_values = eopatch[(feature_type, feature_name)][array].astype(np.float32)
         ndvi_values = eopatch[(self.ndvi_feature_type, self.ndvi_feature_name)][array]  # type: ignore[index]
         valid_mask = (
             eopatch[self.valid_mask_type][self.valid_mask_name][array]
             if self.valid_mask_type is not None
             else np.ones(feat_values.shape, dtype=bool)
@@ -185,15 +186,15 @@
         dates: Union[List[date], Tuple[date, date, int]],
         valid_mask: Optional[Feature] = None,
     ):
         super().__init__(feature, dates, valid_mask=valid_mask)
 
     def _compute_single_mosaic(self, eopatch: EOPatch, idate: int) -> np.ndarray:
         """Compute single mosaic using the median of values"""
-        array = self._find_time_indices(eopatch.timestamp, idate)
+        array = self._find_time_indices(eopatch.timestamps, idate)
         feature_type, feature_name, _ = self.parsed_feature
 
         feat_values = eopatch[(feature_type, feature_name)][array].astype(np.float32)
         valid_mask = (
             eopatch[(self.valid_mask_type, self.valid_mask_name)][array]
             if self.valid_mask_type is not None
             else np.ones(feat_values.shape, dtype=bool)
```

### Comparing `eo-grow-1.4.0/eogrow/tasks/prediction.py` & `eo_grow-1.5.0/eogrow/tasks/prediction.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/tasks/spatial.py` & `eo_grow-1.5.0/eogrow/tasks/spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
             data = [eopatch[feature] for eopatch in eopatches if feature in eopatch]
             if not data:
                 continue
 
             if feature_type.is_spatial():
                 feature = cast(Feature, feature)  # bbox and timestamp are discarded with above check
-                if feature_type.is_raster():
+                if feature_type.is_array():
                     bboxes: List[BBox] = [patch.bbox for patch in eopatches if feature in patch]  # type: ignore[misc]
                     joined_data = self._join_spatial_rasters(data, bboxes, bbox, self.no_data_map[feature])
                 else:
                     joined_data = self._join_vector_data(data, self.unique_columns_map.get(feature))
             else:
                 joined_data = data[0]
 
@@ -156,42 +156,39 @@
     @staticmethod
     def _filter_vector(gdf: GeoDataFrame, bbox: BBox) -> GeoDataFrame:
         """Spatially filters a GeoDataFrame."""
         bbox = bbox.transform(CRS(gdf.crs))
         intersects_bbox = gdf.geometry.intersects(bbox.geometry)
         return gdf[intersects_bbox].copy(deep=True)
 
-    def execute(self, eopatch: EOPatch, *, bbox: Optional[BBox]) -> EOPatch:
+    def execute(self, eopatch: EOPatch, *, bbox: BBox, skip: bool = False) -> EOPatch:
         """Spatially slices given EOPatch with given bounding box.
 
-        The task allows that no bounding box for slicing is provided. In such case the task will return an EOPatch with
-        only non-spatial features.
-        """
+        Can be skipped in cases where the subbox won't be saved."""
+        if skip:
+            return eopatch
+
         main_bbox = eopatch.bbox
         if not main_bbox:
             raise ValueError("EOPatch is missing a bounding box")
-        if bbox is not None:
-            if main_bbox.crs is not bbox.crs:
-                raise ValueError("Given bbox is not in the same CRS as EOPatch bbox")
-            if not main_bbox.geometry.contains(bbox.geometry):
-                raise ValueError("Given bbox must be fully contained in EOPatch's bbox")
+        if main_bbox.crs is not bbox.crs:
+            raise ValueError("Given bbox is not in the same CRS as EOPatch bbox")
+        if not main_bbox.geometry.contains(bbox.geometry):
+            raise ValueError("Given bbox must be fully contained in EOPatch's bbox")
 
         sliced_eopatch = EOPatch(bbox=bbox)
 
         for feature in self.features:
             feature_type, _ = feature
             if feature_type is FeatureType.BBOX:
                 continue
             data = eopatch[feature]
 
             if feature_type.is_spatial():
-                if bbox is None:
-                    continue
-
-                if feature_type.is_raster():
+                if feature_type.is_array():
                     sliced_data = self._slice_raster(data, main_bbox, bbox)
                 else:
                     sliced_data = self._filter_vector(data, bbox)
             else:
                 sliced_data = data
 
             sliced_eopatch[feature] = sliced_data
@@ -212,18 +209,18 @@
     """Slicing taken from eolearn.io.ImportFromTiffTask.
 
     :param bbox: A bounding box of initial array.
     :param slice_bbox: A bounding box of array to be sliced.
     :param resolution: A working resolution in CRS units.
     :param size: A working size.
     :param raise_misaligned: Whether to raise an error if the slice would be pixel misaligned the initial array.
-    :param limit_x: If provided it will clip the horizontal slice to a given interval, should be used to clip slice_bbox
-    to bbox.
+    :param limit_x: If provided it will clip the horizontal slice to a given interval, should be used to clip
+        slice_bbox to bbox.
     :param limit_y: If provided it will clip the vertical slice to a given interval, should be used to clip slice_bbox
-    to bbox.
+        to bbox.
     :return: A slice over horizontal direction and a slice over vertical direction.
     """
     raster_upper_left = np.array([bbox.min_x, bbox.max_y])
 
     if size is not None and resolution is None:
         width, height = size
         raster_lower_right = np.array([bbox.max_x, bbox.min_y])
```

### Comparing `eo-grow-1.4.0/eogrow/tasks/testing.py` & `eo_grow-1.5.0/eogrow/tasks/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tasks used to generate test data."""
 import datetime as dt
 from typing import Optional, Tuple, Union
 
 import numpy as np
 
-from eolearn.core import EOPatch, EOTask, FeatureTypeSet
+from eolearn.core import EOPatch, EOTask
 from eolearn.core.utils.common import is_discrete_type
 
 from ..types import Feature, TimePeriod
 
 
 class DummyRasterFeatureTask(EOTask):
     """Creates a raster feature with random values"""
@@ -25,15 +25,15 @@
         :param feature: A raster feature to be created.
         :param shape: Shape of the created feature array.
         :param dtype: A dtype of the feature.
         :param min_value: All feature values will be greater or equal to this value.
         :param max_value: If feature has a discrete dtype or max_value == min_value then all feature values will be
             lesser or equal to this value. Otherwise, all features will be strictly lesser to this value.
         """
-        self.feature = self.parse_feature(feature, allowed_feature_types=FeatureTypeSet.RASTER_TYPES)
+        self.feature = self.parse_feature(feature, allowed_feature_types=lambda fty: fty.is_array())
         self.shape = shape
         self.dtype = dtype
         self.min_value = min_value
         self.max_value = max_value
 
         feature_type, _ = self.feature
         if len(self.shape) != feature_type.ndim():
@@ -53,17 +53,16 @@
                 int(self.min_value), int(self.max_value), size=self.shape, dtype=self.dtype, endpoint=True
             )
 
         array = rng.random(size=self.shape)
         array = (self.max_value - self.min_value) * array + self.min_value
         return array.astype(self.dtype)
 
-    def execute(self, eopatch: Optional[EOPatch] = None, seed: Optional[int] = None) -> EOPatch:
+    def execute(self, eopatch: EOPatch, seed: Optional[int] = None) -> EOPatch:
         """Generates a raster feature randomly with a given seed."""
-        eopatch = eopatch or EOPatch()
         rng = np.random.default_rng(seed)
 
         eopatch[self.feature] = self._get_random_raster(rng)
         return eopatch
 
 
 class DummyTimestampFeatureTask(EOTask):
@@ -73,26 +72,25 @@
         """
         :param time_interval: A time interval `[start, end)` from where all timestamps will be generated.
         :param timestamp_num: Number of timestamp in the created timestamp feature.
         """
         self.time_interval = tuple(map(_ensure_datetime, time_interval))
         self.timestamp_num = timestamp_num
 
-    def execute(self, eopatch: Optional[EOPatch] = None, seed: Optional[int] = None) -> EOPatch:
+    def execute(self, eopatch: EOPatch, seed: Optional[int] = None) -> EOPatch:
         """Generates timestamps randomly with a given seed."""
-        eopatch = eopatch or EOPatch()
         rng = np.random.default_rng(seed)
 
         start_time, end_time = self.time_interval
         total_seconds = int((end_time - start_time).total_seconds())
         random_integers = rng.integers(total_seconds, size=self.timestamp_num)
         random_integers.sort()
         timestamps = [start_time + dt.timedelta(seconds=int(seconds)) for seconds in random_integers]
 
-        eopatch.timestamp = timestamps
+        eopatch.timestamps = timestamps
         return eopatch
 
 
 def _ensure_datetime(timestamp: dt.date) -> dt.datetime:
     """Ensures that the given timestamp is a datetime and not a date object."""
     if isinstance(timestamp, dt.datetime):
         return timestamp
```

### Comparing `eo-grow-1.4.0/eogrow/types.py` & `eo_grow-1.5.0/eogrow/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,23 +23,12 @@
 FeatureSpec: TypeAlias = Union[Tuple[FeatureType, str], FeatureType]
 
 BoolOrAuto: TypeAlias = Union[Literal["auto"], bool]
 
 JsonDict: TypeAlias = Dict[str, Any]
 RawSchemaDict: TypeAlias = Dict[str, Any]
 
-AwsAclType: TypeAlias = Literal[
-    "private",
-    "public-read",
-    "public-read-write",
-    "aws-exec-read",
-    "authenticated-read",
-    "bucket-owner-read",
-    "bucket-owner-full-control",
-    "log-delivery-write",
-]
-
 
 class ProcessingType(Enum):
     RAY = "ray"
     SINGLE = "single"
     MULTI = "multi"
```

### Comparing `eo-grow-1.4.0/eogrow/utils/batch.py` & `eo_grow-1.5.0/eogrow/utils/batch.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/utils/eopatch_list.py` & `eo_grow-1.5.0/eogrow/utils/eopatch_list.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/utils/filter.py` & `eo_grow-1.5.0/eogrow/utils/filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 """
 Utilities for filtering eopatch lists
 """
 from concurrent.futures import ThreadPoolExecutor
-from typing import Sequence, Set, Tuple, Union
+from typing import Sequence
 
 import fs
 from fs.base import FS
 from tqdm.auto import tqdm
 
 from eolearn.core import FeatureType
-from eolearn.core.eodata_io import walk_filesystem
-from eolearn.core.types import EllipsisType
+from eolearn.core.eodata_io import FilesystemDataInfo, get_filesystem_data_info
 
 from ..types import FeatureSpec, PatchList
 
 
 def check_if_features_exist(
     filesystem: FS,
     eopatch_path: str,
     features: Sequence[FeatureSpec],
 ) -> bool:
     """Checks whether an EOPatch in the given location has all specified features saved"""
-    not_seen_features: Set[Union[FeatureType, Tuple[FeatureType, Union[str, EllipsisType]]]] = set(features)
     try:
-        for ftype, name, _ in walk_filesystem(filesystem, eopatch_path, features=features):
-            if (ftype, name) in not_seen_features:
-                not_seen_features.remove((ftype, name))
-            elif ftype in not_seen_features:
-                not_seen_features.remove(ftype)
+        existing_data = get_filesystem_data_info(filesystem, eopatch_path, features)
+        meta_features = [spec for spec in features if isinstance(spec, FeatureType)]
+        regular_features = [spec for spec in features if isinstance(spec, tuple)]
+
+        if not all(_check_if_meta_feature_exists(ftype, existing_data) for ftype in meta_features):
+            return False
+
+        for ftype, fname in regular_features:
+            if ftype == FeatureType.META_INFO:
+                raise ValueError("Cannot check for a specific meta-info feature!")
+            if ftype not in existing_data.features or fname not in existing_data.features[ftype]:
+                return False
+        return True
+
     except (IOError, fs.errors.ResourceNotFound):
         return False
-    return len(not_seen_features) == 0
+
+
+def _check_if_meta_feature_exists(ftype: FeatureType, existing_data: FilesystemDataInfo) -> bool:
+    if ftype == FeatureType.BBOX and existing_data.bbox is None:
+        return False
+    if ftype == FeatureType.TIMESTAMPS and existing_data.timestamps is None:
+        return False
+    if ftype == FeatureType.META_INFO and existing_data.meta_info is None:
+        return False
+    return True
 
 
 def get_patches_with_missing_features(
     filesystem: FS,
     patches_folder: str,
     patch_list: PatchList,
     features: Sequence[FeatureSpec],
```

### Comparing `eo-grow-1.4.0/eogrow/utils/fs.py` & `eo_grow-1.5.0/eogrow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/utils/general.py` & `eo_grow-1.5.0/eogrow/utils/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A module containing general utilities that haven't been sorted in any other module
 """
 import datetime as dt
-import math
 from enum import Enum
-from typing import Tuple, Union
+from typing import Union
 
 import numpy as np
 
 from sentinelhub import BBox, DataCollection
 from sentinelhub.data_collections import DataCollectionDefinition
 
 
@@ -27,20 +26,14 @@
 
     if isinstance(param, Enum):
         return param.value
 
     raise TypeError(f"Object of type {type(param)} is not yet supported in jsonify utility function")
 
 
-def reduce_to_coprime(number1: int, number2: int) -> Tuple[int, int]:
-    """Divides given numbers by their greatest common divisor, thus making them coprime."""
-    gcd = math.gcd(number1, number2)
-    return number1 // gcd, number2 // gcd
-
-
 def convert_to_int(values: np.ndarray, raise_diff: bool, error: float = 1e-8) -> np.ndarray:
     """Converts an array of floats into array of integers.
 
     :param values: An array of float values to be converted.
     :param raise_diff: Whether to raise an error if float values differ from integer values for more than the expected
         error.
     :param error: A joined maximal expected numerical error.
@@ -58,19 +51,24 @@
     return rounded_values.astype(int)
 
 
 def convert_bbox_coords_to_int(bbox: BBox, error: float = 1e-8) -> BBox:
     """Converts bounding box coordinates to integers by removing numerical errors. If the difference is larger than a
     numerical error it raises an error."""
     coords = np.array(list(bbox))
-    fixed_coords = convert_to_int(coords, raise_diff=True, error=error)
-    return BBox(tuple(fixed_coords), crs=bbox.crs)
+    min_x, min_y, max_x, max_y = convert_to_int(coords, raise_diff=True, error=error)
+    return BBox((min_x, min_y, max_x, max_y), crs=bbox.crs)
 
 
 def large_list_repr(large_list: list) -> str:
     """Creates a representation of a large list of elements that consists only of a representation of first 3 and the
     last element."""
     if len(large_list) <= 4:
         return repr(large_list)
 
     first_elements = ", ".join(map(repr, large_list[:3]))
     return f"[{first_elements}, ..., {large_list[-1]}]"
+
+
+def current_timestamp(fmt: str = "%Y-%m-%dT%H-%M-%SZ") -> str:
+    """Creates a timestamp string of the current time"""
+    return dt.datetime.utcnow().strftime(fmt)
```

### Comparing `eo-grow-1.4.0/eogrow/utils/grid.py` & `eo_grow-1.5.0/eogrow/utils/grid.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/utils/logging.py` & `eo_grow-1.5.0/eogrow/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eo-grow-1.4.0/eogrow/utils/map.py` & `eo_grow-1.5.0/eogrow/utils/map.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """
 Module with utilities for creating maps
 """
 import logging
 import os
 import shutil
 import subprocess
+import tempfile
 import warnings
+from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Iterable, Literal, Optional
 
+SH_COMMAND_LIMIT = 130000
+OPEN_FILES_LIMIT = 1000
+
+
 LOGGER = logging.getLogger(__name__)
 
 GDAL_DTYPE_SETTINGS = {
     "uint8": "Byte",
     "uint16": "UInt16",
     "int16": "Int16",
     "float32": "Float32",
@@ -42,14 +48,15 @@
     blocksize: int = 2048,
     nodata: Optional[float] = None,
     dtype: Literal[None, "int8", "int16", "uint8", "uint16", "float32"] = None,
     resampling: CogifyResamplingOptions = None,
     quiet: bool = True,
 ) -> None:
     """Make the (geotiff) file a cog
+
     :param tiff_file: .tiff file to cogify
     :param blocksize: block size of tiled COG
     :param nodata: value to be treated as nodata, default value is None
     :param dtype: output type of the in the resulting tiff, default is None
     :param resampling: The resampling method used to produce overviews. The defaults (when using None) are CUBIC for
         floats and NEAREST for integers.
     :param quiet: The process does not produce logs.
@@ -128,14 +135,15 @@
     if version < "3.6.0" and resampling == "MODE":
         warnings.warn(
             (
                 "GDAL versions below 3.6.0 have issues with `MODE` overview resampling. Trying to fix issue by setting"
                 " GDAL_OVR_CHUNK_MAX_SIZE to a large integer (2100000000)."
             ),
             category=RuntimeWarning,
+            stacklevel=2,
         )
         gdaltranslate_options += " --config GDAL_OVR_CHUNK_MAX_SIZE 2100000000"
 
     subprocess.check_call(f"gdal_translate {gdaltranslate_options} {input_file} {output_file}", shell=True)
 
 
 def merge_tiffs(
@@ -170,16 +178,35 @@
 
     if nodata is not None:
         gdalwarp_options += f' -dstnodata "{nodata}"'  # noqa B028
 
     if dtype is not None:
         gdalwarp_options += f" -ot {GDAL_DTYPE_SETTINGS[dtype]}"
 
-    command = f"gdalwarp {gdalwarp_options} {' '.join(input_filenames)} {merged_filename}"
-    subprocess.check_call(command, shell=True)
+    input_filelist = list(input_filenames)
+    command = f"gdalwarp {gdalwarp_options} {' '.join(input_filelist)} {merged_filename}"
+
+    if len(command) > SH_COMMAND_LIMIT or len(input_filelist) > OPEN_FILES_LIMIT:
+        merged_path = Path(merged_filename)
+        vrt_file_path = merged_path.with_name(f"{merged_path.stem}_temp.vrt")
+        LOGGER.info(f"Command too big or too many files to process. Creating an intermediary vrt: {vrt_file_path}")
+        # generate text file with tile names & generate vrt
+        with tempfile.NamedTemporaryFile(mode="w", delete=True) as file_list:
+            file_list.writelines([f"{tname}\n" for tname in input_filelist])
+            generate_vrt_command = f"gdalbuildvrt {vrt_file_path} -input_file_list {file_list.name}"
+            subprocess.check_call(generate_vrt_command, shell=True)
+
+        # create merged file
+        command = f"gdalwarp {gdalwarp_options} {vrt_file_path} {merged_filename}"
+        subprocess.check_call(command, shell=True)
+
+        # cleanup the vrt after the process
+        os.remove(vrt_file_path)
+    else:
+        subprocess.check_call(command, shell=True)
 
 
 def extract_bands(
     input_file: str,
     output_file: str,
     bands: Iterable[int],
     overwrite: bool = True,
```

### Comparing `eo-grow-1.4.0/eogrow/utils/meta.py` & `eo_grow-1.5.0/eogrow/utils/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Utilities for solving different problems in `eo-grow` package structure, which are mostly a pure Python magic.
 """
 from __future__ import annotations
 
 import importlib
-import inspect
 import re
 from typing import TYPE_CHECKING, Any, Dict, Type
 
 from packaging.requirements import Requirement
 
 if TYPE_CHECKING:
     from ..core.pipeline import Pipeline
@@ -23,32 +22,30 @@
     if pipeline_class_name is None:
         raise ValueError(f"Config file is missing `{_PIPELINE_PARAM_NAME}` parameter, don't know which pipeline to use")
 
     pipeline_class = import_object(pipeline_class_name)
     return pipeline_class
 
 
-def collect_schema(object_with_schema: Any) -> Type[BaseSchema]:
+def collect_schema(class_with_schema: Type) -> Type[BaseSchema]:
     """A utility that collects a schema from the given object.
 
     The object is expected to hold a unique internal class which inherits from `BaseSchema`. Example:
 
     class MyObject:
         class Schema(BaseSchema):
             ...
 
     This utility would provide `MySchema`. It works also if `MyObject` inherits from a class that holds the schema.
     """
-    class_with_schema = object_with_schema if inspect.isclass(object_with_schema) else object_with_schema.__class__
-
     try:
         return class_with_schema.Schema
     except AttributeError as exception:
         raise SyntaxError(
-            f"Class {class_with_schema} is missing a schema. Each EOGrowObject class needs to contain a pydantic "
+            f"Class {class_with_schema} is missing a schema. Each `EOGrowObject` class needs to contain a pydantic "
             "model named `Schema`."
         ) from exception
 
 
 def import_object(import_path: str) -> Any:
     """Imports an object from a given import path"""
     if "." not in import_path:
```

### Comparing `eo-grow-1.4.0/eogrow/utils/testing.py` & `eo_grow-1.5.0/eogrow/utils/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Module implementing utilities for unit testing pipeline results
 """
-import functools
 import json
 import os
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, cast
 
 import fs
 import numpy as np
 import pandas as pd
 import rasterio
 import shapely.ops
 from deepdiff import DeepDiff
 from fs.base import FS
+from fs.osfs import OSFS
 
 from eolearn.core import EOPatch, FeatureType
+from eolearn.core.eodata_io import get_filesystem_data_info
 from sentinelhub import BBox
 
 from ..core.config import collect_configs_from_path, interpret_config_from_dict
 from ..core.pipeline import Pipeline
 from ..types import JsonDict
 from ..utils.eopatch_list import load_names
 from ..utils.meta import load_pipeline_class
@@ -104,17 +105,17 @@
         if folder is None:
             folder = self.main_folder
 
         for content in self.filesystem.listdir(folder):
             content_path = fs.path.combine(folder, content)
 
             if self.filesystem.isdir(content_path):
-                eopatch = EOPatch.load(content_path, filesystem=self.filesystem)
-
-                if eopatch.bbox:
+                fs_data_info = get_filesystem_data_info(self.filesystem, content_path)
+                if fs_data_info.bbox is not None:
+                    eopatch = EOPatch.load(content_path, filesystem=self.filesystem)
                     stats[content] = self._calculate_eopatch_stats(eopatch)
                 else:  # Probably it is not an EOPatch folder
                     stats[content] = self._calculate_stats(folder=content_path)
             elif content_path.endswith("tiff"):
                 stats[content] = self._calculate_tiff_stats(content_path)
             elif content_path.endswith(".npy"):
                 stats[content] = self._calculate_numpy_file_stats(content_path)
@@ -134,29 +135,30 @@
                 continue
 
             feature_type_name = feature_type.value
 
             if feature_type is FeatureType.BBOX:
                 stats[feature_type_name] = repr(eopatch.bbox)
 
-            elif feature_type is FeatureType.TIMESTAMP:
-                stats[feature_type_name] = [time.isoformat() for time in eopatch.timestamp]
+            elif feature_type is FeatureType.TIMESTAMPS:
+                stats[feature_type_name] = [time.isoformat() for time in eopatch.timestamps]
 
             else:
                 feature_stats_dict = {}
 
-                if feature_type.is_raster():
+                if feature_type.is_array():
                     calculation_method: Callable = self._calculate_numpy_stats
                 elif feature_type.is_vector():
                     calculation_method = self._calculate_vector_stats
                 else:  # Only FeatureType.META_INFO remains
                     calculation_method = str
 
                 for feature_name in eopatch[feature_type]:
-                    feature_stats_dict[feature_name] = calculation_method(eopatch[feature_type][feature_name])
+                    feature_data = eopatch[feature_type, feature_name]
+                    feature_stats_dict[feature_name] = calculation_method(feature_data)
 
                 stats[feature_type_name] = feature_stats_dict
 
         return stats
 
     def _calculate_numpy_stats(self, raster: np.ndarray) -> JsonDict:
         """Calculates statistics over a raster numpy array"""
@@ -215,22 +217,21 @@
         with self.filesystem.openbin(numpy_filename, "r") as file_handle:
             raster = np.load(file_handle, allow_pickle=True)
 
         return self._calculate_numpy_stats(raster)
 
     def _calculate_vector_stats(self, dataframe: pd.DataFrame) -> JsonDict:
         """Calculates statistics over a vector GeoDataFrame"""  # TODO: add more statistical properties
-        rounder = functools.partial(_round_point_coords, decimals=self.decimals)
-        dataframe["geometry"] = dataframe["geometry"].apply(lambda geometry: shapely.ops.transform(rounder, geometry))
 
-        stats = {
-            "columns": list(dataframe),
-            "row_count": len(dataframe.index),
-            "crs": str(dataframe.crs),
-        }
+        def _rounder(x: float, y: float) -> Tuple[float, float]:
+            return round(x, self.decimals), round(y, self.decimals)
+
+        dataframe["geometry"] = dataframe["geometry"].apply(lambda geometry: shapely.ops.transform(_rounder, geometry))
+
+        stats = {"columns": list(dataframe), "row_count": len(dataframe.index), "crs": str(dataframe.crs)}
 
         if len(dataframe.index):
             stats["first_row"] = list(map(str, dataframe.iloc[0]))
 
         return stats
 
     def _calculate_subsample_stats(self, values: np.ndarray, amount: float = 0.1) -> Dict[str, float]:
@@ -294,81 +295,74 @@
     failed_filename = fs.path.combine(logs_folder, "failed.json")
     assert not load_names(pipeline.storage.filesystem, failed_filename), f"Some executions failed, check {logs_folder}"
 
     finished_filename = os.path.join(logs_folder, "finished.json")
     assert load_names(pipeline.storage.filesystem, finished_filename), "No executions finished"
 
 
-def run_and_test_pipeline(
-    experiment_name: str,
+def run_config(
+    config_path: str,
     *,
-    config_folder: str,
-    stats_folder: str,
-    folder_key: Optional[str] = None,
-    reset_folder: bool = True,
-    save_new_stats: bool = False,
-) -> None:
-    """A default way of testing a pipeline
-
-    :param experiment_name: Name of test experiment, which defines its config and stats filenames
-    :param config_folder: A path to folder containing the config file
-    :param stats_folder: A path to folder containing the file with expected result stats
-    :param folder_key: Type of the folder containing results of the pipeline, if missing it's inferred from config
-    :param reset_folder: If True it will delete content of the folder with results before running the pipeline
-    :param save_new_stats: If True then new file with expected result stats will be saved, potentially overwriting the
-        old one. Otherwise, the old one will be used to compare stats.
+    output_folder_key: Optional[str] = None,
+    reset_output_folder: bool = True,
+) -> Optional[str]:
+    """Runs a pipeline (or multiple) and checks the logs that all the executions were successful. Returns the full path
+    of the output folder (if there is one) so it can be inspected further. In case of chain configs, the output folder
+    of the last config is returned.
+
+    :param config_path: A path to the config file
+    :param output_folder_key: Type of the folder containing results of the pipeline, inferred from config if None
+    :param reset_output_folder: Delete the content of the results folder before running the pipeline
     """
-    config_filename = os.path.join(config_folder, experiment_name + ".json")
-    expected_stats_file = os.path.join(stats_folder, experiment_name + ".json")
-
-    crude_configs = collect_configs_from_path(config_filename)
+    crude_configs = collect_configs_from_path(config_path)
     raw_configs = [interpret_config_from_dict(config) for config in crude_configs]
 
-    for index, config in enumerate(raw_configs):
-        output_folder_key = folder_key or config.get("output_folder_key")
-        if output_folder_key is None:
-            raise ValueError(
-                "Pipeline does not have a `output_folder_key` parameter, `folder_key` must be set by hand."
-            )
+    for config in raw_configs:
+        output_folder_key = output_folder_key or config.get("output_folder_key")
 
         pipeline = load_pipeline_class(config).from_raw_config(config)
 
-        folder = pipeline.storage.get_folder(output_folder_key)
-        filesystem = pipeline.storage.filesystem
+        if reset_output_folder:
+            if output_folder_key is None:
+                raise ValueError("Pipeline does not have an `output_folder_key` parameter, it must be set by hand.")
+            folder = pipeline.storage.get_folder(output_folder_key)
+            pipeline.storage.filesystem.removetree(folder)
 
-        if reset_folder:
-            filesystem.removetree(folder)
         pipeline.run()
 
         check_pipeline_logs(pipeline)
 
-        if index < len(raw_configs) - 1:
-            continue
-
-        tester = ContentTester(filesystem, folder)
+    return pipeline.storage.get_folder(output_folder_key, full_path=True) if output_folder_key else None
 
-        if save_new_stats:
-            tester.save(expected_stats_file)
 
-        stats_difference = tester.compare(expected_stats_file)
-        if stats_difference:
-            stats_difference_repr = stats_difference.to_json(indent=2, sort_keys=True)
-            raise AssertionError(f"Expected and obtained stats differ:\n{stats_difference_repr}")
+def compare_content(
+    folder_path: Optional[str],
+    stats_path: str,
+    *,
+    save_new_stats: bool = False,
+) -> None:
+    """Compares the results from a pipeline run with the saved statistics. Constructed to be coupled with `run_config`
+    hence the `Optional` input.
 
+    :param folder_path: A path to the folder with contents to be compared
+    :param stats_path: A path to the file containing result statistics
+    :param save_new_stats: Save new result stats and skip the comparison
+    """
+    if folder_path is None:
+        raise ValueError("The given path is None. The pipeline likely has no `output_folder_key` parameter.")
 
-def _round_point_coords(x: float, y: float, decimals: int) -> Tuple[float, float]:
-    """Rounds coordinates of a point"""
-    return round(x, decimals), round(y, decimals)
+    tester = ContentTester(OSFS("/"), folder_path)
 
+    if save_new_stats:
+        tester.save(stats_path)
 
-def create_folder_dict(config_folder: str, stats_folder: str, subfolder: Optional[str] = None) -> Dict[str, str]:
-    return {
-        "config_folder": os.path.join(config_folder, subfolder) if subfolder else config_folder,
-        "stats_folder": os.path.join(stats_folder, subfolder) if subfolder else config_folder,
-    }
+    stats_difference = tester.compare(stats_path)
+    if stats_difference:
+        stats_difference_repr = stats_difference.to_json(indent=2, sort_keys=True)
+        raise AssertionError(f"Expected and obtained stats differ:\n{stats_difference_repr}")
 
 
 def generate_tiff_file(
     filesystem: FS,
     file_paths: Iterable[str],
     *,
     tiff_bbox: BBox,
```

### Comparing `eo-grow-1.4.0/eogrow/utils/validators.py` & `eo_grow-1.5.0/eogrow/utils/validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Module defining common validators for schemas and validator wrappers
 """
 import datetime as dt
 import inspect
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Tuple, Type, Union
 
 import numpy as np
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field, validator
 
+from eolearn.core import FeatureType
+from eolearn.core.utils.parsing import parse_feature
 from sentinelhub import DataCollection
 from sentinelhub.data_collections_bands import Band, Bands, MetaBands, Unit
 
-from ..types import RawSchemaDict, TimePeriod
+from ..types import Feature, RawSchemaDict, TimePeriod
 from .meta import collect_schema, import_object
 
 if TYPE_CHECKING:
     from ..core.schemas import ManagerSchema
 
 
 def field_validator(field: str, validator_fun: Callable, allow_reuse: bool = True, **kwargs: Any) -> classmethod:
@@ -45,48 +47,67 @@
 
     optional_validator.__name__ = f"optional_{validator_fun.__name__}"  # used for docbuilding purposes
     # the correct way would be to use `functools.wraps` but this breaks pydantics python magic
 
     return validator(field, allow_reuse=allow_reuse, **kwargs)(optional_validator)
 
 
-def validate_s3_path(value: str) -> str:
-    """Validates the prefix of a S3 bucket path"""
-    assert value.startswith("s3://"), "S3 path must start with s3://"
-    return value
+def ensure_exactly_one_defined(first_param: str, second_param: str, **kwargs: Any) -> classmethod:
+    """A validator (applied to `second_param` field) that makes sure only one of the two parameters is defined.
 
+    Make sure that the definition of `second_param` comes after `first_param˙ (in line-order).
+    """
 
-def ensure_exactly_one_defined(param1: str, param2: str, allow_reuse: bool = True, **kwargs: Any) -> classmethod:
-    """A root validator that makes sure only one of the two parameters is defined."""
-
-    def ensure_exclusion(cls: type, values: RawSchemaDict) -> RawSchemaDict:
-        is_param1_defined = values.get(param1) is None
-        is_param2_defined = values.get(param2) is None
+    def ensure_exclusion(cls: type, value: Optional[Any], values: RawSchemaDict) -> Optional[Any]:
+        is_param1_undefined = values.get(first_param) is None
+        is_param2_undefined = value is None
         assert (
-            is_param1_defined != is_param2_defined
-        ), f"Exactly one of parameters `{param1}` and `{param2}` has to be specified."
+            is_param1_undefined != is_param2_undefined
+        ), f"Exactly one of parameters `{first_param}` and `{second_param}` has to be specified."
+
+        return value
 
-        return values
+    ensure_exclusion.__name__ = f"cannot_be_used_with_{first_param}"  # used for docbuilding purposes
 
-    return root_validator(allow_reuse=allow_reuse, **kwargs)(ensure_exclusion)
+    return field_validator(second_param, ensure_exclusion, **kwargs)
 
 
-def ensure_defined_together(param1: str, param2: str, allow_reuse: bool = True, **kwargs: Any) -> classmethod:
-    """A root validator that makes sure that the two parameters are both (un)defined."""
+def ensure_defined_together(first_param: str, second_param: str, **kwargs: Any) -> classmethod:
+    """A validator (applied to `second_param` field) that makes sure that the two parameters are both (un)defined.
+
+    Make sure that the definition of `second_param` comes after `first_param˙ (in line-order).
+    """
 
-    def ensure_exclusion(cls: type, values: RawSchemaDict) -> RawSchemaDict:
-        is_param1_defined = values.get(param1) is None
-        is_param2_defined = values.get(param2) is None
+    def ensure_both(cls: type, value: Optional[Any], values: RawSchemaDict) -> Optional[Any]:
+        is_param1_undefined = values.get(first_param) is None
+        is_param2_undefined = value is None
         assert (
-            is_param1_defined == is_param2_defined
-        ), f"Both or neither of parameters `{param1}` and `{param2}` have to be specified."
+            is_param1_undefined == is_param2_undefined
+        ), f"Both or neither of parameters `{first_param}` and `{second_param}` have to be specified."
+
+        return value
+
+    ensure_both.__name__ = f"must_be_used_with_{first_param}"  # used for docbuilding purposes
+
+    return field_validator(second_param, ensure_both, **kwargs)
 
-        return values
 
-    return root_validator(allow_reuse=allow_reuse, **kwargs)(ensure_exclusion)
+def ensure_storage_key_presence(key: str, **kwargs: Any) -> classmethod:
+    """A field validator that makes sure that the specified storage key is present in the storage structure."""
+
+    def validate_storage_key(cls: type, key: Optional[str], values: RawSchemaDict) -> Optional[str]:
+        if key is not None:
+            predefined_keys = ["input_data", "logs", "cache"]
+            assert (
+                key in values["storage"].structure or key in predefined_keys
+            ), f"Couldn't find storage key {key!r} in the storage structure!"
+
+        return key
+
+    return field_validator(key, validate_storage_key, **kwargs)
 
 
 def parse_time_period(value: Tuple[str, str]) -> TimePeriod:
     """Allows parsing of preset options of shape `[preset_kind, year]` but that requires `pre` validation"""
     presets = ["yearly", "season", "Q1", "Q2", "Q3", "Q4", "Q1-yearly", "Q2-yearly", "Q3-yearly", "Q4-yearly"]
 
     if value[0] in presets:
@@ -146,16 +167,15 @@
     def _parse_output_types(cls, value: str) -> type:
         if value == "bool":
             return bool
         return np.dtype(value).type
 
 
 class DataCollectionSchema(BaseModel):
-    """Schema used in parsing DataCollection objects. Any extra parameters are passed to the definition as `**params`.
-    """
+    """Schema used in parsing DataCollection objects. Extra parameters are passed to the definition as `**params`."""
 
     name: str = Field(
         "Name of the data collection. When defining BYOC collections use `BYOC_` prefix and for Batch collections use"
         " `BATCH_` to auto-generate fields with `define_byoc` or `define_batch`."
     )
     bands: Union[None, str, Tuple[BandSchema, ...]] = Field(
         None, description="Name of predefined collection in `Bands` or custom specification via `BandSchema`."
@@ -208,7 +228,19 @@
         return DataCollection.define_byoc(collection_id, **params)
 
     if name.startswith("BATCH_"):
         collection_id = name.split("_")[-1]
         return DataCollection.define_batch(collection_id, **params)
 
     return DataCollection.define(name, **params)
+
+
+def restrict_types(
+    allowed_feature_types: Union[Iterable[FeatureType], Callable[[FeatureType], bool]]
+) -> Callable[[Feature], Feature]:
+    """Validates a field representing a feature, where it restricts the possible feature types."""
+
+    def validate_feature(value: Feature) -> Feature:
+        parse_feature(feature=value, allowed_feature_types=allowed_feature_types)
+        return value
+
+    return validate_feature
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eo-grow-1.4.0/eogrow/utils/vector.py` & `eo_grow-1.5.0/eogrow/utils/vector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 """
-Module containing useful utilities for working with vector data
+Module containing utilities for working with vector data
 """
-from typing import List, Union
+from typing import List, Optional, Union
 
 import geopandas as gpd
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.geometry import MultiPolygon, Polygon
 
 from sentinelhub import CRS
 
 
-def concat_gdf(dataframe_list: List[GeoDataFrame], reproject_crs: Union[CRS, int, None] = None) -> GeoDataFrame:
+def concat_gdf(dataframe_list: List[GeoDataFrame], reproject_crs: Optional[CRS] = None) -> GeoDataFrame:
     """Concatenates together multiple GeoDataFrames, all in the same CRS
 
     There exists pandas.concat but no geopandas.concat. Therefore, this function implements it.
 
     :param dataframe_list: A list of GeoDataFrames to be concatenated together
     :param reproject_crs: A CRS in which dataframes should be reprojected before being joined
     :return: A joined GeoDataFrame
     """
     if not (dataframe_list and all(isinstance(gdf, GeoDataFrame) for gdf in dataframe_list)):
         raise ValueError(f"Expected a list of GeoDataFrames with at least 1 element, got {dataframe_list}")
 
-    if reproject_crs:
-        crs = CRS(reproject_crs).pyproj_crs()
+    if reproject_crs is not None:
+        crs = reproject_crs.pyproj_crs()
         dataframe_list = [gdf.to_crs(crs) for gdf in dataframe_list]
     else:
         unique_crs = {vector_gdf.crs for vector_gdf in dataframe_list}
         if len(unique_crs) > 1:
-            raise ValueError("GeoDataFrames are in different CRS, therefore reproject_crs parameter should be given")
+            raise ValueError("GeoDataFrames are in different CRS, therefore `reproject_crs` parameter should be given")
 
     return gpd.GeoDataFrame(pd.concat(dataframe_list, ignore_index=True), crs=dataframe_list[0].crs)
 
 
 def count_points(geometry: Union[Polygon, MultiPolygon]) -> int:
     """Counts a number of points for a given geometry, both from exterior and interiors"""
-    if isinstance(geometry, Polygon):
-        exterior_count = len(geometry.exterior.coords)
-        interior_count = sum(len(interior.coords) for interior in geometry.interiors)
-        return exterior_count + interior_count
-
     if isinstance(geometry, MultiPolygon):
         return sum(count_points(subgeometry) for subgeometry in geometry.geoms)
-
-    raise NotImplementedError(f"Counting points for geometry type {type(geometry)} is not yet supported")
+    exterior_count = len(geometry.exterior.coords)
+    interior_count = sum(len(interior.coords) for interior in geometry.interiors)
+    return exterior_count + interior_count
```

### Comparing `eo-grow-1.4.0/eogrow/utils/zipmap.py` & `eo_grow-1.5.0/eogrow/utils/zipmap.py`

 * *Files identical despite different names*

