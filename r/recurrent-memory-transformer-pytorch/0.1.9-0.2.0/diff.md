# Comparing `tmp/recurrent-memory-transformer-pytorch-0.1.9.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.1.9.tar", last modified: Wed Apr 26 13:37:16 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.0.tar", last modified: Wed Apr 26 14:26:03 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.1.9.tar` & `recurrent-memory-transformer-pytorch-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 13:37:16.000000 recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:37:16.317594 recurrent-memory-transformer-pytorch-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 13:37:00.000000 recurrent-memory-transformer-pytorch-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:26:03.000000 recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:26:03.650043 recurrent-memory-transformer-pytorch-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 14:25:40.000000 recurrent-memory-transformer-pytorch-0.2.0/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/LICENSE` & `recurrent-memory-transformer-pytorch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.1.9
+Version: 0.2.0
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/README.md` & `recurrent-memory-transformer-pytorch-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     heads = 8,                        # heads
     seq_len = 1024,                   # sequence length of a segment
     use_flash_attn = True             # whether to use flash attention
 )
 
 x = torch.randint(0, 256, (1, 1024))
 
-logits1, mem1 = model(x)        # (1, 1024, 20000), (1, 128, 512)
-logits2, mem2 = model(x, mem1)  # (1, 1024, 20000), (1, 128, 512)
-logits3, mem3 = model(x, mem2)  # (1, 1024, 20000), (1, 128, 512)
+logits1, mem1, _ = model(x)        # (1, 1024, 20000), (1, 128, 512), None
+logits2, mem2, _ = model(x, mem1)  # (1, 1024, 20000), (1, 128, 512), None
+logits3, mem3, _ = model(x, mem2)  # (1, 1024, 20000), (1, 128, 512), None
 
 # and so on ...
 
 ```
 
 Train on an absurdly long sequence
 
@@ -67,16 +67,17 @@
 
 loss = model(seq, memory_replay_backprop = True) # memory efficient training from memformer paper
 
 ```
 
 ## Todo
 
-- [ ] add sliding windows as an option, detached or with memory propagated using MRBP
+- [ ] get rotary embeddings working properly with xl memories
 
+- [x] add xl memories, detached
 - [x] offer a way to turn off rotary embeddings, absolute positional embeddings, and add token shift
 - [x] make memories being causally masked an option
 - [x] add the memory replay backprop technique from memformer paper
 - [x] relative positional encoding
 
 ## Alternatives
 
