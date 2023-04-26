# Comparing `tmp/dreem-0.1.6.tar.gz` & `tmp/dreem-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreem-0.1.6.tar", last modified: Mon Apr  3 18:53:35 2023, max compression
+gzip compressed data, was "dreem-0.1.8.tar", last modified: Wed Apr 26 03:43:48 2023, max compression
```

## Comparing `dreem-0.1.6.tar` & `dreem-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.305756 dreem-0.1.6/
--rw-r--r--   0 ymdt       (501) staff       (20)     1227 2023-03-27 06:57:46.000000 dreem-0.1.6/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)      119 2023-03-27 07:03:07.000000 dreem-0.1.6/MANIFEST.in
--rw-r--r--   0 ymdt       (501) staff       (20)     1106 2023-04-03 18:53:35.305568 dreem-0.1.6/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      827 2023-03-27 06:57:46.000000 dreem-0.1.6/README.md
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.289363 dreem-0.1.6/dreem/
--rw-r--r--   0 ymdt       (501) staff       (20)      199 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/__init__.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.291643 dreem-0.1.6/dreem/aggregate/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/aggregate/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2651 2023-03-02 22:29:36.000000 dreem-0.1.6/dreem/aggregate/library.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1976 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/aggregate/library_samples.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6627 2023-03-30 18:12:38.000000 dreem-0.1.6/dreem/aggregate/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3388 2023-04-03 18:48:37.000000 dreem-0.1.6/dreem/aggregate/mutation_count.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.292833 dreem-0.1.6/dreem/align/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.6/dreem/align/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    21882 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/align/fq2bam.py
--rwxr-xr-x   0 ymdt       (501) staff       (20)    25001 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/align/fqs.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6683 2023-03-31 23:28:51.000000 dreem-0.1.6/dreem/align/main.py
--rwxr-xr-x   0 ymdt       (501) staff       (20)     7852 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/align/xams.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.293684 dreem-0.1.6/dreem/cluster/
--rw-r--r--   0 ymdt       (501) staff       (20)    13117 2023-03-30 16:23:58.000000 dreem-0.1.6/dreem/cluster/EMclustering.py
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-30 16:23:58.000000 dreem-0.1.6/dreem/cluster/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     9197 2023-04-03 18:48:30.000000 dreem-0.1.6/dreem/cluster/bitvector.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6513 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/cluster/clusteringAnalysis.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3381 2023-03-30 16:23:58.000000 dreem-0.1.6/dreem/cluster/main.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.294177 dreem-0.1.6/dreem/demultiplex/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/demultiplex/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    38426 2023-03-30 16:23:58.000000 dreem-0.1.6/dreem/demultiplex/demultiplex.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1716 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/demultiplex/main.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.295338 dreem-0.1.6/dreem/draw/
--rw-r--r--   0 ymdt       (501) staff       (20)      315 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/draw/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      225 2023-03-02 22:29:36.000000 dreem-0.1.6/dreem/draw/load_dataset.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5696 2023-03-28 20:44:09.000000 dreem-0.1.6/dreem/draw/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6655 2023-03-28 18:36:59.000000 dreem-0.1.6/dreem/draw/manipulator.py
--rw-r--r--   0 ymdt       (501) staff       (20)    17282 2023-04-03 18:51:59.000000 dreem-0.1.6/dreem/draw/plotter.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.295519 dreem-0.1.6/dreem/draw/resources/
--rw-r--r--   0 ymdt       (501) staff       (20)  1615050 2023-03-02 22:29:36.000000 dreem-0.1.6/dreem/draw/resources/my_dataset.feather
--rw-r--r--   0 ymdt       (501) staff       (20)    16075 2023-04-03 18:48:00.000000 dreem-0.1.6/dreem/draw/study.py
--rw-r--r--   0 ymdt       (501) staff       (20)    11285 2023-03-04 01:28:54.000000 dreem-0.1.6/dreem/draw/util.py
--rw-r--r--   0 ymdt       (501) staff       (20)     9587 2023-03-31 23:28:51.000000 dreem-0.1.6/dreem/main.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.298364 dreem-0.1.6/dreem/resources/
--rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.6/dreem/resources/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      475 2023-02-28 01:36:53.000000 dreem-0.1.6/dreem/resources/get_attributes.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.302158 dreem-0.1.6/dreem/util/
--rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.6/dreem/util/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      163 2023-03-06 17:48:28.000000 dreem-0.1.6/dreem/util/artxt.py
--rw-r--r--   0 ymdt       (501) staff       (20)    24727 2023-04-03 18:48:03.000000 dreem-0.1.6/dreem/util/cli.py
--rw-r--r--   0 ymdt       (501) staff       (20)     4365 2023-02-28 01:36:53.000000 dreem-0.1.6/dreem/util/dms.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6867 2023-03-31 23:28:51.000000 dreem-0.1.6/dreem/util/docdef.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2264 2023-03-02 22:29:36.000000 dreem-0.1.6/dreem/util/docstring.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1911 2023-03-02 22:29:36.000000 dreem-0.1.6/dreem/util/dump.py
--rw-r--r--   0 ymdt       (501) staff       (20)    11822 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/util/files_sanity.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3423 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/util/logs.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5530 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/util/parallel.py
--rw-r--r--   0 ymdt       (501) staff       (20)    58421 2023-03-30 16:23:58.000000 dreem-0.1.6/dreem/util/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7414 2023-03-27 06:57:46.000000 dreem-0.1.6/dreem/util/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     7900 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/util/seq.py
--rw-r--r--   0 ymdt       (501) staff       (20)      859 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/util/shell.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6024 2023-03-31 23:28:51.000000 dreem-0.1.6/dreem/util/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.304889 dreem-0.1.6/dreem/vector/
--rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.6/dreem/vector/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6472 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/vector/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)    71418 2023-04-03 18:48:08.000000 dreem-0.1.6/dreem/vector/profile.py
--rw-r--r--   0 ymdt       (501) staff       (20)    15663 2023-04-03 01:33:28.000000 dreem-0.1.6/dreem/vector/samread.py
--rw-r--r--   0 ymdt       (501) staff       (20)    38386 2023-03-31 23:28:51.000000 dreem-0.1.6/dreem/vector/vector.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.290742 dreem-0.1.6/dreem.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     1106 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     1481 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       43 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/entry_points.txt
--rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        6 2023-04-03 18:53:35.000000 dreem-0.1.6/dreem.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      731 2023-03-27 06:57:46.000000 dreem-0.1.6/env.yml
--rw-r--r--   0 ymdt       (501) staff       (20)      648 2023-04-03 01:51:29.000000 dreem-0.1.6/pyproject.toml
--rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-03 17:22:06.000000 dreem-0.1.6/requirements.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-04-03 18:53:35.305805 dreem-0.1.6/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      965 2023-04-03 18:53:22.000000 dreem-0.1.6/setup.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-03 18:53:35.305306 dreem-0.1.6/test/
--rw-r--r--   0 ymdt       (501) staff       (20)     7060 2023-04-03 17:22:04.000000 dreem-0.1.6/test/test_pipeline.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.445230 dreem-0.1.8/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1227 2023-03-27 06:57:46.000000 dreem-0.1.8/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)      131 2023-04-19 20:17:44.000000 dreem-0.1.8/MANIFEST.in
+-rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-04-26 03:43:48.445064 dreem-0.1.8/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      916 2023-04-22 00:57:35.000000 dreem-0.1.8/README.md
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.433334 dreem-0.1.8/dreem/
+-rw-r--r--   0 ymdt       (501) staff       (20)      177 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/__init__.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.435462 dreem-0.1.8/dreem/aggregate/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/aggregate/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2651 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/aggregate/library.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1976 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/aggregate/library_samples.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6714 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/aggregate/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3388 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/aggregate/mutation_count.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.436492 dreem-0.1.8/dreem/align/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.8/dreem/align/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    21882 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/align/fq2bam.py
+-rwxr-xr-x   0 ymdt       (501) staff       (20)    25001 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/align/fqs.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7100 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/align/main.py
+-rwxr-xr-x   0 ymdt       (501) staff       (20)     9982 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/align/xams.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.437423 dreem-0.1.8/dreem/cluster/
+-rw-r--r--   0 ymdt       (501) staff       (20)    13117 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/cluster/EMclustering.py
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/cluster/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8800 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/bitvector.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6503 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/clusteringAnalysis.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3628 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/cluster/main.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.438014 dreem-0.1.8/dreem/demultiplex/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-27 06:57:46.000000 dreem-0.1.8/dreem/demultiplex/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    38971 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/demultiplex/demultiplex.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1819 2023-04-21 17:32:54.000000 dreem-0.1.8/dreem/demultiplex/main.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.439322 dreem-0.1.8/dreem/draw/
+-rw-r--r--   0 ymdt       (501) staff       (20)      315 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/draw/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      225 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/draw/load_dataset.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5995 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/draw/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6655 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/draw/manipulator.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    22424 2023-04-21 23:08:14.000000 dreem-0.1.8/dreem/draw/plotter.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.439512 dreem-0.1.8/dreem/draw/resources/
+-rw-r--r--   0 ymdt       (501) staff       (20)  1615050 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/draw/resources/my_dataset.feather
+-rw-r--r--   0 ymdt       (501) staff       (20)    16796 2023-04-21 22:52:06.000000 dreem-0.1.8/dreem/draw/study.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    11285 2023-03-04 01:28:54.000000 dreem-0.1.8/dreem/draw/util.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      766 2023-04-24 02:55:28.000000 dreem-0.1.8/dreem/env.yml
+-rw-r--r--   0 ymdt       (501) staff       (20)    10067 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/requirements.txt
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.440691 dreem-0.1.8/dreem/resources/
+-rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/resources/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      475 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/resources/get_attributes.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.443463 dreem-0.1.8/dreem/util/
+-rw-r--r--   0 ymdt       (501) staff       (20)        0 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/util/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      163 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/artxt.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    25083 2023-04-21 17:32:54.000000 dreem-0.1.8/dreem/util/cli.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7279 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/dependencies.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     4365 2023-02-28 01:36:53.000000 dreem-0.1.8/dreem/util/dms.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6867 2023-04-04 22:14:41.000000 dreem-0.1.8/dreem/util/docdef.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2264 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/util/docstring.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1911 2023-03-02 22:29:36.000000 dreem-0.1.8/dreem/util/dump.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    13411 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/files_sanity.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3682 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/logs.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5530 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/parallel.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    58372 2023-04-21 17:36:14.000000 dreem-0.1.8/dreem/util/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7376 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     8030 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/util/seq.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      859 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/shell.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6024 2023-04-11 18:17:48.000000 dreem-0.1.8/dreem/util/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.444277 dreem-0.1.8/dreem/vector/
+-rw-r--r--   0 ymdt       (501) staff       (20)       35 2023-03-06 17:48:28.000000 dreem-0.1.8/dreem/vector/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6621 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    71580 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/profile.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    15683 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/samread.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    38492 2023-04-19 20:17:44.000000 dreem-0.1.8/dreem/vector/vector.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.434490 dreem-0.1.8/dreem.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1195 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     1548 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       43 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/entry_points.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)     2501 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        6 2023-04-26 03:43:48.000000 dreem-0.1.8/dreem.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      648 2023-04-03 01:51:29.000000 dreem-0.1.8/pyproject.toml
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-04-26 03:43:48.445291 dreem-0.1.8/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      971 2023-04-26 03:43:01.000000 dreem-0.1.8/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-04-26 03:43:48.444818 dreem-0.1.8/test/
+-rw-r--r--   0 ymdt       (501) staff       (20)     2001 2023-04-24 02:55:28.000000 dreem-0.1.8/test/test_demultiplexing.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     7167 2023-04-19 20:17:44.000000 dreem-0.1.8/test/test_pipeline.py
```

### Comparing `dreem-0.1.6/LICENSE` & `dreem-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/PKG-INFO` & `dreem-0.1.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-Metadata-Version: 2.1
-Name: dreem
-Version: 0.1.6
-Summary: DREEM solves RNA structure ensembles using chemical probing data
-Home-page: https://github.com/rouskinlab/dreem
-Author: Silvi Rouskin Lab
-Author-email: silvi@hms.harvard.edu
-Requires-Python: >=3.10
-License-File: LICENSE
-
-[![Build documentation](https://github.com/rouskinlab/dreem/actions/workflows/documentation.yaml/badge.svg?branch=main)](https://github.com/rouskinlab/dreem/actions/workflows/documentation.yaml)
+[![Build docs](https://github.com/rouskinlab/dreem/actions/workflows/documentation.yml/badge.svg)](https://github.com/rouskinlab/dreem/actions/workflows/documentation.yml)
 [![Run tests](https://github.com/rouskinlab/dreem/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/rouskinlab/dreem/actions/workflows/tests.yaml)
 
 # DREEM
 
 Prof. Silvi Rouskin's [DREEM algorithm](https://www.nature.com/articles/s41586-020-2253-5).
 
+## Installation
+
+Installation instructions [here](https://rouskinlab.github.io/dreem/dreem/installation.html).
+
 ## Documentation
 
 The documentation is available on [Github Pages](https://rouskinlab.github.io/dreem).
 
 ## Contributors
 
 Yves Martin, Scott Grote, Matthew Allan, Albéric de Lajarte.
```

### Comparing `dreem-0.1.6/dreem/aggregate/library.py` & `dreem-0.1.8/dreem/aggregate/library.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/aggregate/library_samples.py` & `dreem-0.1.8/dreem/aggregate/library_samples.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/aggregate/main.py` & `dreem-0.1.8/dreem/aggregate/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                         opt_rnastructure_deltag_ensemble,
                         opt_rnastructure_probability,
                         opt_verbose)
 from ..util.dump import *
 from ..util.files_sanity import check_library, check_samples
 from ..util.rnastructure import RNAstructure
 from ..vector.profile import VectorReader
-
+from ..util.dependencies import *
 
 params = [
     opt_fasta,
     opt_bv_files,
     opt_library,
     opt_samples,
     opt_clustering_file,
@@ -67,14 +67,16 @@
         rnastructure_dms_max_paired_value: float,
         rnastructure_deltag_ensemble: bool,
         rnastructure_probability: bool,
         verbose: bool):
     """Run the aggregate module.
 
     """
+    
+    check_rnastructure_exists(rnastructure_path)
 
     # Extract the arguments
     if library != '':
         library = check_library(pd.read_csv(library), fasta, out_dir) if library is not None else None
     else:
         library = None
     if samples != '':
```

### Comparing `dreem-0.1.6/dreem/aggregate/mutation_count.py` & `dreem-0.1.8/dreem/aggregate/mutation_count.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/align/fq2bam.py` & `dreem-0.1.8/dreem/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/align/fqs.py` & `dreem-0.1.8/dreem/align/fqs.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/align/main.py` & `dreem-0.1.8/dreem/align/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from logging import getLogger
 import pathlib
 
 from click import command
 
 from .fq2bam import get_bam_files
 from .fqs import FastqUnit
 from ..util import docdef
@@ -21,17 +22,23 @@
                         opt_cut_nextseq,
                         opt_bt2_local, opt_bt2_unal,
                         opt_bt2_discordant, opt_bt2_mixed,
                         opt_bt2_dovetail, opt_bt2_contain,
                         opt_bt2_i, opt_bt2_x, opt_bt2_score_min,
                         opt_bt2_s, opt_bt2_l, opt_bt2_d, opt_bt2_r,
                         opt_bt2_gbar, opt_bt2_dpad, opt_bt2_orient)
+
 from ..util.parallel import lock_output
 
 
+logger = getLogger(__name__)
+
+from ..util.dependencies import check_bowtie2_exists, check_cutadapt_exists, check_fastqc_exists, check_samtools_exists
+
+
 # Parameters for command line interface
 params = [
     # Inputs
     opt_fasta,
     opt_fastqs,
     opt_fastqi,
     opt_fastq1,
@@ -142,24 +149,33 @@
         bt2_x: int,
         bt2_gbar: int,
         bt2_l: int,
         bt2_s: str,
         bt2_d: int,
         bt2_r: int,
         bt2_dpad: int,
-        bt2_orient: str):
+        bt2_orient: str) -> tuple[str, ...]:
     """
     Run the alignment module.
 
     Align the reads to the set of reference sequences and output one BAM file
     for each sample aligned to each reference in the directory 'output'.
     Temporary intermediary files are written in the directory 'temp' and then
     deleted after they are no longer needed.
     """
 
+    check_bowtie2_exists()
+    check_cutadapt_exists()
+    check_fastqc_exists()
+    check_samtools_exists()
+    
+    if not fasta:
+        logger.critical("No FASTA file was given to alignment")
+        return ()
+
     # FASTQ files of read sequences may come from up to seven different
     # sources (i.e. each argument beginning with "fq_unit"). This step
     # collects all of them into one list (fq_units) and also bundles
     # together pairs of FASTQ files containing mate 1 and mate 2 reads.
     fq_units = list(FastqUnit.from_strs(fastqs=fastqs,
                                         fastqi=fastqi,
                                         fastq1=fastq1,
```

### Comparing `dreem-0.1.6/dreem/align/xams.py` & `dreem-0.1.8/dreem/align/xams.py`

 * *Files 25% similar despite different names*

```diff
@@ -88,79 +88,121 @@
     min_fields = 11
     max_flag = 4095  # 2^12 - 1
 
     def get_score(line: bytes, ptn: re.Pattern[bytes]):
         return (float(match.groups()[0])
                 if (match := ptn.search(line)) else None)
 
-    def is_best_alignment(line: bytes):
+    def is_best_align(line: bytes):
         return ((score_x := get_score(line, pattern_x)) is None
                 or score_x < get_score(line, pattern_a))
 
     def read_is_paired(line: bytes):
         info = line.split()
         if len(info) < min_fields:
             raise ValueError(f"Invalid SAM line:\n{line.decode()}")
         flag = int(info[1])
         if flag < 0 or flag > max_flag:
             raise ValueError(f"Invalid SAM flag: {flag}")
         return bool(flag % 2)
 
-    def write_summary(n_copy: int, n_skip: int, paired: bool):
-        n_total = n_copy + n_skip
-        f_copy = round(100 * n_copy / n_total, 3) if n_total else float('nan')
-        endedness_ = "paired" if paired else "single"
+    def write_summary_single(written: int, skipped: int):
+        total = written + skipped
+        f_written = (round(100 * written / total, 3) if total
+                     else float('nan'))
         return (f"Summary of removing multiply-mapped reads from {sam_inp}\n"
-                f"Count of all reads ({endedness_}-end): {n_total}\n"
-                f"Uniquely-mapped reads (written): {n_copy}\n"
-                f"Multiply-mapped reads (removed): {n_skip}\n"
-                f"Percent uniquely mapped: {f_copy} %")
+                f"Total number of single-end reads: {total}\n"
+                f"Uniquely-mapped reads (written):  {written}\n"
+                f"Multiply-mapped reads (skipped):  {skipped}\n"
+                f"Percent uniquely mapped (written): {f_written} %")
+
+    def write_summary_paired(pairs_written: int, pairs_skipped: int,
+                             mates_written: int, mates_skipped: int):
+        mates = mates_written + mates_skipped
+        pairs = pairs_written + pairs_skipped
+        pairs_one_mate = 2 * pairs - mates
+        pairs_both_mates = pairs - pairs_one_mate
+        f_written = (round(100 * pairs_written / pairs, 3) if pairs
+                     else float('nan'))
+        return (f"Summary of removing multiply-mapped reads from {sam_inp}\n"
+                f"Total number of mates aligning: {mates}\n"
+                f"Total number of pairs of mates: {pairs}\n"
+                f"Pairs with both mates aligning: {pairs_both_mates}"
+                f"Pairs with a mate not aligning: {pairs_one_mate}"
+                f"Uniquely-mapped pairs (written):  {pairs_written}\n"
+                f"Multiply-mapped pairs (skipped):  {pairs_skipped}\n"
+                f"Percent uniquely mapped (written): {f_written} %")
 
     def iter_single(sam: BinaryIO, line: bytes):
         """ For each read, yield the best-scoring alignment, excluding
         reads that aligned equally well to multiple locations. """
         n_copy = 0
         n_skip = 0
         while line:
-            if is_best_alignment(line):
+            if is_best_align(line):
                 n_copy += 1
                 yield line
             else:
                 n_skip += 1
             line = sam.readline()
-        logger.debug(write_summary(n_copy, n_skip, paired=False))
+        logger.debug(write_summary_single(n_copy, n_skip))
 
     def iter_paired(sam: BinaryIO, line1: bytes):
         """ For each pair of reads, yield the pair of alignments for
         which both the forward alignment and the reverse alignment in
         the pair scored best among all alignments for the forward and
         reverse reads, respectively. Exclude pairs for which the forward
         and/or reverse read aligned equally well to multiple locations,
         or for which the best alignments for the forward and reverse
         reads individually are not part of the same alignment pair. """
-        n_copy = 0
-        n_skip = 0
+        n_pairs_written = 0
+        n_pairs_skipped = 0
+        n_mates_written = 0
+        n_mates_skipped = 0
         while line1:
-            if not (line2 := sam.readline()):
-                logger.critical(f"SAM file {sam_inp} is paired-end but has a "
-                                f"mate 1 with no mate 2: '{line1.decode()}'")
+            if SAM_DELIMITER not in line1:
+                # If the line is blank, skip it.
+                line1 = sam.readline()
                 continue
-            if ((name1 := line1.split(SAM_DELIMITER, 1)[0])
-                    != (name2 := line2.split(SAM_DELIMITER, 1)[0])):
-                logger.error(f"SAM file {sam_inp} has a mate 1 ({name1}) and "
-                             f"mate 2 ({name2}) with different names")
-                continue
-            if is_best_alignment(line1) and is_best_alignment(line2):
-                n_copy += 1
+            # Check if there is at least one more line in the file.
+            if (line2 := sam.readline()) and SAM_DELIMITER in line2:
+                # Check if the reads on lines 1 and 2 are mates.
+                if (line1.split(SAM_DELIMITER, 1)[0]
+                        == line2.split(SAM_DELIMITER, 1)[0]):
+                    # If they are mates of each other, check if the
+                    # lines represent the best alignment for both.
+                    if is_best_align(line1) and is_best_align(line2):
+                        # If so, then yield both mates.
+                        n_pairs_written += 1
+                        n_mates_written += 2
+                        yield line1
+                        yield line2
+                    else:
+                        # Otherwise, skip both mates.
+                        n_pairs_skipped += 1
+                        n_mates_skipped += 2
+                    # Read the next line from the file.
+                    line1 = sam.readline()
+                    continue
+            # If line2 does not have the mate of line1, then check only
+            # line1 now and consider line2 on the next iteration.
+            if is_best_align(line1):
+                # Yield only line1.
+                n_pairs_written += 1
+                n_mates_written += 1
                 yield line1
-                yield line2
             else:
-                n_skip += 1
-            line1 = sam.readline()
-        logger.debug(write_summary(n_copy, n_skip, paired=True))
+                # Skip line1.
+                n_pairs_skipped += 1
+                n_mates_skipped += 1
+            # Since line2 was not used yet, consider it on the next
+            # iteration instead of reading another line from the file.
+            line1 = line2
+        logger.debug(write_summary_paired(n_pairs_written, n_pairs_skipped,
+                                          n_mates_written, n_mates_skipped))
 
     # Make the output directory.
     sam_out.parent.mkdir(parents=True, exist_ok=True)
     logger.debug(f"Ensuring directory: {sam_out.parent}")
 
     # Deduplicate the alignments.
     with (open(sam_inp, "rb") as sami, open(sam_out, "xb") as samo):
```

### Comparing `dreem-0.1.6/dreem/cluster/EMclustering.py` & `dreem-0.1.8/dreem/cluster/EMclustering.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/cluster/bitvector.py` & `dreem-0.1.8/dreem/cluster/bitvector.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.read_hist = preprocessing[4]
         self.read_names = preprocessing[5]
         self.report = preprocessing[6]
         self.base_to_keep = preprocessing[7]
         self.publish_preprocessing_report(path=path[:-len('.json')]+'_preprocessing_report.txt')
         
     #TODO optimize this 
-    def preprocessing(self, path, signal_thresh = 0.005, include_gu = False, min_reads=1000, include_del=False, max_mut_close_by = 4):
+    def preprocessing(self, path, signal_thresh = 0.005, include_gu = False, min_reads=1000, include_del=False, min_mut_dist = 4):
         """Preprocess the bitvector.
         
         - Remove the bases G and U
         - Count and remove duplicates
         - Remove the bases with a Mutation fraction below signal_thresh
         - save the read names and the read count
         
@@ -68,98 +68,86 @@
             Report of the preprocessing.
             #TODO define
             
         """
         report = {}
 
         reader = VectorReader.load(path)
-        bv = reader.get_all_vectors()
-        bv.columns = reader.columns
+        bv = reader.get_all_vectors(numeric=True)
 
-        report['total_number_of_reads'] = bv.shape[0]     
-        
-        # Take the read names
-        read_names = np.array(bv.index.tolist(), dtype = str)
+        report['total_number_of_reads'] = bv.shape[0]
         
         ## PER BASE REMOVALS
         # Remove the non-informative bases types
         sequence = reader.seq.decode()
         report['sequence'] = sequence
         
         # Remove the G and U bases
         temp_n_cols = bv.shape[1]
         bases_to_drop = []
         if not include_gu:
-            bases_to_drop = [c for c in bv.columns if c[0] in ['G','T']]
-            bv = bv.drop(columns=bases_to_drop)
+            bases_to_drop = [pos for pos, base in zip(bv.columns,
+                                                      reader.seq,
+                                                      strict=True)
+                             if base != A_INT and base != C_INT]
+            bv.drop(columns=bases_to_drop, inplace=True)
         report['removed_G_U'] = len(bases_to_drop)
 
-        # Remove the low-mutation-rate bases
-        bin_bv = mutations_bin_arr(bv)
-        sub_rate = np.sum(bin_bv, axis = 0)/bin_bv.shape[0]
-        bases_to_drop = [unpaired for unpaired, mut_rate in zip(bv.columns, sub_rate) if mut_rate < signal_thresh]
-        bases_to_keep = set(bv.columns)-set(bases_to_drop)
-        bases_to_keep = [int(i[1:]) for i in bases_to_keep]; bases_to_keep.sort()
-
-        temp_n_cols = bv.shape[1]
-        bv = bv.drop(columns=bases_to_drop)
-        report['too_low_mutation_rate'] = temp_n_cols - bv.shape[1]
-        report['min_mutation_rate'] = signal_thresh
-
-
         ## PER READ REMOVALS
-        # Remove the bit mut_vectors with too many mutations
+        # Remove the bit vectors with too many mutations
         temp_n_reads = bv.shape[0]
-        bin_bv = mutations_bin_arr(bv)
-        n_muts_per_reads = np.sum(bin_bv, axis = 1)
-        idx = np.nonzero( n_muts_per_reads < np.mean(n_muts_per_reads) + 3*np.std(n_muts_per_reads) )[0]
-        bv, read_names = bv.take(idx), read_names[idx]
+        n_muts_per_read = reader.query_vectors(bv, SUB_N | INDEL, subsets=True).sum(axis=1)
+        n_muts_per_read_limit = n_muts_per_read.mean() + 3 * n_muts_per_read.std()
+        bv.drop(index=bv.index[n_muts_per_read > n_muts_per_read_limit], inplace=True)
         report['too_many_mutations'] = temp_n_reads - bv.shape[0]
         
-        # Remove the bitvectors with deletions
-        if not include_del:
-            temp_n_reads = bv.shape[0]
-            dels = deletions_bin_array(bv)
-            no_deletion_in_the_read = np.nonzero(~np.sum(dels, axis=1, dtype=bool))[0]
-            bv, read_names = bv.take(no_deletion_in_the_read), read_names[no_deletion_in_the_read]
-            report['no_info_around_mutations'] = temp_n_reads - bv.shape[0]
+        # Remove the low-mutation-rate bases
+        match_count = (reader.query_vectors(bv, MATCH).sum(axis=0) +
+                       reader.query_vectors(bv, MATCH | INS_5).sum(axis=0))
+        mut_query = SUB_N | INDEL if include_del else SUB_N
+        mut_count = reader.query_vectors(bv, mut_query, subsets=True).sum(axis=0)
+        mut_rate = mut_count / (match_count + mut_count)
+        temp_n_cols = bv.shape[1]
+        bv.drop(columns=bv.columns[mut_rate < signal_thresh], inplace=True)
+        report['too_low_mutation_rate'] = temp_n_cols - bv.shape[1]
+        report['min_mutation_rate'] = signal_thresh
 
         # MAKE BV BINARY
-        for i, c in enumerate(bv.columns):
-            bv[c] = mutations_bin_arr(bv[c])
+        mut_query = SUB_N | INDEL if include_del else SUB_N
+        bv = reader.query_vectors(bv, mut_query, subsets=True)
 
-        #Remove the bit mut_vectors with 'max_mut_close_by' consecutive mutations
-        idx_remove_consecutive_mutations = []
-        for i0, c0 in enumerate(bv.columns[:-1]):
-            for c1 in bv.columns[i0+1:i0+max_mut_close_by+1]:
-                if int(c1[1:]) - int(c0[1:]) <= max_mut_close_by:
-                    idx_remove_consecutive_mutations += np.nonzero(np.logical_and(bv[c0], bv[c1]).values)[0].tolist()
-        mask = np.ones(bv.shape[0], dtype=bool)
-        mask[idx_remove_consecutive_mutations] = False
+        # Remove the bit mut_vectors with 'max_mut_close_by' consecutive mutations
+        muts_too_close = pd.Series(np.zeros(bv.shape[0], dtype=bool),
+                                   index=bv.index)
+        for pos5 in bv.columns:
+            pos3 = pos5 + min_mut_dist - 1
+            muts_too_close |= bv.loc[:, pos5: pos3].sum(axis=1) > 1
         temp_n_reads = bv.shape[0]
-        bv, read_names = bv.take(np.arange(bv.shape[0])[mask]), read_names[mask]
-        report['mutations_close_by'] = temp_n_reads - bv.shape[0] 
+        bv.drop(index=muts_too_close[muts_too_close].index, inplace=True)
+        report['mutations_close_by'] = temp_n_reads - bv.shape[0]
 
         # Turn bv into a np array
-        bv = np.array(bv, dtype = np.uint8)    
+        bases_to_keep = bv.columns - reader.end5  # convert to 0 indexing
+        read_names = bv.index.to_list()
+        bv = np.array(bv, dtype = np.uint8)
         
         # What's this #TODO
         report['too_few_informative_bits'] = '#TODO'
         
         # Remove the duplicates and count the reads
         bv, read_idx, read_inverse, read_hist = np.unique(bv, axis = 0, return_index=True, return_inverse=True, return_counts = True)
         report['number_of_unique_reads'] = read_hist.shape[0]
         report['number_of_used_reads'] = np.sum(read_hist)
         report['bases_used'] = bv.shape[1]
         
         
         # Sanity check
         assert report['number_of_used_reads'] >= min_reads, "Too few reads after preprocessing"
         assert len(report['sequence']) == report['bases_used'] + report['too_low_mutation_rate'] + report['removed_G_U']
-        assert report['total_number_of_reads'] == report['number_of_used_reads'] + report['too_many_mutations'] + report['no_info_around_mutations'] + report['mutations_close_by']
+        assert report['total_number_of_reads'] == report['number_of_used_reads'] + report['too_many_mutations'] + report['mutations_close_by']
         return sequence, bv, read_idx, read_inverse, read_hist, read_names, report, bases_to_keep
     
 
    
    
     def publish_preprocessing_report(self, path):
         """Publish the report in a text file.
@@ -179,16 +167,16 @@
         + "\nResidues removed because they have Mutation fraction below {} : {}".format(self.report['min_mutation_rate'], self.report['too_low_mutation_rate']) \
         + "\nNumber of bit mut_vectors in total: "+ str(self.report['total_number_of_reads'])\
         + "\nNumber of bit mut_vectors used: "+ str(self.report['number_of_used_reads']) \
         + "\nNumber of unique bit mut_vectors used: " + str(self.report['number_of_unique_reads']) \
         + "\nNumber of bit mut_vectors discarded: "+ str(self.report['total_number_of_reads'] - self.report['number_of_used_reads']) \
         + "\nBit mut_vectors removed because of too many mutations: " + str(self.report['too_many_mutations']) \
         + "\nBit mut_vectors removed because of too few informative bits: " + str(self.report['too_few_informative_bits']) \
-        + "\nBit mut_vectors removed because of mutations close by: " + str(self.report['mutations_close_by']) \
-        + "\nBit mut_vectors removed because of no info around mutations:  " + str(self.report['no_info_around_mutations'])
+        + "\nBit mut_vectors removed because of mutations close by: " + str(self.report['mutations_close_by'])
+        #+ "\nBit mut_vectors removed because of no info around mutations:  " + str(self.report['no_info_around_mutations']
         
         with open(path, 'w') as f:
             print(report)
             f.write(report)
            
            
     def associate_reads_with_likelihoods(self, likelihood_per_read):
@@ -206,15 +194,15 @@
 
         reads: dict
             Dictionary associating the read name with the likelihood.
 
         """
 
         reads = {}
-        for name, idx in zip(self.read_names, self.read_inverse):
+        for name, idx in zip(self.read_names, self.read_inverse, strict=True):
             reads[name] = {}
             for k in range(likelihood_per_read.shape[1]):
                 reads[name]['K'+str(k+1)] = likelihood_per_read[idx,k]
 
         return reads
```

### Comparing `dreem-0.1.6/dreem/cluster/clusteringAnalysis.py` & `dreem-0.1.8/dreem/cluster/clusteringAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,21 @@
             - log_likelihood: float
                 Log-likelihood of the model.
         '''
 
         # global dT # !! For test_input !!
         em = EMclustering(self.bitvector.bv, 1, self.bitvector.read_hist, self.bitvector.base_to_keep, self.bitvector.sequence,
                                 **self.clustering_args)
-        results = {'K1': [em.run()] }
-        for k in range(2,self.K_max+1):
+        results = {1: [em.run()]}
+        for k in range(2, self.K_max + 1):
             em = EMclustering(self.bitvector.bv, k, self.bitvector.read_hist, self.bitvector.base_to_keep, self.bitvector.sequence,
                                 **self.clustering_args)
 
             pool = multiprocessing.Pool(processes=self.clustering_args["max_procs"])
-            results['K'+str(k)] = sorted(pool.starmap(em.run, [() for _ in range(self.num_runs)]), key=lambda res: res['log_likelihood'], reverse=True)
+            results[k] = sorted(pool.starmap(em.run, [() for _ in range(self.num_runs)]), key=lambda res: res['log_likelihood'], reverse=True)
             pool.close()
             pool.join()
         
         return results
         
 
 if __name__ == '__main__':
```

### Comparing `dreem-0.1.6/dreem/cluster/main.py` & `dreem-0.1.8/dreem/cluster/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import json
-import os
 from click import command
+import pandas as pd
 
 from ..cluster.bitvector import BitVector
 from ..cluster.clusteringAnalysis import ClusteringAnalysis
 from ..cluster.EMclustering import EMclustering
 from ..util.cli import (opt_report, opt_out_dir,
                         opt_max_procs,
                         opt_max_clusters, opt_num_runs, opt_signal_thresh,
                         opt_include_gu, opt_include_del, opt_polya_max,
                         opt_min_iter, opt_max_iter, opt_convergence_cutoff, opt_min_reads, opt_verbose)
 
 from ..util import docdef, path
 
 
 params = [
-    opt_verbose,
     # Input/output directories
     opt_report,
     opt_out_dir,
     # Parallelization
     opt_max_procs,
     # Clustering options
     opt_max_clusters,
@@ -55,16 +53,15 @@
         max_iter: int,
         convergence_cutoff: float,
         min_reads: int):
     """
     Run the clustering module. 
     """
 
-    # Create the output file
-    best_clusters_samples = {}
+    cluster_out_files = list()
 
     # Create a clustering args 
     clustering_args = dict(
         max_clusters=max_clusters,
         min_iter=min_iter,
         max_iter=max_iter,
         signal_thresh=signal_thresh,
@@ -73,35 +70,36 @@
         min_reads=min_reads,
         convergence_cutoff=convergence_cutoff,
         num_runs=num_runs,
         max_procs=max_procs
     )
 
     # Get the bitvector files in the input directory and all of its subdirectories
-    for i, report_file in enumerate(mp_report):
+    for report_file in mp_report:
         report_path = path.MutVectorReportFilePath.parse(report_file)
-        sample = report_path.sample
-        ref = report_path.ref
-        end5 = report_path.end5
-        end3 = report_path.end3
 
         # Run the clustering algorithm
         bitvector = BitVector(path=report_file, signal_thresh=signal_thresh, include_gu=include_gu, min_reads=min_reads,
                               include_del=include_del)
         ca = ClusteringAnalysis(bitvector, max_clusters, num_runs, clustering_args)
         clusters = ca.run()
 
         # Compute the likelihood of each read for each cluster
-        reads_best_cluster = {}
-        for k in clusters:
-            em = EMclustering(bitvector.bv, int(k[1]), bitvector.read_hist, bitvector.base_to_keep, bitvector.sequence,
+        columns = [(k, c + 1) for k in clusters for c in range(k)]
+        reads_best_cluster = pd.DataFrame(dtype=float,
+                                          index=pd.Index(bitvector.read_names, name="Read Name"),
+                                          columns=pd.MultiIndex.from_tuples(columns,
+                                                                            names=["K", "i"]))
+        for k, clusters_k in clusters.items():
+            em = EMclustering(bitvector.bv, k, bitvector.read_hist, bitvector.base_to_keep, bitvector.sequence,
                               **clustering_args)
-            likelihood_reads_best_cluster, _, _ = em.expectation(clusters[k][0]['mu'], clusters[k][0]['pi'])
-            reads_best_cluster[k] = bitvector.associate_reads_with_likelihoods(likelihood_reads_best_cluster)
+            likelihood_reads_best_cluster, _, _ = em.expectation(clusters_k[0]['mu'], clusters_k[0]['pi'])
+            for c in range(k):
+                reads_best_cluster.loc[:, (k, c + 1)] = likelihood_reads_best_cluster[bitvector.read_inverse, c]
+
+        # Save the results
+        cluster_out_file = str(report_path.path.with_name("clusters.csv.gz"))
+        reads_best_cluster.to_csv(cluster_out_file, header=True, index=True,
+                                  compression="gzip")
+        cluster_out_files.append(cluster_out_file)
 
-        best_clusters_samples[sample, ref, end5, end3] = reads_best_cluster
-
-    # Save the results
-    with open(os.path.join(out_dir, 'best_cluster_reads.json'), 'w') as f:
-        json.dump(best_clusters_samples, f, indent=4)
-
-    return os.path.join(out_dir, 'best_cluster_reads.json')
+    return cluster_out_files
```

### Comparing `dreem-0.1.6/dreem/demultiplex/demultiplex.py` & `dreem-0.1.8/dreem/demultiplex/demultiplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,38 +354,46 @@
 
             organized_joint_dict[k]=temp_dictionary_pickle_loc
         
         #union_dict.clear()
         """
         now that the reads are organized we have to open each pickle file write fastqs 
         """
-        fqs=[]
+        #fqs=[]
+        for k in sequence_objects.keys():
+            
+            if(len(union_dict[k])>1):
+                fq=sample_fq_dir+k+"_R"+str(fastq_id)+".fastq"
+                fq_buff=open(fq,"wt")
+                fq_buff.close()
 
         for x in range(len(self.pickle_file_list)):
 
             p_file_object=open(self.pickle_file_list[x],"rb")
             pickled_fastq_dict=pickle.load(p_file_object)
             p_file_object.close()
             
             for k in organized_joint_dict.keys():
 
-                #print("writing filtered fastqs"+str(k))
-                fq=sample_fq_dir+k+"_R"+str(fastq_id)+".fastq"
-                fqs.append(fq)
+                if(len(union_dict[k])>1):
 
-                sequence_objects[k].fastqs[fastq_id]=fq
+                    #print("writing filtered fastqs"+str(k))
+                    fq=sample_fq_dir+k+"_R"+str(fastq_id)+".fastq"
+                    #fqs.append(fq)
 
-                specific_reads= organized_joint_dict[k][x]
+                    sequence_objects[k].fastqs[fastq_id]=fq
 
-                fq_buff=open(fq,"a") if x!=0 else open(fq,"wt") 
+                    specific_reads= organized_joint_dict[k][x]
 
-                for r in specific_reads:
-                    lines=pickled_fastq_dict[r]
-                    fq_buff.writelines(lines)
-                fq_buff.close()
+                    fq_buff=open(fq,"a")
+
+                    for r in specific_reads:
+                        lines=pickled_fastq_dict[r]
+                        fq_buff.writelines(lines)
+                    fq_buff.close()
         #fqs.sort()
     """
     this methods removes the pickles that contain split fastq information
     """
     def destroy_temp_data(self):
         for x in range(len(self.pickle_file_list)):
             os.remove(self.pickle_file_list[x])
@@ -740,15 +748,15 @@
         return False
 
 def check_all_done(seq_objects:dict()):
     return_dict={}
 
     
     for k in seq_objects.keys():
-
+        print("checking: "+k,end="\r")
         if not (check_done(seq_objects[k].workspace)):
             
             print("check done not done! ",check_done(seq_objects[k].workspace))
             return_dict[k]=seq_objects[k]
     return return_dict
 
 def grep_both_fastq(sequence_object:Sequence_Obj,clipped:int,rev_clipped:int,index_tolerence:int,delete_fastqs:bool,mismatches_allowed:int):
@@ -809,18 +817,19 @@
         itr_val+=1
     
     print("checking")
     not_done_dict=check_all_done(sequence_objects)
     #print(not_done_list)
 
     while len(not_done_dict) > 0 and itr_val >4:
+        print("rip")
         itr_val=iteration
         #itr_val=iteration
         #not_done_dict=check_all_done(sequence_objects)
-        parallel_grepping(sequence_objects=not_done_dict,fwd_clips=0,rev_clips=0,index_tolerence=0,delete_fastq=False,iteration=itr_val+1,mismatches=mismatches)
+        parallel_grepping(sequence_objects=not_done_dict,fwd_clips=fwd_clips,rev_clips=rev_clips,index_tolerence=index_tolerence,delete_fastq=delete_fastq,iteration=itr_val+1,mismatches=mismatches)
     if(itr_val>4):
         print("could not finish some of the reads: ",list(not_done_dict.keys()))
     
         #warning could not finish one of the reads
     return not_done_dict    
 
 def regular_grepping(sequence_objects:dict,fwd_clips:int,rev_clips:int,index_tolerence:int,delete_fastq:bool,paired:bool=True,mismatches:int=0,iteration:int=0,overwrite:bool=False):
@@ -984,28 +993,31 @@
                 dict_of_lists[fq+"_"+data_key].append(len(fq_read_data[data_key]))
     df=pd.DataFrame()
 
     for k in dict_of_lists.keys():
         df[k]=dict_of_lists[k]
     print("len: mixed: ",len(mixed_total_dict[FQS[0]]))
     print("len: mixed: ",len(mixed_total_dict[FQS[0]])," / ",orginal_len[FQS[0]]," = ",len(mixed_total_dict[FQS[0]])/orginal_len[FQS[0]])
+    len_col=[" "]*len(sequence_objects.keys())
+    len_col[0]=len(mixed_total_dict[FQS[0]])
     df["percent_reads_used"]=[(1-(len(mixed_total_dict[FQS[0]])/orginal_len[FQS[0]]))*100]*len(sequence_objects.keys())
+    df["total_read_count"]=len_col
 
     print(working_directory+"demultiplex_info.csv")
     df.to_csv(working_directory+"demultiplex_info.csv",index=False)
 
 
 
 """
 split is default to 10. disregarding extremes, the higher the split the lighter the memeory load
 library csv 
     each construct must have a secondary signiture start index and len in order to process, 
     barcode given in main arguements 
 """
-def demultiplex_run(library_csv,demulti_workspace,mixed_fastq1,mixed_fastq2,fasta,barcode_start=0,barcode_length=0,split:int=10,clipped:int=0,rev_clipped:int=0,index_tolerance:int=0,parallel:bool=False,mismatch_tolerence:int=0,overwrite:bool=False):
+def demultiplex_run(library_csv,demulti_workspace,report_folder,mixed_fastq1,mixed_fastq2,fasta,barcode_start=0,barcode_length=0,split:int=10,clipped:int=0,rev_clipped:int=0,index_tolerance:int=0,parallel:bool=False,mismatch_tolerence:int=0,overwrite:bool=False):
 
     if(type(mixed_fastq1)==type(("x","x"))):
         mixed_fastq1=mixed_fastq1[0]
         mixed_fastq2=mixed_fastq2[0]
     sample_name=mixed_fastq1.split("_R1")[0].split("/")[-1]
 
     """
@@ -1084,21 +1096,22 @@
     #multigrepped_read_analysis()
 
     """
     organizes reads for writing
     uses super_fastq object to write fastqs in efficent way
     """
 
-    fq1_paths=super_fq1.super_write_fastqs(unioned_sets_dictionary,temp_ws,1,sequence_objects,sample_name=sample_name)
+    fq1_paths=super_fq1.super_write_fastqs(unioned_sets_dictionary,report_folder,1,sequence_objects,sample_name=sample_name)
     #super_fq1.destroy_temp_data()
 
-    fq2_paths=super_fq2.super_write_fastqs(unioned_sets_dictionary,temp_ws,2,sequence_objects,sample_name=sample_name)
+    fq2_paths=super_fq2.super_write_fastqs(unioned_sets_dictionary,report_folder,2,sequence_objects,sample_name=sample_name)
     #super_fq2.destroy_temp_data()
 
     """
     makes report on what amount of reads were found in which stage
     """
     #sequence_objects:dict,fq1:str,fq2:str,working_directory:str,unioned_sets:dict)
     print("creating report!!!")
-    create_report(sequence_objects,mixed_fastq1,mixed_fastq2,temp_ws,unioned_sets_dictionary)
+    create_report(sequence_objects,mixed_fastq1,mixed_fastq2,report_folder,unioned_sets_dictionary)
+
 
-    return (),(),(temp_ws+sample_name+"/",)
+    return (),(),(report_folder+sample_name+"/",)
```

### Comparing `dreem-0.1.6/dreem/demultiplex/main.py` & `dreem-0.1.8/dreem/demultiplex/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from click import command
 
 from ..demultiplex.demultiplex import demultiplex_run
 from ..util.cli import (
     opt_barcode_length, opt_barcode_start, opt_parallel_demultiplexing, opt_clipped_demultiplexing,
-    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_library, opt_fastq1, opt_fastq2,opt_out_dir)
+    opt_mismatch_tolerence, opt_index_tolerence, opt_demulti_overwrite, opt_fasta, opt_library, opt_fastq1, opt_fastq2,opt_out_dir,opt_temp_dir)
 
 params = [
     # Inputs
     opt_fasta,
     opt_fastq1,
     opt_fastq2,
     opt_library,
     opt_barcode_start,
     opt_barcode_length,
     opt_out_dir,
+    opt_temp_dir,
 
     # options
     opt_parallel_demultiplexing,
     opt_clipped_demultiplexing,
     opt_mismatch_tolerence,
     opt_index_tolerence,
-    opt_demulti_overwrite
+    opt_demulti_overwrite,
+
 
 ]
 
 
 # Turn into DREEM command.
 
 @command("demultiplex", params=params)
 def cli(**kwargs):
     return run(**kwargs)
 
 
-def run(library: str, out_dir: str, fastq1: str, fastq2: str, fasta: str, barcode_start=0,
+def run(library: str, out_dir: str, temp_dir:str, fastq1: str, fastq2: str, fasta: str, barcode_start=0,
         barcode_length=0, clipped: int = 0, index_tolerance: int = 0, parallel_demultiplexing: bool = False,
         mismatch_tolerence: int = 0, demulti_overwrite: bool = False):
+    
     return demultiplex_run(library_csv=library,
                            overwrite=demulti_overwrite,
-                           demulti_workspace=out_dir,
+                           demulti_workspace=temp_dir,
+                           report_folder=out_dir,
                            mixed_fastq1=fastq1,
                            mixed_fastq2=fastq2,
                            barcode_start=barcode_start,
                            barcode_length=barcode_length,
                            clipped=clipped,
                            index_tolerance=index_tolerance,
                            parallel=parallel_demultiplexing,
```

### Comparing `dreem-0.1.6/dreem/draw/main.py` & `dreem-0.1.8/dreem/draw/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 
 import pandas as pd
 from click import command
 
 from ..util import docdef
-from ..util.cli import (opt_out_dir, opt_draw_input, opt_library,
-                        opt_flat, opt_coords,
+from ..util.cli import (opt_out_dir, opt_draw_input,
+                        opt_flat, opt_coords,opt_section, 
                         opt_mutation_fraction, opt_mutation_fraction_identity,
                         opt_base_coverage, opt_mutations_in_barcodes,
                         opt_mutations_per_read_per_sample,  
                         )
 from ..util.dump import *
 from .study import Study
-from ..aggregate.library_samples import get_library_info
+from logging import getLogger; logger = getLogger(__name__)
 
 params = [
     opt_draw_input,
     opt_out_dir,
-    opt_library,
     opt_flat,
     opt_coords,
+    opt_section,
     opt_mutation_fraction,
     opt_mutation_fraction_identity,
     opt_base_coverage,
     opt_mutations_in_barcodes,
     opt_mutations_per_read_per_sample,
 ]
 
@@ -33,131 +33,133 @@
     return run(**kwargs)
 
 
 @docdef.auto()
 def run( 
         inpt: tuple[str], 
         *,
-        library: str,
         flat: list,
         out_dir: str,
         coords: tuple,
+        section: str,
         mutation_fraction: bool,
         mutation_fraction_identity:bool,
         base_coverage: bool,
         mutations_in_barcodes: bool,
         mutation_per_read_per_reference: bool,
         ):
     """Run the draw command.
 
     """
 
-
+    if type(inpt) == str:
+        inpt = (inpt,)
+    if type(inpt[0]) == str:
+        data = [json.loads(open(i).read()) for i in inpt]  
+        logger.info('Loaded {} input files'.format(len(data)))
+    else:
+        data = inpt
+    
     study = Study(
-        data = inpt,
+        data = data,
     )
     
     # Check output directory.
     out_dir = os.path.join(out_dir, 'draw')
     if not os.path.isdir(out_dir):
         os.makedirs(out_dir)
+        logger.info('Created output directory: {}'.format(out_dir))
  
     for sample in study.get_samples():
+        logger.info('Drawing sample: {}'.format(sample))
             
         path = os.path.join(out_dir, sample)
         if not os.path.isdir(path):
             os.makedirs(path)
+            logger.info('Created output directory: {}'.format(path))
+
+        refs, section, base_index = select_coords(coords, sample, study, section)
         
-        refs, starts, ends = select_coords(coords, sample, study)
-        
-        for ref, start, end in zip(refs, starts, ends):
-                        
-            section_name = str(start) + '-' + str(end)
-            
-            if library != '':
-                _, section_tranlation = get_library_info(pd.read_csv(library), ref)
-                if section_name in section_tranlation:
-                    section_name = section_tranlation[section_name]
-            
+        all_plots = {'mutation_fraction': mutation_fraction, 'mutation_fraction_identity': mutation_fraction_identity, 'base_coverage': base_coverage, 'mutations_in_barcodes': mutations_in_barcodes, 'mutation_per_read_per_reference': mutation_per_read_per_reference}
+        logger.info('Drawing {} references - section pairs'.format(len(refs)) +'\n\t'+ '\n\t'.join(['{} - {}'.format(ref, section) for ref, section in zip(refs, section)])\
+                    + '\n' + 'plot types: \n\t' + '\n\t'.join([k for k, v in all_plots.items() if v])\
+            )
+
+        for ref, section, base_index in zip(refs, section, base_index):
+                                
             if flat:
-                prefix = os.path.join(path, '__'.join([ref, section_name,'']))
+                prefix = os.path.join(path, '__'.join([ref, section,'']))
             else:
-                prefix = os.path.join(path, ref, section_name , '')
+                prefix = os.path.join(path, ref, section , '')
                 os.makedirs(prefix, exist_ok=True)
-            
-            section, base_index = find_section_for_these_coords(study, sample, ref, start, end)
-            
+                        
             if mutation_fraction:
                 study.mutation_fraction(
                     sample=sample,
                     reference=ref,
                     section=section,
                     cluster='pop_avg',
-                    base_index = base_index,
+                    #base_index = base_index,
                     to_html = os.path.join(prefix,'mutation_fraction.html') if not flat else prefix + 'mutation_fraction.html',
                 )
             
             if mutation_fraction_identity:
                 study.mutation_fraction_identity(
                     sample=sample,
                     reference=ref,
                     section=section,
                     cluster='pop_avg',
-                    base_index = base_index,
+                    #base_index = base_index,
                     to_html = os.path.join(prefix,'mutation_fraction_identity.html') if not flat else prefix + 'mutation_fraction_identity.html',
                 )
             
             if base_coverage:
                 study.base_coverage(
                     sample=sample,
                     reference=ref,
                     section=section,
                     cluster='pop_avg',
-                    base_index = base_index,
+                    #base_index = base_index,
                     to_html = os.path.join(prefix,'base_coverage.html') if not flat else prefix + 'base_coverage.html',
                 )
                 
             if mutations_in_barcodes:
                 study.mutations_in_barcodes(
                     sample=sample,
                     reference=ref,
                     section=section,
                     cluster='pop_avg',
-                    base_index = base_index,
+                    #base_index = base_index,
                     to_html = os.path.join(prefix, 'mutations_in_barcodes.html') if not flat else prefix + 'mutations_in_barcodes.html',
                 )
                 
             if mutation_per_read_per_reference:
                 study.mutation_per_read_per_reference(
                     sample=sample,
                     reference=ref,
                     section=section,
                     cluster='pop_avg',
-                    base_index = base_index,
+                    #base_index = base_index,
                     to_html = os.path.join(prefix, 'mutation_per_read_per_reference.html') if not flat else prefix + 'mutation_per_read_per_reference.html',
-                )               
+                )             
+                
+        logger.info('Done drawing sample: {}'.format(sample))  
 
 
-def select_coords(coords, sample, study):
+def select_coords(coords, sample, study, section):
     
-    refs, starts, ends = [], [], []
-    
-    if len(coords):
-        for t in coords:
-            refs.append(t[0])
-            starts.append(t[1])
-            ends.append(t[2])
-    else:
-        for _, row in study.df[study.df['sample']==sample].iterrows():
-            refs.append(row['reference'])
-            starts.append(row['section_start'])
-            ends.append(row['section_end'])
+    refs, section_out, base_index = [], [], []
+
+    for t in coords:
+        refs.append(t[0])
+        section_out.append('full')
+        base_index.append(np.arange(t[1], t[2] + 1))
     
-    return refs, starts, ends
-            
-            
-def find_section_for_these_coords(study, sample, ref, start, end):
-    df = study.df[(study.df['sample']==sample)&(study.df['reference']==ref)]
-    for _, row in df.iterrows():
-        if row['section_start'] <= start and row['section_end'] >= end:
-            return row['section'], np.arange(start-row['section_start']+1, end-row['section_start']+2).tolist()
-    raise ValueError(f'No section found for {sample}, {ref}, {start}, {end}. Change your section in your library file or your coordinates.')    
+    for s in section:
+        for ref in study.df[study.df['sample']==sample]['reference'].unique():
+            if s in study.df[(study.df['sample']==sample) & (study.df['reference']==ref)]['section'].unique():
+                refs.append(ref)
+                section_out.append(s)
+                base_index.append(None) 
+
+    return refs, section_out, base_index
+
```

### Comparing `dreem-0.1.6/dreem/draw/manipulator.py` & `dreem-0.1.8/dreem/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/draw/plotter.py` & `dreem-0.1.8/dreem/draw/plotter.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import plotly.graph_objects as go
 from plotly.offline import plot, iplot
 
 from ..draw import  util
 from itertools import cycle
 from typing import Tuple, List
 from sklearn import metrics
-from sklearn.linear_model import LogisticRegression
+from sklearn.linear_model import LogisticRegression, LinearRegression
 from plotly.subplots import make_subplots
 import plotly.express as px
 from dms_ci import dms_ci
 
 
+
 LIST_COLORS = ['red','green','blue','orange','purple','black','yellow','pink','brown','grey','cyan','magenta']
 
 def mutation_fraction(df, show_ci:bool=True)->dict:
     assert len(df) == 1, "df must have only one row"
     mh = df.iloc[0]
     cmap = {"A": "red", "T": "green", "G": "orange", "C": "blue"}  # Color map
     
@@ -383,25 +384,26 @@
 
     return {
         'fig':fig,
         'data':data
         }
     
 def num_aligned_reads_per_reference_frequency_distribution(data):
+    assert len(samples:=data['sample'].unique()) == 1, "data must have 1 sample"
     data = data['num_aligned'].values
     return {
             'fig':go.Figure(
                 go.Histogram(
                     x=data, 
                     showlegend=False, 
                     marker_color='indianred',
                     hovertemplate="Number of aligned reads: %{x}<br>Count: %{y}<extra></extra>"
                     ),
                 layout=go.Layout(
-                    title=go.layout.Title(text='Number of aligned reads per reference frequency'),
+                    title=go.layout.Title(text='{} - Reads per reference count'.format(samples[0])),
                     xaxis=dict(title="Number of aligned reads"),
                     yaxis=dict(title="Count"),
                     plot_bgcolor='white',
                     paper_bgcolor='white'
                     )          
                 ),
             'data':data
@@ -447,7 +449,127 @@
             xaxis=dict(title="Position"),
             yaxis=dict(title="Count")
             )
         )
     fig.update_layout(plot_bgcolor='white',paper_bgcolor='white')
     
     return {'fig':fig, 'data':data}
+
+
+
+def compare_mutation_profiles(data, max_plots = 100, max_axis=None):
+
+    # total number of plots
+    totNumPlots =  int((data.shape[0] *  (1+data.shape[0]))/2)
+    if totNumPlots > max_plots:
+        print('Too many plots: {} rows combined together make {} plots when using these arguments. Filtered dataset is: \n\n{}.'.format(data.shape[0], totNumPlots, data[['sample','reference','section','cluster','sub_rate_x']]))
+        return {'fig': go.Figure(), 'data': data}
+    
+    if data.shape[0] == 0:
+        print('No data found for this combination of arguments')
+        return {'fig': go.Figure(), 'data': data}    
+
+    if data.shape[0] == 1:
+        print('Only one row found for this combination of arguments.')
+        return {'fig': go.Figure(), 'data': data}        
+
+    # Assert sequence is the same for all rows
+    assert data['sequence'].nunique() == 1, 'Sequence is not the same for all rows. Select a subset of the data that has the same sequence.'
+
+    # sort by unique_id
+    data = data.sort_values('unique_id').reset_index(drop=True)
+
+    # plot these
+    fig = go.Figure()
+    
+    makePlotLabel = lambda x, y: '{} vs {}'.format(x, y)
+    
+    traceTrack = []
+    annotationTrack = []
+    
+    for idx1, row1 in data.iloc[:-1].iterrows():
+        for _, row2 in data.iloc[idx1+1:].iterrows():
+            x, y = row1['sub_rate'], row2['sub_rate']
+            xlabel, ylabel = row1['unique_id'], row2['unique_id']
+            plotLabel = makePlotLabel(xlabel, ylabel)
+            
+            # make the plot squared 
+            if max_axis is not None:
+                maxValue = max_axis
+            else:
+                maxValue = max(x.max(), y.max(), 0.14) + 0.01
+            
+            fig.update_xaxes(range=[0, maxValue], constrain='domain')
+            fig.update_yaxes(range=[0, maxValue], constrain='domain')
+            
+            # plot x vs y then the linear regression line, then the 1:1 line, then the R2 and RMSE values
+            fig.add_trace(go.Scatter(x=x, y=y, mode='markers', name='mutation fraction', text=plotLabel, visible=False),)
+            traceTrack.append(plotLabel)
+            
+            # linear regression line
+            model = LinearRegression()
+            model.fit(x.reshape(-1,1), y)
+            slope, intercept, r_value = model.coef_[0], model.intercept_, model.score(x.reshape(-1,1), y)
+            fig.add_trace(go.Scatter(x=x, y=slope*x+intercept, mode='lines', name='linear regression: y = {}x + {}'.format(round(slope,4), round(intercept,4)), visible=False))
+            traceTrack.append(plotLabel)
+            
+            # 1:1 line
+            fig.add_trace(go.Scatter(x=[0, maxValue], y=[0, maxValue], mode='lines', name='1:1 line', visible=False))
+            traceTrack.append(plotLabel)
+            
+            # R2, RMSE and linear regression line
+            annot = 'R2 = {} <br> RMSE = {} <br> Lin Reg: y = {}x + {}'.format(round(r_value**2,4), round(np.sqrt(np.mean((y - (slope*x+intercept))**2)),2), round(slope,4), round(intercept,4))
+            fig.add_annotation(visible = False, y=0.13,text=annot, showarrow=False)
+            annotationTrack.append(annot)
+            
+            # make the axis equal
+            fig.update_layout(
+                xaxis=dict(
+                    scaleanchor="y",
+                    scaleratio=1,
+                ))
+            
+            # add labels
+            fig.update_layout(
+                xaxis_title="{} sub rate".format(xlabel),
+                yaxis_title="{} sub rate".format(ylabel),
+                margin=dict(
+                    l=0,
+                    r=0,
+                    b=50,
+                    t=50,
+                    pad=4
+                ),
+                title = plotLabel + ' mutation fraction correlation',
+            )
+            
+    # add button to select a specific plot using the traceTrack and a dropdown menu
+    fig.update_layout(
+        updatemenus=[
+            dict(
+                active=0,
+                buttons=list([
+                    # make the annotation visible and the plot visible
+                    dict(label=plot,
+                            method="update",
+                            args=[{"visible": [True if traceTrack[j] == plot else False for j in range(len(traceTrack))]},
+                                    {"annotations": [dict(visible = True if np.unique(traceTrack)[j] == plot else False, y=0.13,text=annotationTrack[idx], showarrow=False) for j in range(len(annotationTrack))]}
+                                  ])
+                    for idx, plot in enumerate(np.unique(traceTrack))
+                ]),
+                x = 1,
+                y = 0.4,
+                xanchor = 'left',
+                yanchor = 'top',
+            )
+        ]
+    )
+    
+    # make the first plot visible
+    fig.data[0].visible = True
+    fig.data[1].visible = True
+    fig.data[2].visible = True
+
+    # make the first annotation visible
+    fig.layout.annotations[0].visible = True
+    
+    return {'fig': fig, 'data': data}
```

### Comparing `dreem-0.1.6/dreem/draw/resources/my_dataset.feather` & `dreem-0.1.8/dreem/draw/resources/my_dataset.feather`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/draw/study.py` & `dreem-0.1.8/dreem/draw/study.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,7 +344,25 @@
 
         """
         return self.wrap_to_plotter(
             plotter.mutation_per_read_per_reference,
             locals(),
             kwargs
         )
+
+    @save_plot
+    @doc_inherit(save_plot, style=style_child_takes_over_parent)
+    @doc_inherit(default_arguments_multi_rows, style=style_child_takes_over_parent)
+    def compare_mutation_profiles(self, max_plots = 100, max_axis = None, **kwargs):
+        """Plot the mutation fraction of multiple mutation profiles.
+
+        Args:
+            max_plots: maximum number of plots to show.
+            max_axis: maximum value of the x and y axis. If None, the maximum value of the data will be used if above 0.15, otherwise 0.15.
+        """
+        kwargs['unique_id'] = True
+        
+        return self.wrap_to_plotter(
+            plotter.compare_mutation_profiles,
+            locals(),
+            kwargs
+        )
```

### Comparing `dreem-0.1.6/dreem/draw/util.py` & `dreem-0.1.8/dreem/draw/util.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/main.py` & `dreem-0.1.8/dreem/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import cProfile
 import os
 import json
 
 from click import Context, group, pass_context
 
 from . import align, cluster, demultiplex, vector, aggregate, draw
+from .util.dependencies import *
 from .util import docdef, logs
 from .util.cli import (merge_params, opt_demultiplex, opt_cluster,
-                       opt_verbose, opt_quiet, opt_log, opt_profile)
+                       opt_verbose, opt_quiet, opt_log, opt_profile,
+                       opt_version)
+
 
 logging_params = [
     opt_verbose,
     opt_quiet,
     opt_log,
     opt_profile,
 ]
 
+misc_params = [
+    opt_version,
+]
+
 all_params = merge_params(logging_params,
                           [opt_demultiplex],
                           demultiplex.params,
                           align.params,
                           vector.params,
                           [opt_cluster],
                           cluster.params,
                           aggregate.params,
                           aggregate.params,
-                          draw.params
+                          draw.params,
+                          misc_params,
                           )
 
 
 # Group for all DREEM commands
 @group(params=all_params,
        invoke_without_command=True,
        context_settings={"show_default": True})
@@ -162,27 +170,42 @@
         rnastructure_dms_min_unpaired_value: float,
         rnastructure_dms_max_paired_value: float,
         rnastructure_deltag_ensemble: bool,
         rnastructure_probability: bool,
         # Drawing
         inpt: tuple[str],
         flat: bool,
+        section: str,
         mutation_fraction: bool,
         mutation_fraction_identity: bool,
         base_coverage: bool,
         mutation_per_read_per_reference: bool,
         mutations_in_barcodes: bool,
+        # Misc
+        version: bool
         ):
+
+    if version:
+        #print(f"DREEM version {__version__}")
+        return 0
+
+    check_bowtie2_exists()
+    check_cutadapt_exists()
+    check_fastqc_exists()
+    check_samtools_exists()
+    check_rnastructure_exists(rnastructure_path)
+    
     """ Run entire DREEM pipeline. """
     # Demultiplexing
     if demult_on:
         fastqs_dir_dm, fastqi_dir_dm, fastq12_dir_dm = demultiplex.run(
             fasta=fasta,
             library=library,
             out_dir=out_dir,
+            temp_dir=temp_dir,
             demulti_overwrite=demulti_overwrite,
             fastq1=fastq1,
             fastq2=fastq2,
             clipped=clipped,
             index_tolerance=index_tolerance,
             mismatch_tolerence=mismatch_tolerence,
             parallel_demultiplexing=parallel_demultiplexing,
@@ -307,19 +330,19 @@
         rnastructure_probability=rnastructure_probability,
     )
 
     draw.run(
         inpt=list(inpt) + [json.load(open(os.path.join(out_dir, f), 'r')) for f in os.listdir(out_dir) if
                            f.endswith(".json")],
         out_dir=out_dir,
-        library=library,
         flat=flat,
         mutation_fraction=mutation_fraction,
         mutation_fraction_identity=mutation_fraction_identity,
         base_coverage=base_coverage,
         mutation_per_read_per_reference=mutation_per_read_per_reference,
         mutations_in_barcodes=mutations_in_barcodes,
+        section=section
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `dreem-0.1.6/dreem/util/cli.py` & `dreem-0.1.8/dreem/util/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,31 +118,31 @@
 # Demultiplexing options
 
 opt_demultiplex = Option(("--demult-on/--demult-off",),
                          type=bool,
                          default=False,
                          help="Whether to run demultiplexing")
 
-opt_parallel_demultiplexing = Option(("--parallel_demultiplexing",),
+opt_parallel_demultiplexing = Option(("--parallel-demultiplexing",),
                                      type=bool,
                                      default=False,
                                      help="Whether to run demultiplexing at maximum speed by submitting multithreaded grep functions")
 
 opt_clipped_demultiplexing = Option(("--clipped",),
                                     type=int,
                                     default=0,
                                     help="Designates the amount of clipped patterns to search for in the sample, will raise compution time")
 
-opt_mismatch_tolerence = Option(("--mismatch_tolerence",),
+opt_mismatch_tolerence = Option(("--mismatch-tolerence",),
                                 type=int,
                                 default=0,
                                 help="Designates the allowable amount of mismatches allowed in a string and still be considered a valid pattern find. \
                             will increase non-parallel computation at a factorial rate. use caution going above 2 mismatches. does not apply to clipped sequences.")
 
-opt_index_tolerence = Option(("--index_tolerance",),
+opt_index_tolerence = Option(("--index-tolerance",),
                              type=int,
                              default=0,
                              help="Designates the allowable amount of distance you allow the pattern to be found in a read from the reference index")
 
 opt_barcode_start = Option(("--barcode-start",),
                            type=int,
                            default=0,
@@ -332,20 +332,20 @@
                            "of a section; reverse primer must be given 5' to 3'"))
 opt_primer_gap = Option(("--primer-gap",),
                         type=int,
                         default=2,
                         help=("Number of bases to leave as a gap between the "
                               "end of a primer and the end of the section"))
 opt_autosect = Option(("--autosect/--no-autosect",),
-                   type=bool,
-                   default=False,
-                   help=("Whether, for every reference that was not explicitly "
-                         "given at least one section (by --initial_coords or "
-                         "--primers), to generate coordinates covering the "
-                         "entire reference sequence automatically"))
+                      type=bool,
+                      default=False,
+                      help=("Whether, for every reference that was not explicitly "
+                            "given at least one section (by --initial_coords or "
+                            "--primers), to generate coordinates covering the "
+                            "entire reference sequence automatically"))
 
 # Vectoring options
 opt_batch_size = Option(("--batch-size", "-z"),
                         type=float,
                         default=32.0,
                         help=("Maximum size of each batch of mutation vectors, "
                               "in millions of base calls"))
@@ -468,14 +468,19 @@
 
 opt_draw_input = Option(("--inpt",),
                         multiple=True,
                         type=Path(exists=True, dir_okay=False),
                         default=(),
                         help="Path to a dreem output format file. Can be specified multiple times.")
 
+opt_section = Option(("--section",),
+                        multiple=True,
+                        default=('full',),
+                        help="Section to draw. Can be specified multiple times.")
+
 opt_flat = Option(("--flat/--no-flat",),
                   is_flag=True,
                   default=True,
                   help="Flatten the output folder structure. This names your files [reference]__[section]__[plot_name].html")
 
 opt_mutation_fraction = Option(("--mutation_fraction", "-mf"),
                                is_flag=True,
@@ -514,14 +519,19 @@
                  default=os.path.join(CWD, datetime.now().strftime(
                      "dreem_%Y-%m-%d_%H:%M:%S.log")))
 opt_profile = Option(("--profile",),
                      type=Path(exists=False, dir_okay=False),
                      default="",
                      help="Profile code performance and log results to file")
 
+# Misc
+opt_version = Option(("--version",),
+                     is_flag=True,
+                     help="Show the version and exit.")
+
 
 def merge_params(*param_lists: list[Parameter]):
     """ Merge lists of Click parameters, dropping duplicates. """
     params = list()
     names = set()
     for param_list in param_lists:
         for param in param_list:
```

### Comparing `dreem-0.1.6/dreem/util/dms.py` & `dreem-0.1.8/dreem/util/dms.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/docdef.py` & `dreem-0.1.8/dreem/util/docdef.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/docstring.py` & `dreem-0.1.8/dreem/util/docstring.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/dump.py` & `dreem-0.1.8/dreem/util/dump.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/files_sanity.py` & `dreem-0.1.8/dreem/util/files_sanity.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,14 +49,33 @@
     cols = []
     cols += ["barcode_start"] if "barcode_start" in library.columns else []
     cols += ["section_start"] if "section_start" in library.columns else []
     cols += ["section_end"] if "section_end" in library.columns else []
     for col in cols:
         library[col] = library[col].apply(lambda x: int(x) if not pd.isnull(x) else x).astype("Int64")
     
+    # Add full section if there is no section or no full
+    for ref, sequence in fasta.groupby("reference"):
+        if not ref in library["reference"].unique():
+            continue
+        # assert that no section is named 'full' and the section_start and section_end are not empty or 1-len(sequence)
+        if "full" in library.loc[library["reference"] == ref, "section"].unique():
+            row = library.loc[(library["reference"] == ref) & (library["section"] == "full")].iloc[0]
+            if row["section_start"] == None and row["section_end"] == None:
+                row["section_start"] = 1
+                row["section_end"] = len(fasta.loc[fasta["reference"] == ref, "sequence"].unique()[0])
+                library.loc[(library["reference"] == ref) & (library["section"] == "full"), "section_start"] = row["section_start"]
+                library.loc[(library["reference"] == ref) & (library["section"] == "full"), "section_end"] = row["section_end"]
+            if (row["section_start"] == 1) and (row["section_end"] == len(fasta.loc[fasta["reference"] == ref, "sequence"].unique()[0])).any():
+                continue
+            raise ValueError(f"reference {ref} has a section named 'full' but the section_start and section_end are not empty or 1-len(sequence)")
+        else:
+            library = pd.concat([library, pd.DataFrame({"reference": ref, "section": "full", "section_start": 1, "section_end": len(fasta.loc[fasta["reference"] == ref, "sequence"].unique()[0])}, index=[0])], axis=0, ignore_index=True)
+    
+    library.reset_index(drop=True, inplace=True)
     # Sections
     # Check that there is only one value for each reference for each column that's not 'reference', 'section', 'section_start', 'section_end'
     if 'section' in library.columns:
         for idx, g in library.groupby("reference"):
             for col in g.columns:
                 if col not in ["reference", "section", "section_start", "section_end"]:
                     un = g[col].unique()
```

### Comparing `dreem-0.1.6/dreem/util/logs.py` & `dreem-0.1.8/dreem/util/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,28 @@
 
 Purpose
 -------
 Central manager of logging.
 """
 
 import logging
+import os
 from subprocess import CompletedProcess
+import sys
+
+#import pkg_resources
+
+#pkg_version = pkg_resources.get_distribution("dreem").version
+
+#WELCOME = f"""
+#Welcome to DREEM version {pkg_version}
+#running on {sys.platform}
+#with {os.cpu_count()} processors.
+#"""
+
 
 
 MAX_VERBOSE = 2
 MAX_QUIET = 2
 FILE_MSG_FORMAT = "LOGMSG>\t%(asctime)s\t%(name)s\t%(levelname)s\n%(message)s\n"
 STREAM_MSG_FORMAT = "%(levelname)s>\t%(message)s"
 
@@ -89,14 +102,15 @@
     logger.addHandler(stream_handler)
     # Add file handler.
     if log_file is not None:
         file_handler = logging.FileHandler(log_file, "a")
         file_handler.setLevel(get_verbosity(verbose=MAX_VERBOSE))
         file_handler.setFormatter(logging.Formatter(FILE_MSG_FORMAT))
         logger.addHandler(file_handler)
+    #logger.info(WELCOME)
 
 
 def log_process(logger: logging.Logger, process: CompletedProcess):
     """ Log the output and error messages of a process. """
     if process.stdout:
         logger.debug(f"STDOUT of {process.args}:\n{process.stdout.decode()}")
     if process.stderr:
```

### Comparing `dreem-0.1.6/dreem/util/parallel.py` & `dreem-0.1.8/dreem/util/parallel.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/path.py` & `dreem-0.1.8/dreem/util/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,163 +1,136 @@
 """
 Path module of DREEM
 ========================================================================
-
 Purpose
 ========================================================================
 Several modules in DREEM produce files used by other modules.
 For example, the alignment module creates alignment map files,
 from which the vectoring module generates mutation vector files,
 from which the aggregate module computes statistics and generates plots.
-
 Modules that pass files to each other must agree on
 - the path to the file, so that the second module can find the file
 - the meaning of each part of the path, so that the second module can
   parse information contained in the path
-
 Although these path conventions could be written separately in each
 module this strategy is not ideal for several reasons:
 - It would risk inconsistencies among the modules, causing bugs.
 - Changing the conventions would require modifying every module,
   which would be not only tedious but also risky for the first reason.
 - Defining all the conventions in one place would reduce the size of the
   code base, improving readability, maintainability, and distribution.  
-
 This module defines all file path conventions for all other modules.
-
-
 Concepts
 ========================================================================
-
 Paths and path segments
 -----------------------
 Every path is represented as a collection of path segments.
 Each segment is the space between two path separators, except for the
 first ("top") segment of a path, which can contain separators.
-
 For example, this path to an alignment map file
 ```/home/rfranklin/tmv/exp58/output/alignment/dms2/tmv-genome.bam```
 would be represented as the following segments:
 - top (full path of the top-level directory): ```/home/rfranklin/tmv/exp58/```
 - module (DREEM module producing the results): ```alignment```
 - sample (name of the sample from the experiment): ```dms2```
 - ref (name of the reference sequence the sample was aligned to): tmv-genome
-
 Classes of paths
 ----------------
-
-
 Usage
 ========================================================================
-
 Creating a path of a specific type using its class
 --------------------------------------------------
 An instance of a specific type of path can be created in three ways:
-
 1. Calling the class directly, giving the names and values of the path
 segments as keyword arguments:
 >>> xam_inp = OneRefAlignmentOutFilePath(top=os.getcwd(),
 ...                                       module=Module.ALIGN,
 ...                                       sample="dms2",
 ...                                       ref="tmv-rna",
 ...                                       ext=".bam")
 >>> assert str(xam_inp) == os.getcwd() + "/alignment/dms2/tmv-rna.bam"
-
 2. Calling the class directly, giving the names and values of the path
 segments as a dictionary of keyword arguments:
 >>> bam_fields = {"top": os.getcwd(), "module": Module.ALIGN,
 ...               "sample": "dms2", "ref": "tmv-rna", "ext": ".bam"}
 >>> xam_inp = OneRefAlignmentOutFilePath(**bam_fields)
 >>> assert str(xam_inp) == os.getcwd() + "/alignment/dms2/tmv-rna.bam"
-
 3. Parsing the path from a string (or from any other object whose
    __str__ method returns a valid path, such as a pathlib.Path object):
 >>> path = os.getcwd() + "/alignment/dms2/tmv-rna.bam"
 >>> xam_inp = OneRefAlignmentOutFilePath.parse(path)
 >>> assert xam_inp.dict() == {"top": os.getcwd(),
 ...                            "module": Module.ALIGN,
 ...                            "sample": "dms2",
 ...                            "ref": "tmv-rna",
 ...                            "ext": ".bam"}
-
 Creating a path by inferring the type from the fields
 -----------------------------------------------------
 This module also provides a convenience function called make_path, which
 behaves identically to the first two examples (of calling the class directly),
 except that instead of the code specifying the type of path to be created,
 make_path infers the type from the keywords arguments. For example:
-
 A few notes on the function make_path:
 - There is no equivalent of parse_path() for make_path because it is impossible
   to uniquely assign fields to segments of an arbitrary path if neither the
   structure nor the values of the fields are known.
 - A TypeError is raised if there is no class of path whose field names match the
   names of the keyword arguments given to make_path.
 - In most cases, this function suffices and alleviates the need to import every
   class of path that will be used in a module.
-
-
 Implementation Details
 ========================================================================
-
 Representation of paths and path segments
 -----------------------------------------
 In this module, every path is represented as a sequence of path segments. Every
 kind of path is represented by a subclass of BasePath, and every kind of segment
 is represented by a subclass of BaseSeg. For example, one subclass of BasePath
 represents the full path to a mutation vector report file, and is made of path
 segments that represent the name of the report file, the name of the directory
 in which it resides, and so on up.
-
 Responsibilities of paths and path segments
 -------------------------------------------
 Each path segment class is responsible for storing information contained in the
 segment (i.e. the value of each field), generating a string representation of
 the segment from the values of the fields, and parsing string representations
 of the segment to determine the values of the fields encoded within. Each path
 class is responsible for storing a series of path segments in the proper order,
 ensuring that the path has all expected and no unexpected segments, ensuring
 that the values of all of its segments are consistent with each other, and
 generating and parsing string representations of the entire path by calling the
 corresponding method of each segment and assembling the results.
-
 Path segment classes and inheritance structure
 ----------------------------------------------
 Every path segment class represents a specific component of a path, such as a
 directory named after a sample or the name of a mutation vector batch file.
-
 The base class of every path segment is BaseSeg, which does not represent any
 specific path segment and should not be instantiated. Every other type of path
 segment is a subclass of BaseSeg. BaseSeg is itself decorated with @dataclass
 but contains no fields. However, it provides all shared methods for path segment
 subclasses (all of which are also decorated with @dataclass):
 - Initialization: __init__ (from @dataclass), __post_init__, validate
 - Field access: fields, field_names, astuple, asdict, replace, _get_dtypes
 - Interface: parse_seg, format_seg
-
 The subclasses of BaseSeg that represent directories are structured as follows:
-
 Subclass of BaseSeg     Fields      Constraints
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 BaseSeg                 -           -
     TopSeg              top         must have permission to read & write
     SubSeg              -           may not contain a path separator
         ModSeg          module      must be a valid module name
         StepStepSeg     step        must be a valid step name
         SampleSeg       sample      -
         RefsetSeg       refset      -
         RefSeg          ref         -
         StructSeg       -           -
             SectionSeg   end5, end3  1 ≤ end5 (int) ≤ end3 (int)
             FileSeg     ext         must be a valid file extension
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 Most segments for file types inherit from both ExtenSeg and another class that
 provides one or more fields that are part of the file name:
-
 Subclass of ExtenSeg    Also subclass of
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 MutVectorBatchSeg       -
 MutVectorReportSeg	    SectionSeg
 XamSeg                  -
     XamMixedSeg         RefsetSeg
     XamSplitSeg         RefSeg
@@ -170,19 +143,16 @@
 Fastq1Seg               -
     Fastq1SampleSeg     SampleSeg
     Fastq1DemultSeg     RefSeg
 Fastq2Seg               -
     Fastq2SampleSeg     SampleSeg
     Fastq2DemultSeg     RefSeg
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 Implementation of path and path segment classes as Pydantic models
 ------------------------------------------------------------------
-
-
 """
 
 # Imports ##############################################################
 
 from __future__ import annotations
 from enum import Enum
 from functools import cache
@@ -399,30 +369,26 @@
 class StructSeg(SubSeg):
     """
     Segment representing any path segment whose name contains an internal
     structure with one or more fields. For example, a segment could encode the
     name of a sample and the year, month, and day on which it was generated.
     This base class provides all the methods of structured segments but does
     not itself have any fields.
-
     Class attributes
     ----------------
     format_str: str
         Specify how to represent the path segment as a string, using Python's
         string formatting mini-language. The string is created by calling
         ```self.format_str.format(*self.dict())```.
-
         Note: ```format_str``` must be compatible with ```pattern_str```
     pattern_str: str
         Specify how to parse a string representing the path to determine the
         values of the fields. The string is parsed using ```re.match```,
         and ```match.groups()``` is used to get the values of the fields.
-
         Note: ```pattern_str``` must be compatible with ```format_str```
-
     Examples
     --------
     >>> class SampleBatchSeg(StructSeg, BatchSeg, SampleSeg):
     ...     format_str = "samp-{}_batch-{}"
     ...     pattern_str = f"samp-{VALID_FIELD_PATTERN}_batch-([0-9]+)"
     >>> str(SampleBatchSeg(sample="tmv", batch=37))
     'samp-tmv_batch-37'
@@ -447,28 +413,26 @@
             f"Segment '{seg_str}' failed to match pattern {cls.pattern_str}")
 
     @classmethod
     def parse(cls, seg_str: Any):
         """
         Return a new instance of the class by parsing the values of the
         fields from a string and passing them to the class constructor.
-
         Parameters
         ----------
         seg_str: Any
             Literal representation of the segment as a ```str``` (or as
             any other object ```x``` for which ```str(x)``` is a valid
             path segment, e.g. an instance of ```pathlib.Path```).
         
         Returns
         -------
         StructSeg
             New instance of StructSeg with fields from ```seg_str```;
             satisfies ```str(seg_inst) == str(seg_str)```.
-
         Raises
         ------
         ValueError
             if the string representation of the newly created instance
             of the class did not match ```seg_str```.
         """
         # Create a new instance of the class by parsing seg_str.
@@ -504,15 +468,14 @@
         # If the fields match, then the formatted string is valid.
         return seg_str
 
 
 class SectionSeg(StructSeg):
     """
     Segment for a directory of a section of a reference sequence.
-
     Fields
     ------
     end5: int
         The 5'-most coordinate in the section; 1-indexed, inclusive.
     end3: int
         The 3'-most coordinate in the section; 1-indexed, inclusive.
     """
@@ -531,20 +494,18 @@
                                  f"> end3 ({values['end3']})")
         return values
 
 
 class FileSeg(StructSeg):
     """
     Segment representing a file name with an extension.
-
     Fields
     ------
     ext: str
         The file extension. Must begin with a period.
-
     Class attributes
     ----------------
     exts: tuple[str]
         All valid file extensions for the class. Each must begin with a period.
     """
     ext: str
     exts: ClassVar[tuple[str, ...]] = tuple()
@@ -782,31 +743,28 @@
     @classmethod
     def _parse_segments(cls,
                         remaining_seg_types: list[type[BaseSeg]],
                         path: str):
         """
         Return a dict of the names and values of the fields encoded
         within a string representation of a path.
-
         Parameters
         ----------
         remaining_seg_types: list[type[BaseSeg]]
             Types of segments in the path that have yet to be used to
             parse part of the path string. The segment types are ordered
             from beginning (left) to end (right) of the path. The first
             item (left-most segment type) must be ```TopSeg```.
         path: str
             Path to be parsed, represented as a string.
-
         Return
         ------
         dict[str, Any]
             A dict of the names (keys) and values (values) of the fields
             encoded in the path string.
-
         Raises
         ------
         PathTypeError
             if any part of the path remains to be parsed after all the
             types of segments have been consumed.
         """
         try:
@@ -853,27 +811,24 @@
         return dict(**cls._parse_segments(remaining_seg_types, remaining_segs),
                     **rightmost_seg_type.parse(rightmost_seg).dict())
 
     @classmethod
     def parse(cls, path: Any):
         """
         Return a new instance of the class by parsing a given path.
-
         Parameters
         ----------
         path: Any
             A ```str``` representing the path to be parsed (or any other
             object ```x``` for which ```str(x)``` returns a valid path,
             e.g. an instance of ```pathlib.Path```).
-
         Returns
         -------
         BasePath
             A new instance of this class that represents the given path.
-
         Raises
         ------
         PathValueError
             if the newly created instance of the class yields a string
             representation that does not match the ```path``` argument.
         """
         path_inst = cls(**cls._parse_segments(list(cls.segment_types()),
@@ -915,15 +870,14 @@
         existing field. """
         return {**self.dict(), **fields}
 
     def edit(self, **fields):
         """ Return a new path instance based on this instance with some
         fields modified according to the keyword arguments. Set a field
         to ```None``` to delete it from the new path instance.
-
         Return
         ------
         BasePath
             Path: modified; Type: modified
         """
         return create(**self._get_new_fields(**fields))
 
@@ -933,28 +887,26 @@
         merging the given fields with the existing fields of this path
         and determining which type matches those fields. Set a field to
         ```None``` to delete it from the new path instance. Note that,
         except for 'ext' (which determines file types), the values of
         the given fields do not affect the return value, since the type
         of path does not depend on the values of the fields, but rather
         on which fields it has (again, except for the field 'ext').
-
         Return
         ------
         BasePath
             Path: preserved; Type: modified
         """
         new_type = get_path_class_by_fields(**self._get_new_fields(**fields))
         return new_type.parse(self)
 
     def move(self, **fields):
         """ Return a new path instance that has the same type as the
         original but has a different path. Determine the new path based
         on the fields given as keyword arguments.
-
         Return
         ------
         BasePath
             Path: modified; Type: preserved
         """
         # First, create the new path (modified path and modified type)
         # using the edit method.
@@ -1531,8 +1483,8 @@
 
 def create(**fields):
     """ Create a new path instance with the given fields. """
     return get_path_class_by_fields(**fields)(**clean_fields(fields))
 
 
 # Ensure that there are no two paths with identical fields.
-_generate_fields_exts_to_path_class()
+_generate_fields_exts_to_path_class()
```

### Comparing `dreem-0.1.6/dreem/util/rnastructure.py` & `dreem-0.1.8/dreem/util/rnastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     # cast the temp file into a dot_bracket structure and extract the attributes
     def __extract_deltaG_struct(self):
         run_command(f"{self.rnastructure_path}ct2dot {self.ct_file} 1 {self.dot_file}")
         temp_dot = open(self.dot_file, 'r')
         first_line = temp_dot.readline().split()
         # If only dots in the structure, no deltaG 
-        print('first_line',first_line)
+
         if len(first_line) == 4:
             _, _, deltaG, _ = first_line
             deltaG = float(deltaG)
         if len(first_line) == 1:
             deltaG, _ = 0.0, first_line[0][1:]
 
         sequence = temp_dot.readline()[:-1] #  Remove the \n
```

### Comparing `dreem-0.1.6/dreem/util/seq.py` & `dreem-0.1.8/dreem/util/seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
         """ Reverse transcribe RNA to DNA. """
         return DNA(self.replace(b"U", b"T"))
 
 
 def parse_fasta(fasta: str | Path):
     """ Parse a FASTA file and iterate through the reference names and
     sequences. """
+    if not fasta:
+        raise TypeError("No FASTA file given")
     logger.info(f"Began parsing FASTA: {fasta}")
     # Get the name of the set of references.
     refset = path.RefsetSeqInFilePath.parse(fasta).refset
     has_ref_named_refset = False
     # Record the names of all the references.
     names = set()
     with open(fasta, "rb") as f:
@@ -161,14 +163,16 @@
             yield name, seq
     logger.info(f"Ended parsing {len(names)} references from FASTA: {fasta}")
 
 
 def write_fasta(fasta: str | Path, refs: Iterable[tuple[str, DNA]]):
     """ Write an iterable of reference names and DNA sequences to a
     FASTA file. """
+    if not fasta:
+        raise TypeError("No FASTA file given")
     logger.info(f"Began writing FASTA file: {fasta}")
     # Get the name of the set of references.
     refset = path.RefsetSeqInFilePath.parse(fasta).refset
     has_ref_named_refset = False
     # Record the names of all the references.
     names = set()
     with open(fasta, "xb") as f:
```

### Comparing `dreem-0.1.6/dreem/util/shell.py` & `dreem-0.1.8/dreem/util/shell.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/util/util.py` & `dreem-0.1.8/dreem/util/util.py`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/dreem/vector/main.py` & `dreem-0.1.8/dreem/vector/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging
+from logging import getLogger
 import pathlib
 from typing import Iterable
 
 from click import command
 import pandas as pd
 
 from ..util import docdef, path
@@ -15,70 +15,73 @@
                         opt_parallel, opt_max_procs,
                         opt_rerun, opt_save_temp)
 from ..util.parallel import lock_output
 from ..util.seq import DNA
 from ..vector.profile import generate_profiles, get_writers
 
 
+logger = getLogger(__name__)
+
+
 def add_coords_from_library(library_path: str,
                             initial_coords: tuple[tuple[str, int, int]]):
     library_coords = list()
     try:
         library = pd.read_csv(library_path)
         for ref, end5, end3 in zip(library["reference"],
                                    library["section_start"],
                                    library["section_end"], strict=True):
             try:
                 coord = (str(pathlib.Path(ref).with_suffix("")),
                          int(end5),
                          int(end3))
             except ValueError as error:
-                logging.error(f"Failed to add coordinates {ref, end5, end3} "
+                logger.error(f"Failed to add coordinates {ref, end5, end3} "
                               f"with the following error: {error}")
             else:
                 if coord in initial_coords or coord in library_coords:
-                    logging.warning(f"Skipping duplicate coordinates: {coord}")
+                    logger.warning(f"Skipping duplicate coordinates: {coord}")
                 else:
                     library_coords.append(coord)
     except (FileNotFoundError, KeyError, ValueError) as error:
-        logging.error(f"Failed to add coordinates from {library_path} "
+        logger.critical(f"Failed to add coordinates from {library_path} "
                       f"with the following error: {error}")
     return initial_coords + tuple(library_coords)
 
 
 def encode_primers(primers: Iterable[tuple[str, str, str]]):
     for ref, fwd, rev in primers:
         try:
             yield ref, DNA(fwd.encode()), DNA(rev.encode())
         except ValueError as error:
-            logging.error(f"Failed to add primer pair {ref, fwd, rev} "
+            logger.error(f"Failed to add primer pair {ref, fwd, rev} "
                           f"with the following error: {error}")
 
 
 def list_bam_paths(bamf: tuple[str, ...], bamd: tuple[str, ...]):
     bam_files: set[pathlib.Path] = set()
 
     def add_bam_file(file: pathlib.Path):
         if not file.is_file():
-            logging.error(f"Skipping non-existant BAM file: {file}")
+            logger.critical(f"Skipping non-existant BAM file: {file}")
             return
         if file.suffix != path.BAM_EXT:
-            logging.warning(f"Skipping non-BAM-formatted file: {file}")
+            logger.critical(f"Skipping non-BAM-formatted file: {file}")
             return
         if file in bam_files:
-            logging.warning(f"Skipping duplicate BAM file: {file}")
+            logger.warning(f"Skipping duplicate BAM file: {file}")
             return
         bam_files.add(file)
 
     for bam_file in bamf:
         add_bam_file(pathlib.Path(bam_file))
     for bam_dir in bamd:
         dpath = pathlib.Path(bam_dir)
         if not dpath.is_dir():
-            logging.error(f"Skipping non-existant BAM directory: {dpath}")
+            logger.critical(f"Skipping non-existant BAM directory: {dpath}")
             continue
         for bamd_file in dpath.iterdir():
             add_bam_file(bamd_file)
 
     return list(bam_files)
 
 
@@ -140,14 +143,18 @@
         max_procs: int,
         parallel: bool,
         rerun: bool,
         save_temp: bool):
     """ Run the vectoring step. Generate a vector encoding mutations for
     each read (or read pair, if paired-end). """
 
+    if not fasta:
+        logger.critical("No FASTA file was given to vectoring")
+        return ()
+
     # If a library file is given, add coordinates from the file.
     if library:
         coords_lib = add_coords_from_library(library_path=library,
                                              initial_coords=coords)
     else:
         coords_lib = coords
```

### Comparing `dreem-0.1.6/dreem/vector/profile.py` & `dreem-0.1.8/dreem/vector/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from ..util.seq import (BLANK, MATCH, DELET, INS_5, INS_3,
                         SUB_A, SUB_C, SUB_G, SUB_T, EVERY,
                         BASES, DNA, parse_fasta)
 from ..util.util import digest_file
 from ..vector.samread import SamReader
 from ..vector.vector import vectorize_line, vectorize_pair, VectorError
 
-
 logger = getLogger(__name__)
 
 SectionTuple = namedtuple("PrimerTuple", ["pos5", "pos3"])
 
 
 def mib_to_bytes(batch_size: float):
     """
@@ -459,18 +458,15 @@
                      read_names: list[str],
                      vectors: tuple[bytearray, ...],
                      n_passed: int):
         """ Write a batch of mutation vectors to an ORC file. """
         # Process the mutation vectors into a 2D NumPy array.
         logger.info(f"Began writing batch {batch_num} of {self}")
         array = np.frombuffer(b"".join(vectors), dtype=np.byte)
-        try:
-            array.shape = (n_passed, self.length)
-        except ValueError:
-            return None
+        array.shape = (n_passed, self.length)
         # Data must be converted to pd.DataFrame for PyArrow to write.
         # Set copy=False to prevent copying the mutation vectors.
         mut_frame = pd.DataFrame(data=array,
                                  index=read_names,
                                  columns=self.columns,
                                  copy=False)
         mv_file = self.get_mv_batch_path(out_dir, batch_num)
@@ -496,15 +492,16 @@
                 vectorize_line(line1, muts, self.byteseq, self.length,
                                self.end5, self.ref, min_qual, ambid)
             if not any(muts):
                 raise VectorError(f"{read_name} gave a blank mutation vector")
         except VectorError as error:
             logger.error(
                 f"Read '{read_name.decode()}' failed to vectorize: {error}")
-            return "", b""
+            read_name = b""
+            muts = bytearray()
         return read_name, muts
 
     def _vectorize_records(self, /, *,
                            reader: SamReader,
                            start: int,
                            stop: int,
                            strict_pairs: bool,
@@ -551,20 +548,20 @@
                                                    **kwargs)
         # Compute the number of reads that passed and failed.
         n_reads = len(muts)
         n_pass = len(read_names)
         n_fail = n_reads - n_pass
         if n_pass == 0:
             logger.critical(f"Failed to assemble batch {batch_num} of {self}")
-            return n_pass, n_fail, "FAIL"
+            return n_pass, n_fail, ""
         # Write the names and vectors to a file.
         b_file = self._write_batch(out_dir, batch_num, read_names, muts, n_pass)
         if b_file is None:
             logger.critical(f"Failed to assemble batch {batch_num} of {self}")
-            return n_pass, n_fail, "FAIL"
+            return n_pass, n_fail, ""
         # Compute the MD5 checksum of the file.
         checksum = digest_file(b_file.path)
         logger.debug(f"Ended vectorizing batch {batch_num} of {self} "
                      f"({start} - {stop}): {n_pass} pass, {n_fail} fail")
         return n_pass, n_fail, checksum
 
     def _vectorize_bam(self, /, *,
@@ -1034,15 +1031,15 @@
     @property
     def shape(self):
         return self.n_vectors, self.length
 
     def get_batch(self,
                   batch: int,
                   positions: Sequence[int] | None = None,
-                  numeric: bool = True):
+                  numeric: bool = False):
         """
         Return the mutation vectors from one batch. Optionally, select
         a subset of the columns of the mutation vectors.
 
         Parameters
         ----------
         batch: int (≥ 0)
@@ -1073,14 +1070,18 @@
             subseq = self.subseq(positions)
             columns = [self.INDEX_COL] + self.seq_pos_to_cols(subseq, positions)
         # Read the vectors from the ORC file using PyArrow as backend.
         vectors = pd.read_orc(self.get_mv_batch_path(self.out_dir, batch).path,
                               columns=columns)
         # Remove the column of read names and set it as the index.
         vectors.set_index(self.INDEX_COL, drop=True, inplace=True)
+        # Convert the index from bytes to str and give it a name.
+        vectors.set_index(pd.Index(vectors.index.map(bytes.decode),
+                                   name="Read Name"),
+                          inplace=True)
         if numeric:
             # Convert the remaining columns to their integer positions.
             vectors.columns = positions if positions else self.positions
         # The vectors are stored as signed 8-bit integers (np.int8) and
         # must be cast to unsigned 8-bit integers (np.uint8) so that the
         # bitwise operations work. This step must be doneafter removing
         # the column of read names (which cannot be cast to np.uint8).
@@ -1141,19 +1142,19 @@
         if self.n_batches == 0:
             return pd.DataFrame(columns=(self.positions if positions is None
                                          else positions), dtype=int)
         # Load and concatenate every vector batch into one DataFrame.
         return pd.concat(self.get_all_batches(positions, numeric), axis=0)
 
     @classmethod
-    def _query_vectors(cls, /,
-                       vectors: pd.DataFrame,
-                       query: int, *,
-                       subsets: bool = False,
-                       supersets: bool = False) -> pd.DataFrame:
+    def query_vectors(cls, /,
+                      vectors: pd.DataFrame,
+                      query: int, *,
+                      subsets: bool = False,
+                      supersets: bool = False) -> pd.DataFrame:
         """
         Return a boolean array of the same shape as vectors where
         element i,j is True if and only if the byte at element i,j of
         vectors matches the given query byte. By default, a byte in
         vectors matches if it equals the query byte and is not blank
         (i.e. 00000000). Matches can be extended to include bitwise
         subsets and supersets of query by setting the corresponding
@@ -1181,28 +1182,28 @@
             raise TypeError(
                 f"Expected query of type int, but got {type(query).__name__}")
         if not BLANK <= query <= EVERY:
             raise ValueError(
                 f"Expected query in range {BLANK} - {EVERY}, but got {query}")
         if supersets and subsets:
             # Count both supersets and subsets.
-            return (cls._query_vectors(vectors, query, supersets=True)
-                    | cls._query_vectors(vectors, query, subsets=True))
+            return (cls.query_vectors(vectors, query, supersets=True)
+                    | cls.query_vectors(vectors, query, subsets=True))
         if supersets:
             # Non-blank vector bytes that are matches and supersets of
             # the query byte count.
             if query == BLANK:
                 # If query is BLANK (00000000), then every non-blank
                 # byte is a superset.
                 return vectors.astype(bool, copy=True)
             if query == EVERY:
                 # If the query is EVERY (11111111), then no bitwise
                 # supersets exist. Since subsets do not count, only
                 # exact matches count.
-                return cls._query_vectors(vectors, query)
+                return cls.query_vectors(vectors, query)
             # No shortcut method can be used, so the supersets must be
             # computed explicitly. A vector byte is a match or superset
             # of the query byte iff both of the following are true:
             # - The bitwise intersection of the vector and query bytes
             #   equals the query byte, meaning that every bit set to 1
             #   in the query byte is also set to 1 in the vector byte,
             #   and thus the vector byte is a superset of the query.
@@ -1228,15 +1229,15 @@
                 # byte is a subset.
                 return vectors.astype(bool, copy=True)
             if (query & (query - 1)) == 0:
                 # If query is a power of 2, then it has exactly one bit
                 # set to 1. Thus, the only possible subset of the query
                 # is the blank byte, which never counts. Since supersets
                 # do not count either, only exact matches count.
-                return cls._query_vectors(vectors, query)
+                return cls.query_vectors(vectors, query)
             # No shortcut method can be used, so the subsets must be
             # computed explicitly. A vector byte is a match or subset of
             # the query byte iff both of the following are true:
             # - The bitwise union of the vector and query bytes equals
             #   the query byte, meaning that there are no bits set to 1
             #   in the vector byte that are not 1 in the query byte,
             #   and thus the vector byte is a subset of the query.
@@ -1280,18 +1281,18 @@
             return pd.Series([], dtype=int)
         # Initialize empty list to count the mutations in each vector.
         counts = list()
         # Iterate over all batches of vectors.
         for vectors in self.get_all_batches(positions):
             # Count the number of mutations in each vector in the batch
             # and append them to the list of counts.
-            counts.append(self._query_vectors(vectors,
-                                              query,
-                                              subsets=subsets,
-                                              supersets=supersets).sum(axis=1))
+            counts.append(self.query_vectors(vectors,
+                                             query,
+                                             subsets=subsets,
+                                             supersets=supersets).sum(axis=1))
         # Concatenate and return the number of mutations in each vector
         # among all batches.
         return pd.concat(counts, axis=0)
 
     @cache
     def count_muts_by_pos(self, /,
                           query: int, *,
@@ -1328,18 +1329,18 @@
         counts = pd.Series(np.zeros(self.length, dtype=int),
                            index=(self.positions if positions is None
                                   else positions))
         # Iterate over all batches of vectors.
         for vectors in self.get_all_batches(positions, numeric):
             # Add the number of mutations at each position in the batch
             # to the cumulative count of mutations at each position.
-            counts += self._query_vectors(vectors,
-                                          query,
-                                          subsets=subsets,
-                                          supersets=supersets).sum(axis=0)
+            counts += self.query_vectors(vectors,
+                                         query,
+                                         subsets=subsets,
+                                         supersets=supersets).sum(axis=0)
         return counts
 
     def get_cluster_mus(self, /,
                         membership: pd.DataFrame,
                         query: int, *,
                         subsets: bool = False,
                         supersets: bool = False,
@@ -1411,18 +1412,18 @@
 
         5.  Compute the mutation rates for each cluster by dividing the
             cluster-weighted number of mutations at each position by the
             weighted number of reads in the cluster:
 
             return mutsums / readsums
         """
-        return (self._query_vectors(self.get_all_vectors(positions, numeric),
-                                    query,
-                                    subsets=subsets,
-                                    supersets=supersets).T.dot(membership)
+        return (self.query_vectors(self.get_all_vectors(positions, numeric),
+                                   query,
+                                   subsets=subsets,
+                                   supersets=supersets).T.dot(membership)
                 / membership.sum(axis=0))
 
     @classmethod
     def load(cls, report_file: str, validate_checksums: bool = True):
         if not (report := VectorReport.load(report_file, validate_checksums)):
             logger.critical(f"Failed to load report from {report_file}")
             return
@@ -1622,24 +1623,24 @@
         else b"?"
     )
 ) for i in range(256)])))
 
 
 def trans_vectors_iter(vectors: pd.DataFrame):
     for index, row in zip(vectors.index, vectors.values, strict=True):
-        translated = row.tobytes(order='C').translate(vector_trans_table)
-        yield b"%b\t%b\n" % (index, translated)
+        vector = row.tobytes(order='C').translate(vector_trans_table).decode()
+        yield f"{index}\t{vector}\n"
 
 
 def trans_vectors_block(vectors: pd.DataFrame, reference: bool = False):
     lines = trans_vectors_iter(vectors)
     if reference:
         # Display the reference sequence above the vectors.
         try:
             # Get the reference sequence from the column names.
             seq, _ = VectorReader.cols_to_seq_pos(vectors.columns.tolist())
             # Prepend the reference sequence to the lines of vectors.
-            lines = chain([b"Reference\t%b\n" % seq], lines)
+            lines = chain([f"Reference\t{seq.decode()}\n"], lines)
         except Exception as error:
             logger.error(f"Could not determine sequence from columns of the "
                          f"vectors (perhaps you used numeric=True): {error} ")
-    return b"".join(lines)
+    return "".join(lines)
```

### Comparing `dreem-0.1.6/dreem/vector/samread.py` & `dreem-0.1.8/dreem/vector/samread.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             flag = first_line.split(SAM_DELIMITER, 2)[1]
             paired = bool(int(flag) & 1)
             logger.debug(f"SAM file {self.sam_path} has "
                          f"{'paired' if paired else 'single'}-ended reads")
             return paired
         except (IndexError, ValueError):
             raise ValueError("Failed to determine pairing from first record: "
-                             + first_line.decode())
+                             + first_line.decode()+f" {self.sam_path}")
 
     @property
     def mates_per_record(self):
         """ Mates per record: 1 if single-end, 2 if paired-end. """
         return self.paired + 1
 
     def iter_records(self, start: int, stop: int, strict_pairs: bool):
```

### Comparing `dreem-0.1.6/dreem/vector/vector.py` & `dreem-0.1.8/dreem/vector/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,40 +686,36 @@
                 region_idx3 = region_length
             # Act based on the CIGAR operation and its length.
             if cigar_op == CIG_MATCH:
                 # The read and reference sequences match over the entire
                 # CIGAR operation.
                 for base, qual in zip(read.seq[read_idx5: read_idx3],
                                       read.qual[read_idx5: read_idx3]):
-                    muts[region_idx5] = (encode_match(base, qual, min_qual)
-                                         | muts[region_idx5])
+                    muts[region_idx5] = encode_match(base, qual, min_qual)
                     region_idx5 += 1
             elif cigar_op == CIG_ALIGN or cigar_op == CIG_SUBST:
                 # The read contains only matches or substitutions (no
                 # indels) relative to the reference over the entire
                 # CIGAR operation.
                 for ref_base, read_base, read_qual in zip(
                         region_seq[region_idx5: region_idx3],
                         read.seq[read_idx5: read_idx3],
                         read.qual[read_idx5: read_idx3],
                         strict=True):
-                    muts[region_idx5] = (encode_compare(ref_base,
-                                                        read_base,
-                                                        read_qual,
-                                                        min_qual)
-                                         | muts[region_idx5])
+                    muts[region_idx5] = encode_compare(ref_base, read_base,
+                                                       read_qual, min_qual)
                     region_idx5 += 1
             elif cigar_op == CIG_DELET:
                 # The portion of the reference sequence corresponding
                 # to the CIGAR operation is deleted from the read.
                 # Create one Deletion object for each base in the
                 # reference sequence that is missing from the read.
                 while region_idx5 < region_idx3:
                     dels.append(Deletion(region_idx5, read_idx5))
-                    muts[region_idx5] = muts[region_idx5] | DELET
+                    muts[region_idx5] = DELET
                     region_idx5 += 1
             elif cigar_op == CIG_INSRT:
                 # The read contains an insertion of one or more bases
                 # that are not present in the reference sequence.
                 # Create one Insertion object for each base in the read
                 # sequence that is not present in the reference. Every
                 # mutation needs to be assigned a coordinate in the
@@ -804,16 +800,18 @@
         raise VectorValueError(f"Read '{read.qname.decode()}' had reference "
                                f"'{read.rname}' (≠ '{ref}')")
     vectorize_read(read, muts, seq, length, end5, qmin, ambid)
 
 
 def vectorize_pair(line1: bytes, line2: bytes, muts: bytearray, seq: bytes,
                    length: int, end5: int, ref: str, qmin: int, ambid: bool):
+    # Parse lines 1 and 2 into SAM reads.
     read1 = SamRead(line1)
     read2 = SamRead(line2)
+    # Ensure that reads 1 and 2 are compatible mates.
     if not read1.flag.paired:
         raise VectorValueError(f"Read 1 ({read1.qname.decode()}) was not "
                                f"paired, but read 2 ('{read2.qname.decode()}') "
                                f"was given")
     if not read2.flag.paired:
         raise VectorValueError(f"Read 2 ({read2.qname.decode()}) was not "
                                f"paired, but read 1 ({read1.qname.decode()}) "
@@ -832,9 +830,16 @@
     if not (read1.flag.first and read2.flag.second):
         raise VectorValueError(f"Read '{read1.qname.decode()}' had mate 1 "
                                f"labeled {2 - read1.flag.first} and mate 2 "
                                f"labeled {1 + read2.flag.second}")
     if read1.flag.rev == read2.flag.rev:
         raise VectorValueError(f"Read '{read1.qname.decode()}' had "
                                "mates 1 and 2 facing the same way")
-    vectorize_read(read1, muts, seq, length, end5, qmin, ambid)
-    vectorize_read(read2, muts, seq, length, end5, qmin, ambid)
+    # Vectorize read 1.
+    muts1 = muts.copy()
+    vectorize_read(read1, muts1, seq, length, end5, qmin, ambid)
+    # Vectorize read 2.
+    muts2 = muts.copy()
+    vectorize_read(read2, muts2, seq, length, end5, qmin, ambid)
+    # Compute the consensus of reads 1 and 2.
+    for i, (m1, m2) in enumerate(zip(muts1, muts2, strict=True)):
+        muts[i] = inter if (inter := m1 & m2) else m1 | m2
```

### Comparing `dreem-0.1.6/dreem.egg-info/SOURCES.txt` & `dreem-0.1.8/dreem.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
-env.yml
 pyproject.toml
-requirements.txt
 setup.py
 dreem/__init__.py
+dreem/env.yml
 dreem/main.py
+dreem/requirements.txt
 dreem.egg-info/PKG-INFO
 dreem.egg-info/SOURCES.txt
 dreem.egg-info/dependency_links.txt
 dreem.egg-info/entry_points.txt
 dreem.egg-info/requires.txt
 dreem.egg-info/top_level.txt
 dreem/aggregate/__init__.py
@@ -40,14 +40,15 @@
 dreem/draw/util.py
 dreem/draw/resources/my_dataset.feather
 dreem/resources/__init__.py
 dreem/resources/get_attributes.py
 dreem/util/__init__.py
 dreem/util/artxt.py
 dreem/util/cli.py
+dreem/util/dependencies.py
 dreem/util/dms.py
 dreem/util/docdef.py
 dreem/util/docstring.py
 dreem/util/dump.py
 dreem/util/files_sanity.py
 dreem/util/logs.py
 dreem/util/parallel.py
@@ -57,8 +58,9 @@
 dreem/util/shell.py
 dreem/util/util.py
 dreem/vector/__init__.py
 dreem/vector/main.py
 dreem/vector/profile.py
 dreem/vector/samread.py
 dreem/vector/vector.py
+test/test_demultiplexing.py
 test/test_pipeline.py
```

### Comparing `dreem-0.1.6/dreem.egg-info/requires.txt` & `dreem-0.1.8/dreem/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 click-option-group==0.5.5
 colorlog==6.7.0
 commonmark==0.9.1
 contourpy==1.0.6
 cookiecutter==2.1.1
 cssselect2==0.7.0
 custom-inherit==2.4.1
-cutadapt==4.1
+cutadapt>=4.1
 cycler==0.11.0
 debugpy==1.6.3
 decorator==5.1.1
 distlib==0.3.6
 dms_ci>=0.1.0
 dnaio==0.10.0
 docutils==0.17.1
```

### Comparing `dreem-0.1.6/env.yml` & `dreem-0.1.8/dreem/env.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 name: dreem
 channels:
   - conda-forge
   - bioconda
   - defaults
 dependencies:
-  - bowtie2=2.4.5
+  - bowtie2>=2.4.5, !=2.5.0
   - bzip2=1.0.8
   - ca-certificates=2023.01.10
   - certifi=2022.12.7
   - expat=2.4.9
-  - fastqc=0.12.1
+  - fastqc>=0.12.1
   - font-ttf-dejavu-sans-mono=2.37
   - fontconfig=2.14.1
   - freetype=2.12.1
   - gdbm=1.18
   - icu=58.2
   - libcxx=14.0.6
   - libffi=3.4.2
@@ -22,20 +22,21 @@
   - libxml2=2.9.14
   - llvm-openmp=14.0.6
   - ncurses=6.4
   - openjdk=11.0.13
   - openssl=1.1.1t
   - perl=5.34.0
   - pip=22.3.1
-  - python=3.10.9
+  - python>=3.10, <4.0
   - readline=8.2
-  - rnastructure=6.3
-  - samtools=1.16.1
+  - rnastructure>=6.3
+  - samtools>=1.16.1
   - setuptools=65.6.3
   - sqlite=3.40.1
   - tk=8.6.12
   - tzdata=2022g
   - wheel=0.38.4
   - xz=5.2.10
   - zlib=1.2.13
+  - seqkit=2.4.0
   - pip:
     - -r requirements.txt
```

### Comparing `dreem-0.1.6/pyproject.toml` & `dreem-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dreem-0.1.6/requirements.txt` & `dreem-0.1.8/dreem.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 click-option-group==0.5.5
 colorlog==6.7.0
 commonmark==0.9.1
 contourpy==1.0.6
 cookiecutter==2.1.1
 cssselect2==0.7.0
 custom-inherit==2.4.1
-cutadapt==4.1
+cutadapt>=4.1
 cycler==0.11.0
 debugpy==1.6.3
 decorator==5.1.1
 distlib==0.3.6
 dms_ci>=0.1.0
 dnaio==0.10.0
 docutils==0.17.1
```

### Comparing `dreem-0.1.6/setup.py` & `dreem-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 
 requirements = []
-with open('requirements.txt', 'r') as fh:
+with open('dreem/requirements.txt', 'r') as fh:
     for line in fh:
         requirements.append(line.strip())
 
 # PYTHON_VERSION = (3,10)
 
 # if sys.version_info < PYTHON_VERSION:
 #    sys.exit(f"Python >= {PYTHON_VERSION[0]}.{PYTHON_VERSION[1]} required.")
 
 readme = open('README.md').read()
 
 setup(
     name="dreem",
-    version='0.1.6',
+    version='0.1.8',
     description="DREEM solves RNA structure ensembles using chemical probing data",
     long_description=readme,
     author="Silvi Rouskin Lab",
     author_email="silvi@hms.harvard.edu",
     url="https://github.com/rouskinlab/dreem",
     packages=find_packages(),
     package_dir={'dreem': 'dreem'},
```

### Comparing `dreem-0.1.6/test/test_pipeline.py` & `dreem-0.1.8/test/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,20 @@
         fastq1=(os.path.join(test_files, sample, '{}_R1.fastq'.format(sample)),),
         fastq2=(os.path.join(test_files, sample, '{}_R2.fastq'.format(sample)),),
         fasta=os.path.join(test_files, sample, '{}.fasta'.format(sample)),
         library=os.path.join(test_files, sample, 'library.csv'),
         samples=os.path.join(test_files, sample, 'samples.csv'),
         rerun=True,
         flat=True,
+        #rnastructure_path='/Users/ymdt/src/RNAstructure/exe/',
     )
 
 @pytest.mark.parametrize('sample', ['my_cli_sample'])
 def test_run_cli(sample):
-    os.system('dreem --out-dir {} --temp-dir {} --fastq1 {} --fastq2 {} --fasta {} --library {} --samples {} --rerun '.format(
+    os.system('dreem --out-dir {} --temp-dir {} --fastq1 {} --fastq2 {} --fasta {} --library {} --samples {} --section roi --section ms2 --section 1-50 --rerun '.format(
         top_dir,
         temp_dir,
         os.path.join(test_files, sample, '{}_R1.fastq'.format(sample)),
         os.path.join(test_files, sample, '{}_R2.fastq'.format(sample)),
         os.path.join(test_files, sample, '{}.fasta'.format(sample)),
         os.path.join(test_files, sample, 'library.csv'),
         os.path.join(test_files, sample, 'samples.csv'),
```

