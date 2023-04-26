# Comparing `tmp/nest-analysis-1.0.2.tar.gz` & `tmp/nest-analysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nest-analysis-1.0.2.tar", last modified: Mon Jan 30 07:51:22 2023, max compression
+gzip compressed data, was "nest-analysis-1.0.3.tar", last modified: Tue Apr 25 16:20:31 2023, max compression
```

## Comparing `nest-analysis-1.0.2.tar` & `nest-analysis-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,55 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.833603 nest-analysis-1.0.2/
--rw-r--r--   0 ben        (501) staff       (20)     1075 2022-07-20 21:32:56.000000 nest-analysis-1.0.2/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      164 2023-01-30 07:51:22.833674 nest-analysis-1.0.2/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     3380 2023-01-30 03:05:11.000000 nest-analysis-1.0.2/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.826752 nest-analysis-1.0.2/nest/
--rw-r--r--   0 ben        (501) staff       (20)      144 2023-01-10 19:24:56.000000 nest-analysis-1.0.2/nest/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.828270 nest-analysis-1.0.2/nest/cci/
--rw-r--r--   0 ben        (501) staff       (20)       66 2022-10-24 20:36:35.000000 nest-analysis-1.0.2/nest/cci/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)    13656 2022-12-21 01:38:54.000000 nest-analysis-1.0.2/nest/cci/cci.py
--rw-r--r--   0 ben        (501) staff       (20)     2835 2022-05-03 06:28:46.000000 nest-analysis-1.0.2/nest/cci/cellchat.py
--rw-r--r--   0 ben        (501) staff       (20)     2065 2023-01-30 07:14:51.000000 nest-analysis-1.0.2/nest/cci/spatial.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.828804 nest-analysis-1.0.2/nest/data/
--rw-r--r--   0 ben        (501) staff       (20)       43 2022-05-03 06:28:46.000000 nest-analysis-1.0.2/nest/data/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6094 2023-01-30 03:17:28.000000 nest-analysis-1.0.2/nest/data/data.py
--rw-r--r--   0 ben        (501) staff       (20)     1276 2022-10-24 20:37:25.000000 nest-analysis-1.0.2/nest/data/database.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.829820 nest-analysis-1.0.2/nest/hmrf/
--rw-r--r--   0 ben        (501) staff       (20)       19 2022-05-03 06:28:46.000000 nest-analysis-1.0.2/nest/hmrf/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     7301 2022-11-16 03:05:05.000000 nest-analysis-1.0.2/nest/hmrf/hmrf.py
--rw-r--r--   0 ben        (501) staff       (20)     3523 2022-11-16 03:05:05.000000 nest-analysis-1.0.2/nest/hmrf/hmrf_new.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.831188 nest-analysis-1.0.2/nest/hotspot/
--rw-r--r--   0 ben        (501) staff       (20)      137 2022-10-22 01:59:31.000000 nest-analysis-1.0.2/nest/hotspot/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)    18087 2023-01-30 03:05:11.000000 nest-analysis-1.0.2/nest/hotspot/coexpression.py
--rw-r--r--   0 ben        (501) staff       (20)     5232 2022-12-05 23:03:42.000000 nest-analysis-1.0.2/nest/hotspot/geometry.py
--rw-r--r--   0 ben        (501) staff       (20)    15610 2023-01-16 01:20:03.000000 nest-analysis-1.0.2/nest/hotspot/hotspot.py
--rw-r--r--   0 ben        (501) staff       (20)     4737 2022-11-08 22:57:54.000000 nest-analysis-1.0.2/nest/hotspot/hotspots_3d.py
--rw-r--r--   0 ben        (501) staff       (20)     4335 2022-12-23 16:49:12.000000 nest-analysis-1.0.2/nest/hotspot/interaction_hotspot.py
--rw-r--r--   0 ben        (501) staff       (20)     8875 2022-12-21 02:51:11.000000 nest-analysis-1.0.2/nest/methods.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.832331 nest-analysis-1.0.2/nest/plot/
--rw-r--r--   0 ben        (501) staff       (20)       89 2022-10-22 01:59:16.000000 nest-analysis-1.0.2/nest/plot/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6125 2023-01-10 18:37:27.000000 nest-analysis-1.0.2/nest/plot/hotspots.py
--rw-r--r--   0 ben        (501) staff       (20)        0 2022-10-22 01:58:53.000000 nest-analysis-1.0.2/nest/plot/pl3d.py
--rw-r--r--   0 ben        (501) staff       (20)    11768 2023-01-01 04:07:01.000000 nest-analysis-1.0.2/nest/plot/plot.py
--rw-r--r--   0 ben        (501) staff       (20)     7046 2022-12-06 09:42:34.000000 nest-analysis-1.0.2/nest/plot/tracksplot.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.832789 nest-analysis-1.0.2/nest/utility/
--rw-r--r--   0 ben        (501) staff       (20)       23 2022-10-24 20:36:47.000000 nest-analysis-1.0.2/nest/utility/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     3118 2023-01-30 07:37:15.000000 nest-analysis-1.0.2/nest/utility/utility.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-01-30 07:51:22.833469 nest-analysis-1.0.2/nest_analysis.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)      164 2023-01-30 07:51:22.000000 nest-analysis-1.0.2/nest_analysis.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      781 2023-01-30 07:51:22.000000 nest-analysis-1.0.2/nest_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-01-30 07:51:22.000000 nest-analysis-1.0.2/nest_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)      139 2023-01-30 07:51:22.000000 nest-analysis-1.0.2/nest_analysis.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        5 2023-01-30 07:51:22.000000 nest-analysis-1.0.2/nest_analysis.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       89 2022-01-08 19:57:45.000000 nest-analysis-1.0.2/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)      379 2023-01-30 07:51:22.833935 nest-analysis-1.0.2/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.075050 nest-analysis-1.0.3/
+-rw-r--r--   0 ben        (501) staff       (20)     1075 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)      164 2023-04-25 16:20:31.075105 nest-analysis-1.0.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     3536 2023-04-25 16:18:26.000000 nest-analysis-1.0.3/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.068615 nest-analysis-1.0.3/nest/
+-rw-r--r--   0 ben        (501) staff       (20)      168 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.070297 nest-analysis-1.0.3/nest/benchmarks/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     3515 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/agglomerative.py
+-rw-r--r--   0 ben        (501) staff       (20)     4964 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/parameters.py
+-rw-r--r--   0 ben        (501) staff       (20)     9985 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/parameters_synthetic.py
+-rw-r--r--   0 ben        (501) staff       (20)     6205 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/parameters_synthetic_segmentation.py
+-rw-r--r--   0 ben        (501) staff       (20)     4917 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/subsampling.py
+-rw-r--r--   0 ben        (501) staff       (20)     1936 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/benchmarks/synthetic_analysis.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.070893 nest-analysis-1.0.3/nest/cci/
+-rw-r--r--   0 ben        (501) staff       (20)       66 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/cci/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)    13656 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/cci/cci.py
+-rw-r--r--   0 ben        (501) staff       (20)     2835 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/cci/cellchat.py
+-rw-r--r--   0 ben        (501) staff       (20)     2065 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/cci/spatial.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.071313 nest-analysis-1.0.3/nest/data/
+-rw-r--r--   0 ben        (501) staff       (20)       43 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/data/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6117 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/data/data.py
+-rw-r--r--   0 ben        (501) staff       (20)     1276 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/data/database.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.071595 nest-analysis-1.0.3/nest/datasets/
+-rw-r--r--   0 ben        (501) staff       (20)       23 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/datasets/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)      828 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/datasets/slideseq.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.072058 nest-analysis-1.0.3/nest/hmrf/
+-rw-r--r--   0 ben        (501) staff       (20)       19 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hmrf/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     7301 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hmrf/hmrf.py
+-rw-r--r--   0 ben        (501) staff       (20)     3523 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hmrf/hmrf_new.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.072984 nest-analysis-1.0.3/nest/hotspot/
+-rw-r--r--   0 ben        (501) staff       (20)      137 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)    19054 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/coexpression.py
+-rw-r--r--   0 ben        (501) staff       (20)     5406 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/geometry.py
+-rw-r--r--   0 ben        (501) staff       (20)    16378 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/hotspot.py
+-rw-r--r--   0 ben        (501) staff       (20)     4737 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/hotspots_3d.py
+-rw-r--r--   0 ben        (501) staff       (20)     4335 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/hotspot/interaction_hotspot.py
+-rw-r--r--   0 ben        (501) staff       (20)     8989 2023-04-25 01:33:35.000000 nest-analysis-1.0.3/nest/methods.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.073654 nest-analysis-1.0.3/nest/plot/
+-rw-r--r--   0 ben        (501) staff       (20)       89 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/plot/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6289 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/plot/hotspots.py
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/plot/pl3d.py
+-rw-r--r--   0 ben        (501) staff       (20)    11915 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/plot/plot.py
+-rw-r--r--   0 ben        (501) staff       (20)     7046 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/plot/tracksplot.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.074191 nest-analysis-1.0.3/nest/utility/
+-rw-r--r--   0 ben        (501) staff       (20)       23 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/utility/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     3118 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/nest/utility/utility.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-04-25 16:20:31.074920 nest-analysis-1.0.3/nest_analysis.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)      164 2023-04-25 16:20:31.000000 nest-analysis-1.0.3/nest_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1086 2023-04-25 16:20:31.000000 nest-analysis-1.0.3/nest_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-04-25 16:20:31.000000 nest-analysis-1.0.3/nest_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)      136 2023-04-25 16:20:31.000000 nest-analysis-1.0.3/nest_analysis.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)        5 2023-04-25 16:20:31.000000 nest-analysis-1.0.3/nest_analysis.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       89 2023-04-21 19:05:26.000000 nest-analysis-1.0.3/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)      375 2023-04-25 16:20:31.075343 nest-analysis-1.0.3/setup.cfg
```

### Comparing `nest-analysis-1.0.2/LICENSE` & `nest-analysis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/README.md` & `nest-analysis-1.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-[![Documentation Status](https://readthedocs.org/projects/nest-analysis/badge/?version=latest)](https://nest-analysis.readthedocs.io/en/latest/?badge=latest)
-
-
 # NeST
 
 ## Analysis of nested hierarchical structure in spatial transcriptomic data
 
 Please see our manuscript at [TBA].
 
 ## Installation
 
-For best results, or to run the rpy2 based functionality, installing in 
-an isolated conda environment is recommended. A full installation including NeST can be
-created with the included environment.yml file:
 
-`conda env create environment.yml`
+For best results, or to run the rpy2 based functionality, installing in 
+an isolated conda environment is recommended. A full installation including NeST and the provided examples can be
+created by:
 
-`conda activate nest`
+1. Clone the NeST repository
+2. Navigate inside the repository in a command prompt
+3. Create the conda environment using the provided environment file: `conda env create environment.yml`
+4. Activate the conda environment: `conda activate nest`
+5. Install the NeST package locally: `pip install .`
+6. To run examples, navigate inside the `examples/` directory and run `jupyter notebook`.
 
-NeST can also be directly installed through pip as 
+NeST can be directly installed through pip as 
 `pip install nest-analysis`
 
+
 ## Usage
 
 Here we overview the main functions available in NeST along with examples from Slideseq (Stickels et al 2021) and Seqfish [cite] datasets. See `/examples` for further information and full running example.
 
 ### Nested Hierarchical Structure
 
 We load the adata object through `squidpy` wrapped by the `nest.data.get_data` function, which can be used to load a variety of datasets including all used in the manuscript.
```

### Comparing `nest-analysis-1.0.2/nest/cci/cci.py` & `nest-analysis-1.0.3/nest/cci/cci.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/cci/cellchat.py` & `nest-analysis-1.0.3/nest/cci/cellchat.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/cci/spatial.py` & `nest-analysis-1.0.3/nest/cci/spatial.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/data/data.py` & `nest-analysis-1.0.3/nest/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 
 def default_parameters(dataset):
     if "V1_Breast_Cancer_Block_A" in dataset:
         neighbor_eps = 300
         min_samples = 4
         hotspot_min_size = 15
-    elif dataset in VISIUM_DATASETS:
+    elif dataset in VISIUM_DATASETS or dataset == "visium":
         neighbor_eps = 170
         min_samples = 4
         hotspot_min_size = 15
     elif dataset == "seqfish":
         neighbor_eps = 0.12
         min_samples = 10
         hotspot_min_size = 25
```

### Comparing `nest-analysis-1.0.2/nest/data/database.py` & `nest-analysis-1.0.3/nest/data/database.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/hmrf/hmrf.py` & `nest-analysis-1.0.3/nest/hmrf/hmrf.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/hmrf/hmrf_new.py` & `nest-analysis-1.0.3/nest/hmrf/hmrf_new.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/hotspot/coexpression.py` & `nest-analysis-1.0.3/nest/hotspot/coexpression.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,42 +122,62 @@
     for idx in range(adata.shape[0]):
         t = np.where(multi_hotspots_array[idx, :])
         type_counter[t] += 1
 
     return sorted(type_counter.items(), key=lambda x: -x[1])
 
 
-def hotspot_decomposition(adata, compute_type_counts=False, neg_weight=1.0):
+def hotspot_decomposition(adata: AnnData, neg_weight: float = 1.0, verbose=False):
+    """
+    Decompose the single-gene hotspots computed for each gene in terms of coexpression hotspots 
+    by a simple greedy optimization algorithm.
+
+    :param adata: anndata object containing single-gene and coexpression hotspots
+    :type adata: AnnData
+    :param neg_weight: How much to penalize spots in coex. hotspot not in single gene hotspot (default 1.0)
+    :type neg_weight: float
+    :param verbose: Controls whether a progress bar is displayed (default: False)
+    :type verbose: bool
+
+    :returns: weights_dict dictionary, where keys are genes present in `adata`, and items are a tuple of a binary membership
+        vector over all coex. hotspots, and a quality score.
+    """
     # assumes that single-gene hotspots and multi-gene hotspots have already been computed
     all_hotspots = [v for v in adata.obs if "hotspots_" in v and "multi" not in v]
     multi_hotspots = [v for v in adata.obs if "hotspots_multi" in v]
 
     multi_hotspots_df = sc.get.obs_df(adata, keys=multi_hotspots)
     # compute to matrix, 0 -> 1, nan -> 0
     multi_hotspots_array = np.nan_to_num(np.array(multi_hotspots_df, dtype=np.float32) + 1).astype(
         np.int_)
 
     weights_dict = hotspot_decomposition_keys(adata, all_hotspots, multi_hotspots_array,
-                                              neg_weight=neg_weight)
+                                              neg_weight=neg_weight, verbose=verbose)
 
     type_counter = Counter()
     if compute_type_counts:
         types = [tuple(np.where(weights)[0]) for (weights, _) in weights_dict.values() if
                  np.sum(weights) > 0]
         for t in types:
             for subset in powerset(t):
                 type_counter[subset] += 1
         return weights_dict, sorted(type_counter.items(), key=lambda x: -x[1])
 
     return weights_dict
 
 
-def hotspot_decomposition_keys(adata, keys, multi_hotspots_array, neg_weight=None):
+def hotspot_decomposition_keys(adata, keys, multi_hotspots_array, neg_weight=None, verbose=False):
     weights_dict = {}
-    for hotspot in tqdm(keys):
+    
+    if verbose:
+        pbar = tqdm(keys)
+    else:
+        pbar = keys
+
+    for hotspot in pbar:
         hotspot_vector = np.array(adata.obs[hotspot], dtype=np.float32)
         hotspot_vector[pd.notnull(hotspot_vector)] = 1
         hotspot_vector = np.nan_to_num(np.array(hotspot_vector, dtype=np.float32)).astype(np.int_)
 
         weights, score = hotspot_decomposition_sub(hotspot_vector, multi_hotspots_array,
                                                    neg_weight=neg_weight)
         hotspot_name = hotspot[9:]
@@ -227,14 +247,15 @@
             hotspot_lookup.append((hotspot_key, v.categories[c]))
 
         num_hotspots += n_hotspots
 
     indices = np.concatenate(indices_list)
     data = np.ones(indices.shape)
     hotspot_matrix = csr_matrix((data, indices, indptr)).tocsc()
+    hotspot_matrix.resize(hotspot_matrix.shape[0], adata.shape[0])
 
     hotspot_sizes = np.array(hotspot_sizes, dtype=np.float32)
 
     # Iterate over columns, each representing a spot and the hotspots it belongs to
     num_pairs = 0
     combination_iterators = []
     num_pairs_arr = []
@@ -385,19 +406,22 @@
             continue
         multigene_hotspot = [hotspot_lookup[i] for i in c]
         multigene_hotspots.append(multigene_hotspot)
 
     return multigene_hotspots
 
 
-def compute_multi_boundaries(adata, alpha_max, alpha_min, ids=None):
+def compute_multi_boundaries(adata, alpha_max, alpha_min, ids=None, verbose=False):
     multi_hotspots = [v for v in adata.obs if "hotspots_multi" in v]
 
     adata.uns["multi_boundaries"] = {}
-    for idx, hotspot_key in tqdm(enumerate(multi_hotspots), total=len(multi_hotspots)):
+    pbar = enumerate(multi_hotspots)
+    if verbose:
+        pbar = tqdm(pbar, total=len(multi_hotspots))
+    for idx, hotspot_key in pbar:
         if ids is not None and idx not in ids:
             continue
         boundary = compute_hotspot_boundary(adata, hotspot_key, 0, alpha_max=alpha_max,
                                             alpha_min=alpha_min)
         # saving of anndata converts dictionary indices in .uns to strings anyway
         adata.uns["multi_boundaries"][str(idx)] = boundary
 
@@ -405,15 +429,15 @@
 def multi_closure(adata):
     hotspot_keys = [v for v in adata.obs if "hotspots_multi" in v]
     points = adata.obsm['spatial']
     for idx, hotspot_key in enumerate(hotspot_keys):
         boundary = adata.uns["multi_boundaries"][str(idx)]
         path = matplotlib.path.Path(boundary)
         v = pd.Categorical(path.contains_points(points, radius=-0.01), categories=(True,))
-        v.categories = [0]
+        v.rename_categories([0])
         adata.obs[hotspot_key] = v
 
 
 def powerset(iterable):
     s = list(iterable)
     return chain.from_iterable(combinations(s, r) for r in range(1, len(s) + 1))
 
@@ -442,8 +466,10 @@
             count += 1
         cc[v] += 1
         res[idx] = mapping[v]
     min_size = 50
     for k, v in cc.items():
         if v < min_size:
             res[res == mapping[k]] = 0
-    adata.obs['coex_multiset'] = pd.Categorical(res)
+    adata.obs['coex_multiset'] = pd.Categorical(res)
+
+    return mapping
```

### Comparing `nest-analysis-1.0.2/nest/hotspot/geometry.py` & `nest-analysis-1.0.3/nest/hotspot/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,23 +97,28 @@
                 print(var.shape, var)
         genes_by_fc = [v[0] for v in sorted(zip(markers[cur_ind], gene_fc), key=lambda x: -x[1])]
         markers[cur_ind] = genes_by_fc
 
     return markers
 
 
-def similarity_map(adata, idx, ax=None, linewidth=0.5, linecolor="black", title=""):
+def similarity_map(adata, idx, adata_ref=None, ax=None, linewidth=0.5, linecolor="black", title=""):
+    if adata_ref is None:
+        adata_ref = adata
     ncells = adata.shape[0]
     arr = np.zeros(ncells)
     var_names = np.array([v.casefold() for v in adata.var_names])
-    for key, c in adata.uns['multi_hotspots'][str(idx)]:
-        sub = pd.notnull(adata.obs[key]).to_numpy().astype(np.int_).reshape(-1)
-        arr += sub
+    for key, c in adata_ref.uns['multi_hotspots'][str(idx)]:
+        try:
+            sub = pd.notnull(adata.obs[key]).to_numpy().astype(np.int_).reshape(-1)
+            arr += sub
+        except KeyError:
+            continue
     # normalize
-    arr /= np.max(arr)
+    arr /= len(adata_ref.uns['multi_hotspots'][str(idx)])
 
     return arr
 
 
 def sim_linkage(adata, method='single'):
     # Compute pairwise similarity between all clusters
     n_ch = len(adata.uns['multi_hotspots'])
```

### Comparing `nest-analysis-1.0.2/nest/hotspot/hotspot.py` & `nest-analysis-1.0.3/nest/hotspot/hotspot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from statsmodels.stats.multitest import fdrcorrection
 from scipy.stats import mannwhitneyu
 from scipy.spatial import Delaunay
 try:
     from scipy.sparse import csc_array
 except ImportError:
     from scipy.sparse import csc_matrix as csc_array
+from sklearn.neighbors import BallTree
 from tqdm import tqdm
 from shapely import geometry
 from shapely.ops import unary_union, polygonize
 from multiprocessing import Pool
 import matplotlib as mpl
 
 from nest.utility import get_neighbor_adjacency
@@ -438,8 +439,26 @@
         return (key, c, try_alpha_shape(subcoords, alpha_max=10,
                                alpha_min=0.001))
     except ValueError:
         return (key, c, None)
 
 
 def clear_hotspots(adata):
-    adata.obs.drop(adata.obs.filter(regex='hotspots').columns.tolist(), axis=1, inplace=True)
+    adata.obs.drop(adata.obs.filter(regex='hotspots').columns.tolist(), axis=1, inplace=True)
+
+
+def get_min_samples_from_density(adata, eps, density):
+    """
+    Helper function for choosing the min_samples parameter used in computing single-gene hotspots. Given adata object and the
+    neighbor_eps parameter (how far to look), choose a min_samples corresponding to, on average, at least a fraction `density` of
+    spots within neighbor_eps being active.
+    """
+    # Compute mean number of other spots within neighbor_eps
+    coords = adata.obsm['spatial']
+    tree = BallTree(coords)
+    n_cells = len(coords)
+
+    nearby_col = tree.query_radius(coords, eps)
+    mean_neighbors = np.mean([len(v) for v in nearby_col]) - 1
+    min_samples  = np.ceil(density * mean_neighbors).astype(np.int_)
+
+    return min_samples
```

### Comparing `nest-analysis-1.0.2/nest/hotspot/hotspots_3d.py` & `nest-analysis-1.0.3/nest/hotspot/hotspots_3d.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/hotspot/interaction_hotspot.py` & `nest-analysis-1.0.3/nest/hotspot/interaction_hotspot.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/methods.py` & `nest-analysis-1.0.3/nest/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 raise KeyError
             res = adata.uns['cellchat_res']
         except KeyError as e:
             res = self.run(adata, group_by)
             adata.uns['cellchat_res'] = res
         v = res[res['interaction_name_2'] == interaction][np.array(['target', 'prob'])].groupby('target').sum()
         # TODO: check that we have a nonzero number of rows in v
-        v.index = adata.obs['class'].cat.categories[v.index - 1]
+        v.index = adata.obs[group_by].cat.categories[v.index - 1]
         # fill in any missing categories with 0 for next step lookup to work
         for s in set(np.unique(adata.obs[group_by])) - set(v.index):
             v.loc[s, 'prob'] = 0
         adata.obs[key] = np.array(v.loc[adata.obs[group_by], 'prob'])
 
 class BayesSpace:
     """
@@ -164,15 +164,19 @@
         import sys
         import contextlib
 
         output = sys.stdout if verbose else None
         adatasub = adata.copy()
         with contextlib.redirect_stdout(output):
             adatasub.var_names_make_unique()
-            adatasub.X = np.exp(adatasub.X.toarray()) - 1
+            try:
+                adatasub.X = adatasub.X.toarray()
+            except AttributeError:
+                pass
+            adatasub.X = np.exp(adatasub.X) - 1
             spg.prefilter_genes(adatasub, min_cells=3)  # avoiding all genes are zeros
             spg.prefilter_specialgenes(adatasub)
             # Normalize and take log for UMI
             sc.pp.normalize_per_cell(adatasub)
             sc.pp.log1p(adatasub)
 
             # get adjacency matrix
@@ -206,15 +210,15 @@
 
             clf = spg.SpaGCN()
             clf.set_l(l)
 
             # Run
             clf.train(adatasub, adj, init_spa=True, init="kmeans", n_clusters=self.regions, tol=5e-3,
                       lr=0.05,
-                      max_epochs=200)
+                      max_epochs=500)
             y_pred, prob = clf.predict()
             adata.obs[self.label_name] = pd.Categorical(y_pred)
 
     @property
     def class_labels(self):
         return self.y_pred
```

### Comparing `nest-analysis-1.0.2/nest/plot/hotspots.py` & `nest-analysis-1.0.3/nest/plot/hotspots.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,14 @@
             **kwargs)
 
     if show:
         plt.show()
 
 
 def hotspots_multiple(adata, nrows, ncols, hotspot_keys=None, figsize=None):
-    # interactions = ["WNT5A_FZD2", "WNT5B_FZD2", "WNT11_FZD2", "APLN_APLNR",
-    #                "FGF5_FGFR1", "FGF10_FGFR1", "FGF15_FGFR1", "FGF5_FGFR2"]
 
     if hotspot_keys is None:
         obs_keys = list(adata.obs)
         hotspot_keys = [v[9:] for v in obs_keys if "hotspots_" in v]
         nrows = int(np.ceil(len(hotspot_keys) / ncols))
 
     fig, axs = plt.subplots(nrows, ncols, figsize=figsize)
@@ -58,15 +56,15 @@
             axs[i, j].set_xlabel('')
             axs[i, j].set_ylabel('')
     plt.tight_layout()
 
 
 def multi_hotspots(adata, show=True, inds=None, spotcolor=None, ax=None, num=None, linewidth=0.5,
                    legend_ncol=None, alpha_img=1.0, color_type=None, alpha=150, base_color=None,
-                   frameon=False, cm1=None,
+                   frameon=False, cm1=None, show_colorbar=False,
                    **kwargs):
     # TODO: docstring
     if color_type is None:
         color_type = "index"
 
     #cm1 = mpl.cm.get_cmap('tab20')
     if cm1 is None:
@@ -142,28 +140,30 @@
         ax.legend(legend_handles, legend_labels, loc="center left", bbox_to_anchor=(1, 0.5),
                   ncol=legend_ncol, frameon=False)
         #ax.legend(legend_handles, legend_labels, loc="upper center", bbox_to_anchor=(0.5, 0.0),
         #          ncol=legend_ncol)
     elif color_type == "genes":
         ax.get_figure().colorbar(sm, orientation='vertical', label='coexpressed genes',
                                  shrink=0.8)
+    elif show_colorbar == True:
+        ax.get_figure().colorbar(mpl.cm.ScalarMappable(norm=colors.NoNorm(vmin=0, vmax=1), cmap=sns.color_palette("Reds", as_cmap=True)), 
+                                 orientation='vertical', label="",
+                                 shrink=0.6)
 
 
     #plt.tight_layout()
     if show:
         plt.show()
 
 
-def all_coex_hotspots(adata, ncol=4, figsize=None):
+def all_coex_hotspots(adata, ncol=4, figsize=None, **kwargs):
     num_coex_hotspot = len(adata.uns['multi_hotspots']) + 1
     nrow = np.ceil(num_coex_hotspot / ncol).astype(np.int_)
     fig, axs = plt.subplots(nrow, ncol, figsize=figsize)
     axs = axs.ravel()
     keyfn = lambda x: int(x[0])
     for idx, (k, multi_hotspot) in enumerate(sorted(adata.uns['multi_hotspots'].items(), key=keyfn)):
         num_genes = len(multi_hotspot)
         hotspots(adata, f"multi_{k}", title=f"CH {k} ({num_genes} genes)", labels=None, palette="b",
-                         alpha_img=0.5, show=False, ax=axs[idx])
+                         alpha_img=0.5, show=False, ax=axs[idx], **kwargs)
     for k in range(num_coex_hotspot-1, nrow*ncol):
-        axs[k].set_axis_off()
-
-
+        axs[k].set_axis_off()
```

### Comparing `nest-analysis-1.0.2/nest/plot/plot.py` & `nest-analysis-1.0.3/nest/plot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,34 +151,37 @@
         ax.set_title(" - ".join([v.capitalize() for v in interaction.split("_")]))
     if show:
         plt.show()
 
     return ax
 
 
-def plot_similarity_map(adata, idx, ax=None, linewidth=0.5, linecolor="black", title="",
+def plot_similarity_map(adata, idx, adata_ref=None, ax=None, linewidth=0.5, linecolor="black", title="",
                         show=False, **kwargs):
     if ax is None:
         fig, ax = plt.subplots()
     try:
         scale_factor = list(adata.uns['spatial'].values())[0]['scalefactors'][
             'tissue_hires_scalef']
     except KeyError:
         if scale is not None:
             scale_factor = scale
         else:
             scale_factor = 1
-    try:
-        boundary = scale_factor * adata.uns["multi_boundaries"][str(idx)]
-    except KeyError:
-        raise ValueError("Need to compute boundaries first")
-    #ax.fill(boundary[:, 0], boundary[:, 1], color_string)
-    ax.plot(boundary[:, 0], boundary[:, 1], linewidth=linewidth, color=linecolor)
+    if adata_ref is None or adata_ref is adata:
+        try:
+            boundary = scale_factor * adata.uns["multi_boundaries"][str(idx)]
+            #ax.fill(boundary[:, 0], boundary[:, 1], color_string)
+            ax.plot(boundary[:, 0], boundary[:, 1], linewidth=linewidth, color=linecolor)
+        except KeyError:
+            # if no boundaries are computed, don't draw the boundary
+            pass
+        
 
-    arr = similarity_map(adata, idx=idx)
+    arr = similarity_map(adata, idx=idx, adata_ref=adata_ref)
 
     adata.obs['tmp'] = arr
     spatial(adata, color="tmp", alpha_img=0.5, ax=ax, title=title, frameon=False, show=show,
             **kwargs)
 
 
 # Construct hotspot tree
```

### Comparing `nest-analysis-1.0.2/nest/plot/tracksplot.py` & `nest-analysis-1.0.3/nest/plot/tracksplot.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest/utility/utility.py` & `nest-analysis-1.0.3/nest/utility/utility.py`

 * *Files identical despite different names*

### Comparing `nest-analysis-1.0.2/nest_analysis.egg-info/SOURCES.txt` & `nest-analysis-1.0.3/nest_analysis.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 nest/__init__.py
 nest/methods.py
+nest/benchmarks/__init__.py
+nest/benchmarks/agglomerative.py
+nest/benchmarks/parameters.py
+nest/benchmarks/parameters_synthetic.py
+nest/benchmarks/parameters_synthetic_segmentation.py
+nest/benchmarks/subsampling.py
+nest/benchmarks/synthetic_analysis.py
 nest/cci/__init__.py
 nest/cci/cci.py
 nest/cci/cellchat.py
 nest/cci/spatial.py
 nest/data/__init__.py
 nest/data/data.py
 nest/data/database.py
+nest/datasets/__init__.py
+nest/datasets/slideseq.py
 nest/hmrf/__init__.py
 nest/hmrf/hmrf.py
 nest/hmrf/hmrf_new.py
 nest/hotspot/__init__.py
 nest/hotspot/coexpression.py
 nest/hotspot/geometry.py
 nest/hotspot/hotspot.py
```

