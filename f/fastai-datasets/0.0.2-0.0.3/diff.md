# Comparing `tmp/fastai-datasets-0.0.2.tar.gz` & `tmp/fastai-datasets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.2.tar", last modified: Tue Apr 18 07:51:35 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.3.tar", last modified: Tue Apr 25 14:48:13 2023, max compression
```

## Comparing `fastai-datasets-0.0.2.tar` & `fastai-datasets-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.308423 fastai-datasets-0.0.2/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5790 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4144 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       21 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12364 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.2/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3354 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5806 2023-04-18 07:11:00.000000 fastai-datasets-0.0.2/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2231 2023-04-16 20:50:00.000000 fastai-datasets-0.0.2/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-18 07:51:35.304423 fastai-datasets-0.0.2/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5790 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-18 07:51:35.000000 fastai-datasets-0.0.2/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-18 07:51:29.000000 fastai-datasets-0.0.2/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-18 07:51:35.308423 fastai-datasets-0.0.2/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.2/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.279806 fastai-datasets-0.0.3/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3894 2023-04-25 14:46:07.000000 fastai-datasets-0.0.3/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.3/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3802 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5841 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1894 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-25 14:48:02.000000 fastai-datasets-0.0.3/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-25 14:48:13.279806 fastai-datasets-0.0.3/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/setup.py
```

### Comparing `fastai-datasets-0.0.2/LICENSE` & `fastai-datasets-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/PKG-INFO` & `fastai-datasets-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.2
+Version: 0.0.3
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
-Description: # fastai-datasets
+Description: fastai-datasets
+        ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         # Docs
         
         See https://irad-zehavi.github.io/fastai-datasets/
         
@@ -34,86 +35,79 @@
         ### Easily load a dataset
         
         ``` python
         mnist = MNIST()
         mnist.dls().show_batch()
         ```
         
-        <img src="index_files/figure-commonmark/cell-3-output-1.png"
-        class="quarto-discovered-preview-image" />
+        ![](index_files/figure-commonmark/cell-3-output-1.png)
         
         ### Show the class distribution
         
         ``` python
         mnist.plot_class_distribution()
         ```
         
-            Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+            <div>
+              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+            </div>
+            
         
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-            Class map: scanning targets:   0%|          | 0/10000 [00:00<?, ?it/s]
-        
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-        ![](index_files/figure-commonmark/cell-4-output-5.png)
+        ![](index_files/figure-commonmark/cell-4-output-2.png)
         
         ### Sample a subset
         
         Whole datasets:
         
         ``` python
         mnist
         ```
         
-            [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]
-            (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+            [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]
+            (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]]
         
         Subset:
         
         ``` python
         mnist.random_sub_dsets(1000)
         ```
         