@@ -165,7 +166,30 @@
     author  = {Ming Ding and Zhuoyi Yang and Wenyi Hong and Wendi Zheng and Chang Zhou and Da Yin and Junyang Lin and Xu Zou and Zhou Shao and Hongxia Yang and Jie Tang},
     year    = {2021},
     eprint  = {2105.13290},
     archivePrefix = {arXiv},
     primaryClass = {cs.CV}
 }
 ```
+
+```bibtex
+@software{Dayma_DALLE_Mini_2021,
+    author  = {Dayma, Boris and Patil, Suraj and Cuenca, Pedro and Saifullah, Khalid and Abraham, Tanishq and Lê Khắc, Phúc and Melas, Luke and Ghosh, Ritobrata},
+    doi     = {10.5281/zenodo.5146400},
+    license = {Apache-2.0},
+    month   = {jul},
+    title   = {{DALL·E Mini}},
+    url     = {https://github.com/borisdayma/dalle-mini},
+    version = {v0.1-alpha},
+    year    = {2021}}
+```
+
+```bibtex
+@inproceedings{anonymous2022normformer,
+    title   = {NormFormer: Improved Transformer Pretraining with Extra Normalization},
+    author  = {Anonymous},
+    booktitle = {Submitted to The Tenth International Conference on Learning Representations },
+    year    = {2022},
+    url     = {https://openreview.net/forum?id=GMYWzWztDx5},
+    note    = {under review}
+}
+```
```

#### html2text {}

```diff
@@ -8,32 +8,32 @@
 recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer model =
 RecurrentMemoryTransformer( num_tokens = 20000, # number of tokens
 num_memory_tokens = 128, # number of memory tokens, this will determine the
 bottleneck for information being passed to the future dim = 512, # model
 dimensions depth = 6, # transformer depth causal = True, # autoregressive or
 not dim_head = 64, # dimension per head heads = 8, # heads seq_len = 1024, #
 sequence length of a segment use_flash_attn = True # whether to use flash
-attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1 = model(x) # (1,
-1024, 20000), (1, 128, 512) logits2, mem2 = model(x, mem1) # (1, 1024, 20000),
-(1, 128, 512) logits3, mem3 = model(x, mem2) # (1, 1024, 20000), (1, 128, 512)
-# and so on ... ``` Train on an absurdly long sequence ```python import torch
-from recurrent_memory_transformer_pytorch import ( RecurrentMemoryTransformer,
-RecurrentMemoryTransformerWrapper ) model = RecurrentMemoryTransformer
-( num_tokens = 256, num_memory_tokens = 128, dim = 512, depth = 6, seq_len =
-1024, use_flash_attn = True, causal = True ) model =
+attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1, _ = model(x) #
+(1, 1024, 20000), (1, 128, 512), None logits2, mem2, _ = model(x, mem1) # (1,
+1024, 20000), (1, 128, 512), None logits3, mem3, _ = model(x, mem2) # (1, 1024,
+20000), (1, 128, 512), None # and so on ... ``` Train on an absurdly long
+sequence ```python import torch from recurrent_memory_transformer_pytorch
+import ( RecurrentMemoryTransformer, RecurrentMemoryTransformerWrapper ) model
+= RecurrentMemoryTransformer( num_tokens = 256, num_memory_tokens = 128, dim =
+512, depth = 6, seq_len = 1024, use_flash_attn = True, causal = True ) model =
 RecurrentMemoryTransformerWrapper(model).cuda() seq = torch.randint(0, 256, (4,
 65536)).cuda() # absurdly long sequence, in reality, they curriculum learned
 this starting with 1 segment to about 7-8 segments loss = model(seq,
 memory_replay_backprop = True) # memory efficient training from memformer paper
-``` ## Todo - [ ] add sliding windows as an option, detached or with memory
-propagated using MRBP - [x] offer a way to turn off rotary embeddings, absolute
-positional embeddings, and add token shift - [x] make memories being causally
-masked an option - [x] add the memory replay backprop technique from memformer
-paper - [x] relative positional encoding ## Alternatives - Block_Recurrent
-Transformer - Memformer ## Citations ```bibtex @inproceedings
+``` ## Todo - [ ] get rotary embeddings working properly with xl memories - [x]
+add xl memories, detached - [x] offer a way to turn off rotary embeddings,
+absolute positional embeddings, and add token shift - [x] make memories being
+causally masked an option - [x] add the memory replay backprop technique from
+memformer paper - [x] relative positional encoding ## Alternatives - Block
+Recurrent_Transformer - Memformer ## Citations ```bibtex @inproceedings
 {bulatov2022recurrent, title = {Recurrent Memory Transformer}, author = {Aydar
 Bulatov and Yuri Kuratov and Mikhail Burtsev}, booktitle = {Advances in Neural
 Information Processing Systems}, editor = {Alice H. Oh and Alekh Agarwal and
 Danielle Belgrave and Kyunghyun Cho}, year = {2022}, url = {https://
 openreview.net/forum?id=Uynr3iPhksa} } ``` ```bibtex @misc{bulatov2023scaling,
 title = {Scaling Transformer to 1M tokens and beyond with RMT}, author = {Aydar
 Bulatov and Yuri Kuratov and Mikhail S. Burtsev}, year = {2023}, eprint =
@@ -55,8 +55,17 @@
 {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year = {2021},
 publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578}, url =
 {https://doi.org/10.5281/zenodo.5196578} } ``` ```bibtex @misc{ding2021cogview,
 title = {CogView: Mastering Text-to-Image Generation via Transformers}, author
 = {Ming Ding and Zhuoyi Yang and Wenyi Hong and Wendi Zheng and Chang Zhou and
 Da Yin and Junyang Lin and Xu Zou and Zhou Shao and Hongxia Yang and Jie Tang},
 year = {2021}, eprint = {2105.13290}, archivePrefix = {arXiv}, primaryClass =
-{cs.CV} } ```
+{cs.CV} } ``` ```bibtex @software{Dayma_DALLE_Mini_2021, author = {Dayma, Boris
+and Patil, Suraj and Cuenca, Pedro and Saifullah, Khalid and Abraham, Tanishq
+and LÃª Kháº¯c, PhÃºc and Melas, Luke and Ghosh, Ritobrata}, doi = {10.5281/
+zenodo.5146400}, license = {Apache-2.0}, month = {jul}, title = {{DALLÂ·E
+Mini}}, url = {https://github.com/borisdayma/dalle-mini}, version = {v0.1-
+alpha}, year = {2021}} ``` ```bibtex @inproceedings{anonymous2022normformer,
+title = {NormFormer: Improved Transformer Pretraining with Extra
+Normalization}, author = {Anonymous}, booktitle = {Submitted to The Tenth
+International Conference on Learning Representations }, year = {2022}, url =
+{https://openreview.net/forum?id=GMYWzWztDx5}, note = {under review} } ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 from functools import partial
 from itertools import zip_longest
 from contextlib import nullcontext
+from typing import Optional, List
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat, pack, unpack
 
@@ -151,33 +152,44 @@
         self.to_kv = Linear(dim, dim_inner * 2)
         self.to_out = Linear(dim_inner, dim)
 
     def forward(
         self,
         x,
         rotary_emb = None,
-        mask = None
+        mask = None,
+        xl_memories = None
     ):
         h = self.heads
 
         x = self.norm(x)
 
         q = self.to_q(x)
         k, v = self.to_kv(x).chunk(2, dim = -1)
 
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
+        next_xl_memories = torch.stack((k, v))
+
+        if exists(xl_memories):
+            kx, vx = xl_memories
+            k = torch.cat((kx, k), dim = -2)
+            v = torch.cat((vx, v), dim = -2)
+
+            mask = F.pad(mask, (xl_memories.shape[-2], 0), value = True)
+
         if exists(rotary_emb):
             q = apply_rotary_pos_emb(rotary_emb, q)
             k = apply_rotary_pos_emb(rotary_emb, k)
 
         out = self.attend(q, k, v, mask = mask)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
-        return self.to_out(out)
+
+        return self.to_out(out), next_xl_memories
 
 # transformer
 
 class RecurrentMemoryTransformer(nn.Module):
     def __init__(
         self,
         dim,
@@ -191,14 +203,16 @@
         heads = 8,
         ff_mult = 4,
         use_flash_attn = False,
         ignore_index = -1,
         abs_pos_emb = True,
         rotary_pos_emb = False,
         token_shift = True,
+        use_xl_memories = False,
+        xl_mem_len = None,
         emb_gradient_frac = 0.1,   # trick from cogview paper that leads to a bit more stability
         memory_not_causal = True,  # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
@@ -224,14 +238,23 @@
 
         self.read_memory_emb = nn.Parameter(torch.zeros(dim))
         nn.init.normal_(self.read_memory_emb, std = 0.02)
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
+        # xl memories
+
+        xl_mem_len = default(xl_mem_len, seq_len)
+        assert xl_mem_len <= seq_len
+        self.xl_mem_len = xl_mem_len
+
+        self.use_xl_memories = use_xl_memories
+        assert not (rotary_pos_emb and use_xl_memories), 'rotary not compatible with xl memories yet'
+
         # layers
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
@@ -262,14 +285,15 @@
     def forward(
         self,
         x,
         read_memories = None,
         *,
         mask = None,
         labels = None,
+        xl_memories: Optional[List[torch.Tensor]] = None
     ):
         b, n, device, mem_length, return_loss = *x.shape, x.device, self.num_memory_tokens, exists(labels)
 
         pos = torch.arange(n, device = device)
 
         x = self.token_emb(x)
 
@@ -321,38 +345,54 @@
             pos = pos + 10000
             pos = F.pad(pos, (read_mem_length, mem_length), value = 0)
 
             rotary_emb = self.rotary_pos_emb(pos)
 
         shift_fn = partial(self.maybe_token_shift, ps = ps)
 
+        # prepare xl memories
+
+        xl_memories_iter = iter(default(xl_memories, []))
+        new_xl_memories = []
+
         # attention and feedforward
 
         for attn, ff in self.layers:
-            x = attn(shift_fn(x), mask = mask, rotary_emb = rotary_emb) + x
+            attn_out, xl_memories = attn(shift_fn(x), mask = mask, xl_memories = next(xl_memories_iter, None), rotary_emb = rotary_emb)
+            new_xl_memories.append(xl_memories)
+
+            x = x + attn_out
+
             x = ff(shift_fn(x)) + x
 
+        # whether to return xl memories
+
+        next_xl_memories = None
+
+        if self.use_xl_memories:
+            next_xl_memories = list(map(lambda t: torch.detach(t[..., -self.xl_mem_len:, :]), new_xl_memories))
+
         # split out memories using unpack
 
         read_memories, x, write_memories = unpack(x, ps, 'b * d')
 
         # to logits
 
         logits = self.to_logits(x)
 
         if not return_loss:
-            return logits, write_memories
+            return logits, write_memories, next_xl_memories
 
         loss = F.cross_entropy(
             rearrange(logits, 'b n c -> b c n'),
             labels,
             ignore_index = self.ignore_index
         )
 
-        return loss, write_memories
+        return loss, write_memories, next_xl_memories
 
 # wrapper to manage many segments
 
 class RecurrentMemoryTransformerWrapper(nn.Module):
     def __init__(
         self,
         transformer: RecurrentMemoryTransformer
@@ -365,45 +405,48 @@
     @eval_decorator
     def generate(
         self,
         prime,
         *,
         length,
         memories = None,
+        xl_memories: Optional[List[torch.Tensor]] = None,
         temperature = 1.,
         filter_thres = 0.9,
     ):
         assert self.transformer.causal, 'only autoregressive transformers can generate'
 
         start_len, seq_len = prime.shape[-1], self.seq_len
 
         assert length >= start_len
 
         *past_segments, curr_segment = prime.split(seq_len, dim = -1)
 
         # catch memories up to the current segment
 
         for past_segment in past_segments:
-            _, memories = self.forward(past_segment, memories)
+            _, memories, xl_memories = self.transformer(past_segment, memories, xl_memories = xl_memories)
 
         # sample for the remaining length
 
         for ind in range(length - start_len):
-            logits, next_memories = self.forward(curr_segment, memories)
+            logits, next_memories, next_xl_memories = self.transformer(curr_segment, memories, xl_memories = xl_memories)
 
             logits = logits[:, -1]
 
             filtered_logits = top_k(logits, thres = filter_thres)
             sampled = gumbel_sample(filtered_logits, temperature = temperature)
             sampled = rearrange(sampled, 'b -> b 1')
 
             curr_segment = torch.cat((curr_segment, sampled), dim = -1)
 
             if divisible_by(curr_segment.shape[-1] - 1, seq_len):
                 memories = next_memories
+                xl_memories = next_xl_memories
+
                 past_segment, curr_segment = curr_segment[..., :seq_len], curr_segment[..., -1:]
                 past_segments.append(past_segment)
 
         # add current segment to all segments
 
         past_segments.append(curr_segment)
 
@@ -416,14 +459,15 @@
 
     def forward(
         self,
         x,
         memories = None,
         *,
         mask = None,
+        xl_memories: Optional[List[torch.Tensor]] = None,
         return_loss = False,
         labels = None,
         memory_replay_backprop = False,  # whether to have the class do the backwards pass memory efficiently
         mrbp_loss_weight = 1.            # if using memory replay backprop with gradient accumulation, scale loss by this factor ex. (1. / <num grad accum steps>)
     ):
         seq_len = self.seq_len
 
@@ -452,30 +496,36 @@
         if exists(mask):
             mask_segments = mask.split(seq_len, dim = -1)
 
         # keep replay buffer
 
         replay_buffer = [memories]
 
+        # replay buffer for xl memories
+
+        xl_segments = [xl_memories]
+
         # decide context of forward depending on whether doing memory-replay-backprop
 
         forward_context = nullcontext if not memory_replay_backprop else torch.no_grad
 
         # forward and get all outputs (can be either loss or logits)
 
         logits = []
         losses = []
 
         for segment, mask_segment, label_segment, loss_weight in zip_longest(segments, mask_segments, label_segments, segment_length_frac):
 
             with forward_context():
-                output, memories = self.transformer(segment, memories, mask = mask_segment, labels = label_segment)
+                output, memories, xl_memories = self.transformer(segment, memories, mask = mask_segment, labels = label_segment)
 
             replay_buffer.append(memories)
 
+            xl_segments.append(xl_memories)
+
             if return_loss:
                 losses.append(output * loss_weight)
             else:
                 logits.append(output)
 
         # whether to do memory replay backpropagation
 
@@ -485,28 +535,29 @@
         if memory_replay_backprop:
             memories_grad = torch.zeros_like(replay_buffer[-1])
 
             reversed_inputs = zip_longest(*map(reversed, [
                 range(num_segments),
                 segments,
                 replay_buffer[:-1],
+                xl_segments[:-1],
                 mask_segments,
                 label_segments,
                 segment_length_frac,
             ]))
 
             total_loss = 0.
 
-            for i, segment, segment_memories, mask_segment, label_segment, loss_weight in reversed_inputs:
+            for i, segment, segment_memories, segment_xl_memories, mask_segment, label_segment, loss_weight in reversed_inputs:
                 is_first = i == 0
 
                 if exists(segment_memories):
                     segment_memories.requires_grad_()
 
-                loss, next_segment_memories = self.transformer(segment, segment_memories, mask = mask_segment, labels = label_segment)
+                loss, next_segment_memories, _ = self.transformer(segment, segment_memories, mask = mask_segment, xl_memories = segment_xl_memories, labels = label_segment)
 
                 weighted_loss = loss * loss_weight * mrbp_loss_weight
 
                 weighted_loss.backward(retain_graph = True)
 
                 next_segment_memories.backward(memories_grad)
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.1.9
+Version: 0.2.0
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.1.9/setup.py` & `recurrent-memory-transformer-pytorch-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.9',
+  version = '0.2.0',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

