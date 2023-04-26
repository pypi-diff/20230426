# Comparing `tmp/PyXAB-0.2.0.tar.gz` & `tmp/PyXAB-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyXAB-0.2.0.tar", last modified: Tue Mar 21 19:43:08 2023, max compression
+gzip compressed data, was "dist/PyXAB-0.2.1.tar", last modified: Wed Apr 26 03:18:03 2023, max compression
```

## Comparing `PyXAB-0.2.0.tar` & `PyXAB-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.607650 PyXAB-0.2.0/
--rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.0/LICENSE
--rw-r--r--   0 william    (501) staff       (20)    15697 2023-03-21 19:43:08.607885 PyXAB-0.2.0/PKG-INFO
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.591876 PyXAB-0.2.0/PyXAB/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.0/PyXAB/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.598152 PyXAB-0.2.0/PyXAB/algos/
--rw-r--r--   0 william    (501) staff       (20)     1414 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/Algo.py
--rw-r--r--   0 william    (501) staff       (20)     6138 2023-03-21 19:41:05.000000 PyXAB-0.2.0/PyXAB/algos/DOO.py
--rw-r--r--   0 william    (501) staff       (20)     5086 2023-03-21 19:41:05.000000 PyXAB-0.2.0/PyXAB/algos/GPO.py
--rw-r--r--   0 william    (501) staff       (20)    10125 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/HCT.py
--rw-r--r--   0 william    (501) staff       (20)     8908 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/HOO.py
--rw-r--r--   0 william    (501) staff       (20)     2357 2023-03-13 22:43:37.000000 PyXAB-0.2.0/PyXAB/algos/PCT.py
--rw-r--r--   0 william    (501) staff       (20)     5422 2023-03-21 19:41:05.000000 PyXAB-0.2.0/PyXAB/algos/POO.py
--rw-r--r--   0 william    (501) staff       (20)     5380 2023-03-21 19:41:05.000000 PyXAB-0.2.0/PyXAB/algos/SOO.py
--rw-r--r--   0 william    (501) staff       (20)     7178 2023-03-13 14:03:23.000000 PyXAB-0.2.0/PyXAB/algos/SequOOL.py
--rw-r--r--   0 william    (501) staff       (20)     7337 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/StoSOO.py
--rw-r--r--   0 william    (501) staff       (20)    11015 2023-03-13 14:03:23.000000 PyXAB-0.2.0/PyXAB/algos/StroquOOL.py
--rw-r--r--   0 william    (501) staff       (20)    11937 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/VHCT.py
--rw-r--r--   0 william    (501) staff       (20)     2359 2023-03-13 22:43:37.000000 PyXAB-0.2.0/PyXAB/algos/VPCT.py
--rw-r--r--   0 william    (501) staff       (20)      320 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/algos/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.601505 PyXAB-0.2.0/PyXAB/partition/
--rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/BinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/DimensionBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/KaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.0/PyXAB/partition/Node.py
--rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/Partition.py
--rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/RandomBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/RandomKaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/partition/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.605092 PyXAB-0.2.0/PyXAB/synthetic_obj/
--rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Ackley.py
--rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Cexample.py
--rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/DifficultFunc.py
--rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/DoubleSine.py
--rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Garland.py
--rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Himmelblau.py
--rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Objective.py
--rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/Rastrigin.py
--rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.0/PyXAB/synthetic_obj/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.607041 PyXAB-0.2.0/PyXAB/utils/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.0/PyXAB/utils/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.0/PyXAB/utils/plot.py
--rw-r--r--   0 william    (501) staff       (20)     2477 2023-03-13 22:43:37.000000 PyXAB-0.2.0/PyXAB/utils/run_cumulative.py
--rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.0/PyXAB/utils/visualize_gif.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-03-21 19:43:08.593209 PyXAB-0.2.0/PyXAB.egg-info/
--rw-r--r--   0 william    (501) staff       (20)    15697 2023-03-21 19:43:08.000000 PyXAB-0.2.0/PyXAB.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1157 2023-03-21 19:43:08.000000 PyXAB-0.2.0/PyXAB.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2023-03-21 19:43:08.000000 PyXAB-0.2.0/PyXAB.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       25 2023-03-21 19:43:08.000000 PyXAB-0.2.0/PyXAB.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)        6 2023-03-21 19:43:08.000000 PyXAB-0.2.0/PyXAB.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)    13382 2023-03-13 03:58:11.000000 PyXAB-0.2.0/README.md
--rw-r--r--   0 william    (501) staff       (20)      103 2023-03-21 19:43:08.608366 PyXAB-0.2.0/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)     3881 2023-03-21 19:41:05.000000 PyXAB-0.2.0/setup.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.051119 PyXAB-0.2.1/
+-rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.1/LICENSE
+-rw-r--r--   0 william    (501) staff       (20)    15987 2023-04-26 03:18:03.051351 PyXAB-0.2.1/PKG-INFO
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.031588 PyXAB-0.2.1/PyXAB/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.1/PyXAB/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.038325 PyXAB-0.2.1/PyXAB/algos/
+-rw-r--r--   0 william    (501) staff       (20)     1415 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/Algo.py
+-rw-r--r--   0 william    (501) staff       (20)     6130 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/DOO.py
+-rw-r--r--   0 william    (501) staff       (20)     5335 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/GPO.py
+-rw-r--r--   0 william    (501) staff       (20)    10126 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/HCT.py
+-rw-r--r--   0 william    (501) staff       (20)     8909 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/HOO.py
+-rw-r--r--   0 william    (501) staff       (20)     2358 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/PCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5670 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/POO.py
+-rw-r--r--   0 william    (501) staff       (20)     5390 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/SOO.py
+-rw-r--r--   0 william    (501) staff       (20)     7170 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/SequOOL.py
+-rw-r--r--   0 william    (501) staff       (20)     7337 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/algos/StoSOO.py
+-rw-r--r--   0 william    (501) staff       (20)    10994 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/StroquOOL.py
+-rw-r--r--   0 william    (501) staff       (20)    11938 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/VHCT.py
+-rw-r--r--   0 william    (501) staff       (20)     2360 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/VPCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5218 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/Zooming.py
+-rw-r--r--   0 william    (501) staff       (20)      331 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.043475 PyXAB-0.2.1/PyXAB/partition/
+-rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/BinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/DimensionBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/KaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.1/PyXAB/partition/Node.py
+-rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/Partition.py
+-rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/RandomBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/RandomKaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.048445 PyXAB-0.2.1/PyXAB/synthetic_obj/
+-rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Ackley.py
+-rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Cexample.py
+-rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/DifficultFunc.py
+-rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/DoubleSine.py
+-rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Garland.py
+-rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Himmelblau.py
+-rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Objective.py
+-rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Rastrigin.py
+-rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.050511 PyXAB-0.2.1/PyXAB/utils/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.1/PyXAB/utils/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.1/PyXAB/utils/plot.py
+-rw-r--r--   0 william    (501) staff       (20)     2477 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/utils/run_synthetic.py
+-rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/utils/visualize_gif.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.032963 PyXAB-0.2.1/PyXAB.egg-info/
+-rw-r--r--   0 william    (501) staff       (20)    15987 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     1179 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (501) staff       (20)        1 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (501) staff       (20)       25 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/requires.txt
+-rw-r--r--   0 william    (501) staff       (20)        6 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/top_level.txt
+-rw-r--r--   0 william    (501) staff       (20)    13664 2023-04-26 03:17:41.000000 PyXAB-0.2.1/README.md
+-rw-r--r--   0 william    (501) staff       (20)      103 2023-04-26 03:18:03.051821 PyXAB-0.2.1/setup.cfg
+-rw-r--r--   0 william    (501) staff       (20)     3881 2023-04-26 03:17:54.000000 PyXAB-0.2.1/setup.py
```

### Comparing `PyXAB-0.2.0/LICENSE` & `PyXAB-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PKG-INFO` & `PyXAB-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -120,14 +120,15 @@
         
         ### *X*-armed bandit algorithms
         
         * Algorithm starred are meta-algorithms (wrappers)
         
         | Algorithm                                                                           | Research Paper                                                                                                                                                                           | Year |
         |-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
