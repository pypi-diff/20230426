# Comparing `tmp/contextualbandits-0.3.8.tar.gz` & `tmp/contextualbandits-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/contextualbandits-0.3.8.tar", last modified: Mon Aug 24 19:02:40 2020, max compression
+gzip compressed data, was "dist/contextualbandits-0.3.9.tar", last modified: Thu Aug 27 17:46:11 2020, max compression
```

## Comparing `contextualbandits-0.3.8.tar` & `contextualbandits-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/
--rw-r--r--   0 david     (1000) david     (1000)      434 2020-05-07 16:35:17.000000 contextualbandits-0.3.8/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      399 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)    12205 2020-08-19 16:06:07.000000 contextualbandits-0.3.8/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits/
--rw-r--r--   0 david     (1000) david     (1000)       91 2020-04-28 19:24:31.000000 contextualbandits-0.3.8/contextualbandits/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     4057 2020-07-04 11:36:04.000000 contextualbandits-0.3.8/contextualbandits/_cy_utils.pyx
--rw-r--r--   0 david     (1000) david     (1000)     5685 2020-07-08 16:43:14.000000 contextualbandits-0.3.8/contextualbandits/cy_cpp_helpers.cpp
--rw-r--r--   0 david     (1000) david     (1000)    18239 2020-05-25 19:45:24.000000 contextualbandits-0.3.8/contextualbandits/evaluation.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits/linreg/
--rw-r--r--   0 david     (1000) david     (1000)    19565 2020-08-24 17:47:15.000000 contextualbandits-0.3.8/contextualbandits/linreg/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      469 2020-08-24 15:53:31.000000 contextualbandits-0.3.8/contextualbandits/linreg/linreg_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      467 2020-08-24 15:53:47.000000 contextualbandits-0.3.8/contextualbandits/linreg/linreg_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)    24387 2020-08-24 17:27:02.000000 contextualbandits-0.3.8/contextualbandits/linreg/linreg_untyped.pxi
--rw-r--r--   0 david     (1000) david     (1000)    18099 2020-07-11 14:56:11.000000 contextualbandits-0.3.8/contextualbandits/offpolicy.py
--rw-r--r--   0 david     (1000) david     (1000)   190593 2020-08-24 18:35:35.000000 contextualbandits-0.3.8/contextualbandits/online.py
--rw-r--r--   0 david     (1000) david     (1000)    54026 2020-08-24 18:47:13.000000 contextualbandits-0.3.8/contextualbandits/utils.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      399 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      642 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       72 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       18 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/contextualbandits.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       84 2020-07-09 15:21:32.000000 contextualbandits-0.3.8/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2020-08-24 19:02:40.000000 contextualbandits-0.3.8/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)     2338 2020-08-20 17:26:05.000000 contextualbandits-0.3.8/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/
+-rw-r--r--   0 david     (1000) david     (1000)      434 2020-05-07 16:35:17.000000 contextualbandits-0.3.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      399 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)    12324 2020-08-25 20:35:09.000000 contextualbandits-0.3.9/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/contextualbandits/
+-rw-r--r--   0 david     (1000) david     (1000)       91 2020-04-28 19:24:31.000000 contextualbandits-0.3.9/contextualbandits/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     4057 2020-07-04 11:36:04.000000 contextualbandits-0.3.9/contextualbandits/_cy_utils.pyx
+-rw-r--r--   0 david     (1000) david     (1000)     5685 2020-07-08 16:43:14.000000 contextualbandits-0.3.9/contextualbandits/cy_cpp_helpers.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    18239 2020-05-25 19:45:24.000000 contextualbandits-0.3.9/contextualbandits/evaluation.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/contextualbandits/linreg/
+-rw-r--r--   0 david     (1000) david     (1000)    32271 2020-08-27 16:53:25.000000 contextualbandits-0.3.9/contextualbandits/linreg/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      469 2020-08-24 15:53:31.000000 contextualbandits-0.3.9/contextualbandits/linreg/linreg_double.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      467 2020-08-24 15:53:47.000000 contextualbandits-0.3.9/contextualbandits/linreg/linreg_float.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    27965 2020-08-27 17:23:16.000000 contextualbandits-0.3.9/contextualbandits/linreg/linreg_untyped.pxi
+-rw-r--r--   0 david     (1000) david     (1000)    18099 2020-07-11 14:56:11.000000 contextualbandits-0.3.9/contextualbandits/offpolicy.py
+-rw-r--r--   0 david     (1000) david     (1000)   192620 2020-08-27 17:43:56.000000 contextualbandits-0.3.9/contextualbandits/online.py
+-rw-r--r--   0 david     (1000) david     (1000)    56177 2020-08-27 17:20:17.000000 contextualbandits-0.3.9/contextualbandits/utils.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/contextualbandits.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      399 2020-08-27 17:46:10.000000 contextualbandits-0.3.9/contextualbandits.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      642 2020-08-27 17:46:10.000000 contextualbandits-0.3.9/contextualbandits.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2020-08-27 17:46:10.000000 contextualbandits-0.3.9/contextualbandits.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       72 2020-08-27 17:46:10.000000 contextualbandits-0.3.9/contextualbandits.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       18 2020-08-27 17:46:10.000000 contextualbandits-0.3.9/contextualbandits.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       84 2020-07-09 15:21:32.000000 contextualbandits-0.3.9/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       79 2020-08-27 17:46:11.000000 contextualbandits-0.3.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     2338 2020-08-25 21:03:17.000000 contextualbandits-0.3.9/setup.py
```

### Comparing `contextualbandits-0.3.8/README.md` & `contextualbandits-0.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 * Added new online method `ParametricTS`.
 * Added option for `ExploreFirst` to make choices using active learning.
 * Updated the online example notebook for better results with both full-refit and streaming-mode versions after the latest additions.
 * Added a `random_state` parameter to the methods for getting reproducible results.
 * Added option to use base classifier's `warm_start` if available (for faster model fitting).
 * Added functionality for `refit_buffer` in the batch/streaming train mode (see docs for details).
 * Added a linear regression class which keeps the matrices used for the closed-form solution, so that it can be fit incrementally while giving the same solution as if fitted to all data at once.
+* LinTS and LogisticTS are faster to maker predictions due to pre-computing some of the necessary steps after fitting.
 * LinUCB speed has been improved by taking more efficient matrix operation routes and using Cython code.
 
 
 ## Implemented algorithms
 
 Methods in this package include:
```

### Comparing `contextualbandits-0.3.8/contextualbandits/_cy_utils.pyx` & `contextualbandits-0.3.9/contextualbandits/_cy_utils.pyx`

 * *Files identical despite different names*

### Comparing `contextualbandits-0.3.8/contextualbandits/cy_cpp_helpers.cpp` & `contextualbandits-0.3.9/contextualbandits/cy_cpp_helpers.cpp`

 * *Files identical despite different names*

### Comparing `contextualbandits-0.3.8/contextualbandits/evaluation.py` & `contextualbandits-0.3.9/contextualbandits/evaluation.py`

 * *Files identical despite different names*

### Comparing `contextualbandits-0.3.8/contextualbandits/linreg/__init__.py` & `contextualbandits-0.3.9/contextualbandits/offpolicy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,502 +1,400 @@
+# -*- coding: utf-8 -*-
+
 import numpy as np
-import ctypes
-from scipy.sparse import issparse, isspmatrix_csr
-import warnings
-from sklearn.base import BaseEstimator
-from . import _wrapper_double, _wrapper_float
+from .utils import _check_constructor_input, _check_fit_input, \
+    _check_X_input, _check_1d_inp, _check_beta_prior, _check_smoothing, \
+    _check_njobs, _check_random_state, _OnePredictor, _ZeroPredictor, _RandomPredictor
+from .online import SeparateClassifiers
+from copy import deepcopy
+from joblib import Parallel, delayed
 
+__all__ = ["DoublyRobustEstimator", "OffsetTree"]
 
