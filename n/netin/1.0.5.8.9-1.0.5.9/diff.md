# Comparing `tmp/netin-1.0.5.8.9.tar.gz` & `tmp/netin-1.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.8.9.tar", last modified: Wed Apr 26 20:11:02 2023, max compression
+gzip compressed data, was "netin-1.0.5.9.tar", last modified: Wed Apr 26 21:43:46 2023, max compression
```

## Comparing `netin-1.0.5.8.9.tar` & `netin-1.0.5.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8.9/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8.9/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.8.9/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.911203 netin-1.0.5.8.9/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8.9/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8.9/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8.9/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8.9/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8.9/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8.9/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8.9/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8.9/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      479 2023-04-26 20:02:17.000000 netin-1.0.5.8.9/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.8.9/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/algorithms/sampling/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.8.9/netin/algorithms/sampling/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8.9/netin/algorithms/sampling/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8.9/netin/algorithms/sampling/degree_group_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8.9/netin/algorithms/sampling/degree_rank.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8.9/netin/algorithms/sampling/partial_crawls.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_edges.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_neighbor.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8.9/netin/algorithms/sampling/random_nodes.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6159 2023-04-25 17:16:17.000000 netin-1.0.5.8.9/netin/algorithms/sampling/sampling.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      523 2023-04-26 19:54:04.000000 netin-1.0.5.8.9/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8.9/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27992 2023-04-26 19:54:50.000000 netin-1.0.5.8.9/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8.9/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2748 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8.9/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8.9/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8.9/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8.9/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8.9/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8.9/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9951 2023-04-26 19:47:38.000000 netin-1.0.5.8.9/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.8.9/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.8.9/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5753 2023-04-26 19:48:11.000000 netin-1.0.5.8.9/netin/stats/networks.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8.9/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8.9/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.8.9/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.8.9/netin/utils/io.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.8.9/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.8.9/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.8.9/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.8.9/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.915203 netin-1.0.5.8.9/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3928 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8.9/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 20:11:02.000000 netin-1.0.5.8.9/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8.9/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8.9/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8.9/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 20:11:02.919203 netin-1.0.5.8.9/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.8.9/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.9/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.9/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3926 2023-04-26 21:43:46.498003 netin-1.0.5.9/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2654 2023-04-25 12:36:58.000000 netin-1.0.5.9/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.9/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.9/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.9/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.9/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.9/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.9/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.9/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.9/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      477 2023-04-26 21:37:21.000000 netin-1.0.5.9/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-25 16:30:10.000000 netin-1.0.5.9/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      280 2023-04-25 16:30:06.000000 netin-1.0.5.9/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.9/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.9/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.9/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.9/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.9/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.9/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.9/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6171 2023-04-26 21:06:58.000000 netin-1.0.5.9/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      524 2023-04-26 20:32:15.000000 netin-1.0.5.9/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.9/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14272 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5388 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    28889 2023-04-26 21:31:14.000000 netin-1.0.5.9/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8253 2023-04-26 21:06:58.000000 netin-1.0.5.9/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3565 2023-04-26 21:42:50.000000 netin-1.0.5.9/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7286 2023-04-26 21:43:01.000000 netin-1.0.5.9/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7758 2023-04-26 21:42:54.000000 netin-1.0.5.9/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-26 19:47:38.000000 netin-1.0.5.9/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.9/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.9/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.9/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.9/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.9/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.9/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9948 2023-04-26 20:38:34.000000 netin-1.0.5.9/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      574 2023-04-26 19:48:59.000000 netin-1.0.5.9/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5041 2023-04-26 00:35:20.000000 netin-1.0.5.9/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5990 2023-04-26 20:37:47.000000 netin-1.0.5.9/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.9/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.9/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1447 2023-04-26 18:57:24.000000 netin-1.0.5.9/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      583 2023-04-25 21:31:19.000000 netin-1.0.5.9/netin/utils/io.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2184 2023-04-25 17:56:25.000000 netin-1.0.5.9/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      462 2023-04-26 01:14:12.000000 netin-1.0.5.9/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      493 2023-04-26 01:13:59.000000 netin-1.0.5.9/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    27179 2023-04-26 01:45:19.000000 netin-1.0.5.9/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.494003 netin-1.0.5.9/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3926 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1708 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.9/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-26 21:43:46.000000 netin-1.0.5.9/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-26 21:43:46.498003 netin-1.0.5.9/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.9/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.9/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.9/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-26 21:43:46.498003 netin-1.0.5.9/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4291 2023-04-26 19:17:45.000000 netin-1.0.5.9/setup.py
```

### Comparing `netin-1.0.5.8.9/LICENSE` & `netin-1.0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/PKG-INFO` & `netin-1.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.9
+Version: 1.0.5.9
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.9/README.rst` & `netin-1.0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/examples/notebooks/deleteme.py` & `netin-1.0.5.9/examples/notebooks/deleteme.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/degree_group_rank.py` & `netin-1.0.5.9/netin/algorithms/sampling/degree_group_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/degree_rank.py` & `netin-1.0.5.9/netin/algorithms/sampling/degree_rank.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/partial_crawls.py` & `netin-1.0.5.9/netin/algorithms/sampling/partial_crawls.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/random_edges.py` & `netin-1.0.5.9/netin/algorithms/sampling/random_edges.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/random_neighbor.py` & `netin-1.0.5.9/netin/algorithms/sampling/random_neighbor.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/random_nodes.py` & `netin-1.0.5.9/netin/algorithms/sampling/random_nodes.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/algorithms/sampling/sampling.py` & `netin-1.0.5.9/netin/algorithms/sampling/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             num_edges = sample.number_of_edges()
 
         if num_edges < const.MIN_EDGES:
             raise RuntimeWarning("The sample has no edges.")
 
         self.sample = sample.copy()
         self.sample.node_list = [n for n in self.sample.node_list if n in self.sample.nodes()]
