# Comparing `tmp/auto_gptq-0.0.4.tar.gz` & `tmp/auto_gptq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.0.4.tar", last modified: Wed Apr 26 05:57:33 2023, max compression
+gzip compressed data, was "auto_gptq-0.0.5.tar", last modified: Wed Apr 26 10:01:56 2023, max compression
```

## Comparing `auto_gptq-0.0.4.tar` & `auto_gptq-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.845845 auto_gptq-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-04-23 08:35:20.000000 auto_gptq-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 05:57:33.845845 auto_gptq-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9621 2023-04-26 05:56:45.000000 auto_gptq-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.839845 auto_gptq-0.0.4/auto_gptq/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.841845 auto_gptq-0.0.4/auto_gptq/eval_tasks/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.841845 auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/language_modeling_task.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/eval_tasks/text_summarization_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.843845 auto_gptq-0.0.4/auto_gptq/modeling/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-24 05:55:08.000000 auto_gptq-0.0.4/auto_gptq/modeling/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15567 2023-04-26 05:56:39.000000 auto_gptq-0.0.4/auto_gptq/modeling/_base.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/modeling/_const.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-04-26 05:56:45.000000 auto_gptq-0.0.4/auto_gptq/modeling/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/modeling/auto.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-24 17:06:09.000000 auto_gptq-0.0.4/auto_gptq/modeling/bloom.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 17:09:50.000000 auto_gptq-0.0.4/auto_gptq/modeling/gpt_neox.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-23 08:35:20.000000 auto_gptq-0.0.4/auto_gptq/modeling/gptj.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-23 08:35:20.000000 auto_gptq-0.0.4/auto_gptq/modeling/llama.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/modeling/moss.py
--rw-r--r--   0 root         (0) root         (0)      696 2023-04-23 08:35:20.000000 auto_gptq-0.0.4/auto_gptq/modeling/opt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.843845 auto_gptq-0.0.4/auto_gptq/nn_modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/nn_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9822 2023-04-26 05:56:45.000000 auto_gptq-0.0.4/auto_gptq/nn_modules/qlinear.py
--rw-r--r--   0 root         (0) root         (0)    18408 2023-04-26 05:56:45.000000 auto_gptq-0.0.4/auto_gptq/nn_modules/qlinear_triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.844845 auto_gptq-0.0.4/auto_gptq/nn_modules/triton_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/nn_modules/triton_utils/custom_autotune.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.844845 auto_gptq-0.0.4/auto_gptq/quantization/
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/quantization/gptq.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/auto_gptq/quantization/quantizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.840845 auto_gptq-0.0.4/auto_gptq.egg-info/
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 05:57:33.000000 auto_gptq-0.0.4/auto_gptq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1279 2023-04-26 05:57:33.000000 auto_gptq-0.0.4/auto_gptq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 05:57:33.000000 auto_gptq-0.0.4/auto_gptq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-04-26 05:57:33.000000 auto_gptq-0.0.4/auto_gptq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 05:57:33.000000 auto_gptq-0.0.4/auto_gptq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:57:33.844845 auto_gptq-0.0.4/quant_cuda/
--rw-r--r--   0 root         (0) root         (0)     2287 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/quant_cuda/quant_cuda.cpp
--rw-r--r--   0 root         (0) root         (0)    12817 2023-04-25 18:02:10.000000 auto_gptq-0.0.4/quant_cuda/quant_cuda_kernel.cu
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 05:57:33.845845 auto_gptq-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1419 2023-04-26 05:56:45.000000 auto_gptq-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.646464 auto_gptq-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9621 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.641464 auto_gptq-0.0.5/auto_gptq/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.642464 auto_gptq-0.0.5/auto_gptq/eval_tasks/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.642464 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/eval_tasks/text_summarization_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/modeling/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-24 05:55:08.000000 auto_gptq-0.0.5/auto_gptq/modeling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15952 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_base.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_const.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/auto.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-24 17:06:09.000000 auto_gptq-0.0.5/auto_gptq/modeling/bloom.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 17:09:50.000000 auto_gptq-0.0.5/auto_gptq/modeling/gpt_neox.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/gptj.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/llama.py
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/modeling/moss.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-23 08:35:20.000000 auto_gptq-0.0.5/auto_gptq/modeling/opt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/nn_modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9822 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear.py
+-rw-r--r--   0 root         (0) root         (0)    18408 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear_triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.644464 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/auto_gptq/quantization/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/gptq.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/auto_gptq/quantization/quantizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.641464 auto_gptq-0.0.5/auto_gptq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 10:01:56.000000 auto_gptq-0.0.5/auto_gptq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:01:56.645464 auto_gptq-0.0.5/quant_cuda/
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/quant_cuda/quant_cuda.cpp
+-rw-r--r--   0 root         (0) root         (0)    12817 2023-04-26 09:57:15.000000 auto_gptq-0.0.5/quant_cuda/quant_cuda_kernel.cu
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:01:56.646464 auto_gptq-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-04-26 10:00:09.000000 auto_gptq-0.0.5/setup.py
```

### Comparing `auto_gptq-0.0.4/LICENSE` & `auto_gptq-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/README.md` & `auto_gptq-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AutoGPTQ
 An easy-to-use model quantization package with user-friendly apis, based on GPTQ algorithm.
 
 ## News or Update
