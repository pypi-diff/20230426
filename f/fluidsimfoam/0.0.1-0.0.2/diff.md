# Comparing `tmp/fluidsimfoam-0.0.1.tar.gz` & `tmp/fluidsimfoam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsimfoam-0.0.1.tar", max compression
+gzip compressed data, was "fluidsimfoam-0.0.2.tar", max compression
```

## Comparing `fluidsimfoam-0.0.1.tar` & `fluidsimfoam-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,41 @@
--rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.1/LICENSE
--rw-r--r--   0        0        0     1760 2023-03-07 21:43:14.042015 fluidsimfoam-0.0.1/README.md
--rw-r--r--   0        0        0     1174 2023-03-09 20:43:08.717722 fluidsimfoam-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1385 2023-03-09 20:44:10.802711 fluidsimfoam-0.0.1/src/fluidsimfoam/__init__.py
--rw-r--r--   0        0        0     1004 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.1/src/fluidsimfoam/info.py
--rw-r--r--   0        0        0      737 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.1/src/fluidsimfoam/log.py
--rw-r--r--   0        0        0     1115 2023-03-09 20:43:08.717722 fluidsimfoam-0.0.1/src/fluidsimfoam/next_fluidsim_core.py
--rw-r--r--   0        0        0       25 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.1/src/fluidsimfoam/output/__init__.py
--rw-r--r--   0        0        0      193 2023-03-02 21:06:12.233495 fluidsimfoam-0.0.1/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6000 2023-03-09 21:09:52.414381 fluidsimfoam-0.0.1/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     6640 2023-03-09 21:09:31.188386 fluidsimfoam-0.0.1/src/fluidsimfoam/output/base.py
--rw-r--r--   0        0        0     2263 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/U.jinja
--rw-r--r--   0        0        0      497 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/__init__.py
--rw-r--r--   0        0        0      870 2023-03-09 20:43:42.985533 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2020 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/blockMeshDict.jinja
--rw-r--r--   0        0        0     1619 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/controlDict.jinja
--rw-r--r--   0        0        0     1371 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/fvSchemes.jinja
--rw-r--r--   0        0        0     1481 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/fvSolution.jinja
--rw-r--r--   0        0        0     2145 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/p.jinja
--rw-r--r--   0        0        0      949 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/transportProperties.jinja
--rw-r--r--   0        0        0      871 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/resources/turbulenceProperties.jinja
--rw-r--r--   0        0        0     2658 2023-03-09 20:42:59.455925 fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/__init__.py
--rw-r--r--   0        0        0     2569 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2443 2023-03-09 21:09:52.222620 fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3358 2023-03-09 21:02:37.197363 fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/base.py
--rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.1/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
--rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.1/src/fluidsimfoam/util/console.py
--rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.1/setup.py
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-03-02 21:01:46.291446 fluidsimfoam-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2121 2023-04-26 15:04:34.458125 fluidsimfoam-0.0.2/README.md
+-rw-r--r--   0        0        0     1348 2023-04-26 13:27:25.261100 fluidsimfoam-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1807 2023-04-26 14:23:21.793720 fluidsimfoam-0.0.2/src/fluidsimfoam/__init__.py
+-rw-r--r--   0        0        0     1396 2023-04-26 14:37:40.374320 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__init__.py
+-rw-r--r--   0        0        0     1479 2023-04-26 14:37:42.998294 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12515 2023-04-21 00:50:26.088622 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/ast.cpython-310.pyc
+-rw-r--r--   0        0        0     4172 2023-04-26 12:06:21.876324 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0        0        0    10425 2023-04-20 19:59:36.408013 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0    11079 2023-04-21 00:50:23.720680 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/ast.py
+-rw-r--r--   0        0        0     1080 2023-04-23 15:48:42.099657 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/LICENSE
+-rw-r--r--   0        0        0    13165 2023-04-26 14:48:53.674766 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__init__.py
+-rw-r--r--   0        0        0    14349 2023-04-26 14:48:56.026761 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2350 2023-04-24 21:00:37.401533 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3091 2023-04-24 20:58:19.530657 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/__pycache__/grading.cpython-310.pyc
+-rw-r--r--   0        0        0     1810 2023-04-24 21:00:31.761612 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/edges.py
+-rw-r--r--   0        0        0     3426 2023-04-24 20:58:16.942659 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/blockmeshhelper/grading.py
+-rw-r--r--   0        0        0     3702 2023-04-26 12:06:20.328322 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/generators.py
+-rw-r--r--   0        0        0     1918 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar.lark
+-rw-r--r--   0        0        0     2335 2023-04-18 19:23:17.863337 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/grammar_advanced.lark
+-rw-r--r--   0        0        0     9483 2023-04-20 19:59:34.795586 fluidsimfoam-0.0.2/src/fluidsimfoam/foam_input_files/parser.py
+-rw-r--r--   0        0        0     1283 2023-04-26 12:46:10.782261 fluidsimfoam-0.0.2/src/fluidsimfoam/info.py
+-rw-r--r--   0        0        0       70 2023-04-26 12:56:51.898012 fluidsimfoam-0.0.2/src/fluidsimfoam/init_fields.py
+-rw-r--r--   0        0        0      737 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.2/src/fluidsimfoam/log.py
+-rw-r--r--   0        0        0      310 2023-04-20 19:12:16.643975 fluidsimfoam-0.0.2/src/fluidsimfoam/make.py
+-rw-r--r--   0        0        0     1115 2023-03-09 20:43:08.717722 fluidsimfoam-0.0.2/src/fluidsimfoam/next_fluidsim_core.py
+-rw-r--r--   0        0        0      208 2023-04-26 13:04:37.103178 fluidsimfoam-0.0.2/src/fluidsimfoam/operators.py
+-rw-r--r--   0        0        0       25 2023-03-02 21:01:46.299445 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__init__.py
+-rw-r--r--   0        0        0      193 2023-03-02 21:06:12.233495 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9044 2023-04-26 13:42:10.597508 fluidsimfoam-0.0.2/src/fluidsimfoam/output/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0    10986 2023-04-26 13:42:06.101527 fluidsimfoam-0.0.2/src/fluidsimfoam/output/base.py
+-rw-r--r--   0        0        0      497 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.2/src/fluidsimfoam/resources/__init__.py
+-rw-r--r--   0        0        0      870 2023-03-09 20:43:42.985533 fluidsimfoam-0.0.2/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2759 2023-04-26 14:14:21.141790 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__init__.py
+-rw-r--r--   0        0        0     2614 2023-04-26 14:14:23.597814 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1642 2023-04-21 01:35:51.333383 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1683 2023-04-21 01:35:47.023225 fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/base.py
+-rw-r--r--   0        0        0      592 2023-04-21 18:34:01.041339 fluidsimfoam-0.0.2/src/fluidsimfoam/tasks.py
+-rw-r--r--   0        0        0     1145 2023-03-09 20:43:42.785643 fluidsimfoam-0.0.2/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc
+-rw-r--r--   0        0        0      861 2023-03-09 20:43:08.721719 fluidsimfoam-0.0.2/src/fluidsimfoam/util/console.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 fluidsimfoam-0.0.2/PKG-INFO
```

### Comparing `fluidsimfoam-0.0.1/LICENSE` & `fluidsimfoam-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/README.md` & `fluidsimfoam-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+<div align="center">
+
 # Fluidsimfoam
 
