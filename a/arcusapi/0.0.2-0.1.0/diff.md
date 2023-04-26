# Comparing `tmp/arcusapi-0.0.2.tar.gz` & `tmp/arcusapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcusapi-0.0.2.tar", last modified: Fri Mar  3 17:46:24 2023, max compression
+gzip compressed data, was "arcusapi-0.1.0.tar", last modified: Wed Apr 26 02:47:53 2023, max compression
```

## Comparing `arcusapi-0.0.2.tar` & `arcusapi-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,56 @@
-drwxr-xr-x   0 kunalgosar   (501) staff       (20)        0 2023-03-03 17:46:24.510086 arcusapi-0.0.2/
--rw-r--r--   0 kunalgosar   (501) staff       (20)    11344 2023-03-03 16:40:32.000000 arcusapi-0.0.2/LICENSE
--rw-r--r--   0 kunalgosar   (501) staff       (20)      568 2023-03-03 17:46:24.509733 arcusapi-0.0.2/PKG-INFO
--rw-r--r--   0 kunalgosar   (501) staff       (20)       47 2023-03-03 17:26:39.000000 arcusapi-0.0.2/README.md
--rw-r--r--   0 kunalgosar   (501) staff       (20)      588 2023-03-03 17:46:09.000000 arcusapi-0.0.2/pyproject.toml
--rw-r--r--   0 kunalgosar   (501) staff       (20)       38 2023-03-03 17:46:24.510193 arcusapi-0.0.2/setup.cfg
-drwxr-xr-x   0 kunalgosar   (501) staff       (20)        0 2023-03-03 17:46:24.503979 arcusapi-0.0.2/src/
-drwxr-xr-x   0 kunalgosar   (501) staff       (20)        0 2023-03-03 17:46:24.507580 arcusapi-0.0.2/src/arcus/
--rw-r--r--   0 kunalgosar   (501) staff       (20)       34 2023-03-03 17:42:37.000000 arcusapi-0.0.2/src/arcus/__init__.py
--rw-r--r--   0 kunalgosar   (501) staff       (20)      157 2023-03-03 16:45:37.000000 arcusapi-0.0.2/src/arcus/api.py
-drwxr-xr-x   0 kunalgosar   (501) staff       (20)        0 2023-03-03 17:46:24.509325 arcusapi-0.0.2/src/arcusapi.egg-info/
--rw-r--r--   0 kunalgosar   (501) staff       (20)      568 2023-03-03 17:46:24.000000 arcusapi-0.0.2/src/arcusapi.egg-info/PKG-INFO
--rw-r--r--   0 kunalgosar   (501) staff       (20)      215 2023-03-03 17:46:24.000000 arcusapi-0.0.2/src/arcusapi.egg-info/SOURCES.txt
--rw-r--r--   0 kunalgosar   (501) staff       (20)        1 2023-03-03 17:46:24.000000 arcusapi-0.0.2/src/arcusapi.egg-info/dependency_links.txt
--rw-r--r--   0 kunalgosar   (501) staff       (20)        6 2023-03-03 17:46:24.000000 arcusapi-0.0.2/src/arcusapi.egg-info/top_level.txt
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.072070 arcusapi-0.1.0/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.0/LICENSE
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-04-26 02:47:53.071889 arcusapi-0.1.0/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-04-26 02:14:25.000000 arcusapi-0.1.0/README.md
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.060102 arcusapi-0.1.0/arcus/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3263 2023-04-18 15:39:42.000000 arcusapi-0.1.0/arcus/api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      957 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1435 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.060556 arcusapi-0.1.0/arcus/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      687 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.064714 arcusapi-0.1.0/arcus/model/shared/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/shared/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1707 2023-04-19 17:39:01.000000 arcusapi-0.1.0/arcus/model/shared/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/shared/data.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     5669 2023-04-24 21:56:28.000000 arcusapi-0.1.0/arcus/model/shared/metrics.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     9379 2023-04-24 21:56:45.000000 arcusapi-0.1.0/arcus/model/shared/trial.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.065981 arcusapi-0.1.0/arcus/model/torch/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1228 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.067707 arcusapi-0.1.0/arcus/model/torch/data/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/data_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/data_loader.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/torch/data/data_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/torch/data/dataset.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/lightning_utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2867 2023-04-24 21:57:55.000000 arcusapi-0.1.0/arcus/model/torch/data/tensor.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3196 2023-04-24 21:58:58.000000 arcusapi-0.1.0/arcus/model/torch/metrics.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.068965 arcusapi-0.1.0/arcus/model/torch/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/embedding_getter.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/model_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-04-19 17:39:01.000000 arcusapi-0.1.0/arcus/model/torch/model/module.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-14 04:36:28.000000 arcusapi-0.1.0/arcus/model/torch/model/utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11284 2023-04-18 15:39:42.000000 arcusapi-0.1.0/arcus/model/torch/trainer.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3860 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/utils.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.069346 arcusapi-0.1.0/arcus/prompt/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/__init.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.069792 arcusapi-0.1.0/arcus/prompt/text/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1006 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/config.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.070346 arcusapi-0.1.0/arcus/prompt/text/llms/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/llm.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3706 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/openai.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.071049 arcusapi-0.1.0/arcusapi.egg-info/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1219 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)       87 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/requires.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/top_level.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      725 2023-04-24 03:38:46.000000 arcusapi-0.1.0/pyproject.toml
+-rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-04-26 02:47:53.072116 arcusapi-0.1.0/setup.cfg
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.071467 arcusapi-0.1.0/tests/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3472 2023-04-18 15:39:42.000000 arcusapi-0.1.0/tests/test_api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.0/tests/test_constants.py
```

### Comparing `arcusapi-0.0.2/LICENSE` & `arcusapi-0.1.0/LICENSE`

 * *Files identical despite different names*

