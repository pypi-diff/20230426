# Comparing `tmp/speechtotext-python-0.3.7.tar.gz` & `tmp/speechtotext-python-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.7.tar", last modified: Tue Apr 25 07:26:48 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.8.tar", last modified: Wed Apr 26 12:31:12 2023, max compression
```

## Comparing `speechtotext-python-0.3.7.tar` & `speechtotext-python-0.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4099 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.590268 speechtotext-python-0.3.7/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6847 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.590268 speechtotext-python-0.3.7/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.595373 speechtotext-python-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 12:31:12.595373 speechtotext-python-0.3.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4111 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6847 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 12:31:12.000000 speechtotext-python-0.3.8/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 12:31:12.591373 speechtotext-python-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 12:29:51.000000 speechtotext-python-0.3.8/tests/test_metrics.py
```

### Comparing `speechtotext-python-0.3.7/LICENSE` & `speechtotext-python-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/PKG-INFO` & `speechtotext-python-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.7/setup.py` & `speechtotext-python-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	'deepgram-sdk', 'azure-cognitiveservices-speech', 
 	'speechmatics-python==1.6.4', 'pydub', 'docstring_parser'
 ]
 
 # What packages are optional?
 EXTRAS = {
 	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
-			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine']
+			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'graphviz']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

### Comparing `speechtotext-python-0.3.7/speechtotext/datasets.py` & `speechtotext-python-0.3.8/speechtotext/datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/speechtotext/functions.py` & `speechtotext-python-0.3.8/speechtotext/functions.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/speechtotext_python.egg-info/PKG-INFO` & `speechtotext-python-0.3.8/speechtotext_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.7/tests/test_datasets.py` & `speechtotext-python-0.3.8/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/tests/test_functions.py` & `speechtotext-python-0.3.8/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/tests/test_imports.py` & `speechtotext-python-0.3.8/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.7/tests/test_metrics.py` & `speechtotext-python-0.3.8/tests/test_metrics.py`

 * *Files identical despite different names*

