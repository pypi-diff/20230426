# Comparing `tmp/lpynn-0.0.2.tar.gz` & `tmp/lpynn-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpynn-0.0.2.tar", last modified: Tue Apr 25 23:46:15 2023, max compression
+gzip compressed data, was "lpynn-0.0.2.1.tar", last modified: Tue Apr 25 23:49:15 2023, max compression
```

## Comparing `lpynn-0.0.2.tar` & `lpynn-0.0.2.1.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:46:15.086303 lpynn-0.0.2/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpynn-0.0.2/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     1195 2023-04-25 23:46:15.086144 lpynn-0.0.2/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      746 2023-04-21 16:22:30.000000 lpynn-0.0.2/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:46:15.084766 lpynn-0.0.2/lpynn/
--rw-r--r--   0 ubaid      (501) staff       (20)        0 2023-04-21 16:22:30.000000 lpynn-0.0.2/lpynn/__init__.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:46:15.085926 lpynn-0.0.2/lpynn/perceptron/
--rw-r--r--   0 ubaid      (501) staff       (20)      132 2023-04-21 16:22:30.000000 lpynn-0.0.2/lpynn/perceptron/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)     7587 2023-04-25 23:44:21.000000 lpynn-0.0.2/lpynn/perceptron/goto.py
--rw-r--r--   0 ubaid      (501) staff       (20)    15500 2023-04-25 23:44:21.000000 lpynn-0.0.2/lpynn/perceptron/lpython.py
--rw-r--r--   0 ubaid      (501) staff       (20)     4154 2023-04-25 23:45:00.000000 lpynn-0.0.2/lpynn/perceptron/perceptron_main.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:46:15.085356 lpynn-0.0.2/lpynn.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     1195 2023-04-25 23:46:15.000000 lpynn-0.0.2/lpynn.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      278 2023-04-25 23:46:15.000000 lpynn-0.0.2/lpynn.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-25 23:46:15.000000 lpynn-0.0.2/lpynn.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        6 2023-04-25 23:46:15.000000 lpynn-0.0.2/lpynn.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-25 23:46:15.086344 lpynn-0.0.2/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1906 2023-04-25 23:45:26.000000 lpynn-0.0.2/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.507017 lpynn-0.0.2.1/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-04-25 23:49:15.506910 lpynn-0.0.2.1/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      746 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506084 lpynn-0.0.2.1/lpynn/
+-rw-r--r--   0 ubaid      (501) staff       (20)        0 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/lpynn/__init__.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506753 lpynn-0.0.2.1/lpynn/perceptron/
+-rw-r--r--   0 ubaid      (501) staff       (20)      132 2023-04-21 16:22:30.000000 lpynn-0.0.2.1/lpynn/perceptron/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)     4153 2023-04-25 23:48:43.000000 lpynn-0.0.2.1/lpynn/perceptron/perceptron_main.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-25 23:49:15.506525 lpynn-0.0.2.1/lpynn.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1197 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      225 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        6 2023-04-25 23:49:15.000000 lpynn-0.0.2.1/lpynn.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-25 23:49:15.507049 lpynn-0.0.2.1/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1908 2023-04-25 23:48:34.000000 lpynn-0.0.2.1/setup.py
```

### Comparing `lpynn-0.0.2/LICENSE` & `lpynn-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lpynn-0.0.2/PKG-INFO` & `lpynn-0.0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpynn
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A basic neural networks python package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpynn-0.0.2/README.md` & `lpynn-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lpynn-0.0.2/lpynn/perceptron/perceptron_main.py` & `lpynn-0.0.2.1/lpynn/perceptron/perceptron_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .lpython import dataclass, i32, f64
+from lpython import dataclass, i32, f64
 
 @dataclass
 class Perceptron:
     no_of_inputs: i32
     weights: list[f64]
     learn_rate: f64
     iterations_limit: i32
```

### Comparing `lpynn-0.0.2/lpynn.egg-info/PKG-INFO` & `lpynn-0.0.2.1/lpynn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpynn
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A basic neural networks python package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lpynn-0.0.2/setup.py` & `lpynn-0.0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
 REQUIRED_PACKAGES=[]
 
-VERSION="0.0.2"
+VERSION="0.0.2.1"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpynn",                                               # name of project
```