-class LinearRegression(BaseEstimator):
+class DoublyRobustEstimator:
     """
-    Linear Regression
+    Doubly-Robust Estimator
+    
+    Estimates the expected reward for each arm, applies a correction for the actions that
+    were chosen, and converts the problem to const-sensitive classification, on which the
+    base algorithm is then fit.
     
-    Typical Linear Regression model, which keeps track of the aggregated data
-    needed to obtain the closed-form solution in a way that calling 'partial_fit'
-    multiple times would be equivalent to a single call to 'fit' with all the data.
-
     Note
     ----
-    Doing linear regression this way requires both memory and computation time
-    which scale quadratically with the number of columns/features/variables. As
-    such, the class will by default use C 'float' types (typically ``np.float32``)
-    instead of C 'double' (``np.float64``), in order to save memory.
-
+    This technique converts the problem into a cost-sensitive classification problem
+    by calculating a matrix of expected rewards and turning it into costs. The base
+    algorithm is then fit to this data, using either the Weighted All-Pairs approach,
+    which requires a binary classifier with sample weights as base algorithm, or the
+    Regression One-Vs-Rest approach, which requires a regressor as base algorithm.
+    
+    In the Weighted All-Pairs approach, this technique will fail if there are actions that
+    were never taken by the exploration policy, as it cannot construct a model for them.
+    
+    The expected rewards are estimated with the imputer algorithm passed here, which should
+    output a number in the range [0,1].
+    
+    This technique is meant for the case of contiunous rewards in the [0,1] interval,
+    but here it is used for the case of discrete rewards {0,1}, under which it performs
+    poorly. It is not recommended to use, but provided for comparison purposes.
+    
+    
+    Alo important: this method requires to form reward estimates of all arms for each observation. In order to
+    do so, you can either provide estimates as an array (see Parameters), or pass a model.
+    
+    One method to obtain reward estimates is to fit a model to the data and use its predictions as
+    reward estimates. You can do so by passing an object of class
+    `contextualbandits.online.SeparateClassifiers` which should be already fitted, or by passing a
+    classifier with a 'predict_proba' method, which will be put into a 'SeparateClassifiers'
+     object and fit to the same data passed to this function to obtain reward estimates.
+    
+    The estimates can make invalid predictions if there are some arms for which every time
+    they were chosen they resulted in a reward, or never resulted in a reward. In such cases,
+    this function includes the option to impute the "predictions" for them (which would otherwise
+    always be exactly zero or one regardless of the context) by replacing them with random
+    numbers ~Beta(3,1) or ~Beta(1,3) for the cases of always good and always bad.
+    
+    This is just a wild idea though, and doesn't guarantee reasonable results in such siutation.
+    
+    Note that, if you are using the 'SeparateClassifiers' class from the online module in this
+    same package, it comes with a method 'predict_proba_separate' that can be used to get reward
+    estimates. It still can suffer from the same problem of always-one and always-zero predictions though.
+    
     Parameters
     ----------
-    lambda_ : float
-        Strenght of the L2 regularization.
-    fit_intercept : bool
-        Whether to add an intercept term to the formula. If passing 'True', it will
-        be the last entry in the coefficients.
-    method : str, one of 'chol' or 'sm'
-        Method used to fit the model. Options are:
-
-        ``'chol'``:
-            Uses the Cholesky decomposition to solve the linear system from the
-            least-squares closed-form each time 'fit' or 'partial_fit' is called.
-            This is likely to be faster when fitting the model to a large number
-            of observations at once, and is able to better exploit multi-threading.
-        ``'sm'``:
-            Starts with an inverse diagonal matrix and updates it as each
-            new observation comes using the Sherman-Morrison formula, thus
-            never explicitly solving the linear system, nor needing to calculate
-            a matrix inverse. This is likely to be faster when fitting the model
-            to small batches of observations. Be aware that with this method, it
-            will add regularization to the intercept if passing 'fit_intercept=True'.
-
-        Note that it is possible to change the method after the object has
-        already been fit (e.g. if you want non-regularization intercept
-        with fast online updates, you might use Cholesky first and then switch
-        to Sherman-Morrison).
-    calc_inv : bool
-        When using ``method='chol'``, whether to also produce a matrix inverse, which
-        is required for using the LinUCB and LinTS prediction modes. Ignored when
-        passing ``method='sm'`` (the default). Note that is is possible to change
-        the method after the object has already been fit.
-    use_float : bool
-        Whether to use C 'float' type for the required matrices. If passing 'False',
-        will use C 'double'. Be aware that memory usage for this model can grow
-        very large. Can be changed after initialization.
-    copy_X : bool
-        Whether to make deep copies of the 'X' input passed to the model's methods.
-        If passing 'False', the 'X' object might be modified in-place. Note that
-        if passing 'False', passing 'X' which is a non-contiguous subset of a
-        larger array (e.g. 'X[:10, :100]') might provide the wrong results.
-
-    Attributes
+    base_algorithm : obj
+        Base algorithm to be used for cost-sensitive classification.
+    reward_estimator : obj or array (n_samples, n_choices)
+        One of the following:
+            * An array with the first column corresponding to the reward estimates for the action chosen
+              by the new policy, and the second column corresponding to the reward estimates for the
+              action chosen in the data (see Note for details).
+            * An already-fit object of class 'contextualbandits.online.SeparateClassifiers', which will
+              be used to make predictions on the actions chosen and the actions that the new
+              policy would choose.
+            * A classifier with a 'predict_proba' method, which will be fit to the same test data
+              passed here in order to obtain reward estimates (see Note 2 for details).
+    nchoices : int
+        Number of arms/labels to choose from.
+        Only used when passing a classifier object to 'reward_estimator'.
+    method : str, either 'rovr' or 'wap'
+        Whether to use Regression One-Vs-Rest or Weighted All-Pairs (see Note 1)
+    handle_invalid : bool
+        Whether to replace 0/1 estimated rewards with randomly-generated numbers (see Note 2)
+    random_state : int, None, RandomState, or Generator
+        Either an integer which will be used as seed for initializing a
+        ``Generator`` object for random number generation, a ``RandomState``
+        object (from NumPy) from which to draw an integer, or a ``Generator``
+        object (from NumPy), which will be used directly.
+        This is used when passing ``handle_invalid=True`` or ``beta_prior != None``.
+    c : None or float
+        Constant by which to multiply all scores from the exploration policy.
+    pmin : None or float
+        Scores (from the exploration policy) will be converted to the minimum between
+        pmin and the original estimate.
+    beta_prior : tuple((a, b), n), str "auto", or None
+        Beta prior to pass to 'SeparateClassifiers'. Only used when passing to
+        'reward_estimator' a classifier with 'predict_proba'. See the documentation
+        of 'SeparateClassifiers' for details about it.
+    smoothing : tuple(a, b), list, or None
+        Smoothing parameter to pass to ``SeparateClassifiers``. Only used when passing to 'reward_estimator'
+        a classifier with 'predict_proba'. See the documentation of ``SeparateClassifiers`` for details.
+    njobs : int or None
+        Number of parallel jobs to run. If passing None will set it to 1. If passing -1 will
+        set it to the number of CPU cores.
+    kwargs_costsens
+        Additional keyword arguments to pass to the cost-sensitive classifier.
+    
+    References
     ----------
-    coef_ : array(n) or array(n+1)
-        The obtained coefficients. If passing 'fit_intercept=True', the intercept
-        will be at the last entry.
+    .. [1] Dudík, Miroslav, John Langford, and Lihong Li. "Doubly robust policy evaluation and learning."
+           arXiv preprint arXiv:1103.4601 (2011).
+    .. [2] Dudík, Miroslav, et al. "Doubly robust policy evaluation and optimization."
+           Statistical Science 29.4 (2014): 485-511.
     """
