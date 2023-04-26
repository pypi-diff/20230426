# Comparing `tmp/chunkflow-1.1.4.tar.gz` & `tmp/chunkflow-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkflow-1.1.4.tar", last modified: Thu Sep  8 16:58:01 2022, max compression
+gzip compressed data, was "chunkflow-1.1.5.tar", last modified: Wed Apr 26 18:13:34 2023, max compression
```

## Comparing `chunkflow-1.1.4.tar` & `chunkflow-1.1.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.424609 chunkflow-1.1.4/
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    11357 2020-08-10 15:53:37.000000 chunkflow-1.1.4/LICENSE
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      181 2020-08-10 15:53:37.000000 chunkflow-1.1.4/MANIFEST.in
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9727 2022-09-08 16:58:01.422535 chunkflow-1.1.4/PKG-INFO
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     7918 2022-08-05 16:12:07.000000 chunkflow-1.1.4/README.md
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.078540 chunkflow-1.1.4/chunkflow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      178 2022-08-02 16:49:36.000000 chunkflow-1.1.4/chunkflow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       45 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/__main__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       18 2022-09-08 16:57:29.000000 chunkflow-1.1.4/chunkflow/__version__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.131326 chunkflow-1.1.4/chunkflow/chunk/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       24 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.139616 chunkflow-1.1.4/chunkflow/chunk/affinity_map/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       29 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/affinity_map/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1447 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/chunk/affinity_map/base.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    26918 2022-09-08 16:48:55.000000 chunkflow-1.1.4/chunkflow/chunk/base.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.152223 chunkflow-1.1.4/chunkflow/chunk/image/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       24 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9546 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/chunk/image/adjust_grey.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      719 2021-06-26 14:11:17.000000 chunkflow-1.1.4/chunkflow/chunk/image/base.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.159755 chunkflow-1.1.4/chunkflow/chunk/image/convnet/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    21914 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/inferencer.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.188129 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/__init__.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2932 2022-04-01 14:45:22.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/base.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1747 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/identity.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2548 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/patch_mask.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4447 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/pytorch.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1240 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/pznet.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2747 2022-04-26 21:36:45.000000 chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/universal.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1857 2022-09-05 18:35:32.000000 chunkflow-1.1.4/chunkflow/chunk/probability_map.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4411 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/chunk/segmentation.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2461 2022-04-01 14:41:10.000000 chunkflow-1.1.4/chunkflow/chunk/validate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.275474 chunkflow-1.1.4/chunkflow/flow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/flow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2190 2022-06-02 14:32:32.000000 chunkflow-1.1.4/chunkflow/flow/aggregate_skeleton_fragments.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      292 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/flow/base.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      778 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/flow/cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4183 2022-06-02 14:32:32.000000 chunkflow-1.1.4/chunkflow/flow/downsample_upload.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    88305 2022-09-07 15:42:36.000000 chunkflow-1.1.4/chunkflow/flow/flow.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1941 2022-08-22 20:12:53.000000 chunkflow-1.1.4/chunkflow/flow/load_pngs.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     8049 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/flow/load_precomputed.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1942 2022-04-01 14:41:10.000000 chunkflow-1.1.4/chunkflow/flow/log_summary.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4092 2022-08-30 18:29:45.000000 chunkflow-1.1.4/chunkflow/flow/mask.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     6671 2021-09-01 17:56:07.000000 chunkflow-1.1.4/chunkflow/flow/mesh.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2396 2022-06-22 14:21:36.000000 chunkflow-1.1.4/chunkflow/flow/mesh_manifest.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     8894 2022-08-31 23:34:37.000000 chunkflow-1.1.4/chunkflow/flow/neuroglancer.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4734 2022-04-28 21:05:13.000000 chunkflow-1.1.4/chunkflow/flow/normalize_section_contrast.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1052 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/flow/normalize_section_shang.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4577 2022-09-02 15:29:20.000000 chunkflow-1.1.4/chunkflow/flow/plugin.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1859 2022-08-12 19:19:27.000000 chunkflow-1.1.4/chunkflow/flow/save_pngs.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     5525 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/flow/save_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9147 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/flow/setup_env.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1121 2022-06-02 14:32:33.000000 chunkflow-1.1.4/chunkflow/flow/skeletonize.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      675 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/flow/view.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.296728 chunkflow-1.1.4/chunkflow/lib/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      349 2021-02-16 16:29:56.000000 chunkflow-1.1.4/chunkflow/lib/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.309167 chunkflow-1.1.4/chunkflow/lib/aws/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/lib/aws/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1952 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/lib/aws/cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     7326 2022-08-15 14:19:32.000000 chunkflow-1.1.4/chunkflow/lib/aws/sqs_queue.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    17614 2022-08-16 15:14:04.000000 chunkflow-1.1.4/chunkflow/lib/cartesian_coordinate.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4143 2022-08-16 15:21:58.000000 chunkflow-1.1.4/chunkflow/lib/flow.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.317192 chunkflow-1.1.4/chunkflow/lib/gala/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2021-04-26 17:46:23.000000 chunkflow-1.1.4/chunkflow/lib/gala/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    49887 2022-06-02 14:32:33.000000 chunkflow-1.1.4/chunkflow/lib/gala/evaluate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.334279 chunkflow-1.1.4/chunkflow/lib/igneous/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/chunkflow/lib/igneous/__init__.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)    13737 2022-04-01 14:41:11.000000 chunkflow-1.1.4/chunkflow/lib/igneous/downsample.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4832 2022-09-08 16:47:30.000000 chunkflow-1.1.4/chunkflow/lib/igneous/downsample_scales.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2749 2022-04-21 18:47:59.000000 chunkflow-1.1.4/chunkflow/lib/igneous/tasks.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     4483 2022-08-15 14:20:03.000000 chunkflow-1.1.4/chunkflow/lib/region_of_interest.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)    25097 2022-09-07 14:26:17.000000 chunkflow-1.1.4/chunkflow/lib/synapses.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2488 2022-08-15 14:20:03.000000 chunkflow-1.1.4/chunkflow/volume.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.108670 chunkflow-1.1.4/chunkflow.egg-info/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     9727 2022-09-08 16:57:59.000000 chunkflow-1.1.4/chunkflow.egg-info/PKG-INFO
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2953 2022-09-08 16:58:00.000000 chunkflow-1.1.4/chunkflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2022-09-08 16:57:59.000000 chunkflow-1.1.4/chunkflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       74 2022-09-08 16:57:59.000000 chunkflow-1.1.4/chunkflow.egg-info/entry_points.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 16:01:41.000000 chunkflow-1.1.4/chunkflow.egg-info/not-zip-safe
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      305 2022-09-08 16:57:59.000000 chunkflow-1.1.4/chunkflow.egg-info/requires.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       16 2022-09-08 16:57:59.000000 chunkflow-1.1.4/chunkflow.egg-info/top_level.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      306 2022-08-25 19:47:59.000000 chunkflow-1.1.4/requirements.txt
--rw-rw-r--   0 jwu       (1647) jwu       (1647)       38 2022-09-08 16:58:01.425389 chunkflow-1.1.4/setup.cfg
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2251 2022-08-02 16:49:36.000000 chunkflow-1.1.4/setup.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.345781 chunkflow-1.1.4/tests/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      134 2022-04-01 14:41:11.000000 chunkflow-1.1.4/tests/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.356896 chunkflow-1.1.4/tests/chunk/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.367133 chunkflow-1.1.4/tests/chunk/image/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/image/__init__.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.378376 chunkflow-1.1.4/tests/chunk/image/convnet/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/image/convnet/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     5200 2022-04-13 14:39:59.000000 chunkflow-1.1.4/tests/chunk/image/convnet/test_inferencer.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      739 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/image/convnet/test_patch_mask.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/image/test_adjust_grey.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      251 2021-02-16 16:29:56.000000 chunkflow-1.1.4/tests/chunk/image/test_image.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.385534 chunkflow-1.1.4/tests/chunk/segmentation/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/segmentation/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      643 2022-04-01 14:41:11.000000 chunkflow-1.1.4/tests/chunk/segmentation/test_segmentation.py
--rwxrwxr-x   0 jwu       (1647) jwu       (1647)     6269 2022-08-15 14:19:32.000000 chunkflow-1.1.4/tests/chunk/test_chunk.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      522 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/chunk/test_validate.py
-drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2022-09-08 16:58:01.418203 chunkflow-1.1.4/tests/flow/
--rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/flow/__init__.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      339 2020-09-01 21:59:09.000000 chunkflow-1.1.4/tests/flow/test_cloud_watch.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1900 2022-04-21 18:47:36.000000 chunkflow-1.1.4/tests/flow/test_downsample_upload.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     6963 2022-08-15 14:19:32.000000 chunkflow-1.1.4/tests/flow/test_flow.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     2263 2022-08-15 14:19:32.000000 chunkflow-1.1.4/tests/flow/test_load_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1839 2022-08-15 14:19:32.000000 chunkflow-1.1.4/tests/flow/test_load_save.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      556 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/flow/test_mesh.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      939 2022-04-01 14:41:11.000000 chunkflow-1.1.4/tests/flow/test_normalize_section_contrast.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)     1119 2022-07-13 14:15:10.000000 chunkflow-1.1.4/tests/flow/test_save_precomputed.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      140 2020-08-10 15:53:37.000000 chunkflow-1.1.4/tests/test_command_line.py
--rw-rw-r--   0 jwu       (1647) jwu       (1647)      926 2022-08-15 14:24:09.000000 chunkflow-1.1.4/tests/test_volume.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.769557 chunkflow-1.1.5/
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    11357 2020-08-10 15:53:37.000000 chunkflow-1.1.5/LICENSE
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      181 2020-08-10 15:53:37.000000 chunkflow-1.1.5/MANIFEST.in
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:13:34.766870 chunkflow-1.1.5/PKG-INFO
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     8011 2023-04-26 17:27:33.000000 chunkflow-1.1.5/README.md
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.288592 chunkflow-1.1.5/chunkflow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      178 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       45 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/__main__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       18 2023-04-26 18:12:55.000000 chunkflow-1.1.5/chunkflow/__version__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.357872 chunkflow-1.1.5/chunkflow/chunk/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       66 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/chunk/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.369549 chunkflow-1.1.5/chunkflow/chunk/affinity_map/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       29 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/affinity_map/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1447 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/chunk/affinity_map/base.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    31292 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/chunk/base.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.386544 chunkflow-1.1.5/chunkflow/chunk/image/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       24 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     9513 2022-12-06 02:16:24.000000 chunkflow-1.1.5/chunkflow/chunk/image/adjust_grey.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4532 2022-12-22 17:42:06.000000 chunkflow-1.1.5/chunkflow/chunk/image/base.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.397132 chunkflow-1.1.5/chunkflow/chunk/image/convnet/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    21829 2022-09-26 15:05:03.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/inferencer.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.436700 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/__init__.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2932 2022-04-01 14:45:22.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/base.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1747 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/identity.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2548 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/patch_mask.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4447 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pytorch.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1240 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pznet.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     2747 2022-09-20 18:00:38.000000 chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/universal.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1857 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/chunk/probability_map.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4468 2022-11-15 22:01:01.000000 chunkflow-1.1.5/chunkflow/chunk/segmentation.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2461 2022-04-01 14:41:10.000000 chunkflow-1.1.5/chunkflow/chunk/validate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.544155 chunkflow-1.1.5/chunkflow/flow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/flow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2190 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/aggregate_skeleton_fragments.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      292 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/base.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      778 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4183 2023-04-26 17:11:23.000000 chunkflow-1.1.5/chunkflow/flow/downsample_upload.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    96194 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/flow.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1941 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/load_pngs.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8118 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/load_precomputed.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     1942 2022-04-01 14:41:10.000000 chunkflow-1.1.5/chunkflow/flow/log_summary.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4087 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/mask.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     6645 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/mesh.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2396 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/mesh_manifest.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    10625 2023-04-26 17:27:32.000000 chunkflow-1.1.5/chunkflow/flow/neuroglancer.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4386 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/plugin.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1859 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/save_pngs.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     5213 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/save_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     9147 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/flow/setup_env.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1114 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/flow/skeletonize.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      675 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/flow/view.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.582365 chunkflow-1.1.5/chunkflow/lib/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      349 2021-02-16 16:29:56.000000 chunkflow-1.1.5/chunkflow/lib/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.598398 chunkflow-1.1.5/chunkflow/lib/aws/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/aws/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1952 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/aws/cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     7319 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/aws/sqs_queue.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    23021 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/cartesian_coordinate.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4143 2023-01-24 15:51:25.000000 chunkflow-1.1.5/chunkflow/lib/flow.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.608570 chunkflow-1.1.5/chunkflow/lib/gala/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2021-04-26 17:46:23.000000 chunkflow-1.1.5/chunkflow/lib/gala/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    48548 2022-09-26 15:05:03.000000 chunkflow-1.1.5/chunkflow/lib/gala/evaluate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.631085 chunkflow-1.1.5/chunkflow/lib/igneous/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/chunkflow/lib/igneous/__init__.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)    13737 2022-04-01 14:41:11.000000 chunkflow-1.1.5/chunkflow/lib/igneous/downsample.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     4832 2022-09-20 17:57:52.000000 chunkflow-1.1.5/chunkflow/lib/igneous/downsample_scales.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2525 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/igneous/tasks.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     4524 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/region_of_interest.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)    27402 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/synapses.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      497 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/lib/utils.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1337 2023-04-26 17:27:32.000000 chunkflow-1.1.5/chunkflow/point_cloud.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     7051 2023-04-26 17:27:33.000000 chunkflow-1.1.5/chunkflow/volume.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.329157 chunkflow-1.1.5/chunkflow.egg-info/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     8811 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2914 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       55 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/entry_points.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 16:01:41.000000 chunkflow-1.1.5/chunkflow.egg-info/not-zip-safe
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      300 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/requires.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       16 2023-04-26 18:13:33.000000 chunkflow-1.1.5/chunkflow.egg-info/top_level.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      301 2023-01-25 17:39:25.000000 chunkflow-1.1.5/requirements.txt
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)       38 2023-04-26 18:13:34.770756 chunkflow-1.1.5/setup.cfg
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2251 2022-09-20 17:57:52.000000 chunkflow-1.1.5/setup.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.647773 chunkflow-1.1.5/tests/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      134 2022-04-01 14:41:11.000000 chunkflow-1.1.5/tests/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.663884 chunkflow-1.1.5/tests/chunk/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.679714 chunkflow-1.1.5/tests/chunk/image/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/__init__.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.697556 chunkflow-1.1.5/tests/chunk/image/convnet/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/convnet/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     5238 2023-02-01 21:21:25.000000 chunkflow-1.1.5/tests/chunk/image/convnet/test_inferencer.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      739 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/convnet/test_patch_mask.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        1 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/image/test_adjust_grey.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      294 2022-12-22 16:53:55.000000 chunkflow-1.1.5/tests/chunk/image/test_image.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.708247 chunkflow-1.1.5/tests/chunk/segmentation/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/segmentation/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      643 2022-04-01 14:41:11.000000 chunkflow-1.1.5/tests/chunk/segmentation/test_segmentation.py
+-rwxrwxr-x   0 jwu       (1647) jwu       (1647)     6226 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/chunk/test_chunk.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      522 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/chunk/test_validate.py
+drwxrwxr-x   0 jwu       (1647) jwu       (1647)        0 2023-04-26 18:13:34.760305 chunkflow-1.1.5/tests/flow/
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)        0 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/flow/__init__.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      339 2020-09-01 21:59:09.000000 chunkflow-1.1.5/tests/flow/test_cloud_watch.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1900 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_downsample_upload.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     6958 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/flow/test_flow.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     2263 2023-01-25 17:33:29.000000 chunkflow-1.1.5/tests/flow/test_load_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1839 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_load_save.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      556 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/flow/test_mesh.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      429 2023-01-25 17:33:14.000000 chunkflow-1.1.5/tests/flow/test_normalize_section_contrast.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)     1119 2022-09-20 17:57:52.000000 chunkflow-1.1.5/tests/flow/test_save_precomputed.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      140 2020-08-10 15:53:37.000000 chunkflow-1.1.5/tests/test_command_line.py
+-rw-rw-r--   0 jwu       (1647) jwu       (1647)      948 2023-04-26 17:27:33.000000 chunkflow-1.1.5/tests/test_volume.py
```

### Comparing `chunkflow-1.1.4/LICENSE` & `chunkflow-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/PKG-INFO` & `chunkflow-1.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,146 +1,127 @@
-Metadata-Version: 2.1
-Name: chunkflow
-Version: 1.1.4
-Summary: Composable image chunk operators to create pipeline for distributed computation.
-Home-page: https://github.com/seung-lab/chunkflow
-Author: Jingpeng Wu
-Author-email: jingpeng.wu@gmail.com
-License: Apache License 2.0
-Description: ![alt text](https://github.com/seung-lab/chunkflow/blob/master/docs/logo/RGB_web/Chunkflow_logo_RBG.jpg?raw=true)
-        ----------------------
-        ![GitHub workflow](https://github.com/seung-lab/chunkflow/actions/workflows/.github/workflows/python-app.yml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/pychunkflow/badge/?version=latest)](https://pychunkflow.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/chunkflow.svg)](https://badge.fury.io/py/chunkflow)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://hub.docker.com/r/seunglab/chunkflow)
-        [![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fjingpeng_wu)](https://twitter.com/jingpeng_wu)
-        <!---[![Docker Build Status](https://img.shields.io/docker/cloud/build/seunglab/chunkflow.svg)]#(https://hub.docker.com/r/seunglab/chunkflow)--->
-        <!-- [![Build Status](https://travis-ci.org/seung-lab/chunkflow.svg?branch=master)](https://travis-ci.org/seung-lab/chunkflow) -->
-        <!-- [![Coverage Status](https://coveralls.io/repos/github/seung-lab/chunkflow/badge.svg?branch=master)](https://coveralls.io/github/seung-lab/chunkflow?branch=master) -->
-        
-        ## Problem 
-        - Petabyte scale 3D image processing is slow and computationally demanding;
-        - Computation has to be distributed with linear scalability;
-        - Local cluster and public cloud computing are not fully used at the same time;
-        - Duplicated code across a variety of routine tasks is hard to maintain.
-        
-        ## Features
-        - **Composable** operators. The chunk operators could be composed in a command line for flexible usage.
-        - **Hybrid Cloud Distributed** computation in both local and cloud computers. The task scheduling frontend and computationally heavy backend are decoupled using AWS Simple Queue Service. The backend could be any computer with an internet connection and cloud authentication. Benefit from the robust design, the cheap unstable instances (preemptable intance in Google Cloud, spot instance in AWS) could be used to reduce cost by about threefold!
-        - **Petabyte** scale. We have used chunkflow to output over eighteen-petabyte images and scaled up to 3600 nodes with NVIDIA GPUs across three regions in [Google Cloud](https://cloud.google.com/), and chunkflow is still reliable.
-        - Operators work with **3D** image volumes.
-        - You can **plug in** your own code as an operator.
-        
-        Check out the [Documentation](https://pychunkflow.readthedocs.io/en/latest/index.html) for [installation](https://pychunkflow.readthedocs.io/en/latest/install.html) and [usage](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). Try it out by following the [tutorial](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). 
-        
-        ## Image Segmentation Example
-        Perform Convolutional net inference to segment 3D image volume with one single command!
-        
-        ```shell
-        #!/bin/bash
-        
-        chunkflow \
-            load-tif --file-name path/of/image.tif -o image \
-            inference --convnet-model path/of/model.py --convnet-weight-path path/of/weight.pt \
-                --input-patch-size 20 256 256 --output-patch-overlap 4 64 64 --num-output-channels 3 \
-                -f pytorch --batch-size 12 --mask-output-chunk -i image -o affs \
-            plugin -f agglomerate --threshold 0.7 --aff-threshold-low 0.001 --aff-threshold-high 0.9999 -i affs -o seg \
-            neuroglancer -i image,affs,seg -p 33333 -v 30 6 6
-        ```
-        you can see your 3D image and segmentation directly in [Neuroglancer](https://github.com/google/neuroglancer)!
-        
-        ![Image_Segmentation](https://github.com/seung-lab/chunkflow/blob/master/docs/source/_static/image/image_seg.png)
-        
-        ## Composable Operators
-        After installation, You can simply type `chunkflow` and it will list all the operators with help message. We keep adding new operators and will keep it update here. For the detailed usage, please checkout our [Documentation](https://pychunkflow.readthedocs.io/en/latest/).
-        
-        | Operator Name   | Function |
-        | --------------- | -------- |
-        | adjust-bbox 	  | adjust the corner offset of bounding box |
-        | aggregate-skeleton-fragments| Merge skeleton fragments from chunks |
-        | channel-voting  | Vote across channels of semantic map |
-        | cleanup         | remove empty files to clean up storage |
-        | cloud-watch     | Realtime speedometer in AWS CloudWatch |
-        | connected-components | Threshold the boundary map to get a segmentation |
-        | copy-var        | Copy a variable to a new name |
-        | create-chunk    | Create a fake chunk for easy test |
-        | create-info     | Create info file of Neuroglancer Precomputed volume |
-        | crop-margin     | Crop the margin of a chunk |
-        | delete-chunk    | Delete chunk in task to reduce RAM requirement |
-        | delete-task-in-queue | Delete the task in AWS SQS queue |
-        | downsample-upload | Downsample the chunk hierarchically and upload to volume |
-        | download-mesh   | Download meshes from Neuroglancer Precomputed volume |
-        | evaluate-segmentation | Compare segmentation chunks |
-        | fetch-task-from-file | Fetch task from a file |
-        | fetch-task-from-sqs | Fetch task from AWS SQS queue one by one |
-        | generate-tasks  | Generate tasks one by one |
-        | gaussian-filter | 2D Gaussian blurring operated in-place |
-        | inference       | Convolutional net inference |
-        | load-synapses   | Load synapses from a file |
-        | save-synapses   | Save synapses as a HDF5 file. |
-        | log-summary     | Summary of logs |
-        | mark-complete   | mark task completion as an empty file | 
-        | mask            | Black out the chunk based on another mask chunk |
-        | mask-out-objects| Mask out selected or small objects |
-        | multiply 		  | Multiply chunks with another chunk |
-        | mesh            | Build 3D meshes from segmentation chunk |
-        | mesh-manifest   | Collect mesh fragments for object |
-        | neuroglancer    | Visualize chunks using neuroglancer |
-        | normalize-contrast-nkem | Normalize image contrast using histograms |
-        | normalize-intensity | Normalize image intensity to -1:1 |
-        | normalize-section-shang | Normalization algorithm created by Shang |
-        | plugin          | Import local code as a customized operator. |
-        | quantize        | Quantize the affinity map |
-        | load-h5         | Read HDF5 files |
-        | load-npy        | Read NPY files |
-        | load-json       | Read JSON files |
-        | load-pngs       | Read png files |
-        | load-precomputed| Cutout chunk from a local/cloud storage volume |
-        | load-tif        | Read TIFF files |
-        | load-nrrd       | Read NRRD files |
-        | remap-segmentation | Renumber a serials of segmentation chunks |
-        | setup-env       | Prepare storage infor files and produce tasks |
-        | skeletonize     | Create centerlines of objects in a segmentation chunk |
-        | skip-task  	  | If a result file already exists, skip this task |
-        | skip-all-zero   | If a chunk has all zero, skip this task |	
-        | skip-none       | If an item in task is None, skip this task |	
-        | threshold       | Use a threshold to segment the probability map |
-        | view            | Another chunk viewer in browser using CloudVolume |
-        | save-h5        | Save chunk as HDF5 file |
-        | save-pngs      | Save chunk as a serials of png files |
-        | save-precomputed| Save chunk to local/cloud storage volume |
-        | save-tif       | Save chunk as TIFF file |
-        | save-nrrd      | Save chunk as NRRD file |
-        
-        ## Affiliation
-        This package is developed at Princeton University and Flatiron Institute.
-        
-        ## Reference
-        We have a [paper](https://www.nature.com/articles/s41592-021-01088-5) for this repo: 
-        ```bibtex
-        
-        @article{wu_chunkflow_2021,
-        	title = {Chunkflow: hybrid cloud processing of large {3D} images by convolutional nets},
-        	issn = {1548-7105},
-        	shorttitle = {Chunkflow},
-        	url = {https://www.nature.com/articles/s41592-021-01088-5},
-        	doi = {10.1038/s41592-021-01088-5},
-        	journal = {Nature Methods},
-        	author = {Wu, Jingpeng and Silversmith, William M. and Lee, Kisuk and Seung, H. Sebastian},
-        	year = {2021},
-        	pages = {1--2}
-        }
-        ```
-        
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+![alt text](https://github.com/seung-lab/chunkflow/blob/master/docs/logo/RGB_web/Chunkflow_logo_RBG.jpg?raw=true)
+----------------------
+![GitHub workflow](https://github.com/seung-lab/chunkflow/actions/workflows/.github/workflows/python-app.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/pychunkflow/badge/?version=latest)](https://pychunkflow.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/chunkflow.svg)](https://badge.fury.io/py/chunkflow)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://hub.docker.com/r/seunglab/chunkflow)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fjingpeng_wu)](https://twitter.com/jingpeng_wu)
+<!---[![Docker Build Status](https://img.shields.io/docker/cloud/build/seunglab/chunkflow.svg)]#(https://hub.docker.com/r/seunglab/chunkflow)--->
+<!-- [![Build Status](https://travis-ci.org/seung-lab/chunkflow.svg?branch=master)](https://travis-ci.org/seung-lab/chunkflow) -->
+<!-- [![Coverage Status](https://coveralls.io/repos/github/seung-lab/chunkflow/badge.svg?branch=master)](https://coveralls.io/github/seung-lab/chunkflow?branch=master) -->
+
+## Problem 
+- Petabyte scale 3D image processing is slow and computationally demanding;
+- Computation has to be distributed with linear scalability;
+- Local cluster and public cloud computing are not fully used at the same time;
+- Duplicated code across a variety of routine tasks is hard to maintain.
+
+## Features
+- **Composable** operators. The chunk operators could be composed in a command line for flexible usage.
+- **Hybrid Cloud Distributed** computation in both local and cloud computers. The task scheduling frontend and computationally heavy backend are decoupled using AWS Simple Queue Service. The backend could be any computer with an internet connection and cloud authentication. Benefit from the robust design, the cheap unstable instances (preemptable intance in Google Cloud, spot instance in AWS) could be used to reduce cost by about threefold!
+- **Petabyte** scale. We have used chunkflow to output over eighteen-petabyte images and scaled up to 3600 nodes with NVIDIA GPUs across three regions in [Google Cloud](https://cloud.google.com/), and chunkflow is still reliable.
+- Operators work with **3D** image volumes.
+- You can **plug in** your own code as an operator.
+
+Check out the [Documentation](https://pychunkflow.readthedocs.io/en/latest/index.html) for [installation](https://pychunkflow.readthedocs.io/en/latest/install.html) and [usage](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). Try it out by following the [tutorial](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). 
+
+## Image Segmentation Example
+Perform Convolutional net inference to segment 3D image volume with one single command!
+
+```shell
+#!/bin/bash
+
+chunkflow \
+    load-tif --file-name path/of/image.tif -o image \
+    inference --convnet-model path/of/model.py --convnet-weight-path path/of/weight.pt \
+        --input-patch-size 20 256 256 --output-patch-overlap 4 64 64 --num-output-channels 3 \
+        -f pytorch --batch-size 12 --mask-output-chunk -i image -o affs \
+    plugin -f agglomerate --threshold 0.7 --aff-threshold-low 0.001 --aff-threshold-high 0.9999 -i affs -o seg \
+    neuroglancer -i image,affs,seg -p 33333 -v 30 6 6
+```
+you can see your 3D image and segmentation directly in [Neuroglancer](https://github.com/google/neuroglancer)!
+
+![Image_Segmentation](https://github.com/seung-lab/chunkflow/blob/master/docs/source/_static/image/image_seg.png)
+
+## Composable Operators
+After installation, You can simply type `chunkflow` and it will list all the operators with help message. We keep adding new operators and will keep it update here. For the detailed usage, please checkout our [Documentation](https://pychunkflow.readthedocs.io/en/latest/).
+
+| Operator Name   | Function |
+| --------------- | -------- |
+| adjust-bbox 	  | adjust the corner offset of bounding box |
+| aggregate-skeleton-fragments| Merge skeleton fragments from chunks |
+| channel-voting  | Vote across channels of semantic map |
+| cleanup         | remove empty files to clean up storage |
+| cloud-watch     | Realtime speedometer in AWS CloudWatch |
+| connected-components | Threshold the boundary map to get a segmentation |
+| copy-var        | Copy a variable to a new name |
+| create-chunk    | Create a fake chunk for easy test |
+| create-info     | Create info file of Neuroglancer Precomputed volume |
+| crop-margin     | Crop the margin of a chunk |
+| delete-chunk    | Delete chunk in task to reduce RAM requirement |
+| delete-task-in-queue | Delete the task in AWS SQS queue |
+| downsample-upload | Downsample the chunk hierarchically and upload to volume |
+| download-mesh   | Download meshes from Neuroglancer Precomputed volume |
+| evaluate-segmentation | Compare segmentation chunks |
+| fetch-task-from-file | Fetch task from a file |
+| fetch-task-from-sqs | Fetch task from AWS SQS queue one by one |
+| generate-tasks  | Generate tasks one by one |
+| gaussian-filter | 2D Gaussian blurring operated in-place |
+| inference       | Convolutional net inference |
+| load-synapses   | Load synapses from a file |
+| save-synapses   | Save synapses as a HDF5 file. |
+| save-points     | Save point cloud as a HDF5 file. |
+| log-summary     | Summary of logs |
+| mark-complete   | mark task completion as an empty file | 
+| mask            | Black out the chunk based on another mask chunk |
+| mask-out-objects| Mask out selected or small objects |
+| multiply 		  | Multiply chunks with another chunk |
+| mesh            | Build 3D meshes from segmentation chunk |
+| mesh-manifest   | Collect mesh fragments for object |
+| neuroglancer    | Visualize chunks using neuroglancer |
+| normalize-contrast-nkem | Normalize image contrast using histograms |
+| normalize-intensity | Normalize image intensity to -1:1 |
+| normalize-section-shang | Normalization algorithm created by Shang |
+| plugin          | Import local code as a customized operator. |
+| quantize        | Quantize the affinity map |
+| load-h5         | Read HDF5 files |
+| load-npy        | Read NPY files |
+| load-json       | Read JSON files |
+| load-pngs       | Read png files |
+| load-precomputed| Cutout chunk from a local/cloud storage volume |
+| load-tif        | Read TIFF files |
+| load-nrrd       | Read NRRD files |
+| load-zarr    	  | Read Zarr files |
+| remap-segmentation | Renumber a serials of segmentation chunks |
+| setup-env       | Prepare storage infor files and produce tasks |
+| skeletonize     | Create centerlines of objects in a segmentation chunk |
+| skip-task  	  | If a result file already exists, skip this task |
+| skip-all-zero   | If a chunk has all zero, skip this task |	
+| skip-none       | If an item in task is None, skip this task |	
+| threshold       | Use a threshold to segment the probability map |
+| view            | Another chunk viewer in browser using CloudVolume |
+| save-h5        | Save chunk as HDF5 file |
+| save-pngs      | Save chunk as a serials of png files |
+| save-precomputed| Save chunk to local/cloud storage volume |
+| save-tif       | Save chunk as TIFF file |
+| save-nrrd      | Save chunk as NRRD file |
+
+## Affiliation
+This package is developed at Princeton University and Flatiron Institute.
+
+## Reference
+We have a [paper](https://www.nature.com/articles/s41592-021-01088-5) for this repo: 
+```bibtex
+
+@article{wu_chunkflow_2021,
+	title = {Chunkflow: hybrid cloud processing of large {3D} images by convolutional nets},
+	issn = {1548-7105},
+	shorttitle = {Chunkflow},
+	url = {https://www.nature.com/articles/s41592-021-01088-5},
+	doi = {10.1038/s41592-021-01088-5},
+	journal = {Nature Methods},
+	author = {Wu, Jingpeng and Silversmith, William M. and Lee, Kisuk and Seung, H. Sebastian},
+	year = {2021},
+	pages = {1--2}
+}
+```
```

### Comparing `chunkflow-1.1.4/README.md` & `chunkflow-1.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: chunkflow
+Version: 1.1.5
+Summary: Composable image chunk operators to create pipeline for distributed computation.
+Home-page: https://github.com/seung-lab/chunkflow
+Author: Jingpeng Wu
+Author-email: jingpeng.wu@gmail.com
+License: Apache License 2.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://github.com/seung-lab/chunkflow/blob/master/docs/logo/RGB_web/Chunkflow_logo_RBG.jpg?raw=true)
 ----------------------
 ![GitHub workflow](https://github.com/seung-lab/chunkflow/actions/workflows/.github/workflows/python-app.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/pychunkflow/badge/?version=latest)](https://pychunkflow.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/chunkflow.svg)](https://badge.fury.io/py/chunkflow)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://hub.docker.com/r/seunglab/chunkflow)
@@ -66,14 +87,15 @@
 | fetch-task-from-file | Fetch task from a file |
 | fetch-task-from-sqs | Fetch task from AWS SQS queue one by one |
 | generate-tasks  | Generate tasks one by one |
 | gaussian-filter | 2D Gaussian blurring operated in-place |
 | inference       | Convolutional net inference |
 | load-synapses   | Load synapses from a file |
 | save-synapses   | Save synapses as a HDF5 file. |
+| save-points     | Save point cloud as a HDF5 file. |
 | log-summary     | Summary of logs |
 | mark-complete   | mark task completion as an empty file | 
 | mask            | Black out the chunk based on another mask chunk |
 | mask-out-objects| Mask out selected or small objects |
 | multiply 		  | Multiply chunks with another chunk |
 | mesh            | Build 3D meshes from segmentation chunk |
 | mesh-manifest   | Collect mesh fragments for object |
@@ -86,14 +108,15 @@
 | load-h5         | Read HDF5 files |
 | load-npy        | Read NPY files |
 | load-json       | Read JSON files |
 | load-pngs       | Read png files |
 | load-precomputed| Cutout chunk from a local/cloud storage volume |
 | load-tif        | Read TIFF files |
 | load-nrrd       | Read NRRD files |
+| load-zarr    	  | Read Zarr files |
 | remap-segmentation | Renumber a serials of segmentation chunks |
 | setup-env       | Prepare storage infor files and produce tasks |
 | skeletonize     | Create centerlines of objects in a segmentation chunk |
 | skip-task  	  | If a result file already exists, skip this task |
 | skip-all-zero   | If a chunk has all zero, skip this task |	
 | skip-none       | If an item in task is None, skip this task |	
 | threshold       | Use a threshold to segment the probability map |
```

### Comparing `chunkflow-1.1.4/chunkflow/chunk/affinity_map/base.py` & `chunkflow-1.1.5/chunkflow/chunk/affinity_map/base.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/base.py` & `chunkflow-1.1.5/chunkflow/chunk/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 from __future__ import annotations
 import logging
-from typing import Union
+from typing import Union, Optional
 import os
 from numbers import Number
 
 import h5py
 import numpy as np
 import nrrd
 from numpy.core.numerictypes import issubdtype
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
-from scipy.ndimage import gaussian_filter
-
 import tifffile
 import cc3d
 from cloudvolume.lib import yellow, Bbox
 
 from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
 
 # from typing import Tuple
 # Offset = Tuple[int, int, int]
 from .validate import validate_by_template_matching
 
+def layer_type_is_valid(type: str):
+    return type in set([None, 'image', 'segmentation', 'probability_map', 'affinity_map', 'unknown'])
+
 
 class Chunk(NDArrayOperatorsMixin):
-    r"""
-       Chunk 
-    
-    a chunk of big array with offset
-    implementation using numpy `dispatch<
-    https://docs.scipy.org/doc/numpy/user/basics.dispatch.html#module-numpy.doc.dispatch>`_.
-    and `examples<https://docs.scipy.org/doc/numpy/user/basics.dispatch.html#module-numpy.doc.dispatch>`_.
-
-    :param array: the data array chunk in a big dataset
-    :param voxel_offset (Cartesian): the offset of this array chunk. 3 numbers: z, y, x
-    :param voxel_size (Cartesian): the size of each voxel, normally with unit of nm. 3 numbers: z, y, x.
-    :return: a new chunk with array data and global offset
-    """
     def __init__(self, array: np.ndarray, 
             voxel_offset: Cartesian = None, 
-            voxel_size: Cartesian = None):
-        assert array.ndim >= 3 and array.ndim <= 4
-        assert isinstance(array, np.ndarray) or isinstance(array, Chunk)
+            voxel_size: Cartesian = None,
+            layer_type: str = None):
+        """chunk of a volume
+    
+        a chunk of big array with offset
+        implementation using numpy `dispatch<
+        https://docs.scipy.org/doc/numpy/user/basics.dispatch.html#module-numpy.doc.dispatch>`_.
+        and `examples<https://docs.scipy.org/doc/numpy/user/basics.dispatch.html#module-numpy.doc.dispatch>`_.
+
+        Args:
+            array (np.ndarray): the data
+            voxel_offset (Cartesian, optional): voxel offset. Defaults to None.
+            voxel_size (Cartesian, optional): voxel size. Defaults to None.
+            type (str, optional): type of chunk. [None, image, segmentation, probability_map, affinity_map, unknown]. Defaults to None.
         
+        Return: 
+            a new chunk with array data and global offset
+        """
+        if array.ndim == 2:
+            array = np.expand_dims(array, axis=0)
+        else:
+            assert array.ndim >= 3 and array.ndim <= 4
+        assert isinstance(array, np.ndarray) or isinstance(array, Chunk)
+        assert layer_type_is_valid(layer_type), f'layer type: {layer_type} is unsupported!'
+
         self.array = array
         if voxel_offset is None:
             if isinstance(array, Chunk):
                 self.array = array.array
                 voxel_offset = array.voxel_offset
             else:
                 voxel_offset = Cartesian(0, 0, 0)
@@ -64,20 +73,36 @@
         if voxel_size is not None and not isinstance(voxel_size, Cartesian):
             voxel_size = Cartesian.from_collection(voxel_size)
         self.voxel_size = voxel_size
         if voxel_size is not None:
             assert len(voxel_size) == 3
             assert np.alltrue([vs > 0 for vs in voxel_size])
         
+        if layer_type is not None:
+            self.layer_type = layer_type 
+        else:
+            # best guess
+            if self.is_image:
+                self.layer_type = 'image'
+            elif self.is_segmentation:
+                self.layer_type = 'segmentation'
+            elif self.is_probability_map:
+                self.layer_type = 'probability_map'
+            elif self.is_affinity_map:
+                self.layer_type = 'affinity_map'
+            else:
+                self.layer_type = 'unknown'
+
     # One might also consider adding the built-in list type to this
     # list, to support operations like np.add(array_like, list)
     _HANDLED_TYPES = (np.ndarray, Number)
     
     @classmethod
-    def from_array(cls, array: np.ndarray, bbox: BoundingBox, voxel_size: tuple = None):
+    def from_array(cls, array: np.ndarray, bbox: BoundingBox, 
+            voxel_size: Optional[tuple] = None):
         """
         :param array: ndarray data
         :param bbox: cloudvolume bounding box
         :param voxel_size: physical size of each voxel.
         :return: construct a new Chunk
         """
         return cls(array, voxel_offset=bbox.minpt, voxel_size=voxel_size)
@@ -172,31 +197,34 @@
                 raise NotImplementedError(f'do not support this data type: {dtype}')
         else:
             raise NotImplementedError(f'do not support the pattern: {pattern}')
 
         return cls(arr, voxel_offset=voxel_offset, voxel_size=voxel_size)
 
     def clone(self):
-        return Chunk(self.array.copy(), 
-            voxel_offset=self.voxel_offset, voxel_size=self.voxel_size)
+        return Chunk(
+            self.array.copy(), 
+            voxel_offset=self.voxel_offset, 
+            voxel_size=self.voxel_size
+        )
 
     @classmethod
     def from_nrrd(cls, file_name: str, voxel_offset: tuple=None, dtype: str = None,
             voxel_size: tuple=None):
         arr, _ = nrrd.read(file_name)
 
         if dtype:
             arr = arr.astype(dtype)
         return cls(arr, voxel_offset=voxel_offset, voxel_size=voxel_size)
     
     def to_nrrd(self, file_name: str=None):
         if file_name is None:
-            file_name = f'{self.bbox.to_filename()}.nrrd'
+            file_name = f'{self.bbox.string}.nrrd'
         elif not file_name.endswith('.nrrd'):
-            file_name += f'_{self.bbox.to_filename()}.nrrd'
+            file_name += f'_{self.bbox.string}.nrrd'
 
         logging.info(f'write chunk to file: {file_name}')
         nrrd.write(file_name, self.array)
 
     @classmethod
     def from_tif(cls, file_name: str, voxel_offset: tuple=None, dtype: str = None,
             voxel_size: tuple=None):
@@ -205,15 +233,15 @@
         if dtype:
             arr = arr.astype(dtype)
         logging.info(f'read tif chunk with size of {arr.shape}, voxel offset: {voxel_offset}, voxel size: {voxel_size}')
         return cls(arr, voxel_offset=voxel_offset, voxel_size=voxel_size)
     
     def to_tif(self, file_name: str=None, compression: str = 'zlib'):
         if file_name is None:
-            file_name = f'{self.bbox.to_filename()}.tif'
+            file_name = f'{self.bbox.string}.tif'
         logging.info(f'write chunk to file: {file_name}')
 
         if self.array.dtype==np.float32:
             # visualization in float32 is not working correctly in ImageJ
             # this might not work correctly if you want to save the image as it is!
             print(yellow('transforming data type from float32 to uint8'))
             img = self.array*255 
@@ -239,27 +267,28 @@
     def from_h5(cls, file_name: str,
                 voxel_offset: tuple=None,
                 dataset_path: str = None,
                 voxel_size: tuple = None,
                 cutout_start: tuple = None,
                 cutout_stop: tuple = None,
                 cutout_size: tuple = None,
-                dtype: str = None):
+                dtype: str = None,
+                layer_type: str = None):
 
-        if not os.path.exists(file_name):
-            raise ValueError(f'the file do not exist: {file_name}')
+        file_name = os.path.expanduser(file_name)
+        assert os.path.exists(file_name), f'the file do not exist: {file_name}'
         
         if cutout_start is not None and cutout_size is not None:
             cutout_stop = tuple(t+s for t, s in zip(cutout_start, cutout_size))
 
         if not h5py.is_hdf5(file_name):
             assert cutout_start is not None 
             assert cutout_stop is not None
             bbox = BoundingBox.from_list([*cutout_start, *cutout_stop])
-            file_name += f'{bbox.to_filename()}.h5'
+            file_name += f'{bbox.string}.h5'
 
             if not os.path.exists(file_name) or os.path.getsize(file_name)==0:
                 # fill with zero
                 assert dtype is not None
                 logging.info(f'{file_name} do not exist or is empty, will return None.')
                 # return cls.from_bbox(bbox, dtype=dtype, voxel_size=voxel_size, all_zero=True)
                 return None
@@ -279,19 +308,32 @@
                     voxel_offset = Cartesian(0, 0, 0)
 
             if voxel_size is None:
                 if 'voxel_size' in f:
                     voxel_size = Cartesian(*f['voxel_size'])
                 else:
                     voxel_size = Cartesian(1, 1, 1)
+
+            if layer_type is None:
+                if 'layer_type' in f.attrs:
+                    layer_type = f.attrs['layer_type']
+                    # type = str(f['type'])
+                    assert layer_type_is_valid(layer_type)
             
             if cutout_start is None:
                 cutout_start = voxel_offset
             if cutout_size is None:
                 cutout_size = dset.shape[-3:]
+                cutout_size = Cartesian.from_collection(cutout_size)
+            elif np.min(cutout_size) < 0:
+                cutout_size = [x for x in cutout_size]
+                for idx in range(-1, -4, -1):
+                    if cutout_size[idx]<0:
+                        cutout_size[idx] = dset.shape[idx]
+                cutout_size = Cartesian.from_collection(cutout_size)
             if cutout_stop is None:
                 cutout_stop = tuple(t+s for t, s in zip(cutout_start, cutout_size))
 
             for c, v in zip(cutout_start, voxel_offset):
                 assert c >= v, "can only cutout after the global voxel offset."
             
             assert len(cutout_start) == 3
@@ -309,45 +351,48 @@
         if arr.dtype == np.dtype('<f4'):
             arr = arr.astype('float32')
         elif arr.dtype == np.dtype('<f8'):
             arr = arr.astype('float64') 
 
         logging.info(f'new chunk voxel offset: {cutout_start}')
 
-        return cls(arr, voxel_offset=cutout_start, voxel_size=voxel_size)
+        return cls(arr, voxel_offset=cutout_start, voxel_size=voxel_size, layer_type=layer_type)
 
     def to_h5(self, file_name: str, with_offset: bool=True, 
-                chunk_size: Cartesian = Cartesian(64,64,64),
+                chunk_size: Union[Cartesian, tuple] = (8,8,8),
                 with_unique: bool= True, 
                 compression="gzip",
                 voxel_size: tuple = None):
         """
         :param file_name: output file name. If it is not end with h5, the coordinate will be appended to the file name.
         :param with_offset: save the voxel offset or not
         :param with_unique: if this is a segmentation chunk, save the unique object ids or not.
         :param compression: use HDF5 compression or not. Options are gzip, lzf
         """
         if chunk_size:
             assert len(chunk_size) == 3
+        if isinstance(chunk_size, Cartesian):
+            chunk_size = tuple(*chunk_size)
 
         if not file_name.endswith('.h5'):
-            file_name += self.bbox.to_filename() + '.h5'
+            file_name += self.bbox.string + '.h5'
 
         logging.info(f'write chunk to file: {file_name}')
         if os.path.exists(file_name):
             print(yellow(f'deleting existing file: {file_name}'))
             os.remove(file_name)
 
-
         with h5py.File(file_name, 'w') as f:
             f.create_dataset('/main', data=self.array, chunks=chunk_size, compression=compression)
             if voxel_size is None and self.voxel_size is not None:
                 voxel_size = self.voxel_size
             if voxel_size is not None:
                 f.create_dataset('/voxel_size', data=voxel_size)
+            if self.layer_type is not None:
+                f.attrs['layer_type'] = self.layer_type
 
             if with_offset and self.voxel_offset is not None:
                 f.create_dataset('/voxel_offset', data=self.voxel_offset)
 
             if with_unique and self.is_segmentation:
                 unique = np.unique(self.array)
                 if unique[0]:
@@ -416,29 +461,76 @@
             return self.array == value
         elif isinstance(value, np.ndarray):
             # return np.all(self.array == value)
             return self.array == value
         else:
             raise NotImplementedError
 
-    def set_properties(self, properties: dict):
-        if 'voxel_offset' in properties:
-            self.voxel_offset = properties['voxel_offset']
 
-        if 'voxel_size' in properties:
-            self.voxel_size = properties['voxel_size']
+    # @property
+    # def voxel_offset(self) -> Cartesian:
+    #     return self.voxel_offset
+
+    # @voxel_offset.setter
+    # def voxel_offset(self, value: Cartesian):
+    #     self.voxel_offset = value
+
+    # @property
+    # def voxel_size(self) -> Cartesian:
+    #     return self.voxel_size
+
+    # @voxel_size.setter
+    # def voxel_size(self, value: Cartesian):
+    #     self.voxel_size = value
+
+    @property
+    def is_image(self) -> bool:
+        return issubdtype(self.dtype, np.uint8) and \
+                    self.ndim == 3
+
+    @property 
+    def is_segmentation(self) -> bool:
+        return self.array.ndim == 3 and \
+                    (np.issubdtype(self.array.dtype, np.integer) or \
+                        np.issubdtype(self.dtype, bool)) and \
+                            self.array.dtype != np.uint8
+
+    @property
+    def is_affinity_map(self) -> bool:
+        return self.array.ndim == 4 and self.shape[0] == 3 and self.array.dtype == np.float32
+    
+    @property
+    def is_probability_map(self) -> bool:
+        return self.array.ndim == 4 and self.array.dtype == np.float32
 
     @property
     def properties(self) -> dict:
         props = dict()
         if self.voxel_offset is not None or self.voxel_offset != Cartesian(0, 0, 0):
             props['voxel_offset'] = self.voxel_offset
         if self.voxel_size is not None or self.voxel_size != Cartesian(1, 1, 1):
             props['voxel_size'] = self.voxel_size
+        if self.layer_type is not None:
+            props['layer_type'] = self.layer_type
+
         return props 
+    
+    def set_properties(self, properties: dict):
+        if 'voxel_offset' in properties:
+            self.voxel_offset = properties['voxel_offset']
+
+        if 'voxel_size' in properties:
+            self.voxel_size = properties['voxel_size']
+        
+        if 'layer_type' in properties:
+            self.layer_type = properties['layer_type']
+
+    @properties.setter
+    def properties(self, value: dict):
+        self.set_properties(value)
 
     @property
     def flags(self):
         return self.array.flags
 
     @property
     def size(self):
@@ -447,34 +539,16 @@
     @property
     def slices(self) -> tuple:
         """
         :getter: the global slice in the big volume
         """
         return tuple(
             slice(o, o + s) for o, s in zip(self.ndoffset, self.shape))
-
-    @property
-    def is_image(self) -> bool:
-        return self.array.ndim == 3 and self.array.dtype == np.uint8
-
-    @property 
-    def is_segmentation(self) -> bool:
-        return self.array.ndim == 3 and (np.issubdtype(
-            self.array.dtype, np.integer) or np.issubdtype(
-                self.dtype, bool)) and self.array.dtype != np.uint8
-
-    @property
-    def is_affinity_map(self) -> bool:
-        return self.array.ndim == 4 and self.shape[0] == 3 and self.array.dtype == np.float32
     
     @property
-    def is_probability_map(self) -> bool:
-        return self.array.ndim == 4 and self.array.dtype == np.float32
-
-    @property
     def ndoffset(self) -> tuple:
         """ 
         make the voxel offset have the same dimension with array
         """
         if self.ndim == 4:
             return (0, *self.voxel_offset)
         else:
@@ -483,15 +557,27 @@
     @property
     def bbox(self) -> BoundingBox:
         """
         :getter: the bounding box in the big volume
         """
         bbox = BoundingBox.from_delta(self.voxel_offset, self.array.shape[-3:])
         return bbox
-    
+
+    @property
+    def bounding_box(self) -> BoundingBox:
+        return self.bbox
+
+    @property
+    def start(self) -> Cartesian:
+        return self.bbox.start
+
+    @property
+    def stop(self) -> Cartesian:
+        return self.bbox.stop
+
     @property
     def ndim(self) -> int:
         return self.array.ndim 
 
     @property 
     def shape(self) -> tuple:
         return self.array.shape 
@@ -500,15 +586,15 @@
     def dtype(self) -> np.dtype:
         return self.array.dtype 
 
     @property
     def voxel_stop(self) -> tuple:
         return tuple(o + s for o, s in zip(self.voxel_offset, self.shape))
 
-    def astype(self, dtype: np.dtype):
+    def astype(self, dtype: Union[np.dtype, str]):
         if dtype is None:
             new_array = self.array
         elif dtype != self.array.dtype:
             new_array = self.array.astype(dtype)
         else:
             new_array = self.array
         return Chunk(new_array, voxel_offset=self.voxel_offset, voxel_size=self.voxel_size)
@@ -519,14 +605,32 @@
 
     def max(self, *args, **kwargs):
         return self.array.max(*args, **kwargs)
 
     def min(self, *args, **kwargs):
         return self.array.min(*args, **kwargs)
 
+    def shrink(self, size: tuple):
+        """shrink the array from surrounding boundary
+
+        Args:
+            size (tuple): the shrink size in -Z,-Y, -X, Z, Y, X direction.
+            sometimes, the shrinking might be asymmetric. that's why we need
+            6 elements rather than 3.
+        """
+        assert len(size) == 6 or len(size) == 3
+        z, y, x = self.shape[-3:]
+        self.array = self.array[
+            ...,
+            size[0]:z-size[-3],
+            size[1]:y-size[-2],
+            size[2]:x-size[-1],
+        ]
+        self.voxel_offset += Cartesian.from_collection(size[:3])
+
     def transpose(self, only_array: bool=False):
         """To-Do: support arbitrary axis transpose"""
         new_array = self.array.transpose()
         if not only_array and self.voxel_offset is not None:
             voxel_offset = self.voxel_offset[::-1]
         else:
             voxel_offset = self.voxel_offset
@@ -550,40 +654,62 @@
     def channel_voting(self):
         assert self.ndim == 4
         assert self.shape[0] <= 256
         out = np.empty(self.shape[1:], dtype=np.uint8)
         np.argmax(self.array, axis=0, out=out)
         # our selected channel index start from 1
         out += 1
-        return Chunk(out, voxel_offset=self.voxel_offset, voxel_size=self.voxel_size)
+        return Chunk(out, 
+            voxel_offset=self.voxel_offset, 
+            voxel_size=self.voxel_size,
+            layer_type='segmentation',
+        )
 
     def mask_using_last_channel(self, threshold: float = 0.3) -> np.ndarray:
         mask = (self.array[-1, :, :, :] < threshold)
         ret = self.array[:-1, ...]
         ret *= mask
         return Chunk(ret, voxel_offset=self.voxel_offset, voxel_size=self.voxel_size)
 
     def crop_margin(
             self, 
             margin_size: tuple = None, 
             output_bbox: BoundingBox=None
         ):
+        """_summary_
+
+        Args:
+            margin_size (tuple, optional): -z,-y,-x,+z,+y,+x. Defaults to None.
+            output_bbox (BoundingBox, optional): _description_. Defaults to None.
+
+        Returns:
+            _type_: _description_
+        """
 
         if margin_size:
-            new_array = self.array[...,
-                margin_size[0]: -margin_size[0],
-                margin_size[1]: -margin_size[1],
-                margin_size[2]: -margin_size[2]]
+            sz,sy,sx = self.array.shape[-3:]
+            if len(margin_size) == 3:
+                new_array = self.array[...,
+                    margin_size[0]: sz-margin_size[0],
+                    margin_size[1]: sy-margin_size[1],
+                    margin_size[2]: sx-margin_size[2]]
+            elif len(margin_size) == 6:
+                new_array = self.array[...,
+                    margin_size[0]: sz-margin_size[3],
+                    margin_size[1]: sy-margin_size[4],
+                    margin_size[2]: sx-margin_size[5]]
+            else:
+                raise ValueError('only support 3 or 6 elements.')
             voxel_offset = tuple(
                 o + m for o, m in zip(self.voxel_offset, margin_size))
             return Chunk(new_array, voxel_offset=voxel_offset, voxel_size=self.voxel_size)
         else:
             logging.info('automatically crop the chunk to output bounding box.')
             assert output_bbox is not None
-            return self.cutout(output_bbox.to_slices())
+            return self.cutout(output_bbox.slices)
     
     def threshold(self, threshold: float):
         array = self.array > threshold
         if array.ndim == 4:
             assert array.shape[0] == 1
             array = array[0, ...]
         seg = Chunk(array, voxel_offset = self.voxel_offset, voxel_size=self.voxel_size)
@@ -618,24 +744,27 @@
         """
         cutout a region of interest from this chunk
 
         :param slices: the global slices of region of interest
         :return: another chunk of region of interest
         """
         if isinstance(x, BoundingBox) or isinstance(x, Bbox):
-            slices = x.to_slices()
+            slices = x.slices
         else:
             slices = x
             
         if len(slices) == self.ndim - 1:
             slices = (slice(0, self.shape[0]), ) + slices
         internalSlices = self._get_internal_slices(slices)
         arr = self.array[internalSlices]
         voxel_offset = tuple(s.start for s in slices[-3:])
-        return Chunk(arr, voxel_offset=voxel_offset, voxel_size=self.voxel_size)
+        return Chunk(arr, 
+            voxel_offset=voxel_offset, 
+            voxel_size=self.voxel_size, 
+            layer_type=self.layer_type)
 
     def save(self, patch):
         """
         replace a region of interest from another chunk
 
         :param patch: a small chunk to replace subvolume
         """
```

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/adjust_grey.py` & `chunkflow-1.1.5/chunkflow/chunk/image/adjust_grey.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     nominalmax:
         max threshold
     clipvalues:
         clip values or not.
     """
     assert nominalmin < nominalmax
     assert image.ndim == 3
-    voxel_offset = image.voxel_offset
+    # voxel_offset = image.voxel_offset
     originaltype = image.dtype
     arr = image.astype(np.float32)
 
     # number of bits per voxel
     nbits = np.dtype(originaltype).itemsize * 8
     default_nominalmax = float(2**nbits - 1)
 
@@ -224,16 +224,15 @@
                   min_max_invalid=[True, True],
                   do_clipping=clipvalues,
                   make_copy=False)
 
     # cast to original data type if necessary
     #arr = np.round(arr)
     #arr = arr.astype(originaltype)
-
-    return Chunk(arr, voxel_offset=voxel_offset)
+    return arr
 
 
 def test1_grey_augment():
     from numpy.random import randint
     x = np.random.rand(*randint(200, size=randint(5)))
     print(x.shape)
     y = grey_augment(x, value_range=[0, 1])
```

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/inferencer.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/inferencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,31 +30,31 @@
     The output buffer is smaller than the input chunk size, and the cropped 
     margin area is not allocated. This will save about 20% of memory usage.
     what's more, the output buffer is formated as memory map and was mapped 
     to disk. This is particularly useful for multiple channel output with 
     large chunk size.
     """
     def __init__(self,
-                 convnet_model: Union[str, PatchInferencerBase],
-                 convnet_weight_path: str,
-                 input_patch_size: Union[tuple, list, Cartesian],
-                 output_patch_size: Union[tuple, list, Cartesian] = None,
-                 patch_num: Union[tuple, list, Cartesian] = None,
-                 num_output_channels: int = 3,
-                 output_patch_overlap: Union[tuple, list, Cartesian] = None,
-                 output_crop_margin: Union[tuple, list, Cartesian] = None,
-                 dtype = 'float32',
-                 framework: str = 'universal',
-                 batch_size: int = 1,
-                 bump: str = 'wu',
-                 input_size: Union[tuple, list, Cartesian] = None,
-                 mask_output_chunk: bool = True,
-                 mask_myelin_threshold = None,
-                 test_time_augmentation: bool = False,
-                 dry_run: bool = False):
+            convnet_model: Union[str, PatchInferencerBase],
+            convnet_weight_path: str,
+            input_patch_size: Union[tuple, list, Cartesian],
+            output_patch_size: Union[tuple, list, Cartesian] = None,
+            patch_num: Union[tuple, list, Cartesian] = None,
+            num_output_channels: int = 3,
+            output_patch_overlap: Union[tuple, list, Cartesian] = None,
+            output_crop_margin: Union[tuple, list, Cartesian] = None,
+            dtype = 'float32',
+            framework: str = 'universal',
+            batch_size: int = 1,
+            bump: str = 'wu',
+            input_size: Union[tuple, list, Cartesian] = None,
+            mask_output_chunk: bool = True,
+            mask_myelin_threshold = None,
+            test_time_augmentation: bool = False,
+            dry_run: bool = False):
         """convnet inference patch by patch in a chunk
 
         Args:
             convnet_model (Union[str, PatchInferencerBase]): the path of convnet model
             convnet_weight_path (str): the path of trained model weights
             input_patch_size (Union[tuple, list, Cartesian]): input patch size, zyx
             output_patch_size (Union[tuple, list, Cartesian], optional): output patch size. Defaults to the same with input patch size.
```

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/base.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/base.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/identity.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/identity.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/patch_mask.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/patch_mask.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/pytorch.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pytorch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/pznet.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/pznet.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/image/convnet/patch/universal.py` & `chunkflow-1.1.5/chunkflow/chunk/image/convnet/patch/universal.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/probability_map.py` & `chunkflow-1.1.5/chunkflow/chunk/probability_map.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/chunk/segmentation.py` & `chunkflow-1.1.5/chunkflow/chunk/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 __doc__ = """Image chunk class"""
 import os
 import json
+from typing import Union
 
 import logging
 import multiprocessing
-from typing import Union
 
 import numpy as np
-from .base import Chunk
-
-# from ...lib.gala import evaluate
-from chunkflow.lib.gala import evaluate
-from chunkflow.lib.cartesian_coordinate import Cartesian
 
 import kimimaro
 import fastremap
 
 from cloudfiles import CloudFiles
 
+# from ...lib.gala import evaluate
+from .base import Chunk
+from chunkflow.lib.gala import evaluate
+from chunkflow.lib.cartesian_coordinate import Cartesian
+
 
 class Segmentation(Chunk):
     """
     a chunk of segmentation volume.
     """
     def __init__(self, array: np.ndarray, 
             voxel_offset: Cartesian=None, 
@@ -56,32 +56,33 @@
             groundtruth = groundtruth.array
 
         rand_index = evaluate.rand_index(this.array, groundtruth)
         adjusted_rand_index = evaluate.adj_rand_index(this.array, groundtruth)
         variation_of_information = evaluate.vi(this.array, groundtruth)
         fowlkes_mallows_index = evaluate.fm_index(this.array, groundtruth)
         edit_distance = evaluate.edit_distance(this.array, groundtruth, size_threshold=size_threshold)
-        print('rand index: ', rand_index)
-        print('adjusted rand index: ', adjusted_rand_index)
-        print('variation of information: ', variation_of_information)
-        print('edit distance: ', edit_distance)
-        print('Fowlkes Mallows Index: ', fowlkes_mallows_index)
+        print(f'rand index: {rand_index: .3f}')
+        print(f'adjusted rand index: {adjusted_rand_index: .3f}')
+        print(f'variation of information: {variation_of_information: .3f}')
+        print(f'edit distance: {edit_distance}')
+        print(f'Fowlkes Mallows Index: {fowlkes_mallows_index: .3f}')
 
         ret = {}
         ret['rand_index'] = rand_index
         ret['adjusted_rand_index'] = adjusted_rand_index
         ret['variation_of_information'] = variation_of_information
         ret['fowlkes_mallows_index'] = fowlkes_mallows_index
         ret['edit_distance'] = edit_distance
         return ret
 
-    def remap(self, start_id: int):
+    def remap(self, start_id: int = 0):
         fastremap.renumber(self.array, preserve_zero=True, in_place=True)
         seg = self.astype(np.uint64)
-        seg.array[seg.array>0] += start_id
+        if start_id > 0:
+            seg.array[seg.array>0] += start_id
         start_id = seg.max()
         return seg, start_id
 
     def mask_fragments(self, voxel_num_threshold: int):
         uniq, counts = fastremap.unique(self.array, return_counts=True)
         fragment_ids = uniq[counts <= voxel_num_threshold]
         logging.info(f'masking out {len(fragment_ids)} fragments in {len(uniq)} with a percentage of {len(fragment_ids)/len(uniq)}')
@@ -110,8 +111,7 @@
     def skeletonize(self, voxel_size):
         skels = kimimaro.skeletonize(
             self.array,
             anisotropy=voxel_size,
             parallel=multiprocessing.cpu_count() // 2
         )
         return skels
-
```

### Comparing `chunkflow-1.1.4/chunkflow/chunk/validate.py` & `chunkflow-1.1.5/chunkflow/chunk/validate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/aggregate_skeleton_fragments.py` & `chunkflow-1.1.5/chunkflow/flow/aggregate_skeleton_fragments.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/cloud_watch.py` & `chunkflow-1.1.5/chunkflow/flow/cloud_watch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/downsample_upload.py` & `chunkflow-1.1.5/chunkflow/flow/downsample_upload.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/flow.py` & `chunkflow-1.1.5/chunkflow/flow/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,77 @@
 import os
 from pathlib import Path
 from time import time
 
 from typing import Generator, List
 
 from copy import deepcopy
-from matplotlib import use
 
 import numpy as np
 import click
 import json
 from tqdm import tqdm
-from traitlets import default 
 
-from chunkflow.lib.flow import *
+import zarr
+import tinybrain
 
+from chunkflow.lib.flow import *
 from cloudvolume import CloudVolume
 from cloudvolume.lib import Vec
 from cloudfiles import CloudFiles
 
 from chunkflow.lib.aws.sqs_queue import SQSQueue
 from chunkflow.lib.cartesian_coordinate import Cartesian, BoundingBox, BoundingBoxes
 from chunkflow.lib.synapses import Synapses
 
 from chunkflow.chunk import Chunk
+from chunkflow.chunk.image import Image
 from chunkflow.chunk.affinity_map import AffinityMap
 from chunkflow.chunk.segmentation import Segmentation
 from chunkflow.chunk.image.convnet.inferencer import Inferencer
+from chunkflow.point_cloud import PointCloud
 
 # import operator functions
 from .aggregate_skeleton_fragments import AggregateSkeletonFragmentsOperator
 from .cloud_watch import CloudWatchOperator
-from .load_precomputed import ReadPrecomputedOperator
+from .load_precomputed import LoadPrecomputedOperator
 from .downsample_upload import DownsampleUploadOperator
 from .log_summary import load_log, print_log_statistics
 from .mask import MaskOperator
 from .mesh import MeshOperator
 from .mesh_manifest import MeshManifestOperator
 from .neuroglancer import NeuroglancerOperator
-from .normalize_section_contrast import NormalizeSectionContrastOperator
-from .normalize_section_shang import NormalizeSectionShangOperator
 from .plugin import Plugin
 from .load_pngs import load_png_images
 from .save_precomputed import SavePrecomputedOperator
 from .save_pngs import SavePNGsOperator
 from .setup_env import setup_environment
 from .skeletonize import SkeletonizeOperator
 from .view import ViewOperator
 
+@main.command('create-bbox')
+@click.option('--start', '-s', 
+    type=click.INT, required=True, nargs=3,
+    help = 'voxel offset or start of the bounding box.')
+@click.option('--stop', '-p',
+    type=click.INT, default=None, nargs=3, callback=default_none,
+    help='voxel stop or end of bounding box.')
+@click.option('--size', '-z', 
+    type=click.INT, default=None, nargs=3, callback=default_none,
+    help='volume size or dimension.')
+@generator
+def create_bbox(start: tuple, stop: tuple, size: tuple):
+    assert stop is not None or size is not None
+    if stop is None:
+        stop = Cartesian.from_collection(start) + Cartesian.from_collection(size)
+    bbox = BoundingBox(start, stop)
+    task = get_initial_task()
+    task['bbox'] = bbox
+    yield task
+
 
 @main.command('generate-tasks')
 @click.option('--layer-path', '-l',
               type=str, default=None,
               help='dataset layer path to fetch dataset information.')
 @click.option('--mip', '-m',
               type=click.INT, default=None, help='mip level of the dataset layer.')
@@ -86,21 +106,24 @@
     help='force alignment of block size. Note that the alignment start from (0, 0, 0).')
 @click.option('--task-index-start', '-i',
               type=click.INT, default=0, help='starting index of task list.')
 @click.option('--task-index-stop', '-p',
               type=click.INT, default=None, help='stop index of task list.')
 @click.option('--disbatch/--no-disbatch', '-d',
               default=False, help='use disBatch environment variable or not')
+@click.option('--use-https/--use-credential', default=False,
+    help='if we read from a public dataset in cloud storage, it is required to use https.')
 @generator
 def generate_tasks(
         layer_path: str, mip: int, roi_start: tuple, roi_stop: tuple, 
         roi_size: tuple, chunk_size: tuple, bounding_box:str,
         grid_size: tuple, file_path: str, queue_name: str, 
         respect_chunk_size: bool, aligned_block_size: tuple, 
-        task_index_start: tuple, task_index_stop: tuple, disbatch: bool ):
+        task_index_start: tuple, task_index_stop: tuple, 
+        disbatch: bool, use_https: bool):
     """Generate a batch of tasks."""
     if mip is None:
         mip = state['mip']
     assert mip >=0 
 
     if bounding_box is not None:
         bboxes = [BoundingBox.from_string(bounding_box)]
@@ -110,27 +133,29 @@
             assert chunk_size == bboxes[0].shape
     else:
         bboxes = BoundingBoxes.from_manual_setup(
             chunk_size, layer_path=layer_path,
             roi_start=roi_start, roi_stop=roi_stop, 
             roi_size=roi_size, mip=mip, grid_size=grid_size,
             respect_chunk_size=respect_chunk_size,
-            aligned_block_size=aligned_block_size
+            aligned_block_size=aligned_block_size,
+            use_https=use_https
         )
     print(f'number of all the candidate tasks: {len(bboxes)}')
     
     if task_index_start:
         if task_index_stop is None:
             # task_index_stop = task_index_start + 1
             task_index_stop = len(bboxes)
         bboxes = [*bboxes[task_index_start:task_index_stop]]
         logging.info(f'selected task indexes from {task_index_start} to {task_index_stop}')
     elif disbatch:
         assert 'DISBATCH_REPEAT_INDEX' in os.environ
         disbatch_index = int(os.environ['DISBATCH_REPEAT_INDEX'])
+        assert disbatch_index < len(bboxes), f'DISBATCH_REPEAT_INDEX is larger than the task number!'
         bboxes = [bboxes[disbatch_index],]
         logging.info(f'selected a task with disBatch index {disbatch_index}')
         
     # write out as a file
     # this could be used for iteration in slurm cluster.
     if file_path:
         if not file_path.endswith('.npy'):
@@ -146,34 +171,34 @@
         queue = SQSQueue(queue_name)
         queue.send_message_list(bboxes)
     else:
         for bbox_index, bbox in enumerate(bboxes):
             if disbatch:
                 assert len(bboxes) == 1
                 bbox_index = disbatch_index
-            print(f'executing task {bbox_index+task_index_start} in {bbox_num+task_index_start} with bounding box: {bbox.to_filename()}')
-            logging.info(f'executing task {bbox_index+task_index_start} in {bbox_num+task_index_start} with bounding box: {bbox.to_filename()}')
+            print(f'executing task {bbox_index+task_index_start} in {bbox_num+task_index_start} with bounding box: {bbox.string}')
+            logging.info(f'executing task {bbox_index+task_index_start} in {bbox_num+task_index_start} with bounding box: {bbox.string}')
             task = get_initial_task()
             task['bbox'] = bbox
             task['bbox_index'] = bbox_index
             task['bbox_num'] = bbox_num
-            task['log']['bbox'] = bbox.to_filename()
+            task['log']['bbox'] = bbox.string
             yield task
 
 
 @main.command('adjust-bbox')
 @click.option('--corner-offset', '-c', type=click.INT, nargs=6, default=None,
     help='adjust bounding box corner offset')
 @operator
 def adjust_bbox(tasks, corner_offset: tuple):
     """adjust the corner of bounding box."""
     for task in tasks:
         if task is not None:
             bbox = task['bbox']
-            bbox.adjust_corner(corner_offset)
+            bbox = bbox.adjust_corner(corner_offset)
             logging.info(f'after bounding box adjustment: {bbox.string}')
             task['bbox'] = bbox
         yield task
 
 
 @main.command('skip-task')
 @click.option('--prefix', '-p', required=True, type=str,
@@ -190,16 +215,16 @@
         mode: str, adjust_size: int):
     """if a result file already exists, skip this task."""
     for task in tasks:
         if task is not None:
             bbox = task['bbox']
             if adjust_size is not None:
                 bbox = bbox.clone()
-                bbox.adjust(adjust_size)
-            file_name = prefix + bbox.to_filename() + suffix
+                bbox = bbox.adjust(adjust_size)
+            file_name = prefix + bbox.string + suffix
 
             if 'empty' in mode:
                 if not os.path.exists(file_name) or os.path.getsize(file_name)==0:
                     logging.info(f'file {file_name} do not exist or is empty, skip this task.')
                     task = None
             elif 'missing' in mode:
                 if not os.path.exists(file_name):
@@ -229,24 +254,24 @@
 
     Yields:
         None
     """
     for task in tasks:
         if task is not None:
             bbox = task['bbox']
-            fname = f'{prefix}{bbox.to_filename()}{suffix}'
+            fname = f'{prefix}{bbox.string}{suffix}'
             Path(fname).touch()
         yield task
 
 @main.command('skip-all-zero')
 @click.option('--input-chunk-name', '-i',
     type=str, default=DEFAULT_CHUNK_NAME, help='input chunk name')
 @click.option('--prefix', '-p', type=str, default=None, 
     help = 'pre-path of a file. we would like to keep a trace that this task was executed.')
-@click.option('--suffix', '-s', type=str, default=None,
+@click.option('--suffix', '-s', type=str, default=".h5",
     help='post-path of a file. normally include the extention of result file.')
 @click.option('--adjust-size', '-a', type=click.INT, default=None,
     help='change the bounding box of chunk if it do not match with final result file name.')
 @click.option('--chunk-bbox/--task-bbox', default=True,
     help='use the bbox in task or generate from chunk. Default is using chunk bounding box.')
 @operator
 def skip_all_zero(tasks, input_chunk_name: str, prefix: str, suffix: str, adjust_size: int, chunk_bbox: bool):
@@ -257,16 +282,17 @@
             if not np.any(chunk):
                 logging.info('all zero chunk, skip this task')
                 if prefix is not None or suffix is not None:
                     if chunk_bbox:
                         bbox = chunk.bbox.clone()
                     else:
                         bbox = task['bbox']
-                    bbox.adjust(adjust_size)
-                    fname = f'{prefix}{bbox.to_filename()}{suffix}'
+                    if adjust_size is not None:
+                        bbox = bbox.adjust(adjust_size)
+                    fname = f'{prefix}{bbox.string}{suffix}'
                     if not os.path.exists(fname):
                         logging.info(f'create an empty file as mark: {fname}')
                         Path(fname).touch()
                 # target task as None and task will be skipped
                 task = None
         yield task
 
@@ -286,15 +312,15 @@
             if data is None:
                 # target task as None and task will be skipped
                 task = None
                 if touch:
                     assert prefix is not None
                     assert suffix is not None
                     bbox = task['bbox']
-                    fname = f'{prefix}{bbox.to_filename()}{suffix}'
+                    fname = f'{prefix}{bbox.string}{suffix}'
                     Path(fname).touch()
         yield task
 
 
 @main.command('setup-env')
 @click.option('--volume-start', required=True, nargs=3, type=click.INT,
               help='start coordinate of output volume in mip 0')
@@ -358,15 +384,15 @@
     if queue_name is not None and not state['dry_run']:
         queue = SQSQueue(queue_name, visibility_timeout=visibility_timeout)
         queue.send_message_list(bboxes)
     else:
         for bbox in bboxes:
             task = get_initial_task()
             task['bbox'] = bbox
-            task['log']['bbox'] = bbox.to_filename()
+            task['log']['bbox'] = bbox.string
             yield task
 
 
 @main.command('cloud-watch')
 @click.option('--name',
               type=str,
               default='cloud-watch',
@@ -453,15 +479,15 @@
 @click.option('--max-mip', '-m',
               type=click.INT, default=0, 
               help = 'maximum mip level.')
 @operator
 def create_info(tasks,input_chunk_name: str, output_layer_path: str, channel_num: int, 
                 layer_type: str, data_type: str, encoding: str, voxel_size: tuple, 
                 voxel_offset: tuple, volume_size: tuple, block_size: tuple, factor: tuple, max_mip: int):
-    """Create metadata for Neuroglancer Precomputed volume."""
+    """Create attrsdata for Neuroglancer Precomputed volume."""
     
     for task in tasks:
         if task is not None:
             if not input_chunk_name in task:
                 if voxel_offset is None:
                     voxel_offset = Cartesian(0, 0, 0)
             else:
@@ -575,15 +601,15 @@
         bbox = BoundingBox.from_filename(bbox_str)
         
         # record the task handle to delete after the processing
         task = get_initial_task() 
         task['queue'] = queue
         task['task_handle'] = task_handle
         task['bbox'] = bbox
-        task['log']['bbox'] = bbox.to_filename()
+        task['log']['bbox'] = bbox.string
         yield task
 
 
 @main.command('aggregate-skeleton-fragments')
 @click.option('--name', type=str, default='aggregate-skeleton-fragments',
               help='name of operator')
 @click.option('--input-name', '-i', type=str, default='prefix',
@@ -670,23 +696,23 @@
             if os.path.isfile(file_path) and \
                     (file_path.endswith('.h5') or \
                     file_path.endswith('.json')):
                 fname = file_path
             elif os.path.isdir(file_path):
                 bbox = task['bbox']
                 if suffix is not None:
-                    fname = os.path.join(file_path, f'{bbox.to_filename()}{suffix}')
+                    fname = os.path.join(file_path, f'{bbox.string}{suffix}')
                 else:
-                    fname = os.path.join(file_path, f'{bbox.to_filename()}')
+                    fname = os.path.join(file_path, f'{bbox.string}')
                     if not os.path.exists(fname) and '.' not in fname:
                         fname += '.h5'
                         
             elif not os.path.exists(file_path):
                 bbox = task['bbox']
-                fname = f'{file_path}{bbox.to_filename()}{suffix}'
+                fname = f'{file_path}{bbox.string}{suffix}'
             else:
                 fname = file_path
             assert os.path.isfile(fname), f'can not find file: {fname}'
 
             if set_bbox:
                 bbox = BoundingBox.from_string(fname)
                 assert bbox is not None
@@ -707,37 +733,58 @@
                 if syns.pre_num == 0:
                     syns = None
                 task[output_name] = syns
             task['log']['timer'][name] = time() - start
         yield task
 
 
+@main.command('save-points')
+@click.option('--input-name', '-i', type=str, default='point_cloud')
+@click.option('--file-path', '-f',
+    type=click.Path(file_okay=True, dir_okay=True, resolve_path=True),
+    required=True, help='HDF5 file path.')
+@operator
+def save_points(tasks, input_name: str, file_path: str):
+    """Save synapses as HDF5 file."""
+    for task in tasks:
+        if task is not None:
+            points = task[input_name]
+            assert isinstance(points, PointCloud)
+            points.to_h5(file_path)
+        yield task
+
+ 
 @main.command('save-synapses')
 @click.option('--input-name', '-i', type=str, default=DEFAULT_SYNAPSES_NAME)
 @click.option('--file-path', '-f',
     type=click.Path(file_okay=True, dir_okay=True, resolve_path=True),
     required=True, help='HDF5 file path.')
 @operator
 def save_synapses(tasks, input_name: str, file_path: str):
     """Save synapses as HDF5 file."""
     for task in tasks:
         if task is not None:
             syns = task[input_name]
-            if not file_path.endswith('.h5'):
-                if 'bbox' in task:
-                    bbox = task['bbox']
-                    if os.path.isdir(file_path):
-                        file_path = os.path.join(file_path, bbox.string)
-                    else:
-                        file_path += bbox.string
-                file_path += '.h5'
-            if syns is None:
-                Path(file_path).touch()
+            if file_path.endswith('.json'):
+                data = syns.json_dict
+                with open(file_path, 'w') as file:
+                    json.dump(data, file)
             else:
-                syns.to_h5(file_path)
+                if not file_path.endswith('.h5'):
+                    if 'bbox' in task:
+                        bbox = task['bbox']
+                        if os.path.isdir(file_path):
+                            file_path = os.path.join(file_path, bbox.string)
+                        else:
+                            file_path += bbox.string
+                    file_path += '.h5'
+                if syns is None:
+                    Path(file_path).touch()
+                else:
+                    syns.to_h5(file_path)
         yield task
 
 @main.command('load-npy')
 @click.option('--name', '-n', type=str, default='load-npy', help='name of operator')
 @click.option('--file-path', '-f', 
     type=click.Path(file_okay=True, dir_okay=True, resolve_path=True),
     required=True, help='NPY file path')
@@ -748,17 +795,17 @@
     """Read NPY files."""
     for task in tasks:
         if task is not None:
             start = time()
             if not file_path.endswith('.npy'):
                 bbox = task['bbox']
                 if os.path.isdir(file_path):
-                    file_path = os.path.join(file_path, f'{bbox.to_filename()}.npy')
+                    file_path = os.path.join(file_path, f'{bbox.string}.npy')
                 else:
-                    file_path = f'{file_path}{bbox.to_filename()}.npy'
+                    file_path = f'{file_path}{bbox.string}.npy'
             assert os.path.exists(file_path)
             if 0 == os.path.getsize(file_path):
                 task[output_name] = None
             else:
                 with open(file_path, 'rb') as file:
                     array = np.load(file)
                 array *= np.asarray(resolution, dtype=array.dtype)
@@ -777,17 +824,17 @@
     """Read JSON file."""
     for task in tasks:
         if task is not None:
             start = time()
             if not file_path.endswith('.json'):
                 bbox = task['bbox']
                 if os.path.isdir(file_path):
-                    file_path = os.path.join(file_path, f'{bbox.to_filename()}.json')
+                    file_path = os.path.join(file_path, f'{bbox.string}.json')
                 else:
-                    file_path = f'{file_path}{bbox.to_filename()}.json'
+                    file_path = f'{file_path}{bbox.string}.json'
             assert os.path.exists(file_path)
             with open(file_path, 'r') as file:
                 task[output_name] = json.load(file)
             task['log']['timer'][name] = time() - start
         yield task
 
 
@@ -895,15 +942,15 @@
               type=click.Path(exists=True, dir_okay=False),
               help='read chunk from TIFF file.')
 @click.option('--voxel-offset', '-v', type=click.INT, nargs=3, callback=default_none,
               help='global offset of this chunk')
 @click.option('--voxel-size', '-s', type=click.INT, nargs=3, default=None, callback=default_none,
               help='physical size of voxels. The unit is assumed to be nm.')
 @click.option('--dtype', '-d',
-              type=click.Choice(['uint8', 'uint32', 'uint64', 'float32', 'float64', 'float16']),
+              type=click.Choice(['uint8', 'uint16', 'uint32', 'uint64', 'float32', 'float64', 'float16']),
               help='convert to data type')
 @click.option('--output-chunk-name', '-o', type=str, default='chunk',
               help='chunk name in the global state')
 @operator
 def read_tif(tasks, name: str, file_name: str, voxel_offset: tuple,
              voxel_size: tuple, dtype: str, output_chunk_name: str):
     """Read tiff files."""
@@ -965,15 +1012,15 @@
                help='cutout size of the chunk.')
 @click.option('--set-bbox/--no-set-bbox', default=False, 
     help='set up bounding box in the task or not')
 @click.option('--output-chunk-name', '-o',
               type=str, default=DEFAULT_CHUNK_NAME,
               help='chunk name in the global state')
 @operator
-def read_h5(tasks, name: str, file_name: str, dataset_path: str,
+def load_h5(tasks, name: str, file_name: str, dataset_path: str,
             dtype: str, voxel_offset: tuple, voxel_size: tuple, 
             cutout_start: tuple, cutout_stop: tuple, 
             cutout_size: tuple, set_bbox: bool,
             output_chunk_name: str):
     """Read HDF5 files."""
     for task in tasks:
         if task is not None:
@@ -982,15 +1029,15 @@
                 bbox = task['bbox']
                 logging.info(f'bbox: {bbox}')
                 cutout_start_tmp = bbox.minpt
                 cutout_stop_tmp = bbox.maxpt
                 cutout_size_tmp = cutout_stop_tmp - cutout_start_tmp
 
                 if not file_name.endswith('.h5'):
-                    file_name = f'{file_name}{bbox.to_filename()}.h5'
+                    file_name = f'{file_name}{bbox.string}.h5'
             else:
                 cutout_start_tmp = cutout_start
                 cutout_stop_tmp = cutout_stop
                 cutout_size_tmp = cutout_size
 
             chunk = Chunk.from_h5(
                 file_name,
@@ -1026,39 +1073,44 @@
               default="gzip", help="compression used in the dataset.")
 @click.option('--with-offset/--without-offset', default=True, type=bool,
               help='add voxel_offset dataset or not.')
 @click.option('--voxel-size', '-v',
     default=None, type=click.INT, callback=default_none, nargs=3,
     help='voxel size of this chunk.'
 )
+@click.option('--dtype', '-d', default=None, type=str, 
+    help='data type conversion.')
 @click.option('--touch/--no-touch', default=True, 
 help = 'create an empty file if the input is None.'
 )
 @operator
-def save_h5(tasks, input_name, file_name, chunk_size, compression, with_offset, voxel_size, touch):
+def save_h5(tasks, input_name: str, file_name: str, chunk_size: tuple, 
+        compression: str, with_offset: bool, voxel_size: tuple, dtype: str, touch: bool):
     """Save chunk to HDF5 file."""
     for task in tasks:
         if task is not None:
             data = task[input_name]
             if isinstance(data, Chunk):
                 if not file_name.endswith('.h5'):
-                    file_name = f'{file_name}{data.bbox.to_filename()}.h5'
+                    file_name = f'{file_name}{data.bbox.string}.h5'
 
+                if dtype is not None:
+                    data = data.astype(dtype)
                 data.to_h5(
                     file_name, with_offset, 
                     chunk_size=chunk_size, 
                     compression=compression,
                     voxel_size=voxel_size)
             elif isinstance(data, Synapses):
                 data.to_h5(file_name)
             elif data is None:
                 if touch:
                     if not file_name.endswith('.h5'):
                         bbox = task['bbox']
-                        file_name = f'{file_name}{bbox.to_filename()}.h5'
+                        file_name = f'{file_name}{bbox.string}.h5'
                     Path(file_name).touch()
             else:
                 raise ValueError(f'unsuported type of input data: {data}')
         yield task
 
 
 @main.command('save-pngs')
@@ -1184,15 +1236,15 @@
         mip = state['mip']
     assert mip >= 0
 
     if expand_direction is not None:
         # only -1 or 1
         expand_direction = int(expand_direction)
     
-    operator = ReadPrecomputedOperator(
+    operator = LoadPrecomputedOperator(
         volume_path,
         mip=mip,
         expand_margin_size=expand_margin_size,
         expand_direction=expand_direction,
         fill_missing=fill_missing,
         validate_mip=validate_mip,
         blackout_sections=blackout_sections,
@@ -1222,14 +1274,112 @@
             # assert output_chunk_name not in task
             task[output_chunk_name] = operator(bbox)
             task['log']['timer'][name] = time() - start
             task['cutout_volume_path'] = volume_path
         yield task
 
 
+@main.command('load-zarr')
+@click.option('--store', '-f', type=str, required=True,
+    help='Zarr store path')
+@click.option('--path', '-p', type=str, default = None,
+    help = 'Zarr path in the store')
+@click.option('--chunk-start', '-s', type=click.INT, nargs=3, default=None,
+    help='voxel offset or start')
+@click.option('--chunk-size', '-z', type=click.INT, nargs=3, default=None,
+    help='chunk size')
+@click.option('--voxel-size', '-v', type=click.FLOAT, nargs=3, default=None)
+@click.option('--backend', '-b', type=str, default='NestedDirectoryStore',
+    help='the storage backend.')
+@click.option('--output-chunk-name', '-o', type=str, default=DEFAULT_CHUNK_NAME,
+    help='output chunk name.')
+@operator
+def load_zarr(tasks, store: str, path: str, chunk_start: tuple, voxel_size: tuple, 
+        chunk_size: tuple, backend: str, output_chunk_name: str):
+    """Load Zarr arrays."""
+    if backend == 'NestedDirectoryStore':
+        store = zarr.NestedDirectoryStore(store)
+    z = zarr.open(store, mode='r', path=path)
+    attrs = z.attrs.asdict()
+    
+    # Note that this is the physical
+    if 'offset' in attrs:
+        physical_volume_offset = Cartesian.from_collection(attrs['offset'])
+        volume_offset = physical_volume_offset / voxel_size
+    elif 'voxel_offset' in attrs:
+        volume_offset = Cartesian.from_collection(attrs['voxel_offset'])
+    else:
+        print('no voxel offset, set default value: 0x0x0')
+        volume_offset = Cartesian(0, 0, 0)
+
+    if voxel_size is None:
+        if 'resolution' in attrs:
+            voxel_size = Cartesian.from_collection(attrs['resolution'])
+        elif 'voxel_size' in attrs:
+            voxel_size = Cartesian.from_collection(attrs['voxel_size'])
+        else:
+            print('no voxel size, set default value: 1x1x1')
+            voxel_size = Cartesian(1, 1, 1)
+            # raise ValueError(f'no voxel size attribute!')
+    for task in tasks:
+        if task is not None:
+            if chunk_size is None and chunk_start is None and 'bbox' not in task:
+                arr = z[:]
+                voxel_offset = volume_offset
+            else:
+                if chunk_start is not None and chunk_size is not None:
+                    bbox = BoundingBox.from_delta(chunk_start, chunk_size)
+                elif 'bbox' in task:
+                    bbox = task['bbox']
+                    chunk_start = bbox.start
+                    chunk_size = bbox.shape
+                else:
+                    raise ValueError(f'bounding box not defined.')
+                arr_start = bbox.start - volume_offset
+                arr_bbox = BoundingBox.from_delta(arr_start, bbox.shape)
+                arr = z[arr_bbox.slices]
+                voxel_offset = chunk_start
+            chunk = Chunk(arr, voxel_offset=voxel_offset, voxel_size=voxel_size) 
+            task[output_chunk_name] = chunk
+        yield task
+
+
+@main.command('save-zarr')
+@click.option('--store', '-s', type=str, required=True,
+    help = 'Zarr store path')
+@click.option('--shape', '-s', type=click.INT, nargs=3,
+    default=None, callback=default_none,
+    help='shape of the whole volume.')
+@click.option('--input-chunk-name', '-i', type=str, default=DEFAULT_CHUNK_NAME,
+    help='input chunk name.')
+@operator
+def save_zarr(tasks, store: str, shape: tuple, input_chunk_name: str):
+    """Load Zarr arrays."""
+    
+    if os.path.exists(store):
+        zarr_store = zarr.open(store, mode='w')
+    else:
+        assert shape is not None
+        zarr_store = zarr.open(store, mode='w', shape=shape,)
+    for task in tasks:
+        if task is not None:
+            chunk = task[input_chunk_name]
+            if not os.path.exists(store):
+                # create it and store the whole array here.
+                za[:] = chunk.array
+            else:
+                if chunk.ndim == 4: 
+                    za[(slice(None),) + chunk.slices] = chunk.array
+                elif chunk.ndim == 3:
+                    za[chunk.slices] = chunk.array
+                else:
+                    raise ValueError(f'only support 3D and 4D array for now, but get {chunk.ndim}')
+        yield task
+
+
 @main.command('remap-segmentation')
 @click.option('--input-chunk-name', '-i',
     type=str, default=DEFAULT_CHUNK_NAME, help='input chunk name.')
 @click.option('--output-chunk-name', '-o',
     type=str, default=DEFAULT_CHUNK_NAME, help='output chunk name.')
 @operator
 def remap_segmentation(tasks, input_chunk_name, output_chunk_name):
@@ -1270,14 +1420,44 @@
         if task is not None:
             seg = Segmentation(task[segmentation_chunk_name])
             groundtruth = Segmentation(task[groundtruth_chunk_name])
             task[output] = seg.evaluate(groundtruth)
         yield task
 
 
+@main.command('downsample')
+@click.option('--input-chunk-name', '-i', type=str, default=DEFAULT_CHUNK_NAME,
+    help = 'input chunk name')
+@click.option('--output-chunk-name', '-o', type=str, default=DEFAULT_CHUNK_NAME,
+    help='output chunk name')
+@click.option('--factor', '-f', type=click.INT, nargs=3, default=(2,2,2),
+    help='downsample factor in zyx. The default is 2x2x2.')
+@operator
+def downsample(tasks, input_chunk_name: str, output_chunk_name: str, factor: tuple):
+    for task in tasks:
+        if task is not None:
+            chunk = task[input_chunk_name]
+            if chunk.is_image:
+                arr = tinybrain.downsample_with_averaging(chunk.array, factor)[0]
+            elif chunk.is_segmentation:
+                arr = tinybrain.downsample_segmentation(chunk.array, factor)[0]
+            else:
+                raise TypeError(f'only support image or segmentation, but got: {chunk.dtype}')
+                
+            factor = Cartesian.from_collection(factor)
+            voxel_offset = chunk.voxel_offset // factor
+            voxel_size = chunk.voxel_size * factor
+
+            output_chunk = Chunk(arr, 
+                voxel_offset=voxel_offset,
+                voxel_size=voxel_size,
+                layer_type=chunk.layer_type)
+            task[output_chunk_name] = output_chunk
+        yield task
+
 @main.command('downsample-upload')
 @click.option('--name',
               type=str, default='downsample-upload', help='name of operator')
 @click.option('--input-chunk-name', '-i',
               type=str, default='chunk', help='input chunk name')
 @click.option('--volume-path', '-v', type=str, help='path of output volume')
 @click.option('--factor', '-f', type=click.INT, nargs=3, default=(2, 2, 2), 
@@ -1367,47 +1547,51 @@
             chunk /= 127.5
             chunk -= 1.0
             task[output_chunk_name] = chunk
             task['log']['timer'][name] = time() - start
         yield task
 
 
-@main.command('normalize-contrast-nkem')
+@main.command('normalize-contrast')
 @click.option('--name', type=str, default='normalize-contrast-nkem',
               help='name of operator.')
 @click.option('--input-chunk-name', '-i',
               type=str, default=DEFAULT_CHUNK_NAME, help='input chunk name')
 @click.option('--output-chunk-name', '-o',
               type=str, default=DEFAULT_CHUNK_NAME, help='output chunk name')
-@click.option('--levels-path', '-p', type=str, required=True,
-              help='the path of section histograms.')
 @click.option('--lower-clip-fraction', '-l', type=click.FLOAT, default=0.01, 
               help='lower intensity fraction to clip out.')
 @click.option('--upper-clip-fraction', '-u', type=click.FLOAT, default=0.01, 
               help='upper intensity fraction to clip out.')
 @click.option('--minval', type=click.INT, default=1, 
               help='the minimum intensity of transformed chunk.')
 @click.option('--maxval', type=click.INT, default=255,
               help='the maximum intensity of transformed chunk.')
+@click.option('--per-section/--whole', default=True, 
+help='per section normalization or normalize the whole chunk.')
 @operator
-def normalize_contrast_nkem(tasks, name, input_chunk_name, output_chunk_name, 
-                                levels_path, lower_clip_fraction,
-                                upper_clip_fraction, minval, maxval):
+def normalize_contrast(tasks, 
+        name: str, input_chunk_name: str, output_chunk_name: str, 
+        lower_clip_fraction: float, upper_clip_fraction: float, 
+        minval: int, maxval: int, per_section: bool):
     """Normalize the section contrast using precomputed histograms."""
     
-    operator = NormalizeSectionContrastOperator(
-        levels_path,
-        lower_clip_fraction=lower_clip_fraction,
-        upper_clip_fraction=upper_clip_fraction,
-        minval=minval, maxval=maxval, name=name)
-
     for task in tasks:
         if task is not None:
             start = time()
-            task[output_chunk_name] = operator(task[input_chunk_name])
+            chunk = task[input_chunk_name]
+            chunk = chunk.clone()
+            chunk = Image.from_chunk(chunk)
+            chunk.normalize_contrast(
+                lower_clip_fraction=lower_clip_fraction,
+                upper_clip_fraction=upper_clip_fraction,
+                minval=minval,
+                maxval=maxval,
+                per_section=per_section) 
+            task[output_chunk_name] = chunk
             task['log']['timer'][name] = time() - start
         yield task
 
 
 @main.command('normalize-section-shang')
 @click.option('--name',
               type=str,
@@ -1432,24 +1616,20 @@
 @operator
 def normalize_section_shang(tasks, name, input_chunk_name, output_chunk_name, 
                             nominalmin, nominalmax, clipvalues):
     """Normalize voxel values based on slice min/max within the chunk, Shang's method.
     The transformed chunk has floating point values.
     """
 
-    operator = NormalizeSectionShangOperator(
-        nominalmin=nominalmin,
-        nominalmax=nominalmax,
-        clipvalues=clipvalues,
-        name=name)
-
     for task in tasks:
         if task is not None:
             start = time()
-            task[output_chunk_name] = operator(task[input_chunk_name])
+            chunk = task[input_chunk_name]
+            chunk = chunk.normalize_section_shang(nominalmin, nominalmax, clipvalues)
+            task[output_chunk_name] = chunk
             task['log']['timer'][name] = time() - start
         yield task
 
 
 @main.command('plugin')
 @click.option('--name',
               type=str,
@@ -1474,15 +1654,20 @@
     operator = Plugin(file, name=name)
 
     for task in tasks:
         if task is not None:
             start = time()
             if input_names is not None:
                 input_name_list = input_names.split(',')
-                inputs = [task[i] for i in input_name_list]
+                inputs = []
+                for input_name in input_name_list:
+                    if input_name == 'None':
+                        inputs.append(None)
+                    else:
+                        inputs.append(task[input_name])
             else:
                 inputs = []
             outputs = operator(inputs, args=args)
             if isinstance(outputs, list) or isinstance(outputs, tuple): 
                 output_name_list = output_names.split(',')
                 assert len(outputs) == len(output_name_list)
                 for output_name, output in zip(output_name_list, outputs):
@@ -1624,23 +1809,24 @@
 @click.option('--input-names', '-i', type=str, default=DEFAULT_CHUNK_NAME)
 @click.option('--output-names', '-o', type=str, default=None)
 @click.option('--multiplier-name', '-m', type=str, required=True,
     help='multiplier chunk name.')
 @operator
 def multiply(tasks, input_names: str, output_names: str, multiplier_name: str):
     """Multiply chunks with another chunk"""
+    input_names = input_names.split(',')
     if output_names is None:
         output_names = input_names
+    else:
+        output_names = output_names.split(',')
+        assert len(input_names)==len(output_names), \
+            'the number of input and output chunks should be the same'
 
     for task in tasks:
         if task is not None:
-            input_names = input_names.split(',')
-            output_names = output_names.split(',')
-            assert len(input_names)==len(output_names), \
-                'the number of input and output chunks should be the same'
             for input_name, output_name in zip(input_names, output_names):
                 task[output_name] = task[input_name] * task[multiplier_name]
         
         yield task
 
 
 @main.command('mask')
@@ -1736,18 +1922,18 @@
         yield task
 
 
 @main.command('crop-margin')
 @click.option('--name', type=str, default='crop-margin',
     help='name of this operator')
 @click.option('--margin-size', '-m',
-    type=click.INT, nargs=3, default=None, callback=default_none,
+    type=click.INT, nargs=6, default=None, callback=default_none,
     help='crop the chunk margin. ' +
             'The default is None and will use the bbox as croping range.')
-@click.option('--crop-bbox/--no-crop-bbox', default=True,
+@click.option('--crop-bbox/--no-crop-bbox', default=False,
     help='adjust the bounding box or not.')
 @click.option('--input-chunk-name', '-i',
     type=str, default='chunk', help='input chunk name.')
 @click.option('--output-chunk-name', '-o',
     type=str, default='chunk', help='output chunk name.')
 @operator
 def crop_margin(tasks, name: str, margin_size: tuple, crop_bbox: bool, 
@@ -1759,19 +1945,19 @@
             if margin_size:
                 task[output_chunk_name] = task[
                     input_chunk_name].crop_margin(
                     margin_size=margin_size)
                 if crop_bbox and 'bbox' in task:
                     bbox = task['bbox']
                     assert isinstance(bbox, BoundingBox)
-                    bbox.adjust(-Cartesian.from_collection(margin_size))
+                    bbox = bbox.adjust(-Cartesian.from_collection(margin_size))
             else:
                 # use the output bbox for croping 
                 task[output_chunk_name] = task[
-                    input_chunk_name].cutout(task['bbox'].to_slices())
+                    input_chunk_name].cutout(task['bbox'].slices)
             task['log']['timer'][name] = time() - start
         yield task
 
 
 @main.command('mesh')
 @click.option('--name', type=str, default='mesh', help='name of operator')
 @click.option('--input-chunk-name', '-i',
@@ -1948,35 +2134,40 @@
 @click.option('--create-thumbnail/--no-create-thumbnail',
     default=False, help='create thumbnail or not. ' +
     'the thumbnail is a downsampled and quantized version of the chunk.')
 @click.option('--intensity-threshold', '-t',
     default=None, type=click.FLOAT,
     help='do not save anything if all voxel intensity is below threshold.'
 )
+@click.option('--fill-missing/--no-fill', default=False,
+    help='save blocks with all zeros or not. Default is not.')
 @operator
 def save_precomputed(tasks, name: str, volume_path: str, 
         input_chunk_name: str, mip: int, upload_log: bool, 
-        create_thumbnail: bool, intensity_threshold: float):
+        create_thumbnail: bool, intensity_threshold: float,
+        fill_missing: bool):
     """Save chunk to volume."""
     if mip is None:
         mip = state['mip']
 
     operator = SavePrecomputedOperator(
         volume_path,
         mip,
         upload_log=upload_log,
         create_thumbnail=create_thumbnail,
-        name=name
+        name=name,
+        fill_missing=fill_missing,
     )
 
     for task in tasks:
         if task is not None:
             # the time elapsed was recorded internally
             chunk = task[input_chunk_name]
             if intensity_threshold is not None and np.all(chunk.array < intensity_threshold):
+                print(f'average intensity lower than threshold, skip this task.')
                 pass
             else:
                 operator(chunk, log=task.get('log', {'timer': {}}))
                 # task['output_volume_path'] = volume_path
 
         yield task
 
@@ -2002,19 +2193,18 @@
             logging.info('Segment probability map using a threshold...')
             task[output_chunk_name] = task[input_chunk_name].threshold(threshold)
             task['log']['timer'][name] = time() - start
         yield task
 
 
 @main.command('channel-voting')
-@click.option('--name', type=str, default='channel-voting', help='name of operator')
-@click.option('--input-chunk-name', type=str, default=DEFAULT_CHUNK_NAME)
-@click.option('--output-chunk-name', type=str, default=DEFAULT_CHUNK_NAME)
+@click.option('--input-chunk-name', '-i', type=str, default=DEFAULT_CHUNK_NAME)
+@click.option('--output-chunk-name', '-o', type=str, default=DEFAULT_CHUNK_NAME)
 @operator
-def channel_voting(tasks, name, input_chunk_name, output_chunk_name):
+def channel_voting(tasks, input_chunk_name, output_chunk_name):
     """all channels vote to get a uint8 volume. The channel with max intensity wins."""
     for task in tasks:
         task[output_chunk_name] = task[input_chunk_name].channel_voting() 
         yield task
 
 
 @main.command('view')
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/load_pngs.py` & `chunkflow-1.1.5/chunkflow/flow/load_pngs.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/load_precomputed.py` & `chunkflow-1.1.5/chunkflow/flow/load_precomputed.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
 from chunkflow.chunk.validate import validate_by_template_matching
 from tinybrain import downsample_with_averaging
 from chunkflow.chunk import Chunk
 from .base import OperatorBase
 
 
-class ReadPrecomputedOperator(OperatorBase):
+class LoadPrecomputedOperator(OperatorBase):
     def __init__(self,
                  volume_path: str,
                  mip: int = 0,
                  expand_margin_size: Cartesian=Cartesian(0, 0, 0),
                  expand_direction: int = None,
                  fill_missing: bool = False,
                  validate_mip: int = None,
@@ -60,16 +60,16 @@
             #parallel=True,
         
     def __call__(self, output_bbox: BoundingBox):
         # if we do not clone this bounding box, 
         # the bounding box in task will be modified!
         assert isinstance(output_bbox, BoundingBox)
         output_bbox = output_bbox.clone()
-        output_bbox.adjust(self.expand_margin_size)
-        chunk_slices = output_bbox.to_slices()
+        output_bbox = output_bbox.adjust(self.expand_margin_size)
+        chunk_slices = output_bbox.slices
         
         if self.dry_run:
             # input_bbox = BoundingBox.from_slices(chunk_slices)
             # we can not use pattern=zero since it might got skipped by 
             # the operator of skip-all-zero
             return Chunk.from_bbox(
                 output_bbox,
@@ -94,18 +94,20 @@
         # if the channel number is 1, squeeze it as 3d array
         # this should not be neccessary
         # TODO: remove this step and use 4D array all over this package.
         # always use 4D array will simplify some operations
         # voxel_offset = Cartesian(s.start for s in chunk_slices)
         if chunk.shape[0] == 1:
             chunk = np.squeeze(chunk, axis=0)
-
+        
         chunk = Chunk(
-            chunk, voxel_offset=output_bbox.start,
-            voxel_size=Cartesian.from_collection(self.vol.resolution[::-1]))
+            chunk, 
+            voxel_offset=output_bbox.start,
+            voxel_size=Cartesian.from_collection(self.vol.resolution[::-1]),
+            layer_type=self.vol.layer_type)
 
         if self.blackout_sections:
             chunk = self._blackout_sections(chunk)
 
         if self.validate_mip:
             self._validate_chunk(chunk)
         
@@ -185,13 +187,13 @@
         # because of the rounding error of integer division
         for _ in range(self.validate_mip - chunk_mip):
             clamped_input = downsample_with_averaging(clamped_input, (2, 2, 1))
 
         # validation by template matching
         assert validate_by_template_matching(clamped_input)
 
-        validate_input = validate_vol[validate_bbox.to_slices()]
+        validate_input = validate_vol[validate_bbox.slices]
         if validate_input.shape[3] == 1:
             validate_input = np.squeeze(validate_input, axis=3)
 
         # use the validate input to check the downloaded input
         assert np.alltrue(validate_input == clamped_input)
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/log_summary.py` & `chunkflow-1.1.5/chunkflow/flow/log_summary.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/mask.py` & `chunkflow-1.1.5/chunkflow/flow/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def _read_mask_in_high_mip(self, chunk_bbox, factor):
         """
         chunk_bbox: the bounding box of the chunk in lower mip level
         """
         # print("download mask chunk...")
         # make sure that the slices only contains zyx without channel
-        chunk_slices = chunk_bbox.to_slices()[-3:]
+        chunk_slices = chunk_bbox.slices[-3:]
 
         # only scale the indices in XY plane
         # only scale the indices in XY plane
         mask_slices = tuple(
             slice(a.start // f, a.stop // f)
             for a, f in zip(chunk_slices[-3:], factor))
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/mesh.py` & `chunkflow-1.1.5/chunkflow/flow/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
             np.amax(mesh.vertices, axis=0)
         )
         return data, mesh_bounds
 
     def _get_file_name(self, bbox, obj_id):
         if self.output_format == 'precomputed':
             # bbox is in z,y,x order, should transform to x,y,z order 
-            bbox2 = Bbox.from_slices(bbox.to_slices()[::-1])
-            return '{}:0:{}'.format(obj_id, bbox2.to_filename())
+            bbox2 = Bbox.from_slices(bbox.slices[::-1])
+            return '{}:0:{}'.format(obj_id, bbox2.string)
         elif self.output_format == 'ply':
             return '{}.ply'.format(obj_id)
         elif self.output_format == 'obj':
             return '{}.obj'.format(obj_id)
         else:
             raise ValueError('unsupported format!')
 
@@ -148,22 +148,22 @@
             for obj_id in self.mesher.ids():
                 data, mesh_bbox = self._get_mesh_data(obj_id, bbox.minpt)
                 meshes.append(data)
                 mesh_bboxes[obj_id] = mesh_bbox.to_list()
 
             # use shared format in default!
             self.storage.put(
-                f"{self.mesh_path}/{bbox.to_filename()}.frags",
+                f"{self.mesh_path}/{bbox.string}.frags",
                 content=pickle.dumps(meshes),
                 compress='gzip',
                 content_type="application/python-pickle",
                 cache_control=False,
             )
             self.storage.put_json(
-                f"{self.mesh_path}/{bbox.to_filename()}.spatial",
+                f"{self.mesh_path}/{bbox.string}.spatial",
                 mesh_bboxes,
                 compress='gzip',
                 cache_control=False,
             )
         else:
             if 'precomputed' in self.output_format:
                 compress = 'gzip'
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/mesh_manifest.py` & `chunkflow-1.1.5/chunkflow/flow/mesh_manifest.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/neuroglancer.py` & `chunkflow-1.1.5/chunkflow/flow/neuroglancer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import neuroglancer as ng
 import numpy as np
 
 from chunkflow.chunk import Chunk
 from chunkflow.lib.synapses import Synapses
+from chunkflow.point_cloud import PointCloud
 
 from .base import OperatorBase
 
 
 class NeuroglancerOperator(OperatorBase):
     def __init__(self,
                  name: str = 'neuroglancer',
@@ -71,35 +72,48 @@
   setColor(prop_color());
   setPointMarkerSize(prop_size());
 }
 ''',
             ),
         )
 
-        self._append_point_annotation_layer(viewer_state, name + '_pre', pre_synapses)
+        self._append_point_annotation_layer(
+            viewer_state, name + '_pre', pre_synapses)
 
 
 
-    def _append_point_annotation_layer(self, viewer_state: ng.viewer_state.ViewerState, name: str, points: np.ndarray):
+    def _append_point_annotation_layer(self, 
+            viewer_state: ng.viewer_state.ViewerState, 
+            name: str, points: PointCloud, 
+            color: str = '#ff0', size: int = 8):
         annotations = []
         
-        for sid in range(points.shape[0]):
+        for sid in range(points.point_num):
             # we would like to show line first and then the presynapse point
             # so, we have distinct color to show T-bar
             pre_annotation = ng.PointAnnotation(
                 id=str(sid),
-                point=points[sid, :].tolist(),
-                props=['#ff0', 8]
+                point=points.points[sid, :].tolist(),
+                props=[color, size]
             )
             annotations.append(pre_annotation)
 
         viewer_state.layers.append(
             name=name,
             layer=ng.LocalAnnotationLayer(
-                dimensions=ng.CoordinateSpace(names=['z', 'y', 'x'], units="nm", scales=(1, 1, 1)),
+                dimensions=ng.CoordinateSpace(
+                    names=['z', 'y', 'x'], 
+                    units="nm", 
+                    #scales=(1, 1, 1)
+                    scales=(
+                        points.voxel_size.z, 
+                        points.voxel_size.y, 
+                        points.voxel_size.x, 
+                    )
+                ),
                 annotation_properties=[
                     ng.AnnotationPropertySpec(
                         id='color',
                         type='rgb',
                         default='red',
                     ),
                     ng.AnnotationPropertySpec(
@@ -121,23 +135,27 @@
     def _append_image_layer(self, viewer_state: ng.viewer_state.ViewerState, chunk_name: str, chunk: Chunk):
         voxel_size = self._get_voxel_size(chunk)
         dimensions = ng.CoordinateSpace(
             scales=voxel_size,
             units=['nm', 'nm', 'nm'],
             names=['z', 'y', 'x']
         )
-        shader="""#uicontrol int channel slider(min=0, max=4)
-#uicontrol vec3 color color(default="white")
-#uicontrol float brightness slider(min=-1, max=1)
-#uicontrol float contrast slider(min=-3, max=3, step=0.01)
+        shader="""#uicontrol invlerp normalized
 void main() {
-  emitRGB(color *
-          (toNormalized(getDataValue(channel)) + brightness) *
-          exp(contrast));
+  emitGrayscale(normalized());
 }"""
+#         shader="""#uicontrol int channel slider(min=0, max=4)
+# #uicontrol vec3 color color(default="white")
+# #uicontrol float brightness slider(min=-1, max=1)
+# #uicontrol float contrast slider(min=-3, max=3, step=0.01)
+# void main() {
+#   emitRGB(color *
+#           (toNormalized(getDataValue(channel)) + brightness) *
+#           exp(contrast));
+# }"""
         viewer_state.layers.append(
             name=chunk_name,
             layer=ng.LocalVolume(
                 data=chunk,
                 dimensions=dimensions,
                 # offset is in nm, not voxels
                 voxel_offset=chunk.voxel_offset,
@@ -145,14 +163,16 @@
             shader=shader
         )
 
     def _append_segmentation_layer(self, viewer_state: ng.viewer_state.ViewerState, chunk_name: str, chunk: Chunk):
         if np.issubdtype(chunk.dtype, np.int64):
             assert chunk.min() >= 0
             chunk = chunk.astype(np.uint64)
+        elif np.issubdtype(chunk.dtype, np.uint8):
+            chunk = chunk.astype(np.uint32)
         voxel_size = self._get_voxel_size(chunk)
         dimensions = ng.CoordinateSpace(
             scales=voxel_size,
             units=['nm', 'nm', 'nm'],
             names=['z', 'y', 'x']
         )       
         viewer_state.layers.append(
@@ -223,30 +243,49 @@
         ng.set_server_bind_address(bind_address='0.0.0.0', bind_port=self.port)
         viewer = ng.Viewer()
         with viewer.txn() as viewer_state:
             for name in selected:
                 data = datas[name]
                 if data is None:
                     continue
+                elif isinstance(data, PointCloud):
+                    # points
+                    self._append_point_annotation_layer(viewer_state, name, data)
                 elif isinstance(data, Synapses):
                     # this could be synapses
                     self._append_synapse_annotation_layer(viewer_state, name, data)
                 elif isinstance(data, np.ndarray) and 2 == data.ndim and 3 == data.shape[1]:
                     # points
                     self._append_point_annotation_layer(viewer_state, name, data)
-                elif data.is_image or (data.ndim==3 and np.issubdtype(data.dtype, np.floating)):
-                    self._append_image_layer(viewer_state, name, data)
-                elif data.is_segmentation:
-                    self._append_segmentation_layer(viewer_state, name, data)
-                elif data.is_probability_map:
-                    self._append_probability_map_layer(viewer_state, name, data)
+                elif isinstance(data, Chunk):
+                    if data.layer_type is None:
+                        if data.is_image or data.is_affinity_map:
+                            self._append_image_layer(viewer_state, name, data)
+                        elif data.is_segmentation:
+                            self._append_segmentation_layer(viewer_state, name, data)
+                        elif data.is_probability_map:
+                            self._append_probability_map_layer(viewer_state, name, data)
+                        else:
+                            raise ValueError('unsupported data type.')
+                    if data.layer_type == 'segmentation':
+                        self._append_segmentation_layer(viewer_state, name, data)
+                    elif data.layer_type == 'probability_map':
+                        self._append_probability_map_layer(viewer_state, name, data)
+                    elif data.layer_type in set(['image', 'affinity_map']):
+                        self._append_image_layer(viewer_state, name, data)
+                    else: 
+                        raise ValueError('only support image, affinity map, probability_map, and segmentation for now.')
+
                 else:
                     breakpoint()
                     raise ValueError(f'do not support this type: {type(data)}')
 
         print('Open this url in browser: ')
         viewer_url = viewer.get_viewer_url()
+        if '.fios-router.home' in viewer_url:
+            _, _, address2 = viewer_url.split(':')
+            viewer_url = 'http://localhost:' + address2
         print(viewer_url)
 
         key = None
         while key!='q':
             key = input('Press q and enter/return to quit neuroglancer.')
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/normalize_section_contrast.py` & `chunkflow-1.1.5/chunkflow/chunk/image/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,41 @@
-# -*- coding: utf-8 -*-
-import json
-import numpy as np
-from cloudfiles import CloudFiles
-from chunkflow.chunk import Chunk
+__doc__ = """Image chunk class"""
 
-from .base import OperatorBase
+from tqdm import tqdm
+import numpy as np
 
+from chunkflow.chunk import Chunk
+from .adjust_grey import normalize_section_shang
+from .convnet.inferencer import Inferencer
 
-class NormalizeSectionContrastOperator(OperatorBase):
-    """Contrast Correction based on LuminanceLevelsTask output.
 
-    Note that this operator was modified from Will's ContrastNormalizationTask in igneous:
-    https://github.com/seung-lab/igneous/blob/master/igneous/tasks.py#L735
+class Image(Chunk):
     """
-    def __init__(self,
-                 levels_path: str,
-                 lower_clip_fraction: float = 0.01,
-                 upper_clip_fraction: float = 0.01,
-                 minval: int = 1,
-                 maxval: int = np.iinfo(np.uint8).max,
-                 #maxval: int = np.iinfo(np.uint32).max,
-                 name: str = 'normalize-contrast'):
-        """
-        levels_path: (str) path of section histogram files.
-        clip_fraction: (float) the fraction of intensity to be clamped.
-        minval: (float)
-        maxval: (float) Note that the original algorithm use default maxval as 
-                float(np.iinfo(np.float32)).max. It is meaningless to use value 
-                larger than the max value of uint8.
-        """
-        super().__init__(name=name)
-        assert 0 <= lower_clip_fraction <= 1
-        assert 0 <= upper_clip_fraction <= 1
-        assert lower_clip_fraction + upper_clip_fraction <= 1
-
-        self.levels_path = levels_path
-        self.lower_clip_fraction = float(lower_clip_fraction)
-        self.upper_clip_fraction = float(upper_clip_fraction)
-
-        self.minval = minval
-        self.maxval = maxval
-       
-        # intensity value lookup table cache
-        self.lookup_tables = dict()
-        self.stor = CloudFiles(self.levels_path)
-
-    def __call__(self, chunk):
-        # this is a image, not affinitymap
-        assert chunk.ndim == 3
-        # we have to use np.dtype function to make it match
-        # https://stackoverflow.com/questions/26921836/correct-way-to-test-for-numpy-dtype
-        assert chunk.dtype is np.dtype(np.uint8)
-        
-        for z in range(chunk.bbox.minpt[-3], chunk.bbox.maxpt[-3]):
-            lookup_table = self.fetch_lookup_table(z)
-            slices = (slice(z, z+1), *chunk.slices[-2:])
-            image = chunk.cutout(slices)
-            image_voxel_offset = image.voxel_offset
-            image = lookup_table[tuple(image)]
-            image = np.expand_dims(image, 0)
-            assert image.ndim == 3
-            image = Chunk(image, voxel_offset=image_voxel_offset)
-            chunk.save(image)
+    a chunk of image volume.
+    """
+    def __init__(self, array: np.ndarray, **kwargs):
+        super().__init__(array, **kwargs)
 
-        return chunk
+    @classmethod
+    def from_chunk(cls, chk: Chunk):
+        return cls(chk.array, **chk.properties)
+
+    def inference(self, inferencer: Inferencer):
+        """run convolutional net inference for this image chunk"""
+        return inferencer(self)
+
+    def normalize_section_shang(self, nominalmin, nominalmax, clipvalues):
+        return normalize_section_shang(self.array, nominalmin, nominalmax,
+                                       clipvalues)
 
-    def find_section_clamping_values(self, zlevel):
+    def _find_section_clamping_values(self, 
+            hist: np.ndarray, lower_clip_fraction: float, upper_clip_fraction: float):
         """compute the clamping values for each section."""
         # remove the np.copy from original code since we only need this once
-        filtered = zlevel
+        filtered = hist
 
         # remove pure black from frequency counts as
         # it has no information in our images
         filtered[0] = 0
 
         cdf = np.zeros(shape=(len(filtered), ), dtype=np.uint64)
         cdf[0] = filtered[0]
@@ -82,44 +45,89 @@
         total = cdf[-1]
 
         if total == 0:
             return (0, 0)
 
         lower = 0
         for i, val in enumerate(cdf):
-            if float(val) / float(total) > self.lower_clip_fraction:
+            if float(val) / float(total) > lower_clip_fraction:
                 break
             lower = i
 
         upper = 0
         for i, val in enumerate(cdf):
-            if float(val) / float(total) > 1 - self.upper_clip_fraction:
+            if float(val) / float(total) > 1 - upper_clip_fraction:
                 break
             upper = i
         
         return lower, upper
+    
+    def _hist_to_lookup_table(self, 
+            hist: np.ndarray, lower_clip_fraction: float, upper_clip_fraction: float,
+            minval: int = 1,
+            maxval: int = 255):
+        """histogram to lookup table
 
-    def fetch_lookup_table(self, z):
-        """
-        readout the histograms in each corresponding section.
-        lookup tables are constructed and cached.
+        Args:
+            hist (np.ndarray): histogram
+
+        Returns:
+            np.ndarray: lookup table
         """
-        if z not in self.lookup_tables:
-            data = self.stor.get(f'{z}')
-            assert data is not None, f'histogram of section {z} is missing!'
-            data = json.loads(data.decode('utf-8'))
-            levels = np.array(data['levels'], dtype=np.uint64)
-            lower, upper = self.find_section_clamping_values(levels)
+        lower, upper = self._find_section_clamping_values(
+            hist, lower_clip_fraction, upper_clip_fraction)
              
-            if lower == upper:
-                lookup_table = np.arange(0, 256, dtype=np.uint8)
-            else:
-                # compute the lookup table
-                lookup_table = np.arange(0, 256, dtype=np.float32)
-                lookup_table = (lookup_table - float(lower)) * (
-                    self.maxval / (float(upper) - float(lower)))
-            np.clip(lookup_table, self.minval, self.maxval, out=lookup_table)
+        if lower == upper:
+            #lookup_table = np.arange(0, 256, dtype=np.uint8)
+            # no need to perform any transform
+            return None
+        else:
+            # compute the lookup table
+            lookup_table = np.arange(0, 256, dtype=np.float32)
+            lookup_table = (lookup_table - float(lower)) * (
+                maxval / (float(upper) - float(lower)))
+            np.clip(lookup_table, minval, maxval, out=lookup_table)
             lookup_table = np.round(lookup_table)
             lookup_table = lookup_table.astype( np.uint8 ) 
-            
-            self.lookup_tables[z] = lookup_table
-        return self.lookup_tables[z]
+            return lookup_table
+
+
+    def normalize_contrast(self, 
+            lower_clip_fraction: float = 0.01, 
+            upper_clip_fraction: float = 0.01,
+            minval: int = 1,
+            maxval: int = 255,
+            per_section: bool = True
+            ):
+
+        def _normalize_array(array: np.ndarray, 
+                lower_clip_fraction: float, 
+                upper_clip_fraction: float,
+                minval: int = 1,
+                maxval: int = 255):
+            hist = np.bincount(array.flatten(), minlength=255)
+            lookup_table = self._hist_to_lookup_table(
+                hist, lower_clip_fraction, upper_clip_fraction, 
+                minval=minval, maxval=maxval)
+            if lookup_table is not None:
+                array = lookup_table[array]
+            return array
+        
+
+        if per_section:
+            for z in tqdm(range(self.bbox.start.z, self.bbox.stop.z)):
+                slices = (slice(z, z+1), *self.slices[-2:])
+                section = self.cutout(slices)
+                # section = Image.from_chunk(section)
+                section.array = _normalize_array(
+                    section.array,
+                    lower_clip_fraction, upper_clip_fraction,
+                    minval=minval, maxval=maxval
+                )
+                self.save(section)
+            else:
+                # chunk = Image.from_chunk(chunk)
+                self.array = _normalize_array(
+                    self.array,
+                    lower_clip_fraction, upper_clip_fraction,
+                    minval=minval, maxval=maxval 
+                )
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/plugin.py` & `chunkflow-1.1.5/chunkflow/flow/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 import os.path as path
-from ast import literal_eval
 from typing import Union
 
 import numpy as np
 
 from chunkflow.lib.cartesian_coordinate import Cartesian
+from chunkflow.lib.utils import str_to_dict
 
 from .base import OperatorBase
 
 from chunkflow.lib import load_source
 from chunkflow.chunk import Chunk
+from chunkflow.point_cloud import PointCloud
+
 
 def array_to_chunk(arr: Union[np.ndarray, Chunk], voxel_offset: Cartesian, 
         voxel_size: Cartesian, shape: tuple):
     if isinstance(arr, np.ndarray):
         # in case the plugin did some symmetric cropping
         offset = tuple(vo + (ins - outs)//2 for vo, ins, outs in zip(voxel_offset, shape[-3:], arr.shape[-3:]) )
         return Chunk(arr, voxel_offset=offset, voxel_size=voxel_size)
     else:
         return arr
 
-def simplest_type(s: str):
-    try:
-        return literal_eval(s)
-    except:
-        return s
 
 class Plugin(OperatorBase):
     r"""
     Chunk operation using a custom python file.
     """
     def __init__(self, plugin_file_name: str,
                  name: str = 'plugin-1'):
@@ -73,22 +70,16 @@
         shape = None
         for inp in inputs:
             if isinstance(inp, Chunk):
                 voxel_offset = inp.voxel_offset
                 voxel_size = inp.voxel_size
                 shape = inp.shape
                 break
-        if args is not None:
-            if '=' in args:
-                keywords = {}
-                for item in args.split(';'):
-                    assert '=' in item
-                    item = item.split('=')
-                    keywords[item[0]] = simplest_type(item[1])
-                args = keywords
+        if args is not None and '=' in args:
+            args = str_to_dict(args)
 
         if len(inputs) == 0 and args is None:
             outputs = self.execute()
         elif len(inputs) == 0 and args is not None:
             if isinstance(args, str):
                 outputs = self.execute(args=args)
             elif isinstance(args, dict):
@@ -110,14 +101,16 @@
             outputs = [*outputs] 
         # automatically convert the ndarrays to Chunks
         if voxel_offset is not None and outputs is not None:
             assert shape is not None
             if isinstance(outputs, list) or isinstance(outputs, tuple):
                 for idx, output in enumerate(outputs):
                     outputs[idx] = array_to_chunk(output, voxel_offset, voxel_size, shape)
+            elif isinstance(outputs, PointCloud):
+                pass
             elif isinstance(outputs, np.ndarray):
                     outputs = array_to_chunk(outputs, voxel_offset, voxel_size, shape)
             elif isinstance(outputs, Chunk):
                 # this is good
                 pass
             else:
                 # will return outputs as is
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/save_pngs.py` & `chunkflow-1.1.5/chunkflow/flow/save_pngs.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/save_precomputed.py` & `chunkflow-1.1.5/chunkflow/flow/save_precomputed.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 
 class SavePrecomputedOperator(OperatorBase):
     def __init__(self,
                  volume_path: str,
                  mip: int,
                  upload_log: bool = True,
                  create_thumbnail: bool = False,
-                intensity_threshold: int = None,
+                 fill_missing: bool = False,
                  name: str = 'save-precomputed'):
         super().__init__(name=name)
         
         self.upload_log = upload_log
         self.create_thumbnail = create_thumbnail
         self.mip = mip
-        self.intensity_threshold = intensity_threshold
 
         # if not volume_path.startswith('precomputed://'):
         #     volume_path += 'precomputed://'
         self.volume_path = volume_path
         
         # gevent.monkey.patch_all(thread=False)
         self.volume = CloudVolume(
             self.volume_path,
-            fill_missing=True,
+            fill_missing=fill_missing,
             bounded=False,
             autocrop=True,
             mip=self.mip,
             cache=False,
             green_threads=True,
             delete_black_uploads=True,
             progress=True)
@@ -56,24 +55,19 @@
         """Create a fake all zero chunk. 
         this is used in skip some operation based on mask."""
         shape = (num_channels, *bbox.size3())
         arr = np.zeros(shape, dtype=dtype)
         chunk = Chunk(arr, voxel_offset=(0, *bbox.minpt))
         return chunk
 
-    def __call__(self, chunk, log=None):
+    def __call__(self, chunk: Chunk, log=None):
         assert isinstance(chunk, Chunk)
         logging.info('save chunk.')
         
         start = time.time()
-        
-        if self.intensity_threshold is not None and np.all(chunk.array < self.intensity_threshold):
-            print('the voxel intensity in this chunk are all below intensity threshold, return directly without saving anything.')
-            return 
-
         chunk = self._auto_convert_dtype(chunk, self.volume)
         
         # transpose czyx to xyzc order
         arr = np.transpose(chunk.array)
         self.volume[chunk.slices[::-1]] = arr
         
         if self.create_thumbnail:
@@ -146,10 +140,10 @@
     def _upload_log(self, log, output_bbox):
         assert log
         assert isinstance(output_bbox, BoundingBox)
 
         logging.info(f'uploaded log: {log}')
 
         # write to google cloud storage
-        self.log_storage.put_json(output_bbox.to_filename() +
+        self.log_storage.put_json(output_bbox.string +
                                   '.json',
                                   content=json.dumps(log))
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/setup_env.py` & `chunkflow-1.1.5/chunkflow/flow/setup_env.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/flow/skeletonize.py` & `chunkflow-1.1.5/chunkflow/flow/skeletonize.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,12 +27,12 @@
             print('no segmentation, skip computation.')
             return None
  
         logging.info('skeletonize segmentation...')
       
         seg = Segmentation.from_chunk(seg)
         skels = seg.skeletonize(voxel_size)
-        bbox_str = seg.bbox.to_filename()
+        bbox_str = seg.bbox.string
         for neuron_id, skel in skels.items():
             file_name = f'{neuron_id}:{bbox_str}'
             self.storage.put(file_name, skel.to_precomputed())
         return skels
```

### Comparing `chunkflow-1.1.4/chunkflow/flow/view.py` & `chunkflow-1.1.5/chunkflow/flow/view.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/lib/aws/cloud_watch.py` & `chunkflow-1.1.5/chunkflow/lib/aws/cloud_watch.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/lib/aws/sqs_queue.py` & `chunkflow-1.1.5/chunkflow/lib/aws/sqs_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             a list of input messages. the messages are string.
         '''
         # the maximum number in a batch is 10
         task_entries = []
         for mid, message in tqdm(enumerate(message_list), 
                                  desc='sending messages to sqs queue: '):
             if isinstance(message, BoundingBox):
-                message = message.to_filename()
+                message = message.string
 
             entry = {'Id': str(mid), 'MessageBody': message}
             task_entries.append(entry)
 
             # use batch mode to produce tasks
             if len(task_entries) == 10:
                 self._send_entry_list(task_entries)
```

### Comparing `chunkflow-1.1.4/chunkflow/lib/cartesian_coordinate.py` & `chunkflow-1.1.5/chunkflow/lib/cartesian_coordinate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # support the class method with parameter type of itself
 from __future__ import annotations
 
+import random
 import logging
 import os
 from collections import UserList, namedtuple
 from math import ceil, floor
-from typing import Union
+from typing import Union, List
 from numbers import Number
 import itertools
+from functools import cached_property
 import re
-
+from dataclasses import dataclass
 from copy import deepcopy
 
 import numpy as np
 import h5py
 
 from cloudvolume import CloudVolume
 from cloudvolume.lib import Vec, Bbox
@@ -29,24 +31,25 @@
 
 class Cartesian(namedtuple('Cartesian', ['z', 'y', 'x'])):
     """Cartesian coordinate or offset."""
     __slots__ = ()
 
     @classmethod
     def from_collection(cls, col: Union[tuple, list, Vec]):
+        assert len(col) == 3
         return cls(*col)
 
     @property
     def ceil(self):
         return Cartesian(ceil(self.z), ceil(self.y), ceil(self.x))
     
     @property
     def floor(self):
         return Cartesian(floor(self.z), floor(self.y), floor(self.x))
-
+    
     def __hash__(self):
         return hash((self.z, self.y, self.x))
 
     def __eq__(self, other: Union[int, tuple, Cartesian]) -> bool:
         if isinstance(other, int):
             return np.all([x==other for x in self])
         elif isinstance(other, Cartesian) or isinstance(other, tuple):
@@ -168,31 +171,40 @@
     @property
     def vec(self):
         return Vec(*self)
 
     @property
     def tuple(self):
         return (self.z, self.y, self.x)
+    
+    @property
+    def list(self):
+        return [self.z, self.y, self.x]
 
 
-class BoundingBox(Bbox):
-    def __init__(self, 
-            minpt: Union[list, Cartesian],
-            maxpt: Union[list, Cartesian],
-            dtype: np.dtype =None):
-        if isinstance(minpt, Cartesian):
-            minpt = minpt.vec
+@dataclass(frozen=True)
+class BoundingBox():
+    start: Cartesian
+    stop: Cartesian
+    # def __post_init__(self, start, stop) -> BoundingBox:
+    #     if not isinstance(start, Cartesian):
+    #         assert len(start) == 3
+    #         start = Cartesian.from_collection(start)
+    #     if not isinstance(stop, Cartesian):
+    #         assert len(stop) == 3
+    #         stop = Cartesian.from_collection(stop)
+    #     self.__setattr__('start', start)
+    #     self.__setattr__('stop', stop)
         
-        if isinstance(maxpt, Cartesian):
-            maxpt = maxpt.vec
-        super().__init__(minpt, maxpt, dtype=dtype)
-
     @classmethod
     def from_bbox(cls, bbox: Bbox):
-        return cls(bbox.minpt, bbox.maxpt)
+        assert isinstance(bbox, Bbox)
+        start = Cartesian.from_collection(bbox.minpt)
+        stop  = Cartesian.from_collection(bbox.maxpt)
+        return cls(start, stop)
     
     @classmethod
     def from_string(cls, string: str):
         match = BOUNDING_BOX_RE.search(string)
         if match is None:
             return None
         else:
@@ -201,29 +213,28 @@
             )
             start = Cartesian(zstart, ystart, xstart)
             stop = Cartesian(zstop, ystop, xstop)
             return cls(start, stop)
 
     @classmethod
     def from_delta(cls, 
-            minpt: Union[list, tuple, Cartesian, np.ndarray], 
+            start: Union[list, tuple, Cartesian, np.ndarray], 
             plus: Union[list, tuple, Cartesian, np.ndarray]):
-        bbox = super().from_delta(minpt, plus)
-        return cls.from_bbox(bbox)
+        if not isinstance(start, Cartesian):
+            start = Cartesian.from_collection(start)
+        if not isinstance(plus, Cartesian):
+            plus = Cartesian.from_collection(plus)
+        stop = start + plus
+        return cls(start, stop)
 
     @classmethod
     def from_list(cls, lst: list):
-        bbox = Bbox.from_list(lst)
-        return cls.from_bbox(bbox)
-
-    @classmethod
-    def from_vec(cls, arr: np.ndarray):
-        assert len(arr) == 3
-        bbox = Bbox.from_vec(arr)
-        return cls.from_bbox(bbox)
+        start = Cartesian.from_collection(lst[:3])
+        stop  = Cartesian.from_collection(lst[-3:])
+        return cls(start, stop)
 
     @classmethod
     def from_points(cls, arr: np.ndarray):
         bbox = Bbox.from_points(arr)
         return cls.from_bbox(bbox)
 
     @classmethod
@@ -237,91 +248,184 @@
         """Create bounding box from center and extent
 
         Args:
             center (Cartesian): center coordinate
             extent (int): the range to extent, like radius
             even_size (bool): produce even size or odd size including the center.
         """
-        minpt = center - extent
+        start = center - extent
         # the maxpt is not inclusive, so we need +1
-        maxpt = center + extent
+        stop = center + extent
         if not even_size:
             # this will make the size to be odd
-            maxpt += 1
-        return cls(minpt, maxpt)
+            stop += 1
+        return cls(start, stop)
 
-    @property
+    @cached_property
     def string(self):
-        return self.to_filename()
+        bbox = Bbox(self.start, self.stop)
+        return bbox.to_filename()
+    
+    # @property
+    # def center(self) -> Cartesian:
+    #     ct = (self.minpt + self.maxpt) // 2
+    #     ct = Cartesian.from_collection(ct)
+    #     return ct
 
     @property
-    def start(self):
-        return Cartesian.from_collection(self.minpt)
+    def minpt(self) -> Cartesian:
+        return self.start
     
     @property
-    def stop(self):
-        return Cartesian.from_collection(self.maxpt)
+    def maxpt(self) -> Cartesian:
+        return self.stop
+
+    @cached_property
+    def slices(self):
+        return (
+            slice(self.start.z, self.stop.z),
+            slice(self.start.y, self.stop.y),
+            slice(self.start.x, self.stop.x),
+        )
 
     @property
+    def random_coordinate(self) -> Cartesian:
+        """find a random coordinate inside this bounding box
+
+        Returns:
+            Cartesian: the coordinate inside this bounding box
+        """
+        z = random.randrange(self.start.z, self.stop.z)
+        y = random.randrange(self.start.y, self.stop.y)
+        x = random.randrange(self.start.x, self.stop.x)
+        return Cartesian(z, y, x)
+
+    @cached_property
     def shape(self):
         return self.stop - self.start
-        
+
+    def get_aligned_block_bounding_boxes(self, 
+            block_size: Cartesian) -> BoundingBoxes:
+        bboxes = BoundingBoxes()
+        for z in range(self.start.z, self.stop.z-block_size.z, block_size.z):
+            for y in range(self.start.y, self.stop.y-block_size.y, block_size.y):
+                for x in range(self.start.x, self.stop.x-block_size.x, block_size.x):
+                    bbox = BoundingBox.from_delta(Cartesian(z,y,x), block_size)
+                    bboxes.append(bbox)
+        return bboxes
+    
+    def get_unaligned_block_bounding_boxes(self, 
+            block_size: Cartesian) -> BoundingBoxes:
+        bboxes = BoundingBoxes()
+        for z in range(self.start.z, self.stop.z, block_size.z):
+            for y in range(self.start.y, self.stop.y, block_size.y):
+                for x in range(self.start.x, self.stop.x, block_size.x):
+                    block_start = Cartesian(z,y,x)
+                    block_stop = block_start + block_size
+                    # the block stop can not exceed the boundary of volume
+                    block_stop = block_stop.intersection(
+                        BoundingBox(block_start, self.stop)
+                    )
+                    bbox = BoundingBox(block_start, block_stop)
+                    bboxes.append(bbox)
+        return bboxes
+       
     def __repr__(self):
-        return f'BoundingBox({self.minpt}, {self.maxpt}, dtype={self.dtype}'
+        return f'BoundingBox({self.start}, {self.stop}'
+
+    def __mul__(self, operand: Cartesian | int):
+        assert isinstance(operand, int) or isinstance(operand, Cartesian)
+        start = self.start * operand
+        stop = self.stop * operand
+        return BoundingBox(start, stop)
+
+    def __floordiv__(self, other: int | Cartesian | BoundingBox) -> BoundingBox:
+        if isinstance(other, int) or isinstance(other, Cartesian):
+            minpt = self.minpt // other
+            maxpt = self.maxpt // other
+        elif isinstance(other, BoundingBox):
+            minpt = self.minpt // other.minpt
+            maxpt = self.maxpt // other.maxpt
+        elif isinstance(other, np.ndarray):
+            other  = Cartesian.from_collection(other)
+            minpt = self.start // other
+            maxpt = self.stop // other
+        else:
+            raise ValueError(f'unsupported type of operand: {type(other)}')
+        return BoundingBox(minpt, maxpt)
+         
+    def __ifloordiv__(self, other: BoundingBox | int | Cartesian):
+        return self // other
+
+    def inverse_order(self):
+        start = self.start[::-1]
+        stop  = self.stop[::-1]
+        return BoundingBox(start, stop)
 
     def clone(self):
-        bbox = Bbox(self.minpt, self.maxpt, dtype=self.dtype)
-        bbox = bbox.clone()
-        return BoundingBox.from_bbox(bbox)
+        return BoundingBox(self.start, self.stop)
 
     def adjust(self, size: Union[Cartesian, int, tuple, list, Vec]):
         if size is None:
             logging.warn('adjusting bounding box size is None!')
             return self
 
         if not isinstance(size, int):
-            assert len(size)==3 or len(size)==6
+            assert len(size)==3 
             size = Vec(*size)
         else:
             size = Cartesian(size, size, size)
-        self.minpt -= size[:3]
-        self.maxpt += size[-3:]
-        return self
+        start = self.minpt - size[:3]
+        stop  = self.maxpt + size[-3:]
+        return BoundingBox(start, stop)
 
     def adjust_corner(self, corner_offset: Union[tuple, list]):
-        if corner_offset is not None:
-            assert len(corner_offset) == 6
-            self.minpt += Cartesian.from_collection(corner_offset[:3])
-            self.maxpt += Cartesian.from_collection(corner_offset[-3:])
+        assert corner_offset is not None
+        assert len(corner_offset) == 6
+        start = self.start + Cartesian.from_collection(corner_offset[:3])
+        stop  = self.stop + Cartesian.from_collection(corner_offset[-3:])
+        return BoundingBox(start, stop)
 
-    def union(self, bbox2):
+    def union(self, bbox2: BoundingBox):
         """Merge another bounding box
 
         Args:
             bbox2 (Union[BoundingBox, Bbox]): another bounding box
 
         Returns:
             BoundingBox: bounding box after merging
         """
-
-        self.minpt = np.minimum(self.minpt, bbox2.minpt)
-        self.maxpt = np.maximum(self.maxpt, bbox2.maxpt)
-        return self
+        minpt = np.minimum(self.minpt, bbox2.minpt)
+        maxpt = np.maximum(self.maxpt, bbox2.maxpt)
+        start = Cartesian.from_collection(minpt)
+        stop  = Cartesian.from_collection(maxpt)
+        return BoundingBox(start, stop)
+
+    def intersection(self, bbox2: BoundingBox):
+        minpt = np.maximum(self.minpt, bbox2.minpt)
+        maxpt = np.minimum(self.maxpt, bbox2.maxpt)
+        start = Cartesian.from_collection(minpt)
+        stop  = Cartesian.from_collection(maxpt)
+        return BoundingBox(start, stop)
 
     def contains(self, point: Union[tuple, Vec, list]):
         assert 3 == len(point)
         return np.all(np.asarray(
             (self.maxpt >= Vec(*point)))) and np.all(
                 np.asarray((self.minpt <= Vec(*point)))) 
 
     @property
     def shape(self):
         return Cartesian(*(self.maxpt - self.minpt))
 
     @property
+    def slices(self):
+        return tuple(slice(x0, x1) for x0, x1 in zip(self.start, self.stop))
+
+    @property
     def left_neighbors(self):
         sz = self.size3()
 
         minpt = deepcopy(self.minpt)
         minpt[0] -= sz[0]
         bbox_z = self.from_delta(minpt, sz)
 
@@ -332,31 +436,34 @@
         minpt = deepcopy(self.minpt)
         minpt[2] -= sz[2]
         bbox_x = self.from_delta(minpt, sz)
         return bbox_z, bbox_y, bbox_x
 
     
 class BoundingBoxes(UserList):
-    def __init__(self, bboxes: list) -> None:
-        super().__init__()
-        self.data = bboxes
+    # def __init__(self, iterable) -> None:
+    #     super().__init__(
+    #         item for item in iterable if isinstance(item, BoundingBox)
+    #     )
 
     @classmethod
     def from_manual_setup(cls,
             chunk_size:Union[Vec, tuple], 
             chunk_overlap: Union[Vec, tuple, Cartesian]=Cartesian(0,0,0),
             roi_start: Union[Vec, tuple, Cartesian]=None, 
             roi_stop: Union[Vec, tuple, Cartesian]=None, 
             roi_size: Union[Vec, tuple, Cartesian]=None,
             grid_size: Union[Vec, tuple, Cartesian]=None,
             respect_chunk_size: bool = True,
             aligned_block_size: Union[Vec, tuple, Cartesian]=None,
             bounded: bool = False,
             layer_path: str = None,
-            mip: int = 0):
+            mip: int = 0,
+            use_https: bool = False,
+            ):
 
         if not layer_path:
             if grid_size is None and roi_size is None and roi_stop is None:
                 grid_size = Cartesian(1, 1, 1)
 
             if roi_start is None:
                 roi_start = Cartesian(0, 0, 0)
@@ -378,15 +485,15 @@
                 if roi_start is None:
                     roi_start = Cartesian(0, 0, 0)
                 if roi_size is None and chunk_size is not None:
                     roi_size = Cartesian.from_collection(chunk_size)
 
                 roi_stop = roi_start + roi_size
             else:
-                vol = CloudVolume(layer_path, mip=mip)
+                vol = CloudVolume(layer_path, mip=mip, use_https=use_https)
                 # dataset shape as z,y,x
                 dataset_size = vol.mip_shape(mip)[:3][::-1]
                 dataset_offset = vol.mip_voxel_offset(mip)[::-1]
                 dataset_size = Cartesian.from_collection(dataset_size)
                 dataset_offset = Cartesian.from_collection(dataset_offset)
 
                 if roi_size is None:
@@ -505,8 +612,39 @@
     def to_file(self, file_name: str) -> None:
         if file_name.endswith('.npy'):
             np.save(file_name, self.as_array())
         else:
             raise ValueError('only support npy format now.')
 
     def __len__(self):
-        return len(self.data)
+        return len(self.data)
+
+
+@dataclass(frozen=True)
+class PhysicalBoudingBox(BoundingBox):
+    voxel_size: Cartesian
+   
+    @classmethod
+    def from_bounding_box(cls, bbox: BoundingBox, 
+            voxel_size: Cartesian) -> PhysicalBoudingBox:
+        return cls(bbox.start, bbox.stop, 
+            voxel_size)
+        
+    @cached_property
+    def voxel_bounding_box(self) -> BoundingBox:
+        return BoundingBox(self.start, self.stop)
+    
+    def to_other_voxel_size(self, voxel_size2: Cartesian) -> PhysicalBoudingBox:
+        assert voxel_size2 != self.voxel_size
+        
+        if voxel_size2 >= self.voxel_size:
+
+            factors = voxel_size2 // self.voxel_size
+            start = self.start // factors
+            stop = self.stop // factors
+        else:
+            factors = self.voxel_size // voxel_size2
+            start = self.start * factors
+            stop = self.stop * factors
+        return PhysicalBoudingBox(start, stop, voxel_size2)
+
+
```

### Comparing `chunkflow-1.1.4/chunkflow/lib/flow.py` & `chunkflow-1.1.5/chunkflow/lib/flow.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/lib/gala/evaluate.py` & `chunkflow-1.1.5/chunkflow/lib/gala/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -616,56 +616,14 @@
         else:
             coords2 = coords
         sx = x.ravel()[coords2]
         sy = y.ravel()[coords2]
         return eval_fct(sx, sy, *args, **kwargs)
     return special_eval_fct
 
-
-def make_synaptic_functions(fn, fcts):
-    """Make evaluation functions that only evaluate at synaptic sites.
-
-    Parameters
-    ----------
-    fn : string
-        Filename containing synapse coordinates, in Raveler format. [1]
-    fcts : function, or iterable of functions
-        Functions to be converted to synaptic evaluation.
-
-    Returns
-    -------
-    syn_fcts : function or iterable of functions
-        Evaluation functions that will evaluate only at synaptic sites.
-
-    Raises
-    ------
-    ImportError : if the `syngeo` package [2, 3] is not installed.
-
-    References
-    ----------
-    [1] https://wiki.janelia.org/wiki/display/flyem/synapse+annotation+file+format
-    [2] https://github.com/janelia-flyem/synapse-geometry
-    [3] https://github.com/jni/synapse-geometry
-    """
-    from syngeo import io as synio
-    synapse_coords = \
-        synio.raveler_synapse_annotations_to_coords(fn, 'arrays')
-    synapse_coords = np.array(list(it.chain(*synapse_coords)))
-    make_function = partial(special_points_evaluate, coords=synapse_coords)
-    if not isinstance(fcts, coll.Iterable):
-        return make_function(fcts)
-    else:
-        return list(map(make_function, fcts))
-
-
-def make_synaptic_vi(fn):
-    """Shortcut for `make_synaptic_functions(fn, split_vi)`."""
-    return make_synaptic_functions(fn, split_vi)
-
-
 def vi(x, y=None, weights=np.ones(2), ignore_x=[0], ignore_y=[0]):
     """Return the variation of information metric. [1]
 
     VI(X, Y) = H(X | Y) + H(Y | X), where H(.|.) denotes the conditional
     entropy.
 
     Parameters
```

### Comparing `chunkflow-1.1.4/chunkflow/lib/igneous/downsample.py` & `chunkflow-1.1.5/chunkflow/lib/igneous/downsample.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/lib/igneous/downsample_scales.py` & `chunkflow-1.1.5/chunkflow/lib/igneous/downsample_scales.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/chunkflow/lib/igneous/tasks.py` & `chunkflow-1.1.5/chunkflow/lib/igneous/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-import time
-import json
-import math
-import os
-import random
-import re
-# from tempfile import NamedTemporaryFile  # used by BigArrayTask
-
-# from backports import lzma               # used by HyperSquareTask
-# import blosc                             # used by BigArrayTask
-# import h5py                              # used by BigArrayTask
-
 import numpy as np
 
+from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
 from cloudvolume.lib import min2, Vec
 
 from . import downsample, downsample_scales
 
 
 def downsample_and_upload(image,
                           bounds,
@@ -58,23 +47,24 @@
             "No factors generated. Image Shape: {}, Downsample Shape: {}, Volume Shape: {}, Bounds: {}"
             .format(image.shape, ds_shape, vol.volume_size, bounds))
 
     downsamplefn = downsample.method(vol.layer_type, sparse=sparse)
 
     vol.mip = mip
     if not skip_first:
-        vol[bounds.to_slices()] = image
+        vol[bounds.slices] = image
 
     new_bounds = bounds.clone()
 
     for factor3 in factors:
         vol.mip += 1
         image = downsamplefn(image, factor3)
         new_bounds //= factor3
-        new_bounds.maxpt = new_bounds.minpt + Vec(*image.shape[:3])
+        delta = Cartesian.from_collection(image.shape[:3])
+        new_bounds = BoundingBox.from_delta(new_bounds.start, delta)
         if factor3 is factors[-1]:
             # this is the last mip level
-            vol[new_bounds.to_slices()] = image
+            vol[new_bounds.slices] = image
         else:
             # this is not the last mip level
             if not only_last_mip:
-                vol[new_bounds.to_slices()] = image
+                vol[new_bounds.slices] = image
```

### Comparing `chunkflow-1.1.4/chunkflow/lib/region_of_interest.py` & `chunkflow-1.1.5/chunkflow/lib/region_of_interest.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         minpt = tuple( p * s1 // s2 for p, s1, s2 in zip(
             self.minpt, self.voxel_size, voxel_size
         ))
         maxpt = tuple( p * s1 // s2 for p, s1, s2 in zip(
             self.maxpt, self.voxel_size, voxel_size
         ))
         bbox = BoundingBox(minpt, maxpt)
-        return bbox.to_slices()
+        return bbox.slices
 
 
 class ROITree:
     def __init__(self, roi: RegionOfInterest, axis: int,
             left: ROITree, right: ROITree):
         """Split the volume hierarchically using a modified aligned K-D tree
 
@@ -96,32 +96,34 @@
 
         Args:
             roi (RegionOfInterest): the total roi covered by this tree.
             factor (Cartesian): downsampling factor in each level.
             atomic_block_size (Cartesian): the size of the leaf node/block
             atomic_voxel_size (Cartesian): the voxel size of leaf block
         """
-        assert roi.voxel_size % atomic_voxel_size == Cartesian(0, 0, 0)
-        assert roi.voxel_size // atomic_voxel_size % factor == Cartesian(0, 0, 0)
+        pass
+
+        # assert roi.voxel_size % atomic_voxel_size == Cartesian(0, 0, 0)
+        # assert roi.voxel_size // atomic_voxel_size % factor == Cartesian(0, 0, 0)
         
-        if roi.voxel_size == atomic_voxel_size:
-            # this is the leaf roi/block
-            return cls(roi, None, None, None)
-
-        # find the relatively longest axis to split
-        children_voxel_size = roi.voxel_size // factor
-        block_nums = roi.physical_size / (children_voxel_size *  )
-        block_nums = np.ceil(block_nums)
-        axis = np.argmax(block_nums)
-
-        # split along axis
-        left_start = roi.start * factor
-        left_block_nums = 
-        left_stop = left_start + 
-        left_roi = RegionOfInterest()
-        left = cls.from_roi(left_roi, factor, atomic_block_size, atomic_voxel_size)
+        # if roi.voxel_size == atomic_voxel_size:
+        #     # this is the leaf roi/block
+        #     return cls(roi, None, None, None)
+
+        # # find the relatively longest axis to split
+        # children_voxel_size = roi.voxel_size // factor
+        # block_nums = roi.physical_size / (children_voxel_size *  )
+        # block_nums = np.ceil(block_nums)
+        # axis = np.argmax(block_nums)
+
+        # # split along axis
+        # left_start = roi.start * factor
+        # left_block_nums = 
+        # left_stop = left_start + 
+        # left_roi = RegionOfInterest()
+        # left = cls.from_roi(left_roi, factor, atomic_block_size, atomic_voxel_size)
 
 
 
     @property
     def is_leaf(self):
         return self.axis is None
```

### Comparing `chunkflow-1.1.4/chunkflow/lib/synapses.py` & `chunkflow-1.1.5/chunkflow/lib/synapses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
 import os
 import json
 import time
-from typing import List
 from copy import deepcopy
+from typing import List
 
 import numpy as np
 import h5py
-
 from scipy.spatial import KDTree
 
 import chunkflow
 from chunkflow.chunk import Chunk
-from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
+from chunkflow.lib.cartesian_coordinate import Cartesian, BoundingBox
 
 
 class Synapses():
     def __init__(self, 
             pre: np.ndarray,
             pre_confidence: np.ndarray = None, 
             post: np.ndarray = None, 
@@ -297,14 +296,24 @@
             pre_users = pre_users,
             post_users = post_users,
         )
         if not c_order:
             # transform to C order
             syns.transpose_axis()
         return syns
+    
+    @classmethod
+    def from_file(cls, fname: str, resolution: tuple = None, c_order: bool = True):
+        assert os.path.exists(fname)
+        if fname.endswith('.json'):
+            return cls.from_json(fname, resolution = resolution, c_order=c_order)
+        elif fname.endswith('.h5'):
+            return cls.from_h5(fname, resolution=resolution, c_order=c_order)
+        else:
+            raise ValueError(f'only support JSON and HDF5 file, but got {fname}')
 
     def to_h5(self, fname: str) -> None:
         """save to a HDF5 file
 
         Args:
             fname (str): the file name to be saved
         """
@@ -330,24 +339,82 @@
                 hf.attrs['users'] = ';'.join(self.users)
 
             if self.pre_users is not None:
                 hf['pre_users'] = self.pre_users
             if self.post_users is not None:
                 hf['post_users'] = self.post_users
 
-    @classmethod
-    def from_file(cls, fname: str, resolution: tuple = None, c_order: bool = True):
-        assert os.path.exists(fname)
-        if fname.endswith('.json'):
-            return cls.from_json(fname, resolution = resolution, c_order=c_order)
-        elif fname.endswith('.h5'):
-            return cls.from_h5(fname, resolution=resolution, c_order=c_order)
-        else:
-            raise ValueError(f'only support JSON and HDF5 file, but got {fname}')
+    @property
+    def json_dict(self):
+        """to JSON file
+        """
+        data = {}
+        data['pre'] = self.pre.tolist()
+        if self.post is not None:
+            data['post'] = self.post.tolist()
+        
+        if self.pre_confidence is not None:
+            data['pre_confidence'] = self.pre_confidence.tolist()
+        
+        if self.post_confidence is not None:
+            data['post_confidence'] = self.post_confidence.tolist()
+        
+        return data
 
+    def to_dvid_list_of_dict(self, 
+            user: str = 'chunkflow',
+            comment: str = 'ingested using chunkflow'):
+        """convert to dictionary for bulk ingestion of synapses
+        """
+        data = []
+
+        for post_idx in range(self.post_num):
+            pre_idx = self.post[post_idx, 0]
+            pre_coord = self.pre[pre_idx, :][::-1]
+            pre_coord = [int(x) for x in pre_coord]
+
+            post_coord = self.post_coordinates[post_idx, :][::-1]
+            post_coord = [int(x) for x in post_coord]
+            dic = {
+                'Kind': 'PostSyn',
+                'Pos': post_coord,
+                'Prop': {
+                    'annotation': comment,
+                    'conf': str(self.post_confidence[post_idx]),
+                    'user': user
+                },
+                'Rels': [{'Rel': 'PostSynTo', 'To': pre_coord}],
+                'Tags': []
+            }
+            data.append(dic)
+
+        for pre_idx, post_indices in enumerate(self.pre_index2post_indices):
+            rels = []
+            for post_idx in post_indices:
+                post_coord = self.post_coordinates[post_idx, :][::-1]
+                post_coord = [int(x) for x in post_coord]
+                rels.append({
+                    'Rel': 'PreSynTo', 'To': post_coord
+                })
+
+            pre_coord = self.pre[pre_idx, :][::-1]
+            pre_coord = [int(x) for x in pre_coord]
+            data.append({
+                'Kind': 'PreSyn',
+                'Pos': pre_coord,
+                'Prop': {
+                    'annotation': comment,
+                    'conf': str(self.pre_confidence[pre_idx]),
+                    'user': user
+                },
+                'Rels': rels,
+                'Tags': []
+            })
+        return data
+    
     def to_neutu_task(self, fname: str, 
             software_revision: int=4809,
             description: str = "transformed using chunkflow",
             file_version: int = 1,
             body_id: int = None
         ):
         """transform to a JSON file as an input to NeuTu.
@@ -458,21 +525,21 @@
         else:
             return self.post.shape[0]
 
     @property
     def pre_bounding_box(self) -> BoundingBox:
         bbox = BoundingBox.from_points(self.pre)
         # the end point is exclusive
-        bbox.adjust((0,0,0, 1,1,1))
+        bbox = bbox.adjust((0,0,0, 1,1,1))
         return bbox
 
     def post_bounding_box(self) -> BoundingBox:
         bbox = BoundingBox.from_points(self.post_coordinates)
         # the right direction is exclusive
-        bbox.adjust((0,0,0, 1,1,1))
+        bbox = bbox.adjust((0,0,0, 1,1,1))
         return bbox
     
     @property
     def bounding_box(self) -> BoundingBox:
         bbox = self.pre_bounding_box
         bbox.union(self.post_bounding_box)
         return bbox
```

### Comparing `chunkflow-1.1.4/chunkflow.egg-info/PKG-INFO` & `chunkflow-1.1.5/chunkflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,148 @@
 Metadata-Version: 2.1
 Name: chunkflow
-Version: 1.1.4
+Version: 1.1.5
 Summary: Composable image chunk operators to create pipeline for distributed computation.
 Home-page: https://github.com/seung-lab/chunkflow
 Author: Jingpeng Wu
 Author-email: jingpeng.wu@gmail.com
 License: Apache License 2.0
-Description: ![alt text](https://github.com/seung-lab/chunkflow/blob/master/docs/logo/RGB_web/Chunkflow_logo_RBG.jpg?raw=true)
-        ----------------------
-        ![GitHub workflow](https://github.com/seung-lab/chunkflow/actions/workflows/.github/workflows/python-app.yml/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/pychunkflow/badge/?version=latest)](https://pychunkflow.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/chunkflow.svg)](https://badge.fury.io/py/chunkflow)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://hub.docker.com/r/seunglab/chunkflow)
-        [![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fjingpeng_wu)](https://twitter.com/jingpeng_wu)
-        <!---[![Docker Build Status](https://img.shields.io/docker/cloud/build/seunglab/chunkflow.svg)]#(https://hub.docker.com/r/seunglab/chunkflow)--->
-        <!-- [![Build Status](https://travis-ci.org/seung-lab/chunkflow.svg?branch=master)](https://travis-ci.org/seung-lab/chunkflow) -->
-        <!-- [![Coverage Status](https://coveralls.io/repos/github/seung-lab/chunkflow/badge.svg?branch=master)](https://coveralls.io/github/seung-lab/chunkflow?branch=master) -->
-        
-        ## Problem 
-        - Petabyte scale 3D image processing is slow and computationally demanding;
-        - Computation has to be distributed with linear scalability;
-        - Local cluster and public cloud computing are not fully used at the same time;
-        - Duplicated code across a variety of routine tasks is hard to maintain.
-        
-        ## Features
-        - **Composable** operators. The chunk operators could be composed in a command line for flexible usage.
-        - **Hybrid Cloud Distributed** computation in both local and cloud computers. The task scheduling frontend and computationally heavy backend are decoupled using AWS Simple Queue Service. The backend could be any computer with an internet connection and cloud authentication. Benefit from the robust design, the cheap unstable instances (preemptable intance in Google Cloud, spot instance in AWS) could be used to reduce cost by about threefold!
-        - **Petabyte** scale. We have used chunkflow to output over eighteen-petabyte images and scaled up to 3600 nodes with NVIDIA GPUs across three regions in [Google Cloud](https://cloud.google.com/), and chunkflow is still reliable.
-        - Operators work with **3D** image volumes.
-        - You can **plug in** your own code as an operator.
-        
-        Check out the [Documentation](https://pychunkflow.readthedocs.io/en/latest/index.html) for [installation](https://pychunkflow.readthedocs.io/en/latest/install.html) and [usage](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). Try it out by following the [tutorial](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). 
-        
-        ## Image Segmentation Example
-        Perform Convolutional net inference to segment 3D image volume with one single command!
-        
-        ```shell
-        #!/bin/bash
-        
-        chunkflow \
-            load-tif --file-name path/of/image.tif -o image \
-            inference --convnet-model path/of/model.py --convnet-weight-path path/of/weight.pt \
-                --input-patch-size 20 256 256 --output-patch-overlap 4 64 64 --num-output-channels 3 \
-                -f pytorch --batch-size 12 --mask-output-chunk -i image -o affs \
-            plugin -f agglomerate --threshold 0.7 --aff-threshold-low 0.001 --aff-threshold-high 0.9999 -i affs -o seg \
-            neuroglancer -i image,affs,seg -p 33333 -v 30 6 6
-        ```
-        you can see your 3D image and segmentation directly in [Neuroglancer](https://github.com/google/neuroglancer)!
-        
-        ![Image_Segmentation](https://github.com/seung-lab/chunkflow/blob/master/docs/source/_static/image/image_seg.png)
-        
-        ## Composable Operators
-        After installation, You can simply type `chunkflow` and it will list all the operators with help message. We keep adding new operators and will keep it update here. For the detailed usage, please checkout our [Documentation](https://pychunkflow.readthedocs.io/en/latest/).
-        
-        | Operator Name   | Function |
-        | --------------- | -------- |
-        | adjust-bbox 	  | adjust the corner offset of bounding box |
-        | aggregate-skeleton-fragments| Merge skeleton fragments from chunks |
-        | channel-voting  | Vote across channels of semantic map |
-        | cleanup         | remove empty files to clean up storage |
-        | cloud-watch     | Realtime speedometer in AWS CloudWatch |
-        | connected-components | Threshold the boundary map to get a segmentation |
-        | copy-var        | Copy a variable to a new name |
-        | create-chunk    | Create a fake chunk for easy test |
-        | create-info     | Create info file of Neuroglancer Precomputed volume |
-        | crop-margin     | Crop the margin of a chunk |
-        | delete-chunk    | Delete chunk in task to reduce RAM requirement |
-        | delete-task-in-queue | Delete the task in AWS SQS queue |
-        | downsample-upload | Downsample the chunk hierarchically and upload to volume |
-        | download-mesh   | Download meshes from Neuroglancer Precomputed volume |
-        | evaluate-segmentation | Compare segmentation chunks |
-        | fetch-task-from-file | Fetch task from a file |
-        | fetch-task-from-sqs | Fetch task from AWS SQS queue one by one |
-        | generate-tasks  | Generate tasks one by one |
-        | gaussian-filter | 2D Gaussian blurring operated in-place |
-        | inference       | Convolutional net inference |
-        | load-synapses   | Load synapses from a file |
-        | save-synapses   | Save synapses as a HDF5 file. |
-        | log-summary     | Summary of logs |
-        | mark-complete   | mark task completion as an empty file | 
-        | mask            | Black out the chunk based on another mask chunk |
-        | mask-out-objects| Mask out selected or small objects |
-        | multiply 		  | Multiply chunks with another chunk |
-        | mesh            | Build 3D meshes from segmentation chunk |
-        | mesh-manifest   | Collect mesh fragments for object |
-        | neuroglancer    | Visualize chunks using neuroglancer |
-        | normalize-contrast-nkem | Normalize image contrast using histograms |
-        | normalize-intensity | Normalize image intensity to -1:1 |
-        | normalize-section-shang | Normalization algorithm created by Shang |
-        | plugin          | Import local code as a customized operator. |
-        | quantize        | Quantize the affinity map |
-        | load-h5         | Read HDF5 files |
-        | load-npy        | Read NPY files |
-        | load-json       | Read JSON files |
-        | load-pngs       | Read png files |
-        | load-precomputed| Cutout chunk from a local/cloud storage volume |
-        | load-tif        | Read TIFF files |
-        | load-nrrd       | Read NRRD files |
-        | remap-segmentation | Renumber a serials of segmentation chunks |
-        | setup-env       | Prepare storage infor files and produce tasks |
-        | skeletonize     | Create centerlines of objects in a segmentation chunk |
-        | skip-task  	  | If a result file already exists, skip this task |
-        | skip-all-zero   | If a chunk has all zero, skip this task |	
-        | skip-none       | If an item in task is None, skip this task |	
-        | threshold       | Use a threshold to segment the probability map |
-        | view            | Another chunk viewer in browser using CloudVolume |
-        | save-h5        | Save chunk as HDF5 file |
-        | save-pngs      | Save chunk as a serials of png files |
-        | save-precomputed| Save chunk to local/cloud storage volume |
-        | save-tif       | Save chunk as TIFF file |
-        | save-nrrd      | Save chunk as NRRD file |
-        
-        ## Affiliation
-        This package is developed at Princeton University and Flatiron Institute.
-        
-        ## Reference
-        We have a [paper](https://www.nature.com/articles/s41592-021-01088-5) for this repo: 
-        ```bibtex
-        
-        @article{wu_chunkflow_2021,
-        	title = {Chunkflow: hybrid cloud processing of large {3D} images by convolutional nets},
-        	issn = {1548-7105},
-        	shorttitle = {Chunkflow},
-        	url = {https://www.nature.com/articles/s41592-021-01088-5},
-        	doi = {10.1038/s41592-021-01088-5},
-        	journal = {Nature Methods},
-        	author = {Wu, Jingpeng and Silversmith, William M. and Lee, Kisuk and Seung, H. Sebastian},
-        	year = {2021},
-        	pages = {1--2}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![alt text](https://github.com/seung-lab/chunkflow/blob/master/docs/logo/RGB_web/Chunkflow_logo_RBG.jpg?raw=true)
+----------------------
+![GitHub workflow](https://github.com/seung-lab/chunkflow/actions/workflows/.github/workflows/python-app.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/pychunkflow/badge/?version=latest)](https://pychunkflow.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/chunkflow.svg)](https://badge.fury.io/py/chunkflow)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Docker Hub](https://img.shields.io/badge/docker-ready-blue.svg)](https://hub.docker.com/r/seunglab/chunkflow)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fjingpeng_wu)](https://twitter.com/jingpeng_wu)
+<!---[![Docker Build Status](https://img.shields.io/docker/cloud/build/seunglab/chunkflow.svg)]#(https://hub.docker.com/r/seunglab/chunkflow)--->
+<!-- [![Build Status](https://travis-ci.org/seung-lab/chunkflow.svg?branch=master)](https://travis-ci.org/seung-lab/chunkflow) -->
+<!-- [![Coverage Status](https://coveralls.io/repos/github/seung-lab/chunkflow/badge.svg?branch=master)](https://coveralls.io/github/seung-lab/chunkflow?branch=master) -->
+
+## Problem 
+- Petabyte scale 3D image processing is slow and computationally demanding;
+- Computation has to be distributed with linear scalability;
+- Local cluster and public cloud computing are not fully used at the same time;
+- Duplicated code across a variety of routine tasks is hard to maintain.
+
+## Features
+- **Composable** operators. The chunk operators could be composed in a command line for flexible usage.
+- **Hybrid Cloud Distributed** computation in both local and cloud computers. The task scheduling frontend and computationally heavy backend are decoupled using AWS Simple Queue Service. The backend could be any computer with an internet connection and cloud authentication. Benefit from the robust design, the cheap unstable instances (preemptable intance in Google Cloud, spot instance in AWS) could be used to reduce cost by about threefold!
+- **Petabyte** scale. We have used chunkflow to output over eighteen-petabyte images and scaled up to 3600 nodes with NVIDIA GPUs across three regions in [Google Cloud](https://cloud.google.com/), and chunkflow is still reliable.
+- Operators work with **3D** image volumes.
+- You can **plug in** your own code as an operator.
+
+Check out the [Documentation](https://pychunkflow.readthedocs.io/en/latest/index.html) for [installation](https://pychunkflow.readthedocs.io/en/latest/install.html) and [usage](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). Try it out by following the [tutorial](https://pychunkflow.readthedocs.io/en/latest/tutorial.html). 
+
+## Image Segmentation Example
+Perform Convolutional net inference to segment 3D image volume with one single command!
+
+```shell
+#!/bin/bash
+
+chunkflow \
+    load-tif --file-name path/of/image.tif -o image \
+    inference --convnet-model path/of/model.py --convnet-weight-path path/of/weight.pt \
+        --input-patch-size 20 256 256 --output-patch-overlap 4 64 64 --num-output-channels 3 \
+        -f pytorch --batch-size 12 --mask-output-chunk -i image -o affs \
+    plugin -f agglomerate --threshold 0.7 --aff-threshold-low 0.001 --aff-threshold-high 0.9999 -i affs -o seg \
+    neuroglancer -i image,affs,seg -p 33333 -v 30 6 6
+```
+you can see your 3D image and segmentation directly in [Neuroglancer](https://github.com/google/neuroglancer)!
+
+![Image_Segmentation](https://github.com/seung-lab/chunkflow/blob/master/docs/source/_static/image/image_seg.png)
+
+## Composable Operators
+After installation, You can simply type `chunkflow` and it will list all the operators with help message. We keep adding new operators and will keep it update here. For the detailed usage, please checkout our [Documentation](https://pychunkflow.readthedocs.io/en/latest/).
+
+| Operator Name   | Function |
+| --------------- | -------- |
+| adjust-bbox 	  | adjust the corner offset of bounding box |
+| aggregate-skeleton-fragments| Merge skeleton fragments from chunks |
+| channel-voting  | Vote across channels of semantic map |
+| cleanup         | remove empty files to clean up storage |
+| cloud-watch     | Realtime speedometer in AWS CloudWatch |
+| connected-components | Threshold the boundary map to get a segmentation |
+| copy-var        | Copy a variable to a new name |
+| create-chunk    | Create a fake chunk for easy test |
+| create-info     | Create info file of Neuroglancer Precomputed volume |
+| crop-margin     | Crop the margin of a chunk |
+| delete-chunk    | Delete chunk in task to reduce RAM requirement |
+| delete-task-in-queue | Delete the task in AWS SQS queue |
+| downsample-upload | Downsample the chunk hierarchically and upload to volume |
+| download-mesh   | Download meshes from Neuroglancer Precomputed volume |
+| evaluate-segmentation | Compare segmentation chunks |
+| fetch-task-from-file | Fetch task from a file |
+| fetch-task-from-sqs | Fetch task from AWS SQS queue one by one |
+| generate-tasks  | Generate tasks one by one |
+| gaussian-filter | 2D Gaussian blurring operated in-place |
+| inference       | Convolutional net inference |
+| load-synapses   | Load synapses from a file |
+| save-synapses   | Save synapses as a HDF5 file. |
+| save-points     | Save point cloud as a HDF5 file. |
+| log-summary     | Summary of logs |
+| mark-complete   | mark task completion as an empty file | 
+| mask            | Black out the chunk based on another mask chunk |
+| mask-out-objects| Mask out selected or small objects |
+| multiply 		  | Multiply chunks with another chunk |
+| mesh            | Build 3D meshes from segmentation chunk |
+| mesh-manifest   | Collect mesh fragments for object |
+| neuroglancer    | Visualize chunks using neuroglancer |
+| normalize-contrast-nkem | Normalize image contrast using histograms |
+| normalize-intensity | Normalize image intensity to -1:1 |
+| normalize-section-shang | Normalization algorithm created by Shang |
+| plugin          | Import local code as a customized operator. |
+| quantize        | Quantize the affinity map |
+| load-h5         | Read HDF5 files |
+| load-npy        | Read NPY files |
+| load-json       | Read JSON files |
+| load-pngs       | Read png files |
+| load-precomputed| Cutout chunk from a local/cloud storage volume |
+| load-tif        | Read TIFF files |
+| load-nrrd       | Read NRRD files |
+| load-zarr    	  | Read Zarr files |
+| remap-segmentation | Renumber a serials of segmentation chunks |
+| setup-env       | Prepare storage infor files and produce tasks |
+| skeletonize     | Create centerlines of objects in a segmentation chunk |
+| skip-task  	  | If a result file already exists, skip this task |
+| skip-all-zero   | If a chunk has all zero, skip this task |	
+| skip-none       | If an item in task is None, skip this task |	
+| threshold       | Use a threshold to segment the probability map |
+| view            | Another chunk viewer in browser using CloudVolume |
+| save-h5        | Save chunk as HDF5 file |
+| save-pngs      | Save chunk as a serials of png files |
+| save-precomputed| Save chunk to local/cloud storage volume |
+| save-tif       | Save chunk as TIFF file |
+| save-nrrd      | Save chunk as NRRD file |
+
+## Affiliation
+This package is developed at Princeton University and Flatiron Institute.
+
+## Reference
+We have a [paper](https://www.nature.com/articles/s41592-021-01088-5) for this repo: 
+```bibtex
+
+@article{wu_chunkflow_2021,
+	title = {Chunkflow: hybrid cloud processing of large {3D} images by convolutional nets},
+	issn = {1548-7105},
+	shorttitle = {Chunkflow},
+	url = {https://www.nature.com/articles/s41592-021-01088-5},
+	doi = {10.1038/s41592-021-01088-5},
+	journal = {Nature Methods},
+	author = {Wu, Jingpeng and Silversmith, William M. and Lee, Kisuk and Seung, H. Sebastian},
+	year = {2021},
+	pages = {1--2}
+}
+```
```

### Comparing `chunkflow-1.1.4/chunkflow.egg-info/SOURCES.txt` & `chunkflow-1.1.5/chunkflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 chunkflow/__init__.py
 chunkflow/__main__.py
 chunkflow/__version__.py
+chunkflow/point_cloud.py
 chunkflow/volume.py
 chunkflow.egg-info/PKG-INFO
 chunkflow.egg-info/SOURCES.txt
 chunkflow.egg-info/dependency_links.txt
 chunkflow.egg-info/entry_points.txt
 chunkflow.egg-info/not-zip-safe
 chunkflow.egg-info/requires.txt
@@ -42,27 +43,26 @@
 chunkflow/flow/load_pngs.py
 chunkflow/flow/load_precomputed.py
 chunkflow/flow/log_summary.py
 chunkflow/flow/mask.py
 chunkflow/flow/mesh.py
 chunkflow/flow/mesh_manifest.py
 chunkflow/flow/neuroglancer.py
-chunkflow/flow/normalize_section_contrast.py
-chunkflow/flow/normalize_section_shang.py
 chunkflow/flow/plugin.py
 chunkflow/flow/save_pngs.py
 chunkflow/flow/save_precomputed.py
 chunkflow/flow/setup_env.py
 chunkflow/flow/skeletonize.py
 chunkflow/flow/view.py
 chunkflow/lib/__init__.py
 chunkflow/lib/cartesian_coordinate.py
 chunkflow/lib/flow.py
 chunkflow/lib/region_of_interest.py
 chunkflow/lib/synapses.py
+chunkflow/lib/utils.py
 chunkflow/lib/aws/__init__.py
 chunkflow/lib/aws/cloud_watch.py
 chunkflow/lib/aws/sqs_queue.py
 chunkflow/lib/gala/__init__.py
 chunkflow/lib/gala/evaluate.py
 chunkflow/lib/igneous/__init__.py
 chunkflow/lib/igneous/downsample.py
```

### Comparing `chunkflow-1.1.4/setup.py` & `chunkflow-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/chunk/image/convnet/test_inferencer.py` & `chunkflow-1.1.5/tests/chunk/image/convnet/test_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,17 @@
     # output_patch_crop_margin = (2, 32, 32)
     output_patch_overlap = (2, 32, 32)
     # input_patch_overlap = (6, 96, 96)
     # input_patch_stride = (14, 160, 160)
     input_size = (2*14+6, 2*160+96, 2*160+96)
     num_output_channels = 1
      
+    # numpy randint stop is exclusive
     image = np.random.randint(
-        1, 255,
+        1, 256,
         size=input_size, 
         dtype=np.uint8)
     
     # make sure that it works with arbitrary global offset
     image = Chunk(image, voxel_offset=(123, 345, 567))
    
     with Inferencer(None, None, input_patch_size,
```

### Comparing `chunkflow-1.1.4/tests/chunk/image/convnet/test_patch_mask.py` & `chunkflow-1.1.5/tests/chunk/image/convnet/test_patch_mask.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/chunk/segmentation/test_segmentation.py` & `chunkflow-1.1.5/tests/chunk/segmentation/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/chunk/test_chunk.py` & `chunkflow-1.1.5/tests/chunk/test_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
     #def test_math(self):
     #    self.assertEqual(np.max(self.chunk), np.max(self.chunk.array))
     #    self.assertEqual(np.min(self.chunk), np.min(self.chunk.array))
 
     def test_create_from_bounding_box(self):
         bbox = BoundingBox.from_delta(self.voxel_offset, self.size)
-        bbox = BoundingBox.from_bbox(bbox)
         Chunk.from_bbox( bbox )
 
     def test_computation(self):
         self.chunk /= 127.5
         self.chunk -= 1
 
     def test_bbox(self):
```

### Comparing `chunkflow-1.1.4/tests/chunk/test_validate.py` & `chunkflow-1.1.5/tests/chunk/test_validate.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/flow/test_downsample_upload.py` & `chunkflow-1.1.5/tests/flow/test_downsample_upload.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/flow/test_flow.py` & `chunkflow-1.1.5/tests/flow/test_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     CloudVolume.from_numpy(np.transpose(thumbnail),
                             vol_path=thumbnail_volume_path,
                             voxel_offset=cropping_margin_size[::-1],
                             max_mip=4)
 
     # run pipeline by composing functions
     print('cutout image chunk...')
-    cutout_operator = ReadPrecomputedOperator(
+    cutout_operator = LoadPrecomputedOperator(
         input_volume_path,
         mip=mip,
         expand_margin_size=cropping_margin_size)
     chunk = cutout_operator(output_bbox)
 
     print('mask input...')
     mask_input_operator = MaskOperator(input_mask_volume_path,
@@ -143,15 +143,15 @@
                                     upload_log=True,
                                     create_thumbnail=True)
     save_operator(chunk, log={'timer': {'save': 34}})
     print('after saving: {}'.format(chunk.slices))
 
     # evaluate the output
     print('start evaluation...')
-    out = output_vol[output_bbox.to_slices()[::-1] +
+    out = output_vol[output_bbox.slices[::-1] +
                             (slice(0, 3), )]
     out = np.asarray(out)
     out = out[:, :, :, 0] * 255
     out = out.astype(np.uint8)
     out = np.transpose(out)
 
     # ignore the patch overlap around the border
```

### Comparing `chunkflow-1.1.4/tests/flow/test_load_precomputed.py` & `chunkflow-1.1.5/tests/flow/test_load_precomputed.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from cloudvolume import CloudVolume
 from cloudvolume.lib import generate_random_string
 from cloudfiles import CloudFiles
 
 from chunkflow.lib.cartesian_coordinate import BoundingBox
 
-from chunkflow.flow.load_precomputed import ReadPrecomputedOperator
+from chunkflow.flow.load_precomputed import LoadPrecomputedOperator
 
 
 class TestLoadPrecomputed(unittest.TestCase):
     def setUp(self):
         print('test volume cutout...')
         # compute parameters
         self.mip = 0
@@ -31,29 +31,29 @@
         self.blackout_section_ids = [17, 20]
         ids = {'section_ids': self.blackout_section_ids}
         stor = CloudFiles(self.volume_path)
         stor.put_json('blackout_section_ids.json', ids)
 
     def test_cutout(self):
         print('test volume cutout...')
-        operator = ReadPrecomputedOperator(self.volume_path, mip=self.mip)
+        operator = LoadPrecomputedOperator(self.volume_path, mip=self.mip)
 
         offset = (4, 64, 64)
         shape = (28, 320, 320)
         output_bbox = BoundingBox.from_delta(offset, shape)
         chunk = operator(output_bbox)
 
         self.assertEqual(offset, chunk.voxel_offset)
         np.testing.assert_array_equal(chunk, self.img[4:-4, 64:-64, 64:-64])
 
         shutil.rmtree('/tmp/test')
 
     def test_blackout_sections(self):
         print('test blackout sections...')
-        operator = ReadPrecomputedOperator(self.volume_path,
+        operator = LoadPrecomputedOperator(self.volume_path,
                                   mip=self.mip,
                                   blackout_sections=True)
 
         offset = (4, 64, 64)
         shape = (28, 320, 320)
         output_bbox = BoundingBox.from_delta(offset, shape)
         chunk = operator(output_bbox)
```

### Comparing `chunkflow-1.1.4/tests/flow/test_load_save.py` & `chunkflow-1.1.5/tests/flow/test_load_save.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/flow/test_mesh.py` & `chunkflow-1.1.5/tests/flow/test_mesh.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/flow/test_save_precomputed.py` & `chunkflow-1.1.5/tests/flow/test_save_precomputed.py`

 * *Files identical despite different names*

### Comparing `chunkflow-1.1.4/tests/test_volume.py` & `chunkflow-1.1.5/tests/test_volume.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import shutil
 
 import numpy as np
 
 from cloudvolume.lib import generate_random_string
 from chunkflow.lib.cartesian_coordinate import BoundingBox, Cartesian
-from chunkflow.volume import Volume
+from chunkflow.volume import PrecomputedVolume
 
 
 def test_volume():
     print('test volume cutout...')
     # compute parameters
     size = (36, 448, 448)
 
     # create image dataset using cloud-volume
     img = np.random.randint(0, 256, size=size)
     img = img.astype(np.uint8)
     # save the input to disk
     volume_path = 'file:///tmp/test/volume/' + \
         generate_random_string()
     
-    vol = Volume.from_numpy(
+    vol = PrecomputedVolume.from_numpy(
         img,
         volume_path
     )
 
     offset = Cartesian(4, 64, 64)
     shape = (28, 320, 320)
     bbox = BoundingBox.from_delta(offset, shape)
```

