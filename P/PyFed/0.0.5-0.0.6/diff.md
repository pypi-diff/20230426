# Comparing `tmp/pyfed-0.0.5.tar.gz` & `tmp/pyfed-0.0.6.tar.gz`

## Comparing `pyfed-0.0.5.tar` & `pyfed-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.5/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed-0.0.5/.pypirc
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pyfed-0.0.5/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.5/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.5/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.5/src/ml_socket.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.5/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.5/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.5/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed-0.0.5/README.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pyfed-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pyfed-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.6/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed-0.0.6/.pypirc
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pyfed-0.0.6/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.6/src/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.6/src/ml_socket.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.6/src/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed-0.0.6/README.md
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyfed-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 pyfed-0.0.6/PKG-INFO
```

### Comparing `pyfed-0.0.5/.DS_Store` & `pyfed-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/setup.py` & `pyfed-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/src/ml_socket.py` & `pyfed-0.0.6/src/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/src/pyfed.py` & `pyfed-0.0.6/src/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/.gitignore` & `pyfed-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/LICENSE` & `pyfed-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/README.md` & `pyfed-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.5/pyproject.toml` & `pyfed-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "tensorflow >= 2.12.0",
-    "numpy >= 1.24.0",
+    "tensorflow >= 2.10.0",
+    "numpy >= 1.23.0",
+    "tensorboard >= 2.10.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/amirrezasokhankhosh/PyFed"
 "Bug Tracker" = "https://github.com/amirrezasokhankhosh/PyFed/issues"
```

### Comparing `pyfed-0.0.5/PKG-INFO` & `pyfed-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PyFed
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: tensorflow>=2.12.0
+Requires-Dist: numpy>=1.23.0
+Requires-Dist: tensorboard>=2.10.0
+Requires-Dist: tensorflow>=2.10.0
 Description-Content-Type: text/markdown
 
 # PyFed
 
 PyFed is an open-source framework for federated learning algorithms. Federated Learning is a subfield of machine learning which trains a global model using one server and multiple clients which contain their separate datasets. 
 This approach helps clients with the problems of sharing their local data with a server and the risk of data leakage. PyFed is a straightforward and brief package that allows scientists to try Federated Learning for any model using any dataset. Furthermore, PyFed uses Tensorboard to demonstrate the history of training of each client per round.
```

