# Comparing `tmp/grgrlib-0.1.9.tar.gz` & `tmp/grgrlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grgrlib-0.1.9.tar", last modified: Sun Jun 12 21:17:38 2022, max compression
+gzip compressed data, was "grgrlib-0.2.0.tar", last modified: Wed Apr 26 13:02:59 2023, max compression
```

## Comparing `grgrlib-0.1.9.tar` & `grgrlib-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.153880 grgrlib-0.1.9/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       72 2021-12-16 14:43:37.000000 grgrlib-0.1.9/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2022-02-27 22:25:46.000000 grgrlib-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2019-12-03 02:24:07.000000 grgrlib-0.1.9/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1251 2022-06-12 21:17:38.153880 grgrlib-0.1.9/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      812 2022-02-24 19:51:20.000000 grgrlib-0.1.9/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.150546 grgrlib-0.1.9/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2019-10-10 21:03:23.000000 grgrlib-0.1.9/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.150546 grgrlib-0.1.9/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.150546 grgrlib-0.1.9/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2022-05-29 13:20:44.000000 grgrlib-0.1.9/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2442 2022-05-29 19:38:14.000000 grgrlib-0.1.9/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       92 2019-10-10 21:03:23.000000 grgrlib-0.1.9/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       86 2019-10-10 21:03:23.000000 grgrlib-0.1.9/docs/indices.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2019-10-10 21:03:23.000000 grgrlib-0.1.9/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      860 2022-05-29 12:16:15.000000 grgrlib-0.1.9/docs/modules.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2019-10-10 21:03:23.000000 grgrlib-0.1.9/docs/readme.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.153880 grgrlib-0.1.9/grgrlib/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      203 2022-06-12 07:39:50.000000 grgrlib-0.1.9/grgrlib/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      556 2022-02-27 22:25:46.000000 grgrlib-0.1.9/grgrlib/datatools.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1002 2022-04-28 02:56:39.000000 grgrlib-0.1.9/grgrlib/dist.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3482 2022-04-28 03:01:42.000000 grgrlib-0.1.9/grgrlib/econtools.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3437 2022-05-09 11:35:27.000000 grgrlib-0.1.9/grgrlib/generic.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1896 2022-04-28 14:52:37.000000 grgrlib-0.1.9/grgrlib/h5.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8662 2022-06-12 21:17:11.000000 grgrlib-0.1.9/grgrlib/jaxed.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2356 2022-03-21 17:54:07.000000 grgrlib-0.1.9/grgrlib/legacy.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    10355 2022-04-28 03:04:54.000000 grgrlib-0.1.9/grgrlib/linalg.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1634 2022-02-01 10:09:04.000000 grgrlib-0.1.9/grgrlib/multiprocessing.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2016 2022-05-29 12:12:29.000000 grgrlib-0.1.9/grgrlib/njitted.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      891 2022-01-28 23:47:28.000000 grgrlib-0.1.9/grgrlib/numerics.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    24369 2021-07-13 12:16:49.000000 grgrlib-0.1.9/grgrlib/optimize.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2022-05-23 20:07:36.000000 grgrlib-0.1.9/grgrlib/plots.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3355 2022-04-04 21:33:13.000000 grgrlib-0.1.9/grgrlib/stats.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2022-06-12 21:17:38.153880 grgrlib-0.1.9/grgrlib.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1251 2022-06-12 21:17:37.000000 grgrlib-0.1.9/grgrlib.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2022-06-12 21:17:38.000000 grgrlib-0.1.9/grgrlib.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2022-06-12 21:17:37.000000 grgrlib-0.1.9/grgrlib.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       49 2022-06-12 21:17:37.000000 grgrlib-0.1.9/grgrlib.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2022-06-12 21:17:38.000000 grgrlib-0.1.9/grgrlib.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2022-06-12 21:17:38.153880 grgrlib-0.1.9/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      989 2022-06-12 21:16:43.000000 grgrlib-0.1.9/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.803528 grgrlib-0.2.0/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      175 2023-04-25 16:22:51.000000 grgrlib-0.2.0/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      281 2023-04-25 16:22:51.000000 grgrlib-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-04-25 16:22:51.000000 grgrlib-0.2.0/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1433 2023-04-26 13:02:59.803528 grgrlib-0.2.0/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      926 2023-04-25 16:22:51.000000 grgrlib-0.2.0/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.796862 grgrlib-0.2.0/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.793529 grgrlib-0.2.0/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.796862 grgrlib-0.2.0/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2433 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       92 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       86 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/indices.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      795 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      983 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/modules.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       27 2023-04-25 16:22:51.000000 grgrlib-0.2.0/docs/readme.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.800195 grgrlib-0.2.0/grgrlib/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      378 2023-04-26 13:02:06.000000 grgrlib-0.2.0/grgrlib/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-04-26 13:02:52.000000 grgrlib-0.2.0/grgrlib/__version__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      542 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/datatools.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      988 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/dist.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3468 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/econtools.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3423 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/generic.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1882 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/h5.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6132 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/hanktools.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13727 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/jaxed.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2342 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/legacy.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5627 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/linalg.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1620 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/multiprocessing.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7510 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/njitted.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      896 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/numerics.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    24438 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/optimize.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13701 2023-04-26 12:54:54.000000 grgrlib-0.2.0/grgrlib/plots.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2514 2023-04-25 16:22:51.000000 grgrlib-0.2.0/grgrlib/stats.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-26 13:02:59.803528 grgrlib-0.2.0/grgrlib.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1433 2023-04-26 13:02:59.000000 grgrlib-0.2.0/grgrlib.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      695 2023-04-26 13:02:59.000000 grgrlib-0.2.0/grgrlib.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-26 13:02:59.000000 grgrlib-0.2.0/grgrlib.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       91 2023-04-26 13:02:59.000000 grgrlib-0.2.0/grgrlib.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        8 2023-04-26 13:02:59.000000 grgrlib-0.2.0/grgrlib.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       23 2023-04-25 16:22:51.000000 grgrlib-0.2.0/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-26 13:02:59.803528 grgrlib-0.2.0/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1214 2023-04-26 12:59:44.000000 grgrlib-0.2.0/setup.py
```

### Comparing `grgrlib-0.1.9/LICENSE` & `grgrlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grgrlib-0.1.9/PKG-INFO` & `grgrlib-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: grgrlib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Various insanely helpful functions
 Home-page: https://github.com/gboehl/grgrlib
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: njitted
+Provides-Extra: jaxed
+Provides-Extra: opti
+Provides-Extra: data
 License-File: LICENSE
 
 
 grgrlib
 =======
 
