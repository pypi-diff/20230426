# Comparing `tmp/pyfed_macos-0.0.2.tar.gz` & `tmp/pyfed_macos-0.0.3.tar.gz`

## Comparing `pyfed_macos-0.0.2.tar` & `pyfed_macos-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/global_var.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/ml_socket.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/src/pyfed.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/LICENSE
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/.pypirc
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/src/global_var.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/src/ml_socket.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/src/pyfed.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyfed_macos-0.0.3/PKG-INFO
```

### Comparing `pyfed_macos-0.0.2/.DS_Store` & `pyfed_macos-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/src/ml_socket.py` & `pyfed_macos-0.0.3/src/ml_socket.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/src/pyfed.py` & `pyfed_macos-0.0.3/src/pyfed.py`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/.gitignore` & `pyfed_macos-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/LICENSE` & `pyfed_macos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/README.md` & `pyfed_macos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfed_macos-0.0.2/pyproject.toml` & `pyfed_macos-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyFed-macos"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Amirreza Sokhankhosh", email="amirreza.sokhankhosh@gmail.com" },
 ]
 description = "PyFed is an open-source framework for federated learning algorithms." 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyfed_macos-0.0.2/PKG-INFO` & `pyfed_macos-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFed-macos
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyFed is an open-source framework for federated learning algorithms.
 Project-URL: Homepage, https://github.com/amirrezasokhankhosh/PyFed
 Project-URL: Bug Tracker, https://github.com/amirrezasokhankhosh/PyFed/issues
 Author-email: Amirreza Sokhankhosh <amirreza.sokhankhosh@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