-- 2023-04-25 - (Update) - Using `triton` to speed up inference is now supported.
+- 2023-04-26 - (Update) - Using `triton` to speed up inference is now supported.
 - 2023-04-25 - (News&Update) - [MOSS](https://github.com/OpenLMLab/MOSS) is an open-source tool-augmented conversational language model from Fudan University, quantization is now supported in AutoGPTQ.
 - 2023-04-23 - (Update) - Support evaluation on multiple (down-stream) tasks such as: language-modeling, text-classification, text-summarization.
 - 2023-04-22 - (News) - qwopqwop200's [AutoGPTQ-triton](https://github.com/qwopqwop200/AutoGPTQ-triton) provides faster speed to integrate with quantized model, for everyone who can access to triton, try and enjoy yourself!
 - 2023-04-20 - (News) - AutoGPTQ is automatically compatible with Stability-AI's newly released `gpt_neox` type model family [StableLM](https://github.com/Stability-AI/StableLM).
 - 2023-04-16 - (Update) - Support quantization and inference for `bloom`, `gpt_neox`, `gptj`, `llama` and `opt`.
 
 ## Installation
```

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/data_utils.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/sequence_classification_task.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/sequence_classification_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/eval_tasks/text_summarization_task.py` & `auto_gptq-0.0.5/auto_gptq/eval_tasks/text_summarization_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/modeling/_base.py` & `auto_gptq-0.0.5/auto_gptq/modeling/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from typing import Dict, List, Union
 
 import torch
 import torch.nn as nn
 import transformers
 from safetensors.torch import load_file as safe_load, save_file as safe_save
 from transformers import AutoConfig, AutoModelForCausalLM, PreTrainedModel
+from transformers.utils.hub import PushToHubMixin
 
 from ._const import *
 from ._utils import *
 from ..quantization import GPTQ
 
 logger = getLogger(__name__)
 
 
 @dataclass
-class BaseQuantizeConfig:
+class BaseQuantizeConfig(PushToHubMixin):
     bits: int = field(default=4, metadata={"choices": [2, 3, 4, 8]})
     damp_percent: float = field(default=0.01)
     desc_act: bool = field(default=True)
     group_size: int = field(default=-1)
 
     def __post_init__(self):
         fields_info = fields(self)
@@ -31,15 +32,15 @@
         if self.bits not in fields_info[0].metadata["choices"]:
             raise ValueError(f"only support quantize to {fields_info[0].metadata['choices']} bits.")
         if not (0 < self.damp_percent < 1):
             raise ValueError("damp_percent must between 0 and 1.")
         if self.group_size != -1 and self.group_size <= 0:
             raise ValueError("unless equal to -1, group_size must greater then 0.")
 
-    def save_pretrained(self, save_dir: str):
+    def save_pretrained(self, save_dir: str, **kwargs):
         with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
             json.dump(self.to_dict(), f, indent=2)
 
     @classmethod
     def from_pretrained(cls, save_dir: str):
         with open(join(save_dir, "quantize_config.json"), "r", encoding="utf-8") as f:
             return cls(**json.load(f))
@@ -49,15 +50,15 @@
             "bits": self.bits,
             "damp_percent": self.damp_percent,
             "desc_act": self.desc_act,
             "group_size": self.group_size
         }
 
 
-class BaseGPTQForCausalLM(nn.Module):
+class BaseGPTQForCausalLM(nn.Module, PushToHubMixin):
     layers_block_name: str = None
     outside_layer_modules: List[str] = None
     inside_layer_modules: List[List[str]] = None
     lm_head_name: str = "lm_head"
 
     def __init__(self, model: PreTrainedModel, quantized: bool, quantize_config: BaseQuantizeConfig):
         super().__init__()
@@ -289,14 +290,19 @@
         else:
             model_save_name += ".bin"
             torch.save(self.model.state_dict(), join(save_dir, model_save_name))
 
         self.model.config.save_pretrained(save_dir)
         self.quantize_config.save_pretrained(save_dir)
 
+    def save_pretrained(self, save_dir: str, use_safetensors: bool = False, **kwargs):
+        """alias of save_quantized"""
+        logger.warning("you are using save_pretrained, which will re-direct to save_quantized.")
+        self.save_quantized(save_dir, use_safetensors)
+
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path: str,
         quantize_config: BaseQuantizeConfig,
         bf16: bool = False,
         **model_init_kwargs
@@ -318,15 +324,15 @@
         model_init_kwargs["device_map"] = None
         model_init_kwargs["torch_dtype"] = torch.bfloat16 if bf16 else torch.float16
         model_init_kwargs["low_cpu_mem_usage"] = False
         model_init_kwargs["trust_remote_code"] = True
 
         model = AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path, **model_init_kwargs)
         model_config = model.config.to_dict()
-        seq_len_keys = ["max_position_embeddings", "seq_length"]
+        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
         if any([k in model_config for k in seq_len_keys]):
             for key in seq_len_keys:
                 if key in model_config:
                     model.seqlen = model_config[key]
                     break
         else:
             logger.warning("can't get model's sequence length from model config, will set to 4096.")
```

### Comparing `auto_gptq-0.0.4/auto_gptq/modeling/_utils.py` & `auto_gptq-0.0.5/auto_gptq/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/modeling/auto.py` & `auto_gptq-0.0.5/auto_gptq/modeling/auto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._base import BaseQuantizeConfig
+from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
 from ._utils import check_and_get_model_type
 from .bloom import BloomGPTQForCausalLM
 from .gpt_neox import GPTNeoXGPTQForCausalLM
 from .gptj import GPTJGPTQForCausalLM
 from .llama import LlamaGPTQForCausalLM
 from .moss import MOSSGPTQForCausalLM
 from .opt import OPTGPTQForCausalLM
@@ -29,15 +29,15 @@
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path: str,
         quantize_config: BaseQuantizeConfig,
         bf16: bool = False,
         **model_init_kwargs
-    ):
+    ) -> BaseGPTQForCausalLM:
         model_type = check_and_get_model_type(pretrained_model_name_or_path)
         return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
             pretrained_model_name_or_path=pretrained_model_name_or_path,
             quantize_config=quantize_config,
             bf16=bf16,
             **model_init_kwargs
         )