-This is a library of unspeakably (hence the name) useful functions. It serves as a container for functions shared across other projects. 
+This is a library of unspeakably useful functions. It serves as a container for a rather loose collection of tools shared across other projects that may or may not be individually useful. 
 
 Installation with ``pip``
 -----------------------------
 
-It's as simple as:
+It's as simple as typing
 
 .. code-block:: bash
 
    pip install grgrlib
 
+in the terminal (Unix/Mac) or the Anaconda Prompt (Win).
 
 Installation of bleeding-edge version using ``git``
 ---------------------------------------------------
 
 The handy way is to first install ``git``. Linux users just use their respective repos. Look into `this repo <https://github.com/gboehl/pydsge/blob/master/README.rst>`_ for details.
 
 .. code-block:: bash
@@ -39,9 +43,7 @@
    pip install git+https://github.com/gboehl/grgrlib
 
 Alternatively you can clone the repository and then from within the cloned folder run (Windows user from the Anaconda Prompt):
 
 .. code-block:: bash
 
    pip install .
-
-
```

### Comparing `grgrlib-0.1.9/README.rst` & `grgrlib-0.2.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 grgrlib
 =======
 
-This is a library of unspeakably (hence the name) useful functions. It serves as a container for functions shared across other projects. 
+This is a library of unspeakably useful functions. It serves as a container for a rather loose collection of tools shared across other projects that may or may not be individually useful. 
 
 Installation with ``pip``
 -----------------------------
 
-It's as simple as:
+It's as simple as typing
 
 .. code-block:: bash
 
    pip install grgrlib
 
+in the terminal (Unix/Mac) or the Anaconda Prompt (Win).
 
 Installation of bleeding-edge version using ``git``
 ---------------------------------------------------
 
 The handy way is to first install ``git``. Linux users just use their respective repos. Look into `this repo <https://github.com/gboehl/pydsge/blob/master/README.rst>`_ for details.
 
 .. code-block:: bash
```

### Comparing `grgrlib-0.1.9/docs/Makefile` & `grgrlib-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grgrlib-0.1.9/docs/conf.py` & `grgrlib-0.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 html_theme = 'alabaster'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 autodoc_mock_imports = ['econsieve', 'particles', 'numpy', 'pandas', 'emcee', 'kombine', 'pathos',
-                        'yaml', 'sympy', 'scipy', 'numba', 'tqdm', 'dill', 'pygmo', 'matplotlib', 'interpolation', 'chaospy']
+                        'yaml', 'scipy', 'numba', 'tqdm', 'dill', 'pygmo', 'matplotlib', 'interpolation', 'chaospy']
 
 
 def setup(app):
     app.add_stylesheet('css/custom.css')
 
 
 master_doc = 'index'
```

### Comparing `grgrlib-0.1.9/docs/make.bat` & `grgrlib-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grgrlib-0.1.9/docs/modules.rst` & `grgrlib-0.2.0/docs/modules.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Documentation
 ==================
 
-``grgrlib.datatools``
----------------------
-.. automodule:: grgrlib.datatools
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 ``grgrlib.plots``
 ------------------
 A collection of handy plotting functions.
 
 .. automodule:: grgrlib.plots
    :members:
    :undoc-members:
    :show-inheritance:
 
-``grgrlib.optimize``
---------------------
-Hand-written optimizers. Currently only CMA-ES. Look for the documentation of `cmaes` (the UI) to understand its usage.
-
-.. automodule:: grgrlib.optimize
+``grgrlib.jaxed``
+-------------------
+.. automodule:: grgrlib.jaxed
    :members:
    :undoc-members:
    :show-inheritance:
 
 ``grgrlib.njitted``
 -------------------
 .. automodule:: grgrlib.njitted
    :members:
    :undoc-members:
    :show-inheritance:
 
+``grgrlib.datatools``
+---------------------
+.. automodule:: grgrlib.datatools
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 ``grgrlib.multiprocessing``
 ---------------------------
 .. automodule:: grgrlib.multiprocessing
    :members:
    :undoc-members:
    :show-inheritance:
+
+``grgrlib.optimize``
+--------------------
+Hand-written optimizers. Currently only CMA-ES. Look for the documentation of `cmaes` (the UI) to understand its usage.
+
+.. automodule:: grgrlib.optimize
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `grgrlib-0.1.9/grgrlib/datatools.py` & `grgrlib-0.2.0/grgrlib/datatools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 
 
 def sdw_parser(x):
```

### Comparing `grgrlib-0.1.9/grgrlib/dist.py` & `grgrlib-0.2.0/grgrlib/dist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from numba import njit, prange
 from grgrlib.numerics import chebychev
 
 """EXPERIMENTAL!!!"""
```

### Comparing `grgrlib-0.1.9/grgrlib/econtools.py` & `grgrlib-0.2.0/grgrlib/econtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import numpy.linalg as nl
 import scipy.linalg as sl
 import time
 from .linalg import ouc, fast0
```

### Comparing `grgrlib-0.1.9/grgrlib/generic.py` & `grgrlib-0.2.0/grgrlib/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import time
 import os
 import sys
 import numpy as np
 import numpy.linalg as nl
```

### Comparing `grgrlib-0.1.9/grgrlib/h5.py` & `grgrlib-0.2.0/grgrlib/h5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import os
 import h5py
 import numpy as np
```

### Comparing `grgrlib-0.1.9/grgrlib/jaxed.py` & `grgrlib-0.2.0/grgrlib/jaxed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,87 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import jax
 import time
 import functools
 import jax.numpy as jnp
 import scipy.sparse as ssp
 from numpy import ndarray, isnan
+from numpy.linalg import det
 from .plots import spy
 from jax.experimental.host_callback import id_print as jax_print
