# Comparing `tmp/merlin-dataloader-23.2.1.tar.gz` & `tmp/merlin-dataloader-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-dataloader-23.2.1.tar", last modified: Mon Mar 13 18:28:48 2023, max compression
+gzip compressed data, was "merlin-dataloader-23.4.0.tar", last modified: Wed Apr 26 19:02:30 2023, max compression
```

## Comparing `merlin-dataloader-23.2.1.tar` & `merlin-dataloader-23.4.0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.009460 merlin-dataloader-23.2.1/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/merlin/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/merlin/dataloader/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/loader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.017460 merlin-dataloader-23.2.1/merlin/dataloader/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.017460 merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/embedding_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/tf_embedding_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/torch_embedding_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.009460 merlin-dataloader-23.2.1/merlin/dataloader/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.017460 merlin-dataloader-23.2.1/merlin/dataloader/utils/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/utils/tf/tf_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.017460 merlin-dataloader-23.2.1/merlin/dataloader/utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/dataloader/utils/torch/torch_trainer_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.017460 merlin-dataloader-23.2.1/merlin/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/loader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/merlin/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-13 18:28:47.000000 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-13 18:28:47.000000 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 18:28:47.000000 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-13 18:28:47.000000 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-13 18:28:47.000000 merlin-dataloader-23.2.1/merlin_dataloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/requirements/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-13 18:28:48.021460 merlin-dataloader-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-03-13 18:28:37.000000 merlin-dataloader-23.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/merlin/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/merlin/dataloader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29255 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/loader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/ops/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/tf_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/torch_trainer_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/merlin/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.496224 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 19:02:30.000000 merlin-dataloader-23.4.0/merlin_dataloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/requirements/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-26 19:02:30.500224 merlin-dataloader-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-04-26 19:02:03.000000 merlin-dataloader-23.4.0/versioneer.py
```

### Comparing `merlin-dataloader-23.2.1/LICENSE` & `merlin-dataloader-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/PKG-INFO` & `merlin-dataloader-23.4.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.2.1
+Version: 23.4.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-dataloader-23.2.1/README.md` & `merlin-dataloader-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/__init__.py` & `merlin-dataloader-23.4.0/merlin/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/loader_base.py` & `merlin-dataloader-23.4.0/merlin/dataloader/loader_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import contextlib
 import copy
 import itertools
 import math
 import queue
 import threading
 import warnings
 from typing import List, Optional
 
-import numpy as np
-
-try:
-    import cupy
-except ImportError:
-    cupy = None
-
+from merlin.core.compat import HAS_GPU, cudf, cupy
+from merlin.core.compat import numpy as np
+from merlin.core.compat import pandas as pd
 from merlin.core.dispatch import (
-    HAS_GPU,
     annotate,
     concat,
     generate_local_seed,
     is_list_dtype,
     make_df,
     pull_apart_list,
 )
-from merlin.dag import BaseOperator, ColumnSelector, DictArray, Graph, Node
+from merlin.dag import BaseOperator, ColumnSelector, Graph, Node, ungroup_values_offsets
 from merlin.dag.executors import LocalExecutor
 from merlin.io import shuffle_df
 from merlin.schema import Schema, Tags
+from merlin.table import TensorTable
 
 
 def _num_steps(num_samples, step_size):
     return math.ceil(num_samples / step_size)
 
 
 class LoaderBase:
@@ -52,15 +49,15 @@
 
     _use_row_lengths = False
 
     def __init__(
         self,
         dataset,
         batch_size,
-        shuffle=True,
+        shuffle=False,
         seed_fn=None,
         parts_per_chunk=1,
         global_size=None,
         global_rank=None,
         drop_last=False,
         transforms=None,
         device=None,
@@ -69,14 +66,15 @@
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.seed_fn = seed_fn
         self.parts_per_chunk = parts_per_chunk
         self.global_size = global_size or 1
         self.global_rank = global_rank or 0
         self.drop_last = drop_last
+        self._map_fns = []
 
         device = device or 0
         self.device = "cpu" if not HAS_GPU or dataset.cpu else device
 
         if self.device == "cpu":
             self._array_lib = np
         else:
@@ -111,16 +109,18 @@
                         raise TypeError(
                             f"Detected invalid transform, {type(transform)},"
                             "we only support operators based on the merlin core"
                             "`BaseOperator`"
                         )
                     carry_node = carry_node >> transform
                 transform_graph = Graph(carry_node)
-            elif type(transforms, Graph):
+            elif isinstance(transforms, Graph):
                 transform_graph = transforms
+            elif isinstance(transforms, Node):
+                transform_graph = Graph(transforms)
             self._transform_graph = transform_graph
             self.executor = LocalExecutor()
 
         schema = dataset.schema
         self.input_schema = schema
 
     @property
@@ -174,14 +174,24 @@
 
     def _set_epochs(self, epochs):
         self.stop()
         self.__buff = None
         self.__buff_len = None
         self._epochs = epochs
 
+    def __getitem__(self, index):
+        """Gets batch at position `index`.
+
+        Note: This returns the next batch in the iterator.
+              Not the batch at position `index`.
+              This is because the dataloader is implemented as an iterator and
+              don't currently support fetching a batch by index.
+        """
+        return self.__next__()
+
     def __len__(self):
         batches = _num_steps(self._buff_len, self.batch_size)
         if self.drop_last and self._buff_len % self.batch_size > 0:
             batches = batches - 1
         return batches
 
     @property
@@ -352,118 +362,149 @@
 
         Returns
         -------
         Dict[Tensors]
             A dictionary of the column tensor representations.
 
         """
-        split_idx = self._get_segment_lengths(len(gdf))
+        tensors_by_name = self._convert_df_to_tensors(gdf)
+        rows_per_batch = self._get_rows_per_batch(len(gdf))
 
-        # convert dataframe to framework-specific tensors
-        tensors_by_name = self._process_dataframe(gdf)
-
-        # split them into batches and map to the framework-specific output format
         tensor_batches = {}
 
         for tensor_key, tensor_value in tensors_by_name.items():
             if isinstance(tensor_value, tuple):
-                values, offsets = tensor_value
-                row_lengths = offsets[1:] - offsets[:-1]
-                batch_row_lengths = self._split_fn(row_lengths, split_idx)
-                values_split_idx = [self._sum(row_lengths) for row_lengths in batch_row_lengths]
-                batch_values = self._split_fn(values, values_split_idx)
+                # List feature
+                full_tensor_values, full_tensor_offsets = tensor_value
+
+                splits = list(itertools.accumulate(rows_per_batch))
+
+                offsets_grouped_by_batch = []
+                if splits:
+                    for idx, split in enumerate([0] + splits[:-1]):
+                        start = split
+                        end = splits[idx] + 1
+                        offsets_grouped_by_batch.append(full_tensor_offsets[start:end])
+
+                subtracted_offsets_grouped_by_batch = self._subtract_offsets(
+                    offsets_grouped_by_batch
+                )
+                num_values_per_batch = [
+                    int(batch_offsets[-1]) for batch_offsets in subtracted_offsets_grouped_by_batch
+                ]
+
+                batch_values = self._split_values(full_tensor_values, num_values_per_batch)
                 tensor_batches[tensor_key] = {
                     "values": batch_values,
-                    "row_lengths": batch_row_lengths,
+                    "offsets": subtracted_offsets_grouped_by_batch,
                 }
             else:
-                tensor_batches[tensor_key] = self._split_fn(tensor_value, split_idx)
+                # Scalar feature
+                num_values_per_batch = rows_per_batch
+                tensor_batches[tensor_key] = self._split_values(tensor_value, num_values_per_batch)
 
-        for batch_idx in range(len(split_idx)):
+        for batch_idx in range(len(rows_per_batch)):
             batch = {}
             for tensor_key in tensors_by_name:
                 tensor_value = tensor_batches[tensor_key]
                 if isinstance(tensor_value, dict):
-                    values = tensor_value["values"][batch_idx]
-                    row_partition = tensor_value["row_lengths"][batch_idx]
-                    if not use_row_lengths:
-                        row_partition = self._row_lengths_to_offsets(row_partition)
-                    batch[tensor_key] = values, row_partition
+                    full_tensor_values = tensor_value["values"][batch_idx]
+                    offsets = tensor_value["offsets"][batch_idx]
+                    batch[tensor_key] = full_tensor_values, offsets
                 else:
                     batch[tensor_key] = tensor_value[batch_idx]
 
             yield self._process_batch(batch)
 
-    def _get_segment_lengths(self, num_samples):
+    def _get_rows_per_batch(self, num_samples):
         """
         Helper function to build indices to pass
         to <torch|tf>.split functions for breaking
         up into batches
         """
         num_full_batches = _num_steps(num_samples, self.batch_size) - 1
         idx = [self.batch_size for _ in range(num_full_batches)]
         idx.append(num_samples - num_full_batches * self.batch_size)
         return idx
 
-    def _to_sparse_tensor(self, values_offset, column_name):
-        """
-        Create a sparse representation of the input tensor.
-        values_offset is either a tensor or a tuple of tensor, offset.
-        """
-        seq_limit = self.sparse_max[column_name]
-        values, offsets, diff_offsets, num_rows = self._pull_values_offsets(values_offset)
-        max_seq_len = self._get_max_seq_len(diff_offsets)
-        if max_seq_len > seq_limit:
-            raise ValueError(
-                "The default sequence length has been configured "
-                + f"to {seq_limit} but the "
-                + f"largest sequence in this batch have {max_seq_len} length"
-            )
-        sparse_as_dense = column_name in self.sparse_as_dense
-        return self._build_sparse_tensor(
-            values, offsets, diff_offsets, num_rows, seq_limit, sparse_as_dense
-        )
-
-    def _to_tensor(self, gdf):
+    def _to_tensor(self, df_or_series):
         """
         One of the mandatory functions a child class needs
         to implement. Maps from a cudf DataFrame to a
         tensor in the appropriate library, with an optional
         dtype kwarg to do explicit casting if need be
         """
-        raise NotImplementedError
+        if df_or_series.empty:
+            return
+
+        # if you have one series in a dataframe pull that series out
+        # otherwise you will add a dimension to the column [[1,2,3]]
+        try:
+            if len(df_or_series.columns) == 1:
+                df_or_series = df_or_series.iloc[:, 0]
+        except AttributeError:
+            pass
+
+        if self.device == "cpu":
+            tensor = df_or_series.to_numpy()
+        else:
+            tensor = df_or_series.to_cupy()
+
+        return tensor
 
+    @contextlib.contextmanager
     def _get_device_ctx(self, dev):
         """
         One of the mandatory functions a child class needs
         to implement. Maps from a GPU index to a framework
         context object for placing tensors on specific GPUs
         """
-        raise NotImplementedError
+        yield dev
 
     def _cast_to_numpy_dtype(self, dtype):
         """
         Get the numpy dtype from the framework dtype.
         """
-        raise NotImplementedError
+        raise dtype
 
-    def _split_fn(self, tensor, idx, axis=0):
-        raise NotImplementedError
+    def _split_values(self, tensor, values_per_batch, axis=0):
+        # splits are like offsets but without the first and last entry
+        splits = list(itertools.accumulate(values_per_batch))[:-1]
+        return self.array_lib().split(tensor, splits, axis=axis)
+
+    def _subtract_offsets(self, offsets_grouped_by_batch):
+        subtracted_offsets_grouped_by_batch = []
+        for idx, batch_offsets in enumerate(offsets_grouped_by_batch):
+            if idx != 0:
+                previous_batch_offsets = offsets_grouped_by_batch[idx - 1]
+                batch_offsets = batch_offsets - previous_batch_offsets[-1]
+            subtracted_offsets_grouped_by_batch.append(batch_offsets)
+        return subtracted_offsets_grouped_by_batch
 
     def _separate_list_columns(self, gdf):
         lists, scalars = [], []
         for col in gdf.columns:
             if is_list_dtype(gdf[col]):
                 lists.append(col)
             else:
                 scalars.append(col)
         return scalars, lists
 
-    @annotate("_process_dataframe", color="darkgreen", domain="merlin_dataloader")
-    def _process_dataframe(self, gdf):
+    def array_lib(self):
+        return self._array_lib
+
+    def _split_fn(self, tensor, idx, axis=0):
+        splits = list(itertools.accumulate(idx))[:-1]
+        return self.array_lib().split(tensor, splits, axis=axis)
+
+    def _tensor_split(self, tensor, idx, axis=0):
+        return self.array_lib().split(tensor, idx, axis=axis)
+
+    @annotate("_convert_df_to_tensors", color="darkgreen", domain="merlin_dataloader")
+    def _convert_df_to_tensors(self, gdf):
         """Convert a dataframe into framework tensors.
         Returns dictionary of tensors by feature name.
         Where scalar features are grouped under the same key (tuple of column names)
         when they share the same dtype.
         """
         tensors_by_name = {}
         for column_names in self.dtype_reverse_map.values():
@@ -471,51 +512,56 @@
             gdf.drop(columns=column_names, inplace=True)
 
             scalars, lists = self._separate_list_columns(gdf_i)
 
             if scalars:
                 # split out cols and change all scalars
                 # should always return dict column_name: values, offsets (optional)
-                scalars = self._to_tensor(gdf_i[scalars])
-                tensor_key = tuple(column_names) if len(column_names) > 1 else column_names[0]
-                tensors_by_name[tensor_key] = scalars
+                for column_name in column_names:
+                    tensors_by_name[column_name] = self._to_tensor(gdf_i[[column_name]])
 
             if lists:
                 # split out lists
                 for column_name in lists:
                     column = gdf_i.pop(column_name)
+
+                    if cudf and isinstance(column, cudf.Series):
+                        is_fixed_length = (
+                            not self.input_schema[column_name].shape.is_ragged
+                            and (column.list.len() == column.list.len()[0]).all()
+                        )
+                        if is_fixed_length:
+                            values = column.list.leaves.values.reshape(
+                                -1, *cupy.array(column[0]).shape
+                            )
+                            tensors_by_name[column_name] = values
+                            continue
+                    elif isinstance(column, pd.Series):
+                        if not self.input_schema[column_name].shape.is_ragged:
+                            values = np.array(list(_array_leaves(column.values))).reshape(
+                                -1, *np.array(column[0]).shape
+                            )
+                            tensors_by_name[column_name] = values
+                            continue
+
                     leaves, col_offsets = pull_apart_list(column, device=self.device)
 
                     if isinstance(leaves[0], list):
                         leaves, nest_offsets = pull_apart_list(leaves, device=self.device)
                         col_offsets = nest_offsets.iloc[col_offsets[:]]
 
                     tensors_by_name[column_name] = self._to_tensor(leaves), self._to_tensor(
                         col_offsets
                     )
 
         return tensors_by_name
 
     @annotate("_process_batch", color="darkgreen", domain="merlin_dataloader")
     def _process_batch(self, tensors):
-        X = {}
-        for k, v in tensors.items():
-            if isinstance(k, tuple):
-                values = self._tensor_split(v, len(k), axis=1)
-                for column_name, column_value in zip(k, values):
-                    X[column_name] = column_value
-            else:
-                X[k] = v
-
-        for column_name in self.sparse_names:
-            if column_name in self.sparse_max:
-                # raise ValueError(
-                #     f"Did not convert {column_name} to sparse due to missing sparse_max entry"
-                # )
-                X[column_name] = self._to_sparse_tensor(X[column_name], column_name)
+        X = ungroup_values_offsets(tensors)
 
         # Return a tensor if we have only one label column, but return a
         # dictionary of tensors if there are multiple label columns, since
         # dictionary output is required in Merlin Models and Transformers4Rec.
         # If a user is using a vanilla Keras model with multiple labels,
         # they would need to provide matching column names in the output layer
         # of the Keras model.
@@ -525,31 +571,18 @@
             labels = X.pop(self.label_names[0])
         else:
             labels = {}
             for label in self.label_names:
                 labels[label] = X.pop(label)
 
         if self.transforms:
-            X = self.executor.transform(DictArray(X), [self.transforms])
+            X = self.executor.transform(TensorTable(X), [self.transforms])
 
         return X, labels
 
-    def _pack(self, gdf):
-        if isinstance(gdf, np.ndarray):
-            return gdf
-        # if self.device has value ('cpu') gdf should not be transferred to dlpack
-        elif hasattr(gdf, "to_dlpack") and callable(getattr(gdf, "to_dlpack")) and not self.device:
-            return gdf.to_dlpack()
-        elif hasattr(gdf, "to_numpy") and callable(getattr(gdf, "to_numpy")):
-            gdf = gdf.to_numpy()
-            if isinstance(gdf[0], list):
-                gdf = np.stack(gdf)
-            return gdf
-        return gdf.toDlpack()
-
     @property
     def schema(self) -> Schema:
         """Get input schema of data to be loaded
 
         Returns
         -------
         ~merlin.schema.Schema
@@ -619,40 +652,21 @@
             value.select_by_tag(Tags.CATEGORICAL).excluding_by_tag(Tags.TARGET).column_names
         )
         self.cont_names = (
             value.select_by_tag(Tags.CONTINUOUS).excluding_by_tag(Tags.TARGET).column_names
         )
         self.label_names = value.select_by_tag(Tags.TARGET).column_names
 