-        self.sample.node_labels = {n: l for n, l in self.sample.node_labels.items() if n in self.sample.nodes()}
+        self.sample.node_class_values = {n: l for n, l in self.sample.node_class_values.items() if n in self.sample.nodes()}
         gc.collect()
 
     def _set_graph_metadata(self):
         """
         Updates the training sample subgraph metadata
         """
         self.sample.graph['method'] = self.method_name
```

### Comparing `netin-1.0.5.8.9/netin/generators/__init__.py` & `netin-1.0.5.9/netin/generators/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .h import Homophily
 from .pa import PA
 from .pah import PAH
 from .patc import PATC
 from .patch import PATCH
 from .tc import TriadicClosure
 from .undirected import UnDiGraph
-from .undirected import calculate_degree_powerlaw_exponents
+from .undirected import calculate_degree_powerlaw_exponents
```

### Comparing `netin-1.0.5.8.9/netin/generators/dh.py` & `netin-1.0.5.9/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/directed.py` & `netin-1.0.5.9/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/dpa.py` & `netin-1.0.5.9/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/dpah.py` & `netin-1.0.5.9/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/graph.py` & `netin-1.0.5.9/netin/generators/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self.n_m = 0
         self.n_M = 0
         self.model_name = None
         self.class_attribute = None
         self.class_values = None
         self.class_labels = None
         self.node_list = None
-        self.node_labels = None
+        self.node_class_values = None
         self._gen_start_time = None
         self._gen_duration = None
 
     ############################################################
     # Init
     ############################################################
 
@@ -137,14 +137,47 @@
                'seed': self.seed}
         return obj
 
     ############################################################
     # Getters & Setters
     ############################################################
 
+    def set_node_list(self, node_list: np.array):
+        """
+        Sets the node list.
+
+        Parameters
+        ----------
+        node_list: np.array
+            vector of nodes
+        """
+        self.node_list = node_list
+
+    def get_node_list(self) -> np.array:
+        """
+        Returns the vector of nodes.
+
+        Returns
+        -------
+        np.array
+            vector of nodes
+        """
+        return self.node_list
+
+    def set_node_class_values(self, node_class_values: dict):
+        """
+        Sets the node class values.
+
+        Parameters
+        ----------
+        node_class_values: dict
+            dictionary of node class values
+        """
+        self.node_class_values = node_class_values
+
     def set_expected_number_of_nodes(self, n: int):
         """
         Sets the expected number of nodes.
 
         Parameters
         ----------
         n: int
@@ -440,15 +473,15 @@
         """
         Initializes the list of nodes with their respective labels.
         """
         self.node_list = np.arange(self.n)
         self.n_M = int(round(self.n * (1 - self.f_m)))
         self.n_m = self.n - self.n_M
         minorities = np.random.choice(self.node_list, self.n_m, replace=False)
-        self.node_labels = {n: int(n in minorities) for n in self.node_list}
+        self.node_class_values = {n: int(n in minorities) for n in self.node_list}
 
     def get_special_targets(self, source: int) -> object:
         pass
 
     def get_potential_nodes_to_connect(self, source: int, targets: Set[int]) -> Set[int]:
         """
         Returns the set of potential target nodes to connect to the source node.
