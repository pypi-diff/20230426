# Comparing `tmp/fold_core-0.1.3.tar.gz` & `tmp/fold_core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.3.tar", max compression
+gzip compressed data, was "fold_core-0.1.4.tar", max compression
```

## Comparing `fold_core-0.1.3.tar` & `fold_core-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0     3870 2023-04-21 15:22:18.540089 fold_core-0.1.3/LICENSE
--rw-r--r--   0        0        0    10364 2023-04-21 15:22:18.540089 fold_core-0.1.3/README.md
--rw-r--r--   0        0        0     3820 2023-04-21 15:22:18.580089 fold_core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/__init__.py
--rw-r--r--   0        0        0     5273 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/base.py
--rw-r--r--   0        0        0      529 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6359 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4760 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2064 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/select.py
--rw-r--r--   0        0        0     4545 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1931 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      590 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9922 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/common.py
--rw-r--r--   0        0        0     2109 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     7138 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2993 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5735 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/types.py
--rw-r--r--   0        0        0      381 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/random.py
--rw-r--r--   0        0        0     4310 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/splitters.py
--rw-r--r--   0        0        0      928 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4264 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2906 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5675 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7573 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3734 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2171 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2240 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/list.py
--rw-r--r--   0        0        0     2955 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/trim.py
--rw-r--r--   0        0        0    13161 1970-01-01 00:00:00.000000 fold_core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-25 14:21:08.507826 fold_core-0.1.4/LICENSE
+-rw-r--r--   0        0        0    10376 2023-04-25 14:21:08.507826 fold_core-0.1.4/README.md
+-rw-r--r--   0        0        0     3820 2023-04-25 14:21:08.543828 fold_core-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/__init__.py
+-rw-r--r--   0        0        0     5400 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/base.py
+-rw-r--r--   0        0        0      529 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6384 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4785 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2064 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4632 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1931 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      590 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9973 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/common.py
+-rw-r--r--   0        0        0     2109 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     7138 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/encase.py
+-rw-r--r--   0        0        0      852 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/inference.py
+-rw-r--r--   0        0        0     2993 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     6545 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/types.py
+-rw-r--r--   0        0        0      756 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/loop/update.py
+-rw-r--r--   0        0        0      381 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/random.py
+-rw-r--r--   0        0        0     4310 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/splitters.py
+-rw-r--r--   0        0        0      928 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4281 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     3312 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5675 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7624 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3701 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2171 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/checks.py
+-rw-r--r--   0        0        0      638 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/dataframe.py
+-rw-r--r--   0        0        0     2240 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2955 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-04-25 14:21:08.543828 fold_core-0.1.4/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    13173 1970-01-01 00:00:00.000000 fold_core-0.1.4/PKG-INFO
```

### Comparing `fold_core-0.1.3/LICENSE` & `fold_core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/README.md` & `fold_core-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
     <img src="https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
 <h3 align="center"><b>FOLD</b><br></h3>
   <p align="center">
-    Fast <b>Adaptive ML </b> Engine
+    Fast <b>Adaptive Time Series ML </b> Engine
     <br/>
     <a href="https://dream-faster.github.io/fold/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 <!-- INTRO -->
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                       ****
-                           Fast Adaptive ML Engine
+                     Fast Adaptive Time Series ML Engine
                               Explore_the_docs_Â»
 
  ![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/
 docs/images/overview_diagrams/main_diagram.svg) TheAdaptive_ML_Engine that lets
 you build, deploy and update Models easily. An order of magnitude speed-up,
 combined with flexibility and rigour.
```

### Comparing `fold_core-0.1.3/pyproject.toml` & `fold_core-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.3"
+version = "0.1.4"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -124,15 +124,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.3/src/fold/base.py` & `fold_core-0.1.4/src/fold/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         raise NotImplementedError
 
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
+        in_sample: bool,
     ) -> pd.DataFrame:
         raise NotImplementedError
 
     @abstractmethod
     def clone(self, clone_child_transformations: Callable) -> "Composite":
         raise NotImplementedError
 
