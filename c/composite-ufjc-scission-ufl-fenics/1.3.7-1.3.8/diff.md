# Comparing `tmp/composite_ufjc_scission_ufl_fenics-1.3.7.tar.gz` & `tmp/composite_ufjc_scission_ufl_fenics-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composite_ufjc_scission_ufl_fenics-1.3.7.tar", last modified: Wed Mar 15 16:10:55 2023, max compression
+gzip compressed data, was "composite_ufjc_scission_ufl_fenics-1.3.8.tar", last modified: Tue Apr 25 16:30:17 2023, max compression
```

## Comparing `composite_ufjc_scission_ufl_fenics-1.3.7.tar` & `composite_ufjc_scission_ufl_fenics-1.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-15 16:10:55.930988 composite_ufjc_scission_ufl_fenics-1.3.7/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      805 2023-03-15 15:55:00.000000 composite_ufjc_scission_ufl_fenics-1.3.7/LICENSE
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4676 2023-03-15 16:10:55.930988 composite_ufjc_scission_ufl_fenics-1.3.7/PKG-INFO
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3184 2023-03-15 16:07:07.000000 composite_ufjc_scission_ufl_fenics-1.3.7/README.rst
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-15 16:10:55.930988 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      260 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/__init__.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1863 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/characterizer.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    34791 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/composite_ufjc.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    18738 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/core.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     5658 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/default_parameters.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    12244 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/rate_dependence_scission.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    49041 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/scission_model.py
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3497 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/utility.py
-drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-03-15 16:10:55.930988 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4676 2023-03-15 16:10:55.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/PKG-INFO
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      755 2023-03-15 16:10:55.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/SOURCES.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        1 2023-03-15 16:10:55.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/dependency_links.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      257 2023-03-15 16:10:55.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/requires.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       35 2023-03-15 16:10:55.000000 composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/top_level.txt
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       80 2023-03-15 15:45:35.000000 composite_ufjc_scission_ufl_fenics-1.3.7/pyproject.toml
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1916 2023-03-15 16:10:55.930988 composite_ufjc_scission_ufl_fenics-1.3.7/setup.cfg
--rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       68 2023-03-15 15:45:35.000000 composite_ufjc_scission_ufl_fenics-1.3.7/setup.py
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:30:17.168992 composite_ufjc_scission_ufl_fenics-1.3.8/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      805 2023-03-15 15:55:00.000000 composite_ufjc_scission_ufl_fenics-1.3.8/LICENSE
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4836 2023-04-25 16:30:17.168992 composite_ufjc_scission_ufl_fenics-1.3.8/PKG-INFO
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3317 2023-04-25 16:11:12.000000 composite_ufjc_scission_ufl_fenics-1.3.8/README.rst
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:30:17.168992 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      260 2023-04-22 18:59:18.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/__init__.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1863 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/characterizer.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    20443 2023-04-22 18:48:03.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/composite_ufjc.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    18738 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/core.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1033 2023-04-22 18:59:37.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/default_parameters.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    12244 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/rate_dependence_scission.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)    49041 2023-03-15 15:46:40.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/scission_model.py
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     3544 2023-04-22 19:00:22.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/utility.py
+drwxrwxr-x   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        0 2023-04-25 16:30:17.168992 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     4836 2023-04-25 16:30:17.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/PKG-INFO
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      755 2023-04-25 16:30:17.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)        1 2023-04-25 16:30:17.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)      257 2023-04-25 16:30:17.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/requires.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       35 2023-04-25 16:30:17.000000 composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/top_level.txt
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       80 2023-03-15 15:45:35.000000 composite_ufjc_scission_ufl_fenics-1.3.8/pyproject.toml
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)     1944 2023-04-25 16:30:17.168992 composite_ufjc_scission_ufl_fenics-1.3.8/setup.cfg
+-rw-rw-r--   0 jason_mulderrig  (1000) jason_mulderrig  (1000)       68 2023-03-15 15:45:35.000000 composite_ufjc_scission_ufl_fenics-1.3.8/setup.py
```

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/LICENSE` & `composite_ufjc_scission_ufl_fenics-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/PKG-INFO` & `composite_ufjc_scission_ufl_fenics-1.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: composite_ufjc_scission_ufl_fenics
-Version: 1.3.7
+Version: 1.3.8
 Summary: The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
 Home-page: https://github.com/jasonmulderrig/composite-uFJC-scission-UFL-FEniCS
 Author: Jason Mulderrig, Brandon Talamini, Nikolaos Bouklas
 Author-email: jpm445@cornell.edu, talamini1@llnl.gov, nb589@cornell.edu
 Maintainer: Jason Mulderrig
 Maintainer-email: jpm445@cornell.edu, mulderrig.jason@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
-Keywords: ufjc,diffuse chain scission,asymptotic matching,thermodynamics,statistical mechanics,chain extensibility,polymer chain scission,distorted bond potential,dissipated energy,fracture toughness
+Keywords: ufjc,non-local chain scission,polymer network fracture,asymptotic matching,thermodynamics,statistical mechanics,chain extensibility,polymer chain scission,distorted bond potential,dissipated energy,fracture toughness
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -29,15 +29,15 @@
 
 ##################################
 composite uFJC scission UFL FEniCS
 ##################################
 
 |build| |pyversions| |pypi| |license| |zenodo|
 
-The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
+The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS. This repository is dependent upon the `composite-uFJC-scission <https://pypi.org/project/composite-ufjc-scission/>`_ Python package.
 
 ************
 Installation
 ************
 
 This package can be installed using ``pip`` via the `Python Package Index <https://pypi.org/project/composite-ufjc-scission-ufl-fenics/>`_ (PyPI),
