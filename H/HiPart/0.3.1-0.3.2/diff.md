# Comparing `tmp/HiPart-0.3.1.tar.gz` & `tmp/HiPart-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiPart-0.3.1.tar", last modified: Tue Apr 11 01:05:50 2023, max compression
+gzip compressed data, was "HiPart-0.3.2.tar", last modified: Tue Apr 25 14:00:39 2023, max compression
```

## Comparing `HiPart-0.3.1.tar` & `HiPart-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-11 01:05:40.000000 HiPart-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 01:05:40.000000 HiPart-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-11 01:05:50.461252 HiPart-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-11 01:05:40.000000 HiPart-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 01:05:40.000000 HiPart-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:05:50.461252 HiPart-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-11 01:05:40.000000 HiPart-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.457252 HiPart-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/__utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/assets/int_viz.css
--rw-r--r--   0 runner    (1001) docker     (123)    71744 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/interactive_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-11 01:05:40.000000 HiPart-0.3.1/src/HiPart/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/src/HiPart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 01:05:50.000000 HiPart-0.3.1/src/HiPart.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:05:50.461252 HiPart-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17298 2023-04-11 01:05:40.000000 HiPart-0.3.1/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 14:00:22.000000 HiPart-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:00:22.000000 HiPart-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-25 14:00:39.615010 HiPart-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-25 14:00:22.000000 HiPart-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 14:00:23.000000 HiPart-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:00:39.615010 HiPart-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-25 14:00:23.000000 HiPart-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.611010 HiPart-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23326 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/__utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/assets/int_viz.css
+-rw-r--r--   0 runner    (1001) docker     (123)    72232 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/interactive_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-04-25 14:00:23.000000 HiPart-0.3.2/src/HiPart/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/src/HiPart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 14:00:39.000000 HiPart-0.3.2/src/HiPart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:00:39.615010 HiPart-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-04-25 14:00:23.000000 HiPart-0.3.2/tests/test_package.py
```

### Comparing `HiPart-0.3.1/LICENSE` & `HiPart-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.1/PKG-INFO` & `HiPart-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.1
+Version: 0.3.2
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
-Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart
+Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
+Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart/issues
 Keywords: data structure,tree,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -30,14 +32,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/HiPart?color=blue)](https://pypi.org/project/HiPart/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HiPart)](https://pypi.org/project/HiPart/)
 [![example workflow](https://github.com/panagiotisanagnostou/HiPart/actions/workflows/python-app.yml/badge.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/.github/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/panagiotisanagnostou/HiPart/branch/main/graph/badge.svg?token=FHoZrLjqfj)](https://codecov.io/gh/panagiotisanagnostou/HiPart)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/60c751d914474e288b369461e6e3466a)](https://www.codacy.com/gh/panagiotisanagnostou/HiPart/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=panagiotisanagnostou/HiPart&amp;utm_campaign=Badge_Grade)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/LICENSE)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05024/status.svg)](https://doi.org/10.21105/joss.05024)
 
 HiPart: Hierarchical divisive clustering toolbox
 ================================================
 This repository presents the HiPart package, an open-source native python library that provides efficient and interpretable implementations of divisive hierarchical clustering algorithms. HiPart supports interactive visualizations for the manipulation of the execution steps allowing the direct intervention of the clustering outcome. This package is highly suited for Big Data applications as the focus has been given to the computational efficiency of the implemented clustering methodologies. The dependencies used are either Python build-in packages or highly maintained stable external packages. The software is provided under the MIT license.
 
 Installation
 ------------
@@ -45,48 +48,52 @@
 
 ```bash
 pip install HiPart
 ```
 
 Simple Example Execution
 ------------------------
-The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the dePDDP algorithm and only the cluster labels are returned.
+The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the DePDDP algorithm and only the cluster labels are returned.
 
 ```python
-from HiPart.clustering import dePDDP
+from HiPart.clustering import DePDDP
 from sklearn.datasets import make_blobs
 
 X, y = make_blobs(n_samples=1500, centers=6, random_state=0)
 
-clustered_class = dePDDP(max_clusters_number=6).fit_predict(X)
+clustered_class = DePDDP(max_clusters_number=6).fit_predict(X)
 ```
 
 Users can find complete execution examples for all the algorithms of the HiPart package in the [clustering_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_example.py) file of the repository. Also, the users can find a KernelPCA method usage example in the [clustering_with_kpca_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_with_kpca_example.py) file of the repository. Finally, the file [interactive_visualization_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/interactive_visualization_example.py) contains an example execution of the interactive visualization. The instructions for the interactive visualization GUI can be found with the execution of this visualization.
 
 Documentation
 -------------
 The full documentation of the package can be found [here](https://hipart.readthedocs.io).
 
 Citation
 --------
 
 ```bibtex
-@misc{anagnostou2022hipart,
-  doi = {10.48550/ARXIV.2209.08680},
-  url = {https://arxiv.org/abs/2209.08680},
-  author = {Anagnostou, Panagiotis and Tasoulis, Sotiris and Plagianakos, Vassilis and Tasoulis, Dimitris},
-  keywords = {Machine Learning (stat.ML), Artificial Intelligence (cs.AI), Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
+@article{Anagnostou2023HiPart,
   title = {HiPart: Hierarchical Divisive Clustering Toolbox},
-  publisher = {arXiv},
-  year = {2022},
-}
+  author = {Panagiotis Anagnostou and Sotiris Tasoulis and Vassilis P. Plagianakos and Dimitris Tasoulis},
+  year = {2023},
+  journal = {Journal of Open Source Software},
+  publisher = {The Open Journal},
+  volume = {8},
+  number = {84},
+  pages = {5024},
+  doi = {10.21105/joss.05024},
+  url = {https://doi.org/10.21105/joss.05024}
+} 
 ```
 
 Acknowledgments
 ---------------
 This project has received funding from the Hellenic Foundation for Research and Innovation (HFRI), under grant agreement No 1901.
 
 Collaborators
 -------------
 Dimitris Tasoulis [:email:](mailto:d.tasoulis@thesignalgroup.com)
 Panagiotis Anagnostou [:email:](mailto:panagno@uth.gr)
 Sotiris Tasoulis [:email:](mailto:stasoulis@uth.gr)
+Vassilis Plagianakos [:email:](mailto:vpp@uth.gr)
```

### Comparing `HiPart-0.3.1/README.md` & `HiPart-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [![PyPI](https://img.shields.io/pypi/v/HiPart?color=blue)](https://pypi.org/project/HiPart/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HiPart)](https://pypi.org/project/HiPart/)
 [![example workflow](https://github.com/panagiotisanagnostou/HiPart/actions/workflows/python-app.yml/badge.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/.github/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/panagiotisanagnostou/HiPart/branch/main/graph/badge.svg?token=FHoZrLjqfj)](https://codecov.io/gh/panagiotisanagnostou/HiPart)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/60c751d914474e288b369461e6e3466a)](https://www.codacy.com/gh/panagiotisanagnostou/HiPart/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=panagiotisanagnostou/HiPart&amp;utm_campaign=Badge_Grade)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/LICENSE)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05024/status.svg)](https://doi.org/10.21105/joss.05024)
 
 HiPart: Hierarchical divisive clustering toolbox
 ================================================
 This repository presents the HiPart package, an open-source native python library that provides efficient and interpretable implementations of divisive hierarchical clustering algorithms. HiPart supports interactive visualizations for the manipulation of the execution steps allowing the direct intervention of the clustering outcome. This package is highly suited for Big Data applications as the focus has been given to the computational efficiency of the implemented clustering methodologies. The dependencies used are either Python build-in packages or highly maintained stable external packages. The software is provided under the MIT license.
 
 Installation
 ------------
@@ -15,48 +16,52 @@
 
 ```bash
 pip install HiPart
 ```
 
 Simple Example Execution
 ------------------------
-The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the dePDDP algorithm and only the cluster labels are returned.
+The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the DePDDP algorithm and only the cluster labels are returned.
 
 ```python
-from HiPart.clustering import dePDDP
+from HiPart.clustering import DePDDP
 from sklearn.datasets import make_blobs
 
 X, y = make_blobs(n_samples=1500, centers=6, random_state=0)
 
-clustered_class = dePDDP(max_clusters_number=6).fit_predict(X)
+clustered_class = DePDDP(max_clusters_number=6).fit_predict(X)
 ```
 
 Users can find complete execution examples for all the algorithms of the HiPart package in the [clustering_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_example.py) file of the repository. Also, the users can find a KernelPCA method usage example in the [clustering_with_kpca_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_with_kpca_example.py) file of the repository. Finally, the file [interactive_visualization_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/interactive_visualization_example.py) contains an example execution of the interactive visualization. The instructions for the interactive visualization GUI can be found with the execution of this visualization.
 
 Documentation
 -------------
 The full documentation of the package can be found [here](https://hipart.readthedocs.io).
 
 Citation
 --------
 
 ```bibtex
-@misc{anagnostou2022hipart,
-  doi = {10.48550/ARXIV.2209.08680},
-  url = {https://arxiv.org/abs/2209.08680},
-  author = {Anagnostou, Panagiotis and Tasoulis, Sotiris and Plagianakos, Vassilis and Tasoulis, Dimitris},
-  keywords = {Machine Learning (stat.ML), Artificial Intelligence (cs.AI), Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
+@article{Anagnostou2023HiPart,
   title = {HiPart: Hierarchical Divisive Clustering Toolbox},
-  publisher = {arXiv},
-  year = {2022},
-}
+  author = {Panagiotis Anagnostou and Sotiris Tasoulis and Vassilis P. Plagianakos and Dimitris Tasoulis},
+  year = {2023},
+  journal = {Journal of Open Source Software},
+  publisher = {The Open Journal},
+  volume = {8},
+  number = {84},
+  pages = {5024},
+  doi = {10.21105/joss.05024},
+  url = {https://doi.org/10.21105/joss.05024}
+} 
 ```
 
 Acknowledgments
 ---------------
 This project has received funding from the Hellenic Foundation for Research and Innovation (HFRI), under grant agreement No 1901.
 
 Collaborators
 -------------
 Dimitris Tasoulis [:email:](mailto:d.tasoulis@thesignalgroup.com)
 Panagiotis Anagnostou [:email:](mailto:panagno@uth.gr)
 Sotiris Tasoulis [:email:](mailto:stasoulis@uth.gr)
+Vassilis Plagianakos [:email:](mailto:vpp@uth.gr)
```

### Comparing `HiPart-0.3.1/setup.py` & `HiPart-0.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 setuptools.setup(
     name="HiPart",
     version=__version__,
     url="https://github.com/panagiotisanagnostou/HiPart",
     author="Panagiotis Anagnostou",
     author_email="panagno@uth.gr",
@@ -28,15 +28,17 @@
         "statsmodels>=0.13",
         "kdepy",
         "matplotlib",
         "plotly",
         "dash>=2.0",
     ],
     project_urls={
-        "Bug Tracker": "https://github.com/panagiotisanagnostou/HiPart",
+        "Documentation": "https://hipart.readthedocs.io/en/latest/",
+        "Source Code": "https://github.com/panagiotisanagnostou/HiPart/",
+        "Bug Tracker": "https://github.com/panagiotisanagnostou/HiPart/issues",
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `HiPart-0.3.1/src/HiPart/__init__.py` & `HiPart-0.3.2/src/HiPart/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 
 """
 
 from KDEpy.NaiveKDE import NaiveKDE
 from KDEpy.TreeKDE import TreeKDE
 from KDEpy.FFTKDE import FFTKDE
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __author__ = "Panagiotis Anagnostou"
 
 TreeKDE = TreeKDE
 NaiveKDE = NaiveKDE
 FFTKDE = FFTKDE
```

### Comparing `HiPart-0.3.1/src/HiPart/__utility_functions.py` & `HiPart-0.3.2/src/HiPart/__utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import math
 import matplotlib
 import numpy as np
 import statsmodels.api as sm
 import warnings
 
 from KDEpy import FFTKDE
+from sklearn.manifold import TSNE
 from sklearn.decomposition import PCA, KernelPCA, FastICA
 
 
 def execute_decomposition_method(
         data_matrix,
         decomposition_method,
         two_dimentions,
@@ -84,14 +85,20 @@
         two_dimensions = kernel_pca.fit_transform(data_matrix)
     elif decomposition_method == "ica":
         ica = FastICA(
             n_components=n_of_dimentions,
             **decomposition_args
         )
         two_dimensions = ica.fit_transform(data_matrix)
+    elif decomposition_method == "tsne":
+        tsne = TSNE(
+            n_components=n_of_dimentions,
+            **decomposition_args
+        )
+        two_dimensions = tsne.fit_transform(data_matrix)
     else:
         raise ValueError(
             ": The decomposition method ("
             + decomposition_method
             + ") is not supported!"
         )
```

### Comparing `HiPart-0.3.1/src/HiPart/assets/int_viz.css` & `HiPart-0.3.2/src/HiPart/assets/int_viz.css`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.1/src/HiPart/clustering.py` & `HiPart-0.3.2/src/HiPart/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,35 +38,35 @@
     ----------
     Tasoulis, S. K., Tasoulis, D. K., & Plagianakos, V. P. (2010). Enhancing
     principal direction divisive clustering. Pattern Recognition, 43(10), 3391-
     3411.
 
     Parameters
     ----------
-    decomposition_method : str, optional
-        One of the ('pca', 'kpca', 'ica') supported decomposition methods used
-        as kernel for the dePDDP algorithm.
-    max_clusters_number : int, optional
+    decomposition_method : str, (optional)
+        One of the ('pca', 'kpca', 'ica', 'tsne') supported decomposition
+        methods used as kernel for the dePDDP algorithm.
+    max_clusters_number : int, (optional)
         Desired maximum number of clusters to find the dePDDP algorithm.
-    bandwidth_scale : float, optional
+    bandwidth_scale : float, (optional)
         Standard deviation scaler for the density approximation.
-    percentile : float, optional
+    percentile : float, (optional)
         The percentile distance from the dataset's edge in which a split can
         not occur. [0,0.5) values are allowed.
-    min_sample_split : int, optional
+    min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
-    visualization_utility : bool, optional
+    visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
         interactive_visualization of the package can not be created.
     **decomposition_args :
-        Arguments for each of the decomposition methods ("PCA" as "pca",
-        "KernelPCA" as "kpca", "FastICA" as "ica") utilized by the HiPart
-        package, as documented in the scikit-learn package, from which they are
-        implemented.
+        Arguments for each of the decomposition methods ("decomposition.PCA" as
+        "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
+        "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
+        documented in the scikit-learn package, from which they are implemented.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ : numpy.ndarray
         Extracted clusters from the algorithm.
@@ -271,15 +271,15 @@
         return min_density_node
 
     def calculate_node_data(self, indices, key):
         """
         Calculation of the projections onto the Principal Components with the
         utilization of the "Principal Components Analysis" or the "Kernel
         Principal Components Analysis" or the "Independent Component Analysis"
-        methods.
+        or "t-SNE" methods.
 
         Determination of the projection's density and search for its local
         minima. The lowest local minimum point within the allowed sample
         percentiles of the projection's density representation is selected
         as the split point.
 
         This function leads to the second Stopping criterion 2 of the
@@ -370,15 +370,15 @@
 
     @property
     def decomposition_method(self):
         return self._decomposition_method
 
     @decomposition_method.setter
     def decomposition_method(self, v):
-        if not (v in ["pca", "kpca", "ica"]):
+        if not (v in ["pca", "kpca", "ica", "tsne"]):
             raise ValueError(
                 "DePDDP: decomposition_method: "
                 + str(v)
                 + ": Unknown decomposition method!"
             )
         self._decomposition_method = v
 
@@ -496,33 +496,33 @@
     ----------
     Tasoulis, S. K., Tasoulis, D. K., & Plagianakos, V. P. (2010). Enhancing
     principal direction divisive clustering. Pattern Recognition, 43(10), 3391-
     3411.
 
     Parameters
     ----------
-    decomposition_method : str, optional
-        One of the ('pca', 'kpca', 'ica') supported decomposition methods used
-        as kernel for the iPDDP algorithm.
-    max_clusters_number : int, optional
+    decomposition_method : str, (optional)
+        One of the ('pca', 'kpca', 'ica', 'tsne') supported decomposition
+        methods used as kernel for the iPDDP algorithm.
+    max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
-    percentile : float, optional
+    percentile : float, (optional)
         The percentile distance from the dataset's edge in which a split can
         not occur. [0,0.5) values are allowed.
-    min_sample_split : int, optional
+    min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
-    visualization_utility : bool, optional
+    visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
         interactive_visualization of the package can not be created.
     **decomposition_args :
-        Arguments for each of the decomposition methods ("PCA" as "pca",
-        "KernelPCA" as "kpca", "FastICA" as "ica") utilized by the HiPart
-        package, as documented in the scikit-learn package, from which they are
-        implemented.
+        Arguments for each of the decomposition methods ("decomposition.PCA" as
+        "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
+        "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
+        documented in the scikit-learn package, from which they are implemented.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ :
         Extracted clusters from the algorithm.
@@ -734,15 +734,15 @@
         return next_split
 
     def calculate_node_data(self, indices, key):
         """
         Calculation of the projections onto the Principal Components with the
         utilization of the "Principal Components Analysis" or the "Kernel
         Principal Components Analysis" or the "Independent Component Analysis"
-        methods.
+        or "t-SNE" methods.
 
         Determination of the projection's maximum distance between to
         consecutive points and chooses it as the split-point for this node.
 
         This function leads to the second Stopping criterion 2 of the
         algorithm.
 
@@ -830,15 +830,15 @@
 
     @property
     def decomposition_method(self):
         return self._decomposition_method
 
     @decomposition_method.setter
     def decomposition_method(self, v):
-        if not (v in ["pca", "kpca", "ica"]):
+        if not (v in ["pca", "kpca", "ica", "tsne"]):
             raise ValueError(
                 "IPDDP: decomposition_method: "
                 + str(v)
                 + ": Unknown decomposition method!"
             )
         self._decomposition_method = v
 
@@ -934,32 +934,32 @@
     ----------
     Zeimpekis, D., & Gallopoulos, E. (2008). Principal direction divisive
     partitioning with kernels and k-means steering. In Survey of Text Mining
     II (pp. 45-64). Springer, London.
 
     Parameters
     ----------
-    decomposition_method : str, optional
-        One of the supported dimensionality reduction methods used as kernel
-        for the kM-PDDP algorithm.
-    max_clusters_number : int, optional
+    decomposition_method : str, (optional)
+        One of the ('pca', 'kpca', 'ica', 'tsne') supported decomposition
+        methods used as kernel for the kMeans-PDDP algorithm.
+    max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
-    min_sample_split : int, optional
+    min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
-    visualization_utility : bool, optional
+    visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
         interactive_visualization of the package can not be created.
-    random_seed : int, optional
+    random_seed : int, (optional)
         The random seed fed in the k-Means algorithm
     **decomposition_args :
-        Arguments for each of the decomposition methods ("PCA" as "pca",
-        "KernelPCA" as "kpca", "FastICA" as "ica") utilized by the HiPart
-        package, as documented in the scikit-learn package, from which they are
-        implemented.
+        Arguments for each of the decomposition methods ("decomposition.PCA" as
+        "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
+        "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
+        documented in the scikit-learn package, from which they are implemented.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ :
         Extracted clusters from the algorithm.
@@ -1165,15 +1165,15 @@
         return maximum_frobenius
 
     def calculate_node_data(self, indices, key):
         """
         Calculation of the projections onto the Principal Components with the
         utilization of the "Principal Components Analysis" or the "Kernel
         Principal Components Analysis" or the "Independent Component Analysis"
-        methods.
+        or "t-SNE" methods.
 
         Determination of the projection's clusters by utilizing the binary
         k-means clustering algorithm.
 
         This function leads to the second Stopping criterion 2 of the
         algorithm.
 
@@ -1197,15 +1197,15 @@
                 data_matrix=self.X[indices, :],
                 decomposition_method=self.decomposition_method,
                 two_dimentions=self.visualization_utility,
                 decomposition_args=self.decomposition_args,
             )
             one_dimension = np.array([[i] for i in projection[:, 0]])
 
-            model = KMeans(n_clusters=2, random_state=self.random_seed)
+            model = KMeans(n_clusters=2, n_init="auto", random_state=self.random_seed)
             model.fit(one_dimension)
             labels = model.predict(one_dimension)
             centers = model.cluster_centers_
 
             # Labels for the split selection
             label_zero = np.where(labels == 0)
             label_one = np.where(labels == 1)
@@ -1252,15 +1252,15 @@
 
     @property
     def decomposition_method(self):
         return self._decomposition_method
 
     @decomposition_method.setter
     def decomposition_method(self, v):
-        if not (v in ["pca", "kpca", "ica"]):
+        if not (v in ["pca", "kpca", "ica", "tsne"]):
             raise ValueError(
                 "KMPDDP: decomposition_method: "
                 + str(v)
                 + ": Unknown decomposition method!"
             )
         self._decomposition_method = v
 
@@ -1367,30 +1367,30 @@
     References
     ----------
     Boley, D. (1998). Principal direction divisive partitioning. Data mining
     and knowledge discovery, 2(4), 325-344.
 
     Parameters
     ----------
-    decomposition_method : str, optional
-        One of the supported dimensionality reduction methods used as kernel
-        for the PDDP algorithm.
-    max_clusters_number : int, optional
+    decomposition_method : str, (optional)
+        One of the ('pca', 'kpca', 'ica', 'tsne') supported decomposition
+        methods used as kernel for the PDDP algorithm.
+    max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
-    min_sample_split : int, optional
+    min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
-    visualization_utility : bool, optional
+    visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
         interactive_visualization of the package can not be created.
     **decomposition_args :
-        Arguments for each of the decomposition methods ("PCA" as "pca",
-        "KernelPCA" as "kpca", "FastICA" as "ica") utilized by the HiPart
-        package, as documented in the scikit-learn package, from which they are
-        implemented.
+        Arguments for each of the decomposition methods ("decomposition.PCA" as
+        "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
+        "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
+        documented in the scikit-learn package, from which they are implemented.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ :
         Extracted clusters from the algorithm.
@@ -1602,15 +1602,15 @@
         return maximum_scatter
 
     def calculate_node_data(self, indices, key):
         """
         Calculation of the projections onto the Principal Components with the
         utilization of the "Principal Components Analysis" or the "Kernel
         Principal Components Analysis" or the "Independent Component Analysis"
-        methods.
+        or "t-SNE" methods.
 
         The projection's clusters are split on the median pf the projected
         data.
 
         This function leads to the second Stopping criterion 2 of the
         algorithm.
 
@@ -1667,15 +1667,15 @@
 
     @property
     def decomposition_method(self):
         return self._decomposition_method
 
     @decomposition_method.setter
     def decomposition_method(self, v):
-        if not (v in ["pca", "kpca", "ica"]):
+        if not (v in ["pca", "kpca", "ica", "tsne"]):
             raise ValueError(
                 "PDDP: decomposition_method: " + str(v) + ": Unknown decomposition method!"
             )
         self._decomposition_method = v
 
     @property
     def max_clusters_number(self):
@@ -1770,19 +1770,19 @@
     Savaresi, S. M., & Boley, D. L. (2001, April). On the performance of
     bisecting K-means and PDDP. In Proceedings of the 2001 SIAM International
     Conference on Data Mining (pp. 1-14). Society for Industrial and Applied
     Mathematics.
 
     Parameters
     ----------
-    max_clusters_number : int, optional
+    max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
-    min_sample_split : int, optional
+    min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
-    random_seed : int, optional
+    random_seed : int, (optional)
         The random seed fed in the k-Means algorithm.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ : numpy.ndarray
@@ -2002,15 +2002,15 @@
         data : dict
             The necessary data for each node which are splitting point.
 
         """
         # if the number of samples
         if indices.shape[0] > self.min_sample_split:
 
-            model = KMeans(n_clusters=2, random_state=self.random_seed)
+            model = KMeans(n_clusters=2, n_init="auto", random_state=self.random_seed)
             model.fit(data_matrix)
             labels = model.predict(data_matrix)
             centers = model.cluster_centers_
 
             left_child = indices[np.where(labels == 0)]
             right_child = indices[np.where(labels == 1)]
             centers = centers
@@ -2088,28 +2088,28 @@
     @property
     def output_matrix(self):
         tnds = self.tree.nodes
         output_matrix = [np.full(self.samples_number, 0)]
 
         # The dictionary of nodes contains the created node from the KMPDDP
         # algorithm sorted from the root to the last split.
-        for l in tnds:
+        for t in tnds:
             # For the output matrix we don't want the leaves of the tree. Each
             # level of the output matrix represents a split the split exist in
             # the internal nodes of the tree. Only by checking the children of
             # those nodes we can extract the data for the current split.
-            if not tnds[l].is_leaf():
+            if not tnds[t].is_leaf():
                 # create output cluster splitting matrix
                 tmp = np.copy(output_matrix[-1])
                 # Left child according to the tree creation process
-                tmp[self.tree.children(l)[0].data["indices"]] = \
-                    self.tree.children(l)[0].identifier
+                tmp[self.tree.children(t)[0].data["indices"]] = \
+                    self.tree.children(t)[0].identifier
                 # Right child according to the tree creation process
-                tmp[self.tree.children(l)[1].data["indices"]] = \
-                    self.tree.children(l)[1].identifier
+                tmp[self.tree.children(t)[1].data["indices"]] = \
+                    self.tree.children(t)[1].identifier
 
                 # The output_matrix is created transposed
                 output_matrix.append(tmp)
         # the first row contains only zeros
         del output_matrix[0]
 
         # transpose the output_matrix to be extracted
```

### Comparing `HiPart-0.3.1/src/HiPart/interactive_visualization.py` & `HiPart-0.3.2/src/HiPart/interactive_visualization.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.1/src/HiPart/visualizations.py` & `HiPart-0.3.2/src/HiPart/visualizations.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.3.1/src/HiPart.egg-info/PKG-INFO` & `HiPart-0.3.2/src/HiPart.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.3.1
+Version: 0.3.2
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
-Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart
+Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
+Project-URL: Bug Tracker, https://github.com/panagiotisanagnostou/HiPart/issues
 Keywords: data structure,tree,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -30,14 +32,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/HiPart?color=blue)](https://pypi.org/project/HiPart/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HiPart)](https://pypi.org/project/HiPart/)
 [![example workflow](https://github.com/panagiotisanagnostou/HiPart/actions/workflows/python-app.yml/badge.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/.github/workflows/python-app.yml)
 [![codecov](https://codecov.io/gh/panagiotisanagnostou/HiPart/branch/main/graph/badge.svg?token=FHoZrLjqfj)](https://codecov.io/gh/panagiotisanagnostou/HiPart)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/60c751d914474e288b369461e6e3466a)](https://www.codacy.com/gh/panagiotisanagnostou/HiPart/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=panagiotisanagnostou/HiPart&amp;utm_campaign=Badge_Grade)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/panagiotisanagnostou/HiPart/blob/main/LICENSE)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05024/status.svg)](https://doi.org/10.21105/joss.05024)
 
 HiPart: Hierarchical divisive clustering toolbox
 ================================================
 This repository presents the HiPart package, an open-source native python library that provides efficient and interpretable implementations of divisive hierarchical clustering algorithms. HiPart supports interactive visualizations for the manipulation of the execution steps allowing the direct intervention of the clustering outcome. This package is highly suited for Big Data applications as the focus has been given to the computational efficiency of the implemented clustering methodologies. The dependencies used are either Python build-in packages or highly maintained stable external packages. The software is provided under the MIT license.
 
 Installation
 ------------
@@ -45,48 +48,52 @@
 
 ```bash
 pip install HiPart
 ```
 
 Simple Example Execution
 ------------------------
-The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the dePDDP algorithm and only the cluster labels are returned.
+The example bellow is the simplest form of the package's execution. Shortly, it shows the creation of synthetic clustering dataset containing 6 clusters. Afterwards it is clustered with the DePDDP algorithm and only the cluster labels are returned.
 
 ```python
-from HiPart.clustering import dePDDP
+from HiPart.clustering import DePDDP
 from sklearn.datasets import make_blobs
 
 X, y = make_blobs(n_samples=1500, centers=6, random_state=0)
 
-clustered_class = dePDDP(max_clusters_number=6).fit_predict(X)
+clustered_class = DePDDP(max_clusters_number=6).fit_predict(X)
 ```
 
 Users can find complete execution examples for all the algorithms of the HiPart package in the [clustering_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_example.py) file of the repository. Also, the users can find a KernelPCA method usage example in the [clustering_with_kpca_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/clustering_with_kpca_example.py) file of the repository. Finally, the file [interactive_visualization_example](https://github.com/panagiotisanagnostou/HiPart/blob/main/examples/interactive_visualization_example.py) contains an example execution of the interactive visualization. The instructions for the interactive visualization GUI can be found with the execution of this visualization.
 
 Documentation
 -------------
 The full documentation of the package can be found [here](https://hipart.readthedocs.io).
 
 Citation
 --------
 
 ```bibtex
-@misc{anagnostou2022hipart,
-  doi = {10.48550/ARXIV.2209.08680},
-  url = {https://arxiv.org/abs/2209.08680},
-  author = {Anagnostou, Panagiotis and Tasoulis, Sotiris and Plagianakos, Vassilis and Tasoulis, Dimitris},
-  keywords = {Machine Learning (stat.ML), Artificial Intelligence (cs.AI), Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
+@article{Anagnostou2023HiPart,
   title = {HiPart: Hierarchical Divisive Clustering Toolbox},
-  publisher = {arXiv},
-  year = {2022},
-}
+  author = {Panagiotis Anagnostou and Sotiris Tasoulis and Vassilis P. Plagianakos and Dimitris Tasoulis},
+  year = {2023},
+  journal = {Journal of Open Source Software},
+  publisher = {The Open Journal},
+  volume = {8},
+  number = {84},
+  pages = {5024},
+  doi = {10.21105/joss.05024},
+  url = {https://doi.org/10.21105/joss.05024}
+} 
 ```
 
 Acknowledgments
 ---------------
 This project has received funding from the Hellenic Foundation for Research and Innovation (HFRI), under grant agreement No 1901.
 
 Collaborators
 -------------
 Dimitris Tasoulis [:email:](mailto:d.tasoulis@thesignalgroup.com)
 Panagiotis Anagnostou [:email:](mailto:panagno@uth.gr)
 Sotiris Tasoulis [:email:](mailto:stasoulis@uth.gr)
+Vassilis Plagianakos [:email:](mailto:vpp@uth.gr)
```

### Comparing `HiPart-0.3.1/tests/test_package.py` & `HiPart-0.3.2/tests/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,54 +255,54 @@
     assert isinstance(results, np.ndarray) and results.ndim == 1
 
 
 def test_bicecting_kmeans_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["bicecting_kmeans"]
+    matrix_control = data_import["BisectingKmeans"]
 
     matrix_test = BisectingKmeans(
         max_clusters_number=5,
         random_seed=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_depddp_pca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["dePDDP_pca"]
+    matrix_control = data_import["DePDDP_pca"]
 
     matrix_test = DePDDP(
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_ipddp_pca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["iPDDP_pca"]
+    matrix_control = data_import["IPDDP_pca"]
 
     matrix_test = IPDDP(
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_kmpddp_pca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["kM_PDDP_pca"]
+    matrix_control = data_import["KMPDDP_pca"]
 
     matrix_test = KMPDDP(
         max_clusters_number=5,
         random_seed=1256,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
@@ -321,43 +321,43 @@
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_depddp_ica_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["dePDDP_ica"]
+    matrix_control = data_import["DePDDP_ica"]
 
     matrix_test = DePDDP(
         decomposition_method="ica",
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_ipddp_ica_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["iPDDP_ica"]
+    matrix_control = data_import["IPDDP_ica"]
 
     matrix_test = IPDDP(
         decomposition_method="ica",
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_kmpddp_ica_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["kM_PDDP_ica"]
+    matrix_control = data_import["KMPDDP_ica"]
 
     matrix_test = KMPDDP(
         decomposition_method="ica",
         max_clusters_number=5,
         random_seed=1256,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
@@ -378,43 +378,43 @@
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_depddp_kpca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["dePDDP_kpca"]
+    matrix_control = data_import["DePDDP_kpca"]
 
     matrix_test = DePDDP(
         decomposition_method="kpca",
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_ipddp_kpca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["iPDDP_kpca"]
+    matrix_control = data_import["IPDDP_kpca"]
 
     matrix_test = IPDDP(
         decomposition_method="kpca",
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
 def test_kmpddp_kpca_results(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
-    matrix_control = data_import["kM_PDDP_kpca"]
+    matrix_control = data_import["KMPDDP_kpca"]
 
     matrix_test = KMPDDP(
         decomposition_method="kpca",
         max_clusters_number=5,
         random_seed=1256,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
@@ -431,14 +431,71 @@
         decomposition_method="kpca",
         max_clusters_number=5,
         random_state=1256,
     ).fit(data_import["data"]).output_matrix
     assert np.sum(matrix_test == matrix_control) == 6000
 
 
+def test_depddp_tsne_results(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    matrix_control = data_import["DePDDP_tsne"]
+
+    matrix_test = DePDDP(
+        decomposition_method="tsne",
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"]).output_matrix
+    assert np.sum(matrix_test == matrix_control) == 6000
+
+
+def test_ipddp_tsne_results(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    matrix_control = data_import["IPDDP_tsne"]
+
+    matrix_test = IPDDP(
+        decomposition_method="tsne",
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"]).output_matrix
+    assert np.sum(matrix_test == matrix_control) == 6000
+
+
+def test_kmpddp_tsne_results(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    matrix_control = data_import["KMPDDP_tsne"]
+
+    matrix_test = KMPDDP(
+        decomposition_method="tsne",
+        max_clusters_number=5,
+        random_seed=1256,
+        random_state=1256,
+    ).fit(data_import["data"]).output_matrix
+    assert np.sum(matrix_test == matrix_control) == 6000
+
+
+def test_pddp_tsne_results(datadir):
+    with open(datadir.join('test_data.dump'), "rb") as inf:
+        data_import = pickle.load(inf)
+
+    matrix_control = data_import["PDDP_tsne"]
+
+    matrix_test = PDDP(
+        decomposition_method="tsne",
+        max_clusters_number=5,
+        random_state=1256,
+    ).fit(data_import["data"]).output_matrix
+    assert np.sum(matrix_test == matrix_control) == 6000
+
+
 def test_split_visualization_plot_1(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     clustering = DePDDP(max_clusters_number=5).fit(data_import["data"])
     try:
         viz.split_visualization(clustering)
@@ -518,15 +575,14 @@
         viz.split_visualization(clustering)
         assert True
     except Exception:
         assert False
 
 
 def test_split_visualization_typeerror(datadir):
-
     try:
         viz.split_visualization(np.array([1, 2, 3]))
         assert False
     except Exception:
         assert True
```

