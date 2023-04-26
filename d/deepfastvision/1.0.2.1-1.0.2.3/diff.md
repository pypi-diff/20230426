# Comparing `tmp/deepfastvision-1.0.2.1.tar.gz` & `tmp/deepfastvision-1.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfastvision-1.0.2.1.tar", last modified: Wed Apr 26 10:45:34 2023, max compression
+gzip compressed data, was "deepfastvision-1.0.2.3.tar", last modified: Wed Apr 26 11:33:27 2023, max compression
```

## Comparing `deepfastvision-1.0.2.1.tar` & `deepfastvision-1.0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:34.044304 deepfastvision-1.0.2.1/
--rw-rw-rw-   0        0        0     1068 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/LICENSE
--rw-rw-rw-   0        0        0      783 2023-04-26 10:45:34.040305 deepfastvision-1.0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:33.914596 deepfastvision-1.0.2.1/deepfastvision/
--rw-rw-rw-   0        0        0       66 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:33.958570 deepfastvision-1.0.2.1/deepfastvision/core/
--rw-rw-rw-   0        0        0    46998 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/core/DeepTransferClassification.py
--rw-rw-rw-   0        0        0       46 2023-04-26 10:41:05.000000 deepfastvision-1.0.2.1/deepfastvision/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:33.969564 deepfastvision-1.0.2.1/deepfastvision/data_management/
--rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/data_management/__init__.py
--rw-rw-rw-   0        0        0     8201 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/data_management/data_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:33.998331 deepfastvision-1.0.2.1/deepfastvision/model_components/
--rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:34.009326 deepfastvision-1.0.2.1/deepfastvision/model_components/callbacks/
--rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/callbacks/__init__.py
--rw-rw-rw-   0        0        0     2968 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/callbacks/custom_save_weights.py
--rw-rw-rw-   0        0        0     4001 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/export_helpers.py
--rw-rw-rw-   0        0        0     5408 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/model_creation.py
--rw-rw-rw-   0        0        0     5622 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/prediction_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:34.020318 deepfastvision-1.0.2.1/deepfastvision/model_components/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     3232 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/model_components/preprocessing/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:34.032308 deepfastvision-1.0.2.1/deepfastvision/plotting/
--rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/plotting/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.1/deepfastvision/plotting/plot_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:45:33.944576 deepfastvision-1.0.2.1/deepfastvision.egg-info/
--rw-rw-rw-   0        0        0      783 2023-04-26 10:45:33.000000 deepfastvision-1.0.2.1/deepfastvision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-26 10:45:33.000000 deepfastvision-1.0.2.1/deepfastvision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:45:33.000000 deepfastvision-1.0.2.1/deepfastvision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-26 10:45:33.000000 deepfastvision-1.0.2.1/deepfastvision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-26 10:45:33.000000 deepfastvision-1.0.2.1/deepfastvision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:45:34.045302 deepfastvision-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-26 10:41:05.000000 deepfastvision-1.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.571442 deepfastvision-1.0.2.3/
+-rw-rw-rw-   0        0        0     1068 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      783 2023-04-26 11:33:27.567444 deepfastvision-1.0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.422131 deepfastvision-1.0.2.3/deepfastvision/
+-rw-rw-rw-   0        0        0        2 2023-04-26 11:32:44.000000 deepfastvision-1.0.2.3/deepfastvision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.475499 deepfastvision-1.0.2.3/deepfastvision/core/
+-rw-rw-rw-   0        0        0    46998 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/core/DeepTransferClassification.py
+-rw-rw-rw-   0        0        0       68 2023-04-26 11:32:44.000000 deepfastvision-1.0.2.3/deepfastvision/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.486491 deepfastvision-1.0.2.3/deepfastvision/data_management/
+-rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/data_management/__init__.py
+-rw-rw-rw-   0        0        0     8201 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/data_management/data_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.517473 deepfastvision-1.0.2.3/deepfastvision/model_components/
+-rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.531466 deepfastvision-1.0.2.3/deepfastvision/model_components/callbacks/
+-rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     2968 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/callbacks/custom_save_weights.py
+-rw-rw-rw-   0        0        0     4001 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/export_helpers.py
+-rw-rw-rw-   0        0        0     5408 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/model_creation.py
+-rw-rw-rw-   0        0        0     5622 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/prediction_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.542460 deepfastvision-1.0.2.3/deepfastvision/model_components/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3232 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/model_components/preprocessing/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.556451 deepfastvision-1.0.2.3/deepfastvision/plotting/
+-rw-rw-rw-   0        0        0        0 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/plotting/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-04-25 13:26:49.000000 deepfastvision-1.0.2.3/deepfastvision/plotting/plot_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:33:27.454509 deepfastvision-1.0.2.3/deepfastvision.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-04-26 11:33:27.000000 deepfastvision-1.0.2.3/deepfastvision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-26 11:33:27.000000 deepfastvision-1.0.2.3/deepfastvision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 11:33:27.000000 deepfastvision-1.0.2.3/deepfastvision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-26 11:33:27.000000 deepfastvision-1.0.2.3/deepfastvision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-26 11:33:27.000000 deepfastvision-1.0.2.3/deepfastvision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 11:33:27.571442 deepfastvision-1.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-26 11:32:44.000000 deepfastvision-1.0.2.3/setup.py
```

### Comparing `deepfastvision-1.0.2.1/LICENSE` & `deepfastvision-1.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/PKG-INFO` & `deepfastvision-1.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfastvision
-Version: 1.0.2.1
+Version: 1.0.2.3
 Summary: A Python library for rapid prototyping of deep transfer learning vision models
 Home-page: https://github.com/fabprezja/deep-fast-vision
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `deepfastvision-1.0.2.1/deepfastvision/core/DeepTransferClassification.py` & `deepfastvision-1.0.2.3/deepfastvision/core/DeepTransferClassification.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/data_management/data_helpers.py` & `deepfastvision-1.0.2.3/deepfastvision/data_management/data_helpers.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/model_components/callbacks/custom_save_weights.py` & `deepfastvision-1.0.2.3/deepfastvision/model_components/callbacks/custom_save_weights.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/model_components/export_helpers.py` & `deepfastvision-1.0.2.3/deepfastvision/model_components/export_helpers.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/model_components/model_creation.py` & `deepfastvision-1.0.2.3/deepfastvision/model_components/model_creation.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/model_components/prediction_helpers.py` & `deepfastvision-1.0.2.3/deepfastvision/model_components/prediction_helpers.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/model_components/preprocessing/preprocessing.py` & `deepfastvision-1.0.2.3/deepfastvision/model_components/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision/plotting/plot_helpers.py` & `deepfastvision-1.0.2.3/deepfastvision/plotting/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/deepfastvision.egg-info/PKG-INFO` & `deepfastvision-1.0.2.3/deepfastvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfastvision
-Version: 1.0.2.1
+Version: 1.0.2.3
 Summary: A Python library for rapid prototyping of deep transfer learning vision models
 Home-page: https://github.com/fabprezja/deep-fast-vision
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `deepfastvision-1.0.2.1/deepfastvision.egg-info/SOURCES.txt` & `deepfastvision-1.0.2.3/deepfastvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepfastvision-1.0.2.1/setup.py` & `deepfastvision-1.0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deepfastvision",
-    version="1.0.2.1",
+    version="1.0.2.3",
     description="A Python library for rapid prototyping of deep transfer learning vision models",
     author="Fabi Prezja",
     author_email="faprezja@fairn.fi",
     url="https://github.com/fabprezja/deep-fast-vision",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