```

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/README.rst` & `composite_ufjc_scission_ufl_fenics-1.3.8/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##################################
 composite uFJC scission UFL FEniCS
 ##################################
 
 |build| |pyversions| |pypi| |license| |zenodo|
 
-The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
+The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS. This repository is dependent upon the `composite-uFJC-scission <https://pypi.org/project/composite-ufjc-scission/>`_ Python package.
 
 ************
 Installation
 ************
 
 This package can be installed using ``pip`` via the `Python Package Index <https://pypi.org/project/composite-ufjc-scission-ufl-fenics/>`_ (PyPI),
```

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/characterizer.py` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/characterizer.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/core.py` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/core.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/rate_dependence_scission.py` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/rate_dependence_scission.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/scission_model.py` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/scission_model.py`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics/utility.py` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The utilities module for the composite uFJC scission model
 implemented in the Unified Form Language (UFL) for FEniCS.
 """
 
 # import necessary libraries
 from __future__ import division
+from dolfin import *
 import os
 import pathlib
 import pickle
 import matplotlib.pyplot as plt
 
 
 def generate_savedir(namedir):
@@ -53,31 +54,30 @@
 
 def latex_formatting_figure(post_processing_parameters):
     """matplotlib plot formatting settings, with LaTeX.
     
     This function accepts pre-defined post-processing parameters and
     sets various matplotlib plot formatting settings accordingly.
     """
-
     ppp = post_processing_parameters
 
     # LaTeX plot formatting settings
-    plt.rcParams['axes.linewidth'] = ppp.axes_linewidth
-    plt.rcParams['font.family']    = ppp.font_family
+    plt.rcParams['axes.linewidth'] = ppp["axes_linewidth"]
+    plt.rcParams['font.family']    = ppp["font_family"]
     # comment the line below out in WSL2, uncomment the line below in
     # native Linux on workstation
-    plt.rcParams['text.usetex'] = ppp.text_usetex
+    plt.rcParams['text.usetex']    = ppp["text_usetex"]
     
     # plot axis tick settings
-    plt.rcParams['ytick.right']     = ppp.ytick_right
-    plt.rcParams['ytick.direction'] = ppp.ytick_direction
-    plt.rcParams['xtick.top']       = ppp.xtick_top
-    plt.rcParams['xtick.direction'] = ppp.xtick_direction
+    plt.rcParams['ytick.right']     = ppp["ytick_right"]
+    plt.rcParams['ytick.direction'] = ppp["ytick_direction"]
+    plt.rcParams['xtick.top']       = ppp["xtick_top"]
+    plt.rcParams['xtick.direction'] = ppp["xtick_direction"]
     
-    plt.rcParams["xtick.minor.visible"] = ppp.xtick_minor_visible
+    plt.rcParams["xtick.minor.visible"] = ppp["xtick_minor_visible"]
 
 def save_current_figure(
         savedir, xlabel, xlabelfontsize, ylabel, ylabelfontsize, name):
     """Save matplotlib plot figure with labels.
     
     This function saves the current matplotlib plot figure with
     specified axis labels and axis label fontsize.
```

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/PKG-INFO` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: composite-ufjc-scission-ufl-fenics
-Version: 1.3.7
+Version: 1.3.8
 Summary: The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
 Home-page: https://github.com/jasonmulderrig/composite-uFJC-scission-UFL-FEniCS
 Author: Jason Mulderrig, Brandon Talamini, Nikolaos Bouklas
 Author-email: jpm445@cornell.edu, talamini1@llnl.gov, nb589@cornell.edu
 Maintainer: Jason Mulderrig
 Maintainer-email: jpm445@cornell.edu, mulderrig.jason@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
-Keywords: ufjc,diffuse chain scission,asymptotic matching,thermodynamics,statistical mechanics,chain extensibility,polymer chain scission,distorted bond potential,dissipated energy,fracture toughness
+Keywords: ufjc,non-local chain scission,polymer network fracture,asymptotic matching,thermodynamics,statistical mechanics,chain extensibility,polymer chain scission,distorted bond potential,dissipated energy,fracture toughness
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -29,15 +29,15 @@
 
 ##################################
 composite uFJC scission UFL FEniCS
 ##################################
 
 |build| |pyversions| |pypi| |license| |zenodo|
 
-The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
+The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS. This repository is dependent upon the `composite-uFJC-scission <https://pypi.org/project/composite-ufjc-scission/>`_ Python package.
 
 ************
 Installation
 ************
 
 This package can be installed using ``pip`` via the `Python Package Index <https://pypi.org/project/composite-ufjc-scission-ufl-fenics/>`_ (PyPI),
