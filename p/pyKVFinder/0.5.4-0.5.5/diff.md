# Comparing `tmp/pyKVFinder-0.5.4.tar.gz` & `tmp/pyKVFinder-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.5.4.tar", last modified: Wed Apr 19 20:48:04 2023, max compression
+gzip compressed data, was "pyKVFinder-0.5.5.tar", last modified: Wed Apr 26 19:51:03 2023, max compression
```

## Comparing `pyKVFinder-0.5.4.tar` & `pyKVFinder-0.5.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.184976 pyKVFinder-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.180976 pyKVFinder-0.5.4/C/
--rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    81497 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-19 20:48:04.184976 pyKVFinder-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-19 20:47:48.000000 pyKVFinder-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.180976 pyKVFinder-0.5.4/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.180976 pyKVFinder-0.5.4/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.184976 pyKVFinder-0.5.4/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (123)   109719 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    72122 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    64069 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:48:04.180976 pyKVFinder-0.5.4/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 20:48:04.000000 pyKVFinder-0.5.4/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:48:04.184976 pyKVFinder-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-19 20:47:49.000000 pyKVFinder-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/C/
+-rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    81497 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   110025 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72142 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64069 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:51:03.348171 pyKVFinder-0.5.5/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 19:51:03.000000 pyKVFinder-0.5.5/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:51:03.352172 pyKVFinder-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-26 19:50:47.000000 pyKVFinder-0.5.5/setup.py
```

### Comparing `pyKVFinder-0.5.4/C/numpy.i` & `pyKVFinder-0.5.5/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/C/pyKVFinder.c` & `pyKVFinder-0.5.5/C/pyKVFinder.c`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/C/pyKVFinder.h` & `pyKVFinder-0.5.5/C/pyKVFinder.h`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/C/pyKVFinder.i` & `pyKVFinder-0.5.5/C/pyKVFinder.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/LICENSE.txt` & `pyKVFinder-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/PKG-INFO` & `pyKVFinder-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.5.4/README.rst` & `pyKVFinder-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/__init__.py` & `pyKVFinder-0.5.5/pyKVFinder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 Command Line Interface
 ----------------------
   Usage: pyKVFinder [-h] [-v] [--version] [-b <str>] [-O <str>]\
                     [-m <int>] [--nthreads <int>] [-d <str>] [-s <float>]\
                     [-i <float>] [-o <float>] [-V <float>] [-R <float>]\
                     [-S <str>] [--ignore_backbone] [-D] [--plot_frequencies]\
                     [--hydropathy [{EisenbergWeiss, HessaHeijne, KyteDoolittle,\
-                    MoonFleming, WimleyWhite, ZhaoLondon, <.toml>}]]\
+                    MoonFleming, RadzickaWolfenden, WimleyWhite, ZhaoLondon, <.toml>}]]\
                     [-B <.toml>] [-L (<.pdb> | <.xyz>)] [--ligand_cutoff <float>]\
                     (<.pdb> | <.xyz>)
 
 See also
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.5.4/pyKVFinder/argparser.py` & `pyKVFinder-0.5.5/pyKVFinder/argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,23 @@
     Raises
     ------
     argparse.ArgumentTypeError
         Invalid TOML-formatted file: {x} (define a TOML-formatted
         file with hydrophobicity values for standard residues).
     argparse.ArgumentTypeError
         Invalid choice: '{x}' (choose from 'EisenbergWeiss', 'HessaHeijne',
-        'KyteDoolittle', 'MoonFleming', 'WimleyWhite', 'ZhaoLondon' or define a
-        TOML-formatted file with hydrophobicity values for standard residues).
+        'KyteDoolittle', 'MoonFleming', 'RadzickaWolfenden', 'WimleyWhite',
+        'ZhaoLondon' or define a TOML-formatted file with hydrophobicity
+        values for standard residues).
     """
     if x in [
         "EisenbergWeiss",
         "HessaHeijne",
         "KyteDoolittle",
+        "RadzickaWolfenden",
         "MoonFleming",
         "WimleyWhite",
         "ZhaoLondon",
     ]:
         return x
     elif os.path.exists(x):
         import toml
@@ -75,15 +77,15 @@
         except toml.decoder.TomlDecodeError:
             msg = f"Invalid TOML-formatted file: {x} (define a TOML-formatted \
 file with hydrophobicity values for standard residues)."
             raise (argparse.ArgumentTypeError(msg))
         return x
     else:
         msg = f"Invalid choice: '{x}' (choose from 'EisenbergWeiss', 'HessaHeijne', \
-'KyteDoolittle', 'MoonFleming', 'WimleyWhite', 'ZhaoLondon' or define a \
+'KyteDoolittle', 'MoonFleming', 'RadzickaWolfenden', 'WimleyWhite', 'ZhaoLondon' or define a \
 TOML-formatted file with hydrophobicity values for standard residues)."
         raise (argparse.ArgumentTypeError(msg))
 
 
 def _positive_float(x: Any) -> float:
     """Checks if x is a float.
 
@@ -327,15 +329,15 @@
         help="Plot bar charts of calculated frequencies of the detected \
 cavities in a PDF file. (default: %(default)s)",
     )
     extra_modes.add_argument(
         "--hydropathy",
         type=_check_hydropathy_options,
         metavar="{EisenbergWeiss, HessaHeijne, KyteDoolittle, MoonFleming, \
-WimleyWhite, ZhaoLondon, <.toml>}",
+RadzickaWolfenden, WimleyWhite, ZhaoLondon, <.toml>}",
         nargs="?",
         const="EisenbergWeiss",
         default=False,
         help="Hydropathy characterization of the detected cavities. Map \
 hydrophobicity scale values as B-factor at surface points of detected \
 cavities. Hydrophobicity scales options: %(metavar)s. A custom hydrophobicity \
 scale can be defined via a TOML-formatted file. (default: %(default)s) \
```

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.5.5/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.5.5/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder/grid.py` & `pyKVFinder-0.5.5/pyKVFinder/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -4422,2437 +4422,2456 @@
 00011450: 6e65 642c 2069 7420 6173 7369 676e 730a  ned, it assigns.
 00011460: 2020 2020 2020 2020 7a65 726f 2074 6f20          zero to 
 00011470: 7468 6520 6d69 7373 696e 6720 7265 7369  the missing resi
 00011480: 6475 6573 2028 7365 6520 6048 7964 726f  dues (see `Hydro
 00011490: 7068 6f62 6963 6974 7920 7363 616c 6520  phobicity scale 
 000114a0: 6669 6c65 0a20 2020 2020 2020 2074 656d  file.        tem
 000114b0: 706c 6174 6560 292e 2054 6865 2070 6163  plate`). The pac
-000114c0: 6b61 6765 2063 6f6e 7461 696e 7320 7369  kage contains si
-000114d0: 7820 6275 696c 742d 696e 2068 7964 726f  x built-in hydro
-000114e0: 7068 6f62 6963 6974 7920 7363 616c 6573  phobicity scales
-000114f0: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
-00011500: 2045 6973 656e 6265 7267 5765 6973 7320   EisenbergWeiss 
-00011510: 5b31 5d5f 3b0a 2020 2020 2020 2020 2020  [1]_;.          
-00011520: 2020 2a20 4865 7373 6148 6569 6a6e 6520    * HessaHeijne 
-00011530: 5b32 5d5f 3b0a 2020 2020 2020 2020 2020  [2]_;.          
-00011540: 2020 2a20 4b79 7465 446f 6f6c 6974 746c    * KyteDoolittl
-00011550: 6520 5b33 5d5f 3b0a 2020 2020 2020 2020  e [3]_;.        
-00011560: 2020 2020 2a20 4d6f 6f6e 466c 656d 696e      * MoonFlemin
-00011570: 6720 5b34 5d5f 3b0a 2020 2020 2020 2020  g [4]_;.        
-00011580: 2020 2020 2a20 5769 6d6c 6579 5768 6974      * WimleyWhit
-00011590: 6520 5b35 5d5f 3b0a 2020 2020 2020 2020  e [5]_;.        
-000115a0: 2020 2020 2a20 5a68 616f 4c6f 6e64 6f6e      * ZhaoLondon
-000115b0: 205b 365d 5f2e 0a0a 2020 2020 6967 6e6f   [6]_...    igno
-000115c0: 7265 5f62 6163 6b62 6f6e 6520 3a20 626f  re_backbone : bo
-000115d0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-000115e0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-000115f0: 6967 6e6f 7265 2062 6163 6b62 6f6e 6520  ignore backbone 
-00011600: 6174 6f6d 7320 2843 2c20 4341 2c20 4e2c  atoms (C, CA, N,
-00011610: 204f 2920 7768 656e 2064 6566 696e 696e   O) when definin
-00011620: 6720 696e 7465 7266 6163 650a 2020 2020  g interface.    
-00011630: 2020 2020 7265 7369 6475 6573 2c20 6279      residues, by
-00011640: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
-00011650: 2020 2020 7365 6c65 6374 696f 6e20 3a20      selection : 
-00011660: 556e 696f 6e5b 4c69 7374 5b69 6e74 5d2c  Union[List[int],
-00011670: 204c 6973 745b 7374 725d 5d2c 206f 7074   List[str]], opt
-00011680: 696f 6e61 6c0a 2020 2020 2020 2020 4120  ional.        A 
-00011690: 6c69 7374 206f 6620 696e 7465 6765 7220  list of integer 
-000116a0: 6c61 6265 6c73 206f 7220 6120 6c69 7374  labels or a list
-000116b0: 206f 6620 6361 7669 7479 206e 616d 6573   of cavity names
-000116c0: 2074 6f20 6265 2073 656c 6563 7465 642c   to be selected,
-000116d0: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
-000116e0: 2e0a 2020 2020 6e74 6872 6561 6473 203a  ..    nthreads :
-000116f0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
-00011700: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-00011710: 2074 6872 6561 6473 2c20 6279 2064 6566   threads, by def
-00011720: 6175 6c74 204e 6f6e 652e 2049 6620 4e6f  ault None. If No
-00011730: 6e65 2c20 7468 6520 6e75 6d62 6572 206f  ne, the number o
-00011740: 6620 7468 7265 6164 7320 6973 0a20 2020  f threads is.   
-00011750: 2020 2020 2060 6f73 2e63 7075 5f63 6f75       `os.cpu_cou
-00011760: 6e74 2829 202d 2031 602e 0a20 2020 2076  nt() - 1`..    v
-00011770: 6572 626f 7365 203a 2062 6f6f 6c2c 206f  erbose : bool, o
-00011780: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00011790: 5072 696e 7420 6578 7472 6120 696e 666f  Print extra info
-000117a0: 726d 6174 696f 6e20 746f 2073 7461 6e64  rmation to stand
-000117b0: 6172 6420 6f75 7470 7574 2c20 6279 2064  ard output, by d
-000117c0: 6566 6175 6c74 2046 616c 7365 2e0a 0a20  efault False... 
-000117d0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-000117e0: 2d2d 2d2d 2d2d 0a20 2020 2073 6361 6c65  ------.    scale
-000117f0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
-00011800: 790a 2020 2020 2020 2020 4120 6e75 6d70  y.        A nump
-00011810: 792e 6e64 6172 7261 7920 7769 7468 2068  y.ndarray with h
-00011820: 7964 726f 7068 6f62 6963 6974 7920 7363  ydrophobicity sc
-00011830: 616c 6520 7661 6c75 6520 6d61 7070 6564  ale value mapped
-00011840: 2061 7420 7375 7266 6163 650a 2020 2020   at surface.    
-00011850: 2020 2020 706f 696e 7473 2028 7363 616c      points (scal
-00011860: 6573 5b6e 785d 5b6e 795d 5b6e 7a5d 292e  es[nx][ny][nz]).
-00011870: 0a20 2020 2061 7667 5f68 7964 726f 7061  .    avg_hydropa
-00011880: 7468 7920 3a20 4469 6374 5b73 7472 2c20  thy : Dict[str, 
-00011890: 666c 6f61 745d 0a20 2020 2020 2020 2041  float].        A
-000118a0: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
-000118b0: 2061 7665 7261 6765 2068 7964 726f 7061   average hydropa
-000118c0: 7468 7920 666f 7220 6561 6368 2064 6574  thy for each det
-000118d0: 6563 7465 6420 6361 7669 7479 2061 6e64  ected cavity and
-000118e0: 0a20 2020 2020 2020 2074 6865 2072 616e  .        the ran
-000118f0: 6765 206f 6620 7468 6520 6879 6472 6f70  ge of the hydrop
-00011900: 686f 6269 6369 7479 2073 6361 6c65 2028  hobicity scale (
-00011910: 6d69 6e2c 206d 6178 292e 0a0a 2020 2020  min, max)...    
-00011920: 5261 6973 6573 0a20 2020 202d 2d2d 2d2d  Raises.    -----
-00011930: 2d0a 2020 2020 5479 7065 4572 726f 720a  -.    TypeError.
-00011940: 2020 2020 2020 2020 6073 7572 6661 6365          `surface
-00011950: 6020 6d75 7374 2062 6520 6120 6e75 6d70  ` must be a nump
-00011960: 792e 6e64 6172 7261 792e 0a20 2020 2056  y.ndarray..    V
-00011970: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
-00011980: 2020 6073 7572 6661 6365 6020 6861 7320    `surface` has 
-00011990: 7468 6520 696e 636f 7272 6563 7420 7368  the incorrect sh
-000119a0: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
-000119b0: 286e 782c 206e 792c 206e 7a29 2e0a 2020  (nx, ny, nz)..  
-000119c0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-000119d0: 2020 2020 6061 746f 6d69 6360 206d 7573      `atomic` mus
-000119e0: 7420 6265 2061 206c 6973 7420 6f72 2061  t be a list or a
-000119f0: 206e 756d 7079 2e6e 6461 7272 6179 2e0a   numpy.ndarray..
-00011a00: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-00011a10: 2020 2020 2020 2060 6174 6f6d 6963 6020         `atomic` 
-00011a20: 6861 7320 696e 636f 7272 6563 7420 7368  has incorrect sh
-00011a30: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
-00011a40: 286e 2c20 3829 2e0a 2020 2020 5479 7065  (n, 8)..    Type
-00011a50: 4572 726f 720a 2020 2020 2020 2020 6076  Error.        `v
-00011a60: 6572 7469 6365 7360 206d 7573 7420 6265  ertices` must be
-00011a70: 2061 206c 6973 7420 6f72 2061 206e 756d   a list or a num
-00011a80: 7079 2e6e 6461 7272 6179 2e0a 2020 2020  py.ndarray..    
-00011a90: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-00011aa0: 2020 2060 7665 7274 6963 6573 6020 6861     `vertices` ha
-00011ab0: 7320 696e 636f 7272 6563 7420 7368 6170  s incorrect shap
-00011ac0: 652e 2049 7420 6d75 7374 2062 6520 2834  e. It must be (4
-00011ad0: 2c20 3329 2e0a 2020 2020 5479 7065 4572  , 3)..    TypeEr
-00011ae0: 726f 720a 2020 2020 2020 2020 6073 7465  ror.        `ste
-00011af0: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
-00011b00: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
-00011b10: 722e 0a20 2020 2056 616c 7565 4572 726f  r..    ValueErro
-00011b20: 720a 2020 2020 2020 2020 6073 7465 7060  r.        `step`
-00011b30: 206d 7573 7420 6265 2061 2070 6f73 6974   must be a posit
-00011b40: 6976 6520 7265 616c 206e 756d 6265 722e  ive real number.
-00011b50: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
-00011b60: 2020 2020 2020 2060 7072 6f62 655f 696e         `probe_in
-00011b70: 6020 6d75 7374 2062 6520 6120 6e6f 6e2d  ` must be a non-
-00011b80: 6e65 6761 7469 7665 2072 6561 6c20 6e75  negative real nu
-00011b90: 6d62 6572 2e0a 2020 2020 5661 6c75 6545  mber..    ValueE
-00011ba0: 7272 6f72 0a20 2020 2020 2020 2060 7072  rror.        `pr
-00011bb0: 6f62 655f 696e 6020 6d75 7374 2062 6520  obe_in` must be 
-00011bc0: 6120 6e6f 6e2d 6e65 6761 7469 7665 2072  a non-negative r
-00011bd0: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
-00011be0: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-00011bf0: 2020 6068 7964 726f 7068 6f62 6963 6974    `hydrophobicit
-00011c00: 795f 7363 616c 6560 206d 7573 7420 6265  y_scale` must be
-00011c10: 2061 2073 7472 696e 6720 6f72 2061 2070   a string or a p
-00011c20: 6174 686c 6962 2e50 6174 682e 0a20 2020  athlib.Path..   
-00011c30: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-00011c40: 2020 2060 6967 6e6f 7265 5f62 6163 6b62     `ignore_backb
-00011c50: 6f6e 6560 206d 7573 7420 6265 2061 2062  one` must be a b
-00011c60: 6f6f 6c65 616e 2e0a 2020 2020 5479 7065  oolean..    Type
-00011c70: 4572 726f 720a 2020 2020 2020 2020 6073  Error.        `s
-00011c80: 656c 6563 7469 6f6e 6020 6d75 7374 2062  election` must b
-00011c90: 6520 6120 6c69 7374 206f 6620 7374 7269  e a list of stri
-00011ca0: 6e67 7320 2863 6176 6974 7920 6e61 6d65  ngs (cavity name
-00011cb0: 7329 206f 7220 696e 7465 6765 7273 2028  s) or integers (
-00011cc0: 6361 7669 7479 206c 6162 656c 7329 2e0a  cavity labels)..
-00011cd0: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-00011ce0: 2020 2020 2020 2049 6e76 616c 6964 2060         Invalid `
-00011cf0: 7365 6c65 6374 696f 6e60 3a20 7b73 656c  selection`: {sel
-00011d00: 6563 7469 6f6e 7d2e 0a20 2020 2054 7970  ection}..    Typ
-00011d10: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-00011d20: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
-00011d30: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
-00011d40: 6567 6572 2e0a 2020 2020 5661 6c75 6545  eger..    ValueE
-00011d50: 7272 6f72 0a20 2020 2020 2020 2060 6e74  rror.        `nt
-00011d60: 6872 6561 6473 6020 6d75 7374 2062 6520  hreads` must be 
-00011d70: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
-00011d80: 6572 2e0a 2020 2020 5479 7065 4572 726f  er..    TypeErro
-00011d90: 720a 2020 2020 2020 2020 6076 6572 626f  r.        `verbo
-00011da0: 7365 6020 6d75 7374 2062 6520 6120 626f  se` must be a bo
-00011db0: 6f6c 6561 6e2e 0a0a 2020 2020 4e6f 7465  olean...    Note
-00011dc0: 0a20 2020 202d 2d2d 2d0a 2020 2020 5468  .    ----.    Th
-00011dd0: 6520 6361 7669 7479 206e 6f6d 656e 636c  e cavity nomencl
-00011de0: 6174 7572 6520 6973 2062 6173 6564 206f  ature is based o
-00011df0: 6e20 7468 6520 696e 7465 6765 7220 6c61  n the integer la
-00011e00: 6265 6c2e 2054 6865 2063 6176 6974 7920  bel. The cavity 
-00011e10: 6d61 726b 6564 0a20 2020 2077 6974 6820  marked.    with 
-00011e20: 322c 2074 6865 2066 6972 7374 2069 6e74  2, the first int
-00011e30: 6567 6572 2063 6f72 7265 7370 6f6e 6469  eger correspondi
-00011e40: 6e67 2074 6f20 6120 6361 7669 7479 2c20  ng to a cavity, 
-00011e50: 6973 204b 4141 2c20 7468 6520 6361 7669  is KAA, the cavi
-00011e60: 7479 0a20 2020 206d 6172 6b65 6420 7769  ty.    marked wi
-00011e70: 7468 2033 2069 7320 4b41 422c 2074 6865  th 3 is KAB, the
-00011e80: 2063 6176 6974 7920 6d61 726b 6564 2077   cavity marked w
-00011e90: 6974 6820 3420 6973 204b 4143 2061 6e64  ith 4 is KAC and
-00011ea0: 2073 6f20 6f6e 2e0a 0a20 2020 2053 6565   so on...    See
-00011eb0: 2041 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   Also.    ------
-00011ec0: 2d2d 0a20 2020 2072 6561 645f 7064 620a  --.    read_pdb.
-00011ed0: 2020 2020 7265 6164 5f78 797a 0a20 2020      read_xyz.   
-00011ee0: 2073 7061 7469 616c 0a20 2020 2065 7870   spatial.    exp
-00011ef0: 6f72 740a 2020 2020 7772 6974 655f 7265  ort.    write_re
-00011f00: 7375 6c74 730a 0a20 2020 2045 7861 6d70  sults..    Examp
-00011f10: 6c65 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  le.    -------. 
-00011f20: 2020 2057 6974 6820 7468 6520 7375 7266     With the surf
-00011f30: 6163 6520 706f 696e 7473 2069 6465 6e74  ace points ident
-00011f40: 6966 6965 6420 7769 7468 2060 6070 794b  ified with ``pyK
-00011f50: 5646 696e 6465 722e 7370 6174 6961 6c60  VFinder.spatial`
-00011f60: 6020 616e 6420 6174 6f6d 6963 2063 6f6f  ` and atomic coo
-00011f70: 7264 696e 6174 6573 2061 6e64 2069 6e66  rdinates and inf
-00011f80: 6f72 6d61 7469 6f6e 2072 6561 6420 7769  ormation read wi
-00011f90: 7468 2060 6070 794b 5646 696e 6465 722e  th ``pyKVFinder.
-00011fa0: 7265 6164 5f70 6462 6060 206f 7220 6060  read_pdb`` or ``
-00011fb0: 7079 4b56 4669 6e64 6572 2e72 6561 645f  pyKVFinder.read_
-00011fc0: 7879 7a60 602c 2077 6520 6361 6e20 7065  xyz``, we can pe
-00011fd0: 7266 6f72 6d20 6120 6879 6472 6f70 6174  rform a hydropat
-00011fe0: 6879 2063 6861 7261 6374 6572 697a 6174  hy characterizat
-00011ff0: 696f 6e2c 2074 6861 7420 6d61 7073 2061  ion, that maps a
-00012000: 2074 6172 6765 7420 6879 6472 6f70 686f   target hydropho
-00012010: 6269 6369 7479 2073 6361 6c65 206f 6e20  bicity scale on 
-00012020: 7375 7266 6163 6520 706f 696e 7473 2061  surface points a
-00012030: 6e64 2063 616c 6375 6c61 7465 2074 6865  nd calculate the
-00012040: 2061 7665 7261 6765 2068 7964 726f 7061   average hydropa
-00012050: 7468 790a 0a20 2020 203e 3e3e 2066 726f  thy..    >>> fro
-00012060: 6d20 7079 4b56 4669 6e64 6572 2069 6d70  m pyKVFinder imp
-00012070: 6f72 7420 6879 6472 6f70 6174 6879 0a20  ort hydropathy. 
-00012080: 2020 203e 3e3e 2073 6361 6c65 732c 2061     >>> scales, a
-00012090: 7667 5f68 7964 726f 7061 7468 7920 3d20  vg_hydropathy = 
-000120a0: 6879 6472 6f70 6174 6879 2873 7572 6661  hydropathy(surfa
-000120b0: 6365 2c20 6174 6f6d 6963 2c20 7665 7274  ce, atomic, vert
-000120c0: 6963 6573 290a 2020 2020 3e3e 3e20 7363  ices).    >>> sc
-000120d0: 616c 6573 0a20 2020 2061 7272 6179 285b  ales.    array([
-000120e0: 5b5b 302e 2c20 302e 2c20 302e 2c20 2e2e  [[0., 0., 0., ..
-000120f0: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
-00012100: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-00012110: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-00012120: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-00012130: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
-00012140: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
-00012150: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
-00012160: 2020 2e2e 2e2c 0a20 2020 2020 2020 2020    ...,.         
-00012170: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-00012180: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-00012190: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-000121a0: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-000121b0: 302e 2c20 302e 2c20 302e 5d2c 0a20 2020  0., 0., 0.],.   
-000121c0: 2020 2020 2020 2020 205b 302e 2c20 302e           [0., 0.
-000121d0: 2c20 302e 2c20 2e2e 2e2c 2030 2e2c 2030  , 0., ..., 0., 0
-000121e0: 2e2c 2030 2e5d 5d2c 0a20 2020 2020 2020  ., 0.]],.       
-000121f0: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00012200: 2020 5b5b 302e 2c20 302e 2c20 302e 2c20    [[0., 0., 0., 
-00012210: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-00012220: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-00012230: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-00012240: 302e 2c20 302e 2c20 302e 5d2c 0a20 2020  0., 0., 0.],.   
-00012250: 2020 2020 2020 2020 205b 302e 2c20 302e           [0., 0.
-00012260: 2c20 302e 2c20 2e2e 2e2c 2030 2e2c 2030  , 0., ..., 0., 0
-00012270: 2e2c 2030 2e5d 2c0a 2020 2020 2020 2020  ., 0.],.        
-00012280: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
-00012290: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
-000122a0: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
-000122b0: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-000122c0: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
-000122d0: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
-000122e0: 2020 2020 2020 2020 2020 205b 302e 2c20             [0., 
-000122f0: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
-00012300: 2030 2e2c 2030 2e5d 5d5d 290a 2020 2020   0., 0.]]]).    
-00012310: 3e3e 3e20 6176 675f 6879 6472 6f70 6174  >>> avg_hydropat
-00012320: 6879 0a20 2020 207b 274b 4141 273a 202d  hy.    {'KAA': -
-00012330: 302e 3733 2c20 274b 4142 273a 202d 302e  0.73, 'KAB': -0.
-00012340: 3035 2c20 274b 4143 273a 202d 302e 3037  05, 'KAC': -0.07
-00012350: 2c20 274b 4144 273a 202d 302e 3632 2c20  , 'KAD': -0.62, 
-00012360: 274b 4145 273a 202d 302e 3831 2c20 274b  'KAE': -0.81, 'K
-00012370: 4146 273a 202d 302e 3134 2c20 274b 4147  AF': -0.14, 'KAG
-00012380: 273a 202d 302e 3333 2c20 274b 4148 273a  ': -0.33, 'KAH':
-00012390: 202d 302e 3136 2c20 274b 4149 273a 202d   -0.16, 'KAI': -
-000123a0: 302e 342c 2027 4b41 4a27 3a20 302e 3632  0.4, 'KAJ': 0.62
-000123b0: 2c20 274b 414b 273a 202d 302e 3939 2c20  , 'KAK': -0.99, 
-000123c0: 274b 414c 273a 2030 2e33 362c 2027 4b41  'KAL': 0.36, 'KA
-000123d0: 4d27 3a20 2d30 2e33 332c 2027 4b41 4e27  M': -0.33, 'KAN'
-000123e0: 3a20 302e 3138 2c20 274b 414f 273a 2030  : 0.18, 'KAO': 0
-000123f0: 2e38 382c 2027 4b41 5027 3a20 2d30 2e39  .88, 'KAP': -0.9
-00012400: 362c 2027 4b41 5127 3a20 302e 3438 2c20  6, 'KAQ': 0.48, 
-00012410: 274b 4152 273a 2030 2e32 342c 2027 4569  'KAR': 0.24, 'Ei
-00012420: 7365 6e62 6572 6757 6569 7373 273a 205b  senbergWeiss': [
-00012430: 2d31 2e34 322c 2032 2e36 5d7d 0a0a 2020  -1.42, 2.6]}..  
-00012440: 2020 486f 7765 7665 722c 2075 7365 7273    However, users
-00012450: 206d 6179 206f 7074 2074 6f20 6967 6e6f   may opt to igno
-00012460: 7265 2062 6163 6b62 6f6e 6573 2063 6f6e  re backbones con
-00012470: 7461 6374 7320 2843 2c20 4341 2c20 4e2c  tacts (C, CA, N,
-00012480: 204f 2920 7769 7468 2074 6865 2063 6176   O) with the cav
-00012490: 6974 7920 7768 656e 206d 6170 7069 6e67  ity when mapping
-000124a0: 2068 7964 726f 7068 6f62 6963 6974 7920   hydrophobicity 
-000124b0: 7363 616c 6573 206f 6e20 7375 7266 6163  scales on surfac
-000124c0: 6520 706f 696e 7473 2e20 5468 656e 2c20  e points. Then, 
-000124d0: 7573 6572 7320 6d75 7374 2073 6574 2060  users must set `
-000124e0: 6069 676e 6f72 655f 6261 636b 626f 6e65  `ignore_backbone
-000124f0: 6060 2066 6c61 6720 746f 2060 6054 7275  `` flag to ``Tru
-00012500: 6560 602e 0a0a 2020 2020 3e3e 3e20 6672  e``...    >>> fr
-00012510: 6f6d 2070 794b 5646 696e 6465 7220 696d  om pyKVFinder im
-00012520: 706f 7274 2068 7964 726f 7061 7468 790a  port hydropathy.
-00012530: 2020 2020 3e3e 3e20 7363 616c 6573 2c20      >>> scales, 
-00012540: 6176 675f 6879 6472 6f70 6174 6879 203d  avg_hydropathy =
-00012550: 2068 7964 726f 7061 7468 7928 7375 7266   hydropathy(surf
-00012560: 6163 652c 2061 746f 6d69 632c 2076 6572  ace, atomic, ver
-00012570: 7469 6365 732c 2069 676e 6f72 655f 6261  tices, ignore_ba
-00012580: 636b 626f 6e65 3d54 7275 6529 0a20 2020  ckbone=True).   
-00012590: 203e 3e3e 2073 6361 6c65 730a 2020 2020   >>> scales.    
-000125a0: 6172 7261 7928 5b5b 5b30 2e2c 2030 2e2c  array([[[0., 0.,
-000125b0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-000125c0: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-000125d0: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-000125e0: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-000125f0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-00012600: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-00012610: 302e 2c20 302e 2c20 302e 5d2c 0a20 2020  0., 0., 0.],.   
-00012620: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
-00012630: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
-00012640: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-00012650: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
-00012660: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
-00012670: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
-00012680: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-00012690: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
-000126a0: 2c20 302e 2c20 302e 2c20 302e 5d5d 2c0a  , 0., 0., 0.]],.
-000126b0: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
-000126c0: 2020 2020 2020 2020 205b 5b30 2e2c 2030           [[0., 0
-000126d0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-000126e0: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
-000126f0: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
-00012700: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
-00012710: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-00012720: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
-00012730: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
-00012740: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
-00012750: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-00012760: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-00012770: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-00012780: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
-00012790: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
-000127a0: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
-000127b0: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
-000127c0: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d5d  .., 0., 0., 0.]]
-000127d0: 5d29 0a20 2020 203e 3e3e 2061 7667 5f68  ]).    >>> avg_h
-000127e0: 7964 726f 7061 7468 790a 2020 2020 7b27  ydropathy.    {'
-000127f0: 4b41 4127 3a20 2d30 2e37 2c20 274b 4142  KAA': -0.7, 'KAB
-00012800: 273a 2030 2e31 322c 2027 4b41 4327 3a20  ': 0.12, 'KAC': 
-00012810: 2d30 2e30 382c 2027 4b41 4427 3a20 2d30  -0.08, 'KAD': -0
-00012820: 2e35 362c 2027 4b41 4527 3a20 2d30 2e32  .56, 'KAE': -0.2
-00012830: 382c 2027 4b41 4627 3a20 2d30 2e32 352c  8, 'KAF': -0.25,
-00012840: 2027 4b41 4727 3a20 2d30 2e32 382c 2027   'KAG': -0.28, '
-00012850: 4b41 4827 3a20 2d30 2e30 392c 2027 4b41  KAH': -0.09, 'KA
-00012860: 4927 3a20 2d30 2e34 2c20 274b 414a 273a  I': -0.4, 'KAJ':
-00012870: 2030 2e39 362c 2027 4b41 4b27 3a20 2d30   0.96, 'KAK': -0
-00012880: 2e38 372c 2027 4b41 4c27 3a20 302e 3233  .87, 'KAL': 0.23
-00012890: 2c20 274b 414d 273a 2030 2e30 362c 2027  , 'KAM': 0.06, '
-000128a0: 4b41 4e27 3a20 2d30 2e31 2c20 274b 414f  KAN': -0.1, 'KAO
-000128b0: 273a 2030 2e39 392c 2027 4b41 5027 3a20  ': 0.99, 'KAP': 
-000128c0: 2d31 2e30 342c 2027 4b41 5127 3a20 302e  -1.04, 'KAQ': 0.
-000128d0: 3438 2c20 274b 4152 273a 202d 302e 3834  48, 'KAR': -0.84
-000128e0: 2c20 2745 6973 656e 6265 7267 5765 6973  , 'EisenbergWeis
-000128f0: 7327 3a20 5b2d 312e 3432 2c20 322e 365d  s': [-1.42, 2.6]
-00012900: 7d0a 0a20 2020 2052 6566 6572 656e 6365  }..    Reference
-00012910: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00012920: 0a20 2020 202e 2e20 5b31 5d20 4569 7365  .    .. [1] Eise
-00012930: 6e62 6572 6720 442c 2057 6569 7373 2052  nberg D, Weiss R
-00012940: 4d2c 2054 6572 7769 6c6c 6967 6572 2054  M, Terwilliger T
-00012950: 432e 2054 6865 2068 7964 726f 7068 6f62  C. The hydrophob
-00012960: 6963 206d 6f6d 656e 740a 2020 2020 2020  ic moment.      
-00012970: 2064 6574 6563 7473 2070 6572 696f 6469   detects periodi
-00012980: 6369 7479 2069 6e20 7072 6f74 6569 6e20  city in protein 
-00012990: 6879 6472 6f70 686f 6269 6369 7479 2e20  hydrophobicity. 
-000129a0: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
-000129b0: 6865 0a20 2020 2020 2020 4e61 7469 6f6e  he.       Nation
-000129c0: 616c 2041 6361 6465 6d79 206f 6620 5363  al Academy of Sc
-000129d0: 6965 6e63 6573 2e20 3139 3834 3b38 312e  iences. 1984;81.
-000129e0: 0a0a 2020 2020 2e2e 205b 325d 2048 6573  ..    .. [2] Hes
-000129f0: 7361 2054 2c20 4b69 6d20 482c 2042 6968  sa T, Kim H, Bih
-00012a00: 6c6d 6169 6572 204b 2c20 4c75 6e64 696e  lmaier K, Lundin
-00012a10: 2043 2c20 426f 656b 656c 204a 2c20 416e   C, Boekel J, An
-00012a20: 6465 7273 736f 6e20 482c 2065 7420 616c  dersson H, et al
-00012a30: 2e0a 2020 2020 2020 2052 6563 6f67 6e69  ..       Recogni
-00012a40: 7469 6f6e 206f 6620 7472 616e 736d 656d  tion of transmem
-00012a50: 6272 616e 6520 6865 6c69 6365 7320 6279  brane helices by
-00012a60: 2074 6865 2065 6e64 6f70 6c61 736d 6963   the endoplasmic
-00012a70: 2072 6574 6963 756c 756d 0a20 2020 2020   reticulum.     
-00012a80: 2020 7472 616e 736c 6f63 6f6e 2e20 4e61    translocon. Na
-00012a90: 7475 7265 2e20 3230 3035 3b34 3333 2e0a  ture. 2005;433..
-00012aa0: 0a20 2020 202e 2e20 5b33 5d20 4b79 7465  .    .. [3] Kyte
-00012ab0: 204a 2c20 446f 6f6c 6974 746c 6520 5246   J, Doolittle RF
-00012ac0: 2e20 4120 7369 6d70 6c65 206d 6574 686f  . A simple metho
-00012ad0: 6420 666f 7220 6469 7370 6c61 7969 6e67  d for displaying
-00012ae0: 2074 6865 2068 7964 726f 7061 7468 6963   the hydropathic
-00012af0: 0a20 2020 2020 2020 6368 6172 6163 7465  .       characte
-00012b00: 7220 6f66 2061 2070 726f 7465 696e 2e20  r of a protein. 
-00012b10: 4a6f 7572 6e61 6c20 6f66 204d 6f6c 6563  Journal of Molec
-00012b20: 756c 6172 2042 696f 6c6f 6779 2e20 3139  ular Biology. 19
-00012b30: 3832 3b31 3537 2e0a 0a20 2020 202e 2e20  82;157...    .. 
-00012b40: 5b34 5d20 4d6f 6f6e 2043 502c 2046 6c65  [4] Moon CP, Fle
-00012b50: 6d69 6e67 204b 472e 2053 6964 652d 6368  ming KG. Side-ch
-00012b60: 6169 6e20 6879 6472 6f70 686f 6269 6369  ain hydrophobici
-00012b70: 7479 2073 6361 6c65 2064 6572 6976 6564  ty scale derived
-00012b80: 2066 726f 6d0a 2020 2020 2020 2074 7261   from.       tra
-00012b90: 6e73 6d65 6d62 7261 6e65 2070 726f 7465  nsmembrane prote
-00012ba0: 696e 2066 6f6c 6469 6e67 2069 6e74 6f20  in folding into 
-00012bb0: 6c69 7069 6420 6269 6c61 7965 7273 2e20  lipid bilayers. 
-00012bc0: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
-00012bd0: 6865 0a20 2020 2020 2020 4e61 7469 6f6e  he.       Nation
-00012be0: 616c 2041 6361 6465 6d79 206f 6620 5363  al Academy of Sc
-00012bf0: 6965 6e63 6573 2e20 3230 3131 3b31 3038  iences. 2011;108
-00012c00: 2e0a 0a20 2020 202e 2e20 5b35 5d20 5769  ...    .. [5] Wi
-00012c10: 6d6c 6579 2057 432c 2057 6869 7465 2053  mley WC, White S
-00012c20: 482e 2045 7870 6572 696d 656e 7461 6c6c  H. Experimentall
-00012c30: 7920 6465 7465 726d 696e 6564 2068 7964  y determined hyd
-00012c40: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
-00012c50: 650a 2020 2020 2020 2066 6f72 2070 726f  e.       for pro
-00012c60: 7465 696e 7320 6174 206d 656d 6272 616e  teins at membran
-00012c70: 6520 696e 7465 7266 6163 6573 2e20 4e61  e interfaces. Na
-00012c80: 7475 7265 2053 7472 7563 7475 7261 6c20  ture Structural 
-00012c90: 2620 4d6f 6c65 6375 6c61 720a 2020 2020  & Molecular.    
-00012ca0: 2020 2042 696f 6c6f 6779 2e20 3139 3936     Biology. 1996
-00012cb0: 3b33 2e0a 0a20 2020 202e 2e20 5b36 5d20  ;3...    .. [6] 
-00012cc0: 5a68 616f 2047 2c20 4c6f 6e64 6f6e 2045  Zhao G, London E
-00012cd0: 2e20 416e 2061 6d69 6e6f 2061 6369 6420  . An amino acid 
-00012ce0: e280 9c74 7261 6e73 6d65 6d62 7261 6e65  ...transmembrane
-00012cf0: 2074 656e 6465 6e63 79e2 809d 2073 6361   tendency... sca
-00012d00: 6c65 2074 6861 740a 2020 2020 2020 2061  le that.       a
-00012d10: 7070 726f 6163 6865 7320 7468 6520 7468  pproaches the th
-00012d20: 656f 7265 7469 6361 6c20 6c69 6d69 7420  eoretical limit 
-00012d30: 746f 2061 6363 7572 6163 7920 666f 7220  to accuracy for 
-00012d40: 7072 6564 6963 7469 6f6e 206f 660a 2020  prediction of.  
-00012d50: 2020 2020 2074 7261 6e73 6d65 6d62 7261       transmembra
-00012d60: 6e65 2068 656c 6963 6573 3a20 5265 6c61  ne helices: Rela
-00012d70: 7469 6f6e 7368 6970 2074 6f20 6269 6f6c  tionship to biol
-00012d80: 6f67 6963 616c 2068 7964 726f 7068 6f62  ogical hydrophob
-00012d90: 6963 6974 792e 0a20 2020 2020 2020 5072  icity..       Pr
-00012da0: 6f74 6569 6e20 5363 6965 6e63 652e 2032  otein Science. 2
-00012db0: 3030 363b 3135 2e0a 2020 2020 2222 220a  006;15..    """.
-00012dc0: 2020 2020 696d 706f 7274 2074 6f6d 6c0a      import toml.
-00012dd0: 2020 2020 6672 6f6d 205f 7079 4b56 4669      from _pyKVFi
-00012de0: 6e64 6572 2069 6d70 6f72 7420 5f68 7964  nder import _hyd
-00012df0: 726f 7061 7468 790a 0a20 2020 2023 2043  ropathy..    # C
-00012e00: 6865 636b 2061 7267 756d 656e 7473 0a20  heck arguments. 
-00012e10: 2020 2069 6620 7479 7065 2873 7572 6661     if type(surfa
-00012e20: 6365 2920 6e6f 7420 696e 205b 6e75 6d70  ce) not in [nump
-00012e30: 792e 6e64 6172 7261 795d 3a0a 2020 2020  y.ndarray]:.    
-00012e40: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-00012e50: 726f 7228 2260 7375 7266 6163 6560 206d  ror("`surface` m
-00012e60: 7573 7420 6265 2061 206e 756d 7079 2e6e  ust be a numpy.n
-00012e70: 6461 7272 6179 2e22 290a 2020 2020 656c  darray.").    el
-00012e80: 6966 206c 656e 2873 7572 6661 6365 2e73  if len(surface.s
-00012e90: 6861 7065 2920 213d 2033 3a0a 2020 2020  hape) != 3:.    
-00012ea0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00012eb0: 7272 6f72 2822 6073 7572 6661 6365 6020  rror("`surface` 
-00012ec0: 6861 7320 7468 6520 696e 636f 7272 6563  has the incorrec
-00012ed0: 7420 7368 6170 652e 2049 7420 6d75 7374  t shape. It must
-00012ee0: 2062 6520 286e 782c 206e 792c 206e 7a29   be (nx, ny, nz)
-00012ef0: 2e22 290a 2020 2020 6966 2074 7970 6528  .").    if type(
-00012f00: 6174 6f6d 6963 2920 6e6f 7420 696e 205b  atomic) not in [
-00012f10: 6e75 6d70 792e 6e64 6172 7261 792c 206c  numpy.ndarray, l
-00012f20: 6973 745d 3a0a 2020 2020 2020 2020 7261  ist]:.        ra
-00012f30: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-00012f40: 6174 6f6d 6963 6020 6d75 7374 2062 6520  atomic` must be 
-00012f50: 6120 6c69 7374 206f 7220 6120 6e75 6d70  a list or a nump
-00012f60: 792e 6e64 6172 7261 792e 2229 0a20 2020  y.ndarray.").   
-00012f70: 2065 6c69 6620 6c65 6e28 6e75 6d70 792e   elif len(numpy.
-00012f80: 6173 6172 7261 7928 6174 6f6d 6963 292e  asarray(atomic).
-00012f90: 7368 6170 6529 2021 3d20 323a 0a20 2020  shape) != 2:.   
-00012fa0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00012fb0: 4572 726f 7228 2260 6174 6f6d 6963 6020  Error("`atomic` 
-00012fc0: 6861 7320 696e 636f 7272 6563 7420 7368  has incorrect sh
-00012fd0: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
-00012fe0: 286e 2c20 3829 2e22 290a 2020 2020 656c  (n, 8).").    el
-00012ff0: 6966 206e 756d 7079 2e61 7361 7272 6179  if numpy.asarray
-00013000: 2861 746f 6d69 6329 2e73 6861 7065 5b31  (atomic).shape[1
-00013010: 5d20 213d 2038 3a0a 2020 2020 2020 2020  ] != 8:.        
-00013020: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00013030: 2822 6061 746f 6d69 6360 2068 6173 2069  ("`atomic` has i
-00013040: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
-00013050: 4974 206d 7573 7420 6265 2028 6e2c 2038  It must be (n, 8
-00013060: 292e 2229 0a20 2020 2069 6620 7479 7065  ).").    if type
-00013070: 2876 6572 7469 6365 7329 206e 6f74 2069  (vertices) not i
-00013080: 6e20 5b6e 756d 7079 2e6e 6461 7272 6179  n [numpy.ndarray
-00013090: 2c20 6c69 7374 5d3a 0a20 2020 2020 2020  , list]:.       
-000130a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000130b0: 2822 6076 6572 7469 6365 7360 206d 7573  ("`vertices` mus
-000130c0: 7420 6265 2061 206c 6973 7420 6f72 2061  t be a list or a
-000130d0: 206e 756d 7079 2e6e 6461 7272 6179 2e22   numpy.ndarray."
-000130e0: 290a 2020 2020 656c 6966 206e 756d 7079  ).    elif numpy
-000130f0: 2e61 7361 7272 6179 2876 6572 7469 6365  .asarray(vertice
-00013100: 7329 2e73 6861 7065 2021 3d20 2834 2c20  s).shape != (4, 
-00013110: 3329 3a0a 2020 2020 2020 2020 7261 6973  3):.        rais
-00013120: 6520 5661 6c75 6545 7272 6f72 2822 6076  e ValueError("`v
-00013130: 6572 7469 6365 7360 2068 6173 2069 6e63  ertices` has inc
-00013140: 6f72 7265 6374 2073 6861 7065 2e20 4974  orrect shape. It
-00013150: 206d 7573 7420 6265 2028 342c 2033 292e   must be (4, 3).
-00013160: 2229 0a20 2020 2069 6620 7479 7065 2873  ").    if type(s
-00013170: 7465 7029 206e 6f74 2069 6e20 5b66 6c6f  tep) not in [flo
-00013180: 6174 2c20 696e 745d 3a0a 2020 2020 2020  at, int]:.      
-00013190: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-000131a0: 7228 2260 7374 6570 6020 6d75 7374 2062  r("`step` must b
-000131b0: 6520 6120 706f 7369 7469 7665 2072 6561  e a positive rea
-000131c0: 6c20 6e75 6d62 6572 2e22 290a 2020 2020  l number.").    
-000131d0: 656c 6966 2073 7465 7020 3c3d 2030 2e30  elif step <= 0.0
-000131e0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-000131f0: 5661 6c75 6545 7272 6f72 2822 6073 7465  ValueError("`ste
-00013200: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
-00013210: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
-00013220: 722e 2229 0a20 2020 2069 6620 7479 7065  r.").    if type
-00013230: 2870 726f 6265 5f69 6e29 206e 6f74 2069  (probe_in) not i
-00013240: 6e20 5b66 6c6f 6174 2c20 696e 745d 3a0a  n [float, int]:.
-00013250: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00013260: 7065 4572 726f 7228 2260 7072 6f62 655f  peError("`probe_
-00013270: 696e 6020 6d75 7374 2062 6520 6120 6e6f  in` must be a no
-00013280: 6e2d 6e65 6761 7469 7665 2072 6561 6c20  n-negative real 
-00013290: 6e75 6d62 6572 2e22 290a 2020 2020 656c  number.").    el
-000132a0: 6966 2070 726f 6265 5f69 6e20 3c20 302e  if probe_in < 0.
-000132b0: 303a 0a20 2020 2020 2020 2072 6169 7365  0:.        raise
-000132c0: 2056 616c 7565 4572 726f 7228 2260 7072   ValueError("`pr
-000132d0: 6f62 655f 696e 6020 6d75 7374 2062 6520  obe_in` must be 
-000132e0: 6120 6e6f 6e2d 6e65 6761 7469 7665 2072  a non-negative r
-000132f0: 6561 6c20 6e75 6d62 6572 2e22 290a 2020  eal number.").  
-00013300: 2020 6966 2074 7970 6528 6879 6472 6f70    if type(hydrop
-00013310: 686f 6269 6369 7479 5f73 6361 6c65 2920  hobicity_scale) 
-00013320: 6e6f 7420 696e 205b 7374 722c 2070 6174  not in [str, pat
-00013330: 686c 6962 2e50 6174 685d 3a0a 2020 2020  hlib.Path]:.    
-00013340: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-00013350: 726f 7228 2260 6879 6472 6f70 686f 6269  ror("`hydrophobi
-00013360: 6369 7479 5f73 6361 6c65 6020 6d75 7374  city_scale` must
-00013370: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
-00013380: 6120 7061 7468 6c69 622e 5061 7468 2e22  a pathlib.Path."
-00013390: 290a 2020 2020 6966 2074 7970 6528 6967  ).    if type(ig
-000133a0: 6e6f 7265 5f62 6163 6b62 6f6e 6529 206e  nore_backbone) n
-000133b0: 6f74 2069 6e20 5b62 6f6f 6c5d 3a0a 2020  ot in [bool]:.  
-000133c0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-000133d0: 4572 726f 7228 2260 6967 6e6f 7265 5f62  Error("`ignore_b
-000133e0: 6163 6b62 6f6e 6560 206d 7573 7420 6265  ackbone` must be
-000133f0: 2061 2062 6f6f 6c65 616e 2e22 290a 2020   a boolean.").  
-00013400: 2020 6966 2073 656c 6563 7469 6f6e 2069    if selection i
-00013410: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00013420: 2020 2020 2320 4368 6563 6b20 7365 6c65      # Check sele
-00013430: 6374 696f 6e20 7479 7065 730a 2020 2020  ction types.    
-00013440: 2020 2020 6966 2061 6c6c 2869 7369 6e73      if all(isins
-00013450: 7461 6e63 6528 782c 2069 6e74 2920 666f  tance(x, int) fo
-00013460: 7220 7820 696e 2073 656c 6563 7469 6f6e  r x in selection
-00013470: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-00013480: 6173 730a 2020 2020 2020 2020 656c 6966  ass.        elif
-00013490: 2061 6c6c 2869 7369 6e73 7461 6e63 6528   all(isinstance(
-000134a0: 782c 2073 7472 2920 666f 7220 7820 696e  x, str) for x in
-000134b0: 2073 656c 6563 7469 6f6e 293a 0a20 2020   selection):.   
-000134c0: 2020 2020 2020 2020 2073 656c 6563 7469           selecti
-000134d0: 6f6e 203d 205b 5f67 6574 5f63 6176 6974  on = [_get_cavit
-000134e0: 795f 6c61 6265 6c28 7365 6c65 2920 666f  y_label(sele) fo
-000134f0: 7220 7365 6c65 2069 6e20 7365 6c65 6374  r sele in select
-00013500: 696f 6e5d 0a20 2020 2020 2020 2065 6c73  ion].        els
-00013510: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013520: 6169 7365 2054 7970 6545 7272 6f72 280a  aise TypeError(.
-00013530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013540: 2260 7365 6c65 6374 696f 6e60 206d 7573  "`selection` mus
-00013550: 7420 6265 2061 206c 6973 7420 6f66 2073  t be a list of s
-00013560: 7472 696e 6773 2028 6361 7669 7479 206e  trings (cavity n
-00013570: 616d 6573 2920 6f72 2069 6e74 6567 6572  ames) or integer
-00013580: 7320 2863 6176 6974 7920 6c61 6265 6c73  s (cavity labels
-00013590: 292e 220a 2020 2020 2020 2020 2020 2020  ).".            
-000135a0: 290a 2020 2020 2020 2020 2320 4368 6563  ).        # Chec
-000135b0: 6b20 6966 2073 656c 6563 7469 6f6e 2069  k if selection i
-000135c0: 6e63 6c75 6465 7320 7661 6c69 6420 6361  ncludes valid ca
-000135d0: 7669 7479 206c 6162 656c 730a 2020 2020  vity labels.    
-000135e0: 2020 2020 6966 2061 6e79 2878 203c 2032      if any(x < 2
-000135f0: 2066 6f72 2078 2069 6e20 7365 6c65 6374   for x in select
-00013600: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
-00013610: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00013620: 6f72 2866 2249 6e76 616c 6964 2060 7365  or(f"Invalid `se
-00013630: 6c65 6374 696f 6e60 3a20 7b73 656c 6563  lection`: {selec
-00013640: 7469 6f6e 7d2e 2229 0a20 2020 2069 6620  tion}.").    if 
-00013650: 6e74 6872 6561 6473 2069 7320 4e6f 6e65  nthreads is None
-00013660: 3a0a 2020 2020 2020 2020 6e74 6872 6561  :.        nthrea
-00013670: 6473 203d 206f 732e 6370 755f 636f 756e  ds = os.cpu_coun
-00013680: 7428 2920 2d20 310a 2020 2020 656c 7365  t() - 1.    else
-00013690: 3a0a 2020 2020 2020 2020 6966 2074 7970  :.        if typ
-000136a0: 6528 6e74 6872 6561 6473 2920 6e6f 7420  e(nthreads) not 
-000136b0: 696e 205b 696e 745d 3a0a 2020 2020 2020  in [int]:.      
-000136c0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-000136d0: 4572 726f 7228 2260 6e74 6872 6561 6473  Error("`nthreads
-000136e0: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
-000136f0: 7469 7665 2069 6e74 6567 6572 2e22 290a  tive integer.").
-00013700: 2020 2020 2020 2020 656c 6966 206e 7468          elif nth
-00013710: 7265 6164 7320 3c3d 2030 3a0a 2020 2020  reads <= 0:.    
-00013720: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00013730: 6c75 6545 7272 6f72 2822 606e 7468 7265  lueError("`nthre
-00013740: 6164 7360 206d 7573 7420 6265 2061 2070  ads` must be a p
-00013750: 6f73 6974 6976 6520 696e 7465 6765 722e  ositive integer.
-00013760: 2229 0a20 2020 2069 6620 7479 7065 2876  ").    if type(v
-00013770: 6572 626f 7365 2920 6e6f 7420 696e 205b  erbose) not in [
-00013780: 626f 6f6c 5d3a 0a20 2020 2020 2020 2072  bool]:.        r
-00013790: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-000137a0: 6076 6572 626f 7365 6020 6d75 7374 2062  `verbose` must b
-000137b0: 6520 6120 626f 6f6c 6561 6e2e 2229 0a0a  e a boolean.")..
-000137c0: 2020 2020 2320 436f 6e76 6572 7420 7479      # Convert ty
-000137d0: 7065 730a 2020 2020 6966 2074 7970 6528  pes.    if type(
-000137e0: 6174 6f6d 6963 2920 3d3d 206c 6973 743a  atomic) == list:
-000137f0: 0a20 2020 2020 2020 2061 746f 6d69 6320  .        atomic 
-00013800: 3d20 6e75 6d70 792e 6173 6172 7261 7928  = numpy.asarray(
-00013810: 6174 6f6d 6963 290a 2020 2020 6966 2074  atomic).    if t
-00013820: 7970 6528 7665 7274 6963 6573 2920 3d3d  ype(vertices) ==
-00013830: 206c 6973 743a 0a20 2020 2020 2020 2076   list:.        v
-00013840: 6572 7469 6365 7320 3d20 6e75 6d70 792e  ertices = numpy.
-00013850: 6173 6172 7261 7928 7665 7274 6963 6573  asarray(vertices
-00013860: 290a 2020 2020 6966 2074 7970 6528 7374  ).    if type(st
-00013870: 6570 2920 3d3d 2069 6e74 3a0a 2020 2020  ep) == int:.    
-00013880: 2020 2020 7374 6570 203d 2066 6c6f 6174      step = float
-00013890: 2873 7465 7029 0a20 2020 2069 6620 7479  (step).    if ty
-000138a0: 7065 2870 726f 6265 5f69 6e29 203d 3d20  pe(probe_in) == 
-000138b0: 696e 743a 0a20 2020 2020 2020 2070 726f  int:.        pro
-000138c0: 6265 5f69 6e20 3d20 666c 6f61 7428 7072  be_in = float(pr
-000138d0: 6f62 655f 696e 290a 0a20 2020 2023 2043  obe_in)..    # C
-000138e0: 6f6e 7665 7274 206e 756d 7079 2e6e 6461  onvert numpy.nda
-000138f0: 7272 6179 2064 6174 6120 7479 7065 730a  rray data types.
-00013900: 2020 2020 7375 7266 6163 6520 3d20 7375      surface = su
-00013910: 7266 6163 652e 6173 7479 7065 2822 696e  rface.astype("in
-00013920: 7433 3222 2920 6966 2073 7572 6661 6365  t32") if surface
-00013930: 2e64 7479 7065 2021 3d20 2269 6e74 3332  .dtype != "int32
-00013940: 2220 656c 7365 2073 7572 6661 6365 0a20  " else surface. 
-00013950: 2020 2076 6572 7469 6365 7320 3d20 7665     vertices = ve
-00013960: 7274 6963 6573 2e61 7374 7970 6528 2266  rtices.astype("f
-00013970: 6c6f 6174 3634 2229 2069 6620 7665 7274  loat64") if vert
-00013980: 6963 6573 2e64 7479 7065 2021 3d20 2266  ices.dtype != "f
-00013990: 6c6f 6174 3634 2220 656c 7365 2076 6572  loat64" else ver
-000139a0: 7469 6365 730a 0a20 2020 2023 2045 7874  tices..    # Ext
-000139b0: 7261 6374 2061 746f 6d69 6e66 6f20 6672  ract atominfo fr
-000139c0: 6f6d 2061 746f 6d69 630a 2020 2020 6174  om atomic.    at
-000139d0: 6f6d 696e 666f 203d 206e 756d 7079 2e61  ominfo = numpy.a
-000139e0: 7361 7272 6179 280a 2020 2020 2020 2020  sarray(.        
-000139f0: 285b 5b66 227b 6174 6f6d 5b30 5d7d 5f7b  ([[f"{atom[0]}_{
-00013a00: 6174 6f6d 5b31 5d7d 5f7b 6174 6f6d 5b32  atom[1]}_{atom[2
-00013a10: 5d7d 222c 2061 746f 6d5b 335d 5d20 666f  ]}", atom[3]] fo
-00013a20: 7220 6174 6f6d 2069 6e20 6174 6f6d 6963  r atom in atomic
-00013a30: 5b3a 2c20 3a34 5d5d 290a 2020 2020 290a  [:, :4]]).    ).
-00013a40: 0a20 2020 2023 2045 7874 7261 6374 2078  .    # Extract x
-00013a50: 797a 7220 6672 6f6d 2061 746f 6d69 630a  yzr from atomic.
-00013a60: 2020 2020 7879 7a72 203d 2061 746f 6d69      xyzr = atomi
-00013a70: 635b 3a2c 2034 3a5d 2e61 7374 7970 6528  c[:, 4:].astype(
-00013a80: 6e75 6d70 792e 666c 6f61 7436 3429 0a0a  numpy.float64)..
-00013a90: 2020 2020 2320 4765 7420 6e75 6d62 6572      # Get number
-00013aa0: 206f 6620 6361 7669 7469 6573 0a20 2020   of cavities.   
-00013ab0: 206e 6361 7620 3d20 696e 7428 7375 7266   ncav = int(surf
-00013ac0: 6163 652e 6d61 7828 2920 2d20 3129 0a0a  ace.max() - 1)..
-00013ad0: 2020 2020 2320 4765 7420 7369 6e63 6f73      # Get sincos
-00013ae0: 3a20 7369 6e65 2061 6e64 2063 6f73 7369  : sine and cossi
-00013af0: 6e65 206f 6620 7468 6520 6772 6964 2072  ne of the grid r
-00013b00: 6f74 6174 696f 6e20 616e 676c 6573 2028  otation angles (
-00013b10: 7369 6e61 2c20 636f 7361 2c20 7369 6e62  sina, cosa, sinb
-00013b20: 2c20 636f 7362 290a 2020 2020 7369 6e63  , cosb).    sinc
-00013b30: 6f73 203d 205f 6765 745f 7369 6e63 6f73  os = _get_sincos
-00013b40: 2876 6572 7469 6365 7329 0a0a 2020 2020  (vertices)..    
-00013b50: 2320 5365 6c65 6374 2063 6176 6974 6965  # Select cavitie
-00013b60: 730a 2020 2020 6966 2073 656c 6563 7469  s.    if selecti
-00013b70: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00013b80: 2020 2020 2020 2020 7375 7266 6163 6520          surface 
-00013b90: 3d20 5f73 656c 6563 745f 6361 7669 7469  = _select_caviti
-00013ba0: 6573 2873 7572 6661 6365 2c20 7365 6c65  es(surface, sele
-00013bb0: 6374 696f 6e29 0a0a 2020 2020 2320 4765  ction)..    # Ge
-00013bc0: 7420 6469 6d65 6e73 696f 6e73 0a20 2020  t dimensions.   
-00013bd0: 206e 782c 206e 792c 206e 7a20 3d20 7375   nx, ny, nz = su
-00013be0: 7266 6163 652e 7368 6170 650a 2020 2020  rface.shape.    
-00013bf0: 6e76 6f78 656c 7320 3d20 6e78 202a 206e  nvoxels = nx * n
-00013c00: 7920 2a20 6e7a 0a0a 2020 2020 2320 4c6f  y * nz..    # Lo
-00013c10: 6164 2068 7964 726f 7068 6f62 6963 6974  ad hydrophobicit
-00013c20: 7920 7363 616c 6573 0a20 2020 2069 6620  y scales.    if 
-00013c30: 6879 6472 6f70 686f 6269 6369 7479 5f73  hydrophobicity_s
-00013c40: 6361 6c65 2069 6e20 5b0a 2020 2020 2020  cale in [.      
-00013c50: 2020 2245 6973 656e 6265 7267 5765 6973    "EisenbergWeis
-00013c60: 7322 2c0a 2020 2020 2020 2020 2248 6573  s",.        "Hes
-00013c70: 7361 4865 696a 6e65 222c 0a20 2020 2020  saHeijne",.     
-00013c80: 2020 2022 4b79 7465 446f 6f6c 6974 746c     "KyteDoolittl
-00013c90: 6522 2c0a 2020 2020 2020 2020 224d 6f6f  e",.        "Moo
-00013ca0: 6e46 6c65 6d69 6e67 222c 0a20 2020 2020  nFleming",.     
-00013cb0: 2020 2022 5769 6d6c 6579 5768 6974 6522     "WimleyWhite"
-00013cc0: 2c0a 2020 2020 2020 2020 225a 6861 6f4c  ,.        "ZhaoL
-00013cd0: 6f6e 646f 6e22 2c0a 2020 2020 5d3a 0a20  ondon",.    ]:. 
-00013ce0: 2020 2020 2020 2068 7964 726f 7068 6f62         hydrophob
-00013cf0: 6963 6974 795f 7363 616c 6520 3d20 6f73  icity_scale = os
-00013d00: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00013d10: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
-00013d20: 6162 7370 6174 6828 6f73 2e70 6174 682e  abspath(os.path.
-00013d30: 6469 726e 616d 6528 5f5f 6669 6c65 5f5f  dirname(__file__
-00013d40: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00013d50: 6622 6461 7461 2f7b 6879 6472 6f70 686f  f"data/{hydropho
-00013d60: 6269 6369 7479 5f73 6361 6c65 7d2e 746f  bicity_scale}.to
-00013d70: 6d6c 222c 0a20 2020 2020 2020 2029 0a20  ml",.        ). 
-00013d80: 2020 2066 203d 2074 6f6d 6c2e 6c6f 6164     f = toml.load
-00013d90: 2868 7964 726f 7068 6f62 6963 6974 795f  (hydrophobicity_
-00013da0: 7363 616c 6529 0a20 2020 2064 6174 612c  scale).    data,
-00013db0: 206e 616d 6520 3d20 6c69 7374 2866 2e76   name = list(f.v
-00013dc0: 616c 7565 7328 2929 5b30 5d2c 206c 6973  alues())[0], lis
-00013dd0: 7428 662e 6b65 7973 2829 295b 305d 0a20  t(f.keys())[0]. 
-00013de0: 2020 2072 6573 6e2c 2073 6361 6c65 203d     resn, scale =
-00013df0: 206c 6973 7428 6461 7461 2e6b 6579 7328   list(data.keys(
-00013e00: 2929 2c20 6e75 6d70 792e 6173 6172 7261  )), numpy.asarra
-00013e10: 7928 6c69 7374 2864 6174 612e 7661 6c75  y(list(data.valu
-00013e20: 6573 2829 2929 0a0a 2020 2020 2320 556e  es()))..    # Un
-00013e30: 7061 636b 2076 6572 7469 6365 730a 2020  pack vertices.  
-00013e40: 2020 5031 2c20 5032 2c20 5033 2c20 5034    P1, P2, P3, P4
-00013e50: 203d 2076 6572 7469 6365 730a 0a20 2020   = vertices..   
-00013e60: 2023 2052 656d 6f76 6520 6261 636b 626f   # Remove backbo
-00013e70: 6e65 2066 726f 6d20 6174 6f6d 696e 666f  ne from atominfo
-00013e80: 0a20 2020 2069 6620 6967 6e6f 7265 5f62  .    if ignore_b
-00013e90: 6163 6b62 6f6e 653a 0a20 2020 2020 2020  ackbone:.       
-00013ea0: 206d 6173 6b20 3d20 6e75 6d70 792e 7768   mask = numpy.wh
-00013eb0: 6572 6528 0a20 2020 2020 2020 2020 2020  ere(.           
-00013ec0: 2028 6174 6f6d 696e 666f 5b3a 2c20 315d   (atominfo[:, 1]
-00013ed0: 2021 3d20 2243 2229 0a20 2020 2020 2020   != "C").       
-00013ee0: 2020 2020 2026 2028 6174 6f6d 696e 666f       & (atominfo
-00013ef0: 5b3a 2c20 315d 2021 3d20 2243 4122 290a  [:, 1] != "CA").
-00013f00: 2020 2020 2020 2020 2020 2020 2620 2861              & (a
-00013f10: 746f 6d69 6e66 6f5b 3a2c 2031 5d20 213d  tominfo[:, 1] !=
-00013f20: 2022 4e22 290a 2020 2020 2020 2020 2020   "N").          
-00013f30: 2020 2620 2861 746f 6d69 6e66 6f5b 3a2c    & (atominfo[:,
-00013f40: 2031 5d20 213d 2022 4f22 290a 2020 2020   1] != "O").    
-00013f50: 2020 2020 290a 2020 2020 2020 2020 6174      ).        at
-00013f60: 6f6d 696e 666f 203d 2061 746f 6d69 6e66  ominfo = atominf
-00013f70: 6f5b 6d61 736b 5b30 5d2c 5d0a 2020 2020  o[mask[0],].    
-00013f80: 2020 2020 7879 7a72 203d 2078 797a 725b      xyzr = xyzr[
-00013f90: 6d61 736b 5b30 5d2c 5d0a 0a20 2020 2023  mask[0],]..    #
-00013fa0: 2047 6574 2072 6573 6964 7565 206e 616d   Get residue nam
-00013fb0: 6520 6672 6f6d 2061 746f 6d69 6e66 6f0a  e from atominfo.
-00013fc0: 2020 2020 7265 736e 616d 6520 3d20 6c69      resname = li
-00013fd0: 7374 286d 6170 286c 616d 6264 6120 783a  st(map(lambda x:
-00013fe0: 2078 2e73 706c 6974 2822 5f22 295b 325d   x.split("_")[2]
-00013ff0: 2c20 6174 6f6d 696e 666f 5b3a 2c20 305d  , atominfo[:, 0]
-00014000: 2929 0a0a 2020 2020 2320 4765 7420 6879  ))..    # Get hy
-00014010: 6472 6f70 686f 6269 6369 7479 2073 6361  drophobicity sca
-00014020: 6c65 7320 696e 2033 4420 6772 6964 2061  les in 3D grid a
-00014030: 6e64 2061 7665 7261 6765 2068 7964 726f  nd average hydro
-00014040: 7061 7468 790a 2020 2020 7363 616c 6573  pathy.    scales
-00014050: 2c20 6176 675f 6879 6472 6f70 6174 6879  , avg_hydropathy
-00014060: 203d 205f 6879 6472 6f70 6174 6879 280a   = _hydropathy(.
-00014070: 2020 2020 2020 2020 6e76 6f78 656c 732c          nvoxels,
-00014080: 0a20 2020 2020 2020 206e 6361 762c 0a20  .        ncav,. 
-00014090: 2020 2020 2020 2073 7572 6661 6365 2c0a         surface,.
-000140a0: 2020 2020 2020 2020 7879 7a72 2c0a 2020          xyzr,.  
-000140b0: 2020 2020 2020 5031 2c0a 2020 2020 2020        P1,.      
-000140c0: 2020 7369 6e63 6f73 2c0a 2020 2020 2020    sincos,.      
-000140d0: 2020 7265 736e 616d 652c 0a20 2020 2020    resname,.     
-000140e0: 2020 2072 6573 6e2c 0a20 2020 2020 2020     resn,.       
-000140f0: 2073 6361 6c65 2c0a 2020 2020 2020 2020   scale,.        
-00014100: 7374 6570 2c0a 2020 2020 2020 2020 7072  step,.        pr
-00014110: 6f62 655f 696e 2c0a 2020 2020 2020 2020  obe_in,.        
-00014120: 6e74 6872 6561 6473 2c0a 2020 2020 2020  nthreads,.      
-00014130: 2020 7665 7262 6f73 652c 0a20 2020 2029    verbose,.    )
-00014140: 0a20 2020 2061 7667 5f68 7964 726f 7061  .    avg_hydropa
-00014150: 7468 7920 3d20 5f70 726f 6365 7373 5f68  thy = _process_h
-00014160: 7964 726f 7061 7468 7928 6176 675f 6879  ydropathy(avg_hy
-00014170: 6472 6f70 6174 6879 2c20 6e63 6176 2c20  dropathy, ncav, 
-00014180: 7365 6c65 6374 696f 6e29 0a20 2020 2061  selection).    a
-00014190: 7667 5f68 7964 726f 7061 7468 795b 6622  vg_hydropathy[f"
-000141a0: 7b6e 616d 657d 225d 203d 205b 666c 6f61  {name}"] = [floa
-000141b0: 7428 7363 616c 652e 6d69 6e28 2929 2c20  t(scale.min()), 
-000141c0: 666c 6f61 7428 7363 616c 652e 6d61 7828  float(scale.max(
-000141d0: 2929 5d0a 0a20 2020 2072 6574 7572 6e20  ))]..    return 
-000141e0: 7363 616c 6573 2e72 6573 6861 7065 286e  scales.reshape(n
-000141f0: 782c 206e 792c 206e 7a29 2c20 6176 675f  x, ny, nz), avg_
-00014200: 6879 6472 6f70 6174 6879 0a0a 0a64 6566  hydropathy...def
-00014210: 205f 6765 745f 6f70 656e 696e 675f 6e61   _get_opening_na
-00014220: 6d65 2869 6e64 6578 3a20 696e 7429 202d  me(index: int) -
-00014230: 3e20 7374 723a 0a20 2020 2022 2222 4765  > str:.    """Ge
-00014240: 7420 6f70 656e 696e 6720 6e61 6d65 2c20  t opening name, 
-00014250: 6567 204f 4141 2c20 4f41 422c 2061 6e64  eg OAA, OAB, and
-00014260: 2073 6f20 6f6e 2c20 6261 7365 6420 6f6e   so on, based on
-00014270: 2074 6865 2069 6e64 6578 2e0a 0a20 2020   the index...   
-00014280: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00014290: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069  ----------.    i
-000142a0: 6e64 6578 203a 2069 6e74 0a20 2020 2020  ndex : int.     
-000142b0: 2020 2049 6e64 6578 2069 6e20 7468 6520     Index in the 
-000142c0: 6469 6374 696f 6e61 7279 2e0a 0a20 2020  dictionary...   
-000142d0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-000142e0: 2d2d 2d2d 0a20 2020 206f 7065 6e69 6e67  ----.    opening
-000142f0: 5f6e 616d 6520 3a20 7374 720a 2020 2020  _name : str.    
-00014300: 2020 2020 4f70 656e 696e 6720 6e61 6d65      Opening name
-00014310: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
-00014320: 6e69 6e67 5f6e 616d 6520 3d20 6622 4f7b  ning_name = f"O{
-00014330: 6368 7228 3635 202b 2069 6e74 2869 6e64  chr(65 + int(ind
-00014340: 6578 202f 2032 3629 2025 2032 3629 7d7b  ex / 26) % 26)}{
-00014350: 6368 7228 3635 202b 2028 696e 6465 7820  chr(65 + (index 
-00014360: 2520 3236 2929 7d22 0a20 2020 2072 6574  % 26))}".    ret
-00014370: 7572 6e20 6f70 656e 696e 675f 6e61 6d65  urn opening_name
-00014380: 0a0a 0a64 6566 205f 6765 745f 6f70 656e  ...def _get_open
-00014390: 696e 675f 6c61 6265 6c28 6f70 656e 696e  ing_label(openin
-000143a0: 675f 6e61 6d65 3a20 7374 7229 202d 3e20  g_name: str) -> 
-000143b0: 696e 743a 0a20 2020 2022 2222 4765 7420  int:.    """Get 
-000143c0: 6f70 656e 696e 6720 6c61 6265 6c2c 2065  opening label, e
-000143d0: 6720 322c 2033 2c20 616e 6420 736f 206f  g 2, 3, and so o
-000143e0: 6e2c 2062 6173 6564 206f 6e20 7468 6520  n, based on the 
-000143f0: 6f70 656e 696e 6720 6e61 6d65 2e0a 0a20  opening name... 
-00014400: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00014410: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00014420: 206f 7065 6e69 6e67 5f6e 616d 6520 3a20   opening_name : 
-00014430: 7374 720a 2020 2020 2020 2020 4f70 656e  str.        Open
-00014440: 696e 6720 6e61 6d65 0a0a 2020 2020 5265  ing name..    Re
-00014450: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00014460: 2d0a 2020 2020 636f 7065 6e69 6e67 5f6c  -.    copening_l
-00014470: 6162 656c 203a 2069 6e74 0a20 2020 2020  abel : int.     
-00014480: 2020 2049 6e74 6567 6572 206c 6162 656c     Integer label
-00014490: 206f 6620 6561 6368 206f 7065 6e69 6e67   of each opening
-000144a0: 2e0a 0a20 2020 2052 6169 7365 730a 2020  ...    Raises.  
-000144b0: 2020 2d2d 2d2d 2d2d 0a20 2020 2056 616c    ------.    Val
-000144c0: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
-000144d0: 496e 7661 6c69 6420 6f70 656e 696e 6720  Invalid opening 
-000144e0: 6e61 6d65 3a20 606f 7065 6e69 6e67 5f6e  name: `opening_n
-000144f0: 616d 6560 2e0a 2020 2020 2222 220a 2020  ame`..    """.  
-00014500: 2020 2320 4368 6563 6b20 6f70 656e 696e    # Check openin
-00014510: 6720 6e61 6d65 0a20 2020 2069 6620 6f70  g name.    if op
-00014520: 656e 696e 675f 6e61 6d65 5b30 5d20 213d  ening_name[0] !=
-00014530: 2022 4f22 3a0a 2020 2020 2020 2020 7261   "O":.        ra
-00014540: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-00014550: 2249 6e76 616c 6964 206f 7065 6e69 6e67  "Invalid opening
-00014560: 206e 616d 653a 207b 6f70 656e 696e 675f   name: {opening_
-00014570: 6e61 6d65 7d2e 2229 0a0a 2020 2020 2320  name}.")..    # 
-00014580: 4765 7420 6361 7669 7479 206c 6162 656c  Get cavity label
-00014590: 0a20 2020 2063 6176 6974 795f 6c61 6265  .    cavity_labe
-000145a0: 6c20 3d20 286f 7264 286f 7065 6e69 6e67  l = (ord(opening
-000145b0: 5f6e 616d 655b 315d 2920 2d20 3635 2920  _name[1]) - 65) 
-000145c0: 2a20 3236 202b 2028 6f72 6428 6f70 656e  * 26 + (ord(open
-000145d0: 696e 675f 6e61 6d65 5b32 5d29 202d 2036  ing_name[2]) - 6
-000145e0: 3529 202b 2032 0a0a 2020 2020 7265 7475  5) + 2..    retu
-000145f0: 726e 2063 6176 6974 795f 6c61 6265 6c0a  rn cavity_label.
-00014600: 0a0a 6465 6620 5f70 726f 6365 7373 5f6f  ..def _process_o
-00014610: 7065 6e69 6e67 7328 0a20 2020 2072 6177  penings(.    raw
-00014620: 5f6f 7065 6e69 6e67 733a 206e 756d 7079  _openings: numpy
-00014630: 2e6e 6461 7272 6179 2c0a 2020 2020 6f70  .ndarray,.    op
-00014640: 656e 696e 6732 6361 7669 7479 3a20 6e75  ening2cavity: nu
-00014650: 6d70 792e 6e64 6172 7261 792c 0a29 202d  mpy.ndarray,.) -
-00014660: 3e20 4469 6374 5b73 7472 2c20 4469 6374  > Dict[str, Dict
-00014670: 5b73 7472 2c20 666c 6f61 745d 5d3a 0a20  [str, float]]:. 
-00014680: 2020 2022 2222 5072 6f63 6573 7365 7320     """Processes 
-00014690: 6172 7261 7973 206f 6620 6f70 656e 696e  arrays of openin
-000146a0: 6773 2720 6172 6561 732e 0a0a 2020 2020  gs' areas...    
-000146b0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-000146c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7261  ---------.    ra
-000146d0: 775f 6f70 656e 696e 6773 203a 206e 756d  w_openings : num
-000146e0: 7079 2e6e 6461 7272 6179 0a20 2020 2020  py.ndarray.     
-000146f0: 2020 2041 206e 756d 7079 2e6e 6461 7272     A numpy.ndarr
-00014700: 6179 206f 6620 6f70 656e 696e 6773 2720  ay of openings' 
-00014710: 6172 6561 732e 0a20 2020 206f 7065 6e69  areas..    openi
-00014720: 6e67 7332 6361 7669 7479 3a20 6e75 6d70  ngs2cavity: nump
-00014730: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
-00014740: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
-00014750: 7920 6f66 206f 7065 6e69 6e67 7320 6173  y of openings as
-00014760: 2069 6e64 6578 6573 2061 6e64 2063 6176   indexes and cav
-00014770: 6974 6965 7320 6173 2076 616c 7565 732e  ities as values.
-00014780: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00014790: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6172    -------.    ar
-000147a0: 6561 203a 2044 6963 745b 7374 722c 2044  ea : Dict[str, D
-000147b0: 6963 745b 7374 722c 666c 6f61 745d 5d0a  ict[str,float]].
-000147c0: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-000147d0: 6e61 7279 2077 6974 6820 6172 6561 206f  nary with area o
-000147e0: 6620 6561 6368 2064 6574 6563 7465 6420  f each detected 
-000147f0: 6f70 656e 696e 672e 0a20 2020 2022 2222  opening..    """
-00014800: 0a20 2020 2061 7265 6120 3d20 7b7d 0a0a  .    area = {}..
-00014810: 2020 2020 2320 4765 7420 6e75 6d62 6572      # Get number
-00014820: 206f 6620 6f70 656e 696e 6773 0a20 2020   of openings.   
-00014830: 206e 6f70 656e 696e 6773 203d 2072 6177   nopenings = raw
-00014840: 5f6f 7065 6e69 6e67 732e 7368 6170 655b  _openings.shape[
-00014850: 305d 0a0a 2020 2020 666f 7220 696e 6465  0]..    for inde
-00014860: 7820 696e 2072 616e 6765 286e 6f70 656e  x in range(nopen
-00014870: 696e 6773 293a 0a20 2020 2020 2020 2023  ings):.        #
-00014880: 2047 6574 206f 7065 6e69 6e67 206e 616d   Get opening nam
-00014890: 650a 2020 2020 2020 2020 6f70 656e 696e  e.        openin
-000148a0: 6720 3d20 5f67 6574 5f6f 7065 6e69 6e67  g = _get_opening
-000148b0: 5f6e 616d 6528 696e 6465 7829 0a0a 2020  _name(index)..  
-000148c0: 2020 2020 2020 2320 4765 7420 6361 7669        # Get cavi
-000148d0: 7479 206e 616d 650a 2020 2020 2020 2020  ty name.        
-000148e0: 6361 7669 7479 203d 205f 6765 745f 6361  cavity = _get_ca
-000148f0: 7669 7479 5f6e 616d 6528 6f70 656e 696e  vity_name(openin
-00014900: 6732 6361 7669 7479 5b69 6e64 6578 5d29  g2cavity[index])
-00014910: 0a0a 2020 2020 2020 2020 2320 5361 7665  ..        # Save
-00014920: 206f 7065 6e69 6e67 2061 7265 610a 2020   opening area.  
-00014930: 2020 2020 2020 6966 2063 6176 6974 7920        if cavity 
-00014940: 6e6f 7420 696e 2061 7265 612e 6b65 7973  not in area.keys
-00014950: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014960: 6172 6561 5b63 6176 6974 795d 203d 207b  area[cavity] = {
-00014970: 7d0a 2020 2020 2020 2020 6172 6561 5b63  }.        area[c
-00014980: 6176 6974 795d 5b6f 7065 6e69 6e67 5d20  avity][opening] 
-00014990: 3d20 666c 6f61 7428 726f 756e 6428 7261  = float(round(ra
-000149a0: 775f 6f70 656e 696e 6773 5b69 6e64 6578  w_openings[index
-000149b0: 5d2c 2032 2929 0a0a 2020 2020 2320 536f  ], 2))..    # So
-000149c0: 7274 206b 6579 730a 2020 2020 6172 6561  rt keys.    area
-000149d0: 203d 2064 6963 7428 736f 7274 6564 2861   = dict(sorted(a
-000149e0: 7265 612e 6974 656d 7328 2929 290a 0a20  rea.items())).. 
-000149f0: 2020 2072 6574 7572 6e20 6172 6561 0a0a     return area..
-00014a00: 0a64 6566 206f 7065 6e69 6e67 7328 0a20  .def openings(. 
-00014a10: 2020 2063 6176 6974 6965 733a 206e 756d     cavities: num
-00014a20: 7079 2e6e 6461 7272 6179 2c0a 2020 2020  py.ndarray,.    
-00014a30: 6465 7074 6873 3a20 4f70 7469 6f6e 616c  depths: Optional
-00014a40: 5b6e 756d 7079 2e6e 6461 7272 6179 5d20  [numpy.ndarray] 
-00014a50: 3d20 4e6f 6e65 2c0a 2020 2020 7374 6570  = None,.    step
-00014a60: 3a20 556e 696f 6e5b 666c 6f61 742c 2069  : Union[float, i
-00014a70: 6e74 5d20 3d20 302e 362c 0a20 2020 206f  nt] = 0.6,.    o
-00014a80: 7065 6e69 6e67 735f 6375 746f 6666 3a20  penings_cutoff: 
-00014a90: 696e 7420 3d20 312c 0a20 2020 2073 656c  int = 1,.    sel
-00014aa0: 6563 7469 6f6e 3a20 4f70 7469 6f6e 616c  ection: Optional
-00014ab0: 5b55 6e69 6f6e 5b4c 6973 745b 696e 745d  [Union[List[int]
-00014ac0: 2c20 4c69 7374 5b73 7472 5d5d 5d20 3d20  , List[str]]] = 
-00014ad0: 4e6f 6e65 2c0a 2020 2020 6e74 6872 6561  None,.    nthrea
-00014ae0: 6473 3a20 4f70 7469 6f6e 616c 5b69 6e74  ds: Optional[int
-00014af0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7665  ] = None,.    ve
-00014b00: 7262 6f73 653a 2062 6f6f 6c20 3d20 4661  rbose: bool = Fa
-00014b10: 6c73 652c 0a29 202d 3e20 5475 706c 655b  lse,.) -> Tuple[
-00014b20: 696e 742c 206e 756d 7079 2e6e 6461 7272  int, numpy.ndarr
-00014b30: 6179 2c20 4469 6374 5b73 7472 2c20 4469  ay, Dict[str, Di
-00014b40: 6374 5b73 7472 2c20 666c 6f61 745d 5d5d  ct[str, float]]]
-00014b50: 3a0a 2020 2020 2222 225b 5749 505d 2049  :.    """[WIP] I
-00014b60: 6465 6e74 6966 7920 6f70 656e 696e 6773  dentify openings
-00014b70: 206f 6620 7468 6520 6465 7465 6374 6564   of the detected
-00014b80: 2063 6176 6974 6965 7320 616e 6420 6361   cavities and ca
-00014b90: 6c63 756c 6174 6520 7468 6569 7220 6172  lculate their ar
-00014ba0: 6561 732e 0a0a 2020 2020 5061 7261 6d65  eas...    Parame
-00014bb0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00014bc0: 2d2d 2d0a 2020 2020 6361 7669 7469 6573  ---.    cavities
-00014bd0: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00014be0: 0a20 2020 2020 2020 2043 6176 6974 7920  .        Cavity 
-00014bf0: 706f 696e 7473 2069 6e20 7468 6520 3344  points in the 3D
-00014c00: 2067 7269 6420 2863 6176 6974 6965 735b   grid (cavities[
-00014c10: 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020  nx][ny][nz])..  
-00014c20: 2020 2020 2020 4361 7669 7469 6573 2061        Cavities a
-00014c30: 7272 6179 2068 6173 2069 6e74 6567 6572  rray has integer
-00014c40: 206c 6162 656c 7320 696e 2065 6163 6820   labels in each 
-00014c50: 706f 7369 7469 6f6e 2c20 7468 6174 2061  position, that a
-00014c60: 7265 3a0a 0a20 2020 2020 2020 2020 2020  re:..           
-00014c70: 202a 202d 313a 2062 756c 6b20 706f 696e   * -1: bulk poin
-00014c80: 7473 3b0a 0a20 2020 2020 2020 2020 2020  ts;..           
-00014c90: 202a 2030 3a20 6269 6f6d 6f6c 6563 756c   * 0: biomolecul
-00014ca0: 6520 706f 696e 7473 3b0a 0a20 2020 2020  e points;..     
-00014cb0: 2020 2020 2020 202a 2031 3a20 656d 7074         * 1: empt
-00014cc0: 7920 7370 6163 6520 706f 696e 7473 3b0a  y space points;.
-00014cd0: 0a20 2020 2020 2020 2020 2020 202a 203e  .            * >
-00014ce0: 3d32 3a20 6361 7669 7479 2070 6f69 6e74  =2: cavity point
-00014cf0: 732e 0a20 2020 2064 6570 7468 7320 3a20  s..    depths : 
-00014d00: 4f70 7469 6f6e 616c 5b6e 756d 7079 2e6e  Optional[numpy.n
-00014d10: 6461 7272 6179 5d2c 206f 7074 696f 6e61  darray], optiona
-00014d20: 6c0a 2020 2020 2020 2020 4120 6e75 6d70  l.        A nump
-00014d30: 792e 6e64 6172 7261 7920 7769 7468 2064  y.ndarray with d
-00014d40: 6570 7468 206f 6620 6361 7669 7479 2070  epth of cavity p
-00014d50: 6f69 6e74 7320 2864 6570 7468 5b6e 785d  oints (depth[nx]
-00014d60: 5b6e 795d 5b6e 7a5d 292c 2062 7920 6465  [ny][nz]), by de
-00014d70: 6661 756c 7420 4e6f 6e65 2e20 4966 204e  fault None. If N
-00014d80: 6f6e 652c 2064 6570 7468 7320 6973 2063  one, depths is c
-00014d90: 616c 6375 6c61 7465 6420 6672 6f6d 2063  alculated from c
-00014da0: 6176 6974 6965 732e 0a20 2020 2073 7465  avities..    ste
-00014db0: 7020 3a20 556e 696f 6e5b 666c 6f61 742c  p : Union[float,
-00014dc0: 2069 6e74 5d2c 206f 7074 696f 6e61 6c0a   int], optional.
-00014dd0: 2020 2020 2020 2020 4772 6964 2073 7061          Grid spa
-00014de0: 6369 6e67 2028 4129 2c20 6279 2064 6566  cing (A), by def
-00014df0: 6175 6c74 2030 2e36 2e0a 2020 2020 6f70  ault 0.6..    op
-00014e00: 656e 696e 6773 5f63 7574 6f66 6620 3a20  enings_cutoff : 
-00014e10: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-00014e20: 2020 2020 2020 5468 6520 6d69 6e69 6d75        The minimu
-00014e30: 6d20 6e75 6d62 6572 206f 6620 766f 7865  m number of voxe
-00014e40: 6c73 2061 6e20 6f70 656e 696e 6720 6d75  ls an opening mu
-00014e50: 7374 2068 6176 652c 2062 7920 6465 6661  st have, by defa
-00014e60: 756c 7420 312e 0a20 2020 2073 656c 6563  ult 1..    selec
-00014e70: 7469 6f6e 203a 2055 6e69 6f6e 5b4c 6973  tion : Union[Lis
-00014e80: 745b 696e 745d 2c20 4c69 7374 5b73 7472  t[int], List[str
-00014e90: 5d5d 2c20 6f70 7469 6f6e 616c 0a20 2020  ]], optional.   
-00014ea0: 2020 2020 2041 206c 6973 7420 6f66 2069       A list of i
-00014eb0: 6e74 6567 6572 206c 6162 656c 7320 6f72  nteger labels or
-00014ec0: 2061 206c 6973 7420 6f66 2063 6176 6974   a list of cavit
-00014ed0: 7920 6e61 6d65 7320 746f 2062 6520 7365  y names to be se
-00014ee0: 6c65 6374 6564 2c20 6279 2064 6566 6175  lected, by defau
-00014ef0: 6c74 204e 6f6e 652e 0a20 2020 206e 7468  lt None..    nth
-00014f00: 7265 6164 7320 3a20 696e 742c 206f 7074  reads : int, opt
-00014f10: 696f 6e61 6c0a 2020 2020 2020 2020 4e75  ional.        Nu
-00014f20: 6d62 6572 206f 6620 7468 7265 6164 732c  mber of threads,
-00014f30: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
-00014f40: 2e20 4966 204e 6f6e 652c 2074 6865 206e  . If None, the n
-00014f50: 756d 6265 7220 6f66 2074 6872 6561 6473  umber of threads
-00014f60: 2069 730a 2020 2020 2020 2020 606f 732e   is.        `os.
-00014f70: 6370 755f 636f 756e 7428 2920 2d20 3160  cpu_count() - 1`
-00014f80: 2e0a 2020 2020 7665 7262 6f73 6520 3a20  ..    verbose : 
-00014f90: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
-00014fa0: 2020 2020 2020 2050 7269 6e74 2065 7874         Print ext
-00014fb0: 7261 2069 6e66 6f72 6d61 7469 6f6e 2074  ra information t
-00014fc0: 6f20 7374 616e 6461 7264 206f 7574 7075  o standard outpu
-00014fd0: 742c 2062 7920 6465 6661 756c 7420 4661  t, by default Fa
-00014fe0: 6c73 652e 0a0a 2020 2020 5265 7475 726e  lse...    Return
-00014ff0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00015000: 2020 6e6f 7065 6e69 6e67 7320 3a20 696e    nopenings : in
-00015010: 740a 2020 2020 2020 2020 546f 7461 6c20  t.        Total 
-00015020: 6e75 6d62 6572 206f 6620 6f70 656e 696e  number of openin
-00015030: 6773 2e0a 2020 2020 6f70 656e 696e 6773  gs..    openings
-00015040: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-00015050: 0a20 2020 2020 2020 204f 7065 6e69 6e67  .        Opening
-00015060: 7320 706f 696e 7473 2069 6e20 7468 6520  s points in the 
-00015070: 3344 2067 7269 6420 286f 7065 6e69 6e67  3D grid (opening
-00015080: 735b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a  s[nx][ny][nz])..
-00015090: 2020 2020 2020 2020 4f70 656e 696e 6773          Openings
-000150a0: 2061 7272 6179 2068 6173 2069 6e74 6567   array has integ
-000150b0: 6572 206c 6162 656c 7320 696e 2065 6163  er labels in eac
-000150c0: 6820 706f 7369 7469 6f6e 2c20 7468 6174  h position, that
-000150d0: 2061 7265 3a0a 0a20 2020 2020 2020 2020   are:..         
-000150e0: 2020 202a 202d 313a 2062 756c 6b20 706f     * -1: bulk po
-000150f0: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
-00015100: 2020 202a 2030 3a20 6361 7669 7479 206f     * 0: cavity o
-00015110: 7220 6269 6f6d 6f6c 6563 756c 6520 706f  r biomolecule po
-00015120: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
-00015130: 2020 202a 2031 3a20 656d 7074 7920 7370     * 1: empty sp
-00015140: 6163 6520 706f 696e 7473 3b0a 0a20 2020  ace points;..   
-00015150: 2020 2020 2020 2020 202a 203e 3d32 3a20           * >=2: 
-00015160: 4f70 656e 696e 6720 706f 696e 7473 2e0a  Opening points..
-00015170: 0a20 2020 2020 2020 2054 6865 2065 6d70  .        The emp
-00015180: 7479 2073 7061 6365 2070 6f69 6e74 7320  ty space points 
-00015190: 6172 6520 7265 6769 6f6e 7320 7468 6174  are regions that
-000151a0: 2064 6f20 6e6f 7420 6d65 6574 2074 6865   do not meet the
-000151b0: 2063 686f 7365 6e0a 2020 2020 2020 2020   chosen.        
-000151c0: 6f70 656e 696e 6773 2063 7574 6f66 6620  openings cutoff 
-000151d0: 746f 2062 6520 636f 6e73 6964 6572 6564  to be considered
-000151e0: 2061 6e20 6f70 656e 696e 672e 0a20 2020   an opening..   
-000151f0: 2061 6f70 656e 696e 6773 203a 2044 6963   aopenings : Dic
-00015200: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
-00015210: 666c 6f61 745d 5d0a 2020 2020 2020 2020  float]].        
-00015220: 4120 6469 6374 696f 6e61 7279 2077 6974  A dictionary wit
-00015230: 6820 6172 6561 206f 6620 6561 6368 2064  h area of each d
-00015240: 6574 6563 7465 6420 6f70 656e 696e 672e  etected opening.
-00015250: 0a0a 2020 2020 5261 6973 6573 0a20 2020  ..    Raises.   
-00015260: 202d 2d2d 2d2d 2d0a 2020 2020 5479 7065   ------.    Type
-00015270: 4572 726f 720a 2020 2020 2020 2020 6063  Error.        `c
-00015280: 6176 6974 6965 7360 206d 7573 7420 6265  avities` must be
-00015290: 2061 206e 756d 7079 2e6e 6461 7272 6179   a numpy.ndarray
-000152a0: 2e0a 2020 2020 5661 6c75 6545 7272 6f72  ..    ValueError
-000152b0: 0a20 2020 2020 2020 2060 6361 7669 7469  .        `caviti
-000152c0: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
-000152d0: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
-000152e0: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
-000152f0: 206e 7a29 2e0a 2020 2020 5479 7065 4572   nz)..    TypeEr
-00015300: 726f 720a 2020 2020 2020 2020 6064 6570  ror.        `dep
-00015310: 7468 7360 206d 7573 7420 6265 2061 206e  ths` must be a n
-00015320: 756d 7079 2e6e 6461 7272 6179 2e0a 2020  umpy.ndarray..  
-00015330: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
-00015340: 2020 2020 2060 6465 7074 6873 6020 6861       `depths` ha
-00015350: 7320 7468 6520 696e 636f 7272 6563 7420  s the incorrect 
-00015360: 7368 6170 652e 2049 7420 6d75 7374 2062  shape. It must b
-00015370: 6520 286e 782c 206e 792c 206e 7a29 2e0a  e (nx, ny, nz)..
-00015380: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
-00015390: 2020 2020 2020 6073 7465 7060 206d 7573        `step` mus
-000153a0: 7420 6265 2061 2070 6f73 6974 6976 6520  t be a positive 
-000153b0: 7265 616c 206e 756d 6265 722e 0a20 2020  real number..   
-000153c0: 2056 616c 7565 4572 726f 720a 2020 2020   ValueError.    
-000153d0: 2020 2020 6073 7465 7060 206d 7573 7420      `step` must 
-000153e0: 6265 2061 2070 6f73 6974 6976 6520 7265  be a positive re
-000153f0: 616c 206e 756d 6265 722e 0a20 2020 2054  al number..    T
-00015400: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-00015410: 2060 6f70 656e 696e 6773 5f63 7574 6f66   `openings_cutof
-00015420: 6660 206d 7573 7420 6265 2061 6e20 696e  f` must be an in
-00015430: 7465 6765 722e 0a20 2020 2056 616c 7565  teger..    Value
-00015440: 4572 726f 720a 2020 2020 2020 2020 606f  Error.        `o
-00015450: 7065 6e69 6e67 735f 6375 746f 6666 6020  penings_cutoff` 
-00015460: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-00015470: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
-00015480: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-00015490: 2020 6073 656c 6563 7469 6f6e 6020 6d75    `selection` mu
-000154a0: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
-000154b0: 7374 7269 6e67 7320 2863 6176 6974 7920  strings (cavity 
-000154c0: 6e61 6d65 7329 206f 7220 696e 7465 6765  names) or intege
-000154d0: 7273 2028 6361 7669 7479 206c 6162 656c  rs (cavity label
-000154e0: 7329 2e0a 2020 2020 5661 6c75 6545 7272  s)..    ValueErr
-000154f0: 6f72 0a20 2020 2020 2020 2049 6e76 616c  or.        Inval
-00015500: 6964 2060 7365 6c65 6374 696f 6e60 3a20  id `selection`: 
-00015510: 6073 656c 6563 7469 6f6e 602e 0a20 2020  `selection`..   
-00015520: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-00015530: 2020 2060 6e74 6872 6561 6473 6020 6d75     `nthreads` mu
-00015540: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-00015550: 2069 6e74 6567 6572 2e0a 2020 2020 5661   integer..    Va
-00015560: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
-00015570: 2060 6e74 6872 6561 6473 6020 6d75 7374   `nthreads` must
-00015580: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
-00015590: 6e74 6567 6572 2e0a 2020 2020 5479 7065  nteger..    Type
-000155a0: 4572 726f 720a 2020 2020 2020 2020 6076  Error.        `v
-000155b0: 6572 626f 7365 6020 6d75 7374 2062 6520  erbose` must be 
-000155c0: 6120 626f 6f6c 6561 6e0a 0a20 2020 2045  a boolean..    E
-000155d0: 7861 6d70 6c65 0a20 2020 202d 2d2d 2d2d  xample.    -----
-000155e0: 2d2d 0a20 2020 2057 6974 6820 7468 6520  --.    With the 
-000155f0: 6361 7669 7479 2070 6f69 6e74 7320 6964  cavity points id
-00015600: 656e 7469 6669 6564 2077 6974 6820 6060  entified with ``
-00015610: 6465 7465 6374 6060 2c20 7765 2063 616e  detect``, we can
-00015620: 2063 6861 7261 6374 6572 697a 6520 7468   characterize th
-00015630: 6569 7220 6f70 656e 696e 6773 2c20 7468  eir openings, th
-00015640: 6174 2069 6e63 6c75 6465 7320 6e75 6d62  at includes numb
-00015650: 6572 2061 6e64 2061 7265 6120 6f66 206f  er and area of o
-00015660: 7065 6e69 6e67 7320 616e 6420 6465 6669  penings and defi
-00015670: 6e69 6e67 206f 7065 6e69 6e67 2070 6f69  ning opening poi
-00015680: 6e74 733a 0a0a 2020 2020 3e3e 3e20 6672  nts:..    >>> fr
-00015690: 6f6d 2070 794b 5646 696e 6465 7220 696d  om pyKVFinder im
-000156a0: 706f 7274 206f 7065 6e69 6e67 730a 2020  port openings.  
-000156b0: 2020 3e3e 3e20 6e6f 7065 6e69 6e67 732c    >>> nopenings,
-000156c0: 206f 7065 6e69 6e67 732c 2061 6f70 656e   openings, aopen
-000156d0: 696e 6773 203d 206f 7065 6e69 6e67 7328  ings = openings(
-000156e0: 6361 7669 7469 6573 290a 2020 2020 3e3e  cavities).    >>
-000156f0: 3e20 6e6f 7065 6e69 6e67 730a 2020 2020  > nopenings.    
-00015700: 3136 0a20 2020 203e 3e3e 206f 7065 6e69  16.    >>> openi
-00015710: 6e67 730a 2020 2020 6172 7261 7928 5b5b  ngs.    array([[
-00015720: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00015730: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-00015740: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-00015750: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-00015760: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-00015770: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00015780: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00015790: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-000157a0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-000157b0: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-000157c0: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-000157d0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-000157e0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-000157f0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-00015800: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00015810: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00015820: 2c20 2d31 5d5d 2c0a 2020 2020 2020 2020  , -1]],.        
-00015830: 2020 2e2e 2e2c 0a20 2020 2020 2020 2020    ...,.         
-00015840: 205b 5b2d 312c 202d 312c 202d 312c 202e   [[-1, -1, -1, .
-00015850: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-00015860: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-00015870: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-00015880: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-00015890: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-000158a0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-000158b0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-000158c0: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-000158d0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-000158e0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-000158f0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00015900: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-00015910: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-00015920: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00015930: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00015940: 2d31 2c20 2d31 5d5d 5d29 0a20 2020 203e  -1, -1]]]).    >
-00015950: 3e3e 2061 6f70 656e 696e 6773 0a20 2020  >> aopenings.   
-00015960: 207b 274b 4141 273a 207b 274f 4141 273a   {'KAA': {'OAA':
-00015970: 2034 372e 3431 2c20 274f 4147 273a 2033   47.41, 'OAG': 3
-00015980: 2e36 7d2c 2027 4b41 4227 3a20 7b27 4f41  .6}, 'KAB': {'OA
-00015990: 4227 3a20 3235 2e38 347d 2c20 274b 4143  B': 25.84}, 'KAC
-000159a0: 273a 207b 274f 4143 273a 2035 332e 3632  ': {'OAC': 53.62
-000159b0: 7d2c 2027 4b41 4427 3a20 7b27 4f41 4427  }, 'KAD': {'OAD'
-000159c0: 3a20 3132 2e35 397d 2c20 274b 4145 273a  : 12.59}, 'KAE':
-000159d0: 207b 274f 4145 273a 2032 362e 337d 2c20   {'OAE': 26.3}, 
-000159e0: 274b 4146 273a 207b 274f 4146 273a 2031  'KAF': {'OAF': 1
-000159f0: 382e 3436 7d2c 2027 4b41 4727 3a20 7b27  8.46}, 'KAG': {'
-00015a00: 4f41 4827 3a20 3132 2e38 337d 2c20 274b  OAH': 12.83}, 'K
-00015a10: 4148 273a 207b 274f 414b 273a 2035 392e  AH': {'OAK': 59.
-00015a20: 3936 7d2c 2027 4b41 4a27 3a20 7b27 4f41  96}, 'KAJ': {'OA
-00015a30: 4927 3a20 3136 2e31 317d 2c20 274b 414c  I': 16.11}, 'KAL
-00015a40: 273a 207b 274f 414a 273a 2031 372e 337d  ': {'OAJ': 17.3}
-00015a50: 2c20 274b 414d 273a 207b 274f 414c 273a  , 'KAM': {'OAL':
-00015a60: 2033 352e 3237 7d2c 2027 4b41 4f27 3a20   35.27}, 'KAO': 
-00015a70: 7b27 4f41 4d27 3a20 382e 3439 7d2c 2027  {'OAM': 8.49}, '
-00015a80: 4b41 5027 3a20 7b27 4f41 4e27 3a20 3133  KAP': {'OAN': 13
-00015a90: 2e37 317d 2c20 274b 4151 273a 207b 274f  .71}, 'KAQ': {'O
-00015aa0: 414f 273a 2031 332e 3136 7d2c 2027 4b41  AO': 13.16}, 'KA
-00015ab0: 5227 3a20 7b27 4f41 5027 3a20 3135 2e33  R': {'OAP': 15.3
-00015ac0: 367d 7d0a 0a20 2020 2057 6974 6820 7468  6}}..    With th
-00015ad0: 6520 6361 7669 7479 2061 6e64 206f 7065  e cavity and ope
-00015ae0: 6e69 6e67 2070 6f69 6e74 7320 6964 656e  ning points iden
-00015af0: 7469 6669 6564 2c20 7765 2063 616e 3a0a  tified, we can:.
-00015b00: 0a20 2020 202a 2045 7870 6f72 7420 6361  .    * Export ca
-00015b10: 7669 7479 2070 6f69 6e74 7320 7769 7468  vity points with
-00015b20: 206f 7065 6e69 6e67 2070 6f69 6e74 7320   opening points 
-00015b30: 6d61 7070 6564 206f 6e20 7468 656d 3a0a  mapped on them:.
-00015b40: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-00015b50: 4b56 4669 6e64 6572 2069 6d70 6f72 7420  KVFinder import 
-00015b60: 6578 706f 7274 0a20 2020 203e 3e3e 2065  export.    >>> e
-00015b70: 7870 6f72 7428 2263 6176 6974 6965 735f  xport("cavities_
-00015b80: 7769 7468 5f6f 7065 6e69 6e67 732e 7064  with_openings.pd
-00015b90: 6222 2c20 6361 7669 7469 6573 2c20 4e6f  b", cavities, No
-00015ba0: 6e65 2c20 7665 7274 6963 6573 2c20 423d  ne, vertices, B=
-00015bb0: 6f70 656e 696e 6773 290a 0a20 2020 202a  openings)..    *
-00015bc0: 2045 7870 6f72 7420 6f70 656e 696e 6720   Export opening 
-00015bd0: 706f 696e 7473 2077 6974 6820 7361 6d65  points with same
-00015be0: 206e 6f6d 656e 636c 6174 7572 6520 6672   nomenclature fr
-00015bf0: 6f6d 2060 6061 6f70 656e 696e 6773 6060  om ``aopenings``
-00015c00: 3a0a 0a20 2020 203e 3e3e 2066 726f 6d20  :..    >>> from 
-00015c10: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
-00015c20: 7420 6578 706f 7274 5f6f 7065 6e69 6e67  t export_opening
-00015c30: 730a 2020 2020 3e3e 3e20 6578 706f 7274  s.    >>> export
-00015c40: 5f6f 7065 6e69 6e67 7328 226f 7065 6e69  _openings("openi
-00015c50: 6e67 732e 7064 6222 2c20 6f70 656e 696e  ngs.pdb", openin
-00015c60: 6773 2c20 7665 7274 6963 6573 290a 0a20  gs, vertices).. 
-00015c70: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00015c80: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6574  --------.    det
-00015c90: 6563 740a 2020 2020 6465 7074 680a 2020  ect.    depth.  
-00015ca0: 2020 6578 706f 7274 0a20 2020 2065 7870    export.    exp
-00015cb0: 6f72 745f 6f70 656e 696e 6773 0a20 2020  ort_openings.   
-00015cc0: 2022 2222 0a20 2020 2066 726f 6d20 5f70   """.    from _p
-00015cd0: 794b 5646 696e 6465 7220 696d 706f 7274  yKVFinder import
-00015ce0: 205f 6172 6561 2c20 5f6f 7065 6e69 6e67   _area, _opening
-00015cf0: 732c 205f 6f70 656e 696e 6773 3263 6176  s, _openings2cav
-00015d00: 6974 6965 730a 0a20 2020 2023 2043 6865  ities..    # Che
-00015d10: 636b 2061 7267 756d 656e 7473 0a20 2020  ck arguments.   
-00015d20: 2069 6620 7479 7065 2863 6176 6974 6965   if type(cavitie
-00015d30: 7329 206e 6f74 2069 6e20 5b6e 756d 7079  s) not in [numpy
-00015d40: 2e6e 6461 7272 6179 5d3a 0a20 2020 2020  .ndarray]:.     
-00015d50: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-00015d60: 6f72 2822 6063 6176 6974 6965 7360 206d  or("`cavities` m
-00015d70: 7573 7420 6265 2061 206e 756d 7079 2e6e  ust be a numpy.n
-00015d80: 6461 7272 6179 2e22 290a 2020 2020 656c  darray.").    el
-00015d90: 6966 206c 656e 2863 6176 6974 6965 732e  if len(cavities.
-00015da0: 7368 6170 6529 2021 3d20 333a 0a20 2020  shape) != 3:.   
-00015db0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00015dc0: 4572 726f 7228 2260 6361 7669 7469 6573  Error("`cavities
-00015dd0: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
-00015de0: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
-00015df0: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
-00015e00: 7a29 2e22 290a 2020 2020 6966 2064 6570  z).").    if dep
-00015e10: 7468 7320 6973 204e 6f6e 653a 0a20 2020  ths is None:.   
-00015e20: 2020 2020 2064 6570 7468 732c 205f 2c20       depths, _, 
-00015e30: 5f20 3d20 6465 7074 6828 6361 7669 7469  _ = depth(caviti
-00015e40: 6573 2c20 7374 6570 2c20 7365 6c65 6374  es, step, select
-00015e50: 696f 6e2c 206e 7468 7265 6164 732c 2076  ion, nthreads, v
-00015e60: 6572 626f 7365 290a 2020 2020 656c 6966  erbose).    elif
-00015e70: 2074 7970 6528 6465 7074 6873 2920 6e6f   type(depths) no
-00015e80: 7420 696e 205b 6e75 6d70 792e 6e64 6172  t in [numpy.ndar
-00015e90: 7261 795d 3a0a 2020 2020 2020 2020 7261  ray]:.        ra
-00015ea0: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-00015eb0: 6465 7074 6873 6020 6d75 7374 2062 6520  depths` must be 
-00015ec0: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
-00015ed0: 2229 0a20 2020 2065 6c69 6620 6c65 6e28  ").    elif len(
-00015ee0: 6465 7074 6873 2e73 6861 7065 2920 213d  depths.shape) !=
-00015ef0: 2033 3a0a 2020 2020 2020 2020 7261 6973   3:.        rais
-00015f00: 6520 5661 6c75 6545 7272 6f72 2822 6064  e ValueError("`d
-00015f10: 6570 7468 7360 2068 6173 2074 6865 2069  epths` has the i
-00015f20: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
-00015f30: 4974 206d 7573 7420 6265 2028 6e78 2c20  It must be (nx, 
-00015f40: 6e79 2c20 6e7a 292e 2229 0a20 2020 2069  ny, nz).").    i
-00015f50: 6620 7479 7065 2873 7465 7029 206e 6f74  f type(step) not
-00015f60: 2069 6e20 5b66 6c6f 6174 2c20 696e 745d   in [float, int]
-00015f70: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00015f80: 5479 7065 4572 726f 7228 2260 7374 6570  TypeError("`step
-00015f90: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
-00015fa0: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-00015fb0: 2e22 290a 2020 2020 656c 6966 2073 7465  .").    elif ste
-00015fc0: 7020 3c3d 2030 2e30 3a0a 2020 2020 2020  p <= 0.0:.      
-00015fd0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00015fe0: 6f72 2822 6073 7465 7060 206d 7573 7420  or("`step` must 
-00015ff0: 6265 2061 2070 6f73 6974 6976 6520 7265  be a positive re
-00016000: 616c 206e 756d 6265 722e 2229 0a20 2020  al number.").   
-00016010: 2069 6620 7479 7065 286f 7065 6e69 6e67   if type(opening
-00016020: 735f 6375 746f 6666 2920 6e6f 7420 696e  s_cutoff) not in
-00016030: 205b 696e 745d 3a0a 2020 2020 2020 2020   [int]:.        
-00016040: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00016050: 2260 6f70 656e 696e 6773 5f63 7574 6f66  "`openings_cutof
-00016060: 6660 206d 7573 7420 6265 2061 6e20 696e  f` must be an in
-00016070: 7465 6765 722e 2229 0a20 2020 2065 6c69  teger.").    eli
-00016080: 6620 6f70 656e 696e 6773 5f63 7574 6f66  f openings_cutof
-00016090: 6620 3c20 303a 0a20 2020 2020 2020 2072  f < 0:.        r
-000160a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000160b0: 2260 6f70 656e 696e 6773 5f63 7574 6f66  "`openings_cutof
-000160c0: 6660 206d 7573 7420 6265 2061 2070 6f73  f` must be a pos
-000160d0: 6974 6976 6520 696e 7465 6765 722e 2229  itive integer.")
-000160e0: 0a20 2020 2069 6620 7365 6c65 6374 696f  .    if selectio
-000160f0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00016100: 2020 2020 2020 2023 2043 6865 636b 2073         # Check s
-00016110: 656c 6563 7469 6f6e 2074 7970 6573 0a20  election types. 
-00016120: 2020 2020 2020 2069 6620 616c 6c28 6973         if all(is
-00016130: 696e 7374 616e 6365 2878 2c20 696e 7429  instance(x, int)
-00016140: 2066 6f72 2078 2069 6e20 7365 6c65 6374   for x in select
-00016150: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
-00016160: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
-00016170: 6c69 6620 616c 6c28 6973 696e 7374 616e  lif all(isinstan
-00016180: 6365 2878 2c20 7374 7229 2066 6f72 2078  ce(x, str) for x
-00016190: 2069 6e20 7365 6c65 6374 696f 6e29 3a0a   in selection):.
-000161a0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-000161b0: 6374 696f 6e20 3d20 5b5f 6765 745f 6361  ction = [_get_ca
-000161c0: 7669 7479 5f6c 6162 656c 2873 656c 6529  vity_label(sele)
-000161d0: 2066 6f72 2073 656c 6520 696e 2073 656c   for sele in sel
-000161e0: 6563 7469 6f6e 5d0a 2020 2020 2020 2020  ection].        
-000161f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016200: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00016210: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00016220: 2020 2022 6073 656c 6563 7469 6f6e 6020     "`selection` 
-00016230: 6d75 7374 2062 6520 6120 6c69 7374 206f  must be a list o
-00016240: 6620 7374 7269 6e67 7320 2863 6176 6974  f strings (cavit
-00016250: 7920 6e61 6d65 7329 206f 7220 696e 7465  y names) or inte
-00016260: 6765 7273 2028 6361 7669 7479 206c 6162  gers (cavity lab
-00016270: 656c 7329 2e22 0a20 2020 2020 2020 2020  els).".         
-00016280: 2020 2029 0a20 2020 2020 2020 2023 2043     ).        # C
-00016290: 6865 636b 2069 6620 7365 6c65 6374 696f  heck if selectio
-000162a0: 6e20 696e 636c 7564 6573 2076 616c 6964  n includes valid
-000162b0: 2063 6176 6974 7920 6c61 6265 6c73 0a20   cavity labels. 
-000162c0: 2020 2020 2020 2069 6620 616e 7928 7820         if any(x 
-000162d0: 3c20 3220 666f 7220 7820 696e 2073 656c  < 2 for x in sel
-000162e0: 6563 7469 6f6e 293a 0a20 2020 2020 2020  ection):.       
-000162f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00016300: 4572 726f 7228 6622 496e 7661 6c69 6420  Error(f"Invalid 
-00016310: 6073 656c 6563 7469 6f6e 603a 207b 7365  `selection`: {se
-00016320: 6c65 6374 696f 6e7d 2e22 290a 2020 2020  lection}.").    
-00016330: 6966 206e 7468 7265 6164 7320 6973 204e  if nthreads is N
-00016340: 6f6e 653a 0a20 2020 2020 2020 206e 7468  one:.        nth
-00016350: 7265 6164 7320 3d20 6f73 2e63 7075 5f63  reads = os.cpu_c
-00016360: 6f75 6e74 2829 202d 2031 0a20 2020 2065  ount() - 1.    e
-00016370: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
-00016380: 7479 7065 286e 7468 7265 6164 7329 206e  type(nthreads) n
-00016390: 6f74 2069 6e20 5b69 6e74 5d3a 0a20 2020  ot in [int]:.   
-000163a0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-000163b0: 7970 6545 7272 6f72 2822 606e 7468 7265  ypeError("`nthre
-000163c0: 6164 7360 206d 7573 7420 6265 2061 2070  ads` must be a p
-000163d0: 6f73 6974 6976 6520 696e 7465 6765 722e  ositive integer.
-000163e0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-000163f0: 6e74 6872 6561 6473 203c 3d20 303a 0a20  nthreads <= 0:. 
-00016400: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00016410: 2056 616c 7565 4572 726f 7228 2260 6e74   ValueError("`nt
-00016420: 6872 6561 6473 6020 6d75 7374 2062 6520  hreads` must be 
-00016430: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
-00016440: 6572 2e22 290a 2020 2020 6966 2074 7970  er.").    if typ
-00016450: 6528 7665 7262 6f73 6529 206e 6f74 2069  e(verbose) not i
-00016460: 6e20 5b62 6f6f 6c5d 3a0a 2020 2020 2020  n [bool]:.      
-00016470: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00016480: 7228 2260 7665 7262 6f73 6560 206d 7573  r("`verbose` mus
-00016490: 7420 6265 2061 2062 6f6f 6c65 616e 2e22  t be a boolean."
-000164a0: 290a 0a20 2020 2023 2043 6f6e 7665 7274  )..    # Convert
-000164b0: 2074 7970 6573 0a20 2020 2069 6620 7479   types.    if ty
-000164c0: 7065 2873 7465 7029 203d 3d20 696e 743a  pe(step) == int:
-000164d0: 0a20 2020 2020 2020 2073 7465 7020 3d20  .        step = 
-000164e0: 666c 6f61 7428 7374 6570 290a 0a20 2020  float(step)..   
-000164f0: 2023 2053 656c 6563 7420 6361 7669 7469   # Select caviti
-00016500: 6573 0a20 2020 2069 6620 7365 6c65 6374  es.    if select
-00016510: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00016520: 0a20 2020 2020 2020 2063 6176 6974 6965  .        cavitie
-00016530: 7320 3d20 5f73 656c 6563 745f 6361 7669  s = _select_cavi
-00016540: 7469 6573 2863 6176 6974 6965 732c 2073  ties(cavities, s
-00016550: 656c 6563 7469 6f6e 290a 0a20 2020 2023  election)..    #
-00016560: 2047 6574 206e 756d 6265 7220 6f66 2063   Get number of c
-00016570: 6176 6974 6965 730a 2020 2020 6e63 6176  avities.    ncav
-00016580: 203d 2069 6e74 2863 6176 6974 6965 732e   = int(cavities.
-00016590: 6d61 7828 2920 2d20 3129 0a0a 2020 2020  max() - 1)..    
-000165a0: 2320 4765 7420 6361 7669 7469 6573 2073  # Get cavities s
-000165b0: 6861 7065 0a20 2020 206e 782c 206e 792c  hape.    nx, ny,
-000165c0: 206e 7a20 3d20 6361 7669 7469 6573 2e73   nz = cavities.s
-000165d0: 6861 7065 0a0a 2020 2020 2320 4669 6e64  hape..    # Find
-000165e0: 206f 7065 6e69 6e67 730a 2020 2020 6e6f   openings.    no
-000165f0: 7065 6e69 6e67 732c 206f 7065 6e69 6e67  penings, opening
-00016600: 7320 3d20 5f6f 7065 6e69 6e67 7328 0a20  s = _openings(. 
-00016610: 2020 2020 2020 206e 7820 2a20 6e79 202a         nx * ny *
-00016620: 206e 7a2c 2063 6176 6974 6965 732c 2064   nz, cavities, d
-00016630: 6570 7468 732c 206e 6361 762c 206f 7065  epths, ncav, ope
-00016640: 6e69 6e67 735f 6375 746f 6666 2c20 7374  nings_cutoff, st
-00016650: 6570 2c20 6e74 6872 6561 6473 2c20 7665  ep, nthreads, ve
-00016660: 7262 6f73 650a 2020 2020 290a 0a20 2020  rbose.    )..   
-00016670: 2023 2052 6573 6861 7065 206f 7065 6e69   # Reshape openi
-00016680: 6e67 730a 2020 2020 6f70 656e 696e 6773  ngs.    openings
-00016690: 203d 206f 7065 6e69 6e67 732e 7265 7368   = openings.resh
-000166a0: 6170 6528 6e78 2c20 6e79 2c20 6e7a 290a  ape(nx, ny, nz).
-000166b0: 0a20 2020 2023 2043 616c 6375 6c61 7465  .    # Calculate
-000166c0: 206f 7065 6e69 6e67 7320 6172 6561 730a   openings areas.
-000166d0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-000166e0: 2020 2020 2020 2020 7072 696e 7428 223e          print(">
-000166f0: 2045 7374 696d 6174 696e 6720 6f70 656e   Estimating open
-00016700: 696e 6773 2061 7265 6122 290a 2020 2020  ings area").    
-00016710: 616f 7065 6e69 6e67 7320 3d20 5f61 7265  aopenings = _are
-00016720: 6128 6f70 656e 696e 6773 2c20 7374 6570  a(openings, step
-00016730: 2c20 6e6f 7065 6e69 6e67 732c 206e 7468  , nopenings, nth
-00016740: 7265 6164 7329 0a0a 2020 2020 2320 4669  reads)..    # Fi
-00016750: 6e64 2077 6869 6368 206f 7065 6e69 6e67  nd which opening
-00016760: 7320 6265 6c6f 6e67 7320 746f 2065 6163  s belongs to eac
-00016770: 6820 6361 7669 7479 0a20 2020 206f 7065  h cavity.    ope
-00016780: 6e69 6e67 3263 6176 6974 7920 3d20 5f6f  ning2cavity = _o
-00016790: 7065 6e69 6e67 7332 6361 7669 7469 6573  penings2cavities
-000167a0: 286e 6f70 656e 696e 6773 2c20 6361 7669  (nopenings, cavi
-000167b0: 7469 6573 2c20 6f70 656e 696e 6773 2c20  ties, openings, 
-000167c0: 6e74 6872 6561 6473 290a 0a20 2020 2023  nthreads)..    #
-000167d0: 2050 726f 6365 7373 206f 7065 6e69 6e67   Process opening
-000167e0: 730a 2020 2020 616f 7065 6e69 6e67 7320  s.    aopenings 
-000167f0: 3d20 5f70 726f 6365 7373 5f6f 7065 6e69  = _process_openi
-00016800: 6e67 7328 616f 7065 6e69 6e67 732c 206f  ngs(aopenings, o
-00016810: 7065 6e69 6e67 3263 6176 6974 7929 0a0a  pening2cavity)..
-00016820: 2020 2020 7265 7475 726e 206e 6f70 656e      return nopen
-00016830: 696e 6773 2c20 6f70 656e 696e 6773 2c20  ings, openings, 
-00016840: 616f 7065 6e69 6e67 730a 0a0a 6465 6620  aopenings...def 
-00016850: 6578 706f 7274 280a 2020 2020 666e 3a20  export(.    fn: 
-00016860: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-00016870: 6962 2e50 6174 685d 2c0a 2020 2020 6361  ib.Path],.    ca
-00016880: 7669 7469 6573 3a20 4f70 7469 6f6e 616c  vities: Optional
-00016890: 5b6e 756d 7079 2e6e 6461 7272 6179 5d2c  [numpy.ndarray],
-000168a0: 0a20 2020 2073 7572 6661 6365 3a20 4f70  .    surface: Op
-000168b0: 7469 6f6e 616c 5b6e 756d 7079 2e6e 6461  tional[numpy.nda
-000168c0: 7272 6179 5d2c 0a20 2020 2076 6572 7469  rray],.    verti
-000168d0: 6365 733a 2055 6e69 6f6e 5b6e 756d 7079  ces: Union[numpy
-000168e0: 2e6e 6461 7272 6179 2c20 4c69 7374 5b4c  .ndarray, List[L
-000168f0: 6973 745b 666c 6f61 745d 5d5d 2c0a 2020  ist[float]]],.  
-00016900: 2020 7374 6570 3a20 556e 696f 6e5b 666c    step: Union[fl
-00016910: 6f61 742c 2069 6e74 5d20 3d20 302e 362c  oat, int] = 0.6,
-00016920: 0a20 2020 2042 3a20 4f70 7469 6f6e 616c  .    B: Optional
-00016930: 5b6e 756d 7079 2e6e 6461 7272 6179 5d20  [numpy.ndarray] 
-00016940: 3d20 4e6f 6e65 2c0a 2020 2020 6f75 7470  = None,.    outp
-00016950: 7574 5f68 7964 726f 7061 7468 793a 2055  ut_hydropathy: U
-00016960: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-00016970: 622e 5061 7468 5d20 3d20 2268 7964 726f  b.Path] = "hydro
-00016980: 7061 7468 792e 7064 6222 2c0a 2020 2020  pathy.pdb",.    
-00016990: 7363 616c 6573 3a20 4f70 7469 6f6e 616c  scales: Optional
-000169a0: 5b6e 756d 7079 2e6e 6461 7272 6179 5d20  [numpy.ndarray] 
-000169b0: 3d20 4e6f 6e65 2c0a 2020 2020 7365 6c65  = None,.    sele
-000169c0: 6374 696f 6e3a 204f 7074 696f 6e61 6c5b  ction: Optional[
-000169d0: 556e 696f 6e5b 4c69 7374 5b69 6e74 5d2c  Union[List[int],
-000169e0: 204c 6973 745b 7374 725d 5d5d 203d 204e   List[str]]] = N
-000169f0: 6f6e 652c 0a20 2020 206e 7468 7265 6164  one,.    nthread
-00016a00: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-00016a10: 203d 204e 6f6e 652c 0a20 2020 2061 7070   = None,.    app
-00016a20: 656e 643a 2062 6f6f 6c20 3d20 4661 6c73  end: bool = Fals
-00016a30: 652c 0a20 2020 206d 6f64 656c 3a20 696e  e,.    model: in
-00016a40: 7420 3d20 302c 0a29 202d 3e20 4e6f 6e65  t = 0,.) -> None
-00016a50: 3a0a 2020 2020 2222 2245 7870 6f72 7420  :.    """Export 
-00016a60: 6361 7669 7469 7920 2848 2920 616e 6420  cavitiy (H) and 
-00016a70: 7375 7266 6163 6520 2848 4129 2070 6f69  surface (HA) poi
-00016a80: 6e74 7320 746f 2050 4442 2d66 6f72 6d61  nts to PDB-forma
-00016a90: 7474 6564 2066 696c 6520 7769 7468 0a20  tted file with. 
-00016aa0: 2020 2061 2076 6172 6961 626c 6520 2842     a variable (B
-00016ab0: 3b20 6f70 7469 6f6e 616c 2920 696e 2042  ; optional) in B
-00016ac0: 2d66 6163 746f 7220 636f 6c75 6d6e 2c20  -factor column, 
-00016ad0: 616e 6420 6879 6472 6f70 6174 6879 2074  and hydropathy t
-00016ae0: 6f0a 2020 2020 5044 422d 666f 726d 6174  o.    PDB-format
-00016af0: 7465 6420 6669 6c65 2069 6e20 422d 6661  ted file in B-fa
-00016b00: 6374 6f72 2063 6f6c 756d 6e20 6174 2073  ctor column at s
-00016b10: 7572 6661 6365 2070 6f69 6e74 7320 2848  urface points (H
-00016b20: 4129 2e0a 0a20 2020 2050 6172 616d 6574  A)...    Paramet
-00016b30: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00016b40: 2d2d 0a20 2020 2066 6e20 3a20 556e 696f  --.    fn : Unio
-00016b50: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
-00016b60: 6174 685d 0a20 2020 2020 2020 2041 2070  ath].        A p
-00016b70: 6174 6820 746f 2050 4442 2066 696c 6520  ath to PDB file 
-00016b80: 666f 7220 7772 6974 696e 6720 6361 7669  for writing cavi
-00016b90: 7469 6573 2e0a 2020 2020 6361 7669 7469  ties..    caviti
-00016ba0: 6573 203a 206e 756d 7079 2e6e 6461 7272  es : numpy.ndarr
-00016bb0: 6179 2c20 6f70 7469 6f6e 616c 0a20 2020  ay, optional.   
-00016bc0: 2020 2020 2043 6176 6974 7920 706f 696e       Cavity poin
-00016bd0: 7473 2069 6e20 7468 6520 3344 2067 7269  ts in the 3D gri
-00016be0: 6420 2863 6176 6974 6965 735b 6e78 5d5b  d (cavities[nx][
-00016bf0: 6e79 5d5b 6e7a 5d29 2e0a 2020 2020 2020  ny][nz])..      
-00016c00: 2020 4361 7669 7469 6573 2061 7272 6179    Cavities array
-00016c10: 2068 6173 2069 6e74 6567 6572 206c 6162   has integer lab
-00016c20: 656c 7320 696e 2065 6163 6820 706f 7369  els in each posi
-00016c30: 7469 6f6e 2c20 7468 6174 2061 7265 3a0a  tion, that are:.
-00016c40: 0a20 2020 2020 2020 2020 2020 202a 202d  .            * -
-00016c50: 313a 2062 756c 6b20 706f 696e 7473 3b0a  1: bulk points;.
-00016c60: 0a20 2020 2020 2020 2020 2020 202a 2030  .            * 0
-00016c70: 3a20 6269 6f6d 6f6c 6563 756c 6520 706f  : biomolecule po
-00016c80: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
-00016c90: 2020 202a 2031 3a20 656d 7074 7920 7370     * 1: empty sp
-00016ca0: 6163 6520 706f 696e 7473 3b0a 0a20 2020  ace points;..   
-00016cb0: 2020 2020 2020 2020 202a 203e 3d32 3a20           * >=2: 
-00016cc0: 6361 7669 7479 2070 6f69 6e74 732e 0a0a  cavity points...
-00016cd0: 2020 2020 2020 2020 5468 6520 656d 7074          The empt
-00016ce0: 7920 7370 6163 6520 706f 696e 7473 2061  y space points a
-00016cf0: 7265 2072 6567 696f 6e73 2074 6861 7420  re regions that 
-00016d00: 646f 206e 6f74 206d 6565 7420 7468 6520  do not meet the 
-00016d10: 6368 6f73 656e 0a20 2020 2020 2020 2076  chosen.        v
-00016d20: 6f6c 756d 6520 6375 746f 6666 2074 6f20  olume cutoff to 
-00016d30: 6265 2063 6f6e 7369 6465 7265 6420 6120  be considered a 
-00016d40: 6361 7669 7479 2e0a 2020 2020 7375 7266  cavity..    surf
-00016d50: 6163 6520 3a20 6e75 6d70 792e 6e64 6172  ace : numpy.ndar
-00016d60: 7261 792c 206f 7074 696f 6e61 6c0a 2020  ray, optional.  
-00016d70: 2020 2020 2020 5375 7266 6163 6520 706f        Surface po
-00016d80: 696e 7473 2069 6e20 7468 6520 3344 2067  ints in the 3D g
-00016d90: 7269 6420 2873 7572 6661 6365 5b6e 785d  rid (surface[nx]
-00016da0: 5b6e 795d 5b6e 7a5d 292e 2049 6620 4e6f  [ny][nz]). If No
-00016db0: 6e65 2c20 7375 7266 6163 650a 2020 2020  ne, surface.    
-00016dc0: 2020 2020 6973 2061 206e 756d 7079 2e7a      is a numpy.z
-00016dd0: 6572 6f73 2061 7272 6179 2077 6974 6820  eros array with 
-00016de0: 7361 6d65 2073 6861 7065 206f 6620 6361  same shape of ca
-00016df0: 7669 7469 6573 2e0a 2020 2020 2020 2020  vities..        
-00016e00: 5375 7266 6163 6520 6172 7261 7920 6861  Surface array ha
-00016e10: 7320 696e 7465 6765 7220 6c61 6265 6c73  s integer labels
-00016e20: 2069 6e20 6561 6368 2070 6f73 6974 696f   in each positio
-00016e30: 6e2c 2074 6861 7420 6172 653a 0a0a 2020  n, that are:..  
-00016e40: 2020 2020 2020 2020 2020 2a20 2d31 3a20            * -1: 
-00016e50: 6275 6c6b 2070 6f69 6e74 733b 0a0a 2020  bulk points;..  
-00016e60: 2020 2020 2020 2020 2020 2a20 303a 2062            * 0: b
-00016e70: 696f 6d6f 6c65 6375 6c65 206f 7220 656d  iomolecule or em
-00016e80: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
-00016e90: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
-00016ea0: 203e 3d32 3a20 7375 7266 6163 6520 706f   >=2: surface po
-00016eb0: 696e 7473 2e0a 0a20 2020 2020 2020 2054  ints...        T
-00016ec0: 6865 2065 6d70 7479 2073 7061 6365 2070  he empty space p
-00016ed0: 6f69 6e74 7320 6172 6520 7265 6769 6f6e  oints are region
-00016ee0: 7320 7468 6174 2064 6f20 6e6f 7420 6d65  s that do not me
-00016ef0: 6574 2074 6865 2063 686f 7365 6e0a 2020  et the chosen.  
-00016f00: 2020 2020 2020 766f 6c75 6d65 2063 7574        volume cut
-00016f10: 6f66 6620 746f 2062 6520 636f 6e73 6964  off to be consid
-00016f20: 6572 6564 2061 2063 6176 6974 792e 0a20  ered a cavity.. 
-00016f30: 2020 2076 6572 7469 6365 7320 3a20 556e     vertices : Un
-00016f40: 696f 6e5b 6e75 6d70 792e 6e64 6172 7261  ion[numpy.ndarra
-00016f50: 792c 204c 6973 745b 4c69 7374 5b66 6c6f  y, List[List[flo
-00016f60: 6174 5d5d 5d0a 2020 2020 2020 2020 4120  at]]].        A 
-00016f70: 6e75 6d70 792e 6e64 6172 7261 7920 6f72  numpy.ndarray or
-00016f80: 2061 206c 6973 7420 7769 7468 2078 797a   a list with xyz
-00016f90: 2076 6572 7469 6365 7320 636f 6f72 6469   vertices coordi
-00016fa0: 6e61 7465 7320 286f 7269 6769 6e2c 0a20  nates (origin,. 
-00016fb0: 2020 2020 2020 2058 2d61 7869 732c 2059         X-axis, Y
-00016fc0: 2d61 7869 732c 205a 2d61 7869 7329 2e0a  -axis, Z-axis)..
-00016fd0: 2020 2020 7374 6570 203a 2055 6e69 6f6e      step : Union
-00016fe0: 5b66 6c6f 6174 2c20 696e 745d 2c20 6f70  [float, int], op
-00016ff0: 7469 6f6e 616c 0a20 2020 2020 2020 2047  tional.        G
-00017000: 7269 6420 7370 6163 696e 6720 2841 292c  rid spacing (A),
-00017010: 2062 7920 6465 6661 756c 7420 302e 362e   by default 0.6.
-00017020: 0a20 2020 2042 203a 206e 756d 7079 2e6e  .    B : numpy.n
-00017030: 6461 7272 6179 2c20 6f70 7469 6f6e 616c  darray, optional
-00017040: 0a20 2020 2020 2020 2041 206e 756d 7079  .        A numpy
-00017050: 2e6e 6461 7272 6179 2077 6974 6820 7661  .ndarray with va
-00017060: 6c75 6573 2074 6f20 6265 206d 6170 7065  lues to be mappe
-00017070: 6420 6f6e 2042 2d66 6163 746f 7220 636f  d on B-factor co
-00017080: 6c75 6d6e 2069 6e20 6361 7669 7479 0a20  lumn in cavity. 
-00017090: 2020 2020 2020 2070 6f69 6e74 7320 2842         points (B
-000170a0: 5b6e 785d 5b6e 795d 5b6e 7a5d 292c 2062  [nx][ny][nz]), b
-000170b0: 7920 6465 6661 756c 7420 4e6f 6e65 2e0a  y default None..
-000170c0: 2020 2020 6f75 7470 7574 5f68 7964 726f      output_hydro
-000170d0: 7061 7468 7920 3a20 556e 696f 6e5b 7374  pathy : Union[st
-000170e0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
-000170f0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00017100: 2020 2041 2070 6174 6820 746f 2068 7964     A path to hyd
-00017110: 726f 7061 7468 7920 5044 4220 6669 6c65  ropathy PDB file
-00017120: 2028 7375 7266 6163 6520 706f 696e 7473   (surface points
-00017130: 206d 6170 7065 6420 7769 7468 2061 0a20   mapped with a. 
-00017140: 2020 2020 2020 2068 7964 726f 7068 6f62         hydrophob
-00017150: 6963 6974 7920 7363 616c 6529 2c20 6279  icity scale), by
-00017160: 2064 6566 6175 6c74 2060 6879 6472 6f70   default `hydrop
-00017170: 6174 6879 2e70 6462 602e 0a20 2020 2073  athy.pdb`..    s
-00017180: 6361 6c65 7320 3a20 6e75 6d70 792e 6e64  cales : numpy.nd
-00017190: 6172 7261 792c 206f 7074 696f 6e61 6c0a  array, optional.
-000171a0: 2020 2020 2020 2020 4120 6e75 6d70 792e          A numpy.
-000171b0: 6e64 6172 7261 7920 7769 7468 2068 7964  ndarray with hyd
-000171c0: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
-000171d0: 6520 7661 6c75 6573 2074 6f20 6265 206d  e values to be m
-000171e0: 6170 7065 6420 6f6e 0a20 2020 2020 2020  apped on.       
-000171f0: 2042 2d66 6163 746f 7220 636f 6c75 6d6e   B-factor column
-00017200: 2069 6e20 7375 7266 6163 6520 706f 696e   in surface poin
-00017210: 7473 2028 7363 616c 6573 5b6e 785d 5b6e  ts (scales[nx][n
-00017220: 795d 5b6e 7a5d 292c 2062 7920 6465 6661  y][nz]), by defa
-00017230: 756c 740a 2020 2020 2020 2020 4e6f 6e65  ult.        None
-00017240: 2e0a 2020 2020 7365 6c65 6374 696f 6e20  ..    selection 
-00017250: 3a20 556e 696f 6e5b 4c69 7374 5b69 6e74  : Union[List[int
-00017260: 5d2c 204c 6973 745b 7374 725d 5d2c 206f  ], List[str]], o
-00017270: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00017280: 4120 6c69 7374 206f 6620 696e 7465 6765  A list of intege
-00017290: 7220 6c61 6265 6c73 206f 7220 6120 6c69  r labels or a li
-000172a0: 7374 206f 6620 6361 7669 7479 206e 616d  st of cavity nam
-000172b0: 6573 2074 6f20 6265 2073 656c 6563 7465  es to be selecte
-000172c0: 642c 2062 7920 6465 6661 756c 7420 4e6f  d, by default No
-000172d0: 6e65 2e0a 2020 2020 6e74 6872 6561 6473  ne..    nthreads
-000172e0: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-000172f0: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
-00017300: 6f66 2074 6872 6561 6473 2c20 6279 2064  of threads, by d
-00017310: 6566 6175 6c74 204e 6f6e 652e 2049 6620  efault None. If 
-00017320: 4e6f 6e65 2c20 7468 6520 6e75 6d62 6572  None, the number
-00017330: 206f 6620 7468 7265 6164 7320 6973 0a20   of threads is. 
-00017340: 2020 2020 2020 2060 6f73 2e63 7075 5f63         `os.cpu_c
-00017350: 6f75 6e74 2829 202d 2031 602e 0a20 2020  ount() - 1`..   
-00017360: 2061 7070 656e 6420 3a20 626f 6f6c 2c20   append : bool, 
-00017370: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00017380: 2057 6865 7468 6572 2074 6f20 6170 7065   Whether to appe
-00017390: 6e64 2063 6176 6974 6965 7320 746f 2074  nd cavities to t
-000173a0: 6865 2050 4442 2066 696c 652c 2062 7920  he PDB file, by 
-000173b0: 6465 6661 756c 7420 4661 6c73 652e 0a20  default False.. 
-000173c0: 2020 206d 6f64 656c 203a 2069 6e74 2c20     model : int, 
-000173d0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-000173e0: 204d 6f64 656c 206e 756d 6265 722c 2062   Model number, b
-000173f0: 7920 6465 6661 756c 7420 302e 0a0a 2020  y default 0...  
-00017400: 2020 5261 6973 6573 0a20 2020 202d 2d2d    Raises.    ---
-00017410: 2d2d 2d0a 2020 2020 5479 7065 4572 726f  ---.    TypeErro
-00017420: 720a 2020 2020 2020 2020 6066 6e60 206d  r.        `fn` m
-00017430: 7573 7420 6265 2061 2073 7472 696e 6720  ust be a string 
-00017440: 6f72 2070 6174 686c 6962 2e50 6174 682e  or pathlib.Path.
-00017450: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
-00017460: 2020 2020 2020 2060 6361 7669 7469 6573         `cavities
-00017470: 6020 6d75 7374 2062 6520 6120 6e75 6d70  ` must be a nump
-00017480: 792e 6e64 6172 7261 792e 0a20 2020 2056  y.ndarray..    V
-00017490: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
-000174a0: 2020 6063 6176 6974 6965 7360 2068 6173    `cavities` has
-000174b0: 2074 6865 2069 6e63 6f72 7265 6374 2073   the incorrect s
-000174c0: 6861 7065 2e20 4974 206d 7573 7420 6265  hape. It must be
-000174d0: 2028 6e78 2c20 6e79 2c20 6e7a 292e 0a20   (nx, ny, nz).. 
-000174e0: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
-000174f0: 2020 2020 2060 7375 7266 6163 6560 206d       `surface` m
-00017500: 7573 7420 6265 2061 206e 756d 7079 2e6e  ust be a numpy.n
-00017510: 6461 7272 6179 2e0a 2020 2020 5661 6c75  darray..    Valu
-00017520: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-00017530: 7375 7266 6163 6560 2068 6173 2074 6865  surface` has the
-00017540: 2069 6e63 6f72 7265 6374 2073 6861 7065   incorrect shape
-00017550: 2e20 4974 206d 7573 7420 6265 2028 6e78  . It must be (nx
-00017560: 2c20 6e79 2c20 6e7a 292e 0a20 2020 2054  , ny, nz)..    T
-00017570: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-00017580: 2060 7665 7274 6963 6573 6020 6d75 7374   `vertices` must
-00017590: 2062 6520 6120 6c69 7374 206f 7220 6120   be a list or a 
-000175a0: 6e75 6d70 792e 6e64 6172 7261 792e 0a20  numpy.ndarray.. 
-000175b0: 2020 2056 616c 7565 4572 726f 720a 2020     ValueError.  
-000175c0: 2020 2020 2020 6076 6572 7469 6365 7360        `vertices`
-000175d0: 2068 6173 2069 6e63 6f72 7265 6374 2073   has incorrect s
-000175e0: 6861 7065 2e20 4974 206d 7573 7420 6265  hape. It must be
-000175f0: 2028 342c 2033 292e 0a20 2020 2054 7970   (4, 3)..    Typ
-00017600: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-00017610: 7374 6570 6020 6d75 7374 2062 6520 6120  step` must be a 
-00017620: 706f 7369 7469 7665 2072 6561 6c20 6e75  positive real nu
-00017630: 6d62 6572 2e0a 2020 2020 5661 6c75 6545  mber..    ValueE
-00017640: 7272 6f72 0a20 2020 2020 2020 2060 7374  rror.        `st
-00017650: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
-00017660: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
-00017670: 6572 2e0a 2020 2020 5479 7065 4572 726f  er..    TypeErro
-00017680: 720a 2020 2020 2020 2020 6042 6020 6d75  r.        `B` mu
-00017690: 7374 2062 6520 6120 6e75 6d70 792e 6e64  st be a numpy.nd
-000176a0: 6172 7261 792e 0a20 2020 2056 616c 7565  array..    Value
-000176b0: 4572 726f 720a 2020 2020 2020 2020 6042  Error.        `B
-000176c0: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
-000176d0: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
-000176e0: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
-000176f0: 7a29 2e0a 2020 2020 5479 7065 4572 726f  z)..    TypeErro
-00017700: 720a 2020 2020 2020 2020 606f 7574 7075  r.        `outpu
-00017710: 745f 6879 6472 6f70 6174 6879 6020 6d75  t_hydropathy` mu
-00017720: 7374 2062 6520 6120 7374 7269 6e67 2e0a  st be a string..
-00017730: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
-00017740: 2020 2020 2020 6073 6361 6c65 7360 206d        `scales` m
-00017750: 7573 7420 6265 2061 206e 756d 7079 2e6e  ust be a numpy.n
-00017760: 6461 7272 6179 2e0a 2020 2020 5661 6c75  darray..    Valu
+000114c0: 6b61 6765 2063 6f6e 7461 696e 7320 7365  kage contains se
+000114d0: 7665 6e20 6275 696c 742d 696e 2068 7964  ven built-in hyd
+000114e0: 726f 7068 6f62 6963 6974 7920 7363 616c  rophobicity scal
+000114f0: 6573 3a0a 0a20 2020 2020 2020 2020 2020  es:..           
+00011500: 202a 2045 6973 656e 6265 7267 5765 6973   * EisenbergWeis
+00011510: 7320 5b31 5d5f 3b0a 2020 2020 2020 2020  s [1]_;.        
+00011520: 2020 2020 2a20 4865 7373 6148 6569 6a6e      * HessaHeijn
+00011530: 6520 5b32 5d5f 3b0a 2020 2020 2020 2020  e [2]_;.        
+00011540: 2020 2020 2a20 4b79 7465 446f 6f6c 6974      * KyteDoolit
+00011550: 746c 6520 5b33 5d5f 3b0a 2020 2020 2020  tle [3]_;.      
+00011560: 2020 2020 2020 2a20 4d6f 6f6e 466c 656d        * MoonFlem
+00011570: 696e 6720 5b34 5d5f 3b0a 2020 2020 2020  ing [4]_;.      
+00011580: 2020 2020 2020 2a20 5261 647a 6963 6b61        * Radzicka
+00011590: 576f 6c66 656e 6465 6e20 5b35 5d5f 3b0a  Wolfenden [5]_;.
+000115a0: 2020 2020 2020 2020 2020 2020 2a20 5769              * Wi
+000115b0: 6d6c 6579 5768 6974 6520 5b36 5d5f 3b0a  mleyWhite [6]_;.
+000115c0: 2020 2020 2020 2020 2020 2020 2a20 5a68              * Zh
+000115d0: 616f 4c6f 6e64 6f6e 205b 375d 5f2e 0a0a  aoLondon [7]_...
+000115e0: 2020 2020 6967 6e6f 7265 5f62 6163 6b62      ignore_backb
+000115f0: 6f6e 6520 3a20 626f 6f6c 2c20 6f70 7469  one : bool, opti
+00011600: 6f6e 616c 0a20 2020 2020 2020 2057 6865  onal.        Whe
+00011610: 7468 6572 2074 6f20 6967 6e6f 7265 2062  ther to ignore b
+00011620: 6163 6b62 6f6e 6520 6174 6f6d 7320 2843  ackbone atoms (C
+00011630: 2c20 4341 2c20 4e2c 204f 2920 7768 656e  , CA, N, O) when
+00011640: 2064 6566 696e 696e 6720 696e 7465 7266   defining interf
+00011650: 6163 650a 2020 2020 2020 2020 7265 7369  ace.        resi
+00011660: 6475 6573 2c20 6279 2064 6566 6175 6c74  dues, by default
+00011670: 2046 616c 7365 2e0a 2020 2020 7365 6c65   False..    sele
+00011680: 6374 696f 6e20 3a20 556e 696f 6e5b 4c69  ction : Union[Li
+00011690: 7374 5b69 6e74 5d2c 204c 6973 745b 7374  st[int], List[st
+000116a0: 725d 5d2c 206f 7074 696f 6e61 6c0a 2020  r]], optional.  
+000116b0: 2020 2020 2020 4120 6c69 7374 206f 6620        A list of 
+000116c0: 696e 7465 6765 7220 6c61 6265 6c73 206f  integer labels o
+000116d0: 7220 6120 6c69 7374 206f 6620 6361 7669  r a list of cavi
+000116e0: 7479 206e 616d 6573 2074 6f20 6265 2073  ty names to be s
+000116f0: 656c 6563 7465 642c 2062 7920 6465 6661  elected, by defa
+00011700: 756c 7420 4e6f 6e65 2e0a 2020 2020 6e74  ult None..    nt
+00011710: 6872 6561 6473 203a 2069 6e74 2c20 6f70  hreads : int, op
+00011720: 7469 6f6e 616c 0a20 2020 2020 2020 204e  tional.        N
+00011730: 756d 6265 7220 6f66 2074 6872 6561 6473  umber of threads
+00011740: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
+00011750: 652e 2049 6620 4e6f 6e65 2c20 7468 6520  e. If None, the 
+00011760: 6e75 6d62 6572 206f 6620 7468 7265 6164  number of thread
+00011770: 7320 6973 0a20 2020 2020 2020 2060 6f73  s is.        `os
+00011780: 2e63 7075 5f63 6f75 6e74 2829 202d 2031  .cpu_count() - 1
+00011790: 602e 0a20 2020 2076 6572 626f 7365 203a  `..    verbose :
+000117a0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+000117b0: 2020 2020 2020 2020 5072 696e 7420 6578          Print ex
+000117c0: 7472 6120 696e 666f 726d 6174 696f 6e20  tra information 
+000117d0: 746f 2073 7461 6e64 6172 6420 6f75 7470  to standard outp
+000117e0: 7574 2c20 6279 2064 6566 6175 6c74 2046  ut, by default F
+000117f0: 616c 7365 2e0a 0a20 2020 2052 6574 7572  alse...    Retur
+00011800: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00011810: 2020 2073 6361 6c65 7320 3a20 6e75 6d70     scales : nump
+00011820: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
+00011830: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
+00011840: 7920 7769 7468 2068 7964 726f 7068 6f62  y with hydrophob
+00011850: 6963 6974 7920 7363 616c 6520 7661 6c75  icity scale valu
+00011860: 6520 6d61 7070 6564 2061 7420 7375 7266  e mapped at surf
+00011870: 6163 650a 2020 2020 2020 2020 706f 696e  ace.        poin
+00011880: 7473 2028 7363 616c 6573 5b6e 785d 5b6e  ts (scales[nx][n
+00011890: 795d 5b6e 7a5d 292e 0a20 2020 2061 7667  y][nz])..    avg
+000118a0: 5f68 7964 726f 7061 7468 7920 3a20 4469  _hydropathy : Di
+000118b0: 6374 5b73 7472 2c20 666c 6f61 745d 0a20  ct[str, float]. 
+000118c0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
+000118d0: 6172 7920 7769 7468 2061 7665 7261 6765  ary with average
+000118e0: 2068 7964 726f 7061 7468 7920 666f 7220   hydropathy for 
+000118f0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00011900: 7669 7479 2061 6e64 0a20 2020 2020 2020  vity and.       
+00011910: 2074 6865 2072 616e 6765 206f 6620 7468   the range of th
+00011920: 6520 6879 6472 6f70 686f 6269 6369 7479  e hydrophobicity
+00011930: 2073 6361 6c65 2028 6d69 6e2c 206d 6178   scale (min, max
+00011940: 292e 0a0a 2020 2020 5261 6973 6573 0a20  )...    Raises. 
+00011950: 2020 202d 2d2d 2d2d 2d0a 2020 2020 5479     ------.    Ty
+00011960: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+00011970: 6073 7572 6661 6365 6020 6d75 7374 2062  `surface` must b
+00011980: 6520 6120 6e75 6d70 792e 6e64 6172 7261  e a numpy.ndarra
+00011990: 792e 0a20 2020 2056 616c 7565 4572 726f  y..    ValueErro
+000119a0: 720a 2020 2020 2020 2020 6073 7572 6661  r.        `surfa
+000119b0: 6365 6020 6861 7320 7468 6520 696e 636f  ce` has the inco
+000119c0: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+000119d0: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+000119e0: 206e 7a29 2e0a 2020 2020 5479 7065 4572   nz)..    TypeEr
+000119f0: 726f 720a 2020 2020 2020 2020 6061 746f  ror.        `ato
+00011a00: 6d69 6360 206d 7573 7420 6265 2061 206c  mic` must be a l
+00011a10: 6973 7420 6f72 2061 206e 756d 7079 2e6e  ist or a numpy.n
+00011a20: 6461 7272 6179 2e0a 2020 2020 5661 6c75  darray..    Valu
+00011a30: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
+00011a40: 6174 6f6d 6963 6020 6861 7320 696e 636f  atomic` has inco
+00011a50: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+00011a60: 6d75 7374 2062 6520 286e 2c20 3829 2e0a  must be (n, 8)..
+00011a70: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
+00011a80: 2020 2020 2020 6076 6572 7469 6365 7360        `vertices`
+00011a90: 206d 7573 7420 6265 2061 206c 6973 7420   must be a list 
+00011aa0: 6f72 2061 206e 756d 7079 2e6e 6461 7272  or a numpy.ndarr
+00011ab0: 6179 2e0a 2020 2020 5661 6c75 6545 7272  ay..    ValueErr
+00011ac0: 6f72 0a20 2020 2020 2020 2060 7665 7274  or.        `vert
+00011ad0: 6963 6573 6020 6861 7320 696e 636f 7272  ices` has incorr
+00011ae0: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
+00011af0: 7374 2062 6520 2834 2c20 3329 2e0a 2020  st be (4, 3)..  
+00011b00: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
+00011b10: 2020 2020 6073 7465 7060 206d 7573 7420      `step` must 
+00011b20: 6265 2061 2070 6f73 6974 6976 6520 7265  be a positive re
+00011b30: 616c 206e 756d 6265 722e 0a20 2020 2056  al number..    V
+00011b40: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
+00011b50: 2020 6073 7465 7060 206d 7573 7420 6265    `step` must be
+00011b60: 2061 2070 6f73 6974 6976 6520 7265 616c   a positive real
+00011b70: 206e 756d 6265 722e 0a20 2020 2054 7970   number..    Typ
+00011b80: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
+00011b90: 7072 6f62 655f 696e 6020 6d75 7374 2062  probe_in` must b
+00011ba0: 6520 6120 6e6f 6e2d 6e65 6761 7469 7665  e a non-negative
+00011bb0: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
+00011bc0: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+00011bd0: 2020 2020 2060 7072 6f62 655f 696e 6020       `probe_in` 
+00011be0: 6d75 7374 2062 6520 6120 6e6f 6e2d 6e65  must be a non-ne
+00011bf0: 6761 7469 7665 2072 6561 6c20 6e75 6d62  gative real numb
+00011c00: 6572 2e0a 2020 2020 5479 7065 4572 726f  er..    TypeErro
+00011c10: 720a 2020 2020 2020 2020 6068 7964 726f  r.        `hydro
+00011c20: 7068 6f62 6963 6974 795f 7363 616c 6560  phobicity_scale`
+00011c30: 206d 7573 7420 6265 2061 2073 7472 696e   must be a strin
+00011c40: 6720 6f72 2061 2070 6174 686c 6962 2e50  g or a pathlib.P
+00011c50: 6174 682e 0a20 2020 2054 7970 6545 7272  ath..    TypeErr
+00011c60: 6f72 0a20 2020 2020 2020 2060 6967 6e6f  or.        `igno
+00011c70: 7265 5f62 6163 6b62 6f6e 6560 206d 7573  re_backbone` mus
+00011c80: 7420 6265 2061 2062 6f6f 6c65 616e 2e0a  t be a boolean..
+00011c90: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
+00011ca0: 2020 2020 2020 6073 656c 6563 7469 6f6e        `selection
+00011cb0: 6020 6d75 7374 2062 6520 6120 6c69 7374  ` must be a list
+00011cc0: 206f 6620 7374 7269 6e67 7320 2863 6176   of strings (cav
+00011cd0: 6974 7920 6e61 6d65 7329 206f 7220 696e  ity names) or in
+00011ce0: 7465 6765 7273 2028 6361 7669 7479 206c  tegers (cavity l
+00011cf0: 6162 656c 7329 2e0a 2020 2020 5661 6c75  abels)..    Valu
+00011d00: 6545 7272 6f72 0a20 2020 2020 2020 2049  eError.        I
+00011d10: 6e76 616c 6964 2060 7365 6c65 6374 696f  nvalid `selectio
+00011d20: 6e60 3a20 7b73 656c 6563 7469 6f6e 7d2e  n`: {selection}.
+00011d30: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
+00011d40: 2020 2020 2020 2060 6e74 6872 6561 6473         `nthreads
+00011d50: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+00011d60: 7469 7665 2069 6e74 6567 6572 2e0a 2020  tive integer..  
+00011d70: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+00011d80: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
+00011d90: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+00011da0: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
+00011db0: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
+00011dc0: 2020 6076 6572 626f 7365 6020 6d75 7374    `verbose` must
+00011dd0: 2062 6520 6120 626f 6f6c 6561 6e2e 0a0a   be a boolean...
+00011de0: 2020 2020 4e6f 7465 0a20 2020 202d 2d2d      Note.    ---
+00011df0: 2d0a 2020 2020 5468 6520 6361 7669 7479  -.    The cavity
+00011e00: 206e 6f6d 656e 636c 6174 7572 6520 6973   nomenclature is
+00011e10: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
+00011e20: 7465 6765 7220 6c61 6265 6c2e 2054 6865  teger label. The
+00011e30: 2063 6176 6974 7920 6d61 726b 6564 0a20   cavity marked. 
+00011e40: 2020 2077 6974 6820 322c 2074 6865 2066     with 2, the f
+00011e50: 6972 7374 2069 6e74 6567 6572 2063 6f72  irst integer cor
+00011e60: 7265 7370 6f6e 6469 6e67 2074 6f20 6120  responding to a 
+00011e70: 6361 7669 7479 2c20 6973 204b 4141 2c20  cavity, is KAA, 
+00011e80: 7468 6520 6361 7669 7479 0a20 2020 206d  the cavity.    m
+00011e90: 6172 6b65 6420 7769 7468 2033 2069 7320  arked with 3 is 
+00011ea0: 4b41 422c 2074 6865 2063 6176 6974 7920  KAB, the cavity 
+00011eb0: 6d61 726b 6564 2077 6974 6820 3420 6973  marked with 4 is
+00011ec0: 204b 4143 2061 6e64 2073 6f20 6f6e 2e0a   KAC and so on..
+00011ed0: 0a20 2020 2053 6565 2041 6c73 6f0a 2020  .    See Also.  
+00011ee0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072    --------.    r
+00011ef0: 6561 645f 7064 620a 2020 2020 7265 6164  ead_pdb.    read
+00011f00: 5f78 797a 0a20 2020 2073 7061 7469 616c  _xyz.    spatial
+00011f10: 0a20 2020 2065 7870 6f72 740a 2020 2020  .    export.    
+00011f20: 7772 6974 655f 7265 7375 6c74 730a 0a20  write_results.. 
+00011f30: 2020 2045 7861 6d70 6c65 0a20 2020 202d     Example.    -
+00011f40: 2d2d 2d2d 2d2d 0a20 2020 2057 6974 6820  ------.    With 
+00011f50: 7468 6520 7375 7266 6163 6520 706f 696e  the surface poin
+00011f60: 7473 2069 6465 6e74 6966 6965 6420 7769  ts identified wi
+00011f70: 7468 2060 6070 794b 5646 696e 6465 722e  th ``pyKVFinder.
+00011f80: 7370 6174 6961 6c60 6020 616e 6420 6174  spatial`` and at
+00011f90: 6f6d 6963 2063 6f6f 7264 696e 6174 6573  omic coordinates
+00011fa0: 2061 6e64 2069 6e66 6f72 6d61 7469 6f6e   and information
+00011fb0: 2072 6561 6420 7769 7468 2060 6070 794b   read with ``pyK
+00011fc0: 5646 696e 6465 722e 7265 6164 5f70 6462  VFinder.read_pdb
+00011fd0: 6060 206f 7220 6060 7079 4b56 4669 6e64  `` or ``pyKVFind
+00011fe0: 6572 2e72 6561 645f 7879 7a60 602c 2077  er.read_xyz``, w
+00011ff0: 6520 6361 6e20 7065 7266 6f72 6d20 6120  e can perform a 
+00012000: 6879 6472 6f70 6174 6879 2063 6861 7261  hydropathy chara
+00012010: 6374 6572 697a 6174 696f 6e2c 2074 6861  cterization, tha
+00012020: 7420 6d61 7073 2061 2074 6172 6765 7420  t maps a target 
+00012030: 6879 6472 6f70 686f 6269 6369 7479 2073  hydrophobicity s
+00012040: 6361 6c65 206f 6e20 7375 7266 6163 6520  cale on surface 
+00012050: 706f 696e 7473 2061 6e64 2063 616c 6375  points and calcu
+00012060: 6c61 7465 2074 6865 2061 7665 7261 6765  late the average
+00012070: 2068 7964 726f 7061 7468 790a 0a20 2020   hydropathy..   
+00012080: 203e 3e3e 2066 726f 6d20 7079 4b56 4669   >>> from pyKVFi
+00012090: 6e64 6572 2069 6d70 6f72 7420 6879 6472  nder import hydr
+000120a0: 6f70 6174 6879 0a20 2020 203e 3e3e 2073  opathy.    >>> s
+000120b0: 6361 6c65 732c 2061 7667 5f68 7964 726f  cales, avg_hydro
+000120c0: 7061 7468 7920 3d20 6879 6472 6f70 6174  pathy = hydropat
+000120d0: 6879 2873 7572 6661 6365 2c20 6174 6f6d  hy(surface, atom
+000120e0: 6963 2c20 7665 7274 6963 6573 290a 2020  ic, vertices).  
+000120f0: 2020 3e3e 3e20 7363 616c 6573 0a20 2020    >>> scales.   
+00012100: 2061 7272 6179 285b 5b5b 302e 2c20 302e   array([[[0., 0.
+00012110: 2c20 302e 2c20 2e2e 2e2c 2030 2e2c 2030  , 0., ..., 0., 0
+00012120: 2e2c 2030 2e5d 2c0a 2020 2020 2020 2020  ., 0.],.        
+00012130: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+00012140: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+00012150: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00012160: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
+00012170: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
+00012180: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
+00012190: 2020 2020 2020 2020 2020 205b 302e 2c20             [0., 
+000121a0: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
+000121b0: 2030 2e2c 2030 2e5d 2c0a 2020 2020 2020   0., 0.],.      
+000121c0: 2020 2020 2020 5b30 2e2c 2030 2e2c 2030        [0., 0., 0
+000121d0: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+000121e0: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
+000121f0: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
+00012200: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 5d2c  ., 0., 0., 0.]],
+00012210: 0a20 2020 2020 2020 2020 202e 2e2e 2c0a  .          ...,.
+00012220: 2020 2020 2020 2020 2020 5b5b 302e 2c20            [[0., 
+00012230: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
+00012240: 2030 2e2c 2030 2e5d 2c0a 2020 2020 2020   0., 0.],.      
+00012250: 2020 2020 2020 5b30 2e2c 2030 2e2c 2030        [0., 0., 0
+00012260: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+00012270: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
+00012280: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
+00012290: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
+000122a0: 2020 2020 2020 2020 2020 2020 2e2e 2e2c              ...,
+000122b0: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+000122c0: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
+000122d0: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
+000122e0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+000122f0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+00012300: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+00012310: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
+00012320: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
+00012330: 5d5d 290a 2020 2020 3e3e 3e20 6176 675f  ]]).    >>> avg_
+00012340: 6879 6472 6f70 6174 6879 0a20 2020 207b  hydropathy.    {
+00012350: 274b 4141 273a 202d 302e 3733 2c20 274b  'KAA': -0.73, 'K
+00012360: 4142 273a 202d 302e 3035 2c20 274b 4143  AB': -0.05, 'KAC
+00012370: 273a 202d 302e 3037 2c20 274b 4144 273a  ': -0.07, 'KAD':
+00012380: 202d 302e 3632 2c20 274b 4145 273a 202d   -0.62, 'KAE': -
+00012390: 302e 3831 2c20 274b 4146 273a 202d 302e  0.81, 'KAF': -0.
+000123a0: 3134 2c20 274b 4147 273a 202d 302e 3333  14, 'KAG': -0.33
+000123b0: 2c20 274b 4148 273a 202d 302e 3136 2c20  , 'KAH': -0.16, 
+000123c0: 274b 4149 273a 202d 302e 342c 2027 4b41  'KAI': -0.4, 'KA
+000123d0: 4a27 3a20 302e 3632 2c20 274b 414b 273a  J': 0.62, 'KAK':
+000123e0: 202d 302e 3939 2c20 274b 414c 273a 2030   -0.99, 'KAL': 0
+000123f0: 2e33 362c 2027 4b41 4d27 3a20 2d30 2e33  .36, 'KAM': -0.3
+00012400: 332c 2027 4b41 4e27 3a20 302e 3138 2c20  3, 'KAN': 0.18, 
+00012410: 274b 414f 273a 2030 2e38 382c 2027 4b41  'KAO': 0.88, 'KA
+00012420: 5027 3a20 2d30 2e39 362c 2027 4b41 5127  P': -0.96, 'KAQ'
+00012430: 3a20 302e 3438 2c20 274b 4152 273a 2030  : 0.48, 'KAR': 0
+00012440: 2e32 342c 2027 4569 7365 6e62 6572 6757  .24, 'EisenbergW
+00012450: 6569 7373 273a 205b 2d31 2e34 322c 2032  eiss': [-1.42, 2
+00012460: 2e36 5d7d 0a0a 2020 2020 486f 7765 7665  .6]}..    Howeve
+00012470: 722c 2075 7365 7273 206d 6179 206f 7074  r, users may opt
+00012480: 2074 6f20 6967 6e6f 7265 2062 6163 6b62   to ignore backb
+00012490: 6f6e 6573 2063 6f6e 7461 6374 7320 2843  ones contacts (C
+000124a0: 2c20 4341 2c20 4e2c 204f 2920 7769 7468  , CA, N, O) with
+000124b0: 2074 6865 2063 6176 6974 7920 7768 656e   the cavity when
+000124c0: 206d 6170 7069 6e67 2068 7964 726f 7068   mapping hydroph
+000124d0: 6f62 6963 6974 7920 7363 616c 6573 206f  obicity scales o
+000124e0: 6e20 7375 7266 6163 6520 706f 696e 7473  n surface points
+000124f0: 2e20 5468 656e 2c20 7573 6572 7320 6d75  . Then, users mu
+00012500: 7374 2073 6574 2060 6069 676e 6f72 655f  st set ``ignore_
+00012510: 6261 636b 626f 6e65 6060 2066 6c61 6720  backbone`` flag 
+00012520: 746f 2060 6054 7275 6560 602e 0a0a 2020  to ``True``...  
+00012530: 2020 3e3e 3e20 6672 6f6d 2070 794b 5646    >>> from pyKVF
+00012540: 696e 6465 7220 696d 706f 7274 2068 7964  inder import hyd
+00012550: 726f 7061 7468 790a 2020 2020 3e3e 3e20  ropathy.    >>> 
+00012560: 7363 616c 6573 2c20 6176 675f 6879 6472  scales, avg_hydr
+00012570: 6f70 6174 6879 203d 2068 7964 726f 7061  opathy = hydropa
+00012580: 7468 7928 7375 7266 6163 652c 2061 746f  thy(surface, ato
+00012590: 6d69 632c 2076 6572 7469 6365 732c 2069  mic, vertices, i
+000125a0: 676e 6f72 655f 6261 636b 626f 6e65 3d54  gnore_backbone=T
+000125b0: 7275 6529 0a20 2020 203e 3e3e 2073 6361  rue).    >>> sca
+000125c0: 6c65 730a 2020 2020 6172 7261 7928 5b5b  les.    array([[
+000125d0: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
+000125e0: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
+000125f0: 2020 2020 2020 2020 2020 205b 302e 2c20             [0., 
+00012600: 302e 2c20 302e 2c20 2e2e 2e2c 2030 2e2c  0., 0., ..., 0.,
+00012610: 2030 2e2c 2030 2e5d 2c0a 2020 2020 2020   0., 0.],.      
+00012620: 2020 2020 2020 5b30 2e2c 2030 2e2c 2030        [0., 0., 0
+00012630: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+00012640: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
+00012650: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00012660: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
+00012670: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
+00012680: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+00012690: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
+000126a0: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
+000126b0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+000126c0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+000126d0: 2c20 302e 5d5d 2c0a 2020 2020 2020 2020  , 0.]],.        
+000126e0: 2020 2e2e 2e2c 0a20 2020 2020 2020 2020    ...,.         
+000126f0: 205b 5b30 2e2c 2030 2e2c 2030 2e2c 202e   [[0., 0., 0., .
+00012700: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
+00012710: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+00012720: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
+00012730: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
+00012740: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+00012750: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+00012760: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+00012770: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+00012780: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
+00012790: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
+000127a0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+000127b0: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
+000127c0: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
+000127d0: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
+000127e0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
+000127f0: 302e 2c20 302e 5d5d 5d29 0a20 2020 203e  0., 0.]]]).    >
+00012800: 3e3e 2061 7667 5f68 7964 726f 7061 7468  >> avg_hydropath
+00012810: 790a 2020 2020 7b27 4b41 4127 3a20 2d30  y.    {'KAA': -0
+00012820: 2e37 2c20 274b 4142 273a 2030 2e31 322c  .7, 'KAB': 0.12,
+00012830: 2027 4b41 4327 3a20 2d30 2e30 382c 2027   'KAC': -0.08, '
+00012840: 4b41 4427 3a20 2d30 2e35 362c 2027 4b41  KAD': -0.56, 'KA
+00012850: 4527 3a20 2d30 2e32 382c 2027 4b41 4627  E': -0.28, 'KAF'
+00012860: 3a20 2d30 2e32 352c 2027 4b41 4727 3a20  : -0.25, 'KAG': 
+00012870: 2d30 2e32 382c 2027 4b41 4827 3a20 2d30  -0.28, 'KAH': -0
+00012880: 2e30 392c 2027 4b41 4927 3a20 2d30 2e34  .09, 'KAI': -0.4
+00012890: 2c20 274b 414a 273a 2030 2e39 362c 2027  , 'KAJ': 0.96, '
+000128a0: 4b41 4b27 3a20 2d30 2e38 372c 2027 4b41  KAK': -0.87, 'KA
+000128b0: 4c27 3a20 302e 3233 2c20 274b 414d 273a  L': 0.23, 'KAM':
+000128c0: 2030 2e30 362c 2027 4b41 4e27 3a20 2d30   0.06, 'KAN': -0
+000128d0: 2e31 2c20 274b 414f 273a 2030 2e39 392c  .1, 'KAO': 0.99,
+000128e0: 2027 4b41 5027 3a20 2d31 2e30 342c 2027   'KAP': -1.04, '
+000128f0: 4b41 5127 3a20 302e 3438 2c20 274b 4152  KAQ': 0.48, 'KAR
+00012900: 273a 202d 302e 3834 2c20 2745 6973 656e  ': -0.84, 'Eisen
+00012910: 6265 7267 5765 6973 7327 3a20 5b2d 312e  bergWeiss': [-1.
+00012920: 3432 2c20 322e 365d 7d0a 0a20 2020 2052  42, 2.6]}..    R
+00012930: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
+00012940: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
+00012950: 5b31 5d20 4569 7365 6e62 6572 6720 442c  [1] Eisenberg D,
+00012960: 2057 6569 7373 2052 4d2c 2054 6572 7769   Weiss RM, Terwi
+00012970: 6c6c 6967 6572 2054 432e 2054 6865 2068  lliger TC. The h
+00012980: 7964 726f 7068 6f62 6963 206d 6f6d 656e  ydrophobic momen
+00012990: 740a 2020 2020 2020 2064 6574 6563 7473  t.       detects
+000129a0: 2070 6572 696f 6469 6369 7479 2069 6e20   periodicity in 
+000129b0: 7072 6f74 6569 6e20 6879 6472 6f70 686f  protein hydropho
+000129c0: 6269 6369 7479 2e20 5072 6f63 6565 6469  bicity. Proceedi
+000129d0: 6e67 7320 6f66 2074 6865 0a20 2020 2020  ngs of the.     
+000129e0: 2020 4e61 7469 6f6e 616c 2041 6361 6465    National Acade
+000129f0: 6d79 206f 6620 5363 6965 6e63 6573 2e20  my of Sciences. 
+00012a00: 3139 3834 3b38 312e 0a0a 2020 2020 2e2e  1984;81...    ..
+00012a10: 205b 325d 2048 6573 7361 2054 2c20 4b69   [2] Hessa T, Ki
+00012a20: 6d20 482c 2042 6968 6c6d 6169 6572 204b  m H, Bihlmaier K
+00012a30: 2c20 4c75 6e64 696e 2043 2c20 426f 656b  , Lundin C, Boek
+00012a40: 656c 204a 2c20 416e 6465 7273 736f 6e20  el J, Andersson 
+00012a50: 482c 2065 7420 616c 2e0a 2020 2020 2020  H, et al..      
+00012a60: 2052 6563 6f67 6e69 7469 6f6e 206f 6620   Recognition of 
+00012a70: 7472 616e 736d 656d 6272 616e 6520 6865  transmembrane he
+00012a80: 6c69 6365 7320 6279 2074 6865 2065 6e64  lices by the end
+00012a90: 6f70 6c61 736d 6963 2072 6574 6963 756c  oplasmic reticul
+00012aa0: 756d 0a20 2020 2020 2020 7472 616e 736c  um.       transl
+00012ab0: 6f63 6f6e 2e20 4e61 7475 7265 2e20 3230  ocon. Nature. 20
+00012ac0: 3035 3b34 3333 2e0a 0a20 2020 202e 2e20  05;433...    .. 
+00012ad0: 5b33 5d20 4b79 7465 204a 2c20 446f 6f6c  [3] Kyte J, Dool
+00012ae0: 6974 746c 6520 5246 2e20 4120 7369 6d70  ittle RF. A simp
+00012af0: 6c65 206d 6574 686f 6420 666f 7220 6469  le method for di
+00012b00: 7370 6c61 7969 6e67 2074 6865 2068 7964  splaying the hyd
+00012b10: 726f 7061 7468 6963 0a20 2020 2020 2020  ropathic.       
+00012b20: 6368 6172 6163 7465 7220 6f66 2061 2070  character of a p
+00012b30: 726f 7465 696e 2e20 4a6f 7572 6e61 6c20  rotein. Journal 
+00012b40: 6f66 204d 6f6c 6563 756c 6172 2042 696f  of Molecular Bio
+00012b50: 6c6f 6779 2e20 3139 3832 3b31 3537 2e0a  logy. 1982;157..
+00012b60: 0a20 2020 202e 2e20 5b34 5d20 4d6f 6f6e  .    .. [4] Moon
+00012b70: 2043 502c 2046 6c65 6d69 6e67 204b 472e   CP, Fleming KG.
+00012b80: 2053 6964 652d 6368 6169 6e20 6879 6472   Side-chain hydr
+00012b90: 6f70 686f 6269 6369 7479 2073 6361 6c65  ophobicity scale
+00012ba0: 2064 6572 6976 6564 2066 726f 6d0a 2020   derived from.  
+00012bb0: 2020 2020 2074 7261 6e73 6d65 6d62 7261       transmembra
+00012bc0: 6e65 2070 726f 7465 696e 2066 6f6c 6469  ne protein foldi
+00012bd0: 6e67 2069 6e74 6f20 6c69 7069 6420 6269  ng into lipid bi
+00012be0: 6c61 7965 7273 2e20 5072 6f63 6565 6469  layers. Proceedi
+00012bf0: 6e67 7320 6f66 2074 6865 0a20 2020 2020  ngs of the.     
+00012c00: 2020 4e61 7469 6f6e 616c 2041 6361 6465    National Acade
+00012c10: 6d79 206f 6620 5363 6965 6e63 6573 2e20  my of Sciences. 
+00012c20: 3230 3131 3b31 3038 2e0a 0a20 2020 202e  2011;108...    .
+00012c30: 2e20 5b35 5d20 5261 647a 6963 6b61 2041  . [5] Radzicka A
+00012c40: 2c20 576f 6c66 656e 6465 6e20 522e 2043  , Wolfenden R. C
+00012c50: 6f6d 7061 7269 6e67 2074 6865 2070 6f6c  omparing the pol
+00012c60: 6172 6974 6965 7320 6f66 2074 6865 2061  arities of the a
+00012c70: 6d69 6e6f 2061 6369 6473 3a0a 2020 2020  mino acids:.    
+00012c80: 2020 2020 5369 6465 2d63 6861 696e 2064      Side-chain d
+00012c90: 6973 7472 6962 7574 696f 6e20 636f 6566  istribution coef
+00012ca0: 6669 6369 656e 7473 2062 6574 7765 656e  ficients between
+00012cb0: 2074 6865 2076 6170 6f72 2070 6861 7365   the vapor phase
+00012cc0: 2c20 6379 636c 6f68 6578 616e 652c 0a20  , cyclohexane,. 
+00012cd0: 2020 2020 2020 2031 2d6f 6374 616e 6f6c         1-octanol
+00012ce0: 2c20 616e 6420 6e65 7574 7261 6c20 6171  , and neutral aq
+00012cf0: 7565 6f75 7320 736f 6c75 7469 6f6e 2e20  ueous solution. 
+00012d00: 4269 6f63 6865 6d69 7374 7279 2e20 3139  Biochemistry. 19
+00012d10: 3838 3b32 372e 0a0a 2020 2020 2e2e 205b  88;27...    .. [
+00012d20: 365d 2057 696d 6c65 7920 5743 2c20 5768  6] Wimley WC, Wh
+00012d30: 6974 6520 5348 2e20 4578 7065 7269 6d65  ite SH. Experime
+00012d40: 6e74 616c 6c79 2064 6574 6572 6d69 6e65  ntally determine
+00012d50: 6420 6879 6472 6f70 686f 6269 6369 7479  d hydrophobicity
+00012d60: 2073 6361 6c65 0a20 2020 2020 2020 666f   scale.       fo
+00012d70: 7220 7072 6f74 6569 6e73 2061 7420 6d65  r proteins at me
+00012d80: 6d62 7261 6e65 2069 6e74 6572 6661 6365  mbrane interface
+00012d90: 732e 204e 6174 7572 6520 5374 7275 6374  s. Nature Struct
+00012da0: 7572 616c 2026 204d 6f6c 6563 756c 6172  ural & Molecular
+00012db0: 0a20 2020 2020 2020 4269 6f6c 6f67 792e  .       Biology.
+00012dc0: 2031 3939 363b 332e 0a0a 2020 2020 2e2e   1996;3...    ..
+00012dd0: 205b 375d 205a 6861 6f20 472c 204c 6f6e   [7] Zhao G, Lon
+00012de0: 646f 6e20 452e 2041 6e20 616d 696e 6f20  don E. An amino 
+00012df0: 6163 6964 20e2 809c 7472 616e 736d 656d  acid ...transmem
+00012e00: 6272 616e 6520 7465 6e64 656e 6379 e280  brane tendency..
+00012e10: 9d20 7363 616c 6520 7468 6174 0a20 2020  . scale that.   
+00012e20: 2020 2020 6170 7072 6f61 6368 6573 2074      approaches t
+00012e30: 6865 2074 6865 6f72 6574 6963 616c 206c  he theoretical l
+00012e40: 696d 6974 2074 6f20 6163 6375 7261 6379  imit to accuracy
+00012e50: 2066 6f72 2070 7265 6469 6374 696f 6e20   for prediction 
+00012e60: 6f66 0a20 2020 2020 2020 7472 616e 736d  of.       transm
+00012e70: 656d 6272 616e 6520 6865 6c69 6365 733a  embrane helices:
+00012e80: 2052 656c 6174 696f 6e73 6869 7020 746f   Relationship to
+00012e90: 2062 696f 6c6f 6769 6361 6c20 6879 6472   biological hydr
+00012ea0: 6f70 686f 6269 6369 7479 2e0a 2020 2020  ophobicity..    
+00012eb0: 2020 2050 726f 7465 696e 2053 6369 656e     Protein Scien
+00012ec0: 6365 2e20 3230 3036 3b31 352e 0a20 2020  ce. 2006;15..   
+00012ed0: 2022 2222 0a20 2020 2069 6d70 6f72 7420   """.    import 
+00012ee0: 746f 6d6c 0a20 2020 2066 726f 6d20 5f70  toml.    from _p
+00012ef0: 794b 5646 696e 6465 7220 696d 706f 7274  yKVFinder import
+00012f00: 205f 6879 6472 6f70 6174 6879 0a0a 2020   _hydropathy..  
+00012f10: 2020 2320 4368 6563 6b20 6172 6775 6d65    # Check argume
+00012f20: 6e74 730a 2020 2020 6966 2074 7970 6528  nts.    if type(
+00012f30: 7375 7266 6163 6529 206e 6f74 2069 6e20  surface) not in 
+00012f40: 5b6e 756d 7079 2e6e 6461 7272 6179 5d3a  [numpy.ndarray]:
+00012f50: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
+00012f60: 7970 6545 7272 6f72 2822 6073 7572 6661  ypeError("`surfa
+00012f70: 6365 6020 6d75 7374 2062 6520 6120 6e75  ce` must be a nu
+00012f80: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
+00012f90: 2020 2065 6c69 6620 6c65 6e28 7375 7266     elif len(surf
+00012fa0: 6163 652e 7368 6170 6529 2021 3d20 333a  ace.shape) != 3:
+00012fb0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00012fc0: 616c 7565 4572 726f 7228 2260 7375 7266  alueError("`surf
+00012fd0: 6163 6560 2068 6173 2074 6865 2069 6e63  ace` has the inc
+00012fe0: 6f72 7265 6374 2073 6861 7065 2e20 4974  orrect shape. It
+00012ff0: 206d 7573 7420 6265 2028 6e78 2c20 6e79   must be (nx, ny
+00013000: 2c20 6e7a 292e 2229 0a20 2020 2069 6620  , nz).").    if 
+00013010: 7479 7065 2861 746f 6d69 6329 206e 6f74  type(atomic) not
+00013020: 2069 6e20 5b6e 756d 7079 2e6e 6461 7272   in [numpy.ndarr
+00013030: 6179 2c20 6c69 7374 5d3a 0a20 2020 2020  ay, list]:.     
+00013040: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00013050: 6f72 2822 6061 746f 6d69 6360 206d 7573  or("`atomic` mus
+00013060: 7420 6265 2061 206c 6973 7420 6f72 2061  t be a list or a
+00013070: 206e 756d 7079 2e6e 6461 7272 6179 2e22   numpy.ndarray."
+00013080: 290a 2020 2020 656c 6966 206c 656e 286e  ).    elif len(n
+00013090: 756d 7079 2e61 7361 7272 6179 2861 746f  umpy.asarray(ato
+000130a0: 6d69 6329 2e73 6861 7065 2920 213d 2032  mic).shape) != 2
+000130b0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+000130c0: 5661 6c75 6545 7272 6f72 2822 6061 746f  ValueError("`ato
+000130d0: 6d69 6360 2068 6173 2069 6e63 6f72 7265  mic` has incorre
+000130e0: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
+000130f0: 7420 6265 2028 6e2c 2038 292e 2229 0a20  t be (n, 8)."). 
+00013100: 2020 2065 6c69 6620 6e75 6d70 792e 6173     elif numpy.as
+00013110: 6172 7261 7928 6174 6f6d 6963 292e 7368  array(atomic).sh
+00013120: 6170 655b 315d 2021 3d20 383a 0a20 2020  ape[1] != 8:.   
+00013130: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00013140: 4572 726f 7228 2260 6174 6f6d 6963 6020  Error("`atomic` 
+00013150: 6861 7320 696e 636f 7272 6563 7420 7368  has incorrect sh
+00013160: 6170 652e 2049 7420 6d75 7374 2062 6520  ape. It must be 
+00013170: 286e 2c20 3829 2e22 290a 2020 2020 6966  (n, 8).").    if
+00013180: 2074 7970 6528 7665 7274 6963 6573 2920   type(vertices) 
+00013190: 6e6f 7420 696e 205b 6e75 6d70 792e 6e64  not in [numpy.nd
+000131a0: 6172 7261 792c 206c 6973 745d 3a0a 2020  array, list]:.  
+000131b0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+000131c0: 4572 726f 7228 2260 7665 7274 6963 6573  Error("`vertices
+000131d0: 6020 6d75 7374 2062 6520 6120 6c69 7374  ` must be a list
+000131e0: 206f 7220 6120 6e75 6d70 792e 6e64 6172   or a numpy.ndar
+000131f0: 7261 792e 2229 0a20 2020 2065 6c69 6620  ray.").    elif 
+00013200: 6e75 6d70 792e 6173 6172 7261 7928 7665  numpy.asarray(ve
+00013210: 7274 6963 6573 292e 7368 6170 6520 213d  rtices).shape !=
+00013220: 2028 342c 2033 293a 0a20 2020 2020 2020   (4, 3):.       
+00013230: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00013240: 7228 2260 7665 7274 6963 6573 6020 6861  r("`vertices` ha
+00013250: 7320 696e 636f 7272 6563 7420 7368 6170  s incorrect shap
+00013260: 652e 2049 7420 6d75 7374 2062 6520 2834  e. It must be (4
+00013270: 2c20 3329 2e22 290a 2020 2020 6966 2074  , 3).").    if t
+00013280: 7970 6528 7374 6570 2920 6e6f 7420 696e  ype(step) not in
+00013290: 205b 666c 6f61 742c 2069 6e74 5d3a 0a20   [float, int]:. 
+000132a0: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+000132b0: 6545 7272 6f72 2822 6073 7465 7060 206d  eError("`step` m
+000132c0: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
+000132d0: 6520 7265 616c 206e 756d 6265 722e 2229  e real number.")
+000132e0: 0a20 2020 2065 6c69 6620 7374 6570 203c  .    elif step <
+000132f0: 3d20 302e 303a 0a20 2020 2020 2020 2072  = 0.0:.        r
+00013300: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00013310: 2260 7374 6570 6020 6d75 7374 2062 6520  "`step` must be 
+00013320: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
+00013330: 6e75 6d62 6572 2e22 290a 2020 2020 6966  number.").    if
+00013340: 2074 7970 6528 7072 6f62 655f 696e 2920   type(probe_in) 
+00013350: 6e6f 7420 696e 205b 666c 6f61 742c 2069  not in [float, i
+00013360: 6e74 5d3a 0a20 2020 2020 2020 2072 6169  nt]:.        rai
+00013370: 7365 2054 7970 6545 7272 6f72 2822 6070  se TypeError("`p
+00013380: 726f 6265 5f69 6e60 206d 7573 7420 6265  robe_in` must be
+00013390: 2061 206e 6f6e 2d6e 6567 6174 6976 6520   a non-negative 
+000133a0: 7265 616c 206e 756d 6265 722e 2229 0a20  real number."). 
+000133b0: 2020 2065 6c69 6620 7072 6f62 655f 696e     elif probe_in
+000133c0: 203c 2030 2e30 3a0a 2020 2020 2020 2020   < 0.0:.        
+000133d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000133e0: 2822 6070 726f 6265 5f69 6e60 206d 7573  ("`probe_in` mus
+000133f0: 7420 6265 2061 206e 6f6e 2d6e 6567 6174  t be a non-negat
+00013400: 6976 6520 7265 616c 206e 756d 6265 722e  ive real number.
+00013410: 2229 0a20 2020 2069 6620 7479 7065 2868  ").    if type(h
+00013420: 7964 726f 7068 6f62 6963 6974 795f 7363  ydrophobicity_sc
+00013430: 616c 6529 206e 6f74 2069 6e20 5b73 7472  ale) not in [str
+00013440: 2c20 7061 7468 6c69 622e 5061 7468 5d3a  , pathlib.Path]:
+00013450: 0a20 2020 2020 2020 2072 6169 7365 2054  .        raise T
+00013460: 7970 6545 7272 6f72 2822 6068 7964 726f  ypeError("`hydro
+00013470: 7068 6f62 6963 6974 795f 7363 616c 6560  phobicity_scale`
+00013480: 206d 7573 7420 6265 2061 2073 7472 696e   must be a strin
+00013490: 6720 6f72 2061 2070 6174 686c 6962 2e50  g or a pathlib.P
+000134a0: 6174 682e 2229 0a20 2020 2069 6620 7479  ath.").    if ty
+000134b0: 7065 2869 676e 6f72 655f 6261 636b 626f  pe(ignore_backbo
+000134c0: 6e65 2920 6e6f 7420 696e 205b 626f 6f6c  ne) not in [bool
+000134d0: 5d3a 0a20 2020 2020 2020 2072 6169 7365  ]:.        raise
+000134e0: 2054 7970 6545 7272 6f72 2822 6069 676e   TypeError("`ign
+000134f0: 6f72 655f 6261 636b 626f 6e65 6020 6d75  ore_backbone` mu
+00013500: 7374 2062 6520 6120 626f 6f6c 6561 6e2e  st be a boolean.
+00013510: 2229 0a20 2020 2069 6620 7365 6c65 6374  ").    if select
+00013520: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00013530: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+00013540: 2073 656c 6563 7469 6f6e 2074 7970 6573   selection types
+00013550: 0a20 2020 2020 2020 2069 6620 616c 6c28  .        if all(
+00013560: 6973 696e 7374 616e 6365 2878 2c20 696e  isinstance(x, in
+00013570: 7429 2066 6f72 2078 2069 6e20 7365 6c65  t) for x in sele
+00013580: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00013590: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+000135a0: 2065 6c69 6620 616c 6c28 6973 696e 7374   elif all(isinst
+000135b0: 616e 6365 2878 2c20 7374 7229 2066 6f72  ance(x, str) for
+000135c0: 2078 2069 6e20 7365 6c65 6374 696f 6e29   x in selection)
+000135d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000135e0: 6c65 6374 696f 6e20 3d20 5b5f 6765 745f  lection = [_get_
+000135f0: 6361 7669 7479 5f6c 6162 656c 2873 656c  cavity_label(sel
+00013600: 6529 2066 6f72 2073 656c 6520 696e 2073  e) for sele in s
+00013610: 656c 6563 7469 6f6e 5d0a 2020 2020 2020  election].      
+00013620: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013630: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+00013640: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00013650: 2020 2020 2022 6073 656c 6563 7469 6f6e       "`selection
+00013660: 6020 6d75 7374 2062 6520 6120 6c69 7374  ` must be a list
+00013670: 206f 6620 7374 7269 6e67 7320 2863 6176   of strings (cav
+00013680: 6974 7920 6e61 6d65 7329 206f 7220 696e  ity names) or in
+00013690: 7465 6765 7273 2028 6361 7669 7479 206c  tegers (cavity l
+000136a0: 6162 656c 7329 2e22 0a20 2020 2020 2020  abels).".       
+000136b0: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+000136c0: 2043 6865 636b 2069 6620 7365 6c65 6374   Check if select
+000136d0: 696f 6e20 696e 636c 7564 6573 2076 616c  ion includes val
+000136e0: 6964 2063 6176 6974 7920 6c61 6265 6c73  id cavity labels
+000136f0: 0a20 2020 2020 2020 2069 6620 616e 7928  .        if any(
+00013700: 7820 3c20 3220 666f 7220 7820 696e 2073  x < 2 for x in s
+00013710: 656c 6563 7469 6f6e 293a 0a20 2020 2020  election):.     
+00013720: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00013730: 7565 4572 726f 7228 6622 496e 7661 6c69  ueError(f"Invali
+00013740: 6420 6073 656c 6563 7469 6f6e 603a 207b  d `selection`: {
+00013750: 7365 6c65 6374 696f 6e7d 2e22 290a 2020  selection}.").  
+00013760: 2020 6966 206e 7468 7265 6164 7320 6973    if nthreads is
+00013770: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
+00013780: 7468 7265 6164 7320 3d20 6f73 2e63 7075  threads = os.cpu
+00013790: 5f63 6f75 6e74 2829 202d 2031 0a20 2020  _count() - 1.   
+000137a0: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+000137b0: 6620 7479 7065 286e 7468 7265 6164 7329  f type(nthreads)
+000137c0: 206e 6f74 2069 6e20 5b69 6e74 5d3a 0a20   not in [int]:. 
+000137d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000137e0: 2054 7970 6545 7272 6f72 2822 606e 7468   TypeError("`nth
+000137f0: 7265 6164 7360 206d 7573 7420 6265 2061  reads` must be a
+00013800: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
+00013810: 722e 2229 0a20 2020 2020 2020 2065 6c69  r.").        eli
+00013820: 6620 6e74 6872 6561 6473 203c 3d20 303a  f nthreads <= 0:
+00013830: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00013840: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
+00013850: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
+00013860: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
+00013870: 6567 6572 2e22 290a 2020 2020 6966 2074  eger.").    if t
+00013880: 7970 6528 7665 7262 6f73 6529 206e 6f74  ype(verbose) not
+00013890: 2069 6e20 5b62 6f6f 6c5d 3a0a 2020 2020   in [bool]:.    
+000138a0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+000138b0: 726f 7228 2260 7665 7262 6f73 6560 206d  ror("`verbose` m
+000138c0: 7573 7420 6265 2061 2062 6f6f 6c65 616e  ust be a boolean
+000138d0: 2e22 290a 0a20 2020 2023 2043 6f6e 7665  .")..    # Conve
+000138e0: 7274 2074 7970 6573 0a20 2020 2069 6620  rt types.    if 
+000138f0: 7479 7065 2861 746f 6d69 6329 203d 3d20  type(atomic) == 
+00013900: 6c69 7374 3a0a 2020 2020 2020 2020 6174  list:.        at
+00013910: 6f6d 6963 203d 206e 756d 7079 2e61 7361  omic = numpy.asa
+00013920: 7272 6179 2861 746f 6d69 6329 0a20 2020  rray(atomic).   
+00013930: 2069 6620 7479 7065 2876 6572 7469 6365   if type(vertice
+00013940: 7329 203d 3d20 6c69 7374 3a0a 2020 2020  s) == list:.    
+00013950: 2020 2020 7665 7274 6963 6573 203d 206e      vertices = n
+00013960: 756d 7079 2e61 7361 7272 6179 2876 6572  umpy.asarray(ver
+00013970: 7469 6365 7329 0a20 2020 2069 6620 7479  tices).    if ty
+00013980: 7065 2873 7465 7029 203d 3d20 696e 743a  pe(step) == int:
+00013990: 0a20 2020 2020 2020 2073 7465 7020 3d20  .        step = 
+000139a0: 666c 6f61 7428 7374 6570 290a 2020 2020  float(step).    
+000139b0: 6966 2074 7970 6528 7072 6f62 655f 696e  if type(probe_in
+000139c0: 2920 3d3d 2069 6e74 3a0a 2020 2020 2020  ) == int:.      
+000139d0: 2020 7072 6f62 655f 696e 203d 2066 6c6f    probe_in = flo
+000139e0: 6174 2870 726f 6265 5f69 6e29 0a0a 2020  at(probe_in)..  
+000139f0: 2020 2320 436f 6e76 6572 7420 6e75 6d70    # Convert nump
+00013a00: 792e 6e64 6172 7261 7920 6461 7461 2074  y.ndarray data t
+00013a10: 7970 6573 0a20 2020 2073 7572 6661 6365  ypes.    surface
+00013a20: 203d 2073 7572 6661 6365 2e61 7374 7970   = surface.astyp
+00013a30: 6528 2269 6e74 3332 2229 2069 6620 7375  e("int32") if su
+00013a40: 7266 6163 652e 6474 7970 6520 213d 2022  rface.dtype != "
+00013a50: 696e 7433 3222 2065 6c73 6520 7375 7266  int32" else surf
+00013a60: 6163 650a 2020 2020 7665 7274 6963 6573  ace.    vertices
+00013a70: 203d 2076 6572 7469 6365 732e 6173 7479   = vertices.asty
+00013a80: 7065 2822 666c 6f61 7436 3422 2920 6966  pe("float64") if
+00013a90: 2076 6572 7469 6365 732e 6474 7970 6520   vertices.dtype 
+00013aa0: 213d 2022 666c 6f61 7436 3422 2065 6c73  != "float64" els
+00013ab0: 6520 7665 7274 6963 6573 0a0a 2020 2020  e vertices..    
+00013ac0: 2320 4578 7472 6163 7420 6174 6f6d 696e  # Extract atomin
+00013ad0: 666f 2066 726f 6d20 6174 6f6d 6963 0a20  fo from atomic. 
+00013ae0: 2020 2061 746f 6d69 6e66 6f20 3d20 6e75     atominfo = nu
+00013af0: 6d70 792e 6173 6172 7261 7928 0a20 2020  mpy.asarray(.   
+00013b00: 2020 2020 2028 5b5b 6622 7b61 746f 6d5b       ([[f"{atom[
+00013b10: 305d 7d5f 7b61 746f 6d5b 315d 7d5f 7b61  0]}_{atom[1]}_{a
+00013b20: 746f 6d5b 325d 7d22 2c20 6174 6f6d 5b33  tom[2]}", atom[3
+00013b30: 5d5d 2066 6f72 2061 746f 6d20 696e 2061  ]] for atom in a
+00013b40: 746f 6d69 635b 3a2c 203a 345d 5d29 0a20  tomic[:, :4]]). 
+00013b50: 2020 2029 0a0a 2020 2020 2320 4578 7472     )..    # Extr
+00013b60: 6163 7420 7879 7a72 2066 726f 6d20 6174  act xyzr from at
+00013b70: 6f6d 6963 0a20 2020 2078 797a 7220 3d20  omic.    xyzr = 
+00013b80: 6174 6f6d 6963 5b3a 2c20 343a 5d2e 6173  atomic[:, 4:].as
+00013b90: 7479 7065 286e 756d 7079 2e66 6c6f 6174  type(numpy.float
+00013ba0: 3634 290a 0a20 2020 2023 2047 6574 206e  64)..    # Get n
+00013bb0: 756d 6265 7220 6f66 2063 6176 6974 6965  umber of cavitie
+00013bc0: 730a 2020 2020 6e63 6176 203d 2069 6e74  s.    ncav = int
+00013bd0: 2873 7572 6661 6365 2e6d 6178 2829 202d  (surface.max() -
+00013be0: 2031 290a 0a20 2020 2023 2047 6574 2073   1)..    # Get s
+00013bf0: 696e 636f 733a 2073 696e 6520 616e 6420  incos: sine and 
+00013c00: 636f 7373 696e 6520 6f66 2074 6865 2067  cossine of the g
+00013c10: 7269 6420 726f 7461 7469 6f6e 2061 6e67  rid rotation ang
+00013c20: 6c65 7320 2873 696e 612c 2063 6f73 612c  les (sina, cosa,
+00013c30: 2073 696e 622c 2063 6f73 6229 0a20 2020   sinb, cosb).   
+00013c40: 2073 696e 636f 7320 3d20 5f67 6574 5f73   sincos = _get_s
+00013c50: 696e 636f 7328 7665 7274 6963 6573 290a  incos(vertices).
+00013c60: 0a20 2020 2023 2053 656c 6563 7420 6361  .    # Select ca
+00013c70: 7669 7469 6573 0a20 2020 2069 6620 7365  vities.    if se
+00013c80: 6c65 6374 696f 6e20 6973 206e 6f74 204e  lection is not N
+00013c90: 6f6e 653a 0a20 2020 2020 2020 2073 7572  one:.        sur
+00013ca0: 6661 6365 203d 205f 7365 6c65 6374 5f63  face = _select_c
+00013cb0: 6176 6974 6965 7328 7375 7266 6163 652c  avities(surface,
+00013cc0: 2073 656c 6563 7469 6f6e 290a 0a20 2020   selection)..   
+00013cd0: 2023 2047 6574 2064 696d 656e 7369 6f6e   # Get dimension
+00013ce0: 730a 2020 2020 6e78 2c20 6e79 2c20 6e7a  s.    nx, ny, nz
+00013cf0: 203d 2073 7572 6661 6365 2e73 6861 7065   = surface.shape
+00013d00: 0a20 2020 206e 766f 7865 6c73 203d 206e  .    nvoxels = n
+00013d10: 7820 2a20 6e79 202a 206e 7a0a 0a20 2020  x * ny * nz..   
+00013d20: 2023 204c 6f61 6420 6879 6472 6f70 686f   # Load hydropho
+00013d30: 6269 6369 7479 2073 6361 6c65 730a 2020  bicity scales.  
+00013d40: 2020 6966 2068 7964 726f 7068 6f62 6963    if hydrophobic
+00013d50: 6974 795f 7363 616c 6520 696e 205b 0a20  ity_scale in [. 
+00013d60: 2020 2020 2020 2022 4569 7365 6e62 6572         "Eisenber
+00013d70: 6757 6569 7373 222c 0a20 2020 2020 2020  gWeiss",.       
+00013d80: 2022 4865 7373 6148 6569 6a6e 6522 2c0a   "HessaHeijne",.
+00013d90: 2020 2020 2020 2020 224b 7974 6544 6f6f          "KyteDoo
+00013da0: 6c69 7474 6c65 222c 0a20 2020 2020 2020  little",.       
+00013db0: 2022 4d6f 6f6e 466c 656d 696e 6722 2c0a   "MoonFleming",.
+00013dc0: 2020 2020 2020 2020 2252 6164 7a69 636b          "Radzick
+00013dd0: 6157 6f6c 6665 6e64 656e 222c 0a20 2020  aWolfenden",.   
+00013de0: 2020 2020 2022 5769 6d6c 6579 5768 6974       "WimleyWhit
+00013df0: 6522 2c0a 2020 2020 2020 2020 225a 6861  e",.        "Zha
+00013e00: 6f4c 6f6e 646f 6e22 2c0a 2020 2020 5d3a  oLondon",.    ]:
+00013e10: 0a20 2020 2020 2020 2068 7964 726f 7068  .        hydroph
+00013e20: 6f62 6963 6974 795f 7363 616c 6520 3d20  obicity_scale = 
+00013e30: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+00013e40: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
+00013e50: 682e 6162 7370 6174 6828 6f73 2e70 6174  h.abspath(os.pat
+00013e60: 682e 6469 726e 616d 6528 5f5f 6669 6c65  h.dirname(__file
+00013e70: 5f5f 2929 2c0a 2020 2020 2020 2020 2020  __)),.          
+00013e80: 2020 6622 6461 7461 2f7b 6879 6472 6f70    f"data/{hydrop
+00013e90: 686f 6269 6369 7479 5f73 6361 6c65 7d2e  hobicity_scale}.
+00013ea0: 746f 6d6c 222c 0a20 2020 2020 2020 2029  toml",.        )
+00013eb0: 0a20 2020 2066 203d 2074 6f6d 6c2e 6c6f  .    f = toml.lo
+00013ec0: 6164 2868 7964 726f 7068 6f62 6963 6974  ad(hydrophobicit
+00013ed0: 795f 7363 616c 6529 0a20 2020 2064 6174  y_scale).    dat
+00013ee0: 612c 206e 616d 6520 3d20 6c69 7374 2866  a, name = list(f
+00013ef0: 2e76 616c 7565 7328 2929 5b30 5d2c 206c  .values())[0], l
+00013f00: 6973 7428 662e 6b65 7973 2829 295b 305d  ist(f.keys())[0]
+00013f10: 0a20 2020 2072 6573 6e2c 2073 6361 6c65  .    resn, scale
+00013f20: 203d 206c 6973 7428 6461 7461 2e6b 6579   = list(data.key
+00013f30: 7328 2929 2c20 6e75 6d70 792e 6173 6172  s()), numpy.asar
+00013f40: 7261 7928 6c69 7374 2864 6174 612e 7661  ray(list(data.va
+00013f50: 6c75 6573 2829 2929 0a0a 2020 2020 2320  lues()))..    # 
+00013f60: 556e 7061 636b 2076 6572 7469 6365 730a  Unpack vertices.
+00013f70: 2020 2020 5031 2c20 5032 2c20 5033 2c20      P1, P2, P3, 
+00013f80: 5034 203d 2076 6572 7469 6365 730a 0a20  P4 = vertices.. 
+00013f90: 2020 2023 2052 656d 6f76 6520 6261 636b     # Remove back
+00013fa0: 626f 6e65 2066 726f 6d20 6174 6f6d 696e  bone from atomin
+00013fb0: 666f 0a20 2020 2069 6620 6967 6e6f 7265  fo.    if ignore
+00013fc0: 5f62 6163 6b62 6f6e 653a 0a20 2020 2020  _backbone:.     
+00013fd0: 2020 206d 6173 6b20 3d20 6e75 6d70 792e     mask = numpy.
+00013fe0: 7768 6572 6528 0a20 2020 2020 2020 2020  where(.         
+00013ff0: 2020 2028 6174 6f6d 696e 666f 5b3a 2c20     (atominfo[:, 
+00014000: 315d 2021 3d20 2243 2229 0a20 2020 2020  1] != "C").     
+00014010: 2020 2020 2020 2026 2028 6174 6f6d 696e         & (atomin
+00014020: 666f 5b3a 2c20 315d 2021 3d20 2243 4122  fo[:, 1] != "CA"
+00014030: 290a 2020 2020 2020 2020 2020 2020 2620  ).            & 
+00014040: 2861 746f 6d69 6e66 6f5b 3a2c 2031 5d20  (atominfo[:, 1] 
+00014050: 213d 2022 4e22 290a 2020 2020 2020 2020  != "N").        
+00014060: 2020 2020 2620 2861 746f 6d69 6e66 6f5b      & (atominfo[
+00014070: 3a2c 2031 5d20 213d 2022 4f22 290a 2020  :, 1] != "O").  
+00014080: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00014090: 6174 6f6d 696e 666f 203d 2061 746f 6d69  atominfo = atomi
+000140a0: 6e66 6f5b 6d61 736b 5b30 5d2c 5d0a 2020  nfo[mask[0],].  
+000140b0: 2020 2020 2020 7879 7a72 203d 2078 797a        xyzr = xyz
+000140c0: 725b 6d61 736b 5b30 5d2c 5d0a 0a20 2020  r[mask[0],]..   
+000140d0: 2023 2047 6574 2072 6573 6964 7565 206e   # Get residue n
+000140e0: 616d 6520 6672 6f6d 2061 746f 6d69 6e66  ame from atominf
+000140f0: 6f0a 2020 2020 7265 736e 616d 6520 3d20  o.    resname = 
+00014100: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00014110: 783a 2078 2e73 706c 6974 2822 5f22 295b  x: x.split("_")[
+00014120: 325d 2c20 6174 6f6d 696e 666f 5b3a 2c20  2], atominfo[:, 
+00014130: 305d 2929 0a0a 2020 2020 2320 4765 7420  0]))..    # Get 
+00014140: 6879 6472 6f70 686f 6269 6369 7479 2073  hydrophobicity s
+00014150: 6361 6c65 7320 696e 2033 4420 6772 6964  cales in 3D grid
+00014160: 2061 6e64 2061 7665 7261 6765 2068 7964   and average hyd
+00014170: 726f 7061 7468 790a 2020 2020 7363 616c  ropathy.    scal
+00014180: 6573 2c20 6176 675f 6879 6472 6f70 6174  es, avg_hydropat
+00014190: 6879 203d 205f 6879 6472 6f70 6174 6879  hy = _hydropathy
+000141a0: 280a 2020 2020 2020 2020 6e76 6f78 656c  (.        nvoxel
+000141b0: 732c 0a20 2020 2020 2020 206e 6361 762c  s,.        ncav,
+000141c0: 0a20 2020 2020 2020 2073 7572 6661 6365  .        surface
+000141d0: 2c0a 2020 2020 2020 2020 7879 7a72 2c0a  ,.        xyzr,.
+000141e0: 2020 2020 2020 2020 5031 2c0a 2020 2020          P1,.    
+000141f0: 2020 2020 7369 6e63 6f73 2c0a 2020 2020      sincos,.    
+00014200: 2020 2020 7265 736e 616d 652c 0a20 2020      resname,.   
+00014210: 2020 2020 2072 6573 6e2c 0a20 2020 2020       resn,.     
+00014220: 2020 2073 6361 6c65 2c0a 2020 2020 2020     scale,.      
+00014230: 2020 7374 6570 2c0a 2020 2020 2020 2020    step,.        
+00014240: 7072 6f62 655f 696e 2c0a 2020 2020 2020  probe_in,.      
+00014250: 2020 6e74 6872 6561 6473 2c0a 2020 2020    nthreads,.    
+00014260: 2020 2020 7665 7262 6f73 652c 0a20 2020      verbose,.   
+00014270: 2029 0a20 2020 2061 7667 5f68 7964 726f   ).    avg_hydro
+00014280: 7061 7468 7920 3d20 5f70 726f 6365 7373  pathy = _process
+00014290: 5f68 7964 726f 7061 7468 7928 6176 675f  _hydropathy(avg_
+000142a0: 6879 6472 6f70 6174 6879 2c20 6e63 6176  hydropathy, ncav
+000142b0: 2c20 7365 6c65 6374 696f 6e29 0a20 2020  , selection).   
+000142c0: 2061 7667 5f68 7964 726f 7061 7468 795b   avg_hydropathy[
+000142d0: 6622 7b6e 616d 657d 225d 203d 205b 666c  f"{name}"] = [fl
+000142e0: 6f61 7428 7363 616c 652e 6d69 6e28 2929  oat(scale.min())
+000142f0: 2c20 666c 6f61 7428 7363 616c 652e 6d61  , float(scale.ma
+00014300: 7828 2929 5d0a 0a20 2020 2072 6574 7572  x())]..    retur
+00014310: 6e20 7363 616c 6573 2e72 6573 6861 7065  n scales.reshape
+00014320: 286e 782c 206e 792c 206e 7a29 2c20 6176  (nx, ny, nz), av
+00014330: 675f 6879 6472 6f70 6174 6879 0a0a 0a64  g_hydropathy...d
+00014340: 6566 205f 6765 745f 6f70 656e 696e 675f  ef _get_opening_
+00014350: 6e61 6d65 2869 6e64 6578 3a20 696e 7429  name(index: int)
+00014360: 202d 3e20 7374 723a 0a20 2020 2022 2222   -> str:.    """
+00014370: 4765 7420 6f70 656e 696e 6720 6e61 6d65  Get opening name
+00014380: 2c20 6567 204f 4141 2c20 4f41 422c 2061  , eg OAA, OAB, a
+00014390: 6e64 2073 6f20 6f6e 2c20 6261 7365 6420  nd so on, based 
+000143a0: 6f6e 2074 6865 2069 6e64 6578 2e0a 0a20  on the index... 
+000143b0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000143c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000143d0: 2069 6e64 6578 203a 2069 6e74 0a20 2020   index : int.   
+000143e0: 2020 2020 2049 6e64 6578 2069 6e20 7468       Index in th
+000143f0: 6520 6469 6374 696f 6e61 7279 2e0a 0a20  e dictionary... 
+00014400: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00014410: 2d2d 2d2d 2d2d 0a20 2020 206f 7065 6e69  ------.    openi
+00014420: 6e67 5f6e 616d 6520 3a20 7374 720a 2020  ng_name : str.  
+00014430: 2020 2020 2020 4f70 656e 696e 6720 6e61        Opening na
+00014440: 6d65 0a20 2020 2022 2222 0a20 2020 206f  me.    """.    o
+00014450: 7065 6e69 6e67 5f6e 616d 6520 3d20 6622  pening_name = f"
+00014460: 4f7b 6368 7228 3635 202b 2069 6e74 2869  O{chr(65 + int(i
+00014470: 6e64 6578 202f 2032 3629 2025 2032 3629  ndex / 26) % 26)
+00014480: 7d7b 6368 7228 3635 202b 2028 696e 6465  }{chr(65 + (inde
+00014490: 7820 2520 3236 2929 7d22 0a20 2020 2072  x % 26))}".    r
+000144a0: 6574 7572 6e20 6f70 656e 696e 675f 6e61  eturn opening_na
+000144b0: 6d65 0a0a 0a64 6566 205f 6765 745f 6f70  me...def _get_op
+000144c0: 656e 696e 675f 6c61 6265 6c28 6f70 656e  ening_label(open
+000144d0: 696e 675f 6e61 6d65 3a20 7374 7229 202d  ing_name: str) -
+000144e0: 3e20 696e 743a 0a20 2020 2022 2222 4765  > int:.    """Ge
+000144f0: 7420 6f70 656e 696e 6720 6c61 6265 6c2c  t opening label,
+00014500: 2065 6720 322c 2033 2c20 616e 6420 736f   eg 2, 3, and so
+00014510: 206f 6e2c 2062 6173 6564 206f 6e20 7468   on, based on th
+00014520: 6520 6f70 656e 696e 6720 6e61 6d65 2e0a  e opening name..
+00014530: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00014540: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00014550: 2020 206f 7065 6e69 6e67 5f6e 616d 6520     opening_name 
+00014560: 3a20 7374 720a 2020 2020 2020 2020 4f70  : str.        Op
+00014570: 656e 696e 6720 6e61 6d65 0a0a 2020 2020  ening name..    
+00014580: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00014590: 2d2d 2d0a 2020 2020 636f 7065 6e69 6e67  ---.    copening
+000145a0: 5f6c 6162 656c 203a 2069 6e74 0a20 2020  _label : int.   
+000145b0: 2020 2020 2049 6e74 6567 6572 206c 6162       Integer lab
+000145c0: 656c 206f 6620 6561 6368 206f 7065 6e69  el of each openi
+000145d0: 6e67 2e0a 0a20 2020 2052 6169 7365 730a  ng...    Raises.
+000145e0: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2056      ------.    V
+000145f0: 616c 7565 4572 726f 720a 2020 2020 2020  alueError.      
+00014600: 2020 496e 7661 6c69 6420 6f70 656e 696e    Invalid openin
+00014610: 6720 6e61 6d65 3a20 606f 7065 6e69 6e67  g name: `opening
+00014620: 5f6e 616d 6560 2e0a 2020 2020 2222 220a  _name`..    """.
+00014630: 2020 2020 2320 4368 6563 6b20 6f70 656e      # Check open
+00014640: 696e 6720 6e61 6d65 0a20 2020 2069 6620  ing name.    if 
+00014650: 6f70 656e 696e 675f 6e61 6d65 5b30 5d20  opening_name[0] 
+00014660: 213d 2022 4f22 3a0a 2020 2020 2020 2020  != "O":.        
+00014670: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00014680: 2866 2249 6e76 616c 6964 206f 7065 6e69  (f"Invalid openi
+00014690: 6e67 206e 616d 653a 207b 6f70 656e 696e  ng name: {openin
+000146a0: 675f 6e61 6d65 7d2e 2229 0a0a 2020 2020  g_name}.")..    
+000146b0: 2320 4765 7420 6361 7669 7479 206c 6162  # Get cavity lab
+000146c0: 656c 0a20 2020 2063 6176 6974 795f 6c61  el.    cavity_la
+000146d0: 6265 6c20 3d20 286f 7264 286f 7065 6e69  bel = (ord(openi
+000146e0: 6e67 5f6e 616d 655b 315d 2920 2d20 3635  ng_name[1]) - 65
+000146f0: 2920 2a20 3236 202b 2028 6f72 6428 6f70  ) * 26 + (ord(op
+00014700: 656e 696e 675f 6e61 6d65 5b32 5d29 202d  ening_name[2]) -
+00014710: 2036 3529 202b 2032 0a0a 2020 2020 7265   65) + 2..    re
+00014720: 7475 726e 2063 6176 6974 795f 6c61 6265  turn cavity_labe
+00014730: 6c0a 0a0a 6465 6620 5f70 726f 6365 7373  l...def _process
+00014740: 5f6f 7065 6e69 6e67 7328 0a20 2020 2072  _openings(.    r
+00014750: 6177 5f6f 7065 6e69 6e67 733a 206e 756d  aw_openings: num
+00014760: 7079 2e6e 6461 7272 6179 2c0a 2020 2020  py.ndarray,.    
+00014770: 6f70 656e 696e 6732 6361 7669 7479 3a20  opening2cavity: 
+00014780: 6e75 6d70 792e 6e64 6172 7261 792c 0a29  numpy.ndarray,.)
+00014790: 202d 3e20 4469 6374 5b73 7472 2c20 4469   -> Dict[str, Di
+000147a0: 6374 5b73 7472 2c20 666c 6f61 745d 5d3a  ct[str, float]]:
+000147b0: 0a20 2020 2022 2222 5072 6f63 6573 7365  .    """Processe
+000147c0: 7320 6172 7261 7973 206f 6620 6f70 656e  s arrays of open
+000147d0: 696e 6773 2720 6172 6561 732e 0a0a 2020  ings' areas...  
+000147e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000147f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00014800: 7261 775f 6f70 656e 696e 6773 203a 206e  raw_openings : n
+00014810: 756d 7079 2e6e 6461 7272 6179 0a20 2020  umpy.ndarray.   
+00014820: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
+00014830: 7272 6179 206f 6620 6f70 656e 696e 6773  rray of openings
+00014840: 2720 6172 6561 732e 0a20 2020 206f 7065  ' areas..    ope
+00014850: 6e69 6e67 7332 6361 7669 7479 3a20 6e75  nings2cavity: nu
+00014860: 6d70 792e 6e64 6172 7261 790a 2020 2020  mpy.ndarray.    
+00014870: 2020 2020 4120 6e75 6d70 792e 6e64 6172      A numpy.ndar
+00014880: 7261 7920 6f66 206f 7065 6e69 6e67 7320  ray of openings 
+00014890: 6173 2069 6e64 6578 6573 2061 6e64 2063  as indexes and c
+000148a0: 6176 6974 6965 7320 6173 2076 616c 7565  avities as value
+000148b0: 732e 0a0a 2020 2020 5265 7475 726e 730a  s...    Returns.
+000148c0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000148d0: 6172 6561 203a 2044 6963 745b 7374 722c  area : Dict[str,
+000148e0: 2044 6963 745b 7374 722c 666c 6f61 745d   Dict[str,float]
+000148f0: 5d0a 2020 2020 2020 2020 4120 6469 6374  ].        A dict
+00014900: 696f 6e61 7279 2077 6974 6820 6172 6561  ionary with area
+00014910: 206f 6620 6561 6368 2064 6574 6563 7465   of each detecte
+00014920: 6420 6f70 656e 696e 672e 0a20 2020 2022  d opening..    "
+00014930: 2222 0a20 2020 2061 7265 6120 3d20 7b7d  "".    area = {}
+00014940: 0a0a 2020 2020 2320 4765 7420 6e75 6d62  ..    # Get numb
+00014950: 6572 206f 6620 6f70 656e 696e 6773 0a20  er of openings. 
+00014960: 2020 206e 6f70 656e 696e 6773 203d 2072     nopenings = r
+00014970: 6177 5f6f 7065 6e69 6e67 732e 7368 6170  aw_openings.shap
+00014980: 655b 305d 0a0a 2020 2020 666f 7220 696e  e[0]..    for in
+00014990: 6465 7820 696e 2072 616e 6765 286e 6f70  dex in range(nop
+000149a0: 656e 696e 6773 293a 0a20 2020 2020 2020  enings):.       
+000149b0: 2023 2047 6574 206f 7065 6e69 6e67 206e   # Get opening n
+000149c0: 616d 650a 2020 2020 2020 2020 6f70 656e  ame.        open
+000149d0: 696e 6720 3d20 5f67 6574 5f6f 7065 6e69  ing = _get_openi
+000149e0: 6e67 5f6e 616d 6528 696e 6465 7829 0a0a  ng_name(index)..
+000149f0: 2020 2020 2020 2020 2320 4765 7420 6361          # Get ca
+00014a00: 7669 7479 206e 616d 650a 2020 2020 2020  vity name.      
+00014a10: 2020 6361 7669 7479 203d 205f 6765 745f    cavity = _get_
+00014a20: 6361 7669 7479 5f6e 616d 6528 6f70 656e  cavity_name(open
+00014a30: 696e 6732 6361 7669 7479 5b69 6e64 6578  ing2cavity[index
+00014a40: 5d29 0a0a 2020 2020 2020 2020 2320 5361  ])..        # Sa
+00014a50: 7665 206f 7065 6e69 6e67 2061 7265 610a  ve opening area.
+00014a60: 2020 2020 2020 2020 6966 2063 6176 6974          if cavit
+00014a70: 7920 6e6f 7420 696e 2061 7265 612e 6b65  y not in area.ke
+00014a80: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00014a90: 2020 6172 6561 5b63 6176 6974 795d 203d    area[cavity] =
+00014aa0: 207b 7d0a 2020 2020 2020 2020 6172 6561   {}.        area
+00014ab0: 5b63 6176 6974 795d 5b6f 7065 6e69 6e67  [cavity][opening
+00014ac0: 5d20 3d20 666c 6f61 7428 726f 756e 6428  ] = float(round(
+00014ad0: 7261 775f 6f70 656e 696e 6773 5b69 6e64  raw_openings[ind
+00014ae0: 6578 5d2c 2032 2929 0a0a 2020 2020 2320  ex], 2))..    # 
+00014af0: 536f 7274 206b 6579 730a 2020 2020 6172  Sort keys.    ar
+00014b00: 6561 203d 2064 6963 7428 736f 7274 6564  ea = dict(sorted
+00014b10: 2861 7265 612e 6974 656d 7328 2929 290a  (area.items())).
+00014b20: 0a20 2020 2072 6574 7572 6e20 6172 6561  .    return area
+00014b30: 0a0a 0a64 6566 206f 7065 6e69 6e67 7328  ...def openings(
+00014b40: 0a20 2020 2063 6176 6974 6965 733a 206e  .    cavities: n
+00014b50: 756d 7079 2e6e 6461 7272 6179 2c0a 2020  umpy.ndarray,.  
+00014b60: 2020 6465 7074 6873 3a20 4f70 7469 6f6e    depths: Option
+00014b70: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
+00014b80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7374  ] = None,.    st
+00014b90: 6570 3a20 556e 696f 6e5b 666c 6f61 742c  ep: Union[float,
+00014ba0: 2069 6e74 5d20 3d20 302e 362c 0a20 2020   int] = 0.6,.   
+00014bb0: 206f 7065 6e69 6e67 735f 6375 746f 6666   openings_cutoff
+00014bc0: 3a20 696e 7420 3d20 312c 0a20 2020 2073  : int = 1,.    s
+00014bd0: 656c 6563 7469 6f6e 3a20 4f70 7469 6f6e  election: Option
+00014be0: 616c 5b55 6e69 6f6e 5b4c 6973 745b 696e  al[Union[List[in
+00014bf0: 745d 2c20 4c69 7374 5b73 7472 5d5d 5d20  t], List[str]]] 
+00014c00: 3d20 4e6f 6e65 2c0a 2020 2020 6e74 6872  = None,.    nthr
+00014c10: 6561 6473 3a20 4f70 7469 6f6e 616c 5b69  eads: Optional[i
+00014c20: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00014c30: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+00014c40: 4661 6c73 652c 0a29 202d 3e20 5475 706c  False,.) -> Tupl
+00014c50: 655b 696e 742c 206e 756d 7079 2e6e 6461  e[int, numpy.nda
+00014c60: 7272 6179 2c20 4469 6374 5b73 7472 2c20  rray, Dict[str, 
+00014c70: 4469 6374 5b73 7472 2c20 666c 6f61 745d  Dict[str, float]
+00014c80: 5d5d 3a0a 2020 2020 2222 225b 5749 505d  ]]:.    """[WIP]
+00014c90: 2049 6465 6e74 6966 7920 6f70 656e 696e   Identify openin
+00014ca0: 6773 206f 6620 7468 6520 6465 7465 6374  gs of the detect
+00014cb0: 6564 2063 6176 6974 6965 7320 616e 6420  ed cavities and 
+00014cc0: 6361 6c63 756c 6174 6520 7468 6569 7220  calculate their 
+00014cd0: 6172 6561 732e 0a0a 2020 2020 5061 7261  areas...    Para
+00014ce0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00014cf0: 2d2d 2d2d 2d0a 2020 2020 6361 7669 7469  -----.    caviti
+00014d00: 6573 203a 206e 756d 7079 2e6e 6461 7272  es : numpy.ndarr
+00014d10: 6179 0a20 2020 2020 2020 2043 6176 6974  ay.        Cavit
+00014d20: 7920 706f 696e 7473 2069 6e20 7468 6520  y points in the 
+00014d30: 3344 2067 7269 6420 2863 6176 6974 6965  3D grid (cavitie
+00014d40: 735b 6e78 5d5b 6e79 5d5b 6e7a 5d29 2e0a  s[nx][ny][nz])..
+00014d50: 2020 2020 2020 2020 4361 7669 7469 6573          Cavities
+00014d60: 2061 7272 6179 2068 6173 2069 6e74 6567   array has integ
+00014d70: 6572 206c 6162 656c 7320 696e 2065 6163  er labels in eac
+00014d80: 6820 706f 7369 7469 6f6e 2c20 7468 6174  h position, that
+00014d90: 2061 7265 3a0a 0a20 2020 2020 2020 2020   are:..         
+00014da0: 2020 202a 202d 313a 2062 756c 6b20 706f     * -1: bulk po
+00014db0: 696e 7473 3b0a 0a20 2020 2020 2020 2020  ints;..         
+00014dc0: 2020 202a 2030 3a20 6269 6f6d 6f6c 6563     * 0: biomolec
+00014dd0: 756c 6520 706f 696e 7473 3b0a 0a20 2020  ule points;..   
+00014de0: 2020 2020 2020 2020 202a 2031 3a20 656d           * 1: em
+00014df0: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
+00014e00: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
+00014e10: 203e 3d32 3a20 6361 7669 7479 2070 6f69   >=2: cavity poi
+00014e20: 6e74 732e 0a20 2020 2064 6570 7468 7320  nts..    depths 
+00014e30: 3a20 4f70 7469 6f6e 616c 5b6e 756d 7079  : Optional[numpy
+00014e40: 2e6e 6461 7272 6179 5d2c 206f 7074 696f  .ndarray], optio
+00014e50: 6e61 6c0a 2020 2020 2020 2020 4120 6e75  nal.        A nu
+00014e60: 6d70 792e 6e64 6172 7261 7920 7769 7468  mpy.ndarray with
+00014e70: 2064 6570 7468 206f 6620 6361 7669 7479   depth of cavity
+00014e80: 2070 6f69 6e74 7320 2864 6570 7468 5b6e   points (depth[n
+00014e90: 785d 5b6e 795d 5b6e 7a5d 292c 2062 7920  x][ny][nz]), by 
+00014ea0: 6465 6661 756c 7420 4e6f 6e65 2e20 4966  default None. If
+00014eb0: 204e 6f6e 652c 2064 6570 7468 7320 6973   None, depths is
+00014ec0: 2063 616c 6375 6c61 7465 6420 6672 6f6d   calculated from
+00014ed0: 2063 6176 6974 6965 732e 0a20 2020 2073   cavities..    s
+00014ee0: 7465 7020 3a20 556e 696f 6e5b 666c 6f61  tep : Union[floa
+00014ef0: 742c 2069 6e74 5d2c 206f 7074 696f 6e61  t, int], optiona
+00014f00: 6c0a 2020 2020 2020 2020 4772 6964 2073  l.        Grid s
+00014f10: 7061 6369 6e67 2028 4129 2c20 6279 2064  pacing (A), by d
+00014f20: 6566 6175 6c74 2030 2e36 2e0a 2020 2020  efault 0.6..    
+00014f30: 6f70 656e 696e 6773 5f63 7574 6f66 6620  openings_cutoff 
+00014f40: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+00014f50: 2020 2020 2020 2020 5468 6520 6d69 6e69          The mini
+00014f60: 6d75 6d20 6e75 6d62 6572 206f 6620 766f  mum number of vo
+00014f70: 7865 6c73 2061 6e20 6f70 656e 696e 6720  xels an opening 
+00014f80: 6d75 7374 2068 6176 652c 2062 7920 6465  must have, by de
+00014f90: 6661 756c 7420 312e 0a20 2020 2073 656c  fault 1..    sel
+00014fa0: 6563 7469 6f6e 203a 2055 6e69 6f6e 5b4c  ection : Union[L
+00014fb0: 6973 745b 696e 745d 2c20 4c69 7374 5b73  ist[int], List[s
+00014fc0: 7472 5d5d 2c20 6f70 7469 6f6e 616c 0a20  tr]], optional. 
+00014fd0: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
+00014fe0: 2069 6e74 6567 6572 206c 6162 656c 7320   integer labels 
+00014ff0: 6f72 2061 206c 6973 7420 6f66 2063 6176  or a list of cav
+00015000: 6974 7920 6e61 6d65 7320 746f 2062 6520  ity names to be 
+00015010: 7365 6c65 6374 6564 2c20 6279 2064 6566  selected, by def
+00015020: 6175 6c74 204e 6f6e 652e 0a20 2020 206e  ault None..    n
+00015030: 7468 7265 6164 7320 3a20 696e 742c 206f  threads : int, o
+00015040: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00015050: 4e75 6d62 6572 206f 6620 7468 7265 6164  Number of thread
+00015060: 732c 2062 7920 6465 6661 756c 7420 4e6f  s, by default No
+00015070: 6e65 2e20 4966 204e 6f6e 652c 2074 6865  ne. If None, the
+00015080: 206e 756d 6265 7220 6f66 2074 6872 6561   number of threa
+00015090: 6473 2069 730a 2020 2020 2020 2020 606f  ds is.        `o
+000150a0: 732e 6370 755f 636f 756e 7428 2920 2d20  s.cpu_count() - 
+000150b0: 3160 2e0a 2020 2020 7665 7262 6f73 6520  1`..    verbose 
+000150c0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+000150d0: 0a20 2020 2020 2020 2050 7269 6e74 2065  .        Print e
+000150e0: 7874 7261 2069 6e66 6f72 6d61 7469 6f6e  xtra information
+000150f0: 2074 6f20 7374 616e 6461 7264 206f 7574   to standard out
+00015100: 7075 742c 2062 7920 6465 6661 756c 7420  put, by default 
+00015110: 4661 6c73 652e 0a0a 2020 2020 5265 7475  False...    Retu
+00015120: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00015130: 2020 2020 6e6f 7065 6e69 6e67 7320 3a20      nopenings : 
+00015140: 696e 740a 2020 2020 2020 2020 546f 7461  int.        Tota
+00015150: 6c20 6e75 6d62 6572 206f 6620 6f70 656e  l number of open
+00015160: 696e 6773 2e0a 2020 2020 6f70 656e 696e  ings..    openin
+00015170: 6773 203a 206e 756d 7079 2e6e 6461 7272  gs : numpy.ndarr
+00015180: 6179 0a20 2020 2020 2020 204f 7065 6e69  ay.        Openi
+00015190: 6e67 7320 706f 696e 7473 2069 6e20 7468  ngs points in th
+000151a0: 6520 3344 2067 7269 6420 286f 7065 6e69  e 3D grid (openi
+000151b0: 6e67 735b 6e78 5d5b 6e79 5d5b 6e7a 5d29  ngs[nx][ny][nz])
+000151c0: 2e0a 2020 2020 2020 2020 4f70 656e 696e  ..        Openin
+000151d0: 6773 2061 7272 6179 2068 6173 2069 6e74  gs array has int
+000151e0: 6567 6572 206c 6162 656c 7320 696e 2065  eger labels in e
+000151f0: 6163 6820 706f 7369 7469 6f6e 2c20 7468  ach position, th
+00015200: 6174 2061 7265 3a0a 0a20 2020 2020 2020  at are:..       
+00015210: 2020 2020 202a 202d 313a 2062 756c 6b20       * -1: bulk 
+00015220: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
+00015230: 2020 2020 202a 2030 3a20 6361 7669 7479       * 0: cavity
+00015240: 206f 7220 6269 6f6d 6f6c 6563 756c 6520   or biomolecule 
+00015250: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
+00015260: 2020 2020 202a 2031 3a20 656d 7074 7920       * 1: empty 
+00015270: 7370 6163 6520 706f 696e 7473 3b0a 0a20  space points;.. 
+00015280: 2020 2020 2020 2020 2020 202a 203e 3d32             * >=2
+00015290: 3a20 4f70 656e 696e 6720 706f 696e 7473  : Opening points
+000152a0: 2e0a 0a20 2020 2020 2020 2054 6865 2065  ...        The e
+000152b0: 6d70 7479 2073 7061 6365 2070 6f69 6e74  mpty space point
+000152c0: 7320 6172 6520 7265 6769 6f6e 7320 7468  s are regions th
+000152d0: 6174 2064 6f20 6e6f 7420 6d65 6574 2074  at do not meet t
+000152e0: 6865 2063 686f 7365 6e0a 2020 2020 2020  he chosen.      
+000152f0: 2020 6f70 656e 696e 6773 2063 7574 6f66    openings cutof
+00015300: 6620 746f 2062 6520 636f 6e73 6964 6572  f to be consider
+00015310: 6564 2061 6e20 6f70 656e 696e 672e 0a20  ed an opening.. 
+00015320: 2020 2061 6f70 656e 696e 6773 203a 2044     aopenings : D
+00015330: 6963 745b 7374 722c 2044 6963 745b 7374  ict[str, Dict[st
+00015340: 722c 666c 6f61 745d 5d0a 2020 2020 2020  r,float]].      
+00015350: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
+00015360: 6974 6820 6172 6561 206f 6620 6561 6368  ith area of each
+00015370: 2064 6574 6563 7465 6420 6f70 656e 696e   detected openin
+00015380: 672e 0a0a 2020 2020 5261 6973 6573 0a20  g...    Raises. 
+00015390: 2020 202d 2d2d 2d2d 2d0a 2020 2020 5479     ------.    Ty
+000153a0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+000153b0: 6063 6176 6974 6965 7360 206d 7573 7420  `cavities` must 
+000153c0: 6265 2061 206e 756d 7079 2e6e 6461 7272  be a numpy.ndarr
+000153d0: 6179 2e0a 2020 2020 5661 6c75 6545 7272  ay..    ValueErr
+000153e0: 6f72 0a20 2020 2020 2020 2060 6361 7669  or.        `cavi
+000153f0: 7469 6573 6020 6861 7320 7468 6520 696e  ties` has the in
+00015400: 636f 7272 6563 7420 7368 6170 652e 2049  correct shape. I
+00015410: 7420 6d75 7374 2062 6520 286e 782c 206e  t must be (nx, n
+00015420: 792c 206e 7a29 2e0a 2020 2020 5479 7065  y, nz)..    Type
+00015430: 4572 726f 720a 2020 2020 2020 2020 6064  Error.        `d
+00015440: 6570 7468 7360 206d 7573 7420 6265 2061  epths` must be a
+00015450: 206e 756d 7079 2e6e 6461 7272 6179 2e0a   numpy.ndarray..
+00015460: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
+00015470: 2020 2020 2020 2060 6465 7074 6873 6020         `depths` 
+00015480: 6861 7320 7468 6520 696e 636f 7272 6563  has the incorrec
+00015490: 7420 7368 6170 652e 2049 7420 6d75 7374  t shape. It must
+000154a0: 2062 6520 286e 782c 206e 792c 206e 7a29   be (nx, ny, nz)
+000154b0: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
+000154c0: 2020 2020 2020 2020 6073 7465 7060 206d          `step` m
+000154d0: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
+000154e0: 6520 7265 616c 206e 756d 6265 722e 0a20  e real number.. 
+000154f0: 2020 2056 616c 7565 4572 726f 720a 2020     ValueError.  
+00015500: 2020 2020 2020 6073 7465 7060 206d 7573        `step` mus
+00015510: 7420 6265 2061 2070 6f73 6974 6976 6520  t be a positive 
+00015520: 7265 616c 206e 756d 6265 722e 0a20 2020  real number..   
+00015530: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
+00015540: 2020 2060 6f70 656e 696e 6773 5f63 7574     `openings_cut
+00015550: 6f66 6660 206d 7573 7420 6265 2061 6e20  off` must be an 
+00015560: 696e 7465 6765 722e 0a20 2020 2056 616c  integer..    Val
+00015570: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
+00015580: 606f 7065 6e69 6e67 735f 6375 746f 6666  `openings_cutoff
+00015590: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+000155a0: 7469 7665 2069 6e74 6567 6572 2e0a 2020  tive integer..  
+000155b0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
+000155c0: 2020 2020 6073 656c 6563 7469 6f6e 6020      `selection` 
+000155d0: 6d75 7374 2062 6520 6120 6c69 7374 206f  must be a list o
+000155e0: 6620 7374 7269 6e67 7320 2863 6176 6974  f strings (cavit
+000155f0: 7920 6e61 6d65 7329 206f 7220 696e 7465  y names) or inte
+00015600: 6765 7273 2028 6361 7669 7479 206c 6162  gers (cavity lab
+00015610: 656c 7329 2e0a 2020 2020 5661 6c75 6545  els)..    ValueE
+00015620: 7272 6f72 0a20 2020 2020 2020 2049 6e76  rror.        Inv
+00015630: 616c 6964 2060 7365 6c65 6374 696f 6e60  alid `selection`
+00015640: 3a20 6073 656c 6563 7469 6f6e 602e 0a20  : `selection`.. 
+00015650: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
+00015660: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
+00015670: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+00015680: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
+00015690: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
+000156a0: 2020 2060 6e74 6872 6561 6473 6020 6d75     `nthreads` mu
+000156b0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+000156c0: 2069 6e74 6567 6572 2e0a 2020 2020 5479   integer..    Ty
+000156d0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+000156e0: 6076 6572 626f 7365 6020 6d75 7374 2062  `verbose` must b
+000156f0: 6520 6120 626f 6f6c 6561 6e0a 0a20 2020  e a boolean..   
+00015700: 2045 7861 6d70 6c65 0a20 2020 202d 2d2d   Example.    ---
+00015710: 2d2d 2d2d 0a20 2020 2057 6974 6820 7468  ----.    With th
+00015720: 6520 6361 7669 7479 2070 6f69 6e74 7320  e cavity points 
+00015730: 6964 656e 7469 6669 6564 2077 6974 6820  identified with 
+00015740: 6060 6465 7465 6374 6060 2c20 7765 2063  ``detect``, we c
+00015750: 616e 2063 6861 7261 6374 6572 697a 6520  an characterize 
+00015760: 7468 6569 7220 6f70 656e 696e 6773 2c20  their openings, 
+00015770: 7468 6174 2069 6e63 6c75 6465 7320 6e75  that includes nu
+00015780: 6d62 6572 2061 6e64 2061 7265 6120 6f66  mber and area of
+00015790: 206f 7065 6e69 6e67 7320 616e 6420 6465   openings and de
+000157a0: 6669 6e69 6e67 206f 7065 6e69 6e67 2070  fining opening p
+000157b0: 6f69 6e74 733a 0a0a 2020 2020 3e3e 3e20  oints:..    >>> 
+000157c0: 6672 6f6d 2070 794b 5646 696e 6465 7220  from pyKVFinder 
+000157d0: 696d 706f 7274 206f 7065 6e69 6e67 730a  import openings.
+000157e0: 2020 2020 3e3e 3e20 6e6f 7065 6e69 6e67      >>> nopening
+000157f0: 732c 206f 7065 6e69 6e67 732c 2061 6f70  s, openings, aop
+00015800: 656e 696e 6773 203d 206f 7065 6e69 6e67  enings = opening
+00015810: 7328 6361 7669 7469 6573 290a 2020 2020  s(cavities).    
+00015820: 3e3e 3e20 6e6f 7065 6e69 6e67 730a 2020  >>> nopenings.  
+00015830: 2020 3136 0a20 2020 203e 3e3e 206f 7065    16.    >>> ope
+00015840: 6e69 6e67 730a 2020 2020 6172 7261 7928  nings.    array(
+00015850: 5b5b 5b2d 312c 202d 312c 202d 312c 202e  [[[-1, -1, -1, .
+00015860: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+00015870: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+00015880: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+00015890: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+000158a0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+000158b0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+000158c0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+000158d0: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+000158e0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+000158f0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00015900: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00015910: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+00015920: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+00015930: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+00015940: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00015950: 2d31 2c20 2d31 5d5d 2c0a 2020 2020 2020  -1, -1]],.      
+00015960: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
+00015970: 2020 205b 5b2d 312c 202d 312c 202d 312c     [[-1, -1, -1,
+00015980: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00015990: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+000159a0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+000159b0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+000159c0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+000159d0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+000159e0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+000159f0: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
+00015a00: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+00015a10: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00015a20: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+00015a30: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+00015a40: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+00015a50: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00015a60: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00015a70: 2c20 2d31 2c20 2d31 5d5d 5d29 0a20 2020  , -1, -1]]]).   
+00015a80: 203e 3e3e 2061 6f70 656e 696e 6773 0a20   >>> aopenings. 
+00015a90: 2020 207b 274b 4141 273a 207b 274f 4141     {'KAA': {'OAA
+00015aa0: 273a 2034 372e 3431 2c20 274f 4147 273a  ': 47.41, 'OAG':
+00015ab0: 2033 2e36 7d2c 2027 4b41 4227 3a20 7b27   3.6}, 'KAB': {'
+00015ac0: 4f41 4227 3a20 3235 2e38 347d 2c20 274b  OAB': 25.84}, 'K
+00015ad0: 4143 273a 207b 274f 4143 273a 2035 332e  AC': {'OAC': 53.
+00015ae0: 3632 7d2c 2027 4b41 4427 3a20 7b27 4f41  62}, 'KAD': {'OA
+00015af0: 4427 3a20 3132 2e35 397d 2c20 274b 4145  D': 12.59}, 'KAE
+00015b00: 273a 207b 274f 4145 273a 2032 362e 337d  ': {'OAE': 26.3}
+00015b10: 2c20 274b 4146 273a 207b 274f 4146 273a  , 'KAF': {'OAF':
+00015b20: 2031 382e 3436 7d2c 2027 4b41 4727 3a20   18.46}, 'KAG': 
+00015b30: 7b27 4f41 4827 3a20 3132 2e38 337d 2c20  {'OAH': 12.83}, 
+00015b40: 274b 4148 273a 207b 274f 414b 273a 2035  'KAH': {'OAK': 5
+00015b50: 392e 3936 7d2c 2027 4b41 4a27 3a20 7b27  9.96}, 'KAJ': {'
+00015b60: 4f41 4927 3a20 3136 2e31 317d 2c20 274b  OAI': 16.11}, 'K
+00015b70: 414c 273a 207b 274f 414a 273a 2031 372e  AL': {'OAJ': 17.
+00015b80: 337d 2c20 274b 414d 273a 207b 274f 414c  3}, 'KAM': {'OAL
+00015b90: 273a 2033 352e 3237 7d2c 2027 4b41 4f27  ': 35.27}, 'KAO'
+00015ba0: 3a20 7b27 4f41 4d27 3a20 382e 3439 7d2c  : {'OAM': 8.49},
+00015bb0: 2027 4b41 5027 3a20 7b27 4f41 4e27 3a20   'KAP': {'OAN': 
+00015bc0: 3133 2e37 317d 2c20 274b 4151 273a 207b  13.71}, 'KAQ': {
+00015bd0: 274f 414f 273a 2031 332e 3136 7d2c 2027  'OAO': 13.16}, '
+00015be0: 4b41 5227 3a20 7b27 4f41 5027 3a20 3135  KAR': {'OAP': 15
+00015bf0: 2e33 367d 7d0a 0a20 2020 2057 6974 6820  .36}}..    With 
+00015c00: 7468 6520 6361 7669 7479 2061 6e64 206f  the cavity and o
+00015c10: 7065 6e69 6e67 2070 6f69 6e74 7320 6964  pening points id
+00015c20: 656e 7469 6669 6564 2c20 7765 2063 616e  entified, we can
+00015c30: 3a0a 0a20 2020 202a 2045 7870 6f72 7420  :..    * Export 
+00015c40: 6361 7669 7479 2070 6f69 6e74 7320 7769  cavity points wi
+00015c50: 7468 206f 7065 6e69 6e67 2070 6f69 6e74  th opening point
+00015c60: 7320 6d61 7070 6564 206f 6e20 7468 656d  s mapped on them
+00015c70: 3a0a 0a20 2020 203e 3e3e 2066 726f 6d20  :..    >>> from 
+00015c80: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
+00015c90: 7420 6578 706f 7274 0a20 2020 203e 3e3e  t export.    >>>
+00015ca0: 2065 7870 6f72 7428 2263 6176 6974 6965   export("cavitie
+00015cb0: 735f 7769 7468 5f6f 7065 6e69 6e67 732e  s_with_openings.
+00015cc0: 7064 6222 2c20 6361 7669 7469 6573 2c20  pdb", cavities, 
+00015cd0: 4e6f 6e65 2c20 7665 7274 6963 6573 2c20  None, vertices, 
+00015ce0: 423d 6f70 656e 696e 6773 290a 0a20 2020  B=openings)..   
+00015cf0: 202a 2045 7870 6f72 7420 6f70 656e 696e   * Export openin
+00015d00: 6720 706f 696e 7473 2077 6974 6820 7361  g points with sa
+00015d10: 6d65 206e 6f6d 656e 636c 6174 7572 6520  me nomenclature 
+00015d20: 6672 6f6d 2060 6061 6f70 656e 696e 6773  from ``aopenings
+00015d30: 6060 3a0a 0a20 2020 203e 3e3e 2066 726f  ``:..    >>> fro
+00015d40: 6d20 7079 4b56 4669 6e64 6572 2069 6d70  m pyKVFinder imp
+00015d50: 6f72 7420 6578 706f 7274 5f6f 7065 6e69  ort export_openi
+00015d60: 6e67 730a 2020 2020 3e3e 3e20 6578 706f  ngs.    >>> expo
+00015d70: 7274 5f6f 7065 6e69 6e67 7328 226f 7065  rt_openings("ope
+00015d80: 6e69 6e67 732e 7064 6222 2c20 6f70 656e  nings.pdb", open
+00015d90: 696e 6773 2c20 7665 7274 6963 6573 290a  ings, vertices).
+00015da0: 0a20 2020 2053 6565 2041 6c73 6f0a 2020  .    See Also.  
+00015db0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064    --------.    d
+00015dc0: 6574 6563 740a 2020 2020 6465 7074 680a  etect.    depth.
+00015dd0: 2020 2020 6578 706f 7274 0a20 2020 2065      export.    e
+00015de0: 7870 6f72 745f 6f70 656e 696e 6773 0a20  xport_openings. 
+00015df0: 2020 2022 2222 0a20 2020 2066 726f 6d20     """.    from 
+00015e00: 5f70 794b 5646 696e 6465 7220 696d 706f  _pyKVFinder impo
+00015e10: 7274 205f 6172 6561 2c20 5f6f 7065 6e69  rt _area, _openi
+00015e20: 6e67 732c 205f 6f70 656e 696e 6773 3263  ngs, _openings2c
+00015e30: 6176 6974 6965 730a 0a20 2020 2023 2043  avities..    # C
+00015e40: 6865 636b 2061 7267 756d 656e 7473 0a20  heck arguments. 
+00015e50: 2020 2069 6620 7479 7065 2863 6176 6974     if type(cavit
+00015e60: 6965 7329 206e 6f74 2069 6e20 5b6e 756d  ies) not in [num
+00015e70: 7079 2e6e 6461 7272 6179 5d3a 0a20 2020  py.ndarray]:.   
+00015e80: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00015e90: 7272 6f72 2822 6063 6176 6974 6965 7360  rror("`cavities`
+00015ea0: 206d 7573 7420 6265 2061 206e 756d 7079   must be a numpy
+00015eb0: 2e6e 6461 7272 6179 2e22 290a 2020 2020  .ndarray.").    
+00015ec0: 656c 6966 206c 656e 2863 6176 6974 6965  elif len(cavitie
+00015ed0: 732e 7368 6170 6529 2021 3d20 333a 0a20  s.shape) != 3:. 
+00015ee0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00015ef0: 7565 4572 726f 7228 2260 6361 7669 7469  ueError("`caviti
+00015f00: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
+00015f10: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+00015f20: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+00015f30: 206e 7a29 2e22 290a 2020 2020 6966 2064   nz).").    if d
+00015f40: 6570 7468 7320 6973 204e 6f6e 653a 0a20  epths is None:. 
+00015f50: 2020 2020 2020 2064 6570 7468 732c 205f         depths, _
+00015f60: 2c20 5f20 3d20 6465 7074 6828 6361 7669  , _ = depth(cavi
+00015f70: 7469 6573 2c20 7374 6570 2c20 7365 6c65  ties, step, sele
+00015f80: 6374 696f 6e2c 206e 7468 7265 6164 732c  ction, nthreads,
+00015f90: 2076 6572 626f 7365 290a 2020 2020 656c   verbose).    el
+00015fa0: 6966 2074 7970 6528 6465 7074 6873 2920  if type(depths) 
+00015fb0: 6e6f 7420 696e 205b 6e75 6d70 792e 6e64  not in [numpy.nd
+00015fc0: 6172 7261 795d 3a0a 2020 2020 2020 2020  array]:.        
+00015fd0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00015fe0: 2260 6465 7074 6873 6020 6d75 7374 2062  "`depths` must b
+00015ff0: 6520 6120 6e75 6d70 792e 6e64 6172 7261  e a numpy.ndarra
+00016000: 792e 2229 0a20 2020 2065 6c69 6620 6c65  y.").    elif le
+00016010: 6e28 6465 7074 6873 2e73 6861 7065 2920  n(depths.shape) 
+00016020: 213d 2033 3a0a 2020 2020 2020 2020 7261  != 3:.        ra
+00016030: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00016040: 6064 6570 7468 7360 2068 6173 2074 6865  `depths` has the
+00016050: 2069 6e63 6f72 7265 6374 2073 6861 7065   incorrect shape
+00016060: 2e20 4974 206d 7573 7420 6265 2028 6e78  . It must be (nx
+00016070: 2c20 6e79 2c20 6e7a 292e 2229 0a20 2020  , ny, nz).").   
+00016080: 2069 6620 7479 7065 2873 7465 7029 206e   if type(step) n
+00016090: 6f74 2069 6e20 5b66 6c6f 6174 2c20 696e  ot in [float, in
+000160a0: 745d 3a0a 2020 2020 2020 2020 7261 6973  t]:.        rais
+000160b0: 6520 5479 7065 4572 726f 7228 2260 7374  e TypeError("`st
+000160c0: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+000160d0: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+000160e0: 6572 2e22 290a 2020 2020 656c 6966 2073  er.").    elif s
+000160f0: 7465 7020 3c3d 2030 2e30 3a0a 2020 2020  tep <= 0.0:.    
+00016100: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00016110: 7272 6f72 2822 6073 7465 7060 206d 7573  rror("`step` mus
+00016120: 7420 6265 2061 2070 6f73 6974 6976 6520  t be a positive 
+00016130: 7265 616c 206e 756d 6265 722e 2229 0a20  real number."). 
+00016140: 2020 2069 6620 7479 7065 286f 7065 6e69     if type(openi
+00016150: 6e67 735f 6375 746f 6666 2920 6e6f 7420  ngs_cutoff) not 
+00016160: 696e 205b 696e 745d 3a0a 2020 2020 2020  in [int]:.      
+00016170: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+00016180: 7228 2260 6f70 656e 696e 6773 5f63 7574  r("`openings_cut
+00016190: 6f66 6660 206d 7573 7420 6265 2061 6e20  off` must be an 
+000161a0: 696e 7465 6765 722e 2229 0a20 2020 2065  integer.").    e
+000161b0: 6c69 6620 6f70 656e 696e 6773 5f63 7574  lif openings_cut
+000161c0: 6f66 6620 3c20 303a 0a20 2020 2020 2020  off < 0:.       
+000161d0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000161e0: 7228 2260 6f70 656e 696e 6773 5f63 7574  r("`openings_cut
+000161f0: 6f66 6660 206d 7573 7420 6265 2061 2070  off` must be a p
+00016200: 6f73 6974 6976 6520 696e 7465 6765 722e  ositive integer.
+00016210: 2229 0a20 2020 2069 6620 7365 6c65 6374  ").    if select
+00016220: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00016230: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+00016240: 2073 656c 6563 7469 6f6e 2074 7970 6573   selection types
+00016250: 0a20 2020 2020 2020 2069 6620 616c 6c28  .        if all(
+00016260: 6973 696e 7374 616e 6365 2878 2c20 696e  isinstance(x, in
+00016270: 7429 2066 6f72 2078 2069 6e20 7365 6c65  t) for x in sele
+00016280: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+00016290: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+000162a0: 2065 6c69 6620 616c 6c28 6973 696e 7374   elif all(isinst
+000162b0: 616e 6365 2878 2c20 7374 7229 2066 6f72  ance(x, str) for
+000162c0: 2078 2069 6e20 7365 6c65 6374 696f 6e29   x in selection)
+000162d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000162e0: 6c65 6374 696f 6e20 3d20 5b5f 6765 745f  lection = [_get_
+000162f0: 6361 7669 7479 5f6c 6162 656c 2873 656c  cavity_label(sel
+00016300: 6529 2066 6f72 2073 656c 6520 696e 2073  e) for sele in s
+00016310: 656c 6563 7469 6f6e 5d0a 2020 2020 2020  election].      
+00016320: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00016330: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+00016340: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00016350: 2020 2020 2022 6073 656c 6563 7469 6f6e       "`selection
+00016360: 6020 6d75 7374 2062 6520 6120 6c69 7374  ` must be a list
+00016370: 206f 6620 7374 7269 6e67 7320 2863 6176   of strings (cav
+00016380: 6974 7920 6e61 6d65 7329 206f 7220 696e  ity names) or in
+00016390: 7465 6765 7273 2028 6361 7669 7479 206c  tegers (cavity l
+000163a0: 6162 656c 7329 2e22 0a20 2020 2020 2020  abels).".       
+000163b0: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+000163c0: 2043 6865 636b 2069 6620 7365 6c65 6374   Check if select
+000163d0: 696f 6e20 696e 636c 7564 6573 2076 616c  ion includes val
+000163e0: 6964 2063 6176 6974 7920 6c61 6265 6c73  id cavity labels
+000163f0: 0a20 2020 2020 2020 2069 6620 616e 7928  .        if any(
+00016400: 7820 3c20 3220 666f 7220 7820 696e 2073  x < 2 for x in s
+00016410: 656c 6563 7469 6f6e 293a 0a20 2020 2020  election):.     
+00016420: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00016430: 7565 4572 726f 7228 6622 496e 7661 6c69  ueError(f"Invali
+00016440: 6420 6073 656c 6563 7469 6f6e 603a 207b  d `selection`: {
+00016450: 7365 6c65 6374 696f 6e7d 2e22 290a 2020  selection}.").  
+00016460: 2020 6966 206e 7468 7265 6164 7320 6973    if nthreads is
+00016470: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
+00016480: 7468 7265 6164 7320 3d20 6f73 2e63 7075  threads = os.cpu
+00016490: 5f63 6f75 6e74 2829 202d 2031 0a20 2020  _count() - 1.   
+000164a0: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+000164b0: 6620 7479 7065 286e 7468 7265 6164 7329  f type(nthreads)
+000164c0: 206e 6f74 2069 6e20 5b69 6e74 5d3a 0a20   not in [int]:. 
+000164d0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000164e0: 2054 7970 6545 7272 6f72 2822 606e 7468   TypeError("`nth
+000164f0: 7265 6164 7360 206d 7573 7420 6265 2061  reads` must be a
+00016500: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
+00016510: 722e 2229 0a20 2020 2020 2020 2065 6c69  r.").        eli
+00016520: 6620 6e74 6872 6561 6473 203c 3d20 303a  f nthreads <= 0:
+00016530: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00016540: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
+00016550: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
+00016560: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
+00016570: 6567 6572 2e22 290a 2020 2020 6966 2074  eger.").    if t
+00016580: 7970 6528 7665 7262 6f73 6529 206e 6f74  ype(verbose) not
+00016590: 2069 6e20 5b62 6f6f 6c5d 3a0a 2020 2020   in [bool]:.    
+000165a0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+000165b0: 726f 7228 2260 7665 7262 6f73 6560 206d  ror("`verbose` m
+000165c0: 7573 7420 6265 2061 2062 6f6f 6c65 616e  ust be a boolean
+000165d0: 2e22 290a 0a20 2020 2023 2043 6f6e 7665  .")..    # Conve
+000165e0: 7274 2074 7970 6573 0a20 2020 2069 6620  rt types.    if 
+000165f0: 7479 7065 2873 7465 7029 203d 3d20 696e  type(step) == in
+00016600: 743a 0a20 2020 2020 2020 2073 7465 7020  t:.        step 
+00016610: 3d20 666c 6f61 7428 7374 6570 290a 0a20  = float(step).. 
+00016620: 2020 2023 2053 656c 6563 7420 6361 7669     # Select cavi
+00016630: 7469 6573 0a20 2020 2069 6620 7365 6c65  ties.    if sele
+00016640: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
+00016650: 653a 0a20 2020 2020 2020 2063 6176 6974  e:.        cavit
+00016660: 6965 7320 3d20 5f73 656c 6563 745f 6361  ies = _select_ca
+00016670: 7669 7469 6573 2863 6176 6974 6965 732c  vities(cavities,
+00016680: 2073 656c 6563 7469 6f6e 290a 0a20 2020   selection)..   
+00016690: 2023 2047 6574 206e 756d 6265 7220 6f66   # Get number of
+000166a0: 2063 6176 6974 6965 730a 2020 2020 6e63   cavities.    nc
+000166b0: 6176 203d 2069 6e74 2863 6176 6974 6965  av = int(cavitie
+000166c0: 732e 6d61 7828 2920 2d20 3129 0a0a 2020  s.max() - 1)..  
+000166d0: 2020 2320 4765 7420 6361 7669 7469 6573    # Get cavities
+000166e0: 2073 6861 7065 0a20 2020 206e 782c 206e   shape.    nx, n
+000166f0: 792c 206e 7a20 3d20 6361 7669 7469 6573  y, nz = cavities
+00016700: 2e73 6861 7065 0a0a 2020 2020 2320 4669  .shape..    # Fi
+00016710: 6e64 206f 7065 6e69 6e67 730a 2020 2020  nd openings.    
+00016720: 6e6f 7065 6e69 6e67 732c 206f 7065 6e69  nopenings, openi
+00016730: 6e67 7320 3d20 5f6f 7065 6e69 6e67 7328  ngs = _openings(
+00016740: 0a20 2020 2020 2020 206e 7820 2a20 6e79  .        nx * ny
+00016750: 202a 206e 7a2c 2063 6176 6974 6965 732c   * nz, cavities,
+00016760: 2064 6570 7468 732c 206e 6361 762c 206f   depths, ncav, o
+00016770: 7065 6e69 6e67 735f 6375 746f 6666 2c20  penings_cutoff, 
+00016780: 7374 6570 2c20 6e74 6872 6561 6473 2c20  step, nthreads, 
+00016790: 7665 7262 6f73 650a 2020 2020 290a 0a20  verbose.    ).. 
+000167a0: 2020 2023 2052 6573 6861 7065 206f 7065     # Reshape ope
+000167b0: 6e69 6e67 730a 2020 2020 6f70 656e 696e  nings.    openin
+000167c0: 6773 203d 206f 7065 6e69 6e67 732e 7265  gs = openings.re
+000167d0: 7368 6170 6528 6e78 2c20 6e79 2c20 6e7a  shape(nx, ny, nz
+000167e0: 290a 0a20 2020 2023 2043 616c 6375 6c61  )..    # Calcula
+000167f0: 7465 206f 7065 6e69 6e67 7320 6172 6561  te openings area
+00016800: 730a 2020 2020 6966 2076 6572 626f 7365  s.    if verbose
+00016810: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00016820: 223e 2045 7374 696d 6174 696e 6720 6f70  "> Estimating op
+00016830: 656e 696e 6773 2061 7265 6122 290a 2020  enings area").  
+00016840: 2020 616f 7065 6e69 6e67 7320 3d20 5f61    aopenings = _a
+00016850: 7265 6128 6f70 656e 696e 6773 2c20 7374  rea(openings, st
+00016860: 6570 2c20 6e6f 7065 6e69 6e67 732c 206e  ep, nopenings, n
+00016870: 7468 7265 6164 7329 0a0a 2020 2020 2320  threads)..    # 
+00016880: 4669 6e64 2077 6869 6368 206f 7065 6e69  Find which openi
+00016890: 6e67 7320 6265 6c6f 6e67 7320 746f 2065  ngs belongs to e
+000168a0: 6163 6820 6361 7669 7479 0a20 2020 206f  ach cavity.    o
+000168b0: 7065 6e69 6e67 3263 6176 6974 7920 3d20  pening2cavity = 
+000168c0: 5f6f 7065 6e69 6e67 7332 6361 7669 7469  _openings2caviti
+000168d0: 6573 286e 6f70 656e 696e 6773 2c20 6361  es(nopenings, ca
+000168e0: 7669 7469 6573 2c20 6f70 656e 696e 6773  vities, openings
+000168f0: 2c20 6e74 6872 6561 6473 290a 0a20 2020  , nthreads)..   
+00016900: 2023 2050 726f 6365 7373 206f 7065 6e69   # Process openi
+00016910: 6e67 730a 2020 2020 616f 7065 6e69 6e67  ngs.    aopening
+00016920: 7320 3d20 5f70 726f 6365 7373 5f6f 7065  s = _process_ope
+00016930: 6e69 6e67 7328 616f 7065 6e69 6e67 732c  nings(aopenings,
+00016940: 206f 7065 6e69 6e67 3263 6176 6974 7929   opening2cavity)
+00016950: 0a0a 2020 2020 7265 7475 726e 206e 6f70  ..    return nop
+00016960: 656e 696e 6773 2c20 6f70 656e 696e 6773  enings, openings
+00016970: 2c20 616f 7065 6e69 6e67 730a 0a0a 6465  , aopenings...de
+00016980: 6620 6578 706f 7274 280a 2020 2020 666e  f export(.    fn
+00016990: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+000169a0: 686c 6962 2e50 6174 685d 2c0a 2020 2020  hlib.Path],.    
+000169b0: 6361 7669 7469 6573 3a20 4f70 7469 6f6e  cavities: Option
+000169c0: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
+000169d0: 5d2c 0a20 2020 2073 7572 6661 6365 3a20  ],.    surface: 
+000169e0: 4f70 7469 6f6e 616c 5b6e 756d 7079 2e6e  Optional[numpy.n
+000169f0: 6461 7272 6179 5d2c 0a20 2020 2076 6572  darray],.    ver
+00016a00: 7469 6365 733a 2055 6e69 6f6e 5b6e 756d  tices: Union[num
+00016a10: 7079 2e6e 6461 7272 6179 2c20 4c69 7374  py.ndarray, List
+00016a20: 5b4c 6973 745b 666c 6f61 745d 5d5d 2c0a  [List[float]]],.
+00016a30: 2020 2020 7374 6570 3a20 556e 696f 6e5b      step: Union[
+00016a40: 666c 6f61 742c 2069 6e74 5d20 3d20 302e  float, int] = 0.
+00016a50: 362c 0a20 2020 2042 3a20 4f70 7469 6f6e  6,.    B: Option
+00016a60: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
+00016a70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6f75  ] = None,.    ou
+00016a80: 7470 7574 5f68 7964 726f 7061 7468 793a  tput_hydropathy:
+00016a90: 2055 6e69 6f6e 5b73 7472 2c20 7061 7468   Union[str, path
+00016aa0: 6c69 622e 5061 7468 5d20 3d20 2268 7964  lib.Path] = "hyd
+00016ab0: 726f 7061 7468 792e 7064 6222 2c0a 2020  ropathy.pdb",.  
+00016ac0: 2020 7363 616c 6573 3a20 4f70 7469 6f6e    scales: Option
+00016ad0: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
+00016ae0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7365  ] = None,.    se
+00016af0: 6c65 6374 696f 6e3a 204f 7074 696f 6e61  lection: Optiona
+00016b00: 6c5b 556e 696f 6e5b 4c69 7374 5b69 6e74  l[Union[List[int
+00016b10: 5d2c 204c 6973 745b 7374 725d 5d5d 203d  ], List[str]]] =
+00016b20: 204e 6f6e 652c 0a20 2020 206e 7468 7265   None,.    nthre
+00016b30: 6164 733a 204f 7074 696f 6e61 6c5b 696e  ads: Optional[in
+00016b40: 745d 203d 204e 6f6e 652c 0a20 2020 2061  t] = None,.    a
+00016b50: 7070 656e 643a 2062 6f6f 6c20 3d20 4661  ppend: bool = Fa
+00016b60: 6c73 652c 0a20 2020 206d 6f64 656c 3a20  lse,.    model: 
+00016b70: 696e 7420 3d20 302c 0a29 202d 3e20 4e6f  int = 0,.) -> No
+00016b80: 6e65 3a0a 2020 2020 2222 2245 7870 6f72  ne:.    """Expor
+00016b90: 7420 6361 7669 7469 7920 2848 2920 616e  t cavitiy (H) an
+00016ba0: 6420 7375 7266 6163 6520 2848 4129 2070  d surface (HA) p
+00016bb0: 6f69 6e74 7320 746f 2050 4442 2d66 6f72  oints to PDB-for
+00016bc0: 6d61 7474 6564 2066 696c 6520 7769 7468  matted file with
+00016bd0: 0a20 2020 2061 2076 6172 6961 626c 6520  .    a variable 
+00016be0: 2842 3b20 6f70 7469 6f6e 616c 2920 696e  (B; optional) in
+00016bf0: 2042 2d66 6163 746f 7220 636f 6c75 6d6e   B-factor column
+00016c00: 2c20 616e 6420 6879 6472 6f70 6174 6879  , and hydropathy
+00016c10: 2074 6f0a 2020 2020 5044 422d 666f 726d   to.    PDB-form
+00016c20: 6174 7465 6420 6669 6c65 2069 6e20 422d  atted file in B-
+00016c30: 6661 6374 6f72 2063 6f6c 756d 6e20 6174  factor column at
+00016c40: 2073 7572 6661 6365 2070 6f69 6e74 7320   surface points 
+00016c50: 2848 4129 2e0a 0a20 2020 2050 6172 616d  (HA)...    Param
+00016c60: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00016c70: 2d2d 2d2d 0a20 2020 2066 6e20 3a20 556e  ----.    fn : Un
+00016c80: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
+00016c90: 2e50 6174 685d 0a20 2020 2020 2020 2041  .Path].        A
+00016ca0: 2070 6174 6820 746f 2050 4442 2066 696c   path to PDB fil
+00016cb0: 6520 666f 7220 7772 6974 696e 6720 6361  e for writing ca
+00016cc0: 7669 7469 6573 2e0a 2020 2020 6361 7669  vities..    cavi
+00016cd0: 7469 6573 203a 206e 756d 7079 2e6e 6461  ties : numpy.nda
+00016ce0: 7272 6179 2c20 6f70 7469 6f6e 616c 0a20  rray, optional. 
+00016cf0: 2020 2020 2020 2043 6176 6974 7920 706f         Cavity po
+00016d00: 696e 7473 2069 6e20 7468 6520 3344 2067  ints in the 3D g
+00016d10: 7269 6420 2863 6176 6974 6965 735b 6e78  rid (cavities[nx
+00016d20: 5d5b 6e79 5d5b 6e7a 5d29 2e0a 2020 2020  ][ny][nz])..    
+00016d30: 2020 2020 4361 7669 7469 6573 2061 7272      Cavities arr
+00016d40: 6179 2068 6173 2069 6e74 6567 6572 206c  ay has integer l
+00016d50: 6162 656c 7320 696e 2065 6163 6820 706f  abels in each po
+00016d60: 7369 7469 6f6e 2c20 7468 6174 2061 7265  sition, that are
+00016d70: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+00016d80: 202d 313a 2062 756c 6b20 706f 696e 7473   -1: bulk points
+00016d90: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
+00016da0: 2030 3a20 6269 6f6d 6f6c 6563 756c 6520   0: biomolecule 
+00016db0: 706f 696e 7473 3b0a 0a20 2020 2020 2020  points;..       
+00016dc0: 2020 2020 202a 2031 3a20 656d 7074 7920       * 1: empty 
+00016dd0: 7370 6163 6520 706f 696e 7473 3b0a 0a20  space points;.. 
+00016de0: 2020 2020 2020 2020 2020 202a 203e 3d32             * >=2
+00016df0: 3a20 6361 7669 7479 2070 6f69 6e74 732e  : cavity points.
+00016e00: 0a0a 2020 2020 2020 2020 5468 6520 656d  ..        The em
+00016e10: 7074 7920 7370 6163 6520 706f 696e 7473  pty space points
+00016e20: 2061 7265 2072 6567 696f 6e73 2074 6861   are regions tha
+00016e30: 7420 646f 206e 6f74 206d 6565 7420 7468  t do not meet th
+00016e40: 6520 6368 6f73 656e 0a20 2020 2020 2020  e chosen.       
+00016e50: 2076 6f6c 756d 6520 6375 746f 6666 2074   volume cutoff t
+00016e60: 6f20 6265 2063 6f6e 7369 6465 7265 6420  o be considered 
+00016e70: 6120 6361 7669 7479 2e0a 2020 2020 7375  a cavity..    su
+00016e80: 7266 6163 6520 3a20 6e75 6d70 792e 6e64  rface : numpy.nd
+00016e90: 6172 7261 792c 206f 7074 696f 6e61 6c0a  array, optional.
+00016ea0: 2020 2020 2020 2020 5375 7266 6163 6520          Surface 
+00016eb0: 706f 696e 7473 2069 6e20 7468 6520 3344  points in the 3D
+00016ec0: 2067 7269 6420 2873 7572 6661 6365 5b6e   grid (surface[n
+00016ed0: 785d 5b6e 795d 5b6e 7a5d 292e 2049 6620  x][ny][nz]). If 
+00016ee0: 4e6f 6e65 2c20 7375 7266 6163 650a 2020  None, surface.  
+00016ef0: 2020 2020 2020 6973 2061 206e 756d 7079        is a numpy
+00016f00: 2e7a 6572 6f73 2061 7272 6179 2077 6974  .zeros array wit
+00016f10: 6820 7361 6d65 2073 6861 7065 206f 6620  h same shape of 
+00016f20: 6361 7669 7469 6573 2e0a 2020 2020 2020  cavities..      
+00016f30: 2020 5375 7266 6163 6520 6172 7261 7920    Surface array 
+00016f40: 6861 7320 696e 7465 6765 7220 6c61 6265  has integer labe
+00016f50: 6c73 2069 6e20 6561 6368 2070 6f73 6974  ls in each posit
+00016f60: 696f 6e2c 2074 6861 7420 6172 653a 0a0a  ion, that are:..
+00016f70: 2020 2020 2020 2020 2020 2020 2a20 2d31              * -1
+00016f80: 3a20 6275 6c6b 2070 6f69 6e74 733b 0a0a  : bulk points;..
+00016f90: 2020 2020 2020 2020 2020 2020 2a20 303a              * 0:
+00016fa0: 2062 696f 6d6f 6c65 6375 6c65 206f 7220   biomolecule or 
+00016fb0: 656d 7074 7920 7370 6163 6520 706f 696e  empty space poin
+00016fc0: 7473 3b0a 0a20 2020 2020 2020 2020 2020  ts;..           
+00016fd0: 202a 203e 3d32 3a20 7375 7266 6163 6520   * >=2: surface 
+00016fe0: 706f 696e 7473 2e0a 0a20 2020 2020 2020  points...       
+00016ff0: 2054 6865 2065 6d70 7479 2073 7061 6365   The empty space
+00017000: 2070 6f69 6e74 7320 6172 6520 7265 6769   points are regi
+00017010: 6f6e 7320 7468 6174 2064 6f20 6e6f 7420  ons that do not 
+00017020: 6d65 6574 2074 6865 2063 686f 7365 6e0a  meet the chosen.
+00017030: 2020 2020 2020 2020 766f 6c75 6d65 2063          volume c
+00017040: 7574 6f66 6620 746f 2062 6520 636f 6e73  utoff to be cons
+00017050: 6964 6572 6564 2061 2063 6176 6974 792e  idered a cavity.
+00017060: 0a20 2020 2076 6572 7469 6365 7320 3a20  .    vertices : 
+00017070: 556e 696f 6e5b 6e75 6d70 792e 6e64 6172  Union[numpy.ndar
+00017080: 7261 792c 204c 6973 745b 4c69 7374 5b66  ray, List[List[f
+00017090: 6c6f 6174 5d5d 5d0a 2020 2020 2020 2020  loat]]].        
+000170a0: 4120 6e75 6d70 792e 6e64 6172 7261 7920  A numpy.ndarray 
+000170b0: 6f72 2061 206c 6973 7420 7769 7468 2078  or a list with x
+000170c0: 797a 2076 6572 7469 6365 7320 636f 6f72  yz vertices coor
+000170d0: 6469 6e61 7465 7320 286f 7269 6769 6e2c  dinates (origin,
+000170e0: 0a20 2020 2020 2020 2058 2d61 7869 732c  .        X-axis,
+000170f0: 2059 2d61 7869 732c 205a 2d61 7869 7329   Y-axis, Z-axis)
+00017100: 2e0a 2020 2020 7374 6570 203a 2055 6e69  ..    step : Uni
+00017110: 6f6e 5b66 6c6f 6174 2c20 696e 745d 2c20  on[float, int], 
+00017120: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00017130: 2047 7269 6420 7370 6163 696e 6720 2841   Grid spacing (A
+00017140: 292c 2062 7920 6465 6661 756c 7420 302e  ), by default 0.
+00017150: 362e 0a20 2020 2042 203a 206e 756d 7079  6..    B : numpy
+00017160: 2e6e 6461 7272 6179 2c20 6f70 7469 6f6e  .ndarray, option
+00017170: 616c 0a20 2020 2020 2020 2041 206e 756d  al.        A num
+00017180: 7079 2e6e 6461 7272 6179 2077 6974 6820  py.ndarray with 
+00017190: 7661 6c75 6573 2074 6f20 6265 206d 6170  values to be map
+000171a0: 7065 6420 6f6e 2042 2d66 6163 746f 7220  ped on B-factor 
+000171b0: 636f 6c75 6d6e 2069 6e20 6361 7669 7479  column in cavity
+000171c0: 0a20 2020 2020 2020 2070 6f69 6e74 7320  .        points 
+000171d0: 2842 5b6e 785d 5b6e 795d 5b6e 7a5d 292c  (B[nx][ny][nz]),
+000171e0: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
+000171f0: 2e0a 2020 2020 6f75 7470 7574 5f68 7964  ..    output_hyd
+00017200: 726f 7061 7468 7920 3a20 556e 696f 6e5b  ropathy : Union[
+00017210: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
+00017220: 685d 2c20 6f70 7469 6f6e 616c 0a20 2020  h], optional.   
+00017230: 2020 2020 2041 2070 6174 6820 746f 2068       A path to h
+00017240: 7964 726f 7061 7468 7920 5044 4220 6669  ydropathy PDB fi
+00017250: 6c65 2028 7375 7266 6163 6520 706f 696e  le (surface poin
+00017260: 7473 206d 6170 7065 6420 7769 7468 2061  ts mapped with a
+00017270: 0a20 2020 2020 2020 2068 7964 726f 7068  .        hydroph
+00017280: 6f62 6963 6974 7920 7363 616c 6529 2c20  obicity scale), 
+00017290: 6279 2064 6566 6175 6c74 2060 6879 6472  by default `hydr
+000172a0: 6f70 6174 6879 2e70 6462 602e 0a20 2020  opathy.pdb`..   
+000172b0: 2073 6361 6c65 7320 3a20 6e75 6d70 792e   scales : numpy.
+000172c0: 6e64 6172 7261 792c 206f 7074 696f 6e61  ndarray, optiona
+000172d0: 6c0a 2020 2020 2020 2020 4120 6e75 6d70  l.        A nump
+000172e0: 792e 6e64 6172 7261 7920 7769 7468 2068  y.ndarray with h
+000172f0: 7964 726f 7068 6f62 6963 6974 7920 7363  ydrophobicity sc
+00017300: 616c 6520 7661 6c75 6573 2074 6f20 6265  ale values to be
+00017310: 206d 6170 7065 6420 6f6e 0a20 2020 2020   mapped on.     
+00017320: 2020 2042 2d66 6163 746f 7220 636f 6c75     B-factor colu
+00017330: 6d6e 2069 6e20 7375 7266 6163 6520 706f  mn in surface po
+00017340: 696e 7473 2028 7363 616c 6573 5b6e 785d  ints (scales[nx]
+00017350: 5b6e 795d 5b6e 7a5d 292c 2062 7920 6465  [ny][nz]), by de
+00017360: 6661 756c 740a 2020 2020 2020 2020 4e6f  fault.        No
+00017370: 6e65 2e0a 2020 2020 7365 6c65 6374 696f  ne..    selectio
+00017380: 6e20 3a20 556e 696f 6e5b 4c69 7374 5b69  n : Union[List[i
+00017390: 6e74 5d2c 204c 6973 745b 7374 725d 5d2c  nt], List[str]],
+000173a0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+000173b0: 2020 4120 6c69 7374 206f 6620 696e 7465    A list of inte
+000173c0: 6765 7220 6c61 6265 6c73 206f 7220 6120  ger labels or a 
+000173d0: 6c69 7374 206f 6620 6361 7669 7479 206e  list of cavity n
+000173e0: 616d 6573 2074 6f20 6265 2073 656c 6563  ames to be selec
+000173f0: 7465 642c 2062 7920 6465 6661 756c 7420  ted, by default 
+00017400: 4e6f 6e65 2e0a 2020 2020 6e74 6872 6561  None..    nthrea
+00017410: 6473 203a 2069 6e74 2c20 6f70 7469 6f6e  ds : int, option
+00017420: 616c 0a20 2020 2020 2020 204e 756d 6265  al.        Numbe
+00017430: 7220 6f66 2074 6872 6561 6473 2c20 6279  r of threads, by
+00017440: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
+00017450: 6620 4e6f 6e65 2c20 7468 6520 6e75 6d62  f None, the numb
+00017460: 6572 206f 6620 7468 7265 6164 7320 6973  er of threads is
+00017470: 0a20 2020 2020 2020 2060 6f73 2e63 7075  .        `os.cpu
+00017480: 5f63 6f75 6e74 2829 202d 2031 602e 0a20  _count() - 1`.. 
+00017490: 2020 2061 7070 656e 6420 3a20 626f 6f6c     append : bool
+000174a0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000174b0: 2020 2057 6865 7468 6572 2074 6f20 6170     Whether to ap
+000174c0: 7065 6e64 2063 6176 6974 6965 7320 746f  pend cavities to
+000174d0: 2074 6865 2050 4442 2066 696c 652c 2062   the PDB file, b
+000174e0: 7920 6465 6661 756c 7420 4661 6c73 652e  y default False.
+000174f0: 0a20 2020 206d 6f64 656c 203a 2069 6e74  .    model : int
+00017500: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00017510: 2020 204d 6f64 656c 206e 756d 6265 722c     Model number,
+00017520: 2062 7920 6465 6661 756c 7420 302e 0a0a   by default 0...
+00017530: 2020 2020 5261 6973 6573 0a20 2020 202d      Raises.    -
+00017540: 2d2d 2d2d 2d0a 2020 2020 5479 7065 4572  -----.    TypeEr
+00017550: 726f 720a 2020 2020 2020 2020 6066 6e60  ror.        `fn`
+00017560: 206d 7573 7420 6265 2061 2073 7472 696e   must be a strin
+00017570: 6720 6f72 2070 6174 686c 6962 2e50 6174  g or pathlib.Pat
+00017580: 682e 0a20 2020 2054 7970 6545 7272 6f72  h..    TypeError
+00017590: 0a20 2020 2020 2020 2060 6361 7669 7469  .        `caviti
+000175a0: 6573 6020 6d75 7374 2062 6520 6120 6e75  es` must be a nu
+000175b0: 6d70 792e 6e64 6172 7261 792e 0a20 2020  mpy.ndarray..   
+000175c0: 2056 616c 7565 4572 726f 720a 2020 2020   ValueError.    
+000175d0: 2020 2020 6063 6176 6974 6965 7360 2068      `cavities` h
+000175e0: 6173 2074 6865 2069 6e63 6f72 7265 6374  as the incorrect
+000175f0: 2073 6861 7065 2e20 4974 206d 7573 7420   shape. It must 
+00017600: 6265 2028 6e78 2c20 6e79 2c20 6e7a 292e  be (nx, ny, nz).
+00017610: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
+00017620: 2020 2020 2020 2060 7375 7266 6163 6560         `surface`
+00017630: 206d 7573 7420 6265 2061 206e 756d 7079   must be a numpy
+00017640: 2e6e 6461 7272 6179 2e0a 2020 2020 5661  .ndarray..    Va
+00017650: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
+00017660: 2060 7375 7266 6163 6560 2068 6173 2074   `surface` has t
+00017670: 6865 2069 6e63 6f72 7265 6374 2073 6861  he incorrect sha
+00017680: 7065 2e20 4974 206d 7573 7420 6265 2028  pe. It must be (
+00017690: 6e78 2c20 6e79 2c20 6e7a 292e 0a20 2020  nx, ny, nz)..   
+000176a0: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
+000176b0: 2020 2060 7665 7274 6963 6573 6020 6d75     `vertices` mu
+000176c0: 7374 2062 6520 6120 6c69 7374 206f 7220  st be a list or 
+000176d0: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
+000176e0: 0a20 2020 2056 616c 7565 4572 726f 720a  .    ValueError.
+000176f0: 2020 2020 2020 2020 6076 6572 7469 6365          `vertice
+00017700: 7360 2068 6173 2069 6e63 6f72 7265 6374  s` has incorrect
+00017710: 2073 6861 7065 2e20 4974 206d 7573 7420   shape. It must 
+00017720: 6265 2028 342c 2033 292e 0a20 2020 2054  be (4, 3)..    T
+00017730: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
+00017740: 2060 7374 6570 6020 6d75 7374 2062 6520   `step` must be 
+00017750: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
+00017760: 6e75 6d62 6572 2e0a 2020 2020 5661 6c75  number..    Valu
 00017770: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-00017780: 7363 616c 6573 6020 6861 7320 7468 6520  scales` has the 
-00017790: 696e 636f 7272 6563 7420 7368 6170 652e  incorrect shape.
-000177a0: 2049 7420 6d75 7374 2062 6520 286e 782c   It must be (nx,
-000177b0: 206e 792c 206e 7a29 2e0a 2020 2020 5479   ny, nz)..    Ty
-000177c0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
-000177d0: 6073 656c 6563 7469 6f6e 6020 6d75 7374  `selection` must
-000177e0: 2062 6520 6120 6c69 7374 206f 6620 7374   be a list of st
-000177f0: 7269 6e67 7320 2863 6176 6974 7920 6e61  rings (cavity na
-00017800: 6d65 7329 206f 7220 696e 7465 6765 7273  mes) or integers
-00017810: 2028 6361 7669 7479 206c 6162 656c 7329   (cavity labels)
-00017820: 2e0a 2020 2020 5661 6c75 6545 7272 6f72  ..    ValueError
-00017830: 0a20 2020 2020 2020 2049 6e76 616c 6964  .        Invalid
-00017840: 2060 7365 6c65 6374 696f 6e60 3a20 7b73   `selection`: {s
-00017850: 656c 6563 7469 6f6e 7d2e 0a20 2020 2054  election}..    T
-00017860: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-00017870: 2060 6e74 6872 6561 6473 6020 6d75 7374   `nthreads` must
-00017880: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
-00017890: 6e74 6567 6572 2e0a 2020 2020 5661 6c75  nteger..    Valu
-000178a0: 6545 7272 6f72 0a20 2020 2020 2020 2060  eError.        `
-000178b0: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
-000178c0: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
-000178d0: 6567 6572 2e0a 2020 2020 5479 7065 4572  eger..    TypeEr
-000178e0: 726f 720a 2020 2020 2020 2020 6061 7070  ror.        `app
-000178f0: 656e 6460 206d 7573 7420 6265 2061 2062  end` must be a b
-00017900: 6f6f 6c65 616e 2e0a 2020 2020 5479 7065  oolean..    Type
-00017910: 4572 726f 720a 2020 2020 2020 2020 606d  Error.        `m
-00017920: 6f64 656c 6020 6d75 7374 2062 6520 6120  odel` must be a 
-00017930: 696e 7465 6765 722e 0a20 2020 2052 756e  integer..    Run
-00017940: 7469 6d65 4572 726f 720a 2020 2020 2020  timeError.      
-00017950: 2020 5573 6572 206d 7573 7420 6465 6669    User must defi
-00017960: 6e65 2060 7375 7266 6163 6560 2077 6865  ne `surface` whe
-00017970: 6e20 6e6f 7420 6465 6669 6e69 6e67 2060  n not defining `
-00017980: 6361 7669 7469 6573 602e 0a0a 2020 2020  cavities`...    
-00017990: 4e6f 7465 0a20 2020 202d 2d2d 2d0a 2020  Note.    ----.  
-000179a0: 2020 5468 6520 6361 7669 7479 206e 6f6d    The cavity nom
-000179b0: 656e 636c 6174 7572 6520 6973 2062 6173  enclature is bas
-000179c0: 6564 206f 6e20 7468 6520 696e 7465 6765  ed on the intege
-000179d0: 7220 6c61 6265 6c2e 2054 6865 2063 6176  r label. The cav
-000179e0: 6974 7920 6d61 726b 6564 0a20 2020 2077  ity marked.    w
-000179f0: 6974 6820 322c 2074 6865 2066 6972 7374  ith 2, the first
-00017a00: 2069 6e74 6567 6572 2063 6f72 7265 7370   integer corresp
-00017a10: 6f6e 6469 6e67 2074 6f20 6120 6361 7669  onding to a cavi
-00017a20: 7479 2c20 6973 204b 4141 2c20 7468 6520  ty, is KAA, the 
-00017a30: 6361 7669 7479 0a20 2020 206d 6172 6b65  cavity.    marke
-00017a40: 6420 7769 7468 2033 2069 7320 4b41 422c  d with 3 is KAB,
-00017a50: 2074 6865 2063 6176 6974 7920 6d61 726b   the cavity mark
-00017a60: 6564 2077 6974 6820 3420 6973 204b 4143  ed with 4 is KAC
-00017a70: 2061 6e64 2073 6f20 6f6e 2e0a 0a20 2020   and so on...   
-00017a80: 2053 6565 2041 6c73 6f0a 2020 2020 2d2d   See Also.    --
-00017a90: 2d2d 2d2d 2d2d 0a20 2020 2064 6574 6563  ------.    detec
-00017aa0: 740a 2020 2020 7370 6174 6961 6c0a 2020  t.    spatial.  
-00017ab0: 2020 6465 7074 680a 2020 2020 6879 6472    depth.    hydr
-00017ac0: 6f70 6174 6879 0a20 2020 2077 7269 7465  opathy.    write
-00017ad0: 5f72 6573 756c 7473 0a0a 2020 2020 4578  _results..    Ex
-00017ae0: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-00017af0: 2d0a 2020 2020 5769 7468 2074 6865 2063  -.    With the c
-00017b00: 6176 6974 7920 616e 6420 7375 7266 6163  avity and surfac
-00017b10: 6520 706f 696e 7473 2069 6465 6e74 6966  e points identif
-00017b20: 6965 6420 616e 6420 6465 7074 6820 616e  ied and depth an
-00017b30: 6420 6879 6472 6f70 686f 6269 6369 7479  d hydrophobicity
-00017b40: 2073 6361 6c65 206d 6170 7065 6420 696e   scale mapped in
-00017b50: 2074 6865 2033 4420 6772 6964 2c20 7765   the 3D grid, we
-00017b60: 2063 616e 3a0a 0a20 2020 202a 2045 7870   can:..    * Exp
-00017b70: 6f72 7420 6361 7669 7479 2070 6f69 6e74  ort cavity point
-00017b80: 730a 0a20 2020 203e 3e3e 2066 726f 6d20  s..    >>> from 
-00017b90: 7079 4b56 4669 6e64 6572 2069 6d70 6f72  pyKVFinder impor
-00017ba0: 7420 6578 706f 7274 0a20 2020 203e 3e3e  t export.    >>>
-00017bb0: 2065 7870 6f72 7428 2763 6176 6974 795f   export('cavity_
-00017bc0: 776f 5f73 7572 6661 6365 2e70 6462 272c  wo_surface.pdb',
-00017bd0: 2063 6176 6974 6965 732c 204e 6f6e 652c   cavities, None,
-00017be0: 2076 6572 7469 6365 7329 0a0a 2020 2020   vertices)..    
-00017bf0: 2a20 4578 706f 7274 2063 6176 6974 7920  * Export cavity 
-00017c00: 616e 6420 7375 7266 6163 6520 706f 696e  and surface poin
-00017c10: 7473 0a0a 2020 2020 3e3e 3e20 6578 706f  ts..    >>> expo
-00017c20: 7274 2827 6361 7669 7469 6573 2e70 6462  rt('cavities.pdb
-00017c30: 272c 2063 6176 6974 6965 732c 2073 7572  ', cavities, sur
-00017c40: 6661 6365 2c20 7665 7274 6963 6573 290a  face, vertices).
-00017c50: 0a20 2020 202a 2045 7870 6f72 7420 6361  .    * Export ca
-00017c60: 7669 7479 2061 6e64 2073 7572 6661 6365  vity and surface
-00017c70: 2070 6f69 6e74 7320 7769 7468 2064 6570   points with dep
-00017c80: 7468 206d 6170 7065 6420 6f6e 2074 6865  th mapped on the
-00017c90: 6d0a 0a20 2020 203e 3e3e 2065 7870 6f72  m..    >>> expor
-00017ca0: 7428 2763 6176 6974 6965 735f 7769 7468  t('cavities_with
-00017cb0: 5f64 6570 7468 2e70 6462 272c 2063 6176  _depth.pdb', cav
-00017cc0: 6974 6965 732c 2073 7572 6661 6365 2c20  ities, surface, 
-00017cd0: 7665 7274 6963 6573 2c20 423d 6465 7074  vertices, B=dept
-00017ce0: 6873 290a 0a20 2020 202a 2045 7870 6f72  hs)..    * Expor
-00017cf0: 7420 7375 7266 6163 6520 706f 696e 7473  t surface points
-00017d00: 2077 6974 6820 6879 6472 6f70 686f 6269   with hydrophobi
-00017d10: 6369 7479 5f73 6361 6c65 206d 6170 7065  city_scale mappe
-00017d20: 6420 6f6e 2074 6865 6d0a 0a20 2020 203e  d on them..    >
-00017d30: 3e3e 2065 7870 6f72 7428 4e6f 6e65 2c20  >> export(None, 
-00017d40: 4e6f 6e65 2c20 7375 7266 6163 652c 2076  None, surface, v
-00017d50: 6572 7469 6365 732c 206f 7574 7075 745f  ertices, output_
-00017d60: 6879 6472 6f70 6174 6879 3d27 6879 6472  hydropathy='hydr
-00017d70: 6f70 6174 6879 2e70 6462 272c 2073 6361  opathy.pdb', sca
-00017d80: 6c65 733d 7363 616c 6573 290a 0a20 2020  les=scales)..   
-00017d90: 202a 2045 7870 6f72 7420 616c 6c0a 0a20   * Export all.. 
-00017da0: 2020 203e 3e3e 2065 7870 6f72 7428 2763     >>> export('c
-00017db0: 6176 6974 6965 732e 7064 6227 2c20 6361  avities.pdb', ca
-00017dc0: 7669 7469 6573 2c20 7375 7266 6163 652c  vities, surface,
-00017dd0: 2076 6572 7469 6365 732c 2042 3d64 6570   vertices, B=dep
-00017de0: 7468 732c 206f 7574 7075 745f 6879 6472  ths, output_hydr
-00017df0: 6f70 6174 6879 3d27 6879 6472 6f70 6174  opathy='hydropat
-00017e00: 6879 2e70 6462 272c 2073 6361 6c65 733d  hy.pdb', scales=
-00017e10: 7363 616c 6573 290a 0a20 2020 2022 2222  scales)..    """
-00017e20: 0a20 2020 2066 726f 6d20 5f70 794b 5646  .    from _pyKVF
-00017e30: 696e 6465 7220 696d 706f 7274 205f 6578  inder import _ex
-00017e40: 706f 7274 2c20 5f65 7870 6f72 745f 620a  port, _export_b.
-00017e50: 0a20 2020 2023 2043 6865 636b 2061 7267  .    # Check arg
-00017e60: 756d 656e 7473 0a20 2020 2069 6620 666e  uments.    if fn
-00017e70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00017e80: 2020 2020 2020 6966 2074 7970 6528 666e        if type(fn
-00017e90: 2920 6e6f 7420 696e 205b 7374 722c 2070  ) not in [str, p
-00017ea0: 6174 686c 6962 2e50 6174 685d 3a0a 2020  athlib.Path]:.  
-00017eb0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017ec0: 5479 7065 4572 726f 7228 2260 666e 6020  TypeError("`fn` 
-00017ed0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-00017ee0: 206f 7220 6120 7061 7468 6c69 622e 5061   or a pathlib.Pa
-00017ef0: 7468 2e22 290a 2020 2020 2020 2020 6f73  th.").        os
-00017f00: 2e6d 616b 6564 6972 7328 6f73 2e70 6174  .makedirs(os.pat
-00017f10: 682e 6162 7370 6174 6828 6f73 2e70 6174  h.abspath(os.pat
-00017f20: 682e 6469 726e 616d 6528 666e 2929 2c20  h.dirname(fn)), 
-00017f30: 6578 6973 745f 6f6b 3d54 7275 6529 0a20  exist_ok=True). 
-00017f40: 2020 2069 6620 6361 7669 7469 6573 2069     if cavities i
-00017f50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00017f60: 2020 2020 6966 2074 7970 6528 6361 7669      if type(cavi
-00017f70: 7469 6573 2920 6e6f 7420 696e 205b 6e75  ties) not in [nu
-00017f80: 6d70 792e 6e64 6172 7261 795d 3a0a 2020  mpy.ndarray]:.  
-00017f90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017fa0: 5479 7065 4572 726f 7228 2260 6361 7669  TypeError("`cavi
-00017fb0: 7469 6573 6020 6d75 7374 2062 6520 6120  ties` must be a 
-00017fc0: 6e75 6d70 792e 6e64 6172 7261 792e 2229  numpy.ndarray.")
-00017fd0: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
-00017fe0: 6e28 6361 7669 7469 6573 2e73 6861 7065  n(cavities.shape
-00017ff0: 2920 213d 2033 3a0a 2020 2020 2020 2020  ) != 3:.        
-00018000: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00018010: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00018020: 2020 2020 2020 2260 6361 7669 7469 6573        "`cavities
-00018030: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
-00018040: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
-00018050: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
-00018060: 7a29 2e22 0a20 2020 2020 2020 2020 2020  z).".           
-00018070: 2029 0a20 2020 2069 6620 7375 7266 6163   ).    if surfac
-00018080: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00018090: 2020 2020 2020 2069 6620 7479 7065 2873         if type(s
-000180a0: 7572 6661 6365 2920 6e6f 7420 696e 205b  urface) not in [
+00017780: 7374 6570 6020 6d75 7374 2062 6520 6120  step` must be a 
+00017790: 706f 7369 7469 7665 2072 6561 6c20 6e75  positive real nu
+000177a0: 6d62 6572 2e0a 2020 2020 5479 7065 4572  mber..    TypeEr
+000177b0: 726f 720a 2020 2020 2020 2020 6042 6020  ror.        `B` 
+000177c0: 6d75 7374 2062 6520 6120 6e75 6d70 792e  must be a numpy.
+000177d0: 6e64 6172 7261 792e 0a20 2020 2056 616c  ndarray..    Val
+000177e0: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
+000177f0: 6042 6020 6861 7320 7468 6520 696e 636f  `B` has the inco
+00017800: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+00017810: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+00017820: 206e 7a29 2e0a 2020 2020 5479 7065 4572   nz)..    TypeEr
+00017830: 726f 720a 2020 2020 2020 2020 606f 7574  ror.        `out
+00017840: 7075 745f 6879 6472 6f70 6174 6879 6020  put_hydropathy` 
+00017850: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+00017860: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
+00017870: 2020 2020 2020 2020 6073 6361 6c65 7360          `scales`
+00017880: 206d 7573 7420 6265 2061 206e 756d 7079   must be a numpy
+00017890: 2e6e 6461 7272 6179 2e0a 2020 2020 5661  .ndarray..    Va
+000178a0: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
+000178b0: 2060 7363 616c 6573 6020 6861 7320 7468   `scales` has th
+000178c0: 6520 696e 636f 7272 6563 7420 7368 6170  e incorrect shap
+000178d0: 652e 2049 7420 6d75 7374 2062 6520 286e  e. It must be (n
+000178e0: 782c 206e 792c 206e 7a29 2e0a 2020 2020  x, ny, nz)..    
+000178f0: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
+00017900: 2020 6073 656c 6563 7469 6f6e 6020 6d75    `selection` mu
+00017910: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
+00017920: 7374 7269 6e67 7320 2863 6176 6974 7920  strings (cavity 
+00017930: 6e61 6d65 7329 206f 7220 696e 7465 6765  names) or intege
+00017940: 7273 2028 6361 7669 7479 206c 6162 656c  rs (cavity label
+00017950: 7329 2e0a 2020 2020 5661 6c75 6545 7272  s)..    ValueErr
+00017960: 6f72 0a20 2020 2020 2020 2049 6e76 616c  or.        Inval
+00017970: 6964 2060 7365 6c65 6374 696f 6e60 3a20  id `selection`: 
+00017980: 7b73 656c 6563 7469 6f6e 7d2e 0a20 2020  {selection}..   
+00017990: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
+000179a0: 2020 2060 6e74 6872 6561 6473 6020 6d75     `nthreads` mu
+000179b0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+000179c0: 2069 6e74 6567 6572 2e0a 2020 2020 5661   integer..    Va
+000179d0: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
+000179e0: 2060 6e74 6872 6561 6473 6020 6d75 7374   `nthreads` must
+000179f0: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
+00017a00: 6e74 6567 6572 2e0a 2020 2020 5479 7065  nteger..    Type
+00017a10: 4572 726f 720a 2020 2020 2020 2020 6061  Error.        `a
+00017a20: 7070 656e 6460 206d 7573 7420 6265 2061  ppend` must be a
+00017a30: 2062 6f6f 6c65 616e 2e0a 2020 2020 5479   boolean..    Ty
+00017a40: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+00017a50: 606d 6f64 656c 6020 6d75 7374 2062 6520  `model` must be 
+00017a60: 6120 696e 7465 6765 722e 0a20 2020 2052  a integer..    R
+00017a70: 756e 7469 6d65 4572 726f 720a 2020 2020  untimeError.    
+00017a80: 2020 2020 5573 6572 206d 7573 7420 6465      User must de
+00017a90: 6669 6e65 2060 7375 7266 6163 6560 2077  fine `surface` w
+00017aa0: 6865 6e20 6e6f 7420 6465 6669 6e69 6e67  hen not defining
+00017ab0: 2060 6361 7669 7469 6573 602e 0a0a 2020   `cavities`...  
+00017ac0: 2020 4e6f 7465 0a20 2020 202d 2d2d 2d0a    Note.    ----.
+00017ad0: 2020 2020 5468 6520 6361 7669 7479 206e      The cavity n
+00017ae0: 6f6d 656e 636c 6174 7572 6520 6973 2062  omenclature is b
+00017af0: 6173 6564 206f 6e20 7468 6520 696e 7465  ased on the inte
+00017b00: 6765 7220 6c61 6265 6c2e 2054 6865 2063  ger label. The c
+00017b10: 6176 6974 7920 6d61 726b 6564 0a20 2020  avity marked.   
+00017b20: 2077 6974 6820 322c 2074 6865 2066 6972   with 2, the fir
+00017b30: 7374 2069 6e74 6567 6572 2063 6f72 7265  st integer corre
+00017b40: 7370 6f6e 6469 6e67 2074 6f20 6120 6361  sponding to a ca
+00017b50: 7669 7479 2c20 6973 204b 4141 2c20 7468  vity, is KAA, th
+00017b60: 6520 6361 7669 7479 0a20 2020 206d 6172  e cavity.    mar
+00017b70: 6b65 6420 7769 7468 2033 2069 7320 4b41  ked with 3 is KA
+00017b80: 422c 2074 6865 2063 6176 6974 7920 6d61  B, the cavity ma
+00017b90: 726b 6564 2077 6974 6820 3420 6973 204b  rked with 4 is K
+00017ba0: 4143 2061 6e64 2073 6f20 6f6e 2e0a 0a20  AC and so on... 
+00017bb0: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
+00017bc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6574  --------.    det
+00017bd0: 6563 740a 2020 2020 7370 6174 6961 6c0a  ect.    spatial.
+00017be0: 2020 2020 6465 7074 680a 2020 2020 6879      depth.    hy
+00017bf0: 6472 6f70 6174 6879 0a20 2020 2077 7269  dropathy.    wri
+00017c00: 7465 5f72 6573 756c 7473 0a0a 2020 2020  te_results..    
+00017c10: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
+00017c20: 2d2d 2d0a 2020 2020 5769 7468 2074 6865  ---.    With the
+00017c30: 2063 6176 6974 7920 616e 6420 7375 7266   cavity and surf
+00017c40: 6163 6520 706f 696e 7473 2069 6465 6e74  ace points ident
+00017c50: 6966 6965 6420 616e 6420 6465 7074 6820  ified and depth 
+00017c60: 616e 6420 6879 6472 6f70 686f 6269 6369  and hydrophobici
+00017c70: 7479 2073 6361 6c65 206d 6170 7065 6420  ty scale mapped 
+00017c80: 696e 2074 6865 2033 4420 6772 6964 2c20  in the 3D grid, 
+00017c90: 7765 2063 616e 3a0a 0a20 2020 202a 2045  we can:..    * E
+00017ca0: 7870 6f72 7420 6361 7669 7479 2070 6f69  xport cavity poi
+00017cb0: 6e74 730a 0a20 2020 203e 3e3e 2066 726f  nts..    >>> fro
+00017cc0: 6d20 7079 4b56 4669 6e64 6572 2069 6d70  m pyKVFinder imp
+00017cd0: 6f72 7420 6578 706f 7274 0a20 2020 203e  ort export.    >
+00017ce0: 3e3e 2065 7870 6f72 7428 2763 6176 6974  >> export('cavit
+00017cf0: 795f 776f 5f73 7572 6661 6365 2e70 6462  y_wo_surface.pdb
+00017d00: 272c 2063 6176 6974 6965 732c 204e 6f6e  ', cavities, Non
+00017d10: 652c 2076 6572 7469 6365 7329 0a0a 2020  e, vertices)..  
+00017d20: 2020 2a20 4578 706f 7274 2063 6176 6974    * Export cavit
+00017d30: 7920 616e 6420 7375 7266 6163 6520 706f  y and surface po
+00017d40: 696e 7473 0a0a 2020 2020 3e3e 3e20 6578  ints..    >>> ex
+00017d50: 706f 7274 2827 6361 7669 7469 6573 2e70  port('cavities.p
+00017d60: 6462 272c 2063 6176 6974 6965 732c 2073  db', cavities, s
+00017d70: 7572 6661 6365 2c20 7665 7274 6963 6573  urface, vertices
+00017d80: 290a 0a20 2020 202a 2045 7870 6f72 7420  )..    * Export 
+00017d90: 6361 7669 7479 2061 6e64 2073 7572 6661  cavity and surfa
+00017da0: 6365 2070 6f69 6e74 7320 7769 7468 2064  ce points with d
+00017db0: 6570 7468 206d 6170 7065 6420 6f6e 2074  epth mapped on t
+00017dc0: 6865 6d0a 0a20 2020 203e 3e3e 2065 7870  hem..    >>> exp
+00017dd0: 6f72 7428 2763 6176 6974 6965 735f 7769  ort('cavities_wi
+00017de0: 7468 5f64 6570 7468 2e70 6462 272c 2063  th_depth.pdb', c
+00017df0: 6176 6974 6965 732c 2073 7572 6661 6365  avities, surface
+00017e00: 2c20 7665 7274 6963 6573 2c20 423d 6465  , vertices, B=de
+00017e10: 7074 6873 290a 0a20 2020 202a 2045 7870  pths)..    * Exp
+00017e20: 6f72 7420 7375 7266 6163 6520 706f 696e  ort surface poin
+00017e30: 7473 2077 6974 6820 6879 6472 6f70 686f  ts with hydropho
+00017e40: 6269 6369 7479 5f73 6361 6c65 206d 6170  bicity_scale map
+00017e50: 7065 6420 6f6e 2074 6865 6d0a 0a20 2020  ped on them..   
+00017e60: 203e 3e3e 2065 7870 6f72 7428 4e6f 6e65   >>> export(None
+00017e70: 2c20 4e6f 6e65 2c20 7375 7266 6163 652c  , None, surface,
+00017e80: 2076 6572 7469 6365 732c 206f 7574 7075   vertices, outpu
+00017e90: 745f 6879 6472 6f70 6174 6879 3d27 6879  t_hydropathy='hy
+00017ea0: 6472 6f70 6174 6879 2e70 6462 272c 2073  dropathy.pdb', s
+00017eb0: 6361 6c65 733d 7363 616c 6573 290a 0a20  cales=scales).. 
+00017ec0: 2020 202a 2045 7870 6f72 7420 616c 6c0a     * Export all.
+00017ed0: 0a20 2020 203e 3e3e 2065 7870 6f72 7428  .    >>> export(
+00017ee0: 2763 6176 6974 6965 732e 7064 6227 2c20  'cavities.pdb', 
+00017ef0: 6361 7669 7469 6573 2c20 7375 7266 6163  cavities, surfac
+00017f00: 652c 2076 6572 7469 6365 732c 2042 3d64  e, vertices, B=d
+00017f10: 6570 7468 732c 206f 7574 7075 745f 6879  epths, output_hy
+00017f20: 6472 6f70 6174 6879 3d27 6879 6472 6f70  dropathy='hydrop
+00017f30: 6174 6879 2e70 6462 272c 2073 6361 6c65  athy.pdb', scale
+00017f40: 733d 7363 616c 6573 290a 0a20 2020 2022  s=scales)..    "
+00017f50: 2222 0a20 2020 2066 726f 6d20 5f70 794b  "".    from _pyK
+00017f60: 5646 696e 6465 7220 696d 706f 7274 205f  VFinder import _
+00017f70: 6578 706f 7274 2c20 5f65 7870 6f72 745f  export, _export_
+00017f80: 620a 0a20 2020 2023 2043 6865 636b 2061  b..    # Check a
+00017f90: 7267 756d 656e 7473 0a20 2020 2069 6620  rguments.    if 
+00017fa0: 666e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  fn is not None:.
+00017fb0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00017fc0: 666e 2920 6e6f 7420 696e 205b 7374 722c  fn) not in [str,
+00017fd0: 2070 6174 686c 6962 2e50 6174 685d 3a0a   pathlib.Path]:.
+00017fe0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00017ff0: 6520 5479 7065 4572 726f 7228 2260 666e  e TypeError("`fn
+00018000: 6020 6d75 7374 2062 6520 6120 7374 7269  ` must be a stri
+00018010: 6e67 206f 7220 6120 7061 7468 6c69 622e  ng or a pathlib.
+00018020: 5061 7468 2e22 290a 2020 2020 2020 2020  Path.").        
+00018030: 6f73 2e6d 616b 6564 6972 7328 6f73 2e70  os.makedirs(os.p
+00018040: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
+00018050: 6174 682e 6469 726e 616d 6528 666e 2929  ath.dirname(fn))
+00018060: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
+00018070: 0a20 2020 2069 6620 6361 7669 7469 6573  .    if cavities
+00018080: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00018090: 2020 2020 2020 6966 2074 7970 6528 6361        if type(ca
+000180a0: 7669 7469 6573 2920 6e6f 7420 696e 205b  vities) not in [
 000180b0: 6e75 6d70 792e 6e64 6172 7261 795d 3a0a  numpy.ndarray]:.
 000180c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000180d0: 6520 5479 7065 4572 726f 7228 2260 7375  e TypeError("`su
-000180e0: 7266 6163 6560 206d 7573 7420 6265 2061  rface` must be a
-000180f0: 206e 756d 7079 2e6e 6461 7272 6179 2e22   numpy.ndarray."
-00018100: 290a 2020 2020 2020 2020 656c 6966 206c  ).        elif l
-00018110: 656e 2873 7572 6661 6365 2e73 6861 7065  en(surface.shape
-00018120: 2920 213d 2033 3a0a 2020 2020 2020 2020  ) != 3:.        
-00018130: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00018140: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00018150: 2020 2020 2020 2260 7375 7266 6163 6560        "`surface`
-00018160: 2068 6173 2074 6865 2069 6e63 6f72 7265   has the incorre
-00018170: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
-00018180: 7420 6265 2028 6e78 2c20 6e79 2c20 6e7a  t be (nx, ny, nz
-00018190: 292e 220a 2020 2020 2020 2020 2020 2020  ).".            
-000181a0: 290a 2020 2020 6966 2074 7970 6528 7665  ).    if type(ve
-000181b0: 7274 6963 6573 2920 6e6f 7420 696e 205b  rtices) not in [
-000181c0: 6e75 6d70 792e 6e64 6172 7261 792c 206c  numpy.ndarray, l
-000181d0: 6973 745d 3a0a 2020 2020 2020 2020 7261  ist]:.        ra
-000181e0: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-000181f0: 7665 7274 6963 6573 6020 6d75 7374 2062  vertices` must b
-00018200: 6520 6120 6c69 7374 206f 7220 6120 6e75  e a list or a nu
-00018210: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
-00018220: 2020 2065 6c69 6620 6e75 6d70 792e 6173     elif numpy.as
-00018230: 6172 7261 7928 7665 7274 6963 6573 292e  array(vertices).
-00018240: 7368 6170 6520 213d 2028 342c 2033 293a  shape != (4, 3):
-00018250: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00018260: 616c 7565 4572 726f 7228 2260 7665 7274  alueError("`vert
-00018270: 6963 6573 6020 6861 7320 696e 636f 7272  ices` has incorr
-00018280: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
-00018290: 7374 2062 6520 2834 2c20 3329 2e22 290a  st be (4, 3).").
-000182a0: 2020 2020 6966 2074 7970 6528 7374 6570      if type(step
-000182b0: 2920 6e6f 7420 696e 205b 666c 6f61 742c  ) not in [float,
-000182c0: 2069 6e74 5d3a 0a20 2020 2020 2020 2072   int]:.        r
-000182d0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-000182e0: 6073 7465 7060 206d 7573 7420 6265 2061  `step` must be a
-000182f0: 2070 6f73 6974 6976 6520 7265 616c 206e   positive real n
-00018300: 756d 6265 722e 2229 0a20 2020 2065 6c69  umber.").    eli
-00018310: 6620 7374 6570 203c 3d20 302e 303a 0a20  f step <= 0.0:. 
-00018320: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00018330: 7565 4572 726f 7228 2260 7374 6570 6020  ueError("`step` 
-00018340: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-00018350: 7665 2072 6561 6c20 6e75 6d62 6572 2e22  ve real number."
-00018360: 290a 2020 2020 6966 2042 2069 7320 6e6f  ).    if B is no
-00018370: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00018380: 6966 2074 7970 6528 4229 206e 6f74 2069  if type(B) not i
-00018390: 6e20 5b6e 756d 7079 2e6e 6461 7272 6179  n [numpy.ndarray
-000183a0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
-000183b0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-000183c0: 6042 6020 6d75 7374 2062 6520 6120 6e75  `B` must be a nu
-000183d0: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
-000183e0: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
-000183f0: 422e 7368 6170 6529 2021 3d20 333a 0a20  B.shape) != 3:. 
-00018400: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018410: 2056 616c 7565 4572 726f 7228 2260 4260   ValueError("`B`
-00018420: 2068 6173 2074 6865 2069 6e63 6f72 7265   has the incorre
-00018430: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
-00018440: 7420 6265 2028 6e78 2c20 6e79 2c20 6e7a  t be (nx, ny, nz
-00018450: 292e 2229 0a20 2020 2069 6620 6f75 7470  ).").    if outp
-00018460: 7574 5f68 7964 726f 7061 7468 7920 6973  ut_hydropathy is
-00018470: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00018480: 2020 2069 6620 7479 7065 286f 7574 7075     if type(outpu
-00018490: 745f 6879 6472 6f70 6174 6879 2920 6e6f  t_hydropathy) no
-000184a0: 7420 696e 205b 7374 722c 2070 6174 686c  t in [str, pathl
-000184b0: 6962 2e50 6174 685d 3a0a 2020 2020 2020  ib.Path]:.      
-000184c0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-000184d0: 4572 726f 7228 2260 6f75 7470 7574 5f68  Error("`output_h
-000184e0: 7964 726f 7061 7468 7960 206d 7573 7420  ydropathy` must 
-000184f0: 6265 2061 2073 7472 696e 6720 6f72 2061  be a string or a
-00018500: 2070 6174 686c 6962 2e50 6174 682e 2229   pathlib.Path.")
-00018510: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
-00018520: 6469 7273 286f 732e 7061 7468 2e61 6273  dirs(os.path.abs
-00018530: 7061 7468 286f 732e 7061 7468 2e64 6972  path(os.path.dir
-00018540: 6e61 6d65 286f 7574 7075 745f 6879 6472  name(output_hydr
-00018550: 6f70 6174 6879 2929 2c20 6578 6973 745f  opathy)), exist_
-00018560: 6f6b 3d54 7275 6529 0a20 2020 2069 6620  ok=True).    if 
-00018570: 7363 616c 6573 2069 7320 6e6f 7420 4e6f  scales is not No
-00018580: 6e65 3a0a 2020 2020 2020 2020 6966 2074  ne:.        if t
-00018590: 7970 6528 7363 616c 6573 2920 6e6f 7420  ype(scales) not 
-000185a0: 696e 205b 6e75 6d70 792e 6e64 6172 7261  in [numpy.ndarra
-000185b0: 795d 3a0a 2020 2020 2020 2020 2020 2020  y]:.            
-000185c0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000185d0: 2260 7363 616c 6573 6020 6d75 7374 2062  "`scales` must b
-000185e0: 6520 6120 6e75 6d70 792e 6e64 6172 7261  e a numpy.ndarra
-000185f0: 792e 2229 0a20 2020 2020 2020 2065 6c69  y.").        eli
-00018600: 6620 6c65 6e28 7363 616c 6573 2e73 6861  f len(scales.sha
-00018610: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
-00018620: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00018630: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00018640: 2020 2020 2020 2020 2260 7363 616c 6573          "`scales
-00018650: 6020 6861 7320 7468 6520 696e 636f 7272  ` has the incorr
-00018660: 6563 7420 7368 6170 652e 2049 7420 6d75  ect shape. It mu
-00018670: 7374 2062 6520 286e 782c 206e 792c 206e  st be (nx, ny, n
-00018680: 7a29 2e22 0a20 2020 2020 2020 2020 2020  z).".           
-00018690: 2029 0a20 2020 2069 6620 7365 6c65 6374   ).    if select
-000186a0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-000186b0: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
-000186c0: 2073 656c 6563 7469 6f6e 2074 7970 6573   selection types
-000186d0: 0a20 2020 2020 2020 2069 6620 616c 6c28  .        if all(
-000186e0: 6973 696e 7374 616e 6365 2878 2c20 696e  isinstance(x, in
-000186f0: 7429 2066 6f72 2078 2069 6e20 7365 6c65  t) for x in sele
-00018700: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-00018710: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-00018720: 2065 6c69 6620 616c 6c28 6973 696e 7374   elif all(isinst
-00018730: 616e 6365 2878 2c20 7374 7229 2066 6f72  ance(x, str) for
-00018740: 2078 2069 6e20 7365 6c65 6374 696f 6e29   x in selection)
-00018750: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00018760: 6c65 6374 696f 6e20 3d20 5b5f 6765 745f  lection = [_get_
-00018770: 6361 7669 7479 5f6c 6162 656c 2873 656c  cavity_label(sel
-00018780: 6529 2066 6f72 2073 656c 6520 696e 2073  e) for sele in s
-00018790: 656c 6563 7469 6f6e 5d0a 2020 2020 2020  election].      
-000187a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000187b0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-000187c0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-000187d0: 2020 2020 2022 6073 656c 6563 7469 6f6e       "`selection
-000187e0: 6020 6d75 7374 2062 6520 6120 6c69 7374  ` must be a list
-000187f0: 206f 6620 7374 7269 6e67 7320 2863 6176   of strings (cav
-00018800: 6974 7920 6e61 6d65 7329 206f 7220 696e  ity names) or in
-00018810: 7465 6765 7273 2028 6361 7669 7479 206c  tegers (cavity l
-00018820: 6162 656c 7329 2e22 0a20 2020 2020 2020  abels).".       
-00018830: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
-00018840: 2043 6865 636b 2069 6620 7365 6c65 6374   Check if select
-00018850: 696f 6e20 696e 636c 7564 6573 2076 616c  ion includes val
-00018860: 6964 2063 6176 6974 7920 6c61 6265 6c73  id cavity labels
-00018870: 0a20 2020 2020 2020 2069 6620 616e 7928  .        if any(
-00018880: 7820 3c20 3220 666f 7220 7820 696e 2073  x < 2 for x in s
-00018890: 656c 6563 7469 6f6e 293a 0a20 2020 2020  election):.     
-000188a0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000188b0: 7565 4572 726f 7228 6622 496e 7661 6c69  ueError(f"Invali
-000188c0: 6420 6073 656c 6563 7469 6f6e 603a 207b  d `selection`: {
-000188d0: 7365 6c65 6374 696f 6e7d 2e22 290a 2020  selection}.").  
-000188e0: 2020 6966 206e 7468 7265 6164 7320 6973    if nthreads is
-000188f0: 204e 6f6e 653a 0a20 2020 2020 2020 206e   None:.        n
-00018900: 7468 7265 6164 7320 3d20 6f73 2e63 7075  threads = os.cpu
-00018910: 5f63 6f75 6e74 2829 202d 2031 0a20 2020  _count() - 1.   
-00018920: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
-00018930: 6620 7479 7065 286e 7468 7265 6164 7329  f type(nthreads)
-00018940: 206e 6f74 2069 6e20 5b69 6e74 5d3a 0a20   not in [int]:. 
-00018950: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018960: 2054 7970 6545 7272 6f72 2822 606e 7468   TypeError("`nth
-00018970: 7265 6164 7360 206d 7573 7420 6265 2061  reads` must be a
-00018980: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
-00018990: 722e 2229 0a20 2020 2020 2020 2065 6c69  r.").        eli
-000189a0: 6620 6e74 6872 6561 6473 203c 3d20 303a  f nthreads <= 0:
-000189b0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000189c0: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
-000189d0: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
-000189e0: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
-000189f0: 6567 6572 2e22 290a 2020 2020 6966 2074  eger.").    if t
-00018a00: 7970 6528 6170 7065 6e64 2920 6e6f 7420  ype(append) not 
-00018a10: 696e 205b 626f 6f6c 5d3a 0a20 2020 2020  in [bool]:.     
-00018a20: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-00018a30: 6f72 2822 6061 7070 656e 6460 206d 7573  or("`append` mus
-00018a40: 7420 6265 2061 2062 6f6f 6c65 616e 2e22  t be a boolean."
-00018a50: 290a 2020 2020 6966 2074 7970 6528 6d6f  ).    if type(mo
-00018a60: 6465 6c29 206e 6f74 2069 6e20 5b69 6e74  del) not in [int
-00018a70: 5d3a 0a20 2020 2020 2020 2072 6169 7365  ]:.        raise
-00018a80: 2054 7970 6545 7272 6f72 2822 606d 6f64   TypeError("`mod
-00018a90: 656c 6020 6d75 7374 2062 6520 6120 696e  el` must be a in
-00018aa0: 7465 6765 722e 2229 0a0a 2020 2020 2320  teger.")..    # 
-00018ab0: 436f 6e76 6572 7420 7479 7065 730a 2020  Convert types.  
-00018ac0: 2020 6966 2074 7970 6528 7665 7274 6963    if type(vertic
-00018ad0: 6573 2920 3d3d 206c 6973 743a 0a20 2020  es) == list:.   
-00018ae0: 2020 2020 2076 6572 7469 6365 7320 3d20       vertices = 
-00018af0: 6e75 6d70 792e 6173 6172 7261 7928 7665  numpy.asarray(ve
-00018b00: 7274 6963 6573 290a 2020 2020 6966 2074  rtices).    if t
-00018b10: 7970 6528 7374 6570 2920 3d3d 2069 6e74  ype(step) == int
-00018b20: 3a0a 2020 2020 2020 2020 7374 6570 203d  :.        step =
-00018b30: 2066 6c6f 6174 2873 7465 7029 0a0a 2020   float(step)..  
-00018b40: 2020 2320 436f 6e76 6572 7420 6e75 6d70    # Convert nump
-00018b50: 792e 6e64 6172 7261 7920 6461 7461 2074  y.ndarray data t
-00018b60: 7970 6573 0a20 2020 2076 6572 7469 6365  ypes.    vertice
-00018b70: 7320 3d20 7665 7274 6963 6573 2e61 7374  s = vertices.ast
-00018b80: 7970 6528 2266 6c6f 6174 3634 2229 2069  ype("float64") i
-00018b90: 6620 7665 7274 6963 6573 2e64 7479 7065  f vertices.dtype
-00018ba0: 2021 3d20 2266 6c6f 6174 3634 2220 656c   != "float64" el
-00018bb0: 7365 2076 6572 7469 6365 730a 2020 2020  se vertices.    
-00018bc0: 6966 2042 2069 7320 6e6f 7420 4e6f 6e65  if B is not None
-00018bd0: 3a0a 2020 2020 2020 2020 4220 3d20 422e  :.        B = B.
-00018be0: 6173 7479 7065 2822 666c 6f61 7436 3422  astype("float64"
-00018bf0: 2920 6966 2042 2e64 7479 7065 2021 3d20  ) if B.dtype != 
-00018c00: 2266 6c6f 6174 3634 2220 656c 7365 2042  "float64" else B
-00018c10: 0a20 2020 2069 6620 7363 616c 6573 2069  .    if scales i
-00018c20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00018c30: 2020 2020 7363 616c 6573 203d 2073 6361      scales = sca
-00018c40: 6c65 732e 6173 7479 7065 2822 666c 6f61  les.astype("floa
-00018c50: 7436 3422 2920 6966 2073 6361 6c65 732e  t64") if scales.
-00018c60: 6474 7970 6520 213d 2022 666c 6f61 7436  dtype != "float6
-00018c70: 3422 2065 6c73 6520 7363 616c 6573 0a0a  4" else scales..
-00018c80: 2020 2020 2320 4765 7420 7369 6e63 6f73      # Get sincos
-00018c90: 3a20 7369 6e65 2061 6e64 2063 6f73 7369  : sine and cossi
-00018ca0: 6e65 206f 6620 7468 6520 6772 6964 2072  ne of the grid r
-00018cb0: 6f74 6174 696f 6e20 616e 676c 6573 2028  otation angles (
-00018cc0: 7369 6e61 2c20 636f 7361 2c20 7369 6e62  sina, cosa, sinb
-00018cd0: 2c20 636f 7362 290a 2020 2020 7369 6e63  , cosb).    sinc
-00018ce0: 6f73 203d 205f 6765 745f 7369 6e63 6f73  os = _get_sincos
-00018cf0: 2876 6572 7469 6365 7329 0a0a 2020 2020  (vertices)..    
-00018d00: 2320 556e 7061 636b 2076 6572 7469 6365  # Unpack vertice
-00018d10: 730a 2020 2020 5031 2c20 5032 2c20 5033  s.    P1, P2, P3
-00018d20: 2c20 5034 203d 2076 6572 7469 6365 730a  , P4 = vertices.
-00018d30: 0a20 2020 2023 2049 6620 7375 7266 6163  .    # If surfac
-00018d40: 6520 6973 204e 6f6e 652c 2063 7265 6174  e is None, creat
-00018d50: 6520 616e 2065 6d70 7479 2067 7269 640a  e an empty grid.
-00018d60: 2020 2020 6966 2063 6176 6974 6965 7320      if cavities 
-00018d70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00018d80: 2020 2020 2069 6620 7375 7266 6163 6520       if surface 
-00018d90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00018da0: 2020 2020 2073 7572 6661 6365 203d 206e       surface = n
-00018db0: 756d 7079 2e7a 6572 6f73 2863 6176 6974  umpy.zeros(cavit
-00018dc0: 6965 732e 7368 6170 652c 2064 7479 7065  ies.shape, dtype
-00018dd0: 3d22 696e 7433 3222 290a 2020 2020 2020  ="int32").      
-00018de0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00018df0: 2020 2020 7375 7266 6163 6520 3d20 7375      surface = su
-00018e00: 7266 6163 652e 6173 7479 7065 2822 696e  rface.astype("in
-00018e10: 7433 3222 2920 6966 2073 7572 6661 6365  t32") if surface
-00018e20: 2e64 7479 7065 2021 3d20 2269 6e74 3332  .dtype != "int32
-00018e30: 2220 656c 7365 2073 7572 6661 6365 0a0a  " else surface..
-00018e40: 2020 2020 2320 5365 6c65 6374 2063 6176      # Select cav
-00018e50: 6974 6965 730a 2020 2020 6966 2073 656c  ities.    if sel
-00018e60: 6563 7469 6f6e 2069 7320 6e6f 7420 4e6f  ection is not No
-00018e70: 6e65 3a0a 2020 2020 2020 2020 7375 7266  ne:.        surf
-00018e80: 6163 6520 3d20 5f73 656c 6563 745f 6361  ace = _select_ca
-00018e90: 7669 7469 6573 2873 7572 6661 6365 2c20  vities(surface, 
-00018ea0: 7365 6c65 6374 696f 6e29 0a20 2020 2020  selection).     
-00018eb0: 2020 2069 6620 6361 7669 7469 6573 2069     if cavities i
-00018ec0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00018ed0: 2020 2020 2020 2020 6361 7669 7469 6573          cavities
-00018ee0: 203d 205f 7365 6c65 6374 5f63 6176 6974   = _select_cavit
-00018ef0: 6965 7328 6361 7669 7469 6573 2c20 7365  ies(cavities, se
-00018f00: 6c65 6374 696f 6e29 0a0a 2020 2020 6966  lection)..    if
-00018f10: 2063 6176 6974 6965 7320 6973 204e 6f6e   cavities is Non
-00018f20: 653a 0a20 2020 2020 2020 2069 6620 7375  e:.        if su
-00018f30: 7266 6163 6520 6973 204e 6f6e 653a 0a20  rface is None:. 
-00018f40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00018f50: 2052 756e 7469 6d65 4572 726f 7228 0a20   RuntimeError(. 
-00018f60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00018f70: 2255 7365 7220 6d75 7374 2064 6566 696e  "User must defin
-00018f80: 6520 6073 7572 6661 6365 6020 7768 656e  e `surface` when
-00018f90: 206e 6f74 2064 6566 696e 696e 6720 6063   not defining `c
-00018fa0: 6176 6974 6965 7360 2e22 0a20 2020 2020  avities`.".     
-00018fb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018fc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00018fd0: 2020 2023 2047 6574 206e 756d 6265 7220     # Get number 
-00018fe0: 6f66 2063 6176 6974 6965 730a 2020 2020  of cavities.    
-00018ff0: 2020 2020 2020 2020 6e63 6176 203d 2069          ncav = i
-00019000: 6e74 2873 7572 6661 6365 2e6d 6178 2829  nt(surface.max()
-00019010: 202d 2031 290a 0a20 2020 2020 2020 2020   - 1)..         
-00019020: 2020 2023 2045 7870 6f72 7420 6879 6472     # Export hydr
-00019030: 6f70 6174 6879 0a20 2020 2020 2020 2020  opathy.         
-00019040: 2020 205f 6578 706f 7274 5f62 280a 2020     _export_b(.  
-00019050: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00019060: 7470 7574 5f68 7964 726f 7061 7468 792c  tput_hydropathy,
-00019070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019080: 2073 7572 6661 6365 2c0a 2020 2020 2020   surface,.      
-00019090: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-000190a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000190b0: 2020 2073 6361 6c65 732c 0a20 2020 2020     scales,.     
-000190c0: 2020 2020 2020 2020 2020 2050 312c 0a20             P1,. 
-000190d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000190e0: 696e 636f 732c 0a20 2020 2020 2020 2020  incos,.         
-000190f0: 2020 2020 2020 2073 7465 702c 0a20 2020         step,.   
-00019100: 2020 2020 2020 2020 2020 2020 206e 6361               nca
-00019110: 762c 0a20 2020 2020 2020 2020 2020 2020  v,.             
-00019120: 2020 206e 7468 7265 6164 732c 0a20 2020     nthreads,.   
-00019130: 2020 2020 2020 2020 2020 2020 2061 7070               app
-00019140: 656e 642c 0a20 2020 2020 2020 2020 2020  end,.           
-00019150: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
-00019160: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00019170: 7365 3a0a 2020 2020 2020 2020 2320 4368  se:.        # Ch
-00019180: 6563 6b20 616e 6420 636f 6e76 6572 7420  eck and convert 
-00019190: 6361 7669 7469 6573 2064 7479 7065 0a20  cavities dtype. 
-000191a0: 2020 2020 2020 2063 6176 6974 6965 7320         cavities 
-000191b0: 3d20 6361 7669 7469 6573 2e61 7374 7970  = cavities.astyp
-000191c0: 6528 2269 6e74 3332 2229 2069 6620 6361  e("int32") if ca
-000191d0: 7669 7469 6573 2e64 7479 7065 2021 3d20  vities.dtype != 
-000191e0: 2269 6e74 3332 2220 656c 7365 2063 6176  "int32" else cav
-000191f0: 6974 6965 730a 0a20 2020 2020 2020 2023  ities..        #
-00019200: 2047 6574 206e 756d 6265 7220 6f66 2063   Get number of c
-00019210: 6176 6974 6965 730a 2020 2020 2020 2020  avities.        
-00019220: 6e63 6176 203d 2069 6e74 2863 6176 6974  ncav = int(cavit
-00019230: 6965 732e 6d61 7828 2920 2d20 3129 0a0a  ies.max() - 1)..
-00019240: 2020 2020 2020 2020 2320 4578 706f 7274          # Export
-00019250: 2063 6176 6974 6965 730a 2020 2020 2020   cavities.      
-00019260: 2020 6966 2042 2069 7320 4e6f 6e65 3a0a    if B is None:.
-00019270: 2020 2020 2020 2020 2020 2020 5f65 7870              _exp
-00019280: 6f72 7428 0a20 2020 2020 2020 2020 2020  ort(.           
-00019290: 2020 2020 2066 6e2c 2063 6176 6974 6965       fn, cavitie
-000192a0: 732c 2073 7572 6661 6365 2c20 5031 2c20  s, surface, P1, 
-000192b0: 7369 6e63 6f73 2c20 7374 6570 2c20 6e63  sincos, step, nc
-000192c0: 6176 2c20 6e74 6872 6561 6473 2c20 6170  av, nthreads, ap
-000192d0: 7065 6e64 2c20 6d6f 6465 6c0a 2020 2020  pend, model.    
-000192e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000192f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00019300: 2020 2020 5f65 7870 6f72 745f 6228 0a20      _export_b(. 
-00019310: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019320: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00019330: 2020 2063 6176 6974 6965 732c 0a20 2020     cavities,.   
-00019340: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-00019350: 6661 6365 2c0a 2020 2020 2020 2020 2020  face,.          
-00019360: 2020 2020 2020 422c 0a20 2020 2020 2020        B,.       
-00019370: 2020 2020 2020 2020 2050 312c 0a20 2020           P1,.   
-00019380: 2020 2020 2020 2020 2020 2020 2073 696e               sin
-00019390: 636f 732c 0a20 2020 2020 2020 2020 2020  cos,.           
-000193a0: 2020 2020 2073 7465 702c 0a20 2020 2020       step,.     
-000193b0: 2020 2020 2020 2020 2020 206e 6361 762c             ncav,
-000193c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000193d0: 206e 7468 7265 6164 732c 0a20 2020 2020   nthreads,.     
-000193e0: 2020 2020 2020 2020 2020 2061 7070 656e             appen
-000193f0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00019400: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
-00019410: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00019420: 2023 2045 7870 6f72 7420 6879 6472 6f70   # Export hydrop
-00019430: 6174 6879 2073 7572 6661 6365 2070 6f69  athy surface poi
-00019440: 6e74 730a 2020 2020 2020 2020 6966 2073  nts.        if s
-00019450: 6361 6c65 7320 6973 204e 6f6e 653a 0a20  cales is None:. 
-00019460: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00019470: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00019480: 2020 2020 2020 2020 2020 5f65 7870 6f72            _expor
-00019490: 745f 6228 0a20 2020 2020 2020 2020 2020  t_b(.           
-000194a0: 2020 2020 206f 7574 7075 745f 6879 6472       output_hydr
-000194b0: 6f70 6174 6879 2c0a 2020 2020 2020 2020  opathy,.        
-000194c0: 2020 2020 2020 2020 7375 7266 6163 652c          surface,
-000194d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000194e0: 2073 7572 6661 6365 2c0a 2020 2020 2020   surface,.      
-000194f0: 2020 2020 2020 2020 2020 7363 616c 6573            scales
-00019500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019510: 2020 5031 2c0a 2020 2020 2020 2020 2020    P1,.          
-00019520: 2020 2020 2020 7369 6e63 6f73 2c0a 2020        sincos,.  
-00019530: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00019540: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
-00019550: 2020 2020 6e63 6176 2c0a 2020 2020 2020      ncav,.      
-00019560: 2020 2020 2020 2020 2020 6e74 6872 6561            nthrea
-00019570: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00019580: 2020 2020 6170 7065 6e64 2c0a 2020 2020      append,.    
-00019590: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000195a0: 6c2c 0a20 2020 2020 2020 2020 2020 2029  l,.            )
-000195b0: 0a0a 0a64 6566 2065 7870 6f72 745f 6f70  ...def export_op
-000195c0: 656e 696e 6773 280a 2020 2020 666e 3a20  enings(.    fn: 
-000195d0: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-000195e0: 6962 2e50 6174 685d 2c0a 2020 2020 6f70  ib.Path],.    op
-000195f0: 656e 696e 6773 3a20 6e75 6d70 792e 6e64  enings: numpy.nd
-00019600: 6172 7261 792c 0a20 2020 2076 6572 7469  array,.    verti
-00019610: 6365 733a 2055 6e69 6f6e 5b6e 756d 7079  ces: Union[numpy
-00019620: 2e6e 6461 7272 6179 2c20 4c69 7374 5b4c  .ndarray, List[L
-00019630: 6973 745b 666c 6f61 745d 5d5d 2c0a 2020  ist[float]]],.  
-00019640: 2020 7374 6570 3a20 556e 696f 6e5b 666c    step: Union[fl
-00019650: 6f61 742c 2069 6e74 5d20 3d20 302e 362c  oat, int] = 0.6,
-00019660: 0a20 2020 2073 656c 6563 7469 6f6e 3a20  .    selection: 
-00019670: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b4c  Optional[Union[L
-00019680: 6973 745b 696e 745d 2c20 4c69 7374 5b73  ist[int], List[s
-00019690: 7472 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020  tr]]] = None,.  
-000196a0: 2020 6e74 6872 6561 6473 3a20 4f70 7469    nthreads: Opti
-000196b0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000196c0: 2c0a 2020 2020 6170 7065 6e64 3a20 626f  ,.    append: bo
-000196d0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-000196e0: 6d6f 6465 6c3a 2069 6e74 203d 2030 2c0a  model: int = 0,.
-000196f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00019700: 2222 4578 706f 7274 206f 7065 6e69 6e67  ""Export opening
-00019710: 2070 6f69 6e74 7320 2848 2920 746f 2061   points (H) to a
-00019720: 2050 4442 2d66 6f72 6d61 7474 6564 2066   PDB-formatted f
-00019730: 696c 652e 0a0a 2020 2020 5061 7261 6d65  ile...    Parame
-00019740: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00019750: 2d2d 2d0a 2020 2020 666e 203a 2055 6e69  ---.    fn : Uni
-00019760: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
-00019770: 5061 7468 5d0a 2020 2020 2020 2020 4120  Path].        A 
-00019780: 7061 7468 2074 6f20 5044 4220 6669 6c65  path to PDB file
-00019790: 2066 6f72 2077 7269 7469 6e67 206f 7065   for writing ope
-000197a0: 6e69 6e67 732e 0a20 2020 206f 7065 6e69  nings..    openi
-000197b0: 6e67 7320 3a20 6e75 6d70 792e 6e64 6172  ngs : numpy.ndar
-000197c0: 7261 790a 2020 2020 2020 2020 4f70 656e  ray.        Open
-000197d0: 696e 6773 2070 6f69 6e74 7320 696e 2074  ings points in t
-000197e0: 6865 2033 4420 6772 6964 2028 6f70 656e  he 3D grid (open
-000197f0: 696e 6773 5b6e 785d 5b6e 795d 5b6e 7a5d  ings[nx][ny][nz]
-00019800: 292e 0a20 2020 2020 2020 204f 7065 6e69  )..        Openi
-00019810: 6e67 7320 6172 7261 7920 6861 7320 696e  ngs array has in
-00019820: 7465 6765 7220 6c61 6265 6c73 2069 6e20  teger labels in 
-00019830: 6561 6368 2070 6f73 6974 696f 6e2c 2074  each position, t
-00019840: 6861 7420 6172 653a 0a0a 2020 2020 2020  hat are:..      
-00019850: 2020 2020 2020 2a20 2d31 3a20 6275 6c6b        * -1: bulk
-00019860: 2070 6f69 6e74 733b 0a0a 2020 2020 2020   points;..      
-00019870: 2020 2020 2020 2a20 303a 2063 6176 6974        * 0: cavit
-00019880: 7920 6f72 2062 696f 6d6f 6c65 6375 6c65  y or biomolecule
-00019890: 2070 6f69 6e74 733b 0a0a 2020 2020 2020   points;..      
-000198a0: 2020 2020 2020 2a20 313a 2065 6d70 7479        * 1: empty
-000198b0: 2073 7061 6365 2070 6f69 6e74 733b 0a0a   space points;..
-000198c0: 2020 2020 2020 2020 2020 2020 2a20 3e3d              * >=
-000198d0: 323a 204f 7065 6e69 6e67 2070 6f69 6e74  2: Opening point
-000198e0: 732e 0a0a 2020 2020 2020 2020 5468 6520  s...        The 
-000198f0: 656d 7074 7920 7370 6163 6520 706f 696e  empty space poin
-00019900: 7473 2061 7265 2072 6567 696f 6e73 2074  ts are regions t
-00019910: 6861 7420 646f 206e 6f74 206d 6565 7420  hat do not meet 
-00019920: 7468 6520 6368 6f73 656e 0a20 2020 2020  the chosen.     
-00019930: 2020 206f 7065 6e69 6e67 7320 6375 746f     openings cuto
-00019940: 6666 2074 6f20 6265 2063 6f6e 7369 6465  ff to be conside
-00019950: 7265 6420 616e 206f 7065 6e69 6e67 2e0a  red an opening..
-00019960: 2020 2020 7665 7274 6963 6573 203a 2055      vertices : U
-00019970: 6e69 6f6e 5b6e 756d 7079 2e6e 6461 7272  nion[numpy.ndarr
-00019980: 6179 2c20 4c69 7374 5b4c 6973 745b 666c  ay, List[List[fl
-00019990: 6f61 745d 5d5d 0a20 2020 2020 2020 2041  oat]]].        A
-000199a0: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
-000199b0: 7220 6120 6c69 7374 2077 6974 6820 7879  r a list with xy
-000199c0: 7a20 7665 7274 6963 6573 2063 6f6f 7264  z vertices coord
-000199d0: 696e 6174 6573 2028 6f72 6967 696e 2c0a  inates (origin,.
-000199e0: 2020 2020 2020 2020 582d 6178 6973 2c20          X-axis, 
-000199f0: 592d 6178 6973 2c20 5a2d 6178 6973 292e  Y-axis, Z-axis).
-00019a00: 0a20 2020 2073 7465 7020 3a20 556e 696f  .    step : Unio
-00019a10: 6e5b 666c 6f61 742c 2069 6e74 5d2c 206f  n[float, int], o
-00019a20: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00019a30: 4772 6964 2073 7061 6369 6e67 2028 4129  Grid spacing (A)
-00019a40: 2c20 6279 2064 6566 6175 6c74 2030 2e36  , by default 0.6
-00019a50: 2e0a 2020 2020 7365 6c65 6374 696f 6e20  ..    selection 
-00019a60: 3a20 556e 696f 6e5b 4c69 7374 5b69 6e74  : Union[List[int
-00019a70: 5d2c 204c 6973 745b 7374 725d 5d2c 206f  ], List[str]], o
-00019a80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00019a90: 4120 6c69 7374 206f 6620 696e 7465 6765  A list of intege
-00019aa0: 7220 6c61 6265 6c73 206f 7220 6120 6c69  r labels or a li
-00019ab0: 7374 206f 6620 6f70 656e 696e 6720 6e61  st of opening na
-00019ac0: 6d65 7320 746f 2062 6520 7365 6c65 6374  mes to be select
-00019ad0: 6564 2c20 6279 2064 6566 6175 6c74 204e  ed, by default N
-00019ae0: 6f6e 652e 0a20 2020 206e 7468 7265 6164  one..    nthread
-00019af0: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
-00019b00: 6c0a 2020 2020 2020 2020 4e75 6d62 6572  l.        Number
-00019b10: 206f 6620 7468 7265 6164 732c 2062 7920   of threads, by 
-00019b20: 6465 6661 756c 7420 4e6f 6e65 2e20 4966  default None. If
-00019b30: 204e 6f6e 652c 2074 6865 206e 756d 6265   None, the numbe
-00019b40: 7220 6f66 2074 6872 6561 6473 2069 730a  r of threads is.
-00019b50: 2020 2020 2020 2020 606f 732e 6370 755f          `os.cpu_
-00019b60: 636f 756e 7428 2920 2d20 3160 2e0a 2020  count() - 1`..  
-00019b70: 2020 6170 7065 6e64 203a 2062 6f6f 6c2c    append : bool,
-00019b80: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00019b90: 2020 5768 6574 6865 7220 746f 2061 7070    Whether to app
-00019ba0: 656e 6420 6f70 656e 696e 6773 2074 6f20  end openings to 
-00019bb0: 7468 6520 5044 4220 6669 6c65 2c20 6279  the PDB file, by
-00019bc0: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
-00019bd0: 2020 2020 6d6f 6465 6c20 3a20 696e 742c      model : int,
-00019be0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00019bf0: 2020 4d6f 6465 6c20 6e75 6d62 6572 2c20    Model number, 
-00019c00: 6279 2064 6566 6175 6c74 2030 2e0a 0a20  by default 0... 
-00019c10: 2020 2052 6169 7365 730a 2020 2020 2d2d     Raises.    --
-00019c20: 2d2d 2d2d 0a20 2020 2054 7970 6545 7272  ----.    TypeErr
-00019c30: 6f72 0a20 2020 2020 2020 2060 6f70 656e  or.        `open
-00019c40: 696e 6773 6020 6d75 7374 2062 6520 6120  ings` must be a 
-00019c50: 6e75 6d70 792e 6e64 6172 7261 792e 0a20  numpy.ndarray.. 
-00019c60: 2020 2056 616c 7565 4572 726f 720a 2020     ValueError.  
-00019c70: 2020 2020 2020 606f 7065 6e69 6e67 7360        `openings`
-00019c80: 2068 6173 2074 6865 2069 6e63 6f72 7265   has the incorre
-00019c90: 6374 2073 6861 7065 2e20 4974 206d 7573  ct shape. It mus
-00019ca0: 7420 6265 2028 6e78 2c20 6e79 2c20 6e7a  t be (nx, ny, nz
-00019cb0: 292e 0a20 2020 2054 7970 6545 7272 6f72  )..    TypeError
-00019cc0: 0a20 2020 2020 2020 2060 7665 7274 6963  .        `vertic
-00019cd0: 6573 6020 6d75 7374 2062 6520 6120 6c69  es` must be a li
-00019ce0: 7374 206f 7220 6120 6e75 6d70 792e 6e64  st or a numpy.nd
-00019cf0: 6172 7261 792e 0a20 2020 2056 616c 7565  array..    Value
-00019d00: 4572 726f 720a 2020 2020 2020 2020 6076  Error.        `v
-00019d10: 6572 7469 6365 7360 2068 6173 2069 6e63  ertices` has inc
-00019d20: 6f72 7265 6374 2073 6861 7065 2e20 4974  orrect shape. It
-00019d30: 206d 7573 7420 6265 2028 342c 2033 292e   must be (4, 3).
-00019d40: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
-00019d50: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
-00019d60: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-00019d70: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
-00019d80: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
-00019d90: 2020 2020 2060 7374 6570 6020 6d75 7374       `step` must
-00019da0: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
-00019db0: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
-00019dc0: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-00019dd0: 2020 6073 656c 6563 7469 6f6e 6020 6d75    `selection` mu
-00019de0: 7374 2062 6520 6120 6c69 7374 206f 6620  st be a list of 
-00019df0: 7374 7269 6e67 7320 286f 7065 6e69 6e67  strings (opening
-00019e00: 206e 616d 6573 2920 6f72 2069 6e74 6567   names) or integ
-00019e10: 6572 7320 286f 7065 6e69 6e67 206c 6162  ers (opening lab
-00019e20: 656c 7329 2e0a 2020 2020 5661 6c75 6545  els)..    ValueE
-00019e30: 7272 6f72 0a20 2020 2020 2020 2049 6e76  rror.        Inv
-00019e40: 616c 6964 2060 7365 6c65 6374 696f 6e60  alid `selection`
-00019e50: 3a20 7b73 656c 6563 7469 6f6e 7d2e 0a20  : {selection}.. 
-00019e60: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
-00019e70: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
-00019e80: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-00019e90: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
-00019ea0: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-00019eb0: 2020 2060 6e74 6872 6561 6473 6020 6d75     `nthreads` mu
-00019ec0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-00019ed0: 2069 6e74 6567 6572 2e0a 2020 2020 5479   integer..    Ty
-00019ee0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
-00019ef0: 6061 7070 656e 6460 206d 7573 7420 6265  `append` must be
-00019f00: 2061 2062 6f6f 6c65 616e 2e0a 2020 2020   a boolean..    
-00019f10: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
-00019f20: 2020 606d 6f64 656c 6020 6d75 7374 2062    `model` must b
-00019f30: 6520 6120 696e 7465 6765 722e 0a20 2020  e a integer..   
-00019f40: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-00019f50: 2020 2060 666e 6020 6d75 7374 2062 6520     `fn` must be 
-00019f60: 6120 7374 7269 6e67 206f 7220 7061 7468  a string or path
-00019f70: 6c69 622e 5061 7468 2e0a 0a20 2020 204e  lib.Path...    N
-00019f80: 6f74 650a 2020 2020 2d2d 2d2d 0a20 2020  ote.    ----.   
-00019f90: 2054 6865 206f 7065 6e69 6e67 206e 6f6d   The opening nom
-00019fa0: 656e 636c 6174 7572 6520 6973 2062 6173  enclature is bas
-00019fb0: 6564 206f 6e20 7468 6520 696e 7465 6765  ed on the intege
-00019fc0: 7220 6c61 6265 6c2e 2054 6865 206f 7065  r label. The ope
-00019fd0: 6e69 6e67 206d 6172 6b65 640a 2020 2020  ning marked.    
-00019fe0: 7769 7468 2032 2c20 7468 6520 6669 7273  with 2, the firs
-00019ff0: 7420 696e 7465 6765 7220 636f 7272 6573  t integer corres
-0001a000: 706f 6e64 696e 6720 746f 2061 206f 7065  ponding to a ope
-0001a010: 6e69 6e67 2c20 6973 204f 4141 2c20 7468  ning, is OAA, th
-0001a020: 6520 6f70 656e 696e 670a 2020 2020 6d61  e opening.    ma
-0001a030: 726b 6564 2077 6974 6820 3320 6973 204f  rked with 3 is O
-0001a040: 4142 2c20 7468 6520 6f70 656e 696e 6720  AB, the opening 
-0001a050: 6d61 726b 6564 2077 6974 6820 3420 6973  marked with 4 is
-0001a060: 204f 4143 2061 6e64 2073 6f20 6f6e 2e0a   OAC and so on..
-0001a070: 0a20 2020 2053 6565 2041 6c73 6f0a 2020  .    See Also.  
-0001a080: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065    --------.    e
-0001a090: 7870 6f72 740a 2020 2020 6465 7465 6374  xport.    detect
-0001a0a0: 0a20 2020 2064 6570 7468 730a 2020 2020  .    depths.    
-0001a0b0: 6f70 656e 696e 6773 0a0a 2020 2020 4578  openings..    Ex
-0001a0c0: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-0001a0d0: 2d0a 2020 2020 5769 7468 2074 6865 206f  -.    With the o
-0001a0e0: 7065 6e69 6e67 2070 6f69 6e74 7320 6964  pening points id
-0001a0f0: 656e 7469 6669 6564 2077 6974 6820 6060  entified with ``
-0001a100: 6f70 656e 696e 6773 6060 2c20 7765 2063  openings``, we c
-0001a110: 616e 2065 7870 6f72 7420 7468 656d 2074  an export them t
-0001a120: 6f20 6120 5044 422d 666f 726d 6174 7465  o a PDB-formatte
-0001a130: 6420 6669 6c65 3a0a 0a20 2020 203e 3e3e  d file:..    >>>
-0001a140: 2066 726f 6d20 7079 4b56 4669 6e64 6572   from pyKVFinder
-0001a150: 2069 6d70 6f72 7420 6578 706f 7274 5f6f   import export_o
-0001a160: 7065 6e69 6e67 730a 2020 2020 3e3e 3e20  penings.    >>> 
-0001a170: 6578 706f 7274 5f6f 7065 6e69 6e67 7328  export_openings(
-0001a180: 276f 7065 6e69 6e67 732e 7064 6227 2c20  'openings.pdb', 
-0001a190: 6f70 656e 696e 6773 2c20 7665 7274 6963  openings, vertic
-0001a1a0: 6573 290a 2020 2020 2222 220a 2020 2020  es).    """.    
-0001a1b0: 6672 6f6d 205f 7079 4b56 4669 6e64 6572  from _pyKVFinder
-0001a1c0: 2069 6d70 6f72 7420 5f65 7870 6f72 745f   import _export_
-0001a1d0: 6f70 656e 696e 6773 0a0a 2020 2020 2320  openings..    # 
-0001a1e0: 4368 6563 6b20 6172 6775 6d65 6e74 730a  Check arguments.
-0001a1f0: 2020 2020 6966 2074 7970 6528 6f70 656e      if type(open
-0001a200: 696e 6773 2920 6e6f 7420 696e 205b 6e75  ings) not in [nu
-0001a210: 6d70 792e 6e64 6172 7261 795d 3a0a 2020  mpy.ndarray]:.  
-0001a220: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-0001a230: 4572 726f 7228 2260 6f70 656e 696e 6773  Error("`openings
-0001a240: 6020 6d75 7374 2062 6520 6120 6e75 6d70  ` must be a nump
-0001a250: 792e 6e64 6172 7261 792e 2229 0a20 2020  y.ndarray.").   
-0001a260: 2065 6c69 6620 6c65 6e28 6f70 656e 696e   elif len(openin
-0001a270: 6773 2e73 6861 7065 2920 213d 2033 3a0a  gs.shape) != 3:.
-0001a280: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0001a290: 6c75 6545 7272 6f72 2822 606f 7065 6e69  lueError("`openi
-0001a2a0: 6e67 7360 2068 6173 2074 6865 2069 6e63  ngs` has the inc
-0001a2b0: 6f72 7265 6374 2073 6861 7065 2e20 4974  orrect shape. It
-0001a2c0: 206d 7573 7420 6265 2028 6e78 2c20 6e79   must be (nx, ny
-0001a2d0: 2c20 6e7a 292e 2229 0a20 2020 2069 6620  , nz).").    if 
-0001a2e0: 7479 7065 2876 6572 7469 6365 7329 206e  type(vertices) n
-0001a2f0: 6f74 2069 6e20 5b6e 756d 7079 2e6e 6461  ot in [numpy.nda
-0001a300: 7272 6179 2c20 6c69 7374 5d3a 0a20 2020  rray, list]:.   
-0001a310: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0001a320: 7272 6f72 2822 6076 6572 7469 6365 7360  rror("`vertices`
-0001a330: 206d 7573 7420 6265 2061 206c 6973 7420   must be a list 
-0001a340: 6f72 2061 206e 756d 7079 2e6e 6461 7272  or a numpy.ndarr
-0001a350: 6179 2e22 290a 2020 2020 656c 6966 206e  ay.").    elif n
-0001a360: 756d 7079 2e61 7361 7272 6179 2876 6572  umpy.asarray(ver
-0001a370: 7469 6365 7329 2e73 6861 7065 2021 3d20  tices).shape != 
-0001a380: 2834 2c20 3329 3a0a 2020 2020 2020 2020  (4, 3):.        
-0001a390: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0001a3a0: 2822 6076 6572 7469 6365 7360 2068 6173  ("`vertices` has
-0001a3b0: 2069 6e63 6f72 7265 6374 2073 6861 7065   incorrect shape
-0001a3c0: 2e20 4974 206d 7573 7420 6265 2028 342c  . It must be (4,
-0001a3d0: 2033 292e 2229 0a20 2020 2069 6620 7479   3).").    if ty
-0001a3e0: 7065 2873 7465 7029 206e 6f74 2069 6e20  pe(step) not in 
-0001a3f0: 5b66 6c6f 6174 2c20 696e 745d 3a0a 2020  [float, int]:.  
-0001a400: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-0001a410: 4572 726f 7228 2260 7374 6570 6020 6d75  Error("`step` mu
-0001a420: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-0001a430: 2072 6561 6c20 6e75 6d62 6572 2e22 290a   real number.").
-0001a440: 2020 2020 656c 6966 2073 7465 7020 3c3d      elif step <=
-0001a450: 2030 2e30 3a0a 2020 2020 2020 2020 7261   0.0:.        ra
-0001a460: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0001a470: 6073 7465 7060 206d 7573 7420 6265 2061  `step` must be a
-0001a480: 2070 6f73 6974 6976 6520 7265 616c 206e   positive real n
-0001a490: 756d 6265 722e 2229 0a20 2020 2069 6620  umber.").    if 
-0001a4a0: 7365 6c65 6374 696f 6e20 6973 206e 6f74  selection is not
-0001a4b0: 204e 6f6e 653a 0a20 2020 2020 2020 2023   None:.        #
-0001a4c0: 2043 6865 636b 2073 656c 6563 7469 6f6e   Check selection
-0001a4d0: 2074 7970 6573 0a20 2020 2020 2020 2069   types.        i
-0001a4e0: 6620 616c 6c28 6973 696e 7374 616e 6365  f all(isinstance
-0001a4f0: 2878 2c20 696e 7429 2066 6f72 2078 2069  (x, int) for x i
-0001a500: 6e20 7365 6c65 6374 696f 6e29 3a0a 2020  n selection):.  
-0001a510: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-0001a520: 2020 2020 2020 2065 6c69 6620 616c 6c28         elif all(
-0001a530: 6973 696e 7374 616e 6365 2878 2c20 7374  isinstance(x, st
-0001a540: 7229 2066 6f72 2078 2069 6e20 7365 6c65  r) for x in sele
-0001a550: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
-0001a560: 2020 2020 7365 6c65 6374 696f 6e20 3d20      selection = 
-0001a570: 5b5f 6765 745f 6f70 656e 696e 675f 6c61  [_get_opening_la
-0001a580: 6265 6c28 7365 6c65 2920 666f 7220 7365  bel(sele) for se
-0001a590: 6c65 2069 6e20 7365 6c65 6374 696f 6e5d  le in selection]
-0001a5a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001a5b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0001a5c0: 2054 7970 6545 7272 6f72 280a 2020 2020   TypeError(.    
-0001a5d0: 2020 2020 2020 2020 2020 2020 2260 7365              "`se
-0001a5e0: 6c65 6374 696f 6e60 206d 7573 7420 6265  lection` must be
-0001a5f0: 2061 206c 6973 7420 6f66 2073 7472 696e   a list of strin
-0001a600: 6773 2028 6361 7669 7479 206e 616d 6573  gs (cavity names
-0001a610: 2920 6f72 2069 6e74 6567 6572 7320 2863  ) or integers (c
-0001a620: 6176 6974 7920 6c61 6265 6c73 292e 220a  avity labels).".
-0001a630: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001a640: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
-0001a650: 2073 656c 6563 7469 6f6e 2069 6e63 6c75   selection inclu
-0001a660: 6465 7320 7661 6c69 6420 6361 7669 7479  des valid cavity
-0001a670: 206c 6162 656c 730a 2020 2020 2020 2020   labels.        
-0001a680: 6966 2061 6e79 2878 203c 2032 2066 6f72  if any(x < 2 for
-0001a690: 2078 2069 6e20 7365 6c65 6374 696f 6e29   x in selection)
-0001a6a0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001a6b0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-0001a6c0: 2249 6e76 616c 6964 2060 7365 6c65 6374  "Invalid `select
-0001a6d0: 696f 6e60 3a20 7b73 656c 6563 7469 6f6e  ion`: {selection
-0001a6e0: 7d2e 2229 0a20 2020 2069 6620 6e74 6872  }.").    if nthr
-0001a6f0: 6561 6473 2069 7320 4e6f 6e65 3a0a 2020  eads is None:.  
-0001a700: 2020 2020 2020 6e74 6872 6561 6473 203d        nthreads =
-0001a710: 206f 732e 6370 755f 636f 756e 7428 2920   os.cpu_count() 
-0001a720: 2d20 310a 2020 2020 656c 7365 3a0a 2020  - 1.    else:.  
-0001a730: 2020 2020 2020 6966 2074 7970 6528 6e74        if type(nt
-0001a740: 6872 6561 6473 2920 6e6f 7420 696e 205b  hreads) not in [
-0001a750: 696e 745d 3a0a 2020 2020 2020 2020 2020  int]:.          
-0001a760: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0001a770: 7228 2260 6e74 6872 6561 6473 6020 6d75  r("`nthreads` mu
-0001a780: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-0001a790: 2069 6e74 6567 6572 2e22 290a 2020 2020   integer.").    
-0001a7a0: 2020 2020 656c 6966 206e 7468 7265 6164      elif nthread
-0001a7b0: 7320 3c3d 2030 3a0a 2020 2020 2020 2020  s <= 0:.        
-0001a7c0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0001a7d0: 7272 6f72 2822 606e 7468 7265 6164 7360  rror("`nthreads`
-0001a7e0: 206d 7573 7420 6265 2061 2070 6f73 6974   must be a posit
-0001a7f0: 6976 6520 696e 7465 6765 722e 2229 0a20  ive integer."). 
-0001a800: 2020 2069 6620 7479 7065 2861 7070 656e     if type(appen
-0001a810: 6429 206e 6f74 2069 6e20 5b62 6f6f 6c5d  d) not in [bool]
-0001a820: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0001a830: 5479 7065 4572 726f 7228 2260 6170 7065  TypeError("`appe
-0001a840: 6e64 6020 6d75 7374 2062 6520 6120 626f  nd` must be a bo
-0001a850: 6f6c 6561 6e2e 2229 0a20 2020 2069 6620  olean.").    if 
-0001a860: 7479 7065 286d 6f64 656c 2920 6e6f 7420  type(model) not 
-0001a870: 696e 205b 696e 745d 3a0a 2020 2020 2020  in [int]:.      
-0001a880: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0001a890: 7228 2260 6d6f 6465 6c60 206d 7573 7420  r("`model` must 
-0001a8a0: 6265 2061 2069 6e74 6567 6572 2e22 290a  be a integer.").
-0001a8b0: 0a20 2020 2023 2043 6f6e 7665 7274 2074  .    # Convert t
-0001a8c0: 7970 6573 0a20 2020 2069 6620 7479 7065  ypes.    if type
-0001a8d0: 2876 6572 7469 6365 7329 203d 3d20 6c69  (vertices) == li
-0001a8e0: 7374 3a0a 2020 2020 2020 2020 7665 7274  st:.        vert
-0001a8f0: 6963 6573 203d 206e 756d 7079 2e61 7361  ices = numpy.asa
-0001a900: 7272 6179 2876 6572 7469 6365 7329 0a20  rray(vertices). 
-0001a910: 2020 2069 6620 7479 7065 2873 7465 7029     if type(step)
-0001a920: 203d 3d20 696e 743a 0a20 2020 2020 2020   == int:.       
-0001a930: 2073 7465 7020 3d20 666c 6f61 7428 7374   step = float(st
-0001a940: 6570 290a 0a20 2020 2023 2043 6f6e 7665  ep)..    # Conve
-0001a950: 7274 206e 756d 7079 2e6e 6461 7272 6179  rt numpy.ndarray
-0001a960: 2064 6174 6120 7479 7065 730a 2020 2020   data types.    
-0001a970: 7665 7274 6963 6573 203d 2076 6572 7469  vertices = verti
-0001a980: 6365 732e 6173 7479 7065 2822 666c 6f61  ces.astype("floa
-0001a990: 7436 3422 2920 6966 2076 6572 7469 6365  t64") if vertice
-0001a9a0: 732e 6474 7970 6520 213d 2022 666c 6f61  s.dtype != "floa
-0001a9b0: 7436 3422 2065 6c73 6520 7665 7274 6963  t64" else vertic
-0001a9c0: 6573 0a0a 2020 2020 2320 4765 7420 7369  es..    # Get si
-0001a9d0: 6e63 6f73 3a20 7369 6e65 2061 6e64 2063  ncos: sine and c
-0001a9e0: 6f73 7369 6e65 206f 6620 7468 6520 6772  ossine of the gr
-0001a9f0: 6964 2072 6f74 6174 696f 6e20 616e 676c  id rotation angl
-0001aa00: 6573 2028 7369 6e61 2c20 636f 7361 2c20  es (sina, cosa, 
-0001aa10: 7369 6e62 2c20 636f 7362 290a 2020 2020  sinb, cosb).    
-0001aa20: 7369 6e63 6f73 203d 205f 6765 745f 7369  sincos = _get_si
-0001aa30: 6e63 6f73 2876 6572 7469 6365 7329 0a0a  ncos(vertices)..
-0001aa40: 2020 2020 2320 4372 6561 7465 2062 6173      # Create bas
-0001aa50: 6520 6469 7265 6374 6f72 6965 7320 6f66  e directories of
-0001aa60: 2072 6573 756c 7473 0a20 2020 2069 6620   results.    if 
-0001aa70: 666e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  fn is not None:.
-0001aa80: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0001aa90: 666e 2920 6e6f 7420 696e 205b 7374 722c  fn) not in [str,
-0001aaa0: 2070 6174 686c 6962 2e50 6174 685d 3a0a   pathlib.Path]:.
-0001aab0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001aac0: 6520 5479 7065 4572 726f 7228 2260 666e  e TypeError("`fn
-0001aad0: 6020 6d75 7374 2062 6520 6120 7374 7269  ` must be a stri
-0001aae0: 6e67 206f 7220 6120 7061 7468 6c69 622e  ng or a pathlib.
-0001aaf0: 5061 7468 2e22 290a 2020 2020 2020 2020  Path.").        
-0001ab00: 6f73 2e6d 616b 6564 6972 7328 6f73 2e70  os.makedirs(os.p
-0001ab10: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
-0001ab20: 6174 682e 6469 726e 616d 6528 666e 2929  ath.dirname(fn))
-0001ab30: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
-0001ab40: 0a0a 2020 2020 2320 556e 7061 636b 2076  ..    # Unpack v
-0001ab50: 6572 7469 6365 730a 2020 2020 5031 2c20  ertices.    P1, 
-0001ab60: 5f2c 205f 2c20 5f20 3d20 7665 7274 6963  _, _, _ = vertic
-0001ab70: 6573 0a0a 2020 2020 2320 5365 6c65 6374  es..    # Select
-0001ab80: 2063 6176 6974 6965 730a 2020 2020 6966   cavities.    if
-0001ab90: 2073 656c 6563 7469 6f6e 2069 7320 6e6f   selection is no
-0001aba0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001abb0: 6f70 656e 696e 6773 203d 205f 7365 6c65  openings = _sele
-0001abc0: 6374 5f63 6176 6974 6965 7328 6f70 656e  ct_cavities(open
-0001abd0: 696e 6773 2c20 7365 6c65 6374 696f 6e29  ings, selection)
-0001abe0: 0a0a 2020 2020 2320 4765 7420 6e75 6d62  ..    # Get numb
-0001abf0: 6572 206f 6620 6f70 656e 696e 6773 0a20  er of openings. 
-0001ac00: 2020 206e 6f70 656e 696e 6773 203d 2069     nopenings = i
-0001ac10: 6e74 286f 7065 6e69 6e67 732e 6d61 7828  nt(openings.max(
-0001ac20: 2920 2d20 3129 0a0a 2020 2020 2320 4578  ) - 1)..    # Ex
-0001ac30: 706f 7274 206f 7065 6e69 6e67 730a 2020  port openings.  
-0001ac40: 2020 5f65 7870 6f72 745f 6f70 656e 696e    _export_openin
-0001ac50: 6773 2866 6e2c 206f 7065 6e69 6e67 732c  gs(fn, openings,
-0001ac60: 2050 312c 2073 696e 636f 732c 2073 7465   P1, sincos, ste
-0001ac70: 702c 206e 6f70 656e 696e 6773 2c20 6e74  p, nopenings, nt
-0001ac80: 6872 6561 6473 2c20 6170 7065 6e64 2c20  hreads, append, 
-0001ac90: 6d6f 6465 6c29 0a                        model).
+000180d0: 6520 5479 7065 4572 726f 7228 2260 6361  e TypeError("`ca
+000180e0: 7669 7469 6573 6020 6d75 7374 2062 6520  vities` must be 
+000180f0: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
+00018100: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
+00018110: 6c65 6e28 6361 7669 7469 6573 2e73 6861  len(cavities.sha
+00018120: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
+00018130: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00018140: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00018150: 2020 2020 2020 2020 2260 6361 7669 7469          "`caviti
+00018160: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
+00018170: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+00018180: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+00018190: 206e 7a29 2e22 0a20 2020 2020 2020 2020   nz).".         
+000181a0: 2020 2029 0a20 2020 2069 6620 7375 7266     ).    if surf
+000181b0: 6163 6520 6973 206e 6f74 204e 6f6e 653a  ace is not None:
+000181c0: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
+000181d0: 2873 7572 6661 6365 2920 6e6f 7420 696e  (surface) not in
+000181e0: 205b 6e75 6d70 792e 6e64 6172 7261 795d   [numpy.ndarray]
+000181f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00018200: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
+00018210: 7375 7266 6163 6560 206d 7573 7420 6265  surface` must be
+00018220: 2061 206e 756d 7079 2e6e 6461 7272 6179   a numpy.ndarray
+00018230: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
+00018240: 206c 656e 2873 7572 6661 6365 2e73 6861   len(surface.sha
+00018250: 7065 2920 213d 2033 3a0a 2020 2020 2020  pe) != 3:.      
+00018260: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00018270: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00018280: 2020 2020 2020 2020 2260 7375 7266 6163          "`surfac
+00018290: 6560 2068 6173 2074 6865 2069 6e63 6f72  e` has the incor
+000182a0: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
+000182b0: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
+000182c0: 6e7a 292e 220a 2020 2020 2020 2020 2020  nz).".          
+000182d0: 2020 290a 2020 2020 6966 2074 7970 6528    ).    if type(
+000182e0: 7665 7274 6963 6573 2920 6e6f 7420 696e  vertices) not in
+000182f0: 205b 6e75 6d70 792e 6e64 6172 7261 792c   [numpy.ndarray,
+00018300: 206c 6973 745d 3a0a 2020 2020 2020 2020   list]:.        
+00018310: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00018320: 2260 7665 7274 6963 6573 6020 6d75 7374  "`vertices` must
+00018330: 2062 6520 6120 6c69 7374 206f 7220 6120   be a list or a 
+00018340: 6e75 6d70 792e 6e64 6172 7261 792e 2229  numpy.ndarray.")
+00018350: 0a20 2020 2065 6c69 6620 6e75 6d70 792e  .    elif numpy.
+00018360: 6173 6172 7261 7928 7665 7274 6963 6573  asarray(vertices
+00018370: 292e 7368 6170 6520 213d 2028 342c 2033  ).shape != (4, 3
+00018380: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00018390: 2056 616c 7565 4572 726f 7228 2260 7665   ValueError("`ve
+000183a0: 7274 6963 6573 6020 6861 7320 696e 636f  rtices` has inco
+000183b0: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+000183c0: 6d75 7374 2062 6520 2834 2c20 3329 2e22  must be (4, 3)."
+000183d0: 290a 2020 2020 6966 2074 7970 6528 7374  ).    if type(st
+000183e0: 6570 2920 6e6f 7420 696e 205b 666c 6f61  ep) not in [floa
+000183f0: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
+00018400: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00018410: 2822 6073 7465 7060 206d 7573 7420 6265  ("`step` must be
+00018420: 2061 2070 6f73 6974 6976 6520 7265 616c   a positive real
+00018430: 206e 756d 6265 722e 2229 0a20 2020 2065   number.").    e
+00018440: 6c69 6620 7374 6570 203c 3d20 302e 303a  lif step <= 0.0:
+00018450: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00018460: 616c 7565 4572 726f 7228 2260 7374 6570  alueError("`step
+00018470: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+00018480: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
+00018490: 2e22 290a 2020 2020 6966 2042 2069 7320  .").    if B is 
+000184a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000184b0: 2020 6966 2074 7970 6528 4229 206e 6f74    if type(B) not
+000184c0: 2069 6e20 5b6e 756d 7079 2e6e 6461 7272   in [numpy.ndarr
+000184d0: 6179 5d3a 0a20 2020 2020 2020 2020 2020  ay]:.           
+000184e0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000184f0: 2822 6042 6020 6d75 7374 2062 6520 6120  ("`B` must be a 
+00018500: 6e75 6d70 792e 6e64 6172 7261 792e 2229  numpy.ndarray.")
+00018510: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
+00018520: 6e28 422e 7368 6170 6529 2021 3d20 333a  n(B.shape) != 3:
+00018530: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00018540: 7365 2056 616c 7565 4572 726f 7228 2260  se ValueError("`
+00018550: 4260 2068 6173 2074 6865 2069 6e63 6f72  B` has the incor
+00018560: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
+00018570: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
+00018580: 6e7a 292e 2229 0a20 2020 2069 6620 6f75  nz).").    if ou
+00018590: 7470 7574 5f68 7964 726f 7061 7468 7920  tput_hydropathy 
+000185a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000185b0: 2020 2020 2069 6620 7479 7065 286f 7574       if type(out
+000185c0: 7075 745f 6879 6472 6f70 6174 6879 2920  put_hydropathy) 
+000185d0: 6e6f 7420 696e 205b 7374 722c 2070 6174  not in [str, pat
+000185e0: 686c 6962 2e50 6174 685d 3a0a 2020 2020  hlib.Path]:.    
+000185f0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00018600: 7065 4572 726f 7228 2260 6f75 7470 7574  peError("`output
+00018610: 5f68 7964 726f 7061 7468 7960 206d 7573  _hydropathy` mus
+00018620: 7420 6265 2061 2073 7472 696e 6720 6f72  t be a string or
+00018630: 2061 2070 6174 686c 6962 2e50 6174 682e   a pathlib.Path.
+00018640: 2229 0a20 2020 2020 2020 206f 732e 6d61  ").        os.ma
+00018650: 6b65 6469 7273 286f 732e 7061 7468 2e61  kedirs(os.path.a
+00018660: 6273 7061 7468 286f 732e 7061 7468 2e64  bspath(os.path.d
+00018670: 6972 6e61 6d65 286f 7574 7075 745f 6879  irname(output_hy
+00018680: 6472 6f70 6174 6879 2929 2c20 6578 6973  dropathy)), exis
+00018690: 745f 6f6b 3d54 7275 6529 0a20 2020 2069  t_ok=True).    i
+000186a0: 6620 7363 616c 6573 2069 7320 6e6f 7420  f scales is not 
+000186b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+000186c0: 2074 7970 6528 7363 616c 6573 2920 6e6f   type(scales) no
+000186d0: 7420 696e 205b 6e75 6d70 792e 6e64 6172  t in [numpy.ndar
+000186e0: 7261 795d 3a0a 2020 2020 2020 2020 2020  ray]:.          
+000186f0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+00018700: 7228 2260 7363 616c 6573 6020 6d75 7374  r("`scales` must
+00018710: 2062 6520 6120 6e75 6d70 792e 6e64 6172   be a numpy.ndar
+00018720: 7261 792e 2229 0a20 2020 2020 2020 2065  ray.").        e
+00018730: 6c69 6620 6c65 6e28 7363 616c 6573 2e73  lif len(scales.s
+00018740: 6861 7065 2920 213d 2033 3a0a 2020 2020  hape) != 3:.    
+00018750: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00018760: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00018770: 2020 2020 2020 2020 2020 2260 7363 616c            "`scal
+00018780: 6573 6020 6861 7320 7468 6520 696e 636f  es` has the inco
+00018790: 7272 6563 7420 7368 6170 652e 2049 7420  rrect shape. It 
+000187a0: 6d75 7374 2062 6520 286e 782c 206e 792c  must be (nx, ny,
+000187b0: 206e 7a29 2e22 0a20 2020 2020 2020 2020   nz).".         
+000187c0: 2020 2029 0a20 2020 2069 6620 7365 6c65     ).    if sele
+000187d0: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
+000187e0: 653a 0a20 2020 2020 2020 2023 2043 6865  e:.        # Che
+000187f0: 636b 2073 656c 6563 7469 6f6e 2074 7970  ck selection typ
+00018800: 6573 0a20 2020 2020 2020 2069 6620 616c  es.        if al
+00018810: 6c28 6973 696e 7374 616e 6365 2878 2c20  l(isinstance(x, 
+00018820: 696e 7429 2066 6f72 2078 2069 6e20 7365  int) for x in se
+00018830: 6c65 6374 696f 6e29 3a0a 2020 2020 2020  lection):.      
+00018840: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00018850: 2020 2065 6c69 6620 616c 6c28 6973 696e     elif all(isin
+00018860: 7374 616e 6365 2878 2c20 7374 7229 2066  stance(x, str) f
+00018870: 6f72 2078 2069 6e20 7365 6c65 6374 696f  or x in selectio
+00018880: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+00018890: 7365 6c65 6374 696f 6e20 3d20 5b5f 6765  selection = [_ge
+000188a0: 745f 6361 7669 7479 5f6c 6162 656c 2873  t_cavity_label(s
+000188b0: 656c 6529 2066 6f72 2073 656c 6520 696e  ele) for sele in
+000188c0: 2073 656c 6563 7469 6f6e 5d0a 2020 2020   selection].    
+000188d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000188e0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+000188f0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00018900: 2020 2020 2020 2022 6073 656c 6563 7469         "`selecti
+00018910: 6f6e 6020 6d75 7374 2062 6520 6120 6c69  on` must be a li
+00018920: 7374 206f 6620 7374 7269 6e67 7320 2863  st of strings (c
+00018930: 6176 6974 7920 6e61 6d65 7329 206f 7220  avity names) or 
+00018940: 696e 7465 6765 7273 2028 6361 7669 7479  integers (cavity
+00018950: 206c 6162 656c 7329 2e22 0a20 2020 2020   labels).".     
+00018960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018970: 2023 2043 6865 636b 2069 6620 7365 6c65   # Check if sele
+00018980: 6374 696f 6e20 696e 636c 7564 6573 2076  ction includes v
+00018990: 616c 6964 2063 6176 6974 7920 6c61 6265  alid cavity labe
+000189a0: 6c73 0a20 2020 2020 2020 2069 6620 616e  ls.        if an
+000189b0: 7928 7820 3c20 3220 666f 7220 7820 696e  y(x < 2 for x in
+000189c0: 2073 656c 6563 7469 6f6e 293a 0a20 2020   selection):.   
+000189d0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000189e0: 616c 7565 4572 726f 7228 6622 496e 7661  alueError(f"Inva
+000189f0: 6c69 6420 6073 656c 6563 7469 6f6e 603a  lid `selection`:
+00018a00: 207b 7365 6c65 6374 696f 6e7d 2e22 290a   {selection}.").
+00018a10: 2020 2020 6966 206e 7468 7265 6164 7320      if nthreads 
+00018a20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00018a30: 206e 7468 7265 6164 7320 3d20 6f73 2e63   nthreads = os.c
+00018a40: 7075 5f63 6f75 6e74 2829 202d 2031 0a20  pu_count() - 1. 
+00018a50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00018a60: 2069 6620 7479 7065 286e 7468 7265 6164   if type(nthread
+00018a70: 7329 206e 6f74 2069 6e20 5b69 6e74 5d3a  s) not in [int]:
+00018a80: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00018a90: 7365 2054 7970 6545 7272 6f72 2822 606e  se TypeError("`n
+00018aa0: 7468 7265 6164 7360 206d 7573 7420 6265  threads` must be
+00018ab0: 2061 2070 6f73 6974 6976 6520 696e 7465   a positive inte
+00018ac0: 6765 722e 2229 0a20 2020 2020 2020 2065  ger.").        e
+00018ad0: 6c69 6620 6e74 6872 6561 6473 203c 3d20  lif nthreads <= 
+00018ae0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00018af0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00018b00: 2260 6e74 6872 6561 6473 6020 6d75 7374  "`nthreads` must
+00018b10: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
+00018b20: 6e74 6567 6572 2e22 290a 2020 2020 6966  nteger.").    if
+00018b30: 2074 7970 6528 6170 7065 6e64 2920 6e6f   type(append) no
+00018b40: 7420 696e 205b 626f 6f6c 5d3a 0a20 2020  t in [bool]:.   
+00018b50: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00018b60: 7272 6f72 2822 6061 7070 656e 6460 206d  rror("`append` m
+00018b70: 7573 7420 6265 2061 2062 6f6f 6c65 616e  ust be a boolean
+00018b80: 2e22 290a 2020 2020 6966 2074 7970 6528  .").    if type(
+00018b90: 6d6f 6465 6c29 206e 6f74 2069 6e20 5b69  model) not in [i
+00018ba0: 6e74 5d3a 0a20 2020 2020 2020 2072 6169  nt]:.        rai
+00018bb0: 7365 2054 7970 6545 7272 6f72 2822 606d  se TypeError("`m
+00018bc0: 6f64 656c 6020 6d75 7374 2062 6520 6120  odel` must be a 
+00018bd0: 696e 7465 6765 722e 2229 0a0a 2020 2020  integer.")..    
+00018be0: 2320 436f 6e76 6572 7420 7479 7065 730a  # Convert types.
+00018bf0: 2020 2020 6966 2074 7970 6528 7665 7274      if type(vert
+00018c00: 6963 6573 2920 3d3d 206c 6973 743a 0a20  ices) == list:. 
+00018c10: 2020 2020 2020 2076 6572 7469 6365 7320         vertices 
+00018c20: 3d20 6e75 6d70 792e 6173 6172 7261 7928  = numpy.asarray(
+00018c30: 7665 7274 6963 6573 290a 2020 2020 6966  vertices).    if
+00018c40: 2074 7970 6528 7374 6570 2920 3d3d 2069   type(step) == i
+00018c50: 6e74 3a0a 2020 2020 2020 2020 7374 6570  nt:.        step
+00018c60: 203d 2066 6c6f 6174 2873 7465 7029 0a0a   = float(step)..
+00018c70: 2020 2020 2320 436f 6e76 6572 7420 6e75      # Convert nu
+00018c80: 6d70 792e 6e64 6172 7261 7920 6461 7461  mpy.ndarray data
+00018c90: 2074 7970 6573 0a20 2020 2076 6572 7469   types.    verti
+00018ca0: 6365 7320 3d20 7665 7274 6963 6573 2e61  ces = vertices.a
+00018cb0: 7374 7970 6528 2266 6c6f 6174 3634 2229  stype("float64")
+00018cc0: 2069 6620 7665 7274 6963 6573 2e64 7479   if vertices.dty
+00018cd0: 7065 2021 3d20 2266 6c6f 6174 3634 2220  pe != "float64" 
+00018ce0: 656c 7365 2076 6572 7469 6365 730a 2020  else vertices.  
+00018cf0: 2020 6966 2042 2069 7320 6e6f 7420 4e6f    if B is not No
+00018d00: 6e65 3a0a 2020 2020 2020 2020 4220 3d20  ne:.        B = 
+00018d10: 422e 6173 7479 7065 2822 666c 6f61 7436  B.astype("float6
+00018d20: 3422 2920 6966 2042 2e64 7479 7065 2021  4") if B.dtype !
+00018d30: 3d20 2266 6c6f 6174 3634 2220 656c 7365  = "float64" else
+00018d40: 2042 0a20 2020 2069 6620 7363 616c 6573   B.    if scales
+00018d50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00018d60: 2020 2020 2020 7363 616c 6573 203d 2073        scales = s
+00018d70: 6361 6c65 732e 6173 7479 7065 2822 666c  cales.astype("fl
+00018d80: 6f61 7436 3422 2920 6966 2073 6361 6c65  oat64") if scale
+00018d90: 732e 6474 7970 6520 213d 2022 666c 6f61  s.dtype != "floa
+00018da0: 7436 3422 2065 6c73 6520 7363 616c 6573  t64" else scales
+00018db0: 0a0a 2020 2020 2320 4765 7420 7369 6e63  ..    # Get sinc
+00018dc0: 6f73 3a20 7369 6e65 2061 6e64 2063 6f73  os: sine and cos
+00018dd0: 7369 6e65 206f 6620 7468 6520 6772 6964  sine of the grid
+00018de0: 2072 6f74 6174 696f 6e20 616e 676c 6573   rotation angles
+00018df0: 2028 7369 6e61 2c20 636f 7361 2c20 7369   (sina, cosa, si
+00018e00: 6e62 2c20 636f 7362 290a 2020 2020 7369  nb, cosb).    si
+00018e10: 6e63 6f73 203d 205f 6765 745f 7369 6e63  ncos = _get_sinc
+00018e20: 6f73 2876 6572 7469 6365 7329 0a0a 2020  os(vertices)..  
+00018e30: 2020 2320 556e 7061 636b 2076 6572 7469    # Unpack verti
+00018e40: 6365 730a 2020 2020 5031 2c20 5032 2c20  ces.    P1, P2, 
+00018e50: 5033 2c20 5034 203d 2076 6572 7469 6365  P3, P4 = vertice
+00018e60: 730a 0a20 2020 2023 2049 6620 7375 7266  s..    # If surf
+00018e70: 6163 6520 6973 204e 6f6e 652c 2063 7265  ace is None, cre
+00018e80: 6174 6520 616e 2065 6d70 7479 2067 7269  ate an empty gri
+00018e90: 640a 2020 2020 6966 2063 6176 6974 6965  d.    if cavitie
+00018ea0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00018eb0: 2020 2020 2020 2069 6620 7375 7266 6163         if surfac
+00018ec0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00018ed0: 2020 2020 2020 2073 7572 6661 6365 203d         surface =
+00018ee0: 206e 756d 7079 2e7a 6572 6f73 2863 6176   numpy.zeros(cav
+00018ef0: 6974 6965 732e 7368 6170 652c 2064 7479  ities.shape, dty
+00018f00: 7065 3d22 696e 7433 3222 290a 2020 2020  pe="int32").    
+00018f10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00018f20: 2020 2020 2020 7375 7266 6163 6520 3d20        surface = 
+00018f30: 7375 7266 6163 652e 6173 7479 7065 2822  surface.astype("
+00018f40: 696e 7433 3222 2920 6966 2073 7572 6661  int32") if surfa
+00018f50: 6365 2e64 7479 7065 2021 3d20 2269 6e74  ce.dtype != "int
+00018f60: 3332 2220 656c 7365 2073 7572 6661 6365  32" else surface
+00018f70: 0a0a 2020 2020 2320 5365 6c65 6374 2063  ..    # Select c
+00018f80: 6176 6974 6965 730a 2020 2020 6966 2073  avities.    if s
+00018f90: 656c 6563 7469 6f6e 2069 7320 6e6f 7420  election is not 
+00018fa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7375  None:.        su
+00018fb0: 7266 6163 6520 3d20 5f73 656c 6563 745f  rface = _select_
+00018fc0: 6361 7669 7469 6573 2873 7572 6661 6365  cavities(surface
+00018fd0: 2c20 7365 6c65 6374 696f 6e29 0a20 2020  , selection).   
+00018fe0: 2020 2020 2069 6620 6361 7669 7469 6573       if cavities
+00018ff0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019000: 2020 2020 2020 2020 2020 6361 7669 7469            caviti
+00019010: 6573 203d 205f 7365 6c65 6374 5f63 6176  es = _select_cav
+00019020: 6974 6965 7328 6361 7669 7469 6573 2c20  ities(cavities, 
+00019030: 7365 6c65 6374 696f 6e29 0a0a 2020 2020  selection)..    
+00019040: 6966 2063 6176 6974 6965 7320 6973 204e  if cavities is N
+00019050: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+00019060: 7375 7266 6163 6520 6973 204e 6f6e 653a  surface is None:
+00019070: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00019080: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
+00019090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000190a0: 2066 2255 7365 7220 6d75 7374 2064 6566   f"User must def
+000190b0: 696e 6520 6073 7572 6661 6365 6020 7768  ine `surface` wh
+000190c0: 656e 206e 6f74 2064 6566 696e 696e 6720  en not defining 
+000190d0: 6063 6176 6974 6965 7360 2e22 0a20 2020  `cavities`.".   
+000190e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000190f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00019100: 2020 2020 2023 2047 6574 206e 756d 6265       # Get numbe
+00019110: 7220 6f66 2063 6176 6974 6965 730a 2020  r of cavities.  
+00019120: 2020 2020 2020 2020 2020 6e63 6176 203d            ncav =
+00019130: 2069 6e74 2873 7572 6661 6365 2e6d 6178   int(surface.max
+00019140: 2829 202d 2031 290a 0a20 2020 2020 2020  () - 1)..       
+00019150: 2020 2020 2023 2045 7870 6f72 7420 6879       # Export hy
+00019160: 6472 6f70 6174 6879 0a20 2020 2020 2020  dropathy.       
+00019170: 2020 2020 205f 6578 706f 7274 5f62 280a       _export_b(.
+00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019190: 6f75 7470 7574 5f68 7964 726f 7061 7468  output_hydropath
+000191a0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+000191b0: 2020 2073 7572 6661 6365 2c0a 2020 2020     surface,.    
+000191c0: 2020 2020 2020 2020 2020 2020 7375 7266              surf
+000191d0: 6163 652c 0a20 2020 2020 2020 2020 2020  ace,.           
+000191e0: 2020 2020 2073 6361 6c65 732c 0a20 2020       scales,.   
+000191f0: 2020 2020 2020 2020 2020 2020 2050 312c               P1,
+00019200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019210: 2073 696e 636f 732c 0a20 2020 2020 2020   sincos,.       
+00019220: 2020 2020 2020 2020 2073 7465 702c 0a20           step,. 
+00019230: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00019240: 6361 762c 0a20 2020 2020 2020 2020 2020  cav,.           
+00019250: 2020 2020 206e 7468 7265 6164 732c 0a20       nthreads,. 
+00019260: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019270: 7070 656e 642c 0a20 2020 2020 2020 2020  ppend,.         
+00019280: 2020 2020 2020 206d 6f64 656c 2c0a 2020         model,.  
+00019290: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000192a0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+000192b0: 4368 6563 6b20 616e 6420 636f 6e76 6572  Check and conver
+000192c0: 7420 6361 7669 7469 6573 2064 7479 7065  t cavities dtype
+000192d0: 0a20 2020 2020 2020 2063 6176 6974 6965  .        cavitie
+000192e0: 7320 3d20 6361 7669 7469 6573 2e61 7374  s = cavities.ast
+000192f0: 7970 6528 2269 6e74 3332 2229 2069 6620  ype("int32") if 
+00019300: 6361 7669 7469 6573 2e64 7479 7065 2021  cavities.dtype !
+00019310: 3d20 2269 6e74 3332 2220 656c 7365 2063  = "int32" else c
+00019320: 6176 6974 6965 730a 0a20 2020 2020 2020  avities..       
+00019330: 2023 2047 6574 206e 756d 6265 7220 6f66   # Get number of
+00019340: 2063 6176 6974 6965 730a 2020 2020 2020   cavities.      
+00019350: 2020 6e63 6176 203d 2069 6e74 2863 6176    ncav = int(cav
+00019360: 6974 6965 732e 6d61 7828 2920 2d20 3129  ities.max() - 1)
+00019370: 0a0a 2020 2020 2020 2020 2320 4578 706f  ..        # Expo
+00019380: 7274 2063 6176 6974 6965 730a 2020 2020  rt cavities.    
+00019390: 2020 2020 6966 2042 2069 7320 4e6f 6e65      if B is None
+000193a0: 3a0a 2020 2020 2020 2020 2020 2020 5f65  :.            _e
+000193b0: 7870 6f72 7428 0a20 2020 2020 2020 2020  xport(.         
+000193c0: 2020 2020 2020 2066 6e2c 2063 6176 6974         fn, cavit
+000193d0: 6965 732c 2073 7572 6661 6365 2c20 5031  ies, surface, P1
+000193e0: 2c20 7369 6e63 6f73 2c20 7374 6570 2c20  , sincos, step, 
+000193f0: 6e63 6176 2c20 6e74 6872 6561 6473 2c20  ncav, nthreads, 
+00019400: 6170 7065 6e64 2c20 6d6f 6465 6c0a 2020  append, model.  
+00019410: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00019420: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00019430: 2020 2020 2020 5f65 7870 6f72 745f 6228        _export_b(
+00019440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019450: 2066 6e2c 0a20 2020 2020 2020 2020 2020   fn,.           
+00019460: 2020 2020 2063 6176 6974 6965 732c 0a20       cavities,. 
+00019470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019480: 7572 6661 6365 2c0a 2020 2020 2020 2020  urface,.        
+00019490: 2020 2020 2020 2020 422c 0a20 2020 2020          B,.     
+000194a0: 2020 2020 2020 2020 2020 2050 312c 0a20             P1,. 
+000194b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000194c0: 696e 636f 732c 0a20 2020 2020 2020 2020  incos,.         
+000194d0: 2020 2020 2020 2073 7465 702c 0a20 2020         step,.   
+000194e0: 2020 2020 2020 2020 2020 2020 206e 6361               nca
+000194f0: 762c 0a20 2020 2020 2020 2020 2020 2020  v,.             
+00019500: 2020 206e 7468 7265 6164 732c 0a20 2020     nthreads,.   
+00019510: 2020 2020 2020 2020 2020 2020 2061 7070               app
+00019520: 656e 642c 0a20 2020 2020 2020 2020 2020  end,.           
+00019530: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
+00019540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019550: 2020 2023 2045 7870 6f72 7420 6879 6472     # Export hydr
+00019560: 6f70 6174 6879 2073 7572 6661 6365 2070  opathy surface p
+00019570: 6f69 6e74 730a 2020 2020 2020 2020 6966  oints.        if
+00019580: 2073 6361 6c65 7320 6973 204e 6f6e 653a   scales is None:
+00019590: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+000195a0: 730a 2020 2020 2020 2020 656c 7365 3a0a  s.        else:.
+000195b0: 2020 2020 2020 2020 2020 2020 5f65 7870              _exp
+000195c0: 6f72 745f 6228 0a20 2020 2020 2020 2020  ort_b(.         
+000195d0: 2020 2020 2020 206f 7574 7075 745f 6879         output_hy
+000195e0: 6472 6f70 6174 6879 2c0a 2020 2020 2020  dropathy,.      
+000195f0: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
+00019600: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00019610: 2020 2073 7572 6661 6365 2c0a 2020 2020     surface,.    
+00019620: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00019630: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00019640: 2020 2020 5031 2c0a 2020 2020 2020 2020      P1,.        
+00019650: 2020 2020 2020 2020 7369 6e63 6f73 2c0a          sincos,.
+00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019670: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+00019680: 2020 2020 2020 6e63 6176 2c0a 2020 2020        ncav,.    
+00019690: 2020 2020 2020 2020 2020 2020 6e74 6872              nthr
+000196a0: 6561 6473 2c0a 2020 2020 2020 2020 2020  eads,.          
+000196b0: 2020 2020 2020 6170 7065 6e64 2c0a 2020        append,.  
+000196c0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+000196d0: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
+000196e0: 2029 0a0a 0a64 6566 2065 7870 6f72 745f   )...def export_
+000196f0: 6f70 656e 696e 6773 280a 2020 2020 666e  openings(.    fn
+00019700: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+00019710: 686c 6962 2e50 6174 685d 2c0a 2020 2020  hlib.Path],.    
+00019720: 6f70 656e 696e 6773 3a20 6e75 6d70 792e  openings: numpy.
+00019730: 6e64 6172 7261 792c 0a20 2020 2076 6572  ndarray,.    ver
+00019740: 7469 6365 733a 2055 6e69 6f6e 5b6e 756d  tices: Union[num
+00019750: 7079 2e6e 6461 7272 6179 2c20 4c69 7374  py.ndarray, List
+00019760: 5b4c 6973 745b 666c 6f61 745d 5d5d 2c0a  [List[float]]],.
+00019770: 2020 2020 7374 6570 3a20 556e 696f 6e5b      step: Union[
+00019780: 666c 6f61 742c 2069 6e74 5d20 3d20 302e  float, int] = 0.
+00019790: 362c 0a20 2020 2073 656c 6563 7469 6f6e  6,.    selection
+000197a0: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+000197b0: 5b4c 6973 745b 696e 745d 2c20 4c69 7374  [List[int], List
+000197c0: 5b73 7472 5d5d 5d20 3d20 4e6f 6e65 2c0a  [str]]] = None,.
+000197d0: 2020 2020 6e74 6872 6561 6473 3a20 4f70      nthreads: Op
+000197e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000197f0: 6e65 2c0a 2020 2020 6170 7065 6e64 3a20  ne,.    append: 
+00019800: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00019810: 2020 6d6f 6465 6c3a 2069 6e74 203d 2030    model: int = 0
+00019820: 2c0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ,.) -> None:.   
+00019830: 2022 2222 4578 706f 7274 206f 7065 6e69   """Export openi
+00019840: 6e67 2070 6f69 6e74 7320 2848 2920 746f  ng points (H) to
+00019850: 2061 2050 4442 2d66 6f72 6d61 7474 6564   a PDB-formatted
+00019860: 2066 696c 652e 0a0a 2020 2020 5061 7261   file...    Para
+00019870: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00019880: 2d2d 2d2d 2d0a 2020 2020 666e 203a 2055  -----.    fn : U
+00019890: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
+000198a0: 622e 5061 7468 5d0a 2020 2020 2020 2020  b.Path].        
+000198b0: 4120 7061 7468 2074 6f20 5044 4220 6669  A path to PDB fi
+000198c0: 6c65 2066 6f72 2077 7269 7469 6e67 206f  le for writing o
+000198d0: 7065 6e69 6e67 732e 0a20 2020 206f 7065  penings..    ope
+000198e0: 6e69 6e67 7320 3a20 6e75 6d70 792e 6e64  nings : numpy.nd
+000198f0: 6172 7261 790a 2020 2020 2020 2020 4f70  array.        Op
+00019900: 656e 696e 6773 2070 6f69 6e74 7320 696e  enings points in
+00019910: 2074 6865 2033 4420 6772 6964 2028 6f70   the 3D grid (op
+00019920: 656e 696e 6773 5b6e 785d 5b6e 795d 5b6e  enings[nx][ny][n
+00019930: 7a5d 292e 0a20 2020 2020 2020 204f 7065  z])..        Ope
+00019940: 6e69 6e67 7320 6172 7261 7920 6861 7320  nings array has 
+00019950: 696e 7465 6765 7220 6c61 6265 6c73 2069  integer labels i
+00019960: 6e20 6561 6368 2070 6f73 6974 696f 6e2c  n each position,
+00019970: 2074 6861 7420 6172 653a 0a0a 2020 2020   that are:..    
+00019980: 2020 2020 2020 2020 2a20 2d31 3a20 6275          * -1: bu
+00019990: 6c6b 2070 6f69 6e74 733b 0a0a 2020 2020  lk points;..    
+000199a0: 2020 2020 2020 2020 2a20 303a 2063 6176          * 0: cav
+000199b0: 6974 7920 6f72 2062 696f 6d6f 6c65 6375  ity or biomolecu
+000199c0: 6c65 2070 6f69 6e74 733b 0a0a 2020 2020  le points;..    
+000199d0: 2020 2020 2020 2020 2a20 313a 2065 6d70          * 1: emp
+000199e0: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
+000199f0: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+00019a00: 3e3d 323a 204f 7065 6e69 6e67 2070 6f69  >=2: Opening poi
+00019a10: 6e74 732e 0a0a 2020 2020 2020 2020 5468  nts...        Th
+00019a20: 6520 656d 7074 7920 7370 6163 6520 706f  e empty space po
+00019a30: 696e 7473 2061 7265 2072 6567 696f 6e73  ints are regions
+00019a40: 2074 6861 7420 646f 206e 6f74 206d 6565   that do not mee
+00019a50: 7420 7468 6520 6368 6f73 656e 0a20 2020  t the chosen.   
+00019a60: 2020 2020 206f 7065 6e69 6e67 7320 6375       openings cu
+00019a70: 746f 6666 2074 6f20 6265 2063 6f6e 7369  toff to be consi
+00019a80: 6465 7265 6420 616e 206f 7065 6e69 6e67  dered an opening
+00019a90: 2e0a 2020 2020 7665 7274 6963 6573 203a  ..    vertices :
+00019aa0: 2055 6e69 6f6e 5b6e 756d 7079 2e6e 6461   Union[numpy.nda
+00019ab0: 7272 6179 2c20 4c69 7374 5b4c 6973 745b  rray, List[List[
+00019ac0: 666c 6f61 745d 5d5d 0a20 2020 2020 2020  float]]].       
+00019ad0: 2041 206e 756d 7079 2e6e 6461 7272 6179   A numpy.ndarray
+00019ae0: 206f 7220 6120 6c69 7374 2077 6974 6820   or a list with 
+00019af0: 7879 7a20 7665 7274 6963 6573 2063 6f6f  xyz vertices coo
+00019b00: 7264 696e 6174 6573 2028 6f72 6967 696e  rdinates (origin
+00019b10: 2c0a 2020 2020 2020 2020 582d 6178 6973  ,.        X-axis
+00019b20: 2c20 592d 6178 6973 2c20 5a2d 6178 6973  , Y-axis, Z-axis
+00019b30: 292e 0a20 2020 2073 7465 7020 3a20 556e  )..    step : Un
+00019b40: 696f 6e5b 666c 6f61 742c 2069 6e74 5d2c  ion[float, int],
+00019b50: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00019b60: 2020 4772 6964 2073 7061 6369 6e67 2028    Grid spacing (
+00019b70: 4129 2c20 6279 2064 6566 6175 6c74 2030  A), by default 0
+00019b80: 2e36 2e0a 2020 2020 7365 6c65 6374 696f  .6..    selectio
+00019b90: 6e20 3a20 556e 696f 6e5b 4c69 7374 5b69  n : Union[List[i
+00019ba0: 6e74 5d2c 204c 6973 745b 7374 725d 5d2c  nt], List[str]],
+00019bb0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00019bc0: 2020 4120 6c69 7374 206f 6620 696e 7465    A list of inte
+00019bd0: 6765 7220 6c61 6265 6c73 206f 7220 6120  ger labels or a 
+00019be0: 6c69 7374 206f 6620 6f70 656e 696e 6720  list of opening 
+00019bf0: 6e61 6d65 7320 746f 2062 6520 7365 6c65  names to be sele
+00019c00: 6374 6564 2c20 6279 2064 6566 6175 6c74  cted, by default
+00019c10: 204e 6f6e 652e 0a20 2020 206e 7468 7265   None..    nthre
+00019c20: 6164 7320 3a20 696e 742c 206f 7074 696f  ads : int, optio
+00019c30: 6e61 6c0a 2020 2020 2020 2020 4e75 6d62  nal.        Numb
+00019c40: 6572 206f 6620 7468 7265 6164 732c 2062  er of threads, b
+00019c50: 7920 6465 6661 756c 7420 4e6f 6e65 2e20  y default None. 
+00019c60: 4966 204e 6f6e 652c 2074 6865 206e 756d  If None, the num
+00019c70: 6265 7220 6f66 2074 6872 6561 6473 2069  ber of threads i
+00019c80: 730a 2020 2020 2020 2020 606f 732e 6370  s.        `os.cp
+00019c90: 755f 636f 756e 7428 2920 2d20 3160 2e0a  u_count() - 1`..
+00019ca0: 2020 2020 6170 7065 6e64 203a 2062 6f6f      append : boo
+00019cb0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
+00019cc0: 2020 2020 5768 6574 6865 7220 746f 2061      Whether to a
+00019cd0: 7070 656e 6420 6f70 656e 696e 6773 2074  ppend openings t
+00019ce0: 6f20 7468 6520 5044 4220 6669 6c65 2c20  o the PDB file, 
+00019cf0: 6279 2064 6566 6175 6c74 2046 616c 7365  by default False
+00019d00: 2e0a 2020 2020 6d6f 6465 6c20 3a20 696e  ..    model : in
+00019d10: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+00019d20: 2020 2020 4d6f 6465 6c20 6e75 6d62 6572      Model number
+00019d30: 2c20 6279 2064 6566 6175 6c74 2030 2e0a  , by default 0..
+00019d40: 0a20 2020 2052 6169 7365 730a 2020 2020  .    Raises.    
+00019d50: 2d2d 2d2d 2d2d 0a20 2020 2054 7970 6545  ------.    TypeE
+00019d60: 7272 6f72 0a20 2020 2020 2020 2060 6f70  rror.        `op
+00019d70: 656e 696e 6773 6020 6d75 7374 2062 6520  enings` must be 
+00019d80: 6120 6e75 6d70 792e 6e64 6172 7261 792e  a numpy.ndarray.
+00019d90: 0a20 2020 2056 616c 7565 4572 726f 720a  .    ValueError.
+00019da0: 2020 2020 2020 2020 606f 7065 6e69 6e67          `opening
+00019db0: 7360 2068 6173 2074 6865 2069 6e63 6f72  s` has the incor
+00019dc0: 7265 6374 2073 6861 7065 2e20 4974 206d  rect shape. It m
+00019dd0: 7573 7420 6265 2028 6e78 2c20 6e79 2c20  ust be (nx, ny, 
+00019de0: 6e7a 292e 0a20 2020 2054 7970 6545 7272  nz)..    TypeErr
+00019df0: 6f72 0a20 2020 2020 2020 2060 7665 7274  or.        `vert
+00019e00: 6963 6573 6020 6d75 7374 2062 6520 6120  ices` must be a 
+00019e10: 6c69 7374 206f 7220 6120 6e75 6d70 792e  list or a numpy.
+00019e20: 6e64 6172 7261 792e 0a20 2020 2056 616c  ndarray..    Val
+00019e30: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
+00019e40: 6076 6572 7469 6365 7360 2068 6173 2069  `vertices` has i
+00019e50: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
+00019e60: 4974 206d 7573 7420 6265 2028 342c 2033  It must be (4, 3
+00019e70: 292e 0a20 2020 2054 7970 6545 7272 6f72  )..    TypeError
+00019e80: 0a20 2020 2020 2020 2060 7374 6570 6020  .        `step` 
+00019e90: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+00019ea0: 7665 2072 6561 6c20 6e75 6d62 6572 2e0a  ve real number..
+00019eb0: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
+00019ec0: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
+00019ed0: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+00019ee0: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
+00019ef0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
+00019f00: 2020 2020 6073 656c 6563 7469 6f6e 6020      `selection` 
+00019f10: 6d75 7374 2062 6520 6120 6c69 7374 206f  must be a list o
+00019f20: 6620 7374 7269 6e67 7320 286f 7065 6e69  f strings (openi
+00019f30: 6e67 206e 616d 6573 2920 6f72 2069 6e74  ng names) or int
+00019f40: 6567 6572 7320 286f 7065 6e69 6e67 206c  egers (opening l
+00019f50: 6162 656c 7329 2e0a 2020 2020 5661 6c75  abels)..    Valu
+00019f60: 6545 7272 6f72 0a20 2020 2020 2020 2049  eError.        I
+00019f70: 6e76 616c 6964 2060 7365 6c65 6374 696f  nvalid `selectio
+00019f80: 6e60 3a20 7b73 656c 6563 7469 6f6e 7d2e  n`: {selection}.
+00019f90: 0a20 2020 2054 7970 6545 7272 6f72 0a20  .    TypeError. 
+00019fa0: 2020 2020 2020 2060 6e74 6872 6561 6473         `nthreads
+00019fb0: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+00019fc0: 7469 7665 2069 6e74 6567 6572 2e0a 2020  tive integer..  
+00019fd0: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+00019fe0: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
+00019ff0: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+0001a000: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
+0001a010: 5479 7065 4572 726f 720a 2020 2020 2020  TypeError.      
+0001a020: 2020 6061 7070 656e 6460 206d 7573 7420    `append` must 
+0001a030: 6265 2061 2062 6f6f 6c65 616e 2e0a 2020  be a boolean..  
+0001a040: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
+0001a050: 2020 2020 606d 6f64 656c 6020 6d75 7374      `model` must
+0001a060: 2062 6520 6120 696e 7465 6765 722e 0a20   be a integer.. 
+0001a070: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
+0001a080: 2020 2020 2060 666e 6020 6d75 7374 2062       `fn` must b
+0001a090: 6520 6120 7374 7269 6e67 206f 7220 7061  e a string or pa
+0001a0a0: 7468 6c69 622e 5061 7468 2e0a 0a20 2020  thlib.Path...   
+0001a0b0: 204e 6f74 650a 2020 2020 2d2d 2d2d 0a20   Note.    ----. 
+0001a0c0: 2020 2054 6865 206f 7065 6e69 6e67 206e     The opening n
+0001a0d0: 6f6d 656e 636c 6174 7572 6520 6973 2062  omenclature is b
+0001a0e0: 6173 6564 206f 6e20 7468 6520 696e 7465  ased on the inte
+0001a0f0: 6765 7220 6c61 6265 6c2e 2054 6865 206f  ger label. The o
+0001a100: 7065 6e69 6e67 206d 6172 6b65 640a 2020  pening marked.  
+0001a110: 2020 7769 7468 2032 2c20 7468 6520 6669    with 2, the fi
+0001a120: 7273 7420 696e 7465 6765 7220 636f 7272  rst integer corr
+0001a130: 6573 706f 6e64 696e 6720 746f 2061 206f  esponding to a o
+0001a140: 7065 6e69 6e67 2c20 6973 204f 4141 2c20  pening, is OAA, 
+0001a150: 7468 6520 6f70 656e 696e 670a 2020 2020  the opening.    
+0001a160: 6d61 726b 6564 2077 6974 6820 3320 6973  marked with 3 is
+0001a170: 204f 4142 2c20 7468 6520 6f70 656e 696e   OAB, the openin
+0001a180: 6720 6d61 726b 6564 2077 6974 6820 3420  g marked with 4 
+0001a190: 6973 204f 4143 2061 6e64 2073 6f20 6f6e  is OAC and so on
+0001a1a0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f0a  ...    See Also.
+0001a1b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001a1c0: 2065 7870 6f72 740a 2020 2020 6465 7465   export.    dete
+0001a1d0: 6374 0a20 2020 2064 6570 7468 730a 2020  ct.    depths.  
+0001a1e0: 2020 6f70 656e 696e 6773 0a0a 2020 2020    openings..    
+0001a1f0: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
+0001a200: 2d2d 2d0a 2020 2020 5769 7468 2074 6865  ---.    With the
+0001a210: 206f 7065 6e69 6e67 2070 6f69 6e74 7320   opening points 
+0001a220: 6964 656e 7469 6669 6564 2077 6974 6820  identified with 
+0001a230: 6060 6f70 656e 696e 6773 6060 2c20 7765  ``openings``, we
+0001a240: 2063 616e 2065 7870 6f72 7420 7468 656d   can export them
+0001a250: 2074 6f20 6120 5044 422d 666f 726d 6174   to a PDB-format
+0001a260: 7465 6420 6669 6c65 3a0a 0a20 2020 203e  ted file:..    >
+0001a270: 3e3e 2066 726f 6d20 7079 4b56 4669 6e64  >> from pyKVFind
+0001a280: 6572 2069 6d70 6f72 7420 6578 706f 7274  er import export
+0001a290: 5f6f 7065 6e69 6e67 730a 2020 2020 3e3e  _openings.    >>
+0001a2a0: 3e20 6578 706f 7274 5f6f 7065 6e69 6e67  > export_opening
+0001a2b0: 7328 276f 7065 6e69 6e67 732e 7064 6227  s('openings.pdb'
+0001a2c0: 2c20 6f70 656e 696e 6773 2c20 7665 7274  , openings, vert
+0001a2d0: 6963 6573 290a 2020 2020 2222 220a 2020  ices).    """.  
+0001a2e0: 2020 6672 6f6d 205f 7079 4b56 4669 6e64    from _pyKVFind
+0001a2f0: 6572 2069 6d70 6f72 7420 5f65 7870 6f72  er import _expor
+0001a300: 745f 6f70 656e 696e 6773 0a0a 2020 2020  t_openings..    
+0001a310: 2320 4368 6563 6b20 6172 6775 6d65 6e74  # Check argument
+0001a320: 730a 2020 2020 6966 2074 7970 6528 6f70  s.    if type(op
+0001a330: 656e 696e 6773 2920 6e6f 7420 696e 205b  enings) not in [
+0001a340: 6e75 6d70 792e 6e64 6172 7261 795d 3a0a  numpy.ndarray]:.
+0001a350: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0001a360: 7065 4572 726f 7228 2260 6f70 656e 696e  peError("`openin
+0001a370: 6773 6020 6d75 7374 2062 6520 6120 6e75  gs` must be a nu
+0001a380: 6d70 792e 6e64 6172 7261 792e 2229 0a20  mpy.ndarray."). 
+0001a390: 2020 2065 6c69 6620 6c65 6e28 6f70 656e     elif len(open
+0001a3a0: 696e 6773 2e73 6861 7065 2920 213d 2033  ings.shape) != 3
+0001a3b0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+0001a3c0: 5661 6c75 6545 7272 6f72 2822 606f 7065  ValueError("`ope
+0001a3d0: 6e69 6e67 7360 2068 6173 2074 6865 2069  nings` has the i
+0001a3e0: 6e63 6f72 7265 6374 2073 6861 7065 2e20  ncorrect shape. 
+0001a3f0: 4974 206d 7573 7420 6265 2028 6e78 2c20  It must be (nx, 
+0001a400: 6e79 2c20 6e7a 292e 2229 0a20 2020 2069  ny, nz).").    i
+0001a410: 6620 7479 7065 2876 6572 7469 6365 7329  f type(vertices)
+0001a420: 206e 6f74 2069 6e20 5b6e 756d 7079 2e6e   not in [numpy.n
+0001a430: 6461 7272 6179 2c20 6c69 7374 5d3a 0a20  darray, list]:. 
+0001a440: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0001a450: 6545 7272 6f72 2822 6076 6572 7469 6365  eError("`vertice
+0001a460: 7360 206d 7573 7420 6265 2061 206c 6973  s` must be a lis
+0001a470: 7420 6f72 2061 206e 756d 7079 2e6e 6461  t or a numpy.nda
+0001a480: 7272 6179 2e22 290a 2020 2020 656c 6966  rray.").    elif
+0001a490: 206e 756d 7079 2e61 7361 7272 6179 2876   numpy.asarray(v
+0001a4a0: 6572 7469 6365 7329 2e73 6861 7065 2021  ertices).shape !
+0001a4b0: 3d20 2834 2c20 3329 3a0a 2020 2020 2020  = (4, 3):.      
+0001a4c0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0001a4d0: 6f72 2822 6076 6572 7469 6365 7360 2068  or("`vertices` h
+0001a4e0: 6173 2069 6e63 6f72 7265 6374 2073 6861  as incorrect sha
+0001a4f0: 7065 2e20 4974 206d 7573 7420 6265 2028  pe. It must be (
+0001a500: 342c 2033 292e 2229 0a20 2020 2069 6620  4, 3).").    if 
+0001a510: 7479 7065 2873 7465 7029 206e 6f74 2069  type(step) not i
+0001a520: 6e20 5b66 6c6f 6174 2c20 696e 745d 3a0a  n [float, int]:.
+0001a530: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0001a540: 7065 4572 726f 7228 2260 7374 6570 6020  peError("`step` 
+0001a550: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+0001a560: 7665 2072 6561 6c20 6e75 6d62 6572 2e22  ve real number."
+0001a570: 290a 2020 2020 656c 6966 2073 7465 7020  ).    elif step 
+0001a580: 3c3d 2030 2e30 3a0a 2020 2020 2020 2020  <= 0.0:.        
+0001a590: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0001a5a0: 2822 6073 7465 7060 206d 7573 7420 6265  ("`step` must be
+0001a5b0: 2061 2070 6f73 6974 6976 6520 7265 616c   a positive real
+0001a5c0: 206e 756d 6265 722e 2229 0a20 2020 2069   number.").    i
+0001a5d0: 6620 7365 6c65 6374 696f 6e20 6973 206e  f selection is n
+0001a5e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001a5f0: 2023 2043 6865 636b 2073 656c 6563 7469   # Check selecti
+0001a600: 6f6e 2074 7970 6573 0a20 2020 2020 2020  on types.       
+0001a610: 2069 6620 616c 6c28 6973 696e 7374 616e   if all(isinstan
+0001a620: 6365 2878 2c20 696e 7429 2066 6f72 2078  ce(x, int) for x
+0001a630: 2069 6e20 7365 6c65 6374 696f 6e29 3a0a   in selection):.
+0001a640: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0001a650: 0a20 2020 2020 2020 2065 6c69 6620 616c  .        elif al
+0001a660: 6c28 6973 696e 7374 616e 6365 2878 2c20  l(isinstance(x, 
+0001a670: 7374 7229 2066 6f72 2078 2069 6e20 7365  str) for x in se
+0001a680: 6c65 6374 696f 6e29 3a0a 2020 2020 2020  lection):.      
+0001a690: 2020 2020 2020 7365 6c65 6374 696f 6e20        selection 
+0001a6a0: 3d20 5b5f 6765 745f 6f70 656e 696e 675f  = [_get_opening_
+0001a6b0: 6c61 6265 6c28 7365 6c65 2920 666f 7220  label(sele) for 
+0001a6c0: 7365 6c65 2069 6e20 7365 6c65 6374 696f  sele in selectio
+0001a6d0: 6e5d 0a20 2020 2020 2020 2065 6c73 653a  n].        else:
+0001a6e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001a6f0: 7365 2054 7970 6545 7272 6f72 280a 2020  se TypeError(.  
+0001a700: 2020 2020 2020 2020 2020 2020 2020 2260                "`
+0001a710: 7365 6c65 6374 696f 6e60 206d 7573 7420  selection` must 
+0001a720: 6265 2061 206c 6973 7420 6f66 2073 7472  be a list of str
+0001a730: 696e 6773 2028 6361 7669 7479 206e 616d  ings (cavity nam
+0001a740: 6573 2920 6f72 2069 6e74 6567 6572 7320  es) or integers 
+0001a750: 2863 6176 6974 7920 6c61 6265 6c73 292e  (cavity labels).
+0001a760: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0001a770: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+0001a780: 6966 2073 656c 6563 7469 6f6e 2069 6e63  if selection inc
+0001a790: 6c75 6465 7320 7661 6c69 6420 6361 7669  ludes valid cavi
+0001a7a0: 7479 206c 6162 656c 730a 2020 2020 2020  ty labels.      
+0001a7b0: 2020 6966 2061 6e79 2878 203c 2032 2066    if any(x < 2 f
+0001a7c0: 6f72 2078 2069 6e20 7365 6c65 6374 696f  or x in selectio
+0001a7d0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+0001a7e0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0001a7f0: 2866 2249 6e76 616c 6964 2060 7365 6c65  (f"Invalid `sele
+0001a800: 6374 696f 6e60 3a20 7b73 656c 6563 7469  ction`: {selecti
+0001a810: 6f6e 7d2e 2229 0a20 2020 2069 6620 6e74  on}.").    if nt
+0001a820: 6872 6561 6473 2069 7320 4e6f 6e65 3a0a  hreads is None:.
+0001a830: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
+0001a840: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+0001a850: 2920 2d20 310a 2020 2020 656c 7365 3a0a  ) - 1.    else:.
+0001a860: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+0001a870: 6e74 6872 6561 6473 2920 6e6f 7420 696e  nthreads) not in
+0001a880: 205b 696e 745d 3a0a 2020 2020 2020 2020   [int]:.        
+0001a890: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0001a8a0: 726f 7228 2260 6e74 6872 6561 6473 6020  ror("`nthreads` 
+0001a8b0: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
+0001a8c0: 7665 2069 6e74 6567 6572 2e22 290a 2020  ve integer.").  
+0001a8d0: 2020 2020 2020 656c 6966 206e 7468 7265        elif nthre
+0001a8e0: 6164 7320 3c3d 2030 3a0a 2020 2020 2020  ads <= 0:.      
+0001a8f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0001a900: 6545 7272 6f72 2822 606e 7468 7265 6164  eError("`nthread
+0001a910: 7360 206d 7573 7420 6265 2061 2070 6f73  s` must be a pos
+0001a920: 6974 6976 6520 696e 7465 6765 722e 2229  itive integer.")
+0001a930: 0a20 2020 2069 6620 7479 7065 2861 7070  .    if type(app
+0001a940: 656e 6429 206e 6f74 2069 6e20 5b62 6f6f  end) not in [boo
+0001a950: 6c5d 3a0a 2020 2020 2020 2020 7261 6973  l]:.        rais
+0001a960: 6520 5479 7065 4572 726f 7228 2260 6170  e TypeError("`ap
+0001a970: 7065 6e64 6020 6d75 7374 2062 6520 6120  pend` must be a 
+0001a980: 626f 6f6c 6561 6e2e 2229 0a20 2020 2069  boolean.").    i
+0001a990: 6620 7479 7065 286d 6f64 656c 2920 6e6f  f type(model) no
+0001a9a0: 7420 696e 205b 696e 745d 3a0a 2020 2020  t in [int]:.    
+0001a9b0: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0001a9c0: 726f 7228 2260 6d6f 6465 6c60 206d 7573  ror("`model` mus
+0001a9d0: 7420 6265 2061 2069 6e74 6567 6572 2e22  t be a integer."
+0001a9e0: 290a 0a20 2020 2023 2043 6f6e 7665 7274  )..    # Convert
+0001a9f0: 2074 7970 6573 0a20 2020 2069 6620 7479   types.    if ty
+0001aa00: 7065 2876 6572 7469 6365 7329 203d 3d20  pe(vertices) == 
+0001aa10: 6c69 7374 3a0a 2020 2020 2020 2020 7665  list:.        ve
+0001aa20: 7274 6963 6573 203d 206e 756d 7079 2e61  rtices = numpy.a
+0001aa30: 7361 7272 6179 2876 6572 7469 6365 7329  sarray(vertices)
+0001aa40: 0a20 2020 2069 6620 7479 7065 2873 7465  .    if type(ste
+0001aa50: 7029 203d 3d20 696e 743a 0a20 2020 2020  p) == int:.     
+0001aa60: 2020 2073 7465 7020 3d20 666c 6f61 7428     step = float(
+0001aa70: 7374 6570 290a 0a20 2020 2023 2043 6f6e  step)..    # Con
+0001aa80: 7665 7274 206e 756d 7079 2e6e 6461 7272  vert numpy.ndarr
+0001aa90: 6179 2064 6174 6120 7479 7065 730a 2020  ay data types.  
+0001aaa0: 2020 7665 7274 6963 6573 203d 2076 6572    vertices = ver
+0001aab0: 7469 6365 732e 6173 7479 7065 2822 666c  tices.astype("fl
+0001aac0: 6f61 7436 3422 2920 6966 2076 6572 7469  oat64") if verti
+0001aad0: 6365 732e 6474 7970 6520 213d 2022 666c  ces.dtype != "fl
+0001aae0: 6f61 7436 3422 2065 6c73 6520 7665 7274  oat64" else vert
+0001aaf0: 6963 6573 0a0a 2020 2020 2320 4765 7420  ices..    # Get 
+0001ab00: 7369 6e63 6f73 3a20 7369 6e65 2061 6e64  sincos: sine and
+0001ab10: 2063 6f73 7369 6e65 206f 6620 7468 6520   cossine of the 
+0001ab20: 6772 6964 2072 6f74 6174 696f 6e20 616e  grid rotation an
+0001ab30: 676c 6573 2028 7369 6e61 2c20 636f 7361  gles (sina, cosa
+0001ab40: 2c20 7369 6e62 2c20 636f 7362 290a 2020  , sinb, cosb).  
+0001ab50: 2020 7369 6e63 6f73 203d 205f 6765 745f    sincos = _get_
+0001ab60: 7369 6e63 6f73 2876 6572 7469 6365 7329  sincos(vertices)
+0001ab70: 0a0a 2020 2020 2320 4372 6561 7465 2062  ..    # Create b
+0001ab80: 6173 6520 6469 7265 6374 6f72 6965 7320  ase directories 
+0001ab90: 6f66 2072 6573 756c 7473 0a20 2020 2069  of results.    i
+0001aba0: 6620 666e 2069 7320 6e6f 7420 4e6f 6e65  f fn is not None
+0001abb0: 3a0a 2020 2020 2020 2020 6966 2074 7970  :.        if typ
+0001abc0: 6528 666e 2920 6e6f 7420 696e 205b 7374  e(fn) not in [st
+0001abd0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
+0001abe0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001abf0: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
+0001ac00: 666e 6020 6d75 7374 2062 6520 6120 7374  fn` must be a st
+0001ac10: 7269 6e67 206f 7220 6120 7061 7468 6c69  ring or a pathli
+0001ac20: 622e 5061 7468 2e22 290a 2020 2020 2020  b.Path.").      
+0001ac30: 2020 6f73 2e6d 616b 6564 6972 7328 6f73    os.makedirs(os
+0001ac40: 2e70 6174 682e 6162 7370 6174 6828 6f73  .path.abspath(os
+0001ac50: 2e70 6174 682e 6469 726e 616d 6528 666e  .path.dirname(fn
+0001ac60: 2929 2c20 6578 6973 745f 6f6b 3d54 7275  )), exist_ok=Tru
+0001ac70: 6529 0a0a 2020 2020 2320 556e 7061 636b  e)..    # Unpack
+0001ac80: 2076 6572 7469 6365 730a 2020 2020 5031   vertices.    P1
+0001ac90: 2c20 5f2c 205f 2c20 5f20 3d20 7665 7274  , _, _, _ = vert
+0001aca0: 6963 6573 0a0a 2020 2020 2320 5365 6c65  ices..    # Sele
+0001acb0: 6374 2063 6176 6974 6965 730a 2020 2020  ct cavities.    
+0001acc0: 6966 2073 656c 6563 7469 6f6e 2069 7320  if selection is 
+0001acd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001ace0: 2020 6f70 656e 696e 6773 203d 205f 7365    openings = _se
+0001acf0: 6c65 6374 5f63 6176 6974 6965 7328 6f70  lect_cavities(op
+0001ad00: 656e 696e 6773 2c20 7365 6c65 6374 696f  enings, selectio
+0001ad10: 6e29 0a0a 2020 2020 2320 4765 7420 6e75  n)..    # Get nu
+0001ad20: 6d62 6572 206f 6620 6f70 656e 696e 6773  mber of openings
+0001ad30: 0a20 2020 206e 6f70 656e 696e 6773 203d  .    nopenings =
+0001ad40: 2069 6e74 286f 7065 6e69 6e67 732e 6d61   int(openings.ma
+0001ad50: 7828 2920 2d20 3129 0a0a 2020 2020 2320  x() - 1)..    # 
+0001ad60: 4578 706f 7274 206f 7065 6e69 6e67 730a  Export openings.
+0001ad70: 2020 2020 5f65 7870 6f72 745f 6f70 656e      _export_open
+0001ad80: 696e 6773 2866 6e2c 206f 7065 6e69 6e67  ings(fn, opening
+0001ad90: 732c 2050 312c 2073 696e 636f 732c 2073  s, P1, sincos, s
+0001ada0: 7465 702c 206e 6f70 656e 696e 6773 2c20  tep, nopenings, 
+0001adb0: 6e74 6872 6561 6473 2c20 6170 7065 6e64  nthreads, append
+0001adc0: 2c20 6d6f 6465 6c29 0a                   , model).
```

### Comparing `pyKVFinder-0.5.4/pyKVFinder/main.py` & `pyKVFinder-0.5.5/pyKVFinder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1565,2944 +1565,2945 @@
 000061c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
 000061d0: 204e 616d 6520 6f66 2061 2062 7569 6c74   Name of a built
 000061e0: 2d69 6e20 6879 6472 6f70 686f 6269 6369  -in hydrophobici
 000061f0: 7479 2073 6361 6c65 2028 4569 7365 6e62  ty scale (Eisenb
 00006200: 6572 6757 6569 7373 2c20 4865 7373 6148  ergWeiss, HessaH
 00006210: 6569 6a6e 652c 0a20 2020 2020 2020 204b  eijne,.        K
 00006220: 7974 6544 6f6f 6c69 7474 652c 204d 6f6f  yteDoolitte, Moo
-00006230: 6e46 6c65 6d69 6e67 2c20 5769 6d6c 6579  nFleming, Wimley
-00006240: 5768 6974 652c 205a 6861 6f4c 6f6e 646f  White, ZhaoLondo
-00006250: 6e29 206f 7220 6120 7061 7468 2074 6f20  n) or a path to 
-00006260: 610a 2020 2020 2020 2020 544f 4d4c 2d66  a.        TOML-f
-00006270: 6f72 6d61 7474 6564 2066 696c 6520 7769  ormatted file wi
-00006280: 7468 2061 2063 7573 746f 6d20 6879 6472  th a custom hydr
-00006290: 6f70 686f 6269 6369 7479 2073 6361 6c65  ophobicity scale
-000062a0: 2c20 6279 2064 6566 6175 6c74 0a20 2020  , by default.   
-000062b0: 2020 2020 2060 4569 7365 6e62 6572 6757       `EisenbergW
-000062c0: 6569 7373 602e 0a20 2020 2073 7572 6661  eiss`..    surfa
-000062d0: 6365 203a 2073 7472 2c20 6f70 7469 6f6e  ce : str, option
-000062e0: 616c 0a20 2020 2020 2020 204b 6579 776f  al.        Keywo
-000062f0: 7264 7320 6f70 7469 6f6e 7320 6172 6520  rds options are 
-00006300: 5345 5320 2853 6f6c 7665 6e74 2045 7863  SES (Solvent Exc
-00006310: 6c75 6465 6420 5375 7266 6163 6529 206f  luded Surface) o
-00006320: 7220 5341 5320 2853 6f6c 7665 6e74 0a20  r SAS (Solvent. 
-00006330: 2020 2020 2020 2041 6363 6573 7369 626c         Accessibl
-00006340: 6520 5375 7266 6163 6529 2c20 6279 2064  e Surface), by d
-00006350: 6566 6175 6c74 2053 4553 2e0a 2020 2020  efault SES..    
-00006360: 6967 6e6f 7265 5f62 6163 6b62 6f6e 6520  ignore_backbone 
-00006370: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-00006380: 0a20 2020 2020 2020 2057 6865 7468 6572  .        Whether
-00006390: 2074 6f20 6967 6e6f 7265 2062 6163 6b62   to ignore backb
-000063a0: 6f6e 6520 6174 6f6d 7320 2843 2c20 4341  one atoms (C, CA
-000063b0: 2c20 4e2c 204f 2920 7768 656e 2064 6566  , N, O) when def
-000063c0: 696e 696e 6720 696e 7465 7266 6163 650a  ining interface.
-000063d0: 2020 2020 2020 2020 7265 7369 6475 6573          residues
-000063e0: 2c20 6279 2064 6566 6175 6c74 2046 616c  , by default Fal
-000063f0: 7365 2e0a 2020 2020 6d6f 6465 6c20 3a20  se..    model : 
-00006400: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-00006410: 2020 2020 2020 4d6f 6465 6c20 6e75 6d62        Model numb
-00006420: 6572 2c20 6279 2064 6566 6175 6c74 204e  er, by default N
-00006430: 6f6e 652e 2049 6620 4e6f 6e65 2c20 6b65  one. If None, ke
-00006440: 6570 2061 746f 6d73 2066 726f 6d20 616c  ep atoms from al
-00006450: 6c20 6d6f 6465 6c73 2e0a 2020 2020 6e74  l models..    nt
-00006460: 6872 6561 6473 203a 2069 6e74 2c20 6f70  hreads : int, op
-00006470: 7469 6f6e 616c 0a20 2020 2020 2020 204e  tional.        N
-00006480: 756d 6265 7220 6f66 2074 6872 6561 6473  umber of threads
-00006490: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-000064a0: 652e 2049 6620 4e6f 6e65 2c20 7468 6520  e. If None, the 
-000064b0: 6e75 6d62 6572 206f 6620 7468 7265 6164  number of thread
-000064c0: 7320 6973 0a20 2020 2020 2020 2060 6f73  s is.        `os
-000064d0: 2e63 7075 5f63 6f75 6e74 2829 202d 2031  .cpu_count() - 1
-000064e0: 602e 0a20 2020 2076 6572 626f 7365 203a  `..    verbose :
-000064f0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00006500: 2020 2020 2020 2020 5072 696e 7420 6578          Print ex
-00006510: 7472 6120 696e 666f 726d 6174 696f 6e20  tra information 
-00006520: 746f 2073 7461 6e64 6172 6420 6f75 7470  to standard outp
-00006530: 7574 2c20 6279 2064 6566 6175 6c74 2046  ut, by default F
-00006540: 616c 7365 2e0a 0a20 2020 2052 6574 7572  alse...    Retur
-00006550: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00006560: 2020 2072 6573 756c 7473 203a 2070 794b     results : pyK
-00006570: 5646 696e 6465 7252 6573 756c 7473 0a20  VFinderResults. 
-00006580: 2020 2020 2020 2041 2063 6c61 7373 2077         A class w
-00006590: 6974 6820 7468 6520 666f 6c6c 6f77 696e  ith the followin
-000065a0: 6720 6174 7472 6962 7574 6573 2064 6566  g attributes def
-000065b0: 696e 6564 3a0a 0a20 2020 2020 2020 2020  ined:..         
-000065c0: 2020 202a 2063 6176 6974 6965 7320 3a20     * cavities : 
-000065d0: 6e75 6d70 792e 6e64 6172 7261 790a 0a20  numpy.ndarray.. 
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000065f0: 6176 6974 7920 706f 696e 7473 2069 6e20  avity points in 
-00006600: 7468 6520 3344 2067 7269 6420 2863 6176  the 3D grid (cav
-00006610: 6974 6965 735b 6e78 5d5b 6e79 5d5b 6e7a  ities[nx][ny][nz
-00006620: 5d29 2e0a 2020 2020 2020 2020 2020 2020  ])..            
-00006630: 2020 2020 4361 7669 7469 6573 2061 7272      Cavities arr
-00006640: 6179 2068 6173 2069 6e74 6567 6572 206c  ay has integer l
-00006650: 6162 656c 7320 696e 2065 6163 6820 706f  abels in each po
-00006660: 7369 7469 6f6e 2c20 7468 6174 2061 7265  sition, that are
-00006670: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006680: 2020 202a 202d 313a 2062 756c 6b20 706f     * -1: bulk po
-00006690: 696e 7473 3b0a 2020 2020 2020 2020 2020  ints;.          
-000066a0: 2020 2020 2020 2a20 303a 2062 696f 6d6f        * 0: biomo
-000066b0: 6c65 6375 6c65 2070 6f69 6e74 733b 0a20  lecule points;. 
-000066c0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-000066d0: 2031 3a20 656d 7074 7920 7370 6163 6520   1: empty space 
-000066e0: 706f 696e 7473 3b0a 2020 2020 2020 2020  points;.        
-000066f0: 2020 2020 2020 2020 2a20 3e3d 323a 2063          * >=2: c
-00006700: 6176 6974 7920 706f 696e 7473 2e0a 0a20  avity points... 
-00006710: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00006720: 6865 2065 6d70 7479 2073 7061 6365 2070  he empty space p
-00006730: 6f69 6e74 7320 6172 6520 7265 6769 6f6e  oints are region
-00006740: 7320 7468 6174 2064 6f20 6e6f 7420 6d65  s that do not me
-00006750: 6574 2074 6865 2063 686f 7365 6e0a 2020  et the chosen.  
-00006760: 2020 2020 2020 2020 2020 2020 2020 766f                vo
-00006770: 6c75 6d65 2063 7574 6f66 6620 746f 2062  lume cutoff to b
-00006780: 6520 636f 6e73 6964 6572 6564 2061 2063  e considered a c
-00006790: 6176 6974 792e 0a0a 2020 2020 2020 2020  avity...        
-000067a0: 2020 2020 2a20 7375 7266 6163 6520 3a20      * surface : 
-000067b0: 6e75 6d70 792e 6e64 6172 7261 790a 0a20  numpy.ndarray.. 
-000067c0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-000067d0: 7572 6661 6365 2070 6f69 6e74 7320 696e  urface points in
-000067e0: 2074 6865 2033 4420 6772 6964 2028 7375   the 3D grid (su
-000067f0: 7266 6163 655b 6e78 5d5b 6e79 5d5b 6e7a  rface[nx][ny][nz
-00006800: 5d29 2e0a 2020 2020 2020 2020 2020 2020  ])..            
-00006810: 2020 2020 5375 7266 6163 6520 6172 7261      Surface arra
-00006820: 7920 6861 7320 696e 7465 6765 7220 6c61  y has integer la
-00006830: 6265 6c73 2069 6e20 6561 6368 2070 6f73  bels in each pos
-00006840: 6974 696f 6e2c 2074 6861 7420 6172 653a  ition, that are:
-00006850: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006860: 2020 2a20 2d31 3a20 6275 6c6b 2070 6f69    * -1: bulk poi
-00006870: 6e74 733b 0a20 2020 2020 2020 2020 2020  nts;.           
-00006880: 2020 2020 202a 2030 3a20 6269 6f6d 6f6c       * 0: biomol
-00006890: 6563 756c 6520 6f72 2065 6d70 7479 2073  ecule or empty s
-000068a0: 7061 6365 2070 6f69 6e74 733b 0a20 2020  pace points;.   
-000068b0: 2020 2020 2020 2020 2020 2020 202a 203e               * >
-000068c0: 3d32 3a20 7375 7266 6163 6520 706f 696e  =2: surface poin
-000068d0: 7473 2e0a 0a20 2020 2020 2020 2020 2020  ts...           
-000068e0: 2020 2020 2054 6865 2065 6d70 7479 2073       The empty s
-000068f0: 7061 6365 2070 6f69 6e74 7320 6172 6520  pace points are 
-00006900: 7265 6769 6f6e 7320 7468 6174 2064 6f20  regions that do 
-00006910: 6e6f 7420 6d65 6574 2074 6865 2063 686f  not meet the cho
-00006920: 7365 6e0a 2020 2020 2020 2020 2020 2020  sen.            
-00006930: 2020 2020 766f 6c75 6d65 2063 7574 6f66      volume cutof
-00006940: 6620 746f 2062 6520 636f 6e73 6964 6572  f to be consider
-00006950: 6564 2061 2063 6176 6974 792e 0a0a 2020  ed a cavity...  
-00006960: 2020 2020 2020 2020 2020 2a20 6465 7074            * dept
-00006970: 6873 203a 206e 756d 7079 2e6e 6461 7272  hs : numpy.ndarr
-00006980: 6179 2c20 6f70 7469 6f6e 616c 0a0a 2020  ay, optional..  
-00006990: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-000069a0: 6e75 6d70 792e 6e64 6172 7261 7920 7769  numpy.ndarray wi
-000069b0: 7468 2064 6570 7468 206f 6620 6361 7669  th depth of cavi
-000069c0: 7479 2070 6f69 6e74 7320 2864 6570 7468  ty points (depth
-000069d0: 5b6e 785d 5b6e 795d 5b6e 7a5d 292e 0a0a  [nx][ny][nz])...
-000069e0: 2020 2020 2020 2020 2020 2020 2a20 7363              * sc
-000069f0: 616c 6573 203a 206e 756d 7079 2e6e 6461  ales : numpy.nda
-00006a00: 7272 6179 2c20 6f70 7469 6f6e 616c 0a0a  rray, optional..
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a20: 4120 6e75 6d70 792e 6e64 6172 7261 7920  A numpy.ndarray 
-00006a30: 7769 7468 2068 7964 726f 7068 6f62 6963  with hydrophobic
-00006a40: 6974 7920 7363 616c 6520 7661 6c75 6520  ity scale value 
-00006a50: 6d61 7070 6564 2061 7420 7375 7266 6163  mapped at surfac
-00006a60: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00006a70: 2020 706f 696e 7473 2028 7363 616c 6573    points (scales
-00006a80: 5b6e 785d 5b6e 795d 5b6e 7a5d 292e 0a0a  [nx][ny][nz])...
-00006a90: 2020 2020 2020 2020 2020 2020 2a20 6e63              * nc
-00006aa0: 6176 203a 2069 6e74 0a0a 2020 2020 2020  av : int..      
-00006ab0: 2020 2020 2020 2020 2020 4e75 6d62 6572            Number
-00006ac0: 206f 6620 6361 7669 7469 6573 2e0a 0a20   of cavities... 
-00006ad0: 2020 2020 2020 2020 2020 202a 2076 6f6c             * vol
-00006ae0: 756d 6520 3a20 4469 6374 5b73 7472 2c20  ume : Dict[str, 
-00006af0: 666c 6f61 745d 0a0a 2020 2020 2020 2020  float]..        
-00006b00: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-00006b10: 6e61 7279 2077 6974 6820 766f 6c75 6d65  nary with volume
-00006b20: 206f 6620 6561 6368 2064 6574 6563 7465   of each detecte
-00006b30: 6420 6361 7669 7479 2e0a 0a20 2020 2020  d cavity...     
-00006b40: 2020 2020 2020 202a 2061 7265 6120 3a20         * area : 
-00006b50: 4469 6374 5b73 7472 2c20 666c 6f61 745d  Dict[str, float]
-00006b60: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006b70: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
-00006b80: 6974 6820 6172 6561 206f 6620 6561 6368  ith area of each
-00006b90: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
-00006ba0: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
-00006bb0: 206d 6178 5f64 6570 7468 203a 2044 6963   max_depth : Dic
-00006bc0: 745b 7374 722c 2066 6c6f 6174 5d2c 206f  t[str, float], o
-00006bd0: 7074 696f 6e61 6c0a 0a20 2020 2020 2020  ptional..       
-00006be0: 2020 2020 2020 2020 2041 2064 6963 7469           A dicti
-00006bf0: 6f6e 6172 7920 7769 7468 206d 6178 696d  onary with maxim
-00006c00: 756d 2064 6570 7468 206f 6620 6561 6368  um depth of each
-00006c10: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
-00006c20: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
-00006c30: 2061 7667 5f64 6570 7468 203a 2044 6963   avg_depth : Dic
-00006c40: 745b 7374 722c 2066 6c6f 6174 5d2c 206f  t[str, float], o
-00006c50: 7074 696f 6e61 6c0a 0a20 2020 2020 2020  ptional..       
-00006c60: 2020 2020 2020 2020 2041 2064 6963 7469           A dicti
-00006c70: 6f6e 6172 7920 7769 7468 2061 7665 7261  onary with avera
-00006c80: 6765 2064 6570 7468 206f 6620 6561 6368  ge depth of each
-00006c90: 2064 6574 6563 7465 6420 6361 7669 7479   detected cavity
-00006ca0: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
-00006cb0: 2061 7667 5f68 7964 726f 7061 7468 7920   avg_hydropathy 
-00006cc0: 3a20 4469 6374 5b73 7472 2c20 666c 6f61  : Dict[str, floa
-00006cd0: 745d 2c20 6f70 7469 6f6e 616c 0a0a 2020  t], optional..  
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00006cf0: 6469 6374 696f 6e61 7279 2077 6974 6820  dictionary with 
-00006d00: 6176 6572 6167 6520 6879 6472 6f70 6174  average hydropat
-00006d10: 6879 2066 6f72 2065 6163 6820 6465 7465  hy for each dete
-00006d20: 6374 6564 2063 6176 6974 7920 616e 640a  cted cavity and.
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 7468 6520 7261 6e67 6520 6f66 2074 6865  the range of the
-00006d50: 2068 7964 726f 7068 6f62 6963 6974 7920   hydrophobicity 
-00006d60: 7363 616c 6520 286d 696e 2c20 6d61 7829  scale (min, max)
-00006d70: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
-00006d80: 2072 6573 6964 7565 733a 2044 6963 745b   residues: Dict[
-00006d90: 7374 722c 204c 6973 745b 4c69 7374 5b73  str, List[List[s
-00006da0: 7472 5d5d 5d0a 0a20 2020 2020 2020 2020  tr]]]..         
-00006db0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-00006dc0: 6172 7920 7769 7468 2061 206c 6973 7420  ary with a list 
-00006dd0: 6f66 2069 6e74 6572 6661 6365 2072 6573  of interface res
-00006de0: 6964 7565 7320 666f 7220 6561 6368 2064  idues for each d
-00006df0: 6574 6563 7465 640a 2020 2020 2020 2020  etected.        
-00006e00: 2020 2020 2020 2020 6361 7669 7479 2e0a          cavity..
-00006e10: 0a20 2020 2020 2020 2020 2020 202a 2066  .            * f
-00006e20: 7265 7175 656e 6369 6573 203a 2044 6963  requencies : Dic
-00006e30: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
-00006e40: 2044 6963 745b 7374 722c 2069 6e74 5d5d   Dict[str, int]]
-00006e50: 5d2c 206f 7074 696f 6e61 6c0a 0a20 2020  ], optional..   
-00006e60: 2020 2020 2020 2020 2020 2020 2041 2064               A d
-00006e70: 6963 7469 6f6e 6172 7920 7769 7468 2066  ictionary with f
-00006e80: 7265 7175 656e 6369 6573 206f 6620 7265  requencies of re
-00006e90: 7369 6475 6573 2061 6e64 2063 6c61 7373  sidues and class
-00006ea0: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
-00006eb0: 2020 2020 2072 6573 6964 7565 7320 6f66       residues of
-00006ec0: 2065 6163 6820 6465 7465 6374 6564 2063   each detected c
-00006ed0: 6176 6974 792e 0a0a 2020 2020 2020 2020  avity...        
-00006ee0: 2020 2020 2a20 5f76 6572 7469 6365 7320      * _vertices 
-00006ef0: 3a20 6e75 6d70 792e 6e64 6172 7261 790a  : numpy.ndarray.
-00006f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f10: 2041 206e 756d 7079 2e6e 6461 7272 6179   A numpy.ndarray
-00006f20: 206f 7220 6120 6c69 7374 2077 6974 6820   or a list with 
-00006f30: 7879 7a20 7665 7274 6963 6573 2063 6f6f  xyz vertices coo
-00006f40: 7264 696e 6174 6573 2028 6f72 6967 696e  rdinates (origin
-00006f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006f60: 2020 582d 6178 6973 2c20 592d 6178 6973    X-axis, Y-axis
-00006f70: 2c20 5a2d 6178 6973 292e 0a0a 2020 2020  , Z-axis)...    
-00006f80: 2020 2020 2020 2020 2a20 5f73 7465 7020          * _step 
-00006f90: 3a20 666c 6f61 740a 0a20 2020 2020 2020  : float..       
-00006fa0: 2020 2020 2020 2020 2047 7269 6420 7370           Grid sp
-00006fb0: 6163 696e 6720 2841 292e 0a0a 2020 2020  acing (A)...    
-00006fc0: 2020 2020 2020 2020 2a20 5f69 6e70 7574          * _input
-00006fd0: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
-00006fe0: 7468 6c69 622e 5061 7468 5d2c 206f 7074  thlib.Path], opt
-00006ff0: 696f 6e61 6c0a 0a20 2020 2020 2020 2020  ional..         
-00007000: 2020 2020 2020 2041 2070 6174 6820 746f         A path to
-00007010: 2069 6e70 7574 2050 4442 206f 7220 5859   input PDB or XY
-00007020: 5a20 6669 6c65 2e0a 0a20 2020 2020 2020  Z file...       
-00007030: 2020 2020 202a 205f 6c69 6761 6e64 203a       * _ligand :
-00007040: 2055 6e69 6f6e 5b73 7472 2c20 7061 7468   Union[str, path
-00007050: 6c69 622e 5061 7468 5d2c 206f 7074 696f  lib.Path], optio
-00007060: 6e61 6c0a 0a20 2020 2020 2020 2020 2020  nal..           
-00007070: 2020 2020 2041 2070 6174 6820 746f 206c       A path to l
-00007080: 6967 616e 6420 5044 4220 6f72 2058 595a  igand PDB or XYZ
-00007090: 2066 696c 652e 0a0a 2020 2020 5261 6973   file...    Rais
-000070a0: 6573 0a20 2020 202d 2d2d 2d2d 2d0a 2020  es.    ------.  
-000070b0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-000070c0: 2020 2020 6069 6e70 7574 6020 6d75 7374      `input` must
-000070d0: 2068 6176 6520 2e70 6462 206f 7220 2e78   have .pdb or .x
-000070e0: 797a 2065 7874 656e 7369 6f6e 2e0a 2020  yz extension..  
-000070f0: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-00007100: 2020 2020 606c 6967 616e 6460 206d 7573      `ligand` mus
-00007110: 7420 6861 7665 202e 7064 6220 6f72 202e  t have .pdb or .
-00007120: 7879 7a20 6578 7465 6e73 696f 6e2e 0a0a  xyz extension...
-00007130: 2020 2020 4e6f 7465 0a20 2020 202d 2d2d      Note.    ---
-00007140: 2d0a 2020 2020 5468 6520 6361 7669 7479  -.    The cavity
-00007150: 206e 6f6d 656e 636c 6174 7572 6520 6973   nomenclature is
-00007160: 2062 6173 6564 206f 6e20 7468 6520 696e   based on the in
-00007170: 7465 6765 7220 6c61 6265 6c2e 2054 6865  teger label. The
-00007180: 2063 6176 6974 7920 6d61 726b 6564 0a20   cavity marked. 
-00007190: 2020 2077 6974 6820 322c 2074 6865 2066     with 2, the f
-000071a0: 6972 7374 2069 6e74 6567 6572 2063 6f72  irst integer cor
-000071b0: 7265 7370 6f6e 6469 6e67 2074 6f20 6120  responding to a 
-000071c0: 6361 7669 7479 2c20 6973 204b 4141 2c20  cavity, is KAA, 
-000071d0: 7468 6520 6361 7669 7479 0a20 2020 206d  the cavity.    m
-000071e0: 6172 6b65 6420 7769 7468 2033 2069 7320  arked with 3 is 
-000071f0: 4b41 422c 2074 6865 2063 6176 6974 7920  KAB, the cavity 
-00007200: 6d61 726b 6564 2077 6974 6820 3420 6973  marked with 4 is
-00007210: 204b 4143 2061 6e64 2073 6f20 6f6e 2e0a   KAC and so on..
-00007220: 0a20 2020 204e 6f74 650a 2020 2020 2d2d  .    Note.    --
-00007230: 2d2d 0a20 2020 2054 6865 2063 6c61 7373  --.    The class
-00007240: 6573 206f 6620 7265 7369 6475 6573 2061  es of residues a
-00007250: 7265 3a0a 0a20 2020 202a 2041 6c69 7068  re:..    * Aliph
-00007260: 6174 6963 2061 706f 6c61 7220 2852 3129  atic apolar (R1)
-00007270: 3a20 416c 616e 696e 652c 2047 6c79 6369  : Alanine, Glyci
-00007280: 6e65 2c20 4973 6f6c 6575 6369 6e65 2c20  ne, Isoleucine, 
-00007290: 4c65 7563 696e 652c 204d 6574 6869 6f6e  Leucine, Methion
-000072a0: 696e 652c 2056 616c 696e 652e 0a0a 2020  ine, Valine...  
-000072b0: 2020 2a20 4172 6f6d 6174 6963 2028 5232    * Aromatic (R2
-000072c0: 293a 2050 6865 6e79 6c61 6c61 6e69 6e65  ): Phenylalanine
-000072d0: 2c20 5472 7970 746f 7068 616e 2c20 5479  , Tryptophan, Ty
-000072e0: 726f 7369 6e65 2e0a 0a20 2020 202a 2050  rosine...    * P
-000072f0: 6f6c 6172 2055 6e63 6861 7267 6564 2028  olar Uncharged (
-00007300: 5233 293a 2041 7370 6172 6167 696e 652c  R3): Asparagine,
-00007310: 2043 7973 7465 696e 652c 2047 6c75 7461   Cysteine, Gluta
-00007320: 6d69 6e65 2c20 5072 6f6c 696e 652c 2053  mine, Proline, S
-00007330: 6572 696e 652c 2054 6872 656f 6e69 6e65  erine, Threonine
-00007340: 2e0a 0a20 2020 202a 204e 6567 6174 6976  ...    * Negativ
-00007350: 656c 7920 6368 6172 6765 6420 2852 3429  ely charged (R4)
-00007360: 3a20 4173 7061 7274 6174 652c 2047 6c75  : Aspartate, Glu
-00007370: 7461 6d61 7465 2e0a 0a20 2020 202a 2050  tamate...    * P
-00007380: 6f73 6974 6976 656c 7920 6368 6172 6765  ositively charge
-00007390: 6420 2852 3529 3a20 4172 6769 6e69 6e65  d (R5): Arginine
-000073a0: 2c20 4869 7374 6964 696e 652c 204c 7973  , Histidine, Lys
-000073b0: 696e 652e 0a0a 2020 2020 2a20 4e6f 6e2d  ine...    * Non-
-000073c0: 7374 616e 6461 7264 2028 5258 293a 204e  standard (RX): N
-000073d0: 6f6e 2d73 7461 6e64 6172 6420 7265 7369  on-standard resi
-000073e0: 6475 6573 2e0a 0a20 2020 2053 6565 2041  dues...    See A
-000073f0: 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  lso.    --------
-00007400: 0a20 2020 2070 794b 5646 696e 6465 7252  .    pyKVFinderR
-00007410: 6573 756c 7473 0a0a 2020 2020 4578 616d  esults..    Exam
-00007420: 706c 650a 2020 2020 2d2d 2d2d 2d2d 2d0a  ple.    -------.
-00007430: 2020 2020 5468 6520 2a2a 7374 616e 6461      The **standa
-00007440: 7264 2077 6f72 6b66 6c6f 772a 2a20 666f  rd workflow** fo
-00007450: 7220 6361 7669 7479 2064 6574 6563 7469  r cavity detecti
-00007460: 6f6e 2077 6974 6820 7370 6174 6961 6c20  on with spatial 
-00007470: 2873 7572 6661 6365 2070 6f69 6e74 732c  (surface points,
-00007480: 2076 6f6c 756d 652c 2061 7265 6129 2061   volume, area) a
-00007490: 6e64 2063 6f6e 7374 6974 7574 696f 6e61  nd constitutiona
-000074a0: 6c20 2869 6e74 6572 6661 6365 2072 6573  l (interface res
-000074b0: 6964 7565 7320 616e 6420 7468 6569 7220  idues and their 
-000074c0: 6672 6571 7565 6e63 6965 7329 2063 6861  frequencies) cha
-000074d0: 7261 6374 6572 697a 6174 696f 6e20 2063  racterization  c
-000074e0: 616e 2062 6520 7275 6e20 6174 206f 6e63  an be run at onc
-000074f0: 6520 7769 7468 206f 6e65 2063 6f6d 6d61  e with one comma
-00007500: 6e64 3a0a 0a20 2020 203e 3e3e 2069 6d70  nd:..    >>> imp
-00007510: 6f72 7420 6f73 0a20 2020 203e 3e3e 2069  ort os.    >>> i
-00007520: 6d70 6f72 7420 7079 4b56 4669 6e64 6572  mport pyKVFinder
-00007530: 0a20 2020 203e 3e3e 2070 6462 203d 206f  .    >>> pdb = o
-00007540: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00007550: 6174 682e 6469 726e 616d 6528 7079 4b56  ath.dirname(pyKV
-00007560: 4669 6e64 6572 2e5f 5f66 696c 655f 5f29  Finder.__file__)
-00007570: 2c20 2764 6174 6127 2c20 2774 6573 7473  , 'data', 'tests
-00007580: 272c 2027 3146 4d4f 2e70 6462 2729 0a20  ', '1FMO.pdb'). 
-00007590: 2020 203e 3e3e 2072 6573 756c 7473 203d     >>> results =
-000075a0: 2070 794b 5646 696e 6465 722e 7275 6e5f   pyKVFinder.run_
-000075b0: 776f 726b 666c 6f77 2870 6462 290a 2020  workflow(pdb).  
-000075c0: 2020 3e3e 3e20 7265 7375 6c74 730a 2020    >>> results.  
-000075d0: 2020 3c70 794b 5646 696e 6465 7252 6573    <pyKVFinderRes
-000075e0: 756c 7473 206f 626a 6563 743e 0a20 2020  ults object>.   
-000075f0: 203e 3e3e 2072 6573 756c 7473 2e63 6176   >>> results.cav
-00007600: 6974 6965 730a 2020 2020 6172 7261 7928  ities.    array(
-00007610: 5b5b 5b2d 312c 202d 312c 202d 312c 202e  [[[-1, -1, -1, .
-00007620: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-00007630: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-00007640: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-00007650: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-00007660: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00007670: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00007680: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-00007690: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-000076a0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-000076b0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-000076c0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000076d0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-000076e0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-000076f0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00007700: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00007710: 2d31 2c20 2d31 5d5d 2c0a 2020 2020 2020  -1, -1]],.      
-00007720: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-00007730: 2020 2020 205b 5b2d 312c 202d 312c 202d       [[-1, -1, -
-00007740: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00007750: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00007760: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00007770: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00007780: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00007790: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-000077a0: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-000077b0: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-000077c0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-000077d0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-000077e0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-000077f0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-00007800: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-00007810: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00007820: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-00007830: 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c 2064  -1, -1, -1]]], d
-00007840: 7479 7065 3d69 6e74 3332 290a 2020 2020  type=int32).    
-00007850: 3e3e 3e20 7265 7375 6c74 732e 7375 7266  >>> results.surf
-00007860: 6163 650a 2020 2020 6172 7261 7928 5b5b  ace.    array([[
-00007870: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00007880: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-00007890: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-000078a0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-000078b0: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-000078c0: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-000078d0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-000078e0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-000078f0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00007900: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-00007910: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-00007920: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-00007930: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-00007940: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-00007950: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00007960: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00007970: 2c20 2d31 5d5d 2c0a 2020 2020 2020 2020  , -1]],.        
-00007980: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00007990: 2020 205b 5b2d 312c 202d 312c 202d 312c     [[-1, -1, -1,
-000079a0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-000079b0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-000079c0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-000079d0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-000079e0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-000079f0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00007a00: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00007a10: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-00007a20: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00007a30: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00007a40: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00007a50: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00007a60: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00007a70: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00007a80: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00007a90: 2c20 2d31 2c20 2d31 5d5d 5d2c 2064 7479  , -1, -1]]], dty
-00007aa0: 7065 3d69 6e74 3332 290a 2020 2020 3e3e  pe=int32).    >>
-00007ab0: 3e20 7265 7375 6c74 732e 6e63 6176 0a20  > results.ncav. 
-00007ac0: 2020 203e 3e3e 2031 380a 2020 2020 3e3e     >>> 18.    >>
-00007ad0: 3e20 7265 7375 6c74 732e 766f 6c75 6d65  > results.volume
-00007ae0: 0a20 2020 207b 274b 4141 273a 2031 3337  .    {'KAA': 137
-00007af0: 2e31 362c 2027 4b41 4227 3a20 3437 2e35  .16, 'KAB': 47.5
-00007b00: 322c 2027 4b41 4327 3a20 3636 2e39 362c  2, 'KAC': 66.96,
-00007b10: 2027 4b41 4427 3a20 382e 3231 2c20 274b   'KAD': 8.21, 'K
-00007b20: 4145 273a 2034 332e 3633 2c20 274b 4146  AE': 43.63, 'KAF
-00007b30: 273a 2031 322e 3533 2c20 274b 4147 273a  ': 12.53, 'KAG':
-00007b40: 2036 2e32 362c 2027 4b41 4827 3a20 3532   6.26, 'KAH': 52
-00007b50: 302e 3133 2c20 274b 4149 273a 2031 322e  0.13, 'KAI': 12.
-00007b60: 3331 2c20 274b 414a 273a 2032 362e 3537  31, 'KAJ': 26.57
-00007b70: 2c20 274b 414b 273a 2031 322e 3331 2c20  , 'KAK': 12.31, 
-00007b80: 274b 414c 273a 2033 332e 3931 2c20 274b  'KAL': 33.91, 'K
-00007b90: 414d 273a 2032 332e 3131 2c20 274b 414e  AM': 23.11, 'KAN
-00007ba0: 273a 2031 3032 2e38 322c 2027 4b41 4f27  ': 102.82, 'KAO'
-00007bb0: 3a20 362e 3035 2c20 274b 4150 273a 2031  : 6.05, 'KAP': 1
-00007bc0: 352e 3535 2c20 274b 4151 273a 2037 2e39  5.55, 'KAQ': 7.9
-00007bd0: 392c 2027 4b41 5227 3a20 372e 3738 7d0a  9, 'KAR': 7.78}.
-00007be0: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-00007bf0: 6172 6561 0a20 2020 207b 274b 4141 273a  area.    {'KAA':
-00007c00: 2031 3236 2e34 312c 2027 4b41 4227 3a20   126.41, 'KAB': 
-00007c10: 3632 2e33 372c 2027 4b41 4327 3a20 3734  62.37, 'KAC': 74
-00007c20: 2e35 372c 2027 4b41 4427 3a20 3139 2e30  .57, 'KAD': 19.0
-00007c30: 362c 2027 4b41 4527 3a20 3537 2e30 382c  6, 'KAE': 57.08,
-00007c40: 2027 4b41 4627 3a20 3232 2e37 372c 2027   'KAF': 22.77, '
-00007c50: 4b41 4727 3a20 3135 2e33 382c 2027 4b41  KAG': 15.38, 'KA
-00007c60: 4827 3a20 3439 362e 3937 2c20 274b 4149  H': 496.97, 'KAI
-00007c70: 273a 2033 302e 3538 2c20 274b 414a 273a  ': 30.58, 'KAJ':
-00007c80: 2034 352e 3634 2c20 274b 414b 273a 2033   45.64, 'KAK': 3
-00007c90: 302e 3538 2c20 274b 414c 273a 2034 352e  0.58, 'KAL': 45.
-00007ca0: 3538 2c20 274b 414d 273a 2034 352e 3235  58, 'KAM': 45.25
-00007cb0: 2c20 274b 414e 273a 2031 3239 2e37 372c  , 'KAN': 129.77,
-00007cc0: 2027 4b41 4f27 3a20 3132 2e32 382c 2027   'KAO': 12.28, '
-00007cd0: 4b41 5027 3a20 3235 2e30 342c 2027 4b41  KAP': 25.04, 'KA
-00007ce0: 5127 3a20 3133 2e34 362c 2027 4b41 5227  Q': 13.46, 'KAR'
-00007cf0: 3a20 3136 2e36 7d0a 2020 2020 3e3e 3e20  : 16.6}.    >>> 
-00007d00: 7265 7375 6c74 732e 7265 7369 6475 6573  results.residues
-00007d10: 0a20 2020 207b 274b 4141 273a 205b 5b27  .    {'KAA': [['
-00007d20: 3134 272c 2027 4527 2c20 2753 4552 275d  14', 'E', 'SER']
-00007d30: 2c20 5b27 3135 272c 2027 4527 2c20 2756  , ['15', 'E', 'V
-00007d40: 414c 275d 2c20 5b27 3138 272c 2027 4527  AL'], ['18', 'E'
-00007d50: 2c20 2750 4845 275d 2c20 5b27 3139 272c  , 'PHE'], ['19',
-00007d60: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
-00007d70: 3130 3027 2c20 2745 272c 2027 5048 4527  100', 'E', 'PHE'
-00007d80: 5d2c 205b 2731 3532 272c 2027 4527 2c20  ], ['152', 'E', 
-00007d90: 274c 4555 275d 2c20 5b27 3135 3527 2c20  'LEU'], ['155', 
-00007da0: 2745 272c 2027 474c 5527 5d2c 205b 2731  'E', 'GLU'], ['1
-00007db0: 3536 272c 2027 4527 2c20 2754 5952 275d  56', 'E', 'TYR']
-00007dc0: 2c20 5b27 3239 3227 2c20 2745 272c 2027  , ['292', 'E', '
-00007dd0: 4c59 5327 5d2c 205b 2733 3032 272c 2027  LYS'], ['302', '
-00007de0: 4527 2c20 2754 5250 275d 2c20 5b27 3330  E', 'TRP'], ['30
-00007df0: 3327 2c20 2745 272c 2027 494c 4527 5d2c  3', 'E', 'ILE'],
-00007e00: 205b 2733 3036 272c 2027 4527 2c20 2754   ['306', 'E', 'T
-00007e10: 5952 275d 5d2c 2027 4b41 4227 3a20 5b5b  YR']], 'KAB': [[
-00007e20: 2731 3827 2c20 2745 272c 2027 5048 4527  '18', 'E', 'PHE'
-00007e30: 5d2c 205b 2732 3227 2c20 2745 272c 2027  ], ['22', 'E', '
-00007e40: 414c 4127 5d2c 205b 2732 3527 2c20 2745  ALA'], ['25', 'E
-00007e50: 272c 2027 4153 5027 5d2c 205b 2732 3627  ', 'ASP'], ['26'
-00007e60: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-00007e70: 2732 3927 2c20 2745 272c 2027 4c59 5327  '29', 'E', 'LYS'
-00007e80: 5d2c 205b 2739 3727 2c20 2745 272c 2027  ], ['97', 'E', '
-00007e90: 414c 4127 5d2c 205b 2739 3827 2c20 2745  ALA'], ['98', 'E
-00007ea0: 272c 2027 5641 4c27 5d2c 205b 2739 3927  ', 'VAL'], ['99'
-00007eb0: 2c20 2745 272c 2027 4153 4e27 5d2c 205b  , 'E', 'ASN'], [
-00007ec0: 2731 3536 272c 2027 4527 2c20 2754 5952  '156', 'E', 'TYR
-00007ed0: 275d 5d2c 2027 4b41 4327 3a20 5b5b 2731  ']], 'KAC': [['1
-00007ee0: 3431 272c 2027 4527 2c20 2750 524f 275d  41', 'E', 'PRO']
-00007ef0: 2c20 5b27 3134 3227 2c20 2745 272c 2027  , ['142', 'E', '
-00007f00: 4849 5327 5d2c 205b 2731 3434 272c 2027  HIS'], ['144', '
-00007f10: 4527 2c20 2741 5247 275d 2c20 5b27 3134  E', 'ARG'], ['14
-00007f20: 3527 2c20 2745 272c 2027 5048 4527 5d2c  5', 'E', 'PHE'],
-00007f30: 205b 2731 3438 272c 2027 4527 2c20 2741   ['148', 'E', 'A
-00007f40: 4c41 275d 2c20 5b27 3239 3927 2c20 2745  LA'], ['299', 'E
-00007f50: 272c 2027 5448 5227 5d2c 205b 2733 3030  ', 'THR'], ['300
-00007f60: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
-00007f70: 5b27 3330 3527 2c20 2745 272c 2027 494c  ['305', 'E', 'IL
-00007f80: 4527 5d2c 205b 2733 3130 272c 2027 4527  E'], ['310', 'E'
-00007f90: 2c20 2756 414c 275d 2c20 5b27 3331 3127  , 'VAL'], ['311'
-00007fa0: 2c20 2745 272c 2027 474c 5527 5d2c 205b  , 'E', 'GLU'], [
-00007fb0: 2733 3133 272c 2027 4527 2c20 2750 524f  '313', 'E', 'PRO
-00007fc0: 275d 5d2c 2027 4b41 4427 3a20 5b5b 2731  ']], 'KAD': [['1
-00007fd0: 3232 272c 2027 4527 2c20 2754 5952 275d  22', 'E', 'TYR']
-00007fe0: 2c20 5b27 3132 3427 2c20 2745 272c 2027  , ['124', 'E', '
-00007ff0: 414c 4127 5d2c 205b 2731 3736 272c 2027  ALA'], ['176', '
-00008000: 4527 2c20 2747 4c4e 275d 2c20 5b27 3331  E', 'GLN'], ['31
-00008010: 3827 2c20 2745 272c 2027 5048 4527 5d2c  8', 'E', 'PHE'],
-00008020: 205b 2733 3230 272c 2027 4527 2c20 2747   ['320', 'E', 'G
-00008030: 4c59 275d 2c20 5b27 3332 3127 2c20 2745  LY'], ['321', 'E
-00008040: 272c 2027 5052 4f27 5d2c 205b 2733 3232  ', 'PRO'], ['322
-00008050: 272c 2027 4527 2c20 2747 4c59 275d 2c20  ', 'E', 'GLY'], 
-00008060: 5b27 3332 3327 2c20 2745 272c 2027 4153  ['323', 'E', 'AS
-00008070: 5027 5d5d 2c20 274b 4145 273a 205b 5b27  P']], 'KAE': [['
-00008080: 3935 272c 2027 4527 2c20 274c 4555 275d  95', 'E', 'LEU']
-00008090: 2c20 5b27 3938 272c 2027 4527 2c20 2756  , ['98', 'E', 'V
-000080a0: 414c 275d 2c20 5b27 3939 272c 2027 4527  AL'], ['99', 'E'
-000080b0: 2c20 2741 534e 275d 2c20 5b27 3130 3027  , 'ASN'], ['100'
-000080c0: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-000080d0: 2731 3033 272c 2027 4527 2c20 274c 4555  '103', 'E', 'LEU
-000080e0: 275d 2c20 5b27 3130 3427 2c20 2745 272c  '], ['104', 'E',
-000080f0: 2027 5641 4c27 5d2c 205b 2731 3035 272c   'VAL'], ['105',
-00008100: 2027 4527 2c20 274c 5953 275d 2c20 5b27   'E', 'LYS'], ['
-00008110: 3130 3627 2c20 2745 272c 2027 4c45 5527  106', 'E', 'LEU'
-00008120: 5d5d 2c20 274b 4146 273a 205b 5b27 3132  ]], 'KAF': [['12
-00008130: 3327 2c20 2745 272c 2027 5641 4c27 5d2c  3', 'E', 'VAL'],
-00008140: 205b 2731 3234 272c 2027 4527 2c20 2741   ['124', 'E', 'A
-00008150: 4c41 275d 2c20 5b27 3137 3527 2c20 2745  LA'], ['175', 'E
-00008160: 272c 2027 4153 5027 5d2c 205b 2731 3736  ', 'ASP'], ['176
-00008170: 272c 2027 4527 2c20 2747 4c4e 275d 2c20  ', 'E', 'GLN'], 
-00008180: 5b27 3138 3127 2c20 2745 272c 2027 474c  ['181', 'E', 'GL
-00008190: 4e27 5d5d 2c20 274b 4147 273a 205b 5b27  N']], 'KAG': [['
-000081a0: 3334 272c 2027 4527 2c20 2753 4552 275d  34', 'E', 'SER']
-000081b0: 2c20 5b27 3337 272c 2027 4527 2c20 2754  , ['37', 'E', 'T
-000081c0: 4852 275d 2c20 5b27 3936 272c 2027 4527  HR'], ['96', 'E'
-000081d0: 2c20 2747 4c4e 275d 2c20 5b27 3130 3627  , 'GLN'], ['106'
-000081e0: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
-000081f0: 2731 3037 272c 2027 4527 2c20 2747 4c55  '107', 'E', 'GLU
-00008200: 275d 2c20 5b27 3130 3827 2c20 2745 272c  '], ['108', 'E',
-00008210: 2027 5048 4527 5d2c 205b 2731 3039 272c   'PHE'], ['109',
-00008220: 2027 4527 2c20 2753 4552 275d 5d2c 2027   'E', 'SER']], '
-00008230: 4b41 4827 3a20 5b5b 2734 3927 2c20 2745  KAH': [['49', 'E
-00008240: 272c 2027 4c45 5527 5d2c 205b 2735 3027  ', 'LEU'], ['50'
-00008250: 2c20 2745 272c 2027 474c 5927 5d2c 205b  , 'E', 'GLY'], [
-00008260: 2735 3127 2c20 2745 272c 2027 5448 5227  '51', 'E', 'THR'
-00008270: 5d2c 205b 2735 3227 2c20 2745 272c 2027  ], ['52', 'E', '
-00008280: 474c 5927 5d2c 205b 2735 3327 2c20 2745  GLY'], ['53', 'E
-00008290: 272c 2027 5345 5227 5d2c 205b 2735 3427  ', 'SER'], ['54'
-000082a0: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-000082b0: 2735 3527 2c20 2745 272c 2027 474c 5927  '55', 'E', 'GLY'
-000082c0: 5d2c 205b 2735 3627 2c20 2745 272c 2027  ], ['56', 'E', '
-000082d0: 4152 4727 5d2c 205b 2735 3727 2c20 2745  ARG'], ['57', 'E
-000082e0: 272c 2027 5641 4c27 5d2c 205b 2737 3027  ', 'VAL'], ['70'
-000082f0: 2c20 2745 272c 2027 414c 4127 5d2c 205b  , 'E', 'ALA'], [
-00008300: 2737 3227 2c20 2745 272c 2027 4c59 5327  '72', 'E', 'LYS'
-00008310: 5d2c 205b 2737 3427 2c20 2745 272c 2027  ], ['74', 'E', '
-00008320: 4c45 5527 5d2c 205b 2738 3427 2c20 2745  LEU'], ['84', 'E
-00008330: 272c 2027 474c 4e27 5d2c 205b 2738 3727  ', 'GLN'], ['87'
-00008340: 2c20 2745 272c 2027 4849 5327 5d2c 205b  , 'E', 'HIS'], [
-00008350: 2738 3827 2c20 2745 272c 2027 5448 5227  '88', 'E', 'THR'
-00008360: 5d2c 205b 2739 3127 2c20 2745 272c 2027  ], ['91', 'E', '
-00008370: 474c 5527 5d2c 205b 2731 3034 272c 2027  GLU'], ['104', '
-00008380: 4527 2c20 2756 414c 275d 2c20 5b27 3132  E', 'VAL'], ['12
-00008390: 3027 2c20 2745 272c 2027 4d45 5427 5d2c  0', 'E', 'MET'],
-000083a0: 205b 2731 3231 272c 2027 4527 2c20 2747   ['121', 'E', 'G
-000083b0: 4c55 275d 2c20 5b27 3132 3227 2c20 2745  LU'], ['122', 'E
-000083c0: 272c 2027 5459 5227 5d2c 205b 2731 3233  ', 'TYR'], ['123
-000083d0: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
-000083e0: 5b27 3132 3727 2c20 2745 272c 2027 474c  ['127', 'E', 'GL
-000083f0: 5527 5d2c 205b 2731 3636 272c 2027 4527  U'], ['166', 'E'
-00008400: 2c20 2741 5350 275d 2c20 5b27 3136 3827  , 'ASP'], ['168'
-00008410: 2c20 2745 272c 2027 4c59 5327 5d2c 205b  , 'E', 'LYS'], [
-00008420: 2731 3730 272c 2027 4527 2c20 2747 4c55  '170', 'E', 'GLU
-00008430: 275d 2c20 5b27 3137 3127 2c20 2745 272c  '], ['171', 'E',
-00008440: 2027 4153 4e27 5d2c 205b 2731 3733 272c   'ASN'], ['173',
-00008450: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
-00008460: 3138 3327 2c20 2745 272c 2027 5448 5227  183', 'E', 'THR'
-00008470: 5d2c 205b 2731 3834 272c 2027 4527 2c20  ], ['184', 'E', 
-00008480: 2741 5350 275d 2c20 5b27 3138 3627 2c20  'ASP'], ['186', 
-00008490: 2745 272c 2027 474c 5927 5d2c 205b 2731  'E', 'GLY'], ['1
-000084a0: 3837 272c 2027 4527 2c20 2750 4845 275d  87', 'E', 'PHE']
-000084b0: 2c20 5b27 3230 3127 2c20 2745 272c 2027  , ['201', 'E', '
-000084c0: 5448 5227 5d2c 205b 2733 3237 272c 2027  THR'], ['327', '
-000084d0: 4527 2c20 2750 4845 275d 5d2c 2027 4b41  E', 'PHE']], 'KA
-000084e0: 4927 3a20 5b5b 2731 3331 272c 2027 4527  I': [['131', 'E'
-000084f0: 2c20 2748 4953 275d 2c20 5b27 3133 3827  , 'HIS'], ['138'
-00008500: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-00008510: 2731 3432 272c 2027 4527 2c20 2748 4953  '142', 'E', 'HIS
-00008520: 275d 2c20 5b27 3134 3627 2c20 2745 272c  '], ['146', 'E',
-00008530: 2027 5459 5227 5d2c 205b 2731 3734 272c   'TYR'], ['174',
-00008540: 2027 4527 2c20 2749 4c45 275d 2c20 5b27   'E', 'ILE'], ['
-00008550: 3331 3427 2c20 2745 272c 2027 5048 4527  314', 'E', 'PHE'
-00008560: 5d5d 2c20 274b 414a 273a 205b 5b27 3333  ]], 'KAJ': [['33
-00008570: 272c 2027 4527 2c20 2750 524f 275d 2c20  ', 'E', 'PRO'], 
-00008580: 5b27 3839 272c 2027 4527 2c20 274c 4555  ['89', 'E', 'LEU
-00008590: 275d 2c20 5b27 3932 272c 2027 4527 2c20  '], ['92', 'E', 
-000085a0: 274c 5953 275d 2c20 5b27 3933 272c 2027  'LYS'], ['93', '
-000085b0: 4527 2c20 2741 5247 275d 2c20 5b27 3936  E', 'ARG'], ['96
-000085c0: 272c 2027 4527 2c20 2747 4c4e 275d 2c20  ', 'E', 'GLN'], 
-000085d0: 5b27 3334 3927 2c20 2745 272c 2027 474c  ['349', 'E', 'GL
-000085e0: 5527 5d2c 205b 2733 3530 272c 2027 4527  U'], ['350', 'E'
-000085f0: 2c20 2750 4845 275d 5d2c 2027 4b41 4b27  , 'PHE']], 'KAK'
-00008600: 3a20 5b5b 2731 3537 272c 2027 4527 2c20  : [['157', 'E', 
-00008610: 274c 4555 275d 2c20 5b27 3136 3227 2c20  'LEU'], ['162', 
-00008620: 2745 272c 2027 4c45 5527 5d2c 205b 2731  'E', 'LEU'], ['1
-00008630: 3633 272c 2027 4527 2c20 2749 4c45 275d  63', 'E', 'ILE']
-00008640: 2c20 5b27 3136 3427 2c20 2745 272c 2027  , ['164', 'E', '
-00008650: 5459 5227 5d2c 205b 2731 3835 272c 2027  TYR'], ['185', '
-00008660: 4527 2c20 2750 4845 275d 2c20 5b27 3138  E', 'PHE'], ['18
-00008670: 3827 2c20 2745 272c 2027 414c 4127 5d5d  8', 'E', 'ALA']]
-00008680: 2c20 274b 414c 273a 205b 5b27 3439 272c  , 'KAL': [['49',
-00008690: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
-000086a0: 3132 3727 2c20 2745 272c 2027 474c 5527  127', 'E', 'GLU'
-000086b0: 5d2c 205b 2731 3239 272c 2027 4527 2c20  ], ['129', 'E', 
-000086c0: 2750 4845 275d 2c20 5b27 3133 3027 2c20  'PHE'], ['130', 
-000086d0: 2745 272c 2027 5345 5227 5d2c 205b 2733  'E', 'SER'], ['3
-000086e0: 3236 272c 2027 4527 2c20 2741 534e 275d  26', 'E', 'ASN']
-000086f0: 2c20 5b27 3332 3727 2c20 2745 272c 2027  , ['327', 'E', '
-00008700: 5048 4527 5d2c 205b 2733 3238 272c 2027  PHE'], ['328', '
-00008710: 4527 2c20 2741 5350 275d 2c20 5b27 3333  E', 'ASP'], ['33
-00008720: 3027 2c20 2745 272c 2027 5459 5227 5d5d  0', 'E', 'TYR']]
-00008730: 2c20 274b 414d 273a 205b 5b27 3531 272c  , 'KAM': [['51',
-00008740: 2027 4527 2c20 2754 4852 275d 2c20 5b27   'E', 'THR'], ['
-00008750: 3535 272c 2027 4527 2c20 2747 4c59 275d  55', 'E', 'GLY']
-00008760: 2c20 5b27 3536 272c 2027 4527 2c20 2741  , ['56', 'E', 'A
-00008770: 5247 275d 2c20 5b27 3733 272c 2027 4527  RG'], ['73', 'E'
-00008780: 2c20 2749 4c45 275d 2c20 5b27 3734 272c  , 'ILE'], ['74',
-00008790: 2027 4527 2c20 274c 4555 275d 2c20 5b27   'E', 'LEU'], ['
-000087a0: 3735 272c 2027 4527 2c20 2741 5350 275d  75', 'E', 'ASP']
-000087b0: 2c20 5b27 3131 3527 2c20 2745 272c 2027  , ['115', 'E', '
-000087c0: 4153 4e27 5d2c 205b 2733 3335 272c 2027  ASN'], ['335', '
-000087d0: 4527 2c20 2749 4c45 275d 2c20 5b27 3333  E', 'ILE'], ['33
-000087e0: 3627 2c20 2745 272c 2027 4152 4727 5d5d  6', 'E', 'ARG']]
-000087f0: 2c20 274b 414e 273a 205b 5b27 3136 3527  , 'KAN': [['165'
-00008800: 2c20 2745 272c 2027 4152 4727 5d2c 205b  , 'E', 'ARG'], [
-00008810: 2731 3636 272c 2027 4527 2c20 2741 5350  '166', 'E', 'ASP
-00008820: 275d 2c20 5b27 3136 3727 2c20 2745 272c  '], ['167', 'E',
-00008830: 2027 4c45 5527 5d2c 205b 2731 3939 272c   'LEU'], ['199',
-00008840: 2027 4527 2c20 2743 5953 275d 2c20 5b27   'E', 'CYS'], ['
-00008850: 3230 3027 2c20 2745 272c 2027 474c 5927  200', 'E', 'GLY'
-00008860: 5d2c 205b 2732 3031 272c 2027 4527 2c20  ], ['201', 'E', 
-00008870: 2754 4852 275d 2c20 5b27 3230 3427 2c20  'THR'], ['204', 
-00008880: 2745 272c 2027 5459 5227 5d2c 205b 2732  'E', 'TYR'], ['2
-00008890: 3035 272c 2027 4527 2c20 274c 4555 275d  05', 'E', 'LEU']
-000088a0: 2c20 5b27 3230 3627 2c20 2745 272c 2027  , ['206', 'E', '
-000088b0: 414c 4127 5d2c 205b 2732 3039 272c 2027  ALA'], ['209', '
-000088c0: 4527 2c20 2749 4c45 275d 2c20 5b27 3231  E', 'ILE'], ['21
-000088d0: 3927 2c20 2745 272c 2027 5641 4c27 5d2c  9', 'E', 'VAL'],
-000088e0: 205b 2732 3230 272c 2027 4527 2c20 2741   ['220', 'E', 'A
-000088f0: 5350 275d 2c20 5b27 3232 3327 2c20 2745  SP'], ['223', 'E
-00008900: 272c 2027 414c 4127 5d5d 2c20 274b 414f  ', 'ALA']], 'KAO
-00008910: 273a 205b 5b27 3438 272c 2027 4527 2c20  ': [['48', 'E', 
-00008920: 2754 4852 275d 2c20 5b27 3531 272c 2027  'THR'], ['51', '
-00008930: 4527 2c20 2754 4852 275d 2c20 5b27 3536  E', 'THR'], ['56
-00008940: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
-00008950: 5b27 3333 3027 2c20 2745 272c 2027 5459  ['330', 'E', 'TY
-00008960: 5227 5d2c 205b 2733 3331 272c 2027 4527  R'], ['331', 'E'
-00008970: 2c20 2747 4c55 275d 5d2c 2027 4b41 5027  , 'GLU']], 'KAP'
-00008980: 3a20 5b5b 2732 3232 272c 2027 4527 2c20  : [['222', 'E', 
-00008990: 2754 5250 275d 2c20 5b27 3233 3827 2c20  'TRP'], ['238', 
-000089a0: 2745 272c 2027 5048 4527 5d2c 205b 2732  'E', 'PHE'], ['2
-000089b0: 3533 272c 2027 4527 2c20 2747 4c59 275d  53', 'E', 'GLY']
-000089c0: 2c20 5b27 3235 3427 2c20 2745 272c 2027  , ['254', 'E', '
-000089d0: 4c59 5327 5d2c 205b 2732 3535 272c 2027  LYS'], ['255', '
-000089e0: 4527 2c20 2756 414c 275d 2c20 5b27 3237  E', 'VAL'], ['27
-000089f0: 3327 2c20 2745 272c 2027 4c45 5527 5d5d  3', 'E', 'LEU']]
-00008a00: 2c20 274b 4151 273a 205b 5b27 3230 3727  , 'KAQ': [['207'
-00008a10: 2c20 2745 272c 2027 5052 4f27 5d2c 205b  , 'E', 'PRO'], [
-00008a20: 2732 3038 272c 2027 4527 2c20 2747 4c55  '208', 'E', 'GLU
-00008a30: 275d 2c20 5b27 3231 3127 2c20 2745 272c  '], ['211', 'E',
-00008a40: 2027 4c45 5527 5d2c 205b 2732 3133 272c   'LEU'], ['213',
-00008a50: 2027 4527 2c20 274c 5953 275d 2c20 5b27   'E', 'LYS'], ['
-00008a60: 3237 3527 2c20 2745 272c 2027 5641 4c27  275', 'E', 'VAL'
-00008a70: 5d2c 205b 2732 3737 272c 2027 4527 2c20  ], ['277', 'E', 
-00008a80: 274c 4555 275d 5d2c 2027 4b41 5227 3a20  'LEU']], 'KAR': 
-00008a90: 5b5b 2732 3337 272c 2027 4527 2c20 2750  [['237', 'E', 'P
-00008aa0: 524f 275d 2c20 5b27 3233 3827 2c20 2745  RO'], ['238', 'E
-00008ab0: 272c 2027 5048 4527 5d2c 205b 2732 3439  ', 'PHE'], ['249
-00008ac0: 272c 2027 4527 2c20 274c 5953 275d 2c20  ', 'E', 'LYS'], 
-00008ad0: 5b27 3235 3427 2c20 2745 272c 2027 4c59  ['254', 'E', 'LY
-00008ae0: 5327 5d2c 205b 2732 3535 272c 2027 4527  S'], ['255', 'E'
-00008af0: 2c20 2756 414c 275d 2c20 5b27 3235 3627  , 'VAL'], ['256'
-00008b00: 2c20 2745 272c 2027 4152 4727 5d5d 7d0a  , 'E', 'ARG']]}.
-00008b10: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-00008b20: 6672 6571 7565 6e63 6965 730a 2020 2020  frequencies.    
-00008b30: 7b27 4b41 4127 3a20 7b27 5245 5349 4455  {'KAA': {'RESIDU
-00008b40: 4553 273a 207b 2747 4c55 273a 2031 2c20  ES': {'GLU': 1, 
-00008b50: 2749 4c45 273a 2031 2c20 274c 4555 273a  'ILE': 1, 'LEU':
-00008b60: 2032 2c20 274c 5953 273a 2031 2c20 2750   2, 'LYS': 1, 'P
-00008b70: 4845 273a 2032 2c20 2753 4552 273a 2031  HE': 2, 'SER': 1
-00008b80: 2c20 2754 5250 273a 2031 2c20 2754 5952  , 'TRP': 1, 'TYR
-00008b90: 273a 2032 2c20 2756 414c 273a 2031 7d2c  ': 2, 'VAL': 1},
-00008ba0: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
-00008bb0: 2034 2c20 2752 3227 3a20 352c 2027 5233   4, 'R2': 5, 'R3
-00008bc0: 273a 2031 2c20 2752 3427 3a20 312c 2027  ': 1, 'R4': 1, '
-00008bd0: 5235 273a 2031 2c20 2752 5827 3a20 307d  R5': 1, 'RX': 0}
-00008be0: 7d2c 2027 4b41 4227 3a20 7b27 5245 5349  }, 'KAB': {'RESI
-00008bf0: 4455 4553 273a 207b 2741 4c41 273a 2032  DUES': {'ALA': 2
-00008c00: 2c20 2741 534e 273a 2031 2c20 2741 5350  , 'ASN': 1, 'ASP
-00008c10: 273a 2031 2c20 274c 5953 273a 2031 2c20  ': 1, 'LYS': 1, 
-00008c20: 2750 4845 273a 2032 2c20 2754 5952 273a  'PHE': 2, 'TYR':
-00008c30: 2031 2c20 2756 414c 273a 2031 7d2c 2027   1, 'VAL': 1}, '
-00008c40: 434c 4153 5327 3a20 7b27 5231 273a 2033  CLASS': {'R1': 3
-00008c50: 2c20 2752 3227 3a20 332c 2027 5233 273a  , 'R2': 3, 'R3':
-00008c60: 2031 2c20 2752 3427 3a20 312c 2027 5235   1, 'R4': 1, 'R5
-00008c70: 273a 2031 2c20 2752 5827 3a20 307d 7d2c  ': 1, 'RX': 0}},
-00008c80: 2027 4b41 4327 3a20 7b27 5245 5349 4455   'KAC': {'RESIDU
-00008c90: 4553 273a 207b 2741 4c41 273a 2031 2c20  ES': {'ALA': 1, 
-00008ca0: 2741 5247 273a 2031 2c20 2747 4c55 273a  'ARG': 1, 'GLU':
-00008cb0: 2031 2c20 2748 4953 273a 2031 2c20 2749   1, 'HIS': 1, 'I
-00008cc0: 4c45 273a 2031 2c20 2750 4845 273a 2031  LE': 1, 'PHE': 1
-00008cd0: 2c20 2750 524f 273a 2032 2c20 2754 4852  , 'PRO': 2, 'THR
-00008ce0: 273a 2032 2c20 2756 414c 273a 2031 7d2c  ': 2, 'VAL': 1},
-00008cf0: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
-00008d00: 2035 2c20 2752 3227 3a20 312c 2027 5233   5, 'R2': 1, 'R3
-00008d10: 273a 2032 2c20 2752 3427 3a20 312c 2027  ': 2, 'R4': 1, '
-00008d20: 5235 273a 2032 2c20 2752 5827 3a20 307d  R5': 2, 'RX': 0}
-00008d30: 7d2c 2027 4b41 4427 3a20 7b27 5245 5349  }, 'KAD': {'RESI
-00008d40: 4455 4553 273a 207b 2741 4c41 273a 2031  DUES': {'ALA': 1
-00008d50: 2c20 2741 5350 273a 2031 2c20 2747 4c4e  , 'ASP': 1, 'GLN
-00008d60: 273a 2031 2c20 2747 4c59 273a 2032 2c20  ': 1, 'GLY': 2, 
-00008d70: 2750 4845 273a 2031 2c20 2750 524f 273a  'PHE': 1, 'PRO':
-00008d80: 2031 2c20 2754 5952 273a 2031 7d2c 2027   1, 'TYR': 1}, '
-00008d90: 434c 4153 5327 3a20 7b27 5231 273a 2034  CLASS': {'R1': 4
-00008da0: 2c20 2752 3227 3a20 322c 2027 5233 273a  , 'R2': 2, 'R3':
-00008db0: 2031 2c20 2752 3427 3a20 312c 2027 5235   1, 'R4': 1, 'R5
-00008dc0: 273a 2030 2c20 2752 5827 3a20 307d 7d2c  ': 0, 'RX': 0}},
-00008dd0: 2027 4b41 4527 3a20 7b27 5245 5349 4455   'KAE': {'RESIDU
-00008de0: 4553 273a 207b 2741 534e 273a 2031 2c20  ES': {'ASN': 1, 
-00008df0: 274c 4555 273a 2033 2c20 274c 5953 273a  'LEU': 3, 'LYS':
-00008e00: 2031 2c20 2750 4845 273a 2031 2c20 2756   1, 'PHE': 1, 'V
-00008e10: 414c 273a 2032 7d2c 2027 434c 4153 5327  AL': 2}, 'CLASS'
-00008e20: 3a20 7b27 5231 273a 2035 2c20 2752 3227  : {'R1': 5, 'R2'
-00008e30: 3a20 312c 2027 5233 273a 2031 2c20 2752  : 1, 'R3': 1, 'R
-00008e40: 3427 3a20 302c 2027 5235 273a 2031 2c20  4': 0, 'R5': 1, 
-00008e50: 2752 5827 3a20 307d 7d2c 2027 4b41 4627  'RX': 0}}, 'KAF'
-00008e60: 3a20 7b27 5245 5349 4455 4553 273a 207b  : {'RESIDUES': {
-00008e70: 2741 4c41 273a 2031 2c20 2741 5350 273a  'ALA': 1, 'ASP':
-00008e80: 2031 2c20 2747 4c4e 273a 2032 2c20 2756   1, 'GLN': 2, 'V
-00008e90: 414c 273a 2031 7d2c 2027 434c 4153 5327  AL': 1}, 'CLASS'
-00008ea0: 3a20 7b27 5231 273a 2032 2c20 2752 3227  : {'R1': 2, 'R2'
-00008eb0: 3a20 302c 2027 5233 273a 2032 2c20 2752  : 0, 'R3': 2, 'R
-00008ec0: 3427 3a20 312c 2027 5235 273a 2030 2c20  4': 1, 'R5': 0, 
-00008ed0: 2752 5827 3a20 307d 7d2c 2027 4b41 4727  'RX': 0}}, 'KAG'
-00008ee0: 3a20 7b27 5245 5349 4455 4553 273a 207b  : {'RESIDUES': {
-00008ef0: 2747 4c4e 273a 2031 2c20 2747 4c55 273a  'GLN': 1, 'GLU':
-00008f00: 2031 2c20 274c 4555 273a 2031 2c20 2750   1, 'LEU': 1, 'P
-00008f10: 4845 273a 2031 2c20 2753 4552 273a 2032  HE': 1, 'SER': 2
-00008f20: 2c20 2754 4852 273a 2031 7d2c 2027 434c  , 'THR': 1}, 'CL
-00008f30: 4153 5327 3a20 7b27 5231 273a 2031 2c20  ASS': {'R1': 1, 
-00008f40: 2752 3227 3a20 312c 2027 5233 273a 2034  'R2': 1, 'R3': 4
-00008f50: 2c20 2752 3427 3a20 312c 2027 5235 273a  , 'R4': 1, 'R5':
-00008f60: 2030 2c20 2752 5827 3a20 307d 7d2c 2027   0, 'RX': 0}}, '
-00008f70: 4b41 4827 3a20 7b27 5245 5349 4455 4553  KAH': {'RESIDUES
-00008f80: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
-00008f90: 5247 273a 2031 2c20 2741 534e 273a 2031  RG': 1, 'ASN': 1
-00008fa0: 2c20 2741 5350 273a 2032 2c20 2747 4c4e  , 'ASP': 2, 'GLN
-00008fb0: 273a 2031 2c20 2747 4c55 273a 2034 2c20  ': 1, 'GLU': 4, 
-00008fc0: 2747 4c59 273a 2034 2c20 2748 4953 273a  'GLY': 4, 'HIS':
-00008fd0: 2031 2c20 274c 4555 273a 2033 2c20 274c   1, 'LEU': 3, 'L
-00008fe0: 5953 273a 2032 2c20 274d 4554 273a 2031  YS': 2, 'MET': 1
-00008ff0: 2c20 2750 4845 273a 2033 2c20 2753 4552  , 'PHE': 3, 'SER
-00009000: 273a 2031 2c20 2754 4852 273a 2034 2c20  ': 1, 'THR': 4, 
-00009010: 2754 5952 273a 2031 2c20 2756 414c 273a  'TYR': 1, 'VAL':
-00009020: 2033 7d2c 2027 434c 4153 5327 3a20 7b27   3}, 'CLASS': {'
-00009030: 5231 273a 2031 312c 2027 5232 273a 2034  R1': 11, 'R2': 4
-00009040: 2c20 2752 3327 3a20 382c 2027 5234 273a  , 'R3': 8, 'R4':
-00009050: 2036 2c20 2752 3527 3a20 342c 2027 5258   6, 'R5': 4, 'RX
-00009060: 273a 2030 7d7d 2c20 274b 4149 273a 207b  ': 0}}, 'KAI': {
-00009070: 2752 4553 4944 5545 5327 3a20 7b27 4849  'RESIDUES': {'HI
-00009080: 5327 3a20 322c 2027 494c 4527 3a20 312c  S': 2, 'ILE': 1,
-00009090: 2027 5048 4527 3a20 322c 2027 5459 5227   'PHE': 2, 'TYR'
-000090a0: 3a20 317d 2c20 2743 4c41 5353 273a 207b  : 1}, 'CLASS': {
-000090b0: 2752 3127 3a20 312c 2027 5232 273a 2033  'R1': 1, 'R2': 3
-000090c0: 2c20 2752 3327 3a20 302c 2027 5234 273a  , 'R3': 0, 'R4':
-000090d0: 2030 2c20 2752 3527 3a20 322c 2027 5258   0, 'R5': 2, 'RX
-000090e0: 273a 2030 7d7d 2c20 274b 414a 273a 207b  ': 0}}, 'KAJ': {
-000090f0: 2752 4553 4944 5545 5327 3a20 7b27 4152  'RESIDUES': {'AR
-00009100: 4727 3a20 312c 2027 474c 4e27 3a20 312c  G': 1, 'GLN': 1,
-00009110: 2027 474c 5527 3a20 312c 2027 4c45 5527   'GLU': 1, 'LEU'
-00009120: 3a20 312c 2027 4c59 5327 3a20 312c 2027  : 1, 'LYS': 1, '
-00009130: 5048 4527 3a20 312c 2027 5052 4f27 3a20  PHE': 1, 'PRO': 
-00009140: 317d 2c20 2743 4c41 5353 273a 207b 2752  1}, 'CLASS': {'R
-00009150: 3127 3a20 322c 2027 5232 273a 2031 2c20  1': 2, 'R2': 1, 
-00009160: 2752 3327 3a20 312c 2027 5234 273a 2031  'R3': 1, 'R4': 1
-00009170: 2c20 2752 3527 3a20 322c 2027 5258 273a  , 'R5': 2, 'RX':
-00009180: 2030 7d7d 2c20 274b 414b 273a 207b 2752   0}}, 'KAK': {'R
-00009190: 4553 4944 5545 5327 3a20 7b27 414c 4127  ESIDUES': {'ALA'
-000091a0: 3a20 312c 2027 494c 4527 3a20 312c 2027  : 1, 'ILE': 1, '
-000091b0: 4c45 5527 3a20 322c 2027 5048 4527 3a20  LEU': 2, 'PHE': 
-000091c0: 312c 2027 5459 5227 3a20 317d 2c20 2743  1, 'TYR': 1}, 'C
-000091d0: 4c41 5353 273a 207b 2752 3127 3a20 342c  LASS': {'R1': 4,
-000091e0: 2027 5232 273a 2032 2c20 2752 3327 3a20   'R2': 2, 'R3': 
-000091f0: 302c 2027 5234 273a 2030 2c20 2752 3527  0, 'R4': 0, 'R5'
-00009200: 3a20 302c 2027 5258 273a 2030 7d7d 2c20  : 0, 'RX': 0}}, 
-00009210: 274b 414c 273a 207b 2752 4553 4944 5545  'KAL': {'RESIDUE
-00009220: 5327 3a20 7b27 4153 4e27 3a20 312c 2027  S': {'ASN': 1, '
-00009230: 4153 5027 3a20 312c 2027 474c 5527 3a20  ASP': 1, 'GLU': 
-00009240: 312c 2027 4c45 5527 3a20 312c 2027 5048  1, 'LEU': 1, 'PH
-00009250: 4527 3a20 322c 2027 5345 5227 3a20 312c  E': 2, 'SER': 1,
-00009260: 2027 5459 5227 3a20 317d 2c20 2743 4c41   'TYR': 1}, 'CLA
-00009270: 5353 273a 207b 2752 3127 3a20 312c 2027  SS': {'R1': 1, '
-00009280: 5232 273a 2033 2c20 2752 3327 3a20 322c  R2': 3, 'R3': 2,
-00009290: 2027 5234 273a 2032 2c20 2752 3527 3a20   'R4': 2, 'R5': 
-000092a0: 302c 2027 5258 273a 2030 7d7d 2c20 274b  0, 'RX': 0}}, 'K
-000092b0: 414d 273a 207b 2752 4553 4944 5545 5327  AM': {'RESIDUES'
-000092c0: 3a20 7b27 4152 4727 3a20 322c 2027 4153  : {'ARG': 2, 'AS
-000092d0: 4e27 3a20 312c 2027 4153 5027 3a20 312c  N': 1, 'ASP': 1,
-000092e0: 2027 474c 5927 3a20 312c 2027 494c 4527   'GLY': 1, 'ILE'
-000092f0: 3a20 322c 2027 4c45 5527 3a20 312c 2027  : 2, 'LEU': 1, '
-00009300: 5448 5227 3a20 317d 2c20 2743 4c41 5353  THR': 1}, 'CLASS
-00009310: 273a 207b 2752 3127 3a20 342c 2027 5232  ': {'R1': 4, 'R2
-00009320: 273a 2030 2c20 2752 3327 3a20 322c 2027  ': 0, 'R3': 2, '
-00009330: 5234 273a 2031 2c20 2752 3527 3a20 322c  R4': 1, 'R5': 2,
-00009340: 2027 5258 273a 2030 7d7d 2c20 274b 414e   'RX': 0}}, 'KAN
-00009350: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-00009360: 7b27 414c 4127 3a20 322c 2027 4152 4727  {'ALA': 2, 'ARG'
-00009370: 3a20 312c 2027 4153 5027 3a20 322c 2027  : 1, 'ASP': 2, '
-00009380: 4359 5327 3a20 312c 2027 474c 5927 3a20  CYS': 1, 'GLY': 
-00009390: 312c 2027 494c 4527 3a20 312c 2027 4c45  1, 'ILE': 1, 'LE
-000093a0: 5527 3a20 322c 2027 5448 5227 3a20 312c  U': 2, 'THR': 1,
-000093b0: 2027 5459 5227 3a20 312c 2027 5641 4c27   'TYR': 1, 'VAL'
-000093c0: 3a20 317d 2c20 2743 4c41 5353 273a 207b  : 1}, 'CLASS': {
-000093d0: 2752 3127 3a20 372c 2027 5232 273a 2031  'R1': 7, 'R2': 1
-000093e0: 2c20 2752 3327 3a20 322c 2027 5234 273a  , 'R3': 2, 'R4':
-000093f0: 2032 2c20 2752 3527 3a20 312c 2027 5258   2, 'R5': 1, 'RX
-00009400: 273a 2030 7d7d 2c20 274b 414f 273a 207b  ': 0}}, 'KAO': {
-00009410: 2752 4553 4944 5545 5327 3a20 7b27 4152  'RESIDUES': {'AR
-00009420: 4727 3a20 312c 2027 474c 5527 3a20 312c  G': 1, 'GLU': 1,
-00009430: 2027 5448 5227 3a20 322c 2027 5459 5227   'THR': 2, 'TYR'
-00009440: 3a20 317d 2c20 2743 4c41 5353 273a 207b  : 1}, 'CLASS': {
-00009450: 2752 3127 3a20 302c 2027 5232 273a 2031  'R1': 0, 'R2': 1
-00009460: 2c20 2752 3327 3a20 322c 2027 5234 273a  , 'R3': 2, 'R4':
-00009470: 2031 2c20 2752 3527 3a20 312c 2027 5258   1, 'R5': 1, 'RX
-00009480: 273a 2030 7d7d 2c20 274b 4150 273a 207b  ': 0}}, 'KAP': {
-00009490: 2752 4553 4944 5545 5327 3a20 7b27 474c  'RESIDUES': {'GL
-000094a0: 5927 3a20 312c 2027 4c45 5527 3a20 312c  Y': 1, 'LEU': 1,
-000094b0: 2027 4c59 5327 3a20 312c 2027 5048 4527   'LYS': 1, 'PHE'
-000094c0: 3a20 312c 2027 5452 5027 3a20 312c 2027  : 1, 'TRP': 1, '
-000094d0: 5641 4c27 3a20 317d 2c20 2743 4c41 5353  VAL': 1}, 'CLASS
-000094e0: 273a 207b 2752 3127 3a20 332c 2027 5232  ': {'R1': 3, 'R2
-000094f0: 273a 2032 2c20 2752 3327 3a20 302c 2027  ': 2, 'R3': 0, '
-00009500: 5234 273a 2030 2c20 2752 3527 3a20 312c  R4': 0, 'R5': 1,
-00009510: 2027 5258 273a 2030 7d7d 2c20 274b 4151   'RX': 0}}, 'KAQ
-00009520: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
-00009530: 7b27 474c 5527 3a20 312c 2027 4c45 5527  {'GLU': 1, 'LEU'
-00009540: 3a20 322c 2027 4c59 5327 3a20 312c 2027  : 2, 'LYS': 1, '
-00009550: 5052 4f27 3a20 312c 2027 5641 4c27 3a20  PRO': 1, 'VAL': 
-00009560: 317d 2c20 2743 4c41 5353 273a 207b 2752  1}, 'CLASS': {'R
-00009570: 3127 3a20 342c 2027 5232 273a 2030 2c20  1': 4, 'R2': 0, 
-00009580: 2752 3327 3a20 302c 2027 5234 273a 2031  'R3': 0, 'R4': 1
-00009590: 2c20 2752 3527 3a20 312c 2027 5258 273a  , 'R5': 1, 'RX':
-000095a0: 2030 7d7d 2c20 274b 4152 273a 207b 2752   0}}, 'KAR': {'R
-000095b0: 4553 4944 5545 5327 3a20 7b27 4152 4727  ESIDUES': {'ARG'
-000095c0: 3a20 312c 2027 4c59 5327 3a20 322c 2027  : 1, 'LYS': 2, '
-000095d0: 5048 4527 3a20 312c 2027 5052 4f27 3a20  PHE': 1, 'PRO': 
-000095e0: 312c 2027 5641 4c27 3a20 317d 2c20 2743  1, 'VAL': 1}, 'C
-000095f0: 4c41 5353 273a 207b 2752 3127 3a20 322c  LASS': {'R1': 2,
-00009600: 2027 5232 273a 2031 2c20 2752 3327 3a20   'R2': 1, 'R3': 
-00009610: 302c 2027 5234 273a 2030 2c20 2752 3527  0, 'R4': 0, 'R5'
-00009620: 3a20 332c 2027 5258 273a 2030 7d7d 7d0a  : 3, 'RX': 0}}}.
-00009630: 0a20 2020 2048 6f77 6576 6572 2c20 7573  .    However, us
-00009640: 6572 7320 6d61 7920 6f70 7420 746f 2070  ers may opt to p
-00009650: 6572 666f 726d 2063 6176 6974 7920 6465  erform cavity de
-00009660: 7465 6374 696f 6e20 696e 2061 2073 6567  tection in a seg
-00009670: 6d65 6e74 6564 2073 7061 6365 2074 6872  mented space thr
-00009680: 6f75 6768 206c 6967 616e 6420 6164 6a75  ough ligand adju
-00009690: 7374 6d65 6e74 2061 6e64 2f6f 7220 626f  stment and/or bo
-000096a0: 7820 6164 6a75 7374 6d65 6e74 206d 6f64  x adjustment mod
-000096b0: 6573 2e0a 0a20 2020 2054 6865 2063 6176  es...    The cav
-000096c0: 6974 7920 6465 7465 6374 696f 6e20 6361  ity detection ca
-000096d0: 6e20 6265 206c 696d 6974 6564 2061 726f  n be limited aro
-000096e0: 756e 6420 7468 6520 7461 7267 6574 206c  und the target l
-000096f0: 6967 616e 6428 7329 2c20 7768 6963 6820  igand(s), which 
-00009700: 7769 6c6c 2062 6520 7061 7373 6564 2074  will be passed t
-00009710: 6f20 7079 4b56 4669 6e64 6572 2074 6872  o pyKVFinder thr
-00009720: 6f75 6768 2061 202a 2e70 6462 2a20 6f72  ough a *.pdb* or
-00009730: 2061 202a 2e78 797a 2a20 6669 6c65 732e   a *.xyz* files.
-00009740: 2054 6875 732c 2074 6865 2064 6574 6563   Thus, the detec
-00009750: 7465 6420 6361 7669 7469 6573 2061 7265  ted cavities are
-00009760: 206c 696d 6974 6564 2077 6974 6869 6e20   limited within 
-00009770: 6120 7261 6469 7573 2028 6060 6c69 6761  a radius (``liga
-00009780: 6e64 5f63 7574 6f66 6660 6029 206f 6620  nd_cutoff``) of 
-00009790: 7468 6520 7461 7267 6574 206c 6967 616e  the target ligan
-000097a0: 6428 7329 2e0a 0a20 2020 203e 3e3e 206c  d(s)...    >>> l
-000097b0: 6967 616e 6420 3d20 6f73 2e70 6174 682e  igand = os.path.
-000097c0: 6a6f 696e 286f 732e 7061 7468 2e64 6972  join(os.path.dir
-000097d0: 6e61 6d65 2870 794b 5646 696e 6465 722e  name(pyKVFinder.
-000097e0: 5f5f 6669 6c65 5f5f 292c 2027 6461 7461  __file__), 'data
-000097f0: 272c 2027 7465 7374 7327 2c20 2741 444e  ', 'tests', 'ADN
-00009800: 2e70 6462 2729 0a20 2020 203e 3e3e 2072  .pdb').    >>> r
-00009810: 6573 756c 7473 203d 2070 794b 5646 696e  esults = pyKVFin
-00009820: 6465 722e 7275 6e5f 776f 726b 666c 6f77  der.run_workflow
-00009830: 2870 6462 2c20 6c69 6761 6e64 290a 2020  (pdb, ligand).  
-00009840: 2020 3e3e 3e20 7265 7375 6c74 730a 2020    >>> results.  
-00009850: 2020 3c70 794b 5646 696e 6465 7252 6573    <pyKVFinderRes
-00009860: 756c 7473 206f 626a 6563 743e 0a20 2020  ults object>.   
-00009870: 203e 3e3e 2072 6573 756c 7473 2e63 6176   >>> results.cav
-00009880: 6974 6965 730a 2020 2020 6172 7261 7928  ities.    array(
-00009890: 5b5b 5b2d 312c 202d 312c 202d 312c 202e  [[[-1, -1, -1, .
-000098a0: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-000098b0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-000098c0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-000098d0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-000098e0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-000098f0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00009900: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-00009910: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00009920: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-00009930: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-00009940: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00009950: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-00009960: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-00009970: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00009980: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00009990: 2d31 2c20 2d31 5d5d 2c0a 2020 2020 2020  -1, -1]],.      
-000099a0: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-000099b0: 2020 2020 205b 5b2d 312c 202d 312c 202d       [[-1, -1, -
-000099c0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-000099d0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-000099e0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-000099f0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00009a00: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00009a10: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00009a20: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
-00009a30: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-00009a40: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00009a50: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00009a60: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
-00009a70: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
-00009a80: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-00009a90: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-00009aa0: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-00009ab0: 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c 2064  -1, -1, -1]]], d
-00009ac0: 7479 7065 3d69 6e74 3332 290a 2020 2020  type=int32).    
-00009ad0: 3e3e 3e20 7265 7375 6c74 732e 7375 7266  >>> results.surf
-00009ae0: 6163 650a 2020 2020 6172 7261 7928 5b5b  ace.    array([[
-00009af0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-00009b00: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-00009b10: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-00009b20: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-00009b30: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-00009b40: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00009b50: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00009b60: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00009b70: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00009b80: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-00009b90: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-00009ba0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-00009bb0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-00009bc0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-00009bd0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
-00009be0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
-00009bf0: 2c20 2d31 5d5d 2c0a 2020 2020 2020 2020  , -1]],.        
-00009c00: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-00009c10: 2020 205b 5b2d 312c 202d 312c 202d 312c     [[-1, -1, -1,
-00009c20: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-00009c30: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00009c40: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-00009c50: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-00009c60: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
-00009c70: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
-00009c80: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
-00009c90: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-00009ca0: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-00009cb0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-00009cc0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-00009cd0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-00009ce0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
-00009cf0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
-00009d00: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
-00009d10: 2c20 2d31 2c20 2d31 5d5d 5d2c 2064 7479  , -1, -1]]], dty
-00009d20: 7065 3d69 6e74 3332 290a 2020 2020 3e3e  pe=int32).    >>
-00009d30: 3e20 7265 7375 6c74 732e 6e63 6176 0a20  > results.ncav. 
-00009d40: 2020 203e 3e3e 2031 380a 2020 2020 3e3e     >>> 18.    >>
-00009d50: 3e20 7265 7375 6c74 732e 766f 6c75 6d65  > results.volume
-00009d60: 0a20 2020 207b 274b 4141 273a 2033 3635  .    {'KAA': 365
-00009d70: 2e30 342c 2027 4b41 4227 3a20 3136 2e38  .04, 'KAB': 16.8
-00009d80: 357d 0a20 2020 203e 3e3e 2072 6573 756c  5}.    >>> resul
-00009d90: 7473 2e61 7265 610a 2020 2020 7b27 4b41  ts.area.    {'KA
-00009da0: 4127 3a20 3332 382e 3739 2c20 274b 4142  A': 328.79, 'KAB
-00009db0: 273a 2032 332e 3135 7d0a 2020 2020 3e3e  ': 23.15}.    >>
-00009dc0: 3e20 7265 7375 6c74 732e 7265 7369 6475  > results.residu
-00009dd0: 6573 0a20 2020 207b 274b 4141 273a 205b  es.    {'KAA': [
-00009de0: 5b27 3439 272c 2027 4527 2c20 274c 4555  ['49', 'E', 'LEU
-00009df0: 275d 2c20 5b27 3530 272c 2027 4527 2c20  '], ['50', 'E', 
-00009e00: 2747 4c59 275d 2c20 5b27 3531 272c 2027  'GLY'], ['51', '
-00009e10: 4527 2c20 2754 4852 275d 2c20 5b27 3532  E', 'THR'], ['52
-00009e20: 272c 2027 4527 2c20 2747 4c59 275d 2c20  ', 'E', 'GLY'], 
-00009e30: 5b27 3533 272c 2027 4527 2c20 2753 4552  ['53', 'E', 'SER
-00009e40: 275d 2c20 5b27 3535 272c 2027 4527 2c20  '], ['55', 'E', 
-00009e50: 2747 4c59 275d 2c20 5b27 3536 272c 2027  'GLY'], ['56', '
-00009e60: 4527 2c20 2741 5247 275d 2c20 5b27 3537  E', 'ARG'], ['57
-00009e70: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
-00009e80: 5b27 3730 272c 2027 4527 2c20 2741 4c41  ['70', 'E', 'ALA
-00009e90: 275d 2c20 5b27 3732 272c 2027 4527 2c20  '], ['72', 'E', 
-00009ea0: 274c 5953 275d 2c20 5b27 3130 3427 2c20  'LYS'], ['104', 
-00009eb0: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
-00009ec0: 3230 272c 2027 4527 2c20 274d 4554 275d  20', 'E', 'MET']
-00009ed0: 2c20 5b27 3132 3127 2c20 2745 272c 2027  , ['121', 'E', '
-00009ee0: 474c 5527 5d2c 205b 2731 3232 272c 2027  GLU'], ['122', '
-00009ef0: 4527 2c20 2754 5952 275d 2c20 5b27 3132  E', 'TYR'], ['12
-00009f00: 3327 2c20 2745 272c 2027 5641 4c27 5d2c  3', 'E', 'VAL'],
-00009f10: 205b 2731 3237 272c 2027 4527 2c20 2747   ['127', 'E', 'G
-00009f20: 4c55 275d 2c20 5b27 3136 3627 2c20 2745  LU'], ['166', 'E
-00009f30: 272c 2027 4153 5027 5d2c 205b 2731 3638  ', 'ASP'], ['168
-00009f40: 272c 2027 4527 2c20 274c 5953 275d 2c20  ', 'E', 'LYS'], 
-00009f50: 5b27 3137 3027 2c20 2745 272c 2027 474c  ['170', 'E', 'GL
-00009f60: 5527 5d2c 205b 2731 3731 272c 2027 4527  U'], ['171', 'E'
-00009f70: 2c20 2741 534e 275d 2c20 5b27 3137 3327  , 'ASN'], ['173'
-00009f80: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
-00009f90: 2731 3833 272c 2027 4527 2c20 2754 4852  '183', 'E', 'THR
-00009fa0: 275d 2c20 5b27 3138 3427 2c20 2745 272c  '], ['184', 'E',
-00009fb0: 2027 4153 5027 5d2c 205b 2733 3237 272c   'ASP'], ['327',
-00009fc0: 2027 4527 2c20 2750 4845 275d 5d2c 2027   'E', 'PHE']], '
-00009fd0: 4b41 4227 3a20 5b5b 2734 3927 2c20 2745  KAB': [['49', 'E
-00009fe0: 272c 2027 4c45 5527 5d2c 205b 2731 3237  ', 'LEU'], ['127
-00009ff0: 272c 2027 4527 2c20 2747 4c55 275d 2c20  ', 'E', 'GLU'], 
-0000a000: 5b27 3133 3027 2c20 2745 272c 2027 5345  ['130', 'E', 'SE
-0000a010: 5227 5d2c 205b 2733 3236 272c 2027 4527  R'], ['326', 'E'
-0000a020: 2c20 2741 534e 275d 2c20 5b27 3332 3727  , 'ASN'], ['327'
-0000a030: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
-0000a040: 2733 3238 272c 2027 4527 2c20 2741 5350  '328', 'E', 'ASP
-0000a050: 275d 2c20 5b27 3333 3027 2c20 2745 272c  '], ['330', 'E',
-0000a060: 2027 5459 5227 5d5d 7d0a 2020 2020 3e3e   'TYR']]}.    >>
-0000a070: 3e20 7265 7375 6c74 732e 6672 6571 7565  > results.freque
-0000a080: 6e63 6965 730a 2020 2020 7b27 4b41 4127  ncies.    {'KAA'
-0000a090: 3a20 7b27 5245 5349 4455 4553 273a 207b  : {'RESIDUES': {
-0000a0a0: 2741 4c41 273a 2031 2c20 2741 5247 273a  'ALA': 1, 'ARG':
-0000a0b0: 2031 2c20 2741 534e 273a 2031 2c20 2741   1, 'ASN': 1, 'A
-0000a0c0: 5350 273a 2032 2c20 2747 4c55 273a 2033  SP': 2, 'GLU': 3
-0000a0d0: 2c20 2747 4c59 273a 2033 2c20 274c 4555  , 'GLY': 3, 'LEU
-0000a0e0: 273a 2032 2c20 274c 5953 273a 2032 2c20  ': 2, 'LYS': 2, 
-0000a0f0: 274d 4554 273a 2031 2c20 2750 4845 273a  'MET': 1, 'PHE':
-0000a100: 2031 2c20 2753 4552 273a 2031 2c20 2754   1, 'SER': 1, 'T
-0000a110: 4852 273a 2032 2c20 2754 5952 273a 2031  HR': 2, 'TYR': 1
-0000a120: 2c20 2756 414c 273a 2033 7d2c 2027 434c  , 'VAL': 3}, 'CL
-0000a130: 4153 5327 3a20 7b27 5231 273a 2039 2c20  ASS': {'R1': 9, 
-0000a140: 2752 3227 3a20 322c 2027 5233 273a 2035  'R2': 2, 'R3': 5
-0000a150: 2c20 2752 3427 3a20 352c 2027 5235 273a  , 'R4': 5, 'R5':
-0000a160: 2033 2c20 2752 5827 3a20 307d 7d2c 2027   3, 'RX': 0}}, '
-0000a170: 4b41 4227 3a20 7b27 5245 5349 4455 4553  KAB': {'RESIDUES
-0000a180: 273a 207b 2741 534e 273a 2031 2c20 2741  ': {'ASN': 1, 'A
-0000a190: 5350 273a 2031 2c20 2747 4c55 273a 2031  SP': 1, 'GLU': 1
-0000a1a0: 2c20 274c 4555 273a 2031 2c20 2750 4845  , 'LEU': 1, 'PHE
-0000a1b0: 273a 2031 2c20 2753 4552 273a 2031 2c20  ': 1, 'SER': 1, 
-0000a1c0: 2754 5952 273a 2031 7d2c 2027 434c 4153  'TYR': 1}, 'CLAS
-0000a1d0: 5327 3a20 7b27 5231 273a 2031 2c20 2752  S': {'R1': 1, 'R
-0000a1e0: 3227 3a20 322c 2027 5233 273a 2032 2c20  2': 2, 'R3': 2, 
-0000a1f0: 2752 3427 3a20 322c 2027 5235 273a 2030  'R4': 2, 'R5': 0
-0000a200: 2c20 2752 5827 3a20 307d 7d7d 0a0a 2020  , 'RX': 0}}}..  
-0000a210: 2020 4675 7274 6865 722c 2077 6520 6361    Further, we ca
-0000a220: 6e20 616c 736f 2070 6572 666f 726d 2063  n also perform c
-0000a230: 6176 6974 7920 6465 7465 6374 696f 6e20  avity detection 
-0000a240: 6f6e 2061 2063 7573 746f 6d20 3344 2067  on a custom 3D g
-0000a250: 7269 642c 2077 6865 7265 2077 6520 6361  rid, where we ca
-0000a260: 6e20 6578 706c 6f72 6520 636c 6f73 6564  n explore closed
-0000a270: 2072 6567 696f 6e73 2077 6974 6820 6120   regions with a 
-0000a280: 6375 7374 6f6d 2062 6f78 2c20 7768 6963  custom box, whic
-0000a290: 6820 6361 6e20 6265 2064 6566 696e 6564  h can be defined
-0000a2a0: 2062 7920 6120 2a2e 746f 6d6c 2a20 6669   by a *.toml* fi
-0000a2b0: 6c65 2028 7365 6520 6042 6f78 2063 6f6e  le (see `Box con
-0000a2c0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-0000a2d0: 7465 6d70 6c61 7465 6029 2e0a 0a20 2020  template`)...   
-0000a2e0: 203e 3e3e 2066 6e20 3d20 6f73 2e70 6174   >>> fn = os.pat
-0000a2f0: 682e 6a6f 696e 286f 732e 7061 7468 2e64  h.join(os.path.d
-0000a300: 6972 6e61 6d65 2870 794b 5646 696e 6465  irname(pyKVFinde
-0000a310: 722e 5f5f 6669 6c65 5f5f 292c 2027 6461  r.__file__), 'da
-0000a320: 7461 272c 2027 7465 7374 7327 2c20 2763  ta', 'tests', 'c
-0000a330: 7573 746f 6d2d 626f 782e 746f 6d6c 2729  ustom-box.toml')
-0000a340: 0a20 2020 203e 3e3e 2077 6974 6820 6f70  .    >>> with op
-0000a350: 656e 2866 6e2c 2027 7227 2920 6173 2066  en(fn, 'r') as f
-0000a360: 3a0a 2020 2020 2e2e 2e20 2020 2020 7072  :.    ...     pr
-0000a370: 696e 7428 662e 7265 6164 2829 290a 2020  int(f.read()).  
-0000a380: 2020 5b62 6f78 5d0a 2020 2020 7031 203d    [box].    p1 =
-0000a390: 205b 332e 3131 2c20 372e 3334 2c20 312e   [3.11, 7.34, 1.
-0000a3a0: 3539 5d0a 2020 2020 7032 203d 205b 3131  59].    p2 = [11
-0000a3b0: 2e35 312c 2037 2e33 342c 2031 2e35 395d  .51, 7.34, 1.59]
-0000a3c0: 0a20 2020 2070 3320 3d20 5b33 2e31 312c  .    p3 = [3.11,
-0000a3d0: 2031 302e 3734 2c20 312e 3539 5d0a 2020   10.74, 1.59].  
-0000a3e0: 2020 7034 203d 205b 332e 3131 2c20 372e    p4 = [3.11, 7.
-0000a3f0: 3334 2c20 362e 3139 5d0a 2020 2020 3e3e  34, 6.19].    >>
-0000a400: 3e20 7265 7375 6c74 7320 3d20 7079 4b56  > results = pyKV
-0000a410: 4669 6e64 6572 2e72 756e 5f77 6f72 6b66  Finder.run_workf
-0000a420: 6c6f 7728 7064 622c 2062 6f78 3d66 6e29  low(pdb, box=fn)
-0000a430: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
-0000a440: 0a20 2020 203c 7079 4b56 4669 6e64 6572  .    <pyKVFinder
-0000a450: 5265 7375 6c74 7320 6f62 6a65 6374 3e0a  Results object>.
-0000a460: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
-0000a470: 6361 7669 7469 6573 0a20 2020 2061 7272  cavities.    arr
-0000a480: 6179 285b 5b5b 2d31 2c20 2d31 2c20 2d31  ay([[[-1, -1, -1
-0000a490: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-0000a4a0: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-0000a4b0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-0000a4c0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-0000a4d0: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-0000a4e0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-0000a4f0: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-0000a500: 2020 2020 2020 2e2e 2e2c 0a20 2020 2020        ...,.     
-0000a510: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
-0000a520: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
-0000a530: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
-0000a540: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-0000a550: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-0000a560: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-0000a570: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-0000a580: 312c 202d 312c 202d 315d 5d2c 0a20 2020  1, -1, -1]],.   
-0000a590: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000a5a0: 2020 2020 2020 2020 5b5b 2d31 2c20 2d31          [[-1, -1
-0000a5b0: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
-0000a5c0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
-0000a5d0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-0000a5e0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-0000a5f0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000a600: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-0000a610: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
-0000a620: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
-0000a630: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-0000a640: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-0000a650: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
-0000a660: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
-0000a670: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
-0000a680: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-0000a690: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
-0000a6a0: 2e2c 202d 312c 202d 312c 202d 315d 5d5d  ., -1, -1, -1]]]
-0000a6b0: 2c20 6474 7970 653d 696e 7433 3229 0a20  , dtype=int32). 
-0000a6c0: 2020 203e 3e3e 2072 6573 756c 7473 2e73     >>> results.s
-0000a6d0: 7572 6661 6365 0a20 2020 2061 7272 6179  urface.    array
-0000a6e0: 285b 5b5b 2d31 2c20 2d31 2c20 2d31 2c20  ([[[-1, -1, -1, 
-0000a6f0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
-0000a700: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
-0000a710: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
-0000a720: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
-0000a730: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
-0000a740: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
-0000a750: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
-0000a760: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
-0000a770: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
-0000a780: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
-0000a790: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-0000a7a0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
-0000a7b0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
-0000a7c0: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
-0000a7d0: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
-0000a7e0: 202d 312c 202d 315d 5d2c 0a20 2020 2020   -1, -1]],.     
-0000a7f0: 2020 2020 2020 2e2e 2e2c 0a20 2020 2020        ...,.     
-0000a800: 2020 2020 2020 5b5b 2d31 2c20 2d31 2c20        [[-1, -1, 
-0000a810: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
-0000a820: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
-0000a830: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
-0000a840: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
-0000a850: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
-0000a860: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
-0000a870: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
-0000a880: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-0000a890: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
-0000a8a0: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
-0000a8b0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
-0000a8c0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
-0000a8d0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
-0000a8e0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000a8f0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
-0000a900: 202d 312c 202d 312c 202d 315d 5d5d 2c20   -1, -1, -1]]], 
-0000a910: 6474 7970 653d 696e 7433 3229 0a20 2020  dtype=int32).   
-0000a920: 203e 3e3e 2072 6573 756c 7473 2e6e 6361   >>> results.nca
-0000a930: 760a 2020 2020 3e3e 3e20 310a 2020 2020  v.    >>> 1.    
-0000a940: 3e3e 3e20 7265 7375 6c74 732e 766f 6c75  >>> results.volu
-0000a950: 6d65 0a20 2020 207b 274b 4141 273a 2031  me.    {'KAA': 1
-0000a960: 3135 2e37 387d 0a20 2020 203e 3e3e 2072  15.78}.    >>> r
-0000a970: 6573 756c 7473 2e61 7265 610a 2020 2020  esults.area.    
-0000a980: 7b27 4b41 4127 3a20 3333 2e39 317d 0a20  {'KAA': 33.91}. 
-0000a990: 2020 203e 3e3e 2072 6573 756c 7473 2e72     >>> results.r
-0000a9a0: 6573 6964 7565 730a 2020 2020 7b27 4b41  esidues.    {'KA
-0000a9b0: 4127 3a20 5b5b 2734 3927 2c20 2745 272c  A': [['49', 'E',
-0000a9c0: 2027 4c45 5527 5d2c 205b 2735 3027 2c20   'LEU'], ['50', 
-0000a9d0: 2745 272c 2027 474c 5927 5d2c 205b 2735  'E', 'GLY'], ['5
-0000a9e0: 3127 2c20 2745 272c 2027 5448 5227 5d2c  1', 'E', 'THR'],
-0000a9f0: 205b 2735 3727 2c20 2745 272c 2027 5641   ['57', 'E', 'VA
-0000aa00: 4c27 5d2c 205b 2737 3027 2c20 2745 272c  L'], ['70', 'E',
-0000aa10: 2027 414c 4127 5d2c 205b 2731 3034 272c   'ALA'], ['104',
-0000aa20: 2027 4527 2c20 2756 414c 275d 2c20 5b27   'E', 'VAL'], ['
-0000aa30: 3132 3127 2c20 2745 272c 2027 474c 5527  121', 'E', 'GLU'
-0000aa40: 5d2c 205b 2731 3232 272c 2027 4527 2c20  ], ['122', 'E', 
-0000aa50: 2754 5952 275d 2c20 5b27 3132 3327 2c20  'TYR'], ['123', 
-0000aa60: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
-0000aa70: 3237 272c 2027 4527 2c20 2747 4c55 275d  27', 'E', 'GLU']
-0000aa80: 2c20 5b27 3137 3027 2c20 2745 272c 2027  , ['170', 'E', '
-0000aa90: 474c 5527 5d2c 205b 2731 3731 272c 2027  GLU'], ['171', '
-0000aaa0: 4527 2c20 2741 534e 275d 2c20 5b27 3137  E', 'ASN'], ['17
-0000aab0: 3327 2c20 2745 272c 2027 4c45 5527 5d2c  3', 'E', 'LEU'],
-0000aac0: 205b 2731 3833 272c 2027 4527 2c20 2754   ['183', 'E', 'T
-0000aad0: 4852 275d 2c20 5b27 3332 3727 2c20 2745  HR'], ['327', 'E
-0000aae0: 272c 2027 5048 4527 5d5d 7d0a 2020 2020  ', 'PHE']]}.    
-0000aaf0: 3e3e 3e20 7265 7375 6c74 732e 6672 6571  >>> results.freq
-0000ab00: 7565 6e63 6965 730a 2020 2020 7b27 4b41  uencies.    {'KA
-0000ab10: 4127 3a20 7b27 5245 5349 4455 4553 273a  A': {'RESIDUES':
-0000ab20: 207b 2741 4c41 273a 2031 2c20 2741 534e   {'ALA': 1, 'ASN
-0000ab30: 273a 2031 2c20 2747 4c55 273a 2033 2c20  ': 1, 'GLU': 3, 
-0000ab40: 2747 4c59 273a 2031 2c20 274c 4555 273a  'GLY': 1, 'LEU':
-0000ab50: 2032 2c20 2750 4845 273a 2031 2c20 2754   2, 'PHE': 1, 'T
-0000ab60: 4852 273a 2032 2c20 2754 5952 273a 2031  HR': 2, 'TYR': 1
-0000ab70: 2c20 2756 414c 273a 2033 7d2c 2027 434c  , 'VAL': 3}, 'CL
-0000ab80: 4153 5327 3a20 7b27 5231 273a 2037 2c20  ASS': {'R1': 7, 
-0000ab90: 2752 3227 3a20 322c 2027 5233 273a 2033  'R2': 2, 'R3': 3
-0000aba0: 2c20 2752 3427 3a20 332c 2027 5235 273a  , 'R4': 3, 'R5':
-0000abb0: 2030 2c20 2752 5827 3a20 307d 7d7d 0a0a   0, 'RX': 0}}}..
-0000abc0: 2020 2020 486f 7765 7665 722c 2075 7365      However, use
-0000abd0: 7273 206d 6179 206f 7074 2074 6f20 7065  rs may opt to pe
-0000abe0: 7266 6f72 6d20 7468 6520 2a2a 6675 6c6c  rform the **full
-0000abf0: 2077 6f72 6b66 6c6f 772a 2a20 666f 7220   workflow** for 
-0000ac00: 6361 7669 7479 2064 6574 6563 7469 6f6e  cavity detection
-0000ac10: 2077 6974 6820 7370 6174 6961 6c20 2873   with spatial (s
-0000ac20: 7572 6661 6365 2070 6f69 6e74 732c 2076  urface points, v
-0000ac30: 6f6c 756d 6520 616e 6420 6172 6561 292c  olume and area),
-0000ac40: 2063 6f6e 7374 6974 7574 696f 6e61 6c20   constitutional 
-0000ac50: 2869 6e74 6572 6661 6365 2072 6573 6964  (interface resid
-0000ac60: 7565 7320 616e 6420 7468 6569 7220 6672  ues and their fr
-0000ac70: 6571 7565 6e63 6965 7329 2c20 6879 6472  equencies), hydr
-0000ac80: 6f70 6174 6879 2061 6e64 2064 6570 7468  opathy and depth
-0000ac90: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-0000aca0: 6e2e 2054 6869 7320 6675 6c6c 2077 6f72  n. This full wor
-0000acb0: 6b66 6c6f 7720 6361 6e20 6265 2072 756e  kflow can be run
-0000acc0: 2077 6974 6820 6f6e 6520 636f 6d6d 616e   with one comman
-0000acd0: 6420 6279 2073 6574 7469 6e67 2073 6f6d  d by setting som
-0000ace0: 6520 7061 7261 6d65 7465 7273 206f 6620  e parameters of 
-0000acf0: 6060 7275 6e5f 776f 726b 666c 6f77 6060  ``run_workflow``
-0000ad00: 2066 756e 6374 696f 6e3a 0a0a 2020 2020   function:..    
-0000ad10: 3e3e 3e20 7265 7375 6c74 7320 3d20 7079  >>> results = py
-0000ad20: 4b56 4669 6e64 6572 2e72 756e 5f77 6f72  KVFinder.run_wor
-0000ad30: 6b66 6c6f 7728 7064 622c 2069 6e63 6c75  kflow(pdb, inclu
-0000ad40: 6465 5f64 6570 7468 3d54 7275 652c 2069  de_depth=True, i
-0000ad50: 6e63 6c75 6465 5f68 7964 726f 7061 7468  nclude_hydropath
-0000ad60: 793d 5472 7565 2c20 6879 6472 6f70 686f  y=True, hydropho
-0000ad70: 6269 6369 7479 5f73 6361 6c65 3d27 4569  bicity_scale='Ei
-0000ad80: 7365 6e62 6572 6757 6569 7373 2729 0a20  senbergWeiss'). 
-0000ad90: 2020 203e 3e3e 2072 6573 756c 7473 2e64     >>> results.d
-0000ada0: 6570 7468 730a 2020 2020 6172 7261 7928  epths.    array(
-0000adb0: 5b5b 5b30 2e2c 2030 2e2c 2030 2e2c 202e  [[[0., 0., 0., .
-0000adc0: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
-0000add0: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
-0000ade0: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
-0000adf0: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
-0000ae00: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000ae10: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000ae20: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000ae30: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-0000ae40: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
-0000ae50: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
-0000ae60: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000ae70: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
-0000ae80: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
-0000ae90: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
-0000aea0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-0000aeb0: 302e 2c20 302e 5d5d 2c0a 2020 2020 2020  0., 0.]],.      
-0000aec0: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-0000aed0: 2020 2020 205b 5b30 2e2c 2030 2e2c 2030       [[0., 0., 0
-0000aee0: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
-0000aef0: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
-0000af00: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
-0000af10: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
-0000af20: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000af30: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000af40: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000af50: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-0000af60: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000af70: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000af80: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000af90: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-0000afa0: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-0000afb0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-0000afc0: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-0000afd0: 302e 2c20 302e 2c20 302e 5d5d 5d29 0a20  0., 0., 0.]]]). 
-0000afe0: 2020 203e 3e3e 2072 6573 756c 7473 2e73     >>> results.s
-0000aff0: 6361 6c65 730a 2020 2020 6172 7261 7928  cales.    array(
-0000b000: 5b5b 5b30 2e2c 2030 2e2c 2030 2e2c 202e  [[[0., 0., 0., .
-0000b010: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d2c  .., 0., 0., 0.],
-0000b020: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
-0000b030: 2c20 302e 2c20 302e 2c20 2e2e 2e2c 2030  , 0., 0., ..., 0
-0000b040: 2e2c 2030 2e2c 2030 2e5d 2c0a 2020 2020  ., 0., 0.],.    
-0000b050: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000b060: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000b070: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000b080: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
-0000b090: 2020 2020 5b30 2e2c 2030 2e2c 2030 2e2c      [0., 0., 0.,
-0000b0a0: 202e 2e2e 2c20 302e 2c20 302e 2c20 302e   ..., 0., 0., 0.
-0000b0b0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0000b0c0: 302e 2c20 302e 2c20 302e 2c20 2e2e 2e2c  0., 0., 0., ...,
-0000b0d0: 2030 2e2c 2030 2e2c 2030 2e5d 2c0a 2020   0., 0., 0.],.  
-0000b0e0: 2020 2020 2020 2020 2020 5b30 2e2c 2030            [0., 0
-0000b0f0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
-0000b100: 302e 2c20 302e 5d5d 2c0a 2020 2020 2020  0., 0.]],.      
-0000b110: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
-0000b120: 2020 2020 205b 5b30 2e2c 2030 2e2c 2030       [[0., 0., 0
-0000b130: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
-0000b140: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
-0000b150: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
-0000b160: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
-0000b170: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
-0000b180: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
-0000b190: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
-0000b1a0: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
-0000b1b0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
-0000b1c0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
-0000b1d0: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
-0000b1e0: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
-0000b1f0: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
-0000b200: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
-0000b210: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
-0000b220: 302e 2c20 302e 2c20 302e 5d5d 5d29 0a20  0., 0., 0.]]]). 
-0000b230: 2020 203e 3e3e 2072 6573 756c 7473 2e61     >>> results.a
-0000b240: 7667 5f64 6570 7468 0a20 2020 207b 274b  vg_depth.    {'K
-0000b250: 4141 273a 2031 2e33 352c 2027 4b41 4227  AA': 1.35, 'KAB'
-0000b260: 3a20 302e 3931 2c20 274b 4143 273a 2030  : 0.91, 'KAC': 0
-0000b270: 2e36 382c 2027 4b41 4427 3a20 302e 3332  .68, 'KAD': 0.32
-0000b280: 2c20 274b 4145 273a 2030 2e39 392c 2027  , 'KAE': 0.99, '
-0000b290: 4b41 4627 3a20 302e 3234 2c20 274b 4147  KAF': 0.24, 'KAG
-0000b2a0: 273a 2030 2e31 2c20 274b 4148 273a 2033  ': 0.1, 'KAH': 3
-0000b2b0: 2e39 312c 2027 4b41 4927 3a20 302e 302c  .91, 'KAI': 0.0,
-0000b2c0: 2027 4b41 4a27 3a20 302e 3936 2c20 274b   'KAJ': 0.96, 'K
-0000b2d0: 414b 273a 2030 2e30 2c20 274b 414c 273a  AK': 0.0, 'KAL':
-0000b2e0: 2031 2e30 372c 2027 4b41 4d27 3a20 302e   1.07, 'KAM': 0.
-0000b2f0: 3234 2c20 274b 414e 273a 2030 2e30 2c20  24, 'KAN': 0.0, 
-0000b300: 274b 414f 273a 2030 2e32 392c 2027 4b41  'KAO': 0.29, 'KA
-0000b310: 5027 3a20 302e 372c 2027 4b41 5127 3a20  P': 0.7, 'KAQ': 
-0000b320: 302e 3232 2c20 274b 4152 273a 2030 2e31  0.22, 'KAR': 0.1
-0000b330: 327d 0a20 2020 203e 3e3e 2072 6573 756c  2}.    >>> resul
-0000b340: 7473 2e6d 6178 5f64 6570 7468 0a20 2020  ts.max_depth.   
-0000b350: 207b 274b 4141 273a 2033 2e37 392c 2027   {'KAA': 3.79, '
-0000b360: 4b41 4227 3a20 322e 3638 2c20 274b 4143  KAB': 2.68, 'KAC
-0000b370: 273a 2032 2e36 322c 2027 4b41 4427 3a20  ': 2.62, 'KAD': 
-0000b380: 302e 3835 2c20 274b 4145 273a 2033 2e30  0.85, 'KAE': 3.0
-0000b390: 2c20 274b 4146 273a 2030 2e38 352c 2027  , 'KAF': 0.85, '
-0000b3a0: 4b41 4727 3a20 302e 362c 2027 4b41 4827  KAG': 0.6, 'KAH'
-0000b3b0: 3a20 3130 2e37 332c 2027 4b41 4927 3a20  : 10.73, 'KAI': 
-0000b3c0: 302e 302c 2027 4b41 4a27 3a20 322e 3234  0.0, 'KAJ': 2.24
-0000b3d0: 2c20 274b 414b 273a 2030 2e30 2c20 274b  , 'KAK': 0.0, 'K
-0000b3e0: 414c 273a 2033 2e30 2c20 274b 414d 273a  AL': 3.0, 'KAM':
-0000b3f0: 2031 2e32 2c20 274b 414e 273a 2030 2e30   1.2, 'KAN': 0.0
-0000b400: 2c20 274b 414f 273a 2031 2e30 342c 2027  , 'KAO': 1.04, '
-0000b410: 4b41 5027 3a20 322e 3038 2c20 274b 4151  KAP': 2.08, 'KAQ
-0000b420: 273a 2030 2e38 352c 2027 4b41 5227 3a20  ': 0.85, 'KAR': 
-0000b430: 302e 367d 0a20 2020 203e 3e3e 2072 6573  0.6}.    >>> res
-0000b440: 756c 7473 2e61 7667 5f68 7964 726f 7061  ults.avg_hydropa
-0000b450: 7468 790a 2020 2020 7b27 4b41 4127 3a20  thy.    {'KAA': 
-0000b460: 2d30 2e37 332c 2027 4b41 4227 3a20 2d30  -0.73, 'KAB': -0
-0000b470: 2e30 352c 2027 4b41 4327 3a20 2d30 2e30  .05, 'KAC': -0.0
-0000b480: 372c 2027 4b41 4427 3a20 2d30 2e36 322c  7, 'KAD': -0.62,
-0000b490: 2027 4b41 4527 3a20 2d30 2e38 312c 2027   'KAE': -0.81, '
-0000b4a0: 4b41 4627 3a20 2d30 2e31 342c 2027 4b41  KAF': -0.14, 'KA
-0000b4b0: 4727 3a20 2d30 2e33 332c 2027 4b41 4827  G': -0.33, 'KAH'
-0000b4c0: 3a20 2d30 2e31 372c 2027 4b41 4927 3a20  : -0.17, 'KAI': 
-0000b4d0: 2d30 2e34 2c20 274b 414a 273a 2030 2e36  -0.4, 'KAJ': 0.6
-0000b4e0: 322c 2027 4b41 4b27 3a20 2d30 2e39 392c  2, 'KAK': -0.99,
-0000b4f0: 2027 4b41 4c27 3a20 302e 3336 2c20 274b   'KAL': 0.36, 'K
-0000b500: 414d 273a 202d 302e 3333 2c20 274b 414e  AM': -0.33, 'KAN
-0000b510: 273a 2030 2e31 382c 2027 4b41 4f27 3a20  ': 0.18, 'KAO': 
-0000b520: 302e 3838 2c20 274b 4150 273a 202d 302e  0.88, 'KAP': -0.
-0000b530: 3936 2c20 274b 4151 273a 2030 2e34 382c  96, 'KAQ': 0.48,
-0000b540: 2027 4b41 5227 3a20 302e 3234 2c20 2745   'KAR': 0.24, 'E
-0000b550: 6973 656e 6265 7267 5765 6973 7327 3a20  isenbergWeiss': 
-0000b560: 5b2d 312e 3432 2c20 322e 365d 7d0a 2020  [-1.42, 2.6]}.  
-0000b570: 2020 2222 220a 2020 2020 6966 2076 6572    """.    if ver
-0000b580: 626f 7365 3a0a 2020 2020 2020 2020 7072  bose:.        pr
-0000b590: 696e 7428 223e 204c 6f61 6469 6e67 2061  int("> Loading a
-0000b5a0: 746f 6d69 6320 6469 6374 696f 6e61 7279  tomic dictionary
-0000b5b0: 2066 696c 6522 290a 2020 2020 6966 2076   file").    if v
-0000b5c0: 6477 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dw is not None:.
-0000b5d0: 2020 2020 2020 2020 7664 7720 3d20 7265          vdw = re
-0000b5e0: 6164 5f76 6477 2876 6477 290a 2020 2020  ad_vdw(vdw).    
-0000b5f0: 656c 7365 3a0a 2020 2020 2020 2020 7664  else:.        vd
-0000b600: 7720 3d20 7265 6164 5f76 6477 2856 4457  w = read_vdw(VDW
-0000b610: 290a 0a20 2020 2069 6620 7665 7262 6f73  )..    if verbos
-0000b620: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-0000b630: 2822 3e20 5265 6164 696e 6720 5044 4220  ("> Reading PDB 
-0000b640: 636f 6f72 6469 6e61 7465 7322 290a 2020  coordinates").  
-0000b650: 2020 6966 2069 6e70 7574 2e65 6e64 7377    if input.endsw
-0000b660: 6974 6828 222e 7064 6222 293a 0a20 2020  ith(".pdb"):.   
-0000b670: 2020 2020 2061 746f 6d69 6320 3d20 7265       atomic = re
-0000b680: 6164 5f70 6462 2869 6e70 7574 2c20 7664  ad_pdb(input, vd
-0000b690: 772c 206d 6f64 656c 290a 2020 2020 656c  w, model).    el
-0000b6a0: 6966 2069 6e70 7574 2e65 6e64 7377 6974  if input.endswit
-0000b6b0: 6828 222e 7879 7a22 293a 0a20 2020 2020  h(".xyz"):.     
-0000b6c0: 2020 2061 746f 6d69 6320 3d20 7265 6164     atomic = read
-0000b6d0: 5f78 797a 2869 6e70 7574 2c20 7664 7729  _xyz(input, vdw)
-0000b6e0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000b6f0: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-0000b700: 6f72 2822 6074 6172 6765 7460 206d 7573  or("`target` mus
-0000b710: 7420 6861 7665 202e 7064 6220 6f72 202e  t have .pdb or .
-0000b720: 7879 7a20 6578 7465 6e73 696f 6e2e 2229  xyz extension.")
-0000b730: 0a0a 2020 2020 6966 206c 6967 616e 643a  ..    if ligand:
-0000b740: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
-0000b750: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
-0000b760: 2070 7269 6e74 2822 3e20 5265 6164 696e   print("> Readin
-0000b770: 6720 6c69 6761 6e64 2063 6f6f 7264 696e  g ligand coordin
-0000b780: 6174 6573 2229 0a20 2020 2020 2020 2069  ates").        i
-0000b790: 6620 6c69 6761 6e64 2e65 6e64 7377 6974  f ligand.endswit
-0000b7a0: 6828 222e 7064 6222 293a 0a20 2020 2020  h(".pdb"):.     
-0000b7b0: 2020 2020 2020 206c 6174 6f6d 6963 203d         latomic =
-0000b7c0: 2072 6561 645f 7064 6228 6c69 6761 6e64   read_pdb(ligand
-0000b7d0: 2c20 7664 7729 0a20 2020 2020 2020 2065  , vdw).        e
-0000b7e0: 6c69 6620 6c69 6761 6e64 2e65 6e64 7377  lif ligand.endsw
-0000b7f0: 6974 6828 222e 7879 7a22 293a 0a20 2020  ith(".xyz"):.   
-0000b800: 2020 2020 2020 2020 206c 6174 6f6d 6963           latomic
-0000b810: 203d 2072 6561 645f 7879 7a28 6c69 6761   = read_xyz(liga
-0000b820: 6e64 2c20 7664 7729 0a20 2020 2020 2020  nd, vdw).       
-0000b830: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000b840: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-0000b850: 6f72 2822 606c 6967 616e 6460 206d 7573  or("`ligand` mus
-0000b860: 7420 6861 7665 202e 7064 6220 6f72 202e  t have .pdb or .
-0000b870: 7879 7a20 6578 7465 6e73 696f 6e2e 2229  xyz extension.")
-0000b880: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000b890: 2020 206c 6174 6f6d 6963 203d 204e 6f6e     latomic = Non
-0000b8a0: 650a 0a20 2020 2069 6620 7665 7262 6f73  e..    if verbos
-0000b8b0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-0000b8c0: 2822 3e20 4361 6c63 756c 6174 696e 6720  ("> Calculating 
-0000b8d0: 3344 2067 7269 6420 6469 6d65 6e73 696f  3D grid dimensio
-0000b8e0: 6e73 2229 0a20 2020 2069 6620 626f 783a  ns").    if box:
-0000b8f0: 0a20 2020 2020 2020 2023 2047 6574 2076  .        # Get v
-0000b900: 6572 7469 6365 7320 6672 6f6d 2066 696c  ertices from fil
-0000b910: 650a 2020 2020 2020 2020 7665 7274 6963  e.        vertic
-0000b920: 6573 2c20 6174 6f6d 6963 203d 2067 6574  es, atomic = get
-0000b930: 5f76 6572 7469 6365 735f 6672 6f6d 5f66  _vertices_from_f
-0000b940: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-0000b950: 2062 6f78 2c20 6174 6f6d 6963 2c20 7374   box, atomic, st
-0000b960: 6570 2c20 7072 6f62 655f 696e 2c20 7072  ep, probe_in, pr
-0000b970: 6f62 655f 6f75 742c 206e 7468 7265 6164  obe_out, nthread
-0000b980: 730a 2020 2020 2020 2020 290a 0a20 2020  s.        )..   
-0000b990: 2020 2020 2023 2053 6574 2066 6c61 6720       # Set flag 
-0000b9a0: 746f 2062 6f6f 6c65 616e 0a20 2020 2020  to boolean.     
-0000b9b0: 2020 2062 6f78 203d 2054 7275 650a 2020     box = True.  
-0000b9c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b9d0: 2320 4765 7420 7665 7274 6963 6573 2066  # Get vertices f
-0000b9e0: 726f 6d20 696e 7075 740a 2020 2020 2020  rom input.      
-0000b9f0: 2020 7665 7274 6963 6573 203d 2067 6574    vertices = get
-0000ba00: 5f76 6572 7469 6365 7328 6174 6f6d 6963  _vertices(atomic
-0000ba10: 2c20 7072 6f62 655f 6f75 742c 2073 7465  , probe_out, ste
-0000ba20: 7029 0a0a 2020 2020 2020 2020 2320 5365  p)..        # Se
-0000ba30: 7420 666c 6167 2074 6f20 626f 6f6c 6561  t flag to boolea
-0000ba40: 6e0a 2020 2020 2020 2020 626f 7820 3d20  n.        box = 
-0000ba50: 4661 6c73 650a 0a20 2020 2023 2043 616c  False..    # Cal
-0000ba60: 6375 6c61 7465 2064 6973 7461 6e63 6520  culate distance 
-0000ba70: 6265 7477 6565 6e20 706f 696e 7473 0a20  between points. 
-0000ba80: 2020 206e 782c 206e 792c 206e 7a20 3d20     nx, ny, nz = 
-0000ba90: 5f67 6574 5f64 696d 656e 7369 6f6e 7328  _get_dimensions(
-0000baa0: 7665 7274 6963 6573 2c20 7374 6570 290a  vertices, step).
-0000bab0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-0000bac0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-0000bad0: 4469 6d65 6e73 696f 6e73 3a20 286e 783a  Dimensions: (nx:
-0000bae0: 7b6e 787d 2c20 6e79 3a7b 6e79 7d2c 206e  {nx}, ny:{ny}, n
-0000baf0: 7a3a 7b6e 7a7d 2922 290a 0a20 2020 2023  z:{nz})")..    #
-0000bb00: 2043 616c 6375 6c61 7465 2073 696e 2061   Calculate sin a
-0000bb10: 6e64 2063 6f73 206f 6620 616e 676c 6573  nd cos of angles
-0000bb20: 2061 2061 6e64 2062 0a20 2020 2073 696e   a and b.    sin
-0000bb30: 636f 7320 3d20 5f67 6574 5f73 696e 636f  cos = _get_sinco
-0000bb40: 7328 7665 7274 6963 6573 290a 2020 2020  s(vertices).    
-0000bb50: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-0000bb60: 2020 2020 7072 696e 7428 6622 7369 6e61      print(f"sina
-0000bb70: 3a20 7b73 696e 636f 735b 305d 3a2e 3266  : {sincos[0]:.2f
-0000bb80: 7d5c 7473 696e 623a 207b 7369 6e63 6f73  }\tsinb: {sincos
-0000bb90: 5b32 5d3a 2e32 667d 2229 0a20 2020 2020  [2]:.2f}").     
-0000bba0: 2020 2070 7269 6e74 2866 2263 6f73 613a     print(f"cosa:
-0000bbb0: 207b 7369 6e63 6f73 5b31 5d3a 2e32 667d   {sincos[1]:.2f}
-0000bbc0: 5c74 636f 7362 3a20 7b73 696e 636f 735b  \tcosb: {sincos[
-0000bbd0: 335d 3a2e 3266 7d22 290a 0a20 2020 2023  3]:.2f}")..    #
-0000bbe0: 2043 6176 6974 7920 6465 7465 6374 696f   Cavity detectio
-0000bbf0: 6e0a 2020 2020 6e63 6176 2c20 6361 7669  n.    ncav, cavi
-0000bc00: 7469 6573 203d 2064 6574 6563 7428 0a20  ties = detect(. 
-0000bc10: 2020 2020 2020 2061 746f 6d69 632c 0a20         atomic,. 
-0000bc20: 2020 2020 2020 2076 6572 7469 6365 732c         vertices,
-0000bc30: 0a20 2020 2020 2020 2073 7465 702c 0a20  .        step,. 
-0000bc40: 2020 2020 2020 2070 726f 6265 5f69 6e2c         probe_in,
-0000bc50: 0a20 2020 2020 2020 2070 726f 6265 5f6f  .        probe_o
-0000bc60: 7574 2c0a 2020 2020 2020 2020 7265 6d6f  ut,.        remo
-0000bc70: 7661 6c5f 6469 7374 616e 6365 2c0a 2020  val_distance,.  
-0000bc80: 2020 2020 2020 766f 6c75 6d65 5f63 7574        volume_cut
-0000bc90: 6f66 662c 0a20 2020 2020 2020 206c 6174  off,.        lat
-0000bca0: 6f6d 6963 2c0a 2020 2020 2020 2020 6c69  omic,.        li
-0000bcb0: 6761 6e64 5f63 7574 6f66 662c 0a20 2020  gand_cutoff,.   
-0000bcc0: 2020 2020 2062 6f78 2c0a 2020 2020 2020       box,.      
-0000bcd0: 2020 7375 7266 6163 652c 0a20 2020 2020    surface,.     
-0000bce0: 2020 206e 7468 7265 6164 732c 0a20 2020     nthreads,.   
-0000bcf0: 2020 2020 2076 6572 626f 7365 2c0a 2020       verbose,.  
-0000bd00: 2020 290a 0a20 2020 2069 6620 6e63 6176    )..    if ncav
-0000bd10: 203e 2030 3a0a 2020 2020 2020 2020 2320   > 0:.        # 
-0000bd20: 5370 6174 6961 6c20 6368 6172 6163 7465  Spatial characte
-0000bd30: 7269 7a61 7469 6f6e 0a20 2020 2020 2020  rization.       
-0000bd40: 2073 7572 6661 6365 2c20 766f 6c75 6d65   surface, volume
-0000bd50: 2c20 6172 6561 203d 2073 7061 7469 616c  , area = spatial
-0000bd60: 2863 6176 6974 6965 732c 2073 7465 702c  (cavities, step,
-0000bd70: 204e 6f6e 652c 206e 7468 7265 6164 732c   None, nthreads,
-0000bd80: 2076 6572 626f 7365 290a 0a20 2020 2020   verbose)..     
-0000bd90: 2020 2023 2043 6f6e 7374 6974 7574 696f     # Constitutio
-0000bda0: 6e61 6c20 6368 6172 6163 7465 7269 7a61  nal characteriza
-0000bdb0: 7469 6f6e 0a20 2020 2020 2020 2072 6573  tion.        res
-0000bdc0: 6964 7565 7320 3d20 636f 6e73 7469 7475  idues = constitu
-0000bdd0: 7469 6f6e 616c 280a 2020 2020 2020 2020  tional(.        
-0000bde0: 2020 2020 6361 7669 7469 6573 2c0a 2020      cavities,.  
-0000bdf0: 2020 2020 2020 2020 2020 6174 6f6d 6963            atomic
-0000be00: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
-0000be10: 7274 6963 6573 2c0a 2020 2020 2020 2020  rtices,.        
-0000be20: 2020 2020 7374 6570 2c0a 2020 2020 2020      step,.      
-0000be30: 2020 2020 2020 7072 6f62 655f 696e 2c0a        probe_in,.
-0000be40: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
-0000be50: 7265 5f62 6163 6b62 6f6e 652c 0a20 2020  re_backbone,.   
-0000be60: 2020 2020 2020 2020 204e 6f6e 652c 0a20           None,. 
-0000be70: 2020 2020 2020 2020 2020 206e 7468 7265             nthre
-0000be80: 6164 732c 0a20 2020 2020 2020 2020 2020  ads,.           
-0000be90: 2076 6572 626f 7365 2c0a 2020 2020 2020   verbose,.      
-0000bea0: 2020 290a 2020 2020 2020 2020 6672 6571    ).        freq
-0000beb0: 7565 6e63 6965 7320 3d20 6361 6c63 756c  uencies = calcul
-0000bec0: 6174 655f 6672 6571 7565 6e63 6965 7328  ate_frequencies(
-0000bed0: 7265 7369 6475 6573 290a 0a20 2020 2020  residues)..     
-0000bee0: 2020 2023 2044 6570 7468 2063 6861 7261     # Depth chara
-0000bef0: 6374 6572 697a 6174 696f 6e0a 2020 2020  cterization.    
-0000bf00: 2020 2020 6966 2069 6e63 6c75 6465 5f64      if include_d
-0000bf10: 6570 7468 3a0a 2020 2020 2020 2020 2020  epth:.          
-0000bf20: 2020 6465 7074 6873 2c20 6d61 785f 6465    depths, max_de
-0000bf30: 7074 682c 2061 7667 5f64 6570 7468 203d  pth, avg_depth =
-0000bf40: 2064 6570 7468 280a 2020 2020 2020 2020   depth(.        
-0000bf50: 2020 2020 2020 2020 6361 7669 7469 6573          cavities
-0000bf60: 2c20 7374 6570 2c20 4e6f 6e65 2c20 6e74  , step, None, nt
-0000bf70: 6872 6561 6473 2c20 7665 7262 6f73 650a  hreads, verbose.
-0000bf80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000bf90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000bfa0: 2020 2020 2020 2020 6465 7074 6873 2c20          depths, 
-0000bfb0: 6d61 785f 6465 7074 682c 2061 7667 5f64  max_depth, avg_d
-0000bfc0: 6570 7468 203d 204e 6f6e 652c 204e 6f6e  epth = None, Non
-0000bfd0: 652c 204e 6f6e 650a 0a20 2020 2020 2020  e, None..       
-0000bfe0: 2023 2048 7964 726f 7061 7468 7920 6879   # Hydropathy hy
-0000bff0: 6472 6f70 686f 6269 6369 7479 2073 6361  drophobicity sca
-0000c000: 6c65 730a 2020 2020 2020 2020 6966 2069  les.        if i
-0000c010: 6e63 6c75 6465 5f68 7964 726f 7061 7468  nclude_hydropath
-0000c020: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0000c030: 6361 6c65 732c 2061 7667 5f68 7964 726f  cales, avg_hydro
-0000c040: 7061 7468 7920 3d20 6879 6472 6f70 6174  pathy = hydropat
-0000c050: 6879 280a 2020 2020 2020 2020 2020 2020  hy(.            
-0000c060: 2020 2020 7375 7266 6163 652c 0a20 2020      surface,.   
-0000c070: 2020 2020 2020 2020 2020 2020 2061 746f               ato
-0000c080: 6d69 632c 0a20 2020 2020 2020 2020 2020  mic,.           
-0000c090: 2020 2020 2076 6572 7469 6365 732c 0a20       vertices,. 
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c0b0: 7465 702c 0a20 2020 2020 2020 2020 2020  tep,.           
-0000c0c0: 2020 2020 2070 726f 6265 5f69 6e2c 0a20       probe_in,. 
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000c0e0: 7964 726f 7068 6f62 6963 6974 795f 7363  ydrophobicity_sc
-0000c0f0: 616c 652c 0a20 2020 2020 2020 2020 2020  ale,.           
-0000c100: 2020 2020 2069 676e 6f72 655f 6261 636b       ignore_back
-0000c110: 626f 6e65 2c0a 2020 2020 2020 2020 2020  bone,.          
-0000c120: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-0000c130: 2020 2020 2020 2020 2020 2020 6e74 6872              nthr
-0000c140: 6561 6473 2c0a 2020 2020 2020 2020 2020  eads,.          
-0000c150: 2020 2020 2020 7665 7262 6f73 652c 0a20        verbose,. 
-0000c160: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c170: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c180: 2020 2020 2020 2073 6361 6c65 732c 2061         scales, a
-0000c190: 7667 5f68 7964 726f 7061 7468 7920 3d20  vg_hydropathy = 
-0000c1a0: 4e6f 6e65 2c20 4e6f 6e65 0a20 2020 2065  None, None.    e
-0000c1b0: 6c73 653a 0a20 2020 2020 2020 2070 7269  lse:.        pri
-0000c1c0: 6e74 2822 5761 726e 696e 673a 204e 6f20  nt("Warning: No 
-0000c1d0: 6361 7669 7469 6573 2064 6574 6563 7465  cavities detecte
-0000c1e0: 642c 2072 6574 7572 6e69 6e67 204e 6f6e  d, returning Non
-0000c1f0: 6521 2229 0a20 2020 2020 2020 2072 6574  e!").        ret
-0000c200: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2320  urn None..    # 
-0000c210: 5265 7475 726e 2064 6963 740a 2020 2020  Return dict.    
-0000c220: 7265 7375 6c74 7320 3d20 7079 4b56 4669  results = pyKVFi
-0000c230: 6e64 6572 5265 7375 6c74 7328 0a20 2020  nderResults(.   
-0000c240: 2020 2020 2063 6176 6974 6965 732c 0a20       cavities,. 
-0000c250: 2020 2020 2020 2073 7572 6661 6365 2c0a         surface,.
-0000c260: 2020 2020 2020 2020 6465 7074 6873 2c0a          depths,.
-0000c270: 2020 2020 2020 2020 7363 616c 6573 2c0a          scales,.
-0000c280: 2020 2020 2020 2020 766f 6c75 6d65 2c0a          volume,.
-0000c290: 2020 2020 2020 2020 6172 6561 2c0a 2020          area,.  
-0000c2a0: 2020 2020 2020 6d61 785f 6465 7074 682c        max_depth,
-0000c2b0: 0a20 2020 2020 2020 2061 7667 5f64 6570  .        avg_dep
-0000c2c0: 7468 2c0a 2020 2020 2020 2020 6176 675f  th,.        avg_
-0000c2d0: 6879 6472 6f70 6174 6879 2c0a 2020 2020  hydropathy,.    
-0000c2e0: 2020 2020 7265 7369 6475 6573 2c0a 2020      residues,.  
-0000c2f0: 2020 2020 2020 6672 6571 7565 6e63 6965        frequencie
-0000c300: 732c 0a20 2020 2020 2020 2076 6572 7469  s,.        verti
-0000c310: 6365 732c 0a20 2020 2020 2020 2073 7465  ces,.        ste
-0000c320: 702c 0a20 2020 2020 2020 2069 6e70 7574  p,.        input
-0000c330: 2c0a 2020 2020 2020 2020 6c69 6761 6e64  ,.        ligand
-0000c340: 2c0a 2020 2020 290a 0a20 2020 2072 6574  ,.    )..    ret
-0000c350: 7572 6e20 7265 7375 6c74 730a 0a0a 636c  urn results...cl
-0000c360: 6173 7320 4d6f 6c65 6375 6c65 286f 626a  ass Molecule(obj
-0000c370: 6563 7429 3a0a 2020 2020 2222 2241 2063  ect):.    """A c
-0000c380: 6c61 7373 2066 6f72 2072 6570 7265 7365  lass for represe
-0000c390: 6e74 696e 6720 6d6f 6c65 6375 6c61 7220  nting molecular 
-0000c3a0: 7374 7275 6374 7572 6573 2e0a 0a20 2020  structures...   
-0000c3b0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000c3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d  ----------.    m
-0000c3d0: 6f6c 6563 756c 6520 3a20 556e 696f 6e5b  olecule : Union[
-0000c3e0: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-0000c3f0: 685d 0a20 2020 2020 2020 2041 2066 696c  h].        A fil
-0000c400: 6520 7061 7468 2074 6f20 7468 6520 6d6f  e path to the mo
-0000c410: 6c65 6375 6c65 2069 6e20 6569 7468 6572  lecule in either
-0000c420: 2050 4442 206f 7220 5859 5a20 666f 726d   PDB or XYZ form
-0000c430: 6174 0a20 2020 2072 6164 6969 203a 2055  at.    radii : U
-0000c440: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-0000c450: 622e 5061 7468 2c20 4469 6374 5b73 7472  b.Path, Dict[str
-0000c460: 2c20 416e 795d 5d2c 206f 7074 696f 6e61  , Any]], optiona
-0000c470: 6c0a 2020 2020 2020 2020 4120 6669 6c65  l.        A file
-0000c480: 2070 6174 6820 746f 2061 2076 616e 2064   path to a van d
-0000c490: 6572 2057 6161 6c73 2072 6164 6969 2066  er Waals radii f
-0000c4a0: 696c 6520 6f72 2061 2064 6963 7469 6f6e  ile or a diction
-0000c4b0: 6172 7920 6f66 2056 4457 2072 6164 6969  ary of VDW radii
-0000c4c0: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-0000c4d0: 652e 2049 6620 4e6f 6e65 2c20 6170 706c  e. If None, appl
-0000c4e0: 7920 7468 6520 6275 696c 742d 696e 2076  y the built-in v
-0000c4f0: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
-0000c500: 6969 2066 696c 653a 2060 7664 772e 6461  ii file: `vdw.da
-0000c510: 7460 2e0a 2020 2020 6d6f 6465 6c20 3a20  t`..    model : 
-0000c520: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0000c530: 2020 2020 2020 5468 6520 6d6f 6465 6c20        The model 
-0000c540: 6e75 6d62 6572 206f 6620 6120 6d75 6c74  number of a mult
-0000c550: 692d 6d6f 6465 6c20 5044 4220 6669 6c65  i-model PDB file
-0000c560: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-0000c570: 652e 2049 6620 4e6f 6e65 2c20 6b65 6570  e. If None, keep
-0000c580: 2061 746f 6d73 2066 726f 6d20 616c 6c20   atoms from all 
-0000c590: 6d6f 6465 6c73 2e0a 2020 2020 6e74 6872  models..    nthr
-0000c5a0: 6561 6473 203a 2069 6e74 2c20 6f70 7469  eads : int, opti
-0000c5b0: 6f6e 616c 0a20 2020 2020 2020 204e 756d  onal.        Num
-0000c5c0: 6265 7220 6f66 2074 6872 6561 6473 2c20  ber of threads, 
-0000c5d0: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
-0000c5e0: 2049 6620 4e6f 6e65 2c20 7468 6520 6e75   If None, the nu
-0000c5f0: 6d62 6572 206f 6620 7468 7265 6164 7320  mber of threads 
-0000c600: 6973 2060 6f73 2e63 7075 5f63 6f75 6e74  is `os.cpu_count
-0000c610: 2829 202d 2031 602e 0a20 2020 2076 6572  () - 1`..    ver
-0000c620: 626f 7365 203a 2062 6f6f 6c2c 206f 7074  bose : bool, opt
-0000c630: 696f 6e61 6c0a 2020 2020 2020 2020 5072  ional.        Pr
-0000c640: 696e 7420 6578 7472 6120 696e 666f 726d  int extra inform
-0000c650: 6174 696f 6e20 746f 2073 7461 6e64 6172  ation to standar
-0000c660: 6420 6f75 7470 7574 2c20 6279 2064 6566  d output, by def
-0000c670: 6175 6c74 2046 616c 7365 2e0a 0a20 2020  ault False...   
-0000c680: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
-0000c690: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 205f  ----------.    _
-0000c6a0: 6174 6f6d 6963 203a 206e 756d 7079 2e6e  atomic : numpy.n
-0000c6b0: 6461 7272 6179 0a20 2020 2020 2020 2041  darray.        A
-0000c6c0: 206e 756d 7079 2061 7272 6179 2077 6974   numpy array wit
-0000c6d0: 6820 6174 6f6d 6963 2064 6174 6120 2872  h atomic data (r
-0000c6e0: 6573 6964 7565 206e 756d 6265 722c 2063  esidue number, c
-0000c6f0: 6861 696e 2c20 7265 7369 6475 6520 6e61  hain, residue na
-0000c700: 6d65 2c20 6174 6f6d 206e 616d 652c 2078  me, atom name, x
-0000c710: 797a 2063 6f6f 7264 696e 6174 6573 2061  yz coordinates a
-0000c720: 6e64 2072 6164 6975 7329 2066 6f72 2065  nd radius) for e
-0000c730: 6163 6820 6174 6f6d 2e0a 2020 2020 5f64  ach atom..    _d
-0000c740: 696d 203a 2074 7570 6c65 0a20 2020 2020  im : tuple.     
-0000c750: 2020 2047 7269 6420 6469 6d65 6e73 696f     Grid dimensio
-0000c760: 6e73 2e0a 2020 2020 5f67 7269 6420 3a20  ns..    _grid : 
-0000c770: 6e75 6d70 792e 6e64 6172 7261 790a 2020  numpy.ndarray.  
-0000c780: 2020 2020 2020 4d6f 6c65 6375 6c65 2070        Molecule p
-0000c790: 6f69 6e74 7320 696e 2074 6865 2033 4420  oints in the 3D 
-0000c7a0: 6772 6964 2028 6772 6964 5b6e 785d 5b6e  grid (grid[nx][n
-0000c7b0: 795d 5b6e 7a5d 292e 0a20 2020 2020 2020  y][nz])..       
-0000c7c0: 2047 7269 6420 6172 7261 7920 6861 7320   Grid array has 
-0000c7d0: 696e 7465 6765 7220 6c61 6265 6c73 2069  integer labels i
-0000c7e0: 6e20 6561 6368 2070 6f73 6974 696f 6e2c  n each position,
-0000c7f0: 2074 6861 7420 6172 653a 0a0a 2020 2020   that are:..    
-0000c800: 2020 2020 2020 2020 2a20 303a 206d 6f6c          * 0: mol
-0000c810: 6563 756c 6520 706f 696e 7473 3b0a 0a20  ecule points;.. 
-0000c820: 2020 2020 2020 2020 2020 202a 2031 3a20             * 1: 
-0000c830: 736f 6c76 656e 7420 706f 696e 7473 2e0a  solvent points..
-0000c840: 2020 2020 5f6d 6f6c 6563 756c 6520 3a20      _molecule : 
-0000c850: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
-0000c860: 6962 2e50 6174 685d 0a20 2020 2020 2020  ib.Path].       
-0000c870: 2041 2066 696c 6520 7061 7468 2074 6f20   A file path to 
-0000c880: 7468 6520 6d6f 6c65 6375 6c65 2069 6e20  the molecule in 
-0000c890: 6569 7468 6572 2050 4442 206f 7220 5859  either PDB or XY
-0000c8a0: 5a20 666f 726d 6174 2e0a 2020 2020 5f70  Z format..    _p
-0000c8b0: 6164 6469 6e67 203a 2066 6c6f 6174 0a20  adding : float. 
-0000c8c0: 2020 2020 2020 2054 6865 206c 656e 6774         The lengt
-0000c8d0: 6820 746f 2061 6464 2074 6f20 6561 6368  h to add to each
-0000c8e0: 2064 6972 6563 7469 6f6e 206f 6620 7468   direction of th
-0000c8f0: 6520 3344 2067 7269 642e 0a20 2020 205f  e 3D grid..    _
-0000c900: 7072 6f62 6520 3a20 666c 6f61 740a 2020  probe : float.  
-0000c910: 2020 2020 2020 5370 6865 7269 6361 6c20        Spherical 
-0000c920: 7072 6f62 6520 7369 7a65 2074 6f20 6465  probe size to de
-0000c930: 6669 6e65 2074 6865 206d 6f6c 6563 756c  fine the molecul
-0000c940: 6172 2073 7572 6661 6365 2062 6173 6564  ar surface based
-0000c950: 206f 6e20 6120 6d6f 6c65 6375 6c61 7220   on a molecular 
-0000c960: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
-0000c970: 2020 2020 5f72 6164 6969 203a 2044 6963      _radii : Dic
-0000c980: 745b 7374 722c 2041 6e79 5d0a 2020 2020  t[str, Any].    
-0000c990: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
-0000c9a0: 2063 6f6e 7461 696e 696e 6720 7261 6469   containing radi
-0000c9b0: 6920 7661 6c75 6573 2c20 6279 2064 6566  i values, by def
-0000c9c0: 6175 6c74 204e 6f6e 652e 0a20 2020 205f  ault None..    _
-0000c9d0: 7265 7072 6573 656e 7461 7469 6f6e 203a  representation :
-0000c9e0: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
-0000c9f0: 2020 2020 2020 204d 6f6c 6563 756c 6172         Molecular
-0000ca00: 2073 7572 6661 6365 2072 6570 7265 7365   surface represe
-0000ca10: 6e74 6174 696f 6e2e 204b 6579 776f 7264  ntation. Keyword
-0000ca20: 7320 6f70 7469 6f6e 7320 6172 6520 7664  s options are vd
-0000ca30: 5720 2876 616e 2064 6572 2057 6161 6c73  W (van der Waals
-0000ca40: 2073 7572 6661 6365 292c 2053 4553 2028   surface), SES (
-0000ca50: 536f 6c76 656e 7420 4578 636c 7564 6564  Solvent Excluded
-0000ca60: 2053 7572 6661 6365 2920 6f72 2053 4153   Surface) or SAS
-0000ca70: 2028 536f 6c76 656e 7420 4163 6365 7373   (Solvent Access
-0000ca80: 6962 6c65 2053 7572 6661 6365 292c 2062  ible Surface), b
-0000ca90: 7920 6465 6661 756c 7420 5345 532e 0a20  y default SES.. 
-0000caa0: 2020 205f 726f 7461 7469 6f6e 203a 206e     _rotation : n
-0000cab0: 756d 7079 2e6e 6461 7272 6179 0a20 2020  umpy.ndarray.   
-0000cac0: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
-0000cad0: 7272 6179 2077 6974 6820 7369 6e65 2061  rray with sine a
-0000cae0: 6e64 2063 6f73 7369 6e65 206f 6620 7468  nd cossine of th
-0000caf0: 6520 6772 6964 2072 6f74 6174 696f 6e20  e grid rotation 
-0000cb00: 616e 676c 6573 2028 7369 6e61 2c20 636f  angles (sina, co
-0000cb10: 7361 2c20 7369 6e62 2c20 636f 7362 292e  sa, sinb, cosb).
-0000cb20: 0a20 2020 205f 7374 6570 203a 2066 6c6f  .    _step : flo
-0000cb30: 6174 0a20 2020 2020 2020 2047 7269 6420  at.        Grid 
-0000cb40: 7370 6163 696e 6720 2841 292e 0a20 2020  spacing (A)..   
-0000cb50: 205f 7665 7274 6963 6573 203a 206e 756d   _vertices : num
-0000cb60: 7079 2e6e 6461 7272 6179 0a20 2020 2020  py.ndarray.     
-0000cb70: 2020 2041 206e 756d 7079 2e6e 6461 7272     A numpy.ndarr
-0000cb80: 6179 206f 7220 6120 6c69 7374 2077 6974  ay or a list wit
-0000cb90: 6820 7879 7a20 7665 7274 6963 6573 2063  h xyz vertices c
-0000cba0: 6f6f 7264 696e 6174 6573 2028 6f72 6967  oordinates (orig
-0000cbb0: 696e 2c20 582d 6178 6973 2c20 592d 6178  in, X-axis, Y-ax
-0000cbc0: 6973 2c20 5a2d 6178 6973 292e 0a20 2020  is, Z-axis)..   
-0000cbd0: 206e 7468 7265 6164 7320 3a20 696e 740a   nthreads : int.
-0000cbe0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-0000cbf0: 6620 7468 7265 6164 7320 666f 7220 7061  f threads for pa
-0000cc00: 7261 6c6c 656c 2070 726f 6365 7373 696e  rallel processin
-0000cc10: 672e 0a20 2020 2076 6572 626f 7365 203a  g..    verbose :
-0000cc20: 2062 6f6f 6c0a 2020 2020 2020 2020 5768   bool.        Wh
-0000cc30: 6574 6865 7220 746f 2070 7269 6e74 2065  ether to print e
-0000cc40: 7874 7261 2069 6e66 6f72 6d61 7469 6f6e  xtra information
-0000cc50: 2074 6f20 7374 616e 6461 7264 206f 7574   to standard out
-0000cc60: 7075 742e 0a0a 2020 2020 4e6f 7465 0a20  put...    Note. 
-0000cc70: 2020 202d 2d2d 2d0a 2020 2020 5468 6520     ----.    The 
-0000cc80: 7661 6e20 6465 7220 5761 616c 7320 7261  van der Waals ra
-0000cc90: 6469 6920 6669 6c65 2064 6566 696e 6573  dii file defines
-0000cca0: 2074 6865 2072 6164 6975 7320 7661 6c75   the radius valu
-0000ccb0: 6573 2066 6f72 2065 6163 6820 6174 6f6d  es for each atom
-0000ccc0: 2062 7920 7265 7369 6475 6520 616e 6420   by residue and 
-0000ccd0: 7768 656e 206e 6f74 2064 6566 696e 6564  when not defined
-0000cce0: 2c20 6974 2075 7365 7320 6120 6765 6e65  , it uses a gene
-0000ccf0: 7269 6320 7661 6c75 6520 6261 7365 6420  ric value based 
-0000cd00: 6f6e 2074 6865 2061 746f 6d20 7479 7065  on the atom type
-0000cd10: 2e20 5468 6520 6675 6e63 7469 6f6e 2062  . The function b
-0000cd20: 7920 6465 6661 756c 7420 6c6f 6164 7320  y default loads 
-0000cd30: 7468 6520 6275 696c 742d 696e 2076 616e  the built-in van
-0000cd40: 2064 6572 2057 6161 6c73 2072 6164 6969   der Waals radii
-0000cd50: 2066 696c 653a 2060 6076 6477 2e64 6174   file: ``vdw.dat
-0000cd60: 6060 2e0a 0a20 2020 2053 6565 2041 6c73  ``...    See Als
-0000cd70: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
-0000cd80: 2020 2072 6561 645f 7664 770a 0a20 2020     read_vdw..   
-0000cd90: 2045 7861 6d70 6c65 0a20 2020 202d 2d2d   Example.    ---
-0000cda0: 2d2d 2d2d 0a20 2020 2054 6865 2060 604d  ----.    The ``M
-0000cdb0: 6f6c 6563 756c 6560 6020 636c 6173 7320  olecule`` class 
-0000cdc0: 6c6f 6164 7320 7468 6520 7461 7267 6574  loads the target
-0000cdd0: 206d 6f6c 6563 756c 6172 2073 7472 7563   molecular struc
-0000cde0: 7475 7265 2028 436c 4f34 2920 696e 746f  ture (ClO4) into
-0000cdf0: 2070 794b 5646 696e 6465 722e 2063 6c61   pyKVFinder. cla
-0000ce00: 7373 2e0a 0a20 2020 203e 3e3e 2069 6d70  ss...    >>> imp
-0000ce10: 6f72 7420 6f73 0a20 2020 203e 3e3e 2066  ort os.    >>> f
-0000ce20: 726f 6d20 7079 4b56 4669 6e64 6572 2069  rom pyKVFinder i
-0000ce30: 6d70 6f72 7420 4d6f 6c65 6375 6c65 0a20  mport Molecule. 
-0000ce40: 2020 203e 3e3e 2070 6462 203d 206f 732e     >>> pdb = os.
-0000ce50: 7061 7468 2e6a 6f69 6e28 6f73 2e70 6174  path.join(os.pat
-0000ce60: 682e 6469 726e 616d 6528 7079 4b56 4669  h.dirname(pyKVFi
-0000ce70: 6e64 6572 2e5f 5f66 696c 655f 5f29 2c20  nder.__file__), 
-0000ce80: 2764 6174 6127 2c20 2774 6573 7473 272c  'data', 'tests',
-0000ce90: 2027 436c 4f34 2e70 6462 2729 0a20 2020   'ClO4.pdb').   
-0000cea0: 203e 3e3e 206d 6f6c 6563 756c 6520 3d20   >>> molecule = 
-0000ceb0: 4d6f 6c65 6375 6c65 2870 6462 290a 2020  Molecule(pdb).  
-0000cec0: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 0a20    >>> molecule. 
-0000ced0: 2020 203e 3e3e 203c 7079 4b56 4669 6e64     >>> <pyKVFind
-0000cee0: 6572 2e6d 6169 6e2e 4d6f 6c65 6375 6c65  er.main.Molecule
-0000cef0: 206f 626a 6563 7420 6174 2030 7837 6635   object at 0x7f5
-0000cf00: 6464 6163 6632 3233 303e 0a0a 2020 2020  ddacf2230>..    
-0000cf10: 5468 6520 7661 6e20 6465 7220 5761 616c  The van der Waal
-0000cf20: 7320 7261 6469 6920 6361 6e20 6265 2064  s radii can be d
-0000cf30: 6566 696e 6520 6279 3a0a 0a20 2020 2020  efine by:..     
-0000cf40: 2020 202a 2063 7265 6174 696e 6720 6120     * creating a 
-0000cf50: 5079 7468 6f6e 2064 6963 7469 6f6e 6172  Python dictionar
-0000cf60: 793a 0a0a 2020 2020 2020 2020 3e3e 3e20  y:..        >>> 
-0000cf70: 2320 5079 4d4f 4c20 2876 322e 352e 3029  # PyMOL (v2.5.0)
-0000cf80: 2076 6457 2072 6164 6969 2076 616c 7565   vdW radii value
-0000cf90: 730a 2020 2020 2020 2020 3e3e 3e20 7664  s.        >>> vd
-0000cfa0: 7720 3d20 7b27 4745 4e27 3a20 7b27 434c  w = {'GEN': {'CL
-0000cfb0: 273a 2031 2e37 352c 2027 4f27 3a20 312e  ': 1.75, 'O': 1.
-0000cfc0: 3532 7d7d 0a20 2020 2020 2020 203e 3e3e  52}}.        >>>
-0000cfd0: 206d 6f6c 6563 756c 6520 3d20 4d6f 6c65   molecule = Mole
-0000cfe0: 6375 6c65 2870 6462 2c20 7261 6469 693d  cule(pdb, radii=
-0000cff0: 7664 7729 0a20 2020 2020 2020 203e 3e3e  vdw).        >>>
-0000d000: 206d 6f6c 6563 756c 652e 7261 6469 690a   molecule.radii.
-0000d010: 2020 2020 2020 2020 7b27 4745 4e27 3a20          {'GEN': 
-0000d020: 7b27 434c 273a 2031 2e37 352c 2027 4f27  {'CL': 1.75, 'O'
-0000d030: 3a20 312e 3532 7d7d 0a0a 2020 2020 2020  : 1.52}}..      
-0000d040: 2020 2a20 7370 6563 6966 7969 6e67 2061    * specifying a
-0000d050: 202a 2e64 6174 2a20 6669 6c65 2066 6f6c   *.dat* file fol
-0000d060: 6c6f 7769 6e67 2074 656d 706c 6174 6520  lowing template 
-0000d070: 6f66 2060 7661 6e20 6465 7220 5761 616c  of `van der Waal
-0000d080: 7320 7261 6469 6920 6669 6c65 602e 0a0a  s radii file`...
-0000d090: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
-0000d0a0: 2070 794b 5646 696e 6465 7220 696d 706f   pyKVFinder impo
-0000d0b0: 7274 2072 6561 645f 7664 770a 2020 2020  rt read_vdw.    
-0000d0c0: 2020 2020 3e3e 3e20 2320 4368 696d 6572      >>> # Chimer
-0000d0d0: 6158 2076 6457 2072 6164 6969 2076 616c  aX vdW radii val
-0000d0e0: 7565 730a 2020 2020 2020 2020 3e3e 3e20  ues.        >>> 
-0000d0f0: 7769 7468 206f 7065 6e28 2776 6477 2e64  with open('vdw.d
-0000d100: 6174 272c 2027 7727 2920 6173 2066 3a0a  at', 'w') as f:.
-0000d110: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-0000d120: 662e 7772 6974 6528 273e 4745 4e5c 5c6e  f.write('>GEN\\n
-0000d130: 434c 5c5c 745c 5c74 312e 3938 5c5c 6e4f  CL\\t\\t1.98\\nO
-0000d140: 5c5c 745c 5c74 312e 3436 5c5c 6e27 290a  \\t\\t1.46\\n').
-0000d150: 2020 2020 2020 2020 3e3e 3e20 7664 7720          >>> vdw 
-0000d160: 3d20 7265 6164 5f76 6477 2827 7664 772e  = read_vdw('vdw.
-0000d170: 6461 7427 290a 2020 2020 2020 2020 3e3e  dat').        >>
-0000d180: 3e20 6d6f 6c65 6375 6c65 203d 204d 6f6c  > molecule = Mol
-0000d190: 6563 756c 6528 7064 622c 2072 6164 6969  ecule(pdb, radii
-0000d1a0: 3d76 6477 290a 2020 2020 2020 2020 3e3e  =vdw).        >>
-0000d1b0: 3e20 6d6f 6c65 6375 6c65 2e72 6164 6969  > molecule.radii
-0000d1c0: 0a20 2020 2020 2020 207b 2747 454e 273a  .        {'GEN':
-0000d1d0: 207b 2743 4c27 3a20 312e 3938 2c20 274f   {'CL': 1.98, 'O
-0000d1e0: 273a 2031 2e34 367d 7d0a 2020 2020 2222  ': 1.46}}.    ""
-0000d1f0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-0000d200: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0000d210: 662c 0a20 2020 2020 2020 206d 6f6c 6563  f,.        molec
-0000d220: 756c 653a 2055 6e69 6f6e 5b73 7472 2c20  ule: Union[str, 
-0000d230: 7061 7468 6c69 622e 5061 7468 5d2c 0a20  pathlib.Path],. 
-0000d240: 2020 2020 2020 2072 6164 6969 3a20 556e         radii: Un
-0000d250: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
-0000d260: 2e50 6174 682c 2044 6963 745b 7374 722c  .Path, Dict[str,
-0000d270: 2041 6e79 5d5d 203d 204e 6f6e 652c 0a20   Any]] = None,. 
-0000d280: 2020 2020 2020 206d 6f64 656c 3a20 4f70         model: Op
-0000d290: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000d2a0: 6e65 2c0a 2020 2020 2020 2020 6e74 6872  ne,.        nthr
-0000d2b0: 6561 6473 3a20 4f70 7469 6f6e 616c 5b69  eads: Optional[i
-0000d2c0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-0000d2d0: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-0000d2e0: 6c20 3d20 4661 6c73 652c 0a20 2020 2029  l = False,.    )
-0000d2f0: 3a0a 2020 2020 2020 2020 2222 2249 6e69  :.        """Ini
-0000d300: 7469 616c 697a 6520 7468 6520 4d6f 6c65  tialize the Mole
-0000d310: 6375 6c65 206f 626a 6563 7420 7769 7468  cule object with
-0000d320: 206d 6f6c 6563 756c 652c 2072 6164 6969   molecule, radii
-0000d330: 2c20 6d6f 6465 6c2c 206e 7468 7265 6164  , model, nthread
-0000d340: 7320 616e 6420 7665 7262 6f73 652e 0a0a  s and verbose...
-0000d350: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000d360: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000d370: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6d6f  -----.        mo
-0000d380: 6c65 6375 6c65 203a 2055 6e69 6f6e 5b73  lecule : Union[s
-0000d390: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
-0000d3a0: 5d0a 2020 2020 2020 2020 2020 2020 4120  ].            A 
-0000d3b0: 6669 6c65 2070 6174 6820 746f 2074 6865  file path to the
-0000d3c0: 206d 6f6c 6563 756c 6520 696e 2065 6974   molecule in eit
-0000d3d0: 6865 7220 5044 4220 6f72 2058 595a 2066  her PDB or XYZ f
-0000d3e0: 6f72 6d61 742e 0a20 2020 2020 2020 2072  ormat..        r
-0000d3f0: 6164 6969 203a 2055 6e69 6f6e 5b73 7472  adii : Union[str
-0000d400: 2c20 7061 7468 6c69 622e 5061 7468 2c20  , pathlib.Path, 
-0000d410: 4469 6374 5b73 7472 2c20 416e 795d 5d2c  Dict[str, Any]],
-0000d420: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000d430: 2020 2020 2020 4120 6669 6c65 2070 6174        A file pat
-0000d440: 6820 746f 2061 2076 616e 2064 6572 2057  h to a van der W
-0000d450: 6161 6c73 2072 6164 6969 2066 696c 6520  aals radii file 
-0000d460: 6f72 2061 2064 6963 7469 6f6e 6172 7920  or a dictionary 
-0000d470: 6f66 2056 4457 2072 6164 6969 2c20 6279  of VDW radii, by
-0000d480: 2064 6566 6175 6c74 204e 6f6e 652e 2049   default None. I
-0000d490: 6620 4e6f 6e65 2c20 6170 706c 7920 7468  f None, apply th
-0000d4a0: 6520 6275 696c 742d 696e 2076 616e 2064  e built-in van d
-0000d4b0: 6572 2057 6161 6c73 2072 6164 6969 2066  er Waals radii f
-0000d4c0: 696c 653a 2060 7664 772e 6461 7460 2e0a  ile: `vdw.dat`..
-0000d4d0: 2020 2020 2020 2020 6d6f 6465 6c20 3a20          model : 
-0000d4e0: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0000d4f0: 2020 2020 2020 2020 2020 5468 6520 6d6f            The mo
-0000d500: 6465 6c20 6e75 6d62 6572 206f 6620 6120  del number of a 
-0000d510: 6d75 6c74 692d 6d6f 6465 6c20 5044 4220  multi-model PDB 
-0000d520: 6669 6c65 2c20 6279 2064 6566 6175 6c74  file, by default
-0000d530: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
-0000d540: 6b65 6570 2061 746f 6d73 2066 726f 6d20  keep atoms from 
-0000d550: 616c 6c20 6d6f 6465 6c73 2e0a 2020 2020  all models..    
-0000d560: 2020 2020 6e74 6872 6561 6473 203a 2069      nthreads : i
-0000d570: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-0000d580: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-0000d590: 6f66 2074 6872 6561 6473 2c20 6279 2064  of threads, by d
-0000d5a0: 6566 6175 6c74 204e 6f6e 652e 2049 6620  efault None. If 
-0000d5b0: 4e6f 6e65 2c20 7468 6520 6e75 6d62 6572  None, the number
-0000d5c0: 206f 6620 7468 7265 6164 7320 6973 2060   of threads is `
-0000d5d0: 6f73 2e63 7075 5f63 6f75 6e74 2829 202d  os.cpu_count() -
-0000d5e0: 2031 602e 0a20 2020 2020 2020 2076 6572   1`..        ver
-0000d5f0: 626f 7365 203a 2062 6f6f 6c2c 206f 7074  bose : bool, opt
-0000d600: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000d610: 2020 5072 696e 7420 6578 7472 6120 696e    Print extra in
-0000d620: 666f 726d 6174 696f 6e20 746f 2073 7461  formation to sta
-0000d630: 6e64 6172 6420 6f75 7470 7574 2c20 6279  ndard output, by
-0000d640: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
-0000d650: 0a20 2020 2020 2020 2052 6169 7365 730a  .        Raises.
-0000d660: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
-0000d670: 2020 2020 2020 2054 7970 6545 7272 6f72         TypeError
-0000d680: 0a20 2020 2020 2020 2020 2020 2060 6d6f  .            `mo
-0000d690: 6c65 6375 6c65 6020 6d75 7374 2062 6520  lecule` must be 
-0000d6a0: 6120 7374 7269 6e67 206f 7220 6120 7061  a string or a pa
-0000d6b0: 7468 6c69 622e 5061 7468 2e0a 2020 2020  thlib.Path..    
-0000d6c0: 2020 2020 5479 7065 4572 726f 720a 2020      TypeError.  
-0000d6d0: 2020 2020 2020 2020 2020 606d 6f6c 6563            `molec
-0000d6e0: 756c 6560 206d 7573 7420 6861 7665 202e  ule` must have .
-0000d6f0: 7064 6220 6f72 202e 7879 7a20 6578 7465  pdb or .xyz exte
-0000d700: 6e73 696f 6e2e 0a20 2020 2020 2020 2054  nsion..        T
-0000d710: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-0000d720: 2020 2020 2060 6e74 6872 6561 6473 6020       `nthreads` 
-0000d730: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-0000d740: 7665 2069 6e74 6567 6572 2e0a 2020 2020  ve integer..    
-0000d750: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
-0000d760: 2020 2020 2020 2020 2020 2060 6e74 6872             `nthr
-0000d770: 6561 6473 6020 6d75 7374 2062 6520 6120  eads` must be a 
-0000d780: 706f 7369 7469 7665 2069 6e74 6567 6572  positive integer
-0000d790: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-0000d7a0: 2020 2020 2020 2023 2041 7474 7269 6275         # Attribu
-0000d7b0: 7465 730a 2020 2020 2020 2020 7365 6c66  tes.        self
-0000d7c0: 2e5f 6772 6964 203d 204e 6f6e 650a 2020  ._grid = None.  
-0000d7d0: 2020 2020 2020 7365 6c66 2e5f 7374 6570        self._step
-0000d7e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000d7f0: 7365 6c66 2e5f 7061 6464 696e 6720 3d20  self._padding = 
-0000d800: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000d810: 662e 5f70 726f 6265 203d 204e 6f6e 650a  f._probe = None.
-0000d820: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-0000d830: 7072 6573 656e 7461 7469 6f6e 203d 204e  presentation = N
-0000d840: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000d850: 2e5f 7665 7274 6963 6573 203d 204e 6f6e  ._vertices = Non
-0000d860: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000d870: 6469 6d20 3d20 4e6f 6e65 0a20 2020 2020  dim = None.     
-0000d880: 2020 2073 656c 662e 5f72 6f74 6174 696f     self._rotatio
-0000d890: 6e20 3d20 4e6f 6e65 0a20 2020 2020 2020  n = None.       
-0000d8a0: 2073 656c 662e 7665 7262 6f73 6520 3d20   self.verbose = 
-0000d8b0: 7665 7262 6f73 650a 0a20 2020 2020 2020  verbose..       
-0000d8c0: 2023 204d 6f6c 6563 756c 650a 2020 2020   # Molecule.    
-0000d8d0: 2020 2020 6966 2074 7970 6528 6d6f 6c65      if type(mole
-0000d8e0: 6375 6c65 2920 6e6f 7420 696e 205b 7374  cule) not in [st
-0000d8f0: 722c 2070 6174 686c 6962 2e50 6174 685d  r, pathlib.Path]
-0000d900: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000d910: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-0000d920: 6d6f 6c65 6375 6c65 6020 6d75 7374 2062  molecule` must b
-0000d930: 6520 6120 7374 7269 6e67 206f 7220 6120  e a string or a 
-0000d940: 7061 7468 6c69 622e 5061 7468 2e22 290a  pathlib.Path.").
-0000d950: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
-0000d960: 6c65 6375 6c65 203d 206f 732e 7061 7468  lecule = os.path
-0000d970: 2e72 6561 6c70 6174 6828 6d6f 6c65 6375  .realpath(molecu
-0000d980: 6c65 290a 0a20 2020 2020 2020 2023 2076  le)..        # v
-0000d990: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
-0000d9a0: 6969 0a20 2020 2020 2020 2069 6620 7365  ii.        if se
-0000d9b0: 6c66 2e76 6572 626f 7365 3a0a 2020 2020  lf.verbose:.    
-0000d9c0: 2020 2020 2020 2020 7072 696e 7428 223e          print(">
-0000d9d0: 204c 6f61 6469 6e67 2076 616e 2064 6572   Loading van der
-0000d9e0: 2057 6161 6c73 2072 6164 6969 2229 0a20   Waals radii"). 
-0000d9f0: 2020 2020 2020 2069 6620 7261 6469 6920         if radii 
-0000da00: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000da10: 2020 2020 2023 2064 6566 6175 6c74 0a20       # default. 
-0000da20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000da30: 5f72 6164 6969 203d 2072 6561 645f 7664  _radii = read_vd
-0000da40: 7728 5644 5729 0a20 2020 2020 2020 2065  w(VDW).        e
-0000da50: 6c69 6620 7479 7065 2872 6164 6969 2920  lif type(radii) 
-0000da60: 696e 205b 7374 722c 2070 6174 686c 6962  in [str, pathlib
-0000da70: 2e50 6174 685d 3a0a 2020 2020 2020 2020  .Path]:.        
-0000da80: 2020 2020 2320 7664 7720 6669 6c65 0a20      # vdw file. 
-0000da90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000daa0: 5f72 6164 6969 203d 2072 6561 645f 7664  _radii = read_vd
-0000dab0: 7728 7261 6469 6929 0a20 2020 2020 2020  w(radii).       
-0000dac0: 2065 6c69 6620 7479 7065 2872 6164 6969   elif type(radii
-0000dad0: 2920 696e 205b 6469 6374 5d3a 0a20 2020  ) in [dict]:.   
-0000dae0: 2020 2020 2020 2020 2023 2050 726f 6365           # Proce
-0000daf0: 7373 6564 2064 6963 7469 6f6e 6172 790a  ssed dictionary.
-0000db00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000db10: 2e5f 7261 6469 6920 3d20 7261 6469 690a  ._radii = radii.
-0000db20: 0a20 2020 2020 2020 2023 2041 746f 6d69  .        # Atomi
-0000db30: 6320 696e 666f 726d 6174 696f 6e0a 2020  c information.  
-0000db40: 2020 2020 2020 6966 2073 656c 662e 7665        if self.ve
-0000db50: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-0000db60: 2020 2070 7269 6e74 2822 3e20 5265 6164     print("> Read
-0000db70: 696e 6720 6d6f 6c65 6375 6c65 2063 6f6f  ing molecule coo
-0000db80: 7264 696e 6174 6573 2229 0a20 2020 2020  rdinates").     
-0000db90: 2020 2069 6620 6d6f 6c65 6375 6c65 2e65     if molecule.e
-0000dba0: 6e64 7377 6974 6828 222e 7064 6222 293a  ndswith(".pdb"):
-0000dbb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000dbc0: 662e 5f61 746f 6d69 6320 3d20 7265 6164  f._atomic = read
-0000dbd0: 5f70 6462 286d 6f6c 6563 756c 652c 2073  _pdb(molecule, s
-0000dbe0: 656c 662e 7261 6469 692c 206d 6f64 656c  elf.radii, model
-0000dbf0: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
-0000dc00: 6f6c 6563 756c 652e 656e 6473 7769 7468  olecule.endswith
-0000dc10: 2822 2e78 797a 2229 3a0a 2020 2020 2020  (".xyz"):.      
-0000dc20: 2020 2020 2020 7365 6c66 2e5f 6174 6f6d        self._atom
-0000dc30: 6963 203d 2072 6561 645f 7879 7a28 6d6f  ic = read_xyz(mo
-0000dc40: 6c65 6375 6c65 2c20 7365 6c66 2e72 6164  lecule, self.rad
-0000dc50: 6969 290a 2020 2020 2020 2020 656c 7365  ii).        else
-0000dc60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000dc70: 6973 6520 5479 7065 4572 726f 7228 2260  ise TypeError("`
-0000dc80: 6d6f 6c65 6375 6c65 6020 6d75 7374 2068  molecule` must h
-0000dc90: 6176 6520 2e70 6462 206f 7220 2e78 797a  ave .pdb or .xyz
-0000dca0: 2065 7874 656e 7369 6f6e 2e22 290a 0a20   extension.").. 
-0000dcb0: 2020 2020 2020 2023 204e 756d 6265 7220         # Number 
-0000dcc0: 6f66 2074 6872 6561 6473 0a20 2020 2020  of threads.     
-0000dcd0: 2020 2069 6620 6e74 6872 6561 6473 2069     if nthreads i
-0000dce0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000dcf0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0000dd00: 6e74 6872 6561 6473 2920 6e6f 7420 696e  nthreads) not in
-0000dd10: 205b 696e 745d 3a0a 2020 2020 2020 2020   [int]:.        
-0000dd20: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0000dd30: 7065 4572 726f 7228 2260 6e74 6872 6561  peError("`nthrea
-0000dd40: 6473 6020 6d75 7374 2062 6520 6120 706f  ds` must be a po
-0000dd50: 7369 7469 7665 2069 6e74 6567 6572 2e22  sitive integer."
-0000dd60: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000dd70: 6966 206e 7468 7265 6164 7320 3c3d 2030  if nthreads <= 0
-0000dd80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dd90: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000dda0: 6f72 2822 606e 7468 7265 6164 7360 206d  or("`nthreads` m
-0000ddb0: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
-0000ddc0: 6520 696e 7465 6765 722e 2229 0a20 2020  e integer.").   
-0000ddd0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ddf0: 656c 662e 6e74 6872 6561 6473 203d 206e  elf.nthreads = n
-0000de00: 7468 7265 6164 730a 2020 2020 2020 2020  threads.        
-0000de10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000de20: 2020 7365 6c66 2e6e 7468 7265 6164 7320    self.nthreads 
-0000de30: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000de40: 202d 2031 0a0a 2020 2020 4070 726f 7065   - 1..    @prope
-0000de50: 7274 790a 2020 2020 6465 6620 6174 6f6d  rty.    def atom
-0000de60: 6963 2873 656c 6629 202d 3e20 6e75 6d70  ic(self) -> nump
-0000de70: 792e 6e64 6172 7261 793a 0a20 2020 2020  y.ndarray:.     
-0000de80: 2020 2022 2222 4765 7420 5f61 746f 6d69     """Get _atomi
-0000de90: 6320 6174 7472 6962 7574 652e 2222 220a  c attribute.""".
-0000dea0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000deb0: 656c 662e 5f61 746f 6d69 630a 0a20 2020  elf._atomic..   
-0000dec0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000ded0: 6566 2064 696d 2873 656c 6629 202d 3e20  ef dim(self) -> 
-0000dee0: 5475 706c 655b 696e 742c 2069 6e74 2c20  Tuple[int, int, 
-0000def0: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
-0000df00: 2247 6574 205f 6469 6d20 6174 7472 6962  "Get _dim attrib
-0000df10: 7574 6522 2222 0a20 2020 2020 2020 2072  ute""".        r
-0000df20: 6574 7572 6e20 7365 6c66 2e5f 6469 6d0a  eturn self._dim.
-0000df30: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000df40: 2020 2064 6566 2067 7269 6428 7365 6c66     def grid(self
-0000df50: 2920 2d3e 206e 756d 7079 2e6e 6461 7272  ) -> numpy.ndarr
-0000df60: 6179 3a0a 2020 2020 2020 2020 2222 2247  ay:.        """G
-0000df70: 6574 205f 6772 6964 2061 7474 7269 6275  et _grid attribu
-0000df80: 7465 2e22 2222 0a20 2020 2020 2020 2072  te.""".        r
-0000df90: 6574 7572 6e20 7365 6c66 2e5f 6772 6964  eturn self._grid
-0000dfa0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000dfb0: 2020 2020 6465 6620 6d6f 6c65 6375 6c65      def molecule
-0000dfc0: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
-0000dfd0: 7374 722c 2070 6174 686c 6962 2e50 6174  str, pathlib.Pat
-0000dfe0: 685d 3a0a 2020 2020 2020 2020 2222 2247  h]:.        """G
-0000dff0: 6574 205f 6d6f 6c65 6375 6c65 2061 7474  et _molecule att
-0000e000: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
-0000e010: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000e020: 6d6f 6c65 6375 6c65 0a0a 2020 2020 4070  molecule..    @p
-0000e030: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e040: 6e78 2873 656c 6629 202d 3e20 696e 743a  nx(self) -> int:
-0000e050: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000e060: 6772 6964 2075 6e69 7473 2069 6e20 582d  grid units in X-
-0000e070: 6178 6973 2e22 2222 0a20 2020 2020 2020  axis.""".       
-0000e080: 2069 6620 7365 6c66 2e5f 6469 6d20 6973   if self._dim is
-0000e090: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e0a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e0b0: 6c66 2e5f 6469 6d5b 305d 0a0a 2020 2020  lf._dim[0]..    
-0000e0c0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000e0d0: 6620 6e79 2873 656c 6629 202d 3e20 696e  f ny(self) -> in
-0000e0e0: 743a 0a20 2020 2020 2020 2022 2222 4765  t:.        """Ge
-0000e0f0: 7420 6772 6964 2075 6e69 7473 2069 6e20  t grid units in 
-0000e100: 592d 6178 6973 2e22 2222 0a20 2020 2020  Y-axis.""".     
-0000e110: 2020 2069 6620 7365 6c66 2e5f 6469 6d20     if self._dim 
-0000e120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000e140: 7365 6c66 2e5f 6469 6d5b 315d 0a0a 2020  self._dim[1]..  
-0000e150: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000e160: 6465 6620 6e7a 2873 656c 6629 202d 3e20  def nz(self) -> 
-0000e170: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-0000e180: 4765 7420 6772 6964 2075 6e69 7473 2069  Get grid units i
-0000e190: 6e20 5a2d 6178 6973 2e22 2222 0a20 2020  n Z-axis.""".   
-0000e1a0: 2020 2020 2069 6620 7365 6c66 2e5f 6469       if self._di
-0000e1b0: 6d20 6973 206e 6f74 204e 6f6e 653a 0a20  m is not None:. 
-0000e1c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e1d0: 6e20 7365 6c66 2e5f 6469 6d5b 325d 0a0a  n self._dim[2]..
-0000e1e0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000e1f0: 2020 6465 6620 7031 2873 656c 6629 202d    def p1(self) -
-0000e200: 3e20 6e75 6d70 792e 6e64 6172 7261 793a  > numpy.ndarray:
-0000e210: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000e220: 6f72 6967 696e 206f 6620 7468 6520 3344  origin of the 3D
-0000e230: 2067 7269 642e 2222 220a 2020 2020 2020   grid.""".      
-0000e240: 2020 6966 2073 656c 662e 5f76 6572 7469    if self._verti
-0000e250: 6365 7320 6973 206e 6f74 204e 6f6e 653a  ces is not None:
-0000e260: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e270: 7572 6e20 7365 6c66 2e5f 7665 7274 6963  urn self._vertic
-0000e280: 6573 5b30 5d0a 0a20 2020 2040 7072 6f70  es[0]..    @prop
-0000e290: 6572 7479 0a20 2020 2064 6566 2070 3228  erty.    def p2(
-0000e2a0: 7365 6c66 2920 2d3e 206e 756d 7079 2e6e  self) -> numpy.n
-0000e2b0: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-0000e2c0: 2222 2247 6574 2058 2d61 7869 7320 6d61  """Get X-axis ma
-0000e2d0: 7820 6f66 2074 6865 2033 4420 6772 6964  x of the 3D grid
-0000e2e0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
-0000e2f0: 7365 6c66 2e5f 7665 7274 6963 6573 2069  self._vertices i
-0000e300: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000e310: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e320: 656c 662e 5f76 6572 7469 6365 735b 315d  elf._vertices[1]
-0000e330: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000e340: 2020 2020 6465 6620 7033 2873 656c 6629      def p3(self)
-0000e350: 202d 3e20 6e75 6d70 792e 6e64 6172 7261   -> numpy.ndarra
-0000e360: 793a 0a20 2020 2020 2020 2022 2222 4765  y:.        """Ge
-0000e370: 7420 592d 6178 6973 206d 6178 206f 6620  t Y-axis max of 
-0000e380: 7468 6520 3344 2067 7269 642e 2222 220a  the 3D grid.""".
-0000e390: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e3a0: 5f76 6572 7469 6365 7320 6973 206e 6f74  _vertices is not
-0000e3b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000e3c0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000e3d0: 7665 7274 6963 6573 5b32 5d0a 0a20 2020  vertices[2]..   
-0000e3e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000e3f0: 6566 2070 3428 7365 6c66 2920 2d3e 206e  ef p4(self) -> n
-0000e400: 756d 7079 2e6e 6461 7272 6179 3a0a 2020  umpy.ndarray:.  
-0000e410: 2020 2020 2020 2222 2247 6574 205a 2d61        """Get Z-a
-0000e420: 7869 7320 6d61 7820 6f66 2074 6865 2033  xis max of the 3
-0000e430: 4420 6772 6964 2e22 2222 0a20 2020 2020  D grid.""".     
-0000e440: 2020 2069 6620 7365 6c66 2e5f 7665 7274     if self._vert
-0000e450: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
-0000e460: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e470: 7475 726e 2073 656c 662e 5f76 6572 7469  turn self._verti
-0000e480: 6365 735b 335d 0a0a 2020 2020 4070 726f  ces[3]..    @pro
-0000e490: 7065 7274 790a 2020 2020 6465 6620 7061  perty.    def pa
-0000e4a0: 6464 696e 6728 7365 6c66 2920 2d3e 2066  dding(self) -> f
-0000e4b0: 6c6f 6174 3a0a 2020 2020 2020 2020 2222  loat:.        ""
-0000e4c0: 2247 6574 205f 7061 6464 696e 6720 6174  "Get _padding at
-0000e4d0: 7472 6962 7574 652e 2222 220a 2020 2020  tribute.""".    
-0000e4e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e4f0: 5f70 6164 6469 6e67 0a0a 2020 2020 4070  _padding..    @p
-0000e500: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e510: 7072 6f62 6528 7365 6c66 2920 2d3e 2066  probe(self) -> f
-0000e520: 6c6f 6174 3a0a 2020 2020 2020 2020 2222  loat:.        ""
-0000e530: 2247 6574 205f 7072 6f62 6520 6174 7472  "Get _probe attr
-0000e540: 6962 7574 652e 2222 220a 2020 2020 2020  ibute.""".      
-0000e550: 2020 7265 7475 726e 2073 656c 662e 5f70    return self._p
-0000e560: 726f 6265 0a0a 2020 2020 4070 726f 7065  robe..    @prope
-0000e570: 7274 790a 2020 2020 6465 6620 7261 6469  rty.    def radi
-0000e580: 6928 7365 6c66 2920 2d3e 2044 6963 745b  i(self) -> Dict[
-0000e590: 7374 722c 2041 6e79 5d3a 0a20 2020 2020  str, Any]:.     
-0000e5a0: 2020 2022 2222 4765 7420 5f72 6164 6969     """Get _radii
-0000e5b0: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
-0000e5c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e5d0: 6c66 2e5f 7261 6469 690a 0a20 2020 2040  lf._radii..    @
-0000e5e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000e5f0: 2072 6570 7265 7365 6e74 6174 696f 6e28   representation(
-0000e600: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
-0000e610: 2020 2020 2020 2222 2247 6574 205f 7265        """Get _re
-0000e620: 7072 6573 656e 7461 7469 6f6e 2061 7474  presentation att
-0000e630: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
-0000e640: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000e650: 7265 7072 6573 656e 7461 7469 6f6e 0a0a  representation..
-0000e660: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000e670: 2020 6465 6620 726f 7461 7469 6f6e 2873    def rotation(s
-0000e680: 656c 6629 202d 3e20 6e75 6d70 792e 6e64  elf) -> numpy.nd
-0000e690: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
-0000e6a0: 2222 4765 7420 5f72 6f74 6174 696f 6e20  ""Get _rotation 
-0000e6b0: 6174 7472 6962 7574 652e 2222 220a 2020  attribute.""".  
-0000e6c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e6d0: 662e 5f72 6f74 6174 696f 6e0a 0a20 2020  f._rotation..   
-0000e6e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000e6f0: 6566 2073 7465 7028 7365 6c66 2920 2d3e  ef step(self) ->
-0000e700: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
-0000e710: 2222 2247 6574 205f 7374 6570 2061 7474  """Get _step att
-0000e720: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
-0000e730: 2020 2069 6620 7365 6c66 2e5f 7374 6570     if self._step
-0000e740: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e750: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e760: 2073 656c 662e 5f73 7465 700a 0a20 2020   self._step..   
-0000e770: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000e780: 6566 2076 6572 7469 6365 7328 7365 6c66  ef vertices(self
-0000e790: 2920 2d3e 206e 756d 7079 2e6e 6461 7272  ) -> numpy.ndarr
-0000e7a0: 6179 3a0a 2020 2020 2020 2020 2222 2247  ay:.        """G
-0000e7b0: 6574 205f 7665 7274 6963 6573 2061 7474  et _vertices att
-0000e7c0: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
-0000e7d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000e7e0: 7665 7274 6963 6573 0a0a 2020 2020 4070  vertices..    @p
-0000e7f0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000e800: 7879 7a72 2873 656c 6629 202d 3e20 6e75  xyzr(self) -> nu
-0000e810: 6d70 792e 6e64 6172 7261 793a 0a20 2020  mpy.ndarray:.   
-0000e820: 2020 2020 2022 2222 4765 7420 7879 7a20       """Get xyz 
-0000e830: 636f 6f72 6469 6e61 7465 7320 616e 6420  coordinates and 
-0000e840: 7261 6469 7573 206f 6620 6d6f 6c65 6375  radius of molecu
-0000e850: 6c65 2061 746f 6d73 2e22 2222 0a20 2020  le atoms.""".   
-0000e860: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000e870: 2e5f 6174 6f6d 6963 5b3a 2c20 343a 5d2e  ._atomic[:, 4:].
-0000e880: 6173 7479 7065 286e 756d 7079 2e66 6c6f  astype(numpy.flo
-0000e890: 6174 3634 290a 0a20 2020 2064 6566 205f  at64)..    def _
-0000e8a0: 7365 745f 6772 6964 2873 656c 662c 2070  set_grid(self, p
-0000e8b0: 6164 6469 6e67 3a20 4f70 7469 6f6e 616c  adding: Optional
-0000e8c0: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2920  [float] = None) 
-0000e8d0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000e8e0: 2022 2222 4465 6669 6e65 2074 6865 2033   """Define the 3
-0000e8f0: 4420 6772 6964 2066 6f72 2074 6865 2074  D grid for the t
-0000e900: 6172 6765 7420 6d6f 6c65 6375 6c65 2e0a  arget molecule..
-0000e910: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000e920: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000e930: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2070  ------.        p
-0000e940: 6164 6469 6e67 203a 2066 6c6f 6174 2c20  adding : float, 
-0000e950: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000e960: 2020 2020 2054 6865 206c 656e 6774 6820       The length 
-0000e970: 746f 2061 6464 2074 6f20 6561 6368 2064  to add to each d
-0000e980: 6972 6563 7469 6f6e 206f 6620 7468 6520  irection of the 
-0000e990: 3344 2067 7269 642c 2062 7920 6465 6661  3D grid, by defa
-0000e9a0: 756c 7420 4e6f 6e65 2e20 4966 204e 6f6e  ult None. If Non
-0000e9b0: 652c 2061 7574 6f6d 6174 6963 616c 6c79  e, automatically
-0000e9c0: 2064 6566 696e 6520 7468 6520 6c65 6e67   define the leng
-0000e9d0: 7468 2062 6173 6564 206f 6e20 6d6f 6c65  th based on mole
-0000e9e0: 6375 6c65 2063 6f6f 7264 696e 6174 6573  cule coordinates
-0000e9f0: 2c20 7072 6f62 6520 7369 7a65 2c20 6772  , probe size, gr
-0000ea00: 6964 2073 7061 6369 6e67 2061 6e64 2061  id spacing and a
-0000ea10: 746f 6d20 7261 6469 692e 0a0a 2020 2020  tom radii...    
-0000ea20: 2020 2020 5261 6973 6573 0a20 2020 2020      Raises.     
-0000ea30: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
-0000ea40: 2020 5479 7065 4572 726f 720a 2020 2020    TypeError.    
-0000ea50: 2020 2020 2020 2020 6070 6164 6469 6e67          `padding
-0000ea60: 6020 6d75 7374 2062 6520 6120 6e6f 6e2d  ` must be a non-
-0000ea70: 6e65 6761 7469 7665 2072 6561 6c20 6e75  negative real nu
-0000ea80: 6d62 6572 2e0a 2020 2020 2020 2020 5661  mber..        Va
-0000ea90: 6c75 6545 7272 6f72 0a20 2020 2020 2020  lueError.       
-0000eaa0: 2020 2020 2060 7061 6464 696e 6760 206d       `padding` m
-0000eab0: 7573 7420 6265 2061 206e 6f6e 2d6e 6567  ust be a non-neg
-0000eac0: 6174 6976 6520 7265 616c 206e 756d 6265  ative real numbe
-0000ead0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-0000eae0: 2020 2020 2020 2023 2050 6164 6469 6e67         # Padding
-0000eaf0: 0a20 2020 2020 2020 2069 6620 7061 6464  .        if padd
-0000eb00: 696e 6720 6973 206e 6f74 204e 6f6e 653a  ing is not None:
-0000eb10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000eb20: 7479 7065 2870 6164 6469 6e67 2920 6e6f  type(padding) no
-0000eb30: 7420 696e 205b 696e 742c 2066 6c6f 6174  t in [int, float
-0000eb40: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000eb50: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-0000eb60: 6f72 2822 6070 6164 6469 6e67 6020 6d75  or("`padding` mu
-0000eb70: 7374 2062 6520 6120 6e6f 6e2d 6e65 6761  st be a non-nega
-0000eb80: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
-0000eb90: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000eba0: 656c 6966 2070 6164 6469 6e67 203c 2030  elif padding < 0
-0000ebb0: 2e30 3a0a 2020 2020 2020 2020 2020 2020  .0:.            
-0000ebc0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000ebd0: 7272 6f72 2822 6070 6164 6469 6e67 6020  rror("`padding` 
-0000ebe0: 6d75 7374 2062 6520 6120 6e6f 6e2d 6e65  must be a non-ne
-0000ebf0: 6761 7469 7665 2072 6561 6c20 6e75 6d62  gative real numb
-0000ec00: 6572 2e22 290a 2020 2020 2020 2020 2020  er.").          
-0000ec10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ec20: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
-0000ec30: 6464 696e 6720 3d20 7061 6464 696e 670a  dding = padding.
-0000ec40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ec50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000ec60: 7061 6464 696e 6720 3d20 7365 6c66 2e5f  padding = self._
-0000ec70: 6765 745f 7061 6464 696e 6728 290a 0a20  get_padding().. 
-0000ec80: 2020 2020 2020 2023 2033 4420 6772 6964         # 3D grid
-0000ec90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000eca0: 2e76 6572 626f 7365 3a0a 2020 2020 2020  .verbose:.      
-0000ecb0: 2020 2020 2020 7072 696e 7428 223e 2043        print("> C
-0000ecc0: 616c 6375 6c61 7469 6e67 2033 4420 6772  alculating 3D gr
-0000ecd0: 6964 2229 0a20 2020 2020 2020 2073 656c  id").        sel
-0000ece0: 662e 5f76 6572 7469 6365 7320 3d20 6765  f._vertices = ge
-0000ecf0: 745f 7665 7274 6963 6573 2873 656c 662e  t_vertices(self.
-0000ed00: 6174 6f6d 6963 2c20 7365 6c66 2e70 6164  atomic, self.pad
-0000ed10: 6469 6e67 2c20 7365 6c66 2e73 7465 7029  ding, self.step)
-0000ed20: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-0000ed30: 696d 203d 205f 6765 745f 6469 6d65 6e73  im = _get_dimens
-0000ed40: 696f 6e73 2873 656c 662e 7665 7274 6963  ions(self.vertic
-0000ed50: 6573 2c20 7365 6c66 2e73 7465 7029 0a20  es, self.step). 
-0000ed60: 2020 2020 2020 2073 656c 662e 5f72 6f74         self._rot
-0000ed70: 6174 696f 6e20 3d20 5f67 6574 5f73 696e  ation = _get_sin
-0000ed80: 636f 7328 7365 6c66 2e76 6572 7469 6365  cos(self.vertice
-0000ed90: 7329 0a20 2020 2020 2020 2069 6620 7365  s).        if se
-0000eda0: 6c66 2e76 6572 626f 7365 3a0a 2020 2020  lf.verbose:.    
-0000edb0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-0000edc0: 7031 3a20 7b73 656c 662e 7665 7274 6963  p1: {self.vertic
-0000edd0: 6573 5b30 5d7d 2229 0a20 2020 2020 2020  es[0]}").       
-0000ede0: 2020 2020 2070 7269 6e74 2866 2270 323a       print(f"p2:
-0000edf0: 207b 7365 6c66 2e76 6572 7469 6365 735b   {self.vertices[
-0000ee00: 315d 7d22 290a 2020 2020 2020 2020 2020  1]}").          
-0000ee10: 2020 7072 696e 7428 6622 7033 3a20 7b73    print(f"p3: {s
-0000ee20: 656c 662e 7665 7274 6963 6573 5b32 5d7d  elf.vertices[2]}
-0000ee30: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
-0000ee40: 7269 6e74 2866 2270 343a 207b 7365 6c66  rint(f"p4: {self
-0000ee50: 2e76 6572 7469 6365 735b 335d 7d22 290a  .vertices[3]}").
-0000ee60: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000ee70: 7428 226e 783a 207b 7d2c 206e 793a 207b  t("nx: {}, ny: {
-0000ee80: 7d2c 206e 7a3a 207b 7d22 2e66 6f72 6d61  }, nz: {}".forma
-0000ee90: 7428 2a73 656c 662e 6469 6d29 290a 2020  t(*self.dim)).  
-0000eea0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000eeb0: 2273 696e 613a 207b 7d2c 2073 696e 623a  "sina: {}, sinb:
-0000eec0: 207b 7d2c 2063 6f73 613a 207b 7d2c 2063   {}, cosa: {}, c
-0000eed0: 6f73 623a 207b 7d22 2e66 6f72 6d61 7428  osb: {}".format(
-0000eee0: 2a73 656c 662e 726f 7461 7469 6f6e 2929  *self.rotation))
-0000eef0: 0a0a 2020 2020 6465 6620 5f67 6574 5f70  ..    def _get_p
-0000ef00: 6164 6469 6e67 2873 656c 6629 202d 3e20  adding(self) -> 
-0000ef10: 666c 6f61 743a 0a20 2020 2020 2020 2022  float:.        "
-0000ef20: 2222 4175 746f 6d61 7469 6361 6c6c 7920  ""Automatically 
-0000ef30: 6465 6669 6e65 2074 6865 2070 6164 6469  define the paddi
-0000ef40: 6e67 2062 6173 6564 206f 6e20 6d6f 6c65  ng based on mole
-0000ef50: 6375 6c65 2063 6f6f 7264 696e 6174 6573  cule coordinates
-0000ef60: 2c20 7072 6f62 6520 7369 7a65 2c20 6772  , probe size, gr
-0000ef70: 6964 2073 7061 6369 6e67 2061 6e64 2061  id spacing and a
-0000ef80: 746f 6d20 7261 6469 692e 0a0a 2020 2020  tom radii...    
-0000ef90: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000efa0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000efb0: 2020 2020 7061 6464 696e 6720 3a20 666c      padding : fl
-0000efc0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-0000efd0: 5468 6520 6c65 6e67 7468 2074 6f20 6164  The length to ad
-0000efe0: 6420 746f 2065 6163 6820 6469 7265 6374  d to each direct
-0000eff0: 696f 6e20 6f66 2074 6865 2033 4420 6772  ion of the 3D gr
-0000f000: 6964 2e0a 2020 2020 2020 2020 2222 220a  id..        """.
-0000f010: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
-0000f020: 3d20 312e 3120 2a20 7365 6c66 2e78 797a  = 1.1 * self.xyz
-0000f030: 725b 3a2c 2033 5d2e 6d61 7828 290a 2020  r[:, 3].max().  
-0000f040: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0000f050: 7072 6573 656e 7461 7469 6f6e 2069 6e20  presentation in 
-0000f060: 5b22 5345 5322 2c20 2253 4153 225d 3a0a  ["SES", "SAS"]:.
-0000f070: 2020 2020 2020 2020 2020 2020 7061 6464              padd
-0000f080: 696e 6720 2b3d 2073 656c 662e 5f70 726f  ing += self._pro
-0000f090: 6265 0a20 2020 2020 2020 2072 6574 7572  be.        retur
-0000f0a0: 6e20 666c 6f61 7428 7061 6464 696e 672e  n float(padding.
-0000f0b0: 726f 756e 6428 6465 6369 6d61 6c73 3d31  round(decimals=1
-0000f0c0: 2929 0a0a 2020 2020 6465 6620 7664 7728  ))..    def vdw(
-0000f0d0: 7365 6c66 2c20 7374 6570 3a20 666c 6f61  self, step: floa
-0000f0e0: 7420 3d20 302e 362c 2070 6164 6469 6e67  t = 0.6, padding
-0000f0f0: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-0000f100: 5d20 3d20 4e6f 6e65 2920 2d3e 204e 6f6e  ] = None) -> Non
-0000f110: 653a 0a20 2020 2020 2020 2022 2222 4669  e:.        """Fi
-0000f120: 6c6c 2074 6865 2033 4420 6772 6964 2077  ll the 3D grid w
-0000f130: 6974 6820 7468 6520 6d6f 6c65 6375 6c65  ith the molecule
-0000f140: 2061 7320 7468 6520 7661 6e20 6465 7220   as the van der 
-0000f150: 5761 616c 7320 7375 7266 6163 6520 7265  Waals surface re
-0000f160: 7072 6573 656e 7461 7469 6f6e 2e0a 0a20  presentation... 
-0000f170: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000f180: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000f190: 2d2d 2d2d 0a20 2020 2020 2020 2073 7465  ----.        ste
-0000f1a0: 7020 3a20 666c 6f61 742c 206f 7074 696f  p : float, optio
-0000f1b0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000f1c0: 4772 6964 2073 7061 6369 6e67 2028 4129  Grid spacing (A)
-0000f1d0: 2c20 6279 2064 6566 6175 6c74 2030 2e36  , by default 0.6
-0000f1e0: 2e0a 2020 2020 2020 2020 7061 6464 696e  ..        paddin
-0000f1f0: 6720 3a20 666c 6f61 742c 206f 7074 696f  g : float, optio
-0000f200: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000f210: 5468 6520 6c65 6e67 7468 2074 6f20 6164  The length to ad
-0000f220: 6420 746f 2065 6163 6820 6469 7265 6374  d to each direct
-0000f230: 696f 6e20 6f66 2074 6865 2033 4420 6772  ion of the 3D gr
-0000f240: 6964 2c20 6279 2064 6566 6175 6c74 204e  id, by default N
-0000f250: 6f6e 652e 2049 6620 4e6f 6e65 2c20 6175  one. If None, au
-0000f260: 746f 6d61 7469 6361 6c6c 7920 6465 6669  tomatically defi
-0000f270: 6e65 2074 6865 206c 656e 6774 6820 6261  ne the length ba
-0000f280: 7365 6420 6f6e 206d 6f6c 6563 756c 6520  sed on molecule 
-0000f290: 636f 6f72 6469 6e61 7465 732c 2070 726f  coordinates, pro
-0000f2a0: 6265 2073 697a 652c 2067 7269 6420 7370  be size, grid sp
-0000f2b0: 6163 696e 6720 616e 6420 6174 6f6d 2072  acing and atom r
-0000f2c0: 6164 6969 2e0a 0a20 2020 2020 2020 2052  adii...        R
-0000f2d0: 6169 7365 730a 2020 2020 2020 2020 2d2d  aises.        --
-0000f2e0: 2d2d 2d2d 0a20 2020 2020 2020 2054 7970  ----.        Typ
-0000f2f0: 6545 7272 6f72 0a20 2020 2020 2020 2020  eError.         
-0000f300: 2020 2060 7374 6570 6020 6d75 7374 2062     `step` must b
-0000f310: 6520 6120 706f 7369 7469 7665 2072 6561  e a positive rea
-0000f320: 6c20 6e75 6d62 6572 2e0a 2020 2020 2020  l number..      
-0000f330: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
-0000f340: 2020 2020 2020 2020 2060 7374 6570 6020           `step` 
-0000f350: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-0000f360: 7665 2072 6561 6c20 6e75 6d62 6572 2e0a  ve real number..
-0000f370: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0000f380: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000f390: 0a20 2020 2020 2020 2054 6865 2060 604d  .        The ``M
-0000f3a0: 6f6c 6563 756c 652e 7664 7728 2960 6020  olecule.vdw()`` 
-0000f3b0: 6d65 7468 6f64 2074 616b 6573 2061 2067  method takes a g
-0000f3c0: 7269 6420 7370 6163 696e 6720 616e 6420  rid spacing and 
-0000f3d0: 7265 7475 726e 7320 6120 4e75 6d50 7920  returns a NumPy 
-0000f3e0: 6172 7261 7920 7769 7468 2074 6865 206d  array with the m
-0000f3f0: 6f6c 6563 756c 6520 706f 696e 7473 2072  olecule points r
-0000f400: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-0000f410: 7664 5720 7375 7266 6163 6520 696e 2074  vdW surface in t
-0000f420: 6865 2033 4420 6772 6964 2e0a 0a20 2020  he 3D grid...   
-0000f430: 2020 2020 203e 3e3e 2023 2047 7269 6420       >>> # Grid 
-0000f440: 5370 6163 696e 6720 2873 7465 7029 3a20  Spacing (step): 
-0000f450: 302e 310a 2020 2020 2020 2020 3e3e 3e20  0.1.        >>> 
-0000f460: 7374 6570 203d 2030 2e31 0a20 2020 2020  step = 0.1.     
-0000f470: 2020 203e 3e3e 206d 6f6c 6563 756c 652e     >>> molecule.
-0000f480: 7664 7728 7374 6570 3d73 7465 7029 0a20  vdw(step=step). 
-0000f490: 2020 2020 2020 203e 3e3e 206d 6f6c 6563         >>> molec
-0000f4a0: 756c 652e 6772 6964 0a20 2020 2020 2020  ule.grid.       
-0000f4b0: 2061 7272 6179 285b 5b5b 312c 2031 2c20   array([[[1, 1, 
-0000f4c0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-0000f4d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f4e0: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-0000f4f0: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-0000f500: 2020 2020 2020 2020 2020 205b 312c 2031             [1, 1
-0000f510: 2c20 312c 202e 2e2e 2c20 312c 2031 2c20  , 1, ..., 1, 1, 
-0000f520: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-0000f530: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
-0000f540: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-0000f550: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-0000f560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f570: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-0000f580: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-0000f590: 2020 2020 2020 2020 2020 205b 312c 2031             [1, 1
-0000f5a0: 2c20 312c 202e 2e2e 2c20 312c 2031 2c20  , 1, ..., 1, 1, 
-0000f5b0: 315d 5d2c 0a20 2020 2020 2020 2020 2020  1]],.           
-0000f5c0: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
-0000f5d0: 2020 2020 2020 2020 5b5b 312c 2031 2c20          [[1, 1, 
-0000f5e0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-0000f5f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f600: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-0000f610: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-0000f620: 2020 2020 2020 2020 2020 205b 312c 2031             [1, 1
-0000f630: 2c20 312c 202e 2e2e 2c20 312c 2031 2c20  , 1, ..., 1, 1, 
-0000f640: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
-0000f650: 2020 2020 2e2e 2e2c 0a20 2020 2020 2020      ...,.       
-0000f660: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
-0000f670: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
-0000f680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f690: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-0000f6a0: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-0000f6b0: 2020 2020 2020 2020 2020 205b 312c 2031             [1, 1
-0000f6c0: 2c20 312c 202e 2e2e 2c20 312c 2031 2c20  , 1, ..., 1, 1, 
-0000f6d0: 315d 5d5d 2c20 6474 7970 653d 696e 7433  1]]], dtype=int3
-0000f6e0: 3229 0a20 2020 2020 2020 2022 2222 0a20  2).        """. 
-0000f6f0: 2020 2020 2020 2066 726f 6d20 5f70 794b         from _pyK
-0000f700: 5646 696e 6465 7220 696d 706f 7274 205f  VFinder import _
-0000f710: 6669 6c6c 5f72 6563 6570 746f 720a 0a20  fill_receptor.. 
-0000f720: 2020 2020 2020 2023 2043 6865 636b 2061         # Check a
-0000f730: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-0000f740: 2069 6620 7479 7065 2873 7465 7029 206e   if type(step) n
-0000f750: 6f74 2069 6e20 5b69 6e74 2c20 666c 6f61  ot in [int, floa
-0000f760: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
-0000f770: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-0000f780: 2260 7374 6570 6020 6d75 7374 2062 6520  "`step` must be 
-0000f790: 6120 706f 7374 6976 6520 7265 616c 206e  a postive real n
-0000f7a0: 756d 6265 722e 2229 0a20 2020 2020 2020  umber.").       
-0000f7b0: 2065 6c69 6620 7374 6570 203c 3d20 302e   elif step <= 0.
-0000f7c0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0000f7d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000f7e0: 2260 7374 6570 6020 6d75 7374 2062 6520  "`step` must be 
-0000f7f0: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
-0000f800: 6e75 6d62 6572 2e22 290a 2020 2020 2020  number.").      
-0000f810: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f820: 2020 2020 7365 6c66 2e5f 7374 6570 203d      self._step =
-0000f830: 2073 7465 700a 0a20 2020 2020 2020 2023   step..        #
-0000f840: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
-0000f850: 2020 2020 7365 6c66 2e5f 7265 7072 6573      self._repres
-0000f860: 656e 7461 7469 6f6e 203d 2022 7664 5722  entation = "vdW"
-0000f870: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-0000f880: 726f 6265 203d 204e 6f6e 650a 0a20 2020  robe = None..   
-0000f890: 2020 2020 2023 2044 6566 696e 6520 3344       # Define 3D
-0000f8a0: 2067 7269 640a 2020 2020 2020 2020 7365   grid.        se
-0000f8b0: 6c66 2e5f 7365 745f 6772 6964 2870 6164  lf._set_grid(pad
-0000f8c0: 6469 6e67 290a 0a20 2020 2020 2020 2023  ding)..        #
-0000f8d0: 2076 616e 2064 6572 2057 6161 6c73 2061   van der Waals a
-0000f8e0: 746f 6d73 2028 6861 7264 2073 7068 6572  toms (hard spher
-0000f8f0: 6520 6d6f 6465 6c29 2074 6f20 6772 6964  e model) to grid
-0000f900: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000f910: 2e76 6572 626f 7365 3a0a 2020 2020 2020  .verbose:.      
-0000f920: 2020 2020 2020 7072 696e 7428 223e 2049        print("> I
-0000f930: 6e73 6572 7469 6e67 2061 746f 6d73 2077  nserting atoms w
-0000f940: 6974 6820 7661 6e20 6465 7220 5761 616c  ith van der Waal
-0000f950: 7320 7261 6469 6920 696e 746f 2033 4420  s radii into 3D 
-0000f960: 6772 6964 2229 0a20 2020 2020 2020 2073  grid").        s
-0000f970: 656c 662e 5f67 7269 6420 3d20 5f66 696c  elf._grid = _fil
-0000f980: 6c5f 7265 6365 7074 6f72 280a 2020 2020  l_receptor(.    
-0000f990: 2020 2020 2020 2020 7365 6c66 2e6e 7820          self.nx 
-0000f9a0: 2a20 7365 6c66 2e6e 7920 2a20 7365 6c66  * self.ny * self
-0000f9b0: 2e6e 7a2c 0a20 2020 2020 2020 2020 2020  .nz,.           
-0000f9c0: 2073 656c 662e 6e78 2c0a 2020 2020 2020   self.nx,.      
-0000f9d0: 2020 2020 2020 7365 6c66 2e6e 792c 0a20        self.ny,. 
-0000f9e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f9f0: 6e7a 2c0a 2020 2020 2020 2020 2020 2020  nz,.            
-0000fa00: 7365 6c66 2e78 797a 722c 0a20 2020 2020  self.xyzr,.     
-0000fa10: 2020 2020 2020 2073 656c 662e 7031 2c0a         self.p1,.
-0000fa20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fa30: 2e72 6f74 6174 696f 6e2c 0a20 2020 2020  .rotation,.     
-0000fa40: 2020 2020 2020 2073 656c 662e 7374 6570         self.step
-0000fa50: 2c0a 2020 2020 2020 2020 2020 2020 302e  ,.            0.
-0000fa60: 302c 0a20 2020 2020 2020 2020 2020 2046  0,.            F
-0000fa70: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0000fa80: 2020 7365 6c66 2e6e 7468 7265 6164 732c    self.nthreads,
-0000fa90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000faa0: 662e 7665 7262 6f73 652c 0a20 2020 2020  f.verbose,.     
-0000fab0: 2020 2029 2e72 6573 6861 7065 2873 656c     ).reshape(sel
-0000fac0: 662e 6e78 2c20 7365 6c66 2e6e 792c 2073  f.nx, self.ny, s
-0000fad0: 656c 662e 6e7a 290a 0a20 2020 2064 6566  elf.nz)..    def
-0000fae0: 2073 7572 6661 6365 280a 2020 2020 2020   surface(.      
-0000faf0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000fb00: 7374 6570 3a20 666c 6f61 7420 3d20 302e  step: float = 0.
-0000fb10: 362c 0a20 2020 2020 2020 2070 726f 6265  6,.        probe
-0000fb20: 3a20 666c 6f61 7420 3d20 312e 342c 0a20  : float = 1.4,. 
-0000fb30: 2020 2020 2020 2073 7572 6661 6365 3a20         surface: 
-0000fb40: 7374 7220 3d20 2253 4553 222c 0a20 2020  str = "SES",.   
-0000fb50: 2020 2020 2070 6164 6469 6e67 3a20 4f70       padding: Op
-0000fb60: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
-0000fb70: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 204e  None,.    ) -> N
-0000fb80: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000fb90: 4669 6c6c 2074 6865 2033 4420 6772 6964  Fill the 3D grid
-0000fba0: 2077 6974 6820 7468 6520 6d6f 6c65 6375   with the molecu
-0000fbb0: 6c65 2061 7320 7468 6520 7661 6e20 6465  le as the van de
-0000fbc0: 7220 5761 616c 7320 7375 7266 6163 6520  r Waals surface 
-0000fbd0: 7265 7072 6573 656e 7461 7469 6f6e 2e0a  representation..
-0000fbe0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000fbf0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000fc00: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
-0000fc10: 7465 7020 3a20 666c 6f61 742c 206f 7074  tep : float, opt
-0000fc20: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000fc30: 2020 4772 6964 2073 7061 6369 6e67 2028    Grid spacing (
-0000fc40: 4129 2c20 6279 2064 6566 6175 6c74 2030  A), by default 0
-0000fc50: 2e36 2e0a 2020 2020 2020 2020 7072 6f62  .6..        prob
-0000fc60: 6520 3a20 666c 6f61 742c 206f 7074 696f  e : float, optio
-0000fc70: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000fc80: 5370 6865 7269 6361 6c20 7072 6f62 6520  Spherical probe 
-0000fc90: 7369 7a65 2074 6f20 6465 6669 6e65 2074  size to define t
-0000fca0: 6865 206d 6f6c 6563 756c 6172 2073 7572  he molecular sur
-0000fcb0: 6661 6365 2062 6173 6564 206f 6e20 6120  face based on a 
-0000fcc0: 6d6f 6c65 6375 6c61 7220 7265 7072 6573  molecular repres
-0000fcd0: 656e 7461 7469 6f6e 2c20 6279 2064 6566  entation, by def
-0000fce0: 6175 6c74 2031 2e34 2e0a 2020 2020 2020  ault 1.4..      
-0000fcf0: 2020 7375 7266 6163 6520 3a20 7374 722c    surface : str,
-0000fd00: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000fd10: 2020 2020 2020 4d6f 6c65 6375 6c61 7220        Molecular 
-0000fd20: 7375 7266 6163 6520 7265 7072 6573 656e  surface represen
-0000fd30: 7461 7469 6f6e 2e20 4b65 7977 6f72 6473  tation. Keywords
-0000fd40: 206f 7074 696f 6e73 2061 7265 2076 6457   options are vdW
-0000fd50: 2028 7661 6e20 6465 7220 5761 616c 7320   (van der Waals 
-0000fd60: 7375 7266 6163 6529 2c20 5345 5320 2853  surface), SES (S
-0000fd70: 6f6c 7665 6e74 2045 7863 6c75 6465 6420  olvent Excluded 
-0000fd80: 5375 7266 6163 6529 206f 7220 5341 5320  Surface) or SAS 
-0000fd90: 2853 6f6c 7665 6e74 2041 6363 6573 7369  (Solvent Accessi
-0000fda0: 626c 6520 5375 7266 6163 6529 2c20 6279  ble Surface), by
-0000fdb0: 2064 6566 6175 6c74 2022 5345 5322 2e0a   default "SES"..
-0000fdc0: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
-0000fdd0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-0000fde0: 6c0a 2020 2020 2020 2020 2020 2020 5468  l.            Th
-0000fdf0: 6520 6c65 6e67 7468 2074 6f20 6164 6420  e length to add 
-0000fe00: 746f 2065 6163 6820 6469 7265 6374 696f  to each directio
-0000fe10: 6e20 6f66 2074 6865 2033 4420 6772 6964  n of the 3D grid
-0000fe20: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-0000fe30: 652e 2049 6620 4e6f 6e65 2c20 6175 746f  e. If None, auto
-0000fe40: 6d61 7469 6361 6c6c 7920 6465 6669 6e65  matically define
-0000fe50: 2074 6865 206c 656e 6774 6820 6261 7365   the length base
-0000fe60: 6420 6f6e 206d 6f6c 6563 756c 6520 636f  d on molecule co
-0000fe70: 6f72 6469 6e61 7465 732c 2070 726f 6265  ordinates, probe
-0000fe80: 2073 697a 652c 2067 7269 6420 7370 6163   size, grid spac
-0000fe90: 696e 6720 616e 6420 6174 6f6d 2072 6164  ing and atom rad
-0000fea0: 6969 2e0a 0a20 2020 2020 2020 2052 6169  ii...        Rai
-0000feb0: 7365 730a 2020 2020 2020 2020 2d2d 2d2d  ses.        ----
-0000fec0: 2d2d 0a20 2020 2020 2020 2054 7970 6545  --.        TypeE
-0000fed0: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-0000fee0: 2060 7374 6570 6020 6d75 7374 2062 6520   `step` must be 
-0000fef0: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
-0000ff00: 6e75 6d62 6572 2e0a 2020 2020 2020 2020  number..        
-0000ff10: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-0000ff20: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
-0000ff30: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
-0000ff40: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
-0000ff50: 2020 2020 2020 5479 7065 4572 726f 720a        TypeError.
-0000ff60: 2020 2020 2020 2020 2020 2020 6070 726f              `pro
-0000ff70: 6265 5f6f 7574 6020 6d75 7374 2062 6520  be_out` must be 
-0000ff80: 6120 706f 7369 7469 7665 2072 6561 6c20  a positive real 
-0000ff90: 6e75 6d62 6572 2e0a 2020 2020 2020 2020  number..        
-0000ffa0: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-0000ffb0: 2020 2020 2020 2060 7072 6f62 655f 6f75         `probe_ou
-0000ffc0: 7460 206d 7573 7420 6265 2061 2070 6f73  t` must be a pos
-0000ffd0: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
-0000ffe0: 722e 0a0a 2020 2020 2020 2020 4578 616d  r...        Exam
-0000fff0: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
-00010000: 2d2d 2d0a 2020 2020 2020 2020 5468 6520  ---.        The 
-00010010: 6060 4d6f 6c65 6375 6c65 2e73 7572 6661  ``Molecule.surfa
-00010020: 6365 2829 6060 206d 6574 686f 6420 7461  ce()`` method ta
-00010030: 6b65 7320 7468 6520 6772 6964 2073 7061  kes the grid spa
-00010040: 6369 6e67 2c20 7468 6520 7370 6865 7269  cing, the spheri
-00010050: 6361 6c20 7072 6f62 6520 7369 7a65 2074  cal probe size t
-00010060: 6f20 6d6f 6465 6c20 7468 6520 7375 7266  o model the surf
-00010070: 6163 652c 2074 6865 2073 7572 6661 6365  ace, the surface
-00010080: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00010090: 616e 6420 7265 7475 726e 7320 6120 4e75  and returns a Nu
-000100a0: 6d50 7920 6172 7261 7920 7769 7468 2074  mPy array with t
-000100b0: 6865 206d 6f6c 6563 756c 6520 706f 696e  he molecule poin
-000100c0: 7473 2072 6570 7265 7365 6e74 696e 6720  ts representing 
-000100d0: 7468 6520 5345 5320 696e 2074 6865 2033  the SES in the 3
-000100e0: 4420 6772 6964 2e0a 0a20 2020 2020 2020  D grid...       
-000100f0: 2054 6865 206d 6f6c 6563 756c 6172 2073   The molecular s
-00010100: 7572 6661 6365 2063 616e 2062 6520 6d6f  urface can be mo
-00010110: 6465 6c6c 6564 2061 733a 0a0a 2020 2020  delled as:..    
-00010120: 2020 2020 2020 2020 2a20 536f 6c76 656e          * Solven
-00010130: 7420 4578 636c 7564 6564 2053 7572 6661  t Excluded Surfa
-00010140: 6365 2028 5345 5329 3a0a 0a20 2020 2020  ce (SES):..     
-00010150: 2020 2020 2020 203e 3e3e 2023 2053 7572         >>> # Sur
-00010160: 6661 6365 2052 6570 7265 7365 6e74 6174  face Representat
-00010170: 696f 6e3a 2053 4553 0a20 2020 2020 2020  ion: SES.       
-00010180: 2020 2020 203e 3e3e 2073 7572 6661 6365       >>> surface
-00010190: 203d 2027 5345 5327 0a20 2020 2020 2020   = 'SES'.       
-000101a0: 2020 2020 203e 3e3e 2023 2047 7269 6420       >>> # Grid 
-000101b0: 5370 6163 696e 6720 2873 7465 7029 3a20  Spacing (step): 
-000101c0: 302e 310a 2020 2020 2020 2020 2020 2020  0.1.            
-000101d0: 3e3e 3e20 7374 6570 203d 2030 2e31 0a20  >>> step = 0.1. 
-000101e0: 2020 2020 2020 2020 2020 203e 3e3e 2023             >>> #
-000101f0: 2053 7068 6572 6963 616c 2050 726f 6265   Spherical Probe
-00010200: 2028 7072 6f62 6529 3a20 312e 340a 2020   (probe): 1.4.  
-00010210: 2020 2020 2020 2020 2020 3e3e 3e20 7072            >>> pr
-00010220: 6f62 6520 3d20 312e 340a 2020 2020 2020  obe = 1.4.      
-00010230: 2020 2020 2020 3e3e 3e20 6d6f 6c65 6375        >>> molecu
-00010240: 6c65 2e73 7572 6661 6365 2873 7465 703d  le.surface(step=
-00010250: 7374 6570 2c20 7072 6f62 653d 7072 6f62  step, probe=prob
-00010260: 652c 2073 7572 6661 6365 3d73 7572 6661  e, surface=surfa
-00010270: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
-00010280: 3e3e 3e20 6d6f 6c65 6375 6c65 2e67 7269  >>> molecule.gri
-00010290: 640a 2020 2020 2020 2020 2020 2020 6172  d.            ar
-000102a0: 7261 7928 5b5b 5b31 2c20 312c 2031 2c20  ray([[[1, 1, 1, 
-000102b0: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2020 205b 312c 2031 2c20 312c 202e 2e2e     [1, 1, 1, ...
-000102e0: 2c20 312c 2031 2c20 315d 2c0a 2020 2020  , 1, 1, 1],.    
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 5b31 2c20 312c 2031 2c20 2e2e 2e2c 2031  [1, 1, 1, ..., 1
-00010310: 2c20 312c 2031 5d2c 0a20 2020 2020 2020  , 1, 1],.       
-00010320: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-00010330: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010340: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-00010350: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 205b 312c 2031 2c20 312c 202e 2e2e     [1, 1, 1, ...
-00010380: 2c20 312c 2031 2c20 315d 2c0a 2020 2020  , 1, 1, 1],.    
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 5b31 2c20 312c 2031 2c20 2e2e 2e2c 2031  [1, 1, 1, ..., 1
-000103b0: 2c20 312c 2031 5d5d 2c0a 2020 2020 2020  , 1, 1]],.      
-000103c0: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-000103d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000103e0: 2020 2020 205b 5b31 2c20 312c 2031 2c20       [[1, 1, 1, 
-000103f0: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 205b 312c 2031 2c20 312c 202e 2e2e     [1, 1, 1, ...
-00010420: 2c20 312c 2031 2c20 315d 2c0a 2020 2020  , 1, 1, 1],.    
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 5b31 2c20 312c 2031 2c20 2e2e 2e2c 2031  [1, 1, 1, ..., 1
-00010450: 2c20 312c 2031 5d2c 0a20 2020 2020 2020  , 1, 1],.       
-00010460: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-00010470: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010480: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
-00010490: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104b0: 2020 205b 312c 2031 2c20 312c 202e 2e2e     [1, 1, 1, ...
-000104c0: 2c20 312c 2031 2c20 315d 2c0a 2020 2020  , 1, 1, 1],.    
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 5b31 2c20 312c 2031 2c20 2e2e 2e2c 2031  [1, 1, 1, ..., 1
-000104f0: 2c20 312c 2031 5d5d 5d2c 2064 7479 7065  , 1, 1]]], dtype
-00010500: 3d69 6e74 3332 290a 0a20 2020 2020 2020  =int32)..       
-00010510: 2054 6865 206d 6f6c 6563 756c 6172 2073   The molecular s
-00010520: 7572 6661 6365 2063 616e 2062 6520 6d6f  urface can be mo
-00010530: 6465 6c6c 6564 2061 733a 0a0a 2020 2020  delled as:..    
-00010540: 2020 2020 2020 2020 2a20 536f 6c76 656e          * Solven
-00010550: 7420 4163 6365 7373 6962 6c65 2053 7572  t Accessible Sur
-00010560: 6661 6365 2028 5341 5329 3a0a 0a20 2020  face (SAS):..   
-00010570: 2020 2020 2020 2020 203e 3e3e 2023 2053           >>> # S
-00010580: 7572 6661 6365 2052 6570 7265 7365 6e74  urface Represent
-00010590: 6174 696f 6e3a 2053 4153 0a20 2020 2020  ation: SAS.     
-000105a0: 2020 2020 2020 203e 3e3e 2073 7572 6661         >>> surfa
-000105b0: 6365 203d 2027 5341 5327 0a20 2020 2020  ce = 'SAS'.     
-000105c0: 2020 2020 2020 203e 3e3e 2023 2047 7269         >>> # Gri
-000105d0: 6420 5370 6163 696e 6720 2873 7465 7029  d Spacing (step)
-000105e0: 3a20 302e 310a 2020 2020 2020 2020 2020  : 0.1.          
-000105f0: 2020 3e3e 3e20 7374 6570 203d 2030 2e31    >>> step = 0.1
-00010600: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00010610: 2023 2053 7068 6572 6963 616c 2050 726f   # Spherical Pro
-00010620: 6265 2028 7072 6f62 6529 3a20 312e 340a  be (probe): 1.4.
-00010630: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00010640: 7072 6f62 6520 3d20 312e 340a 2020 2020  probe = 1.4.    
-00010650: 2020 2020 2020 2020 3e3e 3e20 6d6f 6c65          >>> mole
-00010660: 6375 6c65 2e73 7572 6661 6365 2873 7465  cule.surface(ste
-00010670: 703d 7374 6570 2c20 7072 6f62 653d 7072  p=step, probe=pr
-00010680: 6f62 652c 2073 7572 6661 6365 3d73 7572  obe, surface=sur
-00010690: 6661 6365 290a 2020 2020 2020 2020 2020  face).          
-000106a0: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 2e67    >>> molecule.g
-000106b0: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
-000106c0: 6172 7261 7928 5b5b 5b31 2c20 312c 2031  array([[[1, 1, 1
-000106d0: 2c20 2e2e 2e2c 2031 2c20 312c 2031 5d2c  , ..., 1, 1, 1],
-000106e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106f0: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
-00010700: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
-00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-00010730: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-00010740: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00010750: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
-00010760: 2020 2020 2020 2020 5b31 2c20 312c 2031          [1, 1, 1
-00010770: 2c20 2e2e 2e2c 2031 2c20 312c 2031 5d2c  , ..., 1, 1, 1],
-00010780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010790: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
-000107a0: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
-000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107c0: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-000107d0: 2031 2c20 312c 2031 5d5d 2c0a 2020 2020   1, 1, 1]],.    
-000107e0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-000107f0: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
-00010800: 2020 2020 2020 205b 5b31 2c20 312c 2031         [[1, 1, 1
-00010810: 2c20 2e2e 2e2c 2031 2c20 312c 2031 5d2c  , ..., 1, 1, 1],
-00010820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010830: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
-00010840: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
-00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-00010870: 2031 2c20 312c 2031 5d2c 0a20 2020 2020   1, 1, 1],.     
-00010880: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-00010890: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
-000108a0: 2020 2020 2020 2020 5b31 2c20 312c 2031          [1, 1, 1
-000108b0: 2c20 2e2e 2e2c 2031 2c20 312c 2031 5d2c  , ..., 1, 1, 1],
-000108c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108d0: 2020 2020 205b 312c 2031 2c20 312c 202e       [1, 1, 1, .
-000108e0: 2e2e 2c20 312c 2031 2c20 315d 2c0a 2020  .., 1, 1, 1],.  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 5b31 2c20 312c 2031 2c20 2e2e 2e2c    [1, 1, 1, ...,
-00010910: 2031 2c20 312c 2031 5d5d 5d2c 2064 7479   1, 1, 1]]], dty
-00010920: 7065 3d69 6e74 3332 290a 2020 2020 2020  pe=int32).      
-00010930: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
-00010940: 6f6d 205f 7079 4b56 4669 6e64 6572 2069  om _pyKVFinder i
-00010950: 6d70 6f72 7420 5f66 696c 6c5f 7265 6365  mport _fill_rece
-00010960: 7074 6f72 0a0a 2020 2020 2020 2020 2320  ptor..        # 
-00010970: 4368 6563 6b20 6172 6775 6d65 6e74 730a  Check arguments.
-00010980: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00010990: 7374 6570 2920 6e6f 7420 696e 205b 696e  step) not in [in
-000109a0: 742c 2066 6c6f 6174 5d3a 0a20 2020 2020  t, float]:.     
-000109b0: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-000109c0: 6545 7272 6f72 2822 6073 7465 7060 206d  eError("`step` m
-000109d0: 7573 7420 6265 2061 2070 6f73 7469 7665  ust be a postive
-000109e0: 2072 6561 6c20 6e75 6d62 6572 2e22 290a   real number.").
-000109f0: 2020 2020 2020 2020 656c 6966 2073 7465          elif ste
-00010a00: 7020 3c3d 2030 2e30 3a0a 2020 2020 2020  p <= 0.0:.      
-00010a10: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00010a20: 6545 7272 6f72 2822 6073 7465 7060 206d  eError("`step` m
-00010a30: 7573 7420 6265 2061 2070 6f73 6974 6976  ust be a positiv
-00010a40: 6520 7265 616c 206e 756d 6265 722e 2229  e real number.")
-00010a50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00010a60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010a70: 5f73 7465 7020 3d20 7374 6570 0a0a 2020  _step = step..  
-00010a80: 2020 2020 2020 2320 5072 6f62 650a 2020        # Probe.  
-00010a90: 2020 2020 2020 6966 2074 7970 6528 7072        if type(pr
-00010aa0: 6f62 6529 206e 6f74 2069 6e20 5b69 6e74  obe) not in [int
-00010ab0: 2c20 666c 6f61 742c 206e 756d 7079 2e66  , float, numpy.f
-00010ac0: 6c6f 6174 3634 5d3a 0a20 2020 2020 2020  loat64]:.       
-00010ad0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-00010ae0: 7272 6f72 2822 6070 726f 6265 5f6f 7574  rror("`probe_out
-00010af0: 6020 6d75 7374 2062 6520 6120 6e6f 6e2d  ` must be a non-
-00010b00: 6e65 6761 7469 7665 2072 6561 6c20 6e75  negative real nu
-00010b10: 6d62 6572 2e22 290a 2020 2020 2020 2020  mber.").        
-00010b20: 656c 6966 2070 726f 6265 203c 3d20 302e  elif probe <= 0.
-00010b30: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00010b40: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00010b50: 2260 7072 6f62 655f 6f75 7460 206d 7573  "`probe_out` mus
-00010b60: 7420 6265 2061 206e 6f6e 2d6e 6567 6174  t be a non-negat
-00010b70: 6976 6520 7265 616c 206e 756d 6265 722e  ive real number.
-00010b80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00010b90: 5f70 726f 6265 203d 2070 726f 6265 0a0a  _probe = probe..
-00010ba0: 2020 2020 2020 2020 2320 5375 7266 6163          # Surfac
-00010bb0: 650a 2020 2020 2020 2020 6966 2073 7572  e.        if sur
-00010bc0: 6661 6365 203d 3d20 2253 4553 223a 0a20  face == "SES":. 
-00010bd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00010be0: 6c66 2e76 6572 626f 7365 3a0a 2020 2020  lf.verbose:.    
-00010bf0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010c00: 7428 223e 2053 7572 6661 6365 2072 6570  t("> Surface rep
-00010c10: 7265 7365 6e74 6174 696f 6e3a 2053 6f6c  resentation: Sol
-00010c20: 7665 6e74 2045 7863 6c75 6465 6420 5375  vent Excluded Su
-00010c30: 7266 6163 6520 2853 4553 292e 2229 0a20  rface (SES)."). 
-00010c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010c50: 5f72 6570 7265 7365 6e74 6174 696f 6e20  _representation 
-00010c60: 3d20 7375 7266 6163 650a 2020 2020 2020  = surface.      
-00010c70: 2020 2020 2020 7375 7266 6163 6520 3d20        surface = 
-00010c80: 5472 7565 0a20 2020 2020 2020 2065 6c69  True.        eli
-00010c90: 6620 7375 7266 6163 6520 3d3d 2022 5341  f surface == "SA
-00010ca0: 5322 3a0a 2020 2020 2020 2020 2020 2020  S":.            
-00010cb0: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-00010cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cd0: 2070 7269 6e74 2822 3e20 5375 7266 6163   print("> Surfac
-00010ce0: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
-00010cf0: 3a20 536f 6c76 656e 7420 4163 6365 7373  : Solvent Access
-00010d00: 6962 6c65 2053 7572 6661 6365 2028 5341  ible Surface (SA
-00010d10: 5329 2e22 290a 2020 2020 2020 2020 2020  S).").          
-00010d20: 2020 7365 6c66 2e5f 7265 7072 6573 656e    self._represen
-00010d30: 7461 7469 6f6e 203d 2073 7572 6661 6365  tation = surface
-00010d40: 0a20 2020 2020 2020 2020 2020 2073 7572  .            sur
-00010d50: 6661 6365 203d 2046 616c 7365 0a20 2020  face = False.   
-00010d60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010d70: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00010d80: 7565 4572 726f 7228 6622 6073 7572 6661  ueError(f"`surfa
-00010d90: 6365 6020 6d75 7374 2062 6520 5341 5320  ce` must be SAS 
-00010da0: 6f72 2053 4553 2c20 6e6f 7420 7b73 7572  or SES, not {sur
-00010db0: 6661 6365 7d2e 2229 0a0a 2020 2020 2020  face}.")..      
-00010dc0: 2020 2320 4465 6669 6e65 2033 4420 6772    # Define 3D gr
-00010dd0: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-00010de0: 5f73 6574 5f67 7269 6428 7061 6464 696e  _set_grid(paddin
-00010df0: 6729 0a0a 2020 2020 2020 2020 2320 4d6f  g)..        # Mo
-00010e00: 6c65 6375 6c61 7220 7375 7266 6163 6520  lecular surface 
-00010e10: 2853 4553 206f 7220 5341 5329 2074 6f20  (SES or SAS) to 
-00010e20: 6772 6964 0a20 2020 2020 2020 2073 656c  grid.        sel
-00010e30: 662e 5f67 7269 6420 3d20 5f66 696c 6c5f  f._grid = _fill_
-00010e40: 7265 6365 7074 6f72 280a 2020 2020 2020  receptor(.      
-00010e50: 2020 2020 2020 7365 6c66 2e6e 7820 2a20        self.nx * 
-00010e60: 7365 6c66 2e6e 7920 2a20 7365 6c66 2e6e  self.ny * self.n
-00010e70: 7a2c 0a20 2020 2020 2020 2020 2020 2073  z,.            s
-00010e80: 656c 662e 6e78 2c0a 2020 2020 2020 2020  elf.nx,.        
-00010e90: 2020 2020 7365 6c66 2e6e 792c 0a20 2020      self.ny,.   
-00010ea0: 2020 2020 2020 2020 2073 656c 662e 6e7a           self.nz
-00010eb0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00010ec0: 6c66 2e78 797a 722c 0a20 2020 2020 2020  lf.xyzr,.       
-00010ed0: 2020 2020 2073 656c 662e 7031 2c0a 2020       self.p1,.  
-00010ee0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010ef0: 6f74 6174 696f 6e2c 0a20 2020 2020 2020  otation,.       
-00010f00: 2020 2020 2073 656c 662e 7374 6570 2c0a       self.step,.
-00010f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010f20: 2e70 726f 6265 2c0a 2020 2020 2020 2020  .probe,.        
-00010f30: 2020 2020 7375 7266 6163 652c 0a20 2020      surface,.   
-00010f40: 2020 2020 2020 2020 2073 656c 662e 6e74           self.nt
-00010f50: 6872 6561 6473 2c0a 2020 2020 2020 2020  hreads,.        
-00010f60: 2020 2020 7365 6c66 2e76 6572 626f 7365      self.verbose
-00010f70: 2c0a 2020 2020 2020 2020 292e 7265 7368  ,.        ).resh
-00010f80: 6170 6528 7365 6c66 2e6e 782c 2073 656c  ape(self.nx, sel
-00010f90: 662e 6e79 2c20 7365 6c66 2e6e 7a29 0a0a  f.ny, self.nz)..
-00010fa0: 2020 2020 6465 6620 766f 6c75 6d65 2873      def volume(s
-00010fb0: 656c 6629 202d 3e20 666c 6f61 743a 0a20  elf) -> float:. 
-00010fc0: 2020 2020 2020 2022 2222 4573 7469 6d61         """Estima
-00010fd0: 7465 2074 6865 2076 6f6c 756d 6520 6f66  te the volume of
-00010fe0: 2074 6865 206d 6f6c 6563 756c 6520 6261   the molecule ba
-00010ff0: 7365 6420 6f6e 2074 6865 206d 6f6c 6563  sed on the molec
-00011000: 756c 6172 2073 7572 6661 6365 2072 6570  ular surface rep
-00011010: 7265 7365 6e74 6174 696f 6e2c 2069 652c  resentation, ie,
-00011020: 2076 6457 2c20 5345 5320 6f72 2053 4153   vdW, SES or SAS
-00011030: 2072 6570 7265 7365 6e74 6174 696f 6e73   representations
-00011040: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00011050: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00011060: 2d2d 0a20 2020 2020 2020 2076 6f6c 756d  --.        volum
-00011070: 6520 3a20 666c 6f61 740a 2020 2020 2020  e : float.      
-00011080: 2020 2020 2020 4d6f 6c65 6375 6c61 7220        Molecular 
-00011090: 766f 6c75 6d65 2028 41c2 b329 2e0a 0a20  volume (A..)... 
-000110a0: 2020 2020 2020 2045 7861 6d70 6c65 0a20         Example. 
-000110b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000110c0: 2020 2020 2020 2057 6974 6820 7468 6520         With the 
-000110d0: 6d6f 6c65 6375 6c61 7220 7375 7266 6163  molecular surfac
-000110e0: 6520 6d6f 6465 6c6c 6564 2062 7920 6060  e modelled by ``
-000110f0: 4d6f 6c65 6375 6c65 2e76 6477 2829 6060  Molecule.vdw()``
-00011100: 206f 7220 6060 4d6f 6c65 6375 6c65 2e73   or ``Molecule.s
-00011110: 7572 6661 6365 2829 6060 2c20 7468 6520  urface()``, the 
-00011120: 766f 6c75 6d65 2063 616e 2062 6520 6573  volume can be es
-00011130: 7469 6d61 7465 6420 6279 2072 756e 6e69  timated by runni
-00011140: 6e67 3a0a 0a20 2020 2020 2020 203e 3e3e  ng:..        >>>
-00011150: 206d 6f6c 6563 756c 652e 766f 6c75 6d65   molecule.volume
-00011160: 2829 0a20 2020 2020 2020 2039 302e 380a  ().        90.8.
-00011170: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011180: 2020 2020 6672 6f6d 205f 7079 4b56 4669      from _pyKVFi
-00011190: 6e64 6572 2069 6d70 6f72 7420 5f76 6f6c  nder import _vol
-000111a0: 756d 650a 0a20 2020 2020 2020 2069 6620  ume..        if 
-000111b0: 7365 6c66 2e67 7269 6420 6973 206e 6f74  self.grid is not
-000111c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000111d0: 2020 2076 6f6c 756d 6520 3d20 5f76 6f6c     volume = _vol
-000111e0: 756d 6528 0a20 2020 2020 2020 2020 2020  ume(.           
-000111f0: 2020 2020 2028 7365 6c66 2e67 7269 6420       (self.grid 
-00011200: 3d3d 2030 292e 6173 7479 7065 286e 756d  == 0).astype(num
-00011210: 7079 2e69 6e74 3332 2920 2a20 322c 2073  py.int32) * 2, s
-00011220: 656c 662e 7374 6570 2c20 312c 2073 656c  elf.step, 1, sel
-00011230: 662e 6e74 6872 6561 6473 0a20 2020 2020  f.nthreads.     
-00011240: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00011250: 2020 2020 2072 6574 7572 6e20 666c 6f61       return floa
-00011260: 7428 766f 6c75 6d65 2e72 6f75 6e64 2864  t(volume.round(d
-00011270: 6563 696d 616c 733d 3229 290a 0a20 2020  ecimals=2))..   
-00011280: 2064 6566 2070 7265 7669 6577 2873 656c   def preview(sel
-00011290: 662c 202a 2a6b 7761 7267 7329 202d 3e20  f, **kwargs) -> 
-000112a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000112b0: 2250 7265 7669 6577 2074 6865 206d 6f6c  "Preview the mol
-000112c0: 6563 756c 6172 2073 7572 6661 6365 2069  ecular surface i
-000112d0: 6e20 7468 6520 3344 2067 7269 642e 0a0a  n the 3D grid...
-000112e0: 2020 2020 2020 2020 4578 616d 706c 650a          Example.
-000112f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00011300: 2020 2020 2020 2020 5769 7468 2074 6865          With the
-00011310: 206d 6f6c 6563 756c 6172 2073 7572 6661   molecular surfa
-00011320: 6365 206d 6f64 656c 6c65 6420 6279 2060  ce modelled by `
-00011330: 604d 6f6c 6563 756c 652e 7664 7728 2960  `Molecule.vdw()`
-00011340: 6020 6f72 2060 604d 6f6c 6563 756c 652e  ` or ``Molecule.
-00011350: 7375 7266 6163 6528 2960 602c 2074 6865  surface()``, the
-00011360: 206d 6f64 656c 6c65 6420 6d6f 6c65 6375   modelled molecu
-00011370: 6c65 2069 6e20 7468 6520 3344 2067 7269  le in the 3D gri
-00011380: 6420 6361 6e20 6265 2070 7265 7669 6577  d can be preview
-00011390: 6564 2062 7920 7275 6e6e 696e 673a 0a0a  ed by running:..
-000113a0: 2020 2020 2020 2020 3e3e 3e20 6d6f 6c65          >>> mole
-000113b0: 6375 6c65 2e70 7265 7669 6577 2829 0a20  cule.preview(). 
-000113c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000113d0: 2020 2069 6620 7365 6c66 2e67 7269 6420     if self.grid 
-000113e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000113f0: 2020 2020 2020 2020 2066 726f 6d20 706c           from pl
-00011400: 6f74 6c79 2e65 7870 7265 7373 2069 6d70  otly.express imp
-00011410: 6f72 7420 7363 6174 7465 725f 3364 0a0a  ort scatter_3d..
-00011420: 2020 2020 2020 2020 2020 2020 782c 2079              x, y
-00011430: 2c20 7a20 3d20 6e75 6d70 792e 6e6f 6e7a  , z = numpy.nonz
-00011440: 6572 6f28 7365 6c66 2e67 7269 6420 3d3d  ero(self.grid ==
-00011450: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-00011460: 6669 6720 3d20 7363 6174 7465 725f 3364  fig = scatter_3d
-00011470: 2878 3d78 2c20 793d 792c 207a 3d7a 2c20  (x=x, y=y, z=z, 
-00011480: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-00011490: 2020 2020 2020 6669 672e 7570 6461 7465        fig.update
-000114a0: 5f6c 6179 6f75 7428 0a20 2020 2020 2020  _layout(.       
-000114b0: 2020 2020 2020 2020 2073 6365 6e65 5f78           scene_x
-000114c0: 6178 6973 5f73 686f 7774 6963 6b6c 6162  axis_showticklab
-000114d0: 656c 733d 4661 6c73 652c 0a20 2020 2020  els=False,.     
-000114e0: 2020 2020 2020 2020 2020 2073 6365 6e65             scene
-000114f0: 5f79 6178 6973 5f73 686f 7774 6963 6b6c  _yaxis_showtickl
-00011500: 6162 656c 733d 4661 6c73 652c 0a20 2020  abels=False,.   
-00011510: 2020 2020 2020 2020 2020 2020 2073 6365               sce
-00011520: 6e65 5f7a 6178 6973 5f73 686f 7774 6963  ne_zaxis_showtic
-00011530: 6b6c 6162 656c 733d 4661 6c73 652c 0a20  klabels=False,. 
-00011540: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00011550: 2020 2020 2020 2020 2066 6967 2e73 686f           fig.sho
-00011560: 7728 290a 0a20 2020 2064 6566 2065 7870  w()..    def exp
-00011570: 6f72 7428 0a20 2020 2020 2020 2073 656c  ort(.        sel
-00011580: 662c 0a20 2020 2020 2020 2066 6e3a 2055  f,.        fn: U
-00011590: 6e69 6f6e 5b73 7472 2c20 7061 7468 6c69  nion[str, pathli
-000115a0: 622e 5061 7468 5d20 3d20 226d 6f6c 6563  b.Path] = "molec
-000115b0: 756c 652e 7064 6222 2c0a 2020 2020 2920  ule.pdb",.    ) 
-000115c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000115d0: 2022 2222 4578 706f 7274 206d 6f6c 6563   """Export molec
-000115e0: 756c 6520 706f 696e 7473 2028 4829 2074  ule points (H) t
-000115f0: 6f20 6120 5044 422d 666f 726d 6174 7465  o a PDB-formatte
-00011600: 6420 6669 6c65 2e0a 0a20 2020 2020 2020  d file...       
-00011610: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00011620: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00011630: 2020 2020 2020 2066 6e20 3a20 556e 696f         fn : Unio
-00011640: 6e5b 7374 722c 2070 6174 686c 6962 2e50  n[str, pathlib.P
-00011650: 6174 685d 2c20 6f70 7469 6f6e 616c 0a20  ath], optional. 
-00011660: 2020 2020 2020 2020 2020 2041 2066 696c             A fil
-00011670: 6520 7061 7468 2074 6f20 7468 6520 6d6f  e path to the mo
-00011680: 6c65 6375 6c61 7220 766f 6c75 6d65 2069  lecular volume i
-00011690: 6e20 7468 6520 6772 6964 2d62 6173 6564  n the grid-based
-000116a0: 2072 6572 7065 7365 6e74 6174 696f 6e20   rerpesentation 
-000116b0: 696e 2050 4442 2066 6f72 6d61 742c 2062  in PDB format, b
-000116c0: 7920 6465 6661 756c 7420 226d 6f6c 6563  y default "molec
-000116d0: 756c 652e 7064 6222 2e0a 0a20 2020 2020  ule.pdb"...     
-000116e0: 2020 2052 6169 7365 730a 2020 2020 2020     Raises.      
-000116f0: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
-00011700: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
-00011710: 2020 2020 2020 2060 666e 6020 6d75 7374         `fn` must
-00011720: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
-00011730: 6120 7061 7468 6c69 622e 5061 7468 2e0a  a pathlib.Path..
-00011740: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00011750: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00011760: 0a20 2020 2020 2020 2057 6974 6820 7468  .        With th
-00011770: 6520 6d6f 6c65 6375 6c61 7220 7375 7266  e molecular surf
-00011780: 6163 6520 6d6f 6465 6c6c 6564 2062 7920  ace modelled by 
-00011790: 6060 4d6f 6c65 6375 6c65 2e76 6477 2829  ``Molecule.vdw()
-000117a0: 6060 206f 7220 6060 4d6f 6c65 6375 6c65  `` or ``Molecule
-000117b0: 2e73 7572 6661 6365 2829 6060 2c20 7468  .surface()``, th
-000117c0: 6520 6d6f 6465 6c6c 6564 206d 6f6c 6563  e modelled molec
-000117d0: 756c 6520 696e 2074 6865 2033 4420 6772  ule in the 3D gr
-000117e0: 6964 2063 616e 2062 6520 6578 706f 7274  id can be export
-000117f0: 6564 2074 6f20 6120 5044 422d 666f 726d  ed to a PDB-form
-00011800: 6174 7465 6420 6669 6c65 2062 7920 7275  atted file by ru
-00011810: 6e6e 696e 673a 0a0a 2020 2020 2020 2020  nning:..        
-00011820: 3e3e 3e20 6d6f 6c65 6375 6c65 2e65 7870  >>> molecule.exp
-00011830: 6f72 7428 276d 6f64 656c 2e70 6462 2729  ort('model.pdb')
-00011840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011850: 2020 2020 2023 2046 696c 656e 616d 6520       # Filename 
-00011860: 2866 6e29 0a20 2020 2020 2020 2069 6620  (fn).        if 
-00011870: 7479 7065 2866 6e29 206e 6f74 2069 6e20  type(fn) not in 
-00011880: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
-00011890: 7468 5d3a 0a20 2020 2020 2020 2020 2020  th]:.           
-000118a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000118b0: 2822 6066 6e60 206d 7573 7420 6265 2061  ("`fn` must be a
-000118c0: 2073 7472 696e 6720 6f72 2061 2070 6174   string or a pat
-000118d0: 686c 6962 2e50 6174 682e 2229 0a20 2020  hlib.Path.").   
-000118e0: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
-000118f0: 286f 732e 7061 7468 2e61 6273 7061 7468  (os.path.abspath
-00011900: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
-00011910: 2866 6e29 292c 2065 7869 7374 5f6f 6b3d  (fn)), exist_ok=
-00011920: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
-00011930: 2053 6176 6520 6772 6964 2074 6f20 5044   Save grid to PD
-00011940: 4220 6669 6c65 0a20 2020 2020 2020 2065  B file.        e
-00011950: 7870 6f72 7428 0a20 2020 2020 2020 2020  xport(.         
-00011960: 2020 2066 6e2c 2028 7365 6c66 2e67 7269     fn, (self.gri
-00011970: 6420 3d3d 2030 292e 6173 7479 7065 286e  d == 0).astype(n
-00011980: 756d 7079 2e69 6e74 3332 2920 2a20 322c  umpy.int32) * 2,
-00011990: 204e 6f6e 652c 2073 656c 662e 7665 7274   None, self.vert
-000119a0: 6963 6573 2c20 7365 6c66 2e73 7465 700a  ices, self.step.
-000119b0: 2020 2020 2020 2020 290a                         ).
+00006230: 6e46 6c65 6d69 6e67 2c20 5261 647a 6963  nFleming, Radzic
+00006240: 6b61 576f 6c66 656e 6465 6e2c 2057 696d  kaWolfenden, Wim
+00006250: 6c65 7957 6869 7465 2c20 5a68 616f 4c6f  leyWhite, ZhaoLo
+00006260: 6e64 6f6e 2920 0a20 2020 2020 2020 206f  ndon) .        o
+00006270: 7220 6120 7061 7468 2074 6f20 6120 544f  r a path to a TO
+00006280: 4d4c 2d66 6f72 6d61 7474 6564 2066 696c  ML-formatted fil
+00006290: 6520 7769 7468 2061 2063 7573 746f 6d20  e with a custom 
+000062a0: 6879 6472 6f70 686f 6269 6369 7479 2073  hydrophobicity s
+000062b0: 6361 6c65 2c0a 2020 2020 2020 2020 6279  cale,.        by
+000062c0: 2064 6566 6175 6c74 2060 4569 7365 6e62   default `Eisenb
+000062d0: 6572 6757 6569 7373 602e 0a20 2020 2073  ergWeiss`..    s
+000062e0: 7572 6661 6365 203a 2073 7472 2c20 6f70  urface : str, op
+000062f0: 7469 6f6e 616c 0a20 2020 2020 2020 204b  tional.        K
+00006300: 6579 776f 7264 7320 6f70 7469 6f6e 7320  eywords options 
+00006310: 6172 6520 5345 5320 2853 6f6c 7665 6e74  are SES (Solvent
+00006320: 2045 7863 6c75 6465 6420 5375 7266 6163   Excluded Surfac
+00006330: 6529 206f 7220 5341 5320 2853 6f6c 7665  e) or SAS (Solve
+00006340: 6e74 0a20 2020 2020 2020 2041 6363 6573  nt.        Acces
+00006350: 7369 626c 6520 5375 7266 6163 6529 2c20  sible Surface), 
+00006360: 6279 2064 6566 6175 6c74 2053 4553 2e0a  by default SES..
+00006370: 2020 2020 6967 6e6f 7265 5f62 6163 6b62      ignore_backb
+00006380: 6f6e 6520 3a20 626f 6f6c 2c20 6f70 7469  one : bool, opti
+00006390: 6f6e 616c 0a20 2020 2020 2020 2057 6865  onal.        Whe
+000063a0: 7468 6572 2074 6f20 6967 6e6f 7265 2062  ther to ignore b
+000063b0: 6163 6b62 6f6e 6520 6174 6f6d 7320 2843  ackbone atoms (C
+000063c0: 2c20 4341 2c20 4e2c 204f 2920 7768 656e  , CA, N, O) when
+000063d0: 2064 6566 696e 696e 6720 696e 7465 7266   defining interf
+000063e0: 6163 650a 2020 2020 2020 2020 7265 7369  ace.        resi
+000063f0: 6475 6573 2c20 6279 2064 6566 6175 6c74  dues, by default
+00006400: 2046 616c 7365 2e0a 2020 2020 6d6f 6465   False..    mode
+00006410: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
+00006420: 6c0a 2020 2020 2020 2020 4d6f 6465 6c20  l.        Model 
+00006430: 6e75 6d62 6572 2c20 6279 2064 6566 6175  number, by defau
+00006440: 6c74 204e 6f6e 652e 2049 6620 4e6f 6e65  lt None. If None
+00006450: 2c20 6b65 6570 2061 746f 6d73 2066 726f  , keep atoms fro
+00006460: 6d20 616c 6c20 6d6f 6465 6c73 2e0a 2020  m all models..  
+00006470: 2020 6e74 6872 6561 6473 203a 2069 6e74    nthreads : int
+00006480: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00006490: 2020 204e 756d 6265 7220 6f66 2074 6872     Number of thr
+000064a0: 6561 6473 2c20 6279 2064 6566 6175 6c74  eads, by default
+000064b0: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
+000064c0: 7468 6520 6e75 6d62 6572 206f 6620 7468  the number of th
+000064d0: 7265 6164 7320 6973 0a20 2020 2020 2020  reads is.       
+000064e0: 2060 6f73 2e63 7075 5f63 6f75 6e74 2829   `os.cpu_count()
+000064f0: 202d 2031 602e 0a20 2020 2076 6572 626f   - 1`..    verbo
+00006500: 7365 203a 2062 6f6f 6c2c 206f 7074 696f  se : bool, optio
+00006510: 6e61 6c0a 2020 2020 2020 2020 5072 696e  nal.        Prin
+00006520: 7420 6578 7472 6120 696e 666f 726d 6174  t extra informat
+00006530: 696f 6e20 746f 2073 7461 6e64 6172 6420  ion to standard 
+00006540: 6f75 7470 7574 2c20 6279 2064 6566 6175  output, by defau
+00006550: 6c74 2046 616c 7365 2e0a 0a20 2020 2052  lt False...    R
+00006560: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00006570: 2d2d 0a20 2020 2072 6573 756c 7473 203a  --.    results :
+00006580: 2070 794b 5646 696e 6465 7252 6573 756c   pyKVFinderResul
+00006590: 7473 0a20 2020 2020 2020 2041 2063 6c61  ts.        A cla
+000065a0: 7373 2077 6974 6820 7468 6520 666f 6c6c  ss with the foll
+000065b0: 6f77 696e 6720 6174 7472 6962 7574 6573  owing attributes
+000065c0: 2064 6566 696e 6564 3a0a 0a20 2020 2020   defined:..     
+000065d0: 2020 2020 2020 202a 2063 6176 6974 6965         * cavitie
+000065e0: 7320 3a20 6e75 6d70 792e 6e64 6172 7261  s : numpy.ndarra
+000065f0: 790a 0a20 2020 2020 2020 2020 2020 2020  y..             
+00006600: 2020 2043 6176 6974 7920 706f 696e 7473     Cavity points
+00006610: 2069 6e20 7468 6520 3344 2067 7269 6420   in the 3D grid 
+00006620: 2863 6176 6974 6965 735b 6e78 5d5b 6e79  (cavities[nx][ny
+00006630: 5d5b 6e7a 5d29 2e0a 2020 2020 2020 2020  ][nz])..        
+00006640: 2020 2020 2020 2020 4361 7669 7469 6573          Cavities
+00006650: 2061 7272 6179 2068 6173 2069 6e74 6567   array has integ
+00006660: 6572 206c 6162 656c 7320 696e 2065 6163  er labels in eac
+00006670: 6820 706f 7369 7469 6f6e 2c20 7468 6174  h position, that
+00006680: 2061 7265 3a0a 0a20 2020 2020 2020 2020   are:..         
+00006690: 2020 2020 2020 202a 202d 313a 2062 756c         * -1: bul
+000066a0: 6b20 706f 696e 7473 3b0a 2020 2020 2020  k points;.      
+000066b0: 2020 2020 2020 2020 2020 2a20 303a 2062            * 0: b
+000066c0: 696f 6d6f 6c65 6375 6c65 2070 6f69 6e74  iomolecule point
+000066d0: 733b 0a20 2020 2020 2020 2020 2020 2020  s;.             
+000066e0: 2020 202a 2031 3a20 656d 7074 7920 7370     * 1: empty sp
+000066f0: 6163 6520 706f 696e 7473 3b0a 2020 2020  ace points;.    
+00006700: 2020 2020 2020 2020 2020 2020 2a20 3e3d              * >=
+00006710: 323a 2063 6176 6974 7920 706f 696e 7473  2: cavity points
+00006720: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+00006730: 2020 2054 6865 2065 6d70 7479 2073 7061     The empty spa
+00006740: 6365 2070 6f69 6e74 7320 6172 6520 7265  ce points are re
+00006750: 6769 6f6e 7320 7468 6174 2064 6f20 6e6f  gions that do no
+00006760: 7420 6d65 6574 2074 6865 2063 686f 7365  t meet the chose
+00006770: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00006780: 2020 766f 6c75 6d65 2063 7574 6f66 6620    volume cutoff 
+00006790: 746f 2062 6520 636f 6e73 6964 6572 6564  to be considered
+000067a0: 2061 2063 6176 6974 792e 0a0a 2020 2020   a cavity...    
+000067b0: 2020 2020 2020 2020 2a20 7375 7266 6163          * surfac
+000067c0: 6520 3a20 6e75 6d70 792e 6e64 6172 7261  e : numpy.ndarra
+000067d0: 790a 0a20 2020 2020 2020 2020 2020 2020  y..             
+000067e0: 2020 2053 7572 6661 6365 2070 6f69 6e74     Surface point
+000067f0: 7320 696e 2074 6865 2033 4420 6772 6964  s in the 3D grid
+00006800: 2028 7375 7266 6163 655b 6e78 5d5b 6e79   (surface[nx][ny
+00006810: 5d5b 6e7a 5d29 2e0a 2020 2020 2020 2020  ][nz])..        
+00006820: 2020 2020 2020 2020 5375 7266 6163 6520          Surface 
+00006830: 6172 7261 7920 6861 7320 696e 7465 6765  array has intege
+00006840: 7220 6c61 6265 6c73 2069 6e20 6561 6368  r labels in each
+00006850: 2070 6f73 6974 696f 6e2c 2074 6861 7420   position, that 
+00006860: 6172 653a 0a0a 2020 2020 2020 2020 2020  are:..          
+00006870: 2020 2020 2020 2a20 2d31 3a20 6275 6c6b        * -1: bulk
+00006880: 2070 6f69 6e74 733b 0a20 2020 2020 2020   points;.       
+00006890: 2020 2020 2020 2020 202a 2030 3a20 6269           * 0: bi
+000068a0: 6f6d 6f6c 6563 756c 6520 6f72 2065 6d70  omolecule or emp
+000068b0: 7479 2073 7061 6365 2070 6f69 6e74 733b  ty space points;
+000068c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000068d0: 202a 203e 3d32 3a20 7375 7266 6163 6520   * >=2: surface 
+000068e0: 706f 696e 7473 2e0a 0a20 2020 2020 2020  points...       
+000068f0: 2020 2020 2020 2020 2054 6865 2065 6d70           The emp
+00006900: 7479 2073 7061 6365 2070 6f69 6e74 7320  ty space points 
+00006910: 6172 6520 7265 6769 6f6e 7320 7468 6174  are regions that
+00006920: 2064 6f20 6e6f 7420 6d65 6574 2074 6865   do not meet the
+00006930: 2063 686f 7365 6e0a 2020 2020 2020 2020   chosen.        
+00006940: 2020 2020 2020 2020 766f 6c75 6d65 2063          volume c
+00006950: 7574 6f66 6620 746f 2062 6520 636f 6e73  utoff to be cons
+00006960: 6964 6572 6564 2061 2063 6176 6974 792e  idered a cavity.
+00006970: 0a0a 2020 2020 2020 2020 2020 2020 2a20  ..            * 
+00006980: 6465 7074 6873 203a 206e 756d 7079 2e6e  depths : numpy.n
+00006990: 6461 7272 6179 2c20 6f70 7469 6f6e 616c  darray, optional
+000069a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000069b0: 2020 4120 6e75 6d70 792e 6e64 6172 7261    A numpy.ndarra
+000069c0: 7920 7769 7468 2064 6570 7468 206f 6620  y with depth of 
+000069d0: 6361 7669 7479 2070 6f69 6e74 7320 2864  cavity points (d
+000069e0: 6570 7468 5b6e 785d 5b6e 795d 5b6e 7a5d  epth[nx][ny][nz]
+000069f0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
+00006a00: 2a20 7363 616c 6573 203a 206e 756d 7079  * scales : numpy
+00006a10: 2e6e 6461 7272 6179 2c20 6f70 7469 6f6e  .ndarray, option
+00006a20: 616c 0a0a 2020 2020 2020 2020 2020 2020  al..            
+00006a30: 2020 2020 4120 6e75 6d70 792e 6e64 6172      A numpy.ndar
+00006a40: 7261 7920 7769 7468 2068 7964 726f 7068  ray with hydroph
+00006a50: 6f62 6963 6974 7920 7363 616c 6520 7661  obicity scale va
+00006a60: 6c75 6520 6d61 7070 6564 2061 7420 7375  lue mapped at su
+00006a70: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
+00006a80: 2020 2020 2020 706f 696e 7473 2028 7363        points (sc
+00006a90: 616c 6573 5b6e 785d 5b6e 795d 5b6e 7a5d  ales[nx][ny][nz]
+00006aa0: 292e 0a0a 2020 2020 2020 2020 2020 2020  )...            
+00006ab0: 2a20 6e63 6176 203a 2069 6e74 0a0a 2020  * ncav : int..  
+00006ac0: 2020 2020 2020 2020 2020 2020 2020 4e75                Nu
+00006ad0: 6d62 6572 206f 6620 6361 7669 7469 6573  mber of cavities
+00006ae0: 2e0a 0a20 2020 2020 2020 2020 2020 202a  ...            *
+00006af0: 2076 6f6c 756d 6520 3a20 4469 6374 5b73   volume : Dict[s
+00006b00: 7472 2c20 666c 6f61 745d 0a0a 2020 2020  tr, float]..    
+00006b10: 2020 2020 2020 2020 2020 2020 4120 6469              A di
+00006b20: 6374 696f 6e61 7279 2077 6974 6820 766f  ctionary with vo
+00006b30: 6c75 6d65 206f 6620 6561 6368 2064 6574  lume of each det
+00006b40: 6563 7465 6420 6361 7669 7479 2e0a 0a20  ected cavity... 
+00006b50: 2020 2020 2020 2020 2020 202a 2061 7265             * are
+00006b60: 6120 3a20 4469 6374 5b73 7472 2c20 666c  a : Dict[str, fl
+00006b70: 6f61 745d 0a0a 2020 2020 2020 2020 2020  oat]..          
+00006b80: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+00006b90: 7279 2077 6974 6820 6172 6561 206f 6620  ry with area of 
+00006ba0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00006bb0: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
+00006bc0: 2020 202a 206d 6178 5f64 6570 7468 203a     * max_depth :
+00006bd0: 2044 6963 745b 7374 722c 2066 6c6f 6174   Dict[str, float
+00006be0: 5d2c 206f 7074 696f 6e61 6c0a 0a20 2020  ], optional..   
+00006bf0: 2020 2020 2020 2020 2020 2020 2041 2064               A d
+00006c00: 6963 7469 6f6e 6172 7920 7769 7468 206d  ictionary with m
+00006c10: 6178 696d 756d 2064 6570 7468 206f 6620  aximum depth of 
+00006c20: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00006c30: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
+00006c40: 2020 202a 2061 7667 5f64 6570 7468 203a     * avg_depth :
+00006c50: 2044 6963 745b 7374 722c 2066 6c6f 6174   Dict[str, float
+00006c60: 5d2c 206f 7074 696f 6e61 6c0a 0a20 2020  ], optional..   
+00006c70: 2020 2020 2020 2020 2020 2020 2041 2064               A d
+00006c80: 6963 7469 6f6e 6172 7920 7769 7468 2061  ictionary with a
+00006c90: 7665 7261 6765 2064 6570 7468 206f 6620  verage depth of 
+00006ca0: 6561 6368 2064 6574 6563 7465 6420 6361  each detected ca
+00006cb0: 7669 7479 2e0a 0a20 2020 2020 2020 2020  vity...         
+00006cc0: 2020 202a 2061 7667 5f68 7964 726f 7061     * avg_hydropa
+00006cd0: 7468 7920 3a20 4469 6374 5b73 7472 2c20  thy : Dict[str, 
+00006ce0: 666c 6f61 745d 2c20 6f70 7469 6f6e 616c  float], optional
+00006cf0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006d00: 2020 4120 6469 6374 696f 6e61 7279 2077    A dictionary w
+00006d10: 6974 6820 6176 6572 6167 6520 6879 6472  ith average hydr
+00006d20: 6f70 6174 6879 2066 6f72 2065 6163 6820  opathy for each 
+00006d30: 6465 7465 6374 6564 2063 6176 6974 7920  detected cavity 
+00006d40: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00006d50: 2020 2020 7468 6520 7261 6e67 6520 6f66      the range of
+00006d60: 2074 6865 2068 7964 726f 7068 6f62 6963   the hydrophobic
+00006d70: 6974 7920 7363 616c 6520 286d 696e 2c20  ity scale (min, 
+00006d80: 6d61 7829 2e0a 0a20 2020 2020 2020 2020  max)...         
+00006d90: 2020 202a 2072 6573 6964 7565 733a 2044     * residues: D
+00006da0: 6963 745b 7374 722c 204c 6973 745b 4c69  ict[str, List[Li
+00006db0: 7374 5b73 7472 5d5d 5d0a 0a20 2020 2020  st[str]]]..     
+00006dc0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
+00006dd0: 7469 6f6e 6172 7920 7769 7468 2061 206c  tionary with a l
+00006de0: 6973 7420 6f66 2069 6e74 6572 6661 6365  ist of interface
+00006df0: 2072 6573 6964 7565 7320 666f 7220 6561   residues for ea
+00006e00: 6368 2064 6574 6563 7465 640a 2020 2020  ch detected.    
+00006e10: 2020 2020 2020 2020 2020 2020 6361 7669              cavi
+00006e20: 7479 2e0a 0a20 2020 2020 2020 2020 2020  ty...           
+00006e30: 202a 2066 7265 7175 656e 6369 6573 203a   * frequencies :
+00006e40: 2044 6963 745b 7374 722c 2044 6963 745b   Dict[str, Dict[
+00006e50: 7374 722c 2044 6963 745b 7374 722c 2069  str, Dict[str, i
+00006e60: 6e74 5d5d 5d2c 206f 7074 696f 6e61 6c0a  nt]]], optional.
+00006e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e80: 2041 2064 6963 7469 6f6e 6172 7920 7769   A dictionary wi
+00006e90: 7468 2066 7265 7175 656e 6369 6573 206f  th frequencies o
+00006ea0: 6620 7265 7369 6475 6573 2061 6e64 2063  f residues and c
+00006eb0: 6c61 7373 2066 6f72 0a20 2020 2020 2020  lass for.       
+00006ec0: 2020 2020 2020 2020 2072 6573 6964 7565           residue
+00006ed0: 7320 6f66 2065 6163 6820 6465 7465 6374  s of each detect
+00006ee0: 6564 2063 6176 6974 792e 0a0a 2020 2020  ed cavity...    
+00006ef0: 2020 2020 2020 2020 2a20 5f76 6572 7469          * _verti
+00006f00: 6365 7320 3a20 6e75 6d70 792e 6e64 6172  ces : numpy.ndar
+00006f10: 7261 790a 0a20 2020 2020 2020 2020 2020  ray..           
+00006f20: 2020 2020 2041 206e 756d 7079 2e6e 6461       A numpy.nda
+00006f30: 7272 6179 206f 7220 6120 6c69 7374 2077  rray or a list w
+00006f40: 6974 6820 7879 7a20 7665 7274 6963 6573  ith xyz vertices
+00006f50: 2063 6f6f 7264 696e 6174 6573 2028 6f72   coordinates (or
+00006f60: 6967 696e 2c0a 2020 2020 2020 2020 2020  igin,.          
+00006f70: 2020 2020 2020 582d 6178 6973 2c20 592d        X-axis, Y-
+00006f80: 6178 6973 2c20 5a2d 6178 6973 292e 0a0a  axis, Z-axis)...
+00006f90: 2020 2020 2020 2020 2020 2020 2a20 5f73              * _s
+00006fa0: 7465 7020 3a20 666c 6f61 740a 0a20 2020  tep : float..   
+00006fb0: 2020 2020 2020 2020 2020 2020 2047 7269               Gri
+00006fc0: 6420 7370 6163 696e 6720 2841 292e 0a0a  d spacing (A)...
+00006fd0: 2020 2020 2020 2020 2020 2020 2a20 5f69              * _i
+00006fe0: 6e70 7574 203a 2055 6e69 6f6e 5b73 7472  nput : Union[str
+00006ff0: 2c20 7061 7468 6c69 622e 5061 7468 5d2c  , pathlib.Path],
+00007000: 206f 7074 696f 6e61 6c0a 0a20 2020 2020   optional..     
+00007010: 2020 2020 2020 2020 2020 2041 2070 6174             A pat
+00007020: 6820 746f 2069 6e70 7574 2050 4442 206f  h to input PDB o
+00007030: 7220 5859 5a20 6669 6c65 2e0a 0a20 2020  r XYZ file...   
+00007040: 2020 2020 2020 2020 202a 205f 6c69 6761           * _liga
+00007050: 6e64 203a 2055 6e69 6f6e 5b73 7472 2c20  nd : Union[str, 
+00007060: 7061 7468 6c69 622e 5061 7468 5d2c 206f  pathlib.Path], o
+00007070: 7074 696f 6e61 6c0a 0a20 2020 2020 2020  ptional..       
+00007080: 2020 2020 2020 2020 2041 2070 6174 6820           A path 
+00007090: 746f 206c 6967 616e 6420 5044 4220 6f72  to ligand PDB or
+000070a0: 2058 595a 2066 696c 652e 0a0a 2020 2020   XYZ file...    
+000070b0: 5261 6973 6573 0a20 2020 202d 2d2d 2d2d  Raises.    -----
+000070c0: 2d0a 2020 2020 5479 7065 4572 726f 720a  -.    TypeError.
+000070d0: 2020 2020 2020 2020 6069 6e70 7574 6020          `input` 
+000070e0: 6d75 7374 2068 6176 6520 2e70 6462 206f  must have .pdb o
+000070f0: 7220 2e78 797a 2065 7874 656e 7369 6f6e  r .xyz extension
+00007100: 2e0a 2020 2020 5479 7065 4572 726f 720a  ..    TypeError.
+00007110: 2020 2020 2020 2020 606c 6967 616e 6460          `ligand`
+00007120: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
+00007130: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
+00007140: 6e2e 0a0a 2020 2020 4e6f 7465 0a20 2020  n...    Note.   
+00007150: 202d 2d2d 2d0a 2020 2020 5468 6520 6361   ----.    The ca
+00007160: 7669 7479 206e 6f6d 656e 636c 6174 7572  vity nomenclatur
+00007170: 6520 6973 2062 6173 6564 206f 6e20 7468  e is based on th
+00007180: 6520 696e 7465 6765 7220 6c61 6265 6c2e  e integer label.
+00007190: 2054 6865 2063 6176 6974 7920 6d61 726b   The cavity mark
+000071a0: 6564 0a20 2020 2077 6974 6820 322c 2074  ed.    with 2, t
+000071b0: 6865 2066 6972 7374 2069 6e74 6567 6572  he first integer
+000071c0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+000071d0: 6f20 6120 6361 7669 7479 2c20 6973 204b  o a cavity, is K
+000071e0: 4141 2c20 7468 6520 6361 7669 7479 0a20  AA, the cavity. 
+000071f0: 2020 206d 6172 6b65 6420 7769 7468 2033     marked with 3
+00007200: 2069 7320 4b41 422c 2074 6865 2063 6176   is KAB, the cav
+00007210: 6974 7920 6d61 726b 6564 2077 6974 6820  ity marked with 
+00007220: 3420 6973 204b 4143 2061 6e64 2073 6f20  4 is KAC and so 
+00007230: 6f6e 2e0a 0a20 2020 204e 6f74 650a 2020  on...    Note.  
+00007240: 2020 2d2d 2d2d 0a20 2020 2054 6865 2063    ----.    The c
+00007250: 6c61 7373 6573 206f 6620 7265 7369 6475  lasses of residu
+00007260: 6573 2061 7265 3a0a 0a20 2020 202a 2041  es are:..    * A
+00007270: 6c69 7068 6174 6963 2061 706f 6c61 7220  liphatic apolar 
+00007280: 2852 3129 3a20 416c 616e 696e 652c 2047  (R1): Alanine, G
+00007290: 6c79 6369 6e65 2c20 4973 6f6c 6575 6369  lycine, Isoleuci
+000072a0: 6e65 2c20 4c65 7563 696e 652c 204d 6574  ne, Leucine, Met
+000072b0: 6869 6f6e 696e 652c 2056 616c 696e 652e  hionine, Valine.
+000072c0: 0a0a 2020 2020 2a20 4172 6f6d 6174 6963  ..    * Aromatic
+000072d0: 2028 5232 293a 2050 6865 6e79 6c61 6c61   (R2): Phenylala
+000072e0: 6e69 6e65 2c20 5472 7970 746f 7068 616e  nine, Tryptophan
+000072f0: 2c20 5479 726f 7369 6e65 2e0a 0a20 2020  , Tyrosine...   
+00007300: 202a 2050 6f6c 6172 2055 6e63 6861 7267   * Polar Uncharg
+00007310: 6564 2028 5233 293a 2041 7370 6172 6167  ed (R3): Asparag
+00007320: 696e 652c 2043 7973 7465 696e 652c 2047  ine, Cysteine, G
+00007330: 6c75 7461 6d69 6e65 2c20 5072 6f6c 696e  lutamine, Prolin
+00007340: 652c 2053 6572 696e 652c 2054 6872 656f  e, Serine, Threo
+00007350: 6e69 6e65 2e0a 0a20 2020 202a 204e 6567  nine...    * Neg
+00007360: 6174 6976 656c 7920 6368 6172 6765 6420  atively charged 
+00007370: 2852 3429 3a20 4173 7061 7274 6174 652c  (R4): Aspartate,
+00007380: 2047 6c75 7461 6d61 7465 2e0a 0a20 2020   Glutamate...   
+00007390: 202a 2050 6f73 6974 6976 656c 7920 6368   * Positively ch
+000073a0: 6172 6765 6420 2852 3529 3a20 4172 6769  arged (R5): Argi
+000073b0: 6e69 6e65 2c20 4869 7374 6964 696e 652c  nine, Histidine,
+000073c0: 204c 7973 696e 652e 0a0a 2020 2020 2a20   Lysine...    * 
+000073d0: 4e6f 6e2d 7374 616e 6461 7264 2028 5258  Non-standard (RX
+000073e0: 293a 204e 6f6e 2d73 7461 6e64 6172 6420  ): Non-standard 
+000073f0: 7265 7369 6475 6573 2e0a 0a20 2020 2053  residues...    S
+00007400: 6565 2041 6c73 6f0a 2020 2020 2d2d 2d2d  ee Also.    ----
+00007410: 2d2d 2d2d 0a20 2020 2070 794b 5646 696e  ----.    pyKVFin
+00007420: 6465 7252 6573 756c 7473 0a0a 2020 2020  derResults..    
+00007430: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
+00007440: 2d2d 2d0a 2020 2020 5468 6520 2a2a 7374  ---.    The **st
+00007450: 616e 6461 7264 2077 6f72 6b66 6c6f 772a  andard workflow*
+00007460: 2a20 666f 7220 6361 7669 7479 2064 6574  * for cavity det
+00007470: 6563 7469 6f6e 2077 6974 6820 7370 6174  ection with spat
+00007480: 6961 6c20 2873 7572 6661 6365 2070 6f69  ial (surface poi
+00007490: 6e74 732c 2076 6f6c 756d 652c 2061 7265  nts, volume, are
+000074a0: 6129 2061 6e64 2063 6f6e 7374 6974 7574  a) and constitut
+000074b0: 696f 6e61 6c20 2869 6e74 6572 6661 6365  ional (interface
+000074c0: 2072 6573 6964 7565 7320 616e 6420 7468   residues and th
+000074d0: 6569 7220 6672 6571 7565 6e63 6965 7329  eir frequencies)
+000074e0: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
+000074f0: 6e20 2063 616e 2062 6520 7275 6e20 6174  n  can be run at
+00007500: 206f 6e63 6520 7769 7468 206f 6e65 2063   once with one c
+00007510: 6f6d 6d61 6e64 3a0a 0a20 2020 203e 3e3e  ommand:..    >>>
+00007520: 2069 6d70 6f72 7420 6f73 0a20 2020 203e   import os.    >
+00007530: 3e3e 2069 6d70 6f72 7420 7079 4b56 4669  >> import pyKVFi
+00007540: 6e64 6572 0a20 2020 203e 3e3e 2070 6462  nder.    >>> pdb
+00007550: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00007560: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+00007570: 7079 4b56 4669 6e64 6572 2e5f 5f66 696c  pyKVFinder.__fil
+00007580: 655f 5f29 2c20 2764 6174 6127 2c20 2774  e__), 'data', 't
+00007590: 6573 7473 272c 2027 3146 4d4f 2e70 6462  ests', '1FMO.pdb
+000075a0: 2729 0a20 2020 203e 3e3e 2072 6573 756c  ').    >>> resul
+000075b0: 7473 203d 2070 794b 5646 696e 6465 722e  ts = pyKVFinder.
+000075c0: 7275 6e5f 776f 726b 666c 6f77 2870 6462  run_workflow(pdb
+000075d0: 290a 2020 2020 3e3e 3e20 7265 7375 6c74  ).    >>> result
+000075e0: 730a 2020 2020 3c70 794b 5646 696e 6465  s.    <pyKVFinde
+000075f0: 7252 6573 756c 7473 206f 626a 6563 743e  rResults object>
+00007600: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
+00007610: 2e63 6176 6974 6965 730a 2020 2020 6172  .cavities.    ar
+00007620: 7261 7928 5b5b 5b2d 312c 202d 312c 202d  ray([[[-1, -1, -
+00007630: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00007640: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+00007650: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+00007660: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+00007670: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00007680: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00007690: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+000076a0: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+000076b0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+000076c0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+000076d0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+000076e0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+000076f0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+00007700: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+00007710: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+00007720: 2d31 2c20 2d31 2c20 2d31 5d5d 2c0a 2020  -1, -1, -1]],.  
+00007730: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+00007740: 2020 2020 2020 2020 205b 5b2d 312c 202d           [[-1, -
+00007750: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00007760: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+00007770: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+00007780: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+00007790: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+000077a0: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+000077b0: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+000077c0: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+000077d0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+000077e0: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+000077f0: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+00007800: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+00007810: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+00007820: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+00007830: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+00007840: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d5d  .., -1, -1, -1]]
+00007850: 5d2c 2064 7479 7065 3d69 6e74 3332 290a  ], dtype=int32).
+00007860: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
+00007870: 7375 7266 6163 650a 2020 2020 6172 7261  surface.    arra
+00007880: 7928 5b5b 5b2d 312c 202d 312c 202d 312c  y([[[-1, -1, -1,
+00007890: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+000078a0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+000078b0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+000078c0: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+000078d0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+000078e0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+000078f0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+00007900: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
+00007910: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+00007920: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00007930: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+00007940: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+00007950: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+00007960: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00007970: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00007980: 2c20 2d31 2c20 2d31 5d5d 2c0a 2020 2020  , -1, -1]],.    
+00007990: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+000079a0: 2020 2020 2020 205b 5b2d 312c 202d 312c         [[-1, -1,
+000079b0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+000079c0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+000079d0: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+000079e0: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+000079f0: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+00007a00: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+00007a10: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+00007a20: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+00007a30: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+00007a40: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00007a50: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+00007a60: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+00007a70: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+00007a80: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00007a90: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00007aa0: 2c20 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c  , -1, -1, -1]]],
+00007ab0: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
+00007ac0: 2020 3e3e 3e20 7265 7375 6c74 732e 6e63    >>> results.nc
+00007ad0: 6176 0a20 2020 203e 3e3e 2031 380a 2020  av.    >>> 18.  
+00007ae0: 2020 3e3e 3e20 7265 7375 6c74 732e 766f    >>> results.vo
+00007af0: 6c75 6d65 0a20 2020 207b 274b 4141 273a  lume.    {'KAA':
+00007b00: 2031 3337 2e31 362c 2027 4b41 4227 3a20   137.16, 'KAB': 
+00007b10: 3437 2e35 322c 2027 4b41 4327 3a20 3636  47.52, 'KAC': 66
+00007b20: 2e39 362c 2027 4b41 4427 3a20 382e 3231  .96, 'KAD': 8.21
+00007b30: 2c20 274b 4145 273a 2034 332e 3633 2c20  , 'KAE': 43.63, 
+00007b40: 274b 4146 273a 2031 322e 3533 2c20 274b  'KAF': 12.53, 'K
+00007b50: 4147 273a 2036 2e32 362c 2027 4b41 4827  AG': 6.26, 'KAH'
+00007b60: 3a20 3532 302e 3133 2c20 274b 4149 273a  : 520.13, 'KAI':
+00007b70: 2031 322e 3331 2c20 274b 414a 273a 2032   12.31, 'KAJ': 2
+00007b80: 362e 3537 2c20 274b 414b 273a 2031 322e  6.57, 'KAK': 12.
+00007b90: 3331 2c20 274b 414c 273a 2033 332e 3931  31, 'KAL': 33.91
+00007ba0: 2c20 274b 414d 273a 2032 332e 3131 2c20  , 'KAM': 23.11, 
+00007bb0: 274b 414e 273a 2031 3032 2e38 322c 2027  'KAN': 102.82, '
+00007bc0: 4b41 4f27 3a20 362e 3035 2c20 274b 4150  KAO': 6.05, 'KAP
+00007bd0: 273a 2031 352e 3535 2c20 274b 4151 273a  ': 15.55, 'KAQ':
+00007be0: 2037 2e39 392c 2027 4b41 5227 3a20 372e   7.99, 'KAR': 7.
+00007bf0: 3738 7d0a 2020 2020 3e3e 3e20 7265 7375  78}.    >>> resu
+00007c00: 6c74 732e 6172 6561 0a20 2020 207b 274b  lts.area.    {'K
+00007c10: 4141 273a 2031 3236 2e34 312c 2027 4b41  AA': 126.41, 'KA
+00007c20: 4227 3a20 3632 2e33 372c 2027 4b41 4327  B': 62.37, 'KAC'
+00007c30: 3a20 3734 2e35 372c 2027 4b41 4427 3a20  : 74.57, 'KAD': 
+00007c40: 3139 2e30 362c 2027 4b41 4527 3a20 3537  19.06, 'KAE': 57
+00007c50: 2e30 382c 2027 4b41 4627 3a20 3232 2e37  .08, 'KAF': 22.7
+00007c60: 372c 2027 4b41 4727 3a20 3135 2e33 382c  7, 'KAG': 15.38,
+00007c70: 2027 4b41 4827 3a20 3439 362e 3937 2c20   'KAH': 496.97, 
+00007c80: 274b 4149 273a 2033 302e 3538 2c20 274b  'KAI': 30.58, 'K
+00007c90: 414a 273a 2034 352e 3634 2c20 274b 414b  AJ': 45.64, 'KAK
+00007ca0: 273a 2033 302e 3538 2c20 274b 414c 273a  ': 30.58, 'KAL':
+00007cb0: 2034 352e 3538 2c20 274b 414d 273a 2034   45.58, 'KAM': 4
+00007cc0: 352e 3235 2c20 274b 414e 273a 2031 3239  5.25, 'KAN': 129
+00007cd0: 2e37 372c 2027 4b41 4f27 3a20 3132 2e32  .77, 'KAO': 12.2
+00007ce0: 382c 2027 4b41 5027 3a20 3235 2e30 342c  8, 'KAP': 25.04,
+00007cf0: 2027 4b41 5127 3a20 3133 2e34 362c 2027   'KAQ': 13.46, '
+00007d00: 4b41 5227 3a20 3136 2e36 7d0a 2020 2020  KAR': 16.6}.    
+00007d10: 3e3e 3e20 7265 7375 6c74 732e 7265 7369  >>> results.resi
+00007d20: 6475 6573 0a20 2020 207b 274b 4141 273a  dues.    {'KAA':
+00007d30: 205b 5b27 3134 272c 2027 4527 2c20 2753   [['14', 'E', 'S
+00007d40: 4552 275d 2c20 5b27 3135 272c 2027 4527  ER'], ['15', 'E'
+00007d50: 2c20 2756 414c 275d 2c20 5b27 3138 272c  , 'VAL'], ['18',
+00007d60: 2027 4527 2c20 2750 4845 275d 2c20 5b27   'E', 'PHE'], ['
+00007d70: 3139 272c 2027 4527 2c20 274c 4555 275d  19', 'E', 'LEU']
+00007d80: 2c20 5b27 3130 3027 2c20 2745 272c 2027  , ['100', 'E', '
+00007d90: 5048 4527 5d2c 205b 2731 3532 272c 2027  PHE'], ['152', '
+00007da0: 4527 2c20 274c 4555 275d 2c20 5b27 3135  E', 'LEU'], ['15
+00007db0: 3527 2c20 2745 272c 2027 474c 5527 5d2c  5', 'E', 'GLU'],
+00007dc0: 205b 2731 3536 272c 2027 4527 2c20 2754   ['156', 'E', 'T
+00007dd0: 5952 275d 2c20 5b27 3239 3227 2c20 2745  YR'], ['292', 'E
+00007de0: 272c 2027 4c59 5327 5d2c 205b 2733 3032  ', 'LYS'], ['302
+00007df0: 272c 2027 4527 2c20 2754 5250 275d 2c20  ', 'E', 'TRP'], 
+00007e00: 5b27 3330 3327 2c20 2745 272c 2027 494c  ['303', 'E', 'IL
+00007e10: 4527 5d2c 205b 2733 3036 272c 2027 4527  E'], ['306', 'E'
+00007e20: 2c20 2754 5952 275d 5d2c 2027 4b41 4227  , 'TYR']], 'KAB'
+00007e30: 3a20 5b5b 2731 3827 2c20 2745 272c 2027  : [['18', 'E', '
+00007e40: 5048 4527 5d2c 205b 2732 3227 2c20 2745  PHE'], ['22', 'E
+00007e50: 272c 2027 414c 4127 5d2c 205b 2732 3527  ', 'ALA'], ['25'
+00007e60: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
+00007e70: 2732 3627 2c20 2745 272c 2027 5048 4527  '26', 'E', 'PHE'
+00007e80: 5d2c 205b 2732 3927 2c20 2745 272c 2027  ], ['29', 'E', '
+00007e90: 4c59 5327 5d2c 205b 2739 3727 2c20 2745  LYS'], ['97', 'E
+00007ea0: 272c 2027 414c 4127 5d2c 205b 2739 3827  ', 'ALA'], ['98'
+00007eb0: 2c20 2745 272c 2027 5641 4c27 5d2c 205b  , 'E', 'VAL'], [
+00007ec0: 2739 3927 2c20 2745 272c 2027 4153 4e27  '99', 'E', 'ASN'
+00007ed0: 5d2c 205b 2731 3536 272c 2027 4527 2c20  ], ['156', 'E', 
+00007ee0: 2754 5952 275d 5d2c 2027 4b41 4327 3a20  'TYR']], 'KAC': 
+00007ef0: 5b5b 2731 3431 272c 2027 4527 2c20 2750  [['141', 'E', 'P
+00007f00: 524f 275d 2c20 5b27 3134 3227 2c20 2745  RO'], ['142', 'E
+00007f10: 272c 2027 4849 5327 5d2c 205b 2731 3434  ', 'HIS'], ['144
+00007f20: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
+00007f30: 5b27 3134 3527 2c20 2745 272c 2027 5048  ['145', 'E', 'PH
+00007f40: 4527 5d2c 205b 2731 3438 272c 2027 4527  E'], ['148', 'E'
+00007f50: 2c20 2741 4c41 275d 2c20 5b27 3239 3927  , 'ALA'], ['299'
+00007f60: 2c20 2745 272c 2027 5448 5227 5d2c 205b  , 'E', 'THR'], [
+00007f70: 2733 3030 272c 2027 4527 2c20 2754 4852  '300', 'E', 'THR
+00007f80: 275d 2c20 5b27 3330 3527 2c20 2745 272c  '], ['305', 'E',
+00007f90: 2027 494c 4527 5d2c 205b 2733 3130 272c   'ILE'], ['310',
+00007fa0: 2027 4527 2c20 2756 414c 275d 2c20 5b27   'E', 'VAL'], ['
+00007fb0: 3331 3127 2c20 2745 272c 2027 474c 5527  311', 'E', 'GLU'
+00007fc0: 5d2c 205b 2733 3133 272c 2027 4527 2c20  ], ['313', 'E', 
+00007fd0: 2750 524f 275d 5d2c 2027 4b41 4427 3a20  'PRO']], 'KAD': 
+00007fe0: 5b5b 2731 3232 272c 2027 4527 2c20 2754  [['122', 'E', 'T
+00007ff0: 5952 275d 2c20 5b27 3132 3427 2c20 2745  YR'], ['124', 'E
+00008000: 272c 2027 414c 4127 5d2c 205b 2731 3736  ', 'ALA'], ['176
+00008010: 272c 2027 4527 2c20 2747 4c4e 275d 2c20  ', 'E', 'GLN'], 
+00008020: 5b27 3331 3827 2c20 2745 272c 2027 5048  ['318', 'E', 'PH
+00008030: 4527 5d2c 205b 2733 3230 272c 2027 4527  E'], ['320', 'E'
+00008040: 2c20 2747 4c59 275d 2c20 5b27 3332 3127  , 'GLY'], ['321'
+00008050: 2c20 2745 272c 2027 5052 4f27 5d2c 205b  , 'E', 'PRO'], [
+00008060: 2733 3232 272c 2027 4527 2c20 2747 4c59  '322', 'E', 'GLY
+00008070: 275d 2c20 5b27 3332 3327 2c20 2745 272c  '], ['323', 'E',
+00008080: 2027 4153 5027 5d5d 2c20 274b 4145 273a   'ASP']], 'KAE':
+00008090: 205b 5b27 3935 272c 2027 4527 2c20 274c   [['95', 'E', 'L
+000080a0: 4555 275d 2c20 5b27 3938 272c 2027 4527  EU'], ['98', 'E'
+000080b0: 2c20 2756 414c 275d 2c20 5b27 3939 272c  , 'VAL'], ['99',
+000080c0: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
+000080d0: 3130 3027 2c20 2745 272c 2027 5048 4527  100', 'E', 'PHE'
+000080e0: 5d2c 205b 2731 3033 272c 2027 4527 2c20  ], ['103', 'E', 
+000080f0: 274c 4555 275d 2c20 5b27 3130 3427 2c20  'LEU'], ['104', 
+00008100: 2745 272c 2027 5641 4c27 5d2c 205b 2731  'E', 'VAL'], ['1
+00008110: 3035 272c 2027 4527 2c20 274c 5953 275d  05', 'E', 'LYS']
+00008120: 2c20 5b27 3130 3627 2c20 2745 272c 2027  , ['106', 'E', '
+00008130: 4c45 5527 5d5d 2c20 274b 4146 273a 205b  LEU']], 'KAF': [
+00008140: 5b27 3132 3327 2c20 2745 272c 2027 5641  ['123', 'E', 'VA
+00008150: 4c27 5d2c 205b 2731 3234 272c 2027 4527  L'], ['124', 'E'
+00008160: 2c20 2741 4c41 275d 2c20 5b27 3137 3527  , 'ALA'], ['175'
+00008170: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
+00008180: 2731 3736 272c 2027 4527 2c20 2747 4c4e  '176', 'E', 'GLN
+00008190: 275d 2c20 5b27 3138 3127 2c20 2745 272c  '], ['181', 'E',
+000081a0: 2027 474c 4e27 5d5d 2c20 274b 4147 273a   'GLN']], 'KAG':
+000081b0: 205b 5b27 3334 272c 2027 4527 2c20 2753   [['34', 'E', 'S
+000081c0: 4552 275d 2c20 5b27 3337 272c 2027 4527  ER'], ['37', 'E'
+000081d0: 2c20 2754 4852 275d 2c20 5b27 3936 272c  , 'THR'], ['96',
+000081e0: 2027 4527 2c20 2747 4c4e 275d 2c20 5b27   'E', 'GLN'], ['
+000081f0: 3130 3627 2c20 2745 272c 2027 4c45 5527  106', 'E', 'LEU'
+00008200: 5d2c 205b 2731 3037 272c 2027 4527 2c20  ], ['107', 'E', 
+00008210: 2747 4c55 275d 2c20 5b27 3130 3827 2c20  'GLU'], ['108', 
+00008220: 2745 272c 2027 5048 4527 5d2c 205b 2731  'E', 'PHE'], ['1
+00008230: 3039 272c 2027 4527 2c20 2753 4552 275d  09', 'E', 'SER']
+00008240: 5d2c 2027 4b41 4827 3a20 5b5b 2734 3927  ], 'KAH': [['49'
+00008250: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
+00008260: 2735 3027 2c20 2745 272c 2027 474c 5927  '50', 'E', 'GLY'
+00008270: 5d2c 205b 2735 3127 2c20 2745 272c 2027  ], ['51', 'E', '
+00008280: 5448 5227 5d2c 205b 2735 3227 2c20 2745  THR'], ['52', 'E
+00008290: 272c 2027 474c 5927 5d2c 205b 2735 3327  ', 'GLY'], ['53'
+000082a0: 2c20 2745 272c 2027 5345 5227 5d2c 205b  , 'E', 'SER'], [
+000082b0: 2735 3427 2c20 2745 272c 2027 5048 4527  '54', 'E', 'PHE'
+000082c0: 5d2c 205b 2735 3527 2c20 2745 272c 2027  ], ['55', 'E', '
+000082d0: 474c 5927 5d2c 205b 2735 3627 2c20 2745  GLY'], ['56', 'E
+000082e0: 272c 2027 4152 4727 5d2c 205b 2735 3727  ', 'ARG'], ['57'
+000082f0: 2c20 2745 272c 2027 5641 4c27 5d2c 205b  , 'E', 'VAL'], [
+00008300: 2737 3027 2c20 2745 272c 2027 414c 4127  '70', 'E', 'ALA'
+00008310: 5d2c 205b 2737 3227 2c20 2745 272c 2027  ], ['72', 'E', '
+00008320: 4c59 5327 5d2c 205b 2737 3427 2c20 2745  LYS'], ['74', 'E
+00008330: 272c 2027 4c45 5527 5d2c 205b 2738 3427  ', 'LEU'], ['84'
+00008340: 2c20 2745 272c 2027 474c 4e27 5d2c 205b  , 'E', 'GLN'], [
+00008350: 2738 3727 2c20 2745 272c 2027 4849 5327  '87', 'E', 'HIS'
+00008360: 5d2c 205b 2738 3827 2c20 2745 272c 2027  ], ['88', 'E', '
+00008370: 5448 5227 5d2c 205b 2739 3127 2c20 2745  THR'], ['91', 'E
+00008380: 272c 2027 474c 5527 5d2c 205b 2731 3034  ', 'GLU'], ['104
+00008390: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
+000083a0: 5b27 3132 3027 2c20 2745 272c 2027 4d45  ['120', 'E', 'ME
+000083b0: 5427 5d2c 205b 2731 3231 272c 2027 4527  T'], ['121', 'E'
+000083c0: 2c20 2747 4c55 275d 2c20 5b27 3132 3227  , 'GLU'], ['122'
+000083d0: 2c20 2745 272c 2027 5459 5227 5d2c 205b  , 'E', 'TYR'], [
+000083e0: 2731 3233 272c 2027 4527 2c20 2756 414c  '123', 'E', 'VAL
+000083f0: 275d 2c20 5b27 3132 3727 2c20 2745 272c  '], ['127', 'E',
+00008400: 2027 474c 5527 5d2c 205b 2731 3636 272c   'GLU'], ['166',
+00008410: 2027 4527 2c20 2741 5350 275d 2c20 5b27   'E', 'ASP'], ['
+00008420: 3136 3827 2c20 2745 272c 2027 4c59 5327  168', 'E', 'LYS'
+00008430: 5d2c 205b 2731 3730 272c 2027 4527 2c20  ], ['170', 'E', 
+00008440: 2747 4c55 275d 2c20 5b27 3137 3127 2c20  'GLU'], ['171', 
+00008450: 2745 272c 2027 4153 4e27 5d2c 205b 2731  'E', 'ASN'], ['1
+00008460: 3733 272c 2027 4527 2c20 274c 4555 275d  73', 'E', 'LEU']
+00008470: 2c20 5b27 3138 3327 2c20 2745 272c 2027  , ['183', 'E', '
+00008480: 5448 5227 5d2c 205b 2731 3834 272c 2027  THR'], ['184', '
+00008490: 4527 2c20 2741 5350 275d 2c20 5b27 3138  E', 'ASP'], ['18
+000084a0: 3627 2c20 2745 272c 2027 474c 5927 5d2c  6', 'E', 'GLY'],
+000084b0: 205b 2731 3837 272c 2027 4527 2c20 2750   ['187', 'E', 'P
+000084c0: 4845 275d 2c20 5b27 3230 3127 2c20 2745  HE'], ['201', 'E
+000084d0: 272c 2027 5448 5227 5d2c 205b 2733 3237  ', 'THR'], ['327
+000084e0: 272c 2027 4527 2c20 2750 4845 275d 5d2c  ', 'E', 'PHE']],
+000084f0: 2027 4b41 4927 3a20 5b5b 2731 3331 272c   'KAI': [['131',
+00008500: 2027 4527 2c20 2748 4953 275d 2c20 5b27   'E', 'HIS'], ['
+00008510: 3133 3827 2c20 2745 272c 2027 5048 4527  138', 'E', 'PHE'
+00008520: 5d2c 205b 2731 3432 272c 2027 4527 2c20  ], ['142', 'E', 
+00008530: 2748 4953 275d 2c20 5b27 3134 3627 2c20  'HIS'], ['146', 
+00008540: 2745 272c 2027 5459 5227 5d2c 205b 2731  'E', 'TYR'], ['1
+00008550: 3734 272c 2027 4527 2c20 2749 4c45 275d  74', 'E', 'ILE']
+00008560: 2c20 5b27 3331 3427 2c20 2745 272c 2027  , ['314', 'E', '
+00008570: 5048 4527 5d5d 2c20 274b 414a 273a 205b  PHE']], 'KAJ': [
+00008580: 5b27 3333 272c 2027 4527 2c20 2750 524f  ['33', 'E', 'PRO
+00008590: 275d 2c20 5b27 3839 272c 2027 4527 2c20  '], ['89', 'E', 
+000085a0: 274c 4555 275d 2c20 5b27 3932 272c 2027  'LEU'], ['92', '
+000085b0: 4527 2c20 274c 5953 275d 2c20 5b27 3933  E', 'LYS'], ['93
+000085c0: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
+000085d0: 5b27 3936 272c 2027 4527 2c20 2747 4c4e  ['96', 'E', 'GLN
+000085e0: 275d 2c20 5b27 3334 3927 2c20 2745 272c  '], ['349', 'E',
+000085f0: 2027 474c 5527 5d2c 205b 2733 3530 272c   'GLU'], ['350',
+00008600: 2027 4527 2c20 2750 4845 275d 5d2c 2027   'E', 'PHE']], '
+00008610: 4b41 4b27 3a20 5b5b 2731 3537 272c 2027  KAK': [['157', '
+00008620: 4527 2c20 274c 4555 275d 2c20 5b27 3136  E', 'LEU'], ['16
+00008630: 3227 2c20 2745 272c 2027 4c45 5527 5d2c  2', 'E', 'LEU'],
+00008640: 205b 2731 3633 272c 2027 4527 2c20 2749   ['163', 'E', 'I
+00008650: 4c45 275d 2c20 5b27 3136 3427 2c20 2745  LE'], ['164', 'E
+00008660: 272c 2027 5459 5227 5d2c 205b 2731 3835  ', 'TYR'], ['185
+00008670: 272c 2027 4527 2c20 2750 4845 275d 2c20  ', 'E', 'PHE'], 
+00008680: 5b27 3138 3827 2c20 2745 272c 2027 414c  ['188', 'E', 'AL
+00008690: 4127 5d5d 2c20 274b 414c 273a 205b 5b27  A']], 'KAL': [['
+000086a0: 3439 272c 2027 4527 2c20 274c 4555 275d  49', 'E', 'LEU']
+000086b0: 2c20 5b27 3132 3727 2c20 2745 272c 2027  , ['127', 'E', '
+000086c0: 474c 5527 5d2c 205b 2731 3239 272c 2027  GLU'], ['129', '
+000086d0: 4527 2c20 2750 4845 275d 2c20 5b27 3133  E', 'PHE'], ['13
+000086e0: 3027 2c20 2745 272c 2027 5345 5227 5d2c  0', 'E', 'SER'],
+000086f0: 205b 2733 3236 272c 2027 4527 2c20 2741   ['326', 'E', 'A
+00008700: 534e 275d 2c20 5b27 3332 3727 2c20 2745  SN'], ['327', 'E
+00008710: 272c 2027 5048 4527 5d2c 205b 2733 3238  ', 'PHE'], ['328
+00008720: 272c 2027 4527 2c20 2741 5350 275d 2c20  ', 'E', 'ASP'], 
+00008730: 5b27 3333 3027 2c20 2745 272c 2027 5459  ['330', 'E', 'TY
+00008740: 5227 5d5d 2c20 274b 414d 273a 205b 5b27  R']], 'KAM': [['
+00008750: 3531 272c 2027 4527 2c20 2754 4852 275d  51', 'E', 'THR']
+00008760: 2c20 5b27 3535 272c 2027 4527 2c20 2747  , ['55', 'E', 'G
+00008770: 4c59 275d 2c20 5b27 3536 272c 2027 4527  LY'], ['56', 'E'
+00008780: 2c20 2741 5247 275d 2c20 5b27 3733 272c  , 'ARG'], ['73',
+00008790: 2027 4527 2c20 2749 4c45 275d 2c20 5b27   'E', 'ILE'], ['
+000087a0: 3734 272c 2027 4527 2c20 274c 4555 275d  74', 'E', 'LEU']
+000087b0: 2c20 5b27 3735 272c 2027 4527 2c20 2741  , ['75', 'E', 'A
+000087c0: 5350 275d 2c20 5b27 3131 3527 2c20 2745  SP'], ['115', 'E
+000087d0: 272c 2027 4153 4e27 5d2c 205b 2733 3335  ', 'ASN'], ['335
+000087e0: 272c 2027 4527 2c20 2749 4c45 275d 2c20  ', 'E', 'ILE'], 
+000087f0: 5b27 3333 3627 2c20 2745 272c 2027 4152  ['336', 'E', 'AR
+00008800: 4727 5d5d 2c20 274b 414e 273a 205b 5b27  G']], 'KAN': [['
+00008810: 3136 3527 2c20 2745 272c 2027 4152 4727  165', 'E', 'ARG'
+00008820: 5d2c 205b 2731 3636 272c 2027 4527 2c20  ], ['166', 'E', 
+00008830: 2741 5350 275d 2c20 5b27 3136 3727 2c20  'ASP'], ['167', 
+00008840: 2745 272c 2027 4c45 5527 5d2c 205b 2731  'E', 'LEU'], ['1
+00008850: 3939 272c 2027 4527 2c20 2743 5953 275d  99', 'E', 'CYS']
+00008860: 2c20 5b27 3230 3027 2c20 2745 272c 2027  , ['200', 'E', '
+00008870: 474c 5927 5d2c 205b 2732 3031 272c 2027  GLY'], ['201', '
+00008880: 4527 2c20 2754 4852 275d 2c20 5b27 3230  E', 'THR'], ['20
+00008890: 3427 2c20 2745 272c 2027 5459 5227 5d2c  4', 'E', 'TYR'],
+000088a0: 205b 2732 3035 272c 2027 4527 2c20 274c   ['205', 'E', 'L
+000088b0: 4555 275d 2c20 5b27 3230 3627 2c20 2745  EU'], ['206', 'E
+000088c0: 272c 2027 414c 4127 5d2c 205b 2732 3039  ', 'ALA'], ['209
+000088d0: 272c 2027 4527 2c20 2749 4c45 275d 2c20  ', 'E', 'ILE'], 
+000088e0: 5b27 3231 3927 2c20 2745 272c 2027 5641  ['219', 'E', 'VA
+000088f0: 4c27 5d2c 205b 2732 3230 272c 2027 4527  L'], ['220', 'E'
+00008900: 2c20 2741 5350 275d 2c20 5b27 3232 3327  , 'ASP'], ['223'
+00008910: 2c20 2745 272c 2027 414c 4127 5d5d 2c20  , 'E', 'ALA']], 
+00008920: 274b 414f 273a 205b 5b27 3438 272c 2027  'KAO': [['48', '
+00008930: 4527 2c20 2754 4852 275d 2c20 5b27 3531  E', 'THR'], ['51
+00008940: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
+00008950: 5b27 3536 272c 2027 4527 2c20 2741 5247  ['56', 'E', 'ARG
+00008960: 275d 2c20 5b27 3333 3027 2c20 2745 272c  '], ['330', 'E',
+00008970: 2027 5459 5227 5d2c 205b 2733 3331 272c   'TYR'], ['331',
+00008980: 2027 4527 2c20 2747 4c55 275d 5d2c 2027   'E', 'GLU']], '
+00008990: 4b41 5027 3a20 5b5b 2732 3232 272c 2027  KAP': [['222', '
+000089a0: 4527 2c20 2754 5250 275d 2c20 5b27 3233  E', 'TRP'], ['23
+000089b0: 3827 2c20 2745 272c 2027 5048 4527 5d2c  8', 'E', 'PHE'],
+000089c0: 205b 2732 3533 272c 2027 4527 2c20 2747   ['253', 'E', 'G
+000089d0: 4c59 275d 2c20 5b27 3235 3427 2c20 2745  LY'], ['254', 'E
+000089e0: 272c 2027 4c59 5327 5d2c 205b 2732 3535  ', 'LYS'], ['255
+000089f0: 272c 2027 4527 2c20 2756 414c 275d 2c20  ', 'E', 'VAL'], 
+00008a00: 5b27 3237 3327 2c20 2745 272c 2027 4c45  ['273', 'E', 'LE
+00008a10: 5527 5d5d 2c20 274b 4151 273a 205b 5b27  U']], 'KAQ': [['
+00008a20: 3230 3727 2c20 2745 272c 2027 5052 4f27  207', 'E', 'PRO'
+00008a30: 5d2c 205b 2732 3038 272c 2027 4527 2c20  ], ['208', 'E', 
+00008a40: 2747 4c55 275d 2c20 5b27 3231 3127 2c20  'GLU'], ['211', 
+00008a50: 2745 272c 2027 4c45 5527 5d2c 205b 2732  'E', 'LEU'], ['2
+00008a60: 3133 272c 2027 4527 2c20 274c 5953 275d  13', 'E', 'LYS']
+00008a70: 2c20 5b27 3237 3527 2c20 2745 272c 2027  , ['275', 'E', '
+00008a80: 5641 4c27 5d2c 205b 2732 3737 272c 2027  VAL'], ['277', '
+00008a90: 4527 2c20 274c 4555 275d 5d2c 2027 4b41  E', 'LEU']], 'KA
+00008aa0: 5227 3a20 5b5b 2732 3337 272c 2027 4527  R': [['237', 'E'
+00008ab0: 2c20 2750 524f 275d 2c20 5b27 3233 3827  , 'PRO'], ['238'
+00008ac0: 2c20 2745 272c 2027 5048 4527 5d2c 205b  , 'E', 'PHE'], [
+00008ad0: 2732 3439 272c 2027 4527 2c20 274c 5953  '249', 'E', 'LYS
+00008ae0: 275d 2c20 5b27 3235 3427 2c20 2745 272c  '], ['254', 'E',
+00008af0: 2027 4c59 5327 5d2c 205b 2732 3535 272c   'LYS'], ['255',
+00008b00: 2027 4527 2c20 2756 414c 275d 2c20 5b27   'E', 'VAL'], ['
+00008b10: 3235 3627 2c20 2745 272c 2027 4152 4727  256', 'E', 'ARG'
+00008b20: 5d5d 7d0a 2020 2020 3e3e 3e20 7265 7375  ]]}.    >>> resu
+00008b30: 6c74 732e 6672 6571 7565 6e63 6965 730a  lts.frequencies.
+00008b40: 2020 2020 7b27 4b41 4127 3a20 7b27 5245      {'KAA': {'RE
+00008b50: 5349 4455 4553 273a 207b 2747 4c55 273a  SIDUES': {'GLU':
+00008b60: 2031 2c20 2749 4c45 273a 2031 2c20 274c   1, 'ILE': 1, 'L
+00008b70: 4555 273a 2032 2c20 274c 5953 273a 2031  EU': 2, 'LYS': 1
+00008b80: 2c20 2750 4845 273a 2032 2c20 2753 4552  , 'PHE': 2, 'SER
+00008b90: 273a 2031 2c20 2754 5250 273a 2031 2c20  ': 1, 'TRP': 1, 
+00008ba0: 2754 5952 273a 2032 2c20 2756 414c 273a  'TYR': 2, 'VAL':
+00008bb0: 2031 7d2c 2027 434c 4153 5327 3a20 7b27   1}, 'CLASS': {'
+00008bc0: 5231 273a 2034 2c20 2752 3227 3a20 352c  R1': 4, 'R2': 5,
+00008bd0: 2027 5233 273a 2031 2c20 2752 3427 3a20   'R3': 1, 'R4': 
+00008be0: 312c 2027 5235 273a 2031 2c20 2752 5827  1, 'R5': 1, 'RX'
+00008bf0: 3a20 307d 7d2c 2027 4b41 4227 3a20 7b27  : 0}}, 'KAB': {'
+00008c00: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
+00008c10: 273a 2032 2c20 2741 534e 273a 2031 2c20  ': 2, 'ASN': 1, 
+00008c20: 2741 5350 273a 2031 2c20 274c 5953 273a  'ASP': 1, 'LYS':
+00008c30: 2031 2c20 2750 4845 273a 2032 2c20 2754   1, 'PHE': 2, 'T
+00008c40: 5952 273a 2031 2c20 2756 414c 273a 2031  YR': 1, 'VAL': 1
+00008c50: 7d2c 2027 434c 4153 5327 3a20 7b27 5231  }, 'CLASS': {'R1
+00008c60: 273a 2033 2c20 2752 3227 3a20 332c 2027  ': 3, 'R2': 3, '
+00008c70: 5233 273a 2031 2c20 2752 3427 3a20 312c  R3': 1, 'R4': 1,
+00008c80: 2027 5235 273a 2031 2c20 2752 5827 3a20   'R5': 1, 'RX': 
+00008c90: 307d 7d2c 2027 4b41 4327 3a20 7b27 5245  0}}, 'KAC': {'RE
+00008ca0: 5349 4455 4553 273a 207b 2741 4c41 273a  SIDUES': {'ALA':
+00008cb0: 2031 2c20 2741 5247 273a 2031 2c20 2747   1, 'ARG': 1, 'G
+00008cc0: 4c55 273a 2031 2c20 2748 4953 273a 2031  LU': 1, 'HIS': 1
+00008cd0: 2c20 2749 4c45 273a 2031 2c20 2750 4845  , 'ILE': 1, 'PHE
+00008ce0: 273a 2031 2c20 2750 524f 273a 2032 2c20  ': 1, 'PRO': 2, 
+00008cf0: 2754 4852 273a 2032 2c20 2756 414c 273a  'THR': 2, 'VAL':
+00008d00: 2031 7d2c 2027 434c 4153 5327 3a20 7b27   1}, 'CLASS': {'
+00008d10: 5231 273a 2035 2c20 2752 3227 3a20 312c  R1': 5, 'R2': 1,
+00008d20: 2027 5233 273a 2032 2c20 2752 3427 3a20   'R3': 2, 'R4': 
+00008d30: 312c 2027 5235 273a 2032 2c20 2752 5827  1, 'R5': 2, 'RX'
+00008d40: 3a20 307d 7d2c 2027 4b41 4427 3a20 7b27  : 0}}, 'KAD': {'
+00008d50: 5245 5349 4455 4553 273a 207b 2741 4c41  RESIDUES': {'ALA
+00008d60: 273a 2031 2c20 2741 5350 273a 2031 2c20  ': 1, 'ASP': 1, 
+00008d70: 2747 4c4e 273a 2031 2c20 2747 4c59 273a  'GLN': 1, 'GLY':
+00008d80: 2032 2c20 2750 4845 273a 2031 2c20 2750   2, 'PHE': 1, 'P
+00008d90: 524f 273a 2031 2c20 2754 5952 273a 2031  RO': 1, 'TYR': 1
+00008da0: 7d2c 2027 434c 4153 5327 3a20 7b27 5231  }, 'CLASS': {'R1
+00008db0: 273a 2034 2c20 2752 3227 3a20 322c 2027  ': 4, 'R2': 2, '
+00008dc0: 5233 273a 2031 2c20 2752 3427 3a20 312c  R3': 1, 'R4': 1,
+00008dd0: 2027 5235 273a 2030 2c20 2752 5827 3a20   'R5': 0, 'RX': 
+00008de0: 307d 7d2c 2027 4b41 4527 3a20 7b27 5245  0}}, 'KAE': {'RE
+00008df0: 5349 4455 4553 273a 207b 2741 534e 273a  SIDUES': {'ASN':
+00008e00: 2031 2c20 274c 4555 273a 2033 2c20 274c   1, 'LEU': 3, 'L
+00008e10: 5953 273a 2031 2c20 2750 4845 273a 2031  YS': 1, 'PHE': 1
+00008e20: 2c20 2756 414c 273a 2032 7d2c 2027 434c  , 'VAL': 2}, 'CL
+00008e30: 4153 5327 3a20 7b27 5231 273a 2035 2c20  ASS': {'R1': 5, 
+00008e40: 2752 3227 3a20 312c 2027 5233 273a 2031  'R2': 1, 'R3': 1
+00008e50: 2c20 2752 3427 3a20 302c 2027 5235 273a  , 'R4': 0, 'R5':
+00008e60: 2031 2c20 2752 5827 3a20 307d 7d2c 2027   1, 'RX': 0}}, '
+00008e70: 4b41 4627 3a20 7b27 5245 5349 4455 4553  KAF': {'RESIDUES
+00008e80: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
+00008e90: 5350 273a 2031 2c20 2747 4c4e 273a 2032  SP': 1, 'GLN': 2
+00008ea0: 2c20 2756 414c 273a 2031 7d2c 2027 434c  , 'VAL': 1}, 'CL
+00008eb0: 4153 5327 3a20 7b27 5231 273a 2032 2c20  ASS': {'R1': 2, 
+00008ec0: 2752 3227 3a20 302c 2027 5233 273a 2032  'R2': 0, 'R3': 2
+00008ed0: 2c20 2752 3427 3a20 312c 2027 5235 273a  , 'R4': 1, 'R5':
+00008ee0: 2030 2c20 2752 5827 3a20 307d 7d2c 2027   0, 'RX': 0}}, '
+00008ef0: 4b41 4727 3a20 7b27 5245 5349 4455 4553  KAG': {'RESIDUES
+00008f00: 273a 207b 2747 4c4e 273a 2031 2c20 2747  ': {'GLN': 1, 'G
+00008f10: 4c55 273a 2031 2c20 274c 4555 273a 2031  LU': 1, 'LEU': 1
+00008f20: 2c20 2750 4845 273a 2031 2c20 2753 4552  , 'PHE': 1, 'SER
+00008f30: 273a 2032 2c20 2754 4852 273a 2031 7d2c  ': 2, 'THR': 1},
+00008f40: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
+00008f50: 2031 2c20 2752 3227 3a20 312c 2027 5233   1, 'R2': 1, 'R3
+00008f60: 273a 2034 2c20 2752 3427 3a20 312c 2027  ': 4, 'R4': 1, '
+00008f70: 5235 273a 2030 2c20 2752 5827 3a20 307d  R5': 0, 'RX': 0}
+00008f80: 7d2c 2027 4b41 4827 3a20 7b27 5245 5349  }, 'KAH': {'RESI
+00008f90: 4455 4553 273a 207b 2741 4c41 273a 2031  DUES': {'ALA': 1
+00008fa0: 2c20 2741 5247 273a 2031 2c20 2741 534e  , 'ARG': 1, 'ASN
+00008fb0: 273a 2031 2c20 2741 5350 273a 2032 2c20  ': 1, 'ASP': 2, 
+00008fc0: 2747 4c4e 273a 2031 2c20 2747 4c55 273a  'GLN': 1, 'GLU':
+00008fd0: 2034 2c20 2747 4c59 273a 2034 2c20 2748   4, 'GLY': 4, 'H
+00008fe0: 4953 273a 2031 2c20 274c 4555 273a 2033  IS': 1, 'LEU': 3
+00008ff0: 2c20 274c 5953 273a 2032 2c20 274d 4554  , 'LYS': 2, 'MET
+00009000: 273a 2031 2c20 2750 4845 273a 2033 2c20  ': 1, 'PHE': 3, 
+00009010: 2753 4552 273a 2031 2c20 2754 4852 273a  'SER': 1, 'THR':
+00009020: 2034 2c20 2754 5952 273a 2031 2c20 2756   4, 'TYR': 1, 'V
+00009030: 414c 273a 2033 7d2c 2027 434c 4153 5327  AL': 3}, 'CLASS'
+00009040: 3a20 7b27 5231 273a 2031 312c 2027 5232  : {'R1': 11, 'R2
+00009050: 273a 2034 2c20 2752 3327 3a20 382c 2027  ': 4, 'R3': 8, '
+00009060: 5234 273a 2036 2c20 2752 3527 3a20 342c  R4': 6, 'R5': 4,
+00009070: 2027 5258 273a 2030 7d7d 2c20 274b 4149   'RX': 0}}, 'KAI
+00009080: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
+00009090: 7b27 4849 5327 3a20 322c 2027 494c 4527  {'HIS': 2, 'ILE'
+000090a0: 3a20 312c 2027 5048 4527 3a20 322c 2027  : 1, 'PHE': 2, '
+000090b0: 5459 5227 3a20 317d 2c20 2743 4c41 5353  TYR': 1}, 'CLASS
+000090c0: 273a 207b 2752 3127 3a20 312c 2027 5232  ': {'R1': 1, 'R2
+000090d0: 273a 2033 2c20 2752 3327 3a20 302c 2027  ': 3, 'R3': 0, '
+000090e0: 5234 273a 2030 2c20 2752 3527 3a20 322c  R4': 0, 'R5': 2,
+000090f0: 2027 5258 273a 2030 7d7d 2c20 274b 414a   'RX': 0}}, 'KAJ
+00009100: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
+00009110: 7b27 4152 4727 3a20 312c 2027 474c 4e27  {'ARG': 1, 'GLN'
+00009120: 3a20 312c 2027 474c 5527 3a20 312c 2027  : 1, 'GLU': 1, '
+00009130: 4c45 5527 3a20 312c 2027 4c59 5327 3a20  LEU': 1, 'LYS': 
+00009140: 312c 2027 5048 4527 3a20 312c 2027 5052  1, 'PHE': 1, 'PR
+00009150: 4f27 3a20 317d 2c20 2743 4c41 5353 273a  O': 1}, 'CLASS':
+00009160: 207b 2752 3127 3a20 322c 2027 5232 273a   {'R1': 2, 'R2':
+00009170: 2031 2c20 2752 3327 3a20 312c 2027 5234   1, 'R3': 1, 'R4
+00009180: 273a 2031 2c20 2752 3527 3a20 322c 2027  ': 1, 'R5': 2, '
+00009190: 5258 273a 2030 7d7d 2c20 274b 414b 273a  RX': 0}}, 'KAK':
+000091a0: 207b 2752 4553 4944 5545 5327 3a20 7b27   {'RESIDUES': {'
+000091b0: 414c 4127 3a20 312c 2027 494c 4527 3a20  ALA': 1, 'ILE': 
+000091c0: 312c 2027 4c45 5527 3a20 322c 2027 5048  1, 'LEU': 2, 'PH
+000091d0: 4527 3a20 312c 2027 5459 5227 3a20 317d  E': 1, 'TYR': 1}
+000091e0: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
+000091f0: 3a20 342c 2027 5232 273a 2032 2c20 2752  : 4, 'R2': 2, 'R
+00009200: 3327 3a20 302c 2027 5234 273a 2030 2c20  3': 0, 'R4': 0, 
+00009210: 2752 3527 3a20 302c 2027 5258 273a 2030  'R5': 0, 'RX': 0
+00009220: 7d7d 2c20 274b 414c 273a 207b 2752 4553  }}, 'KAL': {'RES
+00009230: 4944 5545 5327 3a20 7b27 4153 4e27 3a20  IDUES': {'ASN': 
+00009240: 312c 2027 4153 5027 3a20 312c 2027 474c  1, 'ASP': 1, 'GL
+00009250: 5527 3a20 312c 2027 4c45 5527 3a20 312c  U': 1, 'LEU': 1,
+00009260: 2027 5048 4527 3a20 322c 2027 5345 5227   'PHE': 2, 'SER'
+00009270: 3a20 312c 2027 5459 5227 3a20 317d 2c20  : 1, 'TYR': 1}, 
+00009280: 2743 4c41 5353 273a 207b 2752 3127 3a20  'CLASS': {'R1': 
+00009290: 312c 2027 5232 273a 2033 2c20 2752 3327  1, 'R2': 3, 'R3'
+000092a0: 3a20 322c 2027 5234 273a 2032 2c20 2752  : 2, 'R4': 2, 'R
+000092b0: 3527 3a20 302c 2027 5258 273a 2030 7d7d  5': 0, 'RX': 0}}
+000092c0: 2c20 274b 414d 273a 207b 2752 4553 4944  , 'KAM': {'RESID
+000092d0: 5545 5327 3a20 7b27 4152 4727 3a20 322c  UES': {'ARG': 2,
+000092e0: 2027 4153 4e27 3a20 312c 2027 4153 5027   'ASN': 1, 'ASP'
+000092f0: 3a20 312c 2027 474c 5927 3a20 312c 2027  : 1, 'GLY': 1, '
+00009300: 494c 4527 3a20 322c 2027 4c45 5527 3a20  ILE': 2, 'LEU': 
+00009310: 312c 2027 5448 5227 3a20 317d 2c20 2743  1, 'THR': 1}, 'C
+00009320: 4c41 5353 273a 207b 2752 3127 3a20 342c  LASS': {'R1': 4,
+00009330: 2027 5232 273a 2030 2c20 2752 3327 3a20   'R2': 0, 'R3': 
+00009340: 322c 2027 5234 273a 2031 2c20 2752 3527  2, 'R4': 1, 'R5'
+00009350: 3a20 322c 2027 5258 273a 2030 7d7d 2c20  : 2, 'RX': 0}}, 
+00009360: 274b 414e 273a 207b 2752 4553 4944 5545  'KAN': {'RESIDUE
+00009370: 5327 3a20 7b27 414c 4127 3a20 322c 2027  S': {'ALA': 2, '
+00009380: 4152 4727 3a20 312c 2027 4153 5027 3a20  ARG': 1, 'ASP': 
+00009390: 322c 2027 4359 5327 3a20 312c 2027 474c  2, 'CYS': 1, 'GL
+000093a0: 5927 3a20 312c 2027 494c 4527 3a20 312c  Y': 1, 'ILE': 1,
+000093b0: 2027 4c45 5527 3a20 322c 2027 5448 5227   'LEU': 2, 'THR'
+000093c0: 3a20 312c 2027 5459 5227 3a20 312c 2027  : 1, 'TYR': 1, '
+000093d0: 5641 4c27 3a20 317d 2c20 2743 4c41 5353  VAL': 1}, 'CLASS
+000093e0: 273a 207b 2752 3127 3a20 372c 2027 5232  ': {'R1': 7, 'R2
+000093f0: 273a 2031 2c20 2752 3327 3a20 322c 2027  ': 1, 'R3': 2, '
+00009400: 5234 273a 2032 2c20 2752 3527 3a20 312c  R4': 2, 'R5': 1,
+00009410: 2027 5258 273a 2030 7d7d 2c20 274b 414f   'RX': 0}}, 'KAO
+00009420: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
+00009430: 7b27 4152 4727 3a20 312c 2027 474c 5527  {'ARG': 1, 'GLU'
+00009440: 3a20 312c 2027 5448 5227 3a20 322c 2027  : 1, 'THR': 2, '
+00009450: 5459 5227 3a20 317d 2c20 2743 4c41 5353  TYR': 1}, 'CLASS
+00009460: 273a 207b 2752 3127 3a20 302c 2027 5232  ': {'R1': 0, 'R2
+00009470: 273a 2031 2c20 2752 3327 3a20 322c 2027  ': 1, 'R3': 2, '
+00009480: 5234 273a 2031 2c20 2752 3527 3a20 312c  R4': 1, 'R5': 1,
+00009490: 2027 5258 273a 2030 7d7d 2c20 274b 4150   'RX': 0}}, 'KAP
+000094a0: 273a 207b 2752 4553 4944 5545 5327 3a20  ': {'RESIDUES': 
+000094b0: 7b27 474c 5927 3a20 312c 2027 4c45 5527  {'GLY': 1, 'LEU'
+000094c0: 3a20 312c 2027 4c59 5327 3a20 312c 2027  : 1, 'LYS': 1, '
+000094d0: 5048 4527 3a20 312c 2027 5452 5027 3a20  PHE': 1, 'TRP': 
+000094e0: 312c 2027 5641 4c27 3a20 317d 2c20 2743  1, 'VAL': 1}, 'C
+000094f0: 4c41 5353 273a 207b 2752 3127 3a20 332c  LASS': {'R1': 3,
+00009500: 2027 5232 273a 2032 2c20 2752 3327 3a20   'R2': 2, 'R3': 
+00009510: 302c 2027 5234 273a 2030 2c20 2752 3527  0, 'R4': 0, 'R5'
+00009520: 3a20 312c 2027 5258 273a 2030 7d7d 2c20  : 1, 'RX': 0}}, 
+00009530: 274b 4151 273a 207b 2752 4553 4944 5545  'KAQ': {'RESIDUE
+00009540: 5327 3a20 7b27 474c 5527 3a20 312c 2027  S': {'GLU': 1, '
+00009550: 4c45 5527 3a20 322c 2027 4c59 5327 3a20  LEU': 2, 'LYS': 
+00009560: 312c 2027 5052 4f27 3a20 312c 2027 5641  1, 'PRO': 1, 'VA
+00009570: 4c27 3a20 317d 2c20 2743 4c41 5353 273a  L': 1}, 'CLASS':
+00009580: 207b 2752 3127 3a20 342c 2027 5232 273a   {'R1': 4, 'R2':
+00009590: 2030 2c20 2752 3327 3a20 302c 2027 5234   0, 'R3': 0, 'R4
+000095a0: 273a 2031 2c20 2752 3527 3a20 312c 2027  ': 1, 'R5': 1, '
+000095b0: 5258 273a 2030 7d7d 2c20 274b 4152 273a  RX': 0}}, 'KAR':
+000095c0: 207b 2752 4553 4944 5545 5327 3a20 7b27   {'RESIDUES': {'
+000095d0: 4152 4727 3a20 312c 2027 4c59 5327 3a20  ARG': 1, 'LYS': 
+000095e0: 322c 2027 5048 4527 3a20 312c 2027 5052  2, 'PHE': 1, 'PR
+000095f0: 4f27 3a20 312c 2027 5641 4c27 3a20 317d  O': 1, 'VAL': 1}
+00009600: 2c20 2743 4c41 5353 273a 207b 2752 3127  , 'CLASS': {'R1'
+00009610: 3a20 322c 2027 5232 273a 2031 2c20 2752  : 2, 'R2': 1, 'R
+00009620: 3327 3a20 302c 2027 5234 273a 2030 2c20  3': 0, 'R4': 0, 
+00009630: 2752 3527 3a20 332c 2027 5258 273a 2030  'R5': 3, 'RX': 0
+00009640: 7d7d 7d0a 0a20 2020 2048 6f77 6576 6572  }}}..    However
+00009650: 2c20 7573 6572 7320 6d61 7920 6f70 7420  , users may opt 
+00009660: 746f 2070 6572 666f 726d 2063 6176 6974  to perform cavit
+00009670: 7920 6465 7465 6374 696f 6e20 696e 2061  y detection in a
+00009680: 2073 6567 6d65 6e74 6564 2073 7061 6365   segmented space
+00009690: 2074 6872 6f75 6768 206c 6967 616e 6420   through ligand 
+000096a0: 6164 6a75 7374 6d65 6e74 2061 6e64 2f6f  adjustment and/o
+000096b0: 7220 626f 7820 6164 6a75 7374 6d65 6e74  r box adjustment
+000096c0: 206d 6f64 6573 2e0a 0a20 2020 2054 6865   modes...    The
+000096d0: 2063 6176 6974 7920 6465 7465 6374 696f   cavity detectio
+000096e0: 6e20 6361 6e20 6265 206c 696d 6974 6564  n can be limited
+000096f0: 2061 726f 756e 6420 7468 6520 7461 7267   around the targ
+00009700: 6574 206c 6967 616e 6428 7329 2c20 7768  et ligand(s), wh
+00009710: 6963 6820 7769 6c6c 2062 6520 7061 7373  ich will be pass
+00009720: 6564 2074 6f20 7079 4b56 4669 6e64 6572  ed to pyKVFinder
+00009730: 2074 6872 6f75 6768 2061 202a 2e70 6462   through a *.pdb
+00009740: 2a20 6f72 2061 202a 2e78 797a 2a20 6669  * or a *.xyz* fi
+00009750: 6c65 732e 2054 6875 732c 2074 6865 2064  les. Thus, the d
+00009760: 6574 6563 7465 6420 6361 7669 7469 6573  etected cavities
+00009770: 2061 7265 206c 696d 6974 6564 2077 6974   are limited wit
+00009780: 6869 6e20 6120 7261 6469 7573 2028 6060  hin a radius (``
+00009790: 6c69 6761 6e64 5f63 7574 6f66 6660 6029  ligand_cutoff``)
+000097a0: 206f 6620 7468 6520 7461 7267 6574 206c   of the target l
+000097b0: 6967 616e 6428 7329 2e0a 0a20 2020 203e  igand(s)...    >
+000097c0: 3e3e 206c 6967 616e 6420 3d20 6f73 2e70  >> ligand = os.p
+000097d0: 6174 682e 6a6f 696e 286f 732e 7061 7468  ath.join(os.path
+000097e0: 2e64 6972 6e61 6d65 2870 794b 5646 696e  .dirname(pyKVFin
+000097f0: 6465 722e 5f5f 6669 6c65 5f5f 292c 2027  der.__file__), '
+00009800: 6461 7461 272c 2027 7465 7374 7327 2c20  data', 'tests', 
+00009810: 2741 444e 2e70 6462 2729 0a20 2020 203e  'ADN.pdb').    >
+00009820: 3e3e 2072 6573 756c 7473 203d 2070 794b  >> results = pyK
+00009830: 5646 696e 6465 722e 7275 6e5f 776f 726b  VFinder.run_work
+00009840: 666c 6f77 2870 6462 2c20 6c69 6761 6e64  flow(pdb, ligand
+00009850: 290a 2020 2020 3e3e 3e20 7265 7375 6c74  ).    >>> result
+00009860: 730a 2020 2020 3c70 794b 5646 696e 6465  s.    <pyKVFinde
+00009870: 7252 6573 756c 7473 206f 626a 6563 743e  rResults object>
+00009880: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
+00009890: 2e63 6176 6974 6965 730a 2020 2020 6172  .cavities.    ar
+000098a0: 7261 7928 5b5b 5b2d 312c 202d 312c 202d  ray([[[-1, -1, -
+000098b0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+000098c0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+000098d0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+000098e0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+000098f0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00009900: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00009910: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+00009920: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+00009930: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+00009940: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+00009950: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+00009960: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+00009970: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+00009980: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+00009990: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+000099a0: 2d31 2c20 2d31 2c20 2d31 5d5d 2c0a 2020  -1, -1, -1]],.  
+000099b0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+000099c0: 2020 2020 2020 2020 205b 5b2d 312c 202d           [[-1, -
+000099d0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+000099e0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+000099f0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+00009a00: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+00009a10: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00009a20: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00009a30: 2c20 2d31 2c20 2d31 2c20 2d31 5d2c 0a20  , -1, -1, -1],. 
+00009a40: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+00009a50: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00009a60: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00009a70: 2c20 2d31 2c20 2d31 5d2c 0a20 2020 2020  , -1, -1],.     
+00009a80: 2020 2020 2020 205b 2d31 2c20 2d31 2c20         [-1, -1, 
+00009a90: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+00009aa0: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+00009ab0: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+00009ac0: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d5d  .., -1, -1, -1]]
+00009ad0: 5d2c 2064 7479 7065 3d69 6e74 3332 290a  ], dtype=int32).
+00009ae0: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
+00009af0: 7375 7266 6163 650a 2020 2020 6172 7261  surface.    arra
+00009b00: 7928 5b5b 5b2d 312c 202d 312c 202d 312c  y([[[-1, -1, -1,
+00009b10: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+00009b20: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+00009b30: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+00009b40: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+00009b50: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+00009b60: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00009b70: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+00009b80: 2020 2020 202e 2e2e 2c0a 2020 2020 2020       ...,.      
+00009b90: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+00009ba0: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+00009bb0: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+00009bc0: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+00009bd0: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+00009be0: 2020 2020 2020 2020 2020 2020 5b2d 312c              [-1,
+00009bf0: 202d 312c 202d 312c 202e 2e2e 2c20 2d31   -1, -1, ..., -1
+00009c00: 2c20 2d31 2c20 2d31 5d5d 2c0a 2020 2020  , -1, -1]],.    
+00009c10: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+00009c20: 2020 2020 2020 205b 5b2d 312c 202d 312c         [[-1, -1,
+00009c30: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+00009c40: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+00009c50: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+00009c60: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+00009c70: 2c0a 2020 2020 2020 2020 2020 2020 5b2d  ,.            [-
+00009c80: 312c 202d 312c 202d 312c 202e 2e2e 2c20  1, -1, -1, ..., 
+00009c90: 2d31 2c20 2d31 2c20 2d31 5d2c 0a20 2020  -1, -1, -1],.   
+00009ca0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+00009cb0: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+00009cc0: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+00009cd0: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+00009ce0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+00009cf0: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+00009d00: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00009d10: 5b2d 312c 202d 312c 202d 312c 202e 2e2e  [-1, -1, -1, ...
+00009d20: 2c20 2d31 2c20 2d31 2c20 2d31 5d5d 5d2c  , -1, -1, -1]]],
+00009d30: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
+00009d40: 2020 3e3e 3e20 7265 7375 6c74 732e 6e63    >>> results.nc
+00009d50: 6176 0a20 2020 203e 3e3e 2031 380a 2020  av.    >>> 18.  
+00009d60: 2020 3e3e 3e20 7265 7375 6c74 732e 766f    >>> results.vo
+00009d70: 6c75 6d65 0a20 2020 207b 274b 4141 273a  lume.    {'KAA':
+00009d80: 2033 3635 2e30 342c 2027 4b41 4227 3a20   365.04, 'KAB': 
+00009d90: 3136 2e38 357d 0a20 2020 203e 3e3e 2072  16.85}.    >>> r
+00009da0: 6573 756c 7473 2e61 7265 610a 2020 2020  esults.area.    
+00009db0: 7b27 4b41 4127 3a20 3332 382e 3739 2c20  {'KAA': 328.79, 
+00009dc0: 274b 4142 273a 2032 332e 3135 7d0a 2020  'KAB': 23.15}.  
+00009dd0: 2020 3e3e 3e20 7265 7375 6c74 732e 7265    >>> results.re
+00009de0: 7369 6475 6573 0a20 2020 207b 274b 4141  sidues.    {'KAA
+00009df0: 273a 205b 5b27 3439 272c 2027 4527 2c20  ': [['49', 'E', 
+00009e00: 274c 4555 275d 2c20 5b27 3530 272c 2027  'LEU'], ['50', '
+00009e10: 4527 2c20 2747 4c59 275d 2c20 5b27 3531  E', 'GLY'], ['51
+00009e20: 272c 2027 4527 2c20 2754 4852 275d 2c20  ', 'E', 'THR'], 
+00009e30: 5b27 3532 272c 2027 4527 2c20 2747 4c59  ['52', 'E', 'GLY
+00009e40: 275d 2c20 5b27 3533 272c 2027 4527 2c20  '], ['53', 'E', 
+00009e50: 2753 4552 275d 2c20 5b27 3535 272c 2027  'SER'], ['55', '
+00009e60: 4527 2c20 2747 4c59 275d 2c20 5b27 3536  E', 'GLY'], ['56
+00009e70: 272c 2027 4527 2c20 2741 5247 275d 2c20  ', 'E', 'ARG'], 
+00009e80: 5b27 3537 272c 2027 4527 2c20 2756 414c  ['57', 'E', 'VAL
+00009e90: 275d 2c20 5b27 3730 272c 2027 4527 2c20  '], ['70', 'E', 
+00009ea0: 2741 4c41 275d 2c20 5b27 3732 272c 2027  'ALA'], ['72', '
+00009eb0: 4527 2c20 274c 5953 275d 2c20 5b27 3130  E', 'LYS'], ['10
+00009ec0: 3427 2c20 2745 272c 2027 5641 4c27 5d2c  4', 'E', 'VAL'],
+00009ed0: 205b 2731 3230 272c 2027 4527 2c20 274d   ['120', 'E', 'M
+00009ee0: 4554 275d 2c20 5b27 3132 3127 2c20 2745  ET'], ['121', 'E
+00009ef0: 272c 2027 474c 5527 5d2c 205b 2731 3232  ', 'GLU'], ['122
+00009f00: 272c 2027 4527 2c20 2754 5952 275d 2c20  ', 'E', 'TYR'], 
+00009f10: 5b27 3132 3327 2c20 2745 272c 2027 5641  ['123', 'E', 'VA
+00009f20: 4c27 5d2c 205b 2731 3237 272c 2027 4527  L'], ['127', 'E'
+00009f30: 2c20 2747 4c55 275d 2c20 5b27 3136 3627  , 'GLU'], ['166'
+00009f40: 2c20 2745 272c 2027 4153 5027 5d2c 205b  , 'E', 'ASP'], [
+00009f50: 2731 3638 272c 2027 4527 2c20 274c 5953  '168', 'E', 'LYS
+00009f60: 275d 2c20 5b27 3137 3027 2c20 2745 272c  '], ['170', 'E',
+00009f70: 2027 474c 5527 5d2c 205b 2731 3731 272c   'GLU'], ['171',
+00009f80: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
+00009f90: 3137 3327 2c20 2745 272c 2027 4c45 5527  173', 'E', 'LEU'
+00009fa0: 5d2c 205b 2731 3833 272c 2027 4527 2c20  ], ['183', 'E', 
+00009fb0: 2754 4852 275d 2c20 5b27 3138 3427 2c20  'THR'], ['184', 
+00009fc0: 2745 272c 2027 4153 5027 5d2c 205b 2733  'E', 'ASP'], ['3
+00009fd0: 3237 272c 2027 4527 2c20 2750 4845 275d  27', 'E', 'PHE']
+00009fe0: 5d2c 2027 4b41 4227 3a20 5b5b 2734 3927  ], 'KAB': [['49'
+00009ff0: 2c20 2745 272c 2027 4c45 5527 5d2c 205b  , 'E', 'LEU'], [
+0000a000: 2731 3237 272c 2027 4527 2c20 2747 4c55  '127', 'E', 'GLU
+0000a010: 275d 2c20 5b27 3133 3027 2c20 2745 272c  '], ['130', 'E',
+0000a020: 2027 5345 5227 5d2c 205b 2733 3236 272c   'SER'], ['326',
+0000a030: 2027 4527 2c20 2741 534e 275d 2c20 5b27   'E', 'ASN'], ['
+0000a040: 3332 3727 2c20 2745 272c 2027 5048 4527  327', 'E', 'PHE'
+0000a050: 5d2c 205b 2733 3238 272c 2027 4527 2c20  ], ['328', 'E', 
+0000a060: 2741 5350 275d 2c20 5b27 3333 3027 2c20  'ASP'], ['330', 
+0000a070: 2745 272c 2027 5459 5227 5d5d 7d0a 2020  'E', 'TYR']]}.  
+0000a080: 2020 3e3e 3e20 7265 7375 6c74 732e 6672    >>> results.fr
+0000a090: 6571 7565 6e63 6965 730a 2020 2020 7b27  equencies.    {'
+0000a0a0: 4b41 4127 3a20 7b27 5245 5349 4455 4553  KAA': {'RESIDUES
+0000a0b0: 273a 207b 2741 4c41 273a 2031 2c20 2741  ': {'ALA': 1, 'A
+0000a0c0: 5247 273a 2031 2c20 2741 534e 273a 2031  RG': 1, 'ASN': 1
+0000a0d0: 2c20 2741 5350 273a 2032 2c20 2747 4c55  , 'ASP': 2, 'GLU
+0000a0e0: 273a 2033 2c20 2747 4c59 273a 2033 2c20  ': 3, 'GLY': 3, 
+0000a0f0: 274c 4555 273a 2032 2c20 274c 5953 273a  'LEU': 2, 'LYS':
+0000a100: 2032 2c20 274d 4554 273a 2031 2c20 2750   2, 'MET': 1, 'P
+0000a110: 4845 273a 2031 2c20 2753 4552 273a 2031  HE': 1, 'SER': 1
+0000a120: 2c20 2754 4852 273a 2032 2c20 2754 5952  , 'THR': 2, 'TYR
+0000a130: 273a 2031 2c20 2756 414c 273a 2033 7d2c  ': 1, 'VAL': 3},
+0000a140: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
+0000a150: 2039 2c20 2752 3227 3a20 322c 2027 5233   9, 'R2': 2, 'R3
+0000a160: 273a 2035 2c20 2752 3427 3a20 352c 2027  ': 5, 'R4': 5, '
+0000a170: 5235 273a 2033 2c20 2752 5827 3a20 307d  R5': 3, 'RX': 0}
+0000a180: 7d2c 2027 4b41 4227 3a20 7b27 5245 5349  }, 'KAB': {'RESI
+0000a190: 4455 4553 273a 207b 2741 534e 273a 2031  DUES': {'ASN': 1
+0000a1a0: 2c20 2741 5350 273a 2031 2c20 2747 4c55  , 'ASP': 1, 'GLU
+0000a1b0: 273a 2031 2c20 274c 4555 273a 2031 2c20  ': 1, 'LEU': 1, 
+0000a1c0: 2750 4845 273a 2031 2c20 2753 4552 273a  'PHE': 1, 'SER':
+0000a1d0: 2031 2c20 2754 5952 273a 2031 7d2c 2027   1, 'TYR': 1}, '
+0000a1e0: 434c 4153 5327 3a20 7b27 5231 273a 2031  CLASS': {'R1': 1
+0000a1f0: 2c20 2752 3227 3a20 322c 2027 5233 273a  , 'R2': 2, 'R3':
+0000a200: 2032 2c20 2752 3427 3a20 322c 2027 5235   2, 'R4': 2, 'R5
+0000a210: 273a 2030 2c20 2752 5827 3a20 307d 7d7d  ': 0, 'RX': 0}}}
+0000a220: 0a0a 2020 2020 4675 7274 6865 722c 2077  ..    Further, w
+0000a230: 6520 6361 6e20 616c 736f 2070 6572 666f  e can also perfo
+0000a240: 726d 2063 6176 6974 7920 6465 7465 6374  rm cavity detect
+0000a250: 696f 6e20 6f6e 2061 2063 7573 746f 6d20  ion on a custom 
+0000a260: 3344 2067 7269 642c 2077 6865 7265 2077  3D grid, where w
+0000a270: 6520 6361 6e20 6578 706c 6f72 6520 636c  e can explore cl
+0000a280: 6f73 6564 2072 6567 696f 6e73 2077 6974  osed regions wit
+0000a290: 6820 6120 6375 7374 6f6d 2062 6f78 2c20  h a custom box, 
+0000a2a0: 7768 6963 6820 6361 6e20 6265 2064 6566  which can be def
+0000a2b0: 696e 6564 2062 7920 6120 2a2e 746f 6d6c  ined by a *.toml
+0000a2c0: 2a20 6669 6c65 2028 7365 6520 6042 6f78  * file (see `Box
+0000a2d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+0000a2e0: 696c 6520 7465 6d70 6c61 7465 6029 2e0a  ile template`)..
+0000a2f0: 0a20 2020 203e 3e3e 2066 6e20 3d20 6f73  .    >>> fn = os
+0000a300: 2e70 6174 682e 6a6f 696e 286f 732e 7061  .path.join(os.pa
+0000a310: 7468 2e64 6972 6e61 6d65 2870 794b 5646  th.dirname(pyKVF
+0000a320: 696e 6465 722e 5f5f 6669 6c65 5f5f 292c  inder.__file__),
+0000a330: 2027 6461 7461 272c 2027 7465 7374 7327   'data', 'tests'
+0000a340: 2c20 2763 7573 746f 6d2d 626f 782e 746f  , 'custom-box.to
+0000a350: 6d6c 2729 0a20 2020 203e 3e3e 2077 6974  ml').    >>> wit
+0000a360: 6820 6f70 656e 2866 6e2c 2027 7227 2920  h open(fn, 'r') 
+0000a370: 6173 2066 3a0a 2020 2020 2e2e 2e20 2020  as f:.    ...   
+0000a380: 2020 7072 696e 7428 662e 7265 6164 2829    print(f.read()
+0000a390: 290a 2020 2020 5b62 6f78 5d0a 2020 2020  ).    [box].    
+0000a3a0: 7031 203d 205b 332e 3131 2c20 372e 3334  p1 = [3.11, 7.34
+0000a3b0: 2c20 312e 3539 5d0a 2020 2020 7032 203d  , 1.59].    p2 =
+0000a3c0: 205b 3131 2e35 312c 2037 2e33 342c 2031   [11.51, 7.34, 1
+0000a3d0: 2e35 395d 0a20 2020 2070 3320 3d20 5b33  .59].    p3 = [3
+0000a3e0: 2e31 312c 2031 302e 3734 2c20 312e 3539  .11, 10.74, 1.59
+0000a3f0: 5d0a 2020 2020 7034 203d 205b 332e 3131  ].    p4 = [3.11
+0000a400: 2c20 372e 3334 2c20 362e 3139 5d0a 2020  , 7.34, 6.19].  
+0000a410: 2020 3e3e 3e20 7265 7375 6c74 7320 3d20    >>> results = 
+0000a420: 7079 4b56 4669 6e64 6572 2e72 756e 5f77  pyKVFinder.run_w
+0000a430: 6f72 6b66 6c6f 7728 7064 622c 2062 6f78  orkflow(pdb, box
+0000a440: 3d66 6e29 0a20 2020 203e 3e3e 2072 6573  =fn).    >>> res
+0000a450: 756c 7473 0a20 2020 203c 7079 4b56 4669  ults.    <pyKVFi
+0000a460: 6e64 6572 5265 7375 6c74 7320 6f62 6a65  nderResults obje
+0000a470: 6374 3e0a 2020 2020 3e3e 3e20 7265 7375  ct>.    >>> resu
+0000a480: 6c74 732e 6361 7669 7469 6573 0a20 2020  lts.cavities.   
+0000a490: 2061 7272 6179 285b 5b5b 2d31 2c20 2d31   array([[[-1, -1
+0000a4a0: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+0000a4b0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+0000a4c0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+0000a4d0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+0000a4e0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0000a4f0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+0000a500: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+0000a510: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
+0000a520: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+0000a530: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+0000a540: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+0000a550: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+0000a560: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+0000a570: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+0000a580: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+0000a590: 2e2c 202d 312c 202d 312c 202d 315d 5d2c  ., -1, -1, -1]],
+0000a5a0: 0a20 2020 2020 2020 2020 2020 2e2e 2e2c  .           ...,
+0000a5b0: 0a20 2020 2020 2020 2020 2020 5b5b 2d31  .           [[-1
+0000a5c0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+0000a5d0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+0000a5e0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+0000a5f0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+0000a600: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+0000a610: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+0000a620: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+0000a630: 2c0a 2020 2020 2020 2020 2020 2020 2e2e  ,.            ..
+0000a640: 2e2c 0a20 2020 2020 2020 2020 2020 205b  .,.            [
+0000a650: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+0000a660: 202d 312c 202d 312c 202d 315d 2c0a 2020   -1, -1, -1],.  
+0000a670: 2020 2020 2020 2020 2020 5b2d 312c 202d            [-1, -
+0000a680: 312c 202d 312c 202e 2e2e 2c20 2d31 2c20  1, -1, ..., -1, 
+0000a690: 2d31 2c20 2d31 5d2c 0a20 2020 2020 2020  -1, -1],.       
+0000a6a0: 2020 2020 205b 2d31 2c20 2d31 2c20 2d31       [-1, -1, -1
+0000a6b0: 2c20 2e2e 2e2c 202d 312c 202d 312c 202d  , ..., -1, -1, -
+0000a6c0: 315d 5d5d 2c20 6474 7970 653d 696e 7433  1]]], dtype=int3
+0000a6d0: 3229 0a20 2020 203e 3e3e 2072 6573 756c  2).    >>> resul
+0000a6e0: 7473 2e73 7572 6661 6365 0a20 2020 2061  ts.surface.    a
+0000a6f0: 7272 6179 285b 5b5b 2d31 2c20 2d31 2c20  rray([[[-1, -1, 
+0000a700: 2d31 2c20 2e2e 2e2c 202d 312c 202d 312c  -1, ..., -1, -1,
+0000a710: 202d 315d 2c0a 2020 2020 2020 2020 2020   -1],.          
+0000a720: 2020 5b2d 312c 202d 312c 202d 312c 202e    [-1, -1, -1, .
+0000a730: 2e2e 2c20 2d31 2c20 2d31 2c20 2d31 5d2c  .., -1, -1, -1],
+0000a740: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+0000a750: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+0000a760: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+0000a770: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
+0000a780: 2020 2020 2020 2020 205b 2d31 2c20 2d31           [-1, -1
+0000a790: 2c20 2d31 2c20 2e2e 2e2c 202d 312c 202d  , -1, ..., -1, -
+0000a7a0: 312c 202d 315d 2c0a 2020 2020 2020 2020  1, -1],.        
+0000a7b0: 2020 2020 5b2d 312c 202d 312c 202d 312c      [-1, -1, -1,
+0000a7c0: 202e 2e2e 2c20 2d31 2c20 2d31 2c20 2d31   ..., -1, -1, -1
+0000a7d0: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0000a7e0: 2d31 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c  -1, -1, -1, ...,
+0000a7f0: 202d 312c 202d 312c 202d 315d 5d2c 0a20   -1, -1, -1]],. 
+0000a800: 2020 2020 2020 2020 2020 2e2e 2e2c 0a20            ...,. 
+0000a810: 2020 2020 2020 2020 2020 5b5b 2d31 2c20            [[-1, 
+0000a820: 2d31 2c20 2d31 2c20 2e2e 2e2c 202d 312c  -1, -1, ..., -1,
+0000a830: 202d 312c 202d 315d 2c0a 2020 2020 2020   -1, -1],.      
+0000a840: 2020 2020 2020 5b2d 312c 202d 312c 202d        [-1, -1, -
+0000a850: 312c 202e 2e2e 2c20 2d31 2c20 2d31 2c20  1, ..., -1, -1, 
+0000a860: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+0000a870: 205b 2d31 2c20 2d31 2c20 2d31 2c20 2e2e   [-1, -1, -1, ..
+0000a880: 2e2c 202d 312c 202d 312c 202d 315d 2c0a  ., -1, -1, -1],.
+0000a890: 2020 2020 2020 2020 2020 2020 2e2e 2e2c              ...,
+0000a8a0: 0a20 2020 2020 2020 2020 2020 205b 2d31  .            [-1
+0000a8b0: 2c20 2d31 2c20 2d31 2c20 2e2e 2e2c 202d  , -1, -1, ..., -
+0000a8c0: 312c 202d 312c 202d 315d 2c0a 2020 2020  1, -1, -1],.    
+0000a8d0: 2020 2020 2020 2020 5b2d 312c 202d 312c          [-1, -1,
+0000a8e0: 202d 312c 202e 2e2e 2c20 2d31 2c20 2d31   -1, ..., -1, -1
+0000a8f0: 2c20 2d31 5d2c 0a20 2020 2020 2020 2020  , -1],.         
+0000a900: 2020 205b 2d31 2c20 2d31 2c20 2d31 2c20     [-1, -1, -1, 
+0000a910: 2e2e 2e2c 202d 312c 202d 312c 202d 315d  ..., -1, -1, -1]
+0000a920: 5d5d 2c20 6474 7970 653d 696e 7433 3229  ]], dtype=int32)
+0000a930: 0a20 2020 203e 3e3e 2072 6573 756c 7473  .    >>> results
+0000a940: 2e6e 6361 760a 2020 2020 3e3e 3e20 310a  .ncav.    >>> 1.
+0000a950: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
+0000a960: 766f 6c75 6d65 0a20 2020 207b 274b 4141  volume.    {'KAA
+0000a970: 273a 2031 3135 2e37 387d 0a20 2020 203e  ': 115.78}.    >
+0000a980: 3e3e 2072 6573 756c 7473 2e61 7265 610a  >> results.area.
+0000a990: 2020 2020 7b27 4b41 4127 3a20 3333 2e39      {'KAA': 33.9
+0000a9a0: 317d 0a20 2020 203e 3e3e 2072 6573 756c  1}.    >>> resul
+0000a9b0: 7473 2e72 6573 6964 7565 730a 2020 2020  ts.residues.    
+0000a9c0: 7b27 4b41 4127 3a20 5b5b 2734 3927 2c20  {'KAA': [['49', 
+0000a9d0: 2745 272c 2027 4c45 5527 5d2c 205b 2735  'E', 'LEU'], ['5
+0000a9e0: 3027 2c20 2745 272c 2027 474c 5927 5d2c  0', 'E', 'GLY'],
+0000a9f0: 205b 2735 3127 2c20 2745 272c 2027 5448   ['51', 'E', 'TH
+0000aa00: 5227 5d2c 205b 2735 3727 2c20 2745 272c  R'], ['57', 'E',
+0000aa10: 2027 5641 4c27 5d2c 205b 2737 3027 2c20   'VAL'], ['70', 
+0000aa20: 2745 272c 2027 414c 4127 5d2c 205b 2731  'E', 'ALA'], ['1
+0000aa30: 3034 272c 2027 4527 2c20 2756 414c 275d  04', 'E', 'VAL']
+0000aa40: 2c20 5b27 3132 3127 2c20 2745 272c 2027  , ['121', 'E', '
+0000aa50: 474c 5527 5d2c 205b 2731 3232 272c 2027  GLU'], ['122', '
+0000aa60: 4527 2c20 2754 5952 275d 2c20 5b27 3132  E', 'TYR'], ['12
+0000aa70: 3327 2c20 2745 272c 2027 5641 4c27 5d2c  3', 'E', 'VAL'],
+0000aa80: 205b 2731 3237 272c 2027 4527 2c20 2747   ['127', 'E', 'G
+0000aa90: 4c55 275d 2c20 5b27 3137 3027 2c20 2745  LU'], ['170', 'E
+0000aaa0: 272c 2027 474c 5527 5d2c 205b 2731 3731  ', 'GLU'], ['171
+0000aab0: 272c 2027 4527 2c20 2741 534e 275d 2c20  ', 'E', 'ASN'], 
+0000aac0: 5b27 3137 3327 2c20 2745 272c 2027 4c45  ['173', 'E', 'LE
+0000aad0: 5527 5d2c 205b 2731 3833 272c 2027 4527  U'], ['183', 'E'
+0000aae0: 2c20 2754 4852 275d 2c20 5b27 3332 3727  , 'THR'], ['327'
+0000aaf0: 2c20 2745 272c 2027 5048 4527 5d5d 7d0a  , 'E', 'PHE']]}.
+0000ab00: 2020 2020 3e3e 3e20 7265 7375 6c74 732e      >>> results.
+0000ab10: 6672 6571 7565 6e63 6965 730a 2020 2020  frequencies.    
+0000ab20: 7b27 4b41 4127 3a20 7b27 5245 5349 4455  {'KAA': {'RESIDU
+0000ab30: 4553 273a 207b 2741 4c41 273a 2031 2c20  ES': {'ALA': 1, 
+0000ab40: 2741 534e 273a 2031 2c20 2747 4c55 273a  'ASN': 1, 'GLU':
+0000ab50: 2033 2c20 2747 4c59 273a 2031 2c20 274c   3, 'GLY': 1, 'L
+0000ab60: 4555 273a 2032 2c20 2750 4845 273a 2031  EU': 2, 'PHE': 1
+0000ab70: 2c20 2754 4852 273a 2032 2c20 2754 5952  , 'THR': 2, 'TYR
+0000ab80: 273a 2031 2c20 2756 414c 273a 2033 7d2c  ': 1, 'VAL': 3},
+0000ab90: 2027 434c 4153 5327 3a20 7b27 5231 273a   'CLASS': {'R1':
+0000aba0: 2037 2c20 2752 3227 3a20 322c 2027 5233   7, 'R2': 2, 'R3
+0000abb0: 273a 2033 2c20 2752 3427 3a20 332c 2027  ': 3, 'R4': 3, '
+0000abc0: 5235 273a 2030 2c20 2752 5827 3a20 307d  R5': 0, 'RX': 0}
+0000abd0: 7d7d 0a0a 2020 2020 486f 7765 7665 722c  }}..    However,
+0000abe0: 2075 7365 7273 206d 6179 206f 7074 2074   users may opt t
+0000abf0: 6f20 7065 7266 6f72 6d20 7468 6520 2a2a  o perform the **
+0000ac00: 6675 6c6c 2077 6f72 6b66 6c6f 772a 2a20  full workflow** 
+0000ac10: 666f 7220 6361 7669 7479 2064 6574 6563  for cavity detec
+0000ac20: 7469 6f6e 2077 6974 6820 7370 6174 6961  tion with spatia
+0000ac30: 6c20 2873 7572 6661 6365 2070 6f69 6e74  l (surface point
+0000ac40: 732c 2076 6f6c 756d 6520 616e 6420 6172  s, volume and ar
+0000ac50: 6561 292c 2063 6f6e 7374 6974 7574 696f  ea), constitutio
+0000ac60: 6e61 6c20 2869 6e74 6572 6661 6365 2072  nal (interface r
+0000ac70: 6573 6964 7565 7320 616e 6420 7468 6569  esidues and thei
+0000ac80: 7220 6672 6571 7565 6e63 6965 7329 2c20  r frequencies), 
+0000ac90: 6879 6472 6f70 6174 6879 2061 6e64 2064  hydropathy and d
+0000aca0: 6570 7468 2063 6861 7261 6374 6572 697a  epth characteriz
+0000acb0: 6174 696f 6e2e 2054 6869 7320 6675 6c6c  ation. This full
+0000acc0: 2077 6f72 6b66 6c6f 7720 6361 6e20 6265   workflow can be
+0000acd0: 2072 756e 2077 6974 6820 6f6e 6520 636f   run with one co
+0000ace0: 6d6d 616e 6420 6279 2073 6574 7469 6e67  mmand by setting
+0000acf0: 2073 6f6d 6520 7061 7261 6d65 7465 7273   some parameters
+0000ad00: 206f 6620 6060 7275 6e5f 776f 726b 666c   of ``run_workfl
+0000ad10: 6f77 6060 2066 756e 6374 696f 6e3a 0a0a  ow`` function:..
+0000ad20: 2020 2020 3e3e 3e20 7265 7375 6c74 7320      >>> results 
+0000ad30: 3d20 7079 4b56 4669 6e64 6572 2e72 756e  = pyKVFinder.run
+0000ad40: 5f77 6f72 6b66 6c6f 7728 7064 622c 2069  _workflow(pdb, i
+0000ad50: 6e63 6c75 6465 5f64 6570 7468 3d54 7275  nclude_depth=Tru
+0000ad60: 652c 2069 6e63 6c75 6465 5f68 7964 726f  e, include_hydro
+0000ad70: 7061 7468 793d 5472 7565 2c20 6879 6472  pathy=True, hydr
+0000ad80: 6f70 686f 6269 6369 7479 5f73 6361 6c65  ophobicity_scale
+0000ad90: 3d27 4569 7365 6e62 6572 6757 6569 7373  ='EisenbergWeiss
+0000ada0: 2729 0a20 2020 203e 3e3e 2072 6573 756c  ').    >>> resul
+0000adb0: 7473 2e64 6570 7468 730a 2020 2020 6172  ts.depths.    ar
+0000adc0: 7261 7928 5b5b 5b30 2e2c 2030 2e2c 2030  ray([[[0., 0., 0
+0000add0: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+0000ade0: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
+0000adf0: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
+0000ae00: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
+0000ae10: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
+0000ae20: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
+0000ae30: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
+0000ae40: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+0000ae50: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+0000ae60: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+0000ae70: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+0000ae80: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
+0000ae90: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
+0000aea0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
+0000aeb0: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
+0000aec0: 302e 2c20 302e 2c20 302e 5d5d 2c0a 2020  0., 0., 0.]],.  
+0000aed0: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+0000aee0: 2020 2020 2020 2020 205b 5b30 2e2c 2030           [[0., 0
+0000aef0: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
+0000af00: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
+0000af10: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
+0000af20: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
+0000af30: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
+0000af40: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
+0000af50: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
+0000af60: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+0000af70: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
+0000af80: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
+0000af90: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
+0000afa0: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
+0000afb0: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
+0000afc0: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
+0000afd0: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
+0000afe0: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d5d  .., 0., 0., 0.]]
+0000aff0: 5d29 0a20 2020 203e 3e3e 2072 6573 756c  ]).    >>> resul
+0000b000: 7473 2e73 6361 6c65 730a 2020 2020 6172  ts.scales.    ar
+0000b010: 7261 7928 5b5b 5b30 2e2c 2030 2e2c 2030  ray([[[0., 0., 0
+0000b020: 2e2c 202e 2e2e 2c20 302e 2c20 302e 2c20  ., ..., 0., 0., 
+0000b030: 302e 5d2c 0a20 2020 2020 2020 2020 2020  0.],.           
+0000b040: 205b 302e 2c20 302e 2c20 302e 2c20 2e2e   [0., 0., 0., ..
+0000b050: 2e2c 2030 2e2c 2030 2e2c 2030 2e5d 2c0a  ., 0., 0., 0.],.
+0000b060: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
+0000b070: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
+0000b080: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
+0000b090: 2020 2020 2020 202e 2e2e 2c0a 2020 2020         ...,.    
+0000b0a0: 2020 2020 2020 2020 5b30 2e2c 2030 2e2c          [0., 0.,
+0000b0b0: 2030 2e2c 202e 2e2e 2c20 302e 2c20 302e   0., ..., 0., 0.
+0000b0c0: 2c20 302e 5d2c 0a20 2020 2020 2020 2020  , 0.],.         
+0000b0d0: 2020 205b 302e 2c20 302e 2c20 302e 2c20     [0., 0., 0., 
+0000b0e0: 2e2e 2e2c 2030 2e2c 2030 2e2c 2030 2e5d  ..., 0., 0., 0.]
+0000b0f0: 2c0a 2020 2020 2020 2020 2020 2020 5b30  ,.            [0
+0000b100: 2e2c 2030 2e2c 2030 2e2c 202e 2e2e 2c20  ., 0., 0., ..., 
+0000b110: 302e 2c20 302e 2c20 302e 5d5d 2c0a 2020  0., 0., 0.]],.  
+0000b120: 2020 2020 2020 2020 202e 2e2e 2c0a 2020           ...,.  
+0000b130: 2020 2020 2020 2020 205b 5b30 2e2c 2030           [[0., 0
+0000b140: 2e2c 2030 2e2c 202e 2e2e 2c20 302e 2c20  ., 0., ..., 0., 
+0000b150: 302e 2c20 302e 5d2c 0a20 2020 2020 2020  0., 0.],.       
+0000b160: 2020 2020 205b 302e 2c20 302e 2c20 302e       [0., 0., 0.
+0000b170: 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c 2030  , ..., 0., 0., 0
+0000b180: 2e5d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
+0000b190: 5b30 2e2c 2030 2e2c 2030 2e2c 202e 2e2e  [0., 0., 0., ...
+0000b1a0: 2c20 302e 2c20 302e 2c20 302e 5d2c 0a20  , 0., 0., 0.],. 
+0000b1b0: 2020 2020 2020 2020 2020 202e 2e2e 2c0a             ...,.
+0000b1c0: 2020 2020 2020 2020 2020 2020 5b30 2e2c              [0.,
+0000b1d0: 2030 2e2c 2030 2e2c 202e 2e2e 2c20 302e   0., 0., ..., 0.
+0000b1e0: 2c20 302e 2c20 302e 5d2c 0a20 2020 2020  , 0., 0.],.     
+0000b1f0: 2020 2020 2020 205b 302e 2c20 302e 2c20         [0., 0., 
+0000b200: 302e 2c20 2e2e 2e2c 2030 2e2c 2030 2e2c  0., ..., 0., 0.,
+0000b210: 2030 2e5d 2c0a 2020 2020 2020 2020 2020   0.],.          
+0000b220: 2020 5b30 2e2c 2030 2e2c 2030 2e2c 202e    [0., 0., 0., .
+0000b230: 2e2e 2c20 302e 2c20 302e 2c20 302e 5d5d  .., 0., 0., 0.]]
+0000b240: 5d29 0a20 2020 203e 3e3e 2072 6573 756c  ]).    >>> resul
+0000b250: 7473 2e61 7667 5f64 6570 7468 0a20 2020  ts.avg_depth.   
+0000b260: 207b 274b 4141 273a 2031 2e33 352c 2027   {'KAA': 1.35, '
+0000b270: 4b41 4227 3a20 302e 3931 2c20 274b 4143  KAB': 0.91, 'KAC
+0000b280: 273a 2030 2e36 382c 2027 4b41 4427 3a20  ': 0.68, 'KAD': 
+0000b290: 302e 3332 2c20 274b 4145 273a 2030 2e39  0.32, 'KAE': 0.9
+0000b2a0: 392c 2027 4b41 4627 3a20 302e 3234 2c20  9, 'KAF': 0.24, 
+0000b2b0: 274b 4147 273a 2030 2e31 2c20 274b 4148  'KAG': 0.1, 'KAH
+0000b2c0: 273a 2033 2e39 312c 2027 4b41 4927 3a20  ': 3.91, 'KAI': 
+0000b2d0: 302e 302c 2027 4b41 4a27 3a20 302e 3936  0.0, 'KAJ': 0.96
+0000b2e0: 2c20 274b 414b 273a 2030 2e30 2c20 274b  , 'KAK': 0.0, 'K
+0000b2f0: 414c 273a 2031 2e30 372c 2027 4b41 4d27  AL': 1.07, 'KAM'
+0000b300: 3a20 302e 3234 2c20 274b 414e 273a 2030  : 0.24, 'KAN': 0
+0000b310: 2e30 2c20 274b 414f 273a 2030 2e32 392c  .0, 'KAO': 0.29,
+0000b320: 2027 4b41 5027 3a20 302e 372c 2027 4b41   'KAP': 0.7, 'KA
+0000b330: 5127 3a20 302e 3232 2c20 274b 4152 273a  Q': 0.22, 'KAR':
+0000b340: 2030 2e31 327d 0a20 2020 203e 3e3e 2072   0.12}.    >>> r
+0000b350: 6573 756c 7473 2e6d 6178 5f64 6570 7468  esults.max_depth
+0000b360: 0a20 2020 207b 274b 4141 273a 2033 2e37  .    {'KAA': 3.7
+0000b370: 392c 2027 4b41 4227 3a20 322e 3638 2c20  9, 'KAB': 2.68, 
+0000b380: 274b 4143 273a 2032 2e36 322c 2027 4b41  'KAC': 2.62, 'KA
+0000b390: 4427 3a20 302e 3835 2c20 274b 4145 273a  D': 0.85, 'KAE':
+0000b3a0: 2033 2e30 2c20 274b 4146 273a 2030 2e38   3.0, 'KAF': 0.8
+0000b3b0: 352c 2027 4b41 4727 3a20 302e 362c 2027  5, 'KAG': 0.6, '
+0000b3c0: 4b41 4827 3a20 3130 2e37 332c 2027 4b41  KAH': 10.73, 'KA
+0000b3d0: 4927 3a20 302e 302c 2027 4b41 4a27 3a20  I': 0.0, 'KAJ': 
+0000b3e0: 322e 3234 2c20 274b 414b 273a 2030 2e30  2.24, 'KAK': 0.0
+0000b3f0: 2c20 274b 414c 273a 2033 2e30 2c20 274b  , 'KAL': 3.0, 'K
+0000b400: 414d 273a 2031 2e32 2c20 274b 414e 273a  AM': 1.2, 'KAN':
+0000b410: 2030 2e30 2c20 274b 414f 273a 2031 2e30   0.0, 'KAO': 1.0
+0000b420: 342c 2027 4b41 5027 3a20 322e 3038 2c20  4, 'KAP': 2.08, 
+0000b430: 274b 4151 273a 2030 2e38 352c 2027 4b41  'KAQ': 0.85, 'KA
+0000b440: 5227 3a20 302e 367d 0a20 2020 203e 3e3e  R': 0.6}.    >>>
+0000b450: 2072 6573 756c 7473 2e61 7667 5f68 7964   results.avg_hyd
+0000b460: 726f 7061 7468 790a 2020 2020 7b27 4b41  ropathy.    {'KA
+0000b470: 4127 3a20 2d30 2e37 332c 2027 4b41 4227  A': -0.73, 'KAB'
+0000b480: 3a20 2d30 2e30 352c 2027 4b41 4327 3a20  : -0.05, 'KAC': 
+0000b490: 2d30 2e30 372c 2027 4b41 4427 3a20 2d30  -0.07, 'KAD': -0
+0000b4a0: 2e36 322c 2027 4b41 4527 3a20 2d30 2e38  .62, 'KAE': -0.8
+0000b4b0: 312c 2027 4b41 4627 3a20 2d30 2e31 342c  1, 'KAF': -0.14,
+0000b4c0: 2027 4b41 4727 3a20 2d30 2e33 332c 2027   'KAG': -0.33, '
+0000b4d0: 4b41 4827 3a20 2d30 2e31 372c 2027 4b41  KAH': -0.17, 'KA
+0000b4e0: 4927 3a20 2d30 2e34 2c20 274b 414a 273a  I': -0.4, 'KAJ':
+0000b4f0: 2030 2e36 322c 2027 4b41 4b27 3a20 2d30   0.62, 'KAK': -0
+0000b500: 2e39 392c 2027 4b41 4c27 3a20 302e 3336  .99, 'KAL': 0.36
+0000b510: 2c20 274b 414d 273a 202d 302e 3333 2c20  , 'KAM': -0.33, 
+0000b520: 274b 414e 273a 2030 2e31 382c 2027 4b41  'KAN': 0.18, 'KA
+0000b530: 4f27 3a20 302e 3838 2c20 274b 4150 273a  O': 0.88, 'KAP':
+0000b540: 202d 302e 3936 2c20 274b 4151 273a 2030   -0.96, 'KAQ': 0
+0000b550: 2e34 382c 2027 4b41 5227 3a20 302e 3234  .48, 'KAR': 0.24
+0000b560: 2c20 2745 6973 656e 6265 7267 5765 6973  , 'EisenbergWeis
+0000b570: 7327 3a20 5b2d 312e 3432 2c20 322e 365d  s': [-1.42, 2.6]
+0000b580: 7d0a 2020 2020 2222 220a 2020 2020 6966  }.    """.    if
+0000b590: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+0000b5a0: 2020 7072 696e 7428 223e 204c 6f61 6469    print("> Loadi
+0000b5b0: 6e67 2061 746f 6d69 6320 6469 6374 696f  ng atomic dictio
+0000b5c0: 6e61 7279 2066 696c 6522 290a 2020 2020  nary file").    
+0000b5d0: 6966 2076 6477 2069 7320 6e6f 7420 4e6f  if vdw is not No
+0000b5e0: 6e65 3a0a 2020 2020 2020 2020 7664 7720  ne:.        vdw 
+0000b5f0: 3d20 7265 6164 5f76 6477 2876 6477 290a  = read_vdw(vdw).
+0000b600: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000b610: 2020 7664 7720 3d20 7265 6164 5f76 6477    vdw = read_vdw
+0000b620: 2856 4457 290a 0a20 2020 2069 6620 7665  (VDW)..    if ve
+0000b630: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+0000b640: 7269 6e74 2822 3e20 5265 6164 696e 6720  rint("> Reading 
+0000b650: 5044 4220 636f 6f72 6469 6e61 7465 7322  PDB coordinates"
+0000b660: 290a 2020 2020 6966 2069 6e70 7574 2e65  ).    if input.e
+0000b670: 6e64 7377 6974 6828 222e 7064 6222 293a  ndswith(".pdb"):
+0000b680: 0a20 2020 2020 2020 2061 746f 6d69 6320  .        atomic 
+0000b690: 3d20 7265 6164 5f70 6462 2869 6e70 7574  = read_pdb(input
+0000b6a0: 2c20 7664 772c 206d 6f64 656c 290a 2020  , vdw, model).  
+0000b6b0: 2020 656c 6966 2069 6e70 7574 2e65 6e64    elif input.end
+0000b6c0: 7377 6974 6828 222e 7879 7a22 293a 0a20  swith(".xyz"):. 
+0000b6d0: 2020 2020 2020 2061 746f 6d69 6320 3d20         atomic = 
+0000b6e0: 7265 6164 5f78 797a 2869 6e70 7574 2c20  read_xyz(input, 
+0000b6f0: 7664 7729 0a20 2020 2065 6c73 653a 0a20  vdw).    else:. 
+0000b700: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000b710: 6545 7272 6f72 2822 6074 6172 6765 7460  eError("`target`
+0000b720: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
+0000b730: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
+0000b740: 6e2e 2229 0a0a 2020 2020 6966 206c 6967  n.")..    if lig
+0000b750: 616e 643a 0a20 2020 2020 2020 2069 6620  and:.        if 
+0000b760: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+0000b770: 2020 2020 2070 7269 6e74 2822 3e20 5265       print("> Re
+0000b780: 6164 696e 6720 6c69 6761 6e64 2063 6f6f  ading ligand coo
+0000b790: 7264 696e 6174 6573 2229 0a20 2020 2020  rdinates").     
+0000b7a0: 2020 2069 6620 6c69 6761 6e64 2e65 6e64     if ligand.end
+0000b7b0: 7377 6974 6828 222e 7064 6222 293a 0a20  swith(".pdb"):. 
+0000b7c0: 2020 2020 2020 2020 2020 206c 6174 6f6d             latom
+0000b7d0: 6963 203d 2072 6561 645f 7064 6228 6c69  ic = read_pdb(li
+0000b7e0: 6761 6e64 2c20 7664 7729 0a20 2020 2020  gand, vdw).     
+0000b7f0: 2020 2065 6c69 6620 6c69 6761 6e64 2e65     elif ligand.e
+0000b800: 6e64 7377 6974 6828 222e 7879 7a22 293a  ndswith(".xyz"):
+0000b810: 0a20 2020 2020 2020 2020 2020 206c 6174  .            lat
+0000b820: 6f6d 6963 203d 2072 6561 645f 7879 7a28  omic = read_xyz(
+0000b830: 6c69 6761 6e64 2c20 7664 7729 0a20 2020  ligand, vdw).   
+0000b840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b850: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000b860: 6545 7272 6f72 2822 606c 6967 616e 6460  eError("`ligand`
+0000b870: 206d 7573 7420 6861 7665 202e 7064 6220   must have .pdb 
+0000b880: 6f72 202e 7879 7a20 6578 7465 6e73 696f  or .xyz extensio
+0000b890: 6e2e 2229 0a20 2020 2065 6c73 653a 0a20  n.").    else:. 
+0000b8a0: 2020 2020 2020 206c 6174 6f6d 6963 203d         latomic =
+0000b8b0: 204e 6f6e 650a 0a20 2020 2069 6620 7665   None..    if ve
+0000b8c0: 7262 6f73 653a 0a20 2020 2020 2020 2070  rbose:.        p
+0000b8d0: 7269 6e74 2822 3e20 4361 6c63 756c 6174  rint("> Calculat
+0000b8e0: 696e 6720 3344 2067 7269 6420 6469 6d65  ing 3D grid dime
+0000b8f0: 6e73 696f 6e73 2229 0a20 2020 2069 6620  nsions").    if 
+0000b900: 626f 783a 0a20 2020 2020 2020 2023 2047  box:.        # G
+0000b910: 6574 2076 6572 7469 6365 7320 6672 6f6d  et vertices from
+0000b920: 2066 696c 650a 2020 2020 2020 2020 7665   file.        ve
+0000b930: 7274 6963 6573 2c20 6174 6f6d 6963 203d  rtices, atomic =
+0000b940: 2067 6574 5f76 6572 7469 6365 735f 6672   get_vertices_fr
+0000b950: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
+0000b960: 2020 2020 2062 6f78 2c20 6174 6f6d 6963       box, atomic
+0000b970: 2c20 7374 6570 2c20 7072 6f62 655f 696e  , step, probe_in
+0000b980: 2c20 7072 6f62 655f 6f75 742c 206e 7468  , probe_out, nth
+0000b990: 7265 6164 730a 2020 2020 2020 2020 290a  reads.        ).
+0000b9a0: 0a20 2020 2020 2020 2023 2053 6574 2066  .        # Set f
+0000b9b0: 6c61 6720 746f 2062 6f6f 6c65 616e 0a20  lag to boolean. 
+0000b9c0: 2020 2020 2020 2062 6f78 203d 2054 7275         box = Tru
+0000b9d0: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
+0000b9e0: 2020 2020 2320 4765 7420 7665 7274 6963      # Get vertic
+0000b9f0: 6573 2066 726f 6d20 696e 7075 740a 2020  es from input.  
+0000ba00: 2020 2020 2020 7665 7274 6963 6573 203d        vertices =
+0000ba10: 2067 6574 5f76 6572 7469 6365 7328 6174   get_vertices(at
+0000ba20: 6f6d 6963 2c20 7072 6f62 655f 6f75 742c  omic, probe_out,
+0000ba30: 2073 7465 7029 0a0a 2020 2020 2020 2020   step)..        
+0000ba40: 2320 5365 7420 666c 6167 2074 6f20 626f  # Set flag to bo
+0000ba50: 6f6c 6561 6e0a 2020 2020 2020 2020 626f  olean.        bo
+0000ba60: 7820 3d20 4661 6c73 650a 0a20 2020 2023  x = False..    #
+0000ba70: 2043 616c 6375 6c61 7465 2064 6973 7461   Calculate dista
+0000ba80: 6e63 6520 6265 7477 6565 6e20 706f 696e  nce between poin
+0000ba90: 7473 0a20 2020 206e 782c 206e 792c 206e  ts.    nx, ny, n
+0000baa0: 7a20 3d20 5f67 6574 5f64 696d 656e 7369  z = _get_dimensi
+0000bab0: 6f6e 7328 7665 7274 6963 6573 2c20 7374  ons(vertices, st
+0000bac0: 6570 290a 2020 2020 6966 2076 6572 626f  ep).    if verbo
+0000bad0: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
+0000bae0: 7428 6622 4469 6d65 6e73 696f 6e73 3a20  t(f"Dimensions: 
+0000baf0: 286e 783a 7b6e 787d 2c20 6e79 3a7b 6e79  (nx:{nx}, ny:{ny
+0000bb00: 7d2c 206e 7a3a 7b6e 7a7d 2922 290a 0a20  }, nz:{nz})").. 
+0000bb10: 2020 2023 2043 616c 6375 6c61 7465 2073     # Calculate s
+0000bb20: 696e 2061 6e64 2063 6f73 206f 6620 616e  in and cos of an
+0000bb30: 676c 6573 2061 2061 6e64 2062 0a20 2020  gles a and b.   
+0000bb40: 2073 696e 636f 7320 3d20 5f67 6574 5f73   sincos = _get_s
+0000bb50: 696e 636f 7328 7665 7274 6963 6573 290a  incos(vertices).
+0000bb60: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0000bb70: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+0000bb80: 7369 6e61 3a20 7b73 696e 636f 735b 305d  sina: {sincos[0]
+0000bb90: 3a2e 3266 7d5c 7473 696e 623a 207b 7369  :.2f}\tsinb: {si
+0000bba0: 6e63 6f73 5b32 5d3a 2e32 667d 2229 0a20  ncos[2]:.2f}"). 
+0000bbb0: 2020 2020 2020 2070 7269 6e74 2866 2263         print(f"c
+0000bbc0: 6f73 613a 207b 7369 6e63 6f73 5b31 5d3a  osa: {sincos[1]:
+0000bbd0: 2e32 667d 5c74 636f 7362 3a20 7b73 696e  .2f}\tcosb: {sin
+0000bbe0: 636f 735b 335d 3a2e 3266 7d22 290a 0a20  cos[3]:.2f}").. 
+0000bbf0: 2020 2023 2043 6176 6974 7920 6465 7465     # Cavity dete
+0000bc00: 6374 696f 6e0a 2020 2020 6e63 6176 2c20  ction.    ncav, 
+0000bc10: 6361 7669 7469 6573 203d 2064 6574 6563  cavities = detec
+0000bc20: 7428 0a20 2020 2020 2020 2061 746f 6d69  t(.        atomi
+0000bc30: 632c 0a20 2020 2020 2020 2076 6572 7469  c,.        verti
+0000bc40: 6365 732c 0a20 2020 2020 2020 2073 7465  ces,.        ste
+0000bc50: 702c 0a20 2020 2020 2020 2070 726f 6265  p,.        probe
+0000bc60: 5f69 6e2c 0a20 2020 2020 2020 2070 726f  _in,.        pro
+0000bc70: 6265 5f6f 7574 2c0a 2020 2020 2020 2020  be_out,.        
+0000bc80: 7265 6d6f 7661 6c5f 6469 7374 616e 6365  removal_distance
+0000bc90: 2c0a 2020 2020 2020 2020 766f 6c75 6d65  ,.        volume
+0000bca0: 5f63 7574 6f66 662c 0a20 2020 2020 2020  _cutoff,.       
+0000bcb0: 206c 6174 6f6d 6963 2c0a 2020 2020 2020   latomic,.      
+0000bcc0: 2020 6c69 6761 6e64 5f63 7574 6f66 662c    ligand_cutoff,
+0000bcd0: 0a20 2020 2020 2020 2062 6f78 2c0a 2020  .        box,.  
+0000bce0: 2020 2020 2020 7375 7266 6163 652c 0a20        surface,. 
+0000bcf0: 2020 2020 2020 206e 7468 7265 6164 732c         nthreads,
+0000bd00: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
+0000bd10: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+0000bd20: 6e63 6176 203e 2030 3a0a 2020 2020 2020  ncav > 0:.      
+0000bd30: 2020 2320 5370 6174 6961 6c20 6368 6172    # Spatial char
+0000bd40: 6163 7465 7269 7a61 7469 6f6e 0a20 2020  acterization.   
+0000bd50: 2020 2020 2073 7572 6661 6365 2c20 766f       surface, vo
+0000bd60: 6c75 6d65 2c20 6172 6561 203d 2073 7061  lume, area = spa
+0000bd70: 7469 616c 2863 6176 6974 6965 732c 2073  tial(cavities, s
+0000bd80: 7465 702c 204e 6f6e 652c 206e 7468 7265  tep, None, nthre
+0000bd90: 6164 732c 2076 6572 626f 7365 290a 0a20  ads, verbose).. 
+0000bda0: 2020 2020 2020 2023 2043 6f6e 7374 6974         # Constit
+0000bdb0: 7574 696f 6e61 6c20 6368 6172 6163 7465  utional characte
+0000bdc0: 7269 7a61 7469 6f6e 0a20 2020 2020 2020  rization.       
+0000bdd0: 2072 6573 6964 7565 7320 3d20 636f 6e73   residues = cons
+0000bde0: 7469 7475 7469 6f6e 616c 280a 2020 2020  titutional(.    
+0000bdf0: 2020 2020 2020 2020 6361 7669 7469 6573          cavities
+0000be00: 2c0a 2020 2020 2020 2020 2020 2020 6174  ,.            at
+0000be10: 6f6d 6963 2c0a 2020 2020 2020 2020 2020  omic,.          
+0000be20: 2020 7665 7274 6963 6573 2c0a 2020 2020    vertices,.    
+0000be30: 2020 2020 2020 2020 7374 6570 2c0a 2020          step,.  
+0000be40: 2020 2020 2020 2020 2020 7072 6f62 655f            probe_
+0000be50: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0000be60: 6967 6e6f 7265 5f62 6163 6b62 6f6e 652c  ignore_backbone,
+0000be70: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+0000be80: 652c 0a20 2020 2020 2020 2020 2020 206e  e,.            n
+0000be90: 7468 7265 6164 732c 0a20 2020 2020 2020  threads,.       
+0000bea0: 2020 2020 2076 6572 626f 7365 2c0a 2020       verbose,.  
+0000beb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000bec0: 6672 6571 7565 6e63 6965 7320 3d20 6361  frequencies = ca
+0000bed0: 6c63 756c 6174 655f 6672 6571 7565 6e63  lculate_frequenc
+0000bee0: 6965 7328 7265 7369 6475 6573 290a 0a20  ies(residues).. 
+0000bef0: 2020 2020 2020 2023 2044 6570 7468 2063         # Depth c
+0000bf00: 6861 7261 6374 6572 697a 6174 696f 6e0a  haracterization.
+0000bf10: 2020 2020 2020 2020 6966 2069 6e63 6c75          if inclu
+0000bf20: 6465 5f64 6570 7468 3a0a 2020 2020 2020  de_depth:.      
+0000bf30: 2020 2020 2020 6465 7074 6873 2c20 6d61        depths, ma
+0000bf40: 785f 6465 7074 682c 2061 7667 5f64 6570  x_depth, avg_dep
+0000bf50: 7468 203d 2064 6570 7468 280a 2020 2020  th = depth(.    
+0000bf60: 2020 2020 2020 2020 2020 2020 6361 7669              cavi
+0000bf70: 7469 6573 2c20 7374 6570 2c20 4e6f 6e65  ties, step, None
+0000bf80: 2c20 6e74 6872 6561 6473 2c20 7665 7262  , nthreads, verb
+0000bf90: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
+0000bfa0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000bfb0: 2020 2020 2020 2020 2020 2020 6465 7074              dept
+0000bfc0: 6873 2c20 6d61 785f 6465 7074 682c 2061  hs, max_depth, a
+0000bfd0: 7667 5f64 6570 7468 203d 204e 6f6e 652c  vg_depth = None,
+0000bfe0: 204e 6f6e 652c 204e 6f6e 650a 0a20 2020   None, None..   
+0000bff0: 2020 2020 2023 2048 7964 726f 7061 7468       # Hydropath
+0000c000: 7920 6879 6472 6f70 686f 6269 6369 7479  y hydrophobicity
+0000c010: 2073 6361 6c65 730a 2020 2020 2020 2020   scales.        
+0000c020: 6966 2069 6e63 6c75 6465 5f68 7964 726f  if include_hydro
+0000c030: 7061 7468 793a 0a20 2020 2020 2020 2020  pathy:.         
+0000c040: 2020 2073 6361 6c65 732c 2061 7667 5f68     scales, avg_h
+0000c050: 7964 726f 7061 7468 7920 3d20 6879 6472  ydropathy = hydr
+0000c060: 6f70 6174 6879 280a 2020 2020 2020 2020  opathy(.        
+0000c070: 2020 2020 2020 2020 7375 7266 6163 652c          surface,
+0000c080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c090: 2061 746f 6d69 632c 0a20 2020 2020 2020   atomic,.       
+0000c0a0: 2020 2020 2020 2020 2076 6572 7469 6365           vertice
+0000c0b0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000c0c0: 2020 2073 7465 702c 0a20 2020 2020 2020     step,.       
+0000c0d0: 2020 2020 2020 2020 2070 726f 6265 5f69           probe_i
+0000c0e0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0000c0f0: 2020 2068 7964 726f 7068 6f62 6963 6974     hydrophobicit
+0000c100: 795f 7363 616c 652c 0a20 2020 2020 2020  y_scale,.       
+0000c110: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
+0000c120: 6261 636b 626f 6e65 2c0a 2020 2020 2020  backbone,.      
+0000c130: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 6e74 6872 6561 6473 2c0a 2020 2020 2020  nthreads,.      
+0000c160: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+0000c170: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+0000c180: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000c190: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+0000c1a0: 732c 2061 7667 5f68 7964 726f 7061 7468  s, avg_hydropath
+0000c1b0: 7920 3d20 4e6f 6e65 2c20 4e6f 6e65 0a20  y = None, None. 
+0000c1c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c1d0: 2070 7269 6e74 2822 5761 726e 696e 673a   print("Warning:
+0000c1e0: 204e 6f20 6361 7669 7469 6573 2064 6574   No cavities det
+0000c1f0: 6563 7465 642c 2072 6574 7572 6e69 6e67  ected, returning
+0000c200: 204e 6f6e 6521 2229 0a20 2020 2020 2020   None!").       
+0000c210: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+0000c220: 2020 2320 5265 7475 726e 2064 6963 740a    # Return dict.
+0000c230: 2020 2020 7265 7375 6c74 7320 3d20 7079      results = py
+0000c240: 4b56 4669 6e64 6572 5265 7375 6c74 7328  KVFinderResults(
+0000c250: 0a20 2020 2020 2020 2063 6176 6974 6965  .        cavitie
+0000c260: 732c 0a20 2020 2020 2020 2073 7572 6661  s,.        surfa
+0000c270: 6365 2c0a 2020 2020 2020 2020 6465 7074  ce,.        dept
+0000c280: 6873 2c0a 2020 2020 2020 2020 7363 616c  hs,.        scal
+0000c290: 6573 2c0a 2020 2020 2020 2020 766f 6c75  es,.        volu
+0000c2a0: 6d65 2c0a 2020 2020 2020 2020 6172 6561  me,.        area
+0000c2b0: 2c0a 2020 2020 2020 2020 6d61 785f 6465  ,.        max_de
+0000c2c0: 7074 682c 0a20 2020 2020 2020 2061 7667  pth,.        avg
+0000c2d0: 5f64 6570 7468 2c0a 2020 2020 2020 2020  _depth,.        
+0000c2e0: 6176 675f 6879 6472 6f70 6174 6879 2c0a  avg_hydropathy,.
+0000c2f0: 2020 2020 2020 2020 7265 7369 6475 6573          residues
+0000c300: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
+0000c310: 6e63 6965 732c 0a20 2020 2020 2020 2076  ncies,.        v
+0000c320: 6572 7469 6365 732c 0a20 2020 2020 2020  ertices,.       
+0000c330: 2073 7465 702c 0a20 2020 2020 2020 2069   step,.        i
+0000c340: 6e70 7574 2c0a 2020 2020 2020 2020 6c69  nput,.        li
+0000c350: 6761 6e64 2c0a 2020 2020 290a 0a20 2020  gand,.    )..   
+0000c360: 2072 6574 7572 6e20 7265 7375 6c74 730a   return results.
+0000c370: 0a0a 636c 6173 7320 4d6f 6c65 6375 6c65  ..class Molecule
+0000c380: 286f 626a 6563 7429 3a0a 2020 2020 2222  (object):.    ""
+0000c390: 2241 2063 6c61 7373 2066 6f72 2072 6570  "A class for rep
+0000c3a0: 7265 7365 6e74 696e 6720 6d6f 6c65 6375  resenting molecu
+0000c3b0: 6c61 7220 7374 7275 6374 7572 6573 2e0a  lar structures..
+0000c3c0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0000c3d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000c3e0: 2020 206d 6f6c 6563 756c 6520 3a20 556e     molecule : Un
+0000c3f0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
+0000c400: 2e50 6174 685d 0a20 2020 2020 2020 2041  .Path].        A
+0000c410: 2066 696c 6520 7061 7468 2074 6f20 7468   file path to th
+0000c420: 6520 6d6f 6c65 6375 6c65 2069 6e20 6569  e molecule in ei
+0000c430: 7468 6572 2050 4442 206f 7220 5859 5a20  ther PDB or XYZ 
+0000c440: 666f 726d 6174 0a20 2020 2072 6164 6969  format.    radii
+0000c450: 203a 2055 6e69 6f6e 5b73 7472 2c20 7061   : Union[str, pa
+0000c460: 7468 6c69 622e 5061 7468 2c20 4469 6374  thlib.Path, Dict
+0000c470: 5b73 7472 2c20 416e 795d 5d2c 206f 7074  [str, Any]], opt
+0000c480: 696f 6e61 6c0a 2020 2020 2020 2020 4120  ional.        A 
+0000c490: 6669 6c65 2070 6174 6820 746f 2061 2076  file path to a v
+0000c4a0: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
+0000c4b0: 6969 2066 696c 6520 6f72 2061 2064 6963  ii file or a dic
+0000c4c0: 7469 6f6e 6172 7920 6f66 2056 4457 2072  tionary of VDW r
+0000c4d0: 6164 6969 2c20 6279 2064 6566 6175 6c74  adii, by default
+0000c4e0: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
+0000c4f0: 6170 706c 7920 7468 6520 6275 696c 742d  apply the built-
+0000c500: 696e 2076 616e 2064 6572 2057 6161 6c73  in van der Waals
+0000c510: 2072 6164 6969 2066 696c 653a 2060 7664   radii file: `vd
+0000c520: 772e 6461 7460 2e0a 2020 2020 6d6f 6465  w.dat`..    mode
+0000c530: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
+0000c540: 6c0a 2020 2020 2020 2020 5468 6520 6d6f  l.        The mo
+0000c550: 6465 6c20 6e75 6d62 6572 206f 6620 6120  del number of a 
+0000c560: 6d75 6c74 692d 6d6f 6465 6c20 5044 4220  multi-model PDB 
+0000c570: 6669 6c65 2c20 6279 2064 6566 6175 6c74  file, by default
+0000c580: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
+0000c590: 6b65 6570 2061 746f 6d73 2066 726f 6d20  keep atoms from 
+0000c5a0: 616c 6c20 6d6f 6465 6c73 2e0a 2020 2020  all models..    
+0000c5b0: 6e74 6872 6561 6473 203a 2069 6e74 2c20  nthreads : int, 
+0000c5c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000c5d0: 204e 756d 6265 7220 6f66 2074 6872 6561   Number of threa
+0000c5e0: 6473 2c20 6279 2064 6566 6175 6c74 204e  ds, by default N
+0000c5f0: 6f6e 652e 2049 6620 4e6f 6e65 2c20 7468  one. If None, th
+0000c600: 6520 6e75 6d62 6572 206f 6620 7468 7265  e number of thre
+0000c610: 6164 7320 6973 2060 6f73 2e63 7075 5f63  ads is `os.cpu_c
+0000c620: 6f75 6e74 2829 202d 2031 602e 0a20 2020  ount() - 1`..   
+0000c630: 2076 6572 626f 7365 203a 2062 6f6f 6c2c   verbose : bool,
+0000c640: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000c650: 2020 5072 696e 7420 6578 7472 6120 696e    Print extra in
+0000c660: 666f 726d 6174 696f 6e20 746f 2073 7461  formation to sta
+0000c670: 6e64 6172 6420 6f75 7470 7574 2c20 6279  ndard output, by
+0000c680: 2064 6566 6175 6c74 2046 616c 7365 2e0a   default False..
+0000c690: 0a20 2020 2041 7474 7269 6275 7465 730a  .    Attributes.
+0000c6a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000c6b0: 2020 205f 6174 6f6d 6963 203a 206e 756d     _atomic : num
+0000c6c0: 7079 2e6e 6461 7272 6179 0a20 2020 2020  py.ndarray.     
+0000c6d0: 2020 2041 206e 756d 7079 2061 7272 6179     A numpy array
+0000c6e0: 2077 6974 6820 6174 6f6d 6963 2064 6174   with atomic dat
+0000c6f0: 6120 2872 6573 6964 7565 206e 756d 6265  a (residue numbe
+0000c700: 722c 2063 6861 696e 2c20 7265 7369 6475  r, chain, residu
+0000c710: 6520 6e61 6d65 2c20 6174 6f6d 206e 616d  e name, atom nam
+0000c720: 652c 2078 797a 2063 6f6f 7264 696e 6174  e, xyz coordinat
+0000c730: 6573 2061 6e64 2072 6164 6975 7329 2066  es and radius) f
+0000c740: 6f72 2065 6163 6820 6174 6f6d 2e0a 2020  or each atom..  
+0000c750: 2020 5f64 696d 203a 2074 7570 6c65 0a20    _dim : tuple. 
+0000c760: 2020 2020 2020 2047 7269 6420 6469 6d65         Grid dime
+0000c770: 6e73 696f 6e73 2e0a 2020 2020 5f67 7269  nsions..    _gri
+0000c780: 6420 3a20 6e75 6d70 792e 6e64 6172 7261  d : numpy.ndarra
+0000c790: 790a 2020 2020 2020 2020 4d6f 6c65 6375  y.        Molecu
+0000c7a0: 6c65 2070 6f69 6e74 7320 696e 2074 6865  le points in the
+0000c7b0: 2033 4420 6772 6964 2028 6772 6964 5b6e   3D grid (grid[n
+0000c7c0: 785d 5b6e 795d 5b6e 7a5d 292e 0a20 2020  x][ny][nz])..   
+0000c7d0: 2020 2020 2047 7269 6420 6172 7261 7920       Grid array 
+0000c7e0: 6861 7320 696e 7465 6765 7220 6c61 6265  has integer labe
+0000c7f0: 6c73 2069 6e20 6561 6368 2070 6f73 6974  ls in each posit
+0000c800: 696f 6e2c 2074 6861 7420 6172 653a 0a0a  ion, that are:..
+0000c810: 2020 2020 2020 2020 2020 2020 2a20 303a              * 0:
+0000c820: 206d 6f6c 6563 756c 6520 706f 696e 7473   molecule points
+0000c830: 3b0a 0a20 2020 2020 2020 2020 2020 202a  ;..            *
+0000c840: 2031 3a20 736f 6c76 656e 7420 706f 696e   1: solvent poin
+0000c850: 7473 2e0a 2020 2020 5f6d 6f6c 6563 756c  ts..    _molecul
+0000c860: 6520 3a20 556e 696f 6e5b 7374 722c 2070  e : Union[str, p
+0000c870: 6174 686c 6962 2e50 6174 685d 0a20 2020  athlib.Path].   
+0000c880: 2020 2020 2041 2066 696c 6520 7061 7468       A file path
+0000c890: 2074 6f20 7468 6520 6d6f 6c65 6375 6c65   to the molecule
+0000c8a0: 2069 6e20 6569 7468 6572 2050 4442 206f   in either PDB o
+0000c8b0: 7220 5859 5a20 666f 726d 6174 2e0a 2020  r XYZ format..  
+0000c8c0: 2020 5f70 6164 6469 6e67 203a 2066 6c6f    _padding : flo
+0000c8d0: 6174 0a20 2020 2020 2020 2054 6865 206c  at.        The l
+0000c8e0: 656e 6774 6820 746f 2061 6464 2074 6f20  ength to add to 
+0000c8f0: 6561 6368 2064 6972 6563 7469 6f6e 206f  each direction o
+0000c900: 6620 7468 6520 3344 2067 7269 642e 0a20  f the 3D grid.. 
+0000c910: 2020 205f 7072 6f62 6520 3a20 666c 6f61     _probe : floa
+0000c920: 740a 2020 2020 2020 2020 5370 6865 7269  t.        Spheri
+0000c930: 6361 6c20 7072 6f62 6520 7369 7a65 2074  cal probe size t
+0000c940: 6f20 6465 6669 6e65 2074 6865 206d 6f6c  o define the mol
+0000c950: 6563 756c 6172 2073 7572 6661 6365 2062  ecular surface b
+0000c960: 6173 6564 206f 6e20 6120 6d6f 6c65 6375  ased on a molecu
+0000c970: 6c61 7220 7265 7072 6573 656e 7461 7469  lar representati
+0000c980: 6f6e 2e0a 2020 2020 5f72 6164 6969 203a  on..    _radii :
+0000c990: 2044 6963 745b 7374 722c 2041 6e79 5d0a   Dict[str, Any].
+0000c9a0: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
+0000c9b0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+0000c9c0: 7261 6469 6920 7661 6c75 6573 2c20 6279  radii values, by
+0000c9d0: 2064 6566 6175 6c74 204e 6f6e 652e 0a20   default None.. 
+0000c9e0: 2020 205f 7265 7072 6573 656e 7461 7469     _representati
+0000c9f0: 6f6e 203a 2073 7472 2c20 6f70 7469 6f6e  on : str, option
+0000ca00: 616c 0a20 2020 2020 2020 204d 6f6c 6563  al.        Molec
+0000ca10: 756c 6172 2073 7572 6661 6365 2072 6570  ular surface rep
+0000ca20: 7265 7365 6e74 6174 696f 6e2e 204b 6579  resentation. Key
+0000ca30: 776f 7264 7320 6f70 7469 6f6e 7320 6172  words options ar
+0000ca40: 6520 7664 5720 2876 616e 2064 6572 2057  e vdW (van der W
+0000ca50: 6161 6c73 2073 7572 6661 6365 292c 2053  aals surface), S
+0000ca60: 4553 2028 536f 6c76 656e 7420 4578 636c  ES (Solvent Excl
+0000ca70: 7564 6564 2053 7572 6661 6365 2920 6f72  uded Surface) or
+0000ca80: 2053 4153 2028 536f 6c76 656e 7420 4163   SAS (Solvent Ac
+0000ca90: 6365 7373 6962 6c65 2053 7572 6661 6365  cessible Surface
+0000caa0: 292c 2062 7920 6465 6661 756c 7420 5345  ), by default SE
+0000cab0: 532e 0a20 2020 205f 726f 7461 7469 6f6e  S..    _rotation
+0000cac0: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
+0000cad0: 0a20 2020 2020 2020 2041 206e 756d 7079  .        A numpy
+0000cae0: 2e6e 6461 7272 6179 2077 6974 6820 7369  .ndarray with si
+0000caf0: 6e65 2061 6e64 2063 6f73 7369 6e65 206f  ne and cossine o
+0000cb00: 6620 7468 6520 6772 6964 2072 6f74 6174  f the grid rotat
+0000cb10: 696f 6e20 616e 676c 6573 2028 7369 6e61  ion angles (sina
+0000cb20: 2c20 636f 7361 2c20 7369 6e62 2c20 636f  , cosa, sinb, co
+0000cb30: 7362 292e 0a20 2020 205f 7374 6570 203a  sb)..    _step :
+0000cb40: 2066 6c6f 6174 0a20 2020 2020 2020 2047   float.        G
+0000cb50: 7269 6420 7370 6163 696e 6720 2841 292e  rid spacing (A).
+0000cb60: 0a20 2020 205f 7665 7274 6963 6573 203a  .    _vertices :
+0000cb70: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
+0000cb80: 2020 2020 2020 2041 206e 756d 7079 2e6e         A numpy.n
+0000cb90: 6461 7272 6179 206f 7220 6120 6c69 7374  darray or a list
+0000cba0: 2077 6974 6820 7879 7a20 7665 7274 6963   with xyz vertic
+0000cbb0: 6573 2063 6f6f 7264 696e 6174 6573 2028  es coordinates (
+0000cbc0: 6f72 6967 696e 2c20 582d 6178 6973 2c20  origin, X-axis, 
+0000cbd0: 592d 6178 6973 2c20 5a2d 6178 6973 292e  Y-axis, Z-axis).
+0000cbe0: 0a20 2020 206e 7468 7265 6164 7320 3a20  .    nthreads : 
+0000cbf0: 696e 740a 2020 2020 2020 2020 4e75 6d62  int.        Numb
+0000cc00: 6572 206f 6620 7468 7265 6164 7320 666f  er of threads fo
+0000cc10: 7220 7061 7261 6c6c 656c 2070 726f 6365  r parallel proce
+0000cc20: 7373 696e 672e 0a20 2020 2076 6572 626f  ssing..    verbo
+0000cc30: 7365 203a 2062 6f6f 6c0a 2020 2020 2020  se : bool.      
+0000cc40: 2020 5768 6574 6865 7220 746f 2070 7269    Whether to pri
+0000cc50: 6e74 2065 7874 7261 2069 6e66 6f72 6d61  nt extra informa
+0000cc60: 7469 6f6e 2074 6f20 7374 616e 6461 7264  tion to standard
+0000cc70: 206f 7574 7075 742e 0a0a 2020 2020 4e6f   output...    No
+0000cc80: 7465 0a20 2020 202d 2d2d 2d0a 2020 2020  te.    ----.    
+0000cc90: 5468 6520 7661 6e20 6465 7220 5761 616c  The van der Waal
+0000cca0: 7320 7261 6469 6920 6669 6c65 2064 6566  s radii file def
+0000ccb0: 696e 6573 2074 6865 2072 6164 6975 7320  ines the radius 
+0000ccc0: 7661 6c75 6573 2066 6f72 2065 6163 6820  values for each 
+0000ccd0: 6174 6f6d 2062 7920 7265 7369 6475 6520  atom by residue 
+0000cce0: 616e 6420 7768 656e 206e 6f74 2064 6566  and when not def
+0000ccf0: 696e 6564 2c20 6974 2075 7365 7320 6120  ined, it uses a 
+0000cd00: 6765 6e65 7269 6320 7661 6c75 6520 6261  generic value ba
+0000cd10: 7365 6420 6f6e 2074 6865 2061 746f 6d20  sed on the atom 
+0000cd20: 7479 7065 2e20 5468 6520 6675 6e63 7469  type. The functi
+0000cd30: 6f6e 2062 7920 6465 6661 756c 7420 6c6f  on by default lo
+0000cd40: 6164 7320 7468 6520 6275 696c 742d 696e  ads the built-in
+0000cd50: 2076 616e 2064 6572 2057 6161 6c73 2072   van der Waals r
+0000cd60: 6164 6969 2066 696c 653a 2060 6076 6477  adii file: ``vdw
+0000cd70: 2e64 6174 6060 2e0a 0a20 2020 2053 6565  .dat``...    See
+0000cd80: 2041 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   Also.    ------
+0000cd90: 2d2d 0a20 2020 2072 6561 645f 7664 770a  --.    read_vdw.
+0000cda0: 0a20 2020 2045 7861 6d70 6c65 0a20 2020  .    Example.   
+0000cdb0: 202d 2d2d 2d2d 2d2d 0a20 2020 2054 6865   -------.    The
+0000cdc0: 2060 604d 6f6c 6563 756c 6560 6020 636c   ``Molecule`` cl
+0000cdd0: 6173 7320 6c6f 6164 7320 7468 6520 7461  ass loads the ta
+0000cde0: 7267 6574 206d 6f6c 6563 756c 6172 2073  rget molecular s
+0000cdf0: 7472 7563 7475 7265 2028 436c 4f34 2920  tructure (ClO4) 
+0000ce00: 696e 746f 2070 794b 5646 696e 6465 722e  into pyKVFinder.
+0000ce10: 2063 6c61 7373 2e0a 0a20 2020 203e 3e3e   class...    >>>
+0000ce20: 2069 6d70 6f72 7420 6f73 0a20 2020 203e   import os.    >
+0000ce30: 3e3e 2066 726f 6d20 7079 4b56 4669 6e64  >> from pyKVFind
+0000ce40: 6572 2069 6d70 6f72 7420 4d6f 6c65 6375  er import Molecu
+0000ce50: 6c65 0a20 2020 203e 3e3e 2070 6462 203d  le.    >>> pdb =
+0000ce60: 206f 732e 7061 7468 2e6a 6f69 6e28 6f73   os.path.join(os
+0000ce70: 2e70 6174 682e 6469 726e 616d 6528 7079  .path.dirname(py
+0000ce80: 4b56 4669 6e64 6572 2e5f 5f66 696c 655f  KVFinder.__file_
+0000ce90: 5f29 2c20 2764 6174 6127 2c20 2774 6573  _), 'data', 'tes
+0000cea0: 7473 272c 2027 436c 4f34 2e70 6462 2729  ts', 'ClO4.pdb')
+0000ceb0: 0a20 2020 203e 3e3e 206d 6f6c 6563 756c  .    >>> molecul
+0000cec0: 6520 3d20 4d6f 6c65 6375 6c65 2870 6462  e = Molecule(pdb
+0000ced0: 290a 2020 2020 3e3e 3e20 6d6f 6c65 6375  ).    >>> molecu
+0000cee0: 6c65 0a20 2020 203e 3e3e 203c 7079 4b56  le.    >>> <pyKV
+0000cef0: 4669 6e64 6572 2e6d 6169 6e2e 4d6f 6c65  Finder.main.Mole
+0000cf00: 6375 6c65 206f 626a 6563 7420 6174 2030  cule object at 0
+0000cf10: 7837 6635 6464 6163 6632 3233 303e 0a0a  x7f5ddacf2230>..
+0000cf20: 2020 2020 5468 6520 7661 6e20 6465 7220      The van der 
+0000cf30: 5761 616c 7320 7261 6469 6920 6361 6e20  Waals radii can 
+0000cf40: 6265 2064 6566 696e 6520 6279 3a0a 0a20  be define by:.. 
+0000cf50: 2020 2020 2020 202a 2063 7265 6174 696e         * creatin
+0000cf60: 6720 6120 5079 7468 6f6e 2064 6963 7469  g a Python dicti
+0000cf70: 6f6e 6172 793a 0a0a 2020 2020 2020 2020  onary:..        
+0000cf80: 3e3e 3e20 2320 5079 4d4f 4c20 2876 322e  >>> # PyMOL (v2.
+0000cf90: 352e 3029 2076 6457 2072 6164 6969 2076  5.0) vdW radii v
+0000cfa0: 616c 7565 730a 2020 2020 2020 2020 3e3e  alues.        >>
+0000cfb0: 3e20 7664 7720 3d20 7b27 4745 4e27 3a20  > vdw = {'GEN': 
+0000cfc0: 7b27 434c 273a 2031 2e37 352c 2027 4f27  {'CL': 1.75, 'O'
+0000cfd0: 3a20 312e 3532 7d7d 0a20 2020 2020 2020  : 1.52}}.       
+0000cfe0: 203e 3e3e 206d 6f6c 6563 756c 6520 3d20   >>> molecule = 
+0000cff0: 4d6f 6c65 6375 6c65 2870 6462 2c20 7261  Molecule(pdb, ra
+0000d000: 6469 693d 7664 7729 0a20 2020 2020 2020  dii=vdw).       
+0000d010: 203e 3e3e 206d 6f6c 6563 756c 652e 7261   >>> molecule.ra
+0000d020: 6469 690a 2020 2020 2020 2020 7b27 4745  dii.        {'GE
+0000d030: 4e27 3a20 7b27 434c 273a 2031 2e37 352c  N': {'CL': 1.75,
+0000d040: 2027 4f27 3a20 312e 3532 7d7d 0a0a 2020   'O': 1.52}}..  
+0000d050: 2020 2020 2020 2a20 7370 6563 6966 7969        * specifyi
+0000d060: 6e67 2061 202a 2e64 6174 2a20 6669 6c65  ng a *.dat* file
+0000d070: 2066 6f6c 6c6f 7769 6e67 2074 656d 706c   following templ
+0000d080: 6174 6520 6f66 2060 7661 6e20 6465 7220  ate of `van der 
+0000d090: 5761 616c 7320 7261 6469 6920 6669 6c65  Waals radii file
+0000d0a0: 602e 0a0a 2020 2020 2020 2020 3e3e 3e20  `...        >>> 
+0000d0b0: 6672 6f6d 2070 794b 5646 696e 6465 7220  from pyKVFinder 
+0000d0c0: 696d 706f 7274 2072 6561 645f 7664 770a  import read_vdw.
+0000d0d0: 2020 2020 2020 2020 3e3e 3e20 2320 4368          >>> # Ch
+0000d0e0: 696d 6572 6158 2076 6457 2072 6164 6969  imeraX vdW radii
+0000d0f0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+0000d100: 3e3e 3e20 7769 7468 206f 7065 6e28 2776  >>> with open('v
+0000d110: 6477 2e64 6174 272c 2027 7727 2920 6173  dw.dat', 'w') as
+0000d120: 2066 3a0a 2020 2020 2020 2020 2e2e 2e20   f:.        ... 
+0000d130: 2020 2020 662e 7772 6974 6528 273e 4745      f.write('>GE
+0000d140: 4e5c 5c6e 434c 5c5c 745c 5c74 312e 3938  N\\nCL\\t\\t1.98
+0000d150: 5c5c 6e4f 5c5c 745c 5c74 312e 3436 5c5c  \\nO\\t\\t1.46\\
+0000d160: 6e27 290a 2020 2020 2020 2020 3e3e 3e20  n').        >>> 
+0000d170: 7664 7720 3d20 7265 6164 5f76 6477 2827  vdw = read_vdw('
+0000d180: 7664 772e 6461 7427 290a 2020 2020 2020  vdw.dat').      
+0000d190: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 203d    >>> molecule =
+0000d1a0: 204d 6f6c 6563 756c 6528 7064 622c 2072   Molecule(pdb, r
+0000d1b0: 6164 6969 3d76 6477 290a 2020 2020 2020  adii=vdw).      
+0000d1c0: 2020 3e3e 3e20 6d6f 6c65 6375 6c65 2e72    >>> molecule.r
+0000d1d0: 6164 6969 0a20 2020 2020 2020 207b 2747  adii.        {'G
+0000d1e0: 454e 273a 207b 2743 4c27 3a20 312e 3938  EN': {'CL': 1.98
+0000d1f0: 2c20 274f 273a 2031 2e34 367d 7d0a 2020  , 'O': 1.46}}.  
+0000d200: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+0000d210: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000d220: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
+0000d230: 6f6c 6563 756c 653a 2055 6e69 6f6e 5b73  olecule: Union[s
+0000d240: 7472 2c20 7061 7468 6c69 622e 5061 7468  tr, pathlib.Path
+0000d250: 5d2c 0a20 2020 2020 2020 2072 6164 6969  ],.        radii
+0000d260: 3a20 556e 696f 6e5b 7374 722c 2070 6174  : Union[str, pat
+0000d270: 686c 6962 2e50 6174 682c 2044 6963 745b  hlib.Path, Dict[
+0000d280: 7374 722c 2041 6e79 5d5d 203d 204e 6f6e  str, Any]] = Non
+0000d290: 652c 0a20 2020 2020 2020 206d 6f64 656c  e,.        model
+0000d2a0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0000d2b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000d2c0: 6e74 6872 6561 6473 3a20 4f70 7469 6f6e  nthreads: Option
+0000d2d0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+0000d2e0: 2020 2020 2020 2020 7665 7262 6f73 653a          verbose:
+0000d2f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000d300: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000d310: 2249 6e69 7469 616c 697a 6520 7468 6520  "Initialize the 
+0000d320: 4d6f 6c65 6375 6c65 206f 626a 6563 7420  Molecule object 
+0000d330: 7769 7468 206d 6f6c 6563 756c 652c 2072  with molecule, r
+0000d340: 6164 6969 2c20 6d6f 6465 6c2c 206e 7468  adii, model, nth
+0000d350: 7265 6164 7320 616e 6420 7665 7262 6f73  reads and verbos
+0000d360: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+0000d370: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0000d380: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000d390: 2020 6d6f 6c65 6375 6c65 203a 2055 6e69    molecule : Uni
+0000d3a0: 6f6e 5b73 7472 2c20 7061 7468 6c69 622e  on[str, pathlib.
+0000d3b0: 5061 7468 5d0a 2020 2020 2020 2020 2020  Path].          
+0000d3c0: 2020 4120 6669 6c65 2070 6174 6820 746f    A file path to
+0000d3d0: 2074 6865 206d 6f6c 6563 756c 6520 696e   the molecule in
+0000d3e0: 2065 6974 6865 7220 5044 4220 6f72 2058   either PDB or X
+0000d3f0: 595a 2066 6f72 6d61 742e 0a20 2020 2020  YZ format..     
+0000d400: 2020 2072 6164 6969 203a 2055 6e69 6f6e     radii : Union
+0000d410: 5b73 7472 2c20 7061 7468 6c69 622e 5061  [str, pathlib.Pa
+0000d420: 7468 2c20 4469 6374 5b73 7472 2c20 416e  th, Dict[str, An
+0000d430: 795d 5d2c 206f 7074 696f 6e61 6c0a 2020  y]], optional.  
+0000d440: 2020 2020 2020 2020 2020 4120 6669 6c65            A file
+0000d450: 2070 6174 6820 746f 2061 2076 616e 2064   path to a van d
+0000d460: 6572 2057 6161 6c73 2072 6164 6969 2066  er Waals radii f
+0000d470: 696c 6520 6f72 2061 2064 6963 7469 6f6e  ile or a diction
+0000d480: 6172 7920 6f66 2056 4457 2072 6164 6969  ary of VDW radii
+0000d490: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
+0000d4a0: 652e 2049 6620 4e6f 6e65 2c20 6170 706c  e. If None, appl
+0000d4b0: 7920 7468 6520 6275 696c 742d 696e 2076  y the built-in v
+0000d4c0: 616e 2064 6572 2057 6161 6c73 2072 6164  an der Waals rad
+0000d4d0: 6969 2066 696c 653a 2060 7664 772e 6461  ii file: `vdw.da
+0000d4e0: 7460 2e0a 2020 2020 2020 2020 6d6f 6465  t`..        mode
+0000d4f0: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
+0000d500: 6c0a 2020 2020 2020 2020 2020 2020 5468  l.            Th
+0000d510: 6520 6d6f 6465 6c20 6e75 6d62 6572 206f  e model number o
+0000d520: 6620 6120 6d75 6c74 692d 6d6f 6465 6c20  f a multi-model 
+0000d530: 5044 4220 6669 6c65 2c20 6279 2064 6566  PDB file, by def
+0000d540: 6175 6c74 204e 6f6e 652e 2049 6620 4e6f  ault None. If No
+0000d550: 6e65 2c20 6b65 6570 2061 746f 6d73 2066  ne, keep atoms f
+0000d560: 726f 6d20 616c 6c20 6d6f 6465 6c73 2e0a  rom all models..
+0000d570: 2020 2020 2020 2020 6e74 6872 6561 6473          nthreads
+0000d580: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+0000d590: 0a20 2020 2020 2020 2020 2020 204e 756d  .            Num
+0000d5a0: 6265 7220 6f66 2074 6872 6561 6473 2c20  ber of threads, 
+0000d5b0: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
+0000d5c0: 2049 6620 4e6f 6e65 2c20 7468 6520 6e75   If None, the nu
+0000d5d0: 6d62 6572 206f 6620 7468 7265 6164 7320  mber of threads 
+0000d5e0: 6973 2060 6f73 2e63 7075 5f63 6f75 6e74  is `os.cpu_count
+0000d5f0: 2829 202d 2031 602e 0a20 2020 2020 2020  () - 1`..       
+0000d600: 2076 6572 626f 7365 203a 2062 6f6f 6c2c   verbose : bool,
+0000d610: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000d620: 2020 2020 2020 5072 696e 7420 6578 7472        Print extr
+0000d630: 6120 696e 666f 726d 6174 696f 6e20 746f  a information to
+0000d640: 2073 7461 6e64 6172 6420 6f75 7470 7574   standard output
+0000d650: 2c20 6279 2064 6566 6175 6c74 2046 616c  , by default Fal
+0000d660: 7365 2e0a 0a20 2020 2020 2020 2052 6169  se...        Rai
+0000d670: 7365 730a 2020 2020 2020 2020 2d2d 2d2d  ses.        ----
+0000d680: 2d2d 0a20 2020 2020 2020 2054 7970 6545  --.        TypeE
+0000d690: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
+0000d6a0: 2060 6d6f 6c65 6375 6c65 6020 6d75 7374   `molecule` must
+0000d6b0: 2062 6520 6120 7374 7269 6e67 206f 7220   be a string or 
+0000d6c0: 6120 7061 7468 6c69 622e 5061 7468 2e0a  a pathlib.Path..
+0000d6d0: 2020 2020 2020 2020 5479 7065 4572 726f          TypeErro
+0000d6e0: 720a 2020 2020 2020 2020 2020 2020 606d  r.            `m
+0000d6f0: 6f6c 6563 756c 6560 206d 7573 7420 6861  olecule` must ha
+0000d700: 7665 202e 7064 6220 6f72 202e 7879 7a20  ve .pdb or .xyz 
+0000d710: 6578 7465 6e73 696f 6e2e 0a20 2020 2020  extension..     
+0000d720: 2020 2054 7970 6545 7272 6f72 0a20 2020     TypeError.   
+0000d730: 2020 2020 2020 2020 2060 6e74 6872 6561           `nthrea
+0000d740: 6473 6020 6d75 7374 2062 6520 6120 706f  ds` must be a po
+0000d750: 7369 7469 7665 2069 6e74 6567 6572 2e0a  sitive integer..
+0000d760: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+0000d770: 6f72 0a20 2020 2020 2020 2020 2020 2060  or.            `
+0000d780: 6e74 6872 6561 6473 6020 6d75 7374 2062  nthreads` must b
+0000d790: 6520 6120 706f 7369 7469 7665 2069 6e74  e a positive int
+0000d7a0: 6567 6572 2e0a 2020 2020 2020 2020 2222  eger..        ""
+0000d7b0: 220a 0a20 2020 2020 2020 2023 2041 7474  "..        # Att
+0000d7c0: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
+0000d7d0: 7365 6c66 2e5f 6772 6964 203d 204e 6f6e  self._grid = Non
+0000d7e0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000d7f0: 7374 6570 203d 204e 6f6e 650a 2020 2020  step = None.    
+0000d800: 2020 2020 7365 6c66 2e5f 7061 6464 696e      self._paddin
+0000d810: 6720 3d20 4e6f 6e65 0a20 2020 2020 2020  g = None.       
+0000d820: 2073 656c 662e 5f70 726f 6265 203d 204e   self._probe = N
+0000d830: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000d840: 2e5f 7265 7072 6573 656e 7461 7469 6f6e  ._representation
+0000d850: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000d860: 7365 6c66 2e5f 7665 7274 6963 6573 203d  self._vertices =
+0000d870: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000d880: 6c66 2e5f 6469 6d20 3d20 4e6f 6e65 0a20  lf._dim = None. 
+0000d890: 2020 2020 2020 2073 656c 662e 5f72 6f74         self._rot
+0000d8a0: 6174 696f 6e20 3d20 4e6f 6e65 0a20 2020  ation = None.   
+0000d8b0: 2020 2020 2073 656c 662e 7665 7262 6f73       self.verbos
+0000d8c0: 6520 3d20 7665 7262 6f73 650a 0a20 2020  e = verbose..   
+0000d8d0: 2020 2020 2023 204d 6f6c 6563 756c 650a       # Molecule.
+0000d8e0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+0000d8f0: 6d6f 6c65 6375 6c65 2920 6e6f 7420 696e  molecule) not in
+0000d900: 205b 7374 722c 2070 6174 686c 6962 2e50   [str, pathlib.P
+0000d910: 6174 685d 3a0a 2020 2020 2020 2020 2020  ath]:.          
+0000d920: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+0000d930: 7228 2260 6d6f 6c65 6375 6c65 6020 6d75  r("`molecule` mu
+0000d940: 7374 2062 6520 6120 7374 7269 6e67 206f  st be a string o
+0000d950: 7220 6120 7061 7468 6c69 622e 5061 7468  r a pathlib.Path
+0000d960: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000d970: 2e5f 6d6f 6c65 6375 6c65 203d 206f 732e  ._molecule = os.
+0000d980: 7061 7468 2e72 6561 6c70 6174 6828 6d6f  path.realpath(mo
+0000d990: 6c65 6375 6c65 290a 0a20 2020 2020 2020  lecule)..       
+0000d9a0: 2023 2076 616e 2064 6572 2057 6161 6c73   # van der Waals
+0000d9b0: 2072 6164 6969 0a20 2020 2020 2020 2069   radii.        i
+0000d9c0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
+0000d9d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000d9e0: 7428 223e 204c 6f61 6469 6e67 2076 616e  t("> Loading van
+0000d9f0: 2064 6572 2057 6161 6c73 2072 6164 6969   der Waals radii
+0000da00: 2229 0a20 2020 2020 2020 2069 6620 7261  ").        if ra
+0000da10: 6469 6920 6973 204e 6f6e 653a 0a20 2020  dii is None:.   
+0000da20: 2020 2020 2020 2020 2023 2064 6566 6175           # defau
+0000da30: 6c74 0a20 2020 2020 2020 2020 2020 2073  lt.            s
+0000da40: 656c 662e 5f72 6164 6969 203d 2072 6561  elf._radii = rea
+0000da50: 645f 7664 7728 5644 5729 0a20 2020 2020  d_vdw(VDW).     
+0000da60: 2020 2065 6c69 6620 7479 7065 2872 6164     elif type(rad
+0000da70: 6969 2920 696e 205b 7374 722c 2070 6174  ii) in [str, pat
+0000da80: 686c 6962 2e50 6174 685d 3a0a 2020 2020  hlib.Path]:.    
+0000da90: 2020 2020 2020 2020 2320 7664 7720 6669          # vdw fi
+0000daa0: 6c65 0a20 2020 2020 2020 2020 2020 2073  le.            s
+0000dab0: 656c 662e 5f72 6164 6969 203d 2072 6561  elf._radii = rea
+0000dac0: 645f 7664 7728 7261 6469 6929 0a20 2020  d_vdw(radii).   
+0000dad0: 2020 2020 2065 6c69 6620 7479 7065 2872       elif type(r
+0000dae0: 6164 6969 2920 696e 205b 6469 6374 5d3a  adii) in [dict]:
+0000daf0: 0a20 2020 2020 2020 2020 2020 2023 2050  .            # P
+0000db00: 726f 6365 7373 6564 2064 6963 7469 6f6e  rocessed diction
+0000db10: 6172 790a 2020 2020 2020 2020 2020 2020  ary.            
+0000db20: 7365 6c66 2e5f 7261 6469 6920 3d20 7261  self._radii = ra
+0000db30: 6469 690a 0a20 2020 2020 2020 2023 2041  dii..        # A
+0000db40: 746f 6d69 6320 696e 666f 726d 6174 696f  tomic informatio
+0000db50: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000db60: 662e 7665 7262 6f73 653a 0a20 2020 2020  f.verbose:.     
+0000db70: 2020 2020 2020 2070 7269 6e74 2822 3e20         print("> 
+0000db80: 5265 6164 696e 6720 6d6f 6c65 6375 6c65  Reading molecule
+0000db90: 2063 6f6f 7264 696e 6174 6573 2229 0a20   coordinates"). 
+0000dba0: 2020 2020 2020 2069 6620 6d6f 6c65 6375         if molecu
+0000dbb0: 6c65 2e65 6e64 7377 6974 6828 222e 7064  le.endswith(".pd
+0000dbc0: 6222 293a 0a20 2020 2020 2020 2020 2020  b"):.           
+0000dbd0: 2073 656c 662e 5f61 746f 6d69 6320 3d20   self._atomic = 
+0000dbe0: 7265 6164 5f70 6462 286d 6f6c 6563 756c  read_pdb(molecul
+0000dbf0: 652c 2073 656c 662e 7261 6469 692c 206d  e, self.radii, m
+0000dc00: 6f64 656c 290a 2020 2020 2020 2020 656c  odel).        el
+0000dc10: 6966 206d 6f6c 6563 756c 652e 656e 6473  if molecule.ends
+0000dc20: 7769 7468 2822 2e78 797a 2229 3a0a 2020  with(".xyz"):.  
+0000dc30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000dc40: 6174 6f6d 6963 203d 2072 6561 645f 7879  atomic = read_xy
+0000dc50: 7a28 6d6f 6c65 6375 6c65 2c20 7365 6c66  z(molecule, self
+0000dc60: 2e72 6164 6969 290a 2020 2020 2020 2020  .radii).        
+0000dc70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000dc80: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+0000dc90: 7228 2260 6d6f 6c65 6375 6c65 6020 6d75  r("`molecule` mu
+0000dca0: 7374 2068 6176 6520 2e70 6462 206f 7220  st have .pdb or 
+0000dcb0: 2e78 797a 2065 7874 656e 7369 6f6e 2e22  .xyz extension."
+0000dcc0: 290a 0a20 2020 2020 2020 2023 204e 756d  )..        # Num
+0000dcd0: 6265 7220 6f66 2074 6872 6561 6473 0a20  ber of threads. 
+0000dce0: 2020 2020 2020 2069 6620 6e74 6872 6561         if nthrea
+0000dcf0: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
+0000dd00: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000dd10: 7970 6528 6e74 6872 6561 6473 2920 6e6f  ype(nthreads) no
+0000dd20: 7420 696e 205b 696e 745d 3a0a 2020 2020  t in [int]:.    
+0000dd30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000dd40: 6520 5479 7065 4572 726f 7228 2260 6e74  e TypeError("`nt
+0000dd50: 6872 6561 6473 6020 6d75 7374 2062 6520  hreads` must be 
+0000dd60: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
+0000dd70: 6572 2e22 290a 2020 2020 2020 2020 2020  er.").          
+0000dd80: 2020 656c 6966 206e 7468 7265 6164 7320    elif nthreads 
+0000dd90: 3c3d 2030 3a0a 2020 2020 2020 2020 2020  <= 0:.          
+0000dda0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000ddb0: 6545 7272 6f72 2822 606e 7468 7265 6164  eError("`nthread
+0000ddc0: 7360 206d 7573 7420 6265 2061 2070 6f73  s` must be a pos
+0000ddd0: 6974 6976 6520 696e 7465 6765 722e 2229  itive integer.")
+0000dde0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000ddf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000de00: 2020 2073 656c 662e 6e74 6872 6561 6473     self.nthreads
+0000de10: 203d 206e 7468 7265 6164 730a 2020 2020   = nthreads.    
+0000de20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000de30: 2020 2020 2020 7365 6c66 2e6e 7468 7265        self.nthre
+0000de40: 6164 7320 3d20 6f73 2e63 7075 5f63 6f75  ads = os.cpu_cou
+0000de50: 6e74 2829 202d 2031 0a0a 2020 2020 4070  nt() - 1..    @p
+0000de60: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000de70: 6174 6f6d 6963 2873 656c 6629 202d 3e20  atomic(self) -> 
+0000de80: 6e75 6d70 792e 6e64 6172 7261 793a 0a20  numpy.ndarray:. 
+0000de90: 2020 2020 2020 2022 2222 4765 7420 5f61         """Get _a
+0000dea0: 746f 6d69 6320 6174 7472 6962 7574 652e  tomic attribute.
+0000deb0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000dec0: 726e 2073 656c 662e 5f61 746f 6d69 630a  rn self._atomic.
+0000ded0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000dee0: 2020 2064 6566 2064 696d 2873 656c 6629     def dim(self)
+0000def0: 202d 3e20 5475 706c 655b 696e 742c 2069   -> Tuple[int, i
+0000df00: 6e74 2c20 696e 745d 3a0a 2020 2020 2020  nt, int]:.      
+0000df10: 2020 2222 2247 6574 205f 6469 6d20 6174    """Get _dim at
+0000df20: 7472 6962 7574 6522 2222 0a20 2020 2020  tribute""".     
+0000df30: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000df40: 6469 6d0a 0a20 2020 2040 7072 6f70 6572  dim..    @proper
+0000df50: 7479 0a20 2020 2064 6566 2067 7269 6428  ty.    def grid(
+0000df60: 7365 6c66 2920 2d3e 206e 756d 7079 2e6e  self) -> numpy.n
+0000df70: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+0000df80: 2222 2247 6574 205f 6772 6964 2061 7474  """Get _grid att
+0000df90: 7269 6275 7465 2e22 2222 0a20 2020 2020  ribute.""".     
+0000dfa0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000dfb0: 6772 6964 0a0a 2020 2020 4070 726f 7065  grid..    @prope
+0000dfc0: 7274 790a 2020 2020 6465 6620 6d6f 6c65  rty.    def mole
+0000dfd0: 6375 6c65 2873 656c 6629 202d 3e20 556e  cule(self) -> Un
+0000dfe0: 696f 6e5b 7374 722c 2070 6174 686c 6962  ion[str, pathlib
+0000dff0: 2e50 6174 685d 3a0a 2020 2020 2020 2020  .Path]:.        
+0000e000: 2222 2247 6574 205f 6d6f 6c65 6375 6c65  """Get _molecule
+0000e010: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
+0000e020: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e030: 6c66 2e5f 6d6f 6c65 6375 6c65 0a0a 2020  lf._molecule..  
+0000e040: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000e050: 6465 6620 6e78 2873 656c 6629 202d 3e20  def nx(self) -> 
+0000e060: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+0000e070: 4765 7420 6772 6964 2075 6e69 7473 2069  Get grid units i
+0000e080: 6e20 582d 6178 6973 2e22 2222 0a20 2020  n X-axis.""".   
+0000e090: 2020 2020 2069 6620 7365 6c66 2e5f 6469       if self._di
+0000e0a0: 6d20 6973 206e 6f74 204e 6f6e 653a 0a20  m is not None:. 
+0000e0b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e0c0: 6e20 7365 6c66 2e5f 6469 6d5b 305d 0a0a  n self._dim[0]..
+0000e0d0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000e0e0: 2020 6465 6620 6e79 2873 656c 6629 202d    def ny(self) -
+0000e0f0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+0000e100: 2222 4765 7420 6772 6964 2075 6e69 7473  ""Get grid units
+0000e110: 2069 6e20 592d 6178 6973 2e22 2222 0a20   in Y-axis.""". 
+0000e120: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000e130: 6469 6d20 6973 206e 6f74 204e 6f6e 653a  dim is not None:
+0000e140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e150: 7572 6e20 7365 6c66 2e5f 6469 6d5b 315d  urn self._dim[1]
+0000e160: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000e170: 2020 2020 6465 6620 6e7a 2873 656c 6629      def nz(self)
+0000e180: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000e190: 2022 2222 4765 7420 6772 6964 2075 6e69   """Get grid uni
+0000e1a0: 7473 2069 6e20 5a2d 6178 6973 2e22 2222  ts in Z-axis."""
+0000e1b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e1c0: 2e5f 6469 6d20 6973 206e 6f74 204e 6f6e  ._dim is not Non
+0000e1d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000e1e0: 6574 7572 6e20 7365 6c66 2e5f 6469 6d5b  eturn self._dim[
+0000e1f0: 325d 0a0a 2020 2020 4070 726f 7065 7274  2]..    @propert
+0000e200: 790a 2020 2020 6465 6620 7031 2873 656c  y.    def p1(sel
+0000e210: 6629 202d 3e20 6e75 6d70 792e 6e64 6172  f) -> numpy.ndar
+0000e220: 7261 793a 0a20 2020 2020 2020 2022 2222  ray:.        """
+0000e230: 4765 7420 6f72 6967 696e 206f 6620 7468  Get origin of th
+0000e240: 6520 3344 2067 7269 642e 2222 220a 2020  e 3D grid.""".  
+0000e250: 2020 2020 2020 6966 2073 656c 662e 5f76        if self._v
+0000e260: 6572 7469 6365 7320 6973 206e 6f74 204e  ertices is not N
+0000e270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000e280: 2072 6574 7572 6e20 7365 6c66 2e5f 7665   return self._ve
+0000e290: 7274 6963 6573 5b30 5d0a 0a20 2020 2040  rtices[0]..    @
+0000e2a0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000e2b0: 2070 3228 7365 6c66 2920 2d3e 206e 756d   p2(self) -> num
+0000e2c0: 7079 2e6e 6461 7272 6179 3a0a 2020 2020  py.ndarray:.    
+0000e2d0: 2020 2020 2222 2247 6574 2058 2d61 7869      """Get X-axi
+0000e2e0: 7320 6d61 7820 6f66 2074 6865 2033 4420  s max of the 3D 
+0000e2f0: 6772 6964 2e22 2222 0a20 2020 2020 2020  grid.""".       
+0000e300: 2069 6620 7365 6c66 2e5f 7665 7274 6963   if self._vertic
+0000e310: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0000e320: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e330: 726e 2073 656c 662e 5f76 6572 7469 6365  rn self._vertice
+0000e340: 735b 315d 0a0a 2020 2020 4070 726f 7065  s[1]..    @prope
+0000e350: 7274 790a 2020 2020 6465 6620 7033 2873  rty.    def p3(s
+0000e360: 656c 6629 202d 3e20 6e75 6d70 792e 6e64  elf) -> numpy.nd
+0000e370: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
+0000e380: 2222 4765 7420 592d 6178 6973 206d 6178  ""Get Y-axis max
+0000e390: 206f 6620 7468 6520 3344 2067 7269 642e   of the 3D grid.
+0000e3a0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0000e3b0: 656c 662e 5f76 6572 7469 6365 7320 6973  elf._vertices is
+0000e3c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e3d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e3e0: 6c66 2e5f 7665 7274 6963 6573 5b32 5d0a  lf._vertices[2].
+0000e3f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000e400: 2020 2064 6566 2070 3428 7365 6c66 2920     def p4(self) 
+0000e410: 2d3e 206e 756d 7079 2e6e 6461 7272 6179  -> numpy.ndarray
+0000e420: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000e430: 205a 2d61 7869 7320 6d61 7820 6f66 2074   Z-axis max of t
+0000e440: 6865 2033 4420 6772 6964 2e22 2222 0a20  he 3D grid.""". 
+0000e450: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000e460: 7665 7274 6963 6573 2069 7320 6e6f 7420  vertices is not 
+0000e470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000e480: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
+0000e490: 6572 7469 6365 735b 335d 0a0a 2020 2020  ertices[3]..    
+0000e4a0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000e4b0: 6620 7061 6464 696e 6728 7365 6c66 2920  f padding(self) 
+0000e4c0: 2d3e 2066 6c6f 6174 3a0a 2020 2020 2020  -> float:.      
+0000e4d0: 2020 2222 2247 6574 205f 7061 6464 696e    """Get _paddin
+0000e4e0: 6720 6174 7472 6962 7574 652e 2222 220a  g attribute.""".
+0000e4f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000e500: 656c 662e 5f70 6164 6469 6e67 0a0a 2020  elf._padding..  
+0000e510: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000e520: 6465 6620 7072 6f62 6528 7365 6c66 2920  def probe(self) 
+0000e530: 2d3e 2066 6c6f 6174 3a0a 2020 2020 2020  -> float:.      
+0000e540: 2020 2222 2247 6574 205f 7072 6f62 6520    """Get _probe 
+0000e550: 6174 7472 6962 7574 652e 2222 220a 2020  attribute.""".  
+0000e560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000e570: 662e 5f70 726f 6265 0a0a 2020 2020 4070  f._probe..    @p
+0000e580: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000e590: 7261 6469 6928 7365 6c66 2920 2d3e 2044  radii(self) -> D
+0000e5a0: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
+0000e5b0: 2020 2020 2020 2022 2222 4765 7420 5f72         """Get _r
+0000e5c0: 6164 6969 2061 7474 7269 6275 7465 2e22  adii attribute."
+0000e5d0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000e5e0: 6e20 7365 6c66 2e5f 7261 6469 690a 0a20  n self._radii.. 
+0000e5f0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000e600: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
+0000e610: 696f 6e28 7365 6c66 2920 2d3e 2073 7472  ion(self) -> str
+0000e620: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000e630: 205f 7265 7072 6573 656e 7461 7469 6f6e   _representation
+0000e640: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
+0000e650: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e660: 6c66 2e5f 7265 7072 6573 656e 7461 7469  lf._representati
+0000e670: 6f6e 0a0a 2020 2020 4070 726f 7065 7274  on..    @propert
+0000e680: 790a 2020 2020 6465 6620 726f 7461 7469  y.    def rotati
+0000e690: 6f6e 2873 656c 6629 202d 3e20 6e75 6d70  on(self) -> nump
+0000e6a0: 792e 6e64 6172 7261 793a 0a20 2020 2020  y.ndarray:.     
+0000e6b0: 2020 2022 2222 4765 7420 5f72 6f74 6174     """Get _rotat
+0000e6c0: 696f 6e20 6174 7472 6962 7574 652e 2222  ion attribute.""
+0000e6d0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000e6e0: 2073 656c 662e 5f72 6f74 6174 696f 6e0a   self._rotation.
+0000e6f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000e700: 2020 2064 6566 2073 7465 7028 7365 6c66     def step(self
+0000e710: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
+0000e720: 2020 2020 2222 2247 6574 205f 7374 6570      """Get _step
+0000e730: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
+0000e740: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000e750: 7374 6570 2069 7320 6e6f 7420 4e6f 6e65  step is not None
+0000e760: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e770: 7475 726e 2073 656c 662e 5f73 7465 700a  turn self._step.
+0000e780: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000e790: 2020 2064 6566 2076 6572 7469 6365 7328     def vertices(
+0000e7a0: 7365 6c66 2920 2d3e 206e 756d 7079 2e6e  self) -> numpy.n
+0000e7b0: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+0000e7c0: 2222 2247 6574 205f 7665 7274 6963 6573  """Get _vertices
+0000e7d0: 2061 7474 7269 6275 7465 2e22 2222 0a20   attribute.""". 
+0000e7e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e7f0: 6c66 2e5f 7665 7274 6963 6573 0a0a 2020  lf._vertices..  
+0000e800: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000e810: 6465 6620 7879 7a72 2873 656c 6629 202d  def xyzr(self) -
+0000e820: 3e20 6e75 6d70 792e 6e64 6172 7261 793a  > numpy.ndarray:
+0000e830: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000e840: 7879 7a20 636f 6f72 6469 6e61 7465 7320  xyz coordinates 
+0000e850: 616e 6420 7261 6469 7573 206f 6620 6d6f  and radius of mo
+0000e860: 6c65 6375 6c65 2061 746f 6d73 2e22 2222  lecule atoms."""
+0000e870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e880: 7365 6c66 2e5f 6174 6f6d 6963 5b3a 2c20  self._atomic[:, 
+0000e890: 343a 5d2e 6173 7479 7065 286e 756d 7079  4:].astype(numpy
+0000e8a0: 2e66 6c6f 6174 3634 290a 0a20 2020 2064  .float64)..    d
+0000e8b0: 6566 205f 7365 745f 6772 6964 2873 656c  ef _set_grid(sel
+0000e8c0: 662c 2070 6164 6469 6e67 3a20 4f70 7469  f, padding: Opti
+0000e8d0: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
+0000e8e0: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
+0000e8f0: 2020 2020 2022 2222 4465 6669 6e65 2074       """Define t
+0000e900: 6865 2033 4420 6772 6964 2066 6f72 2074  he 3D grid for t
+0000e910: 6865 2074 6172 6765 7420 6d6f 6c65 6375  he target molecu
+0000e920: 6c65 2e0a 0a20 2020 2020 2020 2050 6172  le...        Par
+0000e930: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0000e940: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000e950: 2020 2070 6164 6469 6e67 203a 2066 6c6f     padding : flo
+0000e960: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
+0000e970: 2020 2020 2020 2020 2054 6865 206c 656e           The len
+0000e980: 6774 6820 746f 2061 6464 2074 6f20 6561  gth to add to ea
+0000e990: 6368 2064 6972 6563 7469 6f6e 206f 6620  ch direction of 
+0000e9a0: 7468 6520 3344 2067 7269 642c 2062 7920  the 3D grid, by 
+0000e9b0: 6465 6661 756c 7420 4e6f 6e65 2e20 4966  default None. If
+0000e9c0: 204e 6f6e 652c 2061 7574 6f6d 6174 6963   None, automatic
+0000e9d0: 616c 6c79 2064 6566 696e 6520 7468 6520  ally define the 
+0000e9e0: 6c65 6e67 7468 2062 6173 6564 206f 6e20  length based on 
+0000e9f0: 6d6f 6c65 6375 6c65 2063 6f6f 7264 696e  molecule coordin
+0000ea00: 6174 6573 2c20 7072 6f62 6520 7369 7a65  ates, probe size
+0000ea10: 2c20 6772 6964 2073 7061 6369 6e67 2061  , grid spacing a
+0000ea20: 6e64 2061 746f 6d20 7261 6469 692e 0a0a  nd atom radii...
+0000ea30: 2020 2020 2020 2020 5261 6973 6573 0a20          Raises. 
+0000ea40: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
+0000ea50: 2020 2020 2020 5479 7065 4572 726f 720a        TypeError.
+0000ea60: 2020 2020 2020 2020 2020 2020 6070 6164              `pad
+0000ea70: 6469 6e67 6020 6d75 7374 2062 6520 6120  ding` must be a 
+0000ea80: 6e6f 6e2d 6e65 6761 7469 7665 2072 6561  non-negative rea
+0000ea90: 6c20 6e75 6d62 6572 2e0a 2020 2020 2020  l number..      
+0000eaa0: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+0000eab0: 2020 2020 2020 2020 2060 7061 6464 696e           `paddin
+0000eac0: 6760 206d 7573 7420 6265 2061 206e 6f6e  g` must be a non
+0000ead0: 2d6e 6567 6174 6976 6520 7265 616c 206e  -negative real n
+0000eae0: 756d 6265 722e 0a20 2020 2020 2020 2022  umber..        "
+0000eaf0: 2222 0a20 2020 2020 2020 2023 2050 6164  "".        # Pad
+0000eb00: 6469 6e67 0a20 2020 2020 2020 2069 6620  ding.        if 
+0000eb10: 7061 6464 696e 6720 6973 206e 6f74 204e  padding is not N
+0000eb20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000eb30: 2069 6620 7479 7065 2870 6164 6469 6e67   if type(padding
+0000eb40: 2920 6e6f 7420 696e 205b 696e 742c 2066  ) not in [int, f
+0000eb50: 6c6f 6174 5d3a 0a20 2020 2020 2020 2020  loat]:.         
+0000eb60: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000eb70: 6545 7272 6f72 2822 6070 6164 6469 6e67  eError("`padding
+0000eb80: 6020 6d75 7374 2062 6520 6120 6e6f 6e2d  ` must be a non-
+0000eb90: 6e65 6761 7469 7665 2072 6561 6c20 6e75  negative real nu
+0000eba0: 6d62 6572 2e22 290a 2020 2020 2020 2020  mber.").        
+0000ebb0: 2020 2020 656c 6966 2070 6164 6469 6e67      elif padding
+0000ebc0: 203c 2030 2e30 3a0a 2020 2020 2020 2020   < 0.0:.        
+0000ebd0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000ebe0: 6c75 6545 7272 6f72 2822 6070 6164 6469  lueError("`paddi
+0000ebf0: 6e67 6020 6d75 7374 2062 6520 6120 6e6f  ng` must be a no
+0000ec00: 6e2d 6e65 6761 7469 7665 2072 6561 6c20  n-negative real 
+0000ec10: 6e75 6d62 6572 2e22 290a 2020 2020 2020  number.").      
+0000ec20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ec30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ec40: 2e5f 7061 6464 696e 6720 3d20 7061 6464  ._padding = padd
+0000ec50: 696e 670a 2020 2020 2020 2020 656c 7365  ing.        else
+0000ec60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ec70: 6c66 2e5f 7061 6464 696e 6720 3d20 7365  lf._padding = se
+0000ec80: 6c66 2e5f 6765 745f 7061 6464 696e 6728  lf._get_padding(
+0000ec90: 290a 0a20 2020 2020 2020 2023 2033 4420  )..        # 3D 
+0000eca0: 6772 6964 0a20 2020 2020 2020 2069 6620  grid.        if 
+0000ecb0: 7365 6c66 2e76 6572 626f 7365 3a0a 2020  self.verbose:.  
+0000ecc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000ecd0: 223e 2043 616c 6375 6c61 7469 6e67 2033  "> Calculating 3
+0000ece0: 4420 6772 6964 2229 0a20 2020 2020 2020  D grid").       
+0000ecf0: 2073 656c 662e 5f76 6572 7469 6365 7320   self._vertices 
+0000ed00: 3d20 6765 745f 7665 7274 6963 6573 2873  = get_vertices(s
+0000ed10: 656c 662e 6174 6f6d 6963 2c20 7365 6c66  elf.atomic, self
+0000ed20: 2e70 6164 6469 6e67 2c20 7365 6c66 2e73  .padding, self.s
+0000ed30: 7465 7029 0a20 2020 2020 2020 2073 656c  tep).        sel
+0000ed40: 662e 5f64 696d 203d 205f 6765 745f 6469  f._dim = _get_di
+0000ed50: 6d65 6e73 696f 6e73 2873 656c 662e 7665  mensions(self.ve
+0000ed60: 7274 6963 6573 2c20 7365 6c66 2e73 7465  rtices, self.ste
+0000ed70: 7029 0a20 2020 2020 2020 2073 656c 662e  p).        self.
+0000ed80: 5f72 6f74 6174 696f 6e20 3d20 5f67 6574  _rotation = _get
+0000ed90: 5f73 696e 636f 7328 7365 6c66 2e76 6572  _sincos(self.ver
+0000eda0: 7469 6365 7329 0a20 2020 2020 2020 2069  tices).        i
+0000edb0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
+0000edc0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000edd0: 7428 6622 7031 3a20 7b73 656c 662e 7665  t(f"p1: {self.ve
+0000ede0: 7274 6963 6573 5b30 5d7d 2229 0a20 2020  rtices[0]}").   
+0000edf0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0000ee00: 2270 323a 207b 7365 6c66 2e76 6572 7469  "p2: {self.verti
+0000ee10: 6365 735b 315d 7d22 290a 2020 2020 2020  ces[1]}").      
+0000ee20: 2020 2020 2020 7072 696e 7428 6622 7033        print(f"p3
+0000ee30: 3a20 7b73 656c 662e 7665 7274 6963 6573  : {self.vertices
+0000ee40: 5b32 5d7d 2229 0a20 2020 2020 2020 2020  [2]}").         
+0000ee50: 2020 2070 7269 6e74 2866 2270 343a 207b     print(f"p4: {
+0000ee60: 7365 6c66 2e76 6572 7469 6365 735b 335d  self.vertices[3]
+0000ee70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000ee80: 7072 696e 7428 226e 783a 207b 7d2c 206e  print("nx: {}, n
+0000ee90: 793a 207b 7d2c 206e 7a3a 207b 7d22 2e66  y: {}, nz: {}".f
+0000eea0: 6f72 6d61 7428 2a73 656c 662e 6469 6d29  ormat(*self.dim)
+0000eeb0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+0000eec0: 696e 7428 2273 696e 613a 207b 7d2c 2073  int("sina: {}, s
+0000eed0: 696e 623a 207b 7d2c 2063 6f73 613a 207b  inb: {}, cosa: {
+0000eee0: 7d2c 2063 6f73 623a 207b 7d22 2e66 6f72  }, cosb: {}".for
+0000eef0: 6d61 7428 2a73 656c 662e 726f 7461 7469  mat(*self.rotati
+0000ef00: 6f6e 2929 0a0a 2020 2020 6465 6620 5f67  on))..    def _g
+0000ef10: 6574 5f70 6164 6469 6e67 2873 656c 6629  et_padding(self)
+0000ef20: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
+0000ef30: 2020 2022 2222 4175 746f 6d61 7469 6361     """Automatica
+0000ef40: 6c6c 7920 6465 6669 6e65 2074 6865 2070  lly define the p
+0000ef50: 6164 6469 6e67 2062 6173 6564 206f 6e20  adding based on 
+0000ef60: 6d6f 6c65 6375 6c65 2063 6f6f 7264 696e  molecule coordin
+0000ef70: 6174 6573 2c20 7072 6f62 6520 7369 7a65  ates, probe size
+0000ef80: 2c20 6772 6964 2073 7061 6369 6e67 2061  , grid spacing a
+0000ef90: 6e64 2061 746f 6d20 7261 6469 692e 0a0a  nd atom radii...
+0000efa0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000efb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000efc0: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
+0000efd0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+0000efe0: 2020 2020 5468 6520 6c65 6e67 7468 2074      The length t
+0000eff0: 6f20 6164 6420 746f 2065 6163 6820 6469  o add to each di
+0000f000: 7265 6374 696f 6e20 6f66 2074 6865 2033  rection of the 3
+0000f010: 4420 6772 6964 2e0a 2020 2020 2020 2020  D grid..        
+0000f020: 2222 220a 2020 2020 2020 2020 7061 6464  """.        padd
+0000f030: 696e 6720 3d20 312e 3120 2a20 7365 6c66  ing = 1.1 * self
+0000f040: 2e78 797a 725b 3a2c 2033 5d2e 6d61 7828  .xyzr[:, 3].max(
+0000f050: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000f060: 662e 7265 7072 6573 656e 7461 7469 6f6e  f.representation
+0000f070: 2069 6e20 5b22 5345 5322 2c20 2253 4153   in ["SES", "SAS
+0000f080: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000f090: 7061 6464 696e 6720 2b3d 2073 656c 662e  padding += self.
+0000f0a0: 5f70 726f 6265 0a20 2020 2020 2020 2072  _probe.        r
+0000f0b0: 6574 7572 6e20 666c 6f61 7428 7061 6464  eturn float(padd
+0000f0c0: 696e 672e 726f 756e 6428 6465 6369 6d61  ing.round(decima
+0000f0d0: 6c73 3d31 2929 0a0a 2020 2020 6465 6620  ls=1))..    def 
+0000f0e0: 7664 7728 7365 6c66 2c20 7374 6570 3a20  vdw(self, step: 
+0000f0f0: 666c 6f61 7420 3d20 302e 362c 2070 6164  float = 0.6, pad
+0000f100: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b66  ding: Optional[f
+0000f110: 6c6f 6174 5d20 3d20 4e6f 6e65 2920 2d3e  loat] = None) ->
+0000f120: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000f130: 2222 4669 6c6c 2074 6865 2033 4420 6772  ""Fill the 3D gr
+0000f140: 6964 2077 6974 6820 7468 6520 6d6f 6c65  id with the mole
+0000f150: 6375 6c65 2061 7320 7468 6520 7661 6e20  cule as the van 
+0000f160: 6465 7220 5761 616c 7320 7375 7266 6163  der Waals surfac
+0000f170: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
+0000f180: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000f190: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000f1a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000f1b0: 2073 7465 7020 3a20 666c 6f61 742c 206f   step : float, o
+0000f1c0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000f1d0: 2020 2020 4772 6964 2073 7061 6369 6e67      Grid spacing
+0000f1e0: 2028 4129 2c20 6279 2064 6566 6175 6c74   (A), by default
+0000f1f0: 2030 2e36 2e0a 2020 2020 2020 2020 7061   0.6..        pa
+0000f200: 6464 696e 6720 3a20 666c 6f61 742c 206f  dding : float, o
+0000f210: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000f220: 2020 2020 5468 6520 6c65 6e67 7468 2074      The length t
+0000f230: 6f20 6164 6420 746f 2065 6163 6820 6469  o add to each di
+0000f240: 7265 6374 696f 6e20 6f66 2074 6865 2033  rection of the 3
+0000f250: 4420 6772 6964 2c20 6279 2064 6566 6175  D grid, by defau
+0000f260: 6c74 204e 6f6e 652e 2049 6620 4e6f 6e65  lt None. If None
+0000f270: 2c20 6175 746f 6d61 7469 6361 6c6c 7920  , automatically 
+0000f280: 6465 6669 6e65 2074 6865 206c 656e 6774  define the lengt
+0000f290: 6820 6261 7365 6420 6f6e 206d 6f6c 6563  h based on molec
+0000f2a0: 756c 6520 636f 6f72 6469 6e61 7465 732c  ule coordinates,
+0000f2b0: 2070 726f 6265 2073 697a 652c 2067 7269   probe size, gri
+0000f2c0: 6420 7370 6163 696e 6720 616e 6420 6174  d spacing and at
+0000f2d0: 6f6d 2072 6164 6969 2e0a 0a20 2020 2020  om radii...     
+0000f2e0: 2020 2052 6169 7365 730a 2020 2020 2020     Raises.      
+0000f2f0: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
+0000f300: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
+0000f310: 2020 2020 2020 2060 7374 6570 6020 6d75         `step` mu
+0000f320: 7374 2062 6520 6120 706f 7369 7469 7665  st be a positive
+0000f330: 2072 6561 6c20 6e75 6d62 6572 2e0a 2020   real number..  
+0000f340: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+0000f350: 0a20 2020 2020 2020 2020 2020 2060 7374  .            `st
+0000f360: 6570 6020 6d75 7374 2062 6520 6120 706f  ep` must be a po
+0000f370: 7369 7469 7665 2072 6561 6c20 6e75 6d62  sitive real numb
+0000f380: 6572 2e0a 0a20 2020 2020 2020 2045 7861  er...        Exa
+0000f390: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
+0000f3a0: 2d2d 2d2d 0a20 2020 2020 2020 2054 6865  ----.        The
+0000f3b0: 2060 604d 6f6c 6563 756c 652e 7664 7728   ``Molecule.vdw(
+0000f3c0: 2960 6020 6d65 7468 6f64 2074 616b 6573  )`` method takes
+0000f3d0: 2061 2067 7269 6420 7370 6163 696e 6720   a grid spacing 
+0000f3e0: 616e 6420 7265 7475 726e 7320 6120 4e75  and returns a Nu
+0000f3f0: 6d50 7920 6172 7261 7920 7769 7468 2074  mPy array with t
+0000f400: 6865 206d 6f6c 6563 756c 6520 706f 696e  he molecule poin
+0000f410: 7473 2072 6570 7265 7365 6e74 696e 6720  ts representing 
+0000f420: 7468 6520 7664 5720 7375 7266 6163 6520  the vdW surface 
+0000f430: 696e 2074 6865 2033 4420 6772 6964 2e0a  in the 3D grid..
+0000f440: 0a20 2020 2020 2020 203e 3e3e 2023 2047  .        >>> # G
+0000f450: 7269 6420 5370 6163 696e 6720 2873 7465  rid Spacing (ste
+0000f460: 7029 3a20 302e 310a 2020 2020 2020 2020  p): 0.1.        
+0000f470: 3e3e 3e20 7374 6570 203d 2030 2e31 0a20  >>> step = 0.1. 
+0000f480: 2020 2020 2020 203e 3e3e 206d 6f6c 6563         >>> molec
+0000f490: 756c 652e 7664 7728 7374 6570 3d73 7465  ule.vdw(step=ste
+0000f4a0: 7029 0a20 2020 2020 2020 203e 3e3e 206d  p).        >>> m
+0000f4b0: 6f6c 6563 756c 652e 6772 6964 0a20 2020  olecule.grid.   
+0000f4c0: 2020 2020 2061 7272 6179 285b 5b5b 312c       array([[[1,
+0000f4d0: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
+0000f4e0: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
+0000f4f0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+0000f500: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+0000f510: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000f520: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000f530: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+0000f540: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
+0000f550: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
+0000f560: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
+0000f570: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
+0000f580: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+0000f590: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000f5b0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000f5c0: 2031 2c20 315d 5d2c 0a20 2020 2020 2020   1, 1]],.       
+0000f5d0: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
+0000f5e0: 2020 2020 2020 2020 2020 2020 5b5b 312c              [[1,
+0000f5f0: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
+0000f600: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
+0000f610: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+0000f620: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+0000f630: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000f640: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000f650: 2031 2c20 315d 2c0a 2020 2020 2020 2020   1, 1],.        
+0000f660: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
+0000f670: 2020 2020 2020 2020 2020 2020 205b 312c               [1,
+0000f680: 2031 2c20 312c 202e 2e2e 2c20 312c 2031   1, 1, ..., 1, 1
+0000f690: 2c20 315d 2c0a 2020 2020 2020 2020 2020  , 1],.          
+0000f6a0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+0000f6b0: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0000f6d0: 312c 2031 2c20 312c 202e 2e2e 2c20 312c  1, 1, 1, ..., 1,
+0000f6e0: 2031 2c20 315d 5d5d 2c20 6474 7970 653d   1, 1]]], dtype=
+0000f6f0: 696e 7433 3229 0a20 2020 2020 2020 2022  int32).        "
+0000f700: 2222 0a20 2020 2020 2020 2066 726f 6d20  "".        from 
+0000f710: 5f70 794b 5646 696e 6465 7220 696d 706f  _pyKVFinder impo
+0000f720: 7274 205f 6669 6c6c 5f72 6563 6570 746f  rt _fill_recepto
+0000f730: 720a 0a20 2020 2020 2020 2023 2043 6865  r..        # Che
+0000f740: 636b 2061 7267 756d 656e 7473 0a20 2020  ck arguments.   
+0000f750: 2020 2020 2069 6620 7479 7065 2873 7465       if type(ste
+0000f760: 7029 206e 6f74 2069 6e20 5b69 6e74 2c20  p) not in [int, 
+0000f770: 666c 6f61 745d 3a0a 2020 2020 2020 2020  float]:.        
+0000f780: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0000f790: 726f 7228 2260 7374 6570 6020 6d75 7374  ror("`step` must
+0000f7a0: 2062 6520 6120 706f 7374 6976 6520 7265   be a postive re
+0000f7b0: 616c 206e 756d 6265 722e 2229 0a20 2020  al number.").   
+0000f7c0: 2020 2020 2065 6c69 6620 7374 6570 203c       elif step <
+0000f7d0: 3d20 302e 303a 0a20 2020 2020 2020 2020  = 0.0:.         
+0000f7e0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000f7f0: 726f 7228 2260 7374 6570 6020 6d75 7374  ror("`step` must
+0000f800: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
+0000f810: 6561 6c20 6e75 6d62 6572 2e22 290a 2020  eal number.").  
+0000f820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000f830: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
+0000f840: 6570 203d 2073 7465 700a 0a20 2020 2020  ep = step..     
+0000f850: 2020 2023 2041 7474 7269 6275 7465 730a     # Attributes.
+0000f860: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+0000f870: 7072 6573 656e 7461 7469 6f6e 203d 2022  presentation = "
+0000f880: 7664 5722 0a20 2020 2020 2020 2073 656c  vdW".        sel
+0000f890: 662e 5f70 726f 6265 203d 204e 6f6e 650a  f._probe = None.
+0000f8a0: 0a20 2020 2020 2020 2023 2044 6566 696e  .        # Defin
+0000f8b0: 6520 3344 2067 7269 640a 2020 2020 2020  e 3D grid.      
+0000f8c0: 2020 7365 6c66 2e5f 7365 745f 6772 6964    self._set_grid
+0000f8d0: 2870 6164 6469 6e67 290a 0a20 2020 2020  (padding)..     
+0000f8e0: 2020 2023 2076 616e 2064 6572 2057 6161     # van der Waa
+0000f8f0: 6c73 2061 746f 6d73 2028 6861 7264 2073  ls atoms (hard s
+0000f900: 7068 6572 6520 6d6f 6465 6c29 2074 6f20  phere model) to 
+0000f910: 6772 6964 0a20 2020 2020 2020 2069 6620  grid.        if 
+0000f920: 7365 6c66 2e76 6572 626f 7365 3a0a 2020  self.verbose:.  
+0000f930: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000f940: 223e 2049 6e73 6572 7469 6e67 2061 746f  "> Inserting ato
+0000f950: 6d73 2077 6974 6820 7661 6e20 6465 7220  ms with van der 
+0000f960: 5761 616c 7320 7261 6469 6920 696e 746f  Waals radii into
+0000f970: 2033 4420 6772 6964 2229 0a20 2020 2020   3D grid").     
+0000f980: 2020 2073 656c 662e 5f67 7269 6420 3d20     self._grid = 
+0000f990: 5f66 696c 6c5f 7265 6365 7074 6f72 280a  _fill_receptor(.
+0000f9a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f9b0: 2e6e 7820 2a20 7365 6c66 2e6e 7920 2a20  .nx * self.ny * 
+0000f9c0: 7365 6c66 2e6e 7a2c 0a20 2020 2020 2020  self.nz,.       
+0000f9d0: 2020 2020 2073 656c 662e 6e78 2c0a 2020       self.nx,.  
+0000f9e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000f9f0: 792c 0a20 2020 2020 2020 2020 2020 2073  y,.            s
+0000fa00: 656c 662e 6e7a 2c0a 2020 2020 2020 2020  elf.nz,.        
+0000fa10: 2020 2020 7365 6c66 2e78 797a 722c 0a20      self.xyzr,. 
+0000fa20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa30: 7031 2c0a 2020 2020 2020 2020 2020 2020  p1,.            
+0000fa40: 7365 6c66 2e72 6f74 6174 696f 6e2c 0a20  self.rotation,. 
+0000fa50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa60: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+0000fa70: 2020 302e 302c 0a20 2020 2020 2020 2020    0.0,.         
+0000fa80: 2020 2046 616c 7365 2c0a 2020 2020 2020     False,.      
+0000fa90: 2020 2020 2020 7365 6c66 2e6e 7468 7265        self.nthre
+0000faa0: 6164 732c 0a20 2020 2020 2020 2020 2020  ads,.           
+0000fab0: 2073 656c 662e 7665 7262 6f73 652c 0a20   self.verbose,. 
+0000fac0: 2020 2020 2020 2029 2e72 6573 6861 7065         ).reshape
+0000fad0: 2873 656c 662e 6e78 2c20 7365 6c66 2e6e  (self.nx, self.n
+0000fae0: 792c 2073 656c 662e 6e7a 290a 0a20 2020  y, self.nz)..   
+0000faf0: 2064 6566 2073 7572 6661 6365 280a 2020   def surface(.  
+0000fb00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000fb10: 2020 2020 7374 6570 3a20 666c 6f61 7420      step: float 
+0000fb20: 3d20 302e 362c 0a20 2020 2020 2020 2070  = 0.6,.        p
+0000fb30: 726f 6265 3a20 666c 6f61 7420 3d20 312e  robe: float = 1.
+0000fb40: 342c 0a20 2020 2020 2020 2073 7572 6661  4,.        surfa
+0000fb50: 6365 3a20 7374 7220 3d20 2253 4553 222c  ce: str = "SES",
+0000fb60: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+0000fb70: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
+0000fb80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
+0000fb90: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000fba0: 2022 2222 4669 6c6c 2074 6865 2033 4420   """Fill the 3D 
+0000fbb0: 6772 6964 2077 6974 6820 7468 6520 6d6f  grid with the mo
+0000fbc0: 6c65 6375 6c65 2061 7320 7468 6520 7661  lecule as the va
+0000fbd0: 6e20 6465 7220 5761 616c 7320 7375 7266  n der Waals surf
+0000fbe0: 6163 6520 7265 7072 6573 656e 7461 7469  ace representati
+0000fbf0: 6f6e 2e0a 0a20 2020 2020 2020 2050 6172  on...        Par
+0000fc00: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0000fc10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000fc20: 2020 2073 7465 7020 3a20 666c 6f61 742c     step : float,
+0000fc30: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000fc40: 2020 2020 2020 4772 6964 2073 7061 6369        Grid spaci
+0000fc50: 6e67 2028 4129 2c20 6279 2064 6566 6175  ng (A), by defau
+0000fc60: 6c74 2030 2e36 2e0a 2020 2020 2020 2020  lt 0.6..        
+0000fc70: 7072 6f62 6520 3a20 666c 6f61 742c 206f  probe : float, o
+0000fc80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000fc90: 2020 2020 5370 6865 7269 6361 6c20 7072      Spherical pr
+0000fca0: 6f62 6520 7369 7a65 2074 6f20 6465 6669  obe size to defi
+0000fcb0: 6e65 2074 6865 206d 6f6c 6563 756c 6172  ne the molecular
+0000fcc0: 2073 7572 6661 6365 2062 6173 6564 206f   surface based o
+0000fcd0: 6e20 6120 6d6f 6c65 6375 6c61 7220 7265  n a molecular re
+0000fce0: 7072 6573 656e 7461 7469 6f6e 2c20 6279  presentation, by
+0000fcf0: 2064 6566 6175 6c74 2031 2e34 2e0a 2020   default 1.4..  
+0000fd00: 2020 2020 2020 7375 7266 6163 6520 3a20        surface : 
+0000fd10: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+0000fd20: 2020 2020 2020 2020 2020 4d6f 6c65 6375            Molecu
+0000fd30: 6c61 7220 7375 7266 6163 6520 7265 7072  lar surface repr
+0000fd40: 6573 656e 7461 7469 6f6e 2e20 4b65 7977  esentation. Keyw
+0000fd50: 6f72 6473 206f 7074 696f 6e73 2061 7265  ords options are
+0000fd60: 2076 6457 2028 7661 6e20 6465 7220 5761   vdW (van der Wa
+0000fd70: 616c 7320 7375 7266 6163 6529 2c20 5345  als surface), SE
+0000fd80: 5320 2853 6f6c 7665 6e74 2045 7863 6c75  S (Solvent Exclu
+0000fd90: 6465 6420 5375 7266 6163 6529 206f 7220  ded Surface) or 
+0000fda0: 5341 5320 2853 6f6c 7665 6e74 2041 6363  SAS (Solvent Acc
+0000fdb0: 6573 7369 626c 6520 5375 7266 6163 6529  essible Surface)
+0000fdc0: 2c20 6279 2064 6566 6175 6c74 2022 5345  , by default "SE
+0000fdd0: 5322 2e0a 2020 2020 2020 2020 7061 6464  S"..        padd
+0000fde0: 696e 6720 3a20 666c 6f61 742c 206f 7074  ing : float, opt
+0000fdf0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000fe00: 2020 5468 6520 6c65 6e67 7468 2074 6f20    The length to 
+0000fe10: 6164 6420 746f 2065 6163 6820 6469 7265  add to each dire
+0000fe20: 6374 696f 6e20 6f66 2074 6865 2033 4420  ction of the 3D 
+0000fe30: 6772 6964 2c20 6279 2064 6566 6175 6c74  grid, by default
+0000fe40: 204e 6f6e 652e 2049 6620 4e6f 6e65 2c20   None. If None, 
+0000fe50: 6175 746f 6d61 7469 6361 6c6c 7920 6465  automatically de
+0000fe60: 6669 6e65 2074 6865 206c 656e 6774 6820  fine the length 
+0000fe70: 6261 7365 6420 6f6e 206d 6f6c 6563 756c  based on molecul
+0000fe80: 6520 636f 6f72 6469 6e61 7465 732c 2070  e coordinates, p
+0000fe90: 726f 6265 2073 697a 652c 2067 7269 6420  robe size, grid 
+0000fea0: 7370 6163 696e 6720 616e 6420 6174 6f6d  spacing and atom
+0000feb0: 2072 6164 6969 2e0a 0a20 2020 2020 2020   radii...       
+0000fec0: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
+0000fed0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+0000fee0: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
+0000fef0: 2020 2020 2060 7374 6570 6020 6d75 7374       `step` must
+0000ff00: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
+0000ff10: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
+0000ff20: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
+0000ff30: 2020 2020 2020 2020 2020 2060 7374 6570             `step
+0000ff40: 6020 6d75 7374 2062 6520 6120 706f 7369  ` must be a posi
+0000ff50: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
+0000ff60: 2e0a 2020 2020 2020 2020 5479 7065 4572  ..        TypeEr
+0000ff70: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+0000ff80: 6070 726f 6265 5f6f 7574 6020 6d75 7374  `probe_out` must
+0000ff90: 2062 6520 6120 706f 7369 7469 7665 2072   be a positive r
+0000ffa0: 6561 6c20 6e75 6d62 6572 2e0a 2020 2020  eal number..    
+0000ffb0: 2020 2020 5661 6c75 6545 7272 6f72 0a20      ValueError. 
+0000ffc0: 2020 2020 2020 2020 2020 2060 7072 6f62             `prob
+0000ffd0: 655f 6f75 7460 206d 7573 7420 6265 2061  e_out` must be a
+0000ffe0: 2070 6f73 6974 6976 6520 7265 616c 206e   positive real n
+0000fff0: 756d 6265 722e 0a0a 2020 2020 2020 2020  umber...        
+00010000: 4578 616d 706c 650a 2020 2020 2020 2020  Example.        
+00010010: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00010020: 5468 6520 6060 4d6f 6c65 6375 6c65 2e73  The ``Molecule.s
+00010030: 7572 6661 6365 2829 6060 206d 6574 686f  urface()`` metho
+00010040: 6420 7461 6b65 7320 7468 6520 6772 6964  d takes the grid
+00010050: 2073 7061 6369 6e67 2c20 7468 6520 7370   spacing, the sp
+00010060: 6865 7269 6361 6c20 7072 6f62 6520 7369  herical probe si
+00010070: 7a65 2074 6f20 6d6f 6465 6c20 7468 6520  ze to model the 
+00010080: 7375 7266 6163 652c 2074 6865 2073 7572  surface, the sur
+00010090: 6661 6365 2072 6570 7265 7365 6e74 6174  face representat
+000100a0: 696f 6e20 616e 6420 7265 7475 726e 7320  ion and returns 
+000100b0: 6120 4e75 6d50 7920 6172 7261 7920 7769  a NumPy array wi
+000100c0: 7468 2074 6865 206d 6f6c 6563 756c 6520  th the molecule 
+000100d0: 706f 696e 7473 2072 6570 7265 7365 6e74  points represent
+000100e0: 696e 6720 7468 6520 5345 5320 696e 2074  ing the SES in t
+000100f0: 6865 2033 4420 6772 6964 2e0a 0a20 2020  he 3D grid...   
+00010100: 2020 2020 2054 6865 206d 6f6c 6563 756c       The molecul
+00010110: 6172 2073 7572 6661 6365 2063 616e 2062  ar surface can b
+00010120: 6520 6d6f 6465 6c6c 6564 2061 733a 0a0a  e modelled as:..
+00010130: 2020 2020 2020 2020 2020 2020 2a20 536f              * So
+00010140: 6c76 656e 7420 4578 636c 7564 6564 2053  lvent Excluded S
+00010150: 7572 6661 6365 2028 5345 5329 3a0a 0a20  urface (SES):.. 
+00010160: 2020 2020 2020 2020 2020 203e 3e3e 2023             >>> #
+00010170: 2053 7572 6661 6365 2052 6570 7265 7365   Surface Represe
+00010180: 6e74 6174 696f 6e3a 2053 4553 0a20 2020  ntation: SES.   
+00010190: 2020 2020 2020 2020 203e 3e3e 2073 7572           >>> sur
+000101a0: 6661 6365 203d 2027 5345 5327 0a20 2020  face = 'SES'.   
+000101b0: 2020 2020 2020 2020 203e 3e3e 2023 2047           >>> # G
+000101c0: 7269 6420 5370 6163 696e 6720 2873 7465  rid Spacing (ste
+000101d0: 7029 3a20 302e 310a 2020 2020 2020 2020  p): 0.1.        
+000101e0: 2020 2020 3e3e 3e20 7374 6570 203d 2030      >>> step = 0
+000101f0: 2e31 0a20 2020 2020 2020 2020 2020 203e  .1.            >
+00010200: 3e3e 2023 2053 7068 6572 6963 616c 2050  >> # Spherical P
+00010210: 726f 6265 2028 7072 6f62 6529 3a20 312e  robe (probe): 1.
+00010220: 340a 2020 2020 2020 2020 2020 2020 3e3e  4.            >>
+00010230: 3e20 7072 6f62 6520 3d20 312e 340a 2020  > probe = 1.4.  
+00010240: 2020 2020 2020 2020 2020 3e3e 3e20 6d6f            >>> mo
+00010250: 6c65 6375 6c65 2e73 7572 6661 6365 2873  lecule.surface(s
+00010260: 7465 703d 7374 6570 2c20 7072 6f62 653d  tep=step, probe=
+00010270: 7072 6f62 652c 2073 7572 6661 6365 3d73  probe, surface=s
+00010280: 7572 6661 6365 290a 2020 2020 2020 2020  urface).        
+00010290: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
+000102a0: 2e67 7269 640a 2020 2020 2020 2020 2020  .grid.          
+000102b0: 2020 6172 7261 7928 5b5b 5b31 2c20 312c    array([[[1, 1,
+000102c0: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
+000102d0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000102e0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+000102f0: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+00010320: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00010350: 2020 2020 2020 2020 2020 5b31 2c20 312c            [1, 1,
+00010360: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
+00010370: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00010380: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+00010390: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+000103c0: 2e2c 2031 2c20 312c 2031 5d5d 2c0a 2020  ., 1, 1, 1]],.  
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+000103f0: 2020 2020 2020 2020 205b 5b31 2c20 312c           [[1, 1,
+00010400: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
+00010410: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00010420: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+00010430: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010450: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+00010460: 2e2c 2031 2c20 312c 2031 5d2c 0a20 2020  ., 1, 1, 1],.   
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
+00010490: 2020 2020 2020 2020 2020 5b31 2c20 312c            [1, 1,
+000104a0: 2031 2c20 2e2e 2e2c 2031 2c20 312c 2031   1, ..., 1, 1, 1
+000104b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000104c0: 2020 2020 2020 205b 312c 2031 2c20 312c         [1, 1, 1,
+000104d0: 202e 2e2e 2c20 312c 2031 2c20 315d 2c0a   ..., 1, 1, 1],.
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104f0: 2020 2020 5b31 2c20 312c 2031 2c20 2e2e      [1, 1, 1, ..
+00010500: 2e2c 2031 2c20 312c 2031 5d5d 5d2c 2064  ., 1, 1, 1]]], d
+00010510: 7479 7065 3d69 6e74 3332 290a 0a20 2020  type=int32)..   
+00010520: 2020 2020 2054 6865 206d 6f6c 6563 756c       The molecul
+00010530: 6172 2073 7572 6661 6365 2063 616e 2062  ar surface can b
+00010540: 6520 6d6f 6465 6c6c 6564 2061 733a 0a0a  e modelled as:..
+00010550: 2020 2020 2020 2020 2020 2020 2a20 536f              * So
+00010560: 6c76 656e 7420 4163 6365 7373 6962 6c65  lvent Accessible
+00010570: 2053 7572 6661 6365 2028 5341 5329 3a0a   Surface (SAS):.
+00010580: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00010590: 2023 2053 7572 6661 6365 2052 6570 7265   # Surface Repre
+000105a0: 7365 6e74 6174 696f 6e3a 2053 4153 0a20  sentation: SAS. 
+000105b0: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
+000105c0: 7572 6661 6365 203d 2027 5341 5327 0a20  urface = 'SAS'. 
+000105d0: 2020 2020 2020 2020 2020 203e 3e3e 2023             >>> #
+000105e0: 2047 7269 6420 5370 6163 696e 6720 2873   Grid Spacing (s
+000105f0: 7465 7029 3a20 302e 310a 2020 2020 2020  tep): 0.1.      
+00010600: 2020 2020 2020 3e3e 3e20 7374 6570 203d        >>> step =
+00010610: 2030 2e31 0a20 2020 2020 2020 2020 2020   0.1.           
+00010620: 203e 3e3e 2023 2053 7068 6572 6963 616c   >>> # Spherical
+00010630: 2050 726f 6265 2028 7072 6f62 6529 3a20   Probe (probe): 
+00010640: 312e 340a 2020 2020 2020 2020 2020 2020  1.4.            
+00010650: 3e3e 3e20 7072 6f62 6520 3d20 312e 340a  >>> probe = 1.4.
+00010660: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00010670: 6d6f 6c65 6375 6c65 2e73 7572 6661 6365  molecule.surface
+00010680: 2873 7465 703d 7374 6570 2c20 7072 6f62  (step=step, prob
+00010690: 653d 7072 6f62 652c 2073 7572 6661 6365  e=probe, surface
+000106a0: 3d73 7572 6661 6365 290a 2020 2020 2020  =surface).      
+000106b0: 2020 2020 2020 3e3e 3e20 6d6f 6c65 6375        >>> molecu
+000106c0: 6c65 2e67 7269 640a 2020 2020 2020 2020  le.grid.        
+000106d0: 2020 2020 6172 7261 7928 5b5b 5b31 2c20      array([[[1, 
+000106e0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+000106f0: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+00010700: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
+00010710: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
+00010720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010730: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+00010740: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010760: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+00010770: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+00010780: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+00010790: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+000107a0: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
+000107b0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
+000107c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000107d0: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+000107e0: 2e2e 2e2c 2031 2c20 312c 2031 5d5d 2c0a  ..., 1, 1, 1]],.
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010800: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+00010810: 2020 2020 2020 2020 2020 205b 5b31 2c20             [[1, 
+00010820: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+00010830: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+00010840: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
+00010850: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
+00010860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010870: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+00010880: 2e2e 2e2c 2031 2c20 312c 2031 5d2c 0a20  ..., 1, 1, 1],. 
+00010890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108a0: 2020 202e 2e2e 2c0a 2020 2020 2020 2020     ...,.        
+000108b0: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
+000108c0: 312c 2031 2c20 2e2e 2e2c 2031 2c20 312c  1, 1, ..., 1, 1,
+000108d0: 2031 5d2c 0a20 2020 2020 2020 2020 2020   1],.           
+000108e0: 2020 2020 2020 2020 205b 312c 2031 2c20           [1, 1, 
+000108f0: 312c 202e 2e2e 2c20 312c 2031 2c20 315d  1, ..., 1, 1, 1]
+00010900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010910: 2020 2020 2020 5b31 2c20 312c 2031 2c20        [1, 1, 1, 
+00010920: 2e2e 2e2c 2031 2c20 312c 2031 5d5d 5d2c  ..., 1, 1, 1]]],
+00010930: 2064 7479 7065 3d69 6e74 3332 290a 2020   dtype=int32).  
+00010940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010950: 2020 6672 6f6d 205f 7079 4b56 4669 6e64    from _pyKVFind
+00010960: 6572 2069 6d70 6f72 7420 5f66 696c 6c5f  er import _fill_
+00010970: 7265 6365 7074 6f72 0a0a 2020 2020 2020  receptor..      
+00010980: 2020 2320 4368 6563 6b20 6172 6775 6d65    # Check argume
+00010990: 6e74 730a 2020 2020 2020 2020 6966 2074  nts.        if t
+000109a0: 7970 6528 7374 6570 2920 6e6f 7420 696e  ype(step) not in
+000109b0: 205b 696e 742c 2066 6c6f 6174 5d3a 0a20   [int, float]:. 
+000109c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000109d0: 2054 7970 6545 7272 6f72 2822 6073 7465   TypeError("`ste
+000109e0: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
+000109f0: 7469 7665 2072 6561 6c20 6e75 6d62 6572  tive real number
+00010a00: 2e22 290a 2020 2020 2020 2020 656c 6966  .").        elif
+00010a10: 2073 7465 7020 3c3d 2030 2e30 3a0a 2020   step <= 0.0:.  
+00010a20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00010a30: 5661 6c75 6545 7272 6f72 2822 6073 7465  ValueError("`ste
+00010a40: 7060 206d 7573 7420 6265 2061 2070 6f73  p` must be a pos
+00010a50: 6974 6976 6520 7265 616c 206e 756d 6265  itive real numbe
+00010a60: 722e 2229 0a20 2020 2020 2020 2065 6c73  r.").        els
+00010a70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00010a80: 656c 662e 5f73 7465 7020 3d20 7374 6570  elf._step = step
+00010a90: 0a0a 2020 2020 2020 2020 2320 5072 6f62  ..        # Prob
+00010aa0: 650a 2020 2020 2020 2020 6966 2074 7970  e.        if typ
+00010ab0: 6528 7072 6f62 6529 206e 6f74 2069 6e20  e(probe) not in 
+00010ac0: 5b69 6e74 2c20 666c 6f61 742c 206e 756d  [int, float, num
+00010ad0: 7079 2e66 6c6f 6174 3634 5d3a 0a20 2020  py.float64]:.   
+00010ae0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00010af0: 7970 6545 7272 6f72 2822 6070 726f 6265  ypeError("`probe
+00010b00: 5f6f 7574 6020 6d75 7374 2062 6520 6120  _out` must be a 
+00010b10: 6e6f 6e2d 6e65 6761 7469 7665 2072 6561  non-negative rea
+00010b20: 6c20 6e75 6d62 6572 2e22 290a 2020 2020  l number.").    
+00010b30: 2020 2020 656c 6966 2070 726f 6265 203c      elif probe <
+00010b40: 3d20 302e 303a 0a20 2020 2020 2020 2020  = 0.0:.         
+00010b50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010b60: 726f 7228 2260 7072 6f62 655f 6f75 7460  ror("`probe_out`
+00010b70: 206d 7573 7420 6265 2061 206e 6f6e 2d6e   must be a non-n
+00010b80: 6567 6174 6976 6520 7265 616c 206e 756d  egative real num
+00010b90: 6265 722e 2229 0a20 2020 2020 2020 2073  ber.").        s
+00010ba0: 656c 662e 5f70 726f 6265 203d 2070 726f  elf._probe = pro
+00010bb0: 6265 0a0a 2020 2020 2020 2020 2320 5375  be..        # Su
+00010bc0: 7266 6163 650a 2020 2020 2020 2020 6966  rface.        if
+00010bd0: 2073 7572 6661 6365 203d 3d20 2253 4553   surface == "SES
+00010be0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
+00010bf0: 6620 7365 6c66 2e76 6572 626f 7365 3a0a  f self.verbose:.
+00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c10: 7072 696e 7428 223e 2053 7572 6661 6365  print("> Surface
+00010c20: 2072 6570 7265 7365 6e74 6174 696f 6e3a   representation:
+00010c30: 2053 6f6c 7665 6e74 2045 7863 6c75 6465   Solvent Exclude
+00010c40: 6420 5375 7266 6163 6520 2853 4553 292e  d Surface (SES).
+00010c50: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00010c60: 656c 662e 5f72 6570 7265 7365 6e74 6174  elf._representat
+00010c70: 696f 6e20 3d20 7375 7266 6163 650a 2020  ion = surface.  
+00010c80: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
+00010c90: 6520 3d20 5472 7565 0a20 2020 2020 2020  e = True.       
+00010ca0: 2065 6c69 6620 7375 7266 6163 6520 3d3d   elif surface ==
+00010cb0: 2022 5341 5322 3a0a 2020 2020 2020 2020   "SAS":.        
+00010cc0: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
+00010cd0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00010ce0: 2020 2020 2070 7269 6e74 2822 3e20 5375       print("> Su
+00010cf0: 7266 6163 6520 7265 7072 6573 656e 7461  rface representa
+00010d00: 7469 6f6e 3a20 536f 6c76 656e 7420 4163  tion: Solvent Ac
+00010d10: 6365 7373 6962 6c65 2053 7572 6661 6365  cessible Surface
+00010d20: 2028 5341 5329 2e22 290a 2020 2020 2020   (SAS).").      
+00010d30: 2020 2020 2020 7365 6c66 2e5f 7265 7072        self._repr
+00010d40: 6573 656e 7461 7469 6f6e 203d 2073 7572  esentation = sur
+00010d50: 6661 6365 0a20 2020 2020 2020 2020 2020  face.           
+00010d60: 2073 7572 6661 6365 203d 2046 616c 7365   surface = False
+00010d70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00010d80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010d90: 2056 616c 7565 4572 726f 7228 6622 6073   ValueError(f"`s
+00010da0: 7572 6661 6365 6020 6d75 7374 2062 6520  urface` must be 
+00010db0: 5341 5320 6f72 2053 4553 2c20 6e6f 7420  SAS or SES, not 
+00010dc0: 7b73 7572 6661 6365 7d2e 2229 0a0a 2020  {surface}.")..  
+00010dd0: 2020 2020 2020 2320 4465 6669 6e65 2033        # Define 3
+00010de0: 4420 6772 6964 0a20 2020 2020 2020 2073  D grid.        s
+00010df0: 656c 662e 5f73 6574 5f67 7269 6428 7061  elf._set_grid(pa
+00010e00: 6464 696e 6729 0a0a 2020 2020 2020 2020  dding)..        
+00010e10: 2320 4d6f 6c65 6375 6c61 7220 7375 7266  # Molecular surf
+00010e20: 6163 6520 2853 4553 206f 7220 5341 5329  ace (SES or SAS)
+00010e30: 2074 6f20 6772 6964 0a20 2020 2020 2020   to grid.       
+00010e40: 2073 656c 662e 5f67 7269 6420 3d20 5f66   self._grid = _f
+00010e50: 696c 6c5f 7265 6365 7074 6f72 280a 2020  ill_receptor(.  
+00010e60: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00010e70: 7820 2a20 7365 6c66 2e6e 7920 2a20 7365  x * self.ny * se
+00010e80: 6c66 2e6e 7a2c 0a20 2020 2020 2020 2020  lf.nz,.         
+00010e90: 2020 2073 656c 662e 6e78 2c0a 2020 2020     self.nx,.    
+00010ea0: 2020 2020 2020 2020 7365 6c66 2e6e 792c          self.ny,
+00010eb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010ec0: 662e 6e7a 2c0a 2020 2020 2020 2020 2020  f.nz,.          
+00010ed0: 2020 7365 6c66 2e78 797a 722c 0a20 2020    self.xyzr,.   
+00010ee0: 2020 2020 2020 2020 2073 656c 662e 7031           self.p1
+00010ef0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00010f00: 6c66 2e72 6f74 6174 696f 6e2c 0a20 2020  lf.rotation,.   
+00010f10: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00010f20: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
+00010f30: 7365 6c66 2e70 726f 6265 2c0a 2020 2020  self.probe,.    
+00010f40: 2020 2020 2020 2020 7375 7266 6163 652c          surface,
+00010f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010f60: 662e 6e74 6872 6561 6473 2c0a 2020 2020  f.nthreads,.    
+00010f70: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00010f80: 626f 7365 2c0a 2020 2020 2020 2020 292e  bose,.        ).
+00010f90: 7265 7368 6170 6528 7365 6c66 2e6e 782c  reshape(self.nx,
+00010fa0: 2073 656c 662e 6e79 2c20 7365 6c66 2e6e   self.ny, self.n
+00010fb0: 7a29 0a0a 2020 2020 6465 6620 766f 6c75  z)..    def volu
+00010fc0: 6d65 2873 656c 6629 202d 3e20 666c 6f61  me(self) -> floa
+00010fd0: 743a 0a20 2020 2020 2020 2022 2222 4573  t:.        """Es
+00010fe0: 7469 6d61 7465 2074 6865 2076 6f6c 756d  timate the volum
+00010ff0: 6520 6f66 2074 6865 206d 6f6c 6563 756c  e of the molecul
+00011000: 6520 6261 7365 6420 6f6e 2074 6865 206d  e based on the m
+00011010: 6f6c 6563 756c 6172 2073 7572 6661 6365  olecular surface
+00011020: 2072 6570 7265 7365 6e74 6174 696f 6e2c   representation,
+00011030: 2069 652c 2076 6457 2c20 5345 5320 6f72   ie, vdW, SES or
+00011040: 2053 4153 2072 6570 7265 7365 6e74 6174   SAS representat
+00011050: 696f 6e73 2e0a 0a20 2020 2020 2020 2052  ions...        R
+00011060: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00011070: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
+00011080: 6f6c 756d 6520 3a20 666c 6f61 740a 2020  olume : float.  
+00011090: 2020 2020 2020 2020 2020 4d6f 6c65 6375            Molecu
+000110a0: 6c61 7220 766f 6c75 6d65 2028 41c2 b329  lar volume (A..)
+000110b0: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+000110c0: 6c65 0a20 2020 2020 2020 202d 2d2d 2d2d  le.        -----
+000110d0: 2d2d 0a20 2020 2020 2020 2057 6974 6820  --.        With 
+000110e0: 7468 6520 6d6f 6c65 6375 6c61 7220 7375  the molecular su
+000110f0: 7266 6163 6520 6d6f 6465 6c6c 6564 2062  rface modelled b
+00011100: 7920 6060 4d6f 6c65 6375 6c65 2e76 6477  y ``Molecule.vdw
+00011110: 2829 6060 206f 7220 6060 4d6f 6c65 6375  ()`` or ``Molecu
+00011120: 6c65 2e73 7572 6661 6365 2829 6060 2c20  le.surface()``, 
+00011130: 7468 6520 766f 6c75 6d65 2063 616e 2062  the volume can b
+00011140: 6520 6573 7469 6d61 7465 6420 6279 2072  e estimated by r
+00011150: 756e 6e69 6e67 3a0a 0a20 2020 2020 2020  unning:..       
+00011160: 203e 3e3e 206d 6f6c 6563 756c 652e 766f   >>> molecule.vo
+00011170: 6c75 6d65 2829 0a20 2020 2020 2020 2039  lume().        9
+00011180: 302e 380a 2020 2020 2020 2020 2222 220a  0.8.        """.
+00011190: 2020 2020 2020 2020 6672 6f6d 205f 7079          from _py
+000111a0: 4b56 4669 6e64 6572 2069 6d70 6f72 7420  KVFinder import 
+000111b0: 5f76 6f6c 756d 650a 0a20 2020 2020 2020  _volume..       
+000111c0: 2069 6620 7365 6c66 2e67 7269 6420 6973   if self.grid is
+000111d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000111e0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
+000111f0: 5f76 6f6c 756d 6528 0a20 2020 2020 2020  _volume(.       
+00011200: 2020 2020 2020 2020 2028 7365 6c66 2e67           (self.g
+00011210: 7269 6420 3d3d 2030 292e 6173 7479 7065  rid == 0).astype
+00011220: 286e 756d 7079 2e69 6e74 3332 2920 2a20  (numpy.int32) * 
+00011230: 322c 2073 656c 662e 7374 6570 2c20 312c  2, self.step, 1,
+00011240: 2073 656c 662e 6e74 6872 6561 6473 0a20   self.nthreads. 
+00011250: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00011260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011270: 666c 6f61 7428 766f 6c75 6d65 2e72 6f75  float(volume.rou
+00011280: 6e64 2864 6563 696d 616c 733d 3229 290a  nd(decimals=2)).
+00011290: 0a20 2020 2064 6566 2070 7265 7669 6577  .    def preview
+000112a0: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
+000112b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000112c0: 2020 2222 2250 7265 7669 6577 2074 6865    """Preview the
+000112d0: 206d 6f6c 6563 756c 6172 2073 7572 6661   molecular surfa
+000112e0: 6365 2069 6e20 7468 6520 3344 2067 7269  ce in the 3D gri
+000112f0: 642e 0a0a 2020 2020 2020 2020 4578 616d  d...        Exam
+00011300: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
+00011310: 2d2d 2d0a 2020 2020 2020 2020 5769 7468  ---.        With
+00011320: 2074 6865 206d 6f6c 6563 756c 6172 2073   the molecular s
+00011330: 7572 6661 6365 206d 6f64 656c 6c65 6420  urface modelled 
+00011340: 6279 2060 604d 6f6c 6563 756c 652e 7664  by ``Molecule.vd
+00011350: 7728 2960 6020 6f72 2060 604d 6f6c 6563  w()`` or ``Molec
+00011360: 756c 652e 7375 7266 6163 6528 2960 602c  ule.surface()``,
+00011370: 2074 6865 206d 6f64 656c 6c65 6420 6d6f   the modelled mo
+00011380: 6c65 6375 6c65 2069 6e20 7468 6520 3344  lecule in the 3D
+00011390: 2067 7269 6420 6361 6e20 6265 2070 7265   grid can be pre
+000113a0: 7669 6577 6564 2062 7920 7275 6e6e 696e  viewed by runnin
+000113b0: 673a 0a0a 2020 2020 2020 2020 3e3e 3e20  g:..        >>> 
+000113c0: 6d6f 6c65 6375 6c65 2e70 7265 7669 6577  molecule.preview
+000113d0: 2829 0a20 2020 2020 2020 2022 2222 0a20  ().        """. 
+000113e0: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
+000113f0: 7269 6420 6973 206e 6f74 204e 6f6e 653a  rid is not None:
+00011400: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00011410: 6d20 706c 6f74 6c79 2e65 7870 7265 7373  m plotly.express
+00011420: 2069 6d70 6f72 7420 7363 6174 7465 725f   import scatter_
+00011430: 3364 0a0a 2020 2020 2020 2020 2020 2020  3d..            
+00011440: 782c 2079 2c20 7a20 3d20 6e75 6d70 792e  x, y, z = numpy.
+00011450: 6e6f 6e7a 6572 6f28 7365 6c66 2e67 7269  nonzero(self.gri
+00011460: 6420 3d3d 2030 290a 2020 2020 2020 2020  d == 0).        
+00011470: 2020 2020 6669 6720 3d20 7363 6174 7465      fig = scatte
+00011480: 725f 3364 2878 3d78 2c20 793d 792c 207a  r_3d(x=x, y=y, z
+00011490: 3d7a 2c20 2a2a 6b77 6172 6773 290a 2020  =z, **kwargs).  
+000114a0: 2020 2020 2020 2020 2020 6669 672e 7570            fig.up
+000114b0: 6461 7465 5f6c 6179 6f75 7428 0a20 2020  date_layout(.   
+000114c0: 2020 2020 2020 2020 2020 2020 2073 6365               sce
+000114d0: 6e65 5f78 6178 6973 5f73 686f 7774 6963  ne_xaxis_showtic
+000114e0: 6b6c 6162 656c 733d 4661 6c73 652c 0a20  klabels=False,. 
+000114f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011500: 6365 6e65 5f79 6178 6973 5f73 686f 7774  cene_yaxis_showt
+00011510: 6963 6b6c 6162 656c 733d 4661 6c73 652c  icklabels=False,
+00011520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011530: 2073 6365 6e65 5f7a 6178 6973 5f73 686f   scene_zaxis_sho
+00011540: 7774 6963 6b6c 6162 656c 733d 4661 6c73  wticklabels=Fals
+00011550: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+00011560: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+00011570: 2e73 686f 7728 290a 0a20 2020 2064 6566  .show()..    def
+00011580: 2065 7870 6f72 7428 0a20 2020 2020 2020   export(.       
+00011590: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+000115a0: 6e3a 2055 6e69 6f6e 5b73 7472 2c20 7061  n: Union[str, pa
+000115b0: 7468 6c69 622e 5061 7468 5d20 3d20 226d  thlib.Path] = "m
+000115c0: 6f6c 6563 756c 652e 7064 6222 2c0a 2020  olecule.pdb",.  
+000115d0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+000115e0: 2020 2020 2022 2222 4578 706f 7274 206d       """Export m
+000115f0: 6f6c 6563 756c 6520 706f 696e 7473 2028  olecule points (
+00011600: 4829 2074 6f20 6120 5044 422d 666f 726d  H) to a PDB-form
+00011610: 6174 7465 6420 6669 6c65 2e0a 0a20 2020  atted file...   
+00011620: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00011630: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00011640: 2d2d 0a20 2020 2020 2020 2066 6e20 3a20  --.        fn : 
+00011650: 556e 696f 6e5b 7374 722c 2070 6174 686c  Union[str, pathl
+00011660: 6962 2e50 6174 685d 2c20 6f70 7469 6f6e  ib.Path], option
+00011670: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
+00011680: 2066 696c 6520 7061 7468 2074 6f20 7468   file path to th
+00011690: 6520 6d6f 6c65 6375 6c61 7220 766f 6c75  e molecular volu
+000116a0: 6d65 2069 6e20 7468 6520 6772 6964 2d62  me in the grid-b
+000116b0: 6173 6564 2072 6572 7065 7365 6e74 6174  ased rerpesentat
+000116c0: 696f 6e20 696e 2050 4442 2066 6f72 6d61  ion in PDB forma
+000116d0: 742c 2062 7920 6465 6661 756c 7420 226d  t, by default "m
+000116e0: 6f6c 6563 756c 652e 7064 6222 2e0a 0a20  olecule.pdb"... 
+000116f0: 2020 2020 2020 2052 6169 7365 730a 2020         Raises.  
+00011700: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
+00011710: 2020 2020 2054 7970 6545 7272 6f72 0a20       TypeError. 
+00011720: 2020 2020 2020 2020 2020 2060 666e 6020             `fn` 
+00011730: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+00011740: 206f 7220 6120 7061 7468 6c69 622e 5061   or a pathlib.Pa
+00011750: 7468 2e0a 0a20 2020 2020 2020 2045 7861  th...        Exa
+00011760: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
+00011770: 2d2d 2d2d 0a20 2020 2020 2020 2057 6974  ----.        Wit
+00011780: 6820 7468 6520 6d6f 6c65 6375 6c61 7220  h the molecular 
+00011790: 7375 7266 6163 6520 6d6f 6465 6c6c 6564  surface modelled
+000117a0: 2062 7920 6060 4d6f 6c65 6375 6c65 2e76   by ``Molecule.v
+000117b0: 6477 2829 6060 206f 7220 6060 4d6f 6c65  dw()`` or ``Mole
+000117c0: 6375 6c65 2e73 7572 6661 6365 2829 6060  cule.surface()``
+000117d0: 2c20 7468 6520 6d6f 6465 6c6c 6564 206d  , the modelled m
+000117e0: 6f6c 6563 756c 6520 696e 2074 6865 2033  olecule in the 3
+000117f0: 4420 6772 6964 2063 616e 2062 6520 6578  D grid can be ex
+00011800: 706f 7274 6564 2074 6f20 6120 5044 422d  ported to a PDB-
+00011810: 666f 726d 6174 7465 6420 6669 6c65 2062  formatted file b
+00011820: 7920 7275 6e6e 696e 673a 0a0a 2020 2020  y running:..    
+00011830: 2020 2020 3e3e 3e20 6d6f 6c65 6375 6c65      >>> molecule
+00011840: 2e65 7870 6f72 7428 276d 6f64 656c 2e70  .export('model.p
+00011850: 6462 2729 0a20 2020 2020 2020 2022 2222  db').        """
+00011860: 0a20 2020 2020 2020 2023 2046 696c 656e  .        # Filen
+00011870: 616d 6520 2866 6e29 0a20 2020 2020 2020  ame (fn).       
+00011880: 2069 6620 7479 7065 2866 6e29 206e 6f74   if type(fn) not
+00011890: 2069 6e20 5b73 7472 2c20 7061 7468 6c69   in [str, pathli
+000118a0: 622e 5061 7468 5d3a 0a20 2020 2020 2020  b.Path]:.       
+000118b0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+000118c0: 7272 6f72 2822 6066 6e60 206d 7573 7420  rror("`fn` must 
+000118d0: 6265 2061 2073 7472 696e 6720 6f72 2061  be a string or a
+000118e0: 2070 6174 686c 6962 2e50 6174 682e 2229   pathlib.Path.")
+000118f0: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
+00011900: 6469 7273 286f 732e 7061 7468 2e61 6273  dirs(os.path.abs
+00011910: 7061 7468 286f 732e 7061 7468 2e64 6972  path(os.path.dir
+00011920: 6e61 6d65 2866 6e29 292c 2065 7869 7374  name(fn)), exist
+00011930: 5f6f 6b3d 5472 7565 290a 0a20 2020 2020  _ok=True)..     
+00011940: 2020 2023 2053 6176 6520 6772 6964 2074     # Save grid t
+00011950: 6f20 5044 4220 6669 6c65 0a20 2020 2020  o PDB file.     
+00011960: 2020 2065 7870 6f72 7428 0a20 2020 2020     export(.     
+00011970: 2020 2020 2020 2066 6e2c 2028 7365 6c66         fn, (self
+00011980: 2e67 7269 6420 3d3d 2030 292e 6173 7479  .grid == 0).asty
+00011990: 7065 286e 756d 7079 2e69 6e74 3332 2920  pe(numpy.int32) 
+000119a0: 2a20 322c 204e 6f6e 652c 2073 656c 662e  * 2, None, self.
+000119b0: 7665 7274 6963 6573 2c20 7365 6c66 2e73  vertices, self.s
+000119c0: 7465 700a 2020 2020 2020 2020 290a       tep.        ).
```

### Comparing `pyKVFinder-0.5.4/pyKVFinder/utils.py` & `pyKVFinder-0.5.5/pyKVFinder/utils.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.5.4/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.5.5/pyKVFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.5.4/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.5.5/pyKVFinder.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 pyKVFinder.egg-info/entry_points.txt
 pyKVFinder.egg-info/requires.txt
 pyKVFinder.egg-info/top_level.txt
 pyKVFinder/data/EisenbergWeiss.toml
 pyKVFinder/data/HessaHeijne.toml
 pyKVFinder/data/KyteDoolittle.toml
 pyKVFinder/data/MoonFleming.toml
+pyKVFinder/data/RadzickaWolfenden.toml
 pyKVFinder/data/WimleyWhite.toml
 pyKVFinder/data/ZhaoLondon.toml
 pyKVFinder/data/vdw.dat
 pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
 pyKVFinder/data/tests/1FMO.pdb
 pyKVFinder/data/tests/1FMO.xyz
 pyKVFinder/data/tests/ADN.pdb
```

### Comparing `pyKVFinder-0.5.4/pyproject.toml` & `pyKVFinder-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "toml==0.10.2",
-    "numpy==1.24.2",
+    "numpy==1.24.3",
     "matplotlib==3.7.1",
     "plotly==5.14.1",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "black==23.3.0", "flake8==6.0.0"]
```

### Comparing `pyKVFinder-0.5.4/setup.py` & `pyKVFinder-0.5.5/setup.py`

 * *Files identical despite different names*

