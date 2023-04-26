# Comparing `tmp/serialzy-1.1.0.tar.gz` & `tmp/serialzy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialzy-1.1.0.tar", last modified: Tue Mar 14 10:13:39 2023, max compression
+gzip compressed data, was "serialzy-1.1.1.tar", last modified: Tue Apr 25 16:58:19 2023, max compression
```

## Comparing `serialzy-1.1.0.tar` & `serialzy-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-14 10:13:39.658086 serialzy-1.1.0/
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      659 2023-03-10 14:21:54.000000 serialzy-1.1.0/AUTHORS
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      578 2023-03-10 14:21:54.000000 serialzy-1.1.0/LICENSE
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       40 2023-03-10 14:21:54.000000 serialzy-1.1.0/MANIFEST.in
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7496 2023-03-14 10:13:39.657440 serialzy-1.1.0/PKG-INFO
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7094 2023-03-10 14:21:54.000000 serialzy-1.1.0/README.md
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      329 2023-03-10 14:21:54.000000 serialzy-1.1.0/pyproject.toml
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       57 2023-03-10 14:21:54.000000 serialzy-1.1.0/requirements.txt
-drwxr-xr-x   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-14 10:13:39.645678 serialzy-1.1.0/serialzy/
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       33 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/__init__.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7468 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/api.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     2928 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/base.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     2162 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/cloudpickle.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       41 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/errors.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7647 2023-03-13 12:55:58.000000 serialzy-1.1.0/serialzy/registry.py
-drwxr-xr-x   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-14 10:13:39.656288 serialzy-1.1.0/serialzy/serializers/
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/serializers/__init__.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     3845 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/serializers/base_model.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     2103 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/catboost.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1562 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/ellipsis.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1016 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/lightgbm.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1424 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/primitive.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     2812 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/proto.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7446 2023-03-13 13:42:09.000000 serialzy-1.1.0/serialzy/serializers/sequence.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1912 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/tensorflow.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1028 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/torch.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     6582 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/union.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1111 2023-03-11 12:46:45.000000 serialzy-1.1.0/serialzy/serializers/xgboost.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1317 2023-03-11 16:34:05.000000 serialzy-1.1.0/serialzy/types.py
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      795 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/utils.py
-drwxr-xr-x   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-14 10:13:39.656819 serialzy-1.1.0/serialzy/version/
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)        6 2023-03-13 13:52:18.000000 serialzy-1.1.0/serialzy/version/version
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      129 2023-03-10 14:21:54.000000 serialzy-1.1.0/serialzy/version.py
-drwxr-xr-x   0 tomato   (425660600) LD\Domain Users (593637566)        0 2023-03-14 10:13:39.648708 serialzy-1.1.0/serialzy.egg-info/
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     7496 2023-03-14 10:13:39.000000 serialzy-1.1.0/serialzy.egg-info/PKG-INFO
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)      827 2023-03-14 10:13:39.000000 serialzy-1.1.0/serialzy.egg-info/SOURCES.txt
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)        1 2023-03-14 10:13:39.000000 serialzy-1.1.0/serialzy.egg-info/dependency_links.txt
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       58 2023-03-14 10:13:39.000000 serialzy-1.1.0/serialzy.egg-info/requires.txt
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       30 2023-03-14 10:13:39.000000 serialzy-1.1.0/serialzy.egg-info/top_level.txt
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)       38 2023-03-14 10:13:39.658244 serialzy-1.1.0/setup.cfg
--rw-r--r--   0 tomato   (425660600) LD\Domain Users (593637566)     1106 2023-03-10 14:21:54.000000 serialzy-1.1.0/setup.py
+drwxr-xr-x   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-04-25 16:58:19.826357 serialzy-1.1.1/
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       40 2023-01-25 18:09:39.000000 serialzy-1.1.1/MANIFEST.in
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     8087 2023-04-25 16:58:19.825829 serialzy-1.1.1/PKG-INFO
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     7094 2023-03-07 14:20:04.000000 serialzy-1.1.1/README.md
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)      329 2023-01-25 18:09:39.000000 serialzy-1.1.1/pyproject.toml
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       57 2023-01-25 18:09:39.000000 serialzy-1.1.1/requirements.txt
+drwxr-xr-x   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-04-25 16:58:19.810638 serialzy-1.1.1/serialzy/
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       33 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/__init__.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     7468 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/api.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     2928 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/base.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     2162 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/cloudpickle.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       41 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/errors.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1663 2023-04-25 16:57:31.000000 serialzy-1.1.1/serialzy/exception.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     7768 2023-04-25 16:57:31.000000 serialzy-1.1.1/serialzy/registry.py
+drwxr-xr-x   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-04-25 16:58:19.824316 serialzy-1.1.1/serialzy/serializers/
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/serializers/__init__.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     3845 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/base_model.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     2103 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/catboost.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1562 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/serializers/ellipsis.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1016 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/lightgbm.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1424 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/serializers/primitive.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     2812 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/serializers/proto.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     7446 2023-04-24 08:43:20.000000 serialzy-1.1.1/serialzy/serializers/sequence.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1912 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/tensorflow.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1028 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/torch.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     6582 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/union.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1111 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/serializers/xgboost.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1317 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/types.py
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)      795 2023-03-07 14:20:04.000000 serialzy-1.1.1/serialzy/utils.py
+drwxr-xr-x   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-04-25 16:58:19.825051 serialzy-1.1.1/serialzy/version/
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)        6 2023-04-25 16:56:35.000000 serialzy-1.1.1/serialzy/version/version
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)      129 2023-01-25 18:09:39.000000 serialzy-1.1.1/serialzy/version.py
+drwxr-xr-x   0 whitecloud (806798049) LD\Domain Users (593637566)        0 2023-04-25 16:58:19.813867 serialzy-1.1.1/serialzy.egg-info/
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     8087 2023-04-25 16:58:19.000000 serialzy-1.1.1/serialzy.egg-info/PKG-INFO
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)      833 2023-04-25 16:58:19.000000 serialzy-1.1.1/serialzy.egg-info/SOURCES.txt
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)        1 2023-04-25 16:58:19.000000 serialzy-1.1.1/serialzy.egg-info/dependency_links.txt
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       58 2023-04-25 16:58:19.000000 serialzy-1.1.1/serialzy.egg-info/requires.txt
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       30 2023-04-25 16:58:19.000000 serialzy-1.1.1/serialzy.egg-info/top_level.txt
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)       38 2023-04-25 16:58:19.826597 serialzy-1.1.1/setup.cfg
+-rw-r--r--   0 whitecloud (806798049) LD\Domain Users (593637566)     1106 2023-01-25 18:09:39.000000 serialzy-1.1.1/setup.py
```

### Comparing `serialzy-1.1.0/PKG-INFO` & `serialzy-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 Metadata-Version: 2.1
 Name: serialzy