@@ -520,15 +553,15 @@
         Basic instructions run before generating the graph.
         """
         self._gen_start_time = time.time()
 
         # init graph and nodes
         self._initialize()
         self.add_nodes_from(self.node_list)
-        nx.set_node_attributes(self, self.node_labels, self.class_attribute)
+        nx.set_node_attributes(self, self.node_class_values, self.class_attribute)
 
         # iterate
         # for each source_node, get target (based on specific mechanisms), then add edge, update special targets
 
     def _terminate(self):
         """
         Instructions run after the generation of the graph.
@@ -780,15 +813,15 @@
         g.add_nodes_from((n, d.copy()) for n, d in self._node.items())
         g.add_edges_from(
             (u, v, datadict.copy())
             for u, nbrs in self._adj.items()
             for v, datadict in nbrs.items()
         )
         g.node_list = self.node_list.copy()
-        g.node_labels = self.node_labels.copy()
+        g.node_class_values = self.node_class_values.copy()
         g.n_m = self.n_m
         g.n_M = self.n_M
         return g
 
 
 def fit_powerlaw_groups(g: Graph, metric: str) -> Tuple[powerlaw.Fit, powerlaw.Fit]:
     """
@@ -855,21 +888,24 @@
         plo_M, plo_m = netin.calculate_out_degree_powerlaw_exponents(g)
         gn = netin.DiGraph(n=n, d=d, f_m=f_m, plo_M=plo_M, plo_m=plo_m, seed=seed)
     else:
         k = net.get_min_degree(g)
         gn = netin.UnDiGraph(n=n, k=k, f_m=f_m, seed=seed)
 
     gn.set_model_name(name)
-    gn.add_edges_from(g.edges(data=True))
     gn.add_nodes_from(g.nodes(data=True))
+    gn.add_edges_from(g.edges(data=True))
 
     counter = Counter([obj[class_attribute] for n, obj in g.nodes(data=True)])
     class_values, class_counts = zip(*counter.most_common())  # from M to m
     class_labels = ['female' if c == 1 else 'male' if c == 0 else 'unknown' for c in class_values]
     gn._initialize(class_attribute=class_attribute, class_values=class_values, class_labels=class_labels)
 
+    gn.set_node_list(np.asarray(g.nodes()))
+    gn.set_node_class_values({n: obj[class_attribute] for n, obj in g.nodes(data=True)})
+
     obj = {'model': gn.get_model_name(),
            'e': g.number_of_edges()}
 
     gn.graph.update(obj)
 
     return gn
```

### Comparing `netin-1.0.5.8.9/netin/generators/h.py` & `netin-1.0.5.9/netin/generators/h.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             Target node id
 
         Returns
         -------
         h: float
             homophily (similarity) between source and target nodes (minimum=0, maximum=1.)
         """