-        self.sparse_names = []
-        self.sparse_max = {}
-        self.sparse_as_dense = set()
         self.dtype_reverse_map = {}
 
         for col_name, col_spec in self._input_schema.column_schemas.items():
             if col_spec.dtype not in self.dtype_reverse_map:
                 self.dtype_reverse_map[col_spec.dtype] = [col_name]
             else:
                 self.dtype_reverse_map[col_spec.dtype].append(col_name)
-            if col_spec.is_list:
-                self.sparse_names.append(col_name)
-
-                value_count = col_spec.value_count
-                if value_count and value_count.max:
-                    self.sparse_max[col_name] = value_count.max
-
-                if not col_spec.is_ragged:
-                    self.sparse_as_dense.add(col_name)
-
-                    if not value_count:
-                        # TODO: error message linking to docs
-                        raise ValueError(
-                            f"Dense column {col_name} doesn't have the max value_count defined"
-                            " in the schema"
-                        )
 
         if self._transform_graph is not None:
             self._transforms = self._transform_graph.construct_schema(
                 self._input_schema
             ).output_node
             self._output_schema = self._transforms.output_schema
         else:
@@ -749,15 +763,15 @@
             if spill is not None and not spill.empty:
                 chunks.insert(0, spill)
 
             chunks = concat(chunks)
             chunks.reset_index(drop=True, inplace=True)
             chunks, spill = self.get_batch_div_chunk(chunks, self.dataloader.batch_size)
             if self.shuffle:
-                chunks = shuffle_df(chunks)
+                chunks = shuffle_df(chunks, keep_index=True)
 
             if len(chunks) > 0:
                 chunks = self.dataloader.make_tensors(chunks, self.dataloader._use_row_lengths)
                 # put returns True if buffer is stopped before
                 # packet can be put in queue. Keeps us from
                 # freezing on a put on a full queue
                 if self.put(chunks):
@@ -797,7 +811,15 @@
         spill = make_df(chunks.iloc[spill_idx:])
         chunks = make_df(chunks.iloc[:spill_idx])
         if not chunks.empty:
             chunks.reset_index(drop=True, inplace=True)
         if not spill.empty:
             spill.reset_index(drop=True, inplace=True)
         return chunks, spill
+
+
+def _array_leaves(x):
+    if isinstance(x, (list, np.ndarray)):
+        for element in x:
+            yield from _array_leaves(element)
+    else:
+        yield x
```

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/ops/__init__.py` & `merlin-dataloader-23.4.0/merlin/dataloader/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/ops/embeddings/torch_embedding_op.py` & `merlin-dataloader-23.4.0/merlin/dataloader/ops/embeddings.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import Optional, Union
 
-import torch
-from torch.nn import Embedding
+import numpy as np
 
-from merlin.dataloader.ops.embeddings.embedding_op import (
-    EmbeddingOperator,
-    MmapNumpyTorchEmbedding,
-    NumpyEmbeddingOperator,
-)
+from merlin.core.protocols import Transformable
+from merlin.dag import BaseOperator
+from merlin.dag.selector import ColumnSelector
+from merlin.schema import ColumnSchema, Schema, Tags
+from merlin.table import Device, TensorColumn
 
 
-class TorchEmbeddingOperator(EmbeddingOperator):
+class EmbeddingOperator(BaseOperator):
     """Create an operator that will apply a torch embedding table to supplied indices.
     This operator allows the user to supply an id lookup table if the indices supplied
     via the id_lookup_table.
 
     Parameters
     ----------
     embeddings : np.ndarray
@@ -37,70 +37,74 @@
         the name of the column that will be used as indices, by default "id"
     embedding_name : str, optional
         name of new column of embeddings, added to output, by default "embeddings"
     id_lookup_table : np.array, optional
         numpy array of values that represent embedding indices, by default None
     """
 
-    def _load_embeddings(self, embeddings):
-        return (
-            embeddings
-            if isinstance(embeddings, Embedding)
-            else Embedding.from_pretrained(torch.FloatTensor(embeddings))
+    def __init__(
+        self,
+        embeddings: Union[np.ndarray, str],
+        lookup_key: str = "id",
+        embedding_name: str = "embeddings",
+        id_lookup_table: Optional[Union[np.ndarray, str]] = None,
+        mmap=False,
+    ):
+        if mmap:
+            embeddings = np.load(embeddings, mmap_mode="r")
+            id_lookup_table = np.load(id_lookup_table) if id_lookup_table else None
+        self.embeddings = embeddings
+        self.lookup_key = lookup_key
+        self.embedding_name = embedding_name
+        self.id_lookup_table = id_lookup_table
+
+    def transform(
+        self, col_selector: ColumnSelector, transformable: Transformable
+    ) -> Transformable:
+        keys = transformable[self.lookup_key]
+        indices = keys.cpu().values
+        if self.id_lookup_table is not None:
+            indices = np.in1d(self.id_lookup_table, indices)
+        embeddings = self.embeddings[indices]
+        embeddings_col = TensorColumn(embeddings, offsets=keys.cpu().offsets)
+        transformable[self.embedding_name] = (
+            embeddings_col.gpu() if keys.device == Device.GPU else embeddings_col
         )
+        return transformable
 
-    def _create_tensor(self, values):
-        return torch.Tensor(values).to(torch.int32)
-
-    def _embeddings_lookup(self, indices):
-        return self.embeddings(indices)
-
-    def _format_embeddings(self, embeddings, keys):
-        return torch.squeeze(embeddings.to(keys.device))
-
-    def _get_dtype(self, embeddings):
-        return embeddings.weight.numpy().dtype
-
-
-class Torch_NumpyEmbeddingOperator(NumpyEmbeddingOperator):
-    """Create an embedding table from supplied embeddings to add embedding entry
-    to records based on supplied indices. Support for indices lookup table is available.
-    Embedding table is stored in host memory.
-
-    Parameters
-    ----------
-    embeddings : np.ndarray
-        numpy ndarray representing embedding values
-    lookup_key : str, optional
-        the name of the column that will be used as indices, by default "id"
-    embedding_name : str, optional
-        name of new column of embeddings, added to output, by default "embeddings"
-    id_lookup_table : np.array, optional
-        numpy array of values that represent embedding indices, by default None
-    """
-
-    def _format_embeddings(self, embeddings, keys):
-        return torch.from_numpy(embeddings).to(keys.device).squeeze(1)
-
-
-class Torch_MmapNumpyTorchEmbedding(MmapNumpyTorchEmbedding):
-    """Operator loads numpy embedding table from file using memory map to be used to create
-    torch embedding representations. This allows for larger than host memory embedding
-    tables to be used for embedding lookups. The only limit to the size is what fits in
-    storage, preferred storage device is SSD for faster lookups.
-
-    Parameters
-    ----------
-    embedding_npz : numpy ndarray file
-        file holding numpy ndarray representing embedding table
-    ids_lookup_npz : numpy array file, optional
-        file holding numpy array of values that represent embedding indices, by default None
-    lookup_key : str, optional
-        the name of the column that will be used as indices, by default "id"
-    embedding_name : str, optional
-        name of new column of embeddings, added to output, by default "embeddings"
-    transform_function : _type_, optional
-        function that will transform embedding from numpy to torch, by default None
-    """
+    def compute_output_schema(
+        self,
+        input_schema: Schema,
+        col_selector: ColumnSelector,
+        prev_output_schema: Schema = None,
+    ) -> Schema:
+        """Creates the output schema for this operator.
+
+        Parameters
+        ----------
+        input_schema : Schema
+            schema coming from ancestor nodes
+        col_selector : ColumnSelector
+            subselection of columns to apply to this operator
+        prev_output_schema : Schema, optional
+            the output schema of the previously executed operators, by default None
+
+        Returns
+        -------
+        Schema
+            Schema representing the correct output for this operator.
+        """
+        col_schemas = []
+        for _, col_schema in input_schema.column_schemas.items():
+            col_schemas.append(col_schema)
+        id_schema = input_schema.column_schemas[self.lookup_key]
+        embedding_dim = self.embeddings.shape[1]
+        col_schemas.append(
+            ColumnSchema(
+                name=self.embedding_name,
+                tags=[Tags.EMBEDDING],
+                dtype=self.embeddings.dtype,
+                dims=id_schema.shape.as_tuple + (embedding_dim,),
+            )
+        )
 
-    def _format_embeddings(self, embeddings, keys):
-        return torch.from_numpy(embeddings).to(keys.device).squeeze(1)
+        return Schema(col_schemas)
```

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/tf_utils.py` & `merlin-dataloader-23.4.0/merlin/dataloader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/utils/tf/tf_trainer.py` & `merlin-dataloader-23.4.0/merlin/dataloader/utils/tf/tf_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # External dependencies
 import argparse
 import glob
 import logging
 import os
 