+[![PyPI](https://img.shields.io/pypi/v/fluidsimfoam)](https://pypi.org/project/fluidsimfoam/)
+[![Documentation Status](https://readthedocs.org/projects/fluidsimfoam/badge/?version=latest)](https://fluidsimfoam.readthedocs.io/en/latest/?badge=latest)
+
 <!-- badges -->
 
 Python framework for [OpenFOAM]
 
+</div>
+
 Fluidsimfoam is a Python package which **will** allow one to write [Fluidsim]
 solvers based for the simulations on the C++ CFD code [OpenFOAM]. There
 **will** be open-source solvers (in particular fluidsimfoam-phill and
 fluidsimfoam-tgv) and it **will** not be difficult to write your own solver
 based on your [OpenFOAM] cases.
 
 With a Fluidsimfoam solver, it **will** becomes very easy to
@@ -15,26 +22,29 @@
 - launch/restart simulations with Python scripts and terminal commands,
 - load simulations, read the associated parameters/data and produce nice figures/movies.
 
 Fluidsimfoam can be seen as a workflow manager for [OpenFOAM] or a Python
 wrapper around [OpenFOAM]. It uses [OpenFOAM] on the background and is thus NOT
 a rewrite of [OpenFOAM]!
 
-Fluidsimfoam is now in very early development. The goal is to get the
+Fluidsimfoam is now in early development. The goal is to get the
 equivalent of [Snek5000], our Fluidsim framework for [Nek5000].
 
-## Related projects
+We currently target OpenFOAM v2206. See more in [Fluidsimfoam
+documentation](https://fluidsimfoam.readthedocs.org).
 
-- [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
-  [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
-  OpenFOAM. GNU GPL. Still maintained. Should be used by Fluidsimfoam.
+## Related projects
 
 - [Fluidfoam] Another Fluiddyn package (like Fluidsimfoam) to use/plot OpenFOAM
   data. Will be used by Fluidsimfoam.
 
+- [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
+  [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
+  OpenFOAM. GNU GPL. Still maintained.
+
 - [PythonFlu] ([wiki](https://openfoamwiki.net/index.php/Contrib_pythonFlu))
 
 - [Swak4Foam]
 
 [PyFoam]: https://openfoamwiki.net/index.php/Contrib/PyFoam
 [fluidsim]: https://fluidsim.readthedocs.io
 [fluidfoam]: https://fluidfoam.readthedocs.io
```

### Comparing `fluidsimfoam-0.0.1/pyproject.toml` & `fluidsimfoam-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 [tool.poetry]
 name = "fluidsimfoam"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python framework for OpenFOAM"
 authors = ["pierre.augier <pierre.augier@univ-grenoble-alpes.fr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fluidsim-core = "^0.7.2"
 inflection = "^0.5.1"
 fluiddyn = "^0.5.2"
 ipython = "^8.11.0"
 pandas = "^1.5.3"
 jinja2 = "^3.1.2"
+lark = "^1.1.5"
+rich = "^13.3.3"
+invoke = "^2.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 fluidsimfoam-tgv = { path = "./doc/examples/fluidsimfoam-tgv/", develop = true }
+fluidsimfoam-cbox = { path = "./doc/examples/fluidsimfoam-cbox/", develop = true }
 pytest-mock = "^3.10.0"
+pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
+ipdb = "^0.13.13"
 
 [tool.poetry.group.doc.dependencies]
 myst-nb = "^0.17.1"
 sphinx-inline-tabs = "^2022.1.2b11"
 sphinx-copybutton = "^0.5.1"
 pydata-sphinx-theme = "^0.13.1"
```

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/__init__.py` & `fluidsimfoam-0.0.2/src/fluidsimfoam/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+"""
+Fluidsimfoam API reference
+
+.. rubric:: Sub-packages
+
+.. autosummary::
+   :toctree:
+
+   foam_input_files
+   output
+   resources
+   solvers
+   util
+
+.. rubric:: Modules
+
+.. autosummary::
+   :toctree:
+
+   info
+   init_fields
+   log
+   make
+   next_fluidsim_core
+   operators
+   tasks
+
+"""
 import importlib.metadata
 
 from fluidsim_core.params import Parameters
 
 from .next_fluidsim_core import path_try_from_fluidsim_path
 
 __version__ = importlib.metadata.version(__package__ or __name__)
@@ -22,15 +50,19 @@
     from fluidsimfoam.solvers import get_solver_short_name, import_cls_simul
 
     path_dir = path_try_from_fluidsim_path(path_dir)
 
     short_name = get_solver_short_name(path_dir)
     Simul = import_cls_simul(short_name)
 
-    params = Parameters(path_file=path_dir / "params_simul.xml")
+    path_params = path_dir / "params_simul.xml"
+    if not path_params.exists():
+        path_params = path_dir / ".data_fluidsim/params_simul.xml"
+
+    params = Parameters(path_file=path_params)
 
     # Modify parameters prior to loading
     params.NEW_DIR_RESULTS = False
     params.output.HAS_TO_SAVE = False
     params.path_run = path_dir
 
     return Simul(params)
```

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/log.py` & `fluidsimfoam-0.0.2/src/fluidsimfoam/log.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/next_fluidsim_core.py` & `fluidsimfoam-0.0.2/src/fluidsimfoam/next_fluidsim_core.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.2/src/fluidsimfoam/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/__init__.py` & `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Solver framework
 
 .. autosummary::
    :toctree:
 
    base
-   kth
 
 """
 
 import importlib
 from functools import partial
 from pkgutil import ModuleInfo
 from types import ModuleType
@@ -95,14 +94,17 @@
 
     Returns
     -------
     short_name: str
 
     """
     info_solver_xml = path_dir / "info_solver.xml"
+    if not info_solver_xml.exists():
+        info_solver_xml = path_dir / ".data_fluidsim/info_solver.xml"
+
     if info_solver_xml.exists():
         info_solver = InfoSolverCore(path_file=info_solver_xml)
         short_name = info_solver.short_name
     else:
         logger.warning(
             f"The {info_solver_xml} file is missing! "
             "Attempting to guess solver from the directory name."
```

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc` & `fluidsimfoam-0.0.2/src/fluidsimfoam/solvers/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar  9 20:42:59 2023 UTC, .py size: 2658 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,161 +1,164 @@
-00000000: 6f0d 0d0a 0000 0000 d344 0a64 620a 0000  o........D.db...
+00000000: 6f0d 0d0a 0000 0000 bd31 4964 c70a 0000  o........1Id....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000080: 0100 6503 6509 6a0e 640a 640b 8d02 5a0e  ..e.e.j.d.d...Z.
 00000090: 640c 650e 5f00 6503 6509 6a0f 640a 640b  d.e._.e.e.j.d.d.
 000000a0: 8d02 5a0f 640d 650f 5f00 640e 640f 8400  ..Z.d.e._.d.d...
 000000b0: 5a10 6410 6411 8400 5a11 6412 6413 8400  Z.d.d...Z.d.d...
-000000c0: 5a12 6402 5300 2914 7a42 0a53 6f6c 7665  Z.d.S.).zB.Solve
+000000c0: 5a12 6402 5300 2914 7a3b 0a53 6f6c 7665  Z.d.S.).z;.Solve
 000000d0: 7220 6672 616d 6577 6f72 6b0a 0a2e 2e20  r framework.... 
 000000e0: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
 000000f0: 203a 746f 6374 7265 653a 0a0a 2020 2062   :toctree:..   b
-00000100: 6173 650a 2020 206b 7468 0a0a e900 0000  ase.   kth......
-00000110: 004e 2901 da07 7061 7274 6961 6c29 01da  .N)...partial)..
-00000120: 0a4d 6f64 756c 6549 6e66 6f29 01da 0a4d  .ModuleInfo)...M
-00000130: 6f64 756c 6554 7970 6529 01da 066c 6f61  oduleType)...loa
-00000140: 6465 7229 01da 0e49 6e66 6f53 6f6c 7665  der)...InfoSolve
-00000150: 7243 6f72 65e9 0200 0000 2901 da06 6c6f  rCore.....)...lo
-00000160: 6767 6572 7a14 666c 7569 6473 696d 666f  ggerz.fluidsimfo
-00000170: 616d 2e73 6f6c 7665 7273 2901 5a0e 656e  am.solvers).Z.en
-00000180: 7472 7970 6f69 6e74 5f67 7270 7a4c 5265  trypoint_grpzLRe
-00000190: 7475 726e 7320 6120 6469 6374 696f 6e61  turns a dictiona
-000001a0: 7279 206f 6620 616c 6c20 7265 6769 7374  ry of all regist
-000001b0: 6572 6564 2073 6f6c 7665 7273 2072 6567  ered solvers reg
-000001c0: 6973 7465 7265 6420 6173 2061 6e20 656e  istered as an en
-000001d0: 7472 7970 6f69 6e74 2e0a 7a23 496d 706f  trypoint..z#Impo
-000001e0: 7274 2074 6865 2053 696d 756c 2063 6c61  rt the Simul cla
-000001f0: 7373 206f 6620 6120 736f 6c76 6572 2e63  ss of a solver.c
-00000200: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000210: 0400 0000 4300 0000 7356 0000 0074 007c  ....C...sV...t.|
-00000220: 0074 0183 0272 0c74 026a 03a0 047c 00a1  .t...r.t.j...|..
-00000230: 017d 016e 1a74 007c 0074 0583 0272 157c  .}.n.t.|.t...r.|
-00000240: 006a 067d 016e 1174 007c 0074 0783 0272  .j.}.n.t.|.t...r
-00000250: 1d7c 006a 0853 0074 0964 0174 0a7c 0083  .|.j.S.t.d.t.|..
-00000260: 019b 009d 0283 0182 017c 016a 0b64 0275  .........|.j.d.u
-00000270: 0153 0029 0375 2701 0000 4368 6563 6b73  .S.).u'...Checks
-00000280: 2069 6620 6120 6d6f 6475 6c65 2069 7320   if a module is 
-00000290: 6120 7061 636b 6167 6520 6f72 206e 6f74  a package or not
-000002a0: 2e20 4173 206f 6620 5045 5020 3435 3120  . As of PEP 451 
-000002b0: 7468 6973 2069 6e66 6f72 6d61 7469 6f6e  this information
-000002c0: 0a20 2020 2069 7320 616c 736f 2061 7661  .    is also ava
-000002d0: 696c 6162 6c65 206f 6e20 7468 6520 6d6f  ilable on the mo
-000002e0: 6475 6c65 e280 9973 205f 5f73 7065 635f  dule...s __spec_
-000002f0: 5f2e 7375 626d 6f64 756c 655f 7365 6172  _.submodule_sear
-00000300: 6368 5f6c 6f63 6174 696f 6e73 0a20 2020  ch_locations.   
-00000310: 2061 7474 7269 6275 7465 2c20 7768 6963   attribute, whic
-00000320: 6820 7769 6c6c 206e 6f74 2062 6520 4e6f  h will not be No
-00000330: 6e65 2066 6f72 2070 6163 6b61 6765 732e  ne for packages.
-00000340: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000350: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00000360: 2020 2020 6d6f 6475 6c65 3a20 7374 7220      module: str 
-00000370: 6f72 206d 6f64 756c 650a 0a20 2020 2052  or module..    R
-00000380: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00000390: 2d2d 0a20 2020 2062 6f6f 6c0a 0a20 2020  --.    bool..   
-000003a0: 207a 0f43 616e 6e6f 7420 7072 6f63 6573   z.Cannot proces
-000003b0: 7320 4e29 0cda 0a69 7369 6e73 7461 6e63  s N)...isinstanc
-000003c0: 65da 0373 7472 da09 696d 706f 7274 6c69  e..str..importli
-000003d0: 62da 0475 7469 6cda 0966 696e 645f 7370  b..util..find_sp
-000003e0: 6563 7204 0000 00da 085f 5f73 7065 635f  ecr......__spec_
-000003f0: 5f72 0300 0000 5a05 6973 706b 67da 0a56  _r....Z.ispkg..V
-00000400: 616c 7565 4572 726f 72da 0474 7970 65da  alueError..type.
-00000410: 1a73 7562 6d6f 6475 6c65 5f73 6561 7263  .submodule_searc
-00000420: 685f 6c6f 6361 7469 6f6e 7329 02da 066d  h_locations)...m
-00000430: 6f64 756c 65da 0473 7065 63a9 0072 1400  odule..spec..r..
-00000440: 0000 fa42 2f68 6f6d 652f 7069 6572 7265  ...B/home/pierre
-00000450: 2f44 6576 2f66 6c75 6964 7369 6d66 6f61  /Dev/fluidsimfoa
-00000460: 6d2f 7372 632f 666c 7569 6473 696d 666f  m/src/fluidsimfo
-00000470: 616d 2f73 6f6c 7665 7273 2f5f 5f69 6e69  am/solvers/__ini
-00000480: 745f 5f2e 7079 da0a 6973 5f70 6163 6b61  t__.py..is_packa
-00000490: 6765 2300 0000 7310 0000 000a 0e0e 010a  ge#...s.........
-000004a0: 0108 010a 0106 0112 020a 0272 1600 0000  ...........r....
-000004b0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000004c0: 0008 0000 0043 0000 0073 4800 0000 7400  .....C...sH...t.
-000004d0: 8300 7c00 1900 7d01 7a05 7c01 6a01 7d02  ..|...}.z.|.j.}.
-000004e0: 5700 6e0c 0400 7402 7916 0100 0100 0100  W.n...t.y.......
-000004f0: 7c01 6a03 7d02 5900 6e01 7700 7404 7c02  |.j.}.Y.n.w.t.|.
-00000500: 8301 721d 7c02 5300 7c02 a005 6401 a101  ..r.|.S.|...d...
-00000510: 6402 1900 5300 2903 7ad8 5265 7475 726e  d...S.).z.Return
-00000520: 206e 616d 6520 6f66 2074 6865 2073 6f6c   name of the sol
-00000530: 7665 7220 7061 636b 6167 6520 6279 2063  ver package by c
-00000540: 6865 636b 696e 6720 7468 6520 6060 736e  hecking the ``sn
-00000550: 656b 3530 3030 2e73 6f6c 7665 7273 6060  ek5000.solvers``
-00000560: 0a20 2020 2065 6e74 7279 706f 696e 7420  .    entrypoint 
-00000570: 6772 6f75 702e 0a0a 2020 2020 5061 7261  group...    Para
-00000580: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00000590: 2d2d 2d2d 2d0a 2020 2020 6e61 6d65 5f73  -----.    name_s
-000005a0: 6f6c 7665 723a 2073 7472 0a20 2020 2020  olver: str.     
-000005b0: 2020 2053 686f 7274 206e 616d 6520 6f66     Short name of
-000005c0: 2074 6865 2073 6f6c 7665 720a 0a20 2020   the solver..   
-000005d0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-000005e0: 2d2d 2d2d 0a20 2020 2073 7472 0a0a 2020  ----.    str..  
-000005f0: 2020 da01 2e72 0100 0000 2906 da11 6176    ...r....)...av
-00000600: 6169 6c61 626c 655f 736f 6c76 6572 7372  ailable_solversr
-00000610: 1200 0000 da0e 4174 7472 6962 7574 6545  ......AttributeE
-00000620: 7272 6f72 da0b 6d6f 6475 6c65 5f6e 616d  rror..module_nam
-00000630: 6572 1600 0000 da0a 7270 6172 7469 7469  er......rpartiti
-00000640: 6f6e 2903 5a0b 6e61 6d65 5f73 6f6c 7665  on).Z.name_solve
-00000650: 725a 0a65 6e74 7279 706f 696e 7472 1200  rZ.entrypointr..
-00000660: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000670: 00da 1267 6574 5f73 6f6c 7665 725f 7061  ...get_solver_pa
-00000680: 636b 6167 653d 0000 0073 1200 0000 0a0e  ckage=...s......
-00000690: 0201 0a02 0c01 0a01 02ff 0802 0401 0e02  ................
-000006a0: 721c 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000006b0: 0000 0400 0000 0500 0000 4300 0000 734e  ..........C...sN
-000006c0: 0000 007c 0064 011b 007d 017c 01a0 00a1  ...|.d...}.|....
-000006d0: 0072 1274 017c 0164 028d 017d 027c 026a  .r.t.|.d...}.|.j
-000006e0: 027d 037c 0353 0074 03a0 0464 037c 019b  .}.|.S.t...d.|..
-000006f0: 0064 049d 03a1 0101 007c 00a0 05a1 006a  .d.......|.....j
-00000700: 06a0 0764 05a1 0164 0619 007d 037c 0353  ...d...d...}.|.S
-00000710: 0029 077a e644 6574 6563 7473 2073 686f  .).z.Detects sho
-00000720: 7274 206e 616d 6520 6f66 2074 6865 2073  rt name of the s
-00000730: 6f6c 7665 7220 6672 6f6d 2060 6069 6e66  olver from ``inf
-00000740: 6f5f 736f 6c76 6572 2e78 6d6c 6060 2069  o_solver.xml`` i
-00000750: 6620 7072 6573 656e 7420 6f72 0a20 2020  f present or.   
-00000760: 2074 6865 2070 6174 682e 0a0a 2020 2020   the path...    
-00000770: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00000780: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7061  ---------.    pa
-00000790: 7468 5f64 6972 3a20 7061 7468 2d6c 696b  th_dir: path-lik
-000007a0: 650a 2020 2020 2020 2020 5061 7468 2074  e.        Path t
-000007b0: 6f20 6120 7369 6d75 6c61 7469 6f6e 2064  o a simulation d
-000007c0: 6972 6563 746f 7279 0a0a 2020 2020 5265  irectory..    Re
-000007d0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-000007e0: 2d0a 2020 2020 7368 6f72 745f 6e61 6d65  -.    short_name
-000007f0: 3a20 7374 720a 0a20 2020 207a 0f69 6e66  : str..    z.inf
-00000800: 6f5f 736f 6c76 6572 2e78 6d6c 2901 da09  o_solver.xml)...
-00000810: 7061 7468 5f66 696c 657a 0454 6865 207a  path_filez.The z
-00000820: 4520 6669 6c65 2069 7320 6d69 7373 696e  E file is missin
-00000830: 6721 2041 7474 656d 7074 696e 6720 746f  g! Attempting to
-00000840: 2067 7565 7373 2073 6f6c 7665 7220 6672   guess solver fr
-00000850: 6f6d 2074 6865 2064 6972 6563 746f 7279  om the directory
-00000860: 206e 616d 652e da01 5f72 0100 0000 2908   name..._r....).
-00000870: da06 6578 6973 7473 7206 0000 00da 0a73  ..existsr......s
-00000880: 686f 7274 5f6e 616d 6572 0800 0000 da07  hort_namer......
-00000890: 7761 726e 696e 67da 0861 6273 6f6c 7574  warning..absolut
-000008a0: 65da 046e 616d 65da 0573 706c 6974 2904  e..name..split).
-000008b0: da08 7061 7468 5f64 6972 5a0f 696e 666f  ..path_dirZ.info
-000008c0: 5f73 6f6c 7665 725f 786d 6cda 0b69 6e66  _solver_xml..inf
-000008d0: 6f5f 736f 6c76 6572 7220 0000 0072 1400  o_solverr ...r..
-000008e0: 0000 7214 0000 0072 1500 0000 da15 6765  ..r....r......ge
-000008f0: 745f 736f 6c76 6572 5f73 686f 7274 5f6e  t_solver_short_n
-00000900: 616d 6557 0000 0073 1400 0000 080e 0801  ameW...s........
-00000910: 0a01 0601 0408 04fa 0a01 04ff 1404 0402  ................
-00000920: 7227 0000 0029 13da 075f 5f64 6f63 5f5f  r'...)...__doc__
-00000930: 720b 0000 00da 0966 756e 6374 6f6f 6c73  r......functools
-00000940: 7202 0000 00da 0770 6b67 7574 696c 7203  r......pkgutilr.
-00000950: 0000 00da 0574 7970 6573 7204 0000 00da  .....typesr.....
-00000960: 0d66 6c75 6964 7369 6d5f 636f 7265 7205  .fluidsim_corer.
-00000970: 0000 005a 1266 6c75 6964 7369 6d5f 636f  ...Z.fluidsim_co
-00000980: 7265 2e69 6e66 6f72 0600 0000 da03 6c6f  re.infor......lo
-00000990: 6772 0800 0000 7218 0000 00da 1069 6d70  gr....r......imp
-000009a0: 6f72 745f 636c 735f 7369 6d75 6c72 1600  ort_cls_simulr..
-000009b0: 0000 721c 0000 0072 2700 0000 7214 0000  ..r....r'...r...
-000009c0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-000009d0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
-000009e0: 0000 0004 0008 0b0c 010c 010c 010c 020c  ................
-000009f0: 010c 0202 0206 0106 ff06 0302 0406 0106  ................
-00000a00: ff06 0308 0308 1a0c 1a                   .........
+00000100: 6173 650a 0ae9 0000 0000 4e29 01da 0770  ase.......N)...p
+00000110: 6172 7469 616c 2901 da0a 4d6f 6475 6c65  artial)...Module
+00000120: 496e 666f 2901 da0a 4d6f 6475 6c65 5479  Info)...ModuleTy
+00000130: 7065 2901 da06 6c6f 6164 6572 2901 da0e  pe)...loader)...
+00000140: 496e 666f 536f 6c76 6572 436f 7265 e902  InfoSolverCore..
+00000150: 0000 0029 01da 066c 6f67 6765 727a 1466  ...)...loggerz.f
+00000160: 6c75 6964 7369 6d66 6f61 6d2e 736f 6c76  luidsimfoam.solv
+00000170: 6572 7329 015a 0e65 6e74 7279 706f 696e  ers).Z.entrypoin
+00000180: 745f 6772 707a 4c52 6574 7572 6e73 2061  t_grpzLReturns a
+00000190: 2064 6963 7469 6f6e 6172 7920 6f66 2061   dictionary of a
+000001a0: 6c6c 2072 6567 6973 7465 7265 6420 736f  ll registered so
+000001b0: 6c76 6572 7320 7265 6769 7374 6572 6564  lvers registered
+000001c0: 2061 7320 616e 2065 6e74 7279 706f 696e   as an entrypoin
+000001d0: 742e 0a7a 2349 6d70 6f72 7420 7468 6520  t..z#Import the 
+000001e0: 5369 6d75 6c20 636c 6173 7320 6f66 2061  Simul class of a
+000001f0: 2073 6f6c 7665 722e 6301 0000 0000 0000   solver.c.......
+00000200: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000210: 0073 5600 0000 7400 7c00 7401 8302 720c  .sV...t.|.t...r.
+00000220: 7402 6a03 a004 7c00 a101 7d01 6e1a 7400  t.j...|...}.n.t.
+00000230: 7c00 7405 8302 7215 7c00 6a06 7d01 6e11  |.t...r.|.j.}.n.
+00000240: 7400 7c00 7407 8302 721d 7c00 6a08 5300  t.|.t...r.|.j.S.
+00000250: 7409 6401 740a 7c00 8301 9b00 9d02 8301  t.d.t.|.........
+00000260: 8201 7c01 6a0b 6402 7501 5300 2903 7527  ..|.j.d.u.S.).u'
+00000270: 0100 0043 6865 636b 7320 6966 2061 206d  ...Checks if a m
+00000280: 6f64 756c 6520 6973 2061 2070 6163 6b61  odule is a packa
+00000290: 6765 206f 7220 6e6f 742e 2041 7320 6f66  ge or not. As of
+000002a0: 2050 4550 2034 3531 2074 6869 7320 696e   PEP 451 this in
+000002b0: 666f 726d 6174 696f 6e0a 2020 2020 6973  formation.    is
+000002c0: 2061 6c73 6f20 6176 6169 6c61 626c 6520   also available 
+000002d0: 6f6e 2074 6865 206d 6f64 756c 65e2 8099  on the module...
+000002e0: 7320 5f5f 7370 6563 5f5f 2e73 7562 6d6f  s __spec__.submo
+000002f0: 6475 6c65 5f73 6561 7263 685f 6c6f 6361  dule_search_loca
+00000300: 7469 6f6e 730a 2020 2020 6174 7472 6962  tions.    attrib
+00000310: 7574 652c 2077 6869 6368 2077 696c 6c20  ute, which will 
+00000320: 6e6f 7420 6265 204e 6f6e 6520 666f 7220  not be None for 
+00000330: 7061 636b 6167 6573 2e0a 0a20 2020 2050  packages...    P
+00000340: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00000350: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d 6f64  --------.    mod
+00000360: 756c 653a 2073 7472 206f 7220 6d6f 6475  ule: str or modu
+00000370: 6c65 0a0a 2020 2020 5265 7475 726e 730a  le..    Returns.
+00000380: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000390: 626f 6f6c 0a0a 2020 2020 7a0f 4361 6e6e  bool..    z.Cann
+000003a0: 6f74 2070 726f 6365 7373 204e 290c da0a  ot process N)...
+000003b0: 6973 696e 7374 616e 6365 da03 7374 72da  isinstance..str.
+000003c0: 0969 6d70 6f72 746c 6962 da04 7574 696c  .importlib..util
+000003d0: da09 6669 6e64 5f73 7065 6372 0400 0000  ..find_specr....
+000003e0: da08 5f5f 7370 6563 5f5f 7203 0000 00da  ..__spec__r.....
+000003f0: 0569 7370 6b67 da0a 5661 6c75 6545 7272  .ispkg..ValueErr
+00000400: 6f72 da04 7479 7065 da1a 7375 626d 6f64  or..type..submod
+00000410: 756c 655f 7365 6172 6368 5f6c 6f63 6174  ule_search_locat
+00000420: 696f 6e73 2902 da06 6d6f 6475 6c65 da04  ions)...module..
+00000430: 7370 6563 a900 7215 0000 00fa 422f 686f  spec..r.....B/ho
+00000440: 6d65 2f70 6965 7272 652f 4465 762f 666c  me/pierre/Dev/fl
+00000450: 7569 6473 696d 666f 616d 2f73 7263 2f66  uidsimfoam/src/f
+00000460: 6c75 6964 7369 6d66 6f61 6d2f 736f 6c76  luidsimfoam/solv
+00000470: 6572 732f 5f5f 696e 6974 5f5f 2e70 79da  ers/__init__.py.
+00000480: 0a69 735f 7061 636b 6167 6522 0000 0073  .is_package"...s
+00000490: 1000 0000 0a0e 0e01 0a01 0801 0a01 0601  ................
+000004a0: 1202 0a02 7217 0000 0063 0100 0000 0000  ....r....c......
+000004b0: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
+000004c0: 0000 7348 0000 0074 0083 007c 0019 007d  ..sH...t...|...}
+000004d0: 017a 057c 016a 017d 0257 006e 0c04 0074  .z.|.j.}.W.n...t
+000004e0: 0279 1601 0001 0001 007c 016a 037d 0259  .y.......|.j.}.Y
+000004f0: 006e 0177 0074 047c 0283 0172 1d7c 0253  .n.w.t.|...r.|.S
+00000500: 007c 02a0 0564 01a1 0164 0219 0053 0029  .|...d...d...S.)
+00000510: 037a d852 6574 7572 6e20 6e61 6d65 206f  .z.Return name o
+00000520: 6620 7468 6520 736f 6c76 6572 2070 6163  f the solver pac
+00000530: 6b61 6765 2062 7920 6368 6563 6b69 6e67  kage by checking
+00000540: 2074 6865 2060 6073 6e65 6b35 3030 302e   the ``snek5000.
+00000550: 736f 6c76 6572 7360 600a 2020 2020 656e  solvers``.    en
+00000560: 7472 7970 6f69 6e74 2067 726f 7570 2e0a  trypoint group..
+00000570: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00000580: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00000590: 2020 206e 616d 655f 736f 6c76 6572 3a20     name_solver: 
+000005a0: 7374 720a 2020 2020 2020 2020 5368 6f72  str.        Shor
+000005b0: 7420 6e61 6d65 206f 6620 7468 6520 736f  t name of the so
+000005c0: 6c76 6572 0a0a 2020 2020 5265 7475 726e  lver..    Return
+000005d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+000005e0: 2020 7374 720a 0a20 2020 20da 012e 7201    str..    ...r.
+000005f0: 0000 0029 06da 1161 7661 696c 6162 6c65  ...)...available
+00000600: 5f73 6f6c 7665 7273 7213 0000 00da 0e41  _solversr......A
+00000610: 7474 7269 6275 7465 4572 726f 72da 0b6d  ttributeError..m
+00000620: 6f64 756c 655f 6e61 6d65 7217 0000 00da  odule_namer.....
+00000630: 0a72 7061 7274 6974 696f 6e29 03da 0b6e  .rpartition)...n
+00000640: 616d 655f 736f 6c76 6572 da0a 656e 7472  ame_solver..entr
+00000650: 7970 6f69 6e74 7213 0000 0072 1500 0000  ypointr....r....
+00000660: 7215 0000 0072 1600 0000 da12 6765 745f  r....r......get_
+00000670: 736f 6c76 6572 5f70 6163 6b61 6765 3c00  solver_package<.
+00000680: 0000 7312 0000 000a 0e02 010a 020c 010a  ..s.............
+00000690: 0102 ff08 0204 010e 0272 1f00 0000 6301  .........r....c.
+000006a0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+000006b0: 0000 0043 0000 0073 5e00 0000 7c00 6401  ...C...s^...|.d.
+000006c0: 1b00 7d01 7c01 a000 a100 730c 7c00 6402  ..}.|.....s.|.d.
+000006d0: 1b00 7d01 7c01 a000 a100 721a 7401 7c01  ..}.|.....r.t.|.
+000006e0: 6403 8d01 7d02 7c02 6a02 7d03 7c03 5300  d...}.|.j.}.|.S.
+000006f0: 7403 a004 6404 7c01 9b00 6405 9d03 a101  t...d.|...d.....
+00000700: 0100 7c00 a005 a100 6a06 a007 6406 a101  ..|.....j...d...
+00000710: 6407 1900 7d03 7c03 5300 2908 7ae6 4465  d...}.|.S.).z.De
+00000720: 7465 6374 7320 7368 6f72 7420 6e61 6d65  tects short name
+00000730: 206f 6620 7468 6520 736f 6c76 6572 2066   of the solver f
+00000740: 726f 6d20 6060 696e 666f 5f73 6f6c 7665  rom ``info_solve
+00000750: 722e 786d 6c60 6020 6966 2070 7265 7365  r.xml`` if prese
+00000760: 6e74 206f 720a 2020 2020 7468 6520 7061  nt or.    the pa
+00000770: 7468 2e0a 0a20 2020 2050 6172 616d 6574  th...    Paramet
+00000780: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00000790: 2d2d 0a20 2020 2070 6174 685f 6469 723a  --.    path_dir:
+000007a0: 2070 6174 682d 6c69 6b65 0a20 2020 2020   path-like.     
+000007b0: 2020 2050 6174 6820 746f 2061 2073 696d     Path to a sim
+000007c0: 756c 6174 696f 6e20 6469 7265 6374 6f72  ulation director
+000007d0: 790a 0a20 2020 2052 6574 7572 6e73 0a20  y..    Returns. 
+000007e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2073     -------.    s
+000007f0: 686f 7274 5f6e 616d 653a 2073 7472 0a0a  hort_name: str..
+00000800: 2020 2020 7a0f 696e 666f 5f73 6f6c 7665      z.info_solve
+00000810: 722e 786d 6c7a 1e2e 6461 7461 5f66 6c75  r.xmlz..data_flu
+00000820: 6964 7369 6d2f 696e 666f 5f73 6f6c 7665  idsim/info_solve
+00000830: 722e 786d 6c29 01da 0970 6174 685f 6669  r.xml)...path_fi
+00000840: 6c65 7a04 5468 6520 7a45 2066 696c 6520  lez.The zE file 
+00000850: 6973 206d 6973 7369 6e67 2120 4174 7465  is missing! Atte
+00000860: 6d70 7469 6e67 2074 6f20 6775 6573 7320  mpting to guess 
+00000870: 736f 6c76 6572 2066 726f 6d20 7468 6520  solver from the 
+00000880: 6469 7265 6374 6f72 7920 6e61 6d65 2eda  directory name..
+00000890: 015f 7201 0000 0029 08da 0665 7869 7374  ._r....)...exist
+000008a0: 7372 0600 0000 da0a 7368 6f72 745f 6e61  sr......short_na
+000008b0: 6d65 7208 0000 00da 0777 6172 6e69 6e67  mer......warning
+000008c0: da08 6162 736f 6c75 7465 da04 6e61 6d65  ..absolute..name
+000008d0: da05 7370 6c69 7429 04da 0870 6174 685f  ..split)...path_
+000008e0: 6469 725a 0f69 6e66 6f5f 736f 6c76 6572  dirZ.info_solver
+000008f0: 5f78 6d6c da0b 696e 666f 5f73 6f6c 7665  _xml..info_solve
+00000900: 7272 2300 0000 7215 0000 0072 1500 0000  rr#...r....r....
+00000910: 7216 0000 00da 1567 6574 5f73 6f6c 7665  r......get_solve
+00000920: 725f 7368 6f72 745f 6e61 6d65 5600 0000  r_short_nameV...
+00000930: 7318 0000 0008 0e08 0108 0108 020a 0106  s...............
+00000940: 0104 0804 fa0a 0104 ff14 0404 0272 2a00  .............r*.
+00000950: 0000 2913 da07 5f5f 646f 635f 5f72 0b00  ..)...__doc__r..
+00000960: 0000 da09 6675 6e63 746f 6f6c 7372 0200  ....functoolsr..
+00000970: 0000 da07 706b 6775 7469 6c72 0300 0000  ....pkgutilr....
+00000980: da05 7479 7065 7372 0400 0000 5a0d 666c  ..typesr....Z.fl
+00000990: 7569 6473 696d 5f63 6f72 6572 0500 0000  uidsim_corer....
+000009a0: 5a12 666c 7569 6473 696d 5f63 6f72 652e  Z.fluidsim_core.
+000009b0: 696e 666f 7206 0000 00da 036c 6f67 7208  infor......logr.
+000009c0: 0000 0072 1900 0000 da10 696d 706f 7274  ...r......import
+000009d0: 5f63 6c73 5f73 696d 756c 7217 0000 0072  _cls_simulr....r
+000009e0: 1f00 0000 722a 0000 0072 1500 0000 7215  ....r*...r....r.
+000009f0: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+00000a00: 6d6f 6475 6c65 3e01 0000 0073 2600 0000  module>....s&...
+00000a10: 0400 080a 0c01 0c01 0c01 0c02 0c01 0c02  ................
+00000a20: 0202 0601 06ff 0603 0204 0601 06ff 0603  ................
+00000a30: 0803 081a 0c1a                           ......
```

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc` & `fluidsimfoam-0.0.2/src/fluidsimfoam/util/__pycache__/console.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/src/fluidsimfoam/util/console.py` & `fluidsimfoam-0.0.2/src/fluidsimfoam/util/console.py`

 * *Files identical despite different names*

### Comparing `fluidsimfoam-0.0.1/PKG-INFO` & `fluidsimfoam-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: fluidsimfoam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python framework for OpenFOAM
 License: BSD-3-Clause
 Author: pierre.augier
 Author-email: pierre.augier@univ-grenoble-alpes.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fluiddyn (>=0.5.2,<0.6.0)
 Requires-Dist: fluidsim-core (>=0.7.2,<0.8.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: invoke (>=2.0.0,<3.0.0)
 Requires-Dist: ipython (>=8.11.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: lark (>=1.1.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: rich (>=13.3.3,<14.0.0)
 Description-Content-Type: text/markdown
 
+<div align="center">
+
 # Fluidsimfoam
 
+[![PyPI](https://img.shields.io/pypi/v/fluidsimfoam)](https://pypi.org/project/fluidsimfoam/)
+[![Documentation Status](https://readthedocs.org/projects/fluidsimfoam/badge/?version=latest)](https://fluidsimfoam.readthedocs.io/en/latest/?badge=latest)
+
 <!-- badges -->
 
 Python framework for [OpenFOAM]
 
+</div>
+
 Fluidsimfoam is a Python package which **will** allow one to write [Fluidsim]
 solvers based for the simulations on the C++ CFD code [OpenFOAM]. There
 **will** be open-source solvers (in particular fluidsimfoam-phill and
 fluidsimfoam-tgv) and it **will** not be difficult to write your own solver
 based on your [OpenFOAM] cases.
 
 With a Fluidsimfoam solver, it **will** becomes very easy to
@@ -35,26 +46,29 @@
 - launch/restart simulations with Python scripts and terminal commands,
 - load simulations, read the associated parameters/data and produce nice figures/movies.
 
 Fluidsimfoam can be seen as a workflow manager for [OpenFOAM] or a Python
 wrapper around [OpenFOAM]. It uses [OpenFOAM] on the background and is thus NOT
 a rewrite of [OpenFOAM]!
 
-Fluidsimfoam is now in very early development. The goal is to get the
+Fluidsimfoam is now in early development. The goal is to get the
 equivalent of [Snek5000], our Fluidsim framework for [Nek5000].
 
-## Related projects
+We currently target OpenFOAM v2206. See more in [Fluidsimfoam
+documentation](https://fluidsimfoam.readthedocs.org).
 
-- [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
-  [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
-  OpenFOAM. GNU GPL. Still maintained. Should be used by Fluidsimfoam.
+## Related projects
 
 - [Fluidfoam] Another Fluiddyn package (like Fluidsimfoam) to use/plot OpenFOAM
   data. Will be used by Fluidsimfoam.
 
+- [PyFoam] ([PyPI package](https://pypi.org/project/PyFoam/),
+  [hg repo](http://hg.code.sf.net/p/openfoam-extend/PyFoam)) Python utilities for
+  OpenFOAM. GNU GPL. Still maintained.
+
 - [PythonFlu] ([wiki](https://openfoamwiki.net/index.php/Contrib_pythonFlu))
 
 - [Swak4Foam]
 
 [PyFoam]: https://openfoamwiki.net/index.php/Contrib/PyFoam
 [fluidsim]: https://fluidsim.readthedocs.io
 [fluidfoam]: https://fluidfoam.readthedocs.io
```

