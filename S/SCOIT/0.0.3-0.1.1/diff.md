# Comparing `tmp/SCOIT-0.0.3.tar.gz` & `tmp/SCOIT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SCOIT-0.0.3.tar", last modified: Wed Sep 21 15:13:52 2022, max compression
+gzip compressed data, was "dist/SCOIT-0.1.1.tar", last modified: Wed Apr 26 03:57:28 2023, max compression
```

## Comparing `SCOIT-0.0.3.tar` & `SCOIT-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2022-09-21 15:13:52.648088 SCOIT-0.0.3/
--rw-r--r--   0 wangruohan   (501) staff       (20)     1070 2022-07-29 09:06:11.000000 SCOIT-0.0.3/LICENSE
--rw-r--r--   0 wangruohan   (501) staff       (20)     4869 2022-09-21 15:13:52.647803 SCOIT-0.0.3/PKG-INFO
--rw-r--r--   0 wangruohan   (501) staff       (20)     4328 2022-07-30 09:20:36.000000 SCOIT-0.0.3/README.md
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2022-09-21 15:13:52.646187 SCOIT-0.0.3/SCOIT.egg-info/
--rw-r--r--   0 wangruohan   (501) staff       (20)     4869 2022-09-21 15:13:52.000000 SCOIT-0.0.3/SCOIT.egg-info/PKG-INFO
--rw-r--r--   0 wangruohan   (501) staff       (20)      239 2022-09-21 15:13:52.000000 SCOIT-0.0.3/SCOIT.egg-info/SOURCES.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)        1 2022-09-21 15:13:52.000000 SCOIT-0.0.3/SCOIT.egg-info/dependency_links.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)       19 2022-09-21 15:13:52.000000 SCOIT-0.0.3/SCOIT.egg-info/requires.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)        6 2022-09-21 15:13:52.000000 SCOIT-0.0.3/SCOIT.egg-info/top_level.txt
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2022-09-21 15:13:52.646995 SCOIT-0.0.3/scoit/
--rw-r--r--   0 wangruohan   (501) staff       (20)      167 2022-09-21 14:39:57.000000 SCOIT-0.0.3/scoit/__init__.py
--rw-r--r--   0 wangruohan   (501) staff       (20)    16990 2022-07-29 09:06:11.000000 SCOIT-0.0.3/scoit/multi_omics_model.py
--rw-r--r--   0 wangruohan   (501) staff       (20)     9527 2022-09-21 14:40:14.000000 SCOIT-0.0.3/scoit/tensorsc_model.py
--rw-r--r--   0 wangruohan   (501) staff       (20)       38 2022-09-21 15:13:52.648186 SCOIT-0.0.3/setup.cfg
--rw-r--r--   0 wangruohan   (501) staff       (20)      820 2022-09-21 15:13:36.000000 SCOIT-0.0.3/setup.py
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.307657 SCOIT-0.1.1/
+-rw-r--r--   0 wangruohan   (501) staff       (20)     1070 2022-07-29 09:06:11.000000 SCOIT-0.1.1/LICENSE
+-rw-r--r--   0 wangruohan   (501) staff       (20)     6585 2023-04-26 03:57:28.307312 SCOIT-0.1.1/PKG-INFO
+-rw-r--r--   0 wangruohan   (501) staff       (20)     6044 2023-04-26 03:46:00.000000 SCOIT-0.1.1/README.md
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.301508 SCOIT-0.1.1/SCOIT.egg-info/
+-rw-r--r--   0 wangruohan   (501) staff       (20)     6585 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/PKG-INFO
+-rw-r--r--   0 wangruohan   (501) staff       (20)      313 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/SOURCES.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)        1 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/dependency_links.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)       19 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/requires.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)        6 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/top_level.txt
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.306290 SCOIT-0.1.1/scoit/
+-rw-rw-r--   0 wangruohan   (501) staff       (20)      167 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/__init__.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     2251 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/cell_analysis.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     1005 2023-04-26 03:43:07.000000 SCOIT-0.1.1/scoit/gene_analysis.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    16990 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/multi_omics_model.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    20854 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/tensorsc_model.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    18424 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/unionCom_alignment.py
+-rw-r--r--   0 wangruohan   (501) staff       (20)       38 2023-04-26 03:57:28.307770 SCOIT-0.1.1/setup.cfg
+-rw-rw-r--   0 wangruohan   (501) staff       (20)      820 2023-04-26 03:18:22.000000 SCOIT-0.1.1/setup.py
```

### Comparing `SCOIT-0.0.3/LICENSE` & `SCOIT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SCOIT-0.0.3/PKG-INFO` & `SCOIT-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 Metadata-Version: 2.1
 Name: SCOIT
