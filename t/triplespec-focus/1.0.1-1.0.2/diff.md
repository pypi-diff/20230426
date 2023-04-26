# Comparing `tmp/triplespec_focus-1.0.1.tar.gz` & `tmp/triplespec_focus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplespec_focus-1.0.1.tar", last modified: Thu Dec 15 14:11:21 2022, max compression
+gzip compressed data, was "triplespec_focus-1.0.2.tar", last modified: Tue Apr 25 18:52:21 2023, max compression
```

## Comparing `triplespec_focus-1.0.1.tar` & `triplespec_focus-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.544679 triplespec_focus-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.532678 triplespec_focus-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.536678 triplespec_focus-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2022-12-15 14:11:21.544679 triplespec_focus-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.536678 triplespec_focus-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.540679 triplespec_focus-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   714605 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/_static/focus_results.png
--rw-r--r--   0 runner    (1001) docker     (123)   159166 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/_static/in_terminal_help.png
--rw-r--r--   0 runner    (1001) docker     (123)   880333 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/_static/slit_view_sample.png
--rw-r--r--   0 runner    (1001) docker     (123)    26011 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/_static/soar_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/data_overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/use_as_library.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/docs/use_from_terminal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-15 14:11:21.544679 triplespec_focus-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.540679 triplespec_focus-1.0.1/triplespec_focus/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.544679 triplespec_focus-1.0.1/triplespec_focus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/tests/test_triplespec_focus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/triplespec_focus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2022-12-15 14:10:54.000000 triplespec_focus-1.0.1/triplespec_focus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 14:11:21.540679 triplespec_focus-1.0.1/triplespec_focus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-15 14:11:21.000000 triplespec_focus-1.0.1/triplespec_focus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.455854 triplespec_focus-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.459854 triplespec_focus-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.459854 triplespec_focus-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.459854 triplespec_focus-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   714605 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/_static/focus_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159166 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/_static/in_terminal_help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   880333 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/_static/slit_view_sample.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26011 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/_static/soar_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/data_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.459854 triplespec_focus-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/source/triplespec_focus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/use_as_library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/docs/use_from_terminal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/triplespec_focus/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/triplespec_focus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/tests/test_triplespec_focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/triplespec_focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-25 18:52:08.000000 triplespec_focus-1.0.2/triplespec_focus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:52:21.463853 triplespec_focus-1.0.2/triplespec_focus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 18:52:21.000000 triplespec_focus-1.0.2/triplespec_focus.egg-info/top_level.txt
```

### Comparing `triplespec_focus-1.0.1/.github/workflows/codeql-analysis.yml` & `triplespec_focus-1.0.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/.github/workflows/python-package.yml` & `triplespec_focus-1.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/.github/workflows/python-publish.yml` & `triplespec_focus-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/.gitignore` & `triplespec_focus-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/LICENSE` & `triplespec_focus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/PKG-INFO` & `triplespec_focus-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplespec_focus
-Version: 1.0.1
+Version: 1.0.2
 Summary: Finds best focus for TripleSpec spectrograph based on a series of images obtained with different focus values
 Home-page: https://github.com/soar-telescope/triplespec_focus
 Author: Simon Torres
 Author-email: simon.torres@noirlab.edu
 License: BSD-3-Clause
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `triplespec_focus-1.0.1/README.md` & `triplespec_focus-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/Makefile` & `triplespec_focus-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/_static/focus_results.png` & `triplespec_focus-1.0.2/docs/_static/focus_results.png`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/_static/in_terminal_help.png` & `triplespec_focus-1.0.2/docs/_static/in_terminal_help.png`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/_static/slit_view_sample.png` & `triplespec_focus-1.0.2/docs/_static/slit_view_sample.png`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/_static/soar_logo.png` & `triplespec_focus-1.0.2/docs/_static/soar_logo.png`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/conf.py` & `triplespec_focus-1.0.2/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,26 +40,27 @@
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
     'matplotlib.sphinxext.plot_directive',
 ]
 
+autoclass_content = 'both'
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 
 source_suffix = ['.rst']
 
 
 master_doc = 'index'
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', 'test_', 'tests']
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `triplespec_focus-1.0.1/docs/data_overview.rst` & `triplespec_focus-1.0.2/docs/data_overview.rst`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/index.rst` & `triplespec_focus-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/make.bat` & `triplespec_focus-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/use_as_library.rst` & `triplespec_focus-1.0.2/docs/use_as_library.rst`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/docs/use_from_terminal.rst` & `triplespec_focus-1.0.2/docs/use_from_terminal.rst`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/setup.cfg` & `triplespec_focus-1.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -44,19 +44,22 @@
 	coverage
 	requests
 docs = 
 	matplotlib
 	sphinx
 	sphinx-rtd-theme
 
+[coverage:run]
+omit = */tests/*,*__init__.py
+
 [options.entry_points]
 triplespec_focus = triplespec_focus.run_triplespec_focus
 
 [flake8]
-max-line-length = 100
-max-doc-length = 79
+max-line-length = 120
+max-doc-length = 120
 ignore = E126,E127,E128,E201,E202,E203,E221,E225,E226,E227,E231,E251,E501,E731,E741,W503,W504,W505
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `triplespec_focus-1.0.1/setup.py` & `triplespec_focus-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/tox.ini` & `triplespec_focus-1.0.2/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     MPLBACKEND=agg
     # Disable the accelerate linear algebra library when running on macos as
     # latest numpy versions do not work with it
     NPY_BLAS_ORDER=
     NPY_LAPACK_ORDER=
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI
+passenv = HOME,WINDIR,LC_ALL,LC_CTYPE,CC,CI
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
@@ -62,32 +62,29 @@
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     alldeps: all
 
 commands =
