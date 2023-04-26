# Comparing `tmp/netin-1.0.5.8.8.tar.gz` & `tmp/netin-1.0.5.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.8.8.tar", last modified: Wed Apr 26 01:48:35 2023, max compression
+gzip compressed data, was "netin-1.0.5.8.9.tar", last modified: Wed Apr 26 20:11:02 2023, max compression
```

## Comparing `netin-1.0.5.8.8.tar` & `netin-1.0.5.8.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8.8/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8.8/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.8.8/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8.8/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8.8/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8.8/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8.8/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8.8/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8.8/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8.8/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8.8/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      423 2023-04-26 01:47:14.000000 netin-1.0.5.8.8/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.8.8/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.8.8/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8.8/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8.8/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8.8/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8.8/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6159 2023-04-25 17:16:17.000000 netin-1.0.5.8.8/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      296 2023-04-24 23:15:30.000000 netin-1.0.5.8.8/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8.8/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14008 2023-04-26 01:27:29.000000 netin-1.0.5.8.8/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-24 18:05:02.000000 netin-1.0.5.8.8/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5395 2023-04-26 00:57:56.000000 netin-1.0.5.8.8/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    23204 2023-04-26 00:15:00.000000 netin-1.0.5.8.8/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8.8/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2747 2023-04-24 18:05:16.000000 netin-1.0.5.8.8/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-24 18:05:38.000000 netin-1.0.5.8.8/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-25 11:41:22.000000 netin-1.0.5.8.8/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-24 18:05:57.000000 netin-1.0.5.8.8/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8.8/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8.8/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8.8/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8.8/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8.8/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8.8/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9295 2023-04-26 01:26:41.000000 netin-1.0.5.8.8/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      495 2023-04-24 13:42:57.000000 netin-1.0.5.8.8/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.8.8/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3615 2023-04-26 01:44:17.000000 netin-1.0.5.8.8/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8.8/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8.8/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1265 2023-04-26 01:25:38.000000 netin-1.0.5.8.8/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.8.8/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.8.8/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.8.8/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.8.8/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.8.8/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8.8/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8.8/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8.8/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8.8/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4256 2023-04-25 10:29:59.000000 netin-1.0.5.8.8/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8.9/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8.9/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.8.9/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.911203 netin-1.0.5.8.9/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8.9/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8.9/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8.9/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8.9/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8.9/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8.9/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8.9/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8.9/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      479 2023-04-26 20:02:17.000000 netin-1.0.5.8.9/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.8.9/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.8.9/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8.9/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8.9/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8.9/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8.9/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6159 2023-04-25 17:16:17.000000 netin-1.0.5.8.9/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      523 2023-04-26 19:54:04.000000 netin-1.0.5.8.9/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8.9/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27992 2023-04-26 19:54:50.000000 netin-1.0.5.8.9/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8.9/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2748 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8.9/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8.9/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8.9/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8.9/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8.9/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8.9/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9951 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.8.9/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.8.9/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5753 2023-04-26 19:48:11.000000 netin-1.0.5.8.9/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8.9/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8.9/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.8.9/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.8.9/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.8.9/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.8.9/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.8.9/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.8.9/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8.9/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8.9/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8.9/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8.9/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.8.9/setup.py
```

### Comparing `netin-1.0.5.8.8/LICENSE` & `netin-1.0.5.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/PKG-INFO` & `netin-1.0.5.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.8
+Version: 1.0.5.8.9
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.8/README.rst` & `netin-1.0.5.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/examples/notebooks/deleteme.py` & `netin-1.0.5.8.9/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/random_edges.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/algorithms/sampling/sampling.py` & `netin-1.0.5.8.9/netin/algorithms/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/dh.py` & `netin-1.0.5.8.9/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/directed.py` & `netin-1.0.5.8.9/netin/generators/directed.py`

 * *Files 5% similar despite different names*

```diff
@@ -251,67 +251,46 @@
             fit_M, fit_m = self.fit_powerlaw(metric)
             print(f"- Powerlaw fit ({metric}):")
             print(f"- {self.get_majority_label()}: alpha={fit_M.power_law.alpha}, sigma={fit_M.power_law.sigma}, "
                   f"min={fit_M.power_law.xmin}, max={fit_M.power_law.xmax}")
             print(f"- {self.get_minority_label()}: alpha={fit_m.power_law.alpha}, sigma={fit_m.power_law.sigma}, "
                   f"min={fit_m.power_law.xmin}, max={fit_m.power_law.xmax}")
 