-    def __init__(self, lambda_=1., fit_intercept=True, method="sm", calc_inv=True,
-                 use_float=True, copy_X=True):
-        self.lambda_ = lambda_
-        self.fit_intercept = fit_intercept
-        self._method = method
-        self._calc_inv = bool(calc_inv)
-        self._use_float = bool(use_float)
-        self.copy_X = bool(copy_X)
-
-        self._set_dtype(force_cast=False)
-        self.coef_ = np.empty(0, dtype=self._dtype)
-        self._XtX = np.empty((0,0), dtype=self._dtype)
-        self._invXtX = np.empty((0,0), dtype=self._dtype)
-        self._XtY = np.empty(0, dtype=self._dtype)
-        self._bufferX = np.empty(0, dtype=self._dtype)
-        self._n = 0
-
-        self.is_fitted_ = False
-
-    def _set_dtype(self, force_cast=False):
-        self._dtype = ctypes.c_float if self._use_float else ctypes.c_double
-
-        if force_cast:
-            if self.coef_.dtype != self._dtype:
-                self.coef_ = self.coef_.astype(self._dtype)
-            if self._XtX.dtype != self._dtype:
-                self._XtX = self._XtX.astype(self._dtype)
-            if self._invXtX.dtype != self._dtype:
-                self._invXtX = self._invXtX.astype(self._dtype)
-            if self._XtY.dtype != self._dtype:
-                self._XtY = self._XtY.astype(self._dtype)
-            if self._bufferX.dtype != self._dtype:
-                self._bufferX = self._bufferX.astype(self._dtype)
-
-    @property
-    def use_float(self):
-        return self._use_float
-    @use_float.setter
-    def use_float(self, value):
-        self._use_float = use_float
-        self._set_dtype(force_cast=True)
-
-    @property
-    def method(self):
-        return self._method
-    
-    @method.setter
-    def method(self, value):
-        assert value in ["chol", "sm"]
-        if self._method != value:
-            cy_funs = _wrapper_float if self._use_float else _wrapper_double
-            if self._method == "sm":
-                self._XtX = np.empty(self._invXtX.shape, dtype=self._dtype)
-                cy_funs.get_matrix_inv(self._invXtX, self._XtX)
-            elif (not self._calc_inv):
-                self._invXtX = np.empty(self._XtX.shape, dtype=self._dtype)
-                cy_funs.get_matrix_inv(self._XtX, self._invXtX)
-                self._calc_inv = True
-        self._method = value
-
-    @property
-    def calc_inv(self):
-        return self._calc_inv
-    
-    @calc_inv.setter
-    def calc_inv(self, value):
-        if bool(value) != self._calc_inv:
-            if self._method == "chol":
-                self._invXtX = np.empty(self._XtX.shape, dtype=self._dtype)
-                cy_funs.get_matrix_inv(self._XtX, self._invXtX)
-            self._calc_inv = bool(value)
-
-
-    def _process_X_y_w(self, X, y, sample_weight, only_X=False):
-        if X.dtype != self._dtype:
-            X = X.astype(self._dtype)
-        if not issparse(X):
-            Xcsr = None
-            if X.__class__.__name__ == "DataFrame":
-                X = X.to_numpy()
-            if self.copy_X:
-                X = X.copy()
-            X = np.array(X)
-            if len(X.shape) != 2:
-                raise ValueError("'X' must be 2-dimensional")
+    def __init__(self, base_algorithm, reward_estimator, nchoices, method='rovr',
+                 handle_invalid=True, random_state=1, c=None, pmin=1e-5,
+                 beta_prior=None, smoothing=(1.,2.), njobs=-1, **kwargs_costsens):
+        assert (method == 'rovr') or (method == 'wap')
+        self.method = method
+        if method == 'wap':
+            _check_constructor_input(base_algorithm, nchoices)
         else:
-            if not isspmatrix_csr(X):
-                warnings.warn("Sparse matrices only supported in CSR format. Input will be converted.")
-                X = csr_matrix(X)
-            Xcsr = X.copy()
-            X = np.empty((0,0), dtype=self._dtype)
-            if len(Xcsr.shape) != 2:
-                raise ValueError("'X' must be 2-dimensional")
-        if only_X:
-            return X, Xcsr
-
-        if issparse(y):
-            raise ValueError("Sparse 'y' not supported.")
-        if issparse(sample_weight):
-            raise ValueError("Sparse 'sample_weight' not supported.")
-
-        y = np.array(y).reshape(-1)
-        if sample_weight is None:
-            w = np.empty(0, dtype=self._dtype)
+            assert isinstance(nchoices, int)
+            assert nchoices > 2
+            assert ('fit' in dir(base_algorithm)) and ('predict' in dir(base_algorithm))
+        
+        if c is not None:
+            assert isinstance(c, float)
+        if pmin is not None:
+            assert isinstance(pmin, float)
+        assert isinstance(handle_invalid, bool)
+        
+        if type(reward_estimator) == np.ndarray:
+            assert reward_estimator.shape[1] == nchoices
+            assert reward_estimator.shape[0] == X.shape[0]
         else:
-            w = np.array(sample_weight).reshape(-1)
+            assert ('predict_proba_separate' in dir(reward_estimator)) or ('predict_proba' in dir(reward_estimator))
 
-        if self.copy_X:
-            y = y.copy()
-            w = w.copy()
-
-        if Xcsr is None:
-            assert X.shape[0] == y.shape[0]
-        else:
-            if Xcsr.shape[0] != y.shape[0]:
-                raise ValueError("'X' and 'y' must have the same number of rows.")
-
-        if sample_weight is not None:
-            if X.shape[0] != w.shape[0]:
-                raise ValueError("'sample_weight' must have the same number of rows as 'X' and 'y'.")
-
-        if y.dtype != self._dtype:
-            y = y.astype(self._dtype)
-        if w.dtype != self._dtype:
-            w = w.astype(self._dtype)
-
-        return X, Xcsr, y, w
-
-    def fit(self, X, y, sample_weight=None):
+        if beta_prior is not None:
+            beta_prior = _check_beta_prior(beta_prior, nchoices, 2)
+        
+        self.base_algorithm = base_algorithm
+        self.reward_estimator = reward_estimator
+        self.nchoices = nchoices
+        self.c = c
+        self.pmin = pmin
+        self.handle_invalid = handle_invalid
+        self.random_state = _check_random_state(random_state)
+        self.beta_prior = beta_prior
+        self.smoothing = _check_smoothing(smoothing, nchoices)
+        self.njobs = _check_njobs(njobs)
+        self.kwargs_costsens = kwargs_costsens
+        self.is_fitted = False
+    
+    def fit(self, X, a, r, p):
         """
-        Fit model to data
-
-        Note
-        ----
-        Calling 'fit' will reset whatever previous data was there. For fitting
-        the model incrementally to new data, use 'partial_fit' instead.
-
+        Fits the Doubly-Robust estimator to partially-labeled data collected from a different policy.
+        
         Parameters
         ----------
-        X : array(m,n) or CSR matrix(m, n)
-            The covariates.
-        y : array-like(m)
-            The target variable.
-        sample_weight : None or array-like(m)
-            Observation weights for each row.
-
-        Returns
-        -------
-        self
-
+        X : array (n_samples, n_features)
+            Matrix of covariates for the available data.
+        a : array (n_samples), int type
+            Arms or actions that were chosen for each observations.
+        r : array (n_samples), {0,1}
+            Rewards that were observed for the chosen actions. Must be binary rewards 0/1.
+        p : array (n_samples)
+            Reward estimates for the actions that were chosen by the policy.
         """
-        assert self.method in ["chol", "sm"]
-
-        self._n = X.shape[1]
-        X, Xcsr, y, w = self._process_X_y_w(X, y, sample_weight)
-
-        cy_funs = _wrapper_float if self._use_float else _wrapper_double
-        if (self.method == "chol") or (X.shape[0] >= X.shape[1]):
-            self._XtX, self._invXtX, self._XtY, self.coef_ = \
-                cy_funs.fit_model_noinv(
-                    X, y, w, Xcsr,
-                    add_bias=self.fit_intercept,
-                    lam = self.lambda_,
-                    calc_inv=(self.calc_inv) or (self.method != "chol")
-                )
+        try:
+            from costsensitive import RegressionOneVsRest, WeightedAllPairs
+        except:
+            raise ValueError("This functionality requires package 'costsensitive'.\nCan be installed with 'pip install costsensitive'.")
+        p = _check_1d_inp(p)
+        assert p.shape[0] == X.shape[0]
+        l = -r
+        
+        if type(self.reward_estimator) == np.ndarray:
+            C = self.reward_estimator
+        elif 'predict_proba_separate' in dir(self.reward_estimator):
+            C = -self.reward_estimator.predict_proba_separate(X)
+        elif 'predict_proba' in dir(self.reward_estimator):
+            reward_estimator = \
+                SeparateClassifiers(self.reward_estimator, self.nchoices,
+                    beta_prior = self.beta_prior, smoothing = self.smoothing,
+                    random_state = self.random_state, njobs = self.njobs)
+            reward_estimator.fit(X, a, r)
+            C = -reward_estimator.predict_proba_separate(X)
         else:
-            self._invXtX, self._XtY, self.coef_ = \
-                cy_funs.fit_model_inv(
-                    X, y, w, Xcsr,
-                    add_bias=self.fit_intercept,
-                    lam = self.lambda_
-                )
-
-        if self.method != "chol":
-            self._bufferX = np.empty(self._n + int(self.fit_intercept), dtype=self._dtype)
-
-        self.is_fitted_ = True
-        return self
-
-
-    def partial_fit(self, X, y, sample_weight=None, *args, **kwargs):
-        """
-        Fit model incrementally to new data
-
-        Parameters
-        ----------
-        X : array(m,n) or CSR matrix(m, n)
-            The covariates.
-        y : array-like(m)
-            The target variable.
-        sample_weight : None or array-like(m)
-            Observation weights for each row.
-
-        Returns
-        -------
-        self
-
-        """
-        if not self.is_fitted_:
-            return self.fit(X, y, sample_weight)
-
-        if X.shape[1] != self._n:
-            raise ValueError("Number of columns in X doesn't match with previous.")
-        X, Xcsr, y, w = self._process_X_y_w(X, y, sample_weight)
-
-        cy_funs = _wrapper_float if self._use_float else _wrapper_double
-        if self.method == "chol":
-            if self._invXtX.shape[0] == 0:
-                self._invXtX = np.empty((self._XtX.shape[0], self._XtX.shape[1]),
-                                        dtype=ctypes.c_float if self._use_float else ctypes.c_double)
-            cy_funs.update_running_noinv(
-                self._XtX, self._XtY, self._invXtX, self.coef_,
-                X, y, w, Xcsr,
-                add_bias=self.fit_intercept,
-                calc_inv=self.calc_inv
-            )
+            raise ValueError("Error: couldn't obtain reward estimates. Are you passing the right input to 'reward_estimator'?")
+        
+        if self.handle_invalid:
+            C[C >= 1] = self.random_state.beta(3, 1, size = C.shape)[C >= 1]
+            C[C <= 0] = self.random_state.beta(1, 3, size = C.shape)[C <= 0]
+        
+        if self.c is not None:
+            p = self.c * p
+        if self.pmin is not None:
+            p = np.clip(p, a_min = self.pmin, a_max = None)
+        
+        C[np.arange(C.shape[0]), a] += (l - C[np.arange(C.shape[0]), a]) / p.reshape(-1)
+        if self.method == 'rovr':
+            self.oracle = RegressionOneVsRest(self.base_algorithm,
+                                              njobs = self.njobs,
+                                              **self.kwargs_costsens)
         else:
-            if not self._bufferX.shape[0]:
-                self._bufferX = np.empty(self._n + int(self.fit_intercept), dtype=self._dtype)
-            cy_funs.update_running_inv(
-                self._invXtX,
-                self._XtY,
-                self.coef_,
-                self._bufferX,
-                X, y, w, Xcsr,
-                add_bias=self.fit_intercept,
-            )
-        return self
-
+            self.oracle = WeightedAllPairs(self.base_algorithm,
+                                           njobs = self.njobs,
+                                           **self.kwargs_costsens)
+        self.oracle.fit(X, C)
+        self.is_fitted = True
+    
     def predict(self, X):
         """
-        Make predictions on new data
-
+        Predict best arm for new data.
+        
         Parameters
         ----------
-        X : array(m,n) or CSR matrix(m, n)
-            The covariates.
-
+        X : array (n_samples, n_features)
+            New observations for which to choose an action.
+            
         Returns
         -------
-        y_hat : array(m)
-            The predicted values given 'X'.
+        pred : array (n_samples,)
+            Actions chosen by this technique.
         """
-        assert self.is_fitted_
-
-        pred = X.dot(self.coef_[:self._n])
-        if self.fit_intercept:
-            pred[:] += self.coef_[self._n]
-        return pred
-
-    def _multiply_x_A_x(self, X):
-        X, Xcsr = self._process_X_y_w(X, None, None, only_X=True)
-        cy_funs = _wrapper_float if self._use_float else _wrapper_double
-        return cy_funs.x_A_x_batch(X, self._invXtX, Xcsr, self.fit_intercept)
-
-    def predict_ucb(self, X, alpha=1.0, add_unfit_noise=False, random_state=None):
+        assert self.is_fitted
+        X = _check_X_input(X)
+        return self.oracle.predict(X)
+    
+    def decision_function(self, X):
         """
-        Make an upper-bound prediction on new data
-
-        Make a prediction on new data with an upper bound given by the LinUCB
-        formula (be aware that it's not probabilistic like a regular CI).
-
+        Get score distribution for the arm's rewards
+        
         Note
         ----
-        If using this method, it's recommended to center the 'X' data passed
-        to 'fit' and 'partial_fit'. If not centered, it's recommendable to
-        lower the ``alpha`` value.
-
+        For details on how this is calculated, see the documentation of the
+        RegressionOneVsRest and WeightedAllPairs classes in the costsensitive package.
+        
         Parameters
         ----------
-        X : array(m,n) or CSR matrix(m, n)
-            The covariates.
-        alpha : float > 0 or array(m, ) > 0
-            The multiplier for the width of the bound. Can also pass an array
-            with different values for each row.
-        add_unfit_noise : bool
-            When making predictions with an unfit model (in this case they are
-            given by empty zero matrices except for the inverse diagonal matrix
-            based on the regularization parameter), whether to add a very small
-            amount of random noise ~ Uniform(0, 10^-12) to it. This is useful in
-            order to break ties at random when using multiple models.
-        random_state : None, np.random.Generator, or np.random.RandomState
-            A NumPy 'Generator' or 'RandomState' object instance to use for generating
-            random numbers. If passing 'None', will use NumPy's random
-            module directly (which can be made reproducible through
-            ``np.random.seed``). Only used when passing ``add_unfit_noise=True``
-            and calling this method on a model that has not been fit to data.
-
+        X : array (n_samples, n_features)
+            New observations for which to evaluate actions.
+            
         Returns
         -------
-        y_hat : array(m)
-            The predicted upper bound on 'y' given 'X' and ``alpha``.
-
-        References
+        pred : array (n_samples, n_choices)
+            Score assigned to each arm for each observation (see Note).
+        """
+        assert self.is_fitted
+        X = _check_X_input(X)
+        return self.oracle.decision_function(X)
+    
+    
+class OffsetTree:
+    """
+    Offset Tree
+    
+    Parameters
+    ----------
+    base_algorithm : obj
+        Binary classifier to be used for each classification sub-problem in the tree.
+    nchoices : int
+        Number of arms/labels to choose from.
+    c : None or float
+        Constant by which to multiply all scores from the exploration policy.
+    pmin : None or float
+        Scores (from the exploration policy) will be converted to the minimum between
+        pmin and the original estimate.
+    random_state : int, None, RandomState, or Generator
+        Either an integer which will be used as seed for initializing a
+        ``Generator`` object for random number generation, a ``RandomState``
+        object (from NumPy) from which to draw an integer, or a ``Generator``
+        object (from NumPy), which will be used directly.
+        This is used when predictions need to be done for an arm with no data.
+    njobs : int or None
+        Number of parallel jobs to run. If passing None will set it to 1. If passing -1 will
+        set it to the number of CPU cores. Note that if the base algorithm is itself parallelized,
+        this might result in a slowdown as both compete for available threads, so don't set
+        parallelization in both.
+    
+    References
+    ----------
+    .. [1] Beygelzimer, Alina, and John Langford. "The offset tree for learning with partial labels."
+           Proceedings of the 15th ACM SIGKDD international conference on Knowledge discovery and data mining. ACM, 2009.
+    """
+    def __init__(self, base_algorithm, nchoices, c = None, pmin = 1e-5,
+                 random_state = 1, njobs = -1):
+        try:
+            from costsensitive import _BinTree
+        except:
+            raise ValueError("This functionality requires package 'costsensitive'.\nCan be installed with 'pip install costsensitive'.")
+        _check_constructor_input(base_algorithm, nchoices)
+        self.base_algorithm = base_algorithm
+        self.nchoices = nchoices
+        self.tree = _BinTree(nchoices)
+        if c is not None:
+            assert isinstance(c, float)
+        if pmin is not None:
+            assert isinstance(pmin, float)
+        self.c = c
+        self.pmin = pmin
+        self.random_state = _check_random_state(random_state)
+        self.njobs = _check_njobs(njobs)
+        self.is_fitted = False
+    
+    def fit(self, X, a, r, p):
+        """
+        Fits the Offset Tree estimator to partially-labeled data collected from a different policy.
+        
+        Parameters
         ----------
-        .. [1] Chu, Wei, et al. "Contextual bandits with linear payoff functions."
-               Proceedings of the Fourteenth International Conference on Artificial Intelligence and Statistics. 2011.
+        X : array (n_samples, n_features)
+            Matrix of covariates for the available data.
+        a : array (n_samples), int type
+            Arms or actions that were chosen for each observations.
+        r : array (n_samples), {0,1}
+            Rewards that were observed for the chosen actions. Must be binary rewards 0/1.
+        p : array (n_samples)
+            Reward estimates for the actions that were chosen by the policy.
         """
