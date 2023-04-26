# Comparing `tmp/kennard_stone-2.0.0.tar.gz` & `tmp/kennard_stone-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kennard_stone-2.0.0.tar", last modified: Sat Apr 22 05:18:59 2023, max compression
+gzip compressed data, was "kennard_stone-2.0.1.tar", last modified: Tue Apr 25 14:21:56 2023, max compression
```

## Comparing `kennard_stone-2.0.0.tar` & `kennard_stone-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.646309 kennard_stone-2.0.0/
--rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.0.0/LICENSE
--rw-r--r--   0 yu9824     (501) staff       (20)       71 2022-04-23 07:40:26.000000 kennard_stone-2.0.0/MANIFEST.in
--rw-r--r--   0 yu9824     (501) staff       (20)     5461 2023-04-22 05:18:59.646162 kennard_stone-2.0.0/PKG-INFO
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.644975 kennard_stone-2.0.0/kennard_stone/
--rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-04-22 05:15:52.000000 kennard_stone-2.0.0/kennard_stone/__init__.py
--rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-20 15:35:56.000000 kennard_stone-2.0.0/kennard_stone/_deprecated.py
--rw-r--r--   0 yu9824     (501) staff       (20)     9586 2023-04-22 05:10:32.000000 kennard_stone-2.0.0/kennard_stone/kennard_stone.py
-drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-22 05:18:59.645939 kennard_stone-2.0.0/kennard_stone.egg-info/
--rw-r--r--   0 yu9824     (501) staff       (20)     5461 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/PKG-INFO
--rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/SOURCES.txt
--rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/dependency_links.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/requires.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-04-22 05:18:59.000000 kennard_stone-2.0.0/kennard_stone.egg-info/top_level.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-20 13:09:17.000000 kennard_stone-2.0.0/requirements.txt
--rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-04-22 05:18:59.646801 kennard_stone-2.0.0/setup.cfg
--rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 04:08:08.000000 kennard_stone-2.0.0/setup.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.864410 kennard_stone-2.0.1/
+-rw-r--r--   0 yu9824     (501) staff       (20)     1063 2022-04-23 07:40:26.000000 kennard_stone-2.0.1/LICENSE
+-rw-r--r--   0 yu9824     (501) staff       (20)       71 2023-04-22 06:08:03.000000 kennard_stone-2.0.1/MANIFEST.in
+-rw-r--r--   0 yu9824     (501) staff       (20)     5431 2023-04-25 14:21:56.864278 kennard_stone-2.0.1/PKG-INFO
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.863433 kennard_stone-2.0.1/kennard_stone/
+-rw-r--r--   0 yu9824     (501) staff       (20)      360 2023-04-25 14:15:51.000000 kennard_stone-2.0.1/kennard_stone/__init__.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     3160 2023-04-22 05:20:01.000000 kennard_stone-2.0.1/kennard_stone/_deprecated.py
+-rw-r--r--   0 yu9824     (501) staff       (20)     9616 2023-04-25 13:35:46.000000 kennard_stone-2.0.1/kennard_stone/kennard_stone.py
+drwxr-xr-x   0 yu9824     (501) staff       (20)        0 2023-04-25 14:21:56.864099 kennard_stone-2.0.1/kennard_stone.egg-info/
+-rw-r--r--   0 yu9824     (501) staff       (20)     5431 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/PKG-INFO
+-rw-r--r--   0 yu9824     (501) staff       (20)      315 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/SOURCES.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)        1 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/dependency_links.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/requires.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       14 2023-04-25 14:21:56.000000 kennard_stone-2.0.1/kennard_stone.egg-info/top_level.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       19 2023-04-22 05:20:01.000000 kennard_stone-2.0.1/requirements.txt
+-rw-r--r--   0 yu9824     (501) staff       (20)       38 2023-04-25 14:21:56.864450 kennard_stone-2.0.1/setup.cfg
+-rw-r--r--   0 yu9824     (501) staff       (20)     2645 2023-04-22 06:08:03.000000 kennard_stone-2.0.1/setup.py
```

### Comparing `kennard_stone-2.0.0/LICENSE` & `kennard_stone-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.0.0/PKG-INFO` & `kennard_stone-2.0.1/kennard_stone.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kennard_stone
-Version: 2.0.0
+Name: kennard-stone
+Version: 2.0.1
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -22,17 +22,17 @@
 
 # Kennard Stone
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
 [![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
-[![Anaconda-license badge](https://anaconda.org/conda-forge/kennard-stone/badges/license.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
 
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
 
 ![simulateion_gif](https://github.com/yu9824/kennard_stone/blob/main/example/simulate.gif?raw=true "Simulateion")
```

### Comparing `kennard_stone-2.0.0/kennard_stone/_deprecated.py` & `kennard_stone-2.0.1/kennard_stone/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kennard_stone-2.0.0/kennard_stone/kennard_stone.py` & `kennard_stone-2.0.1/kennard_stone/kennard_stone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Copyright © 2021 yu9824
 """
 
 from typing import List, Union, Optional
+from itertools import chain
 import warnings
 
 import numpy as np
 
-from itertools import chain
 from sklearn.model_selection._split import BaseShuffleSplit
 from sklearn.model_selection._split import _BaseKFold
 from sklearn.model_selection._split import _validate_shuffle_split
 from sklearn.utils.validation import _num_samples
 from sklearn.utils import indexable, _safe_indexing
 from sklearn.preprocessing import StandardScaler
 from sklearn.utils import check_array
@@ -190,29 +190,29 @@
         idx_remaining = np.delete(idx_remaining, idx_farthest, axis=0)
 
         # 近い順のindexのリスト．i.e. 最初がtest向き，最後がtrain向き
         indexes = self._sort(
             X=X, lst_idx_selected=lst_idx_selected, idx_remaining=idx_remaining
         )
         assert (
-            len(sum(indexes, start=[]))
-            == len(set(sum(indexes, start=[])))
+            len(list(chain.from_iterable(indexes)))
+            == len(set(chain.from_iterable(indexes)))
             == len(self._original_X)
         )
 
         return indexes
 
     def _sort(
         self,
         X,
         lst_idx_selected: List[List[int]],
         idx_remaining: Union[List[int], np.ndarray],
     ) -> List[List[int]]:
         samples_selected: np.ndarray = self._original_X[
-            sum(lst_idx_selected, start=[])
+            list(chain.from_iterable(lst_idx_selected))
         ]
 
         # まだ選択されていない各サンプルにおいて、これまで選択されたすべてのサンプルとの間で
         # ユークリッド距離を計算し，その最小の値を「代表長さ」とする．
 
         min_distance_to_samples_selected = np.sum(
             np.square(
```

### Comparing `kennard_stone-2.0.0/kennard_stone.egg-info/PKG-INFO` & `kennard_stone-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kennard-stone
-Version: 2.0.0
+Name: kennard_stone
+Version: 2.0.1
 Summary: A method for selecting samples by spreading the training data evenly.
 Home-page: https://github.com/yu9824/kennard_stone
 Author: yu9824
 Author-email: yu.9824.job@gmail.com
 Maintainer: yu9824
 Maintainer-email: yu.9824.job@gmail.com
 License: MIT
@@ -22,17 +22,17 @@
 
 # Kennard Stone
 [![python_badge](https://img.shields.io/pypi/pyversions/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![license_badge](https://img.shields.io/pypi/l/kennard-stone)](https://pypi.org/project/kennard-stone/)
 [![PyPI version](https://badge.fury.io/py/kennard-stone.svg)](https://pypi.org/project/kennard-stone/)
 [![Downloads](https://pepy.tech/badge/kennard-stone)](https://pepy.tech/project/kennard-stone)
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/kennard-stone/badges/version.svg)](https://anaconda.org/conda-forge/kennard-stone)
 [![Anaconda-platform badge](https://anaconda.org/conda-forge/kennard-stone/badges/platforms.svg)](https://anaconda.org/conda-forge/kennard-stone)
-[![Anaconda-license badge](https://anaconda.org/conda-forge/kennard-stone/badges/license.svg)](https://anaconda.org/conda-forge/kennard-stone)
 
 ## What is this?
 
 This is an algorithm for evenly partitioning data in a `scikit-learn`-like interface. (See [References](#References) for details of the algorithm.)
 
 ![simulateion_gif](https://github.com/yu9824/kennard_stone/blob/main/example/simulate.gif?raw=true "Simulateion")
```

### Comparing `kennard_stone-2.0.0/setup.py` & `kennard_stone-2.0.1/setup.py`

 * *Files identical despite different names*

