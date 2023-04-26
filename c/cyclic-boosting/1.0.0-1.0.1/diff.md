# Comparing `tmp/cyclic_boosting-1.0.0.tar.gz` & `tmp/cyclic_boosting-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclic_boosting-1.0.0.tar", max compression
+gzip compressed data, was "cyclic_boosting-1.0.1.tar", max compression
```

## Comparing `cyclic_boosting-1.0.0.tar` & `cyclic_boosting-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    14197 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/LICENSE
--rw-r--r--   0        0        0     1268 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/README.md
--rw-r--r--   0        0        0     3489 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/GBSregression.py
--rw-r--r--   0        0        0     1943 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/__init__.py
--rw-r--r--   0        0        0    44776 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/base.py
--rw-r--r--   0        0        0      719 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/__init__.py
--rw-r--r--   0        0        0    10628 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/_binary_search.py
--rw-r--r--   0        0        0     2953 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/_utils.py
--rw-r--r--   0        0        0     8282 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/bin_number_transformer.py
--rw-r--r--   0        0        0    19266 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/ecdf_transformer.py
--rw-r--r--   0        0        0     4896 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/classification.py
--rw-r--r--   0        0        0    13130 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/common_smoothers.py
--rw-r--r--   0        0        0    11607 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/features.py
--rw-r--r--   0        0        0    13132 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/flags.py
--rw-r--r--   0        0        0     2308 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/learning_rate.py
--rw-r--r--   0        0        0     2383 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/link.py
--rw-r--r--   0        0        0     8943 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/location.py
--rw-r--r--   0        0        0     8331 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/nbinom.py
--rw-r--r--   0        0        0     6831 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/observers.py
--rw-r--r--   0        0        0     6108 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/pipelines.py
--rw-r--r--   0        0        0    11070 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/_1dplots.py
--rw-r--r--   0        0        0     7517 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/_2dplots.py
--rw-r--r--   0        0        0    10899 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/__init__.py
--rw-r--r--   0        0        0     7497 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/plot_utils.py
--rw-r--r--   0        0        0    15702 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/price.py
--rw-r--r--   0        0        0     6953 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/regression.py
--rw-r--r--   0        0        0      529 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/base.py
--rw-r--r--   0        0        0     4737 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/extrapolate.py
--rw-r--r--   0        0        0    10724 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/meta_smoother.py
--rw-r--r--   0        0        0    14258 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/multidim.py
--rw-r--r--   0        0        0    26024 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/onedim.py
--rw-r--r--   0        0        0     4940 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/orthofit.py
--rw-r--r--   0        0        0    30546 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/utils.py
--rw-r--r--   0        0        0     1394 2023-04-14 14:34:07.133379 cyclic_boosting-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 cyclic_boosting-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    14197 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1268 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/README.md
+-rw-r--r--   0        0        0     3489 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/GBSregression.py
+-rw-r--r--   0        0        0     1943 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/__init__.py
+-rw-r--r--   0        0        0    44776 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/base.py
+-rw-r--r--   0        0        0      719 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/binning/__init__.py
+-rw-r--r--   0        0        0    10628 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/binning/_binary_search.py
+-rw-r--r--   0        0        0     2953 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/binning/_utils.py
+-rw-r--r--   0        0        0     8282 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/binning/bin_number_transformer.py
+-rw-r--r--   0        0        0    19266 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/binning/ecdf_transformer.py
+-rw-r--r--   0        0        0     4896 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/classification.py
+-rw-r--r--   0        0        0    13130 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/common_smoothers.py
+-rw-r--r--   0        0        0    11607 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/features.py
+-rw-r--r--   0        0        0    13132 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/flags.py
+-rw-r--r--   0        0        0     2308 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/learning_rate.py
+-rw-r--r--   0        0        0     2383 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/link.py
+-rw-r--r--   0        0        0     8943 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/location.py
+-rw-r--r--   0        0        0     8331 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/nbinom.py
+-rw-r--r--   0        0        0     6831 2023-04-26 05:57:05.885602 cyclic_boosting-1.0.1/cyclic_boosting/observers.py
+-rw-r--r--   0        0        0     6108 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/pipelines.py
+-rw-r--r--   0        0        0    11070 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/plots/_1dplots.py
+-rw-r--r--   0        0        0     7517 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/plots/_2dplots.py
+-rw-r--r--   0        0        0    10899 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/plots/__init__.py
+-rw-r--r--   0        0        0     7497 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/plots/plot_utils.py
+-rw-r--r--   0        0        0    15702 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/price.py
+-rw-r--r--   0        0        0     6953 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/regression.py
+-rw-r--r--   0        0        0      529 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/base.py
+-rw-r--r--   0        0        0     4737 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/extrapolate.py
+-rw-r--r--   0        0        0    10724 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/meta_smoother.py
+-rw-r--r--   0        0        0    14258 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/multidim.py
+-rw-r--r--   0        0        0    26024 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/onedim.py
+-rw-r--r--   0        0        0     4940 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/smoothing/orthofit.py
+-rw-r--r--   0        0        0    30546 2023-04-26 05:57:05.889602 cyclic_boosting-1.0.1/cyclic_boosting/utils.py
+-rw-r--r--   0        0        0     1395 2023-04-26 05:57:05.893602 cyclic_boosting-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 cyclic_boosting-1.0.1/PKG-INFO
```

### Comparing `cyclic_boosting-1.0.0/LICENSE` & `cyclic_boosting-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/README.md` & `cyclic_boosting-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/GBSregression.py` & `cyclic_boosting-1.0.1/cyclic_boosting/GBSregression.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/__init__.py` & `cyclic_boosting-1.0.1/cyclic_boosting/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/base.py` & `cyclic_boosting-1.0.1/cyclic_boosting/base.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/binning/__init__.py` & `cyclic_boosting-1.0.1/cyclic_boosting/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/binning/_binary_search.py` & `cyclic_boosting-1.0.1/cyclic_boosting/binning/_binary_search.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/binning/_utils.py` & `cyclic_boosting-1.0.1/cyclic_boosting/binning/_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/binning/bin_number_transformer.py` & `cyclic_boosting-1.0.1/cyclic_boosting/binning/bin_number_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/binning/ecdf_transformer.py` & `cyclic_boosting-1.0.1/cyclic_boosting/binning/ecdf_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/classification.py` & `cyclic_boosting-1.0.1/cyclic_boosting/classification.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/common_smoothers.py` & `cyclic_boosting-1.0.1/cyclic_boosting/common_smoothers.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/features.py` & `cyclic_boosting-1.0.1/cyclic_boosting/features.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/flags.py` & `cyclic_boosting-1.0.1/cyclic_boosting/flags.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/learning_rate.py` & `cyclic_boosting-1.0.1/cyclic_boosting/learning_rate.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/link.py` & `cyclic_boosting-1.0.1/cyclic_boosting/link.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/location.py` & `cyclic_boosting-1.0.1/cyclic_boosting/location.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/nbinom.py` & `cyclic_boosting-1.0.1/cyclic_boosting/nbinom.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/observers.py` & `cyclic_boosting-1.0.1/cyclic_boosting/observers.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/pipelines.py` & `cyclic_boosting-1.0.1/cyclic_boosting/pipelines.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/plots/_1dplots.py` & `cyclic_boosting-1.0.1/cyclic_boosting/plots/_1dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/plots/_2dplots.py` & `cyclic_boosting-1.0.1/cyclic_boosting/plots/_2dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/plots/__init__.py` & `cyclic_boosting-1.0.1/cyclic_boosting/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/plots/plot_utils.py` & `cyclic_boosting-1.0.1/cyclic_boosting/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/price.py` & `cyclic_boosting-1.0.1/cyclic_boosting/price.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/regression.py` & `cyclic_boosting-1.0.1/cyclic_boosting/regression.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/__init__.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/base.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/base.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/extrapolate.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/extrapolate.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/meta_smoother.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/meta_smoother.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/multidim.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/multidim.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/onedim.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/onedim.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/orthofit.py` & `cyclic_boosting-1.0.1/cyclic_boosting/smoothing/orthofit.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/cyclic_boosting/utils.py` & `cyclic_boosting-1.0.1/cyclic_boosting/utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-1.0.0/pyproject.toml` & `cyclic_boosting-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclic-boosting"
-version = "1.0.0"
+version = "1.0.1"
 description = "Implementation of Cyclic Boosting machine learning algorithms"
 authors = ["Blue Yonder GmbH"]
 packages = [{include = "cyclic_boosting"}]
 readme = "README.md"
 classifiers = [
    "Topic :: Scientific/Engineering :: Artificial Intelligence",
    "Programming Language :: Python :: 3 :: Only",
@@ -20,15 +20,15 @@
 numba-scipy = "^0.3.1"
 numpy = ">=1.12.1"
 numexpr = ">=2.5.2"
 scikit-learn = ">=0.18.2"
 pandas = ">=0.20.3"
 matplotlib = ">=1.5.1"
 hypothesis = "^6.70.0"
-scipy = { version = "1.7.2", python = "<3.10" }
+scipy = { version = "1.7.3", python = "<3.10" }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ruff = "^0.0.256"
 pytest = "^7.2.2"
 pre-commit = "^3.2.2"
@@ -54,8 +54,8 @@
 
 [tool.black]
 line-length = 120
 target_version = ["py38"]
 
 [tool.ruff]
 line-length = 120
-ignore = ["E741", "E722"]
+ignore = ["E741", "E722"]
```

### Comparing `cyclic_boosting-1.0.0/PKG-INFO` & `cyclic_boosting-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclic-boosting
-Version: 1.0.0
+Version: 1.0.1
 Summary: Implementation of Cyclic Boosting machine learning algorithms
 Author: Blue Yonder GmbH
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: matplotlib (>=1.5.1)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numba-scipy (>=0.3.1,<0.4.0)
 Requires-Dist: numexpr (>=2.5.2)
 Requires-Dist: numpy (>=1.12.1)
 Requires-Dist: pandas (>=0.20.3)
 Requires-Dist: scikit-learn (>=0.18.2)
-Requires-Dist: scipy (==1.7.2) ; python_version < "3.10"
+Requires-Dist: scipy (==1.7.3) ; python_version < "3.10"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cyclic-boosting
 
 This package contains the implementation of the machine learning algorithm Cyclic Boosting, which is described in [Cyclic Boosting - an explainable supervised machine learning algorithm](https://arxiv.org/abs/2002.03425) and [Demand Forecasting of Individual Probability Density Functions with Machine Learning](https://arxiv.org/abs/2009.07052).
```

