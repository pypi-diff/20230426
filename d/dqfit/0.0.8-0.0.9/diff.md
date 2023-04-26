# Comparing `tmp/dqfit-0.0.8.tar.gz` & `tmp/dqfit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqfit-0.0.8.tar", last modified: Tue Nov 29 15:27:55 2022, max compression
+gzip compressed data, was "dqfit-0.0.9.tar", last modified: Tue Nov 29 15:42:03 2022, max compression
```

## Comparing `dqfit-0.0.8.tar` & `dqfit-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.631307 dqfit-0.0.8/
--rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:27:55.630868 dqfit-0.0.8/PKG-INFO
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.588241 dqfit-0.0.8/dqfit/
--rw-r--r--   0 ah24562    (502) staff       (20)        0 2022-11-29 12:48:24.000000 dqfit-0.0.8/dqfit/__init__.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.626835 dqfit-0.0.8/dqfit/model/
--rw-r--r--   0 ah24562    (502) staff       (20)     6124 2022-11-29 15:26:09.000000 dqfit-0.0.8/dqfit/model/dqi_model.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.628503 dqfit-0.0.8/dqfit/preprocessing/
--rw-r--r--   0 ah24562    (502) staff       (20)     2816 2022-11-29 13:16:08.000000 dqfit-0.0.8/dqfit/preprocessing/ResourceFeatures.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.630005 dqfit-0.0.8/dqfit/preprocessing/resource_helpers/
--rw-r--r--   0 ah24562    (502) staff       (20)     3868 2022-11-29 13:13:37.000000 dqfit-0.0.8/dqfit/preprocessing/resource_helpers/r401.py
--rw-r--r--   0 ah24562    (502) staff       (20)     2397 2022-11-29 15:27:00.000000 dqfit-0.0.8/dqfit/query.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:27:55.608059 dqfit-0.0.8/dqfit.egg-info/
--rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:27:55.000000 dqfit-0.0.8/dqfit.egg-info/PKG-INFO
--rw-r--r--   0 ah24562    (502) staff       (20)      273 2022-11-29 15:27:55.000000 dqfit-0.0.8/dqfit.egg-info/SOURCES.txt
--rw-r--r--   0 ah24562    (502) staff       (20)        1 2022-11-29 15:27:55.000000 dqfit-0.0.8/dqfit.egg-info/dependency_links.txt
--rw-r--r--   0 ah24562    (502) staff       (20)        6 2022-11-29 15:27:55.000000 dqfit-0.0.8/dqfit.egg-info/top_level.txt
--rw-r--r--   0 ah24562    (502) staff       (20)      301 2022-11-29 15:27:32.000000 dqfit-0.0.8/pyproject.toml
--rw-r--r--   0 ah24562    (502) staff       (20)       38 2022-11-29 15:27:55.631435 dqfit-0.0.8/setup.cfg
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.614936 dqfit-0.0.9/
+-rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:42:03.614328 dqfit-0.0.9/PKG-INFO
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.598997 dqfit-0.0.9/dqfit/
+-rw-r--r--   0 ah24562    (502) staff       (20)        0 2022-11-29 12:48:24.000000 dqfit-0.0.9/dqfit/__init__.py
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.610298 dqfit-0.0.9/dqfit/model/
+-rw-r--r--   0 ah24562    (502) staff       (20)     6421 2022-11-29 15:40:20.000000 dqfit-0.0.9/dqfit/model/dqi_model.py
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.611787 dqfit-0.0.9/dqfit/preprocessing/
+-rw-r--r--   0 ah24562    (502) staff       (20)     2816 2022-11-29 13:16:08.000000 dqfit-0.0.9/dqfit/preprocessing/ResourceFeatures.py
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.613315 dqfit-0.0.9/dqfit/preprocessing/resource_helpers/
+-rw-r--r--   0 ah24562    (502) staff       (20)     3868 2022-11-29 13:13:37.000000 dqfit-0.0.9/dqfit/preprocessing/resource_helpers/r401.py
+-rw-r--r--   0 ah24562    (502) staff       (20)     2397 2022-11-29 15:27:00.000000 dqfit-0.0.9/dqfit/query.py
+drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.608847 dqfit-0.0.9/dqfit.egg-info/
+-rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/PKG-INFO
+-rw-r--r--   0 ah24562    (502) staff       (20)      273 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/SOURCES.txt
+-rw-r--r--   0 ah24562    (502) staff       (20)        1 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/dependency_links.txt
+-rw-r--r--   0 ah24562    (502) staff       (20)        6 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/top_level.txt
+-rw-r--r--   0 ah24562    (502) staff       (20)      301 2022-11-29 15:41:18.000000 dqfit-0.0.9/pyproject.toml
+-rw-r--r--   0 ah24562    (502) staff       (20)       38 2022-11-29 15:42:03.615065 dqfit-0.0.9/setup.cfg
```

### Comparing `dqfit-0.0.8/dqfit/model/dqi_model.py` & `dqfit-0.0.9/dqfit/model/dqi_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 import pandas as pd
 
 from dqfit.preprocessing import ResourceFeatures
 from dqfit.query import weights_query
 
 
 class DQIModel:
