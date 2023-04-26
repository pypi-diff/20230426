# Comparing `tmp/netin-1.0.5.8.7.tar.gz` & `tmp/netin-1.0.5.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.8.7.tar", last modified: Wed Apr 26 00:46:58 2023, max compression
+gzip compressed data, was "netin-1.0.5.8.8.tar", last modified: Wed Apr 26 01:48:35 2023, max compression
```

## Comparing `netin-1.0.5.8.7.tar` & `netin-1.0.5.8.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8.7/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8.7/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.8.7/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.861470 netin-1.0.5.8.7/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8.7/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8.7/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8.7/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8.7/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8.7/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8.7/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8.7/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8.7/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      423 2023-04-26 00:16:34.000000 netin-1.0.5.8.7/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.8.7/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.8.7/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8.7/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8.7/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8.7/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8.7/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8.7/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8.7/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8.7/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6159 2023-04-25 17:16:17.000000 netin-1.0.5.8.7/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      296 2023-04-24 23:15:30.000000 netin-1.0.5.8.7/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8.7/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13472 2023-04-24 16:34:00.000000 netin-1.0.5.8.7/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-24 18:05:02.000000 netin-1.0.5.8.7/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5344 2023-04-24 18:36:49.000000 netin-1.0.5.8.7/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    23204 2023-04-26 00:15:00.000000 netin-1.0.5.8.7/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8.7/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2747 2023-04-24 18:05:16.000000 netin-1.0.5.8.7/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-24 18:05:38.000000 netin-1.0.5.8.7/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-25 11:41:22.000000 netin-1.0.5.8.7/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-24 18:05:57.000000 netin-1.0.5.8.7/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8.7/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8.7/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8.7/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8.7/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8.7/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8.7/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8828 2023-04-23 14:52:43.000000 netin-1.0.5.8.7/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      495 2023-04-24 13:42:57.000000 netin-1.0.5.8.7/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.8.7/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3615 2023-04-25 23:22:44.000000 netin-1.0.5.8.7/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8.7/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8.7/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1194 2023-04-24 11:51:14.000000 netin-1.0.5.8.7/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.8.7/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.8.7/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.8.7/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.8.7/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    26872 2023-04-26 00:16:17.000000 netin-1.0.5.8.7/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.865470 netin-1.0.5.8.7/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 00:46:58.000000 netin-1.0.5.8.7/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 00:46:58.000000 netin-1.0.5.8.7/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 00:46:58.000000 netin-1.0.5.8.7/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8.7/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 00:46:58.000000 netin-1.0.5.8.7/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 00:46:58.000000 netin-1.0.5.8.7/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8.7/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8.7/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8.7/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 00:46:58.869470 netin-1.0.5.8.7/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4256 2023-04-25 10:29:59.000000 netin-1.0.5.8.7/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8.8/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8.8/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.8.8/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8.8/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8.8/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8.8/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8.8/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8.8/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8.8/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8.8/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8.8/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      423 2023-04-26 01:47:14.000000 netin-1.0.5.8.8/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.8.8/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.8.8/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8.8/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8.8/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8.8/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8.8/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8.8/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6159 2023-04-25 17:16:17.000000 netin-1.0.5.8.8/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      296 2023-04-24 23:15:30.000000 netin-1.0.5.8.8/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8.8/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14008 2023-04-26 01:27:29.000000 netin-1.0.5.8.8/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-24 18:05:02.000000 netin-1.0.5.8.8/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5395 2023-04-26 00:57:56.000000 netin-1.0.5.8.8/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    23204 2023-04-26 00:15:00.000000 netin-1.0.5.8.8/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8.8/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2747 2023-04-24 18:05:16.000000 netin-1.0.5.8.8/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-24 18:05:38.000000 netin-1.0.5.8.8/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-25 11:41:22.000000 netin-1.0.5.8.8/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-24 18:05:57.000000 netin-1.0.5.8.8/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8.8/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8.8/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8.8/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8.8/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8.8/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8.8/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9295 2023-04-26 01:26:41.000000 netin-1.0.5.8.8/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      495 2023-04-24 13:42:57.000000 netin-1.0.5.8.8/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.8.8/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3615 2023-04-26 01:44:17.000000 netin-1.0.5.8.8/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8.8/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8.8/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1265 2023-04-26 01:25:38.000000 netin-1.0.5.8.8/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.8.8/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.8.8/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.8.8/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.8.8/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.8.8/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.437031 netin-1.0.5.8.8/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8.8/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 01:48:35.000000 netin-1.0.5.8.8/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8.8/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8.8/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8.8/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 01:48:35.441031 netin-1.0.5.8.8/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4256 2023-04-25 10:29:59.000000 netin-1.0.5.8.8/setup.py
```

### Comparing `netin-1.0.5.8.7/LICENSE` & `netin-1.0.5.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/PKG-INFO` & `netin-1.0.5.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.7
+Version: 1.0.5.8.8
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.7/README.rst` & `netin-1.0.5.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/examples/notebooks/deleteme.py` & `netin-1.0.5.8.8/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/random_edges.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/algorithms/sampling/sampling.py` & `netin-1.0.5.8.8/netin/algorithms/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/dh.py` & `netin-1.0.5.8.8/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/directed.py` & `netin-1.0.5.8.8/netin/generators/directed.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,20 @@
         self.activity = None
         self.expected_number_of_edges = None
 
     ############################################################
     # Init
     ############################################################
 