-    pip freeze
     !cov: pytest --pyargs triplespec_focus {toxinidir}/docs {posargs}
     cov: pytest --pyargs triplespec_focus {toxinidir}/docs --cov triplespec_focus --cov-config={toxinidir}/setup.cfg {posargs}
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
-    pip freeze
     sphinx-build -W -b html . _build/html
 
 [testenv:linkcheck]
 changedir = docs
 description = check the links in the HTML docs
 extras = docs
 commands =
-    pip freeze
     sphinx-build -W -b linkcheck . _build/html
 
 [testenv:codestyle]
 skip_install = true
 changedir = .
 description = check code style, e.g. with flake8
 deps = flake8
```

### Comparing `triplespec_focus-1.0.1/triplespec_focus/entrypoints.py` & `triplespec_focus-1.0.2/triplespec_focus/entrypoints.py`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/triplespec_focus/tests/test_triplespec_focus.py` & `triplespec_focus-1.0.2/triplespec_focus/tests/test_triplespec_focus.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,14 +66,24 @@
         self.assertIsNone(self.tspec_focus.fitted_model)
         results = self.tspec_focus.get_best_focus(df=df, x_axis_size=2000)
         self.assertAlmostEqual(self.tspec_focus.best_focus, -1000, places=4)
         self.assertIsNotNone(self.tspec_focus.fitted_model)
         self.assertIsInstance(self.tspec_focus.fitted_model, Model)
         self.assertIsInstance(results, list)
 
+    def test_get_focus_with_fwhm_monotonically_increasing(self):
+        focus_values = [-1300, -1200, -1100, -1000, -900, -800, -700]
+        fwhm_values = [1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7]
+        data = {'focus': focus_values, 'fwhm': fwhm_values}
+        df = DataFrame(data=data)
+        self.assertIsNone(self.tspec_focus.best_focus)
+        self.assertIsNone(self.tspec_focus.fitted_model)
+        results = self.tspec_focus.get_best_focus(df=df, x_axis_size=2000)
+        self.assertIsNone(results)
+
     def test_detect_sources(self):
         ccd = CCDData.read(self.test_file_name, unit='adu')
         self.tspec_focus.show_mask = True
         sources = self.tspec_focus.detect_sources(ccd=ccd, debug_plots=False)
         self.assertIsInstance(sources, QTable)
         self.assertEqual(len(sources), 94)
 
@@ -85,9 +95,7 @@
 
     def test_call_with_file_list(self):
         data_path = Path('./')
 
         results = self.tspec_focus(file_list=sorted(data_path.glob(pattern='*.fits')))
         self.assertIsInstance(results, dict)
         self.assertEqual(len(results), 11)
-
-
```

### Comparing `triplespec_focus-1.0.1/triplespec_focus/tests/test_utils.py` & `triplespec_focus-1.0.2/triplespec_focus/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `triplespec_focus-1.0.1/triplespec_focus/triplespec_focus.py` & `triplespec_focus-1.0.2/triplespec_focus/triplespec_focus.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from astropy.table import QTable
 from astropy.visualization import ZScaleInterval
 from ccdproc import CCDData
 
 from pandas import DataFrame
 from pandas import concat
 from pathlib import Path
