# Comparing `tmp/dianna-0.8.0.tar.gz` & `tmp/dianna-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dianna-0.8.0.tar", last modified: Tue Apr  4 09:51:29 2023, max compression
+gzip compressed data, was "dianna-0.9.0.tar", last modified: Wed Apr 26 12:03:41 2023, max compression
```

## Comparing `dianna-0.8.0.tar` & `dianna-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.831187 dianna-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-04 09:49:26.000000 dianna-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-04 09:49:26.000000 dianna-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-04 09:49:26.000000 dianna-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-04-04 09:51:29.831187 dianna-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-04-04 09:49:26.000000 dianna-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.823187 dianna-0.8.0/dianna/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.827187 dianna-0.8.0/dianna/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/methods/kernelshap.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/methods/lime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/methods/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/methods/rise_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.827187 dianna-0.8.0/dianna/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/utils/maskers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/utils/onnx_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/utils/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.827187 dianna-0.8.0/dianna/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/visualization/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-04 09:49:26.000000 dianna-0.8.0/dianna/visualization/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.823187 dianna-0.8.0/dianna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-04-04 09:51:29.000000 dianna-0.8.0/dianna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-04 09:51:29.000000 dianna-0.8.0/dianna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:51:29.000000 dianna-0.8.0/dianna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:49:33.000000 dianna-0.8.0/dianna.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-04 09:51:29.000000 dianna-0.8.0/dianna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 09:51:29.000000 dianna-0.8.0/dianna.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-04 09:49:26.000000 dianna-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-04 09:51:29.831187 dianna-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 09:49:26.000000 dianna-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:51:29.831187 dianna-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_common_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_kernelshap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_lime.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_onnx_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_text_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-04 09:49:26.000000 dianna-0.8.0/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.350576 dianna-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-26 12:02:41.000000 dianna-0.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-26 12:02:41.000000 dianna-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-26 12:02:41.000000 dianna-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-26 12:03:41.350576 dianna-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-26 12:02:41.000000 dianna-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.338576 dianna-0.9.0/dianna/
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.342576 dianna-0.9.0/dianna/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/methods/kernelshap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/methods/lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/methods/lime_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/methods/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/methods/rise_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.346576 dianna-0.9.0/dianna/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/utils/maskers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/utils/onnx_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/utils/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.346576 dianna-0.9.0/dianna/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/visualization/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-26 12:02:41.000000 dianna-0.9.0/dianna/visualization/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.342576 dianna-0.9.0/dianna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:03:29.000000 dianna-0.9.0/dianna.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 12:03:41.000000 dianna-0.9.0/dianna.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-26 12:02:41.000000 dianna-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-26 12:03:41.350576 dianna-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 12:02:41.000000 dianna-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:03:41.350576 dianna-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_common_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_kernelshap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_onnx_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_text_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-26 12:02:41.000000 dianna-0.9.0/tests/test_xarray.py
```

### Comparing `dianna-0.8.0/CITATION.cff` & `dianna-0.9.0/CITATION.cff`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,20 @@
     family-names: Ootes
     given-names: Laura
     orcid: "https://orcid.org/0000-0002-2800-8309"
   -
     family-names: Chandramouli
     given-names: Pranav
     orcid: "https://orcid.org/0000-0002-7896-2969"
+  -
+    family-names: Smeets
+    given-names: Stef
+    orcid: "https://orcid.org/0000-0002-5413-9038"
 
 doi: 10.5281/zenodo.5801485
-version: "0.8.0"
+version: "0.9.0"
 repository-code: "https://github.com/dianna-ai/dianna"
 keywords:
   - XAI
   - machine learning
 message: "If you use this software, please cite it using these metadata."
 license: Apache-2.0
```

### Comparing `dianna-0.8.0/LICENSE` & `dianna-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/PKG-INFO` & `dianna-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dianna
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep Insight And Neural Network Analysis
 Home-page: https://github.com/dianna-ai/dianna
 Author: DIANNA Team
 Author-email: dianna-ai@esciencecenter.nl
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/dianna-ai/dianna/issues
 Keywords: XAI,machine learning
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: publishing
-Provides-Extra: notebooks
 Provides-Extra: text
+Provides-Extra: dashboard
+Provides-Extra: notebooks
 License-File: LICENSE
 
 <!--
 title: 'DIANNA: Deep Insight And Neural Network Analysis'
 tags:
   - Python
   - explainable AI
@@ -53,18 +55,21 @@
     orcid: 0000-0002-0823-0121
     affiliation: 1
   - name: Laura Ootes^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-2800-8309
     affiliation: 1  
   - name: Pranav Chandramouli^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-7896-2969
-    affiliation: 1    
+    affiliation: 1  
   - name: Aron Jansen^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-4764-9347
