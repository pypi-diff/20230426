# Comparing `tmp/happy_learning-0.4.7.tar.gz` & `tmp/happy_learning-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_learning-0.4.7.tar", last modified: Sun Apr 16 01:37:40 2023, max compression
+gzip compressed data, was "happy_learning-0.4.8.tar", last modified: Wed Apr 26 21:03:42 2023, max compression
```

## Comparing `happy_learning-0.4.7.tar` & `happy_learning-0.4.8.tar`

### file list

```diff
@@ -1,60 +1,58 @@
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.444611 happy_learning-0.4.7/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.7/LICENSE
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-16 01:37:40.444962 happy_learning-0.4.7/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.7/README.md
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.350984 happy_learning-0.4.7/happy_learning/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/__init__.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/arbitrary_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    26284 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   348942 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30523 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    29154 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_tournament.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   144589 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    74567 2023-04-16 00:13:24.000000 happy_learning-0.4.7/happy_learning/neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 00:13:24.000000 happy_learning-0.4.7/happy_learning/neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/self_taught_short_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   142753 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31963 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/utils.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.399220 happy_learning-0.4.7/happy_learning.egg-info/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1814 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/SOURCES.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/dependency_links.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      339 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/requires.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/top_level.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-16 01:37:40.446380 happy_learning-0.4.7/setup.cfg
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4271 2023-04-02 01:33:01.000000 happy_learning-0.4.7/setup.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.443639 happy_learning-0.4.7/test/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4304 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    21131 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3749 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     5231 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    36338 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    17190 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3263 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1934 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_tournament.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    33868 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.7/test/test_neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.7/test/test_neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_self_taught_short_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34195 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.137548 happy_learning-0.4.8/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.8/LICENSE
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-26 21:03:42.137920 happy_learning-0.4.8/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.8/README.md
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.088538 happy_learning-0.4.8/happy_learning/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/__init__.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/arbitrary_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    26360 2023-04-16 23:16:10.000000 happy_learning-0.4.8/happy_learning/environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   350467 2023-04-24 16:52:19.000000 happy_learning-0.4.8/happy_learning/feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    47861 2023-04-26 16:11:34.000000 happy_learning-0.4.8/happy_learning/feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   137255 2023-04-25 10:59:35.000000 happy_learning-0.4.8/happy_learning/genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    74495 2023-04-16 17:16:09.000000 happy_learning-0.4.8/happy_learning/neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 17:16:33.000000 happy_learning-0.4.8/happy_learning/neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/self_taught_short_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   136214 2023-04-25 13:55:53.000000 happy_learning-0.4.8/happy_learning/swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    29520 2023-04-16 11:52:14.000000 happy_learning-0.4.8/happy_learning/text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.8/happy_learning/utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.096675 happy_learning-0.4.8/happy_learning.egg-info/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1745 2023-04-26 21:03:42.000000 happy_learning-0.4.8/happy_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      356 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/requires.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-26 21:03:41.000000 happy_learning-0.4.8/happy_learning.egg-info/top_level.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-26 21:03:42.139332 happy_learning-0.4.8/setup.cfg
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3650 2023-04-26 17:15:04.000000 happy_learning-0.4.8/setup.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-26 21:03:42.136320 happy_learning-0.4.8/test/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4869 2023-04-24 23:30:40.000000 happy_learning-0.4.8/test/test_data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    21152 2023-04-17 16:30:20.000000 happy_learning-0.4.8/test/test_deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3788 2023-04-17 00:38:08.000000 happy_learning-0.4.8/test/test_environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     5483 2023-04-17 00:42:31.000000 happy_learning-0.4.8/test/test_evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    39531 2023-04-24 17:12:05.000000 happy_learning-0.4.8/test/test_feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    17611 2023-04-17 21:02:23.000000 happy_learning-0.4.8/test/test_feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4758 2023-04-26 17:10:24.000000 happy_learning-0.4.8/test/test_feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34272 2023-04-24 23:19:19.000000 happy_learning-0.4.8/test/test_genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.8/test/test_neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.8/test/test_neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_self_taught_short_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34193 2023-04-26 17:28:30.000000 happy_learning-0.4.8/test/test_swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.8/test/test_utils.py
```

### Comparing `happy_learning-0.4.7/LICENSE` & `happy_learning-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/PKG-INFO` & `happy_learning-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_learning
-Version: 0.4.7
+Version: 0.4.8
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.7/README.md` & `happy_learning-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/arbitrary_modeling.py` & `happy_learning-0.4.8/happy_learning/arbitrary_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/chaid_decision_tree.py` & `happy_learning-0.4.8/happy_learning/chaid_decision_tree.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/data_miner.py` & `happy_learning-0.4.8/happy_learning/data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/deep_q_learning.py` & `happy_learning-0.4.8/happy_learning/deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/environment_modeling.py` & `happy_learning-0.4.8/happy_learning/environment_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,20 +346,22 @@
                                                                 )
             _state: dict = self.action_to_state(action=action)
         _model_param: dict = self._state_to_param(model_name=_model_name, state=_state)
         if self.sml_problem.find('clf') >= 0:
             _model = ModelGeneratorClf(model_name=_model_name,
                                        clf_params=_model_param.get(_model_name),
                                        models=[_model_name]
-                                       ).generate_model()
+                                       )
+            _model.generate_model()
         else:
             _model = ModelGeneratorReg(model_name=_model_name,
                                        reg_params=_model_param.get(_model_name),
                                        models=[_model_name]
-                                       ).generate_model()
+                                       )
+            _model.generate_model()
         _model.train(x=data_sets.get('x_train').values, y=data_sets.get('y_train').values)
         _pred_train: np.array = _model.predict(x=data_sets.get('x_train').values)
         _model.eval(obs=data_sets.get('y_train').values, pred=_pred_train, eval_metric=None, train_error=True)
         _pred_test: np.array = _model.predict(x=data_sets.get('x_test').values)
         _model.eval(obs=data_sets.get('y_test').values, pred=_pred_test, eval_metric=None, train_error=False)
         _ml_metric: str = SML_SCORE['ml_metric'][self.sml_problem]
         _best_score: float = SML_SCORE['ml_metric_best'][self.sml_problem]
@@ -425,20 +427,22 @@
         :return: object
             Trained model object
         """
         if self.sml_problem.find('clf') >= 0:
             _model = ModelGeneratorClf(model_name=model_name,
                                        clf_params=param,
                                        models=[model_name]
-                                       ).generate_model()
+                                       )
+            _model.generate_model()
         else:
             _model = ModelGeneratorReg(model_name=model_name,
                                        reg_params=param,
                                        models=[model_name]
-                                       ).generate_model()
+                                       )
+            _model.generate_model()
         _model.train(x=data_sets.get('x_train').values, y=data_sets.get('y_train').values)
         if eval:
             _pred_train: np.array = _model.predict(x=data_sets.get('x_train').values)
             _model.eval(obs=data_sets.get('y_train').values, pred=_pred_train, eval_metric=None, train_error=True)
             _pred_test: np.array = _model.predict(x=data_sets.get('x_test').values)
             _model.eval(obs=data_sets.get('y_test').values, pred=_pred_test, eval_metric=None, train_error=False)
             _ml_metric: str = SML_SCORE['ml_metric'][self.sml_problem]
```

### Comparing `happy_learning-0.4.7/happy_learning/evaluate_machine_learning.py` & `happy_learning-0.4.8/happy_learning/evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/feature_engineer.py` & `happy_learning-0.4.8/happy_learning/feature_engineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,19 @@
 
     :param imp_value: float
         Single imputation value
 
     :param convert_to_float32: bool
         Convert continuous features types as float64 to float32 for compatibility reasons
     """
+    DATA_PROCESSING['df'][features] = DATA_PROCESSING['df'][features].replace(to_replace=INVALID_VALUES,
+                                                                              value=np.nan,
+                                                                              regex=False
+                                                                              )
     if MissingDataAnalysis(df=DATA_PROCESSING['df']).has_nan():
-        DATA_PROCESSING['df'][features] = DATA_PROCESSING['df'][features].replace(to_replace=INVALID_VALUES, value=np.nan, regex=False)
         DATA_PROCESSING['df'][features] = DATA_PROCESSING['df'][features].fillna(value=imp_value, axis=0)
     if convert_to_float32:
         if len(features) == 1:
             DATA_PROCESSING['df'][features[0]] = DATA_PROCESSING['df'][features[0]].astype(np.float32)
         else:
             DATA_PROCESSING['df'][features] = DATA_PROCESSING['df'][features].astype(np.float32)
     _inv_features: List[str] = EasyExploreUtils().get_invariant_features(df=DATA_PROCESSING.get('df')[features])
@@ -353,14 +356,25 @@
                                                       cloud=CLOUD,
                                                       bucket_name=_bucket_name
                                                       ).file()
         if feature in FEATURE_TYPES.get('date'):
             DATA_PROCESSING['df'][feature] = pd.to_datetime(DATA_PROCESSING['df'][feature])
 
 
+def _name_convention(feature: str):
+    """
+    Rename feature based on naming convention
+
+    :param feature: str
+        Name of the feature
+    """
+    if feature.find('.') >= 0:
+        return feature.split('.')[0]
+    return feature
+
 def _process_handler(action: str,
                      feature: str,
                      new_feature: str,
                      process: str,
                      meth: str,
                      param: dict,
                      data: np.array = None,
@@ -1033,14 +1047,15 @@
                  activate_actor: bool = False,
                  critic_config: dict = None,
                  missing_value_analysis: bool = True,
                  auto_cleaning: bool = False,
                  auto_typing: bool = True,
                  auto_engineering: bool = False,
                  auto_text_mining: bool = True,
+                 name_convention: bool = True,
                  file_path: str = None,
                  sep: str = ',',
                  print_msg: bool = True,
                  n_cpu_cores: int = -1,
                  seed: int = 1234,
                  partitions: int = 4,
                  cloud: str = None,
@@ -1103,14 +1118,17 @@
 
         :param auto_typing: bool
             Re-type features automatically if necessary
 
         :param auto_text_mining: bool
             Classify and interpret text data analytically for generating numerical features from text
 
+        :param name_convention: bool
+            Apply naming convention for features
+
         :param file_path: str
             Path of local file to import as data set
 
         :param sep: str
             Separator of data file
 
         :param print_msg: bool
@@ -1220,33 +1238,44 @@
             if df is None:
                 if file_path is None:
                     raise FeatureEngineerException('Neither data object nor file path to data file found')
                 if len(file_path) == 0:
                     raise FeatureEngineerException('Neither data object nor file path to data file found')
                 self._data_import(file_path=file_path, sep=sep, **kwargs)
                 for feature in DATA_PROCESSING['df'].columns:
-                    _save_temp_files(feature=feature, new_name=_force_rename_feature(feature=feature, max_length=100))
+                    if name_convention:
+                        _feature: str = _name_convention(feature=feature)
+                        DATA_PROCESSING['df'].rename(columns={feature: _feature})
+                    else:
+                        _feature: str = feature
+                    _save_temp_files(feature=_feature, new_name=_force_rename_feature(feature=_feature, max_length=100))
+                DATA_PROCESSING['n_cases'] = DATA_PROCESSING['df'].shape[0].compute()
                 DATA_PROCESSING['df'] = None
             else:
                 if isinstance(df, pd.DataFrame):
                     DATA_PROCESSING['df'] = dd.from_pandas(data=df, npartitions=DATA_PROCESSING['cpu_cores'])
                 DATA_PROCESSING['processing']['features']['raw'].update({_force_rename_feature(feature=feature, max_length=100): [] for feature in DATA_PROCESSING.get('df').columns})
                 Log(write=not DATA_PROCESSING.get('show_msg')).log(msg='Data set loaded from given object\nCases: {}\nFeatures: {}'.format(len(DATA_PROCESSING['df']),
                                                                                                                                            len(DATA_PROCESSING['df'].columns)
                                                                                                                                            )
                                                                    )
-                DATA_PROCESSING['n_cases'] = len(DATA_PROCESSING['df'])
+                DATA_PROCESSING['n_cases'] = DATA_PROCESSING['df'].shape[0].compute()
                 global TEMP_INDEXER
                 TEMP_INDEXER['__index__'] = [i for i in range(0, DATA_PROCESSING['n_cases'], 1)]
                 for ignore in IGNORE_FEATURES:
                     if ignore in list(DATA_PROCESSING['df'].columns):
                         del DATA_PROCESSING['df'][ignore]
                 DATA_PROCESSING.update({'original_features': DATA_PROCESSING.get('df').columns.tolist()})
                 for feature in DATA_PROCESSING.get('df').columns:
-                    _save_temp_files(feature=feature, new_name=_force_rename_feature(feature=feature, max_length=100))
+                    if name_convention:
+                        _feature: str = _name_convention(feature=feature)
+                        DATA_PROCESSING['df'].rename(columns={feature: _feature})
+                    else:
+                        _feature: str = feature
+                    _save_temp_files(feature=_feature, new_name=_force_rename_feature(feature=_feature, max_length=100))
                 DATA_PROCESSING['df'] = None
                 Log(write=not print_msg, level='info', env='dev').log(msg='Feature files saved in {}'.format(TEMP_DIR))
         else:
             _init: bool = False
             self.load(file_path=feature_engineer_file_path)
         if _init:
             DATA_PROCESSING['pre_defined_feature_types'] = {}
@@ -1421,15 +1450,15 @@
                                              as_data_frame=True,
                                              use_dask=True,
                                              create_dir=False,
                                              sep=sep,
                                              cloud=CLOUD,
                                              bucket_name=_bucket_name,
                                              **kwargs
-                                             )
+                                             ).file()
         DATA_PROCESSING['processing']['features']['raw'].update({_force_rename_feature(feature=feature, max_length=100): [] for feature in DATA_PROCESSING.get('df').columns})
         Log(write=not DATA_PROCESSING.get('show_msg')).log(
             msg='Data set loaded from file\nCases: {}\nFeatures: {}'.format(len(DATA_PROCESSING['df']),
                                                                             len(DATA_PROCESSING['df'].columns)
                                                                             )
             )
         DATA_PROCESSING['n_cases'] = len(DATA_PROCESSING['df'])
@@ -2079,17 +2108,17 @@
             self.scaling_robust()
             self.scaling_minmax()
             self.normalizer(norm_meth='l2' if kwargs.get('norm_meth') is None else kwargs.get('norm_meth'))
             self.standardizer(with_mean=True if kwargs.get('with_mean') is None else kwargs.get('with_mean'),
                               with_std=True if kwargs.get('with_std') is None else kwargs.get('with_std')
                               )
         if log_transform:
-            self.log_transform(skewness_test=False)
+            self.log_transform(skewed_only=False)
         if exp_transform:
-            self.exp_transform(skewness_test=False)
+            self.exp_transform(skewed_only=False)
         if disparity:
             self.interaction(addition=True if kwargs.get('addition') is None else kwargs.get('addition'),
                              subtraction=True if kwargs.get('subtraction') is None else kwargs.get('subtraction'),
                              multiplication=True if kwargs.get('multiplication') is None else kwargs.get('multiplication'),
                              division=True if kwargs.get('division') is None else kwargs.get('division')
                              )
         if geo_features is not None:
@@ -2574,24 +2603,26 @@
         """
         Export data set
 
         :param file_path: str
             Complete file path of data set
 
         :param create_dir: bool
-            Create directories if they do not exists
+            Create directories if they do not exist
 
         :param overwrite: bool
             Overwrite file with same name or not
         """
         _load_temp_files(features=ALL_FEATURES)
         if CLOUD is None:
             _bucket_name: str = None
         else:
             _bucket_name: str = file_path.split("//")[1].split("/")[0]
+        if file_path.find('.parquet') >= 0:
+            DATA_PROCESSING['df'] = dd.from_pandas(data=DATA_PROCESSING.get('df'), npartitions=4)
         DataExporter(obj=DATA_PROCESSING.get('df'),
                      file_path=file_path,
                      create_dir=create_dir,
                      overwrite=overwrite,
                      cloud=CLOUD,
                      bucket=_bucket_name
                      ).file()
@@ -3443,15 +3474,15 @@
         _load_temp_files(features=_features)
         if set(list(DATA_PROCESSING['df'].columns)).difference(list(DATA_PROCESSING['correlation']['high'].keys())):
             if len(FEATURE_TYPES.get('continuous')) > 1:
                 _df: dd.DataFrame = DATA_PROCESSING.get('df')[FEATURE_TYPES.get('continuous')]
                 for feature in _df.columns:
                     if str(_df[feature].dtype).find('float') < 0:
                         _df[feature] = _df[feature].astype(float)
-                DATA_PROCESSING['correlation']['matrix'] = _df.corr(method=meth, min_periods=None, split_every=False)
+                DATA_PROCESSING['correlation']['matrix'] = _df.corr(method=meth, min_periods=None)
                 #for score in DATA_PROCESSING['correlation']['matrix']:
                 #    pass
         del _df
         return DATA_PROCESSING.get('correlation')
 
     @staticmethod
     def get_features(feature_type: str = None) -> List[str]:
@@ -3500,19 +3531,16 @@
 
         :param unique: bool
             Whether to get unique or all feature values
 
         :return np.ndarray:
             Feature values
         """
-        _features: List[str] = []
-        for ft in FEATURE_TYPES.keys():
-            for feature in FEATURE_TYPES.get(ft):
-                _features.append(feature)
-        if feature in _features:
+        if feature in ALL_FEATURES:
+            _load_temp_files(features=[feature])
             if unique:
                 return DATA_PROCESSING['df'][feature].unique()
             else:
                 return DATA_PROCESSING['df'][feature].values
         return np.ndarray(shape=[0, 0])
 
     @staticmethod
@@ -3631,15 +3659,15 @@
     def get_n_features() -> int:
         """
         Get total number of features in data set
 
         :return: int
             Total number of features
         """
-        return DATA_PROCESSING['n_features']
+        return len(ALL_FEATURES)
 
     @staticmethod
     def get_n_predictors() -> int:
         """
         Get number of predictors
 
         :return List[str]:
@@ -4047,14 +4075,15 @@
                                        )
         else:
             raise FeatureEngineerException('Not enough features ({})'.format(features))
         _data: pd.DataFrame = DATA_PROCESSING['df'][features].fillna(sys.float_info.max).values
         _poly.fit(X=_data)
         _polynomial_features = _poly.transform(X=_data)
         _name_mapper: dict = dict(original={}, interaction={})
+        _interaction_name_mapper: dict = {}
         _new_feature_names: Dict[str, str] = {}
         for i, name in enumerate(_poly.get_feature_names()):
             if i < len(features):
                 _name_mapper['original'].update({name: features[i]})
             else:
                 if name.find(' ') >= 0:
                     _feature_name: str = copy.deepcopy(name)
@@ -4063,27 +4092,30 @@
                     for n in _name_mapper['original'].keys():
                         if name.find(n) >= 0:
                             _feature_match += 1
                             _feature_name = _feature_name.replace(n, _name_mapper['original'].get(n))
                             _interaction.append(_name_mapper['original'].get(n))
                         if _feature_match == _degree:
                             _feature_name = _feature_name.replace(' ', '__')
-                            _name_mapper['interaction'].update({_feature_name: _interaction})
+                            _interaction_name_mapper.update({_feature_name: _interaction})
                             _interaction = []
                             break
                     _new_feature_names.update({name: _feature_name})
                 else:
                     for n in _name_mapper['original'].keys():
                         if name.find(n) >= 0:
-                            _name_mapper['interaction'].update({name: [_name_mapper['original'].get(n)]})
+                            _interaction_name_mapper.update({name: [_name_mapper['original'].get(n)]})
                             _new_feature_names.update({name: name.replace(n, _name_mapper['original'].get(n))})
                             break
-        for feature, poly_feature in zip(features, _name_mapper['original']):
-            for interaction in _name_mapper['interaction'].keys():
-                _name_mapper['interaction'][interaction.replace(poly_feature, feature)] = _name_mapper['interaction'].pop(interaction)
+        for interaction in _interaction_name_mapper.keys():
+            if interaction.find('x') >= 0 and interaction.find('^') > 0:
+                _poly_name: str = interaction.split('^')[0]
+                _name_mapper['interaction'].update({interaction.replace(_poly_name, _name_mapper['original'][_poly_name]): _interaction_name_mapper[interaction]})
+            else:
+                _name_mapper['interaction'].update({interaction: _interaction_name_mapper[interaction]})
         _df: pd.DataFrame = pd.DataFrame(data=_polynomial_features, columns=_poly.get_feature_names())
         _df = _df.drop(columns=list(_name_mapper['original'].keys()), axis=1)
         _df = _df.rename(columns=_new_feature_names)
         _process_handler(action='add',
                          feature='',
                          new_feature='',
                          process='interaction|polynomial',
@@ -4307,15 +4339,15 @@
                     if encoder is None:
                         _values: dict = {label: i for i, label in enumerate(_unique_values)}
                     else:
                         _values: dict = encoder['encoder']['label'][feature]['val']
                     _data: pd.DataFrame = DATA_PROCESSING['df'][feature].replace(_values)
                     _process_handler(action='add',
                                      feature=feature,
-                                     new_feature=feature,
+                                     new_feature=f'{feature}_label_enc',
                                      process='encoder|label',
                                      meth='label_encoder',
                                      param=dict(encode=encode),
                                      data=_data,
                                      force_type='categorical',
                                      obj=dict(label=_unique_values, val=_values)
                                      )
@@ -4923,15 +4955,15 @@
                                                             sparse=False,
                                                             drop_first=False,
                                                             dtype=np.int64
                                                             )
                     _dummies = _dummies.loc[:, ~_dummies.columns.duplicated()]
                     _new_names: dict = {}
                     for dummy in _dummies.columns:
-                        _new_feature: str = _avoid_overwriting(feature=dummy)
+                        _new_feature: str = _avoid_overwriting(feature=_name_convention(feature=dummy))
                         if dummy != _new_feature:
                             _new_names.update({dummy: _new_feature})
                     if len(_new_names) > 0:
                         _dummies = _dummies.rename(columns=_new_names)
                     DATA_PROCESSING['df'] = pd.concat(objs=[DATA_PROCESSING.get('df'), _dummies], axis=1)
                     _process_handler(action='add',
                                      feature=feature,
```

### Comparing `happy_learning-0.4.7/happy_learning/feature_learning.py` & `happy_learning-0.4.8/happy_learning/feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/feature_selector.py` & `happy_learning-0.4.8/happy_learning/feature_selector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,116 @@
 """
 
 Feature selection of structured (tabular) features
 
 """
 
 import copy
-import dask.dataframe as dd
+import numpy as np
 import mlflow
 import os
 import pandas as pd
+import random
 import warnings
 
-from .feature_tournament import FeatureTournament
+from .evaluate_machine_learning import sml_fitness_score
+from .genetic_algorithm import GeneticAlgorithm
 from .sampler import MLSampler
 from .supervised_machine_learning import ModelGeneratorClf, ModelGeneratorReg
+from .swarm_intelligence import SwarmIntelligence
 from .utils import HappyLearningUtils
 from easyexplore.data_visualizer import DataVisualizer
 from easyexplore.utils import Log
-from sklearn.feature_selection import SelectFromModel
-from typing import Dict, List, Union
+from multiprocessing.pool import ThreadPool
+from typing import Dict, List
 
 warnings.filterwarnings('ignore', category=DeprecationWarning)
 warnings.filterwarnings('ignore', category=FutureWarning)
 warnings.filterwarnings('ignore', category=UserWarning)
 warnings.filterwarnings('ignore', category=RuntimeWarning)
 
 
 class FeatureSelectorException(Exception):
     """
-    Class for setting up exception for class FeatureSelection
+    CLass for handling exceptions for class FeatureSelector
     """
     pass
 
 
 class FeatureSelector:
     """
-    Class for analyzing the importance of each feature in the data set
+    Class for calculating shapley values (shapley additive explanations) for feature importance evaluation and feature selection
     """
     def __init__(self,
-                 df: Union[dd.DataFrame, pd.DataFrame],
+                 df: pd.DataFrame,
+                 features: List[str],
                  target: str,
-                 features: List[str] = None,
                  force_target_type: str = None,
+                 model_name: str = 'cat',
+                 init_pairs: int = 3,
+                 init_games: int = 5,
+                 increasing_pair_size_factor: float = 0.5,
+                 games: int = 3,
+                 penalty_factor: float = 0.1,
+                 max_iter: int = 50,
+                 max_players: int = -1,
+                 evolutionary_algorithm: str = 'ga',
+                 use_standard_params: bool = True,
                  aggregate_feature_imp: Dict[str, dict] = None,
                  visualize_all_scores: bool = True,
                  visualize_variant_scores: bool = True,
                  visualize_core_feature_scores: bool = True,
-                 mlflow_log: bool = True,
                  path: str = None,
+                 mlflow_log: bool = True,
+                 multi_threading: bool = False,
                  **kwargs
                  ):
         """
-        :param df: pd.DataFrame
+        :param df: Pandas or dask DataFrame
             Data set
 
+        :param features: List[str]
+            Names of the predictor features
+
         :param target: str
-            Name of the target variable
+            Name of the target feature
 
-        :param features: List[str]
-            Name of the features
+        :param force_target_type: str
+            Force specific target type
+                -> clf_multi: Multi-Classification
+                -> reg: Regression
+
+        :param model_name: str
+            Name of the model
+
+        :param init_pairs: int
+            Number of players in each starting game of the tournament
+
+        :param init_games: int
+            Number of penalty games to qualify players for the tournament
+
+        :param increasing_pair_size_factor: float
+            Factor for increasing amount of player in each game in each step
+
+        :param games: int
+            Number of games to play in each step of the tournament
+
+        :param penalty_factor: float
+            Amount of players to exclude from the tournament because of their poor contribution capabilities
+
+        :param max_iter: int
+            Maximum number of steps of the tournament
+
+        :param max_players: int
+            Maximum number of features used for training machine learning model
+
+        :param evolutionary_algorithm: str
+            Name of the reinforced evolutionary algorithm
+                -> ga: Genetic Algorithm
+                -> si: Swarm Intelligence
 
         :param aggregate_feature_imp: Dict[str, dict]
             Name of the aggregation method and the feature names to aggregate
                 -> core: Aggregate feature importance score by each core (original) feature
                 -> level: Aggregate feature importance score by the processing level of each feature
 
         :param visualize_all_scores: bool
@@ -70,51 +118,73 @@
 
         :param visualize_variant_scores: bool
             Whether to visualize all variants of feature processing importance scores separately or not
 
         :param visualize_core_feature_scores: bool
             Whether to visualize summarized core feature importance scores or not
 
+        :param path: str
+            Path or directory to export visualization to
+
         :param mlflow_log: bool
             Track experiment results using mlflow
 
-        :param path: str
-            Path or directory to export visualization to
+        :param multi_threading: bool
+            Whether to run each game multi- or single-threaded during each iteration
 
         :param kwargs: dict
             Key-word arguments
         """
-        self.seed: int = 1234
-        self.cpu_cores: int = os.cpu_count() - 1 if os.cpu_count() > 1 else os.cpu_count()
-        if isinstance(df, pd.DataFrame):
-            self.df: dd.DataFrame = dd.from_pandas(data=df, npartitions=4 if kwargs.get('partitions') is None else kwargs.get('partitions'))
-        elif isinstance(df, dd.DataFrame):
-            self.df: dd.DataFrame = df
-        else:
-            raise FeatureSelectorException('Format of data set ({}) not supported. Use Pandas or dask DataFrame instead'.format(type(df)))
+        self.df: pd.DataFrame = df
         self.target: str = target
-        self.imp_score: Dict[str, float] = {}
-        self.aggregate_feature_imp: Dict[str, dict] = aggregate_feature_imp
-        self.features: List[str] = list(self.df.columns) if features is None else features
+        self.features: List[str] = features
         if self.target in self.features:
             del self.features[self.features.index(self.target)]
+        self.df = self.df[self.features + [self.target]]
+        self.n_cases: int = self.df.shape[0]
+        self.n_features: int = len(self.features)
         self.force_target_type: str = force_target_type
         if self.force_target_type is None:
             self.ml_type: str = HappyLearningUtils().get_ml_type(values=self.df[self.target].values) if kwargs.get('ml_type') is None else kwargs.get('ml_type')
         else:
             self.ml_type: str = self.force_target_type
         _stratify: bool = False
         if self.ml_type == 'reg':
             self.ml_metric: str = 'rmse_norm'
         elif self.ml_type == 'clf_binary':
             self.ml_metric: str = 'roc_auc'
             _stratify = True if kwargs.get('stratification') is None else kwargs.get('stratification')
         elif self.ml_type == 'clf_multi':
             self.ml_metric: str = 'cohen_kappa'
             _stratify = False if kwargs.get('stratification') is None else kwargs.get('stratification')
+        self.train_test: dict = MLSampler(df=self.df,
+                                          target=self.target,
+                                          features=self.features,
+                                          train_size=0.8 if kwargs.get('train_size') is None else kwargs.get('train_size'),
+                                          random_sample=True if kwargs.get('random') is None else kwargs.get('random'),
+                                          stratification=_stratify
+                                          ).train_test_sampling(validation_split=0 if kwargs.get('validation_size') is None else kwargs.get('validation_size'))
+        self.init_pairs: int = init_pairs
+        self.init_games: int = init_games
+        self.pair_size_factor: float = increasing_pair_size_factor
+        self.game: int = 0
+        self.games: int = games
+        self.penalty_factor: float = penalty_factor
+        self.max_iter: int = max_iter
+        self.max_players: int = max_players if max_players > 1 else len(self.features)
+        self.pairs: List[np.array] = []
+        self.threads: dict = {}
+        self.multi_threading: bool = multi_threading
+        self.tournament: bool = False
+        self.shapley_additive_explanation: dict = dict(sum={}, game={}, tournament={})
+        self.model_name: str = model_name
+        self.evolutionary_algorithm: str = evolutionary_algorithm
+        self.imp_score: Dict[str, float] = {}
+        self.use_standard_params: bool = use_standard_params
+        self.aggregate_feature_imp: Dict[str, dict] = aggregate_feature_imp
         self.visualize_all_scores: bool = visualize_all_scores
         self.visualize_variant_scores: bool = visualize_variant_scores
         self.visualize_core_features_scores: bool = visualize_core_feature_scores
         self.path: str = path
         if self.path is not None:
             self.path = self.path.replace('\\', '/')
             if os.path.isfile(self.path):
@@ -126,29 +196,184 @@
         if self.mlflow_log:
             self.mlflow_client: mlflow.tracking.MlflowClient = mlflow.tracking.MlflowClient(tracking_uri=kwargs.get('tracking_uri'),
                                                                                             registry_uri=kwargs.get('registry_uri')
                                                                                             )
         else:
             self.mlflow_client = None
         self.kwargs: dict = kwargs
-        self.init_pairs: int = self.kwargs.get('init_pairs')
-        self.init_games: int = self.kwargs.get('init_games')
-        self.increasing_pair_size_factor: float = self.kwargs.get('increasing_pair_size_factor')
-        self.games: int = self.kwargs.get('games')
-        self.penalty_factor: float = self.kwargs.get('penalty_factor')
-        self.evolutionary_algorithm: str = self.kwargs.get('evolutionary_algorithm')
-        self.max_iter = self.kwargs.get('max_iter')
-        self.max_players: int = self.kwargs.get('max_players')
-        self.kwargs.pop('init_pairs', None)
-        self.kwargs.pop('init_games', None)
-        self.kwargs.pop('increasing_pair_size_factor', None)
-        self.kwargs.pop('games', None)
-        self.kwargs.pop('evolutionary_algorithm', None)
-        self.kwargs.pop('max_iter', None)
-        self.kwargs.pop('max_players', None)
+        if self.use_standard_params:
+            if self.ml_type == 'reg':
+                _model_param: dict = ModelGeneratorReg(models=[self.model_name]).get_model_parameter()
+            else:
+                _model_param: dict = ModelGeneratorClf(models=[self.model_name]).get_model_parameter()
+            self.feature_tournament_ai: dict = dict(model_name=self.model_name,
+                                                    param=_model_param
+                                                    )
+        else:
+            if self.kwargs.get('model_param') is None:
+                self.feature_tournament_ai: dict = {}
+                self._evolve_feature_tournament_ai()
+                if self.target in self.features:
+                    del self.features[self.features.index(self.target)]
+            else:
+                _model_name: str = list(self.kwargs.get('model_param').keys())[0]
+                self.feature_tournament_ai: dict = dict(model_name=_model_name,
+                                                        param=self.kwargs.get('model_param')[_model_name]
+                                                        )
+
+    def _evolve_feature_tournament_ai(self):
+        """
+        Evolve machine learning model using evolutionary algorithm
+        """
+        Log(write=False, level='info').log(msg='Evolve feature tournament ai ...')
+        if self.evolutionary_algorithm == 'ga':
+            _feature_tournament_ai_learning: GeneticAlgorithm = GeneticAlgorithm(mode='model',
+                                                                                 df=self.df,
+                                                                                 target=self.target,
+                                                                                 features=self.features,
+                                                                                 re_split_data=False if self.kwargs.get('re_split_data') is None else self.kwargs.get('re_split_data'),
+                                                                                 re_sample_cases=False if self.kwargs.get('re_sample_cases') is None else self.kwargs.get('re_sample_cases'),
+                                                                                 re_sample_features=True,
+                                                                                 max_features=self.n_features,
+                                                                                 labels=self.kwargs.get('labels'),
+                                                                                 models=[self.model_name],
+                                                                                 model_params=None,
+                                                                                 burn_in_generations=-1 if self.kwargs.get('burn_in_generations') is None else self.kwargs.get('burn_in_generations'),
+                                                                                 warm_start=True if self.kwargs.get('warm_start') is None else self.kwargs.get('warm_start'),
+                                                                                 max_generations=2 if self.kwargs.get('max_generations_ai') is None else self.kwargs.get('max_generations_ai'),
+                                                                                 pop_size=64 if self.kwargs.get('pop_size') is None else self.kwargs.get('pop_size'),
+                                                                                 mutation_rate=0.1 if self.kwargs.get('mutation_rate') is None else self.kwargs.get('mutation_rate'),
+                                                                                 mutation_prob=0.5 if self.kwargs.get('mutation_prob') is None else self.kwargs.get('mutation_prob'),
+                                                                                 parents_ratio=0.5 if self.kwargs.get('parents_ratio') is None else self.kwargs.get('parents_ratio'),
+                                                                                 early_stopping=0 if self.kwargs.get('early_stopping') is None else self.kwargs.get('early_stopping'),
+                                                                                 convergence=False if self.kwargs.get('convergence') is None else self.kwargs.get('convergence'),
+                                                                                 timer_in_seconds=10000 if self.kwargs.get('timer_in_secondes') is None else self.kwargs.get('timer_in_secondes'),
+                                                                                 force_target_type=self.force_target_type,
+                                                                                 plot=False if self.kwargs.get('plot') is None else self.kwargs.get('plot'),
+                                                                                 output_file_path=self.kwargs.get('output_file_path'),
+                                                                                 multi_threading=False if self.kwargs.get('multi_threading') is None else self.kwargs.get('multi_threading'),
+                                                                                 multi_processing=False if self.kwargs.get('multi_processing') is None else self.kwargs.get('multi_processing'),
+                                                                                 log=False if self.kwargs.get('log') is None else self.kwargs.get('log'),
+                                                                                 verbose=False if self.kwargs.get('verbose') is None else self.kwargs.get('verbose'),
+                                                                                 mlflow_log=False if self.kwargs.get('mlflow_log_evolutionary') is None else self.kwargs.get('mlflow_log_evolutionary')
+                                                                                 )
+        elif self.evolutionary_algorithm == 'si':
+            _feature_tournament_ai_learning: SwarmIntelligence = SwarmIntelligence(mode='model',
+                                                                                   df=self.df,
+                                                                                   target=self.target,
+                                                                                   features=self.features,
+                                                                                   re_split_data=False if self.kwargs.get('re_split_data') is None else self.kwargs.get('re_split_data'),
+                                                                                   re_sample_cases=False if self.kwargs.get('re_sample_cases') is None else self.kwargs.get('re_sample_cases'),
+                                                                                   re_sample_features=True,
+                                                                                   max_features=self.n_features,
+                                                                                   labels=self.kwargs.get('labels'),
+                                                                                   models=[self.model_name],
+                                                                                   model_params=None,
+                                                                                   burn_in_adjustments=-1 if self.kwargs.get('burn_in_adjustments') is None else self.kwargs.get('burn_in_adjustments'),
+                                                                                   warm_start=True if self.kwargs.get('warm_start') is None else self.kwargs.get('warm_start'),
+                                                                                   max_adjustments=2 if self.kwargs.get('max_adjustments_ai') is None else self.kwargs.get('max_adjustments_ai'),
+                                                                                   pop_size=64 if self.kwargs.get('pop_size') is None else self.kwargs.get('pop_size'),
+                                                                                   adjustment_rate=0.1 if self.kwargs.get('adjustment_rate') is None else self.kwargs.get('adjustment_rate'),
+                                                                                   adjustment_prob=0.5 if self.kwargs.get('adjustment_prob') is None else self.kwargs.get('adjustment_prob'),
+                                                                                   early_stopping=0 if self.kwargs.get('early_stopping') is None else self.kwargs.get('early_stopping'),
+                                                                                   convergence=False if self.kwargs.get('convergence') is None else self.kwargs.get('convergence'),
+                                                                                   timer_in_seconds=10000 if self.kwargs.get('timer_in_secondes') is None else self.kwargs.get('timer_in_secondes'),
+                                                                                   force_target_type=self.force_target_type,
+                                                                                   plot=False if self.kwargs.get('plot') is None else self.kwargs.get('plot'),
+                                                                                   output_file_path=self.kwargs.get('output_file_path'),
+                                                                                   multi_threading=False if self.kwargs.get('multi_threading') is None else self.kwargs.get('multi_threading'),
+                                                                                   multi_processing=False if self.kwargs.get('multi_processing') is None else self.kwargs.get('multi_processing'),
+                                                                                   log=False if self.kwargs.get('log') is None else self.kwargs.get('log'),
+                                                                                   verbose=False if self.kwargs.get('verbose') is None else self.kwargs.get('verbose'),
+                                                                                   mlflow_log=False if self.kwargs.get('mlflow_log_evolutionary') is None else self.kwargs.get('mlflow_log_evolutionary')
+                                                                                   )
+        else:
+            raise FeatureSelectorException('Reinforced evolutionary algorithm ({}) not supported'.format(self.evolutionary_algorithm))
+        _feature_tournament_ai_learning.optimize()
+        self.feature_tournament_ai = _feature_tournament_ai_learning.evolution
+        Log(write=False, level='info').log(msg='Feature tournament ai evolved -> {}'.format(self.feature_tournament_ai.get('model_name')))
+
+    def _game(self, iteration: int):
+        """
+        Play tournament game
+
+        :param iteration: int
+            Number of current iteration
+        """
+        for pair in self.pairs:
+            if self.ml_type == 'reg':
+                _game: ModelGeneratorReg = ModelGeneratorReg(model_name=self.feature_tournament_ai.get('model_name'),
+                                                             reg_params=self.feature_tournament_ai.get('param')
+                                                             )
+                _game.generate_model()
+                _game.train(x=self.train_test.get('x_train')[pair].values,
+                            y=self.train_test.get('y_train').values,
+                            #validation=dict(x_val=self.train_test.get('x_val')[pair].values,
+                            #                y_val=self.train_test.get('y_val').values
+                            #                )
+                            )
+                _pred = _game.predict(x=self.train_test.get('x_test')[pair].values)
+                _game.eval(obs=self.train_test.get('y_test').values, pred=_pred, train_error=False)
+                _game_score: float = sml_fitness_score(ml_metric=tuple([0, _game.fitness['test'].get(self.ml_metric)]),
+                                                       train_test_metric=tuple([_game.fitness['train'].get(self.ml_metric), _game.fitness['test'].get(self.ml_metric)]),
+                                                       train_time_in_seconds=_game.train_time,
+                                                       capping_to_zero=True
+                                                       )
+            else:
+                _game: ModelGeneratorClf = ModelGeneratorClf(model_name=self.feature_tournament_ai.get('model_name'),
+                                                             clf_params=self.feature_tournament_ai.get('param')
+                                                             )
+                _game.generate_model()
+                _game.train(x=self.train_test.get('x_train')[pair].values,
+                            y=self.train_test.get('y_train').values,
+                            #validation=dict(x_val=self.train_test.get('x_val')[pair].values,
+                            #                y_val=self.train_test.get('y_val').values
+                            #                )
+                            )
+                _pred = _game.predict(x=self.train_test.get('x_test')[pair].values, probability=False)
+                _game.eval(obs=self.train_test.get('y_test').values, pred=_pred, train_error=False)
+                _game_score: float = sml_fitness_score(ml_metric=tuple([1, _game.fitness['test'].get(self.ml_metric)]),
+                                                       train_test_metric=tuple([_game.fitness['train'].get(self.ml_metric), _game.fitness['test'].get(self.ml_metric)]),
+                                                       train_time_in_seconds=_game.train_time,
+                                                       capping_to_zero=True
+                                                       )
+            for j, imp in enumerate(_game.model.feature_importances_):
+                _shapley_value: float = imp * _game_score
+                if _shapley_value != _shapley_value:
+                    _shapley_value = 0.0
+                if pair[j] in self.shapley_additive_explanation['sum'].keys():
+                    self.shapley_additive_explanation['sum'][pair[j]] += _shapley_value
+                else:
+                    self.shapley_additive_explanation['sum'].update({pair[j]: _shapley_value})
+                if iteration >= self.init_games:
+                    if pair[j] in self.shapley_additive_explanation['game'].keys():
+                        self.shapley_additive_explanation['game'][pair[j]].append(_shapley_value)
+                    else:
+                        self.shapley_additive_explanation['game'].update({pair[j]: [_shapley_value]})
+            if self.mlflow_log:
+                with mlflow.start_run():
+                    for j, imp in enumerate(_game.model.feature_importances_):
+                        _shapley_value: float = imp * _game_score
+                        mlflow.log_metric(key='sml_score', value=_game_score, step=None)
+                        for metric_context in _game.fitness:
+                            for metric in _game.fitness[metric_context]:
+                                mlflow.log_metric(key=f'{metric}_{metric_context}',
+                                                  value=_game.fitness[metric_context][metric]
+                                                  )
+                        _tags: dict = dict(model_name=self.feature_tournament_ai.get('model_name'),
+                                           target_type=self.ml_type,
+                                           game=self.game,
+                                           iteration=iteration,
+                                           init_game=True if iteration < self.init_games else False,
+                                           tree_importance=imp,
+                                           shapley_value=_shapley_value
+                                           )
+                        mlflow.set_tags(tags=_tags)
+                        for k, feature in enumerate(pair):
+                            mlflow.set_tag(key=f'feature_{k}', value=feature)
 
     @staticmethod
     def _mlflow_tracking(stats: Dict[str, pd.DataFrame], file_paths: List[str]):
         """
         Track model performance using mlflow
         """
         for i, stat in enumerate(stats.keys()):
@@ -161,253 +386,201 @@
             with mlflow.start_run():
                 try:
                     _file_name: str = file_paths[i].split('/')[-1].replace('.html', '')
                     mlflow.log_artifact(local_path=file_paths[i], artifact_path=_file_name)
                 except (FileNotFoundError, IndexError):
                     pass
 
-    def eval_redundancy(self,
-                        sorted_features: List[str],
-                        model: str = 'cat',
-                        redundant_threshold: float = 0.01
-                        ) -> dict:
+    def _permutation(self, n: int):
         """
-        Evaluate redundancy of features
-
-        :param sorted_features: List[str]
-            Features sorted by relative importance score
-
-        :param model: str
-            Name of the model
+        Permute combination of players
 
-        :param redundant_threshold: float
-            Threshold for defining redundant features in percent
+        :param n: int
+            Number of players in each game
+        """
+        _shuffle: np.array = np.array(tuple(random.sample(population=self.features, k=self.n_features)))
+        try:
+            _pairs: np.array = np.array_split(ary=_shuffle, indices_or_sections=int(self.n_features / n))
+        except ValueError:
+            _pairs: np.array = self.pairs
+        if self.tournament:
+            for pair in _pairs:
+                for feature in pair:
+                    if feature in self.shapley_additive_explanation['tournament'].keys():
+                        self.shapley_additive_explanation['tournament'][feature].append(len(pair))
+                    else:
+                        self.shapley_additive_explanation['tournament'].update({feature: [len(pair)]})
+        self.pairs = _pairs
 
-        :return dict
-            Redundant features, important features and reduction scores
+    def _play_tournament(self):
         """
-        if self.ml_type == 'reg':
-            _top_score: int = 0
-            _params: dict = ModelGeneratorReg(model_name=model).get_model_parameter()
-            _model_generator: ModelGeneratorReg = ModelGeneratorReg(model_name=model, reg_params=_params)
-        else:
-            _top_score: int = 1
-            _params: dict = ModelGeneratorClf(model_name=model).get_model_parameter()
-            _model_generator: ModelGeneratorClf = ModelGeneratorClf(model_name=model, clf_params=_params)
-        _model_generator.generate_model()
-        _train_test_split: dict = MLSampler(df=self.df,
-                                            target=self.target,
-                                            features=sorted_features
-                                            ).train_test_sampling(validation_split=0.1)
-        _model_generator.train(x=_train_test_split.get('x_train').values, y=_train_test_split.get('y_train').values)
-        _pred = _model_generator.predict(x=_train_test_split.get('x_test').values)
-        _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
-        _model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
-        _threshold = _model_test_score * (1 - redundant_threshold)
-        _features: List[str] = copy.deepcopy(sorted_features)
-        _result: dict = dict(redundant=[], important=[], reduction={})
-        for i in range(len(sorted_features) - 1, 0, -1):
-            if len(_features) == 1:
-                _result['important'] = _features
-                break
-            del _features[i]
-            _model_generator.train(x=_train_test_split.get('x_train')[_features].values, y=_train_test_split.get('y_train').values)
-            _pred = _model_generator.predict(x=_train_test_split.get('x_test')[_features].values)
-            _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
-            _new_model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
-            if _threshold >= _new_model_test_score:
-                _features.append(sorted_features[i])
-                _result['important'] = _features
-                break
+        Play unreal tournament to extract the fittest or most important players based on the concept of shapley values
+        """
+        Log(write=False, level='info').log(msg='Start penalty with {} players...'.format(self.n_features))
+        if self.mlflow_log:
+            mlflow.set_experiment(experiment_name='Shapley Additive Explanation (Feature Tournament)',
+                                  experiment_id=None
+                                  )
+        _game_scores: List[float] = []
+        _permutation_space: int = self.init_pairs
+        _pair_size_factor: float = self.max_iter * self.pair_size_factor
+        for i in range(0, self.max_iter + self.init_games, 1):
+            if i == self.init_games:
+                Log(write=False, level='info').log(msg='Start feature tournament with {} players ...'.format(self.n_features))
+                self.tournament = True
+            elif i > self.init_games:
+                _pair_size: int = _permutation_space + int(_pair_size_factor)
+                if self.n_features >= _pair_size:
+                    _permutation_space = _pair_size
+                    #_permutation_space = int(_permutation_space + (_permutation_space * self.pair_size_factor))
             else:
-                _result['redundant'].append(sorted_features[i])
-                _result['reduction'].update({sorted_features[i]: _model_test_score - _new_model_test_score})
-        Log(write=False,
-            level='info'
-            ).log(msg=f'Number of redundant features: {len(_result["redundant"])}\nNumber of important features: {len(_result["important"])}')
-        return _result
-
-    def get_imp_features(self,
-                         meth: str = 'shapley',
-                         model: str = 'cat',
-                         imp_threshold: float = 0.01,
-                         visualize_game_stats: bool = True,
-                         plot_type: str = 'bar'
-                         ) -> dict:
-        """
-        Get important features
-
-        :param meth: str
-            Feature selection method
-                -> rf: Random Forest for multi-scaled features
-                -> xgb: Extreme Gradient Boosting Decision Tree for multi-scaled features
-                -> lasso: Lasso Regression for continuous features
-                -> pca: Principal Component Analysis for continuous features
-                -> shapley: Shapley Value approximation using feature tournament framework
-
-        :param model: str
-            Name of the supervised learning model to use for ai evolution
+                if i == 0:
+                    _permutation_space = self.init_pairs
+            if _permutation_space > self.max_players:
+                _permutation_space = self.max_players
+            self._permutation(n=_permutation_space)
+            _pool: ThreadPool = ThreadPool(processes=len(self.pairs)) if self.multi_threading else None
+            for g in range(0, self.games, 1):
+                Log(write=False, level='info').log(msg='Iteration {} - Game {} ~ {} players each game'.format(i + 1,
+                                                                                                              g + 1,
+                                                                                                              _permutation_space
+                                                                                                              )
+                                                   )
+                self.game = g
+                if self.multi_threading:
+                    self.threads.update({g: _pool.apply_async(func=self._game, args=[i])})
+                else:
+                    self._game(iteration=i)
+                if i < self.init_games:
+                    break
+                self._permutation(n=_permutation_space)
+            for thread in self.threads.keys():
+                self.threads.get(thread).get()
+            if i + 1 == self.init_games:
+                _shapley_matrix: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation['sum'], index=['score']).transpose()
+                _sorted_shapley_matrix = _shapley_matrix.sort_values(by='score', axis=0, ascending=False, inplace=False)
+                _all_features: int = _sorted_shapley_matrix.shape[0]
+                _sorted_shapley_matrix = _sorted_shapley_matrix.loc[_sorted_shapley_matrix['score'] > 0, :]
+                if _sorted_shapley_matrix.shape[0] == 0:
+                    raise FeatureSelectorException('No feature scored higher than 0 during penalty phase')
+                _n_features: int = _sorted_shapley_matrix.shape[0]
+                Log(write=False, level='info').log(msg='Excluded {} features with score 0'.format(_all_features - _n_features))
+                _exclude_features: int = int(_n_features * self.penalty_factor)
+                self.features = _sorted_shapley_matrix.index.values.tolist()[0:(_n_features - _exclude_features)]
+                self.n_features = len(self.features)
+                Log(write=False, level='info').log(msg='Excluded {} lowest scored features from tournament'.format(_exclude_features))
+            if i + 1 == self.max_iter + self.init_games:
+                _shapley_values: dict = {}
+                for sv in self.shapley_additive_explanation['game'].keys():
+                    _shapley_values.update({sv: self.shapley_additive_explanation['sum'][sv] / len(self.shapley_additive_explanation['game'][sv])})
+                self.shapley_additive_explanation.update({'total': _shapley_values})
+            if self.n_features <= (self.pair_size_factor * _permutation_space):
+                if i + 1 == self.max_iter:
+                    break
+
+    def select(self,
+               imp_threshold: float = 0.01,
+               redundant_threshold: float = 0.02,
+               visualize_game_stats: bool = True,
+               plot_type: str = 'bar'
+               ) -> dict:
+        """
+        Select most important features based on shapley values
 
         :param imp_threshold: float
             Threshold of importance score
 
+        :param redundant_threshold: float
+            Threshold for defining redundant features in percent
+
         :param visualize_game_stats: bool
             Whether to visualize game statistics or not
 
         :param plot_type: str
             Name of the plot type
                 -> pie: Pie Chart
                 -> bar: Bar Chart
 
-        :return: dict:
-            Important features and importance score
+        :return dict
+            Redundant features, important features and reduction scores
         """
+        self._play_tournament()
         _imp_plot: dict = {}
-        _imp_features: List[str] = []
         _core_features: List[str] = []
         _processed_features: List[str] = []
         _imp_threshold: float = imp_threshold if (imp_threshold >= 0) and (imp_threshold <= 1) else 0.7
-        if meth == 'shapley':
-            _imp_scores: dict = FeatureTournament(df=self.df,
-                                                  features=self.features,
-                                                  target=self.target,
-                                                  force_target_type=self.force_target_type,
-                                                  models=['cat'] if model is None else [model],
-                                                  init_pairs=3 if self.init_pairs is None else self.init_pairs,
-                                                  init_games=5 if self.init_games is None else self.init_games,
-                                                  increasing_pair_size_factor=0.05 if self.increasing_pair_size_factor is None else self.increasing_pair_size_factor,
-                                                  games=3 if self.games is None else self.games,
-                                                  penalty_factor=0.1 if self.penalty_factor is None else self.penalty_factor,
-                                                  evolutionary_algorithm='si' if self.evolutionary_algorithm is None else self.evolutionary_algorithm,
-                                                  max_iter=50 if self.max_iter is None else self.max_iter,
-                                                  max_players=-1 if self.max_players is None else self.max_players,
-                                                  mlflow_log=False if self.kwargs.get('mlflow_log_shapley') is None else self.kwargs.get('mlflow_log_shapley'),
-                                                  **self.kwargs
-                                                  ).play()
-            _df: pd.DataFrame = pd.DataFrame(data=_imp_scores.get('total'), index=['score']).transpose()
-            _df = _df.sort_values(by='score', axis=0, ascending=False, inplace=False)
-            _df['feature'] = _df.index.values
-            _imp_features = _df['feature'].values.tolist()
-            for s, feature in enumerate(_imp_features):
-                self.imp_score.update({feature: _df['score'].values.tolist()[s]})
-            _rank: List[int] = []
-            _sorted_scores: List[float] = _df['score'].values.tolist()
-            for r, val in enumerate(_sorted_scores):
-                if r == 0:
-                    _rank.append(r + 1)
-                else:
-                    if val == _sorted_scores[r - 1]:
-                        _rank.append(_rank[-1])
-                    else:
-                        _rank.append(r + 1)
-            _df['rank'] = _rank
-            _game_df: pd.DataFrame = pd.DataFrame(data=_imp_scores.get('game'))
-            #_game_df['game'] = _game_df.index.values
-            _tournament_df: pd.DataFrame = pd.DataFrame(data=_imp_scores.get('tournament'))
-            #_tournament_df['game'] = _tournament_df.index.values
-            _file_paths: List[str] = []
-            if self.visualize_all_scores:
-                if visualize_game_stats:
-                    _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_stats.html'))
-                    _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_size.html'))
-                    _game_plot: dict = {'Feature Tournament Game Stats (Shapley Scores)': dict(data=_game_df,
-                                                                                               features=list(_game_df.columns),
-                                                                                               plot_type='violin',
-                                                                                               melt=True,
-                                                                                               render=True,
-                                                                                               file_path=_file_paths[0] if self.path is not None else None
-                                                                                               ),
-                                        'Feature Tournament Stats (Game Size)': dict(data=_tournament_df,
-                                                                                     features=list(_tournament_df.columns),
-                                                                                     plot_type='heat',
-                                                                                     render=True,
-                                                                                     file_path=_file_paths[1] if self.path is not None else None
-                                                                                     )
-                                        }
-                    DataVisualizer(subplots=_game_plot,
-                                   height=500,
-                                   width=500
-                                   ).run()
-                _file_paths.append(os.path.join(str(self.path), 'feature_importance_shapley.html'))
-                _imp_plot: dict = {'Feature Importance (Shapley Scores)': dict(df=_df,
-                                                                               plot_type=plot_type,
-                                                                               render=True if self.path is None else False,
-                                                                               file_path=_file_paths[-1] if self.path is not None else None,
-                                                                               kwargs=dict(layout={},
-                                                                                           y=_df['score'].values,
-                                                                                           x=_df.index.values.tolist(),
-                                                                                           marker=dict(color=_df['score'],
-                                                                                                       colorscale='rdylgn',
-                                                                                                       autocolorscale=True
-                                                                                                       )
-                                                                                           )
-                                                                               )
-                                   }
-            if self.mlflow_log:
-                self._mlflow_tracking(stats={'Feature Score (Feature Tournament)': _df,
-                                             'Game Size (Feature Tournament)': _tournament_df,
-                                             'Game Score (Feature Tournament)': _game_df
-                                             },
-                                      file_paths=_file_paths)
-        elif meth == 'pca':
-            raise NotImplementedError('Feature selection using Principal Component Analysis (PCA) not implemented')
-        elif meth in ['lasso', 'cat', 'rf', 'gbo', 'xgb']:
-            if self.mlflow_log:
-                _meth: str = 'Lasso Regression' if meth == 'lasso' else 'Decision Tree'
-                mlflow.set_experiment(experiment_name=f'Feature Selector {_meth}',
-                                      experiment_id=None
-                                      )
-            if self.ml_type == 'reg':
-                _ml = ModelGeneratorReg(model_name=meth).generate_model()
+        _df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('total'), index=['score']).transpose()
+        _df = _df.sort_values(by='score', axis=0, ascending=False, inplace=False)
+        _df['feature'] = _df.index.values
+        _imp_features: List[str] = _df['feature'].values.tolist()
+        for s, feature in enumerate(_imp_features):
+            self.imp_score.update({feature: _df['score'].values.tolist()[s]})
+        _rank: List[int] = []
+        _sorted_scores: List[float] = _df['score'].values.tolist()
+        for r, val in enumerate(_sorted_scores):
+            if r == 0:
+                _rank.append(r + 1)
             else:
-                if meth == 'lasso':
-                    raise FeatureSelectorException('Cannot perform classification using Lasso Regression model')
-                _ml = ModelGeneratorClf(model_name=meth).generate_model()
-            _train_test_data: dict = MLSampler(df=self.df, target=self.target, features=self.features, stratification=False).train_test_sampling()
-            _ml.train(x=_train_test_data.get('x_train').values, y=_train_test_data.get('y_train').values)
-            _imp_features = self.df[self.features].columns[SelectFromModel(estimator=_ml.model,
-                                                                           threshold='median' if imp_threshold is None else imp_threshold,
-                                                                           prefit=True,
-                                                                           norm_order=1,
-                                                                           max_features=None
-                                                                           ).get_support()]
-            _imp_features = list(set(_imp_features))
-            self.imp_score.update({self.features[i]: ft_imp for i, ft_imp in enumerate(_ml.model.feature_importances_)})
-            if plot_type not in ['pie', 'bar']:
-                raise FeatureSelectorException(
-                    'Plot type ({}) for visualizing feature importance not supported'.format(plot_type))
-            _df: pd.DataFrame = pd.DataFrame(data=self.imp_score.values(), index=list(self.imp_score.keys()),
-                                             columns=['importance'])
-            _df = _df.sort_values(by=['importance'], axis=0, ascending=False, inplace=False, kind='quicksort')
-            if self.visualize_all_scores:
-                _imp_plot: dict = {'Feature Importance ({})'.format(meth.upper()): dict(data=_df,
-                                                                                        plot_type=plot_type,
-                                                                                        melt=False,
-                                                                                        interactive=True,
-                                                                                        render=True if self.path is None else False,
-                                                                                        file_path='{}feature_importance_{}.html'.format(self.path, meth.upper()) if self.path is not None else None,
-                                                                                        kwargs=dict(layout={})
-                                                                                        )
-                                   }
-                if plot_type == 'pie':
-                    _imp_plot[list(_imp_plot.keys())[0]]['kwargs'].update({'values': _df['importance'].values * 100,
-                                                                           'labels': _df.index.values.tolist(),
-                                                                           'textposition': 'inside',
-                                                                           'marker': dict(colors=_df['importance'])
-                                                                           })
-                elif plot_type == 'bar':
-                    _imp_plot[list(_imp_plot.keys())[0]]['kwargs'].update({'y': _df['importance'].values,
-                                                                           'x': _df.index.values.tolist(),
-                                                                           'marker': dict(color=_df['importance'],
-                                                                                          colorscale='rdylgn',
-                                                                                          autocolorscale=True
-                                                                                          )
-                                                                           })
-        else:
-            raise FeatureSelectorException('Method ({}) for scoring and selecting important features not supported'.format(meth))
+                if val == _sorted_scores[r - 1]:
+                    _rank.append(_rank[-1])
+                else:
+                    _rank.append(r + 1)
+        _df['rank'] = _rank
+        _game_df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('game'))
+        # _game_df['game'] = _game_df.index.values
+        _tournament_df: pd.DataFrame = pd.DataFrame(data=self.shapley_additive_explanation.get('tournament'))
+        # _tournament_df['game'] = _tournament_df.index.values
+        _file_paths: List[str] = []
+        if self.visualize_all_scores:
+            if visualize_game_stats:
+                _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_stats.html'))
+                _file_paths.append(os.path.join(str(self.path), 'feature_tournament_game_size.html'))
+                _game_plot: dict = {'Feature Tournament Game Stats (Shapley Scores)': dict(data=_game_df,
+                                                                                           features=list(
+                                                                                               _game_df.columns),
+                                                                                           plot_type='violin',
+                                                                                           melt=True,
+                                                                                           render=True,
+                                                                                           file_path=_file_paths[
+                                                                                               0] if self.path is not None else None
+                                                                                           ),
+                                    'Feature Tournament Stats (Game Size)': dict(data=_tournament_df,
+                                                                                 features=list(_tournament_df.columns),
+                                                                                 plot_type='heat',
+                                                                                 render=True,
+                                                                                 file_path=_file_paths[
+                                                                                     1] if self.path is not None else None
+                                                                                 )
+                                    }
+                DataVisualizer(subplots=_game_plot,
+                               height=500,
+                               width=500
+                               ).run()
+            _file_paths.append(os.path.join(str(self.path), 'feature_importance_shapley.html'))
+            _imp_plot: dict = {'Feature Importance (Shapley Scores)': dict(df=_df,
+                                                                           plot_type=plot_type,
+                                                                           render=True if self.path is None else False,
+                                                                           file_path=_file_paths[
+                                                                               -1] if self.path is not None else None,
+                                                                           kwargs=dict(layout={},
+                                                                                       y=_df['score'].values,
+                                                                                       x=_df.index.values.tolist(),
+                                                                                       marker=dict(color=_df['score'],
+                                                                                                   colorscale='rdylgn',
+                                                                                                   autocolorscale=True
+                                                                                                   )
+                                                                                       )
+                                                                           )
+                               }
+        if self.mlflow_log:
+            self._mlflow_tracking(stats={'Feature Score (Feature Tournament)': _df,
+                                         'Game Size (Feature Tournament)': _tournament_df,
+                                         'Game Score (Feature Tournament)': _game_df
+                                         },
+                                  file_paths=_file_paths)
         if self.aggregate_feature_imp is not None:
             _aggre_score: dict = {}
             for core_feature in self.aggregate_feature_imp.keys():
                 _feature_scores: dict = {}
                 _aggre_score.update({core_feature: 0.0 if self.imp_score.get(core_feature) is None else self.imp_score.get(core_feature)})
                 if self.imp_score.get(core_feature) is not None:
                     _feature_scores.update({core_feature: self.imp_score.get(core_feature)})
@@ -463,13 +636,72 @@
                                                                                         )
                                   })
         if self.visualize_all_scores or self.visualize_variant_scores or self.visualize_core_features_scores:
             DataVisualizer(subplots=_imp_plot,
                            height=500,
                            width=500
                            ).run()
+        if self.ml_type == 'reg':
+            _model_generator: ModelGeneratorReg = ModelGeneratorReg(model_name=self.feature_tournament_ai.get('model_name'),
+                                                                    reg_params=self.feature_tournament_ai.get('param')
+                                                                    )
+        else:
+            _model_generator: ModelGeneratorClf = ModelGeneratorClf(model_name=self.feature_tournament_ai.get('model_name'),
+                                                                    clf_params=self.feature_tournament_ai.get('param')
+                                                                    )
+        _model_generator.generate_model()
+        _train_test_split: dict = MLSampler(df=self.df,
+                                            target=self.target,
+                                            features=_imp_features
+                                            ).train_test_sampling(validation_split=0.1)
+        _model_generator.train(x=_train_test_split.get('x_train').values, y=_train_test_split.get('y_train').values)
+        _pred = _model_generator.predict(x=_train_test_split.get('x_test').values)
+        _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
+        _model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
+        if self.ml_type == 'reg':
+            _threshold: float = _model_test_score * (1 + redundant_threshold)
+        else:
+            _threshold: float = _model_test_score * (1 - redundant_threshold)
+        print('Metric', _model_test_score)
+        print('Threshold', _threshold)
+        _features: List[str] = copy.deepcopy(_imp_features)
+        print(_features)
+        _result: dict = dict(redundant=[], important=[], reduction={})
+        for i in range(len(_imp_features) - 1, 0, -1):
+            print(_imp_features[i])
+            if len(_features) == 1:
+                _result['important'] = _features
+                break
+            del _features[i]
+            _model_generator.train(x=_train_test_split.get('x_train')[_features].values, y=_train_test_split.get('y_train').values)
+            _pred = _model_generator.predict(x=_train_test_split.get('x_test')[_features].values)
+            _model_generator.eval(obs=_train_test_split.get('y_test').values, pred=_pred)
+            _new_model_test_score: float = _model_generator.fitness['test'].get(self.ml_metric)
+            print('New model score', _new_model_test_score)
+            if self.ml_type == 'reg':
+                if _threshold <= _new_model_test_score:
+                    _features.append(_imp_features[i])
+                    _result['important'] = _features
+                    break
+                else:
+                    _result['redundant'].append(_imp_features[i])
+                    _result['reduction'].update({_imp_features[i]: _model_test_score - _new_model_test_score})
+            else:
+                if _threshold >= _new_model_test_score:
+                    _features.append(_imp_features[i])
+                    _result['important'] = _features
+                    break
+                else:
+                    _result['redundant'].append(_imp_features[i])
+                    _result['reduction'].update({_imp_features[i]: _model_test_score - _new_model_test_score})
+        Log(write=False,
+            level='info'
+            ).log(msg=f'Number of redundant features: {len(_result["redundant"])}\nNumber of important features: {len(_result["important"])}')
         return dict(imp_features=_imp_features,
                     imp_score=self.imp_score,
                     imp_threshold=imp_threshold,
                     imp_core_features=_core_features,
-                    imp_processed_features=_processed_features
+                    imp_processed_features=_processed_features,
+                    redundant=_result['redundant'],
+                    important=_result['important'],
+                    reduction=_result['reduction']
                     )
```

### Comparing `happy_learning-0.4.7/happy_learning/genetic_algorithm.py` & `happy_learning-0.4.8/happy_learning/genetic_algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1589,137 +1589,130 @@
                 _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
                 _best_model_results['rel_diff'] = _best_model_results['obs'] / _best_model_results['pred']
             elif self.target_type == 'clf_multi':
                 _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
             _best_model_results = _best_model_results.round(decimals=4)
             if self.target_type == 'reg':
                 _file_paths.append(os.path.join(self.output_file_path, 'evaluation_coords.html'))
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction Evaluation of final inherited ML Model:',
+                               features=['obs', 'abs_diff', 'rel_diff', 'pred'],
+                               color_feature='pred',
+                               plot_type='parcoords',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'evaluation_coords.html'),
+                               ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'scatter_contour.html'))
-                _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                           features=['obs', 'abs_diff',
-                                                                                                     'rel_diff', 'pred'],
-                                                                                           color_feature='pred',
-                                                                                           plot_type='parcoords',
-                                                                                           file_path=_file_paths[0],
-                                                                                           kwargs=dict(layout={})
-                                                                                           ),
-                                'Prediction vs. Observation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                                features=['obs', 'pred'],
-                                                                                                plot_type='joint',
-                                                                                                file_path=_file_paths[1],
-                                                                                                kwargs=dict(layout={})
-                                                                                                )
-                                })
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction vs. Observation of final inherited ML Model:',
+                               features=['obs', 'pred'],
+                               plot_type='joint',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'scatter_contour.html'),
+                               ).run()
             else:
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'clf_metrics_table.html'))
                 _eval_clf: EvalClf = EvalClf(obs=self.data_set.get('y_test'),
                                              pred=self.data_set.get('pred'),
                                              labels=self.target_labels
                                              )
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=_eval_clf.confusion(),
                                                                index=[f'{label}_obs' for label in self.target_labels],
                                                                columns=[f'{label}_pred' for label in self.target_labels]
                                                                )
                 _cf_row_sum = pd.DataFrame()
                 _cf_row_sum[' '] = _confusion_matrix.sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_row_sum.transpose()], axis=0)
                 _cf_col_sum = pd.DataFrame()
                 _cf_col_sum[' '] = _confusion_matrix.transpose().sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_col_sum], axis=1)
-                _charts.update({'Confusion Matrix': dict(data=_confusion_matrix,
-                                                         plot_type='table',
-                                                         file_path=_file_paths[0]
-                                                         )
-                                })
-                _charts.update({'Confusion Matrix Heatmap': dict(data=_confusion_matrix,
-                                                                 features=self.target_labels,
-                                                                 plot_type='heat',
-                                                                 file_path=_file_paths[1],
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_table.html'),
+                               ).run()
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix Heatmap:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_heatmap.html'),
+                               ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
                                                                           # index=['obs', 'pred'],
                                                                           # columns=['obs', 'pred']
                                                                           )
-                _charts.update({'Confusion Matrix Normalized Heatmap:': dict(data=_confusion_matrix_normalized,
-                                                                             features=self.target_labels,
-                                                                             plot_type='heat',
-                                                                             file_path=_file_paths[2],
-                                                                             kwargs=dict(layout={})
-                                                                             )
-                                })
-                _charts.update({'Classification Report:': dict(data=_best_model_results,
-                                                               plot_type='table',
-                                                               file_path=_file_paths[3],
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
+                DataVisualizer(df=_confusion_matrix_normalized,
+                               title='Confusion Matrix Normalized Heatmap:',
+                               features=_confusion_matrix_normalized.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_normal_heatmap.html'),
+                               ).run()
+                _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
+                DataVisualizer(df=_best_model_results,
+                               title='Classification Report:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'clf_report_table.html'),
+                               ).run()
                 _classification_report: dict = _eval_clf.classification_report()
                 _confusion_metrics: dict = dict(precision=[], recall=[], f1=[])
                 for label in self.target_labels:
                     _confusion_metrics['precision'].append(_classification_report.get(label)['precision'])
                     _confusion_metrics['recall'].append(_classification_report.get(label)['recall'])
                     _confusion_metrics['f1'].append(_classification_report.get(label)['f1-score'])
-                _charts.update({'Classification Metrics': dict(data=pd.DataFrame(data=_confusion_metrics,
-                                                                                 index=self.target_labels,
-                                                                                 columns=list(_confusion_metrics.keys())
-                                                                                 ),
-                                                               plot_type='table',
-                                                               file_path=_file_paths[4],
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'clf_metrics_table.html'))
+                _clf_metrics: pd.DataFrame = pd.DataFrame(data=_confusion_metrics,
+                                                          index=self.target_labels,
+                                                          columns=list(_confusion_metrics.keys())
+                                                          )
+                DataVisualizer(df=_clf_metrics,
+                               title='Classification Metrics:',
+                               features=_clf_metrics.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'clf_metrics_table.html'),
+                               ).run()
                 if self.target_type == 'clf_multi':
                     _file_paths.append(os.path.join(self.output_file_path, 'evaluation_category.html'))
-                    _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                               features=['obs',
-                                                                                                         'abs_diff',
-                                                                                                         'pred'
-                                                                                                         ],
-                                                                                               color_feature='pred',
-                                                                                               plot_type='parcoords',
-                                                                                               file_path=_file_paths[-1],
-                                                                                               kwargs=dict(layout={})
-                                                                                               )
-                                    })
+                    DataVisualizer(df=_best_model_results,
+                                   title='Prediction Evaluation of final inherited ML Model:',
+                                   features=['obs', 'abs_diff', 'pred'],
+                                   color_feature='pred',
+                                   plot_type='parcoords',
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'evaluation_category.html'),
+                                   ).run()
                 else:
-                    _file_paths.append(os.path.join(self.output_file_path, 'roc_auc_curve.html'))
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
                     _roc_curve['baseline'] = _roc_curve_values['false_positive_rate'][1]
-                    _charts.update({'ROC-AUC Curve': dict(data=_roc_curve,
-                                                          features=['roc_curve', 'baseline'],
-                                                          time_features=['baseline'],
-                                                          # xaxis_label=['False Positive Rate'],
-                                                          # yaxis_label=['True Positive Rate'],
-                                                          melt=True,
-                                                          plot_type='line',
-                                                          use_auto_extensions=False,
-                                                          file_path=_file_paths[-1],
-                                                          kwargs=dict(layout={})
-                                                          )
-                                    })
-            DataVisualizer(subplots=_charts,
-                           interactive=True,
-                           file_path=self.output_file_path,
-                           render=True if self.output_file_path is None else False,
-                           height=750,
-                           width=750,
-                           unit='px'
-                           ).run()
+                    _file_paths.append(os.path.join(self.output_file_path, 'roc_auc_curve.html'))
+                    DataVisualizer(df=_roc_curve,
+                                   title='ROC-AUC Curve:',
+                                   features=['roc_curve', 'baseline'],
+                                   time_features=['baseline'],
+                                   plot_type='line',
+                                   # xaxis_label=['False Positive Rate'],
+                                   # yaxis_label=['True Positive Rate'],
+                                   use_auto_extensions=False,
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'roc_auc_curve.html'),
+                                   ).run()
             for path in _file_paths:
                 _file_name: str = path.split('/')[-1].replace('.html', '')
                 try:
                     mlflow.log_artifact(local_path=path, artifact_path=_file_name)
                 except FileNotFoundError:
                     Log(write=self.log, logger_file_path=self.output_file_path).log(f'File artifact {path} not found')
 
@@ -1871,27 +1864,27 @@
                        ga: bool = True,
                        model: bool = True,
                        evolution_history: bool = False,
                        generation_history: bool = False,
                        final_generation: bool = False
                        ):
         """
-        Save evolution meta data generated by genetic algorithm to local hard drive as pickle file
+        Save evolution metadata generated by genetic algorithm to local hard drive as pickle file
 
         :param ga: bool
             Save GeneticAlgorithm class object (required for continuing evolution / optimization)
 
         :param model: bool
             Save evolved model
 
         :param evolution_history: bool
-            Save evolution history meta data
+            Save evolution history metadata
 
         :param generation_history: bool
-            Save generation history meta data
+            Save generation history metadata
 
         :param final_generation: bool
             Save settings of each individual of final generation
         """
         # Export evolution history data:
         if evolution_history:
             DataExporter(obj=self.evolution_history,
@@ -1923,18 +1916,15 @@
                          ).file()
         # Export evolved model:
         if model:
             _file_name_extension: str = '' if self.kwargs.get('model_file_name_extension') is None else '_{}'.format(self.kwargs.get('model_file_name_extension'))
             _file_name: str = 'model{}.p'.format(_file_name_extension)
             if self.cloud is None:
                 if self.deep_learning:
-                    if self.current_generation_meta_data['model_name'][self.best_individual_idx] == 'trans':
-                        torch.save(obj=self.model.model, f=os.path.join(self.output_file_path, _file_name))
-                    else:
-                        torch.save(obj=self.model, f=os.path.join(self.output_file_path, _file_name))
+                    torch.save(obj=self.model, f=os.path.join(self.output_file_path, _file_name))
                 else:
                     DataExporter(obj=self.model,
                                  file_path=os.path.join(self.output_file_path, _file_name),
                                  create_dir=False,
                                  overwrite=True
                                  ).file()
             else:
@@ -1954,31 +1944,32 @@
                                  overwrite=True,
                                  cloud=self.cloud,
                                  bucket_name=self.bucket_name,
                                  region=self.kwargs.get('region')
                                  ).file()
         # Export GeneticAlgorithm class object:
         if ga:
-            if self.stopping_reason is None:
-                self.feature_engineer = None
-            else:
-                self.df = None
-                self.model = None
-                self.population = []
-                self.feature_engineer = None
-            _file_name_extension: str = '' if self.kwargs.get('ga_file_name_extension') is None else '_{}'.format(self.kwargs.get('ga_file_name_extension'))
-            _file_name: str = 'genetic{}.p'.format(_file_name_extension)
-            DataExporter(obj=self,
-                         file_path=os.path.join(self.output_file_path, _file_name),
-                         create_dir=False,
-                         overwrite=True,
-                         cloud=self.cloud,
-                         bucket_name=self.bucket_name,
-                         region=self.kwargs.get('region')
-                         ).file()
+            if not self.deep_learning:
+                if self.stopping_reason is None:
+                    self.feature_engineer = None
+                else:
+                    self.df = None
+                    self.model = None
+                    self.population = []
+                    self.feature_engineer = None
+                _file_name_extension: str = '' if self.kwargs.get('ga_file_name_extension') is None else '_{}'.format(self.kwargs.get('ga_file_name_extension'))
+                _file_name: str = 'genetic{}.p'.format(_file_name_extension)
+                DataExporter(obj=self,
+                             file_path=os.path.join(self.output_file_path, _file_name),
+                             create_dir=False,
+                             overwrite=True,
+                             cloud=self.cloud,
+                             bucket_name=self.bucket_name,
+                             region=self.kwargs.get('region')
+                             ).file()
 
     def visualize(self,
                   results_table: bool = True,
                   model_distribution: bool = False,
                   model_evolution: bool = True,
                   param_distribution: bool = False,
                   train_time_distribution: bool = True,
@@ -2059,220 +2050,199 @@
         if self.target_type == 'reg':
             _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
             _best_model_results['rel_diff'] = _best_model_results['obs'] / _best_model_results['pred']
         elif self.target_type == 'clf_multi':
             _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
         _best_model_results = _best_model_results.round(decimals=4)
         if results_table:
-            _charts.update({'Results of Genetic Algorithm:': dict(data=_evolution_history_data,
-                                                                  plot_type='table',
-                                                                  file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_metadata_table.html'),
-                                                                  kwargs=dict(layout={})
-                                                                  )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Results of Genetic Algorithm:',
+                           features=_evolution_history_data.columns.to_list(),
+                           plot_type='table',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_metadata_table.html'),
+                           ).run()
         if model_evolution:
-            _charts.update({'Evolution of used ML Models:': dict(data=_evolution_history_data,
-                                                                 features=['fitness_score', 'generation'],
-                                                                 color_feature='model',
-                                                                 plot_type='scatter',
-                                                                 melt=True,
-                                                                 file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_model_evolution.html'),
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Evolution of used ML Models:',
+                           features=['fitness_score', 'generation'],
+                           color_feature='model',
+                           plot_type='scatter',
+                           melt=True,
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_model_evolution.html'),
+                           ).run()
         if model_distribution:
             if self.models is None or len(self.models) > 1:
-                _charts.update({'Distribution of used ML Models:': dict(data=_evolution_history_data,
-                                                                        features=['model'],
-                                                                        group_by=['generation'] if per_generation else None,
-                                                                        plot_type='pie',
-                                                                        file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_model_distribution.html'),
-                                                                        kwargs=dict(layout={})
-                                                                        )
-                                })
+                DataVisualizer(df=_evolution_history_data,
+                               title='Distribution of used ML Models:',
+                               features=['model'],
+                               group_by=['generation'] if per_generation else None,
+                               plot_type='pie',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_model_distribution.html'),
+                               ).run()
         #if param_distribution:
         #    _charts.update({'Distribution of ML Model parameters:': dict(data=_evolution_history_data,
         #                                                                 features=['model_param'],
         #                                                                 group_by=['generation'] if per_generation else None,
         #                                                                 plot_type='tree',
         #                                                                 file_path=self.output_file_path if self.output_file_path is None else '{}{}'.format(self.output_file_path, 'ga_parameter_treemap.html')
         #                                                                 )
         #                    })
         if train_time_distribution:
-            _charts.update({'Distribution of elapsed Training Time:': dict(data=_evolution_history_data,
-                                                                           features=['train_time_in_seconds'],
-                                                                           group_by=['model'],
-                                                                           plot_type='violin',
-                                                                           melt=True if len(self.models) > 1 else False,
-                                                                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_training_time_distribution.html'),
-                                                                           kwargs=dict(layout={})
-                                                                           )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Distribution of elapsed Training Time:',
+                           features=['train_time_in_seconds'],
+                           group_by=['model'],
+                           melt=True,
+                           plot_type='violin',
+                           use_auto_extensions=False,
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_training_time_distribution.html'),
+                           ).run()
         if breeding_map:
             _breeding_map: pd.DataFrame = pd.DataFrame(data=dict(gen_0=self.generation_history['population']['gen_0'].get('fitness')), index=[0])
             for g in self.generation_history['population'].keys():
                 if g != 'gen_0':
                     _breeding_map[g] = self.generation_history['population'][g].get('fitness')
-            _charts.update({'Breeding Heat Map:': dict(data=_breeding_map,
-                                                       plot_type='heat',
-                                                       file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_breeding_heatmap.html'),
-                                                       kwargs=dict(layout={})
-                                                       )
-                            })
+            DataVisualizer(df=_breeding_map,
+                           title='Breeding Heat Map:',
+                           features=_breeding_map.columns.to_list(),
+                           plot_type='heat',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_breeding_heatmap.html'),
+                           ).run()
         if breeding_graph:
-            _charts.update({'Breeding Network Graph:': dict(data=_evolution_history_data,
-                                                            features=['generation', 'fitness_score'],
-                                                            graph_features=dict(node='id', edge='parent'),
-                                                            color_feature='model',
-                                                            plot_type='network',
-                                                            file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_breeding_graph.html'),
-                                                            kwargs=dict(layout={})
-                                                            )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Breeding Network Graph:',
+                           features=['generation', 'fitness_score'],
+                           graph_features=dict(node='id', edge='parent'),
+                           color_feature='model',
+                           plot_type='network',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_breeding_graph.html'),
+                           ).run()
         if fitness_distribution:
-            _charts.update({'Distribution of Fitness Metric:': dict(data=_evolution_history_data,
-                                                                    features=['fitness_score'],
-                                                                    time_features=['generation'],
-                                                                    plot_type='ridgeline',
-                                                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_fitness_score_distribution_per_generation.html'),
-                                                                    kwargs=dict(layout={})
-                                                                    )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Distribution of Fitness Metric:',
+                           features=['fitness_score'],
+                           time_features=['generation'],
+                           plot_type='ridgeline',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_fitness_score_distribution_per_generation.html'),
+                           ).run()
         if fitness_dimensions:
-            _charts.update({'Evolution Meta Data:': dict(data=_evolution_history_data,
-                                                         features=['train_time_in_seconds',
-                                                                   'ml_metric',
-                                                                   'train_test_diff',
-                                                                   'fitness_score',
-                                                                   'parent',
-                                                                   'id',
-                                                                   'generation',
-                                                                   'model'
-                                                                   ],
-                                                         color_feature='model',
-                                                         plot_type='parcoords',
-                                                         file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_metadata_evolution_coords.html'),
-                                                         kwargs=dict(layout={})
-                                                         )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Evolution Meta Data:',
+                           features=['train_time_in_seconds',
+                                     'ml_metric',
+                                     'train_test_diff',
+                                     'fitness_score',
+                                     'parent',
+                                     'id',
+                                     'generation',
+                                     'model'
+                                     ],
+                           color_feature='model',
+                           plot_type='parcoords',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_metadata_evolution_coords.html'),
+                           ).run()
         if fitness_evolution:
-            _charts.update({'Fitness Evolution:': dict(data=_evolution_gradient_data,
-                                                       features=['min', 'median', 'mean', 'max'],
-                                                       time_features=['generation'],
-                                                       plot_type='line',
-                                                       melt=True,
-                                                       file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_evolution_fitness_score.html'),
-                                                       kwargs=dict(layout={})
-                                                       )
-                            })
+            DataVisualizer(df=_evolution_gradient_data,
+                           title='Fitness Evolution:',
+                           features=['min', 'median', 'mean', 'max'],
+                           time_features=['generation'],
+                           melt=True,
+                           plot_type='line',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_evolution_fitness_score.html'),
+                           ).run()
         if epoch_stats:
             if self.deep_learning:
                 _epoch_metric_score: pd.DataFrame = pd.DataFrame(data=self.evolution.get('epoch_metric_score'))
                 _epoch_metric_score['epoch'] = [epoch + 1 for epoch in range(0, _epoch_metric_score.shape[0], 1)]
-                _charts.update({'Epoch Evaluation of fittest neural network': dict(data=_epoch_metric_score,
-                                                                                   features=['train', 'val'],
-                                                                                   time_features=['epoch'],
-                                                                                   plot_type='line',
-                                                                                   melt=True,
-                                                                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_epoch_metric_score.html'),
-                                                                                   kwargs=dict(layout={})
-                                                                                   )
-                                })
+                DataVisualizer(df=_epoch_metric_score,
+                               title='Epoch Evaluation of fittest neural network:',
+                               features=['train', 'val'],
+                               time_features=['epoch'],
+                               melt=True,
+                               plot_type='line',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_epoch_metric_score.html'),
+                               ).run()
         if prediction_of_best_model:
             if self.target_type == 'reg':
-                _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                           features=['obs', 'abs_diff', 'rel_diff', 'pred'],
-                                                                                           color_feature='pred',
-                                                                                           plot_type='parcoords',
-                                                                                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_evaluation_coords.html'),
-                                                                                           kwargs=dict(layout={})
-                                                                                           ),
-                                'Prediction vs. Observation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                                features=['obs', 'pred'],
-                                                                                                plot_type='joint',
-                                                                                                file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_scatter_contour.html'),
-                                                                                                kwargs=dict(layout={})
-                                                                                                )
-                                })
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction Evaluation of final inherited ML Model:',
+                               features=['obs', 'abs_diff', 'rel_diff', 'pred'],
+                               color_feature='pred',
+                               plot_type='parcoords',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_evaluation_coords.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction vs. Observation of final inherited ML Model:',
+                               features=['obs', 'pred'],
+                               plot_type='joint',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_scatter_contour.html'),
+                               ).run()
             else:
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                             pred=self.data_set.get('pred')
                                                                             ).confusion(),
                                                                index=self.target_labels,
                                                                columns=self.target_labels
                                                                )
                 _cf_row_sum = pd.DataFrame()
                 _cf_row_sum[' '] = _confusion_matrix.sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_row_sum.transpose()], axis=0)
                 _cf_col_sum = pd.DataFrame()
                 _cf_col_sum[' '] = _confusion_matrix.transpose().sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_col_sum], axis=1)
-                _charts.update({'Confusion Matrix': dict(data=_confusion_matrix,
-                                                         plot_type='table',
-                                                         file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_table.html'),
-                                                         kwargs=dict(layout={})
-                                                         )
-                                })
-                _charts.update({'Confusion Matrix Heatmap': dict(data=_best_model_results,
-                                                                 features=['obs', 'pred'],
-                                                                 plot_type='heat',
-                                                                 file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_heatmap.html'),
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                                })
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_table.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Confusion Matrix Heatmap:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_heatmap.html'),
+                               ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
-                                                                          #index=['obs', 'pred'],
-                                                                          #columns=['obs', 'pred']
+                                                                          index=self.target_labels,
+                                                                          columns=self.target_labels
                                                                           )
-                _charts.update({'Confusion Matrix Normalized Heatmap:': dict(data=_confusion_matrix_normalized,
-                                                                             features=self.target_labels,
-                                                                             plot_type='heat',
-                                                                             file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_normal_heatmap.html'),
-                                                                             kwargs=dict(layout={})
-                                                                             )
-                                })
-                _charts.update({'Classification Report:': dict(data=_best_model_results,
-                                                               plot_type='table',
-                                                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_clf_report_table.html'),
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                DataVisualizer(df=_confusion_matrix_normalized,
+                               title='Confusion Matrix Normalized Heatmap:',
+                               features=_confusion_matrix_normalized.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_confusion_normal_heatmap.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Classification Report:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_clf_report_table.html'),
+                               ).run()
                 if self.target_type == 'clf_multi':
-                    _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                               features=['obs', 'abs_diff', 'pred'],
-                                                                                               color_feature='pred',
-                                                                                               plot_type='parcoords',
-                                                                                               brushing=True,
-                                                                                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_evaluation_category.html'),
-                                                                                               kwargs=dict(layout={})
-                                                                                               )
-                                    })
+                    DataVisualizer(df=_best_model_results,
+                                   title='Prediction Evaluation of final inherited ML Model:',
+                                   features=['obs', 'abs_diff', 'pred'],
+                                   color_feature='pred',
+                                   plot_type='parcoords',
+                                   brushing=True,
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_evaluation_category.html'),
+                                   ).run()
                 else:
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
                     _roc_curve['baseline'] = _roc_curve_values['false_positive_rate'][1]
-                    _charts.update({'ROC-AUC Curve': dict(data=_roc_curve,
-                                                          features=['roc_curve', 'baseline'],
-                                                          time_features=['baseline'],
-                                                          #xaxis_label=['False Positive Rate'],
-                                                          #yaxis_label=['True Positive Rate'],
-                                                          melt=True,
-                                                          plot_type='line',
-                                                          use_auto_extensions=False,
-                                                          file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_roc_auc_curve.html'),
-                                                          kwargs=dict(layout={})
-                                                          )
-                                    })
-        if len(_charts.keys()) > 0:
-            DataVisualizer(subplots=_charts,
-                           interactive=True,
-                           file_path=self.output_file_path,
-                           render=True if self.output_file_path is None else False,
-                           height=750,
-                           width=750,
-                           unit='px'
-                           ).run()
+                    DataVisualizer(df=_roc_curve,
+                                   title='ROC-AUC Curve:',
+                                   features=['roc_curve', 'baseline'],
+                                   time_features=['baseline'],
+                                   plot_type='line',
+                                   melt=True,
+                                   use_auto_extensions=False,
+                                   # xaxis_label=['False Positive Rate'],
+                                   # yaxis_label=['True Positive Rate'],
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'ga_prediction_roc_auc_curve.html'),
+                                   ).run()
```

### Comparing `happy_learning-0.4.7/happy_learning/missing_data_analysis.py` & `happy_learning-0.4.8/happy_learning/missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/multiple_imputation.py` & `happy_learning-0.4.8/happy_learning/multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/neural_network_generator_torch.py` & `happy_learning-0.4.8/happy_learning/neural_network_generator_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
                     )
 
     def multi_layer_perceptron(self) -> MLP:
         """
         Generate Multi-Layer Perceptron (MLP) classifier parameter configuration randomly
 
         :return dict:
-            Configured Multi-Layer Perceptron (MLP) hyper parameter set
+            Configured Multi-Layer Perceptron (MLP) hyperparameter set
         """
         return MLP(input_size=len(self.predictors), output_size=self.output_size, parameters=self.model_param)
 
     def multi_layer_perceptron_param(self) -> dict:
         """
         Generate Multi-Layer Perceptron (MLP) classifier parameter configuration randomly
 
@@ -739,15 +739,15 @@
                 _activation_torch.update({_param_names[layer]: ACTIVATION['weighted_sum'][self.model_param.get('activation')](lambd=0.5 if self.model_param.get('lambd') is None else self.model_param.get('lambd'))})
             else:
                 self.model_param.update({_param_names[layer]: ACTIVATION['weighted_sum'][self.model_param.get('activation')]()})
         self.model_param.update(_activation_torch)
 
     def _config_hidden_layers(self):
         """
-        Configure hyper parameters of the hidden layers
+        Configure hyperparameters of the hidden layers
         """
         if self.hidden_layer_size_category is None:
             self.hidden_layer_size_category = np.random.choice(a=list(HIDDEN_LAYER_CATEGORY.keys()))
             _hidden_layer_size: tuple = HIDDEN_LAYER_CATEGORY.get(self.hidden_layer_size_category)
         else:
             _hidden_layer_size: tuple = HIDDEN_LAYER_CATEGORY.get(self.hidden_layer_size_category)
         if self.hidden_layer_size is None or self.hidden_layer_size <= 0:
@@ -764,15 +764,15 @@
     def _config_params(self,
                        loss: bool = False,
                        optimizer: bool = False,
                        activation: bool = False,
                        hidden_layers: bool = False
                        ):
         """
-        Finalize configuration of hyper parameter settings of the neural network
+        Finalize configuration of hyperparameter settings of the neural network
 
         :param loss: bool
             Configure loss function initially based on the size of the output layer
 
         :param optimizer: bool
             Configure optimizer
 
@@ -898,17 +898,16 @@
                         #patience=np.random.uniform(low=2, high=20),
                         dropout=np.random.uniform(low=0.05, high=0.95),
                         alpha_dropout=np.random.choice(a=[False, True]),
                         activation=np.random.choice(a=list(ACTIVATION['weighted_sum'].keys())),
                         optimizer=np.random.choice(a=list(OPTIMIZER.keys()))
                         )
         else:
-            return dict(embedding=dict(embedding_len=300,
-                                       embedding_model=np.random.choice(a=list(EMBEDDING.keys()))
-                                       )
+            return dict(embedding_len=300,
+                        embedding_model=np.random.choice(a=list(EMBEDDING.keys()))
                         )
 
     def _import_data_torch(self):
         """
         Import data sets (Training, Testing, Validation) from file
         """
         if self.learning_type == 'batch':
@@ -916,15 +915,15 @@
                 _unique_labels: list = pd.read_csv(filepath_or_buffer=self.train_data_path, sep=self.sep)[self.target].unique().tolist()
                 _data_fields: List[tuple] = []
                 self.embedding_text: Field = Field(sequential=True,
                                                    tokenize=lambda x: x.split(),
                                                    lower=True,
                                                    include_lengths=True,
                                                    batch_first=True,
-                                                   fix_length=300 if self.model_param.get('embedding_len') is None else self.model_param.get('embedding_len')
+                                                   fix_length=300 if self.model_param['embedding_len'] is None else self.model_param['embedding_len']
                                                    )
                 self.embedding_label: Field = Field(sequential=False, is_target=True, unk_token=None)
                 for predictor in self.predictors:
                     _data_fields.append((predictor, self.embedding_text))
                 _data_fields.append((self.target, self.embedding_label))
                 _train_data: TabularDataset = TabularDataset(path=self.train_data_path,
                                                              format='csv',
@@ -942,15 +941,15 @@
                 _validation_data: TabularDataset = TabularDataset(path=self.validation_data_path,
                                                                   format='csv',
                                                                   fields=_data_fields,
                                                                   skip_header=True
                                                                   )
                 if self.model_param.get('embedding_model') == 'fast_text':
                     self.embedding_text.build_vocab(_train_data,
-                                                    vectors=EMBEDDING[self.model_param.get('embedding_model')](language='de' if self.model_param.get('lang') is None else self.model_param.get('lang'))
+                                                    vectors=EMBEDDING['fast_text'](language='de' if self.model_param.get('lang') is None else self.model_param.get('lang'))
                                                     )
                 self.embedding_label.build_vocab(_train_data)
                 if 0 in _unique_labels:
                     for label in _unique_labels:
                         self.embedding_label.vocab.stoi.update({str(label): label})
                 else:
                     for label in _unique_labels:
@@ -1139,17 +1138,17 @@
                                                      validation_data_path=self.validation_data_path,
                                                      model_param=self.model_param,
                                                      **self.kwargs
                                                      ),
                                        '{}_param'.format(_model)
                                        )()
             self.model_param.update(self._get_param_space(general=True))
-            self._config_params(hidden_layers=True)
             if self.sequential_type == 'text':
-                self._config_params(natural_language=True)
+                self.model_param.update(self._get_param_space(general=False))
+            self._config_params(hidden_layers=True)
         else:
             self.model_param = copy.deepcopy(self.input_param)
         _idx: int = 0 if len(self.model_param_mutated.keys()) == 0 else len(self.model_param_mutated.keys()) + 1
         self.model_param_mutated.update({str(_idx): {copy.deepcopy(self.model_name): {}}})
         for param in list(self.model_param.keys()):
             self.model_param_mutated[str(_idx)][copy.deepcopy(self.model_name)].update({param: copy.deepcopy(self.model_param.get(param))})
         self.model_param_mutation = 'new_model'
@@ -1296,17 +1295,17 @@
                                                          test_data_path=self.test_data_path,
                                                          validation_data_path=self.validation_data_path,
                                                          **self.kwargs
                                                          ),
                                            '{}_param'.format(NETWORK_TYPE.get(self.model_name))
                                            )()
                 self.model_param.update(self._get_param_space(general=True))
-                self.model_param.update(learning_rate=0.001)
                 if self.sequential_type == 'text':
-                    self._config_params(natural_language=True)
+                    self.model_param.update(self._get_param_space(general=False))
+                self.model_param.update(learning_rate=0.001)
             else:
                 self.model_param = copy.deepcopy(self.input_param)
             if len(self.predictors) > 0:
                 if self.target != '':
                     self._import_data_torch()
                 else:
                     raise NeuralNetworkException('No target feature found')
```

### Comparing `happy_learning-0.4.7/happy_learning/neural_network_torch.py` & `happy_learning-0.4.8/happy_learning/neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/sampler.py` & `happy_learning-0.4.8/happy_learning/sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/self_taught_short_text_clustering.py` & `happy_learning-0.4.8/happy_learning/self_taught_short_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/supervised_machine_learning.py` & `happy_learning-0.4.8/happy_learning/supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/swarm_intelligence.py` & `happy_learning-0.4.8/happy_learning/swarm_intelligence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1510,136 +1510,130 @@
                 _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
                 _best_model_results['rel_diff'] = _best_model_results['obs'] / _best_model_results['pred']
             elif self.target_type == 'clf_multi':
                 _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
             _best_model_results = _best_model_results.round(decimals=4)
             if self.target_type == 'reg':
                 _file_paths.append(os.path.join(self.output_file_path, 'evaluation_coords.html'))
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction Evaluation of final inherited ML Model:',
+                               features=['obs', 'abs_diff', 'rel_diff', 'pred'],
+                               color_feature='pred',
+                               plot_type='parcoords',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'evaluation_coords.html'),
+                               ).run()
                 _file_paths.append(os.path.join(self.output_file_path, 'scatter_contour.html'))
-                _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                           features=['obs', 'abs_diff',
-                                                                                                     'rel_diff', 'pred'],
-                                                                                           color_feature='pred',
-                                                                                           plot_type='parcoords',
-                                                                                           file_path=_file_paths[0],
-                                                                                           kwargs=dict(layout={})
-                                                                                           ),
-                                'Prediction vs. Observation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                                features=['obs', 'pred'],
-                                                                                                plot_type='joint',
-                                                                                                file_path=_file_paths[1],
-                                                                                                kwargs=dict(layout={})
-                                                                                                )
-                                })
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction vs. Observation of final inherited ML Model:',
+                               features=['obs', 'pred'],
+                               plot_type='joint',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'scatter_contour.html'),
+                               ).run()
             else:
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
-                _file_paths.append(os.path.join(self.output_file_path, 'clf_metrics_table.html'))
                 _eval_clf: EvalClf = EvalClf(obs=self.data_set.get('y_test'),
                                              pred=self.data_set.get('pred'),
                                              labels=self.target_labels
                                              )
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=_eval_clf.confusion(),
                                                                index=[f'{label}_obs' for label in self.target_labels],
                                                                columns=[f'{label}_pred' for label in self.target_labels]
                                                                )
                 _cf_row_sum = pd.DataFrame()
                 _cf_row_sum[' '] = _confusion_matrix.sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_row_sum.transpose()], axis=0)
                 _cf_col_sum = pd.DataFrame()
                 _cf_col_sum[' '] = _confusion_matrix.transpose().sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_col_sum], axis=1)
-                _charts.update({'Confusion Matrix': dict(data=_confusion_matrix,
-                                                         plot_type='table',
-                                                         file_path=_file_paths[0],
-                                                         kwargs=dict(layout={})
-                                                         )
-                                })
-                _charts.update({'Confusion Matrix Heatmap': dict(data=_best_model_results,
-                                                                 features=['obs', 'pred'],
-                                                                 plot_type='heat',
-                                                                 file_path=_file_paths[1],
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_table.html'))
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_table.html'),
+                               ).run()
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_heatmap.html'))
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix Heatmap:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_heatmap.html'),
+                               ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
                                                                           # index=['obs', 'pred'],
                                                                           # columns=['obs', 'pred']
                                                                           )
-                _charts.update({'Confusion Matrix Normalized Heatmap:': dict(data=_confusion_matrix_normalized,
-                                                                             features=self.target_labels,
-                                                                             plot_type='heat',
-                                                                             file_path=_file_paths[2],
-                                                                             kwargs=dict(layout={})
-                                                                             )
-                                })
-                _charts.update({'Classification Report:': dict(data=_best_model_results,
-                                                               plot_type='table',
-                                                               file_path=_file_paths[3],
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'confusion_normal_heatmap.html'))
+                DataVisualizer(df=_confusion_matrix_normalized,
+                               title='Confusion Matrix Normalized Heatmap:',
+                               features=_confusion_matrix_normalized.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'confusion_normal_heatmap.html'),
+                               ).run()
+                _file_paths.append(os.path.join(self.output_file_path, 'clf_report_table.html'))
+                DataVisualizer(df=_best_model_results,
+                               title='Classification Report:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'clf_report_table.html'),
+                               ).run()
                 _classification_report: dict = _eval_clf.classification_report()
                 _confusion_metrics: dict = dict(precision=[], recall=[], f1=[])
                 for label in self.target_labels:
                     _confusion_metrics['precision'].append(_classification_report.get(label)['precision'])
                     _confusion_metrics['recall'].append(_classification_report.get(label)['recall'])
                     _confusion_metrics['f1'].append(_classification_report.get(label)['f1-score'])
-                _charts.update({'Classification Metrics': dict(data=pd.DataFrame(data=_confusion_metrics,
-                                                                                 index=self.target_labels,
-                                                                                 columns=list(_confusion_metrics.keys())
-                                                                                 ),
-                                                               plot_type='table',
-                                                               file_path=_file_paths[4],
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                _file_paths.append(os.path.join(self.output_file_path, 'clf_metrics_table.html'))
+                _clf_metrics: pd.DataFrame = pd.DataFrame(data=_confusion_metrics,
+                                                          index=self.target_labels,
+                                                          columns=list(_confusion_metrics.keys())
+                                                          )
+                DataVisualizer(df=_clf_metrics,
+                               title='Classification Metrics:',
+                               features=_clf_metrics.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'clf_metrics_table.html'),
+                               ).run()
                 if self.target_type == 'clf_multi':
                     _file_paths.append(os.path.join(self.output_file_path, 'evaluation_category.html'))
-                    _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                               features=['obs', 'abs_diff',
-                                                                                                         'pred'],
-                                                                                               color_feature='pred',
-                                                                                               plot_type='parcoords',
-                                                                                               file_path=_file_paths[-1],
-                                                                                               kwargs=dict(layout={})
-                                                                                               )
-                                    })
+                    DataVisualizer(df=_best_model_results,
+                                   title='Prediction Evaluation of final inherited ML Model:',
+                                   features=['obs', 'abs_diff', 'pred'],
+                                   color_feature='pred',
+                                   plot_type='parcoords',
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'evaluation_category.html'),
+                                   ).run()
                 else:
-                    _file_paths.append(os.path.join(self.output_file_path, 'roc_auc_curve_baseline_baseline_baseline_baseline.html'))
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
                     _roc_curve['baseline'] = _roc_curve_values['false_positive_rate'][1]
-                    _charts.update({'ROC-AUC Curve': dict(data=_roc_curve,
-                                                          features=['roc_curve', 'baseline'],
-                                                          time_features=['baseline'],
-                                                          # xaxis_label=['False Positive Rate'],
-                                                          # yaxis_label=['True Positive Rate'],
-                                                          melt=True,
-                                                          plot_type='line',
-                                                          use_auto_extensions=False,
-                                                          file_path=_file_paths[-1],
-                                                          kwargs=dict(layout={})
-                                                          )
-                                    })
-            DataVisualizer(subplots=_charts,
-                           interactive=True,
-                           file_path=self.output_file_path,
-                           render=True if self.output_file_path is None else False,
-                           height=750,
-                           width=750,
-                           unit='px'
-                           ).run()
+                    _file_paths.append(os.path.join(self.output_file_path, 'roc_auc_curve.html'))
+                    DataVisualizer(df=_roc_curve,
+                                   title='ROC-AUC Curve:',
+                                   features=['roc_curve', 'baseline'],
+                                   time_features=['baseline'],
+                                   plot_type='line',
+                                   # xaxis_label=['False Positive Rate'],
+                                   # yaxis_label=['True Positive Rate'],
+                                   use_auto_extensions=False,
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'roc_auc_curve.html'),
+                                   ).run()
             for path in _file_paths:
                 _file_name: str = path.split('/')[-1].replace('.html', '')
                 try:
                     mlflow.log_artifact(local_path=path, artifact_path=_file_name)
                 except FileNotFoundError:
                     Log(write=self.log, logger_file_path=self.output_file_path).log(f'File artifact {path} not found')
 
@@ -1791,27 +1785,27 @@
                        si: bool = True,
                        model: bool = True,
                        evolution_history: bool = False,
                        adjustment_history: bool = False,
                        final_adjustment: bool = False
                        ):
         """
-        Save evolution meta data generated by genetic algorithm to local hard drive as pickle file
+        Save evolution metadata generated by genetic algorithm to local hard drive as pickle file
 
         :param si: bool
             Save SwarmIntelligence class object (required for continuing evolution / optimization)
 
         :param model: bool
             Save evolved model
 
         :param evolution_history: bool
-            Save evolution history meta data
+            Save evolution history metadata
 
         :param adjustment_history: bool
-            Save adjustment history meta data
+            Save adjustment history metadata
 
         :param final_adjustment: bool
             Save settings of each individual of final adjustment
         """
         # Export evolution history data:
         if evolution_history:
             DataExporter(obj=self.evolution_history,
@@ -1843,18 +1837,15 @@
                          ).file()
         # Export evolved model:
         if model:
             _file_name_extension: str = '' if self.kwargs.get('model_file_name_extension') is None else '_{}'.format(self.kwargs.get('model_file_name_extension'))
             _file_name: str = 'model{}.p'.format(_file_name_extension)
             if self.cloud is None:
                 if self.deep_learning:
-                    if self.current_adjustment_meta_data['model_name'][self.best_global_idx] == 'trans':
-                        torch.save(obj=self.model.model, f=os.path.join(self.output_file_path, _file_name))
-                    else:
-                        torch.save(obj=self.model, f=os.path.join(self.output_file_path, _file_name))
+                    torch.save(obj=self.model, f=os.path.join(self.output_file_path, _file_name))
                 else:
                     DataExporter(obj=self.model,
                                  file_path=os.path.join(self.output_file_path, _file_name),
                                  create_dir=False,
                                  overwrite=True
                                  ).file()
             else:
@@ -1874,44 +1865,45 @@
                                  overwrite=True,
                                  cloud=self.cloud,
                                  bucket_name=self.bucket_name,
                                  region=self.kwargs.get('region')
                                  ).file()
         # Export SwarmIntelligence class object:
         if si:
-            if self.stopping_reason is None:
-                self.feature_engineer = None
-            else:
-                self.df = None
-                self.model = None
-                self.population = []
-                self.feature_engineer = None
-            _file_name_extension: str = '' if self.kwargs.get('si_file_name_extension') is None else '_{}'.format(self.kwargs.get('si_file_name_extension'))
-            _file_name: str = 'swarm{}.p'.format(_file_name_extension)
-            DataExporter(obj=self,
-                         file_path=os.path.join(self.output_file_path, _file_name),
-                         create_dir=False,
-                         overwrite=True,
-                         cloud=self.cloud,
-                         bucket_name=self.bucket_name,
-                         region=self.kwargs.get('region')
-                         ).file()
+            if not self.deep_learning:
+                if self.stopping_reason is None:
+                    self.feature_engineer = None
+                else:
+                    self.df = None
+                    self.model = None
+                    self.population = []
+                    self.feature_engineer = None
+                _file_name_extension: str = '' if self.kwargs.get('si_file_name_extension') is None else '_{}'.format(self.kwargs.get('si_file_name_extension'))
+                _file_name: str = 'swarm{}.p'.format(_file_name_extension)
+                DataExporter(obj=self,
+                             file_path=os.path.join(self.output_file_path, _file_name),
+                             create_dir=False,
+                             overwrite=True,
+                             cloud=self.cloud,
+                             bucket_name=self.bucket_name,
+                             region=self.kwargs.get('region')
+                             ).file()
 
     def visualize(self,
                   results_table: bool = True,
                   model_distribution: bool = False,
                   model_evolution: bool = True,
                   param_distribution: bool = False,
                   train_time_distribution: bool = True,
                   breeding_map: bool = False,
                   breeding_graph: bool = False,
                   fitness_distribution: bool = True,
                   fitness_evolution: bool = True,
                   fitness_dimensions: bool = True,
-                  per_adjustment: bool = True,
+                  per_generation: bool = True,
                   prediction_of_best_model: bool = True,
                   epoch_stats: bool = True
                   ):
         """
         Visualize evolutionary activity
 
         :param results_table: bool
@@ -1951,248 +1943,245 @@
                 -> Line Chart
 
         :param fitness_dimensions: bool
             Calculated loss value for each dimension in fitness metric
                 -> Radar Chart
                 -> Tree Map
 
-        :param per_adjustment: bool
-            Visualize results of each adjustment in detail or visualize just evolutionary results
+        :param per_generation: bool
+            Visualize results of each generation in detail or visualize just evolutionary results
 
         :param prediction_of_best_model: bool
             Evaluation of prediction of the fittest model of evolution
                 -> Parallel Coordinate Chart
                 -> Joint Chart
 
         :param epoch_stats: bool
             Visualize train and validation error for each training epoch (deep learning only)
         """
-        _charts: dict = {}
         _evolution_history_data: pd.DataFrame = pd.DataFrame(data=self.evolution_history)
         _m: List[str] = ['fitness_score', 'ml_metric', 'train_test_diff']
         _evolution_history_data[_m] = _evolution_history_data[_m].round(decimals=2)
         _evolution_gradient_data: pd.DataFrame = pd.DataFrame(data=self.evolution_gradient)
-        _evolution_gradient_data['adjustment'] = [i for i in range(0, len(self.evolution_gradient.get('max')), 1)]
+        _evolution_gradient_data['generation'] = [i for i in range(0, len(self.evolution_gradient.get('max')), 1)]
         _best_model_results: pd.DataFrame = pd.DataFrame(data=dict(obs=self.data_set.get('y_test'),
                                                                    pred=self.data_set.get('pred')
                                                                    )
                                                          )
         if self.target_type == 'reg':
             _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
             _best_model_results['rel_diff'] = _best_model_results['obs'] / _best_model_results['pred']
         elif self.target_type == 'clf_multi':
             _best_model_results['abs_diff'] = _best_model_results['obs'] - _best_model_results['pred']
         _best_model_results = _best_model_results.round(decimals=4)
         if results_table:
-            _charts.update({'Results of Genetic Algorithm:': dict(data=_evolution_history_data,
-                                                                  plot_type='table',
-                                                                  file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_metadata_table.html'),
-                                                                  kwargs=dict(layout={})
-                                                                  )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Results of Genetic Algorithm:',
+                           features=_evolution_history_data.columns.to_list(),
+                           plot_type='table',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_metadata_table.html'),
+                           ).run()
         if model_evolution:
-            _charts.update({'Evolution of used ML Models:': dict(data=_evolution_history_data,
-                                                                 features=['fitness_score', 'adjustment'],
-                                                                 color_feature='model',
-                                                                 plot_type='scatter',
-                                                                 melt=True,
-                                                                 file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_model_evolution.html'),
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Evolution of used ML Models:',
+                           features=['fitness_score', 'generation'],
+                           color_feature='model',
+                           plot_type='scatter',
+                           melt=True,
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_model_evolution.html'),
+                           ).run()
         if model_distribution:
             if self.models is None or len(self.models) > 1:
-                _charts.update({'Distribution of used ML Models:': dict(data=_evolution_history_data,
-                                                                        features=['model'],
-                                                                        group_by=['adjustment'] if per_adjustment else None,
-                                                                        plot_type='pie',
-                                                                        file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_model_distribution.html'),
-                                                                        kwargs=dict(layout={})
-                                                                        )
-                                })
-        #if param_distribution:
+                DataVisualizer(df=_evolution_history_data,
+                               title='Distribution of used ML Models:',
+                               features=['model'],
+                               group_by=['generation'] if per_generation else None,
+                               plot_type='pie',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_model_distribution.html'),
+                               ).run()
+        # if param_distribution:
         #    _charts.update({'Distribution of ML Model parameters:': dict(data=_evolution_history_data,
         #                                                                 features=['model_param'],
-        #                                                                 group_by=['adjustment'] if per_adjustment else None,
+        #                                                                 group_by=['generation'] if per_generation else None,
         #                                                                 plot_type='tree',
-        #                                                                 file_path=self.output_file_path if self.output_file_path is None else '{}{}'.format(self.output_file_path, 'si_parameter_treemap.html')
+        #                                                                 file_path=self.output_file_path if self.output_file_path is None else '{}{}'.format(self.output_file_path, 'ga_parameter_treemap.html')
         #                                                                 )
         #                    })
         if train_time_distribution:
-            _charts.update({'Distribution of elapsed Training Time:': dict(data=_evolution_history_data,
-                                                                           features=['train_time_in_seconds'],
-                                                                           group_by=['model'],
-                                                                           plot_type='violin',
-                                                                           melt=False,
-                                                                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_training_time_distribution.html'),
-                                                                           kwargs=dict(layout={})
-                                                                           )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Distribution of elapsed Training Time:',
+                           features=['train_time_in_seconds'],
+                           group_by=['model'],
+                           melt=True,
+                           plot_type='violin',
+                           use_auto_extensions=False,
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_training_time_distribution.html'),
+                           ).run()
         if breeding_map:
-            _breeding_map: pd.DataFrame = pd.DataFrame(data=dict(adjustment_0=self.adjustment_history['population']['adjustment_0'].get('fitness')), index=[0])
-            for g in self.adjustment_history['population'].keys():
-                if g != 'adjustment_0':
-                    _breeding_map[g] = self.adjustment_history['population'][g].get('fitness')
-            _charts.update({'Breeding Heat Map:': dict(data=_breeding_map,
-                                                       plot_type='heat',
-                                                       file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_breeding_heatmap.html'),
-                                                       kwargs=dict(layout={})
-                                                       )
-                            })
+            _breeding_map: pd.DataFrame = pd.DataFrame(
+                data=dict(gen_0=self.generation_history['population']['gen_0'].get('fitness')), index=[0])
+            for g in self.generation_history['population'].keys():
+                if g != 'gen_0':
+                    _breeding_map[g] = self.generation_history['population'][g].get('fitness')
+            DataVisualizer(df=_breeding_map,
+                           title='Breeding Heat Map:',
+                           features=_breeding_map.columns.to_list(),
+                           plot_type='heat',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_breeding_heatmap.html'),
+                           ).run()
         if breeding_graph:
-            _charts.update({'Breeding Network Graph:': dict(data=_evolution_history_data,
-                                                            features=['adjustment', 'fitness_score'],
-                                                            graph_features=dict(node='id', edge='best'),
-                                                            color_feature='model',
-                                                            plot_type='network',
-                                                            file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_breeding_graph.html'),
-                                                            kwargs=dict(layout={})
-                                                            )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Breeding Network Graph:',
+                           features=['generation', 'fitness_score'],
+                           graph_features=dict(node='id', edge='parent'),
+                           color_feature='model',
+                           plot_type='network',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_breeding_graph.html'),
+                           ).run()
         if fitness_distribution:
-            _charts.update({'Distribution of Fitness Metric:': dict(data=_evolution_history_data,
-                                                                    features=['fitness_score'],
-                                                                    time_features=['adjustment'],
-                                                                    plot_type='ridgeline',
-                                                                    file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_fitness_score_distribution_per_adjustment.html'),
-                                                                    kwargs=dict(layout={})
-                                                                    )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Distribution of Fitness Metric:',
+                           features=['fitness_score'],
+                           time_features=['generation'],
+                           plot_type='ridgeline',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_fitness_score_distribution_per_generation.html'),
+                           ).run()
         if fitness_dimensions:
-            _charts.update({'Evolution Meta Data:': dict(data=_evolution_history_data,
-                                                         features=['train_time_in_seconds',
-                                                                   'ml_metric',
-                                                                   'train_test_diff',
-                                                                   'fitness_score',
-                                                                   'best',
-                                                                   'id',
-                                                                   'adjustment',
-                                                                   'model'
-                                                                   ],
-                                                         color_feature='model',
-                                                         plot_type='parcoords',
-                                                         file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_metadata_evolution_coords.html'),
-                                                         kwargs=dict(layout={})
-                                                         )
-                            })
+            DataVisualizer(df=_evolution_history_data,
+                           title='Evolution Meta Data:',
+                           features=['train_time_in_seconds',
+                                     'ml_metric',
+                                     'train_test_diff',
+                                     'fitness_score',
+                                     'parent',
+                                     'id',
+                                     'generation',
+                                     'model'
+                                     ],
+                           color_feature='model',
+                           plot_type='parcoords',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_metadata_evolution_coords.html'),
+                           ).run()
         if fitness_evolution:
-            _charts.update({'Fitness Evolution:': dict(data=_evolution_gradient_data,
-                                                       features=['min', 'median', 'mean', 'max'],
-                                                       time_features=['adjustment'],
-                                                       melt=True,
-                                                       plot_type='line',
-                                                       file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_evolution_fitness_score.html'),
-                                                       kwargs=dict(layout={})
-                                                       )
-                            })
+            DataVisualizer(df=_evolution_gradient_data,
+                           title='Fitness Evolution:',
+                           features=['min', 'median', 'mean', 'max'],
+                           time_features=['generation'],
+                           melt=True,
+                           plot_type='line',
+                           file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                               self.output_file_path, 'si_evolution_fitness_score.html'),
+                           ).run()
         if epoch_stats:
             if self.deep_learning:
                 _epoch_metric_score: pd.DataFrame = pd.DataFrame(data=self.evolution.get('epoch_metric_score'))
                 _epoch_metric_score['epoch'] = [epoch + 1 for epoch in range(0, _epoch_metric_score.shape[0], 1)]
-                print(_epoch_metric_score)
-                _charts.update({'Epoch Evaluation of fittest neural network': dict(data=_epoch_metric_score,
-                                                                                   features=['train', 'val'],
-                                                                                   time_features=['epoch'],
-                                                                                   plot_type='line',
-                                                                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_epoch_metric_score.html'),
-                                                                                   kwargs=dict(layout={})
-                                                                                   )
-                                })
+                DataVisualizer(df=_epoch_metric_score,
+                               title='Epoch Evaluation of fittest neural network:',
+                               features=['train', 'val'],
+                               time_features=['epoch'],
+                               melt=True,
+                               plot_type='line',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_epoch_metric_score.html'),
+                               ).run()
         if prediction_of_best_model:
             if self.target_type == 'reg':
-                _charts.update({'Prediction Evaluation of final adjusted ML Model:': dict(data=_best_model_results,
-                                                                                          features=['obs', 'abs_diff', 'rel_diff', 'pred'],
-                                                                                          color_feature='pred',
-                                                                                          plot_type='parcoords',
-                                                                                          file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_evaluation_coords.html'),
-                                                                                          kwargs=dict(layout={})
-                                                                                          ),
-                                'Prediction vs. Observation of final adjusted ML Model:': dict(data=_best_model_results,
-                                                                                               features=['obs', 'pred'],
-                                                                                               plot_type='joint',
-                                                                                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_scatter_contour.html'),
-                                                                                               kwargs=dict(layout={})
-                                                                                               )
-                                })
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction Evaluation of final inherited ML Model:',
+                               features=['obs', 'abs_diff', 'rel_diff', 'pred'],
+                               color_feature='pred',
+                               plot_type='parcoords',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_evaluation_coords.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Prediction vs. Observation of final inherited ML Model:',
+                               features=['obs', 'pred'],
+                               plot_type='joint',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_scatter_contour.html'),
+                               ).run()
             else:
                 _confusion_matrix: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                             pred=self.data_set.get('pred')
                                                                             ).confusion(),
                                                                index=self.target_labels,
                                                                columns=self.target_labels
                                                                )
                 _cf_row_sum = pd.DataFrame()
                 _cf_row_sum[' '] = _confusion_matrix.sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_row_sum.transpose()], axis=0)
                 _cf_col_sum = pd.DataFrame()
                 _cf_col_sum[' '] = _confusion_matrix.transpose().sum()
                 _confusion_matrix = pd.concat([_confusion_matrix, _cf_col_sum], axis=1)
-                _charts.update({'Confusion Matrix': dict(data=_confusion_matrix,
-                                                         plot_type='table',
-                                                         file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_confusion_table.html'),
-                                                         kwargs=dict(layout={})
-                                                         )
-                                })
-                _charts.update({'Confusion Matrix Heatmap': dict(data=_best_model_results,
-                                                                 features=['obs', 'pred'],
-                                                                 plot_type='heat',
-                                                                 file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_confusion_heatmap.html'),
-                                                                 kwargs=dict(layout={})
-                                                                 )
-                                })
+                DataVisualizer(df=_confusion_matrix,
+                               title='Confusion Matrix:',
+                               features=_confusion_matrix.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_confusion_table.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Confusion Matrix Heatmap:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_confusion_heatmap.html'),
+                               ).run()
                 _confusion_matrix_normalized: pd.DataFrame = pd.DataFrame(data=EvalClf(obs=self.data_set.get('y_test'),
                                                                                        pred=self.data_set.get('pred')
                                                                                        ).confusion(normalize='pred'),
-                                                                          #index=['obs', 'pred'],
-                                                                          #columns=['obs', 'pred']
+                                                                          index=self.target_labels,
+                                                                          columns=self.target_labels
                                                                           )
-                _charts.update({'Confusion Matrix Normalized Heatmap:': dict(data=_confusion_matrix_normalized,
-                                                                             features=self.target_labels,
-                                                                             plot_type='heat',
-                                                                             file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_confusion_normal_heatmap.html'),
-                                                                             kwargs=dict(layout={})
-                                                                             )
-                                })
-                _charts.update({'Classification Report:': dict(data=_best_model_results,
-                                                               plot_type='table',
-                                                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_clf_report_table.html'),
-                                                               kwargs=dict(layout={})
-                                                               )
-                                })
+                DataVisualizer(df=_confusion_matrix_normalized,
+                               title='Confusion Matrix Normalized Heatmap:',
+                               features=_confusion_matrix_normalized.columns.to_list(),
+                               plot_type='heat',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_confusion_normal_heatmap.html'),
+                               ).run()
+                DataVisualizer(df=_best_model_results,
+                               title='Classification Report:',
+                               features=_best_model_results.columns.to_list(),
+                               plot_type='table',
+                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                   self.output_file_path, 'si_prediction_clf_report_table.html'),
+                               ).run()
                 if self.target_type == 'clf_multi':
-                    _charts.update({'Prediction Evaluation of final inherited ML Model:': dict(data=_best_model_results,
-                                                                                               features=['obs', 'abs_diff', 'pred'],
-                                                                                               color_feature='pred',
-                                                                                               plot_type='parcoords',
-                                                                                               brushing=True,
-                                                                                               file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_evaluation_category.html'),
-                                                                                               kwargs=dict(layout={})
-                                                                                               )
-                                    })
+                    DataVisualizer(df=_best_model_results,
+                                   title='Prediction Evaluation of final inherited ML Model:',
+                                   features=['obs', 'abs_diff', 'pred'],
+                                   color_feature='pred',
+                                   plot_type='parcoords',
+                                   brushing=True,
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'si_prediction_evaluation_category.html'),
+                                   ).run()
                 else:
                     _roc_curve = pd.DataFrame()
                     _roc_curve_values: dict = EvalClf(obs=_best_model_results['obs'],
                                                       pred=_best_model_results['pred']
                                                       ).roc_curve()
                     _roc_curve['roc_curve'] = _roc_curve_values['true_positive_rate'][1]
                     _roc_curve['baseline'] = _roc_curve_values['false_positive_rate'][1]
-                    _charts.update({'ROC-AUC Curve': dict(data=_roc_curve,
-                                                          features=['roc_curve', 'baseline'],
-                                                          time_features=['baseline'],
-                                                          #xaxis_label=['False Positive Rate'],
-                                                          #yaxis_label=['True Positive Rate'],
-                                                          melt=True,
-                                                          plot_type='line',
-                                                          use_auto_extensions=False,
-                                                          file_path=self.output_file_path if self.output_file_path is None else os.path.join(self.output_file_path, 'si_prediction_roc_auc_curve.html'),
-                                                          kwargs=dict(layout={})
-                                                          )
-                                    })
-        if len(_charts.keys()) > 0:
-            DataVisualizer(subplots=_charts,
-                           interactive=True,
-                           file_path=self.output_file_path,
-                           render=True if self.output_file_path is None else False,
-                           height=750,
-                           width=750,
-                           unit='px'
-                           ).run()
+                    DataVisualizer(df=_roc_curve,
+                                   title='ROC-AUC Curve:',
+                                   features=['roc_curve', 'baseline'],
+                                   time_features=['baseline'],
+                                   plot_type='line',
+                                   melt=True,
+                                   use_auto_extensions=False,
+                                   # xaxis_label=['False Positive Rate'],
+                                   # yaxis_label=['True Positive Rate'],
+                                   file_path=self.output_file_path if self.output_file_path is None else os.path.join(
+                                       self.output_file_path, 'si_prediction_roc_auc_curve.html'),
+                                   ).run()
```

### Comparing `happy_learning-0.4.7/happy_learning/text_clustering.py` & `happy_learning-0.4.8/happy_learning/text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/text_clustering_generator.py` & `happy_learning-0.4.8/happy_learning/text_clustering_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from .evaluate_machine_learning import EvalClf, EvalCluster
 from .self_taught_short_text_clustering import get_sentence_embedding, STC
 from .text_clustering import GibbsSamplingDirichletMultinomialModeling, LatentDirichletAllocation, \
     LatentSemanticIndexing, NonNegativeMatrixFactorization
 from datetime import datetime
 from easyexplore.data_import_export import CLOUD_PROVIDER, DataImporter
 from gensim import corpora
-from simpletransformers.model import ClassificationModel
 from torch.utils.data import TensorDataset, DataLoader
 from typing import List
 
 CLUSTER_ALGORITHMS: dict = dict(gsdmm='gibbs_sampling_dirichlet_multinomial_modeling',
                                 lda='latent_dirichlet_allocation',
                                 lsi='latent_semantic_indexing',
                                 nmf='non_negative_matrix_factorization',
@@ -443,48 +442,14 @@
             _data_tensor: TensorDataset = TensorDataset(_embedding_tensor, _target_tensor)
             _batch_size: int = 16 if self.cluster_params.get('batch_size') is None else self.cluster_params.get('batch_size')
             _data_loader: DataLoader = DataLoader(dataset=_data_tensor, batch_size=_batch_size, shuffle=True)
             self.cluster_params.update({'dimensions': [_embedding.shape[0], _embedding.shape[1]], 'iterator': _data_loader})
             self.stc = self.self_taught_short_text_clustering()
             self.stc.fit(x=_embedding_tensor)
             self.fitness = self.stc.nmi_score
-        elif self.eval_method == 'trans':
-            _df_train: pd.DataFrame = pd.DataFrame(data=dict(text=np.array(self.x), label=self.cluster_label))
-            _args: dict = dict(do_lower_case=True,
-                               evaluate_during_training=False,
-                               manual_seed=1234,
-                               no_save=True,
-                               no_cache=False,
-                               overwrite_output_dir=True,
-                               silent=True
-                               )
-            _kwargs: dict = dict(cache_dir=self.language_model_path, local_files_only=False if self.language_model_path is None else True)
-            _model_type: str = 'xlm' if self.language_model_path is None else self.language_model_path.split('/')[-2].split('-')[0]
-            _transformer = ClassificationModel(model_type=_model_type,
-                                               model_name='xlm-roberta-large' if self.language_model_path is None else self.language_model_path,
-                                               tokenizer_type=None,
-                                               tokenizer_name=None,
-                                               num_labels=len(list(set(self.cluster_label))),
-                                               weight=None,
-                                               args=_args,
-                                               use_cuda=torch.cuda.is_available(),
-                                               cuda_device=0 if torch.cuda.is_available() else -1,
-                                               onnx_execution_provider=None,
-                                               **_kwargs
-                                               )
-            _transformer.train_model(train_df=_df_train,
-                                     multi_label=False,
-                                     output_dir=None,
-                                     show_running_loss=False,
-                                     eval_df=None,
-                                     verbose=False
-                                     )
-            _predictions, _raw_output = _transformer.predict(to_predict=_df_train['text'].values.tolist())
-            self.fitness = EvalClf(obs=self.cluster_label, pred=_predictions.tolist()).roc_auc_multi(meth='ovr')
-            del _df_train, _predictions, _raw_output
         self.fitness_score = self.fitness
 
     def _import_data(self):
         """
         Import data set
         """
         if self.df is None:
```

### Comparing `happy_learning-0.4.7/happy_learning/text_miner.py` & `happy_learning-0.4.8/happy_learning/text_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning/utils.py` & `happy_learning-0.4.8/happy_learning/utils.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/happy_learning.egg-info/PKG-INFO` & `happy_learning-0.4.8/happy_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy-learning
-Version: 0.4.7
+Version: 0.4.8
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `happy_learning-0.4.7/happy_learning.egg-info/SOURCES.txt` & `happy_learning-0.4.8/happy_learning.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 happy_learning/data_miner.py
 happy_learning/deep_q_learning.py
 happy_learning/environment_modeling.py
 happy_learning/evaluate_machine_learning.py
 happy_learning/feature_engineer.py
 happy_learning/feature_learning.py
 happy_learning/feature_selector.py
-happy_learning/feature_tournament.py
 happy_learning/genetic_algorithm.py
 happy_learning/missing_data_analysis.py
 happy_learning/multiple_imputation.py
 happy_learning/neural_network_generator_torch.py
 happy_learning/neural_network_torch.py
 happy_learning/sampler.py
 happy_learning/self_taught_short_text_clustering.py
@@ -35,15 +34,14 @@
 test/test_data_miner.py
 test/test_deep_q_learning.py
 test/test_environment_modeling.py
 test/test_evaluate_machine_learning.py
 test/test_feature_engineer.py
 test/test_feature_learning.py
 test/test_feature_selector.py
-test/test_feature_tournament.py
 test/test_genetic_algorithm.py
 test/test_missing_data_analysis.py
 test/test_multiple_imputation.py
 test/test_neural_network_generator_torch.py
 test/test_neural_network_torch.py
 test/test_sampler.py
 test/test_self_taught_short_clustering.py
```

### Comparing `happy_learning-0.4.7/setup.py` & `happy_learning-0.4.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import setuptools
 import subprocess
 import sys
 
 #from happy_learning.text_miner import LANG_MODELS
 
-# Install complete dask library for handling big data sets using parallel computing:
-#subprocess.run(['python{} -m pip install "dask[distributed]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
-#subprocess.run(['python{} -m pip install "dask[complete]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
-
-# Install jupyter notebook extensions:
-#subprocess.run(['python{} -m pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
-
 # Install spacy language models:
 #subprocess.run('python{} -m pip install spacy'.format('3' if sys.platform.find('win') != 0 else ''), shell=True)
 #for lang in LANG_MODELS.keys():
 #    for model in LANG_MODELS[lang]['model']['spacy'].keys():
 #        subprocess.run('python{} -m spacy download {}'.format('3' if sys.platform.find('win') != 0 else '',
 #                                                              LANG_MODELS[lang]['model']['spacy'][model]
 #                                                              ),
@@ -26,15 +19,15 @@
 with open('requirements.txt', 'r') as _requirements:
     requires = _requirements.read()
 
 requires = [r.strip() for r in requires.split('\n') if ((r.strip()[0] != "#") and (len(r.strip()) > 3) and "-e git://" not in r)]
 
 setuptools.setup(
     name='happy_learning',
-    version='0.4.7',
+    version='0.4.8',
     author='Gianni Francesco Balistreri',
     author_email='gbalistreri@gmx.de',
     description='Toolbox for reinforced developing of machine learning models (as proof-of-concept)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch',
     license='GNU',
@@ -53,15 +46,14 @@
                          'test/test_data_miner.py',
                          'test/test_deep_q_learning.py',
                          'test/test_environment_modeling.py',
                          'test/test_evaluate_machine_learning.py',
                          'test/test_feature_engineer.py',
                          'test/test_feature_learning.py',
                          'test/test_feature_selector.py',
-                         'test/test_feature_tournament.py',
                          'test/test_genetic_algorithm.py',
                          'test/test_missing_data_analysis.py',
                          'test/test_multiple_imputation.py',
                          'test/test_neural_network_generator_torch.py',
                          'test/test_neural_network_torch.py',
                          'test/test_sampler.py',
                          'test/test_self_taught_short_clustering.py',
```

### Comparing `happy_learning-0.4.7/test/test_data_miner.py` & `happy_learning-0.4.8/test/test_data_miner.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,34 +2,41 @@
 import pandas as pd
 import unittest
 
 from happy_learning.data_miner import DataMiner
 from happy_learning.feature_engineer import FeatureEngineer
 from typing import List
 
+TEMP_DIR: str = 'data'
 DATA_SET: pd.DataFrame = pd.read_csv(filepath_or_buffer='data/avocado.csv')
 
 
 class DataMinerTest(unittest.TestCase):
     """
     Class for testing class DataMiner
     """
     def test_supervised_clf(self):
-        _feature_engineer: FeatureEngineer = FeatureEngineer(df=DATA_SET, target_feature='type')
+        _feature_engineer: FeatureEngineer = FeatureEngineer(temp_dir=TEMP_DIR,
+                                                             df=DATA_SET,
+                                                             target_feature='type'
+                                                             )
         _feature_engineer.set_predictors(exclude_original_data=False)
-        DataMiner(df=_feature_engineer.get_data(dask_df=True),
+        DataMiner(temp_dir=TEMP_DIR,
+                  df=_feature_engineer.get_data(dask_df=True),
                   file_path=None,
                   target=_feature_engineer.get_target(),
                   predictors=_feature_engineer.get_predictors(),
                   feature_engineer=_feature_engineer,
                   feature_generator=True,
                   train_critic=True,
                   plot=True,
                   output_path='data',
-                  **dict(max_generations=2)
+                  **dict(max_generations=2,
+                         pop_size=4
+                         )
                   ).supervised(models=['cat', 'xgb'],
                                feature_selector='shapley',
                                top_features=0.5,
                                optimizer='ga',
                                force_target_type=None,
                                train=True,
                                train_size=0.8,
@@ -37,40 +44,45 @@
                                clf_eval_metric='auc',
                                reg_eval_metric='rmse_norm',
                                save_train_test_data=True,
                                save_ga=True,
                                **dict(engineer_categorical=False)
                                )
         _found_results: List[bool] = []
-        for result in ['feature_learning_data.parquet',
-                       'feature_learning.p',
+        for result in ['feature_learning.p',
                        'feature_importance_shapley.html',
                        'feature_tournament_game_size.html',
                        'genetic.p',
                        'model.p'
                        ]:
-            if os.path.isfile('data/{}'.format(result)):
+            if os.path.isfile(f'data/{result}'):
                 _found_results.append(True)
             else:
                 _found_results.append(False)
         self.assertTrue(expr=all(_found_results))
 
     def test_supervised_reg(self):
-        _feature_engineer: FeatureEngineer = FeatureEngineer(df=DATA_SET, target_feature='AveragePrice')
+        _feature_engineer: FeatureEngineer = FeatureEngineer(temp_dir=TEMP_DIR,
+                                                             df=DATA_SET,
+                                                             target_feature='AveragePrice'
+                                                             )
         _feature_engineer.set_predictors(exclude_original_data=False)
-        DataMiner(df=_feature_engineer.get_data(dask_df=True),
+        DataMiner(temp_dir=TEMP_DIR,
+                  df=_feature_engineer.get_data(dask_df=True),
                   file_path=None,
                   target=_feature_engineer.get_target(),
                   predictors=_feature_engineer.get_predictors(),
                   feature_engineer=_feature_engineer,
                   feature_generator=True,
                   train_critic=True,
                   plot=True,
                   output_path='data',
-                  **dict(max_generations=2)
+                  **dict(max_generations=2,
+                         pop_size=4
+                         )
                   ).supervised(models=['cat', 'xgb'],
                                feature_selector='shapley',
                                top_features=0.5,
                                optimizer='ga',
                                force_target_type=None,
                                train=True,
                                train_size=0.8,
```

### Comparing `happy_learning-0.4.7/test/test_deep_q_learning.py` & `happy_learning-0.4.8/test/test_deep_q_learning.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import unittest
 
 from happy_learning.deep_q_learning import DQNAgent
 from happy_learning.sampler import MLSampler
 from happy_learning.supervised_machine_learning import ModelGeneratorClf
 from typing import List
 
-OUTPUT_PATH: str = './data/'
-DF: pd.DataFrame = pd.read_csv(filepath_or_buffer=f'{OUTPUT_PATH}avocado.csv', sep=',')
+OUTPUT_PATH: str = 'data/'
+DF: pd.DataFrame = pd.read_csv(filepath_or_buffer=f'{OUTPUT_PATH}avocado.csv', sep=',').loc[0:10000, ]
 DF = DF.replace({'conventional': 0, 'organic': 1})
 DF['type'] = DF['type'].astype(int)
 CLF_TARGET: str = 'type'
 REG_TARGET: str = 'AveragePrice'
 FEATURES: List[str] = ['Total Volume',
                        'Total Bags',
                        '4046',
@@ -30,16 +30,18 @@
    Class for testing methods of class DQNAgent
    """
    def test_apply_learning(self):
        """
        Test apply learning (inference) function
        """
        _model_name: str = 'cat'
-       _param: dict = ModelGeneratorClf(model_name=_model_name).generate_model().model_param
-       agent: DQNAgent = DQNAgent(episodes=10,
+       _model: ModelGeneratorClf = ModelGeneratorClf(model_name=_model_name)
+       _model.generate_model()
+       _param: dict = _model.model_param
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm=_model_name)
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        _new_param: dict = agent.apply_learning(model_name=_model_name,
@@ -51,303 +53,303 @@
                                                max_actions=1,
                                                force_all_actions=False
                                                )
        self.assertNotEqual(first=_param, second=_new_param)
 
    def test_optimize_clf_ada(self):
        """
-       Test hyper-parameter optimization of ada boost classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of ada boost classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='ada')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_cat(self):
        """
-       Test hyper-parameter optimization of cat boost classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of cat boost classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='cat')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_lida(self):
        """
-       Test hyper-parameter optimization of linear discriminant analysis classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of linear discriminant analysis classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='lida')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_log(self):
        """
