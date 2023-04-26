# Comparing `tmp/zoish-3.4.0.tar.gz` & `tmp/zoish-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoish-3.4.0.tar", max compression
+gzip compressed data, was "zoish-3.5.0.tar", max compression
```

## Comparing `zoish-3.4.0.tar` & `zoish-3.5.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1323 2023-04-20 18:05:36.346876 zoish-3.4.0/LICENSE
--rw-r--r--   0        0        0    10737 2023-04-20 18:05:36.347039 zoish-3.4.0/README.md
--rw-r--r--   0        0        0     1264 2023-04-25 16:04:07.186113 zoish-3.4.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-04-20 18:05:36.358370 zoish-3.4.0/zoish/.env
--rw-r--r--   0        0        0      925 2023-04-25 16:04:07.187113 zoish-3.4.0/zoish/__init__.py
--rw-r--r--   0        0        0     1938 2023-04-20 18:05:36.358804 zoish-3.4.0/zoish/abstracs/feature_selector_abstracts.py
--rw-r--r--   0        0        0    60046 2023-04-20 18:05:36.359334 zoish-3.4.0/zoish/base_classes/best_estimator_getters.py
--rw-r--r--   0        0        0      675 2023-04-20 18:05:36.359553 zoish-3.4.0/zoish/config.yaml
--rw-r--r--   0        0        0      375 2023-04-20 18:05:36.359847 zoish-3.4.0/zoish/decorators/decorators.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.360014 zoish-3.4.0/zoish/examples/__init__.py
--rw-r--r--   0        0        0    54613 2023-04-20 18:05:36.361103 zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
--rw-r--r--   0        0        0    42652 2023-04-20 18:05:36.361831 zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61640 2023-04-20 18:05:36.362393 zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
--rw-r--r--   0        0        0    97297 2023-04-20 18:05:36.362969 zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0   114986 2023-04-20 18:05:36.363251 zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
--rw-r--r--   0        0        0    20432 2023-04-20 18:05:36.363794 zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
--rw-r--r--   0        0        0    40581 2023-04-20 18:05:36.364116 zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    63450 2023-04-20 18:05:36.364446 zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
--rw-r--r--   0        0        0    56051 2023-04-20 18:05:36.364756 zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    71923 2023-04-20 18:05:36.365059 zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
--rw-r--r--   0        0        0    22310 2023-04-20 18:05:36.365292 zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
--rw-r--r--   0        0        0    53217 2023-04-20 18:05:36.365575 zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61941 2023-04-20 18:05:36.366026 zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
--rw-r--r--   0        0        0   102159 2023-04-20 18:05:36.366576 zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   118140 2023-04-20 18:05:36.366880 zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.367139 zoish-3.4.0/zoish/examples/shap/__init__.py
--rw-r--r--   0        0        0    21194 2023-04-20 18:05:36.369666 zoish-3.4.0/zoish/examples/shap/shap_grid_search_classification.ipynb
--rw-r--r--   0        0        0    58856 2023-04-20 18:05:36.370122 zoish-3.4.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    61444 2023-04-20 18:05:36.373990 zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
--rw-r--r--   0        0        0   413648 2023-04-20 18:05:36.376447 zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
--rw-r--r--   0        0        0   465032 2023-04-20 18:05:36.396730 zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
--rw-r--r--   0        0        0    88426 2023-04-20 18:05:36.397119 zoish-3.4.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
--rw-r--r--   0        0        0    69117 2023-04-20 18:05:36.397585 zoish-3.4.0/zoish/examples/shap/shap_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.397811 zoish-3.4.0/zoish/examples/single_feature/__init__.py
--rw-r--r--   0        0        0    40086 2023-04-20 18:05:36.398323 zoish-3.4.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
--rw-r--r--   0        0        0    45581 2023-04-20 18:05:36.398779 zoish-3.4.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
--rw-r--r--   0        0        0    85377 2023-04-20 18:05:36.399183 zoish-3.4.0/zoish/examples/single_feature/single_random_search_classification.ipynb
--rw-r--r--   0        0        0   106211 2023-04-20 18:05:36.399543 zoish-3.4.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
--rw-r--r--   0        0        0   122582 2023-04-20 18:05:36.399841 zoish-3.4.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.399998 zoish-3.4.0/zoish/factories/factories.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.400140 zoish-3.4.0/zoish/feature_selectors/__init__.py
--rw-r--r--   0        0        0    85614 2023-04-20 18:05:36.400421 zoish-3.4.0/zoish/feature_selectors/recursive_feature_addition.py
--rw-r--r--   0        0        0    85793 2023-04-20 18:05:36.402572 zoish-3.4.0/zoish/feature_selectors/recursive_feature_elimination.py
--rw-r--r--   0        0        0    85872 2023-04-20 18:05:36.403025 zoish-3.4.0/zoish/feature_selectors/select_by_shuffling.py
--rw-r--r--   0        0        0   100851 2023-04-20 18:05:36.403301 zoish-3.4.0/zoish/feature_selectors/shap_selectors.py
--rw-r--r--   0        0        0    86006 2023-04-20 18:05:36.403660 zoish-3.4.0/zoish/feature_selectors/single_feature_selectors.py
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403823 zoish-3.4.0/zoish/logs/zoish.log
--rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403960 zoish-3.4.0/zoish/mediators/mediators.py
--rw-r--r--   0        0        0       95 2023-04-20 18:05:36.404077 zoish-3.4.0/zoish/project_conf.py
--rw-r--r--   0        0        0       48 2023-04-25 16:04:07.187113 zoish-3.4.0/zoish/version.py
--rw-r--r--   0        0        0    12618 1970-01-01 00:00:00.000000 zoish-3.4.0/setup.py
--rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 zoish-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1323 2023-04-20 18:05:36.346876 zoish-3.5.0/LICENSE
+-rw-r--r--   0        0        0    10737 2023-04-20 18:05:36.347039 zoish-3.5.0/README.md
+-rw-r--r--   0        0        0     1264 2023-04-25 22:23:05.050109 zoish-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-04-20 18:05:36.358370 zoish-3.5.0/zoish/.env
+-rw-r--r--   0        0        0      925 2023-04-25 22:23:05.051109 zoish-3.5.0/zoish/__init__.py
+-rw-r--r--   0        0        0     1938 2023-04-20 18:05:36.358804 zoish-3.5.0/zoish/abstracs/feature_selector_abstracts.py
+-rw-r--r--   0        0        0    60046 2023-04-20 18:05:36.359334 zoish-3.5.0/zoish/base_classes/best_estimator_getters.py
+-rw-r--r--   0        0        0      675 2023-04-20 18:05:36.359553 zoish-3.5.0/zoish/config.yaml
+-rw-r--r--   0        0        0      375 2023-04-20 18:05:36.359847 zoish-3.5.0/zoish/decorators/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.360014 zoish-3.5.0/zoish/examples/__init__.py
+-rw-r--r--   0        0        0    54613 2023-04-20 18:05:36.361103 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    42652 2023-04-20 18:05:36.361831 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61640 2023-04-20 18:05:36.362393 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb
+-rw-r--r--   0        0        0    97297 2023-04-20 18:05:36.362969 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0   114986 2023-04-20 18:05:36.363251 zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    20432 2023-04-20 18:05:36.363794 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    40581 2023-04-20 18:05:36.364116 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    63450 2023-04-20 18:05:36.364446 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb
+-rw-r--r--   0        0        0    56051 2023-04-20 18:05:36.364756 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    71923 2023-04-20 18:05:36.365059 zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb
+-rw-r--r--   0        0        0    22310 2023-04-20 18:05:36.365292 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    53217 2023-04-20 18:05:36.365575 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61941 2023-04-20 18:05:36.366026 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb
+-rw-r--r--   0        0        0   102159 2023-04-20 18:05:36.366576 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   118140 2023-04-20 18:05:36.366880 zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.367139 zoish-3.5.0/zoish/examples/shap/__init__.py
+-rw-r--r--   0        0        0    21194 2023-04-20 18:05:36.369666 zoish-3.5.0/zoish/examples/shap/shap_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    58856 2023-04-20 18:05:36.370122 zoish-3.5.0/zoish/examples/shap/shap_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    61444 2023-04-20 18:05:36.373990 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_1.ipynb
+-rw-r--r--   0        0        0   413648 2023-04-20 18:05:36.376447 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_2.ipynb
+-rw-r--r--   0        0        0   465032 2023-04-20 18:05:36.396730 zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_3.ipynb
+-rw-r--r--   0        0        0    88426 2023-04-20 18:05:36.397119 zoish-3.5.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb
+-rw-r--r--   0        0        0    69117 2023-04-20 18:05:36.397585 zoish-3.5.0/zoish/examples/shap/shap_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.397811 zoish-3.5.0/zoish/examples/single_feature/__init__.py
+-rw-r--r--   0        0        0    40086 2023-04-20 18:05:36.398323 zoish-3.5.0/zoish/examples/single_feature/single_grid_search_classification.ipynb
+-rw-r--r--   0        0        0    45581 2023-04-20 18:05:36.398779 zoish-3.5.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb
+-rw-r--r--   0        0        0    85377 2023-04-20 18:05:36.399183 zoish-3.5.0/zoish/examples/single_feature/single_random_search_classification.ipynb
+-rw-r--r--   0        0        0   106211 2023-04-20 18:05:36.399543 zoish-3.5.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb
+-rw-r--r--   0        0        0   122582 2023-04-20 18:05:36.399841 zoish-3.5.0/zoish/examples/single_feature/single_tune_search_regression.ipynb
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.399998 zoish-3.5.0/zoish/factories/factories.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.400140 zoish-3.5.0/zoish/feature_selectors/__init__.py
+-rw-r--r--   0        0        0    85614 2023-04-20 18:05:36.400421 zoish-3.5.0/zoish/feature_selectors/recursive_feature_addition.py
+-rw-r--r--   0        0        0    85793 2023-04-20 18:05:36.402572 zoish-3.5.0/zoish/feature_selectors/recursive_feature_elimination.py
+-rw-r--r--   0        0        0    85872 2023-04-20 18:05:36.403025 zoish-3.5.0/zoish/feature_selectors/select_by_shuffling.py
+-rw-r--r--   0        0        0   100851 2023-04-20 18:05:36.403301 zoish-3.5.0/zoish/feature_selectors/shap_selectors.py
+-rw-r--r--   0        0        0    86006 2023-04-20 18:05:36.403660 zoish-3.5.0/zoish/feature_selectors/single_feature_selectors.py
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403823 zoish-3.5.0/zoish/logs/zoish.log
+-rw-r--r--   0        0        0        0 2023-04-20 18:05:36.403960 zoish-3.5.0/zoish/mediators/mediators.py
+-rw-r--r--   0        0        0       95 2023-04-20 18:05:36.404077 zoish-3.5.0/zoish/project_conf.py
+-rw-r--r--   0        0        0       48 2023-04-25 22:23:05.052109 zoish-3.5.0/zoish/version.py
+-rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 zoish-3.5.0/PKG-INFO
```

### Comparing `zoish-3.4.0/LICENSE` & `zoish-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/README.md` & `zoish-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/pyproject.toml` & `zoish-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoish"
-version = "3.4.0"
+version = "3.5.0"
 description = "Zoish: Automated feature selectoion tools"
 
 authors = ["drhosseinjavedani <h.javedani@gmail.com>"]
 homepage = "https://github.com/drhosseinjavedani/zoish"
 license = "BSD 2-Clause License"
 
 readme = "README.md"