+        | [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py)     | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf)                                                                                                              | 2008 |
         | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py)           | [*X*-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html)                                                                                                                           | 2011 |
         | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
         | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
         | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
         | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
         | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
         | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.0 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.1 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
@@ -43,31 +43,33 @@
 update if needed ``` To install via git, run the following lines of code
 ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
 . ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
 meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
 ------------------------------------------------------------------------|------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|------| | [T-HOO](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
-bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
+blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
+(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
+jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
+Deterministic Function without the Knowledge of its Smoothness](https://
+proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
+Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
 without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
-Optimization of a Deterministic Function without the Knowledge of its
-Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
-Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
-valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
-Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
-optimization of noisy functions with unknown smoothness](https://
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
+[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
+v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
+Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
+[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
+[Black-box optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/Algo.py` & `PyXAB-0.2.1/PyXAB/algos/Algo.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -63,8 +63,8 @@
         Every algorithm needs a function to get the last point
 
         Returns
         -------
         chosen_point: list
             The point chosen by the algorithm
         """
-        pass
+        pass
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/DOO.py` & `PyXAB-0.2.1/PyXAB/algos/DOO.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pdb
 
 
 class DOO_node(P_node):
     """
     Implementation of the node in the DOO algorithm
     """
-    
+
     def __init__(self, depth, index, parent, domain):
         """
         Initialization of the DOO node
         
         Parameters
         ----------
         depth: int
@@ -99,15 +99,15 @@
         return self.reward
 
 
 class DOO(Algorithm):
     """
     The implementation of the DOO algorithm (Munos, 2011)
     """
-    
+
     def __init__(self, n=100, delta=None, domain=None, partition=None):
         """
         The initialization of the DOO algorithm
 
         Parameters
         ----------
         n: int
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/GPO.py` & `PyXAB-0.2.1/PyXAB/algos/GPO.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,22 @@
         super(GPO, self).__init__()
         if domain is None:
             raise ValueError("Parameter space is not given.")
         if partition is None:
             raise ValueError("Partition of the parameter space is not given.")
         if algo is None:
             raise ValueError("Algorithm for GPO is not given")
-        if algo.__name__ != 'T_HOO' and algo.__name__ != 'HCT' and algo.__name__ != 'VHCT':
-            raise NotImplementedError('GPO has not yet included implementations for this algorithm')
+        if (
+            algo.__name__ != "T_HOO"
+            and algo.__name__ != "HCT"
+            and algo.__name__ != "VHCT"
+        ):
+            raise NotImplementedError(
+                "GPO has not yet included implementations for this algorithm"
+            )
 
         self.rounds = rounds
         self.rhomax = rhomax
         self.numax = numax
         self.Dmax = np.log(2) / np.log(1 / rhomax)
         self.domain = domain
         self.partition = partition
@@ -86,21 +92,28 @@
             The point chosen by the GPO algorithm
         """
         if self.phase > self.N:  # If already finished
             return self.goodx
         else:
             if self.counter == 0:
                 rho = self.rhomax ** (2 * self.N / (2 * self.phase + 1))
-                if self.algo.__name__ == 'T_HOO':
+                if self.algo.__name__ == "T_HOO":
                     self.curr_algo = self.algo(
-                        nu=self.numax, rho=rho, rounds=self.rounds, domain=self.domain, partition=self.partition
+                        nu=self.numax,
+                        rho=rho,
+                        rounds=self.rounds,
+                        domain=self.domain,
+                        partition=self.partition,
                     )
-                elif self.algo.__name__ == 'HCT' or self.algo.__name__ == 'VHCT':
+                elif self.algo.__name__ == "HCT" or self.algo.__name__ == "VHCT":
                     self.curr_algo = self.algo(
-                        nu=self.numax, rho=rho, domain=self.domain, partition=self.partition
+                        nu=self.numax,
+                        rho=rho,
+                        domain=self.domain,
+                        partition=self.partition,
                     )
                 # TODO: add more algorithms that do not need nu or rho
             if self.counter < self.half_phase_length:
                 point = self.curr_algo.pull(time)
                 self.goodx = point
 
             elif self.counter == self.half_phase_length:
@@ -153,8 +166,8 @@
         """
         The function to get the last point in GPO
 
         Returns
         -------
 
         """
-        return self.V_x[np.argmax(np.array(self.V_reward))]
+        return self.V_x[np.argmax(np.array(self.V_reward))]
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/HCT.py` & `PyXAB-0.2.1/PyXAB/algos/HCT.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,8 @@
 
         Returns
         -------
         chosen_point: list
             The point chosen by the algorithm
         """
 
-        return self.pull(0)
+        return self.pull(0)
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/HOO.py` & `PyXAB-0.2.1/PyXAB/algos/HOO.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -339,8 +339,8 @@
 
         Returns
         -------
         chosen_point: list
             The point chosen by the algorithm
         """
 
-        return self.pull(0)
+        return self.pull(0)
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/PCT.py` & `PyXAB-0.2.1/PyXAB/algos/PCT.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
         """
         The function to get the last point for PCT
 
         Returns
         -------
 
         """
-        return self.algorithm.get_last_point()
+        return self.algorithm.get_last_point()
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/POO.py` & `PyXAB-0.2.1/PyXAB/algos/POO.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,22 @@
         super(POO, self).__init__()
         if domain is None:
             raise ValueError("Parameter space is not given.")
         if partition is None:
             raise ValueError("Partition of the parameter space is not given.")
         if algo is None:
             raise ValueError("Algorithm for POO is not given")
-        if algo.__name__ != 'T_HOO' and algo.__name__ != 'HCT' and algo.__name__ != 'VHCT':
-            raise NotImplementedError('POO has not yet included implementations for this algorithm')
+        if (
+            algo.__name__ != "T_HOO"
+            and algo.__name__ != "HCT"
+            and algo.__name__ != "VHCT"
+        ):
+            raise NotImplementedError(
+                "POO has not yet included implementations for this algorithm"
+            )
 
         self.rounds = rounds
         self.rhomax = rhomax
         self.numax = numax
         self.Dmax = np.log(2) / np.log(1 / rhomax)  # TODO: Change this 2 to K-arm
         self.domain = domain
         self.partition = partition
@@ -85,21 +91,28 @@
             The point chosen by the POO algorithm
         """
 
         if self.N <= 0.5 * self.Dmax * np.log(self.n / np.log(self.n)):
 
             if self.counter == 0:
                 rho = self.rhomax ** (2 * self.N / (2 * self.phase + 1))
-                if self.algo.__name__ == 'T_HOO':
+                if self.algo.__name__ == "T_HOO":
                     self.curr_algo = self.algo(
-                        nu=self.numax, rho=rho, rounds=self.rounds, domain=self.domain, partition=self.partition
+                        nu=self.numax,
+                        rho=rho,
+                        rounds=self.rounds,
+                        domain=self.domain,
+                        partition=self.partition,
                     )
-                elif self.algo.__name__ == 'HCT' or self.algo.__name__ == 'VHCT':
+                elif self.algo.__name__ == "HCT" or self.algo.__name__ == "VHCT":
                     self.curr_algo = self.algo(
-                        nu=self.numax, rho=rho, domain=self.domain, partition=self.partition
+                        nu=self.numax,
+                        rho=rho,
+                        domain=self.domain,
+                        partition=self.partition,
                     )
                 # TODO: add more algorithms that do not need nu or rho
                 self.V_algo.append(self.curr_algo)
                 self.V_reward.append(0)
                 self.Times.append(0)
             point = self.V_algo[-1].pull(time)
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/SOO.py` & `PyXAB-0.2.1/PyXAB/algos/SOO.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 """Implementation of SOO (Munos, 2011)
 """
 # Author: Haoze Li <li4456@purdue.edu>
 # License: MIT
 
 
-import math 
+import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
 import pdb
 
+
 class SOO_node(P_node):
     """
     Implementation of the node in the SOO algorithm
     """
-    
+
     def __init__(self, depth, index, parent, domain):
         """
         Initialization of the SOO node
         
         Parameters
         ----------
         depth: int
@@ -28,61 +29,61 @@
             index of the node
         parent: 
             parent node of the current node
         domain: list(list)
             domain that this node represents
         """
         super(SOO_node, self).__init__(depth, index, parent, domain)
-        
+
         self.visited = False
         self.reward = -np.inf
-        
+
     def update_reward(self, reward):
         """
         The function to update the reward of the node
 
         Parameters
         ----------
         reward: float
             the reward for evaluating the node
         
         Returns
         -------
         
         """
         self.reward = reward
-        
+
     def get_reward(self):
         """
         The function to get the reward of the node
         
         Returns
         -------
 
         """
         return self.reward
-    
+
     def visit(self):
         """
         The function to visit the node
         
         Returns
         -------
         
         """
-        
+
         self.visited = True
-        
+
 
 class SOO(Algorithm):
     """
     The implementation of the SOO algorithm (Munos, 2011)
     """
-    
-    def __init__(self, n=100, h_max=100, domain=None, partition=None): 
+
+    def __init__(self, n=100, h_max=100, domain=None, partition=None):
         """
         The initialization of the SOO algorithm
         
         Parameters
         ----------
         n: int
             The total number of rounds (budget)
@@ -90,100 +91,105 @@
             The largest searching depth
         domain: list(list)
             The domain of the objective to be optimized
         partition: 
             The partition choice of the algorithm
         """
         super(SOO, self).__init__()
-        if domain is None: 
+        if domain is None:
             raise ValueError("Parameter space is not given.")
         if partition is None:
             raise ValueError("Partition of the parameter space is not given.")
         self.partition = partition(domain=domain, node=SOO_node)
-        
+
         self.iteration = 0
         self.n = n
         self.h_max = h_max
-        
+
         self.curr_node = None
-        
+
     def pull(self, time):
         """
         The pull function of SOO that returns a point in every round
 
         Parameters
         ----------
         time: int
             time stamp parameter
         
         Returns
         -------
         point: list
             the point to be evaluated
         """
-        
-        self.iteration = time 
+
+        self.iteration = time
         node_list = self.partition.get_node_list()
-        flag = False # indicate if we should terminate the iteration
-        
-        while True: 
+        flag = False  # indicate if we should terminate the iteration
+
+        while True:
             h = 0
             v_max = -np.inf
             while h <= min(self.partition.get_depth(), self.h_max):
                 max_value = -np.inf
                 max_node = None
-                for node in node_list[h]: # for all node in the layer
-                    if node.get_children() is None: # if the node is not evaluated, evaluate it 
-                        if not node.visited: 
+                for node in node_list[h]:  # for all node in the layer
+                    if (
+                        node.get_children() is None
+                    ):  # if the node is not evaluated, evaluate it
+                        if not node.visited:
                             node.visit()
                             self.curr_node = node
                             return node.get_cpoint()
-                        if node.get_reward() >= max_value: # find the leaf node with maximal reward
-                            max_value = node.get_reward() 
+                        if (
+                            node.get_reward() >= max_value
+                        ):  # find the leaf node with maximal reward
+                            max_value = node.get_reward()
                             max_node = node
                 if max_value >= v_max:
-                    if max_node is not None: # Found a leaf node
+                    if max_node is not None:  # Found a leaf node
                         self.partition.make_children(max_node, newlayer=True)
                         v_max = max_value
                 h += 1
-            if max_node is None: 
-                if flag: # We terminate the outer loop if we cannot find a leaf node that satisfies those conditions
+            if max_node is None:
+                if (
+                    flag
+                ):  # We terminate the outer loop if we cannot find a leaf node that satisfies those conditions
                     return self.partition.get_root().get_cpoint()
-                flag = True # We set flag = True iff the loop cannot find the node starting from root.
-                
+                flag = True  # We set flag = True iff the loop cannot find the node starting from root.
+
     def receive_reward(self, time, reward):
         """
         The receive_reward function of SOO to obtain the reward and update Statistics (for current node)
 
         Parameters
         ----------
         time: int
             The time stamp parameter
         reward: float
             The reward of the evaluation
         
         Returns
         -------
         """
-        
+
         self.curr_node.update_reward(reward)
-        
+
     def get_last_point(self):
         """
         The function to get the last point in SOO
 
         Returns
         -------
         point: list
             The output of the SOO algorithm at last
         """
-        
+
         max_value = -np.inf
         max_node = None
         node_list = self.partition.get_node_list()
         for h in range(len(node_list)):
             for node in node_list[h]:
                 if node.get_reward() >= max_value:
                     max_value = node.get_reward()
                     max_node = node
         return max_node.get_cpoint()
-
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/SequOOL.py` & `PyXAB-0.2.1/PyXAB/algos/SequOOL.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pdb
 
 
 class SequOOL_node(P_node):
     """
     Implementation of the SequOOL node
     """
-    
+
     def __init__(self, depth, index, parent, domain):
         """
         Initialization of the SequOOL node
         Parameters
         ----------
         depth: int
             fepth of the node
@@ -83,15 +83,15 @@
         return False if self.opened else True
 
 
 class SequOOL(Algorithm):
     """
     The implementation of the SequOOL algorithm (Barlett, 2019)
     """
-    
+
     def __init__(self, n=1000, domain=None, partition=None):
         """
         The initialization of the SequOOL algorithm
         
         Parameters
         ----------
         n: int
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/StoSOO.py` & `PyXAB-0.2.1/PyXAB/algos/StoSOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/algos/StroquOOL.py` & `PyXAB-0.2.1/PyXAB/algos/StroquOOL.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pdb
 
 
 class StroquOOL_node(P_node):
     """
     Implementation of the node in the StroquOOL algorithm
     """
-    
+
     def __init__(self, depth, index, parent, domain):
         """
         Initialization of the StroquOOL node
 
         Paramaters
         ----------
         depth: int
@@ -71,15 +71,14 @@
         
         Returns
         -------
         
         """
         if self.visited_times > 0:
             self.mean_reward = np.sum(np.array(self.rewards)) / len(self.rewards)
-            
 
     def get_mean_reward(self):
         """
         The function to get the mean of the reward list of the node
 
         Returns
         -------
@@ -118,15 +117,15 @@
         self.rewards = []
 
 
 class StroquOOL(Algorithm):
     """
     The implementation of the StroquOOL algorithm (Bartlett, 2019)
     """
-    
+
     def __init__(self, n=1000, domain=None, partition=None):
         """
         The initialization of the StroquOOL algorithm
 
         Parameters
         ----------
         n: int
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/VHCT.py` & `PyXAB-0.2.1/PyXAB/algos/VHCT.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -453,8 +453,8 @@
 
         Returns
         -------
         chosen_point: list
             The point chosen by the algorithm
         """
 
-        return self.pull(0)
+        return self.pull(0)
```