-       Test hyper-parameter optimization of logistic regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of logistic regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='log')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_gbo(self):
        """
-       Test hyper-parameter optimization of gradient boosting decision tree classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of gradient boosting decision tree classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='gbo')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_knn(self):
        """
-       Test hyper-parameter optimization of k-nearest neighbor classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of k-nearest neighbor classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='knn')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_qda(self):
        """
-       Test hyper-parameter optimization of quadratic discriminant analysis classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of quadratic discriminant analysis classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='qda')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_rf(self):
        """
-       Test hyper-parameter optimization of random forest classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of random forest classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='rf')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_svm(self):
        """
-       Test hyper-parameter optimization of support vector machine classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of support vector machine classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='svm')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_nusvm(self):
        """
-       Test hyper-parameter optimization of nu support vector machine classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of nu support vector machine classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='nusvm')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_clf_xgb(self):
        """
-       Test hyper-parameter optimization of extreme gradient boosting decision tree classification using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of extreme gradient boosting decision tree classification using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='xgb')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_ada(self):
        """
-       Test hyper-parameter optimization of ada boost regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of ada boost regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='ada')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_cat(self):
        """
-       Test hyper-parameter optimization of cat boost regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of cat boost regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='cat')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_elastic(self):
        """
-       Test hyper-parameter optimization of elastic net regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of elastic net regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='elastic')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_gam(self):
        """
-       Test hyper-parameter optimization of generalized additive models regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of generalized additive models regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='gam')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_rf(self):
        """
