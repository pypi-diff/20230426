# Comparing `tmp/Slpapy-0.2.1.tar.gz` & `tmp/Slpapy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.2.1.tar", last modified: Mon Apr 24 01:56:38 2023, max compression
+gzip compressed data, was "Slpapy-0.2.2.tar", last modified: Wed Apr 26 05:05:08 2023, max compression
```

## Comparing `Slpapy-0.2.1.tar` & `Slpapy-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.913779 Slpapy-0.2.1/
--rw-rw-rw-   0        0        0      159 2023-04-24 01:56:38.912779 Slpapy-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.878780 Slpapy-0.2.1/Slpapy/
--rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.2.1/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.1/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.910779 Slpapy-0.2.1/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.1/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.1/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.1/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.1/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.1/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.1/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.1/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5223 2023-04-24 01:55:15.000000 Slpapy-0.2.1/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:56:38.887780 Slpapy-0.2.1/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 01:56:38.000000 Slpapy-0.2.1/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 01:56:38.913779 Slpapy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-04-24 01:55:15.000000 Slpapy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:05:08.874923 Slpapy-0.2.2/
+-rw-rw-rw-   0        0        0      159 2023-04-26 05:05:08.874923 Slpapy-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 05:05:08.845923 Slpapy-0.2.2/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.2.2/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.2/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:05:08.872923 Slpapy-0.2.2/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.2/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.2/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.2/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.2/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.2/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.2/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.2/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.2/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.2/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.2/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.2/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.2/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.2/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.2/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5424 2023-04-26 05:03:54.000000 Slpapy-0.2.2/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:05:08.852924 Slpapy-0.2.2/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-04-26 05:05:08.000000 Slpapy-0.2.2/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-04-26 05:05:08.000000 Slpapy-0.2.2/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 05:05:08.000000 Slpapy-0.2.2/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-26 05:05:08.000000 Slpapy-0.2.2/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 05:05:08.000000 Slpapy-0.2.2/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 05:05:08.875924 Slpapy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-04-26 05:04:11.000000 Slpapy-0.2.2/setup.py
```

### Comparing `Slpapy-0.2.1/Slpapy/Data_reconstruction.py` & `Slpapy-0.2.2/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/MZ_ppm_match.py` & `Slpapy-0.2.2/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/beats.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/logging.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.2.2/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.1/Slpapy/processing_analyze.py` & `Slpapy-0.2.2/Slpapy/processing_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,37 @@
 from .Spatial_map import Spatial_map
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
 
+def matrix_mz_filter(adata, mz,):
+    # 删除adata的var中包含的mz的var值
+    adata = adata[:, ~adata.var.index.isin(mz)]
+    return adata
+
+
+
+
+
 
 
 def XYadata(adata):
     df = preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])
     counts = csr_matrix(df, dtype=np.float32)
     XYmatrix = ad.AnnData(counts)
     # 为x和y轴提供索引
     XYmatrix.obs_names = adata.obs_names
     XYmatrix.var_names = ['X', 'Y']
     t = adata.obs
     adata = ad.concat([adata, XYmatrix], axis=1)
     adata.obs = t
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
+    print('Space integration complete')
     return adata
 
 
 def pp_analyze(adata,onlyhighly):
     # 显示在所有细胞中在每个单细胞中产生最高计数分数的脂质
     # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
     # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
```

### Comparing `Slpapy-0.2.1/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.2.2/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

