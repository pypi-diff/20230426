# Comparing `tmp/pypint-1.6.2.tar.gz` & `tmp/pypint-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypint-1.6.2.tar", last modified: Wed Dec 30 22:30:04 2020, max compression
+gzip compressed data, was "pypint-1.6.3.tar", last modified: Wed Apr 26 10:37:13 2023, max compression
```

## Comparing `pypint-1.6.2.tar` & `pypint-1.6.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 22:30:04.500912 pypint-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-30 22:29:53.000000 pypint-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-12-30 22:30:04.500912 pypint-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      345 2020-12-30 22:29:53.000000 pypint-1.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 22:30:04.496912 pypint-1.6.2/pypint/
--rw-r--r--   0 runner    (1001) docker     (116)     7453 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      756 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/cfg.py
--rw-r--r--   0 runner    (1001) docker     (116)      792 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/console.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 22:30:04.500912 pypint-1.6.2/pypint/converters/
--rw-r--r--   0 runner    (1001) docker     (116)      252 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3955 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/biocham.py
--rw-r--r--   0 runner    (1001) docker     (116)     4458 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/cadbiom.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 22:30:04.500912 pypint-1.6.2/pypint/converters/lib/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1335 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/lib/boolean_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      565 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/lib/export_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    10874 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/lib/sbgnpd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1367 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/minibn.py
--rw-r--r--   0 runner    (1001) docker     (116)    10875 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/converters/sbgnpd.py
--rw-r--r--   0 runner    (1001) docker     (116)    15742 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/model.py
--rw-r--r--   0 runner    (1001) docker     (116)    28961 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)    11484 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/types.py
--rw-r--r--   0 runner    (1001) docker     (116)     1278 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/ui.py
--rw-r--r--   0 runner    (1001) docker     (116)      259 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-30 22:30:04.496912 pypint-1.6.2/pypint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2020-12-30 22:30:04.000000 pypint-1.6.2/pypint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      649 2020-12-30 22:29:53.000000 pypint-1.6.2/pypint_setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-30 22:30:04.500912 pypint-1.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1539 2020-12-30 22:29:53.000000 pypint-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:13.913076 pypint-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 10:37:03.000000 pypint-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 10:37:13.913076 pypint-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 10:37:03.000000 pypint-1.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:13.909076 pypint-1.6.3/pypint/
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:13.909076 pypint-1.6.3/pypint/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/biocham.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/cadbiom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:13.913076 pypint-1.6.3/pypint/converters/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/lib/boolean_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/lib/export_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/lib/sbgnpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/minibn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/converters/sbgnpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28961 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:37:13.909076 pypint-1.6.3/pypint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 10:37:13.000000 pypint-1.6.3/pypint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 10:37:03.000000 pypint-1.6.3/pypint_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:37:13.913076 pypint-1.6.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-26 10:37:03.000000 pypint-1.6.3/setup.py
```

### Comparing `pypint-1.6.2/PKG-INFO` & `pypint-1.6.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pypint
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python interface to Pint
 Home-page: http://loicpauleve.name/pint
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: CeCILL
-Description: Python interface to Pint
-        ------------------------
-        
-        Pint is a static analyser for the transient dynamics of automata networks.
-        
-        This python module provides an interface to Pint command line tools.
-        It also provides customization for the Jupyter notebook interface to ease user
-        interaction.
-        
-        See http://loicpauleve.name/pint for more information.
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.4
+
+Python interface to Pint
+------------------------
+
+Pint is a static analyser for the transient dynamics of automata networks.
+
+This python module provides an interface to Pint command line tools.
+It also provides customization for the Jupyter notebook interface to ease user
+interaction.
+
+See http://loicpauleve.name/pint for more information.
+
```

### Comparing `pypint-1.6.2/pypint/__init__.py` & `pypint-1.6.3/pypint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 When loaded, the `pypint` module will perform the follow tasks:
 
 * add Pint third-party binary path (`bin` subdirectory of
   ``pint-config share-path``) to the ``PATH`` environment variable.
 * if in IPython, displays the version of Pint binaries, and executes
   :py:func:`.ipython_install`.
 """
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 
 import os
 import shutil
 import subprocess
 import sys
 
 if sys.version_info[0] < 3:
```

### Comparing `pypint-1.6.2/pypint/cfg.py` & `pypint-1.6.3/pypint/cfg.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/console.py` & `pypint-1.6.3/pypint/console.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/biocham.py` & `pypint-1.6.3/pypint/converters/biocham.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/cadbiom.py` & `pypint-1.6.3/pypint/converters/cadbiom.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/lib/boolean_utils.py` & `pypint-1.6.3/pypint/converters/lib/boolean_utils.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/lib/export_utils.py` & `pypint-1.6.3/pypint/converters/lib/export_utils.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/lib/sbgnpd.py` & `pypint-1.6.3/pypint/converters/lib/sbgnpd.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/converters/minibn.py` & `pypint-1.6.3/pypint/converters/minibn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import boolean.boolean
 from colomoto_jupyter.sessionfiles import new_output_file
 from pypint.converters.lib.boolean_utils import BoolToAN
 from pypint.converters.lib.export_utils import pint_protect
 
 from colomoto.minibn import BooleanNetwork, MultiValuedNetwork
 
 def import_minibn(f):
@@ -10,15 +11,15 @@
 
     assert isinstance(f, BooleanNetwork), \
         "{}: only objects of type {} are supported".format(import_minibn, BooleanNetwork)
 
     ba = f.ba
 
     def ls_of_lit(lit):
-        if isinstance(lit, ba.NOT):
+        if isinstance(lit, boolean.boolean.NOT):
             return (lit.args[0].obj, 0)
         else:
             return (lit.obj, 1)
 
     anfile = new_output_file(ext="an")
     with open(anfile, "w") as outf:
         def out(data):
```

### Comparing `pypint-1.6.2/pypint/converters/sbgnpd.py` & `pypint-1.6.3/pypint/converters/sbgnpd.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/model.py` & `pypint-1.6.3/pypint/model.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/tools.py` & `pypint-1.6.3/pypint/tools.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/types.py` & `pypint-1.6.3/pypint/types.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint/ui.py` & `pypint-1.6.3/pypint/ui.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint.egg-info/PKG-INFO` & `pypint-1.6.3/pypint.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pypint
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python interface to Pint
 Home-page: http://loicpauleve.name/pint
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: CeCILL
-Description: Python interface to Pint
-        ------------------------
-        
-        Pint is a static analyser for the transient dynamics of automata networks.
-        
-        This python module provides an interface to Pint command line tools.
-        It also provides customization for the Jupyter notebook interface to ease user
-        interaction.
-        
-        See http://loicpauleve.name/pint for more information.
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.4
+
+Python interface to Pint
+------------------------
+
+Pint is a static analyser for the transient dynamics of automata networks.
+
+This python module provides an interface to Pint command line tools.
+It also provides customization for the Jupyter notebook interface to ease user
+interaction.
+
+See http://loicpauleve.name/pint for more information.
+
```

### Comparing `pypint-1.6.2/pypint.egg-info/SOURCES.txt` & `pypint-1.6.3/pypint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/pypint_setup.py` & `pypint-1.6.3/pypint_setup.py`

 * *Files identical despite different names*

### Comparing `pypint-1.6.2/setup.py` & `pypint-1.6.3/setup.py`

 * *Files identical despite different names*