```

### Comparing `zoish-3.4.0/zoish/__init__.py` & `zoish-3.5.0/zoish/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.4.0"
+__version__ = "3.5.0"
 
 import logging
 import logging.config
 import os
 
 import yaml
 from dotenv import load_dotenv
```

### Comparing `zoish-3.4.0/zoish/abstracs/feature_selector_abstracts.py` & `zoish-3.5.0/zoish/abstracs/feature_selector_abstracts.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/base_classes/best_estimator_getters.py` & `zoish-3.5.0/zoish/base_classes/best_estimator_getters.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/config.yaml` & `zoish-3.5.0/zoish/config.yaml`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_addition_features/recursive_addition_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/recursive_elimination_features/recursive_elimination_tune_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb` & `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/select_by_shuffling/select_by_shuffling_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_grid_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_optuna_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_1.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_1.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_2.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_2.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_random_search_classification_3.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_random_search_classification_3.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_tune_gridsearch_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/shap/shap_tune_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/shap/shap_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/single_feature/single_grid_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/single_feature/single_grid_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/single_feature/single_optuna_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/single_feature/single_random_search_classification.ipynb` & `zoish-3.5.0/zoish/examples/single_feature/single_random_search_classification.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb` & `zoish-3.5.0/zoish/examples/single_feature/single_tune_gridsearch_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/examples/single_feature/single_tune_search_regression.ipynb` & `zoish-3.5.0/zoish/examples/single_feature/single_tune_search_regression.ipynb`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/feature_selectors/recursive_feature_addition.py` & `zoish-3.5.0/zoish/feature_selectors/recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/feature_selectors/recursive_feature_elimination.py` & `zoish-3.5.0/zoish/feature_selectors/recursive_feature_elimination.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/feature_selectors/select_by_shuffling.py` & `zoish-3.5.0/zoish/feature_selectors/select_by_shuffling.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/feature_selectors/shap_selectors.py` & `zoish-3.5.0/zoish/feature_selectors/shap_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/zoish/feature_selectors/single_feature_selectors.py` & `zoish-3.5.0/zoish/feature_selectors/single_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `zoish-3.4.0/setup.py` & `zoish-3.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,269 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: zoish
+Version: 3.5.0
+Summary: Zoish: Automated feature selectoion tools
+Home-page: https://github.com/drhosseinjavedani/zoish
+License: BSD 2-Clause License
+Keywords: Auto ML,Feature Selection,Pipeline,Machine learning,shap
+Author: drhosseinjavedani
+Author-email: h.javedani@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: catboost (>=1.0.6,<2.0.0)
+Requires-Dist: category-encoders (>=2.5.0,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: fasttreeshap (>=0.1.2,<0.2.0)
+Requires-Dist: feature-engine (>=1.4.1,<2.0.0)
+Requires-Dist: imblearn (>=0.0,<0.1)
+Requires-Dist: lightgbm (>=3.3.2,<4.0.0)
+Requires-Dist: lohrasb (>=3.1.0,<4.0.0)
+Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
+Requires-Dist: numba (>=0.55.2,<0.56.0)
+Requires-Dist: numpy (<1.63.0)
+Requires-Dist: optuna (>=2.10.1,<3.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: pip-licenses (>=3.5.4,<4.0.0)
+Requires-Dist: prompt-toolkit (>=3.0.37,<4.0.0)
+Requires-Dist: pycox (>=0.2.3,<0.3.0)
+Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
+Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: shap (>=0.41.0,<0.42.0)
+Requires-Dist: xgboost (>=1.6.1,<2.0.0)
+Requires-Dist: xgbse (>=0.2.3,<0.3.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['zoish',
- 'zoish.abstracs',
- 'zoish.base_classes',
- 'zoish.decorators',
- 'zoish.examples',
- 'zoish.examples.shap',
- 'zoish.examples.single_feature',
- 'zoish.factories',
- 'zoish.feature_selectors',
- 'zoish.mediators']
-
-package_data = \
-{'': ['*'],
- 'zoish': ['logs/*'],
- 'zoish.examples': ['recursive_addition_features/*',
-                    'recursive_elimination_features/*',
-                    'select_by_shuffling/*']}
-
-install_requires = \
-['catboost>=1.0.6,<2.0.0',
- 'category-encoders>=2.5.0,<3.0.0',
- 'click>=8.1.3,<9.0.0',
- 'fasttreeshap>=0.1.2,<0.2.0',
- 'feature-engine>=1.4.1,<2.0.0',
- 'imblearn>=0.0,<0.1',
- 'lightgbm>=3.3.2,<4.0.0',
- 'lohrasb>=3.1.0,<4.0.0',
- 'matplotlib>=3.5.2,<4.0.0',
- 'numba>=0.55.2,<0.56.0',
- 'numpy<1.63.0',
- 'optuna>=2.10.1,<3.0.0',
- 'pandas>=1.4.3,<2.0.0',
- 'pip-licenses>=3.5.4,<4.0.0',
- 'prompt-toolkit>=3.0.37,<4.0.0',
- 'pycox>=0.2.3,<0.3.0',
- 'python-dotenv>=0.21.0,<0.22.0',
- 'scikit-learn>=1.1.1,<2.0.0',
- 'scipy>=1.8.1,<2.0.0',
- 'shap>=0.41.0,<0.42.0',
- 'xgboost>=1.6.1,<2.0.0',
- 'xgbse>=0.2.3,<0.3.0']
-
-setup_kwargs = {
-    'name': 'zoish',
-    'version': '3.4.0',
-    'description': 'Zoish: Automated feature selectoion tools',
-    'long_description': '\n![GitHub Repo stars](https://img.shields.io/github/stars/TorkamaniLab/zoish?style=social) ![GitHub forks](https://img.shields.io/github/forks/TorkamaniLab/zoish?style=social) ![GitHub language count](https://img.shields.io/github/languages/count/TorkamaniLab/zoish) ![GitHub repo size](https://img.shields.io/github/repo-size/TorkamaniLab/zoish) ![GitHub](https://img.shields.io/github/license/TorkamaniLab/zoish) ![PyPI - Downloads](https://img.shields.io/pypi/dd/zoish) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zoish) \n\n# Zoish\n\nZoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  \n- Select By Single Feature Performance\n- Recursive Feature Elimination\n- Recursive Feature Addition\n- Select By Shuffling\n\nAll of them are compatible with [scikit-learn](https://scikit-learn.org) pipeline. \n\n\n## Introduction\n\nAll of the above-mentioned modules of Zoish have class factories that have various methods and parameters. From an estimator to its tunning parameters and from optimizers to their parameters, the final goal is to automate the feature selection of the ML pipeline in a proper way. Optimizers like [Optuna](https://optuna.org/), [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) , [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), [TuneGridSearchCV, and TuneSearchCV](https://github.com/ray-project/tune-sklearn) has critical role in Zoish. They are used to provide the best estimator on a train set that is later used by feature selectors to check what features can improve the accuracy of this best estimator based on desired metrics. In short, Optimizers use information every bit of information in rain set to select the best feature set. \n\nThe main process in Zoish is to split samples to train and validation set, and then optimization will estimate optimal hyper-parameters of the estimators. After that, this best estimator will be input to the feature selection objects and finally, the best subset of features with higher grades will be returned. This subset can be used as the next steps of the ML pipeline. In the next paragraphs, more details about feature selector modules have provided.\n\n### ShapFeatureSelectorFactory\n\nShapFeatureSelectorFactory uses  [SHAP](https://arxiv.org/abs/1705.07874) (SHapley Additive exPlanation)  for a better feature selection. This package uses [FastTreeSHAP](https://arxiv.org/abs/2109.09847) while calculating shap values and [SHAP](https://shap.readthedocs.io/en/latest/index.html) for plotting. Using this module users can : \n\n- find features using the best estimator of tree-based models with the highest shap values after hyper-parameter optimization.\n- draw some shap related plots for selected features.\n- return a  Pandas data frame with a list of features and shap values. \n\n### RecursiveFeatureEliminationFeatureSelectorFactory\n\nThe job of this factory class is to ease the selection of features by following a recursive elimination process. The process uses the best estimator found by the optimizer using all the features. Then it ranks the features according to their importance derived from the best estimator. In the next step, it removes the least important feature and fits again with the best estimator. It calculates the performance of the best estimator again and calculates the performance difference between the new and old results. If the performance drop is below the threshold the feature is removed, and this process will continue until all features have been evaluated. For more information on the logic of the recursive elimination process visit this [RecursiveFeatureElimination](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureElimination.html) page. \n\n### RecursiveFeatureAdditionFeatureSelectorFactory\nIt is very similar to RecursiveFeatureEliminationFeatureSelectorFactory, however, the logic is the opposite. It selects features following a recursive addition process. Visit [RecursiveFeatureAddition](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureAddition.html) for more details. \n\n### SelectByShufflingFeatureSelectorFactory\n\nIn this module, the selection of features is based on determining the drop in machine learning model performance when each feature’s values are randomly shuffled.\n\nIf the variables are important, a random permutation of their values will decrease dramatically the machine learning model performance. Contrarily, the permutation of the values should have little to no effect on the model performance metric we are assessing if the feature is not predictive. To understand how it works completely go to its official page [SelectByShuffling](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectByShuffling.html).\n\n### SingleFeaturePerformanceFeatureSelectorFactory\n\nIt selects features based on the performance of a machine learning model trained to utilize a single feature. In other words, it trains a machine-learning model for every single feature, then determines each model’s performance. If the performance of the model is greater than a user-specified threshold, then the feature is retained, otherwise removed. Go to this [page](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectBySingleFeaturePerformance.html) for more information. \n\n## Installation\n\nZoish package is available on PyPI and can be installed with pip:\n\n```sh\npip install zoish\n```\n\nFor log configuration in development environment use \n\n```sh\nexport env=dev\n\n```\n\nFor log configuration in production environment use \n\n```sh\nexport env=prod\n```\n\n## Examples \n\n### Import required libraries\n```\nfrom zoish.feature_selectors.shap_selectors import ShapFeatureSelector\nimport pandas as pd\nfrom sklearn.model_selection import train_test_split\nimport pandas as pd\nfrom sklearn.pipeline import Pipeline\nfrom sklearn.metrics import r2_score\nfrom feature_engine.imputation import CategoricalImputer, MeanMedianImputer\nfrom category_encoders import OrdinalEncoder\nimport xgboost\nimport optuna\nfrom optuna.samplers import TPESampler\nfrom optuna.pruners import HyperbandPruner\nfrom sklearn.linear_model import LinearRegression\n```\n\n### Computer Hardware Data Set (a classification problem)\n```\nurldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data"\n# column names\ncol_names=[\n    "vendor name",\n    "Model Name",\n    "MYCT",\n    "MMIN",\n    "MMAX",\n    "CACH",\n    "CHMIN",\n    "CHMAX",\n    "PRP"\n]\n# read data\ndata = pd.read_csv(urldata,header=None,names=col_names,sep=\',\')\n\n```\n### Train test split\n```\nX = data.loc[:, data.columns != "PRP"]\ny = data.loc[:, data.columns == "PRP"]\n\nX_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)\n```\n### Find feature types for later use\n```\nint_cols =  X_train.select_dtypes(include=[\'int\']).columns.tolist()\nfloat_cols =  X_train.select_dtypes(include=[\'float\']).columns.tolist()\ncat_cols =  X_train.select_dtypes(include=[\'object\']).columns.tolist()\n```\n\n###  Define Feature selector and set its arguments  \n```\nshap_feature_selector_factory = (\n    ShapFeatureSelector.shap_feature_selector_factory.set_model_params(\n        X=X_train,\n        y=y_train,\n        verbose=10,\n        random_state=0,\n        estimator=xgboost.XGBRegressor(),\n        estimator_params={\n            "max_depth": [4, 5],\n        },\n        fit_params = {\n            "callbacks": None,\n        },\n        method="optuna",\n        # if n_features=None only the threshold will be considered as a cut-off of features grades.\n        # if threshold=None only n_features will be considered to select the top n features.\n        # if both of them are set to some values, the threshold has the priority for selecting features.\n        n_features=5,\n        threshold = None,\n        list_of_obligatory_features_that_must_be_in_model=[],\n        list_of_features_to_drop_before_any_selection=[],\n    )\n    .set_shap_params(\n        model_output="raw",\n        feature_perturbation="interventional",\n        algorithm="v2",\n        shap_n_jobs=-1,\n        memory_tolerance=-1,\n        feature_names=None,\n        approximate=False,\n        shortcut=False,\n    )\n    .set_optuna_params(\n            measure_of_accuracy="r2_score(y_true, y_pred)",\n            # optuna params\n            with_stratified=False,\n            test_size=.3,\n            n_jobs=-1,\n            # optuna params\n            # optuna study init params\n            study=optuna.create_study(\n                storage=None,\n                sampler=TPESampler(),\n                pruner=HyperbandPruner(),\n                study_name="example of optuna optimizer",\n                direction="maximize",\n                load_if_exists=False,\n                directions=None,\n            ),\n            # optuna optimization params\n            study_optimize_objective=None,\n            study_optimize_objective_n_trials=20,\n            study_optimize_objective_timeout=600,\n            study_optimize_n_jobs=-1,\n            study_optimize_catch=(),\n            study_optimize_callbacks=None,\n            study_optimize_gc_after_trial=False,\n            study_optimize_show_progress_bar=False,\n            )\n)\n\n```\n### Build sklearn Pipeline  \n```\npipeline =Pipeline([\n            # int missing values imputers\n            (\'intimputer\', MeanMedianImputer(\n                imputation_method=\'median\', variables=int_cols)),\n            # category missing values imputers\n            (\'catimputer\', CategoricalImputer(variables=cat_cols)),\n            #\n            (\'catencoder\', OrdinalEncoder()),\n            # feature selection\n            ("sfsf", shap_feature_selector_factory),\n            # add any regression model from sklearn e.g., LinearRegression\n            (\'regression\', LinearRegression())\n\n\n ])\n```\n### Run Pipeline\n```\npipeline.fit(X_train,y_train)\ny_pred = pipeline.predict(X_test)\n\n```\n### Plots\n```\nShapFeatureSelector.shap_feature_selector_factory.plot_features_all(\n    type_of_plot="summary_plot",\n    path_to_save_plot="../plots/shap_optuna_search_regression_summary_plot"\n)\n```\n\n###  Check performance of the Pipeline\n```\nprint(\'r2 score : \')\nprint(r2_score(y_test,y_pred))\n\n```\n### Get access to feature selector instance\n```\nprint(ShapFeatureSelector.shap_feature_selector_factory.get_feature_selector_instance())\n```\n\n\nMore examples are available in the [examples](https://github.com/drhosseinjavedani/zoish/tree/main/zoish/examples). \n\n## License\nLicensed under the [BSD 2-Clause](https://opensource.org/licenses/BSD-2-Clause) License.',
-    'author': 'drhosseinjavedani',
-    'author_email': 'h.javedani@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/drhosseinjavedani/zoish',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
 