-    def fit_powerlaw(self, metric: str) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
-        """
-        Fits a power law to the distribution given by 'metric' (the in- or out-degree of nodes in the graph).
-
-        Parameters
-        ----------
-        metric: str
-            metric to fit power law to
-
-        Returns
-        -------
-        powerlaw.Fit
-            power law fit of the majority class
-
-        powerlaw.Fit
-            power law fit of the minority class
-        """
-        # @TODO: validate if metric is not in_degree or out_degree
-        vM = self.get_majority_value()
-        dist_fnc = self.in_degree if metric == 'in_degree' else self.out_degree
-        dM = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] == vM]
-        dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
-
-        fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
-        fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
-        return fit_M, fit_m
-
     def calculate_in_degree_powerlaw_exponents(self) -> Tuple[float, float]:
         """
         Returns the power law exponents for the in-degree distribution of the majority and minority class.
 
         Returns
         -------
         Tuple[float, float]
             power law exponents for the in-degree distribution of the majority and minority class
         """
-        fit_M, fit_m = self.fit_powerlaw(metric='in_degree')
-        pl_M = fit_M.power_law.alpha
-        pl_m = fit_m.power_law.alpha
+        pl_M, pl_m = calculate_in_degree_powerlaw_exponents(self)
+
+        # fit_M, fit_m = self.fit_powerlaw(metric='in_degree')
+        # pl_M = fit_M.power_law.alpha
+        # pl_m = fit_m.power_law.alpha
+
         return pl_M, pl_m
 
     def calculate_out_degree_powerlaw_exponents(self) -> Tuple[float, float]:
         """
         Returns the power law exponents for the out-degree distribution of the majority and minority class.
 
         Returns
         -------
         Tuple[float, float]
             power law exponents for the out-degree distribution of the majority and minority class
         """
-        fit_M, fit_m = self.fit_powerlaw(metric='out_degree')
-        pl_M = fit_M.power_law.alpha
-        pl_m = fit_m.power_law.alpha
+        pl_M, pl_m = calculate_out_degree_powerlaw_exponents(self)
+
+        # fit_M, fit_m = self.fit_powerlaw(metric='out_degree')
+        # pl_M = fit_M.power_law.alpha
+        # pl_m = fit_m.power_law.alpha
+
         return pl_M, pl_m
 
     ############################################################
     # Getters and setters
     ############################################################
 
     def get_expected_number_of_edges(self) -> int:
@@ -372,13 +351,53 @@
         return self.activity
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         obj = self.__class__(n=self.n,
-                              d=self.d,
-                              f_m=self.f_m,
-                              plo_M=self.plo_M,
-                              plo_m=self.plo_m,
-                              seed=self.seed)
+                             d=self.d,
+                             f_m=self.f_m,
+                             plo_M=self.plo_M,
+                             plo_m=self.plo_m,
+                             seed=self.seed)
         return obj