-from photutils import DAOStarFinder
-from photutils import CircularAperture
+from photutils.detection import DAOStarFinder
+from photutils.aperture import CircularAperture
 
 from scipy import optimize
 from typing import List, Union
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 from .utils import (circular_aperture_statistics,
@@ -55,15 +55,16 @@
             date_time_key (str): FITS keyword name for obtaining the date and time from the FITS file. Default DATE-OBS.
             focus_key (str): FITS keyword name for obtaining the focus value from the FITS file. Default TELFOCUS.
             filename_key (str): FITS keyword name for obtaining the file name from the FITS file. Default FILENAME.
             file_pattern (str): Pattern for searching files in the provided data path. Default *.fits.
             n_brightest (int): Number of the brightest sources to use for measuring source statistics. Default 5.
             saturation (float): Data value at which the detector saturates. Default 40000.
             plot_results (bool): If set to True will display information plots at the end. Default False.
-            debug_plots (bool): If set to True will display several plots useful for debugging or viewing the process. Default False.
+            debug_plots (bool): If set to True will display several plots useful for debugging or viewing the process.
+              Default False.
         """
 
         self.best_fwhm = None
         self.best_focus = None
         self.fitted_model = None
         self.best_image_overall = None
         self.date_key: str = date_key
@@ -109,20 +110,23 @@
         This method contains all the logic to obtain the best focus, additionally you can parse the following parameters
 
         Args:
             data_path (Path, str, None): Optional data path to obtain files according to file_pattern. Default None.
             file_list (List, None): Optional file list with files to be used to obtain best focus. Default None.
             source_fwhm (float): Full width at half maximum to use for source detection and statistics.
             det_threshold (float): Number of standard deviation above median to use as detection threshold. Default 5.0.
-            mask_threshold (float): Number of standard deviation below median to use as a threshold for masking values. Default 1.
+            mask_threshold (float): Number of standard deviation below median to use as a threshold for masking values.
+              Default 1.
             n_brightest (int): Number of the brightest sources to use for measuring source statistics. Default 5.
             saturation_level (float): Data value at which the detector saturates. Default 40000.
-            show_mask (bool): If set to True will display masked values in red when debug_plots is also True: Default False.
+            show_mask (bool): If set to True will display masked values in red when debug_plots is also True:
+              Default False.
             plot_results (bool): If set to True will display information plots at the end. Default False.
-            debug_plots (bool): If set to True will display several plots useful for debugging or viewing the process. Default False.
+            debug_plots (bool): If set to True will display several plots useful for debugging or viewing the process.
+              Default False.
             print_all_data (bool): If set to True will print the entire dataset at the end.
 
         Returns:
             A dictionary containing information regarding the current process.
         """
         if file_list:
             self.log.debug(f"Using provided file list containing {len(file_list)} files.")
@@ -196,25 +200,28 @@
 
         all_stars_photometry = []
         all_focus = []
         all_fwhm = []
         for star_id in star_ids:
             star_phot = self.sources_df[self.sources_df['id'] == star_id]
             interpolated_data = self.get_best_focus(df=star_phot)
-            all_stars_photometry.append([star_phot, interpolated_data, self.best_focus])
-            all_focus.append(self.best_focus)
-            all_fwhm.append(self.best_fwhm)
+            if interpolated_data:
+                all_stars_photometry.append([star_phot, interpolated_data, self.best_focus])
+                if self.best_focus and self.best_fwhm:
+                    all_focus.append(self.best_focus)
+                    all_fwhm.append(self.best_fwhm)
 
         mean_focus = np.mean(all_focus)
         median_focus = np.median(all_focus)
         focus_std = np.std(all_focus)
         mean_fwhm = np.mean(all_fwhm)
 
         best_image_overall = CCDData.read(self.best_image_overall, unit='adu')
-        self.best_image_fwhm = self.sources_df[self.sources_df['filename'] == os.path.basename(self.best_image_overall)]['fwhm'].mean()
+        self.best_image_fwhm = self.sources_df[self.sources_df['filename'] == os.path.basename(
+            self.best_image_overall)]['fwhm'].mean()
 
         focus_data = []
         fwhm_data = []
         images = self.sources_df.filename.unique().tolist()
         for image in images:
             summary_df = self.sources_df[self.sources_df['filename'] == image]
             focus = summary_df.focus.unique().tolist()
@@ -272,15 +279,16 @@
     def detect_sources(self, ccd: CCDData, debug_plots: bool = False) -> QTable:
         """Detects sources in the sharpest image
 
         Using DAOStarFinder will detect the stellar sources in it.
 
         Args:
             ccd (CCDData): An image with point sources.
-            debug_plots (bool): If set to True will display the image with the sources. Default False.
+            debug_plots (bool): If set to True will display the image with the sources.
+              Default False.
 
         Returns:
             An Astropy's QTable containing ids, centroids, focus value and image name.
 
         """
         mean, median, std = sigma_clipped_stats(ccd.data, sigma=3.0)
         self.log.debug(f"Mean: {mean}, Median: {median}, Standard Dev: {std}")
@@ -333,32 +341,43 @@
             self.log.critical(f"Unable to detect sources in file: {ccd.header[self.filename_key]}")
         return sources
 
     def get_best_focus(self, df: DataFrame, x_axis_size: int = 2000) -> List[np.ndarray]:
         """Obtains the best focus for a single source
 
         Args:
-            df (DataFrame): Pandas DataFrame containing at least a 'focus' and a 'fwhm' column. The data should belong to a single source.
+            df (DataFrame): Pandas DataFrame containing at least a 'focus' and a 'fwhm' column.
+              The data should belong to a single source.
             x_axis_size (int): Size of the x-axis used to sample the fitted model. Is not an interpolation size.
 
         Returns:
-            A list with the x-axis and the sampled data using the fitted model
+            A list with the x-axis and the sampled data using the fitted model, None if it is not possible to find the
+              focus.
 
         """
         focus_start = df['focus'].min()
         focus_end = df['focus'].max()
 
         x_axis = np.linspace(start=focus_start, stop=focus_end, num=x_axis_size)
 
         self.fitted_model = self.fitter(self.model, df['focus'].tolist(), df['fwhm'].tolist())
         modeled_data = self.fitted_model(x_axis)
         index_of_minimum = np.argmin(modeled_data)
         middle_point = x_axis[index_of_minimum]
-
-        self.best_focus = optimize.brent(self.fitted_model, brack=(focus_start, middle_point, focus_end))
-        self.best_fwhm = modeled_data[index_of_minimum]
-
-        return [x_axis, modeled_data]
+        if middle_point == focus_start or middle_point == focus_end:
+            self.log.warning("The focus vs FWHM curve does not seem to have a V or U shape. Trying by forcing the "
+                             "mean focus as the middle point for Brent's optimization bracket definition.")
+            middle_point = (focus_start + focus_end) / 2.
+
+        self.log.debug(f"Brent optimization bracket, Start (xa): {focus_start} Middle (xb): {middle_point} End (xc): {focus_end}")
+
+        try:
+            self.best_focus = optimize.brent(self.fitted_model, brack=(focus_start, middle_point, focus_end))
+            self.best_fwhm = modeled_data[index_of_minimum]
+            self.log.info(f"Found best focus at {self.best_focus} with a fwhm of {self.best_fwhm}")
+            return [x_axis, modeled_data]
+        except ValueError as error:
+            self.log.error(error)
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `triplespec_focus-1.0.1/triplespec_focus/utils.py` & `triplespec_focus-1.0.2/triplespec_focus/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ccdproc import CCDData
 from logging import Logger
 
 from matplotlib import cm, pyplot as plt
 from pandas import DataFrame
 from typing import Union, List
 
-from photutils import CircularAperture, CircularAnnulus, ApertureStats
+from photutils.aperture import CircularAperture, CircularAnnulus, ApertureStats
 
 log = logging.getLogger(__name__)
 
 
 def circular_aperture_statistics(ccd: CCDData,
                                  positions: np.ndarray,
                                  aperture_radius: float = 10,
```

### Comparing `triplespec_focus-1.0.1/triplespec_focus.egg-info/PKG-INFO` & `triplespec_focus-1.0.2/triplespec_focus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplespec-focus
-Version: 1.0.1
+Version: 1.0.2
 Summary: Finds best focus for TripleSpec spectrograph based on a series of images obtained with different focus values
 Home-page: https://github.com/soar-telescope/triplespec_focus
 Author: Simon Torres
 Author-email: simon.torres@noirlab.edu
 License: BSD-3-Clause
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `triplespec_focus-1.0.1/triplespec_focus.egg-info/SOURCES.txt` & `triplespec_focus-1.0.2/triplespec_focus.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 docs/make.bat
 docs/use_as_library.rst
 docs/use_from_terminal.rst
 docs/_static/focus_results.png
 docs/_static/in_terminal_help.png
 docs/_static/slit_view_sample.png
 docs/_static/soar_logo.png
+docs/source/modules.rst
+docs/source/triplespec_focus.rst
 triplespec_focus/__init__.py
 triplespec_focus/entrypoints.py
 triplespec_focus/triplespec_focus.py
 triplespec_focus/utils.py
 triplespec_focus.egg-info/PKG-INFO
 triplespec_focus.egg-info/SOURCES.txt
 triplespec_focus.egg-info/dependency_links.txt
```