-Version: 1.1.0
+Version: 1.1.1
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: ʎzy developers
 License: LICENSE
+Description: [![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
+        [![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
+        [![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
+        
+        # serialzy
+        
+        Serialzy is a library for python objects serialization into portable and interoperable data formats (if possible).
+        
+        ### Example
+        
+        Suppose you have a catboost model:
+        
+        ```python
+        from catboost import CatBoostClassifier
+        
+        model = CatBoostClassifier()
+        model.fit(...)
+        ```
+        
+        Firstly you should find a proper serializer for the catboost model type or the corresponding data format:
+        
+        ```python
+        from serialzy.registry import DefaultSerializerRegistry
+        
+        registry = DefaultSerializerRegistry()
+        serializer = registry.find_serializer_by_type(type(model)) # registry.find_serializer_by_data_format("cbm")
+        ```
+        
+        Serializers have several properties:
+        
+        ```python
+        serializer.available()      # can be used in the current environment
+        serializer.requirements()   # libraries needed to be installed to use this serializer
+        serializer.stable()         # has portable data format
+        ```
+        
+        Serializers can provide data format and schema for a type:
+        
+        ```python
+        serializer.data_format()
+        serializer.schema(type(model))
+        ```
+        
+        Serialization:
+        
+        ```python
+        with open('model.cbm', 'wb') as file:
+            serializer.serialize(model, file)
+        ```
+        
+        Deserialization:
+        
+        ```python
+        with open('result', 'rb') as file:
+            deserialized_obj = serializer.deserialize(file)
+        ```
+        
+        ### List of supported libraries for stable serialization:
+        
+        | Library                                     | Types                                                                                                                                                                                                                                                                                                                | Data format                                                                                                   | 
+        |---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
+        | Python std lib                              | int, str, float, bool, None                                                                                                                                                                                                                                                                                          | [string representation](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/primitive.py)                                                                                     |
+        | Python std lib                              | List, Tuple                                                                                                                                                                                                                                                                                                          | [custom format](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/sequence.py)              |
+        | [CatBoost](https://catboost.ai)             | [CatBoostRegressor](https://catboost.ai/en/docs/concepts/python-reference_catboostregressor), [CatBoostClassifier](https://catboost.ai/en/docs/concepts/python-reference_catboostclassifier), [CatBoostRanker](https://catboost.ai/en/docs/concepts/python-reference_catboostranker)                                 | [cbm](https://catboost.ai/en/docs/concepts/python-reference_catboost_save_model)                              |
+        | [CatBoost](https://catboost.ai)             | [Pool](https://catboost.ai/en/docs/concepts/python-reference_pool)                                                                                                                                                                                                                                                   | [quantized pool](https://catboost.ai/en/docs/concepts/python-reference_pool_save)                             |
+        | [Tensorflow.Keras](https://keras.io)        | [Sequential](https://keras.io/guides/sequential_model/), [Model](https://keras.io/api/models/model/) with subclasses                                                                                                                                                                                                 | [tf_keras](https://keras.io/api/models/model_saving_apis/)                                                    |
+        | [Tensorflow](https://www.tensorflow.org)    | [Checkpoint](https://www.tensorflow.org/api_docs/python/tf/train/Checkpoint), [Module](https://www.tensorflow.org/api_docs/python/tf/Module) with subclasses                                                                                                                                                         | [tf_pure](https://www.tensorflow.org/api_docs/python/tf/saved_model)                                          |
+        | [LightGBM](https://lightgbm.readthedocs.io) | [LGBMClassifier](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMClassifier.html), [LGBMRegressor](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRegressor.html), [LGBMRanker](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRanker.html)                     | [lgbm](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.Booster.html#lightgbm.Booster.save_model) |
+        | [XGBoost](https://lightgbm.readthedocs.io)  | [XGBClassifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRegressor](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRanker](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn) | [xgb](https://xgboost.readthedocs.io/en/latest/python/python_intro.html#training)                             |
+        | [Torch](https://pytorch.org)                | [Module](https://pytorch.org/docs/stable/notes/modules.html) with subclasses                                                                                                                                                                                                                                         | [pt](https://pytorch.org/docs/stable/generated/torch.jit.save.html#torch.jit.save)                            |
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-[![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
-[![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
-[![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
-
-# serialzy
-
-Serialzy is a library for python objects serialization into portable and interoperable data formats (if possible).
-
-### Example
-
-Suppose you have a catboost model:
-
-```python
-from catboost import CatBoostClassifier
-
-model = CatBoostClassifier()
-model.fit(...)
-```
-
-Firstly you should find a proper serializer for the catboost model type or the corresponding data format:
-
-```python
-from serialzy.registry import DefaultSerializerRegistry
-
-registry = DefaultSerializerRegistry()
-serializer = registry.find_serializer_by_type(type(model)) # registry.find_serializer_by_data_format("cbm")
-```
-
-Serializers have several properties:
-
-```python
-serializer.available()      # can be used in the current environment
-serializer.requirements()   # libraries needed to be installed to use this serializer
-serializer.stable()         # has portable data format
-```
-
-Serializers can provide data format and schema for a type:
-
-```python
-serializer.data_format()
-serializer.schema(type(model))
-```
-
-Serialization:
-
-```python
-with open('model.cbm', 'wb') as file:
-    serializer.serialize(model, file)
-```
-
-Deserialization:
-
-```python
-with open('result', 'rb') as file:
-    deserialized_obj = serializer.deserialize(file)
-```
-
-### List of supported libraries for stable serialization:
-
-| Library                                     | Types                                                                                                                                                                                                                                                                                                                | Data format                                                                                                   | 
-|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
-| Python std lib                              | int, str, float, bool, None                                                                                                                                                                                                                                                                                          | [string representation](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/primitive.py)                                                                                     |
-| Python std lib                              | List, Tuple                                                                                                                                                                                                                                                                                                          | [custom format](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/sequence.py)              |
-| [CatBoost](https://catboost.ai)             | [CatBoostRegressor](https://catboost.ai/en/docs/concepts/python-reference_catboostregressor), [CatBoostClassifier](https://catboost.ai/en/docs/concepts/python-reference_catboostclassifier), [CatBoostRanker](https://catboost.ai/en/docs/concepts/python-reference_catboostranker)                                 | [cbm](https://catboost.ai/en/docs/concepts/python-reference_catboost_save_model)                              |
-| [CatBoost](https://catboost.ai)             | [Pool](https://catboost.ai/en/docs/concepts/python-reference_pool)                                                                                                                                                                                                                                                   | [quantized pool](https://catboost.ai/en/docs/concepts/python-reference_pool_save)                             |
-| [Tensorflow.Keras](https://keras.io)        | [Sequential](https://keras.io/guides/sequential_model/), [Model](https://keras.io/api/models/model/) with subclasses                                                                                                                                                                                                 | [tf_keras](https://keras.io/api/models/model_saving_apis/)                                                    |
-| [Tensorflow](https://www.tensorflow.org)    | [Checkpoint](https://www.tensorflow.org/api_docs/python/tf/train/Checkpoint), [Module](https://www.tensorflow.org/api_docs/python/tf/Module) with subclasses                                                                                                                                                         | [tf_pure](https://www.tensorflow.org/api_docs/python/tf/saved_model)                                          |
-| [LightGBM](https://lightgbm.readthedocs.io) | [LGBMClassifier](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMClassifier.html), [LGBMRegressor](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRegressor.html), [LGBMRanker](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRanker.html)                     | [lgbm](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.Booster.html#lightgbm.Booster.save_model) |
-| [XGBoost](https://lightgbm.readthedocs.io)  | [XGBClassifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRegressor](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRanker](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn) | [xgb](https://xgboost.readthedocs.io/en/latest/python/python_intro.html#training)                             |
-| [Torch](https://pytorch.org)                | [Module](https://pytorch.org/docs/stable/notes/modules.html) with subclasses                                                                                                                                                                                                                                         | [pt](https://pytorch.org/docs/stable/generated/torch.jit.save.html#torch.jit.save)                            |
```

### Comparing `serialzy-1.1.0/README.md` & `serialzy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/api.py` & `serialzy-1.1.1/serialzy/api.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/base.py` & `serialzy-1.1.1/serialzy/base.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/cloudpickle.py` & `serialzy-1.1.1/serialzy/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/registry.py` & `serialzy-1.1.1/serialzy/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import defaultdict
 from types import ModuleType
 from typing import Dict, List, Optional, Type, cast, Iterable, Any
 
 import serialzy.serializers
 from serialzy.api import Serializer, SerializerRegistry
 from serialzy.cloudpickle import CloudpickleSerializer
+from serialzy.exception import register_exception_serializer_to_pickle
 from serialzy.utils import load_all_modules_from
 from serialzy.types import get_type
 
 _LOG = logging.getLogger(__name__)
 
 
 class DefaultSerializerRegistry(SerializerRegistry):
@@ -34,14 +35,15 @@
                 continue
             if serializer.stable():
                 self.register_serializer(serializer, self._default_priority_stable)
             else:
                 self.register_serializer(serializer, self._default_priority_unstable)
         # cloudpickle has the least priority
         self.register_serializer(CloudpickleSerializer(), sys.maxsize - 1)
+        register_exception_serializer_to_pickle()
 
     def register_serializer(self, serializer: Serializer, priority: Optional[int] = None) -> None:
         self._serializer_type_cache.clear()
         self._serializer_data_format_cache.clear()
 
         serializer_type = type(serializer)
         if serializer_type in self._serializer_registry:
```

### Comparing `serialzy-1.1.0/serialzy/serializers/base_model.py` & `serialzy-1.1.1/serialzy/serializers/base_model.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/catboost.py` & `serialzy-1.1.1/serialzy/serializers/catboost.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/ellipsis.py` & `serialzy-1.1.1/serialzy/serializers/ellipsis.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/lightgbm.py` & `serialzy-1.1.1/serialzy/serializers/lightgbm.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/primitive.py` & `serialzy-1.1.1/serialzy/serializers/primitive.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/proto.py` & `serialzy-1.1.1/serialzy/serializers/proto.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/sequence.py` & `serialzy-1.1.1/serialzy/serializers/sequence.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/tensorflow.py` & `serialzy-1.1.1/serialzy/serializers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/torch.py` & `serialzy-1.1.1/serialzy/serializers/torch.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/union.py` & `serialzy-1.1.1/serialzy/serializers/union.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/serializers/xgboost.py` & `serialzy-1.1.1/serialzy/serializers/xgboost.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/types.py` & `serialzy-1.1.1/serialzy/types.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy/utils.py` & `serialzy-1.1.1/serialzy/utils.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.1.0/serialzy.egg-info/PKG-INFO` & `serialzy-1.1.1/serialzy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 Metadata-Version: 2.1
 Name: serialzy
-Version: 1.1.0
+Version: 1.1.1
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: ʎzy developers
 License: LICENSE
+Description: [![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
+        [![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
+        [![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
+        
+        # serialzy
+        
+        Serialzy is a library for python objects serialization into portable and interoperable data formats (if possible).
+        
+        ### Example
+        
+        Suppose you have a catboost model:
+        
+        ```python
+        from catboost import CatBoostClassifier
+        
+        model = CatBoostClassifier()
+        model.fit(...)
+        ```
+        
+        Firstly you should find a proper serializer for the catboost model type or the corresponding data format:
+        
+        ```python
+        from serialzy.registry import DefaultSerializerRegistry
+        
+        registry = DefaultSerializerRegistry()
+        serializer = registry.find_serializer_by_type(type(model)) # registry.find_serializer_by_data_format("cbm")
+        ```
+        
+        Serializers have several properties:
+        
+        ```python
+        serializer.available()      # can be used in the current environment
+        serializer.requirements()   # libraries needed to be installed to use this serializer
+        serializer.stable()         # has portable data format
+        ```
+        
+        Serializers can provide data format and schema for a type:
+        
+        ```python
+        serializer.data_format()
+        serializer.schema(type(model))
+        ```
+        
+        Serialization:
+        
+        ```python
+        with open('model.cbm', 'wb') as file:
+            serializer.serialize(model, file)
+        ```
+        
+        Deserialization:
+        
+        ```python
+        with open('result', 'rb') as file:
+            deserialized_obj = serializer.deserialize(file)
+        ```
+        
+        ### List of supported libraries for stable serialization:
+        
+        | Library                                     | Types                                                                                                                                                                                                                                                                                                                | Data format                                                                                                   | 
+        |---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
+        | Python std lib                              | int, str, float, bool, None                                                                                                                                                                                                                                                                                          | [string representation](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/primitive.py)                                                                                     |
+        | Python std lib                              | List, Tuple                                                                                                                                                                                                                                                                                                          | [custom format](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/sequence.py)              |
+        | [CatBoost](https://catboost.ai)             | [CatBoostRegressor](https://catboost.ai/en/docs/concepts/python-reference_catboostregressor), [CatBoostClassifier](https://catboost.ai/en/docs/concepts/python-reference_catboostclassifier), [CatBoostRanker](https://catboost.ai/en/docs/concepts/python-reference_catboostranker)                                 | [cbm](https://catboost.ai/en/docs/concepts/python-reference_catboost_save_model)                              |
+        | [CatBoost](https://catboost.ai)             | [Pool](https://catboost.ai/en/docs/concepts/python-reference_pool)                                                                                                                                                                                                                                                   | [quantized pool](https://catboost.ai/en/docs/concepts/python-reference_pool_save)                             |
+        | [Tensorflow.Keras](https://keras.io)        | [Sequential](https://keras.io/guides/sequential_model/), [Model](https://keras.io/api/models/model/) with subclasses                                                                                                                                                                                                 | [tf_keras](https://keras.io/api/models/model_saving_apis/)                                                    |
+        | [Tensorflow](https://www.tensorflow.org)    | [Checkpoint](https://www.tensorflow.org/api_docs/python/tf/train/Checkpoint), [Module](https://www.tensorflow.org/api_docs/python/tf/Module) with subclasses                                                                                                                                                         | [tf_pure](https://www.tensorflow.org/api_docs/python/tf/saved_model)                                          |
+        | [LightGBM](https://lightgbm.readthedocs.io) | [LGBMClassifier](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMClassifier.html), [LGBMRegressor](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRegressor.html), [LGBMRanker](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRanker.html)                     | [lgbm](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.Booster.html#lightgbm.Booster.save_model) |
+        | [XGBoost](https://lightgbm.readthedocs.io)  | [XGBClassifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRegressor](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRanker](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn) | [xgb](https://xgboost.readthedocs.io/en/latest/python/python_intro.html#training)                             |
+        | [Torch](https://pytorch.org)                | [Module](https://pytorch.org/docs/stable/notes/modules.html) with subclasses                                                                                                                                                                                                                                         | [pt](https://pytorch.org/docs/stable/generated/torch.jit.save.html#torch.jit.save)                            |
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
-[![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
-[![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
-[![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
-
-# serialzy
-
-Serialzy is a library for python objects serialization into portable and interoperable data formats (if possible).
-
-### Example
-
-Suppose you have a catboost model:
-
-```python
-from catboost import CatBoostClassifier
-
-model = CatBoostClassifier()
-model.fit(...)
-```
-
-Firstly you should find a proper serializer for the catboost model type or the corresponding data format:
-
-```python
-from serialzy.registry import DefaultSerializerRegistry
-
-registry = DefaultSerializerRegistry()
-serializer = registry.find_serializer_by_type(type(model)) # registry.find_serializer_by_data_format("cbm")
-```
-
-Serializers have several properties:
-
-```python
-serializer.available()      # can be used in the current environment
-serializer.requirements()   # libraries needed to be installed to use this serializer
-serializer.stable()         # has portable data format
-```
-
-Serializers can provide data format and schema for a type:
-
-```python
-serializer.data_format()
-serializer.schema(type(model))
-```
-
-Serialization:
-
-```python
-with open('model.cbm', 'wb') as file:
-    serializer.serialize(model, file)
-```
-
-Deserialization:
-
-```python
-with open('result', 'rb') as file:
-    deserialized_obj = serializer.deserialize(file)
-```
-
-### List of supported libraries for stable serialization:
-
-| Library                                     | Types                                                                                                                                                                                                                                                                                                                | Data format                                                                                                   | 
-|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
-| Python std lib                              | int, str, float, bool, None                                                                                                                                                                                                                                                                                          | [string representation](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/primitive.py)                                                                                     |
-| Python std lib                              | List, Tuple                                                                                                                                                                                                                                                                                                          | [custom format](https://github.com/lambdazy/serialzy/blob/main/serialzy/serializers/sequence.py)              |
-| [CatBoost](https://catboost.ai)             | [CatBoostRegressor](https://catboost.ai/en/docs/concepts/python-reference_catboostregressor), [CatBoostClassifier](https://catboost.ai/en/docs/concepts/python-reference_catboostclassifier), [CatBoostRanker](https://catboost.ai/en/docs/concepts/python-reference_catboostranker)                                 | [cbm](https://catboost.ai/en/docs/concepts/python-reference_catboost_save_model)                              |
-| [CatBoost](https://catboost.ai)             | [Pool](https://catboost.ai/en/docs/concepts/python-reference_pool)                                                                                                                                                                                                                                                   | [quantized pool](https://catboost.ai/en/docs/concepts/python-reference_pool_save)                             |
-| [Tensorflow.Keras](https://keras.io)        | [Sequential](https://keras.io/guides/sequential_model/), [Model](https://keras.io/api/models/model/) with subclasses                                                                                                                                                                                                 | [tf_keras](https://keras.io/api/models/model_saving_apis/)                                                    |
-| [Tensorflow](https://www.tensorflow.org)    | [Checkpoint](https://www.tensorflow.org/api_docs/python/tf/train/Checkpoint), [Module](https://www.tensorflow.org/api_docs/python/tf/Module) with subclasses                                                                                                                                                         | [tf_pure](https://www.tensorflow.org/api_docs/python/tf/saved_model)                                          |
-| [LightGBM](https://lightgbm.readthedocs.io) | [LGBMClassifier](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMClassifier.html), [LGBMRegressor](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRegressor.html), [LGBMRanker](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.LGBMRanker.html)                     | [lgbm](https://lightgbm.readthedocs.io/en/v3.3.2/pythonapi/lightgbm.Booster.html#lightgbm.Booster.save_model) |
-| [XGBoost](https://lightgbm.readthedocs.io)  | [XGBClassifier](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRegressor](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn), [XGBRanker](https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn) | [xgb](https://xgboost.readthedocs.io/en/latest/python/python_intro.html#training)                             |
-| [Torch](https://pytorch.org)                | [Module](https://pytorch.org/docs/stable/notes/modules.html) with subclasses                                                                                                                                                                                                                                         | [pt](https://pytorch.org/docs/stable/generated/torch.jit.save.html#torch.jit.save)                            |
```

### Comparing `serialzy-1.1.0/setup.py` & `serialzy-1.1.1/setup.py`

 * *Files identical despite different names*

