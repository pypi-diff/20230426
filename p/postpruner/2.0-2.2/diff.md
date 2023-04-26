# Comparing `tmp/postpruner-2.0.tar.gz` & `tmp/postpruner-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postpruner-2.0.tar", last modified: Thu Apr 20 14:39:06 2023, max compression
+gzip compressed data, was "postpruner-2.2.tar", last modified: Wed Apr 26 21:29:02 2023, max compression
```

## Comparing `postpruner-2.0.tar` & `postpruner-2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.814317 postpruner-2.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-04-20 09:33:20.000000 postpruner-2.0/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-20 14:39:06.814317 postpruner-2.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3678 2023-04-20 09:33:41.000000 postpruner-2.0/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.806317 postpruner-2.0/postpruner/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       28 2023-04-20 07:08:02.000000 postpruner-2.0/postpruner/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-19 23:43:36.000000 postpruner-2.0/postpruner/__main__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.806317 postpruner-2.0/postpruner/dataset/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-2.0/postpruner/dataset/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.806317 postpruner-2.0/postpruner/dataset/evaluate/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-2.0/postpruner/dataset/evaluate/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-19 23:29:53.000000 postpruner-2.0/postpruner/dataset/evaluate/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-19 23:31:54.000000 postpruner-2.0/postpruner/dataset/evaluate/nlp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2385 2023-04-20 14:38:20.000000 postpruner-2.0/postpruner/dataset/evaluate/squad.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/dataset/glue.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/dataset/squad.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.810317 postpruner-2.0/postpruner/efficiency/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-2.0/postpruner/efficiency/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/efficiency/latency.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/efficiency/mac.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.810317 postpruner-2.0/postpruner/figures/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)   105406 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/figures/overview.png
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-19 23:29:53.000000 postpruner-2.0/postpruner/generate_lut.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6900 2023-04-20 11:12:40.000000 postpruner-2.0/postpruner/postpruner.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.810317 postpruner-2.0/postpruner/prune/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-2.0/postpruner/prune/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-19 23:29:53.000000 postpruner-2.0/postpruner/prune/fisher.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/prune/rearrange.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-19 23:29:53.000000 postpruner-2.0/postpruner/prune/rescale.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-19 23:29:53.000000 postpruner-2.0/postpruner/prune/search.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.814317 postpruner-2.0/postpruner/utils/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-19 23:25:18.000000 postpruner-2.0/postpruner/utils/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3307 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/utils/arch.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/utils/linalg.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/utils/meter.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/utils/schedule.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-19 22:11:32.000000 postpruner-2.0/postpruner/utils/timer.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-20 14:39:06.806317 postpruner-2.0/postpruner.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      999 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-20 14:39:06.000000 postpruner-2.0/postpruner.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-20 14:39:06.814317 postpruner-2.0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      438 2023-04-20 14:38:41.000000 postpruner-2.0/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.526570 postpruner-2.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-04-26 19:16:48.000000 postpruner-2.2/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-26 21:29:02.526570 postpruner-2.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3678 2023-04-26 19:16:48.000000 postpruner-2.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.518570 postpruner-2.2/postpruner/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       28 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1684 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/__main__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.518570 postpruner-2.2/postpruner/dataset/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.522570 postpruner-2.2/postpruner/dataset/evaluate/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/evaluate/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1023 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/evaluate/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1232 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/evaluate/nlp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2335 2023-04-26 19:19:18.000000 postpruner-2.2/postpruner/dataset/evaluate/squad.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3804 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/glue.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    22749 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/dataset/squad.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.522570 postpruner-2.2/postpruner/efficiency/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/efficiency/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1565 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/efficiency/latency.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1633 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/efficiency/mac.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.522570 postpruner-2.2/postpruner/figures/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)   105406 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/figures/overview.png
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5007 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/generate_lut.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6900 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/postpruner.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.522570 postpruner-2.2/postpruner/prune/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/prune/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1095 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/prune/fisher.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1303 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/prune/rearrange.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7610 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/prune/rescale.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7421 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/prune/search.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.526570 postpruner-2.2/postpruner/utils/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3354 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/arch.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      689 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/linalg.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/meter.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      180 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/schedule.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      807 2023-04-26 19:16:48.000000 postpruner-2.2/postpruner/utils/timer.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-26 21:29:02.518570 postpruner-2.2/postpruner.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       52 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      999 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       56 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       58 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-04-26 21:29:02.000000 postpruner-2.2/postpruner.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-26 21:29:02.526570 postpruner-2.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      438 2023-04-26 21:28:32.000000 postpruner-2.2/setup.py
```

### Comparing `postpruner-2.0/README.md` & `postpruner-2.2/README.md`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/__main__.py` & `postpruner-2.2/postpruner/__main__.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/dataset/evaluate/glue.py` & `postpruner-2.2/postpruner/dataset/evaluate/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/dataset/evaluate/nlp.py` & `postpruner-2.2/postpruner/dataset/evaluate/nlp.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/dataset/evaluate/squad.py` & `postpruner-2.2/postpruner/dataset/evaluate/squad.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import torch
 from datasets import load_metric
 
 from postpruner.dataset.squad import create_and_fill_np_array, post_processing_function
 from postpruner.utils.arch import apply_neuron_mask
 from postpruner.utils.meter import AverageMeter
+import evaluate
 
 
 @torch.no_grad()
 def eval_squad_acc(
     model,
     head_mask,
     neuron_mask,
     dataloader,
     eval_dataset,
     eval_examples,
     task_name,
 ):
-    metric = load_metric(task_name)
+    metric = evaluate.load(task_name)
 
     model.eval()
-    if neuron_mask is not None:
-        handles = apply_neuron_mask(model, neuron_mask)
+    print("neuron_mask:", neuron_mask)
+    
+    handles = apply_neuron_mask(model, neuron_mask)
 
     all_start_logits = []
     all_end_logits = []
     for batch in dataloader:
         for k, v in batch.items():
             batch[k] = v.to("cuda", non_blocking=True)
 
@@ -33,17 +35,16 @@
         else:
             outputs = model(**batch)
         start_logits = outputs.start_logits
         end_logits = outputs.end_logits
 
         all_start_logits.append(start_logits.cpu().numpy())
         all_end_logits.append(end_logits.cpu().numpy())
-    if neuron_mask is not None:
-        for handle in handles:
-            handle.remove()
+    for handle in handles:
+        handle.remove()
 
     max_len = max([x.shape[1] for x in all_start_logits])
     start_logits_concat = create_and_fill_np_array(all_start_logits, eval_dataset, max_len)
     end_logits_concat = create_and_fill_np_array(all_end_logits, eval_dataset, max_len)
     del all_start_logits
     del all_end_logits
 
@@ -60,16 +61,15 @@
     head_mask,
     neuron_mask,
     dataloader,
 ):
     loss = AverageMeter("squad_loss")
 
     model.eval()
-    if neuron_mask is not None:
-        handles = apply_neuron_mask(model, neuron_mask)
+    handles = apply_neuron_mask(model, neuron_mask)
     for batch in dataloader:
         for k, v in batch.items():
             batch[k] = v.to("cuda", non_blocking=True)
 
         if head_mask is not None:
             outputs = model(head_mask=head_mask, **batch)
         else:
```

