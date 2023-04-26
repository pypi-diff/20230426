# Comparing `tmp/datamachine-0.0.5.tar.gz` & `tmp/datamachine-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.5.tar", last modified: Sun Apr 16 02:45:06 2023, max compression
+gzip compressed data, was "datamachine-0.0.6.tar", last modified: Tue Apr 25 17:17:36 2023, max compression
```

## Comparing `datamachine-0.0.5.tar` & `datamachine-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.453410 datamachine-0.0.5/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      755 2023-04-16 02:45:06.454410 datamachine-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.5/README.md
--rw-rw-rw-   0        0        0      652 2023-04-16 02:44:49.000000 datamachine-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      634 2023-04-16 02:45:06.455410 datamachine-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.439724 datamachine-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.444631 datamachine-0.0.5/src/datamachine/
--rw-rw-rw-   0        0        0       99 2023-04-16 00:10:59.000000 datamachine-0.0.5/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.5/src/datamachine/modular copy.py
--rw-rw-rw-   0        0        0     5028 2023-04-16 02:43:28.000000 datamachine-0.0.5/src/datamachine/modular.py
-drwxrwxrwx   0        0        0        0 2023-04-16 02:45:06.453410 datamachine-0.0.5/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 02:45:06.000000 datamachine-0.0.5/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.818833 datamachine-0.0.6/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-04-25 17:17:36.819497 datamachine-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.6/README.md
+-rw-rw-rw-   0        0        0      652 2023-04-25 17:16:16.000000 datamachine-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      634 2023-04-25 17:17:36.825620 datamachine-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.786955 datamachine-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.805210 datamachine-0.0.6/src/datamachine/
+-rw-rw-rw-   0        0        0      234 2023-04-25 17:09:05.000000 datamachine-0.0.6/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0     7768 2023-04-25 17:09:10.000000 datamachine-0.0.6/src/datamachine/_modular.py
+-rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.6/src/datamachine/xxx.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.818353 datamachine-0.0.6/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.5/LICENSE` & `datamachine-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.5/PKG-INFO` & `datamachine-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datamachine-0.0.5/pyproject.toml` & `datamachine-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `datamachine-0.0.5/setup.cfg` & `datamachine-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
```

### Comparing `datamachine-0.0.5/src/datamachine/modular copy.py` & `datamachine-0.0.6/src/datamachine/xxx.py`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.5/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.0.6/src/datamachine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