-Version: 0.0.3
+Version: 0.1.1
 Summary: SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.
 Home-page: https://github.com/deepomicslab/SCOIT
 Author: WANG Ruohan
 Author-email: ruohawang2-c@my.cityu.edu.hk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCOIT
-SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration. SCOIT accepts the input of datasets from multiple omics, with missing values allowed.
+SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multiomic data integration. SCOIT accepts the input of datasets from multiple omics, with missing values allowed.
 
 ![image](https://github.com/deepomicslab/SCOIT/blob/main/framework.png)
 
 # Getting started
 
 ## Prerequisite
 + numpy
++ scipy
++ sklearn
++ communities
++ igraph
 + pytorch 1.9.0
 
 ## Install
 ```
 pip install SCOIT
 ```
 
 ## Examples
+We put the complete scripts for the analysis described in the manuscript under ```examples/``` directory for detailed usage examples and reproduction. The example data can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1F_WBwNsHggjTqgFfTm6IugNKpb0xJTje?usp=sharing).
+
 This is an example of multiple datasets when features have corresponding information.
+
 ```Python
 from scoit import sc_multi_omics
 
 data = np.array([expression_data, methylation_data])
 sc_model = sc_multi_omics()
 predict_data = sc_model.fit(data) # the imputed data
 np.savetxt("global_cell_embeddings.csv", sc_model.C, delimiter = ',') # global cell embeddings
 np.savetxt("global_gene_embeddings.csv", sc_model.G, delimiter = ',') # global gene embeddings
 np.savetxt("local_cell_embeddings.csv", sc_model.C, delimiter = ',') # omics-specific cell embeddings
 np.savetxt("local_gene_embeddings.csv", sc_model.G, delimiter = ',') # omics-specific gene embeddings
 
 # imputation
 imputed_expression_data = predict_data[0]
 imputed_methylation_data = predict_data[1]
+
 ```
 When the features of different omics do not have corresponding information, please use the ```fit_list``` function, which accepts the input as a list of matrices.
 ```Python
 from scoit import sc_multi_omics
 
 data = [expression_data, protein_data]
 sc_model = sc_multi_omics()
@@ -66,34 +74,68 @@
 from scoit import sc_multi_omics
 
 data = [expression_data, protein_data]
 sc_model = sc_multi_omics()
 predict_data = sc_model.fit_list_complete(data)
 ```
 
-We put the complete scripts for the analysis described in the manuscript under ```examples/``` directory for detailed usage examples and reproduction. The example data can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1F_WBwNsHggjTqgFfTm6IugNKpb0xJTje?usp=sharing).
-
 ## Parameters
 ###  ```sc_multi_omics```
-> + ```K1```: The local element-wise product parameter, see the manuscript for details (default=20).
-> + ```K2```: The local element-wise product parameter (default=20).
-> + ```K3```: The local element-wise product parameter (default=20).
-> + ```random_seed```: The random seed used in optimization (default=111).
+> + ```K1```: The local element-wise product parameter, see the manuscript for details (default=30).
+> + ```K2```: The local element-wise product parameter (default=30).
+> + ```K3```: The local element-wise product parameter (default=30).
+> + ```random_seed```: The random seed used in optimization (default=123).
 
 ###  ```fit```
