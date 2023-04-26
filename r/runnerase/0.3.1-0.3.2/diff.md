# Comparing `tmp/runnerase-0.3.1.tar.gz` & `tmp/runnerase-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runnerase-0.3.1.tar", last modified: Tue Jan 17 17:02:16 2023, max compression
+gzip compressed data, was "runnerase-0.3.2.tar", last modified: Wed Apr 26 07:26:55 2023, max compression
```

## Comparing `runnerase-0.3.1.tar` & `runnerase-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.695064 runnerase-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    34575 2023-01-17 17:01:28.000000 runnerase-0.3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-01-17 17:01:28.000000 runnerase-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2650 2023-01-17 17:02:16.695064 runnerase-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-01-17 17:01:28.000000 runnerase-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-01-17 17:01:28.000000 runnerase-0.3.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.685063 runnerase-0.3.1/runnerase/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21056 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/defaultoptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.689063 runnerase-0.3.1/runnerase/io/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11332 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/io/ase.py
--rw-rw-rw-   0 root         (0) root         (0)     7605 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/io/runnerconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5457 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/io/storageclasses.py
--rw-rw-rw-   0 root         (0) root         (0)    16947 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/io/structuredata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.692064 runnerase-0.3.1/runnerase/plot/
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21605 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/fitresults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.695064 runnerase-0.3.1/runnerase/plot/mpl_styles/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/bar.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/hist.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/line.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/paper.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/presentation.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/mpl_styles/scatterplot.mplstyle
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/scaling.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/sfvalues.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/splittraintest.py
--rw-rw-rw-   0 root         (0) root         (0)     8659 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/symmetryfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/plot/weights.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/singlepoint.py
--rw-rw-rw-   0 root         (0) root         (0)    31095 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/storageclasses.py
--rw-rw-rw-   0 root         (0) root         (0)    28690 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/symmetryfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     4238 2023-01-17 17:01:28.000000 runnerase-0.3.1/runnerase/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 17:02:16.687063 runnerase-0.3.1/runnerase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-01-17 17:02:16.000000 runnerase-0.3.1/runnerase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1089 2023-01-17 17:02:16.000000 runnerase-0.3.1/runnerase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-17 17:02:16.000000 runnerase-0.3.1/runnerase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      276 2023-01-17 17:02:16.000000 runnerase-0.3.1/runnerase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-17 17:02:16.000000 runnerase-0.3.1/runnerase.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-01-17 17:02:16.696064 runnerase-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-01-17 17:01:28.000000 runnerase-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34575 2023-04-26 07:26:07.000000 runnerase-0.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-26 07:26:07.000000 runnerase-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-26 07:26:55.120911 runnerase-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-04-26 07:26:07.000000 runnerase-0.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-04-26 07:26:07.000000 runnerase-0.3.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.110911 runnerase-0.3.2/runnerase/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21056 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/defaultoptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.114911 runnerase-0.3.2/runnerase/io/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/ase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7605 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/runnerconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5457 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/storageclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)    16947 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/io/structuredata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.117911 runnerase-0.3.2/runnerase/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21605 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/fitresults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/runnerase/plot/mpl_styles/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/bar.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/hist.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/line.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/paper.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/presentation.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/mpl_styles/scatterplot.mplstyle
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     6585 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/sfvalues.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/splittraintest.py
+-rw-rw-rw-   0 root         (0) root         (0)     8659 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/symmetryfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/plot/weights.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/singlepoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    31089 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/storageclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)    28833 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/symmetryfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4238 2023-04-26 07:26:07.000000 runnerase-0.3.2/runnerase/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.112911 runnerase-0.3.2/runnerase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      276 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 07:26:55.000000 runnerase-0.3.2/runnerase.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-04-26 07:26:55.121911 runnerase-0.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-04-26 07:26:07.000000 runnerase-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:26:55.120911 runnerase-0.3.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-26 07:26:07.000000 runnerase-0.3.2/tests/test_functional.py
```

### Comparing `runnerase-0.3.1/LICENSE` & `runnerase-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/PKG-INFO` & `runnerase-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runnerase
-Version: 0.3.1
+Version: 0.3.2
 Summary: An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).
 Author-email: Alexander Knoll <alexknoll@mailbox.org>
 Maintainer-email: Alexander Knoll <alexknoll@mailbox.org>
 License: GPLv3+
 Project-URL: Source, https://gitlab.com/runner-suite/runnerase
 Project-URL: Bugs, https://gitlab.com/runner-suite/runnerase/issues
 Project-URL: Documentation, https://runner-suite.gitlab.com/runnerase
```

### Comparing `runnerase-0.3.1/README.md` & `runnerase-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/pyproject.toml` & `runnerase-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'runnerase'
-version = '0.3.1'
+version = '0.3.2'
 description = 'An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).'
 authors = [
     {name='Alexander Knoll', email='alexknoll@mailbox.org'}
 ]
 maintainers = [
     {name='Alexander Knoll', email='alexknoll@mailbox.org'}
 ]