-       Test hyper-parameter optimization of random forest regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of random forest regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='rf')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_svm(self):
        """
-       Test hyper-parameter optimization of support vector machine regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of support vector machine regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='svm')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_nusvm(self):
        """
-       Test hyper-parameter optimization of nu support vector machine regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of nu support vector machine regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='nusvm')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_gbo(self):
        """
-       Test hyper-parameter optimization of gradient boosting decision tree regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of gradient boosting decision tree regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='gbo')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_lasso(self):
        """
-       Test hyper-parameter optimization of lasso regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of lasso regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='lasso')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_knn(self):
        """
-       Test hyper-parameter optimization of k-nearest neighbor regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of k-nearest neighbor regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='knn')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_reg_xgb(self):
        """
-       Test hyper-parameter optimization of extreme gradient boosting decision tree regression using reinforcement learning (Deep-Q-Learning)
+       Test hyperparameter optimization of extreme gradient boosting decision tree regression using reinforcement learning (Deep-Q-Learning)
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='xgb')
                                   )
        _n_optimization_steps_before: int = agent.n_optimization
        agent.optimize(df=DF, target=REG_TARGET, features=FEATURES)
        self.assertGreater(a=agent.n_optimization, b=_n_optimization_steps_before)
 
    def test_optimize_continue(self):
        """
        Test continuing optimization
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='cat')
                                   )
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        _n_optimization_steps_after: int = agent.n_optimization
        agent.optimize_continue(df=DF, target=CLF_TARGET, features=FEATURES)
@@ -359,15 +361,15 @@
        """
        data_sets: dict = MLSampler(df=DF,
                                    target=CLF_TARGET,
                                    features=FEATURES,
                                    train_size=0.8,
                                    stratification=False
                                    ).train_test_sampling(validation_split=0.1)
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='cat')
                                   )
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        agent.save(agent=True, model=True, data_sets=data_sets, experience=True)
        _found_saved_files: int = 0