-        return self.mixing_matrix[self.node_labels[source], self.node_labels[target]]
+        return self.mixing_matrix[self.node_class_values[source], self.node_class_values[target]]
 
     ############################################################
     # Generation
     ############################################################
 
     def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
         """
```

### Comparing `netin-1.0.5.8.9/netin/generators/pah.py` & `netin-1.0.5.9/netin/generators/patch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
-from sympy import Eq
-from sympy import solve
-from sympy import symbols
 
-from netin.generators.h import Homophily
+from netin.generators.tc import TriadicClosure
 from netin.utils import constants as const
-from .pa import PA
+from .pah import PAH
 
 
-class PAH(PA, Homophily):
-    """Creates a new PAH instance. An undirected graph with preferential attachment and homophily.
+class PATCH(PAH, TriadicClosure):
+    """Creates a new PATCH instance. An undirected graph with preferential attachment, homophily, and triadic closure.
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
     k: int
@@ -26,173 +23,181 @@
 
     h_MM: float
         homophily (similarity) between majority nodes (minimum=0, maximum=1.)
 
     h_mm: float
         homophily (similarity) between minority nodes (minimum=0, maximum=1.)
 
-    seed: object
-        seed for random number generator
+    tc: float
+        probability of a new edge to close a triad (minimum=0, maximum=1.)
 
     Notes
     -----
-    The initialization is an undirected with n nodes, where f_m are the minority.
+    The initialization is an undirected with n nodes and no edges.
     Then, everytime a node is selected as source, it gets connected to k target nodes.
-    Target nodes are selected via preferential attachment (in-degree) and homophily (h_**).
-    This model is based on [Karimi2018]_ known as the "Barabasi model with homophily" or "BA Homophily".
+    Target nodes are selected via preferential attachment (in-degree) [BarabasiAlbert1999]_,
+    homophily (h_**; see :class:`netin.Homophily`) [Karimi2018]_,
+    and triadic closure (see :class:`netin.TriadicClosure`) [HolmeKim2002]_.
     """
 
     ############################################################
     # Constructor
     ############################################################
 