-            [(#874) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(4))...]
-            (#126) [(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(6)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+            [(#865) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(1))...]
+            (#135) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(9))...]]
         
         ### Construct a subset based on classes
         
         ``` python
         cifar10 = CIFAR10()
         dig_frog_bird = cifar10.by_target['dog'] + cifar10.by_target['frog'] + cifar10.by_target['bird']
         dig_frog_bird.dls().show_batch()
         ```
         
-            Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+            <div>
+              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+            </div>
+            
         
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-        ![](index_files/figure-commonmark/cell-7-output-3.png)
+        ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         ### Construct a dataset of similarity pairs
         
         ``` python
         Pairs(cifar10, .01).dls().show_batch()
         ```
         
-            Class map: scanning targets: 0it [00:00, ?it/s]
-        
-            Generating positive pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-        
-            Generating negative pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-        
-            Class map: scanning targets: 0it [00:00, ?it/s]
-        
-            Generating positive pairs:   0%|          | 0/50 [00:00<?, ?it/s]
-        
-            Generating negative pairs:   0%|          | 0/50 [00:00<?, ?it/s]
+            <div>
+              <progress value='50' class='' max='50' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [50/50 00:00&lt;00:00 Generating negative pairs]
+            </div>
+            
         
-        ![](index_files/figure-commonmark/cell-8-output-7.png)
+        ![](index_files/figure-commonmark/cell-8-output-2.png)
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `fastai-datasets-0.0.2/README.md` & `fastai-datasets-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# fastai-datasets
+fastai-datasets
+================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 # Docs
 
 See https://irad-zehavi.github.io/fastai-datasets/
 
@@ -26,79 +27,72 @@
 ### Easily load a dataset
 
 ``` python
 mnist = MNIST()
 mnist.dls().show_batch()
 ```
 
-<img src="index_files/figure-commonmark/cell-3-output-1.png"
-class="quarto-discovered-preview-image" />
+![](index_files/figure-commonmark/cell-3-output-1.png)
 
 ### Show the class distribution
 
 ``` python
 mnist.plot_class_distribution()
 ```
 
-    Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+    <div>
+      <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+      100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+    </div>
+    
 
-    Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-
-    Class map: scanning targets:   0%|          | 0/10000 [00:00<?, ?it/s]
-
-    Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-
-![](index_files/figure-commonmark/cell-4-output-5.png)
+![](index_files/figure-commonmark/cell-4-output-2.png)
 
 ### Sample a subset
 
 Whole datasets:
 
 ``` python
 mnist
 ```
 
-    [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]
-    (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+    [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]
+    (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]]
 
 Subset:
 
 ``` python
 mnist.random_sub_dsets(1000)
 ```
 
-    [(#874) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(4))...]
-    (#126) [(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(6)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+    [(#865) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(1))...]
+    (#135) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(9))...]]
 
 ### Construct a subset based on classes
 
 ``` python
 cifar10 = CIFAR10()
 dig_frog_bird = cifar10.by_target['dog'] + cifar10.by_target['frog'] + cifar10.by_target['bird']
 dig_frog_bird.dls().show_batch()
 ```
 
-    Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+    <div>
+      <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+      100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+    </div>
+    
 
-    Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-
-![](index_files/figure-commonmark/cell-7-output-3.png)
+![](index_files/figure-commonmark/cell-7-output-2.png)
 
 ### Construct a dataset of similarity pairs
 
 ``` python
 Pairs(cifar10, .01).dls().show_batch()
 ```
 
-    Class map: scanning targets: 0it [00:00, ?it/s]
-
-    Generating positive pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-
-    Generating negative pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-
-    Class map: scanning targets: 0it [00:00, ?it/s]
-
-    Generating positive pairs:   0%|          | 0/50 [00:00<?, ?it/s]
-
-    Generating negative pairs:   0%|          | 0/50 [00:00<?, ?it/s]
+    <div>
+      <progress value='50' class='' max='50' style='width:300px; height:20px; vertical-align: middle;'></progress>
+      100.00% [50/50 00:00&lt;00:00 Generating negative pairs]
+    </div>
+    
 
-![](index_files/figure-commonmark/cell-8-output-7.png)
+![](index_files/figure-commonmark/cell-8-output-2.png)
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.3/fastai_datasets/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
                                        'fastai_datasets.pairs.Sameness': ('pairs.html#sameness', 'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs.Sameness.__init__': ( 'pairs.html#sameness.__init__',
                                                                                     'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs.Sameness.encodes': ( 'pairs.html#sameness.encodes',
                                                                                    'fastai_datasets/pairs.py'),
                                        'fastai_datasets.pairs._pairs_for_split': ( 'pairs.html#_pairs_for_split',
                                                                                    'fastai_datasets/pairs.py'),
-                                       'fastai_datasets.pairs.show_batch': ('pairs.html#show_batch', 'fastai_datasets/pairs.py')},
+                                       'fastai_datasets.pairs.show_batch': ('pairs.html#show_batch', 'fastai_datasets/pairs.py'),
+                                       'fastai_datasets.pairs.show_results': ('pairs.html#show_results', 'fastai_datasets/pairs.py')},
             'fastai_datasets.patches': { 'fastai_datasets.patches.Datasets.__add__': ( 'Core/patches.html#datasets.__add__',
                                                                                        'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.__repr__': ( 'Core/patches.html#datasets.__repr__',
                                                                                         'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.__sub__': ( 'Core/patches.html#datasets.__sub__',
                                                                                        'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches.Datasets.by_target': ( 'Core/patches.html#datasets.by_target',
@@ -96,11 +97,9 @@
                                                                                                           'transform)].__eq__',
                                                                                                           'fastai_datasets/patches.py'),
                                          'fastai_datasets.patches._dl_args': ('Core/patches.html#_dl_args', 'fastai_datasets/patches.py')},
             'fastai_datasets.pfr': { 'fastai_datasets.pfr.PinterestFaces': ( 'Facial Recognition/pfr.html#pinterestfaces',
                                                                              'fastai_datasets/pfr.py')},
             'fastai_datasets.utils': { 'fastai_datasets.utils.data_path': ('Core/utils.html#data_path', 'fastai_datasets/utils.py'),
                                        'fastai_datasets.utils.fetch_file': ('Core/utils.html#fetch_file', 'fastai_datasets/utils.py'),
-                                       'fastai_datasets.utils.fix_notebook_widgets': ( 'Core/utils.html#fix_notebook_widgets',
-                                                                                       'fastai_datasets/utils.py'),
                                        'fastai_datasets.utils.mtcnn_aligned': ('Core/utils.html#mtcnn_aligned', 'fastai_datasets/utils.py'),
                                        'fastai_datasets.utils.return_list': ('Core/utils.html#return_list', 'fastai_datasets/utils.py')}}}
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets/imagenette.py` & `fastai-datasets-0.0.3/fastai_datasets/imagenette.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/fastai_datasets/lfw.py` & `fastai-datasets-0.0.3/fastai_datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/fastai_datasets/mnist.py` & `fastai-datasets-0.0.3/fastai_datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/fastai_datasets/pairs.py` & `fastai-datasets-0.0.3/fastai_datasets/pairs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __all__ = ['ImagePair', 'Sameness', 'Pairs']
 
 # %% ../nbs/pairs.ipynb 2
 import random
 from typing import NamedTuple, Union
 
 from fastai.vision.all import *
-from tqdm.auto import trange, tqdm
+from fastprogress.fastprogress import *
 
 import fastai_datasets.patches
 from .utils import *
 
 # %% ../nbs/pairs.ipynb 3
 class ImagePair(fastuple):
     """Adds showing functionality to fastai's `fastuple`"""
@@ -36,35 +36,41 @@
 @typedispatch
 def show_batch(x:ImagePair, y, samples, ctxs=None, max_n=9, nrows=None, ncols=3, figsize=None, **kwargs):
     if figsize is None: figsize = (ncols*4, max_n//ncols * 2)
     if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
     ctxs = show_batch[TensorImage](x, y, samples, ctxs=ctxs, max_n=max_n, **kwargs)
     return ctxs
 
+@typedispatch
+def show_results(x:ImagePair, y:TensorCategory, samples, outs, ctxs=None, max_n=9, nrows=None, ncols=3, figsize=None, **kwargs):
+    if figsize is None: figsize = (ncols*4, max_n//ncols * 2.5)
+    if ctxs is None: ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
+    ctxs = show_results[TensorImage, TensorCategory](x, y, samples, outs, ctxs=ctxs, max_n=max_n, **kwargs)
+
 # %% ../nbs/pairs.ipynb 6
 def _pairs_for_split(singles: DataLoaders, split_idx: int, factor: int):
     assert singles.n_inp == 1
 
     indices = L(range_of(singles))[singles.splits[split_idx]]
     num = int(len(indices) * factor)
 
     class_map = defaultdict(list)
-    for i, c in tqdm(zip(indices, singles.i2t.subset(split_idx)), desc='Class map: scanning targets'):
+    for i, c in progress_bar(indices.zipwith(singles.i2t.subset(split_idx)), comment='Class map: scanning targets'):
         class_map[singles.vocab[c]].append(i)
 
     @return_list
     def _positive_pairs():
         multi_item_class_map = {k: v for k, v in class_map.items() if len(v)>1}
-        for _ in trange(num//2, desc=f'Generating positive pairs'):
+        for _ in progress_bar(range(num//2), comment=f'Generating positive pairs'):
             c, idxs = random.choice(list(multi_item_class_map.items()))
             yield tuple(random.sample(idxs, 2))
 
     @return_list
     def _negative_pairs():
-        for _ in trange(num//2, desc=f'Generating negative pairs'):
+        for _ in progress_bar(range(num//2), comment=f'Generating negative pairs'):
             (c1, idxs1), (c2, idxs2) = random.sample(list(class_map.items()), 2)
             yield (random.choice(idxs1), random.choice(idxs2))
 
     return _positive_pairs() + _negative_pairs()
 
 
 def Pairs(singles: Datasets,  # Used to construct pairs
@@ -82,10 +88,9 @@
 
     return Datasets(
         [L(x) for items in pairs_for_splits for x in items],
         tfms=[
             lambda o: tuple_type(singles.tls[0][o]),
             [lambda o: bool(singles.i2t[o[0]] == singles.i2t[o[1]]), Sameness()]
         ],
-        splits=splits,
-        do_setup=False,
+        splits=splits
     )
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets/patches.py` & `fastai-datasets-0.0.3/fastai_datasets/patches.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # %% ../nbs/Core/patches.ipynb 2
 import random
 from collections import defaultdict
 from typing import List, Dict, Sequence, Union
 from functools import partial
 
-from tqdm.auto import tqdm
+from fastprogress.fastprogress import *
 from fastai.vision.all import *
 
 # %% ../nbs/Core/patches.ipynb 5
 @patch
 def sublist(self: TfmdLists, indices: Iterable[int]) -> TfmdLists:
     """a sublist that maintains laziness"""
     sub = self.new_empty()
@@ -94,18 +94,18 @@
     assert self.n_inp == len(self.tls) - 1
     return self.tls[-1]
 
 # %% ../nbs/Core/patches.ipynb 35
 @patch(as_prop=True)
 def by_target(self: Datasets) -> Dict[int, Datasets]:
     if not hasattr(self, '_by_target'):
-        targets = [int(t) for t in tqdm(self.i2t, desc='Class map: scanning targets')]
+        targets = [int(t) for t in progress_bar(self.i2t, comment='Class map: scanning targets')]
         class_map = groupby(enumerate(targets), key=1, val=0)
         self._by_target = {self.vocab[c]: self.sub_dsets(indices)
-                           for c, indices in tqdm(class_map.items(), desc='Class map: partitioning')}
+                           for c, indices in progress_bar(class_map.items(), comment='Class map: partitioning')}
     return self._by_target
 
 
 # %% ../nbs/Core/patches.ipynb 37
 import matplotlib.pyplot as plt
 
 @patch()
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets/pfr.py` & `fastai-datasets-0.0.3/fastai_datasets/pfr.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/fastai_datasets/utils.py` & `fastai-datasets-0.0.3/fastai_datasets/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/Core/utils.ipynb.
 
 # %% auto 0
-__all__ = ['data_path', 'fetch_file', 'return_list', 'mtcnn_aligned', 'fix_notebook_widgets']
+__all__ = ['data_path', 'fetch_file', 'return_list', 'mtcnn_aligned']
 
 # %% ../nbs/Core/utils.ipynb 3
 from fastcore.all import *
 from fastdownload import *
 from fastai.vision.all import *
 
 # %% ../nbs/Core/utils.ipynb 4
@@ -28,15 +28,15 @@
 based on https://github.com/timesler/facenet-pytorch/blob/master/examples/lfw_evaluate.ipynb
 """
 import os
 
 import PIL
 import torch
 from facenet_pytorch import MTCNN, training
-from tqdm.autonotebook import tqdm
+from fastprogress.fastprogress import *
 
 
 def mtcnn_aligned(path: Path,  # path to unaligned images
                   force=False,  # compute MTCNN alignment even if aligned images exist
                   batched=True
                   ) -> Path:   # path to aligned images
     """Uses MTCNN to align and extract faces"""
@@ -54,21 +54,12 @@
     loader = torch.utils.data.DataLoader(
         Datasets(get_image_files(path), [PIL.Image.open, noop]),
         num_workers=0 if os.name == 'nt' else 8,
         batch_size=64 if batched else 1,
         collate_fn=training.collate_pil
     )
 
-    for imgs, paths in tqdm(loader, desc='MTCNN'):
+    for imgs, paths in progress_bar(loader, comment='MTCNN'):
         output_paths = [mtcnn_path/p.relative_to(path) for p in paths]
         mtcnn(imgs, save_path=output_paths)
 
     return mtcnn_path
-
-# %% ../nbs/Core/utils.ipynb 8
-def fix_notebook_widgets():
-    """Taken from https://github.com/microsoft/vscode-jupyter/issues/13163"""
-    from IPython.display import clear_output, DisplayHandle
-    def update_patch(self, obj):
-        clear_output(wait=True)
-        self.display(obj)
-    DisplayHandle.update = update_patch
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets.egg-info/PKG-INFO` & `fastai-datasets-0.0.3/fastai_datasets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.2
+Version: 0.0.3
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
-Description: # fastai-datasets
+Description: fastai-datasets
+        ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         # Docs
         
         See https://irad-zehavi.github.io/fastai-datasets/
         
@@ -34,86 +35,79 @@
         ### Easily load a dataset
         
         ``` python
         mnist = MNIST()
         mnist.dls().show_batch()
         ```
         
-        <img src="index_files/figure-commonmark/cell-3-output-1.png"
-        class="quarto-discovered-preview-image" />
+        ![](index_files/figure-commonmark/cell-3-output-1.png)
         
         ### Show the class distribution
         
         ``` python
         mnist.plot_class_distribution()
         ```
         
-            Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+            <div>
+              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+            </div>
+            
         
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-            Class map: scanning targets:   0%|          | 0/10000 [00:00<?, ?it/s]
-        
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-        ![](index_files/figure-commonmark/cell-4-output-5.png)
+        ![](index_files/figure-commonmark/cell-4-output-2.png)
         
         ### Sample a subset
         
         Whole datasets:
         
         ``` python
         mnist
         ```
         
-            [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]
-            (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+            [(#60000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]
+            (#10000) [(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7))...]]
         
         Subset:
         
         ``` python
         mnist.random_sub_dsets(1000)
         ```
         
-            [(#874) [(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(4))...]
-            (#126) [(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(2)),(PILImage mode=RGB size=28x28, TensorCategory(7)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(6)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(0))...]]
+            [(#865) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(8)),(PILImage mode=RGB size=28x28, TensorCategory(1))...]
+            (#135) [(PILImage mode=RGB size=28x28, TensorCategory(3)),(PILImage mode=RGB size=28x28, TensorCategory(9)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(5)),(PILImage mode=RGB size=28x28, TensorCategory(0)),(PILImage mode=RGB size=28x28, TensorCategory(4)),(PILImage mode=RGB size=28x28, TensorCategory(1)),(PILImage mode=RGB size=28x28, TensorCategory(9))...]]
         
         ### Construct a subset based on classes
         
         ``` python
         cifar10 = CIFAR10()
         dig_frog_bird = cifar10.by_target['dog'] + cifar10.by_target['frog'] + cifar10.by_target['bird']
         dig_frog_bird.dls().show_batch()
         ```
         
-            Class map: scanning targets:   0%|          | 0/60000 [00:00<?, ?it/s]
+            <div>
+              <progress value='10' class='' max='10' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [10/10 00:00&lt;00:00 Class map: partitioning]
+            </div>
+            
         
-            Class map: partitioning:   0%|          | 0/10 [00:00<?, ?it/s]
-        
-        ![](index_files/figure-commonmark/cell-7-output-3.png)
+        ![](index_files/figure-commonmark/cell-7-output-2.png)
         
         ### Construct a dataset of similarity pairs
         
         ``` python
         Pairs(cifar10, .01).dls().show_batch()
         ```
         
-            Class map: scanning targets: 0it [00:00, ?it/s]
-        
-            Generating positive pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-        
-            Generating negative pairs:   0%|          | 0/250 [00:00<?, ?it/s]
-        
-            Class map: scanning targets: 0it [00:00, ?it/s]
-        
-            Generating positive pairs:   0%|          | 0/50 [00:00<?, ?it/s]
-        
-            Generating negative pairs:   0%|          | 0/50 [00:00<?, ?it/s]
+            <div>
+              <progress value='50' class='' max='50' style='width:300px; height:20px; vertical-align: middle;'></progress>
+              100.00% [50/50 00:00&lt;00:00 Generating negative pairs]
+            </div>
+            
         
-        ![](index_files/figure-commonmark/cell-8-output-7.png)
+        ![](index_files/figure-commonmark/cell-8-output-2.png)
         
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `fastai-datasets-0.0.2/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.3/fastai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.2/settings.ini` & `fastai-datasets-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
```

### Comparing `fastai-datasets-0.0.2/setup.py` & `fastai-datasets-0.0.3/setup.py`

 * *Files identical despite different names*

