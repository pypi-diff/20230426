# Comparing `tmp/pymodconn-0.0.3.tar.gz` & `tmp/pymodconn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodconn-0.0.3.tar", last modified: Tue Apr 18 13:39:56 2023, max compression
+gzip compressed data, was "pymodconn-0.0.4.tar", last modified: Tue Apr 25 15:13:13 2023, max compression
```

## Comparing `pymodconn-0.0.3.tar` & `pymodconn-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:56.368075 pymodconn-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 13:39:37.000000 pymodconn-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-18 13:39:56.368075 pymodconn-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 13:39:37.000000 pymodconn-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:56.364075 pymodconn-0.0.3/pymodconn/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 13:39:37.000000 pymodconn-0.0.3/pymodconn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-18 13:39:37.000000 pymodconn-0.0.3/pymodconn/configs_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-04-18 13:39:37.000000 pymodconn-0.0.3/pymodconn/model_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    27521 2023-04-18 13:39:37.000000 pymodconn-0.0.3/pymodconn/model_gen_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:56.368075 pymodconn-0.0.3/pymodconn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-18 13:39:56.000000 pymodconn-0.0.3/pymodconn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 13:39:56.000000 pymodconn-0.0.3/pymodconn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:39:56.000000 pymodconn-0.0.3/pymodconn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 13:39:56.000000 pymodconn-0.0.3/pymodconn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 13:39:37.000000 pymodconn-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-18 13:39:56.368075 pymodconn-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 13:39:37.000000 pymodconn-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:56.368075 pymodconn-0.0.3/tests_usage/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-18 13:39:37.000000 pymodconn-0.0.3/tests_usage/RUN_MODELONLY.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:37.000000 pymodconn-0.0.3/tests_usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 15:12:59.000000 pymodconn-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-25 15:13:13.167431 pymodconn-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-25 15:12:59.000000 pymodconn-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/pymodconn/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/configs_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/major_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/model_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/model_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pymodconn/utils_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:13:13.167431 pymodconn-0.0.4/pymodconn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 15:13:13.000000 pymodconn-0.0.4/pymodconn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 15:12:59.000000 pymodconn-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 15:13:13.167431 pymodconn-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 15:12:59.000000 pymodconn-0.0.4/setup.py
```

### Comparing `pymodconn-0.0.3/LICENSE` & `pymodconn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodconn-0.0.3/PKG-INFO` & `pymodconn-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pymodconn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
 Home-page: https://github.com/gaurav306/pymodconn
 Author: Gaurav Chaudhary
 Author-email: gaurav.chaudhary@ntnu.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymodconn
 
 pymodconn = A Python library for developing modular sequence to sequence control oriented neural networks
```

### Comparing `pymodconn-0.0.3/README.md` & `pymodconn-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pymodconn-0.0.3/pymodconn/configs_init.py` & `pymodconn-0.0.4/pymodconn/configs_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 	# Write to the yaml file
 	if mode == 'w':
 		with open(filename, 'w') as yamlfile:
 			yaml.dump(data_yaml, yamlfile)
 
 
 def assert_check_configs(configs):
-	assert configs['model']['optimizer'] == 'Adam' or configs['model']['optimizer'] == 'SGD', 'Adam must be either Adam or SGD'
-	assert configs['model']['model_type_prob'] == 'prob' or configs['model'][
+	assert configs['optimizer'] == 'Adam' or configs['optimizer'] == 'SGD', 'Adam must be either Adam or SGD'
+	assert configs['model_type_prob'] == 'prob' or configs[
 		'model_type_prob'] == 'nonprob', 'model_type_prob must be either prob or nonprob'
-	assert configs['model']['loss_prob'] == 'nonparametric' or configs['model'][
+	assert configs['loss_prob'] == 'nonparametric' or configs[
 		'loss_prob'] == 'parametric', 'loss_prob must be either nonparametric or parametric'
-	assert configs['model']['control_future_cells'] == 1 or configs['model']['control_future_cells'] == 6, 'control_future_cells must be either 1 or 6'
-	assert configs['model']['all_layers_neurons'] % 8 == 0 and configs['model'][
+	#assert configs['control_future_cells'] == 1 or configs['control_future_cells'] == 6, 'control_future_cells must be either 1 or 6'
+	assert configs['all_layers_neurons'] % 8 == 0 and configs[
 		'all_layers_neurons'] >= 8, 'all_layers_neurons must be divisible by 8 and greater than or equal to 8'
-	assert configs['model']['mha_head'] % 8 == 0 and configs['model'][
+	assert configs['mha_head'] % 8 == 0 and configs[
 		'mha_head'] >= 8, 'mha_head must be divisible by 8 and greater than or equal to 8'
-	assert configs['rnn_units']['rnn_type'] in ['LSTM', 'GRU', 'RNN'], 'rnn_type must be either LSTM, GRU or RNN'
-	assert configs['rnn_units']['input_enc_rnn_depth'] <= 5, 'max depth of RNN units is 5'
+	assert configs['rnn_type'] in ['LSTM', 'GRU', 'RNN'], 'rnn_type must be either LSTM, GRU or RNN'
+	assert configs['input_enc_rnn_depth'] <= 5, 'max depth of RNN units is 5'
 
 
 def get_configs(config_filename):
 	configs = read_write_yaml(config_filename, 'r', None)
 	assert_check_configs(configs)
 	return configs
```

### Comparing `pymodconn-0.0.3/pymodconn.egg-info/PKG-INFO` & `pymodconn-0.0.4/pymodconn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pymodconn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Develops sequence to sequence control oriented neural networks in a highly modular way.
 Home-page: https://github.com/gaurav306/pymodconn
 Author: Gaurav Chaudhary
 Author-email: gaurav.chaudhary@ntnu.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymodconn
 
 pymodconn = A Python library for developing modular sequence to sequence control oriented neural networks
```

