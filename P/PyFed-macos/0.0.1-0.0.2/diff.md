# Comparing `tmp/pyfed_macos-0.0.1.tar.gz` & `tmp/pyfed_macos-0.0.2.tar.gz`

## Comparing `pyfed_macos-0.0.1.tar` & `pyfed_macos-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/src/ml_socket.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 pyfed_macos-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/ml_socket.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/PKG-INFO
```

### Comparing `pyfed_macos-0.0.1/.DS_Store` & `pyfed_macos-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/src/ml_socket.py` & `pyfed_macos-0.0.2/src/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/src/pyfed.py` & `pyfed_macos-0.0.2/src/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/.gitignore` & `pyfed_macos-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/LICENSE` & `pyfed_macos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/README.md` & `pyfed_macos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.1/pyproject.toml` & `pyfed_macos-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed-macos"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
 ]
 dependencies = [
     "tensorflow-macos >= 2.10.0",
     "numpy >= 1.23.0",
-    "tensorboard >= 2.10.0"
+    "tensorboard >= 2.10.0",
+    "h5py >= 3.6.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/amirrezasokhankhosh/PyFed"
 "Bug Tracker" = "https://github.com/amirrezasokhankhosh/PyFed/issues"
```

### Comparing `pyfed_macos-0.0.1/PKG-INFO` & `pyfed_macos-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: PyFed-macos
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: h5py>=3.6.0
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: tensorboard>=2.10.0
 Requires-Dist: tensorflow-macos>=2.10.0
 Description-Content-Type: text/markdown
 
 # PyFed
```