-    affiliation: 1    
+    affiliation: 1  
+  - name: Stef Smeets^[co-first author] # note this makes a footnote saying 'co-first author'
+    orcid: 0000-0002-5413-9038
+    affiliation: 1  
 affiliations:
  - name: Netherlands eScience Center, Amsterdam, the Netherlands
    index: 1
 -->
 
 [![build](https://github.com/dianna-ai/dianna/actions/workflows/build.yml/badge.svg)](https://github.com/dianna-ai/dianna/actions/workflows/build.yml)
 [![Documentation Status](https://readthedocs.org/projects/dianna/badge/?version=latest)](https://dianna.readthedocs.io/en/latest/?badge=latest)
@@ -78,34 +83,34 @@
 <img align="left" src="https://user-images.githubusercontent.com/55382553/153408200-36c4de2e-7865-4934-956d-09eefd893e6a.png">
 
 # Deep Insight And Neural Network Analysis
 
 DIANNA is a Python package that brings explainable AI (XAI) to your research project. It wraps carefully selected XAI methods in a simple, uniform interface.
 It's built by, with and for (academic) researchers and research software engineers working on machine learning projects.
 
-## Why DIANNA? 
-DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format. 
+## Why DIANNA?
+DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format.
 
 After studying the vast XAI landscape we have made choices in the parts of the [XAI Taxonomy](https://doi.org/10.3390/make3030032) on which methods, data modalities and problems types to focus. Our choices, based on the largest usage in scientific literature, are shown graphically in the XAI taxonomy below:
 
 <img src="https://user-images.githubusercontent.com/3244249/196441854-24c8c6b7-2364-4cb3-90b9-1c63e3bdc345.png" alt="XAI_taxonomy" width="60%"/>
 
 The key points of DIANNA:
 
 * Provides an easy-to-use interface for non (X)AI experts
 * Implements well-known XAI methods (LIME, RISE and Kernal SHAP) chosen by systematic and objective evaluation criteria
 * Supports the de-facto standard format for neural network models - ONNX.
 * Includes clear instructions for export/conversions from Tensorflow, Pytorch, Keras and scikit-learn to ONNX.
 * Supports both images and text data modalities. Time series is work in progress, tabular data and even embeddings support is planned.
-* Comes with simple intuitive image and text benchmarks 
-* Easily extendable to other XAI methods 
+* Comes with simple intuitive image and text benchmarks
+* Easily extendable to other XAI methods
 
 For more information on the unique strengths of DIANNA with comparison to other tools, please see the [context landscape](https://dianna.readthedocs.io/en/latest/CONTEXT.html).
 
-## Installation 
+## Installation
 [![workflow pypi badge](https://img.shields.io/pypi/v/dianna.svg?colorB=blue)](https://pypi.python.org/project/dianna/)
 [![supported python versions](https://img.shields.io/pypi/pyversions/dianna)](https://pypi.python.org/project/dianna/)
 
 DIANNA can be installed from PyPI using [pip](https://pip.pypa.io/en/stable/installation/) on any of the supported Python versions (see badge):
 
 ```console
 python3 -m pip install dianna
@@ -132,15 +137,15 @@
 - your trained ONNX model ([convert my pytorch/tensorflow/keras/scikit-learn model to ONNX](https://github.com/dianna-ai/dianna#onnx-models))
 - 1 data item to be explained
 
  You get:
  - a relevance map overlayed over the data item
 
 In the library's documentation, the general usage is explained in [How to use DIANNA](https://dianna.readthedocs.io/en/latest/usage.html)
- 
+
 ### Demo movie
 
 [![Watch the video on YouTube](https://img.youtube.com/vi/u9_c5DJewLU/default.jpg)](https://youtu.be/u9_c5DJewLU)
 
 ### Text example:
 ```python
 model_path = 'your_model.onnx'  # model trained on text
@@ -181,27 +186,27 @@
 ## Datasets
 DIANNA comes with simple datasets. Their main goal is to provide intuitive insight into the working of the XAI methods. They can be used as benchmarks for evaluation and comparison of existing and new XAI methods.
 
 ### Images
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 |Binary MNIST <img width="25" alt="mnist_zero_and_one_half_size" src="https://user-images.githubusercontent.com/3244249/152354583-d7b68902-d402-4098-922b-b1a33b07e3e1.png">| Greyscale images of the digits "1" and "0" - a 2-class subset from the famous [MNIST dataset](http://yann.lecun.com/exdb/mnist/) for handwritten digit classification. |<img width="120" alt="BinaryMNIST" src="https://user-images.githubusercontent.com/3244249/150808267-3d27eae0-78f2-45f8-8569-cb2561f2c2e9.png">| [Binary MNIST dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/MNIST)|
-|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) | 
+|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) |
 |[Simple Scientific (LeafSnap30)](https://zenodo.org/record/5061353/)<img width="20" alt="LeafSnap30 Logo" src="https://user-images.githubusercontent.com/3244249/150815639-2da560d4-8b26-4eeb-9ab4-dabf221a264a.png"> | Color images of tree leaves - a 30-class post-processed subset from the LeafSnap dataset for automatic identification of North American tree species.|<img width="600" alt="LeafSnap" src="https://user-images.githubusercontent.com/3244249/150804246-f714e517-641d-48b2-af26-2f04166870d6.png">| [LeafSnap30 dataset generation](https://github.com/dianna-ai/dianna-exploration/blob/main/example_data/dataset_preparation/LeafSnap/)|
 
 ### Text
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 | [Stanford sentiment treebank](https://nlp.stanford.edu/sentiment/index.html)<img width="20" alt="nlp-logo_half_size" src="https://user-images.githubusercontent.com/3244249/152355020-908c04f3-aa99-489d-b87a-7e6b1f586118.png">|Dataset for predicting the sentiment, positive or negative, of movie reviews. | _This movie was actually neither that funny, nor super witty._|[Sentiment treebank](https://nlp.stanford.edu/sentiment/treebank.html)|
 
 ## ONNX models
 <!-- TODO: Add all links, see issue https://github.com/dianna-ai/dianna/issues/135 -->
 
 **We work with ONNX!** ONNX is a great unified neural network standard which can be used to boost reproducible science. Using ONNX for your model also gives you a boost in performance! In case your models are still in another popular DNN (deep neural network) format, here are some simple recipes to convert them:
-* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://pytorch-lightning.readthedocs.io/en/latest/api/pytorch_lightning.core.LightningModule.html#pytorch_lightning.core.LightningModule) to export pytorch-lightning models to onnx.
+* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://lightning.ai/docs/pytorch/stable/api/lightning.pytorch.core.LightningModule.html) to export pytorch-lightning models to onnx.
 * [tensorflow](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/tensorflow2onnx.ipynb) - use the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package to convert tensorflow models to onnx.
 * [keras](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/keras2onnx.ipynb) - same as the conversion from tensorflow to onnx, the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package also supports keras.
 * [scikit-learn](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/skl2onnx.ipynb) - use the [`skl2onnx`](https://github.com/onnx/sklearn-onnx) package to scikit-learn models to onnx.
 
 More converters with examples and tutorials can be found on the [ONNX tutorial page](https://github.com/onnx/tutorials).
 
 And here are links to notebooks showing how we created our models on the benchmark datasets:
@@ -232,30 +237,30 @@
 |Embedding|coming soon|coming soon|coming soon|
 |Graphs |planned|planned|planned |
 |Tabular||||
 
 
 [LRP](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0130140&type=printable) and [PatternAttribution](https://arxiv.org/pdf/1705.05598.pdf) also feature in the top 5 of our thoroughly evaluated XAI methods using objective criteria (details in coming blog-post). **Contributing by adding these and more (new) post-hoc explainability methods on ONNX models is very welcome!**
 
-## Reference documentation 
+## Reference documentation
 
 For detailed information on using specific DIANNA functions, please visit the [documentation page hosted at Readthedocs](https://dianna.readthedocs.io/en/latest).
 
 ## Contributing
 
 If you want to contribute to the development of DIANNA,
 have a look at the [contribution guidelines](https://dianna.readthedocs.io/en/latest/CONTRIBUTING.html).
 See our [developer documentation](docs/developer_info.rst) for information on developer installation, running tests, generating documentation, versioning and making a release.
 
-## How to cite us 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592607.svg)](https://zenodo.org/record/5592607)
+## How to cite us
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592606.svg)](https://zenodo.org/record/5592606)
 [![RSD](https://img.shields.io/badge/rsd-dianna-00a3e3.svg)](https://www.research-software.nl/software/dianna)
 
 If you use this package for your scientific work, please consider citing it as:
 
-    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A. (2022). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592607
+    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A., Smeets, S. (2023). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592606
 
-See also the [Zenodo page](https://zenodo.org/record/5592607) for exporting the citation to BibTteX and other formats.
+See also the [Zenodo page](https://zenodo.org/record/5592606) for exporting the citation to BibTteX and other formats.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
```

### Comparing `dianna-0.8.0/README.md` & `dianna-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,21 @@
     orcid: 0000-0002-0823-0121
     affiliation: 1
   - name: Laura Ootes^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-2800-8309
     affiliation: 1  
   - name: Pranav Chandramouli^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-7896-2969
-    affiliation: 1    
+    affiliation: 1  
   - name: Aron Jansen^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-4764-9347
-    affiliation: 1    
+    affiliation: 1  
+  - name: Stef Smeets^[co-first author] # note this makes a footnote saying 'co-first author'
+    orcid: 0000-0002-5413-9038
+    affiliation: 1  
 affiliations:
  - name: Netherlands eScience Center, Amsterdam, the Netherlands
    index: 1
 -->
 
 [![build](https://github.com/dianna-ai/dianna/actions/workflows/build.yml/badge.svg)](https://github.com/dianna-ai/dianna/actions/workflows/build.yml)
 [![Documentation Status](https://readthedocs.org/projects/dianna/badge/?version=latest)](https://dianna.readthedocs.io/en/latest/?badge=latest)
@@ -51,34 +54,34 @@
 <img align="left" src="https://user-images.githubusercontent.com/55382553/153408200-36c4de2e-7865-4934-956d-09eefd893e6a.png">
 
 # Deep Insight And Neural Network Analysis
 
 DIANNA is a Python package that brings explainable AI (XAI) to your research project. It wraps carefully selected XAI methods in a simple, uniform interface.
 It's built by, with and for (academic) researchers and research software engineers working on machine learning projects.
 
-## Why DIANNA? 
-DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format. 
+## Why DIANNA?
+DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format.
 
 After studying the vast XAI landscape we have made choices in the parts of the [XAI Taxonomy](https://doi.org/10.3390/make3030032) on which methods, data modalities and problems types to focus. Our choices, based on the largest usage in scientific literature, are shown graphically in the XAI taxonomy below:
 
 <img src="https://user-images.githubusercontent.com/3244249/196441854-24c8c6b7-2364-4cb3-90b9-1c63e3bdc345.png" alt="XAI_taxonomy" width="60%"/>
 
 The key points of DIANNA:
 
 * Provides an easy-to-use interface for non (X)AI experts
 * Implements well-known XAI methods (LIME, RISE and Kernal SHAP) chosen by systematic and objective evaluation criteria
 * Supports the de-facto standard format for neural network models - ONNX.
 * Includes clear instructions for export/conversions from Tensorflow, Pytorch, Keras and scikit-learn to ONNX.
 * Supports both images and text data modalities. Time series is work in progress, tabular data and even embeddings support is planned.
-* Comes with simple intuitive image and text benchmarks 
-* Easily extendable to other XAI methods 
+* Comes with simple intuitive image and text benchmarks
+* Easily extendable to other XAI methods
 
 For more information on the unique strengths of DIANNA with comparison to other tools, please see the [context landscape](https://dianna.readthedocs.io/en/latest/CONTEXT.html).
 
-## Installation 
+## Installation
 [![workflow pypi badge](https://img.shields.io/pypi/v/dianna.svg?colorB=blue)](https://pypi.python.org/project/dianna/)
 [![supported python versions](https://img.shields.io/pypi/pyversions/dianna)](https://pypi.python.org/project/dianna/)
 
 DIANNA can be installed from PyPI using [pip](https://pip.pypa.io/en/stable/installation/) on any of the supported Python versions (see badge):
 
 ```console
 python3 -m pip install dianna
@@ -105,15 +108,15 @@
 - your trained ONNX model ([convert my pytorch/tensorflow/keras/scikit-learn model to ONNX](https://github.com/dianna-ai/dianna#onnx-models))
 - 1 data item to be explained
 
  You get:
  - a relevance map overlayed over the data item
 
 In the library's documentation, the general usage is explained in [How to use DIANNA](https://dianna.readthedocs.io/en/latest/usage.html)
- 
+
 ### Demo movie
 
 [![Watch the video on YouTube](https://img.youtube.com/vi/u9_c5DJewLU/default.jpg)](https://youtu.be/u9_c5DJewLU)
 
 ### Text example:
 ```python
 model_path = 'your_model.onnx'  # model trained on text
@@ -154,27 +157,27 @@
 ## Datasets
 DIANNA comes with simple datasets. Their main goal is to provide intuitive insight into the working of the XAI methods. They can be used as benchmarks for evaluation and comparison of existing and new XAI methods.
 
 ### Images
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 |Binary MNIST <img width="25" alt="mnist_zero_and_one_half_size" src="https://user-images.githubusercontent.com/3244249/152354583-d7b68902-d402-4098-922b-b1a33b07e3e1.png">| Greyscale images of the digits "1" and "0" - a 2-class subset from the famous [MNIST dataset](http://yann.lecun.com/exdb/mnist/) for handwritten digit classification. |<img width="120" alt="BinaryMNIST" src="https://user-images.githubusercontent.com/3244249/150808267-3d27eae0-78f2-45f8-8569-cb2561f2c2e9.png">| [Binary MNIST dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/MNIST)|
-|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) | 
+|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) |
 |[Simple Scientific (LeafSnap30)](https://zenodo.org/record/5061353/)<img width="20" alt="LeafSnap30 Logo" src="https://user-images.githubusercontent.com/3244249/150815639-2da560d4-8b26-4eeb-9ab4-dabf221a264a.png"> | Color images of tree leaves - a 30-class post-processed subset from the LeafSnap dataset for automatic identification of North American tree species.|<img width="600" alt="LeafSnap" src="https://user-images.githubusercontent.com/3244249/150804246-f714e517-641d-48b2-af26-2f04166870d6.png">| [LeafSnap30 dataset generation](https://github.com/dianna-ai/dianna-exploration/blob/main/example_data/dataset_preparation/LeafSnap/)|
 
 ### Text
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 | [Stanford sentiment treebank](https://nlp.stanford.edu/sentiment/index.html)<img width="20" alt="nlp-logo_half_size" src="https://user-images.githubusercontent.com/3244249/152355020-908c04f3-aa99-489d-b87a-7e6b1f586118.png">|Dataset for predicting the sentiment, positive or negative, of movie reviews. | _This movie was actually neither that funny, nor super witty._|[Sentiment treebank](https://nlp.stanford.edu/sentiment/treebank.html)|
 
 ## ONNX models
 <!-- TODO: Add all links, see issue https://github.com/dianna-ai/dianna/issues/135 -->
 
 **We work with ONNX!** ONNX is a great unified neural network standard which can be used to boost reproducible science. Using ONNX for your model also gives you a boost in performance! In case your models are still in another popular DNN (deep neural network) format, here are some simple recipes to convert them:
-* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://pytorch-lightning.readthedocs.io/en/latest/api/pytorch_lightning.core.LightningModule.html#pytorch_lightning.core.LightningModule) to export pytorch-lightning models to onnx.
+* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://lightning.ai/docs/pytorch/stable/api/lightning.pytorch.core.LightningModule.html) to export pytorch-lightning models to onnx.
 * [tensorflow](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/tensorflow2onnx.ipynb) - use the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package to convert tensorflow models to onnx.
 * [keras](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/keras2onnx.ipynb) - same as the conversion from tensorflow to onnx, the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package also supports keras.
 * [scikit-learn](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/skl2onnx.ipynb) - use the [`skl2onnx`](https://github.com/onnx/sklearn-onnx) package to scikit-learn models to onnx.
 
 More converters with examples and tutorials can be found on the [ONNX tutorial page](https://github.com/onnx/tutorials).
 
 And here are links to notebooks showing how we created our models on the benchmark datasets:
@@ -205,30 +208,30 @@
 |Embedding|coming soon|coming soon|coming soon|
 |Graphs |planned|planned|planned |
 |Tabular||||
 
 
 [LRP](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0130140&type=printable) and [PatternAttribution](https://arxiv.org/pdf/1705.05598.pdf) also feature in the top 5 of our thoroughly evaluated XAI methods using objective criteria (details in coming blog-post). **Contributing by adding these and more (new) post-hoc explainability methods on ONNX models is very welcome!**
 
-## Reference documentation 
+## Reference documentation
 
 For detailed information on using specific DIANNA functions, please visit the [documentation page hosted at Readthedocs](https://dianna.readthedocs.io/en/latest).
 
 ## Contributing
 
 If you want to contribute to the development of DIANNA,
 have a look at the [contribution guidelines](https://dianna.readthedocs.io/en/latest/CONTRIBUTING.html).
 See our [developer documentation](docs/developer_info.rst) for information on developer installation, running tests, generating documentation, versioning and making a release.
 
-## How to cite us 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592607.svg)](https://zenodo.org/record/5592607)
+## How to cite us
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592606.svg)](https://zenodo.org/record/5592606)
 [![RSD](https://img.shields.io/badge/rsd-dianna-00a3e3.svg)](https://www.research-software.nl/software/dianna)
 
 If you use this package for your scientific work, please consider citing it as:
 
-    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A. (2022). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592607
+    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A., Smeets, S. (2023). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592606
 
-See also the [Zenodo page](https://zenodo.org/record/5592607) for exporting the citation to BibTteX and other formats.
+See also the [Zenodo page](https://zenodo.org/record/5592606) for exporting the citation to BibTteX and other formats.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
```

### Comparing `dianna-0.8.0/dianna/__init__.py` & `dianna-0.9.0/dianna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from . import utils
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "DIANNA Team"
 __email__ = "dianna-ai@esciencecenter.nl"
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 def explain_timeseries(model_or_function, timeseries_data, method, labels, **kwargs):
     """Explain timeseries data given a model and a chosen method.
 
     Args:
         model_or_function (callable or str): The function that runs the model to be explained _or_
```

### Comparing `dianna-0.8.0/dianna/methods/kernelshap.py` & `dianna-0.9.0/dianna/methods/kernelshap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import warnings
+import logging
 import numpy as np
 import shap
 import skimage.segmentation
 from dianna import utils
+from dianna._logging_utils import LoggingContext
 
 
 class KERNELSHAPImage:
     """Kernel SHAP implementation based on shap https://github.com/slundberg/shap."""
 
     def __init__(self, axis_labels=None, preprocess_function=None):
         """Kernelshap initializer.
@@ -20,21 +21,15 @@
         self.preprocess_function = preprocess_function
         self.axis_labels = axis_labels if axis_labels is not None else []
         # import here because it's slow
         from onnx_tf.backend import prepare
         self.onnx_to_tf = prepare
 
     @staticmethod
-    def _segment_image(
-        image,
-        n_segments,
-        compactness,
-        sigma,
-        **kwargs
-    ):
+    def _segment_image(image, n_segments, compactness, sigma, **kwargs):
         """Create segmentation to explain by segment, not every pixel.
 
         This could help speed-up the calculation when the input size is very large.
 
         This function segments image using k-means clustering in Color-(x,y,z) space. It uses
         scikit-image.
 
@@ -45,30 +40,28 @@
             sigma (float): Width of Gaussian smoothing kernel
             kwargs: These keyword parameters are passed on
 
         Check keyword arguments for the skimage.segmentation.slic function
         via the following link:
         https://scikit-image.org/docs/dev/api/skimage.segmentation.html#skimage.segmentation.slic
         """
-        image_segments = skimage.segmentation.slic(
-            image=image,
-            n_segments=n_segments,
-            compactness=compactness,
-            sigma=sigma,
-            **kwargs
-        )
+        image_segments = skimage.segmentation.slic(image=image,
+                                                   n_segments=n_segments,
+                                                   compactness=compactness,
+                                                   sigma=sigma,
+                                                   **kwargs)
 
         return image_segments
 
     def explain(
         self,
         model,
         input_data,
         labels,
-        nsamples="auto",
+        nsamples='auto',
         background=None,
         n_segments=100,
         compactness=10.0,
         sigma=0,
         **kwargs,
     ):
         """Run the KernelSHAP explainer.
@@ -116,63 +109,63 @@
         self.background = background
 
         # other keyword arguments for the method segment_image
         slic_kwargs = utils.get_kwargs_applicable_to_function(
             skimage.segmentation.slic, kwargs)
 
         # call the segment method to create segmentation of input image
-        self.image_segments = self._segment_image(
-            self.input_data,
-            n_segments,
-            compactness,
-            sigma,
-            **slic_kwargs
-        )
+        self.image_segments = self._segment_image(self.input_data, n_segments,
+                                                  compactness, sigma,
+                                                  **slic_kwargs)
 
         # call the Kernel SHAP explainer
         explainer = shap.KernelExplainer(
             self._runner, np.zeros((len(self.labels), n_segments)))
 
-        with warnings.catch_warnings():
-            # avoid warnings due to version conflicts
-            warnings.simplefilter("ignore")
-            shap_values = explainer.shap_values(
-                np.ones((len(self.labels), n_segments)), nsamples=nsamples
-            )
+        # Temporarily hide warnings, because shap is very spammy
+        with LoggingContext(level=logging.CRITICAL):
+            shap_values = explainer.shap_values(np.ones(
+                (len(self.labels), n_segments)),
+                                                nsamples=nsamples)
 
         return shap_values, self.image_segments
 
     def _prepare_image_data(self, input_data):
         """Transforms the data to be of the shape and type KernelSHAP expects.
 
         Args:
             input_data (NumPy-compatible array): Data to be explained
         Returns:
             transformed input data
         """
         # automatically determine the location of the channels axis if no axis_labels were provided
-        axis_label_names = self.axis_labels.values() if isinstance(self.axis_labels, dict) else self.axis_labels
+        axis_label_names = self.axis_labels.values() if isinstance(
+            self.axis_labels, dict) else self.axis_labels
         if not axis_label_names:
             channels_axis_index = utils.locate_channels_axis(input_data.shape)
             self.axis_labels = {channels_axis_index: 'channels'}
         elif 'channels' not in axis_label_names:
-            raise ValueError("When providing axis_labels it is required to provide the location"
-                             " of the channels axis")
+            raise ValueError(
+                'When providing axis_labels it is required to provide the location'
+                ' of the channels axis')
 
         input_data = utils.to_xarray(input_data, self.axis_labels)
         # ensure channels axis is last and keep track of where it was so we can move it back
         self.channels_axis_index = input_data.dims.index('channels')
         input_data = utils.move_axis(input_data, 'channels', -1)
 
         return input_data
 
-    def _mask_image(
-        self, features, segmentation, image, background=None,
-        channels_axis_index=2, datatype=np.float32
-    ):
+    def _mask_image(self,
+                    features,
+                    segmentation,
+                    image,
+                    background=None,
+                    channels_axis_index=2,
+                    datatype=np.float32):
         """Define a function that depends on a binary mask representing if an image region is hidden.
 
         Args:
             features (np.ndarray): A matrix of samples (# samples x # features)
                                    on which to explain the model's output.
             segmentation (np.ndarray): Image segmentations generated by
                                        the function _segment_image
@@ -182,17 +175,16 @@
             datatype (np.dtype): Datatype for the returned value
         """
         # check the background color
         if background is None:
             background = image.mean(axis=(0, 1))
 
         # Create an empty 4D array
-        out = np.zeros(
-            (features.shape[0], image.shape[0], image.shape[1], image.shape[2])
-        )
+        out = np.zeros((features.shape[0], image.shape[0], image.shape[1],
+                        image.shape[2]))
 
         for i in range(features.shape[0]):
             out[i] = image
             for j in range(features.shape[1]):
                 if features[i, j] == 0:
                     out[i][segmentation == j, :] = background
 
@@ -205,17 +197,15 @@
     def _runner(self, features):
         """Define a runner/wrapper to load models and values.
 
         Args:
             features (np.ndarray): A matrix of samples (# samples x # features)
                                    on which to explain the model's output.
         """
-        model_input = self._mask_image(features,
-                                       self.image_segments,
-                                       self.input_data,
-                                       self.background,
+        model_input = self._mask_image(features, self.image_segments,
+                                       self.input_data, self.background,
                                        self.channels_axis_index,
-                                       self.input_node_dtype.as_numpy_dtype
-                                       )
+                                       self.input_node_dtype.as_numpy_dtype)
         if self.preprocess_function is not None:
             model_input = self.preprocess_function(model_input)
-        return self.onnx_to_tf(self.onnx_model).run(model_input)[f"{self.output_node}"]
+        return self.onnx_to_tf(
+            self.onnx_model).run(model_input)[f'{self.output_node}']
```

### Comparing `dianna-0.8.0/dianna/methods/lime.py` & `dianna-0.9.0/dianna/methods/lime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 from lime.lime_image import LimeImageExplainer
 from lime.lime_text import LimeTextExplainer
 from dianna import utils
 
+# To Do: remove this import when the method for different input type is splitted
+from dianna.methods.lime_timeseries import LIMETimeseries  # noqa: F401 ignore unused import
+
 
 class LIMEText:
     """Wrapper around the LIME explainer.
 
     See Lime explainer by Marco Tulio Correia Ribeiro
     (https://github.com/marcotcr/lime).
     """
```

### Comparing `dianna-0.8.0/dianna/methods/rise.py` & `dianna-0.9.0/dianna/methods/rise.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/dianna/methods/rise_timeseries.py` & `dianna-0.9.0/dianna/methods/rise_timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     number_of_masks = input_data.shape[0]
     batch_predictions = []
     for i in tqdm(range(0, number_of_masks, batch_size), desc='Explaining'):
         batch_predictions.append(runner(input_data[i:i + batch_size]))
     return np.concatenate(batch_predictions)
 
 
-# Duplicate code from rise.py:
+# TODO: Duplicate code from rise.py:
 def normalize(saliency, n_masks, p_keep):
     """Normalizes salience by number of masks and keep probability."""
     return saliency / n_masks / p_keep
 
 
 class RISETimeseries:
     """RISE implementation for timeseries adapted from the image version of RISE."""
```

### Comparing `dianna-0.8.0/dianna/utils/misc.py` & `dianna-0.9.0/dianna/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,50 +14,60 @@
         preprocess_function: function to be run to preprocess the data
     """
     from dianna.utils.onnx_runner import SimpleModelRunner  # pylint: disable=import-outside-toplevel
 
     if isinstance(model_or_function, Path):
         model_or_function = str(model_or_function)
 
-    if isinstance(model_or_function, (str, Path)):
-        runner = SimpleModelRunner(model_or_function, preprocess_function=preprocess_function)
+    if isinstance(model_or_function, (str, bytes, Path)):
+        runner = SimpleModelRunner(model_or_function,
+                                   preprocess_function=preprocess_function)
     elif callable(model_or_function):
         if preprocess_function is None:
             runner = model_or_function
         else:
+
             def runner(input_data):
                 return model_or_function(preprocess_function(input_data))
     else:
-        raise TypeError("model_or_function argument must be string (path to model) or function")
+        raise TypeError(
+            'model_or_function argument must be string (path to model), '
+            'bytes (serialized onnx model), or function')
     return runner
 
 
 def get_kwargs_applicable_to_function(function, kwargs):
     """Returns a subset of `kwargs` of only arguments and keyword arguments of `function`.
 
     Note that if `function` has a `**kwargs`
     argument, this function should not be necessary (provided the function
     handles `**kwargs` robustly).
     """
-    return {key: value for key, value in kwargs.items()
-            if key in inspect.getfullargspec(function).args}
+    return {
+        key: value
+        for key, value in kwargs.items()
+        if key in inspect.getfullargspec(function).args
+    }
 
 
 def to_xarray(data, axis_labels, required_labels=None):
     """Converts numpy data and axes labels to an xarray object."""
     if isinstance(axis_labels, dict):
         # key = axis index, value = label
         # not all axes have to be present in the input, but we need to provide
         # a name for each axis
         # first ensure negative indices are converted to positive ones
         indices = list(axis_labels.keys())
         for index in indices:
             if index < 0:
                 axis_labels[data.ndim + index] = axis_labels.pop(index)
-        labels = [axis_labels[index] if index in axis_labels else f'dim_{index}' for index in range(data.ndim)]
+        labels = [
+            axis_labels[index] if index in axis_labels else f'dim_{index}'
+            for index in range(data.ndim)
+        ]
     else:
         labels = list(axis_labels)
 
     # check if the required labels are present
     if required_labels is not None:
         for label in required_labels:
             assert label in labels, f'Required axis-label missing: {label}'
@@ -80,15 +90,16 @@
     Returns:
         data with axis in new position
     """
     # find current position of axis
     try:
         pos = data.dims.index(label)
     except ValueError as e:
-        raise ValueError(f"Axis name {label} does not exist in input data") from e
+        raise ValueError(
+            f'Axis name {label} does not exist in input data') from e
 
     # create list of labels with new ordering
     axis_labels = list(data.dims)
     # the new position will be _before_ the given index, so will fail with a negative index
     # convert to a positive index in that case
     if new_position < 0:
         new_position += len(axis_labels)
@@ -138,26 +149,31 @@
     sizes = (1, 3)
     for size in sizes:
         # check if the first or last axis has the given size
         channels_first = data_shape[0] == size
         channels_last = data_shape[-1] == size
         # if both are true, we cannot determine the location of the channels axis
         if channels_first and channels_last:
-            raise ValueError(f"Could not automatically determine the location of the colour channels axis"
-                             f" because both the first and last axis have size {size}. Please provide the"
-                             f" location of the channels axis using the axis_labels argument")
+            raise ValueError(
+                f'Could not automatically determine the location of the colour channels axis'
+                f' because both the first and last axis have size {size}. Please provide the'
+                f' location of the channels axis using the axis_labels argument'
+            )
         # if one of the two is true, we return the corresponding axis location
         if channels_first:
             channels_axis_index = 0
             break
         if channels_last:
             channels_axis_index = -1
             break
 
     # if channels_axis_index is still None, the location could not be determined
     if channels_axis_index is None:
-        raise ValueError("Could not automatically determine location of the colour channels axis."
-                         " Please provide the location of the channels axis using the axis_labels argument")
-    warnings.warn(f"The index of the colour channels axis in the input data was automatically determined"
-                  f" to be {channels_axis_index}. Use the axis_labels to manually specify the index of"
-                  f" the channels axis if this is incorrect.")
+        raise ValueError(
+            'Could not automatically determine location of the colour channels axis.'
+            ' Please provide the location of the channels axis using the axis_labels argument'
+        )
+    warnings.warn(
+        f'The index of the colour channels axis in the input data was automatically determined'
+        f' to be {channels_axis_index}. Use the axis_labels to manually specify the index of'
+        f' the channels axis if this is incorrect.')
     return channels_axis_index
```

### Comparing `dianna-0.8.0/dianna/utils/onnx_runner.py` & `dianna-0.9.0/dianna/utils/onnx_runner.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/dianna/utils/tokenizers.py` & `dianna-0.9.0/dianna/utils/tokenizers.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/dianna/visualization/timeseries.py` & `dianna-0.9.0/dianna/visualization/timeseries.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/dianna.egg-info/PKG-INFO` & `dianna-0.9.0/dianna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dianna
-Version: 0.8.0
+Version: 0.9.0
 Summary: Deep Insight And Neural Network Analysis
 Home-page: https://github.com/dianna-ai/dianna
 Author: DIANNA Team
 Author-email: dianna-ai@esciencecenter.nl
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/dianna-ai/dianna/issues
 Keywords: XAI,machine learning
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: publishing
-Provides-Extra: notebooks
 Provides-Extra: text
+Provides-Extra: dashboard
+Provides-Extra: notebooks
 License-File: LICENSE
 
 <!--
 title: 'DIANNA: Deep Insight And Neural Network Analysis'
 tags:
   - Python
   - explainable AI
@@ -53,18 +55,21 @@
     orcid: 0000-0002-0823-0121
     affiliation: 1
   - name: Laura Ootes^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-2800-8309
     affiliation: 1  
   - name: Pranav Chandramouli^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-7896-2969
-    affiliation: 1    
+    affiliation: 1  
   - name: Aron Jansen^[co-first author] # note this makes a footnote saying 'co-first author'
     orcid: 0000-0002-4764-9347
-    affiliation: 1    
+    affiliation: 1  
+  - name: Stef Smeets^[co-first author] # note this makes a footnote saying 'co-first author'
+    orcid: 0000-0002-5413-9038
+    affiliation: 1  
 affiliations:
  - name: Netherlands eScience Center, Amsterdam, the Netherlands
    index: 1
 -->
 
 [![build](https://github.com/dianna-ai/dianna/actions/workflows/build.yml/badge.svg)](https://github.com/dianna-ai/dianna/actions/workflows/build.yml)
 [![Documentation Status](https://readthedocs.org/projects/dianna/badge/?version=latest)](https://dianna.readthedocs.io/en/latest/?badge=latest)
@@ -78,34 +83,34 @@
 <img align="left" src="https://user-images.githubusercontent.com/55382553/153408200-36c4de2e-7865-4934-956d-09eefd893e6a.png">
 
 # Deep Insight And Neural Network Analysis
 
 DIANNA is a Python package that brings explainable AI (XAI) to your research project. It wraps carefully selected XAI methods in a simple, uniform interface.
 It's built by, with and for (academic) researchers and research software engineers working on machine learning projects.
 
-## Why DIANNA? 
-DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format. 
+## Why DIANNA?
+DIANNA software is addressing needs of both (X)AI researchers and mostly the various domains scientists who are using or will use AI models for their research without being experts in (X)AI. DIANNA is future-proof: one of the very few XAI library supporting the [Open Neural Network Exchange (ONNX)](https://onnx.ai/) format.
 
 After studying the vast XAI landscape we have made choices in the parts of the [XAI Taxonomy](https://doi.org/10.3390/make3030032) on which methods, data modalities and problems types to focus. Our choices, based on the largest usage in scientific literature, are shown graphically in the XAI taxonomy below:
 
 <img src="https://user-images.githubusercontent.com/3244249/196441854-24c8c6b7-2364-4cb3-90b9-1c63e3bdc345.png" alt="XAI_taxonomy" width="60%"/>
 
 The key points of DIANNA:
 
 * Provides an easy-to-use interface for non (X)AI experts
 * Implements well-known XAI methods (LIME, RISE and Kernal SHAP) chosen by systematic and objective evaluation criteria
 * Supports the de-facto standard format for neural network models - ONNX.
 * Includes clear instructions for export/conversions from Tensorflow, Pytorch, Keras and scikit-learn to ONNX.
 * Supports both images and text data modalities. Time series is work in progress, tabular data and even embeddings support is planned.
-* Comes with simple intuitive image and text benchmarks 
-* Easily extendable to other XAI methods 
+* Comes with simple intuitive image and text benchmarks
+* Easily extendable to other XAI methods
 
 For more information on the unique strengths of DIANNA with comparison to other tools, please see the [context landscape](https://dianna.readthedocs.io/en/latest/CONTEXT.html).
 
-## Installation 
+## Installation
 [![workflow pypi badge](https://img.shields.io/pypi/v/dianna.svg?colorB=blue)](https://pypi.python.org/project/dianna/)
 [![supported python versions](https://img.shields.io/pypi/pyversions/dianna)](https://pypi.python.org/project/dianna/)
 
 DIANNA can be installed from PyPI using [pip](https://pip.pypa.io/en/stable/installation/) on any of the supported Python versions (see badge):
 
 ```console
 python3 -m pip install dianna
@@ -132,15 +137,15 @@
 - your trained ONNX model ([convert my pytorch/tensorflow/keras/scikit-learn model to ONNX](https://github.com/dianna-ai/dianna#onnx-models))
 - 1 data item to be explained
 
  You get:
  - a relevance map overlayed over the data item
 
 In the library's documentation, the general usage is explained in [How to use DIANNA](https://dianna.readthedocs.io/en/latest/usage.html)
- 
+
 ### Demo movie
 
 [![Watch the video on YouTube](https://img.youtube.com/vi/u9_c5DJewLU/default.jpg)](https://youtu.be/u9_c5DJewLU)
 
 ### Text example:
 ```python
 model_path = 'your_model.onnx'  # model trained on text
@@ -181,27 +186,27 @@
 ## Datasets
 DIANNA comes with simple datasets. Their main goal is to provide intuitive insight into the working of the XAI methods. They can be used as benchmarks for evaluation and comparison of existing and new XAI methods.
 
 ### Images
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 |Binary MNIST <img width="25" alt="mnist_zero_and_one_half_size" src="https://user-images.githubusercontent.com/3244249/152354583-d7b68902-d402-4098-922b-b1a33b07e3e1.png">| Greyscale images of the digits "1" and "0" - a 2-class subset from the famous [MNIST dataset](http://yann.lecun.com/exdb/mnist/) for handwritten digit classification. |<img width="120" alt="BinaryMNIST" src="https://user-images.githubusercontent.com/3244249/150808267-3d27eae0-78f2-45f8-8569-cb2561f2c2e9.png">| [Binary MNIST dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/MNIST)|
-|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) | 
+|[Simple Geometric (circles and triangles)](https://doi.org/10.5281/zenodo.5012824) <img width="20" alt="Simple Geometric Logo" src="https://user-images.githubusercontent.com/3244249/150808842-d35d741e-294a-4ede-bbe9-58e859483589.png"> | Images of circles and triangles for 2-class geometric shape classificaiton. The shapes of varying size and orientation and the background have varying uniform gray levels.  | <img width="130" alt="SimpleGeometric" src="https://user-images.githubusercontent.com/3244249/150808125-e1576237-47fa-4e51-b01e-180904b7c7f6.png">| [Simple geometric shapes dataset generation](https://github.com/dianna-ai/dianna-exploration/tree/main/example_data/dataset_preparation/geometric_shapes) |
 |[Simple Scientific (LeafSnap30)](https://zenodo.org/record/5061353/)<img width="20" alt="LeafSnap30 Logo" src="https://user-images.githubusercontent.com/3244249/150815639-2da560d4-8b26-4eeb-9ab4-dabf221a264a.png"> | Color images of tree leaves - a 30-class post-processed subset from the LeafSnap dataset for automatic identification of North American tree species.|<img width="600" alt="LeafSnap" src="https://user-images.githubusercontent.com/3244249/150804246-f714e517-641d-48b2-af26-2f04166870d6.png">| [LeafSnap30 dataset generation](https://github.com/dianna-ai/dianna-exploration/blob/main/example_data/dataset_preparation/LeafSnap/)|
 
 ### Text
 |Dataset|Description|Examples|Generation|
 |:-----|:----|:---|:----|
 | [Stanford sentiment treebank](https://nlp.stanford.edu/sentiment/index.html)<img width="20" alt="nlp-logo_half_size" src="https://user-images.githubusercontent.com/3244249/152355020-908c04f3-aa99-489d-b87a-7e6b1f586118.png">|Dataset for predicting the sentiment, positive or negative, of movie reviews. | _This movie was actually neither that funny, nor super witty._|[Sentiment treebank](https://nlp.stanford.edu/sentiment/treebank.html)|
 
 ## ONNX models
 <!-- TODO: Add all links, see issue https://github.com/dianna-ai/dianna/issues/135 -->
 
 **We work with ONNX!** ONNX is a great unified neural network standard which can be used to boost reproducible science. Using ONNX for your model also gives you a boost in performance! In case your models are still in another popular DNN (deep neural network) format, here are some simple recipes to convert them:
-* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://pytorch-lightning.readthedocs.io/en/latest/api/pytorch_lightning.core.LightningModule.html#pytorch_lightning.core.LightningModule) to export pytorch-lightning models to onnx.
+* [pytorch and pytorch-lightning](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/pytorch2onnx.ipynb) - use the built-in [`torch.onnx.export`](https://pytorch.org/docs/stable/onnx.html) function to convert pytorch models to onnx, or call the built-in [`to_onnx`](https://pytorch-lightning.readthedocs.io/en/latest/deploy/production_advanced.html) function on your [`LightningModule`](https://lightning.ai/docs/pytorch/stable/api/lightning.pytorch.core.LightningModule.html) to export pytorch-lightning models to onnx.
 * [tensorflow](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/tensorflow2onnx.ipynb) - use the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package to convert tensorflow models to onnx.
 * [keras](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/keras2onnx.ipynb) - same as the conversion from tensorflow to onnx, the [`tf2onnx`](https://github.com/onnx/tensorflow-onnx) package also supports keras.
 * [scikit-learn](https://github.com/dianna-ai/dianna/blob/main/tutorials/conversion_onnx/skl2onnx.ipynb) - use the [`skl2onnx`](https://github.com/onnx/sklearn-onnx) package to scikit-learn models to onnx.
 
 More converters with examples and tutorials can be found on the [ONNX tutorial page](https://github.com/onnx/tutorials).
 
 And here are links to notebooks showing how we created our models on the benchmark datasets:
@@ -232,30 +237,30 @@
 |Embedding|coming soon|coming soon|coming soon|
 |Graphs |planned|planned|planned |
 |Tabular||||
 
 
 [LRP](https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0130140&type=printable) and [PatternAttribution](https://arxiv.org/pdf/1705.05598.pdf) also feature in the top 5 of our thoroughly evaluated XAI methods using objective criteria (details in coming blog-post). **Contributing by adding these and more (new) post-hoc explainability methods on ONNX models is very welcome!**
 
-## Reference documentation 
+## Reference documentation
 
 For detailed information on using specific DIANNA functions, please visit the [documentation page hosted at Readthedocs](https://dianna.readthedocs.io/en/latest).
 
 ## Contributing
 
 If you want to contribute to the development of DIANNA,
 have a look at the [contribution guidelines](https://dianna.readthedocs.io/en/latest/CONTRIBUTING.html).
 See our [developer documentation](docs/developer_info.rst) for information on developer installation, running tests, generating documentation, versioning and making a release.
 
-## How to cite us 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592607.svg)](https://zenodo.org/record/5592607)
+## How to cite us
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592606.svg)](https://zenodo.org/record/5592606)
 [![RSD](https://img.shields.io/badge/rsd-dianna-00a3e3.svg)](https://www.research-software.nl/software/dianna)
 
 If you use this package for your scientific work, please consider citing it as:
 
-    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A. (2022). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592607
+    Ranguelova, E., Bos, P., Liu, Y., Meijer, C., Oostrum, L., Crocioni, G., Ootes, L., Chandramouli, P., Jansen, A., Smeets, S. (2023). dianna (*[VERSION YOU USED]*). Zenodo. https://zenodo.org/record/5592606
 
-See also the [Zenodo page](https://zenodo.org/record/5592607) for exporting the citation to BibTteX and other formats.
+See also the [Zenodo page](https://zenodo.org/record/5592606) for exporting the citation to BibTteX and other formats.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
```

### Comparing `dianna-0.8.0/dianna.egg-info/SOURCES.txt` & `dianna-0.9.0/dianna.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 dianna/__init__.py
+dianna/_logging_utils.py
+dianna/cli.py
 dianna.egg-info/PKG-INFO
 dianna.egg-info/SOURCES.txt
 dianna.egg-info/dependency_links.txt
+dianna.egg-info/entry_points.txt
 dianna.egg-info/not-zip-safe
 dianna.egg-info/requires.txt
 dianna.egg-info/top_level.txt
 dianna/methods/kernelshap.py
 dianna/methods/lime.py
+dianna/methods/lime_timeseries.py
 dianna/methods/rise.py
 dianna/methods/rise_timeseries.py
 dianna/utils/__init__.py
 dianna/utils/maskers.py
 dianna/utils/misc.py
 dianna/utils/onnx_runner.py
 dianna/utils/tokenizers.py
```

### Comparing `dianna-0.8.0/pyproject.toml` & `dianna-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_common_usage.py` & `dianna-0.9.0/tests/test_common_usage.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_kernelshap.py` & `dianna-0.9.0/tests/test_kernelshap.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_lime.py` & `dianna-0.9.0/tests/test_lime.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_onnx_runner.py` & `dianna-0.9.0/tests/test_onnx_runner.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_rise.py` & `dianna-0.9.0/tests/test_rise.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_text_visualization.py` & `dianna-0.9.0/tests/test_text_visualization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,92 @@
 import os
+import re
 import shutil
 import unittest
 from pathlib import Path
-import spacy
-from dianna.utils.tokenizers import SpacyTokenizer
 from dianna.visualization.text import highlight_text
 
 
-spacy.cli.download('en_core_web_sm')
+tokenizer = re.compile(r'(\w+|\S)')
 
 
 class TextExample:
     """Text and explanation for running visualizing tests."""
     original_text = 'Doloremque aliquam totam ut. Aspernatur repellendus autem quia deleniti. Natus accusamus ' \
                     'doloribus et in quam officiis veniam et. '
-    tokenizer = SpacyTokenizer()
-    tokens = tokenizer.tokenize(original_text)
-    explanation = [
-                    ('aliquam', 1, 0.6450221),
-                    ('et', 19, 0.63976675),
-                    ('in', 15, 0.6397511),
-                    ('Aspernatur', 5, 0.6329795),
-                    ('totam', 2, 0.6242337),
-                    ('quia', 8, 0.61881626),
-                    ('quam', 16, 0.6173148),
-                    ('Natus', 11, 0.60527676),
-                    ('ut', 3, 0.60203224)
-                    ]
+
+    tokens = tokenizer.findall(original_text)
+
+    explanation = [('aliquam', 1, 0.6450221), ('et', 19, 0.63976675),
+                   ('in', 15, 0.6397511), ('Aspernatur', 5, 0.6329795),
+                   ('totam', 2, 0.6242337), ('quia', 8, 0.61881626),
+                   ('quam', 16, 0.6173148), ('Natus', 11, 0.60527676),
+                   ('ut', 3, 0.60203224)]
 
 
 class TextExampleWithExpectedHtml:
     """Short text and explanation and its expected html output after visualizing."""
-    expected_html = '<html><body><span style="background:rgba(255, 0, 0, 0.59)">Such</span> ' \
-                    '<span style="background:rgba(255, 0, 0, 0.62)">a</span> ' \
-                    '<span style="background:rgba(255, 0, 0, 0.80)">bad</span> ' \
-                    '<span style="background:rgba(255, 0, 0, 0.63)">movie</span> ' \
-                    '<span style="background:rgba(128, 128, 128, 0.3)">.</span></body></html>\n'
+    expected_html = (
+        '<mark style="background-color: hsl(0, 100%, 63%, 0.8); line-height:1.75">Such</mark> '
+        '<mark style="background-color: hsl(0, 100%, 62%, 0.8); line-height:1.75">a</mark> '
+        '<mark style="background-color: hsl(0, 100%, 50%, 0.8); line-height:1.75">bad</mark> '
+        '<mark style="background-color: hsl(0, 100%, 61%, 0.8); line-height:1.75">movie</mark> '
+        '<mark style="background-color: hsl(0, 0%, 75%, 0.8); line-height:1.75">.</mark>\n'
+    )
 
     original_text = 'Such a bad movie.'
-    tokenizer = SpacyTokenizer()
-    tokens = tokenizer.tokenize(original_text)
-    explanation = [
-                    ('bad', 2, 0.9959058),
-                    ('movie', 3, 0.78263557),
-                    ('a', 1, 0.7753202),
-                    ('Such', 0, 0.73788315)
-                    ]
+
+    tokens = tokenizer.findall(original_text)
+
+    explanation = [('bad', 2, 0.9959058), ('movie', 3, 0.78263557),
+                   ('a', 1, 0.7753202), ('Such', 0, 0.73788315)]
 
 
 class TextVisualizationTestCase(unittest.TestCase):
     """Suite of tests for visualizing text given text and explanation data."""
     temp_folder = 'temp_text_visualization_test'
     html_file_path = str(Path(temp_folder) / 'output.html')
 
     def test_text_visualization_html_output_exists(self):
         """Test if any output is generated at all."""
-        highlight_text(TextExample.explanation, TextExample.tokens,
+        highlight_text(TextExample.explanation,
+                       TextExample.tokens,
                        output_html_filename=self.html_file_path)
 
         assert Path(self.html_file_path).exists()
 
     def test_text_visualization_html_output_contains_text(self):
         """Test if all words in the input are present in the output html."""
-        highlight_text(TextExample.explanation, TextExample.tokens,
+        highlight_text(TextExample.explanation,
+                       TextExample.tokens,
                        output_html_filename=self.html_file_path)
 
         assert Path(self.html_file_path).exists()
         with open(self.html_file_path, encoding='utf-8') as result_file:
             result = result_file.read()
         for word in TextExample.tokens:
             assert word in result
 
     def test_text_visualization_html_output_is_correct(self):
         """Test if exact html output of visualization is correct."""
-        highlight_text(TextExampleWithExpectedHtml.explanation, TextExampleWithExpectedHtml.tokens,
+        highlight_text(TextExampleWithExpectedHtml.explanation,
+                       TextExampleWithExpectedHtml.tokens,
                        output_html_filename=self.html_file_path)
 
         assert Path(self.html_file_path).exists()
 
         with open(self.html_file_path, encoding='utf-8') as result_file:
             result = result_file.read()
+
         assert result == TextExampleWithExpectedHtml.expected_html
 
     def test_text_visualization_show_plot(self):
         """Test if it runs while showing the plot."""
-        highlight_text(TextExample.explanation, TextExample.tokens,
+        highlight_text(TextExample.explanation,
+                       TextExample.tokens,
                        show_plot=True)
 
     def setUp(self) -> None:
         """Setup."""
         os.mkdir(self.temp_folder)
 
     def tearDown(self) -> None:
```

### Comparing `dianna-0.8.0/tests/test_visualization.py` & `dianna-0.9.0/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `dianna-0.8.0/tests/test_xarray.py` & `dianna-0.9.0/tests/test_xarray.py`

 * *Files identical despite different names*