+> + ```normalization```: Whether to applied min-max normalization (default=True).
+> + ```pre_impute```: Whether to applied KNNImputer for pre-processing (default=False).
 > + ```opt```: The optimization algorithm for gradient descent, including SGD, Adam, Adadelta, Adagrad, AdamW, SparseAdam, Adamax, ASGD, LBFGS (default="Adam").
 > + ```dist```:The distribution used for modeling, including gaussian, poisson, negative_bionomial (default="gaussian").
 > + ```lr```: The learning rate for gradient descent (default=1e-2).
 > + ```n_epochs```: The number of optimization epochs (default=1000).
-> + ```lambda_C_regularizer```: The coefficient for the penalty term of global cell embeddings (default=0.01).
-> + ```lambda_G_regularizer```: The coefficient for the penalty term of global gene embeddings (default=0.01).
-> + ```lambda_O_regularizer```: The coefficient list for the penalty term of global omics embeddings; the length of the list should be the same with the number of omics (default=[0.01, 0.01]).
-> + ```lambda_OC_regularizer```: The coefficient list for the penalty term of omics-specific cell embeddings; the length of the list should be the same with the number of omics, not avaiable for complete functions (default=[1, 1]).
-> + ```lambda_OG_regularizer```: The coefficient list for the penalty term of omics-specific gene embeddings, the length of the list should be the same with the number of omics, not avaiable for list functions (default=[1, 1]).
-> + ```batch_size```: The batch size used for gradient descent, not avaiable for complete functions (default=1000).
+> + ```lambda_C_regularizer```: The coefficient for the penalty term of global cell embeddings (default=0, indicating automatically adjust.).
+> + ```lambda_G_regularizer```: The coefficient for the penalty term of global gene embeddings (default=0).
+> + ```lambda_O_regularizer```: The coefficient list for the penalty term of global omics embeddings; the length of the list should be the same with the number of omics (default=[0, 0]).
+> + ```lambda_OC_regularizer```: The coefficient list for the penalty term of omics-specific cell embeddings; the length of the list should be the same with the number of omics, not avaiable for complete functions (default=[0, 0]).
+> + ```lambda_OG_regularizer```: The coefficient list for the penalty term of omics-specific gene embeddings, the length of the list should be the same with the number of omics, not avaiable for list functions (default=[0, 0]).
+> + ```batch_size```: The batch size used for gradient descent, not avaiable for complete functions (default=256).
 > + ```device```: CPU or GPU (default='cuda' if torch.cuda.is_available() else 'cpu').
 > + ```verbose```: Whether to print loss for each epoch (default=True).
 
+###  ```cell_analysis```
+#### ```knn_adj_matrix```
+Construct KNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct KNN graph (default=20).
+#### ```snn_adj_matrix```
+Construct SNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct SNN graph (default=20).
+#### ```jsnn_adj_matrix```
+Construct jSNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct jaccard SNN graph (default=20).
+> + ```prune```: Set the score below the value to zero (default=1/15).
+#### ```RunLouvain```
+Run Louvain algorithm for the graph.
+> + ```k```: Terminate the search once this number of communities is detected (default=None).
+#### ```RunSpectral```
+Run Spectral clustering algorithm for the graph.
+> + ```k```: Number of clusters (default=5).
+#### ```RunLeiden```
+Run Leiden algorithm for the graph.
+
+###  ```gene_analysis```
+#### ```pearson_correlation```
+Calculate the correlation between the features.
+#### ```feature_projection```
+Project the feature embedding to cell embeddings and visualize with UMAP.
+> + ```umap_epochs```: The number of UMAP epochs for visualization (default=100).
+> + ```dimension```: The dimension of the embeddings to use (default=30).
+> + ```figure_name```: The saved figure name (default="feature_projections.png").
+
+
+### Version history
++ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data;
++ `v0.0.1`: Initial version.
+
 ### Maintainer
 WANG Ruohan ruohawang2-c@my.cityu.edu.hk
