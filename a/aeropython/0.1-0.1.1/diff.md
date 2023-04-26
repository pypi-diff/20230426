# Comparing `tmp/aeropython-0.1.tar.gz` & `tmp/aeropython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeropython-0.1.tar", last modified: Mon Apr 24 18:40:18 2023, max compression
+gzip compressed data, was "aeropython-0.1.1.tar", last modified: Tue Apr 25 17:15:51 2023, max compression
```

## Comparing `aeropython-0.1.tar` & `aeropython-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.204904 aeropython-0.1/
--rw-rw-rw-   0        0        0     1074 2023-04-24 18:25:51.000000 aeropython-0.1/LICENSE
--rw-rw-rw-   0        0        0      234 2023-04-24 18:40:18.204904 aeropython-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-04-24 18:25:51.000000 aeropython-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.059332 aeropython-0.1/aeropython/
--rw-rw-rw-   0        0        0     7608 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/AeroPy.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.095138 aeropython-0.1/aeropython/CST_2D/
--rw-rw-rw-   0        0        0       20 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_2D/__init__.py
--rw-rw-rw-   0        0        0    11858 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_2D/core.py
--rw-rw-rw-   0        0        0    17541 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_2D/fitting.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.109419 aeropython-0.1/aeropython/CST_3D/
--rw-rw-rw-   0        0        0       77 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_3D/__init__.py
--rw-rw-rw-   0        0        0    10031 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_3D/core.py
--rw-rw-rw-   0        0        0    12794 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/CST_3D/mesh_tools.py
--rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/__init__.py
--rw-rw-rw-   0        0        0    19701 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/aero_module.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.130702 aeropython-0.1/aeropython/filehandling/
--rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/filehandling/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/filehandling/extract_slices.py
--rw-rw-rw-   0        0        0     1400 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/filehandling/paraview_tools.py
--rw-rw-rw-   0        0        0     8196 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/filehandling/stl_processing.py
--rw-rw-rw-   0        0        0     2652 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/filehandling/vtk.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.168728 aeropython-0.1/aeropython/geometry/
--rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/__init__.py
--rw-rw-rw-   0        0        0    49176 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/airfoil.py
--rw-rw-rw-   0        0        0     4127 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/fitting.py
--rw-rw-rw-   0        0        0     3366 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/frame.py
--rw-rw-rw-   0        0        0    11986 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/parametric.py
--rw-rw-rw-   0        0        0     2401 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/test_inflections.py
--rw-rw-rw-   0        0        0     1789 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/geometry/wing.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.184769 aeropython-0.1/aeropython/morphing/
--rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/morphing/__init__.py
--rw-rw-rw-   0        0        0    14358 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/morphing/camber_2D.py
--rw-rw-rw-   0        0        0     8622 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/morphing/camber_3D.py
--rw-rw-rw-   0        0        0    16426 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/morphing/twist_3D.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.200895 aeropython-0.1/aeropython/structural/
--rw-rw-rw-   0        0        0     4966 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/structural/beam.py
--rw-rw-rw-   0        0        0     9643 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/structural/shell.py
--rw-rw-rw-   0        0        0    14534 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/structural/stable_solution.py
--rw-rw-rw-   0        0        0    42430 2023-04-24 18:25:51.000000 aeropython-0.1/aeropython/xfoil_module.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:40:18.080006 aeropython-0.1/aeropython.egg-info/
--rw-rw-rw-   0        0        0      234 2023-04-24 18:40:17.000000 aeropython-0.1/aeropython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2023-04-24 18:40:17.000000 aeropython-0.1/aeropython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:40:17.000000 aeropython-0.1/aeropython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 18:40:17.000000 aeropython-0.1/aeropython.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-24 18:40:17.000000 aeropython-0.1/aeropython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-24 18:40:18.207945 aeropython-0.1/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-04-24 18:40:14.000000 aeropython-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.638792 aeropython-0.1.1/
+-rw-rw-rw-   0        0        0     1074 2023-04-24 18:25:51.000000 aeropython-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      236 2023-04-25 17:15:51.638792 aeropython-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-04-24 18:25:51.000000 aeropython-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.497295 aeropython-0.1.1/aeropython/
+-rw-rw-rw-   0        0        0     7608 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/AeroPy.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.536119 aeropython-0.1.1/aeropython/CST_2D/
+-rw-rw-rw-   0        0        0       20 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_2D/__init__.py
+-rw-rw-rw-   0        0        0    11858 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_2D/core.py
+-rw-rw-rw-   0        0        0    17541 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_2D/fitting.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.544634 aeropython-0.1.1/aeropython/CST_3D/
+-rw-rw-rw-   0        0        0       77 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_3D/__init__.py
+-rw-rw-rw-   0        0        0    10031 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_3D/core.py
+-rw-rw-rw-   0        0        0    12794 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/CST_3D/mesh_tools.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/__init__.py
+-rw-rw-rw-   0        0        0    19701 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/aero_module.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.560270 aeropython-0.1.1/aeropython/filehandling/
+-rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/filehandling/__init__.py
+-rw-rw-rw-   0        0        0     2622 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/filehandling/extract_slices.py
+-rw-rw-rw-   0        0        0     1400 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/filehandling/paraview_tools.py
+-rw-rw-rw-   0        0        0     8196 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/filehandling/stl_processing.py
+-rw-rw-rw-   0        0        0     2652 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/filehandling/vtk.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.607147 aeropython-0.1.1/aeropython/geometry/
+-rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/__init__.py
+-rw-rw-rw-   0        0        0    49176 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/airfoil.py
+-rw-rw-rw-   0        0        0     4127 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/fitting.py
+-rw-rw-rw-   0        0        0     3366 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/frame.py
+-rw-rw-rw-   0        0        0    11986 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/parametric.py
+-rw-rw-rw-   0        0        0     2401 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/test_inflections.py
+-rw-rw-rw-   0        0        0     1789 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/geometry/wing.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.622770 aeropython-0.1.1/aeropython/morphing/
+-rw-rw-rw-   0        0        0        0 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/morphing/__init__.py
+-rw-rw-rw-   0        0        0    14358 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/morphing/camber_2D.py
+-rw-rw-rw-   0        0        0     8622 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/morphing/camber_3D.py
+-rw-rw-rw-   0        0        0    16426 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/morphing/twist_3D.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.636282 aeropython-0.1.1/aeropython/structural/
+-rw-rw-rw-   0        0        0     4966 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/structural/beam.py
+-rw-rw-rw-   0        0        0     9643 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/structural/shell.py
+-rw-rw-rw-   0        0        0    14534 2023-04-24 18:25:51.000000 aeropython-0.1.1/aeropython/structural/stable_solution.py
+-rw-rw-rw-   0        0        0    42181 2023-04-25 16:42:50.000000 aeropython-0.1.1/aeropython/xfoil_module.py
+drwxrwxrwx   0        0        0        0 2023-04-25 17:15:51.512916 aeropython-0.1.1/aeropython.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-25 17:15:51.000000 aeropython-0.1.1/aeropython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2023-04-25 17:15:51.000000 aeropython-0.1.1/aeropython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 17:15:51.000000 aeropython-0.1.1/aeropython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 18:40:17.000000 aeropython-0.1.1/aeropython.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-25 17:15:51.000000 aeropython-0.1.1/aeropython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-25 17:15:51.638792 aeropython-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-04-25 17:15:39.000000 aeropython-0.1.1/setup.py
```

### Comparing `aeropython-0.1/LICENSE` & `aeropython-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/README.md` & `aeropython-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/AeroPy.py` & `aeropython-0.1.1/aeropython/AeroPy.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/CST_2D/core.py` & `aeropython-0.1.1/aeropython/CST_2D/core.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/CST_2D/fitting.py` & `aeropython-0.1.1/aeropython/CST_2D/fitting.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/CST_3D/core.py` & `aeropython-0.1.1/aeropython/CST_3D/core.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/CST_3D/mesh_tools.py` & `aeropython-0.1.1/aeropython/CST_3D/mesh_tools.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/aero_module.py` & `aeropython-0.1.1/aeropython/aero_module.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/filehandling/extract_slices.py` & `aeropython-0.1.1/aeropython/filehandling/extract_slices.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/filehandling/paraview_tools.py` & `aeropython-0.1.1/aeropython/filehandling/paraview_tools.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/filehandling/stl_processing.py` & `aeropython-0.1.1/aeropython/filehandling/stl_processing.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/filehandling/vtk.py` & `aeropython-0.1.1/aeropython/filehandling/vtk.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/airfoil.py` & `aeropython-0.1.1/aeropython/geometry/airfoil.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/fitting.py` & `aeropython-0.1.1/aeropython/geometry/fitting.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/frame.py` & `aeropython-0.1.1/aeropython/geometry/frame.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/parametric.py` & `aeropython-0.1.1/aeropython/geometry/parametric.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/test_inflections.py` & `aeropython-0.1.1/aeropython/geometry/test_inflections.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/geometry/wing.py` & `aeropython-0.1.1/aeropython/geometry/wing.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/morphing/camber_2D.py` & `aeropython-0.1.1/aeropython/morphing/camber_2D.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/morphing/camber_3D.py` & `aeropython-0.1.1/aeropython/morphing/camber_3D.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/morphing/twist_3D.py` & `aeropython-0.1.1/aeropython/morphing/twist_3D.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/structural/beam.py` & `aeropython-0.1.1/aeropython/structural/beam.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/structural/shell.py` & `aeropython-0.1.1/aeropython/structural/shell.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/structural/stable_solution.py` & `aeropython-0.1.1/aeropython/structural/stable_solution.py`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/aeropython/xfoil_module.py` & `aeropython-0.1.1/aeropython/xfoil_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,22 +330,17 @@
                 pass
 
             issueCmd('%s%s' % (dir, filename))
             issueCmd('')
 
         # For several angles of attack
         if Multiple is True:
-            if output == "Polar":
-                issueCmd('aseq')
-                issueCmd('{}'.format(min(alfas)))
-                issueCmd('{}'.format(max(alfas)))
-                issueCmd('{}'.format(alfas[1]-alfas[0]))
-            else:
-                for alfa in alfas:
-                    submit(output, alfa)
+            for alfa in alfas:
+                submit(output, alfa)
+
 
         # For only one angle of attack
         if Multiple is False:
             submit(output, alfas)
 
         # Exiting
         # From OPER mode
```

### Comparing `aeropython-0.1/aeropython.egg-info/SOURCES.txt` & `aeropython-0.1.1/aeropython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeropython-0.1/setup.py` & `aeropython-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """AeroPython: An easy to use aerodynamic tool."""
 
 from setuptools import setup, find_packages
 
 setup(name='aeropython',
-      version='0.1',
+      version='0.1.1',
       description='An easy to use aerodynamic tool.',
       author='leal26',
       author_email='leal26@tamu.edu',
       url = 'https://github.com/koentjess/AeroPython',
       license='MIT',
       packages=['aeropython', 'aeropython.CST_2D', 'aeropython.CST_3D',
                 'aeropython.morphing', 'aeropython.geometry',
```

