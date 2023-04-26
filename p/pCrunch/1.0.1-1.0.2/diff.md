# Comparing `tmp/pCrunch-1.0.1.tar.gz` & `tmp/pCrunch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pCrunch-1.0.1.tar", last modified: Sat Apr 22 19:20:11 2023, max compression
+gzip compressed data, was "pCrunch-1.0.2.tar", last modified: Tue Apr 25 18:36:44 2023, max compression
```

## Comparing `pCrunch-1.0.1.tar` & `pCrunch-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.746086 pCrunch-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-22 19:20:01.000000 pCrunch-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 19:20:01.000000 pCrunch-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 19:20:11.746086 pCrunch-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-22 19:20:01.000000 pCrunch-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/io/openfast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pCrunch/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/pCrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 19:20:11.000000 pCrunch-1.0.1/pCrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-04-22 19:20:01.000000 pCrunch-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:20:11.746086 pCrunch-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-22 19:20:01.000000 pCrunch-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.734086 pCrunch-1.0.1/tests/io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:20:11.746086 pCrunch-1.0.1/tests/io/data/
--rw-r--r--   0 runner    (1001) docker     (123)   186142 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/AOC_WSt.out
--rw-r--r--   0 runner    (1001) docker     (123)   130830 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/AOC_WSt.outb
--rw-r--r--   0 runner    (1001) docker     (123)  1477853 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_1.out
--rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_2.out
--rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/DLC2.3_3.out
--rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test1.outb
--rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test2.outb
--rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/Test3.outb
--rw-r--r--   0 runner    (1001) docker     (123)  1204577 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/data/step_0.outb
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/test_direct_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 19:20:01.000000 pCrunch-1.0.1/tests/io/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.975500 pCrunch-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-25 18:36:36.000000 pCrunch-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 18:36:36.000000 pCrunch-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-25 18:36:44.975500 pCrunch-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 18:36:36.000000 pCrunch-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.963500 pCrunch-1.0.2/pCrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pCrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pCrunch/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.963500 pCrunch-1.0.2/pCrunch/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pCrunch/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pCrunch/io/openfast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pCrunch/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.963500 pCrunch-1.0.2/pCrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-25 18:36:44.000000 pCrunch-1.0.2/pCrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-25 18:36:44.000000 pCrunch-1.0.2/pCrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:36:44.000000 pCrunch-1.0.2/pCrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 18:36:44.000000 pCrunch-1.0.2/pCrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 18:36:44.000000 pCrunch-1.0.2/pCrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32740 2023-04-25 18:36:36.000000 pCrunch-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:36:44.975500 pCrunch-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 18:36:36.000000 pCrunch-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.959500 pCrunch-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.963500 pCrunch-1.0.2/tests/io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:36:44.975500 pCrunch-1.0.2/tests/io/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   186142 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/AOC_WSt.out
+-rw-r--r--   0 runner    (1001) docker     (123)   130830 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/AOC_WSt.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1477853 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/DLC2.3_1.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/DLC2.3_2.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1758122 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/DLC2.3_3.out
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/Test1.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/Test2.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1347618 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/Test3.outb
+-rw-r--r--   0 runner    (1001) docker     (123)  1204577 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/data/step_0.outb
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/test_direct_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 18:36:36.000000 pCrunch-1.0.2/tests/io/test_parsers.py
```

### Comparing `pCrunch-1.0.1/LICENSE.txt` & `pCrunch-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/PKG-INFO` & `pCrunch-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pCrunch
-Version: 1.0.1
+Version: 1.0.2
 Summary: IO and Post Processing Interface for OpenFAST Results.
 Author-email: NREL WISDEM Team <systems.engineering@nrel.gov>
 Maintainer-email: Jake Nunemaker <jake.nunemaker@nrel.gov>, Nikhar Abbas <nikhar.abbas@nrel.gov>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/NREL/pCrunch
 Keywords: wind,turbine,fatigue,ultimate,aeroelastic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pCrunch-1.0.1/README.rst` & `pCrunch-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pCrunch/analysis.py` & `pCrunch-1.0.2/pCrunch/analysis.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pCrunch/io/__init__.py` & `pCrunch-1.0.2/pCrunch/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pCrunch/io/openfast.py` & `pCrunch-1.0.2/pCrunch/io/openfast.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pCrunch/utility.py` & `pCrunch-1.0.2/pCrunch/utility.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pCrunch.egg-info/PKG-INFO` & `pCrunch-1.0.2/pCrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pCrunch
-Version: 1.0.1
+Version: 1.0.2
 Summary: IO and Post Processing Interface for OpenFAST Results.
 Author-email: NREL WISDEM Team <systems.engineering@nrel.gov>
 Maintainer-email: Jake Nunemaker <jake.nunemaker@nrel.gov>, Nikhar Abbas <nikhar.abbas@nrel.gov>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/NREL/pCrunch
 Keywords: wind,turbine,fatigue,ultimate,aeroelastic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pCrunch-1.0.1/pCrunch.egg-info/SOURCES.txt` & `pCrunch-1.0.2/pCrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/pyproject.toml` & `pCrunch-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "versioneer[toml]"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pCrunch"
-version = "1.0.1"
+version = "1.0.2"
 description = "IO and Post Processing Interface for OpenFAST Results."
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {text = "Apache-2.0"}
 keywords = ["wind", "turbine", "fatigue", "ultimate", "aeroelastic"]
 authors = [
   {name = "NREL WISDEM Team", email = "systems.engineering@nrel.gov" }
@@ -38,15 +38,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: C",
   "Programming Language :: Fortran",
 ]
 
-dependencies = ["matplotlib", "numpy", "scipy", "pyyaml", "seaborn", "fatpack"]
+dependencies = ["fatpack", "numpy", "pandas", "pyyaml", "scipy"]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
 #
```

### Comparing `pCrunch-1.0.1/setup.py` & `pCrunch-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/AOC_WSt.out` & `pCrunch-1.0.2/tests/io/data/AOC_WSt.out`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/AOC_WSt.outb` & `pCrunch-1.0.2/tests/io/data/AOC_WSt.outb`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/DLC2.3_1.out` & `pCrunch-1.0.2/tests/io/data/DLC2.3_1.out`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/DLC2.3_2.out` & `pCrunch-1.0.2/tests/io/data/DLC2.3_2.out`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/DLC2.3_3.out` & `pCrunch-1.0.2/tests/io/data/DLC2.3_3.out`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/Test1.outb` & `pCrunch-1.0.2/tests/io/data/Test1.outb`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/Test2.outb` & `pCrunch-1.0.2/tests/io/data/Test2.outb`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/Test3.outb` & `pCrunch-1.0.2/tests/io/data/Test3.outb`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/data/step_0.outb` & `pCrunch-1.0.2/tests/io/data/step_0.outb`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/test_direct_inputs.py` & `pCrunch-1.0.2/tests/io/test_direct_inputs.py`

 * *Files identical despite different names*

### Comparing `pCrunch-1.0.1/tests/io/test_parsers.py` & `pCrunch-1.0.2/tests/io/test_parsers.py`

 * *Files identical despite different names*

