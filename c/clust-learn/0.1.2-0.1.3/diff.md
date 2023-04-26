# Comparing `tmp/clust-learn-0.1.2.tar.gz` & `tmp/clust-learn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clust-learn-0.1.2.tar", last modified: Sat Feb 18 10:19:01 2023, max compression
+gzip compressed data, was "clust-learn-0.1.3.tar", last modified: Wed Apr 26 21:43:42 2023, max compression
```

## Comparing `clust-learn-0.1.2.tar` & `clust-learn-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-02-18 10:18:51.000000 clust-learn-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-02-18 10:19:01.580972 clust-learn-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28377 2023-02-18 10:18:51.000000 clust-learn-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clearn/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/classifier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/classifier/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clearn/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/clustering/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/clustering/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/clustering/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clearn/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/data_preprocessing/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/data_preprocessing/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clearn/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/dimensionality_reduction/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/dimensionality_reduction/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/dimensionality_reduction/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-02-18 10:18:51.000000 clust-learn-0.1.2/clearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/clust_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-02-18 10:19:01.000000 clust-learn-0.1.2/clust_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-18 10:19:01.000000 clust-learn-0.1.2/clust_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 10:19:01.000000 clust-learn-0.1.2/clust_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-18 10:19:01.000000 clust-learn-0.1.2/clust_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-18 10:19:01.000000 clust-learn-0.1.2/clust_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-18 10:18:52.000000 clust-learn-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 10:19:01.580972 clust-learn-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-18 10:18:52.000000 clust-learn-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 10:19:01.580972 clust-learn-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 10:18:52.000000 clust-learn-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-18 10:18:52.000000 clust-learn-0.1.2/tests/test_clearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 21:43:25.000000 clust-learn-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-04-26 21:43:42.980054 clust-learn-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28377 2023-04-26 21:43:25.000000 clust-learn-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/clearn/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/clust_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-26 21:43:25.000000 clust-learn-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:43:42.980054 clust-learn-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-26 21:43:25.000000 clust-learn-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:25.000000 clust-learn-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 21:43:25.000000 clust-learn-0.1.3/tests/test_clearn.py
```

### Comparing `clust-learn-0.1.2/LICENSE` & `clust-learn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/PKG-INFO` & `clust-learn-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -102,15 +102,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.2
+* Version: 0.1.3
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.2/README.md` & `clust-learn-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.2
+* Version: 0.1.3
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.2/clearn/classifier/classifier.py` & `clust-learn-0.1.3/clearn/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/classifier/utils.py` & `clust-learn-0.1.3/clearn/classifier/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/classifier/viz_utils.py` & `clust-learn-0.1.3/clearn/classifier/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/clustering/clustering.py` & `clust-learn-0.1.3/clearn/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/clustering/table_utils.py` & `clust-learn-0.1.3/clearn/clustering/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/clustering/utils.py` & `clust-learn-0.1.3/clearn/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/clustering/viz_utils.py` & `clust-learn-0.1.3/clearn/clustering/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/data_preprocessing/__init__.py` & `clust-learn-0.1.3/clearn/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/data_preprocessing/data_preprocessing.py` & `clust-learn-0.1.3/clearn/data_preprocessing/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/data_preprocessing/viz_utils.py` & `clust-learn-0.1.3/clearn/data_preprocessing/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/dimensionality_reduction/dimensionality_reduction.py` & `clust-learn-0.1.3/clearn/dimensionality_reduction/dimensionality_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,19 +120,23 @@
             trans = pd.concat([trans, self.num_trans_], axis=1)
         if self.cat_vars is not None:
             self.cat_trans_ = self._transform_cat(self.df[self.cat_vars], n_components_cat)
             trans = pd.concat([trans, self.cat_trans_], axis=1)
 
         idx_positions = np.maximum(len(str(trans.shape[1])), 2)
         trans.columns = [f'dim_{str(i+1).zfill(idx_positions)}' for i in range(trans.shape[1])]
-        self.num_components_ = list(trans.columns)[:self.num_trans_.shape[1]]
-        self.num_trans_.columns = self.num_components_
-        self.cat_components_ = list(trans.columns)[-self.cat_trans_.shape[1]:]
-        self.cat_trans_.columns = self.cat_components_
-        self.n_components_ = len(self.num_components_) + len(self.cat_components_)
+        self.n_components_ = 0
+        if self.num_vars is not None:
+            self.num_components_ = list(trans.columns)[:self.num_trans_.shape[1]]
+            self.num_trans_.columns = self.num_components_
+            self.n_components_ += len(self.num_components_)
+        if self.cat_vars is not None:
+            self.cat_components_ = list(trans.columns)[-self.cat_trans_.shape[1]:]
+            self.cat_trans_.columns = self.cat_components_
+            self.n_components_ += len(self.cat_components_)
         return trans
 
     def _transform_num(self, df, n_components_num=None):
         # For now, we take PCA as reference because SPCA results depend on the number of components
         sc = StandardScaler()
         
         if self.pca_.n_components is None:
```

### Comparing `clust-learn-0.1.2/clearn/dimensionality_reduction/table_utils.py` & `clust-learn-0.1.3/clearn/dimensionality_reduction/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/dimensionality_reduction/viz_utils.py` & `clust-learn-0.1.3/clearn/dimensionality_reduction/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clearn/utils.py` & `clust-learn-0.1.3/clearn/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/clust_learn.egg-info/PKG-INFO` & `clust-learn-0.1.3/clust_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -102,15 +102,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.2
+* Version: 0.1.3
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.2/clust_learn.egg-info/SOURCES.txt` & `clust-learn-0.1.3/clust_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.2/pyproject.toml` & `clust-learn-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clust-learn"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Miguel Alvarez-Garcia", email="malvarez.statistics@gmail.com" },
 ]
 description = "A Python package for explainable cluster analysis"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `clust-learn-0.1.2/setup.py` & `clust-learn-0.1.3/setup.py`

 * *Files identical despite different names*