```

### Comparing `runnerase-0.3.1/runnerase/__init__.py` & `runnerase-0.3.2/runnerase/__init__.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/calculator.py` & `runnerase-0.3.2/runnerase/calculator.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/defaultoptions.py` & `runnerase-0.3.2/runnerase/defaultoptions.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/io/ase.py` & `runnerase-0.3.2/runnerase/io/ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,17 @@
     # Read predicted structures from the output.data file.
     # `read` automatically converts all properties to SI units.
     path = f'{directory}/output.data'
     pred_structures = read(path, ':', format='runner')
     energies = np.array([i.get_potential_energy() for i in pred_structures])
     forces = np.array([i.get_forces() for i in pred_structures], dtype='object')
 
-    # For just one structure, flatten the energy and force arrays.
+    # For just one structure, flatten the force arrays.
+    # Cast dtype object back to float, because for one structure the array is
+    # not ragged.
     if forces.shape[0] == 1:
-        forces = forces[0, :, :]
+        forces = forces[0, :, :].astype(float)
 
     if energies.shape[0] == 1:
         return {'energy': float(energies[0]), 'forces': forces}
 
     return {'energy': energies, 'forces': forces}
```

### Comparing `runnerase-0.3.1/runnerase/io/runnerconfig.py` & `runnerase-0.3.2/runnerase/io/runnerconfig.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/io/storageclasses.py` & `runnerase-0.3.2/runnerase/io/storageclasses.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/io/structuredata.py` & `runnerase-0.3.2/runnerase/io/structuredata.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/__init__.py` & `runnerase-0.3.2/runnerase/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/calculator.py` & `runnerase-0.3.2/runnerase/plot/calculator.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/fitresults.py` & `runnerase-0.3.2/runnerase/plot/fitresults.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/mpl_styles/paper.mplstyle` & `runnerase-0.3.2/runnerase/plot/mpl_styles/paper.mplstyle`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/scaling.py` & `runnerase-0.3.2/runnerase/plot/scaling.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/setup.py` & `runnerase-0.3.2/runnerase/plot/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,21 +25,21 @@
                     '#c3b2a2']
 
     # Deep red.
     highlight_color = '#6F1A07'
     black = '#4C4C4C'
 
     # Style attributes for boxplots.
-    boxplot_style: Dict[str, Any] = dict(
-        widths=0.35,
-        medianprops=dict(color=black),
-        patch_artist=True,
-        flierprops=dict(marker='d', markerfacecolor=black,
-                        markersize=4, markeredgecolor=None)
-    )
+    boxplot_style: Dict[str, Any] = {
+        'widths': 0.35,
+        'medianprops': {'color': 'black'},
+        'patch_artist': True,
+        'flierprops': {'marker': 'd', 'markerfacecolor': 'black',
+                       'markersize': 4, 'markeredgecolor': None}
+    }
 
     @property
     def styles(self):
         """Show the list of styles applied to the plot."""
         return self._styles
 
     @styles.setter
```

### Comparing `runnerase-0.3.1/runnerase/plot/sfvalues.py` & `runnerase-0.3.2/runnerase/plot/sfvalues.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/splittraintest.py` & `runnerase-0.3.2/runnerase/plot/splittraintest.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/symmetryfunctions.py` & `runnerase-0.3.2/runnerase/plot/symmetryfunctions.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/plot/weights.py` & `runnerase-0.3.2/runnerase/plot/weights.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/singlepoint.py` & `runnerase-0.3.2/runnerase/singlepoint.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase/storageclasses.py` & `runnerase-0.3.2/runnerase/storageclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         """
         # Obtain the chemical symbol of the element. RuNNer names weights files
         # like `prefix`.{atomic_number}.`suffix`.
         atomic_number = int(infile.name.split('.')[1])
         element = chemical_symbols[atomic_number]
 
         # Store the weights as a np.ndarray.