-import cupy
-
+from merlin.core.compat import cupy, numpy
 from merlin.io import Dataset
 
 # we can control how much memory to give tensorflow with this environment variable
 # IMPORTANT: make sure you do this before you initialize TF's runtime, otherwise
 # TF will have claimed all free GPU memory
 os.environ["TF_MEMORY_ALLOCATION"] = "0.3"  # fraction of free memory
 
@@ -17,14 +16,15 @@
 import nvtabular as nvt  # noqa: E402 isort:skip
 from nvtabular.framework_utils.tensorflow import layers  # noqa: E402 isort:skip
 from merlin.dataloader.tensorflow import Loader  # noqa: E402 isort:skip
 
 import tensorflow as tf  # noqa: E402 isort:skip
 import horovod.tensorflow as hvd  # noqa: E402 isort:skip
 
+xp = cupy or numpy
 
 LOG = logging.getLogger("multi")
 
 
 parser = argparse.ArgumentParser(description="Process some integers.")
 parser.add_argument("--dir_in", default=None, help="Input directory")
 parser.add_argument("--batch_size", default=None, help="batch size")
@@ -42,29 +42,32 @@
 NUMERIC_COLUMNS = args.conts or []
 TRAIN_PATHS = sorted(
     glob.glob(os.path.join(BASE_DIR, "train/*.parquet"))
 )  # Output from ETL-with-NVTabular
 hvd.init()
 
 # Seed with system randomness (or a static seed)
