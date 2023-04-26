# Comparing `tmp/optimum-neuron-0.0.2.tar.gz` & `tmp/optimum-neuron-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.2.tar", last modified: Wed Apr 19 16:48:44 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.3.tar", last modified: Wed Apr 26 08:34:48 2023, max compression
```

## Comparing `optimum-neuron-0.0.2.tar` & `optimum-neuron-0.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.2/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.2/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     4755 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4523 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.977402 optimum-neuron-0.0.2/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4655 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12023 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/exporters/neuron/model_configs.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.2/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/neuron/trainers.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4745 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17609 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.2/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-04-19 16:23:48.000000 optimum-neuron-0.0.2/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1193 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      277 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-04-19 16:48:44.000000 optimum-neuron-0.0.2/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2549 2023-04-19 16:48:33.000000 optimum-neuron-0.0.2/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-19 16:48:44.981402 optimum-neuron-0.0.2/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    23763 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    26361 2023-04-17 13:39:59.000000 optimum-neuron-0.0.2/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.2/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.2/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.3/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.3/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4755 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4523 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4655 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12023 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/model_configs.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.3/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-24 14:58:35.000000 optimum-neuron-0.0.3/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/trainers.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4745 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17609 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.3/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1193 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      301 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2582 2023-04-26 08:34:38.000000 optimum-neuron-0.0.3/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    23763 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    26361 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.3/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.2/LICENSE` & `optimum-neuron-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/MANIFEST.in` & `optimum-neuron-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/PKG-INFO` & `optimum-neuron-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.2
+Version: 0.0.3
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.2/README.md` & `optimum-neuron-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.3/optimum/commands/export/neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.3/optimum/commands/export/neuronx.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.3/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/__main__.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/config.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.3/optimum/exporters/neuron/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/__init__.py` & `optimum-neuron-0.0.3/optimum/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.3/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.3/optimum/neuron/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/trainers.py` & `optimum-neuron-0.0.3/optimum/neuron/trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/argument_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.3/optimum/neuron/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/optimum/neuron/version.py` & `optimum-neuron-0.0.3/optimum/neuron/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `optimum-neuron-0.0.2/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.3/optimum_neuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.2
+Version: 0.0.3
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.2/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.3/optimum_neuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/pyproject.toml` & `optimum-neuron-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/setup.py` & `optimum-neuron-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
     "transformers >= 4.28.0",
     "optimum",
+    "huggingface_hub >= 0.14.0",
 ]
 
 TESTS_REQUIRE = [
     "pytest",
     "psutil",
     "parameterized",
     "GitPython",
```

### Comparing `optimum-neuron-0.0.2/tests/test_cache_utils.py` & `optimum-neuron-0.0.3/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/tests/test_examples.py` & `optimum-neuron-0.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/tests/test_trainer_callback.py` & `optimum-neuron-0.0.3/tests/test_trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/tests/test_trainers.py` & `optimum-neuron-0.0.3/tests/test_trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.2/tests/test_utils.py` & `optimum-neuron-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

