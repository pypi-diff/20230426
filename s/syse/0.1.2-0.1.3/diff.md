# Comparing `tmp/syse-0.1.2.tar.gz` & `tmp/syse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syse-0.1.2.tar", last modified: Tue Apr 25 22:34:15 2023, max compression
+gzip compressed data, was "syse-0.1.3.tar", last modified: Tue Apr 25 22:57:57 2023, max compression
```

## Comparing `syse-0.1.2.tar` & `syse-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:34:15.860370 syse-0.1.2/
--rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3066 2023-04-25 22:34:15.860370 syse-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2023-04-25 22:23:17.000000 syse-0.1.2/README.md
--rw-rw-rw-   0        0        0      751 2023-04-25 22:23:17.000000 syse-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 22:34:15.860370 syse-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-25 22:23:17.000000 syse-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:34:15.847434 syse-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 22:34:15.853434 syse-0.1.2/src/syse/
--rw-rw-rw-   0        0        0       47 2023-04-17 18:21:04.000000 syse-0.1.2/src/syse/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-04-21 21:40:27.000000 syse-0.1.2/src/syse/_syse.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:34:15.859359 syse-0.1.2/src/syse.egg-info/
--rw-rw-rw-   0        0        0     3066 2023-04-25 22:34:15.000000 syse-0.1.2/src/syse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-25 22:34:15.000000 syse-0.1.2/src/syse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:34:15.000000 syse-0.1.2/src/syse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 22:34:15.000000 syse-0.1.2/src/syse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 22:34:15.000000 syse-0.1.2/src/syse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 22:57:57.875734 syse-0.1.3/
+-rw-rw-rw-   0        0        0     1098 2023-03-20 01:15:09.000000 syse-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3119 2023-04-25 22:57:57.875734 syse-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1118 2023-04-25 22:54:39.000000 syse-0.1.3/README.md
+-rw-rw-rw-   0        0        0      785 2023-04-25 22:57:37.000000 syse-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:57:57.876727 syse-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-04-25 22:57:37.000000 syse-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:57:57.860343 syse-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 22:57:57.868223 syse-0.1.3/src/syse/
+-rw-rw-rw-   0        0        0       47 2023-04-17 18:21:04.000000 syse-0.1.3/src/syse/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-04-21 21:40:27.000000 syse-0.1.3/src/syse/_syse.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:57:57.874726 syse-0.1.3/src/syse.egg-info/
+-rw-rw-rw-   0        0        0     3119 2023-04-25 22:57:57.000000 syse-0.1.3/src/syse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-25 22:57:57.000000 syse-0.1.3/src/syse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:57:57.000000 syse-0.1.3/src/syse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 22:57:57.000000 syse-0.1.3/src/syse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 22:57:57.000000 syse-0.1.3/src/syse.egg-info/top_level.txt
```

### Comparing `syse-0.1.2/LICENSE` & `syse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syse-0.1.2/PKG-INFO` & `syse-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Systems & Industrial Engineering Python Package
-Home-page: https://github.com/apexpromgt/SysE
+Home-page: https://github.com/Apex-Engineering-Management/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,28 +22,29 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/apexpromgt/SysE
+Project-URL: Homepage, https://github.com/Apex-Engineering-Management/SysE
 Project-URL: Documentation, https://syse.readthedocs.io/en/latest/
-Project-URL: Bug Tracker, https://github.com/apexpromgt/SysE/issues
+Project-URL: Bug Tracker, https://github.com/Apex-Engineering-Management/SysE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/syse?period=total&units=none&left_color=black&right_color=red&left_text=Downloads)](https://pepy.tech/project/syse)
 
+
 SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
```

### Comparing `syse-0.1.2/README.md` & `syse-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/syse?period=total&units=none&left_color=black&right_color=red&left_text=Downloads)](https://pepy.tech/project/syse)
 
+
 SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
```

### Comparing `syse-0.1.2/pyproject.toml` & `syse-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syse"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Jonathon Nicholson", email="Jonathon@apexpromgt.com" },
 ]
 description = "Systems & Industrial Engineering Python Package"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
@@ -16,10 +16,10 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/apexpromgt/SysE"
+"Homepage" = "https://github.com/Apex-Engineering-Management/SysE"
 "Documentation" = "https://syse.readthedocs.io/en/latest/"
-"Bug Tracker" = "https://github.com/apexpromgt/SysE/issues"
+"Bug Tracker" = "https://github.com/Apex-Engineering-Management/SysE/issues"
```

### Comparing `syse-0.1.2/setup.py` & `syse-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "syse",
-    version = "0.1.2",
+    version = "0.1.3",
     author = "Jonathon Nicholson",
     author_email = "Jonathon@apexpromgt.com",
     description = "Systems & Industrial Engineering Python Package",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/apexpromgt/SysE",
+    url = "https://github.com/Apex-Engineering-Management/SysE",
     project_urls = {
-        "Homepage": "https://github.com/apexpromgt/SysE",
+        "Homepage": "https://github.com/Apex-Engineering-Management/SysE",
         "Documentation": "https://syse.readthedocs.io/en/latest/",
-        "Bug Tracker":"https://github.com/apexpromgt/SysE/issues"
+        "Bug Tracker":"https://github.com/Apex-Engineering-Management/SysE/issues"
     },
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir = {"": "src"},
```

### Comparing `syse-0.1.2/src/syse/_syse.py` & `syse-0.1.3/src/syse/_syse.py`

 * *Files identical despite different names*

### Comparing `syse-0.1.2/src/syse.egg-info/PKG-INFO` & `syse-0.1.3/src/syse.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: syse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Systems & Industrial Engineering Python Package
-Home-page: https://github.com/apexpromgt/SysE
+Home-page: https://github.com/Apex-Engineering-Management/SysE
 Author: Jonathon Nicholson
 Author-email: Jonathon Nicholson <Jonathon@apexpromgt.com>
 License: MIT License
         
         Copyright (c) [2023] [Jonathon Nicholson]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,28 +22,29 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/apexpromgt/SysE
+Project-URL: Homepage, https://github.com/Apex-Engineering-Management/SysE
 Project-URL: Documentation, https://syse.readthedocs.io/en/latest/
-Project-URL: Bug Tracker, https://github.com/apexpromgt/SysE/issues
+Project-URL: Bug Tracker, https://github.com/Apex-Engineering-Management/SysE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to the SysE Python Package!
 
 [![Documentation Status](https://readthedocs.org/projects/syse/badge/?version=latest)](https://syse.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/syse?period=total&units=none&left_color=black&right_color=red&left_text=Downloads)](https://pepy.tech/project/syse)
 
+
 SysE is a Python library for Industrial and Systems Engineering.
 
 SysE covers common Industrial & Systems Engineering topics such as:
 * Engineering Economics 
 * Probability & Statistics
 * Modeling & Quantitative Analysis
 * Engineering Management
```