-from jax._src.api import (_check_callable, _check_input_dtype_jacfwd, _check_output_dtype_jacfwd, _ensure_index,
-                          _jvp, _std_basis, _jacfwd_unravel, lu, argnums_partial, tree_map, partial, Callable, Sequence, Union, vmap)
+from jax._src.api import (_check_input_dtype_jacfwd, _check_input_dtype_jacrev, _check_output_dtype_jacfwd, _check_output_dtype_jacrev, _ensure_index, _jvp,
+                          _vjp, _std_basis, _jacfwd_unravel, _jacrev_unravel, lu, argnums_partial, tree_map, tree_structure, tree_transpose, partial, Callable, Sequence, Union, vmap)
+# fix import location for jax 0.4.1
+try:
+    from jax._src.api import _check_callable
+except ImportError:
+    from jax._src.api_util import check_callable as _check_callable
+
+
+def jvp_vmap(fun: Callable, argnums: Union[int, Sequence[int]] = 0):
+    """Vectorized (forward-mode) jacobian-vector product of ``fun``. This is by large adopted from the implementation of jacfwd in jax._src.api.
+
+    Args:
+      fun: Function whose value and Jacobian is to be computed.
+      argnums: Optional, integer or sequence of integers. Specifies which
+        positional argument(s) to differentiate with respect to (default ``0``).
+
+    Returns:
+      A function with the same arguments as ``fun``, that evaluates the value and Jacobian of
+      ``fun`` using forward-mode automatic differentiation.
+    """
+    _check_callable(fun)
+    argnums = _ensure_index(argnums)
+
+    def jvpfun(args, tangents, **kwargs):
+
+        f = lu.wrap_init(fun, kwargs)
+        f_partial, dyn_args = argnums_partial(
+            f, argnums, args, require_static_args_hashable=False)
+        pushfwd = partial(_jvp, f_partial, dyn_args)
+        y, jac = vmap(pushfwd, out_axes=(None, -1), in_axes=-1)(tangents)
+
+        return y, jac
+
+    return jvpfun
+
+
+def vjp_vmap(fun: Callable, argnums: Union[int, Sequence[int]] = 0):
+    """Vectorized (reverse-mode) vector-jacobian product of ``fun``. This is by large adopted from the implementation of jacrev in jax._src.api.
+
+    Args:
+      fun: Function whose value and Jacobian are to be computed.
+      argnums: Optional, integer or sequence of integers. Specifies which
+        positional argument(s) to differentiate with respect to (default ``0``).
+
+    Returns:
+      A function with the same arguments as ``fun``, that evaluates the value and Jacobian of
+      ``fun`` using reverse-mode automatic differentiation.
+    """
+    _check_callable(fun)
+
+    def vjpfun(args, tangents, **kwargs):
+        f = lu.wrap_init(fun, kwargs)
+        f_partial, dyn_args = argnums_partial(f, argnums, args,
+                                              require_static_args_hashable=False)
+        y, pullback = _vjp(f_partial, *dyn_args)
+        jac = vmap(pullback)(tangents)
+        return y, jac
+
+    return vjpfun
 
 
 def jacfwd_and_val(fun: Callable, argnums: Union[int, Sequence[int]] = 0,
                    has_aux: bool = False, holomorphic: bool = False) -> Callable:
     """Value and Jacobian of ``fun`` evaluated column-by-column using forward-mode AD. Apart from returning the function value, this is one-to-one adopted from
   jax._src.api.
 
     Args:
-      fun: Function whose Jacobian is to be computed.
+      fun: Function whose value and Jacobian is to be computed.
       argnums: Optional, integer or sequence of integers. Specifies which
         positional argument(s) to differentiate with respect to (default ``0``).
       has_aux: Optional, bool. Indicates whether ``fun`` returns a pair where the
         first element is considered the output of the mathematical function to be
         differentiated and the second element is auxiliary data. Default False.
       holomorphic: Optional, bool. Indicates whether ``fun`` is promised to be
         holomorphic. Default False.
@@ -55,15 +113,64 @@
             return y, jac_tree
         else:
             return y, jac_tree, aux
 
     return jacfun
 
 
-def newton_jax(func, init, jac=None, maxit=30, tol=1e-8, sparse=False, solver=None, func_returns_jac=False, inspect_jac=False, verbose=False, verbose_jac=False):
+def jacrev_and_val(fun: Callable, argnums: Union[int, Sequence[int]] = 0,
+                   has_aux: bool = False, holomorphic: bool = False, allow_int: bool = False) -> Callable:
+    """Value and Jacobian of ``fun`` evaluated row-by-row using reverse-mode AD.
+
+    Args:
+      fun: Function whose value and Jacobian are to be computed.
+      argnums: Optional, integer or sequence of integers. Specifies which
+        positional argument(s) to differentiate with respect to (default ``0``).
+      has_aux: Optional, bool. Indicates whether ``fun`` returns a pair where the
+        first element is considered the output of the mathematical function to be
+        differentiated and the second element is auxiliary data. Default False.
+      holomorphic: Optional, bool. Indicates whether ``fun`` is promised to be
+        holomorphic. Default False.
+      allow_int: Optional, bool. Whether to allow differentiating with
+        respect to integer valued inputs. The gradient of an integer input will
+        have a trivial vector-space dtype (float0). Default False.
+
+    Returns:
+      A function with the same arguments as ``fun``, that evaluates the value and Jacobian of
+      ``fun`` using reverse-mode automatic differentiation. If ``has_aux`` is True
+      then a pair of (jacobian, auxiliary_data) is returned.
+    """
+    _check_callable(fun)
+
+    def jacfun(*args, **kwargs):
+        f = lu.wrap_init(fun, kwargs)
+        f_partial, dyn_args = argnums_partial(f, argnums, args,
+                                              require_static_args_hashable=False)
+        tree_map(partial(_check_input_dtype_jacrev,
+                 holomorphic, allow_int), dyn_args)
+        if not has_aux:
+            y, pullback = _vjp(f_partial, *dyn_args)
+        else:
+            y, pullback, aux = _vjp(f_partial, *dyn_args, has_aux=True)
+        tree_map(partial(_check_output_dtype_jacrev, holomorphic), y)
+        jac = vmap(pullback)(_std_basis(y))
+        jac = jac[0] if isinstance(argnums, int) else jac
+        example_args = dyn_args[0] if isinstance(argnums, int) else dyn_args
+        jac_tree = tree_map(partial(_jacrev_unravel, y), example_args, jac)
+        jac_tree = tree_transpose(tree_structure(
+            example_args), tree_structure(y), jac_tree)
+        if not has_aux:
+            return y, jac_tree
+        else:
+            return y, jac_tree, aux
+
+    return jacfun
+
+
+def newton_jax(func, init, jac=None, maxit=30, tol=1e-8, rtol=None, sparse=False, solver=None, func_returns_jac=False, inspect_jac=False, verbose=False, verbose_jac=False):
     """Newton method for root finding using automatic differenciation with jax. The argument `func` must be jittable with jax.
 
     ...
 
     Parameters
     ----------
     func : callable
