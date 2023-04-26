# Comparing `tmp/cardsort-0.2.3.tar.gz` & `tmp/cardsort-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardsort-0.2.3.tar", max compression
+gzip compressed data, was "cardsort-0.2.4.tar", max compression
```

## Comparing `cardsort-0.2.3.tar` & `cardsort-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1077 2023-04-26 16:09:37.374171 cardsort-0.2.3/LICENSE
--rw-r--r--   0        0        0     2320 2023-04-26 16:09:37.374171 cardsort-0.2.3/README.md
--rw-r--r--   0        0        0     1344 2023-04-26 16:10:31.430422 cardsort-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-26 16:09:37.378171 cardsort-0.2.3/src/cardsort/__init__.py
--rw-r--r--   0        0        0     9780 2023-04-26 16:09:37.378171 cardsort-0.2.3/src/cardsort/analysis.py
--rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cardsort-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-04-26 16:20:46.065297 cardsort-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2320 2023-04-26 16:20:46.065297 cardsort-0.2.4/README.md
+-rw-r--r--   0        0        0     1344 2023-04-26 16:21:26.441783 cardsort-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-04-26 16:20:46.069296 cardsort-0.2.4/src/cardsort/__init__.py
+-rw-r--r--   0        0        0     9780 2023-04-26 16:20:46.069296 cardsort-0.2.4/src/cardsort/analysis.py
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cardsort-0.2.4/PKG-INFO
```

### Comparing `cardsort-0.2.3/LICENSE` & `cardsort-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.3/README.md` & `cardsort-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.3/pyproject.toml` & `cardsort-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardsort"
-version = "0.2.3"
+version = "0.2.4"
 description = "Analyse data from open card sorting"
 authors = ["Katharina Kloppenborg"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `cardsort-0.2.3/src/cardsort/analysis.py` & `cardsort-0.2.4/src/cardsort/analysis.py`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.3/PKG-INFO` & `cardsort-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardsort
-Version: 0.2.3
+Version: 0.2.4
 Summary: Analyse data from open card sorting
 License: MIT
 Author: Katharina Kloppenborg
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