-        if not isinstance(alpha, np.ndarray):
-            assert alpha > 0.
-            if isinstance(alpha, int):
-                alpha = float(alpha)
-            assert isinstance(alpha, float)
+        X, a, r = _check_fit_input(X, a, r)
+        p = _check_1d_inp(p)
+        assert p.shape[0] == X.shape[0]
+        
+        if self.c is not None:
+            p = self.c * p
+        if self.pmin is not None:
+            p = np.clip(p, a_min = self.pmin, a_max = None)
+        
+        self._oracles = [deepcopy(self.base_algorithm) for c in range(self.nchoices - 1)]
+        rs = self.random_state.integers(np.iinfo(np.int32).max, size=self.nchoices)
+        Parallel(n_jobs=self.njobs, verbose=0, require="sharedmem")\
+                (delayed(self._fit)(classif, X, a, r, p, rs) \
+                    for classif in range(len(self._oracles)))
+        self.is_fitted = True
+
+    def _fit(self, classif, X, a, r, p, rs):
+        obs_take = np.in1d(a, self.tree.node_comparisons[classif][0])
+        X_node = X[obs_take, :]
+        a_node = a[obs_take]
+        r_node = r[obs_take]
+        p_node = p[obs_take]
+        
+        r_more_onehalf = r_node >= .5
+        y = (  np.in1d(a_node, self.tree.node_comparisons[classif][2])  ).astype('uint8')
+        
+        y_node = y.copy()
+        y_node[r_more_onehalf] = 1. - y[r_more_onehalf]
+        w_node = (.5 - r_node) / p_node
+        w_node[r_more_onehalf] = (  (r_node - .5) / p_node  )[r_more_onehalf]
+        w_node = w_node * (w_node.shape[0] / np.sum(w_node))
+        
+        n_pos = y_node.sum()
+        if y_node.shape[0] == 0:
+            self._oracles[classif] = _RandomPredictor(_check_random_state(rs[classif]))
+        elif n_pos == y_node.shape[0]:
+            self._oracles[classif] = _OnePredictor()
+        elif n_pos == 0:
+            self._oracles[classif] = _ZeroPredictor()
         else:
-            assert alpha.shape[0] == X.shape[0]
-
-        if (self.method == "chol") and (not self.calc_inv):
-            raise ValueError("Not available when using 'method=\"chol\"' and 'calc_inv=False'.")
-
-        if not self.is_fitted_:
-            pred = alpha * np.sqrt(np.einsum("ij,ij->i", X, X) / self.lambda_)
-            if add_unfit_noise:
-                if random_state is None:
-                    noise = np.random.uniform(low=0., high=1e-12, size=X.shape[0])
-                else:
-                    noise = random_state.uniform(low=0., high=1e-12, size=X.shape[0])
-                pred[:] += noise
-            return pred
-
-        pred = self.predict(X)
-        ci = self._multiply_x_A_x(X)
-        pred[:] += alpha * np.sqrt(ci)
-        return pred
-
-    def predict_thompson(self, X, v_sq=1.0, sample_unique=False, random_state=None):
+            self._oracles[classif].fit(X_node, y_node, sample_weight = w_node)
+            
+    def predict(self, X):
         """
-        Make a guess prediction on new data
-
-        Make a prediction on new data with coefficients sampled from their
-        estimated distribution.
-
+        Predict best arm for new data.
+        
         Note
         ----
-        If using this method, it's recommended to center the 'X' data passed
-        to 'fit' and 'partial_fit'. If not centered, it's recommendable to
-        lower the ``v_sq`` value.
-
-        Note
-        ----
-        It's highly recommended to use ``method="chol"`` if using this functionality.
-
+        While in theory, making predictions from this algorithm should be faster than from others,
+        the implementation here uses a Python loop for each observation, which is slow compared to
+        NumPy array lookups, so the predictions will be slower to calculate than those from other algorithms.
+        
         Parameters
         ----------
-        X : array(m,n) or CSR matrix(m, n)
-            The covariates.
-        v_sq : float > 0
-            The multiplier for the covariance matrix. Larger values lead to
-            more variable results.
-        sample_unique : bool
-            Whether to sample different coefficients each time a prediction is to
-            be made. If passing 'False', when calling 'predict', it will sample
-            the same coefficients for all the observations in the same call to
-            'predict', whereas if passing 'True', will use a different set of
-            coefficients for each observations. Passing 'False' leads to an
-            approach which is theoretically wrong, but as sampling coefficients
-            can be very slow, using 'False' can provide a reasonable speed up
-            without much of a performance penalty.
-        random_state : None, np.random.Generator, or np.random.RandomState
-            A NumPy 'Generator' or 'RandomState' object instance to use for generating
-            random numbers. If passing 'None', will use NumPy's random
-            module directly (which can be made reproducible through
-            ``np.random.seed``).
-
+        X : array (n_samples, n_features)
+            New observations for which to choose an action.
+            
         Returns
         -------
-        y_hat : array(m)
-            The predicted guess on 'y' given 'X' and ``v_sq``.
-
-        References
-        ----------
-        .. [1] Agrawal, Shipra, and Navin Goyal.
-               "Thompson sampling for contextual bandits with linear payoffs."
-               International Conference on Machine Learning. 2013.
+        pred : array (n_samples,)
+            Actions chosen by this technique.
         """
-        assert self.is_fitted_
-        if X.shape[1] != (self.coef_.shape[0]-int(self.fit_intercept)):
-            raise ValueError("'X' has wrong number of columns.")
-        assert v_sq > 0.
-        if isinstance(v_sq, int):
-            v_sq = float(v_sq)
-        assert isinstance(v_sq, float)
-
-        cy_funs = _wrapper_float if self._use_float else _wrapper_double
-        random_state = np.random if random_state is None else random_state
-
-        if self.method != "chol":
-            tol = 1e-20
-            if np.linalg.det(self._invXtX) >= tol:
-                cov = self._invXtX
-            else:
-                cov = self._invXtX.copy()
-                n = cov.shape[1]
-                for i in range(10):
-                    cov[np.arange(n), np.arange(n)] += 1e-1
-                    if np.linalg.det(cov) >= tol:
-                        break
-                np.nan_to_num(cov, copy=False)
-
-
+        assert self.is_fitted
+        X = _check_X_input(X)
+        pred = np.empty(X.shape[0], dtype=int)
+        for i in range(X.shape[0]):
+            pred[i] = self._predict(i, X)
+        return pred
 
-        if sample_unique:
-            if self.method != "chol":
-                coef = random_state.multivariate_normal(mean=self.coef_,
-                                                        cov=v_sq * cov,
-                                                        size=X.shape[0])
+    def _predict(self, i, X):
+        curr_node = 0
+        X_this = X[i].reshape((1,-1))
+        while True:
+            go_right = self._oracles[curr_node].predict(X_this)
+            if go_right:
+                curr_node = self.tree.childs[curr_node][0]
             else:
-                coef = cy_funs.mvnorm_from_invcov(self.coef_,
-                                                  (1./v_sq) * self._XtX,
-                                                  size=X.shape[0],
-                                                  rng=random_state)
-            if not issparse(X):
-                pred = np.einsum("ij,ij->i", X, coef[:,:X.shape[1]])
-            else:
-                pred = X.multiply(coef[:,:X.shape[1]]).sum(axis=1)
-            if self.fit_intercept:
-                pred[:] += coef[:,-1]
-        else:
-            if self.method != "chol":
-                coef = random_state.multivariate_normal(mean=self.coef_,
-                                                        cov=v_sq * cov)
-            else:
-                coef = cy_funs.mvnorm_from_invcov(self.coef_,
-                                                  (1./v_sq) * self._XtX,
-                                                  size=1,
-                                                  rng=random_state)
-                coef = coef.reshape(-1)
-            pred = X.dot(coef[:X.shape[1]])
-            if self.fit_intercept:
-                pred[:] += coef[-1]
-
-        return pred
+                curr_node = self.tree.childs[curr_node][1]
+                
+            if curr_node <= 0:
+                return -curr_node
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `contextualbandits-0.3.8/contextualbandits/linreg/linreg_untyped.pxi` & `contextualbandits-0.3.9/contextualbandits/linreg/linreg_untyped.pxi`

 * *Files 5% similar despite different names*

