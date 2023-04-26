# Comparing `tmp/cosmic_toolbox-0.1.0.tar.gz` & `tmp/cosmic_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_toolbox-0.1.0.tar", last modified: Wed Apr 26 10:20:44 2023, max compression
+gzip compressed data, was "cosmic_toolbox-0.1.1.tar", last modified: Wed Apr 26 14:13:34 2023, max compression
```

## Comparing `cosmic_toolbox-0.1.0.tar` & `cosmic_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 10:20:44.809098 cosmic_toolbox-0.1.0/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      248 2023-04-26 09:19:57.000000 cosmic_toolbox-0.1.0/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1710 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       97 2023-04-26 10:20:22.000000 cosmic_toolbox-0.1.0/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      913 2023-04-26 10:20:44.809157 cosmic_toolbox-0.1.0/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      101 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1260 2023-04-26 10:20:44.809460 cosmic_toolbox-0.1.0/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 10:20:44.805343 cosmic_toolbox-0.1.0/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 10:20:44.807797 cosmic_toolbox-0.1.0/src/cosmic_toolbox/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9245 2023-04-19 12:21:53.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/MultiInterp.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5195 2023-04-19 12:20:49.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/NearestWeightedNDInterpolator.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3741 2023-04-19 12:16:01.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/TransformedGaussianMixture.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      168 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    20488 2023-04-19 12:24:56.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/arraytools.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      703 2023-03-23 15:56:28.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/colors.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5711 2023-03-21 22:26:34.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/copy_guardian.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3453 2023-03-21 22:26:34.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/file_utils.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2865 2023-03-21 22:26:34.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox/logger.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 10:20:44.808573 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      913 2023-04-26 10:20:44.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      746 2023-04-26 10:20:44.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 10:20:44.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-02-22 13:11:51.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      210 2023-04-26 10:20:44.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       15 2023-04-26 10:20:44.000000 cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 10:20:44.808987 cosmic_toolbox-0.1.0/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1649 2023-03-22 13:10:38.000000 cosmic_toolbox-0.1.0/tests/test_arraytools.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)      120 2023-03-21 22:26:34.000000 cosmic_toolbox-0.1.0/tests/test_cosmic_toolbox.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      515 2023-03-23 15:51:11.000000 cosmic_toolbox-0.1.0/tests/test_logger.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 14:13:34.744644 cosmic_toolbox-0.1.1/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      248 2023-04-26 09:19:57.000000 cosmic_toolbox-0.1.1/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1710 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      157 2023-04-26 14:13:07.000000 cosmic_toolbox-0.1.1/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.1/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.1/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      913 2023-04-26 14:13:34.744720 cosmic_toolbox-0.1.1/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      101 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.1/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-02-22 13:11:43.000000 cosmic_toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1314 2023-04-26 14:13:34.745200 cosmic_toolbox-0.1.1/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 14:13:34.740286 cosmic_toolbox-0.1.1/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 14:13:34.743086 cosmic_toolbox-0.1.1/src/cosmic_toolbox/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9213 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/MultiInterp.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5193 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/NearestWeightedNDInterpolator.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3727 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/TransformedGaussianMixture.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      168 2023-04-26 14:13:10.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    20451 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/arraytools.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      701 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/colors.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     5700 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/copy_guardian.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3443 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/file_utils.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2862 2023-04-26 13:49:12.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox/logger.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 14:13:34.744076 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      913 2023-04-26 14:13:34.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      746 2023-04-26 14:13:34.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-04-26 14:13:34.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-02-22 13:11:51.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      258 2023-04-26 14:13:34.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       15 2023-04-26 14:13:34.000000 cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-04-26 14:13:34.744514 cosmic_toolbox-0.1.1/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1649 2023-03-22 13:10:38.000000 cosmic_toolbox-0.1.1/tests/test_arraytools.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)      546 2023-04-26 14:00:15.000000 cosmic_toolbox-0.1.1/tests/test_cosmic_toolbox.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      515 2023-03-23 15:51:11.000000 cosmic_toolbox-0.1.1/tests/test_logger.py
```

### Comparing `cosmic_toolbox-0.1.0/CONTRIBUTING.rst` & `cosmic_toolbox-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cosmic_toolbox-0.1.0/LICENSE` & `cosmic_toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmic_toolbox-0.1.0/PKG-INFO` & `cosmic_toolbox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic_toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of code from the Cosmology Research Group at ETH
 Author: Silvan Fischbacher
 Author-email: silvanf@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/cosmic_toolbox
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cosmic_toolbox-0.1.0/pyproject.toml` & `cosmic_toolbox-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cosmic_toolbox-0.1.0/setup.cfg` & `cosmic_toolbox-0.1.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 project_urls = 
 	Source = https://cosmo-docs.phys.ethz.ch/cosmic_toolbox
 
 [options]
 install_requires = 
 	numpy
 	h5py