-cupy.random.seed(None)
+xp.random.seed(None)
 
 
 def seed_fn():
     """
     Generate consistent dataloader shuffle seeds across workers
 
     Reseeds each worker's dataloader each epoch to get fresh a shuffle
     that's consistent across workers.
     """
     min_int, max_int = tf.int32.limits
     max_rand = max_int // hvd.size()
 
     # Generate a seed fragment on each worker
-    seed_fragment = cupy.random.randint(0, max_rand).get()
+    if cupy:
+        seed_fragment = xp.random.randint(0, max_rand).get()
+    else:
+        seed_fragment = xp.random.randint(0, max_rand)
 
     # Aggregate seed fragments from all Horovod workers
     seed_tensor = tf.constant(seed_fragment)
     reduced_seed = hvd.allreduce(seed_tensor, name="shuffle_seed", op=hvd.mpi_ops.Sum)
 
     return reduced_seed % max_rand
```

### Comparing `merlin-dataloader-23.2.1/merlin/dataloader/utils/torch/torch_trainer_dist.py` & `merlin-dataloader-23.4.0/merlin/dataloader/utils/torch/torch_trainer_dist.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/loader/__init__.py` & `merlin-dataloader-23.4.0/merlin/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/loader/jax.py` & `merlin-dataloader-23.4.0/merlin/loader/jax.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/loader/tensorflow.py` & `merlin-dataloader-23.4.0/merlin/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin/loader/torch.py` & `merlin-dataloader-23.4.0/merlin/loader/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/merlin_dataloader.egg-info/PKG-INFO` & `merlin-dataloader-23.4.0/merlin_dataloader.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.2.1
+Version: 23.4.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-dataloader-23.2.1/merlin_dataloader.egg-info/requires.txt` & `merlin-dataloader-23.4.0/merlin_dataloader.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-merlin-core>=0.8.0
+merlin-core>=23.4.0
 
 [all]
-merlin-core>=0.8.0
+merlin-core>=23.4.0
 tensorflow>=2.3.0
 torch>=1.0
 torch>=1.0
 jax[cpu]
 scipy
 scikit-learn>=0.20
 npy_append_array
@@ -26,15 +26,15 @@
 sphinx_rtd_theme
 natsort<8.2
 myst-nb<0.14
 linkify-it-py<1.1
 markdown==3.3.7
 
 [base]
-merlin-core>=0.8.0
+merlin-core>=23.4.0
 
 [dev]
 scipy
 scikit-learn>=0.20
 npy_append_array
 ipython_genutils
 nbsphinx>=0.6
```

### Comparing `merlin-dataloader-23.2.1/pyproject.toml` & `merlin-dataloader-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/requirements/dev.txt` & `merlin-dataloader-23.4.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/setup.cfg` & `merlin-dataloader-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/setup.py` & `merlin-dataloader-23.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.2.1/versioneer.py` & `merlin-dataloader-23.4.0/versioneer.py`

 * *Files identical despite different names*