+    def _infer_model_name(self):
+        """
+        Infers the name of the model.
+        """
+        return self.set_model_name(const.DIRECTED_MODEL_NAME)
+
     def _validate_parameters(self):
         """
         Validates the parameters of the directed.
         """
         Graph._validate_parameters(self)
         val.validate_float(self.d, minimum=1. / (self.n * (self.n - 1)), maximum=1.)
         val.validate_float(self.plo_M, minimum=1. + const.EPSILON)
@@ -360,7 +366,19 @@
 
         Returns
         -------
         np.array
             activity distribution of all the nodes in the graph
         """
         return self.activity
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        obj = self.__class__(n=self.n,
+                              d=self.d,
+                              f_m=self.f_m,
+                              plo_M=self.plo_M,
+                              plo_m=self.plo_m,
+                              seed=self.seed)
+        return obj
```

### Comparing `netin-1.0.5.8.7/netin/generators/dpa.py` & `netin-1.0.5.8.8/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/dpah.py` & `netin-1.0.5.8.8/netin/generators/dpah.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,11 +150,13 @@
                               d=self.d,
                               f_m=self.f_m,
                               plo_M=self.plo_M,
                               plo_m=self.plo_m,
                               h_MM=self.h_MM,
                               h_mm=self.h_mm,
                               seed=self.seed)
-        obj._initialize(class_attribute=self.class_attribute,
-                        class_values=self.class_values,
-                        class_labels=self.class_labels)
+
+        # @TODO: check if this is necessary
+        # obj._initialize(class_attribute=self.class_attribute,
+        #                 class_values=self.class_values,
+        #                 class_labels=self.class_labels)
         return obj
```

### Comparing `netin-1.0.5.8.7/netin/generators/graph.py` & `netin-1.0.5.8.8/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/h.py` & `netin-1.0.5.8.8/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/pa.py` & `netin-1.0.5.8.8/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/pah.py` & `netin-1.0.5.8.8/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/patc.py` & `netin-1.0.5.8.8/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/patch.py` & `netin-1.0.5.8.8/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/tc.py` & `netin-1.0.5.8.8/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/tests/test_directed.py` & `netin-1.0.5.8.8/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/tests/test_dpah.py` & `netin-1.0.5.8.8/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/tests/test_patch.py` & `netin-1.0.5.8.8/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/tests/test_undirected.py` & `netin-1.0.5.8.8/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/generators/undirected.py` & `netin-1.0.5.8.8/netin/generators/undirected.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Tuple
 from typing import Union
 
 import networkx as nx
 import numpy as np
 import powerlaw
 
+from netin.utils import constants as const
 from netin.utils import validator as val
 from .graph import Graph
 
 
 class UnDiGraph(Graph):
     """Undirected graph base model.
 
@@ -143,14 +144,20 @@
 
         self._terminate()
 
     ############################################################
     # Getters and Setters
     ############################################################
 
+    def _infer_model_name(self):
+        """
+        Infers the name of the model.
+        """
+        return self.set_model_name(const.UNDIRECTED_MODEL_NAME)
+
     def get_expected_number_of_edges(self) -> int:
         """
         Computes and returns the expected number of edges based on minimum degree `k` and number of nodes `n`
 
         Returns
         -------
         int
@@ -226,7 +233,16 @@
         pl_m: float
             Powerlaw exponent for the minority class
         """
         fit_M, fit_m = self.fit_degree_powerlaw()
         pl_M = fit_M.power_law.alpha
         pl_m = fit_m.power_law.alpha
         return pl_M, pl_m
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              k=self.k,
+                              f_m=self.f_m,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.8.7/netin/stats/distributions.py` & `netin-1.0.5.8.8/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/stats/networks.py` & `netin-1.0.5.8.8/netin/stats/networks.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/stats/ranking.py` & `netin-1.0.5.8.8/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/utils/constants.py` & `netin-1.0.5.8.8/netin/utils/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 CLASS_VALUES = [MAJORITY_VALUE, MINORITY_VALUE]
 
 # GENERATIVE MODELS
 
 EPSILON = 0.00001
 MAX_TRIES_EDGE = 100
 
+DIRECTED_MODEL_NAME = 'Directed'
+UNDIRECTED_MODEL_NAME = 'Undirected'
+
 H_MODEL_NAME = 'Homophily'
 TC_MODEL_NAME = 'Triadic Closure'
 
 PA_MODEL_NAME = 'PA'
 PAH_MODEL_NAME = 'PAH'
 PATC_MODEL_NAME = 'PATC'
 PATCH_MODEL_NAME = 'PATCH'