+![GitHub Repo stars](https://img.shields.io/github/stars/TorkamaniLab/zoish?style=social) ![GitHub forks](https://img.shields.io/github/forks/TorkamaniLab/zoish?style=social) ![GitHub language count](https://img.shields.io/github/languages/count/TorkamaniLab/zoish) ![GitHub repo size](https://img.shields.io/github/repo-size/TorkamaniLab/zoish) ![GitHub](https://img.shields.io/github/license/TorkamaniLab/zoish) ![PyPI - Downloads](https://img.shields.io/pypi/dd/zoish) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zoish) 
 
-setup(**setup_kwargs)
+# Zoish
+
+Zoish is a package built to ease machine learning development by providing various feature-selecting modules such as:  
+- Select By Single Feature Performance
+- Recursive Feature Elimination
+- Recursive Feature Addition
+- Select By Shuffling
+
+All of them are compatible with [scikit-learn](https://scikit-learn.org) pipeline. 
+
+
+## Introduction
+
+All of the above-mentioned modules of Zoish have class factories that have various methods and parameters. From an estimator to its tunning parameters and from optimizers to their parameters, the final goal is to automate the feature selection of the ML pipeline in a proper way. Optimizers like [Optuna](https://optuna.org/), [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html) , [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html), [TuneGridSearchCV, and TuneSearchCV](https://github.com/ray-project/tune-sklearn) has critical role in Zoish. They are used to provide the best estimator on a train set that is later used by feature selectors to check what features can improve the accuracy of this best estimator based on desired metrics. In short, Optimizers use information every bit of information in rain set to select the best feature set. 
+
+The main process in Zoish is to split samples to train and validation set, and then optimization will estimate optimal hyper-parameters of the estimators. After that, this best estimator will be input to the feature selection objects and finally, the best subset of features with higher grades will be returned. This subset can be used as the next steps of the ML pipeline. In the next paragraphs, more details about feature selector modules have provided.
+
+### ShapFeatureSelectorFactory
+
+ShapFeatureSelectorFactory uses  [SHAP](https://arxiv.org/abs/1705.07874) (SHapley Additive exPlanation)  for a better feature selection. This package uses [FastTreeSHAP](https://arxiv.org/abs/2109.09847) while calculating shap values and [SHAP](https://shap.readthedocs.io/en/latest/index.html) for plotting. Using this module users can : 
+
+- find features using the best estimator of tree-based models with the highest shap values after hyper-parameter optimization.
+- draw some shap related plots for selected features.
+- return a  Pandas data frame with a list of features and shap values. 
+
+### RecursiveFeatureEliminationFeatureSelectorFactory
+
+The job of this factory class is to ease the selection of features by following a recursive elimination process. The process uses the best estimator found by the optimizer using all the features. Then it ranks the features according to their importance derived from the best estimator. In the next step, it removes the least important feature and fits again with the best estimator. It calculates the performance of the best estimator again and calculates the performance difference between the new and old results. If the performance drop is below the threshold the feature is removed, and this process will continue until all features have been evaluated. For more information on the logic of the recursive elimination process visit this [RecursiveFeatureElimination](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureElimination.html) page. 
+
+### RecursiveFeatureAdditionFeatureSelectorFactory
+It is very similar to RecursiveFeatureEliminationFeatureSelectorFactory, however, the logic is the opposite. It selects features following a recursive addition process. Visit [RecursiveFeatureAddition](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/RecursiveFeatureAddition.html) for more details. 
+
+### SelectByShufflingFeatureSelectorFactory
+
+In this module, the selection of features is based on determining the drop in machine learning model performance when each feature’s values are randomly shuffled.
+
+If the variables are important, a random permutation of their values will decrease dramatically the machine learning model performance. Contrarily, the permutation of the values should have little to no effect on the model performance metric we are assessing if the feature is not predictive. To understand how it works completely go to its official page [SelectByShuffling](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectByShuffling.html).
+
+### SingleFeaturePerformanceFeatureSelectorFactory
+
+It selects features based on the performance of a machine learning model trained to utilize a single feature. In other words, it trains a machine-learning model for every single feature, then determines each model’s performance. If the performance of the model is greater than a user-specified threshold, then the feature is retained, otherwise removed. Go to this [page](https://feature-engine.readthedocs.io/en/latest/api_doc/selection/SelectBySingleFeaturePerformance.html) for more information. 
+
+## Installation
+
+Zoish package is available on PyPI and can be installed with pip:
+
+```sh
+pip install zoish
+```
+
+For log configuration in development environment use 
+
+```sh
+export env=dev
+
+```
+
+For log configuration in production environment use 
+
+```sh
+export env=prod
+```
+
+## Examples 
+
+### Import required libraries
+```
+from zoish.feature_selectors.shap_selectors import ShapFeatureSelector
+import pandas as pd
+from sklearn.model_selection import train_test_split
+import pandas as pd
+from sklearn.pipeline import Pipeline
+from sklearn.metrics import r2_score
+from feature_engine.imputation import CategoricalImputer, MeanMedianImputer
+from category_encoders import OrdinalEncoder
+import xgboost
+import optuna
+from optuna.samplers import TPESampler
+from optuna.pruners import HyperbandPruner
+from sklearn.linear_model import LinearRegression
+```
+
+### Computer Hardware Data Set (a classification problem)
+```
+urldata= "https://archive.ics.uci.edu/ml/machine-learning-databases/cpu-performance/machine.data"
+# column names
+col_names=[
+    "vendor name",
+    "Model Name",
+    "MYCT",
+    "MMIN",
+    "MMAX",
+    "CACH",
+    "CHMIN",
+    "CHMAX",
+    "PRP"
+]
+# read data
+data = pd.read_csv(urldata,header=None,names=col_names,sep=',')
+
+```
+### Train test split
+```
+X = data.loc[:, data.columns != "PRP"]
+y = data.loc[:, data.columns == "PRP"]
+
+X_train, X_test, y_train, y_test =train_test_split(X, y, test_size=0.33, random_state=42)
+```
+### Find feature types for later use
+```
+int_cols =  X_train.select_dtypes(include=['int']).columns.tolist()
+float_cols =  X_train.select_dtypes(include=['float']).columns.tolist()
+cat_cols =  X_train.select_dtypes(include=['object']).columns.tolist()
+```
+
+###  Define Feature selector and set its arguments  
+```
+shap_feature_selector_factory = (
+    ShapFeatureSelector.shap_feature_selector_factory.set_model_params(
+        X=X_train,
+        y=y_train,
+        verbose=10,
+        random_state=0,
+        estimator=xgboost.XGBRegressor(),
+        estimator_params={
+            "max_depth": [4, 5],
+        },
+        fit_params = {
+            "callbacks": None,
+        },
+        method="optuna",
+        # if n_features=None only the threshold will be considered as a cut-off of features grades.
+        # if threshold=None only n_features will be considered to select the top n features.
+        # if both of them are set to some values, the threshold has the priority for selecting features.
+        n_features=5,
+        threshold = None,
+        list_of_obligatory_features_that_must_be_in_model=[],
+        list_of_features_to_drop_before_any_selection=[],
+    )
+    .set_shap_params(
+        model_output="raw",
+        feature_perturbation="interventional",
+        algorithm="v2",
+        shap_n_jobs=-1,
+        memory_tolerance=-1,
+        feature_names=None,
+        approximate=False,
+        shortcut=False,
+    )
+    .set_optuna_params(
+            measure_of_accuracy="r2_score(y_true, y_pred)",
+            # optuna params
+            with_stratified=False,
+            test_size=.3,
+            n_jobs=-1,
+            # optuna params
+            # optuna study init params
+            study=optuna.create_study(
+                storage=None,
+                sampler=TPESampler(),
+                pruner=HyperbandPruner(),
+                study_name="example of optuna optimizer",
+                direction="maximize",
+                load_if_exists=False,
+                directions=None,
+            ),
+            # optuna optimization params
+            study_optimize_objective=None,
+            study_optimize_objective_n_trials=20,
+            study_optimize_objective_timeout=600,
+            study_optimize_n_jobs=-1,
+            study_optimize_catch=(),
+            study_optimize_callbacks=None,
+            study_optimize_gc_after_trial=False,
+            study_optimize_show_progress_bar=False,
+            )
+)
+
+```
+### Build sklearn Pipeline  
+```
+pipeline =Pipeline([
+            # int missing values imputers
+            ('intimputer', MeanMedianImputer(
+                imputation_method='median', variables=int_cols)),
+            # category missing values imputers
+            ('catimputer', CategoricalImputer(variables=cat_cols)),
+            #
+            ('catencoder', OrdinalEncoder()),
+            # feature selection
+            ("sfsf", shap_feature_selector_factory),
+            # add any regression model from sklearn e.g., LinearRegression
+            ('regression', LinearRegression())
+
+
+ ])
+```
+### Run Pipeline
+```
+pipeline.fit(X_train,y_train)
+y_pred = pipeline.predict(X_test)
+
+```
+### Plots
+```
+ShapFeatureSelector.shap_feature_selector_factory.plot_features_all(
+    type_of_plot="summary_plot",
+    path_to_save_plot="../plots/shap_optuna_search_regression_summary_plot"
+)
+```
+
+###  Check performance of the Pipeline
+```
+print('r2 score : ')
+print(r2_score(y_test,y_pred))
+
+```
+### Get access to feature selector instance
+```
+print(ShapFeatureSelector.shap_feature_selector_factory.get_feature_selector_instance())
+```
+
+
+More examples are available in the [examples](https://github.com/drhosseinjavedani/zoish/tree/main/zoish/examples). 
+
+## License
+Licensed under the [BSD 2-Clause](https://opensource.org/licenses/BSD-2-Clause) License.
```

