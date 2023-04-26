# Comparing `tmp/recurrent-memory-transformer-pytorch-0.2.0.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.0.tar", last modified: Wed Apr 26 14:26:03 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.1.tar", last modified: Wed Apr 26 14:32:37 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.2.0.tar` & `recurrent-memory-transformer-pytorch-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:37.211166 recurrent-memory-transformer-pytorch-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:32:37.211166 recurrent-memory-transformer-pytorch-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:37.211166 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17162 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:37.211166 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:32:37.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 14:32:37.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:32:37.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 14:32:37.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:32:37.000000 recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:32:37.211166 recurrent-memory-transformer-pytorch-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 14:32:26.000000 recurrent-memory-transformer-pytorch-0.2.1/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/LICENSE` & `recurrent-memory-transformer-pytorch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/README.md` & `recurrent-memory-transformer-pytorch-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -189,7 +189,18 @@
     author  = {Anonymous},
     booktitle = {Submitted to The Tenth International Conference on Learning Representations },
     year    = {2022},
     url     = {https://openreview.net/forum?id=GMYWzWztDx5},
     note    = {under review}
 }
 ```
+
+```bibtex
+@misc{ding2021erniedoc,
+    title   = {ERNIE-Doc: A Retrospective Long-Document Modeling Transformer},
+    author  = {Siyu Ding and Junyuan Shang and Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang},
+    year    = {2021},
+    eprint  = {2012.15688},
+    archivePrefix = {arXiv},
+    primaryClass = {cs.CL}
+}
+```
```

#### html2text {}

```diff
@@ -65,7 +65,12 @@
 zenodo.5146400}, license = {Apache-2.0}, month = {jul}, title = {{DALLÂ·E
 Mini}}, url = {https://github.com/borisdayma/dalle-mini}, version = {v0.1-
 alpha}, year = {2021}} ``` ```bibtex @inproceedings{anonymous2022normformer,
 title = {NormFormer: Improved Transformer Pretraining with Extra
 Normalization}, author = {Anonymous}, booktitle = {Submitted to The Tenth
 International Conference on Learning Representations }, year = {2022}, url =
 {https://openreview.net/forum?id=GMYWzWztDx5}, note = {under review} } ```
+```bibtex @misc{ding2021erniedoc, title = {ERNIE-Doc: A Retrospective Long-
+Document Modeling Transformer}, author = {Siyu Ding and Junyuan Shang and
+Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang}, year =
+{2021}, eprint = {2012.15688}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,16 +205,17 @@
         use_flash_attn = False,
         ignore_index = -1,
         abs_pos_emb = True,
         rotary_pos_emb = False,
         token_shift = True,
         use_xl_memories = False,
         xl_mem_len = None,
-        emb_gradient_frac = 0.1,   # trick from cogview paper that leads to a bit more stability
-        memory_not_causal = True,  # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
+        enhanced_xl_recurrence = False,     # add simple method for enhancing receptive field of xl memories, from ernie-doc paper
+        emb_gradient_frac = 0.1,            # trick from cogview paper that leads to a bit more stability
+        memory_not_causal = True,           # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
         self.emb_gradient_frac = emb_gradient_frac
 
@@ -247,14 +248,16 @@
         xl_mem_len = default(xl_mem_len, seq_len)
         assert xl_mem_len <= seq_len
         self.xl_mem_len = xl_mem_len
 
         self.use_xl_memories = use_xl_memories
         assert not (rotary_pos_emb and use_xl_memories), 'rotary not compatible with xl memories yet'
 
+        self.enhanced_xl_recurrence = enhanced_xl_recurrence
+
         # layers
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
@@ -347,17 +350,21 @@
 
             rotary_emb = self.rotary_pos_emb(pos)
 
         shift_fn = partial(self.maybe_token_shift, ps = ps)
 
         # prepare xl memories
 
-        xl_memories_iter = iter(default(xl_memories, []))
+        xl_memories = default(xl_memories, [])
+        xl_memories_iter = iter(xl_memories)
         new_xl_memories = []
 
+        if self.enhanced_xl_recurrence and len(xl_memories) > 1:  # simply shift all the xl memories down by one, so lower layer gets access to representations from layer above
+            xl_memories = [*xl_memories[1:], xl_memories[0]]
+
         # attention and feedforward
 
         for attn, ff in self.layers:
             attn_out, xl_memories = attn(shift_fn(x), mask = mask, xl_memories = next(xl_memories_iter, None), rotary_emb = rotary_emb)
             new_xl_memories.append(xl_memories)
 
             x = x + attn_out
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.0/setup.py` & `recurrent-memory-transformer-pytorch-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.0',
+  version = '0.2.1',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