+
+
+def calculate_in_degree_powerlaw_exponents(g: DiGraph) -> Tuple[float, float]:
+    """
+    Returns the power law exponents for the in-degree distribution of the majority and minority class.
+
+    Parameters
+    ----------
+    g: DiGraph
+        Graph to calculate the power law exponents for
+
+    Returns
+    -------
+    Tuple[float, float]
+        power law exponents for the in-degree distribution of the majority and minority class
+    """
+    fit_M, fit_m = g.fit_powerlaw(metric='in_degree')
+    pl_M = fit_M.power_law.alpha
+    pl_m = fit_m.power_law.alpha
+    return pl_M, pl_m
+
+
+def calculate_out_degree_powerlaw_exponents(g: DiGraph) -> Tuple[float, float]:
+    """
+    Returns the power law exponents for the out-degree distribution of the majority and minority class.
+
+    Parameters
+    ----------
+    g: DiGraph
+        Graph to calculate the power law exponents for
+
+    Returns
+    -------
+    Tuple[float, float]
+        power law exponents for the out-degree distribution of the majority and minority class
+    """
+    fit_M, fit_m = g.fit_powerlaw(metric='out_degree')
+    pl_M = fit_M.power_law.alpha
+    pl_m = fit_m.power_law.alpha
+    return pl_M, pl_m
```

### Comparing `netin-1.0.5.8.8/netin/generators/dpa.py` & `netin-1.0.5.8.9/netin/generators/dpa.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union, Set
 
 import numpy as np
 
-from netin.utils import constants as const
 from netin.generators.directed import DiGraph
+from netin.utils import constants as const
 
 
 class DPA(DiGraph):
     """Creates a new DPA instance. A directed graph with preferential attachment.
 
     Parameters
     ----------
```

### Comparing `netin-1.0.5.8.8/netin/generators/dpah.py` & `netin-1.0.5.8.9/netin/generators/dpah.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,20 +143,20 @@
         return h_MM, h_mm
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         obj = self.__class__(n=self.n,
-                              d=self.d,
-                              f_m=self.f_m,
-                              plo_M=self.plo_M,
-                              plo_m=self.plo_m,
-                              h_MM=self.h_MM,
-                              h_mm=self.h_mm,
-                              seed=self.seed)
+                             d=self.d,
+                             f_m=self.f_m,
+                             plo_M=self.plo_M,
+                             plo_m=self.plo_m,
+                             h_MM=self.h_MM,
+                             h_mm=self.h_mm,
+                             seed=self.seed)
 
         # @TODO: check if this is necessary
         # obj._initialize(class_attribute=self.class_attribute,
         #                 class_values=self.class_values,
         #                 class_labels=self.class_labels)
         return obj
```

### Comparing `netin-1.0.5.8.8/netin/generators/graph.py` & `netin-1.0.5.8.9/netin/generators/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import time
+import warnings
 from collections import Counter
-from typing import Union, Set, List
+from typing import Union, Set, List, Tuple, Iterable
 
 import networkx as nx
 import numpy as np
 import pandas as pd
+import powerlaw
 from pqdm.threads import pqdm
-import warnings
 
 import netin
+from netin.stats import networks as net
 from netin.utils import constants as const
 from netin.utils import validator as val
-from netin.stats import networks as net
 
 
 class Graph(nx.Graph):
     """Bi-populated network (base graph model)
 
     Parameters
     ----------
@@ -328,72 +329,98 @@
         -------
         str
             class label
         """
         idx = self.class_values.index(self.nodes[node][self.class_attribute])
         return self.class_labels[idx]
 
-    def get_majority_value(self) -> int:
+    def get_majority_value(self) -> object:
         """
         Returns the value for the majority class.
 
         Returns
         -------
         int
             value for the majority class
+
+        Notes
+        -----
+        Position 0 of the ``class_values`` is the majority value.
+        Position 1 of the ``class_values`` is the minority value.
         """
-        return const.MAJORITY_VALUE
+        # return const.MAJORITY_VALUE
+        return self.class_values[const.MAJORITY_VALUE]
 
-    def get_minority_value(self) -> int:
+    def get_minority_value(self) -> object:
         """
         Returns the value for the minority class
 
         Returns
         -------
         int
             value for the minority class
+
+        Notes
+        -----
+        Position 0 of the ``class_values`` is the majority value.
+        Position 1 of the ``class_values`` is the minority value.
         """
-        return const.MINORITY_VALUE
+        # return const.MINORITY_VALUE
+        return self.class_values[const.MINORITY_VALUE]
 
     def get_majority_label(self) -> str:
         """
         Returns the label for the majority class.
 
         Returns
         -------
         str
             label for the majority class
