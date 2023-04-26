# Comparing `tmp/pychaterr-0.0.1.tar.gz` & `tmp/pychaterr-0.1.0.tar.gz`

## Comparing `pychaterr-0.0.1.tar` & `pychaterr-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pychaterr-0.0.1/pychaterr/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pychaterr-0.0.1/pychaterr/chaterr.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pychaterr-0.0.1/.gitignore
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pychaterr-0.0.1/.hgignore -> /home/omab/.dotfiles/.hgignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pychaterr-0.0.1/LICENSE
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pychaterr-0.0.1/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pychaterr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pychaterr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pychaterr-0.1.0/pychaterr/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pychaterr-0.1.0/pychaterr/chaterr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pychaterr-0.1.0/.gitignore
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pychaterr-0.1.0/.hgignore -> /home/omab/.dotfiles/.hgignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 pychaterr-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pychaterr-0.1.0/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pychaterr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pychaterr-0.1.0/PKG-INFO
```

### Comparing `pychaterr-0.0.1/pychaterr/chaterr.py` & `pychaterr-0.1.0/pychaterr/chaterr.py`

 * *Files identical despite different names*

### Comparing `pychaterr-0.0.1/LICENSE` & `pychaterr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pychaterr-0.0.1/README.md` & `pychaterr-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 
 Then import the module in your code with:
 
 ```python
 import pychaterr
 ```
 
+# Demo
+
+[![asciicast](https://asciinema.org/a/as6OC8KH0Oe6w78Yw10TexmsV.svg)](https://asciinema.org/a/as6OC8KH0Oe6w78Yw10TexmsV)
+
 # Examples
 
 The [examples/](examples/) folder contains examples showing this module behavior.
 
 Run the samples with:
 
 ```shell
```

### Comparing `pychaterr-0.0.1/pyproject.toml` & `pychaterr-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyChatErr"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Matías Aguirre", email="matiasaguirre@gmail.com" },
 ]
 description = "Python generic error handler powered by ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pychaterr-0.0.1/PKG-INFO` & `pychaterr-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyChatErr
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python generic error handler powered by ChatGPT
 Project-URL: Homepage, https://github.com/omab/pychaterr
 Project-URL: Bug Tracker, https://github.com/omab/pychaterr/issues
 Author-email: Matías Aguirre <matiasaguirre@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -43,14 +43,18 @@
 
 Then import the module in your code with:
 
 ```python
 import pychaterr
 ```
 
+# Demo
+
+[![asciicast](https://asciinema.org/a/as6OC8KH0Oe6w78Yw10TexmsV.svg)](https://asciinema.org/a/as6OC8KH0Oe6w78Yw10TexmsV)
+
 # Examples
 
 The [examples/](examples/) folder contains examples showing this module behavior.
 
 Run the samples with:
 
 ```shell
```

