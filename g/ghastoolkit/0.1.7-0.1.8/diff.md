# Comparing `tmp/ghastoolkit-0.1.7.tar.gz` & `tmp/ghastoolkit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.7.tar", last modified: Tue Apr 25 23:51:36 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.8.tar", last modified: Tue Apr 25 23:55:22 2023, max compression
```

## Comparing `ghastoolkit-0.1.7.tar` & `ghastoolkit-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.140591 ghastoolkit-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:51:36.140591 ghastoolkit-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:51:36.140591 ghastoolkit-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.132592 ghastoolkit-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.132592 ghastoolkit-0.1.7/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.136592 ghastoolkit-0.1.7/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.136592 ghastoolkit-0.1.7/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.136592 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:51:36.000000 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 23:51:36.000000 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:51:36.000000 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 23:51:36.000000 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 23:51:36.000000 ghastoolkit-0.1.7/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:51:36.140591 ghastoolkit-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 23:51:05.000000 ghastoolkit-0.1.7/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.210814 ghastoolkit-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.1.7/LICENSE` & `ghastoolkit-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/PKG-INFO` & `ghastoolkit-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.7
+Version: 0.1.8
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.7/README.md` & `ghastoolkit-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/pyproject.toml` & `ghastoolkit-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -18,14 +18,15 @@
 ]
 dependencies = [
     "certifi==2022.12.7",
     "charset-normalizer==3.1.0",
     "idna==3.4",
     "PyYAML==6.0",
     "requests==2.28.2",
+    "ratelimit==2.2.1",
     "urllib3==1.26.15"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/ghastoolkit"
 "Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
```

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/__init__.py` & `ghastoolkit-0.1.8/src/ghastoolkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.8/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.8/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.8/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.8/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.8/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.8/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.1.8/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.8/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.7
+Version: 0.1.8
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.7/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.8/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_codeqldb.py` & `ghastoolkit-0.1.8/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_codescanning.py` & `ghastoolkit-0.1.8/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_depgraph.py` & `ghastoolkit-0.1.8/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_github.py` & `ghastoolkit-0.1.8/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_octokit.py` & `ghastoolkit-0.1.8/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.7/tests/test_secretscanning.py` & `ghastoolkit-0.1.8/tests/test_secretscanning.py`

 * *Files identical despite different names*