### Comparing `PyXAB-0.2.0/PyXAB/algos/VPCT.py` & `PyXAB-0.2.1/PyXAB/algos/VPCT.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -88,8 +88,8 @@
         """
         The function to get the last point of VPCT.
 
         Returns
         -------
 
         """
-        return self.algorithm.get_last_point()
+        return self.algorithm.get_last_point()
```

### Comparing `PyXAB-0.2.0/PyXAB/partition/BinaryPartition.py` & `PyXAB-0.2.1/PyXAB/partition/BinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/DimensionBinaryPartition.py` & `PyXAB-0.2.1/PyXAB/partition/DimensionBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/KaryPartition.py` & `PyXAB-0.2.1/PyXAB/partition/KaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/Node.py` & `PyXAB-0.2.1/PyXAB/partition/Node.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/Partition.py` & `PyXAB-0.2.1/PyXAB/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/RandomBinaryPartition.py` & `PyXAB-0.2.1/PyXAB/partition/RandomBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/partition/RandomKaryPartition.py` & `PyXAB-0.2.1/PyXAB/partition/RandomKaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/Ackley.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/Ackley.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/Cexample.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/Cexample.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/DifficultFunc.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/DifficultFunc.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/DoubleSine.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/DoubleSine.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/Garland.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/Garland.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/Himmelblau.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/Himmelblau.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/synthetic_obj/Rastrigin.py` & `PyXAB-0.2.1/PyXAB/synthetic_obj/Rastrigin.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/utils/plot.py` & `PyXAB-0.2.1/PyXAB/utils/plot.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/utils/run_cumulative.py` & `PyXAB-0.2.1/PyXAB/utils/run_synthetic.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB/utils/visualize_gif.py` & `PyXAB-0.2.1/PyXAB/utils/visualize_gif.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.0/PyXAB.egg-info/PKG-INFO` & `PyXAB-0.2.1/PyXAB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -120,14 +120,15 @@
         
         ### *X*-armed bandit algorithms
         
         * Algorithm starred are meta-algorithms (wrappers)
         
         | Algorithm                                                                           | Research Paper                                                                                                                                                                           | Year |
         |-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