+	cycler
+	scipy
+	scikit-learn
+	pyyaml
+	six
+	matplotlib
 packages = find:
 package_dir = 
 	=src
 zip_safe = False
 python_requires = >=3.7
 
 [options.packages.find]
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/MultiInterp.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/MultiInterp.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,58 +7,54 @@
     division,
     print_function,
     unicode_literals,
 )
 import warnings
 import numpy as np
 import sys
-from chaoshammer.utils import utils
+from cosmic_toolbox.logger import get_logger
 from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator, Rbf
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.neighbors import (
     KNeighborsRegressor,
     RadiusNeighborsRegressor,
     BallTree,
 )
 from sklearn.ensemble import RandomForestRegressor
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 warnings.filterwarnings("once", category=UserWarning)
-LOGGER = utils.get_logger(__file__)
+LOGGER = get_logger(__file__)
 
 
 class Rbft:
     def __init__(self, points, values, **kw_rbf):
-
         self.points = points
         self.values = values
         self.bounds = [np.min(points, axis=0), np.max(points, axis=0)]
         self.scaler = MinMaxScaler()
         self.scaler.fit(self.points)
         self.points = self.scaler.transform(self.points)
         self.interp = Rbf(*list(self.points.T), self.values, **kw_rbf)
 
     def __call__(self, points, **kw_rbf):
-
         values_pred = np.zeros(len(points))
         select = self._in_bounds(points)
         values_pred[~select] = -np.inf
 
         points = self.scaler.transform(points)
         values_pred[select] = self.interp(*list(points[select].T))
         return values_pred
 
     def _in_bounds(self, x):
-
         return np.all(x > self.bounds[0], axis=1) & np.all(x < self.bounds[1], axis=1)
 
 
 def query_split(X, tree, k, n_proc):
-
     nx = X.shape[0]
     n_per_batch = int(np.ceil(nx / n_proc))
     LOGGER.info(
         "querying BallTree with a pool for n_grid={} "
         "n_proc={} n_per_batch={} n_neighbors={}".format(nx, n_proc, n_per_batch, k)
     )
     X_chunks = [X[(i * n_per_batch) : (i + 1) * n_per_batch, :] for i in range(n_proc)]
@@ -71,52 +67,47 @@
 
     distances = np.concatenate([list_y[i][0] for i in range(n_proc)])
     indices = np.concatenate([list_y[i][1] for i in range(n_proc)])
     return distances, indices
 
 
 def query_batch(X, tree, k=100, n_per_batch=10000):
-
     nx = X.shape[0]
     n_batches = int(np.ceil(nx / n_per_batch))
     indices = np.zeros([nx, k], dtype=np.int)
     distances = np.zeros([nx, k])
     for i in range(n_batches):
-
         si, ei = i * n_per_batch, (i + 1) * n_per_batch
         Xq = X[si:ei, :]
         if len(Xq) > 0:
             dist, ind = tree.query(Xq, k=k)
             indices[si:ei, :] = ind
             distances[si:ei, :] = dist
             LOGGER.info("batch={:>6}/{:>6}".format(i, n_batches))
 
     return distances, indices
 
 
 def predict_with_neighbours(y, ind, dist):
-
     yn = y[ind]
     wn = 1.0 / dist
     wn[wn == 0] = 1e10
     yi = np.average(yn, weights=wn, axis=1)
 
     return yi
 
 
 def predict_knn_balltree(Xi, X, y, n_neighbors, tree):
-
     nx, nd = Xi.shape
     dist, ind = tree.query(Xi, k=n_neighbors)
     yi = predict_with_neighbours(y, ind, dist)
     return yi
 
 
 def predict_knn_linear(Xi, X, y, n_neighbors, tree):
-
     nx, nd = Xi.shape
     dist, ind = tree.query(Xi, k=n_neighbors)
     X_nearest = X[ind, :]
     y_nearest = y[ind]
     yi = np.full(nx, -np.inf)
     n_nan = 0
 
@@ -130,156 +121,132 @@
         sys.stdout.write("\r{}/{} {}".format(i, nx, n_nan))
 
     return yi
 
 
 class MultiInterp:
     def __init__(self, X, y, method="nn", **kw):
-
         self.X = X.copy()
         self.y = y.copy()
         self.bounds = [np.min(X, axis=0), np.max(X, axis=0)]
         self.scaler = MinMaxScaler()
         self.scaler.fit(self.X)
         self.X = self.scaler.transform(self.X)
         self.interp = None
         self.method = method
         self.kw = kw
         self.init_interp(**kw)
 
     def __call__(self, Xi, **kw):
-
         yi = np.zeros(len(Xi))
         select = self._in_bounds(Xi)
         yi[~select] = -np.inf
 
         Xi = self.scaler.transform(Xi.copy())
 
         if self.method.lower() == "rbf":
-
             yi[select] = self.interp(*list(Xi[select, :].T), **kw)
 
         elif self.method.lower() == "rbft":
-
             yi[select] = self.interp(Xi[select, :], **kw)
 
         elif self.method.lower() in ["knn_regression", "rnn_regression"]:
-
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 yi[select] = self.interp.predict(Xi[select, :], **kw)
 
         elif self.method.lower() in ["nn", "linear"]:
-
             yi[select] = self.interp(Xi[select, :], **kw)
 
         elif self.method.lower() == "knn_linear":
-
             yi[select] = predict_knn_linear(
                 Xi[select, :],
                 self.X,
                 self.y,
                 self.n_neighbors,
                 self.interp,
                 **kw,
             )
 
         elif self.method.lower() == "random_forest":
-
             yi[select] = self.interp.predict(Xi[select, :], **kw)
 
         elif self.method.lower() == "knn_balltree":
-
             yi[select] = predict_knn_balltree(
                 Xi[select, :],
                 self.X,
                 self.y,
                 self.n_neighbors,
                 self.interp,
                 **kw,
             )
 
         else:
-
             raise Exception(f"unknown interp method {self.method}")
 
         return yi
 
     def _in_bounds(self, X):
-
         return np.all(X > self.bounds[0], axis=1) & np.all(X < self.bounds[1], axis=1)
 
     def init_interp(self, **kw):
-
         if self.method.lower() == "rbf":
-
             self.interp = Rbf(*list(self.X.T), self.y, **kw)
 
         elif self.method.lower() == "rbft":
-
             self.interp = Rbft(points=self.X, values=self.y, **kw)
 
         elif self.method.lower() == "knn":
-
             self.interp = KNeighborsRegressor(**kw)
             self.interp.fit(self.X, self.y)
 
         elif self.method.lower() == "knn_regression":
-
             self.interp = KNeighborsRegressor(**kw)
             self.interp.fit(self.X, self.y)
 
         elif self.method.lower() == "rnn_regression":
-
             kw.setdefault("radius", 0.1)
             self.interp = RadiusNeighborsRegressor(**kw)
             self.interp.fit(self.X, self.y)
 
         elif self.method.lower() == "nn":
-
             self.interp = NearestNDInterpolator(self.X, self.y, **kw)
 
         elif self.method.lower() == "linear":
-
             self.interp = LinearNDInterpolator(self.X, self.y, **kw)
 
         elif self.method.lower() == "knn_linear":
-
             # self.slice_linear_upsampling(n_repeat=1)
             n_neighbors = kw.pop("n_neighbors", self.X.shape[1] * 3)
             self.interp = BallTree(self.X, **kw)
             self.n_neighbors = n_neighbors
 
         elif self.method.lower() == "random_forest":
-
             self.interp = RandomForestRegressor(**kw)
             self.interp.fit(self.X, self.y)
 
         elif self.method.lower() == "knn_balltree":
-
             n_neighbors = kw.pop("n_neighbors", self.X.shape[1] * 3)
             self.interp = BallTree(self.X, **kw)
             self.n_neighbors = n_neighbors
 
         else:
             raise Exception(f"unknown interp method {self.method}")
 
     def precompute_grid_neighbors(self, Xn, n_neighbors=100, n_proc=1):
-
         assert self.method == "knn_balltree"
 
         Xn = self.scaler.transform(Xn.copy())
         dist, ind = query_split(tree=self.interp, X=Xn, k=n_neighbors, n_proc=n_proc)
 
         self.neighbors_ind = ind
         self.neighbors_dist = dist.astype(np.float32)
         self.neighbors_Xn = Xn.astype(np.float32)
 
     def interpolate_grid_neighbours(self, y, n_neighbors=None):
-
         assert len(y) == len(self.X)
         if n_neighbors is None:
             n_neighbors = self.n_neighbors
 
         nn = self.neighbors_ind.shape[1]
         if n_neighbors > nn:
             raise Exception("number of available neighbors {}".format(nn))
@@ -288,17 +255,15 @@
             self.neighbors_ind[:, :n_neighbors],
             self.neighbors_dist[:, :n_neighbors],
         )
 
         return yi
 
     def slice_linear_upsampling(self, n_repeat=1, n_neighbors=1):
-
         for i in range(n_repeat):
-
             bt = BallTree(self.X)
             dist, ids = bt.query(self.X, k=n_neighbors + 1)
             list_Xn = [self.X]
             list_yn = [self.y]
             for j in range(1, n_neighbors + 1):
                 Xn = (self.X + self.X[ids[:, j], :]) / 2.0
                 yn = (self.y + self.y[ids[:, j]]) / 2.0
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/NearestWeightedNDInterpolator.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/NearestWeightedNDInterpolator.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from scipy.interpolate.interpnd import NDInterpolatorBase
 from sklearn.neighbors import BallTree
 from sklearn.preprocessing import MinMaxScaler
 
 
 class NearestWeightedNDInterpolator(NDInterpolatorBase):
     def __init__(self, x, y, k=None, tree_options={}):
