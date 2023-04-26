# Comparing `tmp/remin-0.0.3.tar.gz` & `tmp/remin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.0.3.tar", last modified: Mon Apr 24 20:59:40 2023, max compression
+gzip compressed data, was "remin-0.0.4.tar", last modified: Wed Apr 26 12:00:54 2023, max compression
```

## Comparing `remin-0.0.3.tar` & `remin-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.3/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.3/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.0.3/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-24 20:59:40.413460 remin-0.0.3/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.3/README.md
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/examples/
--rw-rw-r--   0 salih     (1000) salih     (1000)    78602 2023-04-17 09:08:31.000000 remin-0.0.3/examples/example_heat_problem.ipynb
--rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-24 20:59:14.000000 remin-0.0.3/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.3/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-24 20:59:40.413460 remin-0.0.3/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-04-24 20:59:06.000000 remin-0.0.3/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1180 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.3/src/remin/func.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     3548 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/residual.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     4336 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/solver.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      371 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.4/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.4/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.0.4/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-26 12:00:54.042894 remin-0.0.4/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.4/README.md
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.038894 remin-0.0.4/examples/
+-rw-rw-r--   0 salih     (1000) salih     (1000)    78602 2023-04-17 09:08:31.000000 remin-0.0.4/examples/example_heat_problem.ipynb
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.038894 remin-0.0.4/examples/heat/
+-rw-rw-r--   0 salih     (1000) salih     (1000)      526 2023-04-25 20:20:42.000000 remin-0.0.4/examples/heat/model.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/examples/heat/outputs/
+-rw-rw-r--   0 salih     (1000) salih     (1000)   217061 2023-04-25 20:35:40.000000 remin-0.0.4/examples/heat/outputs/heat.png
+-rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-24 20:50:29.000000 remin-0.0.4/examples/heat/outputs/heat_best_model.pt
+-rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-21 02:09:04.000000 remin-0.0.4/examples/heat/outputs/heat_best_model_full_batch.pt
+-rw-rw-r--   0 salih     (1000) salih     (1000)    52733 2023-04-21 01:56:00.000000 remin-0.0.4/examples/heat/outputs/heat_best_model_fully_loaded.pt
+-rw-rw-r--   0 salih     (1000) salih     (1000)    52775 2023-04-21 02:09:04.000000 remin-0.0.4/examples/heat/outputs/heat_final_model_full_batch.pt
+-rw-rw-r--   0 salih     (1000) salih     (1000)    52775 2023-04-21 01:56:00.000000 remin-0.0.4/examples/heat/outputs/heat_final_model_fully_loaded.pt
+-rw-rw-r--   0 salih     (1000) salih     (1000)      760 2023-04-25 20:35:46.000000 remin-0.0.4/examples/heat/postprocess.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1495 2023-04-25 20:42:55.000000 remin-0.0.4/examples/heat/training.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-26 11:59:10.000000 remin-0.0.4/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.4/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-26 12:00:54.042894 remin-0.0.4/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.034894 remin-0.0.4/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-04-26 11:59:09.000000 remin-0.0.4/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1180 2023-04-24 20:56:05.000000 remin-0.0.4/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.4/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     4031 2023-04-26 11:55:58.000000 remin-0.0.4/src/remin/residual.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     4336 2023-04-24 20:56:05.000000 remin-0.0.4/src/remin/solver.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-26 12:00:54.042894 remin-0.0.4/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      735 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-26 12:00:54.000000 remin-0.0.4/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.0.3/.gitignore` & `remin-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/LICENSE` & `remin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/PKG-INFO` & `remin-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.3
+Version: 0.0.4
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `remin-0.0.3/README.md` & `remin-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/examples/example_heat_problem.ipynb` & `remin-0.0.4/examples/example_heat_problem.ipynb`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/pyproject.toml` & `remin-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `remin-0.0.3/src/remin/domain.py` & `remin-0.0.4/src/remin/domain.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/src/remin/func.py` & `remin-0.0.4/src/remin/func.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/src/remin/residual.py` & `remin-0.0.4/src/remin/residual.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from torch.utils.data import (Dataset, ConcatDataset, BatchSampler, DataLoader)
 
 
 class Residual:
 
     def __init__(self, domain, equations, batch_size=None):
         self.domain = domain
-        if isinstance(domain, (list, tuple)):
+        if isinstance(equations, (list, tuple)):
             self.equations = equations
-        self.equations = [equations]
+        else:
+            self.equations = [equations]
         if batch_size is None: self.batch_size = len(domain)
         else: self.batch_size = batch_size
 
     def to_torch(self, device):
         return torch.from_numpy(self.domain).float().to(device)
 
     @staticmethod
@@ -38,26 +39,32 @@
 class ResBatchSampler(BatchSampler):
 
     def __init__(self, cumulative_sizes, batch_sizes) -> None:
         self.cumul_sizes = cumulative_sizes
         self.batch_sizes = batch_sizes
         self.batch_size = sum(batch_sizes)
         self.ndata = len(batch_sizes)
+        self.batch = [None] * self.batch_size
+        self.batch_shift = [None] * self.batch_size
+        start_idx, batch_idx = 0, 0
+        for i in range(self.ndata):
+            batch_size = self.batch_sizes[i]
+            cumul_size = self.cumul_sizes[i]
+            for j in range(batch_size):
+                self.batch_shift[batch_idx + j] = (batch_size, cumul_size)
+                self.batch[batch_idx + j] = start_idx + j
+            start_idx = cumul_size
+            batch_idx += batch_size
 
     def __iter__(self):
         for i in range(self.cumul_sizes[-1] // self.batch_size):
-            batch = []
-            start_idx = 0
-            for idx in range(self.ndata):
-                batch_size = self.batch_sizes[idx]
-                cumul_size = self.cumul_sizes[idx]
-                start = (start_idx + batch_size * i) % cumul_size
-                batch += list(range(start, start + batch_size))
-                start_idx = cumul_size
-            yield batch
+            for j in range(self.batch_size):
+                batch_size, cumul_size = self.batch_shift[j]
+                self.batch[j] = (self.batch[j] + batch_size * i) % cumul_size
+            yield self.batch
 
 
 class ResidualLoader:
 
     def __init__(self, residuals, fully_loaded=False, batched=False, **args) -> None:
         if fully_loaded and batched:
             raise ValueError('Fully loaded models can not be batched.')
@@ -92,11 +99,14 @@
         self.dataset = ConcatDataset(self.datasets)
         self.vsplit = [self.batch_sizes[0]]
         for batch_size in self.batch_sizes[1:-1]:
             self.vsplit.append(self.vsplit[-1] + batch_size)
         if self.batched:
             self.batch_sampler = ResBatchSampler(self.dataset.cumulative_sizes,
                                                  self.batch_sizes)
-        self.loader = DataLoader(self.dataset,
-                                 batch_size=len(self.dataset),
-                                 batch_sampler=self.batch_sampler,
-                                 **self.args)
+            self.loader = DataLoader(self.dataset,
+                                     batch_sampler=self.batch_sampler,
+                                     **self.args)
+        else:
+            self.loader = DataLoader(self.dataset,
+                                     batch_size=len(self.dataset),
+                                     **self.args)
```

### Comparing `remin-0.0.3/src/remin/solver.py` & `remin-0.0.4/src/remin/solver.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.3/src/remin.egg-info/PKG-INFO` & `remin-0.0.4/src/remin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.3
+Version: 0.0.4
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