@@ -94,14 +201,15 @@
     res: dict
         A dictionary of results similar to the output from scipy.optimize.root
     """
 
     st = time.time()
     verbose_jac |= inspect_jac
     verbose |= verbose_jac
+    rtol = rtol or tol
 
     if jac is None and not func_returns_jac:
         if sparse:
             def jac(x): return ssp.csr_array(jax.jacfwd(func)(x))
         else:
             jac = jax.jacfwd(func)
 
@@ -118,17 +226,21 @@
     while True:
 
         xold = xi.copy()
         jacold = jacval.copy() if cnt else None
         cnt += 1
 
         if func_returns_jac:
-            fval, jacval = func(xi)
+            fout = func(xi)
+            fval, jacval, aux = fout if len(fout) == 3 else (*fout, None)
+            if sparse and not isinstance(jacval, ssp._arrays.csr_array):
+                jacval = ssp.csr_array(jacval)
         else:
-            fval, jacval = func(xi), jac(xi)
+            fout, jacval = func(xi), jac(xi)
+            fval, aux = fout if len(fout) == 2 else (fout, None)
 
         jac_is_nan = isnan(jacval.data) if isinstance(
             jacval, ssp._arrays.csr_array) else jnp.isnan(jacval)
         if jac_is_nan.any():
             res['success'] = False
             res['message'] = "The Jacobian contains `NaN`s."
             jacval = jacold if jacold is not None else jacval
@@ -141,15 +253,15 @@
             break
 
         xi -= solver(jacval, fval)
         eps = jnp.abs(xi - xold).max()
 
         if verbose:
             ltime = time.time() - st
-            info_str = f'    Iteration {cnt:3d} | max error {eps:.2e} | lapsed {ltime:3.4f}'
+            info_str = f'    Iteration {cnt:3d} | max. error {eps:.2e} | lapsed {ltime:3.4f}'
             if verbose_jac:
                 jacval = jacval.toarray() if sparse else jacval
                 jacdet = jnp.linalg.det(jacval) if (
                     jacval.shape[0] == jacval.shape[1]) else 0
                 info_str += f' | det {jacdet:1.5g} | rank {jnp.linalg.matrix_rank(jacval)}/{jacval.shape[0]}'
                 if inspect_jac:
                     spy(jacval)
@@ -157,83 +269,89 @@
             print(info_str)
 
         if cnt == maxit:
             res['success'] = False
             res['message'] = f"Maximum number of {maxit} iterations reached."
             break
 
-        if eps < tol:
+        if eps < rtol:
             res['success'] = True
             res['message'] = "The solution converged."
             break
 
         if jnp.isnan(eps):
             res['success'] = False
             res['message'] = f"Function returns 'NaN's"
             break
 
     jacval = jacval.toarray() if isinstance(
-        jacval, ssp._arrays.csr_array) else jacval
+        jacval, (ssp._arrays.csr_array, ssp._arrays.lil_array)) else jacval
 
     res['x'], res['niter'] = xi, cnt
-    res['fun'] = func(xi)[0] if func_returns_jac else func(xi)
-    res['jac'] = jacval
-    res['det'] = jnp.linalg.det(jacval) if (
-        jacval.shape[0] == jacval.shape[1]) else 0
+    res['fun'], res['jac'] = fval, jacval
+    if aux is not None:
+        res['aux'] = aux
+
+    if verbose_jac:
+        # only calculate determinant if requested
+        res['det'] = det(jacval) if (jacval.shape[0] == jacval.shape[1]) else 0
+    else:
+        res['det'] = None
 
     return res
 
 
-def newton_jax_jittable(func, init, jac=None, maxit=30, tol=1e-8):
-    """Newton method for root finding using automatic differenciation with jax BUT running in pure jitted jax. The argument `func` must be jittable with jax. Remember to check the error flags!
-
-    Note that when compiling this function without context, it is necessary to have the function as a static argument. This would imply that AD does not work on functions including a jitted version of this function, which renders jax rather useless. The major advantage of having this function is to include the jittable version (not the jitted one) directly into to-be-jitted code _together with the function for which the root is needed_.
-
+def newton_cond_func(carry):
+    (xi, eps, cnt), (func, verbose, maxit, tol) = carry
+    cond = cnt < maxit
+    cond = jnp.logical_and(cond, eps > tol)
+    cond = jnp.logical_and(cond, ~jnp.isnan(eps))
+    verbose = jnp.logical_and(cnt, verbose)
+    jax.debug.callback(callback_func, cnt, eps, verbose=verbose)
+    return cond
+
+
+def newton_body_func(carry):
+    (xi, eps, cnt), (func, verbose, maxit, tol) = carry
+    xi_old = xi
+    f, jac = func(xi)
+    xi -= jax.scipy.linalg.solve(jac, f)
+    eps = amax(xi-xi_old)
+    return (xi, eps, cnt+1), (func, verbose, maxit, tol)
+
+
+def callback_func(cnt, err, dampening=None, ltime=None, verbose=True):
+    mess = f'    Iteration {cnt:3d} | max. error {err:.2e}'
+    if dampening is not None:
+        mess += f' | dampening {dampening:1.3f}'
+    if ltime is not None:
+        mess += f' | lapsed {ltime:3.4f}s'
+    if verbose:
+        print(mess)
+
+
+@jax.jit
+def newton_jax_jit(func, x_init, maxit=30, tol=1e-8, verbose=True):
+    """Newton method for root finding using automatic differentiation with jax and running in jitted jax.
     ...
 
     Parameters
     ----------
     func : callable
-        Function f for which f(x)=0 should be found. Must be jittable with jax
-    init : array
+        Function returning (y, jac) where f(x)=y=0 should be found and jac is the jacobian. Must be jittable with jax. Could e.g. be the output of jacfwd_and_val.
+    x_init : array
         Initial values of x
-    jac : callable, optional
-        Funciton that returns the jacobian. If not provided, jax.jacfwd is used
     maxit : int, optional
         Maximum number of iterations
     tol : float, optional
         Random seed. Defaults to 0
 
     Returns
     -------
-    res: (xopt, fopt, niter, success)
+    res: (xopt, (fopt, jacopt), niter, success)
     """