-
         self.x = x
         self.y = y
         self.ndim = self.x.shape[1]
         if k is None:
             k = self.ndim + 1  # number of vertices of ndim dimensional simplex
         self.k = k
         self.scaler = MinMaxScaler()
@@ -24,15 +23,14 @@
 
         # from sklearn import neighbors
         # self.knn = neighbors.KNeighborsRegressor(n_neighbors=k,
         #                                          weights='distance')
         # self.knn.fit(self.x , self.y)
 
     def __call__(self, xi):
-
         assert len(xi.shape) == 2
         assert self.ndim == xi.shape[1]
 
         xi = self.scaler.transform(xi)
         # vi = self.knn.predict(xi)
 
         dist, i = self.tree.query(xi, self.k)
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/TransformedGaussianMixture.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/TransformedGaussianMixture.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,102 +41,88 @@
     xi = norm.cdf(x)
     xi = scale_inv(xi, param_bounds, param_bounds_trans)
     return xi
 
 
 class TransformedGaussianMixture:
     def __init__(self, param_bounds=None, *args, **kwargs):
-
         self.eps = 1e-8
         self.bounds_trans = [self.eps, 1 - self.eps]
         self.param_bounds = param_bounds
 
         self.gm = GaussianMixture(*args, **kwargs)
 
     def set_bounds(self, X):
-
         if self.param_bounds is None:
             self.param_bounds = np.array(
                 [
                     np.min(X, axis=0) - 10 * self.eps,
                     np.max(X, axis=0) + 10 * self.eps,
                 ]
             ).T
 
     def fit(self, X, y=None):
-
         self.set_bounds(X)
         X_trans = self._transform_params_forward(X)
         return self.gm.fit(X_trans, y)
 
     def fit_predict(self, X, y=None):
-
         self.set_bounds(X)
         X_trans = self._transform_params_forward(X)
         return self.gm.fit_predict(X_trans, y)
 
     def predict_proba(self, X):
-
         X_trans = self._transform_params_forward(X)
         return self.gm.predict_proba(X_trans)
 
     def sample(self, n_samples=1):
-
         # print('ol')
         # import chaospy
         # means = self.gm.means_[:, :2]
         # covariances = self.gm.covariances_[:, :2, :2]
         # self.chaos_gm = chaospy.GaussianMixture(means, covariances)
         # X_trans, y = self.chaos_gm.sample(n_samples, rule="halton")
         X_trans, y = self.gm.sample(n_samples)
         X = self._transform_params_inverse(X_trans)
         return X, y
 
     def score(self, X, y=None):
-
         X_trans = self._transform_params_forward(X)
         return self.gm.score(X_trans)
 
     def score_samples(self, X):
-
         X_trans = self._transform_params_forward(X)
         return self.gm.score_samples(X_trans)
 
     def set_params(self, **params):
-
         return self.gm.set_params(**params)
 
     def get_params(self, deep=True):
-
         return self.gm.get_params(deep)
 
     def bic(self, X):
-
         X_trans = self._transform_params_forward(X)
         return self.gm.bic(X_trans)
 
     def aic(self, X):
-
         X_trans = self._transform_params_forward(X)
         return self.gm.aic(X_trans)
 
     def _transform_params_forward(self, X):
-
         X_trans = X.copy()
         for i in range(X.shape[1]):
             X_trans[:, i] = trans_fwd(
                 x=np.array(X[:, i]),
                 param_bounds=self.param_bounds[i],
                 param_bounds_trans=self.bounds_trans,
             )
 
         return X_trans
 
     def _transform_params_inverse(self, X_trans):
-
         X = X_trans.copy()
         for i in range(X.shape[1]):
             X[:, i] = trans_inv(
                 x=np.array(X_trans[:, i]),
                 param_bounds=self.param_bounds[i],
                 param_bounds_trans=self.bounds_trans,
             )
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/arraytools.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/arraytools.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,24 @@
         dict(names=names, formats=formats, offsets=offsets, itemsize=itemsize)
     )
     rec_view = rec.view(newdt)
     return rec_view
 
 
 def delete_columns(rec, col_names):
-
     col_names_all = list(rec.dtype.names)
 
     for col_name in col_names:
         if col_name in col_names_all:
             col_names_all.remove(col_name)
 
     return rec[col_names_all].copy()
 
 
 def add_cols(rec, names, shapes=None, data="zeros"):
-
     if data == "zeros":
         data = 0
 
     # check if new data should be sliced
     slice_data = isinstance(data, np.ndarray) and data.ndim == 2
 
     # create new recarray
@@ -51,25 +49,23 @@
     newdtype = np.dtype(rec.dtype.descr + extra_dtype.descr)
     newrec = np.empty(rec.shape, dtype=newdtype)
 
     # add data to new recarray
     for field in rec.dtype.fields:
         newrec[field] = rec[field]
     for ni, name in enumerate(extra_dtype.fields):
-
         if slice_data:
             newrec[name] = data[ni]
         else:
             newrec[name] = data
 
     return newrec
 
 
 def ensure_cols(rec, names, shapes=None, data="zeros"):
