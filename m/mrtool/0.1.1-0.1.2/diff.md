# Comparing `tmp/mrtool-0.1.1.tar.gz` & `tmp/mrtool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrtool-0.1.1.tar", last modified: Wed Mar 15 20:25:20 2023, max compression
+gzip compressed data, was "mrtool-0.1.2.tar", last modified: Wed Apr 26 18:55:07 2023, max compression
```

## Comparing `mrtool-0.1.1.tar` & `mrtool-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.742751 mrtool-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 20:24:27.000000 mrtool-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-15 20:25:20.742751 mrtool-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-15 20:24:27.000000 mrtool-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-15 20:24:27.000000 mrtool-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-15 20:25:20.742751 mrtool-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-15 20:24:27.000000 mrtool-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.734751 mrtool-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.738751 mrtool-0.1.1/src/mrtool/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.738751 mrtool-0.1.1/src/mrtool/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35415 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/cov_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.738751 mrtool-0.1.1/src/mrtool/cov_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/cov_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-03-15 20:24:27.000000 mrtool-0.1.1/src/mrtool/cov_selection/covfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.738751 mrtool-0.1.1/src/mrtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-15 20:25:20.000000 mrtool-0.1.1/src/mrtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-15 20:25:20.000000 mrtool-0.1.1/src/mrtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 20:25:20.000000 mrtool-0.1.1/src/mrtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 20:24:31.000000 mrtool-0.1.1/src/mrtool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-15 20:25:20.000000 mrtool-0.1.1/src/mrtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 20:25:20.000000 mrtool-0.1.1/src/mrtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:25:20.742751 mrtool-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-03-15 20:24:27.000000 mrtool-0.1.1/tests/test_covmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-03-15 20:24:27.000000 mrtool-0.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-15 20:24:27.000000 mrtool-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-26 18:54:05.000000 mrtool-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 18:55:07.990967 mrtool-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-26 18:54:05.000000 mrtool-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 18:54:05.000000 mrtool-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 18:55:07.994967 mrtool-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 18:54:05.000000 mrtool-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.986967 mrtool-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.986967 mrtool-0.1.2/src/mrtool/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35415 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/cov_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool/cov_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/cov_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-04-26 18:54:05.000000 mrtool-0.1.2/src/mrtool/cov_selection/covfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/src/mrtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:54:13.000000 mrtool-0.1.2/src/mrtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 18:55:07.000000 mrtool-0.1.2/src/mrtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:07.990967 mrtool-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_covmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-26 18:54:05.000000 mrtool-0.1.2/tests/test_utils.py
```

### Comparing `mrtool-0.1.1/LICENSE` & `mrtool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/PKG-INFO` & `mrtool-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrtool
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Featured nonlinear mixed effects model"
 Home-page: https://github.com/ihmeuw-msca/mrtool
 Author: IHME Math Sciences
 Author-email: ihme.math.sciences@gmail.com
 License: BSD 2-Clause License
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
```

### Comparing `mrtool-0.1.1/README.rst` & `mrtool-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/setup.cfg` & `mrtool-0.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mrtool
-version = 0.1.1
+version = 0.1.2
 description = "Featured nonlinear mixed effects model"
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = IHME Math Sciences
 author_email = ihme.math.sciences@gmail.com
 license = BSD 2-Clause License
 url = https://github.com/ihmeuw-msca/mrtool
@@ -13,15 +13,15 @@
 zip_safe = False
 install_requires = 
 	numpy
 	pandas
 	scipy
 	xspline
 	xarray
-	limetr==0.0.5
+	limetr==0.0.6
 include_package_data = True
 packages = find:
 package_dir = = src
 
 [options.packages.find]
 where = src
```

### Comparing `mrtool-0.1.1/src/mrtool/core/cov_model.py` & `mrtool-0.1.2/src/mrtool/core/cov_model.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool/core/data.py` & `mrtool-0.1.2/src/mrtool/core/data.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool/core/model.py` & `mrtool-0.1.2/src/mrtool/core/model.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool/core/plots.py` & `mrtool-0.1.2/src/mrtool/core/plots.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool/core/utils.py` & `mrtool-0.1.2/src/mrtool/core/utils.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool/cov_selection/covfinder.py` & `mrtool-0.1.2/src/mrtool/cov_selection/covfinder.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/src/mrtool.egg-info/PKG-INFO` & `mrtool-0.1.2/src/mrtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrtool
-Version: 0.1.1
+Version: 0.1.2
 Summary: "Featured nonlinear mixed effects model"
 Home-page: https://github.com/ihmeuw-msca/mrtool
 Author: IHME Math Sciences
 Author-email: ihme.math.sciences@gmail.com
 License: BSD 2-Clause License
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
```

### Comparing `mrtool-0.1.1/src/mrtool.egg-info/SOURCES.txt` & `mrtool-0.1.2/src/mrtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/tests/test_covmodel.py` & `mrtool-0.1.2/tests/test_covmodel.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/tests/test_data.py` & `mrtool-0.1.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mrtool-0.1.1/tests/test_utils.py` & `mrtool-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