```

### Comparing `SCOIT-0.0.3/SCOIT.egg-info/PKG-INFO` & `SCOIT-0.1.1/SCOIT.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 Metadata-Version: 2.1
 Name: SCOIT
-Version: 0.0.3
+Version: 0.1.1
 Summary: SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.
 Home-page: https://github.com/deepomicslab/SCOIT
 Author: WANG Ruohan
 Author-email: ruohawang2-c@my.cityu.edu.hk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCOIT
-SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration. SCOIT accepts the input of datasets from multiple omics, with missing values allowed.
+SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multiomic data integration. SCOIT accepts the input of datasets from multiple omics, with missing values allowed.
 
 ![image](https://github.com/deepomicslab/SCOIT/blob/main/framework.png)
 
 # Getting started
 
 ## Prerequisite
 + numpy
++ scipy
++ sklearn
++ communities
++ igraph
 + pytorch 1.9.0
 
 ## Install
 ```
 pip install SCOIT
 ```
 
 ## Examples
+We put the complete scripts for the analysis described in the manuscript under ```examples/``` directory for detailed usage examples and reproduction. The example data can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1F_WBwNsHggjTqgFfTm6IugNKpb0xJTje?usp=sharing).
+
 This is an example of multiple datasets when features have corresponding information.
+
 ```Python
 from scoit import sc_multi_omics
 
 data = np.array([expression_data, methylation_data])
 sc_model = sc_multi_omics()
 predict_data = sc_model.fit(data) # the imputed data
 np.savetxt("global_cell_embeddings.csv", sc_model.C, delimiter = ',') # global cell embeddings
 np.savetxt("global_gene_embeddings.csv", sc_model.G, delimiter = ',') # global gene embeddings
 np.savetxt("local_cell_embeddings.csv", sc_model.C, delimiter = ',') # omics-specific cell embeddings
 np.savetxt("local_gene_embeddings.csv", sc_model.G, delimiter = ',') # omics-specific gene embeddings
 
 # imputation
 imputed_expression_data = predict_data[0]
 imputed_methylation_data = predict_data[1]
+
 ```
 When the features of different omics do not have corresponding information, please use the ```fit_list``` function, which accepts the input as a list of matrices.
 ```Python
 from scoit import sc_multi_omics
 
 data = [expression_data, protein_data]
 sc_model = sc_multi_omics()
@@ -66,34 +74,68 @@
 from scoit import sc_multi_omics
 
 data = [expression_data, protein_data]
 sc_model = sc_multi_omics()
 predict_data = sc_model.fit_list_complete(data)
 ```
 
-We put the complete scripts for the analysis described in the manuscript under ```examples/``` directory for detailed usage examples and reproduction. The example data can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1F_WBwNsHggjTqgFfTm6IugNKpb0xJTje?usp=sharing).
-
 ## Parameters
 ###  ```sc_multi_omics```
-> + ```K1```: The local element-wise product parameter, see the manuscript for details (default=20).
-> + ```K2```: The local element-wise product parameter (default=20).
-> + ```K3```: The local element-wise product parameter (default=20).
-> + ```random_seed```: The random seed used in optimization (default=111).
+> + ```K1```: The local element-wise product parameter, see the manuscript for details (default=30).
+> + ```K2```: The local element-wise product parameter (default=30).
+> + ```K3```: The local element-wise product parameter (default=30).
+> + ```random_seed```: The random seed used in optimization (default=123).
 
 ###  ```fit```
+> + ```normalization```: Whether to applied min-max normalization (default=True).
+> + ```pre_impute```: Whether to applied KNNImputer for pre-processing (default=False).
 > + ```opt```: The optimization algorithm for gradient descent, including SGD, Adam, Adadelta, Adagrad, AdamW, SparseAdam, Adamax, ASGD, LBFGS (default="Adam").
 > + ```dist```:The distribution used for modeling, including gaussian, poisson, negative_bionomial (default="gaussian").
 > + ```lr```: The learning rate for gradient descent (default=1e-2).
 > + ```n_epochs```: The number of optimization epochs (default=1000).