```diff
@@ -741,14 +741,105 @@
     cdef int ignore = 0
     cdef char lo = 'L'
     with nogil:
         memcpy(ptr_invX, ptr_X, <size_t>(X.shape[0]*X.shape[1])*sizeof(realtp))
         tpotrf(&lo, &n, ptr_invX, &n, &ignore)
         tpotri(&lo, &n, ptr_invX, &n, &ignore)
 
+### https://stats.stackexchange.com/questions/175271/can-i-get-a-cholesky-decomposition-from-the-inverse-of-a-matrix
+### Sampling from multivariate normal N(mu, Sigma):
+### - Sample Y[n,m] ~ N(0,1)
+### - Convert to desired distribution by transforming:
+###      A = EigVec(Sigma) * diag(sqrt(EigVal(Sigma)))
+###      z = mu + Y * A
+#### (If using the inverse of Sigma, the eigen vectors are the same,
+####  while the eigen values are 1 divided over the eigen values of the inverse)
+def get_mvnorm_multiplier(
+        np.ndarray[realtp, ndim=2] Sigma,
+        realtp multiplier,
+        bint is_inverse,
+        bint overwrite_sigma
+    ):
+
+    Sigma = np.require(Sigma, dtype=C_realtp, requirements=["C_CONTIGUOUS", "OWNDATA"])
+    cdef int m = Sigma.shape[0]
+    cdef np.ndarray[realtp, ndim=2] eig_Vecs = np.empty((0,0), dtype=C_realtp)
+    if overwrite_sigma:
+        eig_Vecs = Sigma
+    else:
+        eig_Vecs = Sigma.copy()
+    cdef np.ndarray[realtp, ndim=1] eig_vals = np.empty(m, dtype=C_realtp)
+    cdef realtp *ptr_Ev = &eig_Vecs[0,0]
+    cdef realtp *ptr_ev = &eig_vals[0]
+
+    cdef char lo = 'L'
+    cdef int one = 1
+    cdef int minus_one = -1
+    cdef char V = 'V'
+    cdef int ignore
+    cdef realtp size_buffer
+
+    tsyev(&V, &lo, &m, ptr_Ev, &m, ptr_ev, &size_buffer, &minus_one, &ignore)
+    cdef int size_buffer_as_int = int(size_buffer)
+    cdef np.ndarray[realtp, ndim=1] buffer_arr = np.empty(size_buffer_as_int, dtype=C_realtp)
+    tsyev(&V, &lo, &m, ptr_Ev, &m, ptr_ev, &buffer_arr[0], &size_buffer_as_int, &ignore)
+
+    ### Note: the obtained eigen values are transposed at this point as they were passed
+    ### assuming column-major (input was a symmetric matrix so it doesn't matter).
+    ### If doing the rest of this part in C, would have to use tscal with incX given by
+    ### the number of columns
+
+    ### Note2: If multiplying the input matrix by a constant, the eigen vectors
+    ### remain the same, while the eigen values get multiplied by that same constant
+    if is_inverse:
+        ix_replace = eig_vals <= 1e-10
+        eig_vals[ix_replace] = 1.
+        eig_vals[:] =  1. / eig_vals
+        eig_vals[ix_replace] = 0.
+    eig_vals[:] = eig_vals.clip(min=0.)
+    eig_vals_orig = eig_vals.copy()
+    eig_vals[:] =  np.sqrt(multiplier * eig_vals)
+
+    return np.einsum("ij,i->ij", eig_Vecs, eig_vals), eig_vals, eig_vals_orig
+
+
+def mvnorm_from_Eig(
+        np.ndarray[realtp, ndim=1] mu,
+        np.ndarray[realtp, ndim=2] EigMultiplier,
+        size_t n,
+        rng
+    ):
+    cdef size_t m = EigMultiplier.shape[0]
+    cdef np.ndarray[realtp, ndim=2] X = np.empty((0,0), dtype=C_realtp)
+    if isinstance(rng, np.random.Generator):
+        X = rng.standard_normal(size=(n, m), dtype=C_realtp)
+    else:
+        X = rng.normal(size=(n, m), dtype=C_realtp).astype(C_realtp)
+    return mu + X.dot(EigMultiplier)
+
+
+def mvnorm_from_Eig_different_m(
+        np.ndarray[realtp, ndim=1] mu,
+        np.ndarray[realtp, ndim=2] EigMultiplier,
+        np.ndarray[realtp, ndim=1] eig_vals_multiplied,
+        np.ndarray[realtp, ndim=1] eig_vals_orig,
+        realtp new_m,
+        size_t n,
+        rng,
+        bint return_multiplier
+    ):
+    new_EigMultiplier = EigMultiplier / eig_vals_multiplied.reshape((-1,1))
+    new_EigMultiplier = np.einsum("ij,i->ij",
+                                  new_EigMultiplier,
+                                  np.sqrt(new_m * eig_vals_orig))
+    if return_multiplier:
+        return new_EigMultiplier, np.sqrt(new_m * eig_vals_orig)
+    else:
+        return mvnorm_from_Eig(mu, new_EigMultiplier, n, rng)
+
 ## https://stats.stackexchange.com/questions/175271/can-i-get-a-cholesky-decomposition-from-the-inverse-of-a-matrix
 def mvnorm_from_invcov(
         np.ndarray[realtp, ndim=1] mu,
         np.ndarray[realtp, ndim=2] invSigma,
         size_t size,
         rng
     ):
```

### Comparing `contextualbandits-0.3.8/contextualbandits/online.py` & `contextualbandits-0.3.9/contextualbandits/online.py`

 * *Files 1% similar despite different names*