-    def __init__(self, n: int, k: int, f_m: float, h_MM: float, h_mm: float, seed: object = None):
-        PA.__init__(self, n=n, k=k, f_m=f_m, seed=seed)
-        Homophily.__init__(self, n=n, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
+    def __init__(self, n: int, k: int, f_m: float, h_mm: float, h_MM: float, tc: float, seed: object = None):
+        PAH.__init__(self, n=n, k=k, f_m=f_m, h_MM=h_MM, h_mm=h_mm, seed=seed)
+        TriadicClosure.__init__(self, n=n, f_m=f_m, tc=tc, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
     def _infer_model_name(self):
         """
         Infers the name of the model.
         """
-        return self.set_model_name(const.PAH_MODEL_NAME)
+        return self.set_model_name(const.PATCH_MODEL_NAME)
 
     def _validate_parameters(self):
         """
         Validates the parameters of the undirected.
         """
-        PA._validate_parameters(self)
-        Homophily._validate_parameters(self)
+        PAH._validate_parameters(self)
+        TriadicClosure._validate_parameters(self)
 
     def get_metadata_as_dict(self) -> dict:
         """
-        Returns the metadata (parameters) of the model as a dictionary.
+        Returns a dictionary with the metadata of the PATCH graph.
 
         Returns
         -------
         dict
-            metadata of the model
+            the graph  metadata as a dictionary
         """
-        obj = PA.get_metadata_as_dict(self)
-        obj.update(Homophily.get_metadata_as_dict(self))
-        return obj
+        obj1 = PAH.get_metadata_as_dict(self)
+        obj2 = TriadicClosure.get_metadata_as_dict(self)
+        obj1.update(obj2)
+        return obj1
 
     ############################################################
     # Generation
     ############################################################
 
-    def _initialize(self, class_attribute: str = 'm', class_values: list = None, class_labels: list = None):
+    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
+                                 special_targets: Union[None, object, iter] = None) -> Tuple[np.array, set[int]]:
         """
-        Initializes the model.
+        Returns the probabilities of nodes to be selected as target nodes.
 
         Parameters
         ----------
-        class_attribute: str
-            name of the attribute that represents the class
+        source: int
+            source node id
 
-        class_values: list
-            values of the class attribute
+        target_set: set
+            set of target node ids
+
+        special_targets: dict
+            dictionary of special target node ids to be considered
+
+        Returns
+        -------
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
 
-        class_labels: list
-            labels of the class attribute mapping the class_values.
         """
-        PA._initialize(self, class_attribute, class_values, class_labels)
-        Homophily._initialize(self, class_attribute, class_values, class_labels)
+        return TriadicClosure.get_target_probabilities(self, source, target_set, special_targets)
 
-    def get_target_probabilities(self, source: Union[None, int], target_set: Union[None, Set[int]],
-                                 special_targets: Union[None, object, iter] = None) -> tuple[np.array, set[int]]:
+    def get_target_probabilities_regular(self, source: Union[None, int], target_set: Union[None, Set[int]],
+                                         special_targets: Union[None, object, iter] = None) -> Tuple[
+        np.ndarray, set[int]]:
         """
-        Returns the probabilities of selecting a target node from a set of nodes based on the preferential attachment
-        and homophily.
+        Returns the probability of nodes to be selected as target nodes using the
+        preferential attachment with homophily mechanism.
 
         Parameters
         ----------
         source: int
-            source node
+            source node id
 
-        target_set: set[int]
-            set of target nodes
+        target_set: set
+            set of target node ids
 
-        special_targets: object
-            special targets
+        special_targets: dict
+            dictionary of special target node ids to be considered
 
         Returns
         -------
-        tuple[np.array, set[int]]
-            probabilities of selecting a target node from a set of nodes, and the set of target nodes
+        tuple
+            probabilities of nodes to be selected as target nodes, and set of target of nodes
         """
-        probs = np.array([self.get_homophily_between_source_and_target(source, target) *
-                          (self.degree(target) + const.EPSILON) for target in target_set])
-        probs /= probs.sum()
-        return probs, target_set
+        return PAH.get_target_probabilities(self, source, target_set, special_targets)
+
+    def get_special_targets(self, source: int) -> object:
+        """
+        Returns an empty dictionary (source node ids)
+
+        Parameters
+        ----------
+        source : int
+            Newly added node
+
+        Returns
+        -------
+        Dict
+            Empty dictionary
+        """
+        return TriadicClosure.get_special_targets(self, source)
 
     ############################################################
     # Calculations
     ############################################################
 
     def info_params(self):
         """
-        Shows the parameters of the model.
+        Shows the (input) parameters of the graph.
         """
-        PA.info_params(self)
-        Homophily.info_params(self)
+        PAH.info_params(self)
+        TriadicClosure.info_params(self)
 
     def info_computed(self):
         """
-        Shows the computed properties of the graph.
+        Shows the (computed) properties of the graph.
         """
-        PA.info_computed(self)
-        Homophily.info_computed(self)
+        PAH.info_computed(self)
+        TriadicClosure.info_computed(self)
 
     def infer_homophily_values(self) -> Tuple[float, float]:
         """
-        Infers the level of homophily using the analytical solution of the model.
+        Infers analytically the homophily values of the graph.
 
         Returns
         -------
-        tuple[float, float]
-            homophily between majority nodes, and homophily between minority nodes
-
-        Notes
-        -----
-        See derivations in [Karimi2018]_.
+        tuple
+            homophily values of the graph (majority, minority)
         """
-        f_m = self.calculate_fraction_of_minority()
-        f_M = 1 - f_m
-
-        e = self.calculate_edge_type_counts()
-        e_MM = e['MM']
-        e_mm = e['mm']
-        M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
-
-        p_MM = e_MM / M
-        p_mm = e_mm / M
-
-        pl_M, pl_m = self.calculate_degree_powerlaw_exponents()
-        b_M = -1 / (pl_M + 1)
-        b_m = -1 / (pl_m + 1)
-
-        # equations
-        hmm, hMM, hmM, hMm = symbols('hmm hMM hmM hMm')
-        eq1 = Eq((f_m * f_m * hmm * (1 - b_M)) / ((f_m * hmm * (1 - b_M)) + (f_M * hmM * (1 - b_m))), p_mm)
-        eq2 = Eq(hmm + hmM, 1)
+        h_MM = None
+        h_mm = None
+        return h_MM, h_mm
 
-        eq3 = Eq((f_M * f_M * hMM * (1 - b_m)) / ((f_M * hMM * (1 - b_m)) + (f_m * hMm * (1 - b_M))), p_MM)
-        eq4 = Eq(hMM + hMm, 1)
+    def infer_triadic_closure(self) -> float:
+        """
+        Infers analytically the triadic closure value of the graph.
 
-        solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
-        h_MM, h_mm = solution[hMM], solution[hmm]
-        return h_MM, h_mm
+        Returns
+        -------
+        float
+            triadic closure probability of the graph
+        """
+        tc = None
+        return tc
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         return self.__class__(n=self.n,
                               k=self.k,
                               f_m=self.f_m,
+                              tc=self.tc,
                               h_MM=self.h_MM,
                               h_mm=self.h_mm,
                               seed=self.seed)
```

### Comparing `netin-1.0.5.8.9/netin/generators/patc.py` & `netin-1.0.5.9/netin/generators/patc.py`

 * *Files 7% similar despite different names*

```diff
@@ -206,19 +206,58 @@
         Approximates analytically the triadic closure value of the graph.
 
         Returns
         -------
         float
             triadic closure probability of the graph
         """
-        tc = nx.average_clustering(self)
+        tc = infer_triadic_closure(self)
         return tc
 
     def _makecopy(self):
         """
         Makes a copy of the current object.
         """
         return self.__class__(n=self.n,
                               k=self.k,
                               f_m=self.f_m,
                               tc=self.tc,
                               seed=self.seed)
+
+    @staticmethod
+    def fit(g, n=None, k=None, seed=None):
+        """
+        It fits the PATC model to the given graph.
+
+        Parameters
+        ----------
+        g: netin.UnDiGraph
+            graph to fit the model to
+
+        n: int
+            number of nodes to override (e.g., to generate a smaller network)
+
+        k: int
+            minimum node degree to override (e.g., to generate a denser network ``k>1``)
+        seed
+
+        Returns
+        -------
+        netin.PATC
+            fitted model
+        """
+        n = n or g.number_of_nodes()
+        k = k or g.calculate_minimum_degree()
+        f_m = g.calculate_fraction_of_minority()
+        tc = infer_triadic_closure(g)
+
+        new_g = PATC(n=n,
+                    k=k,
+                    f_m=f_m,
+                    tc=tc,
+                    seed=seed)
+        new_g.generate()
+
+        return new_g
+
+def infer_triadic_closure(g):
+    return nx.average_clustering(g)
```

### Comparing `netin-1.0.5.8.9/netin/generators/tc.py` & `netin-1.0.5.9/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/tests/test_directed.py` & `netin-1.0.5.9/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/tests/test_dpah.py` & `netin-1.0.5.9/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/tests/test_patch.py` & `netin-1.0.5.9/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/tests/test_undirected.py` & `netin-1.0.5.9/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/generators/undirected.py` & `netin-1.0.5.9/netin/generators/undirected.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,11 +261,11 @@
         Graph to calculate the power law exponents for
 
     Returns
     -------
     Tuple[float, float]
         power law exponents for the in-degree distribution of the majority and minority class
     """
-    fit_M, fit_m = g.fit_powerlaw(metric='in_degree')
+    fit_M, fit_m = g.fit_powerlaw(metric='degree')
     pl_M = fit_M.power_law.alpha
     pl_m = fit_m.power_law.alpha
     return pl_M, pl_m
```

### Comparing `netin-1.0.5.8.9/netin/stats/__init__.py` & `netin-1.0.5.9/netin/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/stats/distributions.py` & `netin-1.0.5.9/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/stats/networks.py` & `netin-1.0.5.9/netin/stats/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,27 @@
     class_attribute: str
         The name of the attribute that holds the class label of each node.
 
     Returns
     -------
     Counter
         Counter holding the edge type counts
+
+    Notes
+    -----
+    Class labels are assumed to be binary. The minority class is assumed to be labeled as 1.
     """
     majority, minority, class_attribute = _get_class_labels(g, class_attribute)
     class_values = [majority, minority]
     class_labels = [const.MAJORITY_LABEL, const.MINORITY_LABEL]
 
     counts = Counter([f"{class_labels[class_values.index(g.nodes[e[0]][class_attribute])]}"
                       f"{class_labels[class_values.index(g.nodes[e[1]][class_attribute])]}"
-                      for e in g.edges])
+                      for e in g.edges if g.nodes[e[0]][class_attribute] in class_values and
+                      g.nodes[e[1]][class_attribute] in class_values])
 
     if fractions:
         total = sum(counts.values())
         counts = Counter({k: v / total for k, v in counts.items()})
 
     return counts
```

### Comparing `netin-1.0.5.8.9/netin/stats/ranking.py` & `netin-1.0.5.9/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/utils/constants.py` & `netin-1.0.5.9/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/utils/io.py` & `netin-1.0.5.9/netin/utils/io.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/utils/validator.py` & `netin-1.0.5.9/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin/viz/handlers.py` & `netin-1.0.5.9/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/netin.egg-info/PKG-INFO` & `netin-1.0.5.9/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.8.9
+Version: 1.0.5.9
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.8.9/netin.egg-info/SOURCES.txt` & `netin-1.0.5.9/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.8.9/setup.py` & `netin-1.0.5.9/setup.py`

 * *Files identical despite different names*

