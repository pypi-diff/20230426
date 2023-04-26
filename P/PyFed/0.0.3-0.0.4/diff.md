# Comparing `tmp/pyfed-0.0.3.tar.gz` & `tmp/pyfed-0.0.4.tar.gz`

## Comparing `pyfed-0.0.3.tar` & `pyfed-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.3/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/ml_socket.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.3/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.3/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed-0.0.3/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfed-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 pyfed-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed-0.0.4/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed-0.0.4/.pypirc
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pyfed-0.0.4/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed-0.0.4/src/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed-0.0.4/src/ml_socket.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed-0.0.4/src/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed-0.0.4/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pyfed-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 pyfed-0.0.4/PKG-INFO
```

### Comparing `pyfed-0.0.3/.DS_Store` & `pyfed-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/src/ml_socket.py` & `pyfed-0.0.4/src/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/src/pyfed.py` & `pyfed-0.0.4/src/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/.gitignore` & `pyfed-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/LICENSE` & `pyfed-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/README.md` & `pyfed-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfed-0.0.3/pyproject.toml` & `pyfed-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed"
-version = "0.0.3"
+version = "0.0.4"
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
+dependencies = [
+    "tensorflow",
+    "numpy",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/amirrezasokhankhosh/PyFed"
 "Bug Tracker" = "https://github.com/amirrezasokhankhosh/PyFed/issues"
```

### Comparing `pyfed-0.0.3/PKG-INFO` & `pyfed-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: PyFed
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: numpy
+Requires-Dist: tensorflow
 Description-Content-Type: text/markdown
 
 # PyFed
 
 PyFed is an open-source framework for federated learning algorithms. Federated Learning is a subfield of machine learning which trains a global model using one server and multiple clients which contain their separate datasets. 
 This approach helps clients with the problems of sharing their local data with a server and the risk of data leakage. PyFed is a straightforward and brief package that allows scientists to try Federated Learning for any model using any dataset. Furthermore, PyFed uses Tensorboard to demonstrate the history of training of each client per round.
```