### Comparing `postpruner-2.0/postpruner/dataset/glue.py` & `postpruner-2.2/postpruner/dataset/glue.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/dataset/squad.py` & `postpruner-2.2/postpruner/dataset/squad.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/efficiency/latency.py` & `postpruner-2.2/postpruner/efficiency/latency.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/efficiency/mac.py` & `postpruner-2.2/postpruner/efficiency/mac.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/figures/overview.png` & `postpruner-2.2/postpruner/figures/overview.png`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/generate_lut.py` & `postpruner-2.2/postpruner/generate_lut.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/postpruner.py` & `postpruner-2.2/postpruner/postpruner.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/prune/fisher.py` & `postpruner-2.2/postpruner/prune/fisher.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/prune/rearrange.py` & `postpruner-2.2/postpruner/prune/rearrange.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/prune/rescale.py` & `postpruner-2.2/postpruner/prune/rescale.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/prune/search.py` & `postpruner-2.2/postpruner/prune/search.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/utils/arch.py` & `postpruner-2.2/postpruner/utils/arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 def register_mask(module, mask):
     hook = lambda _, inputs: (inputs[0] * mask, inputs[1])
     handle = module.register_forward_pre_hook(hook)
     return handle
 
 
 def apply_neuron_mask(model, neuron_mask):
+    if neuron_mask is None:
+        return []
+
     num_hidden_layers = neuron_mask.shape[0]
     handles = []
     for layer_idx in range(num_hidden_layers):
         ffn2 = get_ffn2(model, layer_idx)
         handle = register_mask(ffn2, neuron_mask[layer_idx])
         handles.append(handle)
     return handles
```

### Comparing `postpruner-2.0/postpruner/utils/linalg.py` & `postpruner-2.2/postpruner/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner/utils/timer.py` & `postpruner-2.2/postpruner/utils/timer.py`

 * *Files identical despite different names*

### Comparing `postpruner-2.0/postpruner.egg-info/SOURCES.txt` & `postpruner-2.2/postpruner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

