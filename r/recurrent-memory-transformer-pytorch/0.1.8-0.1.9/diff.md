# Comparing `tmp/recurrent-memory-transformer-pytorch-0.1.8.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.1.8.tar", last modified: Wed Apr 26 03:29:56 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.1.9.tar", last modified: Wed Apr 26 13:37:16 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.1.8.tar` & `recurrent-memory-transformer-pytorch-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:29:56.757645 recurrent-memory-transformer-pytorch-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 03:29:56.757645 recurrent-memory-transformer-pytorch-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:29:56.757645 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:29:56.757645 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 03:29:56.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 03:29:56.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:29:56.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 03:29:56.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 03:29:56.000000 recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 03:29:56.757645 recurrent-memory-transformer-pytorch-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 03:29:46.000000 recurrent-memory-transformer-pytorch-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/LICENSE` & `recurrent-memory-transformer-pytorch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/README.md` & `recurrent-memory-transformer-pytorch-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,18 @@
     year      = {2021},
     publisher = {Zenodo},
     version   = {0.01},
     doi       = {10.5281/zenodo.5196578},
     url       = {https://doi.org/10.5281/zenodo.5196578}
 }
 ```
+
+```bibtex
+@misc{ding2021cogview,
+    title   = {CogView: Mastering Text-to-Image Generation via Transformers},
+    author  = {Ming Ding and Zhuoyi Yang and Wenyi Hong and Wendi Zheng and Chang Zhou and Da Yin and Junyang Lin and Xu Zou and Zhou Shao and Hongxia Yang and Jie Tang},
+    year    = {2021},
+    eprint  = {2105.13290},
+    archivePrefix = {arXiv},
+    primaryClass = {cs.CV}
+}
+```
```

#### html2text {}

```diff
@@ -50,8 +50,13 @@
 {2104.09864}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex
 @inproceedings{Wu2020MemformerAM, title = {Memformer: A Memory-Augmented
 Transformer for Sequence Modeling}, author = {Qingyang Wu and Zhenzhong Lan and
 Kun Qian and Jing Gu and Alborz Geramifard and Zhou Yu}, booktitle = {AACL/
 IJCNLP}, year = {2020} } ``` ```bibtex @software{peng_bo_2021_5196578, author =
 {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year = {2021},
 publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578}, url =
-{https://doi.org/10.5281/zenodo.5196578} } ```
+{https://doi.org/10.5281/zenodo.5196578} } ``` ```bibtex @misc{ding2021cogview,
+title = {CogView: Mastering Text-to-Image Generation via Transformers}, author
+= {Ming Ding and Zhuoyi Yang and Wenyi Hong and Wendi Zheng and Chang Zhou and
+Da Yin and Junyang Lin and Xu Zou and Zhou Shao and Hongxia Yang and Jie Tang},
+year = {2021}, eprint = {2105.13290}, archivePrefix = {arXiv}, primaryClass =
+{cs.CV} } ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat, pack, unpack
 
 from recurrent_memory_transformer_pytorch.attend import Attend
 
+# constants
+
+Linear = partial(nn.Linear, bias = False)
+
 # helpers
 
 def exists(val):
     return val is not None
 
 def identity(t, *args, **kwargs):
     return t
@@ -59,14 +63,20 @@
 def token_shift_fn(t, ps):
     read_mem, t, write_mem = unpack(t, ps, 'b * d')
     t, t_shift = t.chunk(2, dim = -1)
     t_shift = F.pad(t_shift, (0, 0, 1, -1), value = 0.)
     t = torch.cat((t, t_shift), dim = -1)
     return torch.cat((read_mem, t, write_mem), dim = -2)
 
+def frac_gradient(t, frac = 1.):
+    if frac == 1.:
+        return t
+
+    return t * frac + t.detach() * (1. - frac)
+
 # rotary embedding
 
 class RotaryEmbedding(nn.Module):
     def __init__(self, dim, theta = 32768):
         super().__init__()
         inv_freq = 1. / (theta ** (torch.arange(0, dim, 2).float() / dim))
         self.register_buffer('inv_freq', inv_freq)
@@ -101,17 +111,18 @@
         x, gate = x.chunk(2, dim = -1)
         return x * F.gelu(gate)
 
 def FeedForward(dim, mult = 4):
     dim_inner = int(dim * mult * 2 / 3)
     return nn.Sequential(
         RMSNorm(dim),
-        nn.Linear(dim, dim_inner * 2),
+        Linear(dim, dim_inner * 2, bias = False),
         GEGLU(),
-        nn.Linear(dim_inner, dim)
+        RMSNorm(dim_inner),
+        Linear(dim_inner, dim, bias = False)
     )
 
 # attention
 
 class Attention(nn.Module):
     def __init__(
         self,
@@ -132,17 +143,17 @@
             causal = causal and not use_custom_causal_attn_mask,
             dropout = dropout,
             use_flash = use_flash_attn
         )
 
         self.norm = RMSNorm(dim)
 
-        self.to_q = nn.Linear(dim, dim_inner, bias = False)
-        self.to_kv = nn.Linear(dim, dim_inner * 2, bias = False)
-        self.to_out = nn.Linear(dim_inner, dim, bias = False)
+        self.to_q = Linear(dim, dim_inner)
+        self.to_kv = Linear(dim, dim_inner * 2)
+        self.to_out = Linear(dim_inner, dim)
 
     def forward(
         self,
         x,
         rotary_emb = None,
         mask = None
     ):
@@ -180,20 +191,23 @@
         heads = 8,
         ff_mult = 4,
         use_flash_attn = False,
         ignore_index = -1,
         abs_pos_emb = True,
         rotary_pos_emb = False,
         token_shift = True,
-        memory_not_causal = True # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
+        emb_gradient_frac = 0.1,   # trick from cogview paper that leads to a bit more stability
+        memory_not_causal = True,  # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
+        self.emb_gradient_frac = emb_gradient_frac
+
         assert num_memory_tokens > 0
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         # positions
 
         assert any([abs_pos_emb, rotary_pos_emb, token_shift])
@@ -229,15 +243,15 @@
                     use_custom_causal_attn_mask = memory_not_causal
                 ),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
         self.to_logits = nn.Sequential(
             RMSNorm(dim),
-            nn.Linear(dim, num_tokens, bias = False)
+            nn.Linear(dim, num_tokens)
         )
 
         self.ignore_index = ignore_index
 
         # whether to use custom attention mask if causal and memory should not be causal
 
         self.use_custom_causal_attn_mask = causal and memory_not_causal
@@ -260,14 +274,18 @@
         x = self.token_emb(x)
 
         # maybe absolute positional embedding
 
         if exists(self.pos_emb):
             x = x + self.pos_emb(pos)
 
+        # trick from cogview paper
+
+        x = frac_gradient(x, self.emb_gradient_frac)
+
         # prepare read and write memories, as in paper
 
         write_memories = self.init_memory(b)
 
         if exists(read_memories):
             read_mem_length = mem_length
             read_memories = read_memories + self.read_memory_emb
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.8/setup.py` & `recurrent-memory-transformer-pytorch-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

