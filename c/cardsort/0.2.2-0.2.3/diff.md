# Comparing `tmp/cardsort-0.2.2.tar.gz` & `tmp/cardsort-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardsort-0.2.2.tar", max compression
+gzip compressed data, was "cardsort-0.2.3.tar", max compression
```

## Comparing `cardsort-0.2.2.tar` & `cardsort-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1077 2023-04-20 10:55:23.483884 cardsort-0.2.2/LICENSE
--rw-r--r--   0        0        0     2320 2023-04-20 10:55:23.483884 cardsort-0.2.2/README.md
--rw-r--r--   0        0        0     1393 2023-04-20 10:56:05.635603 cardsort-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-20 10:55:23.487884 cardsort-0.2.2/src/cardsort/__init__.py
--rw-r--r--   0        0        0     9780 2023-04-20 10:55:23.487884 cardsort-0.2.2/src/cardsort/analysis.py
--rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 cardsort-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-04-26 16:09:37.374171 cardsort-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2320 2023-04-26 16:09:37.374171 cardsort-0.2.3/README.md
+-rw-r--r--   0        0        0     1344 2023-04-26 16:10:31.430422 cardsort-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-04-26 16:09:37.378171 cardsort-0.2.3/src/cardsort/__init__.py
+-rw-r--r--   0        0        0     9780 2023-04-26 16:09:37.378171 cardsort-0.2.3/src/cardsort/analysis.py
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cardsort-0.2.3/PKG-INFO
```

### Comparing `cardsort-0.2.2/LICENSE` & `cardsort-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.2/README.md` & `cardsort-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.2/pyproject.toml` & `cardsort-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tool.poetry]
 name = "cardsort"
-version = "0.2.2"
+version = "0.2.3"
 description = "Analyse data from open card sorting"
 authors = ["Katharina Kloppenborg"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pandas = "^1.5.3"
 numpy = "^1.24.2"
 matplotlib = "^3.7.1"
 scipy = "^1.10.1"
-myst-nb = "^0.17.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 jupyter = "^1.0.0"
-myst-nb = {version = "^0.17.1", python = "^3.9"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.2.0"
 python-semantic-release = "^7.33.2"
+myst-nb = "^0.17.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
```

### Comparing `cardsort-0.2.2/src/cardsort/analysis.py` & `cardsort-0.2.3/src/cardsort/analysis.py`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.2/PKG-INFO` & `cardsort-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cardsort
-Version: 0.2.2
+Version: 0.2.3
 Summary: Analyse data from open card sorting
 License: MIT
 Author: Katharina Kloppenborg
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: myst-nb (>=0.17.1,<0.18.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Cardsort analysis
```

