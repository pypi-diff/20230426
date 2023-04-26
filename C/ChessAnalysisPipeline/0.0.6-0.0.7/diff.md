# Comparing `tmp/ChessAnalysisPipeline-0.0.6.tar.gz` & `tmp/ChessAnalysisPipeline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChessAnalysisPipeline-0.0.6.tar", last modified: Mon Apr 24 17:11:36 2023, max compression
+gzip compressed data, was "ChessAnalysisPipeline-0.0.7.tar", last modified: Wed Apr 26 10:17:31 2023, max compression
```

## Comparing `ChessAnalysisPipeline-0.0.6.tar` & `ChessAnalysisPipeline-0.0.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.890539 ChessAnalysisPipeline-0.0.6/CHAP/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3941 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   121894 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51967 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/general.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11359 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44627 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/scanparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3070 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/edd/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13698 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3869 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)   104814 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/MLaaS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/ktrain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/mnist_img.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/tfaas_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 17:11:29.000000 ChessAnalysisPipeline-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/models/map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3941 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   121894 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51967 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11359 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44627 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/utils/scanparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3070 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/common/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/edd/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13698 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/edd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/inference/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.308915 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/saxswaxs/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/sin2psi/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/CHAP/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104883 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/tomo/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/CHAP/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 10:17:31.000000 ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/MLaaS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/ktrain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/mnist_img.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/MLaaS/tfaas_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 10:17:13.000000 ChessAnalysisPipeline-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:17:31.312915 ChessAnalysisPipeline-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-26 10:17:23.000000 ChessAnalysisPipeline-0.0.7/setup.py
```

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/TaskManager.py` & `ChessAnalysisPipeline-0.0.7/CHAP/TaskManager.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/__init__.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/models/integration.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/models/integration.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/models/map.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/models/map.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/processor.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/reader.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/fit.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/fit.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/general.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/general.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/material.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/material.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/scanparsers.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/utils/scanparsers.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/common/writer.py` & `ChessAnalysisPipeline-0.0.7/CHAP/common/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/edd/models.py` & `ChessAnalysisPipeline-0.0.7/CHAP/edd/models.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/edd/processor.py` & `ChessAnalysisPipeline-0.0.7/CHAP/edd/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/inference/processor.py` & `ChessAnalysisPipeline-0.0.7/CHAP/inference/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/pipeline.py` & `ChessAnalysisPipeline-0.0.7/CHAP/pipeline.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/processor.py` & `ChessAnalysisPipeline-0.0.7/CHAP/processor.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/reader.py` & `ChessAnalysisPipeline-0.0.7/CHAP/reader.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/runner.py` & `ChessAnalysisPipeline-0.0.7/CHAP/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     opts = optmgr.parser.parse_args()
     if opts.profile:
         from cProfile import runctx  # python profiler
         from pstats import Stats     # profiler statistics
         cmd = 'runner(opts)'
         runctx(cmd, globals(), locals(), 'profile.dat')
         info = Stats('profile.dat')
+#        info.strip_dirs()
         info.sort_stats('cumulative')
         info.print_stats()
     else:
         runner(opts)
 
 
 def runner(opts):
```

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/server.py` & `ChessAnalysisPipeline-0.0.7/CHAP/server.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/tomo/models.py` & `ChessAnalysisPipeline-0.0.7/CHAP/tomo/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     :type detectors: Detector
     :ivar img_x_bounds: Detector image bounds in the x-direction
     :type img_x_bounds: list[int], optional
     """
     tool_type: Literal['reduce_data'] = 'reduce_data'
     detector: Detector = Detector.construct()
     img_x_bounds: Optional[
-        conlist(item_type=conint(ge=0), min_items=2, max_items=2)]
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
 
 
 class TomoFindCenterConfig(BaseModel):
     """
     Class representing the configuration for tomography find center axis.
 
     :ivar tool_type: Type of tomography reconstruction tool; always set
```

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/tomo/processor.py` & `ChessAnalysisPipeline-0.0.7/CHAP/tomo/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1575,14 +1575,16 @@
                 if i == center_stack_index:
                     first_image = scanparser.get_detector_data(
                         detector_prefix, image_offset)
                     theta = float(nxsubentry[1].sample.rotation_angle[0])
 
         # Select image bounds
         title = f'tomography image at theta = {round(theta, 2)+0}'
+        if img_x_bounds == (-1, -1):
+            img_x_bounds = None
         if img_x_bounds is not None:
             if is_index_range(img_x_bounds, ge=0, le=first_image.shape[0]):
                 return img_x_bounds
             if self._interactive:
                 self._logger.warning(
                     f'Invalid parameter img_x_bounds ({img_x_bounds}), '
                     + 'ignoring img_x_bounds')
```

### Comparing `ChessAnalysisPipeline-0.0.6/CHAP/writer.py` & `ChessAnalysisPipeline-0.0.7/CHAP/writer.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/PKG-INFO` & `ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/SOURCES.txt` & `ChessAnalysisPipeline-0.0.7/ChessAnalysisPipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/LICENSE` & `ChessAnalysisPipeline-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/MLaaS/ktrain.py` & `ChessAnalysisPipeline-0.0.7/MLaaS/ktrain.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/MLaaS/mnist_img.py` & `ChessAnalysisPipeline-0.0.7/MLaaS/mnist_img.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/MLaaS/tfaas_client.py` & `ChessAnalysisPipeline-0.0.7/MLaaS/tfaas_client.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/PKG-INFO` & `ChessAnalysisPipeline-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.6/README.md` & `ChessAnalysisPipeline-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.6/setup.py` & `ChessAnalysisPipeline-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 to build doc : python setup.py doc
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
-version = 'v0.0.6'
+version = 'v0.0.7'
 
 def datafiles(idir, pattern=None):
     """Return list of data files in provided relative dir"""
     files = []
     for dirname, dirnames, filenames in os.walk(idir):
         for subdirname in dirnames:
             files.append(os.path.join(dirname, subdirname))
```