-
     # find columns to add
     names = [str(name) for name in names]
     new_names = []
     for name in names:
         if get_dtype([name]).names[0] not in rec.dtype.names:
             new_names.append(name)
 
@@ -211,28 +207,26 @@
 
     assert all_the_same, "Not all entries of the list have the same dtype"
 
     return dtype
 
 
 def new_array(n_rows, columns, ints=[], float_dtype=np.float64, int_dtype=np.int64):
-
     n_columns = len(columns)
     formats = [None] * n_columns
     for ic in range(n_columns):
         if columns[ic] in ints:
             formats[ic] = int_dtype
         else:
             formats[ic] = float_dtype
     newrec = np.zeros(n_rows, dtype=np.dtype(zip(columns, formats)))
     return newrec
 
 
 def get_dtype(columns, main="f8", shapes=None):
-
     list_name = []
     list_dtype = []
 
     if shapes is None:
         shapes = [() for _ in columns]
 
     for col in columns:
@@ -246,26 +240,24 @@
 
     dtype = np.dtype(list(zip(list_name, list_dtype, shapes)))
 
     return dtype
 
 
 def get_storing_dtypes(dtype_list):
-
     if six.PY2:
         dtypes = [(str(dt[0]), str(dt[1])) + dt[2:] for dt in dtype_list]
 
     else:
         dtypes = [(dt[0], dt[1].replace("<U", "|S")) + dt[2:] for dt in dtype_list]
 
     return dtypes
 
 
 def get_loading_dtypes(dtype_list):
-
     if six.PY2:
         dtypes = [(str(dt[0]), str(dt[1])) + dt[2:] for dt in dtype_list]
 
     else:
         dtypes = []
         # handling for h5py>=2.10.0
         for dt in dtype_list:
@@ -274,21 +266,19 @@
             else:
                 dtypes.append((dt[0], dt[1].replace("|S", "<U")) + dt[2:])
 
     return dtypes
 
 
 def set_storing_dtypes(arr):
-
     if six.PY2:
         return arr
 
     # numpy array
     elif hasattr(arr, "dtype"):
-
         dtype = arr.dtype
 
         # ndarray
         if len(dtype) == 0:
             dtypes_store = arr.dtype.str.replace("<U", "|S")
 
         # recarray
@@ -298,15 +288,14 @@
         return arr.astype(dtypes_store)
 
     # string
     elif isinstance(arr, str):
         return arr.encode("utf-8")
 
     else:
-
         # list or tuple
         try:
             arr_fixed = [None] * len(arr)
 
             for i, x in enumerate(arr):
                 if isinstance(x, str):
                     arr_fixed[i] = x.encode("utf-8")
@@ -317,21 +306,19 @@
 
         # single number
         except Exception:
             return arr
 
 
 def set_loading_dtypes(arr):
-
     if six.PY2:
         return arr
 
     # numpy array
     elif hasattr(arr, "dtype"):
-
         dtype = arr.dtype
 
         # ndarray
         if len(dtype) == 0:
             dtypes_load = arr.dtype.str.replace("|S", "<U").replace("|O", "<U")
 
         # recarray
@@ -341,15 +328,14 @@
         return arr.astype(dtypes_load)
 
     # bytes
     elif isinstance(arr, bytes):
         return arr.decode("utf-8")
 
     else:
-
         # list or tuple
         try:
             arr_fixed = [None] * len(arr)
 
             for i, x in enumerate(arr):
                 if isinstance(x, bytes):
                     arr_fixed[i] = x.decode("utf-8")
@@ -360,15 +346,14 @@
 
         # single number
         except Exception:
             return arr
 
 
 def save_hdf(filename, arr, **kwargs):
-
     f5 = h5py.File(name=filename)
 
     try:
         f5.clear()
 
     except Exception:
         for datasetname in f5.keys():
@@ -377,19 +362,17 @@
     arr_store = set_storing_dtypes(arr)
     f5.create_dataset(name="data", data=arr_store, **kwargs)
     f5.close()
     LOGGER.info("saved {}".format(filename))
 
 
 def load_hdf(filename, first_row=-1, last_row=-1):
-
     f5 = h5py.File(name=filename, mode="r")
 
     if (first_row > -1) & (last_row > -1) & (first_row < last_row):
-
         if first_row < last_row:
             data = np.array(f5["data"][first_row:last_row])
 
         else:
             raise Exception(
                 "first_row ({}) should be smaller "
                 "than last_row ({})".format(first_row, last_row)
@@ -404,26 +387,23 @@
 
     LOGGER.info("loaded {}".format(filename))
 
     return data
 
 
 def save_hdf_cols(filename, arr, compression=None, resizable=False):
-
     if compression is None:
         kwargs = {}
     else:
         kwargs = dict(compression=compression)
 
     dtypes_store = get_storing_dtypes(arr.dtype.descr)
 
     with h5py.File(filename, "w") as fh5:
-
         for dt in dtypes_store:
-
             col = dt[0]
             dtype = dt[1]
             extra_dims = dt[2:]
 
             if col in fh5:
                 del fh5[col]
 
@@ -442,17 +422,15 @@
     columns,
     first_row,
     last_row,
     cols_to_add=(),
     selectors=None,
     verb=True,
 ):