+
+        Notes
+        -----
+        Position 0 of the ``class_labels`` is the majority label.
+        Position 1 of the ``class_labels`` is the minority label.
         """
-        return const.MAJORITY_LABEL
+        # return const.MAJORITY_LABEL
+        return self.class_labels[const.MAJORITY_VALUE]
 
     def get_minority_label(self) -> str:
         """
         Returns the labels for the minority class.
 
         Returns
         -------
         str
             label for the minority class
+
+        Notes
+        -----
+        Position 0 of the ``class_labels`` is the majority label.
+        Position 1 of the ``class_labels`` is the minority label.
         """
-        return const.MINORITY_LABEL
+        # return const.MINORITY_LABEL
+        return self.class_labels[const.MINORITY_VALUE]
 
     ############################################################
     # Generation
     ############################################################
 
-    def _initialize(self, class_attribute: str = const.CLASS_ATTRIBUTE, class_values: list = None, class_labels: list = None):
+    def _initialize(self, class_attribute: str = const.CLASS_ATTRIBUTE, class_values: list = None,
+                    class_labels: list = None):
         """
         Initializes the random seed, the graph metadata, and node class information.
         """
         np.random.seed(self.seed)
         self._validate_parameters()
         self._init_graph(class_attribute, class_values, class_labels)
         self._init_nodes()
 
-    def _init_graph(self, class_attribute: str = const.CLASS_ATTRIBUTE, class_values: list = None, class_labels: list = None):
+    def _init_graph(self, class_attribute: str = const.CLASS_ATTRIBUTE, class_values: list = None,
+                    class_labels: list = None):
         """
         Initializes the graph.
         Sets the name of the model, class information, and the graph metadata.
 
         Parameters
         ----------
         class_attribute: str
@@ -588,14 +615,44 @@
         Returns
         -------
         Counter
             counter of edges types
         """
         return net.get_edge_type_counts(self)
 
+    def fit_powerlaw(self, metric: str) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
+        """
+        Fits a power law to the distribution given by 'metric' (the in- or out-degree of nodes in the graph).
+
+        Parameters
+        ----------
+        metric: str
+            metric to fit power law to
+
+        Returns
+        -------
+        powerlaw.Fit
+            power law fit of the majority class
+
+        powerlaw.Fit
+            power law fit of the minority class
+        """
+
+        fit_M, fit_m = fit_powerlaw_groups(self, metric)
+
+        # vM = self.get_majority_value()
+        # dist_fnc = self.in_degree if metric == 'in_degree' else self.out_degree
+        # dM = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] == vM]
+        # dm = [d for n, d in dist_fnc if self.nodes[n][self.class_attribute] != vM]
+        #
+        # fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
+        # fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
+
+        return fit_M, fit_m
+
     ############################################################
     # Metadata
     ############################################################
 
     def compute_node_stats(self, metric: str, **kwargs) -> List[Union[int, float]]:
         """
         Returns the property of each node in the graph based on the metric.
@@ -727,7 +784,92 @@
             for v, datadict in nbrs.items()
         )
         g.node_list = self.node_list.copy()
         g.node_labels = self.node_labels.copy()
         g.n_m = self.n_m
         g.n_M = self.n_M
         return g