```diff
@@ -1074,15 +1074,16 @@
     Logistic regression classifier which either samples its coefficients using
     the variance-covariance matrix of the predictors, or which samples
     predicted values from a confidence interval as a faster alternative.
 
     Note
     ----
     This strategy is implemented for comparison purposes only and it's not
-    recommended to rely on it, particularly not for large datasets.
+    recommended to rely on it, particularly not for large datasets. Performance
+    tends to be very bad compared to the other methods provided here.
 
     Note
     ----
     This strategy does not support fitting the data in batches ('partial_fit'
     will not be available), nor does it support using any other classifier.
     See 'BootstrappedTS' for a more generalizable version.
 
@@ -1112,28 +1113,37 @@
         Whether to construct a confidence interval on arms with no observations
         according to a variance-covariance matrix given by the regulatization
         parameter alone.
         Ignored when passing ``sample_from='coef'``.
     multiplier : float
         Multiplier for the covariance matrix. Pass 1 to take it as-is.
         Ignored when passing ``sample_from='ci'``.
+    n_presampled : None or int
+        If sampling from coefficients, this denotes a number of coefficients to pre-sample
+        after calling 'fit', which will be used later in the predictions. Pre-sampling
+        a large number of coefficients can help to speed up predictions at the expense
+        of longer fitting times, and is recommended if there is a large number of predictions
+        between calls to 'fit'.
+        If passing 'None' (the default), will not pre-sample a finite number of the coefficients
+        at fitting time, but will rather sample (different) coefficients in calls to 'predict'.
+        Ignored when passing ``sample_from="ci"``.
     fit_intercept : bool
         Whether to add an intercept term to the models.
     lambda_ : float
         Strenght of the L2 regularization. Must be greater than zero.
     sample_unique : bool
         Whether to sample different coefficients each time a prediction is to
         be made. If passing 'False', when calling 'predict', it will sample
         the same coefficients for all the observations in the same call to
         'predict', whereas if passing 'True', will use a different set of
-        coefficients for each observations. Passing 'False' leads to an
+        coefficients for each observation/row. Passing 'False' leads to an
         approach which is theoretically wrong, but as sampling coefficients
         can be very slow, using 'False' can provide a reasonable speed up
         without much of a performance penalty.
-        Ignored when passing ``sample_from='ci'``.
+        Ignored when passing ``sample_from='ci'`` or ``n_presampled``.
     beta_prior : str 'auto', None, tuple ((a,b), n), or list[tuple((a,b), n)]
         If not 'None', when there are less than 'n' samples with and without
         a reward from a given arm, it will predict the score for that class as a
         random number drawn from a beta distribution with the prior
         specified by 'a' and 'b'. If set to "auto", will be calculated as:
             beta_prior = ((2/log2(nchoices), 4), 2)
         Can also pass different priors per arm, in which case they should be passed
@@ -1176,30 +1186,34 @@
         as both functions compete for available threads.
 
     References
     ----------
     .. [1] Cortes, David. "Adapting multi-armed bandits policies to contextual bandits scenarios."
            arXiv preprint arXiv:1811.04383 (2018).
     """
-    def __init__(self, nchoices, sample_from="ci", ci_from_empty=False, multiplier=0.1,
-                 fit_intercept=True, lambda_=1.0, sample_unique=False,
+    def __init__(self, nchoices, sample_from="ci", ci_from_empty=False,
+                 multiplier=0.25, n_presampled=None,
+                 fit_intercept=True, lambda_=1.0, sample_unique=True,
                  beta_prior='auto', smoothing=None, noise_to_smooth=True,
                  assume_unique_reward=False, random_state=None, njobs=-1):
-        warnings.warn("This class is experimental. Not recommended to rely on it.")
         assert sample_from in ["ci", "coef"]
         self.sample_from = sample_from
         assert lambda_ > 0.
         assert multiplier > 0.
+        if n_presampled is not None:
+            assert n_presampled > 0
+            assert isinstance(n_presampled, int)
         base = _LogisticUCB_n_TS_single(lambda_=lambda_,
                                         fit_intercept=fit_intercept,
                                         alpha=0.,
                                         m=multiplier,
                                         ts=True,
                                         ts_from_ci = (sample_from == "ci"),
-                                        sample_unique=sample_unique)
+                                        sample_unique=sample_unique,
+                                        n_presampled=n_presampled)
         self._add_common_params(base, beta_prior, smoothing, noise_to_smooth, njobs, nchoices,
                                 False, None, False, assume_unique_reward,
                                 random_state, assign_algo=True, prior_def_ucb=False,
                                 force_unfit_predict=(ci_from_empty) and (sample_from == "ci"))
 
 class SeparateClassifiers(_BasePolicy):
     """
@@ -2305,15 +2319,15 @@
                 pred = self.random_state.integers(self.nchoices, size = X.shape[0])
                 self._choose_active(X, pred)
                 return pred
             
             # case 2: some predictions are within allowance, others are not
             else:
                 n_explore = self.explore_rounds - self.explore_cnt + X.shape[0]
-                pred = np.empty(X.shape[0], type = ctypes.c_double)
+                pred = np.empty(X.shape[0], dtype = ctypes.c_double)
                 pred[:n_explore] = self.random_state.integers(self.nchoices, n_explore)
                 self._choose_active(X[:n_explore], pred[:n_explore])
                 pred[n_explore:] = self._oracles.predict(X[n_explore:])
                 return pred
         else:
             return self._oracles.predict(X)
 
@@ -2324,15 +2338,15 @@
             # case 1: all predictions are within allowance
             if self.explore_cnt <= self.explore_rounds:
                 scores = self.random_state.random(size=(X.shape[0], self.nchoices))
                 self._choose_active(X, scores, choose=False)
             
             # case 2: some predictions are within allowance, others are not
             else:
-                scores = np.empty((X.shape[0], self.nchoices), type = ctypes.c_double)
+                scores = np.empty((X.shape[0], self.nchoices), dtype = ctypes.c_double)
                 scores[:n_explore] = self.random_state.random(size=(n_explore, self.nchoices))
                 self._choose_active(X[:n_explore], scores[:n_explore], choose=False)
                 scores[n_explore:] = self._oracles.decision_function(X[n_explore:])
             
         else:
             scores = self._oracles.decision_function(X)
 
@@ -3027,36 +3041,46 @@
     
     Parameters
     ----------
     nchoices : int or list-like
         Number of arms/labels to choose from. Can also pass a list, array, or Series with arm names, in which case
         the outputs from predict will follow these names and arms can be dropped by name, and new ones added with a
         custom name.
+    lambda_ : float > 0
+        Regularization parameter. References assumed this would always be equal to 1, but this
+        implementation allows to change it.
+    fit_intercept : bool
+        Whether to add an intercept term to the coefficients.
     v_sq : float
         Parameter by which to multiply the covariance matrix (more means higher variance).
         It is recommended to decrease it from the default value of 1.
     sample_from : str, one of "coef", "ci"
         Whether to make predictions by sampling the model coefficients or by
         sampling the predicted value from an interval centered around the coefficients.
         If sampling from the coefficients, it's highly recommended to use ``method="chol"``
         as it will be faster and more precise.
-    lambda_ : float > 0
-        Regularization parameter. References assumed this would always be equal to 1, but this
-        implementation allows to change it.
-    fit_intercept : bool
-        Whether to add an intercept term to the coefficients.
+    n_presampled : None or int
+        If sampling from coefficients, this denotes a number of coefficients to pre-sample
+        after calling 'fit' and/or 'partial_fit', which will be used later in the predictions. Pre-sampling
+        a large number of coefficients can help to speed up predictions at the expense
+        of longer fitting times, and is recommended if there is a large number of predictions
+        between calls to 'fit' or 'partial_fit'.
+        If passing 'None' (the default), will not pre-sample a finite number of the coefficients
+        at fitting time, but will rather sample (different) coefficients in calls to 'predict'.
+        Ignored when passing ``sample_from="ci"``.
     sample_unique : bool
         Whether to sample different coefficients each time a prediction is to
         be made. If passing 'False', when calling 'predict', it will sample
         the same coefficients for all the observations in the same call to
         'predict', whereas if passing 'True', will use a different set of
         coefficients for each observations. Passing 'False' leads to an
         approach which is theoretically wrong, but as sampling coefficients
         can be very slow, using 'False' can provide a reasonable speed up
         without much of a performance penalty.
+        Ignored when passing ``sample_from="ci"`` or ``n_presampled``.
     use_float : bool
         Whether to use C 'float' type for the required matrices. If passing 'False',
         will use C 'double'. Be aware that memory usage for this model can grow
         very large, and that it is more prone to suffer from numeric precision
         problems compared to its UCB counterpart.
     method : str, one of 'chol' or 'sm'
         Method used to fit the model. Options are:
@@ -3070,15 +3094,17 @@
             Starts with an inverse diagonal matrix and updates it as each
             new observation comes using the Sherman-Morrison formula, thus
             never explicitly solving the linear system, nor needing to calculate
             a matrix inverse. This is likely to be faster when fitting the model
             to small batches of observations. Be aware that with this method, it
             will add regularization to the intercept if passing 'fit_intercept=True'.
 
-        If using ``sample_from="ci"``, it's highly recommended to pass "chol" here.
+        Note that, even when using "sm" here, if sampling from the coefficients, it
+        will need after each update to calculate eigen values of the covariance or
+        inverse covariance matrix, so it won't be as fast as LinUCB.
     beta_prior : str 'auto', None, tuple ((a,b), n), or list[tuple((a,b), n)]
         If not 'None', when there are less than 'n' samples with and without
         a reward from a given arm, it will predict the score for that class as a
         random number drawn from a beta distribution with the prior
         specified by 'a' and 'b'. If set to "auto", will be calculated as:
             beta_prior = ((2/log2(nchoices), 4), 2)
         Can also pass different priors per arm, in which case they should be passed
@@ -3125,26 +3151,30 @@
     
     References
     ----------
     .. [1] Agrawal, Shipra, and Navin Goyal.
            "Thompson sampling for contextual bandits with linear payoffs."
            International Conference on Machine Learning. 2013.
     """
-    def __init__(self, nchoices, v_sq=1.0, sample_from="coef", lambda_=1.0, fit_intercept=True,
-                 sample_unique=False, use_float=False, method="sm",
+    def __init__(self, nchoices, lambda_=1.0, fit_intercept=True,
+                 v_sq=1.0, sample_from="coef", n_presampled=None, sample_unique=True,
+                 use_float=False, method="chol",
                  beta_prior=None, smoothing=None, noise_to_smooth=True,
                  assume_unique_reward=False, random_state=None, njobs = 1):
         assert sample_from in ["coef", "ci"]
+        if n_presampled is not None:
+            assert n_presampled > 0
+            assert isinstance(n_presampled, int)
         self._ts = True
         self._add_common_lin(v_sq, lambda_, fit_intercept, use_float, method, nchoices, njobs)
         base = _LinUCB_n_TS_single(alpha=self.v_sq, lambda_=self.lambda_,
                                    fit_intercept=self.fit_intercept,
                                    use_float=self.use_float, method=self.method,
                                    ts=True, ts_from_ci=(sample_from == "ci"),
-                                   sample_unique=sample_unique)
+                                   sample_unique=sample_unique, n_presampled=n_presampled)
         self._add_common_params(base, beta_prior, smoothing, noise_to_smooth, njobs, nchoices,
                                 True, None, False, assume_unique_reward,
                                 random_state, assign_algo=True, prior_def_ucb=False)
 
     def reset_v_sq(self, v_sq=1.0):
         """
         Set the covariance multiplier to a custom number
```