-
     with h5py.File(filename, mode="r") as fh5:
-
         # Infer columns to load
         if columns == "all":
             columns = list(fh5.keys())
 
         # Infer size of data to load
         if last_row is not None:
             if last_row > 0:
@@ -471,15 +449,14 @@
             last_row = size
 
         # Get boolean mask in case any selectors were specified
         if selectors is not None and len(selectors) > 0:
             select = np.ones(size, dtype=np.bool)
 
             for cols in selectors:
-
                 select_fun = selectors[cols]
 
                 if isinstance(cols, str):
                     cols = (cols,)
 
                 select &= select_fun(*[fh5[c][first_row:last_row] for c in cols])
 
@@ -510,15 +487,14 @@
 
 
 def col_name_to_path(dirname, colname):
     return os.path.join(dirname, colname + ".h5")
 
 
 def get_hdf_col_names(path):
-
     # file
     if os.path.isfile(path):
         with h5py.File(path, mode="r") as fh5:
             columns = list(fh5.keys())
 
     # directory
     columns = [
@@ -537,15 +513,14 @@
     dirname_parent=None,
     allow_nonexisting=False,
     cols_to_add=(),
     selectors=None,
     verb=True,
     copy_editor=None,
 ):
-
     if selectors is None:
         selectors = dict()
 
     if copy_editor is None:
         copy_editor = lambda p: p  # noqa
 
     # Infer columns to load
@@ -570,29 +545,27 @@
         columns = list(columns)
 
     # Get filename
     # (for all columns s.t. one can also use selectors
     # using columns that are not loaded)
     dict_filename_cols = {}
     for col in set(columns_all + columns + list(selectors.keys())):
-
         # get the filename from the right folder
         filename_col = col_name_to_path(dirname, col)
 
         if not os.path.isfile(filename_col) and dirname_parent is not None:
             filename_col = col_name_to_path(dirname_parent, col)
 
         dict_filename_cols[col] = filename_col
 
     # Infer size of data to load
     if last_row is not None:
         if last_row > 0:
             size = last_row - first_row
         else:
-
             with h5py.File(dict_filename_cols[columns[0]], mode="r") as fh5:
                 size = len(fh5[columns[0]]) + last_row
                 last_row = size
 
                 if size < 0 or last_row < first_row:
                     raise Exception(
                         "Combination first_row={}, last_row={} invalid".format(
@@ -604,28 +577,25 @@
             size = len(fh5[columns[0]])
             last_row = size
 
     # Get boolean mask in case any selectors were specified
     columns_copied = {}
 
     if len(selectors) > 0:
-
         select = np.ones(size, dtype=np.bool)
 
         for cols in selectors:
-
             select_fun = selectors[cols]
 
             if isinstance(cols, str):
                 cols = (cols,)
 
             data_select = [None] * len(cols)
 
             for ic, c in enumerate(cols):
-
                 filename_col = dict_filename_cols[c]
 
                 if copy_local:
                     if c not in columns_copied:
                         path_local = os.path.join(
                             os.getcwd(), os.path.basename(filename_col)
                         )
@@ -659,29 +629,26 @@
     else:
         select = np.s_[:size]
 
     # Create array holding loaded data
     dtypes_list = [None] * len(columns)
 
     for i, col in enumerate(columns):
-
         with h5py.File(dict_filename_cols[col], mode="r") as fh5:
             dtypes_list[i] = (col, fh5[col].dtype.str, fh5[col].shape[1:])
 
     dtypes_load = get_loading_dtypes(dtypes_list)
     dtypes_load += [(col, np.float32) for col in cols_to_add]
     arr = np.empty(size, dtype=dtypes_load)
 
     # Now copy files one by one and read data
     for col in columns:
-
         filename_col = dict_filename_cols[col]
 
         if copy_local:
-
             if col in columns_copied:
                 path_local = columns_copied[col]
 
             else:
                 path_local = os.path.join(os.getcwd(), os.path.basename(filename_col))
                 file_utils.robust_copy(
                     copy_editor(filename_col), path_local, use_copyfile=True
@@ -720,15 +687,14 @@
     copy_local=True,
     filename_parent=None,
     allow_nonexisting=False,
     cols_to_add=(),
     selectors=None,
     copy_editor=None,
 ):
-
     if last_row is not None:
         if (last_row > 0) & (first_row >= last_row):
             raise Exception(
                 "first_row {} should be smaller than "
                 "last_row {}".format(first_row, last_row)
             )
 
@@ -774,34 +740,31 @@
 def replace_hdf5_dataset(fobj, name, data, **kwargs):
     if name in fobj:
         del fobj[name]
     fobj.create_dataset(name=name, data=set_storing_dtypes(data), **kwargs)
 
 
 def overwrite_hdf5_column(path, name, data, **kwargs):
-
     if os.path.isdir(path):
         path_col = col_name_to_path(path, name)
 
     else:
         path_col = path
 
     with h5py.File(path_col) as fh5:
         replace_hdf5_dataset(fh5, name, set_storing_dtypes(data), **kwargs)
 
 
 def check_hdf_column(filename, column_name):
-
     if os.path.isfile(filename):
         with h5py.File(filename, mode="r") as fh5:
             col_found = column_name in fh5.keys()
 
     else:
         filename_col = col_name_to_path(filename, column_name)
         col_found = os.path.isfile(filename_col)
 
     return col_found
 
 
 def nanequal(a, b):
-
     return (np.isnan(b) & np.isnan(a)) | (a == b)
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/colors.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import matplotlib.pyplot as plt
 from cycler import cycler
 
 
 def get_colors(cycle="silvan"):
-
     if cycle == "silvan":
         return {
             "b": "#0063B9",
             "r": "#BA1A13",
             "g": "#34BA09",
             "orange": "#ED6018",
             "violet": "#6E13BA",
@@ -18,14 +17,13 @@
             "bluegreen": "#09BAAF",
         }
     else:
         return cycle
 
 
 def set_cycle(cycle="silvan"):
-
     colors = get_colors(cycle=cycle)
     if isinstance(colors, dict):
         col = colors.values()
     else:
         col = colors
     plt.rc("axes", prop_cycle=cycler(color=col))
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/copy_guardian.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/copy_guardian.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     ):
         self.n_max_connect = n_max_connect
         self.n_max_attempts_remote = n_max_attempts_remote
         self.time_between_attempts = time_between_attempts
         self.use_copyfile = use_copyfile
 
     def __call__(self, sources, destination):
-
         # Ensure correct type
         if str(sources) == sources:
             sources = [sources]
 
         if str(destination) != destination:
             raise ValueError(
                 "Destination {} not supported. Multiple destinations for "
@@ -67,15 +66,14 @@
                 sources[i] += "/"
 
         if destination.endswith("/"):
             destination = destination[:-1]
 
         # Check if destination is remote
         if file_utils.is_remote(destination):
-
             # Check for remote sources
             for source in sources:
                 if file_utils.is_remote(source):
                     raise IOError(
                         "Cannot copy remote source {} to remote "
                         "destination {}".format(source, destination)
                     )
@@ -83,49 +81,45 @@
             self._copy_remote(sources, destination)
 
         else:
             # Split into local and remote sources
             sources_remote = []
 
             for source in sources:
-
                 # Remote source
                 if file_utils.is_remote(source):
                     sources_remote.append(source)
 
                 # Local source
                 else:
                     self._copy_local(source, destination)
 
             # Now handle remaining (remote) tasks
             if len(sources_remote) > 0:
                 self._copy_remote(sources_remote, destination)
 
     def _copy_local(self, source, destination):
-
         LOGGER.info("Copying locally: {} -> {}".format(source, destination))
 
         if os.path.isdir(source):
             distutils.dir_util.copy_tree(source, destination)
 
         elif os.path.isdir(destination) or not self.use_copyfile:
             shutil.copy(source, destination)
 
         else:
             shutil.copyfile(source, destination)
 
     def _copy_remote(self, sources, destination):
-
         n_attempts = 0
 
         sources_split = self._split_sources_by_host(sources)
         print(sources_split)
 
         while n_attempts < self.n_max_attempts_remote:
-
             self._wait_for_allowance()
             path_semaphore = self._create_semaphore()
 
             copied = True
 
             for srcs in sources_split:
                 for src in srcs:
@@ -150,17 +144,15 @@
 
         else:
             raise IOError(
                 "Failed to rsync {} -> {} ".format(", ".join(sources), destination)
             )
 
     def _wait_for_allowance(self):
-
         while True:
-
             time.sleep(1 + random.random())
 
             file_list = os.listdir(SEMAPHORE_DIRECTORY)
             file_list = list(
                 filter(lambda filename: not filename.startswith("."), file_list)
             )
 
@@ -170,33 +162,30 @@
     def _create_semaphore(self):
         filename = "{}_{}".format(os.getpid(), datetime.datetime.now()).replace(" ", "")
         filepath = os.path.join(SEMAPHORE_DIRECTORY, filename)
         open(filepath, "w").close()
         return filepath
 
     def _call_rsync(self, sources, destination):
-
         LOGGER.info("Rsyncing: {} -> {}".format(", ".join(sources), destination))
 
         cmd = "rsync -av {} {}".format(" ".join(sources), destination)
         print(cmd)
 
         try:
             subprocess.check_call(shlex.split(cmd))
             return True
 
         except subprocess.CalledProcessError:
             return False
 
     def _split_sources_by_host(self, sources):
-
         host_dict = {}
 
         for s in sources:
-
             host = s.split(":/")[0]
 
             if host in host_dict:
                 host_dict[host].append(s)
 
             else:
                 host_dict[host] = [s]
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/file_utils.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,32 @@
 from cosmic_toolbox.logger import get_logger
 
 
 LOGGER = get_logger(__file__)
 
 
 def robust_remove(path):
-
     if is_remote(path):
         LOGGER.info("Removing remote directory {}".format(path))
         host, path = path.split(":")
         cmd = 'ssh {} "rm -rf {}"'.format(host, path)
         subprocess.call(shlex.split(cmd))
 
     else:
-
         if os.path.isfile(path):
             os.remove(path)
 
         elif os.path.isdir(path):
             shutil.rmtree(path)
 
         else:
             LOGGER.info(f"Cannot remove {path} because it does not exist")
 
 
 def write_to_pickle(filepath, obj, compression="none"):
-
     if compression.lower() == "none":
         with open(filepath, "wb") as f:
             pickle.dump(obj, f)
     elif compression.lower() == "lzf":
         import lzf
 
         with lzf.open(filepath, "wb") as f:
@@ -52,15 +49,14 @@
             pickle.dump(obj, f)
 
     else:
         raise Exception(f"uknown compression {compression} [none, lzf, bz2]")
 
 
 def read_from_pickle(filepath, compression="none"):
-
     if compression.lower() == "none":
         with open(filepath, "rb") as f:
             obj = pickle.load(f)
     elif compression.lower() == "lzf":
         import lzf
 
         with lzf.open(filepath, "rb") as f:
@@ -74,15 +70,14 @@
     else:
         raise Exception(f"uknown compression {compression} [none, lzf, bz2]")
 
     return obj
 
 
 def get_abs_path(path):
-
     if "@" in path and ":/" in path:
         abs_path = path
 
     elif os.path.isabs(path):
         abs_path = path
 
     else:
@@ -93,15 +88,14 @@
 
         abs_path = os.path.join(parent, path)
 
     return abs_path
 
 
 def robust_makedirs(path):
-
     if is_remote(path):
         LOGGER.info("Creating remote directory {}".format(path))
         host, path = path.split(":")
         cmd = 'ssh {} "mkdir -p {}"'.format(host, path)
         subprocess.call(shlex.split(cmd))
 
     elif not os.path.isdir(path):
@@ -114,38 +108,34 @@
     dst,
     n_max_connect=10,
     n_max_attempts_remote=10,
     time_between_attempts=10,
     method="CopyGuardian",
     **kwargs,
 ):
-
     from . import copy_guardian
 
     # In case of a remote destination, rsync will create the directory itself
     if not is_remote(dst):
-
         robust_makedirs(os.path.dirname(dst))
 
     if method == "CopyGuardian":
-
         copy_guard = copy_guardian.CopyGuardian(
             n_max_connect,
             n_max_attempts_remote,
             time_between_attempts,
             **kwargs,
         )
         copy_guard(src, dst)
 
     # elif method == 'system_cp':
 
     #    system_copy(sources=src, dest=dst, **kwargs)
 
     else:
-
         raise Exception(f"Unknown copy method {method}")
 
 
 def is_remote(path):
     return "@" in path and ":/" in path
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox/logger.py` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,29 @@
 
 
 class Progressbar:
     def __init__(self, logger=None):
         self.logger = logger
 
     def __call__(self, collection, at_level="info", **kw):
-
         kw.setdefault("bar_format", "{percentage:3.0f}%|{bar:28}|   {r_bar:<40} {desc}")
         kw.setdefault("disable", self.logger.level != logging_levels[at_level])
         kw.setdefault("colour", "blue")
         kw.setdefault("mininterval", 1)
         kw.setdefault("file", sys.stdout)
         from tqdm import tqdm
 
         return tqdm(collection, **kw)
 
 
 def set_logger_level(logger, level):
-
     logger.setLevel(logging_levels[level])
 
 
 def set_all_loggers_level(level):
-
     os.environ["PYTHON_LOGGER_LEVEL"] = level
 
     loggerDict = logging.root.manager.loggerDict
     for key in loggerDict:
         try:
             set_logger_level(logger=loggerDict[key], level=level)
         except Exception as err:
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/PKG-INFO` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of code from the Cosmology Research Group at ETH
 Author: Silvan Fischbacher
 Author-email: silvanf@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/cosmic_toolbox
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cosmic_toolbox-0.1.0/src/cosmic_toolbox.egg-info/SOURCES.txt` & `cosmic_toolbox-0.1.1/src/cosmic_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmic_toolbox-0.1.0/tests/test_arraytools.py` & `cosmic_toolbox-0.1.1/tests/test_arraytools.py`

 * *Files identical despite different names*

### Comparing `cosmic_toolbox-0.1.0/tests/test_logger.py` & `cosmic_toolbox-0.1.1/tests/test_logger.py`

 * *Files identical despite different names*