+
+
+def fit_powerlaw_groups(g: Graph, metric: str) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
+    """
+    Fits a power law to the distribution given by 'metric' (the in- or out-degree of nodes in the graph).
+
+    Parameters
+    ----------
+    g: Graph
+        Graph to fit power law to
+
+    metric: str
+        metric to fit power law to
+
+    Returns
+    -------
+    powerlaw.Fit
+        power law fit of the majority class
+
+    powerlaw.Fit
+        power law fit of the minority class
+    """
+
+    def _get_value_fnc(g: Graph, metric: str) -> Iterable:
+        if metric not in ['in_degree', 'out_degree', 'degree']:
+            raise ValueError(f"`metric` must be either 'in_degree', 'out_degree' or 'degree', not {metric}")
+        return g.in_degree if metric == 'in_degree' else g.out_degree if metric == 'out_degree' else g.degree
+
+    vM = g.get_majority_value()
+    fnc = _get_value_fnc(g, metric)
+    dM = [d for n, d in fnc if g.nodes[n][g.class_attribute] == vM]
+    dm = [d for n, d in fnc if g.nodes[n][g.class_attribute] != vM]
+
+    fit_M = powerlaw.Fit(data=dM, discrete=True, xmin=min(dM), xmax=max(dM), verbose=False)
+    fit_m = powerlaw.Fit(data=dm, discrete=True, xmin=min(dm), xmax=max(dm), verbose=False)
+    return fit_M, fit_m
+
+
+def convert_networkx_to_netin(g: Union[nx.Graph, nx.DiGraph], name: str, class_attribute: str) -> Graph:
+    """
+    Given a networkx graph, it creates a netin graph with the same structure and attributes.
+
+    Parameters
+    ----------
+    g:  networkx
+        Graph to convert
+
+    name:  str
+        name of the dataset
+
+    class_attribute:  str
+        name of the attribute that contains the class label
+
+    Returns
+    -------
+    netin.Graph
+        netin graph with the same structure and attributes
+    """
+    n = g.number_of_nodes()
+    f_m = net.get_minority_fraction(g, class_attribute)
+    seed = None
+
+    if g.is_directed():
+        d = nx.density(g)
+        plo_M, plo_m = netin.calculate_out_degree_powerlaw_exponents(g)
+        gn = netin.DiGraph(n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
+    else:
+        k = net.get_min_degree(g)
+        gn = netin.UnDiGraph(n=n, k=k, f_m=f_m, seed=seed)
+
+    gn.set_model_name(name)
+    gn.add_edges_from(g.edges(data=True))
+    gn.add_nodes_from(g.nodes(data=True))
+
+    counter = Counter([obj[class_attribute] for n, obj in g.nodes(data=True)])
+    class_values, class_counts = zip(*counter.most_common())  # from M to m
+    class_labels = ['female' if c == 1 else 'male' if c == 0 else 'unknown' for c in class_values]
+    gn._initialize(class_attribute=class_attribute, class_values=class_values, class_labels=class_labels)
+
+    obj = {'model': gn.get_model_name(),
+           'e': g.number_of_edges()}
+
+    gn.graph.update(obj)
+
+    return gn
```

### Comparing `netin-1.0.5.8.8/netin/generators/h.py` & `netin-1.0.5.8.9/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/pa.py` & `netin-1.0.5.8.9/netin/generators/pa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Set
 from typing import Union
 
 import numpy as np
 
-from netin.utils import constants as const
 from netin.generators.undirected import UnDiGraph
+from netin.utils import constants as const
 
 
 class PA(UnDiGraph):
     """Creates a new PA instance. An undirected graph with preferential attachment.
 
     Parameters
     ----------
@@ -26,14 +26,15 @@
 
     Notes
     -----
     The initialization is an undirected graph with n nodes and no edges.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
     Target nodes are selected via preferential attachment (in-degree), see [BarabasiAlbert1999]_.
     """
+
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, seed: object = None):
         super().__init__(n, k, f_m, seed)
```

### Comparing `netin-1.0.5.8.8/netin/generators/pah.py` & `netin-1.0.5.8.9/netin/generators/pah.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
-from sympy import symbols
 from sympy import Eq
 from sympy import solve
+from sympy import symbols
 
-from netin.utils import constants as const
 from netin.generators.h import Homophily
+from netin.utils import constants as const
 from .pa import PA
 
 
 class PAH(PA, Homophily):
     """Creates a new PAH instance. An undirected graph with preferential attachment and homophily.
 
     Parameters
```

### Comparing `netin-1.0.5.8.8/netin/generators/patc.py` & `netin-1.0.5.8.9/netin/generators/patc.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union, Set, Tuple
 
-import numpy as np
 import networkx as nx
+import numpy as np
 
-from netin.utils import constants as const
 from netin.generators.tc import TriadicClosure
+from netin.utils import constants as const
 from .pa import PA
 
 
 class PATC(PA, TriadicClosure):
     """Creates a new PATC instance. An undirected graph with preferential attachment and triadic closure.
 
     Parameters