@@ -140,15 +141,15 @@
     @abstractmethod
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         raise NotImplementedError
 
 
 class InvertibleTransformation(Transformation, ABC):
     @abstractmethod
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         raise NotImplementedError
 
 
 class FeatureSelector(Transformation):
     selected_features: List[str]
 
 
@@ -165,14 +166,16 @@
 Pipelines = List[Pipeline]
 """Multiple, independent `Pipeline`s."""
 
 TrainedPipelines = List[pd.Series]
 """A list of trained `Pipeline`s, to be used for backtesting."""
 OutOfSamplePredictions = pd.DataFrame
 """The backtest's resulting out-of-sample predictions."""
+DeployablePipeline = Pipeline
+"""A trained `Pipeline`, to be used for deployment."""
 
 
 def fit_noop(
     self,
     X: pd.DataFrame,
     y: pd.Series,
     sample_weights: Optional[pd.Series] = None,
```

### Comparing `fold_core-0.1.3/src/fold/composites/__init__.py` & `fold_core-0.1.4/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/columns.py` & `fold_core-0.1.4/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/common.py` & `fold_core-0.1.4/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/concat.py` & `fold_core-0.1.4/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/ensemble.py` & `fold_core-0.1.4/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/metalabeling.py` & `fold_core-0.1.4/src/fold/composites/metalabeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         raise NotImplementedError
 
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
+        in_sample: bool,
     ) -> pd.DataFrame:
         primary_predictions = get_prediction_column(primary_results[0])
         meta_probabilities = secondary_results[0][
             [
                 col
                 for col in secondary_results[0].columns
                 if col.startswith("probabilities_")
```

### Comparing `fold_core-0.1.3/src/fold/composites/residual.py` & `fold_core-0.1.4/src/fold/composites/residual.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         raise NotImplementedError
 
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
+        in_sample: bool,
     ) -> pd.DataFrame:
         primary_predictions = get_prediction_column(primary_results[0])
         residual_predictions = get_prediction_column(secondary_results[0])
 
         return (
             (primary_predictions + residual_predictions)
             .rename(f"predictions_{self.name}")
```

### Comparing `fold_core-0.1.3/src/fold/composites/sample.py` & `fold_core-0.1.4/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/select.py` & `fold_core-0.1.4/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/composites/target.py` & `fold_core-0.1.4/src/fold/composites/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 from __future__ import annotations
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Composite, InvertibleTransformation, Pipelines, T
+from ..base import Composite, InvertibleTransformation, Pipeline, Pipelines, T
 from ..utils.checks import get_prediction_column, get_prediction_column_name
+from ..utils.dataframe import to_series
 from ..utils.list import wrap_in_double_list_if_needed
 from .common import get_concatenated_names
 
 
 class TransformTarget(Composite):
     """
     Transforms the target within the context of the wrapped Pipeline.
@@ -53,15 +54,15 @@
     properties = Composite.Properties(
         primary_only_single_pipeline=True,
         secondary_only_single_pipeline=True,
     )
 
     def __init__(
         self,
-        wrapped_pipeline: Pipelines,
+        wrapped_pipeline: Pipeline,
         y_pipeline: Union[List[InvertibleTransformation], InvertibleTransformation],
     ) -> None:
         self.wrapped_pipeline = wrap_in_double_list_if_needed(wrapped_pipeline)
         self.y_pipeline = wrap_in_double_list_if_needed(y_pipeline)
         self.name = "TransformTarget-" + get_concatenated_names(
             self.wrapped_pipeline + self.y_pipeline
         )
@@ -87,29 +88,30 @@
         self,
         X: pd.DataFrame,
         y: T,
         results_primary: List[pd.DataFrame],
         index: int,
         fit: bool,
     ) -> Tuple[pd.DataFrame, T]:
-        return X, results_primary[0].squeeze()
+        return X, to_series(results_primary[0])
 
     def postprocess_result_secondary(
         self,
         primary_results: List[pd.DataFrame],
         secondary_results: List[pd.DataFrame],
         y: Optional[pd.Series],
+        in_sample: bool,
     ) -> pd.DataFrame:
         predictions = get_prediction_column(secondary_results[0])
         for transformation in reversed(self.y_pipeline[0]):
-            predictions = transformation.inverse_transform(predictions)
+            predictions = transformation.inverse_transform(predictions, in_sample)
         orignal_results = secondary_results[0]
-        orignal_results[
-            get_prediction_column_name(orignal_results)
-        ] = predictions.squeeze()
+        orignal_results[get_prediction_column_name(orignal_results)] = to_series(
+            predictions
+        )
         return orignal_results
 
     def get_child_transformations_primary(self) -> Pipelines:
         return self.y_pipeline
 
     def get_child_transformations_secondary(
         self,
```

### Comparing `fold_core-0.1.3/src/fold/loop/backend/__init__.py` & `fold_core-0.1.4/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/backend/ray.py` & `fold_core-0.1.4/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/backend/sequential.py` & `fold_core-0.1.4/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/backtesting.py` & `fold_core-0.1.4/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/checks.py` & `fold_core-0.1.4/src/fold/loop/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/common.py` & `fold_core-0.1.4/src/fold/loop/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,17 @@
         )
     if composite.properties.secondary_requires_predictions:
         assert is_prediction(results_secondary[0]), ValueError(
             "Expected predictions from secondary transformations, but got"
             " something else."
         )
 
-    return composite.postprocess_result_secondary(results_primary, results_secondary, y)
+    return composite.postprocess_result_secondary(
+        results_primary, results_secondary, y, in_sample=stage == Stage.inital_fit
+    )
 
 
 def process_with_inner_loop(
     transformation: Transformation,
     X: pd.DataFrame,
     y: Optional[pd.Series],
     sample_weights: Optional[pd.Series],
```

### Comparing `fold_core-0.1.3/src/fold/loop/convenience.py` & `fold_core-0.1.4/src/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/encase.py` & `fold_core-0.1.4/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/memory.py` & `fold_core-0.1.4/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/loop/training.py` & `fold_core-0.1.4/src/fold/loop/training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # Copyright (c) 2022 - Present Myalo UG (haftungbeschränkt) (Mark Aron Szulyovszky, Daniel Szemerey) <info@dreamfaster.ai>. All rights reserved. See LICENSE in root folder.
 
 
 from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
-from ..base import Composite, Pipeline, TrainedPipelines, Transformation
+from ..base import (
+    Composite,
+    DeployablePipeline,
+    Pipeline,
+    TrainedPipelines,
+    Transformation,
+)
 from ..splitters import Fold, SlidingWindowSplitter, Splitter
 from ..utils.list import wrap_in_list
 from .backend import get_backend_dependent_functions
 from .checks import check_types
 from .common import deepcopy_pipelines, recursively_transform
 from .convenience import replace_transformation_if_not_fold_native
 from .types import Backend, Stage, TrainMethod
@@ -134,14 +140,45 @@
             index=processed_idx,
             name=transformation_over_time[0].name,
         )
         for transformation_over_time in zip(*processed_pipelines)
     ]
 
 
+def train_for_deployment(
+    pipeline: Pipeline,
+    X: pd.DataFrame,
+    y: pd.Series,
+    sample_weights: Optional[pd.Series] = None,
+) -> DeployablePipeline:
+    X, y = check_types(X, y)
+
+    pipeline = wrap_in_list(pipeline)
+    pipeline = replace_transformation_if_not_fold_native(pipeline)
+    _, transformations = process_pipeline_window(
+        X,
+        y,
+        sample_weights,
+        pipeline,
+        Fold(
+            order=0,
+            model_index=0,
+            train_window_start=0,
+            train_window_end=None,
+            update_window_start=0,
+            update_window_end=0,
+            test_window_start=0,
+            test_window_end=None,
+        ),
+        True,
+        backend=Backend.no,
+    )
+    return transformations
+
+
 def process_pipeline_window(
     X: pd.DataFrame,
     y: pd.Series,
     sample_weights: Optional[pd.Series],
     transformations: List[Union[Transformation, Composite]],
     split: Fold,
     never_update: bool,
```

### Comparing `fold_core-0.1.3/src/fold/loop/types.py` & `fold_core-0.1.4/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/models/base.py` & `fold_core-0.1.4/src/fold/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         """
         Predictions for exclusively out-of-sample data, the model has never seen before.
         """
         raise NotImplementedError
 
     @abstractmethod
     def predict_in_sample(
-        self, X: pd.DataFrame, y: pd.Series
+        self, X: pd.DataFrame, past_y: pd.Series
     ) -> Union[pd.Series, pd.DataFrame]:
         """
         Predictions for in-sample, already seen data.
         """
         raise NotImplementedError
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
```

### Comparing `fold_core-0.1.3/src/fold/models/baseline.py` & `fold_core-0.1.4/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/models/dummy.py` & `fold_core-0.1.4/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/models/random.py` & `fold_core-0.1.4/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/models/sklearn.py` & `fold_core-0.1.4/src/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/splitters.py` & `fold_core-0.1.4/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/__init__.py` & `fold_core-0.1.4/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/columns.py` & `fold_core-0.1.4/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/date.py` & `fold_core-0.1.4/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/dev.py` & `fold_core-0.1.4/src/fold/transformations/dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,12 +133,12 @@
         else:
             self.no_of_calls_transform_outofsample += 1
         return_value = self.transform_func(X)
         if return_value is None:
             return X
         return return_value
 
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         self.no_of_calls_inverse_transform += 1
         if self.inverse_transform_func is not None:
             return self.inverse_transform_func(X)
         return X
```

### Comparing `fold_core-0.1.3/src/fold/transformations/difference.py` & `fold_core-0.1.4/src/fold/transformations/difference.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 from typing import Optional
 
 import pandas as pd
 
 from ..base import InvertibleTransformation
+from ..utils.dataframe import to_series
 
 
 class Difference(InvertibleTransformation):
     """
     Performs differencing.
     Sesonal differencing can be achieved by setting `lag` to the seasonality of the data.
     To achieve second-order differencing, simply chain multiple `Difference` transformations.
@@ -49,46 +50,53 @@
 
     References
     ----------
 
     [Stationarity and differencing](https://otexts.com/fpp2/stationarity.html)
     """
 
-    properties = InvertibleTransformation.Properties(requires_X=False)
     name = "Difference"
+    first_values_X: Optional[pd.DataFrame] = None
 
     def __init__(self, lag: int = 1) -> None:
         self.lag = lag
+        self.properties = InvertibleTransformation.Properties(requires_X=False)
 
     def fit(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
     ) -> None:
-        self.last_rows_X = X.iloc[-self.lag : None]
+        self.last_values_X = X.iloc[-self.lag : None]
+        self.first_values_X = X.iloc[: self.lag]
 
     def update(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weights: Optional[pd.Series] = None,
     ) -> None:
-        if len(X) >= self.lag:
-            self.last_rows_X = X.iloc[-self.lag : None]
-        else:
-            self.last_rows_X = pd.concat([self.last_rows_X, X], axis="index").iloc[
-                -self.lag : None
-            ]
+        self.last_values_X = X.iloc[-self.lag : None]
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         if in_sample:
             return X.diff(self.lag)
         else:
             return (
-                pd.concat([self.last_rows_X, X], axis="index")
+                pd.concat([self.last_values_X, X], axis="index")
                 .diff(self.lag)
                 .iloc[self.lag :]
             )
 
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
-        return X.cumsum() + self.last_rows_X.iloc[0].squeeze()
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
+        if in_sample:
+            X = X.copy()
+            X.iloc[: self.lag] = to_series(self.first_values_X)
+            for i in range(self.lag):
+                X.iloc[i :: self.lag] = X.iloc[i :: self.lag].cumsum()
+            return X
+        else:
+            X = pd.concat([to_series(self.last_values_X), X], axis="index")
+            for i in range(self.lag):
+                X.iloc[i :: self.lag] = X.iloc[i :: self.lag].cumsum()
+            return X.iloc[self.lag :]
```

### Comparing `fold_core-0.1.3/src/fold/transformations/function.py` & `fold_core-0.1.4/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/holidays.py` & `fold_core-0.1.4/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/lags.py` & `fold_core-0.1.4/src/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/math.py` & `fold_core-0.1.4/src/fold/transformations/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         elif self.base == "10" or self.base == 10:
             return pd.DataFrame(np.log10(X.values), columns=X.columns, index=X.index)
         elif self.base == "2" or self.base == 2:
             return pd.DataFrame(np.log2(X.values), columns=X.columns, index=X.index)
         else:
             raise ValueError(f"Invalid base: {self.base}")
 
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         if self.base == "e" or self.base == np.e:
             return pd.Series(np.exp(X.values), index=X.index)
         elif self.base == "10" or self.base == 10:
             return 10**X
         elif self.base == "2" or self.base == 2:
             return 2**X
         else:
@@ -145,15 +145,15 @@
             return pd.concat(
                 [X.drop(columns=self.constant.keys()), transformed_columns],
                 axis="columns",
             )
         else:
             return X + self.constant
 
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         constant = self.constant
         if constant is dict:
             constant = next(iter(constant.values()))
         return X - constant
 
     fit = fit_noop
     update = fit_noop
@@ -212,11 +212,11 @@
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         transformed_columns = X[list(self.constant.keys())] + pd.Series(self.constant)
         return pd.concat(
             [X.drop(columns=self.constant.keys()), transformed_columns],
             axis="columns",
         )
 
-    def inverse_transform(self, X: pd.Series) -> pd.Series:
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
         return X - next(iter(self.constant.values()))
 
     update = fit_noop
```

### Comparing `fold_core-0.1.3/src/fold/transformations/sklearn.py` & `fold_core-0.1.4/src/fold/transformations/sklearn.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,16 @@
 
     def transform(self, X: pd.DataFrame, in_sample: bool) -> pd.DataFrame:
         if hasattr(self.transformation, "set_output"):
             return self.transformation.transform(X)
         else:
             return pd.DataFrame(self.transformation.transform(X), columns=X.columns)
 
-    def inverse_transform(self, X: pd.DataFrame) -> pd.DataFrame:
-        return pd.DataFrame(
-            self.transformation.inverse_transform(X), columns=X.columns, index=X.index
-        )
+    def inverse_transform(self, X: pd.Series, in_sample: bool) -> pd.Series:
+        return pd.Series(self.transformation.inverse_transform(X), index=X.index)
 
 
 class WrapSKLearnFeatureSelector(FeatureSelector):
     """
     Wraps an SKLearn Feature Selector class, stores the selected columns in `selected_features` property.
     There's no need to use it directly, `fold` automatically wraps all sklearn feature selectors into this class.
     """
```

### Comparing `fold_core-0.1.3/src/fold/transformations/update.py` & `fold_core-0.1.4/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/transformations/window.py` & `fold_core-0.1.4/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/utils/checks.py` & `fold_core-0.1.4/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/utils/dataset.py` & `fold_core-0.1.4/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/utils/list.py` & `fold_core-0.1.4/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/utils/tests.py` & `fold_core-0.1.4/src/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/src/fold/utils/trim.py` & `fold_core-0.1.4/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.3/PKG-INFO` & `fold_core-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
@@ -68,15 +68,15 @@
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
     <img src="https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
 <h3 align="center"><b>FOLD</b><br></h3>
   <p align="center">
-    Fast <b>Adaptive ML </b> Engine
+    Fast <b>Adaptive Time Series ML </b> Engine
     <br/>
     <a href="https://dream-faster.github.io/fold/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 <!-- INTRO -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.3 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.4 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
@@ -37,15 +37,15 @@
 Dist: tqdm (>=4.0) Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
                                       ****
-                           Fast Adaptive ML Engine
+                     Fast Adaptive Time Series ML Engine
                               Explore_the_docs_Â»
 
  ![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/
 docs/images/overview_diagrams/main_diagram.svg) TheAdaptive_ML_Engine that lets
 you build, deploy and update Models easily. An order of magnitude speed-up,
 combined with flexibility and rigour.
```