```

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/composite_ufjc_scission_ufl_fenics.egg-info/SOURCES.txt` & `composite_ufjc_scission_ufl_fenics-1.3.8/composite_ufjc_scission_ufl_fenics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composite_ufjc_scission_ufl_fenics-1.3.7/setup.cfg` & `composite_ufjc_scission_ufl_fenics-1.3.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 license = GNU General Public License v3 or later (GPLv3+)
 license_files = 
 	LICENSE
 description = The Python package for the composite uFJC model with scission implemented in the Unified Form Language (UFL) for FEniCS.
 long_description = file: README.rst
-keywords = ufjc, diffuse chain scission, asymptotic matching, thermodynamics, statistical mechanics, chain extensibility, polymer chain scission, distorted bond potential, dissipated energy, fracture toughness
+keywords = ufjc, non-local chain scission, polymer network fracture, asymptotic matching, thermodynamics, statistical mechanics, chain extensibility, polymer chain scission, distorted bond potential, dissipated energy, fracture toughness
 
 [options]
 packages = find:
 python_requires = >=3.5, <4
 install_requires = 
 	numpy==1.21.6
 	fenics-fiat==2019.1.0
 	fenics-dijitso==2019.1.0
 	fenics-ufl==2019.1.0
 	fenics-ffc==2019.1.0
 	fenics-dolfin==2019.1.0
 	mshr==2019.1.0
-	composite-ufjc-scission==1.3.7
+	composite-ufjc-scission==1.3.8
 
 [options.extras_require]
 plotting = matplotlib
 meshing = 
 	gmsh
 	meshio
 	pygmsh
```