### Comparing `contextualbandits-0.3.8/contextualbandits/utils.py` & `contextualbandits-0.3.9/contextualbandits/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1024,30 +1024,43 @@
         for model in self.algos:
             if is_from_this_module(model):
                 setattr(model, attr_name, attr_value)
 
 class _LinUCB_n_TS_single:
     def __init__(self, alpha=1.0, lambda_=1.0, fit_intercept=True,
                  use_float=True, method="sm", ts=False, ts_from_ci=False,
-                 sample_unique=False, random_state=1):
-        self.alpha = alpha
+                 sample_unique=False, n_presampled=None, random_state=1):
+        self._alpha = alpha
         self.lambda_ = lambda_
         self.fit_intercept = fit_intercept
         self.use_float = use_float
         self.method = method
         self.ts = ts
         self.ts_from_ci = ts_from_ci
         self.sample_unique = bool(sample_unique)
+        self.n_presampled = n_presampled
         self.random_state = _check_random_state(random_state)
         self.is_fitted = False
         self.model = LinearRegression(lambda_=self.lambda_,
                                       fit_intercept=self.fit_intercept,
                                       method=self.method,
                                       use_float=self.use_float,
-                                      calc_inv=True)
+                                      precompute_ts=(self.ts) and (not self.ts_from_ci),
+                                      precompute_ts_multiplier=self.alpha,
+                                      n_presampled=n_presampled,
+                                      calc_inv= not ( (self.ts) and (not self.ts_from_ci) ))
+
+    @property
+    def alpha(self):
+        return self._alpha
+
+    @alpha.setter
+    def alpha(self, value):
+        self._alpha = alpha
+        self.model.precompute_ts_multiplier = alpha
 
     def fit(self, X, y):
         if X.shape[0]:
             self.model.fit(X, y)
             self.is_fitted = True
         return self
 
@@ -1075,30 +1088,34 @@
     def exploit(self, X):
         if not self.is_fitted:
             return np.zeros(X.shape[0])
         return self.predict(X, exploit = True)
 
 class _LogisticUCB_n_TS_single:
     def __init__(self, lambda_=1., fit_intercept=True, alpha=0.95,
-                 m=1.0, ts=False, ts_from_ci=True, sample_unique=False, random_state=1):
+                 m=1.0, ts=False, ts_from_ci=True,
+                 sample_unique=False, n_presampled=None,
+                 random_state=1):
         self.conf_coef = alpha
         self.m = m
         self.fit_intercept = fit_intercept
         self.lambda_ = lambda_
         self.ts = ts
         self.ts_from_ci = ts_from_ci
         self.warm_start = True
         self.sample_unique = bool(sample_unique)
+        self.n_presampled = n_presampled
         self.random_state = _check_random_state(random_state)
         self.is_fitted = False
         self.model = LogisticRegression(C=1./lambda_, penalty="l2",
                                         fit_intercept=fit_intercept,
                                         solver='lbfgs', max_iter=15000,
                                         warm_start=True)
         self.Sigma = np.empty((0,0), dtype=np.float64)
+        self.EigMultiplier = np.empty((0,0), dtype=np.float64)
 
     def __setattr__(self, name, value):
         if (name == "conf_coef"):
             value = norm_dist.ppf(value / 100.)
         super().__setattr__(name, value)
 
     def fit(self, X, y, *args, **kwargs):
@@ -1118,18 +1135,33 @@
             var,
             self.Sigma,
             np.empty(0, dtype=ctypes.c_double),
             Xcsr = Xcsr,
             add_bias=self.fit_intercept,
             overwrite=1
         )
-        ### It's faster to sample coefficients from an inverse-covariance matrix
-        ### For TS-coef, 'Sigma' will be the inverse of the variance-covariance of the predictors,
+        ### For TS-coef, 'Sigma' will be a transformation on the eigenvalues of the
+        ### inverse of the variance-covariance of the predictors,
         ### For UCB and TS-ci, will be the variance-covariance matrix of the predictors
-        if not (self.ts and not self.ts_from_ci):
+        if (self.ts) and (not self.ts_from_ci):
+            self.EigMultiplier, ignored, ignored_ = \
+                _wrapper_double.get_mvnorm_multiplier(self.Sigma, self.m, True, True)
+            if self.n_presampled is not None:
+                if self.fit_intercept:
+                    coef = np.r_[self.model.coef_.reshape(-1), self.model.intercept_]
+                else:
+                    coef = self.model.coef_.reshape(-1)
+                self.coef_presampled = \
+                    _wrapper_double.mvnorm_from_Eig(coef,
+                                                    self.EigMultiplier,
+                                                    self.n_presampled,
+                                                    self.random_state)
+                self.EigMultiplier = np.empty((0,0), dtype=np.float64)
+                self.Sigma = np.empty((0,0), dtype=np.float64)
+        else:
             _matrix_inv_symm(self.Sigma, self.lambda_)
         self.is_fitted = True
 
     def _process_X(self, X):
         if X.dtype != ctypes.c_double:
             X = X.astype(ctypes.c_double)
         if issparse(X):
@@ -1164,33 +1196,47 @@
         ### Thompson sampling, from coefficients
         if (self.ts) and (not exploit):
             if self.fit_intercept:
                 coef = np.r_[self.model.coef_.reshape(-1), self.model.intercept_]
             else:
                 coef = self.model.coef_.reshape(-1)
 
-            if self.sample_unique:
-                coef = _wrapper_double.mvnorm_from_invcov(coef,
-                                                          (1./self.m) * self.Sigma,
-                                                          size=X.shape[0],
-                                                          rng=self.random_state)
+            if self.n_presampled is not None:
+                n_available = self.coef_presampled.shape[0]
+                n_take = X.shape[0]
+                ix_take = self.random_state.choice(n_available, size=n_take, replace=True)
+                coef = self.coef_presampled[ix_take]
                 if not issparse(X):
-                    pred = np.einsum("ij,ij->i", X, coef[:,:X.shape[1]])
+                    pred = np.einsum("ij,ij->i", X, coef[:, :X.shape[1]])
                 else:
                     pred = np.array(X
-                                    .multiply(coef[:,:X.shape[1]])
+                                    .multiply(coef[:, :X.shape[1]])
                                     .sum(axis=1))\
                                     .reshape(-1)
                 if self.fit_intercept:
                     pred[:] += coef[:,-1]
+            elif self.sample_unique:
+                coef = _wrapper_double.mvnorm_from_Eig(coef,
+                                                       self.EigMultiplier,
+                                                       X.shape[0],
+                                                       self.random_state)
+                if not issparse(X):
+                    pred = np.einsum("ij,ij->i", X, coef[:, :X.shape[1]])
+                else:
+                    pred = np.array(X
+                                    .multiply(coef[:, :X.shape[1]])
+                                    .sum(axis=1))\
+                                    .reshape(-1)
+                if self.fit_intercept:
+                    pred[:] += coef[:, -1]
             else:
-                coef = _wrapper_double.mvnorm_from_invcov(coef,
-                                                          (1./self.m) * self.Sigma,
-                                                          size=1,
-                                                          rng=self.random_state)
+                coef = _wrapper_double.mvnorm_from_Eig(coef,
+                                                       self.EigMultiplier,
+                                                       1,
+                                                       self.random_state)
                 coef = coef.reshape(-1)
                 pred = X.dot(coef[:X.shape[1]])
                 if not isinstance(pred, np.ndarray):
                     pred = np.array(pred).reshape(-1)
                 if self.fit_intercept:
                     pred[:] += coef[-1]
             _apply_sigmoid(pred)
```

### Comparing `contextualbandits-0.3.8/contextualbandits.egg-info/SOURCES.txt` & `contextualbandits-0.3.9/contextualbandits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contextualbandits-0.3.8/setup.py` & `contextualbandits-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'numpy>=1.17',
         'scipy',
         'pandas>=0.25.0',
         'scikit-learn>=0.22',
         'joblib>=0.13',
         'cython'
     ],
-    version = '0.3.8',
+    version = '0.3.9',
     description = 'Python Implementations of Algorithms for Contextual Bandits',
     author = 'David Cortes',
     author_email = 'david.cortes.rivera@gmail.com',
     url = 'https://github.com/david-cortes/contextualbandits',
     keywords = 'contextual bandits offset tree doubly robust policy linucb thompson sampling',
     classifiers = [],
     cmdclass = {'build_ext': build_ext_subclass},
```