-> + ```lambda_C_regularizer```: The coefficient for the penalty term of global cell embeddings (default=0.01).
-> + ```lambda_G_regularizer```: The coefficient for the penalty term of global gene embeddings (default=0.01).
-> + ```lambda_O_regularizer```: The coefficient list for the penalty term of global omics embeddings; the length of the list should be the same with the number of omics (default=[0.01, 0.01]).
-> + ```lambda_OC_regularizer```: The coefficient list for the penalty term of omics-specific cell embeddings; the length of the list should be the same with the number of omics, not avaiable for complete functions (default=[1, 1]).
-> + ```lambda_OG_regularizer```: The coefficient list for the penalty term of omics-specific gene embeddings, the length of the list should be the same with the number of omics, not avaiable for list functions (default=[1, 1]).
-> + ```batch_size```: The batch size used for gradient descent, not avaiable for complete functions (default=1000).
+> + ```lambda_C_regularizer```: The coefficient for the penalty term of global cell embeddings (default=0, indicating automatically adjust.).
+> + ```lambda_G_regularizer```: The coefficient for the penalty term of global gene embeddings (default=0).
+> + ```lambda_O_regularizer```: The coefficient list for the penalty term of global omics embeddings; the length of the list should be the same with the number of omics (default=[0, 0]).
+> + ```lambda_OC_regularizer```: The coefficient list for the penalty term of omics-specific cell embeddings; the length of the list should be the same with the number of omics, not avaiable for complete functions (default=[0, 0]).
+> + ```lambda_OG_regularizer```: The coefficient list for the penalty term of omics-specific gene embeddings, the length of the list should be the same with the number of omics, not avaiable for list functions (default=[0, 0]).
+> + ```batch_size```: The batch size used for gradient descent, not avaiable for complete functions (default=256).
 > + ```device```: CPU or GPU (default='cuda' if torch.cuda.is_available() else 'cpu').
 > + ```verbose```: Whether to print loss for each epoch (default=True).
 
+###  ```cell_analysis```
+#### ```knn_adj_matrix```
+Construct KNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct KNN graph (default=20).
+#### ```snn_adj_matrix```
+Construct SNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct SNN graph (default=20).
+#### ```jsnn_adj_matrix```
+Construct jSNN graph with the cell embeddings.
+> + ```k```: The number of neighbos used to construct jaccard SNN graph (default=20).
+> + ```prune```: Set the score below the value to zero (default=1/15).
+#### ```RunLouvain```
+Run Louvain algorithm for the graph.
+> + ```k```: Terminate the search once this number of communities is detected (default=None).
+#### ```RunSpectral```
+Run Spectral clustering algorithm for the graph.
+> + ```k```: Number of clusters (default=5).
+#### ```RunLeiden```
+Run Leiden algorithm for the graph.
+
+###  ```gene_analysis```
+#### ```pearson_correlation```
+Calculate the correlation between the features.
+#### ```feature_projection```
+Project the feature embedding to cell embeddings and visualize with UMAP.
+> + ```umap_epochs```: The number of UMAP epochs for visualization (default=100).
+> + ```dimension```: The dimension of the embeddings to use (default=30).
+> + ```figure_name```: The saved figure name (default="feature_projections.png").
+
+
+### Version history
++ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data;
++ `v0.0.1`: Initial version.
+
 ### Maintainer
 WANG Ruohan ruohawang2-c@my.cityu.edu.hk
```

### Comparing `SCOIT-0.0.3/scoit/multi_omics_model.py` & `SCOIT-0.1.1/scoit/multi_omics_model.py`

 * *Files identical despite different names*

### Comparing `SCOIT-0.0.3/setup.py` & `SCOIT-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='SCOIT',
-    version='0.0.3',
+    version='0.1.1',
     packages=setuptools.find_packages(),
     url='https://github.com/deepomicslab/SCOIT',
     license='MIT',
 	author='WANG Ruohan',
     author_email='ruohawang2-c@my.cityu.edu.hk',
     description='SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.',
     long_description=long_description,
```