+        | [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py)     | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf)                                                                                                              | 2008 |
         | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py)           | [*X*-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html)                                                                                                                           | 2011 |
         | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
         | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
         | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
         | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
         | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
         | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.0 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.1 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
@@ -43,31 +43,33 @@
 update if needed ``` To install via git, run the following lines of code
 ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
 . ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
 meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
 ------------------------------------------------------------------------|------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|------| | [T-HOO](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
-bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
+blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
+(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
+jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
+Deterministic Function without the Knowledge of its Smoothness](https://
+proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
+Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
 without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
-Optimization of a Deterministic Function without the Knowledge of its
-Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
-Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
-valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
-Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
-optimization of noisy functions with unknown smoothness](https://
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
+[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
+v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
+Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
+[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
+[Black-box optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.0/PyXAB.egg-info/SOURCES.txt` & `PyXAB-0.2.1/PyXAB.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 PyXAB/algos/POO.py
 PyXAB/algos/SOO.py
 PyXAB/algos/SequOOL.py
 PyXAB/algos/StoSOO.py
 PyXAB/algos/StroquOOL.py
 PyXAB/algos/VHCT.py
 PyXAB/algos/VPCT.py
+PyXAB/algos/Zooming.py
 PyXAB/algos/__init__.py
 PyXAB/partition/BinaryPartition.py
 PyXAB/partition/DimensionBinaryPartition.py
 PyXAB/partition/KaryPartition.py
 PyXAB/partition/Node.py
 PyXAB/partition/Partition.py
 PyXAB/partition/RandomBinaryPartition.py
@@ -37,9 +38,9 @@
 PyXAB/synthetic_obj/Garland.py
 PyXAB/synthetic_obj/Himmelblau.py
 PyXAB/synthetic_obj/Objective.py
 PyXAB/synthetic_obj/Rastrigin.py
 PyXAB/synthetic_obj/__init__.py
 PyXAB/utils/__init__.py
 PyXAB/utils/plot.py
-PyXAB/utils/run_cumulative.py
+PyXAB/utils/run_synthetic.py
 PyXAB/utils/visualize_gif.py
```