@@ -385,15 +387,15 @@
            _found_saved_files += 1
        self.assertTrue(expr=_found_saved_files == 6)
 
    def test_visualize(self):
        """
        Test visualization function
        """
-       agent: DQNAgent = DQNAgent(episodes=10,
+       agent: DQNAgent = DQNAgent(episodes=5,
                                   target_update=5,
                                   output_file_path=OUTPUT_PATH,
                                   **dict(sml_algorithm='cat')
                                   )
        agent.optimize(df=DF, target=CLF_TARGET, features=FEATURES)
        agent.visualize()
        _found_saved_plots: int = 0
```

### Comparing `happy_learning-0.4.7/test/test_environment_modeling.py` & `happy_learning-0.4.8/test/test_environment_modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from happy_learning.environment_modeling import EnvironmentModeling
 from happy_learning.sampler import MLSampler
 from happy_learning.supervised_machine_learning import ModelGeneratorClf
 from typing import List
 
 MODEL_NAME: str = 'cat'
 ENV: EnvironmentModeling = EnvironmentModeling(sml_problem='clf_binary', sml_algorithm=MODEL_NAME)
-PARAM: dict = ModelGeneratorClf(model_name=MODEL_NAME).generate_model().model_param
+MODEL: ModelGeneratorClf = ModelGeneratorClf(model_name=MODEL_NAME)
+MODEL.generate_model()
+PARAM: dict = MODEL.model_param
 DF: pd.DataFrame = pd.read_csv(filepath_or_buffer='./data/avocado.csv', sep=',')
 DF = DF.replace({'conventional': 0, 'organic': 1})
 DF['type'] = DF['type'].astype(int)
 CLF_TARGET: str = 'type'
 FEATURES: List[str] = ['Total Volume',
                        'Total Bags',
                        '4046',
```

### Comparing `happy_learning-0.4.7/test/test_evaluate_machine_learning.py` & `happy_learning-0.4.8/test/test_evaluate_machine_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,20 @@
                                      train_time_in_seconds=400
                                      )
         self.assertTrue(expr='fitness_score' in list(_sml_score.keys()))
 
     def test_sml_fitness_score(self):
         _sml_fitness_score: float = sml_fitness_score(ml_metric=(0.56, 1),
                                                       train_test_metric=(0.56, 0.66),
-                                                      train_time_in_seconds=400
+                                                      train_time_in_seconds=400,
+                                                      ml_metric_weights=0.3,
+                                                      train_test_weights=0.77,
+                                                      train_time_in_seconds_weights=0.0000005,
                                                       )
-        self.assertEqual(first=94.42444444444445, second=_sml_fitness_score)
+        self.assertEqual(first=91.42444444444445, second=_sml_fitness_score)
 
     def test_sml_score_test(self):
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `happy_learning-0.4.7/test/test_feature_engineer.py` & `happy_learning-0.4.8/test/test_feature_engineer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import unittest
 
 from happy_learning.feature_engineer import FeatureEngineer, PROCESSING_ACTION_SPACE, SUPPORTED_TYPES
 from typing import Dict, List
 
 DATA_FILE_PATH: str = 'data/avocado.csv'
 FEATURE_ENGINEER_FILE_PATH: str = 'data/feature_engineer.p'
-FEATURE_ENGINEER: FeatureEngineer = FeatureEngineer(df=None,
+FEATURE_ENGINEER: FeatureEngineer = FeatureEngineer(temp_dir='data',
+                                                    df=None,
                                                     file_path=DATA_FILE_PATH,
                                                     target_feature='AveragePrice',
                                                     generate_new_feature=True,
                                                     keep_original_data=True,
                                                     unify_invalid_values=True,
                                                     encode_missing_data=False,
                                                     max_level_processing=5,
@@ -36,51 +37,60 @@
 
     :param features: List[str]
         Name of the features
 
     :return: bool
         FeatureOrchestra check passed or failed
     """
-    return True
+    pass
 
 
-def _check_tracking(meth: str, suffix: str, feature_type: str) -> Dict[str, bool]:
+def _check_tracking(meth: str, suffix: str, feature_type: str, feature: str = None) -> Dict[str, bool]:
     """
     Check internal tracking framework of the FeatureEngineer class
 
     :param meth: str
         Name of the method
 
     :param suffix: str
         Suffix
 
     :param feature_type: str
         Name of the feature type
 
+    :param feature: str
+        Name of the feature
+
     :return: Dict[str, bool]
         Tracking results:
             -> Process tracking
             -> Feature relation tracking (raw)
             -> Feature relation tracking (level)
     """
-    _features: List[str] = copy.deepcopy(FEATURE_ENGINEER.get_features(feature_type=feature_type))
+    if feature in FEATURE_ENGINEER.get_features():
+        _features = [feature]
+    else:
+        _features: List[str] = copy.deepcopy(FEATURE_ENGINEER.get_features(feature_type=feature_type))
     _found_tracked_processes: List[bool] = []
     _found_tracked_feature_relation_raw: List[bool] = []
     _found_tracked_feature_relation_level: List[bool] = []
     _process_tracking: dict = FEATURE_ENGINEER.get_data_processing()['processing']['process']
     _feature_relation_tracking: dict = FEATURE_ENGINEER.get_data_processing()['processing']['features']
     for i, feature in enumerate(_features, start=1):
-        if _process_tracking[str(i)]['meth'] == meth and list(_process_tracking[str(i)]['features'].keys())[0] == '{}_{}'.format(feature, suffix) and _process_tracking[str(i)]['features']['{}_{}'.format(feature, suffix)]:
-            _found_tracked_processes.append(True)
-        else:
-            _found_tracked_processes.append(False)
+        for j, process in enumerate(_process_tracking.keys(), start=1):
+            if _process_tracking[process]['meth'] == meth and list(_process_tracking[process]['features'].keys())[0] == '{}_{}'.format(feature, suffix) and _process_tracking[process]['features']['{}_{}'.format(feature, suffix)] == feature:
+                _found_tracked_processes.append(True)
+                break
+            else:
+                if j == len(_process_tracking.keys()):
+                    _found_tracked_processes.append(False)
         if '{}_{}'.format(feature, suffix) in FEATURE_ENGINEER.get_cleaned_features():
             continue
         if feature in _feature_relation_tracking['raw'].keys():
-            if _feature_relation_tracking['raw'][feature][0] == '{}_{}'.format(feature, suffix):
+            if '{}_{}'.format(feature, suffix) in _feature_relation_tracking['raw'][feature]:
                 _found_tracked_feature_relation_raw.append(True)
             else:
                 _found_tracked_feature_relation_raw.append(False)
         else:
             _found_tracked_feature_relation_raw.append(False)
         if '{}_{}'.format(feature, suffix) in _feature_relation_tracking['level_1'].keys():
             if len(_feature_relation_tracking['level_1']['{}_{}'.format(feature, suffix)]) == 0:
@@ -257,19 +267,17 @@
     def test_clean(self):
         _n_features: int = FEATURE_ENGINEER.get_n_features()
         FEATURE_ENGINEER.clean(markers=dict(features=['type']))
         self.assertTrue(expr=_n_features > FEATURE_ENGINEER.get_n_features())
 
     def test_clean_nan(self):
         FEATURE_ENGINEER.exp_transform()
-        FEATURE_ENGINEER.exp_transform()
-        FEATURE_ENGINEER.exp_transform()
         _n_cases: int = FEATURE_ENGINEER.get_n_cases()
         FEATURE_ENGINEER.clean_nan(other_mis=None)
-        print(FEATURE_ENGINEER.get_data(dask_df=False)['Total Bags_exp_exp'])
+        print(FEATURE_ENGINEER.get_data(dask_df=False)['Total Bags_exp'])
         self.assertTrue(expr=_n_cases > FEATURE_ENGINEER.get_n_cases())
 
     def test_clean_unstable_features(self):
         pass
 
     def test_concat_text(self):
         pass
@@ -282,19 +290,29 @@
         FEATURE_ENGINEER.data_export(file_path=_data_file_path, create_dir=False, overwrite=True)
         if _data_file_path.find('.parquet') >= 0:
             self.assertTrue(expr=os.path.isdir(_data_file_path))
         else:
             self.assertTrue(expr=os.path.isfile(_data_file_path))
 
     def test_data_import(self):
-        _feature_engineer = FeatureEngineer(file_path='data/avocado.csv')
+        _feature_engineer = FeatureEngineer(temp_dir='data',
+                                            file_path='data/avocado.csv'
+                                            )
         self.assertTrue(expr=_feature_engineer.get_n_cases() > 0)
 
     def test_date_categorizer(self):
-        FEATURE_ENGINEER.date_categorizer()
+        FEATURE_ENGINEER.date_categorizer(year=True,
+                                          month=True,
+                                          week=True,
+                                          week_day=True,
+                                          day=True,
+                                          hour=True,
+                                          minute=True,
+                                          second=True
+                                          )
         _tracking_check_year: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='year', feature_type='date')
         _tracking_check_month: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='month', feature_type='date')
         _tracking_check_day: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='day', feature_type='date')
         _tracking_check_hour: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='hour', feature_type='date')
         _tracking_check_minute: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='minute', feature_type='date')
         _tracking_check_second: Dict[str, bool] = _check_tracking(meth='date_categorizer', suffix='second', feature_type='date')
         _tracking_check: Dict[str, bool] = {'process': all([_tracking_check_year.get('process'),
@@ -525,29 +543,28 @@
 
     def test_get_training_data(self):
         FEATURE_ENGINEER.set_predictors(exclude_original_data=False)
         self.assertEqual(first=9, second=len(FEATURE_ENGINEER.get_training_data(output='df_dask').columns))
 
     def test_get_transformations(self):
         _transformations: dict = dict(encoder=['bin', 'label', 'one_hot'],
-                                      scaler=['min_max', 'robust', 'normal', 'standard', 'box_cox', 'log', 'exp'],
+                                      scaler=['minmax', 'robust', 'normal', 'standard', 'box_cox', 'log', 'exp'],
                                       mapper=[],
                                       naming=[],
                                       binning_continuous=[],
                                       binning_date=[]
                                       )
         _found_transformation: List[bool] = []
-        print(FEATURE_ENGINEER.get_transformations())
         _observed_transformation: dict = FEATURE_ENGINEER.get_transformations(transformation=None)
         for transformation in _transformations.keys():
             if transformation in list(_observed_transformation.keys()):
                 _found_transformation.append(True)
                 if len(_transformations.get(transformation)) > 0:
                     for meth in _transformations.get(transformation):
-                        if meth in list(_observed_transformation[transformation][meth].keys()):
+                        if meth in list(_observed_transformation[transformation].keys()):
                             _found_transformation.append(True)
                         else:
                             _found_transformation.append(False)
             else:
                 _found_transformation.append(False)
         self.assertTrue(expr=all(_found_transformation))
 
@@ -563,15 +580,15 @@
     def test_is_unstable(self):
         pass
 
     def test_label_encoder(self):
         _unique_feature_labels = FEATURE_ENGINEER.get_feature_values(feature='type', unique=True)
         _found_labels: List[bool] = [True if type(label) == str else False for label in _unique_feature_labels]
         FEATURE_ENGINEER.label_encoder(encode=True, features=['type'])
-        _found_values: List[bool] = [True if type(value) == np.int64 or type(value) == np.int32 else False for value in FEATURE_ENGINEER.get_feature_values(feature='type', unique=True)]
+        _found_values: List[bool] = [True if type(value) == np.int64 or type(value) == np.int32 else False for value in FEATURE_ENGINEER.get_feature_values(feature='type_label_enc', unique=True)]
         self.assertTrue(expr=all(_found_labels) and all(_found_values))
 
     def test_linguistic_features(self):
         pass
 
     def test_load(self):
         pass
@@ -579,15 +596,15 @@
     def test_log_transform(self):
         FEATURE_ENGINEER.log_transform()
         _tracking_check: Dict[str, bool] = _check_tracking(meth='log_transform', suffix='log', feature_type='continuous')
         self.assertTrue(expr=_tracking_check.get('process') and _tracking_check.get('raw') and _tracking_check.get('level'))
 
     def test_normalizer(self):
         FEATURE_ENGINEER.normalizer()
-        _tracking_check: Dict[str, bool] = _check_tracking(meth='exp_transform', suffix='exp', feature_type='continuous')
+        _tracking_check: Dict[str, bool] = _check_tracking(meth='normalizer', suffix='normal', feature_type='continuous')
         self.assertTrue(expr=_tracking_check.get('process') and _tracking_check.get('raw') and _tracking_check.get('level'))
 
     def test_merge_engineer(self):
         _all_features: List[str] = FEATURE_ENGINEER.get_features()
         _all_features.sort(reverse=False)
         _engineer: FeatureEngineer = FeatureEngineer(df=None, file_path=DATA_FILE_PATH, target_feature='AveragePrice')
         _categorical_features: List[str] = _engineer.get_feature_types().get('categorical')
@@ -607,16 +624,50 @@
         pass
 
     def test_missing_data_analysis(self):
         pass
 
     def test_one_hot_encoder(self):
         FEATURE_ENGINEER.one_hot_encoder()
-        _tracking_check: Dict[str, bool] = _check_tracking(meth='one_hot_encoder', suffix='', feature_type='continuous')
-        self.assertTrue(expr=_tracking_check.get('process') and _tracking_check.get('raw') and _tracking_check.get('level'))
+        _tracking_check_2015: Dict[str, bool] = _check_tracking(meth='one_hot_encoder',
+                                                                suffix='2015',
+                                                                feature_type='categorical',
+                                                                feature='year'
+                                                                )
+        _tracking_check_2016: Dict[str, bool] = _check_tracking(meth='one_hot_encoder',
+                                                                suffix='2016',
+                                                                feature_type='categorical',
+                                                                feature='year'
+                                                                )
+        _tracking_check_2017: Dict[str, bool] = _check_tracking(meth='one_hot_encoder',
+                                                                suffix='2017',
+                                                                feature_type='categorical',
+                                                                feature='year'
+                                                                )
+        _tracking_check_2018: Dict[str, bool] = _check_tracking(meth='one_hot_encoder',
+                                                                suffix='2018',
+                                                                feature_type='categorical',
+                                                                feature='year'
+                                                                )
+        _tracking_process: bool = all([_tracking_check_2015.get('process'),
+                                       _tracking_check_2016.get('process'),
+                                       _tracking_check_2017.get('process'),
+                                       _tracking_check_2018.get('process'),
+                                       ])
+        _tracking_raw: bool = all([_tracking_check_2015.get('raw'),
+                                   _tracking_check_2016.get('raw'),
+                                   _tracking_check_2017.get('raw'),
+                                   _tracking_check_2018.get('raw'),
+                                   ])
+        _tracking_level: bool = all([_tracking_check_2015.get('level'),
+                                     _tracking_check_2016.get('level'),
+                                     _tracking_check_2017.get('level'),
+                                     _tracking_check_2018.get('level'),
+                                     ])
+        self.assertTrue(expr=_tracking_process and _tracking_raw and _tracking_level)
 
     def test_outlier_detection(self):
         pass
 
     def test_re_engineer(self):
         pass
 
@@ -639,24 +690,24 @@
         pass
 
     def test_reset_multi_threading(self):
         pass
 
     def test_reset_target(self):
         FEATURE_ENGINEER.reset_target()
-        self.assertEqual(first=None, second=FEATURE_ENGINEER.get_target())
+        self.assertEqual(first=[], second=FEATURE_ENGINEER.get_target())
 
     def test_rounding(self):
         FEATURE_ENGINEER.rounding()
         _tracking_check: Dict[str, bool] = _check_tracking(meth='rounding', suffix='round_100', feature_type='continuous')
         self.assertTrue(expr=_tracking_check.get('process') and _tracking_check.get('raw') and _tracking_check.get('level'))
 
     def test_save(self):
         FEATURE_ENGINEER.save(file_path='data/feature_engineer.p', cls_obj=True, overwrite=True, create_dir=False)
-        self.assertTrue(expr=os.path.isfile('data/feature_engineer.p') and os.path.isdir('data/feature_engineer_data.parquet'))
+        self.assertTrue(expr=os.path.isfile('data/feature_engineer.p'))
 
     def test_sampler(self):
         pass
 
     def test_scaling_robust(self):
         FEATURE_ENGINEER.scaling_robust()
         _tracking_check: Dict[str, bool] = _check_tracking(meth='scaling_robust', suffix='robust', feature_type='continuous')
```

### Comparing `happy_learning-0.4.7/test/test_feature_learning.py` & `happy_learning-0.4.8/test/test_feature_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 import unittest
 
 from happy_learning.feature_engineer import FeatureEngineer
 from happy_learning.feature_learning import FeatureLearning
 from happy_learning.genetic_algorithm import GeneticAlgorithm
 
 DATA_SET: pd.DataFrame = pd.read_csv(filepath_or_buffer='data/avocado.csv')
+TEMP_DIR: str = 'data'
 
 
 class FeatureLearningTest(unittest.TestCase):
     """
     Class for testing class FeatureLearning
     """
     def test_ga_clf(self):
-        _feature_engineer: FeatureEngineer = FeatureEngineer(df=DATA_SET, target_feature='type')
+        _feature_engineer: FeatureEngineer = FeatureEngineer(temp_dir=TEMP_DIR,
+                                                             df=DATA_SET,
+                                                             target_feature='type'
+                                                             )
         _feature_engineer.set_predictors(exclude=None, exclude_original_data=False)
         _ga: GeneticAlgorithm = GeneticAlgorithm(mode='model',
                                                  target=_feature_engineer.get_target(),
                                                  input_file_path=None,
                                                  train_data_file_path=None,
                                                  test_data_file_path=None,
                                                  valid_data_file_path=None,
@@ -34,16 +38,16 @@
                                                  models=['cat'],
                                                  model_params=None,
                                                  burn_in_generations=-1,
                                                  warm_start=True,
                                                  warm_start_strategy='monotone',
                                                  warm_start_constant_hidden_layers=0,
                                                  warm_start_constant_category='very_small',
-                                                 max_generations=10,
-                                                 pop_size=64,
+                                                 max_generations=1,
+                                                 pop_size=4,
                                                  mutation_rate=0.1,
                                                  mutation_prob=0.15,
                                                  parents_ratio=0.5,
                                                  early_stopping=0,
                                                  convergence=True,
                                                  convergence_measure='min',
                                                  timer_in_seconds=43200,
@@ -91,16 +95,16 @@
                                                                     models=['cat'],
                                                                     model_params=None,
                                                                     burn_in_generations=-1,
                                                                     warm_start=True,
                                                                     warm_start_strategy='monotone',
                                                                     warm_start_constant_hidden_layers=0,
                                                                     warm_start_constant_category='very_small',
-                                                                    max_generations=10,
-                                                                    pop_size=64,
+                                                                    max_generations=1,
+                                                                    pop_size=4,
                                                                     mutation_rate=0.1,
                                                                     mutation_prob=0.15,
                                                                     parents_ratio=0.5,
                                                                     early_stopping=0,
                                                                     convergence=True,
                                                                     convergence_measure='min',
                                                                     timer_in_seconds=43200,
@@ -113,15 +117,18 @@
                                                                     feature_engineer=_feature_learning_engineer,
                                                                     sampling_function=None
                                                                     )
         _ga_using_new_features.optimize()
         self.assertTrue(expr=_ga_using_new_features.final_generation[_ga_using_new_features.best_individual_idx]['fitness_score'] >= _ga.final_generation[_ga.best_individual_idx]['fitness_score'])
 
     def test_ga_reg(self):
-        _feature_engineer: FeatureEngineer = FeatureEngineer(df=DATA_SET, target_feature='AveragePrice')
+        _feature_engineer: FeatureEngineer = FeatureEngineer(temp_dir=TEMP_DIR,
+                                                             df=DATA_SET,
+                                                             target_feature='AveragePrice'
+                                                             )
         _feature_engineer.set_predictors(exclude=None, exclude_original_data=False)
         _ga: GeneticAlgorithm = GeneticAlgorithm(mode='model',
                                                  target=_feature_engineer.get_target(),
                                                  input_file_path=None,
                                                  train_data_file_path=None,
                                                  test_data_file_path=None,
                                                  valid_data_file_path=None,
@@ -138,16 +145,16 @@
                                                  models=['cat'],
                                                  model_params=None,
                                                  burn_in_generations=-1,
                                                  warm_start=True,
                                                  warm_start_strategy='monotone',
                                                  warm_start_constant_hidden_layers=0,
                                                  warm_start_constant_category='very_small',
-                                                 max_generations=10,
-                                                 pop_size=64,
+                                                 max_generations=1,
+                                                 pop_size=4,
                                                  mutation_rate=0.1,
                                                  mutation_prob=0.15,
                                                  parents_ratio=0.5,
                                                  early_stopping=0,
                                                  convergence=True,
                                                  convergence_measure='min',
                                                  timer_in_seconds=43200,
@@ -195,16 +202,16 @@
                                                                     models=['cat'],
                                                                     model_params=None,
                                                                     burn_in_generations=-1,
                                                                     warm_start=True,
                                                                     warm_start_strategy='monotone',
                                                                     warm_start_constant_hidden_layers=0,
                                                                     warm_start_constant_category='very_small',
-                                                                    max_generations=10,
-                                                                    pop_size=64,
+                                                                    max_generations=1,
+                                                                    pop_size=4,
                                                                     mutation_rate=0.1,
                                                                     mutation_prob=0.15,
                                                                     parents_ratio=0.5,
                                                                     early_stopping=0,
                                                                     convergence=True,
                                                                     convergence_measure='min',
                                                                     timer_in_seconds=43200,
```

### Comparing `happy_learning-0.4.7/test/test_genetic_algorithm.py` & `happy_learning-0.4.8/test/test_genetic_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 TEST_DATA_PATH: str = 'data/text_test.csv'
 VALIDATION_DATA_PATH: str = 'data/text_val.csv'
 pd.concat(objs=[pd.DataFrame(data=TRAIN_TEST_REG.get('x_train')), pd.DataFrame(data=TRAIN_TEST_REG.get('y_train'))], axis=1).to_csv(path_or_buf=TRAIN_DATA_REG_PATH, index=False)
 pd.concat(objs=[pd.DataFrame(data=TRAIN_TEST_REG.get('x_test')), pd.DataFrame(data=TRAIN_TEST_REG.get('y_test'))], axis=1).to_csv(path_or_buf=TEST_DATA_REG_PATH, index=False)
 pd.concat(objs=[pd.DataFrame(data=TRAIN_TEST_REG.get('x_val')), pd.DataFrame(data=TRAIN_TEST_REG.get('y_val'))], axis=1).to_csv(path_or_buf=VALIDATION_DATA_REG_PATH, index=False)
 DATA_SET_TEXT_CLF: pd.DataFrame = pd.read_csv(filepath_or_buffer='data/tripadvisor_hotel_reviews.csv').loc[0:100, ]
 DATA_SET_TEXT_CLF = DATA_SET_TEXT_CLF.loc[~DATA_SET_TEXT_CLF.isnull().any(axis=1), :]
-UNIQUE_LABELS: int = 3 # len(DATA_SET_TEXT_CLF['label'].unique())
+UNIQUE_LABELS: int = len(DATA_SET_TEXT_CLF['label'].unique())
 TRAIN_TEST_TEXT_CLF: dict = MLSampler(df=DATA_SET_TEXT_CLF,
                                       target=TARGET_TEXT,
                                       features=PREDICTORS_TEXT,
                                       train_size=0.8,
                                       random_sample=True,
                                       stratification=False,
                                       seed=1234
@@ -149,17 +149,20 @@
                                                  timer_in_seconds=43200,
                                                  force_target_type=None,
                                                  plot=False,
                                                  output_file_path='data',
                                                  deep_learning_type='batch',
                                                  deep_learning_output_size=UNIQUE_LABELS,
                                                  log=False,
+                                                 mlflow_log=False,
                                                  feature_engineer=None,
                                                  sampling_function=None,
-                                                 **dict(sep=',')
+                                                 **dict(sep=',',
+                                                        lang='en'
+                                                        )
                                                  )
         _ga.optimize()
         self.assertTrue(expr=_ga.evolution_gradient.get('max')[0] <= _ga.evolution_gradient.get('max')[-1])
 
     def test_optimize_modeling_text_clustering(self):
         _ga: GeneticAlgorithm = GeneticAlgorithm(mode='model',
                                                  target=None,
@@ -326,62 +329,65 @@
                                                  model_params=None,
                                                  burn_in_generations=-1,
                                                  warm_start=True,
                                                  warm_start_strategy='monotone',
                                                  warm_start_constant_hidden_layers=0,
                                                  warm_start_constant_category='very_small',
                                                  max_generations=1,
-                                                 pop_size=64,
+                                                 pop_size=4,
                                                  mutation_rate=0.1,
                                                  mutation_prob=0.85,
                                                  parents_ratio=0.5,
                                                  early_stopping=0,
                                                  convergence=False,
                                                  convergence_measure='min',
                                                  timer_in_seconds=43200,
                                                  force_target_type=None,
                                                  plot=False,
                                                  output_file_path='data',
                                                  deep_learning_type='batch',
                                                  deep_learning_output_size=None,
                                                  log=False,
+                                                 mlflow_log=False,
                                                  feature_engineer=_feature_engineer,
                                                  sampling_function=None
                                                  )
         _ga.optimize()
-        _ga.visualize(results_table=False,
+        _ga.visualize(results_table=True,
                       model_distribution=True,
                       model_evolution=True,
                       param_distribution=False,
                       train_time_distribution=True,
-                      breeding_map=True,
+                      breeding_map=False,
                       breeding_graph=False,
                       fitness_distribution=True,
                       fitness_evolution=True,
                       fitness_dimensions=True,
                       per_generation=True,
-                      prediction_of_best_model=False,
+                      prediction_of_best_model=True,
                       epoch_stats=False
                       )
         _found_plot: List[bool] = []
         for plot in ['ga_metadata_table',
                      'ga_model_evolution',
-                     'ga_model_distribution',
-                     'ga_parameter_treemap',
-                     'ga_training_time_distribution',
-                     'ga_breeding_heatmap',
-                     'ga_breeding_graph',
+                     'ga_model_distribution_model_generation_0',
+                     'ga_model_distribution_model_generation_1',
+                     #'ga_parameter_treemap',
+                     'ga_training_time_distribution_train_time_in_seconds_model',
+                     #'ga_breeding_heatmap',
+                     #'ga_breeding_graph',
                      'ga_fitness_score_distribution_per_generation',
-                     'ga_metadata_evolution_coords_actor_only',
+                     'ga_metadata_evolution_coords',
                      'ga_evolution_fitness_score',
                      'ga_prediction_confusion_table',
                      'ga_prediction_confusion_heatmap',
-                     'ga_prediction_confusion_normal_heatmap'
+                     'ga_prediction_confusion_normal_heatmap',
+                     'ga_prediction_clf_report_table',
                      ]:
-            if os.path.isfile('data/{}.html'.format(plot)):
+            if os.path.isfile(f'data/{plot}.html'):
                 _found_plot.append(True)
             else:
                 _found_plot.append(False)
         self.assertTrue(expr=all(_found_plot))
 
     def test_visualize_reg(self):
         _feature_engineer: FeatureEngineer = FeatureEngineer(df=DATA_SET, target_feature='AveragePrice', temp_dir=DATA_DIR)
```

### Comparing `happy_learning-0.4.7/test/test_missing_data_analysis.py` & `happy_learning-0.4.8/test/test_missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_multiple_imputation.py` & `happy_learning-0.4.8/test/test_multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_neural_network_generator_torch.py` & `happy_learning-0.4.8/test/test_neural_network_generator_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_neural_network_torch.py` & `happy_learning-0.4.8/test/test_neural_network_torch.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_sampler.py` & `happy_learning-0.4.8/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_supervised_machine_learning.py` & `happy_learning-0.4.8/test/test_supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_swarm_intelligence.py` & `happy_learning-0.4.8/test/test_swarm_intelligence.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                                                    re_split_data=False,
                                                    re_sample_cases=False,
                                                    re_sample_features=False,
                                                    re_populate=True,
                                                    max_trials=2,
                                                    max_features=-1,
                                                    labels=None,
-                                                   models=['cat'],
+                                                   models=['xgb'],
                                                    model_params=None,
                                                    burn_in_adjustments=-1,
                                                    warm_start=True,
                                                    warm_start_strategy='monotone',
                                                    warm_start_constant_hidden_layers=0,
                                                    warm_start_constant_category='very_small',
                                                    max_adjustments=2,
@@ -127,15 +127,15 @@
                                                    re_split_data=False,
                                                    re_sample_cases=False,
                                                    re_sample_features=False,
                                                    re_populate=True,
                                                    max_trials=2,
                                                    max_features=-1,
                                                    labels=None,
-                                                   models=['trans'],
+                                                   models=['rcnn'],
                                                    model_params=None,
                                                    burn_in_adjustments=-1,
                                                    warm_start=True,
                                                    warm_start_strategy='monotone',
                                                    warm_start_constant_hidden_layers=0,
                                                    warm_start_constant_category='very_small',
                                                    max_adjustments=1,
@@ -227,16 +227,16 @@
                                                    models=['cat'],
                                                    model_params=None,
                                                    burn_in_adjustments=-1,
                                                    warm_start=True,
                                                    warm_start_strategy='monotone',
                                                    warm_start_constant_hidden_layers=0,
                                                    warm_start_constant_category='very_small',
-                                                   max_adjustments=5,
-                                                   pop_size=64,
+                                                   max_adjustments=2,
+                                                   pop_size=4,
                                                    adjustment_rate=0.1,
                                                    adjustment_prob=0.85,
                                                    early_stopping=0,
                                                    convergence=True,
                                                    convergence_measure='median',
                                                    timer_in_seconds=43200,
                                                    force_target_type=None,
```

### Comparing `happy_learning-0.4.7/test/test_text_clustering.py` & `happy_learning-0.4.8/test/test_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_text_clustering_generator.py` & `happy_learning-0.4.8/test/test_text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.7/test/test_text_miner.py` & `happy_learning-0.4.8/test/test_text_miner.py`

 * *Files identical despite different names*

