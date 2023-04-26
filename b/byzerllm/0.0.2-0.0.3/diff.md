# Comparing `tmp/byzerllm-0.0.2.tar.gz` & `tmp/byzerllm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.0.2.tar", last modified: Mon Apr 24 12:10:10 2023, max compression
+gzip compressed data, was "byzerllm-0.0.3.tar", last modified: Wed Apr 26 03:16:20 2023, max compression
```

## Comparing `byzerllm-0.0.2.tar` & `byzerllm-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.881198 byzerllm-0.0.2/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-24 12:10:10.880917 byzerllm-0.0.2/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-04-24 12:10:10.881274 byzerllm-0.0.2/setup.cfg
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1205 2023-04-24 12:09:56.000000 byzerllm-0.0.2/setup.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.872729 byzerllm-0.0.2/src/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.873929 byzerllm-0.0.2/src/byzerllm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:26:20.000000 byzerllm-0.0.2/src/byzerllm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.877472 byzerllm-0.0.2/src/byzerllm/chatglm6b/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/arguments.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/trainer_seq2seq.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.878806 byzerllm-0.0.2/src/byzerllm/moss/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/finetune_moss.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.880586 byzerllm-0.0.2/src/byzerllm/moss/models/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/configuration_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/custom_autotune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/modeling_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/quantization.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/tokenization_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/moss_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.875360 byzerllm-0.0.2/src/byzerllm.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      707 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/dependency_links.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.102621 byzerllm-0.0.3/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-26 03:16:20.102350 byzerllm-0.0.3/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-04-26 03:16:20.102692 byzerllm-0.0.3/setup.cfg
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1205 2023-04-24 12:09:56.000000 byzerllm-0.0.3/setup.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.091097 byzerllm-0.0.3/src/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.092495 byzerllm-0.0.3/src/byzerllm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:26:20.000000 byzerllm-0.0.3/src/byzerllm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.096000 byzerllm-0.0.3/src/byzerllm/chatglm6b/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/arguments.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.3/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.097880 byzerllm-0.0.3/src/byzerllm/dolly/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/consts.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/dolly_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/generate.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/dolly/trainer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.098892 byzerllm-0.0.3/src/byzerllm/moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/finetune_moss.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.101769 byzerllm-0.0.3/src/byzerllm/moss/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/configuration_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/custom_autotune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/modeling_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/quantization.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/models/tokenization_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.3/src/byzerllm/moss/moss_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-04-26 03:16:05.000000 byzerllm-0.0.3/src/byzerllm/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-26 03:16:20.093831 byzerllm-0.0.3/src/byzerllm.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      866 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/dependency_links.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-04-26 03:16:20.000000 byzerllm-0.0.3/src/byzerllm.egg-info/top_level.txt
```

### Comparing `byzerllm-0.0.2/setup.py` & `byzerllm-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.0.3/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.0.3/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.0.3/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.0.3/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.0.3/src/byzerllm/moss/models/configuration_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.0.3/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.0.3/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.0.3/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.0.3/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.0.3/src/byzerllm/moss/moss_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.2/src/byzerllm.egg-info/SOURCES.txt` & `byzerllm-0.0.3/src/byzerllm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 src/byzerllm.egg-info/SOURCES.txt
 src/byzerllm.egg-info/dependency_links.txt
 src/byzerllm.egg-info/top_level.txt
 src/byzerllm/chatglm6b/__init__.py
 src/byzerllm/chatglm6b/arguments.py
 src/byzerllm/chatglm6b/finetune.py
 src/byzerllm/chatglm6b/trainer_seq2seq.py
+src/byzerllm/dolly/__init__.py
+src/byzerllm/dolly/consts.py
+src/byzerllm/dolly/dolly_inference.py
+src/byzerllm/dolly/generate.py
+src/byzerllm/dolly/trainer.py
 src/byzerllm/moss/__init__.py
 src/byzerllm/moss/finetune_moss.py
 src/byzerllm/moss/moss_inference.py
 src/byzerllm/moss/models/__init__.py
 src/byzerllm/moss/models/configuration_moss.py
 src/byzerllm/moss/models/custom_autotune.py
 src/byzerllm/moss/models/modeling_moss.py
```

