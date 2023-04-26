# Comparing `tmp/airgiant-0.1.1.tar.gz` & `tmp/airgiant-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.1.1.tar", last modified: Tue Apr 25 13:31:52 2023, max compression
+gzip compressed data, was "airgiant-0.1.2.tar", last modified: Tue Apr 25 13:36:47 2023, max compression
```

## Comparing `airgiant-0.1.1.tar` & `airgiant-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.530736 airgiant-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-25 13:31:52.526736 airgiant-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.1.1/README.md
--rw-rw-rw-   0        0        0      595 2023-04-25 13:31:26.000000 airgiant-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 13:31:52.530736 airgiant-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.395120 airgiant-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.401789 airgiant-0.1.1/src/airgiant/
--rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.1.1/src/airgiant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.526736 airgiant-0.1.1/src/airgiant/state/
--rw-rw-rw-   0        0        0       21 2023-04-25 13:24:38.000000 airgiant-0.1.1/src/airgiant/state/__init__.py
--rw-rw-rw-   0        0        0    15475 2023-04-25 13:31:02.000000 airgiant-0.1.1/src/airgiant/state/behavior.py
--rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.1.1/src/airgiant/state/hello.py
--rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.1.1/src/airgiant/state/imports.py
--rw-rw-rw-   0        0        0      539 2023-04-25 13:31:03.000000 airgiant-0.1.1/src/airgiant/state/main.py
--rw-rw-rw-   0        0        0     1856 2023-04-25 13:31:04.000000 airgiant-0.1.1/src/airgiant/state/make_decision.py
--rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.1.1/src/airgiant/state/tempCodeRunnerFile.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.526736 airgiant-0.1.1/src/airgiant/zed/
--rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.1.1/src/airgiant/zed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.425781 airgiant-0.1.1/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.287867 airgiant-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:36:47.286170 airgiant-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.1.2/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-25 13:35:57.000000 airgiant-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:36:47.287867 airgiant-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.179161 airgiant-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.186490 airgiant-0.1.2/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.1.2/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.283048 airgiant-0.1.2/src/airgiant/state/
+-rw-rw-rw-   0        0        0       21 2023-04-25 13:24:38.000000 airgiant-0.1.2/src/airgiant/state/__init__.py
+-rw-rw-rw-   0        0        0    15475 2023-04-25 13:35:48.000000 airgiant-0.1.2/src/airgiant/state/behavior.py
+-rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.1.2/src/airgiant/state/hello.py
+-rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.1.2/src/airgiant/state/imports.py
+-rw-rw-rw-   0        0        0      542 2023-04-25 13:35:41.000000 airgiant-0.1.2/src/airgiant/state/main.py
+-rw-rw-rw-   0        0        0     1856 2023-04-25 13:31:04.000000 airgiant-0.1.2/src/airgiant/state/make_decision.py
+-rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.1.2/src/airgiant/state/tempCodeRunnerFile.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.283048 airgiant-0.1.2/src/airgiant/zed/
+-rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.1.2/src/airgiant/zed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:36:47.237078 airgiant-0.1.2/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:36:47.000000 airgiant-0.1.2/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-25 13:36:47.000000 airgiant-0.1.2/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:36:47.000000 airgiant-0.1.2/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 13:36:47.000000 airgiant-0.1.2/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.1.1/LICENSE` & `airgiant-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.1.1/PKG-INFO` & `airgiant-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.1.1/pyproject.toml` & `airgiant-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.1.1/src/airgiant/state/behavior.py` & `airgiant-0.1.2/src/airgiant/state/behavior.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.1.1/src/airgiant/state/main.py` & `airgiant-0.1.2/src/airgiant/state/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from imports import *
+from .imports import *
 
 # GLOBAL variables 
 
 person1 = [0,0,0]           # xyz of detected person > see SkelCoord()
 rwristperson = [0,0,0]
 lwristperson = [0,0,0]
 finalstate = 0              # confident state > see decision()
-i = 1                       # true condition
+i = 1                        # true condition
 p = 0                       # person detected (0 not, 1 detected)
 ac=3
 
 
-from behavior import *
+from .behavior import *
 from .make_decision import *
 
 
 logging.basicConfig(
     format="%(asctime)s %(message)s",
     level=logging.CRITICAL #.DEBUG,
 )
```

### Comparing `airgiant-0.1.1/src/airgiant/state/make_decision.py` & `airgiant-0.1.2/src/airgiant/state/make_decision.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.1.1/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.1.2/src/airgiant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

