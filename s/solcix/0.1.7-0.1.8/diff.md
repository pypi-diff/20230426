# Comparing `tmp/solcix-0.1.7.tar.gz` & `tmp/solcix-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solcix-0.1.7.tar", max compression
+gzip compressed data, was "solcix-0.1.8.tar", max compression
```

## Comparing `solcix-0.1.7.tar` & `solcix-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34523 2023-04-07 11:28:07.282960 solcix-0.1.7/LICENSE
--rw-r--r--   0        0        0     8208 2023-04-07 11:28:07.282960 solcix-0.1.7/README.md
--rw-r--r--   0        0        0      871 2023-04-07 11:28:07.282960 solcix-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1109 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/__init__.py
--rw-r--r--   0        0        0     9081 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/__main__.py
--rw-r--r--   0        0        0      182 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/compile/__init__.py
--rw-r--r--   0        0        0    19156 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/compile/solc.py
--rw-r--r--   0        0        0      618 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/constant.py
--rw-r--r--   0        0        0      110 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/datatypes/__init__.py
--rw-r--r--   0        0        0     3949 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/datatypes/datatypes.py
--rw-r--r--   0        0        0     3407 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/errors.py
--rw-r--r--   0        0        0    21648 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/installer.py
--rw-r--r--   0        0        0      241 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/manage/__init__.py
--rw-r--r--   0        0        0     3773 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/manage/manage.py
--rw-r--r--   0        0        0    10656 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/resolver.py
--rw-r--r--   0        0        0      597 2023-04-07 11:28:07.282960 solcix-0.1.7/solcix/utils.py
--rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 solcix-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-26 09:08:46.828764 solcix-0.1.8/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-26 09:08:46.828764 solcix-0.1.8/README.md
+-rw-r--r--   0        0        0      871 2023-04-26 09:08:46.828764 solcix-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1109 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/__init__.py
+-rw-r--r--   0        0        0     9081 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/__main__.py
+-rw-r--r--   0        0        0      182 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/compile/__init__.py
+-rw-r--r--   0        0        0    19156 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/compile/solc.py
+-rw-r--r--   0        0        0      618 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/constant.py
+-rw-r--r--   0        0        0      110 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/datatypes/__init__.py
+-rw-r--r--   0        0        0     3949 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/datatypes/datatypes.py
+-rw-r--r--   0        0        0     3407 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/errors.py
+-rw-r--r--   0        0        0    21648 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/installer.py
+-rw-r--r--   0        0        0      241 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/manage/__init__.py
+-rw-r--r--   0        0        0     3803 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/manage/manage.py
+-rw-r--r--   0        0        0    10656 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/resolver.py
+-rw-r--r--   0        0        0      597 2023-04-26 09:08:46.828764 solcix-0.1.8/solcix/utils.py
+-rw-r--r--   0        0        0     9453 1970-01-01 00:00:00.000000 solcix-0.1.8/PKG-INFO
```

### Comparing `solcix-0.1.7/LICENSE` & `solcix-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/README.md` & `solcix-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Solcix
 
 [![Version](https://img.shields.io/pypi/v/solcix?color=green)](https://pypi.org/project/solcix?style=flat) [![Release](https://img.shields.io/github/v/release/Solratic/solcix?color=green)](https://github.com/Solratic/solcix) [![Python Versions](https://img.shields.io/pypi/pyversions/solcix?style=flat&color=306998)](https://pypi.org/project/solcix/) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black) [![Activity](https://img.shields.io/github/commit-activity/w/Solratic/solcix?color=yellow)](https://github.com/Solratic/solcix) [![License](https://img.shields.io/github/license/Solratic/solcix?style=flat&color=orange)](https://github.com/Solratic/solcix/blob/main/LICENSE)
 
 Solcix is a Solidity version manager written in Python that allows for seamless switching between versions, easy compilation, and simple management of artifacts.
 
+[![asciicast](https://asciinema.org/a/580682.svg)](https://asciinema.org/a/580682)
+
 ## Installation
 
 To install Solcix, you can use pip, the Python package manager:
 
 ### With pip For Windows
 
 ```bash
```

### Comparing `solcix-0.1.7/pyproject.toml` & `solcix-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solcix"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Python wrapper for the Solidity compiler. Switch between versions, compile, and manage artifacts."
 authors = ["alan890104 <alan890104@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cfgv = "3.3.1"
```

### Comparing `solcix-0.1.7/solcix/__init__.py` & `solcix-0.1.8/solcix/__init__.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/__main__.py` & `solcix-0.1.8/solcix/__main__.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/compile/solc.py` & `solcix-0.1.8/solcix/compile/solc.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/constant.py` & `solcix-0.1.8/solcix/constant.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/datatypes/datatypes.py` & `solcix-0.1.8/solcix/datatypes/datatypes.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/errors.py` & `solcix-0.1.8/solcix/errors.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/installer.py` & `solcix-0.1.8/solcix/installer.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/manage/manage.py` & `solcix-0.1.8/solcix/manage/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,13 +113,13 @@
     """
     Clears the current (may be global or local) configuration file.
 
     Returns:
     --------
     None
     """
-    if os.path.exists(".solcix"):
+    if os.path.exists(".solcix") and os.path.isfile(".solcix"):
         os.remove(".solcix")
         print("✨ Cleared local configuration ✨")
     elif os.path.exists(SOLCIX_DIR.joinpath("global-version")):
         os.remove(SOLCIX_DIR.joinpath("global-version"))
         print("✨ Cleared global configuration ✨")
```

### Comparing `solcix-0.1.7/solcix/resolver.py` & `solcix-0.1.8/solcix/resolver.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/solcix/utils.py` & `solcix-0.1.8/solcix/utils.py`

 * *Files identical despite different names*

### Comparing `solcix-0.1.7/PKG-INFO` & `solcix-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solcix
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python wrapper for the Solidity compiler. Switch between versions, compile, and manage artifacts.
 Author: alan890104
 Author-email: alan890104@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,14 +32,16 @@
 
 # Solcix
 
 [![Version](https://img.shields.io/pypi/v/solcix?color=green)](https://pypi.org/project/solcix?style=flat) [![Release](https://img.shields.io/github/v/release/Solratic/solcix?color=green)](https://github.com/Solratic/solcix) [![Python Versions](https://img.shields.io/pypi/pyversions/solcix?style=flat&color=306998)](https://pypi.org/project/solcix/) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black) [![Activity](https://img.shields.io/github/commit-activity/w/Solratic/solcix?color=yellow)](https://github.com/Solratic/solcix) [![License](https://img.shields.io/github/license/Solratic/solcix?style=flat&color=orange)](https://github.com/Solratic/solcix/blob/main/LICENSE)
 
 Solcix is a Solidity version manager written in Python that allows for seamless switching between versions, easy compilation, and simple management of artifacts.
 
+[![asciicast](https://asciinema.org/a/580682.svg)](https://asciinema.org/a/580682)
+
 ## Installation
 
 To install Solcix, you can use pip, the Python package manager:
 
 ### With pip For Windows
 
 ```bash
```

