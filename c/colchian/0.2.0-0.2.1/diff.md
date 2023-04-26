# Comparing `tmp/colchian-0.2.0.tar.gz` & `tmp/colchian-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\colchian-0.2.0.tar", last modified: Wed Apr 26 03:53:35 2023, max compression
+gzip compressed data, was "dist\colchian-0.2.1.tar", last modified: Wed Apr 26 03:57:37 2023, max compression
```

## Comparing `colchian-0.2.0.tar` & `colchian-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 03:53:35.000000 colchian-0.2.0/
--rw-rw-rw-   0        0        0     1101 2021-09-02 05:36:15.000000 colchian-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     8337 2023-04-26 03:53:35.000000 colchian-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7707 2023-04-26 02:30:54.000000 colchian-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian/
--rw-rw-rw-   0        0        0       67 2023-04-26 01:59:40.000000 colchian-0.2.0/colchian/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-26 03:52:32.000000 colchian-0.2.0/colchian/_version.py
--rw-rw-rw-   0        0        0    17515 2023-04-26 02:30:54.000000 colchian-0.2.0/colchian/colchian.py
-drwxrwxrwx   0        0        0        0 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/
--rw-rw-rw-   0        0        0     8337 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 03:53:35.000000 colchian-0.2.0/colchian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-26 03:53:35.000000 colchian-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1761 2023-04-26 02:48:36.000000 colchian-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 03:53:35.000000 colchian-0.2.0/test/
--rw-rw-rw-   0        0        0    15529 2023-04-26 02:30:54.000000 colchian-0.2.0/test/test_colchian.py
--rw-rw-rw-   0        0        0        0 2023-04-26 02:30:54.000000 colchian-0.2.0/test/test_docs_examples.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:57:37.000000 colchian-0.2.1/
+-rw-rw-rw-   0        0        0     1101 2021-09-02 05:36:15.000000 colchian-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     8337 2023-04-26 03:57:37.000000 colchian-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7707 2023-04-26 02:30:54.000000 colchian-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian/
+-rw-rw-rw-   0        0        0       67 2023-04-26 01:59:40.000000 colchian-0.2.1/colchian/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-26 03:57:26.000000 colchian-0.2.1/colchian/_version.py
+-rw-rw-rw-   0        0        0    17515 2023-04-26 02:30:54.000000 colchian-0.2.1/colchian/colchian.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/
+-rw-rw-rw-   0        0        0     8337 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 03:57:37.000000 colchian-0.2.1/colchian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-26 03:56:47.000000 colchian-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-26 03:57:37.000000 colchian-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1761 2023-04-26 02:48:36.000000 colchian-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 03:57:37.000000 colchian-0.2.1/test/
+-rw-rw-rw-   0        0        0    15529 2023-04-26 02:30:54.000000 colchian-0.2.1/test/test_colchian.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 02:30:54.000000 colchian-0.2.1/test/test_docs_examples.py
```

### Comparing `colchian-0.2.0/LICENSE` & `colchian-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colchian-0.2.0/PKG-INFO` & `colchian-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colchian
-Version: 0.2.0
+Version: 0.2.1
 Summary: Validate json/yaml documents using a Python dictionary defining keys and types.
 Home-page: https://gitlab.com/jaapvandervelde/colchian
 Author: BMT Commercial Australia Pty Ltd, Jaap van der Velde
 Author-email: jaap.vandervelde@bmtglobal.com
 License: MIT
 Keywords: json,validator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `colchian-0.2.0/README.md` & `colchian-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `colchian-0.2.0/colchian/colchian.py` & `colchian-0.2.1/colchian/colchian.py`

 * *Files identical despite different names*

### Comparing `colchian-0.2.0/colchian.egg-info/PKG-INFO` & `colchian-0.2.1/colchian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colchian
-Version: 0.2.0
+Version: 0.2.1
 Summary: Validate json/yaml documents using a Python dictionary defining keys and types.
 Home-page: https://gitlab.com/jaapvandervelde/colchian
 Author: BMT Commercial Australia Pty Ltd, Jaap van der Velde
 Author-email: jaap.vandervelde@bmtglobal.com
 License: MIT
 Keywords: json,validator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `colchian-0.2.0/setup.py` & `colchian-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `colchian-0.2.0/test/test_colchian.py` & `colchian-0.2.1/test/test_colchian.py`

 * *Files identical despite different names*