```

### Comparing `netin-1.0.5.8.7/netin/utils/io.py` & `netin-1.0.5.8.8/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/utils/validator.py` & `netin-1.0.5.8.8/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/netin/viz/handlers.py` & `netin-1.0.5.8.8/netin/viz/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     rc('font', family='serif')
     rc('lines', linewidth=1.0)
     rc('axes', linewidth=0.5)
     rc('xtick.major', width=0.5)
     rc('ytick.major', width=0.5)
 
 
-def _get_edge_color(s: int, t: int, g: Graph) -> str:
+def _get_edge_color(s: int, t: int, g: Graph, maj_val: object = None, min_val: object = None) -> str:
     """
     Returns the color of the edge between s and t in the graph g.
     If the edge is homophilic (same attribute value for s and t), the color is the color of the attribute class.
     Otherwise, the color is mixed.
 
     Parameters
     ----------
@@ -65,19 +65,26 @@
         graph netin.Graph
 
     Returns
     -------
     color: str
         color of the edge
     """
+    maj_val = const.MAJORITY_VALUE if maj_val is None else maj_val
+    min_val = const.MINORITY_VALUE if min_val is None else min_val
+
     if g.get_class_value(s) == g.get_class_value(t):
-        if g.get_class_value(s) == const.MINORITY_VALUE:
-            return COLOR_MINORITY
-        else:
+        if g.get_class_value(s) == maj_val:
             return COLOR_MAJORITY
+
+        if g.get_class_value(s) == min_val:
+            return COLOR_MINORITY
+
+        return COLOR_UNKNOWN
+
     return COLOR_MIXED
 
 
 def _get_class_label_color(class_label: str, ylabel: str = None) -> str:
     """
     Returns the color for the class label.
 
@@ -263,50 +270,53 @@
         Additional arguments for the ``subplots_adjust`` and ``savefig`` functions of the figure.
     """
     iter_graph = [data] if isinstance(data, Graph) else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_graph), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
 
-    fig, axes = plt.subplots(nr, nc, figsize=(nc * cell_size, nr * cell_size), sharex=False, sharey=False)
+    sharex, sharey = (share_pos, share_pos)
+    fig, axes = plt.subplots(nr, nc, figsize=(nc * cell_size, nr * cell_size), sharex=sharex, sharey=sharey)
     node_size = kwargs.get('node_size', 1)
     node_shape = kwargs.get('node_shape', 'o')
     edge_width = kwargs.get('edge_width', 0.02)
     edge_style = kwargs.get('edge_style', 'solid')
     edge_arrows = kwargs.get('edge_arrows', True)
     arrow_style = kwargs.get('arrow_style', '-|>')
     arrow_size = kwargs.get('arrow_size', 2)
 
     pos = None
-    # same_n = len(set([g.number_of_nodes() for g in iter_graph])) == 1
     for cell in np.arange(nc * nr):
         row = cell // nc
         col = cell % nc
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
         if cell < len(iter_graph):
             g = iter_graph[cell]
 
-            pos = nx.spring_layout(g) if pos is None or not share_pos else pos # or not same_n
+            if pos is None or not share_pos:
+                pos = nx.spring_layout(g)
 
             # title
             ax.set_title(g.get_model_name())
 
             # nodes
-            maj = g.graph['class_values'][0]
-            # maj = g.graph['class_values'][g.graph['class_labels'].index(maj)]
+            maj_val = g.graph['class_values'][0]
+            min_val = g.graph['class_values'][1]
             nodes, node_colors = zip(
-                *[(node, COLOR_MAJORITY if data[g.graph['class_attribute']] == maj else COLOR_MINORITY)
+                *[(node, COLOR_MAJORITY if data[g.graph['class_attribute']] == maj_val else
+                COLOR_MINORITY if data[g.graph['class_attribute']] == min_val else
+                COLOR_UNKNOWN)
                   for node, data in g.nodes(data=True)])
             nx.draw_networkx_nodes(g, pos, nodelist=nodes, node_size=node_size, node_color=node_colors,
                                    node_shape=node_shape, ax=ax)
 
             # edges
             edges = g.edges()
-            edges, edge_colors = zip(*[((s, t), _get_edge_color(s, t, g)) for s, t in edges])
+            edges, edge_colors = zip(*[((s, t), _get_edge_color(s, t, g, maj_val=maj_val, min_val=min_val)) for s, t in edges])
             nx.draw_networkx_edges(g, pos, ax=ax, edgelist=edges, edge_color=edge_colors,
                                    width=edge_width, style=edge_style, arrows=edge_arrows, arrowstyle=arrow_style,
                                    arrowsize=arrow_size)
 
         # final touch
         ax.set_axis_off()
```

### Comparing `netin-1.0.5.8.7/netin.egg-info/PKG-INFO` & `netin-1.0.5.8.8/netin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.7
+Version: 1.0.5.8.8
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.7/netin.egg-info/SOURCES.txt` & `netin-1.0.5.8.8/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.7/setup.py` & `netin-1.0.5.8.8/setup.py`

 * *Files identical despite different names*

