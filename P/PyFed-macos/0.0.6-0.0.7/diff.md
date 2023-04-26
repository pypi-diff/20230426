# Comparing `tmp/pyfed_macos-0.0.6.tar.gz` & `tmp/pyfed_macos-0.0.7.tar.gz`

## Comparing `pyfed_macos-0.0.6.tar` & `pyfed_macos-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/ml_socket.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/src/pyfed/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/src/pyfed/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/src/pyfed/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/src/pyfed/ml_socket.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/src/pyfed/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/README.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.7/PKG-INFO
```

### Comparing `pyfed_macos-0.0.6/.DS_Store` & `pyfed_macos-0.0.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/src/pyfed/ml_socket.py` & `pyfed_macos-0.0.7/src/pyfed/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/src/pyfed/pyfed.py` & `pyfed_macos-0.0.7/src/pyfed/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/.gitignore` & `pyfed_macos-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/LICENSE` & `pyfed_macos-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/README.md` & `pyfed_macos-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.6/pyproject.toml` & `pyfed_macos-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed_macos"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
+packages = ["pyfed"]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
```

### Comparing `pyfed_macos-0.0.6/PKG-INFO` & `pyfed_macos-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFed_macos
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