-    def __init__(self, context: list =["BCSE","COLE"]) -> None:
+    def __init__(self, context: list = ["BCSE", "COLE"]) -> None:
         self.context = context
 
     @staticmethod
     def set_pass_fail(X, threshold=2):
         if X >= threshold:
             return "pass"
         else:
             return "fail"
 
     def fit(self, bundles):
         # hmm do I like this name better?
         RF = ResourceFeatures.transform(bundles)
-        
+
         def _get_patient_features(resource_level_features):
             # tidy this up
             df = resource_level_features.copy()
             df = df[df["resource_type"] == "Patient"].dropna(how="all", axis=1)
             # display(PF)
             df["dim_type"] = "resource_type"
             df["dim_key"] = "Patient"
             df["dim_weight"] = 1
             return df
 
-        dim_weights = weights_query(context = self.context)
+        dim_weights = weights_query(context=self.context)
         contexts = []
         for context in dim_weights["context"].unique():
             context_dim_weights = dim_weights[dim_weights["context"] == context]
             weighted_resource_features = RF.copy()
             WPF = _get_patient_features(RF)
             WRF = weighted_resource_features.merge(
                 context_dim_weights, left_on="code", right_on="dim_key"
@@ -54,28 +54,33 @@
             D.groupby(["context", "bundle_index"])
             .agg(fit_score=("dim_score", "sum"))
             .reset_index()
         )
         fitness_scores["outcome"] = fitness_scores["fit_score"].apply(
             self.set_pass_fail
         )
+        fitness_scores["outcome"] = pd.Categorical(
+            fitness_scores["outcome"], ["pass", "fail"])
+        fitness_scores = fitness_scores.sort_values(["context", "outcome", "fit_score"], ascending=[
+                                                    True, True, False]).reset_index(drop=True)
         return fitness_scores
 
     @staticmethod
     def visualize(scores):
-        
+
         print(scores['outcome'].value_counts(normalize=True))
         cohort_outcomes = (
             scores.groupby(["context", "outcome"])
             .agg(count=("outcome", "count"))
             .reset_index()
         )
-        
+
         px.bar(
-            cohort_outcomes.sort_values(["context","outcome"], ascending=False),
+            cohort_outcomes.sort_values(
+                ["context", "outcome"], ascending=True),
             x="context",
             y="count",
             color="outcome",
             title=f"Cohort Outcomes",
         ).show()
 
     # def cohort_level_scores(self):
@@ -90,15 +95,14 @@
 # from sklearn.preprocessing import MinMaxScaler, StandardScaler
 # from pathlib import Path
 
 # # could be an abstraction
 # class DQIModel:
 
 
-
 #     def __init__(self, context="systolic") -> None:
 #         """Does stuff"""
 #         self.context = context
 
 #     @property
 #     def weights(self):
 #         package_dir = Path(__file__).parent
```

### Comparing `dqfit-0.0.8/dqfit/preprocessing/ResourceFeatures.py` & `dqfit-0.0.9/dqfit/preprocessing/ResourceFeatures.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.0.8/dqfit/preprocessing/resource_helpers/r401.py` & `dqfit-0.0.9/dqfit/preprocessing/resource_helpers/r401.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.0.8/dqfit/query.py` & `dqfit-0.0.9/dqfit/query.py`

 * *Files identical despite different names*