```

### Comparing `netin-1.0.5.8.8/netin/generators/patch.py` & `netin-1.0.5.8.9/netin/generators/patch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
 
-from netin.utils import constants as const
 from netin.generators.tc import TriadicClosure
+from netin.utils import constants as const
 from .pah import PAH
 
 
 class PATCH(PAH, TriadicClosure):
     """Creates a new PATCH instance. An undirected graph with preferential attachment, homophily, and triadic closure.
 
     Parameters
```

### Comparing `netin-1.0.5.8.8/netin/generators/tc.py` & `netin-1.0.5.8.9/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/tests/test_directed.py` & `netin-1.0.5.8.9/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/tests/test_dpah.py` & `netin-1.0.5.8.9/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/tests/test_patch.py` & `netin-1.0.5.8.9/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/tests/test_undirected.py` & `netin-1.0.5.8.9/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/generators/undirected.py` & `netin-1.0.5.8.9/netin/generators/undirected.py`

 * *Files 7% similar despite different names*

```diff
@@ -229,20 +229,43 @@
         -------
         pl_M : float
             Powerlaw exponent for the majority class
 
         pl_m: float
             Powerlaw exponent for the minority class
         """
-        fit_M, fit_m = self.fit_degree_powerlaw()
-        pl_M = fit_M.power_law.alpha
-        pl_m = fit_m.power_law.alpha
+        pl_M, pl_m = calculate_degree_powerlaw_exponents(self)
+
+        # fit_M, fit_m = self.fit_degree_powerlaw()
+        # pl_M = fit_M.power_law.alpha
+        # pl_m = fit_m.power_law.alpha
+
         return pl_M, pl_m
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         return self.__class__(n=self.n,
                               k=self.k,
                               f_m=self.f_m,
                               seed=self.seed)
+
+
+def calculate_degree_powerlaw_exponents(g: UnDiGraph) -> Tuple[float, float]:
+    """
+    Returns the power law exponents for the in-degree distribution of the majority and minority class.
+
+    Parameters
+    ----------
+    g: DiGraph
+        Graph to calculate the power law exponents for
+
+    Returns
+    -------
+    Tuple[float, float]
+        power law exponents for the in-degree distribution of the majority and minority class
+    """
+    fit_M, fit_m = g.fit_powerlaw(metric='in_degree')
+    pl_M = fit_M.power_law.alpha
+    pl_m = fit_m.power_law.alpha
+    return pl_M, pl_m
```

### Comparing `netin-1.0.5.8.8/netin/stats/distributions.py` & `netin-1.0.5.8.9/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/stats/ranking.py` & `netin-1.0.5.8.9/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/utils/io.py` & `netin-1.0.5.8.9/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/utils/validator.py` & `netin-1.0.5.8.9/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin/viz/handlers.py` & `netin-1.0.5.8.9/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/netin.egg-info/PKG-INFO` & `netin-1.0.5.8.9/netin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.8
+Version: 1.0.5.8.9
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.8/netin.egg-info/SOURCES.txt` & `netin-1.0.5.8.9/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.8/setup.py` & `netin-1.0.5.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,33 +56,37 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 packages = [
     "netin",
-    "netin.algorithms.sampling",
     "netin.generators",
     "netin.utils",
     "netin.stats",
     "netin.viz",
+    "netin.algorithms.sampling",
     "netin.generators.tests",
 ]
 
 docdirbase = "share/doc/netin-%s" % version
+
 # add basic documentation
 data = [(docdirbase, glob("*.txt"))]
+
 # add examples
 for d in [
     ".",
+    "directed",
+    "undirected",
+    "notebooks",
     "advanced",
     "algorithms",
     "basic",
     "drawing",
-    "undirected",
     "subclass",
 ]:
     dd = os.path.join(docdirbase, "examples", d)
     pp = os.path.join("examples", d)
     data.append((dd, glob(os.path.join(pp, "*.txt"))))
     data.append((dd, glob(os.path.join(pp, "*.py"))))
     data.append((dd, glob(os.path.join(pp, "*.bz2"))))
```