@@ -45,15 +45,15 @@
     @classmethod
     def from_quantized(
         cls,
         save_dir: str,
         device: str = "cpu",
         use_safetensors: bool = False,
         use_triton: bool = False
-    ):
+    ) -> BaseGPTQForCausalLM:
         model_type = check_and_get_model_type(save_dir)
         return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized(
             save_dir=save_dir,
             device=device,
             use_safetensors=use_safetensors,
             use_triton=use_triton
         )
```

### Comparing `auto_gptq-0.0.4/auto_gptq/modeling/llama.py` & `auto_gptq-0.0.5/auto_gptq/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/modeling/opt.py` & `auto_gptq-0.0.5/auto_gptq/modeling/opt.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/nn_modules/qlinear.py` & `auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/nn_modules/qlinear_triton.py` & `auto_gptq-0.0.5/auto_gptq/nn_modules/qlinear_triton.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.0.5/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/quantization/gptq.py` & `auto_gptq-0.0.5/auto_gptq/quantization/gptq.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.0.5/auto_gptq/quantization/quantizer.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.0.5/auto_gptq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/quant_cuda/quant_cuda.cpp` & `auto_gptq-0.0.5/quant_cuda/quant_cuda.cpp`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/quant_cuda/quant_cuda_kernel.cu` & `auto_gptq-0.0.5/quant_cuda/quant_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.0.4/setup.py` & `auto_gptq-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 try:
     import torch
     TORCH_AVAILABLE = True
 except ImportError:
     TORCH_AVAILABLE = False
 
+version = "v0.0.5"
 
 requirements = [
     "datasets",
     "numpy",
     "rouge",
     "torch>=1.13.0",
     "safetensors",
@@ -42,22 +43,22 @@
         additional_setup_kwargs = {
             "ext_modules": extensions,
             "cmdclass": {'build_ext': cpp_extension.BuildExtension}
         }
     setup(
         name="auto_gptq",
         packages=find_packages(),
-        version="v0.0.4",
+        version=version,
         install_requires=requirements,
         extras_require=extras_require,
         include_dirs=["quant_cuda"],
         **additional_setup_kwargs
     )
 else:
     setup(
         name="auto_gptq",
         packages=find_packages(),
-        version="v0.0.4",
+        version=version,
         install_requires=requirements,
         extras_require=extras_require,
         include_dirs=["quant_cuda"]
     )
```