-
-    if jac is None:
-        jac = jax.jacfwd(func)
-
-    xi = jnp.array(init)
-
-    def cond_func(tain):
-        xi, xold, cnt = tain
-        eps = jnp.abs(xi - xold).max()
-
-        cond = cnt < maxit
-        cond &= eps > tol
-        cond &= ~jnp.isnan(eps)
-
-        return cond
-
-    def body_func(tain):
-        (xi, _, cnt) = tain
-        cnt += 1
-        xold = xi
-        xi -= jax.scipy.linalg.solve(jac(xi), func(xi))
-        return (xi, xold, cnt)
-
-    tain = jax.lax.while_loop(cond_func, body_func, (xi, xi + 1, 0))
-    eps = jnp.abs(tain[0] - tain[1]).max()
-
-    return tain[0], func(tain[0]), tain[2], eps < tol
+    (xi, eps, cnt), _ = jax.lax.while_loop(newton_cond_func,
+                                           newton_body_func, ((x_init, 1., 0), (func, verbose, maxit, tol)))
+    return xi, func(xi), cnt, eps > tol
 
 
-newton_jax_jit = jax.jit(newton_jax_jittable, static_argnums=(0, 2, 3, 4))
+amax = jax.jit(lambda x: jnp.abs(x).max())
```

### Comparing `grgrlib-0.1.9/grgrlib/legacy.py` & `grgrlib-0.2.0/grgrlib/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 """
 this file contains functions that are not activly developed anymore and only provided for reproducibility purposes
 """
 
 
 def tmcmc(
```

### Comparing `grgrlib-0.1.9/grgrlib/multiprocessing.py` & `grgrlib-0.2.0/grgrlib/multiprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 import dill
 from sys import platform
 
 
 def serializer_unix(func):
     """Dirty hack that transforms the non-serializable function to a serializable one (when using dill)
```

### Comparing `grgrlib-0.1.9/grgrlib/numerics.py` & `grgrlib-0.2.0/grgrlib/numerics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
+from .__pycache__.chebychev import chebychev
 import os
 
 CHEBY_RANGE = 12
 
 
 def chebystr(k):
     if k == 0:
         return 'np.ones_like(x)'
     elif k == 1:
         return 'x'
     else:
-        return '2*x*(%s) - (%s)' %(chebystr(k-1),chebystr(k-2))
+        return '2*x*(%s) - (%s)' % (chebystr(k-1), chebystr(k-2))
+
 
-rows = "\n ".join([f"if order == {i}:\n  return %s" %chebystr(i) for i in range(CHEBY_RANGE)])
+rows = "\n ".join([f"if order == {i}:\n  return %s" %
+                  chebystr(i) for i in range(CHEBY_RANGE)])
 chebyfactory = """
 from numba import njit\n
 import numpy as np\n
 @njit(cache=True)\n
 def chebychev(order, x):\n %s\n else:\n  print('order not implemented')
-""" %rows
+""" % rows
 
 pth = os.path.dirname(__file__)
 cache_path = os.path.join(pth, '__pycache__', 'chebychev.py')
 
 try:
-    cache_file  = open(cache_path, "r")
+    cache_file = open(cache_path, "r")
     content = cache_file.read()
     cache_file.close()
     assert content == chebyfactory
 except:
-    cache_file  = open(cache_path, "w")
+    cache_file = open(cache_path, "w")
     cache_file.write(chebyfactory)
     cache_file.close()
-
-from .__pycache__.chebychev import chebychev
-
```

### Comparing `grgrlib-0.1.9/grgrlib/optimize.py` & `grgrlib-0.2.0/grgrlib/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import time
 import numpy as np
-from grgrlib import map2arr
+from .generic import map2arr
 
 try:
     import chaospy
 
     chaospy_loaded = True
 except ModuleNotFoundError:
     chaospy_loaded = False
@@ -52,15 +51,16 @@
     -----
     The CMA-ES algoritm is not optimized for large populations. In particular, it might get stuck or just not converge. One way to avoid explosion of the covariance for large populations is to manually set the parameter `cs` (very) close to zero. Another way is to reduce `mu` to only update using a few top-samples. This is automatically done if you set the `scaled` option to `True`. Note that doing so might have other disadvantages. If you prefer tighter selecton of only the best sample without reducing the size of the cov update, you can reduce `mu_mean`, which is the size of the offspring vector for the mean only.
 
     All in all, this is a powerful method which, due to its heuristic nature, requires quite some tweaking at times.
 
     """
 
-    es = CMAES(xstart, sigma, popsize=popsize, biject=biject, verbose=verbose, **args)
+    es = CMAES(xstart, sigma, popsize=popsize,
+               biject=biject, verbose=verbose, **args)
 
     es.bfunc = (lambda x: 1 / (1 + np.exp(x))) if biject else (lambda x: x)
     es.objective_fct = lambda x: objective_fct(es.bfunc(x))
 
     es.map = mapper or map
     es.stime = time.time()
 
@@ -146,15 +146,16 @@
         def_pop = 4 + int(3 * np.log(ndim))
         self.lam = popsize or def_pop
 
         mu = int(def_pop / 2.0) if scaled else mu
         # set number of parents/points/solutions for recombination
         self.mu = int(mu or (self.lam / 2))
 
-        self.maxfev = maxfev or 100 * self.lam + 150 * (ndim + 3) ** 2 * self.lam ** 0.5
+        self.maxfev = maxfev or 100 * self.lam + \
+            150 * (ndim + 3) ** 2 * self.lam ** 0.5
 
         if active is None:
             active = False if scaled else True
 
         if active:
             self.weights, self.mueff = self.recombination_weights()
         else:
@@ -175,15 +176,16 @@
         if mu_mean:
             weights_mean = np.zeros(self.lam)
             weights_mean[: self.mu_mean] = (
                 np.log(self.lam + 1)
                 - np.log(np.arange(self.mu_mean) + 1)
                 - np.log(self.lam / self.mu_mean)
             )
-            self.weights_mean = weights_mean / np.sum(weights_mean[: self.mu_mean])
+            self.weights_mean = weights_mean / \
+                np.sum(weights_mean[: self.mu_mean])
         else:
             self.weights_mean = self.weights
 
         # set strategy parameter adaptation:
         # set time constant for cumulation for COV
         def_cc = (4 + self.mueff / ndim) / (ndim + 4 + 2 * self.mueff / ndim)
         self.cc = def_cc if cc is None else cc
@@ -195,15 +197,16 @@
         # define learning rate of rank-one update
         def_c1 = 2 / ((ndim + 1.3) ** 2 + self.mueff)
         self.c1 = def_c1 if c1 is None else c1
 
         # define learning rate of rank-mu update
         def_cmu = np.minimum(
             1 - self.c1,
-            2 * (self.mueff - 2 + 1 / self.mueff) / ((ndim + 2) ** 2 + self.mueff),
+            2 * (self.mueff - 2 + 1 / self.mueff) /
+            ((ndim + 2) ** 2 + self.mueff),
         )
         self.cmu = def_cmu if cmu is None else cmu
 
         # define damping for sigma (usually close to 1)
         self.damps = self.mueff / self.mu + 0.3 + self.cs
 
         if active:
@@ -261,36 +264,37 @@
 
         if self.weights[-1] < 0:
             if self.cmu > 0:
 
                 value = np.abs(1 + self.c1 / self.cmu)
 
                 if self.weights[-1] < 0:
-                    factor = np.abs(value / np.sum(self.weights[self.mu :]))
-                    self.weights[self.mu :] *= factor
+                    factor = np.abs(value / np.sum(self.weights[self.mu:]))
+                    self.weights[self.mu:] *= factor
 
                 value = np.abs((1 - self.c1 - self.cmu) / self.cmu / self.ndim)
 
                 # if nothing to limit
-                if np.sum(self.weights[self.mu :]) < -value:
-                    factor = np.abs(value / np.sum(self.weights[self.mu :]))
+                if np.sum(self.weights[self.mu:]) < -value:
+                    factor = np.abs(value / np.sum(self.weights[self.mu:]))
                     if factor < 1:
-                        self.weights[self.mu :] *= factor
+                        self.weights[self.mu:] *= factor
 
-            sum_neg = np.sum(self.weights[self.mu :])
+            sum_neg = np.sum(self.weights[self.mu:])
             mueffminus = (
-                sum_neg ** 2 / np.sum(self.weights[self.mu :] ** 2) if sum_neg else 0
+                sum_neg ** 2 /
+                np.sum(self.weights[self.mu:] ** 2) if sum_neg else 0
             )
             value = np.abs(1 + 2 * mueffminus / (self.mueff + 2))
 
             # if nothing to limit
             if sum_neg < -value:
                 factor = np.abs(value / sum_neg)
                 if factor < 1:
-                    self.weights[self.mu :] *= factor
+                    self.weights[self.mu:] *= factor
 
         return
 
 
 class CMAES(object):
     def __init__(self, xstart, sigma, popsize, biject, verbose, **args):
 
@@ -368,15 +372,15 @@
         xs = xs[fs.argsort()]
         self.fs = np.sort(fs)
         self.xs = xs
 
         self.best.update(xs[0], self.fs[0], self.counteval)
 
         # compute new weighted mean value via recombination
-        self.xmean = xs[0 : par.mu_mean].T @ par.weights_mean[: par.mu_mean]
+        self.xmean = xs[0: par.mu_mean].T @ par.weights_mean[: par.mu_mean]
 
         # update evolution paths via cumulation:
         y = self.xmean - xold
         z = self.invsqrt @ y
         csn = (par.cs * (2 - par.cs) * par.mueff) ** 0.5 / self.sigma
         # update evolution path
         self.ps = (1 - par.cs) * self.ps + csn * z
@@ -402,15 +406,16 @@
         # rank-mu update
         for k, wk in enumerate(par.weights):
             # guaranty positive definiteness
             if wk < 0:
                 mahalano = np.sum((self.invsqrt @ (xs[k] - xold)) ** 2)
                 wk *= N * self.sigma ** 2 / mahalano
             self.C += (
-                wk * par.cmu / self.sigma ** 2 * np.outer(xs[k] - xold, xs[k] - xold)
+                wk * par.cmu / self.sigma ** 2 *
+                np.outer(xs[k] - xold, xs[k] - xold)
             )
 
         # adapt step-size
         cn, sum_square_ps = par.cs / par.damps, np.sum(self.ps ** 2)
         self.sigma *= np.exp(np.minimum(1, cn * (sum_square_ps / N - 1) / 2))
 
     def stop(self):
```

### Comparing `grgrlib-0.1.9/grgrlib/plots.py` & `grgrlib-0.2.0/grgrlib/plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 from matplotlib.ticker import MaxNLocator
 from matplotlib.colors import LogNorm, SymLogNorm
 
+try:
+    import pandas as pd
+except ModuleNotFoundError:
+    pd = None
+
 
 def grplot(
     X,
     xscale=None,
     labels=None,
     title="",
     styles=None,
@@ -32,26 +35,26 @@
         # make it a tuple
         X = (X,)
 
     # use first object in X to get some infos
     X0 = np.array(X[0])
 
     if xscale is None:
-        if isinstance(X[0], pd.DataFrame):
+        if pd is not None and isinstance(X[0], pd.DataFrame):
             xscale = X[0].index
         elif X0.ndim > 1:
             xscale = np.arange(X[0].shape[-2])
         else:
             xscale = np.arange(len(X0))
     elif isinstance(xscale, tuple):
         xscale = np.arange(xscale[0], xscale[0] +
                            X0.shape[-2] * xscale[1], xscale[1])
 
     if labels is None:
-        if isinstance(X[0], pd.DataFrame):
+        if pd is not None and isinstance(X[0], pd.DataFrame):
             labels = np.array(X[0].keys())
         elif X0.shape[-1] > 1 and X0.ndim > 1:
             labels = np.arange(X0.shape[-1]) + 1
         else:
             labels = np.array([None])
     else:
         labels = np.ascontiguousarray(labels)
@@ -101,18 +104,18 @@
                 )
                 line = stat(x, axis=0)
             else:
                 bulk = x
 
         # check if there are states that are always zero
         if line is not None:
-            selector += np.nanstd(line, 0) > tol
+            selector += np.nanstd(line, 0) >= tol
         if interval is not None:
-            selector += np.nanstd(interval[0], 0) > tol
-            selector += np.nanstd(interval[1], 0) > tol
+            selector += np.nanstd(interval[0], 0) >= tol
+            selector += np.nanstd(interval[1], 0) >= tol
         if bulk is not None:
             selector[:] = 1
 
         X_list.append((line, interval, bulk))
 
     colors = colors or [None] * len(X_list)
     if isinstance(colors, str):
@@ -159,15 +162,15 @@
         try:
             len(ax)
         except TypeError:
             ax = (ax,)
         [axis.set_prop_cycle(None) for axis in ax]
         figs = fig or None
 
-    if not isinstance(xscale, pd.DatetimeIndex):
+    if pd is not None and not isinstance(xscale, pd.DatetimeIndex):
         locator = MaxNLocator(nbins=nlocbins, steps=[1, 2, 4, 8, 10])
 
     handles = []
     for obj_no, obj in enumerate(X_list):
 
         if legend is not None:
             legend_tag = np.ascontiguousarray(legend)[obj_no]
@@ -222,15 +225,15 @@
                 color = colors[obj_no] or "maroon"
 
                 ax[i].plot(
                     xscale, bulk[..., i].swapaxes(0, 1), c=color, alpha=alpha or 0.05
                 )
             ax[i].tick_params(axis="both", which="both",
                               top=False, right=False)
-            if not isinstance(xscale, pd.DatetimeIndex):
+            if pd is not None and not isinstance(xscale, pd.DatetimeIndex):
                 ax[i].xaxis.set_major_locator(locator)
 
         handles.append(subhandles)
 
     if figs is not None:
         [fig.autofmt_xdate() for fig in figs]
 
@@ -360,15 +363,15 @@
     fig_exists = False
 
     if ax is None:
         fig_exists = True
         frc = max(min(s0 / s1, 2), 0.5)
         fig, ax = plt.subplots(1, 1, figsize=(5 + 2 / frc, frc * 5 + 2))
 
-    ax.imshow(np.log10(1e-15 + np.abs(M)), cmap=cmap)
+    ax.imshow(np.log10(1e-15 + np.abs(M)), cmap=cmap, aspect='auto')
 
     if fig_exists:
         fig.tight_layout()
         return fig, ax
 
     return ax
 
@@ -389,61 +392,53 @@
     bounds,
     xlabel=None,
     ylabel=None,
     zlabel=None,
     ax=None,
     draw_colorbar=None,
     cmap=None,
+    **kwargs
 ):
     """Simple interface to a heatmap (uses matplotlib's `imshow`).
 
     Parameters
     ----------
     X : numpy.array
         a matrix-like object
     bounds : float or tuple
         the bounds of the grid. If a float, -/+ this value is taken as the bounds
     xlabel : str (optional)
     ylabel : str (optional)
     zlabel : str (optional)
+    ax : array (optional)
+    draw_colorbar : bool (optional)
+    cmap : matplotlib colormap (optional)
+    kwargs : any argument passet forward to imshow
     """
 
     draw_colorbar = True if draw_colorbar is None else draw_colorbar
     cmap = "hot" if cmap is None else cmap
 
     if ax is None:
         fig, ax = plt.subplots()
     else:
         fig = None
 
     if isinstance(bounds, tuple):
         if isinstance(bounds[0], tuple):
-            extent = [
-                *bounds[0],
-                *bounds[1],
-            ]
+            extent = [*bounds[0], *bounds[1]]
         else:
-            extent = [
-                bounds[0],
-                bounds[1],
-                bounds[0],
-                bounds[1],
-            ]
+            extent = [bounds[0], bounds[1], bounds[0], bounds[1]]
     elif isinstance(bounds, (float, int)):
-        extent = [
-            -bounds,
-            bounds,
-            -bounds,
-            bounds,
-        ]
+        extent = [-bounds, bounds, -bounds, bounds]
     else:
         extent = bounds
 
     img = ax.imshow(X, cmap=cmap, extent=extent,
-                    vmin=np.nanmin(X), vmax=np.nanmax(X))
+                    vmin=np.nanmin(X), vmax=np.nanmax(X), aspect='auto', origin='lower', **kwargs)
 
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.grid(False)
 
     if draw_colorbar:
         clb = plt.colorbar(img, ax=ax)
@@ -476,31 +471,39 @@
     dz = hist.ravel()
 
     ax.bar3d(xpos, ypos, zpos, dx, dy, dz, zsort='average', alpha=alpha)
 
     return ax, (xedges, yedges)
 
 
-def grbar3d(x, bounds=None, xedges=None, yedges=None, width=1, depth=1, ax=None, figsize=None, **kwargs):
+def grbar3d(x, bounds=None, xedges=None, yedges=None, width=1, depth=1, colors=None, cmap=None, ax=None, figsize=None, unset_pane_color=True, **kwargs):
 
     if ax is None:
         fig = plt.figure(figsize=figsize)
         ax = fig.add_subplot(projection='3d')
 
     xedges = np.linspace(*bounds[0], x.shape[0]) if xedges is None else xedges
     yedges = np.linspace(*bounds[1], x.shape[1]) if yedges is None else yedges
+    cmap = plt.cm.magma if cmap is None else cmap
+    colors = cmap((x.flatten() - x.min())/(x.max() - x.min())
+                  ) if colors is None else colors
 
     # xpos, ypos = np.meshgrid(xedges, yedges)
     xpos, ypos = np.meshgrid(xedges, yedges, indexing="ij")
     xpos = xpos.ravel()
     ypos = ypos.ravel()
     zpos = np.zeros_like(x.ravel())
 
     dx = dy = 0.5 * np.ones_like(zpos)
     dz = x.ravel()
 
-    ax.bar3d(xpos, ypos, zpos, width, depth, dz, shade=True, **kwargs)
+    ax.bar3d(xpos, ypos, zpos, width, depth, dz,
+             shade=True, color=colors, **kwargs)
+    if unset_pane_color:
+        ax.xaxis.set_pane_color((1.0, 1.0, 1.0, 1.0))
+        ax.yaxis.set_pane_color((1.0, 1.0, 1.0, 1.0))
+        ax.zaxis.set_pane_color((1.0, 1.0, 1.0, 1.0))
 
     return ax, (xedges, yedges)
 
 
 pplot = grplot
```

### Comparing `grgrlib-0.1.9/grgrlib/stats.py` & `grgrlib-0.2.0/grgrlib/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,11 @@
-#!/bin/python
 # -*- coding: utf-8 -*-
 
 import numpy as np
-from numba import njit
-
-_cond = 1e-9
-
-
-@njit(cache=True)
-def psd_func(M):
-    """Compute the symmetric eigendecomposition
-
-    Note that eigh takes care of array conversion, chkfinite, and assertion that the matrix is square.
-    """
-
-    s, u = np.linalg.eigh(M)
-    eps = _cond * np.max(np.abs(s))
-    d = s[s > eps]
-
-    s_pinv = [0 if abs(x) <= eps else 1 / x for x in s]
-    s_pinv_np = np.array(s_pinv)
-    U = np.multiply(u, np.sqrt(s_pinv_np))
-
-    return U, np.sum(np.log(d)), len(d)
-
-
-@njit(cache=True)
-def mvn_logpdf(x, mean, cov):
-    """log-PDF of multivariate normal"""
-
-    _LOG_2PI = np.log(2 * np.pi)
-
-    dim = mean.shape[0]
-    prec_U, log_det_cov, rank = psd_func(cov)
-    dev = x - mean
-    maha = np.sum(np.square(np.dot(dev, prec_U)), axis=-1)
-    out = -0.5 * (rank * _LOG_2PI + log_det_cov + maha)
-
-    return out
+from .njitted import mvn_logpdf, normal_pdf, normal_cdf
 
 
 def percentile(x, q=0.01):
     """Find share owned by q richest individuals"""
 
     xsort = np.sort(x)
     n = len(x)
@@ -125,10 +89,7 @@
     density = convolve(grid, kernel, mode="same")[npad: npad + nx]
 
     norm_factor = n * dx * (2 * np.pi * std_x ** 2 * scotts_factor ** 2) ** 0.5
 
     density = density / norm_factor
 
     return density, xmin, xmax
-
-
-logpdf = mvn_logpdf  # for legacy reasons
```

### Comparing `grgrlib-0.1.9/grgrlib.egg-info/PKG-INFO` & `grgrlib-0.2.0/grgrlib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: grgrlib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Various insanely helpful functions
 Home-page: https://github.com/gboehl/grgrlib
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: njitted
+Provides-Extra: jaxed
+Provides-Extra: opti
+Provides-Extra: data
 License-File: LICENSE
 
 
 grgrlib
 =======
 
-This is a library of unspeakably (hence the name) useful functions. It serves as a container for functions shared across other projects. 
+This is a library of unspeakably useful functions. It serves as a container for a rather loose collection of tools shared across other projects that may or may not be individually useful. 
 
 Installation with ``pip``
 -----------------------------
 
-It's as simple as:
+It's as simple as typing
 
 .. code-block:: bash
 
    pip install grgrlib
 
+in the terminal (Unix/Mac) or the Anaconda Prompt (Win).
 
 Installation of bleeding-edge version using ``git``
 ---------------------------------------------------
 
 The handy way is to first install ``git``. Linux users just use their respective repos. Look into `this repo <https://github.com/gboehl/pydsge/blob/master/README.rst>`_ for details.
 
 .. code-block:: bash
@@ -39,9 +43,7 @@
    pip install git+https://github.com/gboehl/grgrlib
 
 Alternatively you can clone the repository and then from within the cloned folder run (Windows user from the Anaconda Prompt):
 
 .. code-block:: bash
 
    pip install .
-
-
```

### Comparing `grgrlib-0.1.9/grgrlib.egg-info/SOURCES.txt` & `grgrlib-0.2.0/grgrlib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.rst
+requirements.txt
 setup.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/indices.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/_static/css/custom.css
 grgrlib/__init__.py
+grgrlib/__version__.py
 grgrlib/datatools.py
 grgrlib/dist.py
 grgrlib/econtools.py
 grgrlib/generic.py
 grgrlib/h5.py
+grgrlib/hanktools.py
 grgrlib/jaxed.py
 grgrlib/legacy.py
 grgrlib/linalg.py
 grgrlib/multiprocessing.py
 grgrlib/njitted.py
 grgrlib/numerics.py
 grgrlib/optimize.py
```

### Comparing `grgrlib-0.1.9/setup.py` & `grgrlib-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from setuptools import setup, find_packages
 from os import path
 
+# get version from dedicated version file
+version = {}
+with open("grgrlib/__version__.py") as fp:
+    exec(fp.read(), version)
+
 # read the contents of the README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/gboehl/grgrlib",
     name='grgrlib',
-    version='0.1.9',
+    version=version['__version__'],
     author='Gregor Boehl',
     author_email='admin@gregorboehl.com',
     license='MIT',
     description='Various insanely helpful functions',
     classifiers=[
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.9",
     ],
     packages=find_packages(),
+    extras_require={
+        'njitted': ['numba'],
+        'jaxed': ['jax', 'jaxlib'],
+        'opti': ['chaospy'],
+        'data': ['pandas'],
+    },
     install_requires=[
-        'sympy',
+        'numpy',
         'scipy',
-        'pathos',
         'matplotlib',
-        'numpy',
-        'numba',
-        'pandas'
     ],
     include_package_data=True,
 )
```

