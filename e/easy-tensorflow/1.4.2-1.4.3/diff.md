# Comparing `tmp/easy-tensorflow-1.4.2.tar.gz` & `tmp/easy-tensorflow-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-tensorflow-1.4.2.tar", last modified: Sat Oct 22 20:45:31 2022, max compression
+gzip compressed data, was "dist/easy-tensorflow-1.4.3.tar", last modified: Wed Apr 26 16:02:07 2023, max compression
```

## Comparing `easy-tensorflow-1.4.2.tar` & `easy-tensorflow-1.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7978 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7978 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easy_tensorflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easyflow/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easyflow/data/
--rwxr-xr-x   0 runner    (1001) docker     (121)      140 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1760 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/data/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6299 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/numerical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4629 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/feature_encoders/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8570 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/custom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     8166 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/feature_preprocessor_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/preprocessing/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/easyflow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/tests/test_feature_encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/easyflow/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-22 20:45:31.000000 easy-tensorflow-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-10-22 20:44:16.000000 easy-tensorflow-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1760 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/data/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/numerical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/feature_preprocessor_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/test_feature_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/setup.py
```

### Comparing `easy-tensorflow-1.4.2/CHANGELOG.md` & `easy-tensorflow-1.4.3/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## VERSION 1.4.3
+* Minor update to the classes that contained serialization errors.
+* Minor fix to one of the notebook examples
+
 ## VERSION 1.4.2
 * Added temp fix when using StringLookup layer as first layer in Keras Sequential model
   (reference: https://github.com/keras-team/keras/issues/16101)
 
 ## VERSION 1.4.1
 * Added a new landing page (README) for the project
```

### Comparing `easy-tensorflow-1.4.2/PKG-INFO` & `easy-tensorflow-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-tensorflow
-Version: 1.4.2
+Version: 1.4.3
 Summary: Feature Pipelines for Keras preprocessing layers.
 Home-page: https://github.com/fernandonieuwveldt/easyflow
 Author: Fernando Nieuwveldt
 Author-email: fdnieuwveldt@gmail.com
 License: UNKNOWN
 Description: # EasyFlow: Keras Feature Preprocessing Pipelines
```

### Comparing `easy-tensorflow-1.4.2/README.md` & `easy-tensorflow-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easy_tensorflow.egg-info/PKG-INFO` & `easy-tensorflow-1.4.3/easy_tensorflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-tensorflow
-Version: 1.4.2
+Version: 1.4.3
 Summary: Feature Pipelines for Keras preprocessing layers.
 Home-page: https://github.com/fernandonieuwveldt/easyflow
 Author: Fernando Nieuwveldt
 Author-email: fdnieuwveldt@gmail.com
 License: UNKNOWN
 Description: # EasyFlow: Keras Feature Preprocessing Pipelines
```

### Comparing `easy-tensorflow-1.4.2/easy_tensorflow.egg-info/SOURCES.txt` & `easy-tensorflow-1.4.3/easy_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/data/mapper.py` & `easy-tensorflow-1.4.3/easyflow/data/mapper.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/feature_encoders/__init__.py` & `easy-tensorflow-1.4.3/easyflow/feature_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/feature_encoders/base.py` & `easy-tensorflow-1.4.3/easyflow/feature_encoders/base.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/feature_encoders/categorical_encoders.py` & `easy-tensorflow-1.4.3/easyflow/feature_encoders/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/feature_encoders/numerical_encoders.py` & `easy-tensorflow-1.4.3/easyflow/feature_encoders/numerical_encoders.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/feature_encoders/pipeline.py` & `easy-tensorflow-1.4.3/easyflow/feature_encoders/pipeline.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/__init__.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/base.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/custom.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,19 @@
     def get_config(self):
         """Update config with layers_to_adapt attr
 
         Returns:
             dict: Updated config
         """
         config = super().get_config()
-        config.update(
-            {"layers_to_adapt": self.layers_to_adapt, "pipeline": self.pipeline}
-        )
+        config.update({
+            "layers_to_adapt": self.layers_to_adapt,
+            "adapted_layers": self.adapted_layers,
+            "pipeline": self.pipeline
+        })
         return config
 
 
 class PreprocessorChain(tf.keras.models.Sequential):
     """Preprocessing model that chains one or more layers in a sequential order by subclassing
     Sequential model class. The functionality is the same as Pipeline.
     """
```

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/factory.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/factory.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/feature_preprocessor_layer.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/feature_preprocessor_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,14 @@
                 # get a fresh preprocessing instance
                 cloned_preprocessor = preprocessor if k==0 else preprocessor.from_config(config)
                 feature_ds = extract_feature_column_tensorflow(dataset, feature)
                 # check if layer has adapt method
                 cloned_preprocessor.adapt(feature_ds, *args, **kwargs)
                 self.adapted_preprocessors[feature] = cloned_preprocessor
 
-    # what if inputs is not of type dict?
-    @tf.function
     def call(self, inputs):
         """Apply adapted layers on new data.
 
         Args:
             inputs (dict): Dictionary of Tensors.
 
         Returns:
@@ -91,14 +89,27 @@
             ),
             (
                 "string_categorical_features", StringToIntegerLookup(), string_categoric_features,
             ),
         ]
         return feature_preprocessor_list
 
+    def get_config(self):
+        """Update config with layers_to_adapt attr
+
+        Returns:
+            dict: Updated config
+        """
+        config = super().get_config()
+        config.update({
+            "feature_preprocessor_list": self.feature_preprocessor_list,
+            "adapted_preprocessors": self.adapted_preprocessors
+        })
+        return config
+
 
 class FeaturePreprocessorFromPandasDataFrame(tf.keras.layers.Layer, BaseFeaturePreprocessor):
     """Feature Preprocessing Layer for pandas DataFrame type. The class takes in steps of preprocessing that
     needs to be applied on the dataset. The adapt method records all stateful parameters for each of the steps
     and features that will be adapted. These adapted layers will be stored as an attribute and applied in the
     forward pass of the network.
 
@@ -125,15 +136,14 @@
                 # get a fresh preprocessing instance
                 cloned_preprocessor = preprocessor if k==0 else preprocessor.from_config(config)
                 feature_ds = extract_feature_column_pandas(dataset, feature)
                 # check if layer has adapt method
                 cloned_preprocessor.adapt(feature_ds, *args, **kwargs)
                 self.adapted_preprocessors[feature] = cloned_preprocessor
 
-    @tf.function
     def call(self, inputs):
         """Apply adapted layers on new data
 
         Args:
             inputs (dict): Dictionary of Tensors.
 
         Returns:
@@ -179,14 +189,27 @@
             ),
             (
                 "string_categorical_features", StringToIntegerLookup(), string_categoric_features,
             ),
         ]
         return feature_preprocessor_list
 
+    def get_config(self):
+        """Update config with layers_to_adapt attr
+
+        Returns:
+            dict: Updated config
+        """
+        config = super().get_config()
+        config.update({
+            "feature_preprocessor_list": self.feature_preprocessor_list,
+            "adapted_preprocessors": self.adapted_preprocessors
+        })
+        return config
+
 
 def extract_feature_column_tensorflow(dataset, name):
     """Extract feature from dataset
 
     Args:
         dataset (tf.data.Dataset): Training Data
         name (str): Name of feature to extract
```

### Comparing `easy-tensorflow-1.4.2/easyflow/preprocessing/pipeline.py` & `easy-tensorflow-1.4.3/easyflow/preprocessing/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         preprocessed_input = super(FeaturePreprocessor, self).call(inputs)
         # Should this concatenation happen in feature_preprocessor_layer call methods?
         preprocessed_input = {
             step_name: tf.keras.layers.concatenate(step_layers)
             for step_name, step_layers in preprocessed_input.items()
         }
         return Bunch(**preprocessed_input)
+    
+    def get_config(self):
+        """Override get_config to ensure saving of models works"""
+        return super().get_config().copy()
 
 
 class FeatureUnion(FeaturePreprocessorFactory):
     """Apply column based preprocessing on the data and combine features with a concat layer.
 
     Args:
         feature_encoder_list : List of encoders of the form: ('name', encoder type, list of features)
@@ -61,14 +65,18 @@
             for _, high_level in preprocessed_input.items()
             for low_level in high_level
         ]
         if len(preprocessed_input) > 1:
             return tf.keras.layers.concatenate(preprocessed_input)
         return preprocessed_input.pop()
 
+    def get_config(self):
+        """Override get_config to ensure saving of models works"""
+        return super().get_config().copy()
+
 
 class Bunch(dict):
     """Helper class that bunch set of layer steps into one and can easily be 
     accessed as preprocessor.step_name
 
     Reference: https://github.com/scikit-learn/scikit-learn/sklearn/utils/_bunch.py
     """
```

### Comparing `easy-tensorflow-1.4.2/easyflow/tests/test_feature_encoders.py` & `easy-tensorflow-1.4.3/easyflow/tests/test_feature_encoders.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/easyflow/tests/test_preprocessing.py` & `easy-tensorflow-1.4.3/easyflow/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.2/setup.py` & `easy-tensorflow-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text(encoding='utf-8')
 REQUIREMENTS = (pathlib.Path(__file__).parent / "requirements.txt").read_text().splitlines()[1:]
 REQUIRES_PYTHON = '>=3.7.0'
 
 
 setup(
     name="easy-tensorflow",
-    version="1.4.2",
+    version="1.4.3",
     author="Fernando Nieuwveldt",
     author_email="fdnieuwveldt@gmail.com",
     description="Feature Pipelines for Keras preprocessing layers.",
     long_description_content_type='text/markdown',
     long_description=README,
     url="https://github.com/fernandonieuwveldt/easyflow",
     python_requires=REQUIRES_PYTHON,
```