-        self.data[element] = np.genfromtxt(infile, usecols=(0))  # type: ignore
+        self.data[element] = np.genfromtxt(infile, usecols=0)  # type: ignore
 
     # For some reason pylint thinks that this function has the same signature as
     # ase.io.storageclasses.write_weights.
     # pylint: disable=R0801
     def readall(
         self,
         path: str = '.',
@@ -341,15 +341,15 @@
 
             # Obtain the atomic number of the element and the path to the file.
             number = atomic_numbers[element]
             fullpath = os.path.join(path, f'{prefix}.{number:03d}.{suffix}')
 
             # Store the weights as a np.ndarray.
             self.data[element] = np.genfromtxt(fullpath,
-                                               usecols=(0))  # type: ignore
+                                               usecols=0)  # type: ignore
 
     def write(
         self,
         path: str = '.',
         elements: Optional[List[str]] = None,
         prefix: str = 'weights',
         suffix: str = 'data'
@@ -711,15 +711,15 @@
         if len(force_train) != len(energy_train):
             force_train = [np.nan for i in energy_train]
             force_test = [np.nan for i in energy_test]
 
         # Build the table header.
         colhead_energy = 'RMSE(E) / ' + unit_energy
         colhead_force = 'RMSE(F) / ' + unit_force
-        header = (f"Epoch | {colhead_energy:^18} | {colhead_force:^18} |")
+        header = f"Epoch | {colhead_energy:^18} | {colhead_force:^18} |"
 
         # Build the table subheader.
         subtraintest = f"{'Train':^8} | {'Test':^7}"
         subheader = f"{'':5s} | {subtraintest} | {subtraintest} |"
 
         # Print header, subheader, and their separator lines.
         print(header)
```

### Comparing `runnerase-0.3.1/runnerase/symmetryfunctions.py` & `runnerase-0.3.2/runnerase/symmetryfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from typing import Optional, Dict, List, Union, Tuple, Iterator
 
 from itertools import combinations_with_replacement, product
 
 import numpy as np
 
+from ase.calculators.calculator import CalculatorSetupError
 from ase.geometry import get_distances
 from ase.atoms import Atoms
 from ase.units import Bohr
 
 from runnerase.utils import get_elements
 
 from runnerase.plot import SymmetryFunctionSetPlots
@@ -161,15 +162,15 @@
             tag = 'unknown'
 
         return tag
 
     def to_runner(self, fmt: str = '16.8f') -> str:
         """Convert the symmetry function into RuNNer input.nn format."""
         if self.coefficients is None or self.elements is None:
-            raise Exception('Symmetryfunction is not fully defined yet.')
+            raise CalculatorSetupError('Symmetryfunctions not fully defined.')
 
         centralatom = self.elements[0]
         neighbors = self.elements[1:]
         coefficients = [f'{c:{fmt}}' for c in self.coefficients]
 
         string = f'{centralatom} {self.sftype} ' \
                  + ' '.join(neighbors) \
@@ -382,16 +383,18 @@
         if isinstance(blob, SymmetryFunctionSet):
             self._sets.append(blob)
 
         elif isinstance(blob, SymmetryFunction):
             self._symmetryfunctions.append(blob)
 
         else:
-            raise Exception(f'{self.__class__.__name__} can only store data of'
-                            + 'type SymmetryFunctionSet or SymmetryFunction.')
+            raise CalculatorSetupError(
+                f'{self.__class__.__name__} can only store data of'
+                + 'type SymmetryFunctionSet or SymmetryFunction.'
+            )
 
     def reset(self):
         """Clear all symmetryfunctions and sets from storage."""
         self._sets: List[SymmetryFunctionSet] = []
         self._symmetryfunctions: List[SymmetryFunction] = []
 
     @property
@@ -688,15 +691,17 @@
     """Generate a set of type 3 symmetry functions."""
     if isinstance(eta_angular, SymmetryFunctionSet):
         all_etas: Dict[str, List[float]] = {}
         for symfun in eta_angular:
 
             # Check that the symmetry function has a coefficient.
             if symfun.coefficients is None or symfun.elements is None:
-                raise Exception(f'SymmetryFunction {symfun} is not defined.')
+                raise CalculatorSetupError(
+                    f'SymmetryFunction {symfun} is not defined.'
+                )
 
             label = '-'.join(symfun.elements)
             eta = symfun.coefficients[0]
 
             if label not in all_etas:
                 all_etas[label] = []
             all_etas[label].append(eta)
```

### Comparing `runnerase-0.3.1/runnerase/utils.py` & `runnerase-0.3.2/runnerase/utils.py`

 * *Files identical despite different names*

### Comparing `runnerase-0.3.1/runnerase.egg-info/PKG-INFO` & `runnerase-0.3.2/runnerase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runnerase
-Version: 0.3.1
+Version: 0.3.2
 Summary: An Interface between the Runner Neural Network Energy Representation (RuNNer) and the Atomic Simulation Environment (ASE).
 Author-email: Alexander Knoll <alexknoll@mailbox.org>
 Maintainer-email: Alexander Knoll <alexknoll@mailbox.org>
 License: GPLv3+
 Project-URL: Source, https://gitlab.com/runner-suite/runnerase
 Project-URL: Bugs, https://gitlab.com/runner-suite/runnerase/issues
 Project-URL: Documentation, https://runner-suite.gitlab.com/runnerase
```

### Comparing `runnerase-0.3.1/runnerase.egg-info/SOURCES.txt` & `runnerase-0.3.2/runnerase.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 runnerase/plot/weights.py
 runnerase/plot/mpl_styles/__init__.py
 runnerase/plot/mpl_styles/bar.mplstyle
 runnerase/plot/mpl_styles/hist.mplstyle
 runnerase/plot/mpl_styles/line.mplstyle
 runnerase/plot/mpl_styles/paper.mplstyle
 runnerase/plot/mpl_styles/presentation.mplstyle
-runnerase/plot/mpl_styles/scatterplot.mplstyle
+runnerase/plot/mpl_styles/scatterplot.mplstyle
+tests/test_functional.py
```

