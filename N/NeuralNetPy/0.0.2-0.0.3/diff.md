# Comparing `tmp/NeuralNetPy-0.0.2.tar.gz` & `tmp/NeuralNetPy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralNetPy-0.0.2.tar", last modified: Wed Apr 26 07:23:34 2023, max compression
+gzip compressed data, was "NeuralNetPy-0.0.3.tar", last modified: Wed Apr 26 07:25:00 2023, max compression
```

## Comparing `NeuralNetPy-0.0.2.tar` & `NeuralNetPy-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       91 2023-04-26 07:20:05.000000 NeuralNetPy-0.0.2/NeuralNetPy/__init__.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/activations/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 07:20:08.000000 NeuralNetPy-0.0.2/NeuralNetPy/activations/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1611 2023-04-26 05:56:47.000000 NeuralNetPy-0.0.2/NeuralNetPy/activations/activations.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/layers/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/layers/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     7541 2023-04-26 06:53:53.000000 NeuralNetPy-0.0.2/NeuralNetPy/layers/layers.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/losses/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/losses/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      769 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/losses/losses.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/models/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:59:46.000000 NeuralNetPy-0.0.2/NeuralNetPy/models/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1927 2023-04-26 05:59:34.000000 NeuralNetPy-0.0.2/NeuralNetPy/models/models.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/optimizers/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/optimizers/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1790 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/optimizers/optimizers.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy/utils/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.2/NeuralNetPy/utils/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1463 2023-04-26 06:12:13.000000 NeuralNetPy-0.0.2/NeuralNetPy/utils/utils.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4903 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/PKG-INFO
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      634 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/SOURCES.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/dependency_links.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/not-zip-safe
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       32 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/requires.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       12 2023-04-26 07:23:34.000000 NeuralNetPy-0.0.2/NeuralNetPy.egg-info/top_level.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4903 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/PKG-INFO
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     3798 2023-04-26 06:52:08.000000 NeuralNetPy-0.0.2/README.md
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       38 2023-04-26 07:23:34.615805 NeuralNetPy-0.0.2/setup.cfg
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1522 2023-04-26 07:23:01.000000 NeuralNetPy-0.0.2/setup.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.756709 NeuralNetPy-0.0.3/NeuralNetPy/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       91 2023-04-26 07:20:05.000000 NeuralNetPy-0.0.3/NeuralNetPy/__init__.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/activations/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 07:20:08.000000 NeuralNetPy-0.0.3/NeuralNetPy/activations/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1611 2023-04-26 05:56:47.000000 NeuralNetPy-0.0.3/NeuralNetPy/activations/activations.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/layers/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/layers/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     7541 2023-04-26 06:53:53.000000 NeuralNetPy-0.0.3/NeuralNetPy/layers/layers.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/losses/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/losses/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      769 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/losses/losses.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/models/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:59:46.000000 NeuralNetPy-0.0.3/NeuralNetPy/models/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1927 2023-04-26 05:59:34.000000 NeuralNetPy-0.0.3/NeuralNetPy/models/models.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/optimizers/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/optimizers/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1790 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/optimizers/optimizers.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy/utils/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.3/NeuralNetPy/utils/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1463 2023-04-26 06:12:13.000000 NeuralNetPy-0.0.3/NeuralNetPy/utils/utils.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4643 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/PKG-INFO
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      634 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/not-zip-safe
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       32 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/requires.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       12 2023-04-26 07:25:00.000000 NeuralNetPy-0.0.3/NeuralNetPy.egg-info/top_level.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4643 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/PKG-INFO
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     3798 2023-04-26 06:52:08.000000 NeuralNetPy-0.0.3/README.md
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       38 2023-04-26 07:25:00.760709 NeuralNetPy-0.0.3/setup.cfg
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1262 2023-04-26 07:24:46.000000 NeuralNetPy-0.0.3/setup.py
```

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/activations/activations.py` & `NeuralNetPy-0.0.3/NeuralNetPy/activations/activations.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/layers/layers.py` & `NeuralNetPy-0.0.3/NeuralNetPy/layers/layers.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/losses/losses.py` & `NeuralNetPy-0.0.3/NeuralNetPy/losses/losses.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/models/models.py` & `NeuralNetPy-0.0.3/NeuralNetPy/models/models.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/optimizers/optimizers.py` & `NeuralNetPy-0.0.3/NeuralNetPy/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy/utils/utils.py` & `NeuralNetPy-0.0.3/NeuralNetPy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy.egg-info/PKG-INFO` & `NeuralNetPy-0.0.3/NeuralNetPy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NeuralNetPy
-Version: 0.0.2
-Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models. It includes common layers, activations, losses, and optimizers, making it easy to build a variety of models for different tasks. It also includes helpful utility functions for data preprocessing, training and testing the models, and saving and loading models.
+Version: 0.0.3
+Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.
 Home-page: UNKNOWN
 Author: Joel Maldonado-Ruiz
 Author-email: jmaldonadoruiz0@gmail.com
 License: GNU General Public License v3.0
 Keywords: Neural Network,Python,AI,Numpy,Deep Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `NeuralNetPy-0.0.2/NeuralNetPy.egg-info/SOURCES.txt` & `NeuralNetPy-0.0.3/NeuralNetPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/PKG-INFO` & `NeuralNetPy-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NeuralNetPy
-Version: 0.0.2
-Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models. It includes common layers, activations, losses, and optimizers, making it easy to build a variety of models for different tasks. It also includes helpful utility functions for data preprocessing, training and testing the models, and saving and loading models.
+Version: 0.0.3
+Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.
 Home-page: UNKNOWN
 Author: Joel Maldonado-Ruiz
 Author-email: jmaldonadoruiz0@gmail.com
 License: GNU General Public License v3.0
 Keywords: Neural Network,Python,AI,Numpy,Deep Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `NeuralNetPy-0.0.2/README.md` & `NeuralNetPy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.2/setup.py` & `NeuralNetPy-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     filepath = os.path.join(os.path.dirname(__file__), filename)
     file = open(filepath, 'r')
     return file.read()
 
 
 setup(
     name='NeuralNetPy',
-    version='0.0.2',
+    version='0.0.3',
     author='Joel Maldonado-Ruiz',
     author_email='jmaldonadoruiz0@gmail.com',
-    description='NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models. It includes common layers, activations, losses, and optimizers, making it easy to build a variety of models for different tasks. It also includes helpful utility functions for data preprocessing, training and testing the models, and saving and loading models.',
+    description='NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     license='GNU General Public License v3.0',
     keywords=['Neural Network', 'Python', 'AI', 'Numpy', 'Deep Learning'],
     packages=find_packages(),
     install_requires=['numpy >= 1.23.5', 'matplotlib >= 3.6.3'],
     include_package_data=True,
```

