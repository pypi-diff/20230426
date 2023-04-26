# Comparing `tmp/lifeblood-0.1.6.tar.gz` & `tmp/lifeblood-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeblood-0.1.6.tar", last modified: Thu Jan 19 10:36:51 2023, max compression
+gzip compressed data, was "lifeblood-0.2.1.tar", last modified: Wed Apr 26 08:48:01 2023, max compression
```

## Comparing `lifeblood-0.1.6.tar` & `lifeblood-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,171 @@
-drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-01-19 10:36:51.034787 lifeblood-0.1.6/
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2765 2023-01-19 10:36:51.034787 lifeblood-0.1.6/PKG-INFO
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2298 2023-01-01 15:25:16.000000 lifeblood-0.1.6/README.md
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      103 2021-12-18 19:33:37.000000 lifeblood-0.1.6/pyproject.toml
--rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1180 2023-01-19 10:36:51.034787 lifeblood-0.1.6/setup.cfg
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.483547 lifeblood-0.2.1/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)       74 2023-04-26 00:00:40.000000 lifeblood-0.2.1/MANIFEST.in
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2765 2023-04-26 08:48:01.483547 lifeblood-0.2.1/PKG-INFO
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2298 2023-01-01 15:25:16.000000 lifeblood-0.2.1/README.md
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      103 2021-12-18 19:33:37.000000 lifeblood-0.2.1/pyproject.toml
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1224 2023-04-26 08:48:01.483547 lifeblood-0.2.1/setup.cfg
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.475547 lifeblood-0.2.1/src/lifeblood/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2022-11-13 17:07:09.000000 lifeblood-0.2.1/src/lifeblood/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2346 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/aiosqlite_overlay.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      224 2023-04-22 10:40:02.000000 lifeblood-0.2.1/src/lifeblood/base.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    19920 2023-04-23 22:47:13.000000 lifeblood-0.2.1/src/lifeblood/basenode.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     7194 2022-06-27 22:35:34.000000 lifeblood-0.2.1/src/lifeblood/broadcasting.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      474 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/buffer_serializable.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3385 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/buffered_connection.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     9537 2023-01-10 00:26:24.000000 lifeblood-0.2.1/src/lifeblood/config.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.475547 lifeblood-0.2.1/src/lifeblood/core_nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     9818 2022-08-22 22:25:54.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/attribute_splitter.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1303 2022-08-22 00:53:33.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/del_attrib.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5658 2022-08-26 00:08:03.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/environment_resolver_setter.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      768 2022-02-13 15:47:48.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/kill.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     8169 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/mod_attrib.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      829 2022-06-27 20:43:41.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/null.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    10503 2022-02-06 22:34:31.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/parent_children_waiter.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4822 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/python.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1873 2022-08-22 00:53:41.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/rename_attrib.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6182 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/set_attrib.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2052 2022-02-13 20:58:19.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/spawn_children.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     9893 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/split_waiter.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1395 2022-02-19 19:10:54.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/switch.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3454 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/test.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4526 2022-12-18 01:06:01.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/wait_for_task.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4000 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/core_nodes/wedge.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     7946 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/db_misc.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      233 2022-06-27 22:58:45.000000 lifeblood-0.2.1/src/lifeblood/defaults.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1856 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/enums.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    17465 2023-01-21 14:20:23.000000 lifeblood-0.2.1/src/lifeblood/environment_resolver.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      555 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/exceptions.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4918 2022-04-10 20:28:51.000000 lifeblood-0.2.1/src/lifeblood/filelock.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    14880 2022-08-21 12:48:46.000000 lifeblood-0.2.1/src/lifeblood/invocationjob.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2368 2023-03-03 02:44:33.000000 lifeblood-0.2.1/src/lifeblood/launch.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4857 2023-02-04 00:26:31.000000 lifeblood-0.2.1/src/lifeblood/local_notifier.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2084 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/logging.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3987 2022-01-13 16:08:02.000000 lifeblood-0.2.1/src/lifeblood/maintenance.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      302 2022-07-26 21:30:26.000000 lifeblood-0.2.1/src/lifeblood/matrix_helper.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5463 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/misc.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1749 2022-02-13 19:50:57.000000 lifeblood-0.2.1/src/lifeblood/names.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6502 2023-04-22 10:44:43.000000 lifeblood-0.2.1/src/lifeblood/net_classes.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4947 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/nethelpers.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      488 2023-04-23 22:42:07.000000 lifeblood-0.2.1/src/lifeblood/node_visualization_classes.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2698 2022-12-17 19:57:31.000000 lifeblood-0.2.1/src/lifeblood/nodethings.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      290 2022-06-15 08:48:14.000000 lifeblood-0.2.1/src/lifeblood/os_based_cheats.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2554 2022-03-25 01:03:28.000000 lifeblood-0.2.1/src/lifeblood/paths.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1258 2022-03-22 10:41:39.000000 lifeblood-0.2.1/src/lifeblood/plugin_info.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    12085 2023-01-08 15:47:23.000000 lifeblood-0.2.1/src/lifeblood/pluginloader.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     8190 2022-08-21 12:07:03.000000 lifeblood-0.2.1/src/lifeblood/process_utils.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4609 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/processingcontext.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2408 2022-07-14 21:06:00.000000 lifeblood-0.2.1/src/lifeblood/pulse_checker.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1012 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/rwlock.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.475547 lifeblood-0.2.1/src/lifeblood/scheduler/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5661 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/scheduler/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3071 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/scheduler/data_access.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    14541 2023-04-12 10:34:52.000000 lifeblood-0.2.1/src/lifeblood/scheduler/pinger.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    82761 2023-03-26 00:04:48.000000 lifeblood-0.2.1/src/lifeblood/scheduler/scheduler.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2210 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/scheduler/scheduler_component_base.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/scheduler/state_object.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    53462 2023-04-17 00:35:05.000000 lifeblood-0.2.1/src/lifeblood/scheduler/task_processor.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    40046 2023-04-14 22:40:36.000000 lifeblood-0.2.1/src/lifeblood/scheduler/ui_state_accessor.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     7001 2023-04-14 12:26:16.000000 lifeblood-0.2.1/src/lifeblood/scheduler_event_log.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    13891 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/scheduler_task_protocol.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    61155 2023-03-26 00:06:07.000000 lifeblood-0.2.1/src/lifeblood/scheduler_ui_protocol.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     8637 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/shared_lazy_sqlite_connection.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    19538 2023-01-18 00:19:44.000000 lifeblood-0.2.1/src/lifeblood/simple_worker_pool.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6582 2023-04-23 12:47:53.000000 lifeblood-0.2.1/src/lifeblood/snippets.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.467547 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2841 2022-08-21 12:24:29.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/camera_init.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3021 2022-08-20 22:33:12.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/depth_map.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3046 2022-08-20 20:59:08.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/depth_map_filter.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3628 2022-08-19 23:41:43.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/feature_extraction.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3536 2022-08-19 23:45:10.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/feature_matching.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3658 2022-08-21 12:24:03.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/image_matching.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2486 2022-08-21 00:32:57.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/mesh_filtering.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3548 2022-08-20 21:27:47.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/meshing.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2544 2022-08-20 20:58:49.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/prepare_dense_scene.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3873 2022-08-22 23:29:32.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/sfmtransform.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5118 2022-08-22 22:43:07.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/structure_from_motion.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3581 2022-08-20 22:16:29.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/nodes/texturing.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/python/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/python/3/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2022-08-16 22:19:38.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      380 2022-08-21 11:39:25.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/base_node.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    10732 2023-04-23 22:56:33.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/nodes/blender_batch_render.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2860 2023-04-23 22:27:32.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/nodes/blender_script.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/presets/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    13410 2023-01-11 00:20:00.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/blender/presets/blender_render.lbp
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6126 2022-07-13 00:33:15.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/ffmpeg.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    12859 2023-02-04 00:28:10.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/file_watcher.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     7716 2022-08-21 12:56:01.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/fileop.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3951 2022-12-18 01:11:12.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/filepattern.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1741 2022-02-19 01:34:06.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/framerange_splitter.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4004 2022-08-06 12:35:53.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/copy_temp_hip.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    12522 2022-12-08 02:10:30.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/hip_driver_renderer.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6807 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/hip_ifd_generator.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     3716 2022-03-13 23:39:07.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/hip_script.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4653 2022-10-07 00:15:18.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/hip_usd_generator.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2917 2022-12-21 01:39:08.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/karma.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2699 2022-07-17 22:49:20.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/nodes/mantra.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/presets/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    25180 2022-10-08 12:31:51.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/presets/karma.lbp
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    25557 2022-10-08 12:32:35.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/presets/mantra.lbp
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/python/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/python/3/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2022-10-01 22:34:31.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    10256 2022-10-02 18:09:46.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/rop_base_node.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5156 2022-08-06 23:08:06.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_runner.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1652 2022-02-13 16:03:46.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_stopper.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    18813 2022-06-27 21:55:59.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/distributed_slices.lbp
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2868 2022-10-09 17:55:03.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/nodes/arnold.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6572 2022-09-30 22:41:54.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/nodes/hip_ass_generator.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/presets/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    25196 2022-09-30 23:09:45.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/htoa/presets/htoa.lbp
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    13115 2022-04-23 23:10:42.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/imagemagik.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/data/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1110 2023-03-19 01:12:49.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/data/install_matrix_commander.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)   464243 2023-03-19 01:12:49.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/data/matrixclient.pyz
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/nodes/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     9918 2023-03-19 01:16:39.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/matrixclient/nodes/matrixnotifier.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.471547 lifeblood-0.2.1/src/lifeblood/stock_nodes/stock_presets/
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/stock_nodes/stock_presets/presets/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    12254 2022-07-09 21:09:43.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/stock_presets/presets/cache.lbp
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    16849 2022-07-09 21:14:35.000000 lifeblood-0.2.1/src/lifeblood/stock_nodes/stock_presets/presets/wedge.lbp
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5417 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/taskspawn.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2461 2022-07-06 08:51:26.000000 lifeblood-0.2.1/src/lifeblood/text.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5773 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/toml_coders.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     6426 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/ui_events.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    28259 2023-03-20 22:24:54.000000 lifeblood-0.2.1/src/lifeblood/ui_protocol_data.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    55356 2023-04-23 22:12:25.000000 lifeblood-0.2.1/src/lifeblood/uidata.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    51641 2023-04-24 09:58:33.000000 lifeblood-0.2.1/src/lifeblood/worker.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1057 2022-05-17 23:44:18.000000 lifeblood-0.2.1/src/lifeblood/worker_pool.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     4295 2022-09-07 09:24:22.000000 lifeblood-0.2.1/src/lifeblood/worker_pool_protocol.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.479547 lifeblood-0.2.1/src/lifeblood/worker_runtime_pythonpath/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        0 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood/worker_runtime_pythonpath/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     8071 2022-12-29 16:43:31.000000 lifeblood-0.2.1/src/lifeblood/worker_runtime_pythonpath/lifeblood_connection.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)    12270 2023-03-15 23:27:40.000000 lifeblood-0.2.1/src/lifeblood/worker_task_protocol.py
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.475547 lifeblood-0.2.1/src/lifeblood.egg-info/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     2765 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/PKG-INFO
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5796 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/SOURCES.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)        1 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/dependency_links.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      122 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/entry_points.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      160 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/requires.txt
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)       27 2023-04-26 08:48:01.000000 lifeblood-0.2.1/src/lifeblood.egg-info/top_level.txt
+drwxrwxr-x   0 xapkohheh  (1000) xapkohheh  (1000)        0 2023-04-26 08:48:01.483547 lifeblood-0.2.1/src/lifeblood_client/
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      414 2022-11-13 17:30:38.000000 lifeblood-0.2.1/src/lifeblood_client/__init__.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     1272 2022-11-13 19:58:15.000000 lifeblood-0.2.1/src/lifeblood_client/environment_resolver.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)      805 2021-12-18 19:33:37.000000 lifeblood-0.2.1/src/lifeblood_client/nethelpers.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     7374 2022-11-18 00:00:07.000000 lifeblood-0.2.1/src/lifeblood_client/query.py
+-rw-rw-r--   0 xapkohheh  (1000) xapkohheh  (1000)     5710 2023-01-05 01:32:38.000000 lifeblood-0.2.1/src/lifeblood_client/submitting.py
```

### Comparing `lifeblood-0.1.6/PKG-INFO` & `lifeblood-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeblood
-Version: 0.1.6
+Version: 0.2.1
 Summary: LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `lifeblood-0.1.6/README.md` & `lifeblood-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lifeblood-0.1.6/setup.cfg` & `lifeblood-0.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [metadata]
 name = lifeblood
-version = 0.1.6
+version = 0.2.1
 author = XAPKOHHEH
 description = LIFEBLOOD !!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pedohorse/lifeblood
 project_urls = 
 	Bug Tracker = https://github.com/pedohorse/lifeblood/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
-	= ../src
+	= src
 packages = find:
 python_requires = >=3.8, <3.11
 install_requires = 
 	aiofiles~=0.8
 	aiosqlite~=0.17
 	aiorwlock~=1.3
 	lz4~=4.0
 	psutil~=5.8
 	pywin32==304; platform_system=="Windows"
 	semantic-version~=2.10
 	toml~=0.10
 	watchdog~=2.1
 
 [options.packages.find]
-where = ../src
+where = src
 include = lifeblood*
 exclude = lifeblood_viewer*
 
 [options.package_data]
 lifeblood = core_nodes/**, stock_nodes/**
 
 [options.exclude_package_data]
-lifeblood = core_nodes/**/__pycache__/*, stock_nodes/**/__pycache__/*, **/*.pyc
+lifeblood = core_nodes/**/__pycache__/*, stock_nodes/**/__pycache__/*, **/*.pyc, stock_nodes/matrixclient/data/matrixcommander/**
 
 [options.entry_points]
 console_scripts = 
 	lifeblood = lifeblood.launch:console_entry_point
 	lifeblood_matrix_helper = lifeblood.matrix_helper:main
 
 [egg_info]
```

