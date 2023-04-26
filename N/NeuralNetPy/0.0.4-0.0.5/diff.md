# Comparing `tmp/NeuralNetPy-0.0.4.tar.gz` & `tmp/NeuralNetPy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralNetPy-0.0.4.tar", last modified: Wed Apr 26 15:15:53 2023, max compression
+gzip compressed data, was "NeuralNetPy-0.0.5.tar", last modified: Wed Apr 26 15:34:04 2023, max compression
```

## Comparing `NeuralNetPy-0.0.4.tar` & `NeuralNetPy-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       68 2023-04-26 15:14:58.000000 NeuralNetPy-0.0.4/NeuralNetPy/__init__.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/activations/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 15:09:27.000000 NeuralNetPy-0.0.4/NeuralNetPy/activations/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1611 2023-04-26 05:56:47.000000 NeuralNetPy-0.0.4/NeuralNetPy/activations/activations.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/layers/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/layers/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     7541 2023-04-26 06:53:53.000000 NeuralNetPy-0.0.4/NeuralNetPy/layers/layers.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/losses/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/losses/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      769 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/losses/losses.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/models/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:59:46.000000 NeuralNetPy-0.0.4/NeuralNetPy/models/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1927 2023-04-26 05:59:34.000000 NeuralNetPy-0.0.4/NeuralNetPy/models/models.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/optimizers/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/optimizers/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1790 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/optimizers/optimizers.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy/utils/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.4/NeuralNetPy/utils/__init__.py
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1463 2023-04-26 06:12:13.000000 NeuralNetPy-0.0.4/NeuralNetPy/utils/utils.py
-drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4732 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/PKG-INFO
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      634 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/SOURCES.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/dependency_links.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/not-zip-safe
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       32 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/requires.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       12 2023-04-26 15:15:53.000000 NeuralNetPy-0.0.4/NeuralNetPy.egg-info/top_level.txt
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4732 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/PKG-INFO
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     3887 2023-04-26 15:13:36.000000 NeuralNetPy-0.0.4/README.md
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       38 2023-04-26 15:15:53.521823 NeuralNetPy-0.0.4/setup.cfg
--rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1262 2023-04-26 15:15:34.000000 NeuralNetPy-0.0.4/setup.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       68 2023-04-26 15:14:58.000000 NeuralNetPy-0.0.5/NeuralNetPy/__init__.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/activations/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 15:09:27.000000 NeuralNetPy-0.0.5/NeuralNetPy/activations/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     2942 2023-04-26 15:32:20.000000 NeuralNetPy-0.0.5/NeuralNetPy/activations/activations.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/layers/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/layers/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     7541 2023-04-26 06:53:53.000000 NeuralNetPy-0.0.5/NeuralNetPy/layers/layers.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/losses/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       22 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/losses/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      769 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/losses/losses.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/models/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:59:46.000000 NeuralNetPy-0.0.5/NeuralNetPy/models/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1927 2023-04-26 05:59:34.000000 NeuralNetPy-0.0.5/NeuralNetPy/models/models.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/optimizers/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       26 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/optimizers/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1790 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/optimizers/optimizers.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy/utils/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       21 2023-04-26 05:44:12.000000 NeuralNetPy-0.0.5/NeuralNetPy/utils/__init__.py
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1463 2023-04-26 06:12:13.000000 NeuralNetPy-0.0.5/NeuralNetPy/utils/utils.py
+drwxrwxr-x   0 rnoc      (1000) rnoc      (1000)        0 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4732 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/PKG-INFO
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)      634 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)        1 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/not-zip-safe
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       32 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/requires.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       12 2023-04-26 15:34:04.000000 NeuralNetPy-0.0.5/NeuralNetPy.egg-info/top_level.txt
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     4732 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/PKG-INFO
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     3887 2023-04-26 15:13:36.000000 NeuralNetPy-0.0.5/README.md
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)       38 2023-04-26 15:34:04.765363 NeuralNetPy-0.0.5/setup.cfg
+-rw-rw-r--   0 rnoc      (1000) rnoc      (1000)     1262 2023-04-26 15:34:01.000000 NeuralNetPy-0.0.5/setup.py
```

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy/layers/layers.py` & `NeuralNetPy-0.0.5/NeuralNetPy/layers/layers.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy/losses/losses.py` & `NeuralNetPy-0.0.5/NeuralNetPy/losses/losses.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy/models/models.py` & `NeuralNetPy-0.0.5/NeuralNetPy/models/models.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy/optimizers/optimizers.py` & `NeuralNetPy-0.0.5/NeuralNetPy/optimizers/optimizers.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy/utils/utils.py` & `NeuralNetPy-0.0.5/NeuralNetPy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy.egg-info/PKG-INFO` & `NeuralNetPy-0.0.5/NeuralNetPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralNetPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.
 Home-page: UNKNOWN
 Author: Joel Maldonado-Ruiz
 Author-email: jmaldonadoruiz0@gmail.com
 License: GNU General Public License v3.0
 Keywords: Neural Network,Python,AI,Numpy,Deep Learning
 Platform: UNKNOWN
```

### Comparing `NeuralNetPy-0.0.4/NeuralNetPy.egg-info/SOURCES.txt` & `NeuralNetPy-0.0.5/NeuralNetPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/PKG-INFO` & `NeuralNetPy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralNetPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.
 Home-page: UNKNOWN
 Author: Joel Maldonado-Ruiz
 Author-email: jmaldonadoruiz0@gmail.com
 License: GNU General Public License v3.0
 Keywords: Neural Network,Python,AI,Numpy,Deep Learning
 Platform: UNKNOWN
```

### Comparing `NeuralNetPy-0.0.4/README.md` & `NeuralNetPy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `NeuralNetPy-0.0.4/setup.py` & `NeuralNetPy-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     filepath = os.path.join(os.path.dirname(__file__), filename)
     file = open(filepath, 'r')
     return file.read()
 
 
 setup(
     name='NeuralNetPy',
-    version='0.0.4',
+    version='0.0.5',
     author='Joel Maldonado-Ruiz',
     author_email='jmaldonadoruiz0@gmail.com',
     description='NeuralNetPy is a neural network library created using numpy that allows you to create, train, and save deep learning models.',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     license='GNU General Public License v3.0',
     keywords=['Neural Network', 'Python', 'AI', 'Numpy', 'Deep Learning'],
```