### Comparing `PyXAB-0.2.0/README.md` & `PyXAB-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
 ### *X*-armed bandit algorithms
 
 * Algorithm starred are meta-algorithms (wrappers)
 
 | Algorithm                                                                           | Research Paper                                                                                                                                                                           | Year |
 |-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
+| [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py)     | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf)                                                                                                              | 2008 |
 | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py)           | [*X*-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html)                                                                                                                           | 2011 |
 | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
 | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py)             | [Optimistic Optimization of a Deterministic Function without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 |
 | [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py)       | [Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/valko13.pdf)                                                                                          | 2013 |
 | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HCT.py)             | [Online Stochastic Optimization Under Correlated Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html)                                                                         | 2014 |
 | [POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py)            | [Black-box optimization of noisy functions with unknown smoothness](https://papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)                               | 2015 |
 | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/GPO.py)            | [General Parallel Optimization Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html)                                                                                      | 2019 |
```

#### html2text {}

```diff
@@ -39,31 +39,33 @@
 update if needed ``` To install via git, run the following lines of code
 ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
 . ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
 meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
 ------------------------------------------------------------------------|------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------|------| | [T-HOO](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
-bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
+blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
+(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
+jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
+Deterministic Function without the Knowledge of its Smoothness](https://
+proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
+Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
 without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
-Optimization of a Deterministic Function without the Knowledge of its
-Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
-Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
-valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
-Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
-optimization of noisy functions with unknown smoothness](https://
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
+[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
+v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
+Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
+[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
+[Black-box optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.0/setup.py` & `PyXAB-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyXAB'
 DESCRIPTION = 'PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.'
 URL = 'https://github.com/WilliamLwj/PyXAB'
 EMAIL = 'lil3549@purdue.edu'
 AUTHOR = 'Wenjie Li, Haoze Li'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy>=1.20.3',
     'matplotlib',
     # 'requests', 'maya', 'records',
 ]
```

