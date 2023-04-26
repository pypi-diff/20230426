# Comparing `tmp/CLUEstering-1.2.0.tar.gz` & `tmp/CLUEstering-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CLUEstering-1.2.0.tar", last modified: Thu Oct 13 06:10:49 2022, max compression
+gzip compressed data, was "CLUEstering-1.4.0.tar", last modified: Tue Apr 25 15:45:28 2023, max compression
```

## Comparing `CLUEstering-1.2.0.tar` & `CLUEstering-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.010830 CLUEstering-1.2.0/
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/CLUEstering/
--rw-r--r--   0 simone    (1000) simone    (1000)     8723 2022-09-26 13:50:03.000000 CLUEstering-1.2.0/CLUEstering/CLUEstering.py
--rw-r--r--   0 simone    (1000) simone    (1000)       93 2022-09-26 13:50:03.000000 CLUEstering-1.2.0/CLUEstering/__init__.py
--rw-r--r--   0 simone    (1000) simone    (1000)    17978 2022-10-13 06:05:47.000000 CLUEstering-1.2.0/CLUEstering/binding.cc
-drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/CLUEstering.egg-info/
--rw-r--r--   0 simone    (1000) simone    (1000)     3338 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/PKG-INFO
--rw-r--r--   0 simone    (1000) simone    (1000)      289 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/SOURCES.txt
--rw-r--r--   0 simone    (1000) simone    (1000)        1 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/dependency_links.txt
--rw-r--r--   0 simone    (1000) simone    (1000)       32 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/requires.txt
--rw-r--r--   0 simone    (1000) simone    (1000)       27 2022-10-13 06:10:48.000000 CLUEstering-1.2.0/CLUEstering.egg-info/top_level.txt
--rw-r--r--   0 simone    (1000) simone    (1000)    35149 2022-09-26 08:10:11.000000 CLUEstering-1.2.0/LICENSE
--rw-r--r--   0 simone    (1000) simone    (1000)     3338 2022-10-13 06:10:49.007497 CLUEstering-1.2.0/PKG-INFO
--rw-r--r--   0 simone    (1000) simone    (1000)     2772 2022-09-29 11:42:33.000000 CLUEstering-1.2.0/README.md
--rw-r--r--   0 simone    (1000) simone    (1000)      114 2022-09-26 14:23:51.000000 CLUEstering-1.2.0/pyproject.toml
--rw-r--r--   0 simone    (1000) simone    (1000)       38 2022-10-13 06:10:49.010830 CLUEstering-1.2.0/setup.cfg
--rw-r--r--   0 simone    (1000) simone    (1000)     1093 2022-10-13 06:06:17.000000 CLUEstering-1.2.0/setup.py
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.718152 CLUEstering-1.4.0/
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.714819 CLUEstering-1.4.0/CLUEstering/
+-rw-r--r--   0 simone    (1000) simone    (1000)    33042 2023-04-25 15:14:35.000000 CLUEstering-1.4.0/CLUEstering/CLUEstering.py
+-rw-r--r--   0 simone    (1000) simone    (1000)       94 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/__init__.py
+-rw-r--r--   0 simone    (1000) simone    (1000)     9475 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/binding.cc
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.714819 CLUEstering-1.4.0/CLUEstering/include/
+-rw-r--r--   0 simone    (1000) simone    (1000)     9638 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/Clustering.h
+-rw-r--r--   0 simone    (1000) simone    (1000)     1837 2023-04-18 13:46:58.000000 CLUEstering-1.4.0/CLUEstering/include/Kernels.h
+-rw-r--r--   0 simone    (1000) simone    (1000)      793 2023-04-18 13:46:58.000000 CLUEstering-1.4.0/CLUEstering/include/Point.h
+-rw-r--r--   0 simone    (1000) simone    (1000)     2864 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/Tiles.h
+-rw-r--r--   0 simone    (1000) simone    (1000)      191 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/deltaPhi.h
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.718152 CLUEstering-1.4.0/CLUEstering/include/test/
+-rw-r--r--   0 simone    (1000) simone    (1000)   321644 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/test/doctest.h
+-rw-r--r--   0 simone    (1000) simone    (1000)     1307 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/test/test_deltaphi.cc
+-rw-r--r--   0 simone    (1000) simone    (1000)     1680 2023-04-21 13:43:08.000000 CLUEstering-1.4.0/CLUEstering/include/test/test_distance.cc
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.714819 CLUEstering-1.4.0/CLUEstering.egg-info/
+-rw-r--r--   0 simone    (1000) simone    (1000)     4041 2023-04-25 15:45:28.000000 CLUEstering-1.4.0/CLUEstering.egg-info/PKG-INFO
+-rw-r--r--   0 simone    (1000) simone    (1000)      647 2023-04-25 15:45:28.000000 CLUEstering-1.4.0/CLUEstering.egg-info/SOURCES.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)        1 2023-04-25 15:45:28.000000 CLUEstering-1.4.0/CLUEstering.egg-info/dependency_links.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)       37 2023-04-25 15:45:28.000000 CLUEstering-1.4.0/CLUEstering.egg-info/requires.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)       27 2023-04-25 15:45:28.000000 CLUEstering-1.4.0/CLUEstering.egg-info/top_level.txt
+-rw-r--r--   0 simone    (1000) simone    (1000)    35149 2022-09-26 08:10:11.000000 CLUEstering-1.4.0/LICENSE
+-rw-r--r--   0 simone    (1000) simone    (1000)       26 2023-04-25 15:45:23.000000 CLUEstering-1.4.0/MANIFEST.in
+-rw-r--r--   0 simone    (1000) simone    (1000)     4041 2023-04-25 15:45:28.718152 CLUEstering-1.4.0/PKG-INFO
+-rw-r--r--   0 simone    (1000) simone    (1000)     3499 2023-04-25 15:04:50.000000 CLUEstering-1.4.0/README.md
+-rw-r--r--   0 simone    (1000) simone    (1000)      114 2023-04-25 15:17:55.000000 CLUEstering-1.4.0/pyproject.toml
+-rw-r--r--   0 simone    (1000) simone    (1000)       38 2023-04-25 15:45:28.718152 CLUEstering-1.4.0/setup.cfg
+-rw-r--r--   0 simone    (1000) simone    (1000)     1130 2023-04-25 15:41:15.000000 CLUEstering-1.4.0/setup.py
+drwxr-xr-x   0 simone    (1000) simone    (1000)        0 2023-04-25 15:45:28.718152 CLUEstering-1.4.0/tests/
+-rw-r--r--   0 simone    (1000) simone    (1000)      286 2023-04-25 15:31:02.000000 CLUEstering-1.4.0/tests/test_blob.py
+-rw-r--r--   0 simone    (1000) simone    (1000)     3202 2023-04-25 15:31:53.000000 CLUEstering-1.4.0/tests/test_input_datatypes.py
+-rw-r--r--   0 simone    (1000) simone    (1000)       26 2023-04-25 15:10:33.000000 CLUEstering-1.4.0/tests/test_output_passed.py
```

### Comparing `CLUEstering-1.2.0/CLUEstering.egg-info/PKG-INFO` & `CLUEstering-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: CLUEstering
-Version: 1.2.0
-Summary: A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.
-Author: Simone Balducci
-Author-email: simone.balducci00@gmail.com
-Keywords: Python,Clustering,Binding
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLUEstering 
 The CLUE algorithm is a clustering algorithm written at CERN.
 
 The original algorithm was designed to work in 2 dimensions, with the data distributed in parallel layers.
 Unlike other clustering algorithms, CLUE takes the coordinates of the points and also their weight, which represents their energy, and calculater the energy density of each point.
 This energy density is used to find the seeds for each cluster, their followers and the outliers, which are dismissed as noise.
 CLUE takes 4 parameters in input: 
@@ -33,27 +17,29 @@
 </p>
 
 The C++ code is binded using PyBind11, and the module is created locally during the installation of the library.
 
 In this library is defined the clusterer class. The constructor takes the four parameters, dc_, rhoc, outlierDeltaFactor and pPBin. Passing pPBin is optional since by default it is initialized to 10.
 
 The class has several methods:
-* readData, which takes the data in input and inizializes the class members. The data can be in the form of lists, numpy arrays, string containing the path to a csv file or pandas DataFrame;
-* runCLUE, which takes no parameters and runs the CLUE algorithm;
-* inputPlotter, which takes no parameters and plots the data in input;
-* clusterPlotter, which takes no parameters and plots the data using a different colour for each cluster. The seeds are indicated by stars and the outliers by small grey crosses.
-* toCSV, which takes two strings, the first containing the path to a folder and the second containing the desired name for the csv file (also with the .csv suffix) and produces the csv file containing the cluster informations.
+* read_data, which takes the data in input and inizializes the class members. The data can be in the form of list, numpy array, dictionary, string containing the path to a csv file or pandas DataFrame;
+* change_coordinates, which allows to change the coordinate system used for clustering;
+* choose_kernel, which allows to change the convolution kernel used when calculating the local density of each point. The default kernel is a flat kernel with parameter `0.5`, but it can be changed to an exponential or gaussian kernel, or a custom kernel, which is user defined and can be any continuous function;
+* run_clue, which takes no parameters and runs the CLUE algorithm;
+* input_plotter, which plots all the points in input. This method is useful for getting an idea of the shape of the dataset before clustering. In addition to some plot customizations (like the colour or the size of the points, the addition of a grid, the axis labels and so on) it's also possible to pass the functions for the change of coordinates and change the coordinate system used for plotting.
+* cluster_plotter, which plots the data using a different colour for each cluster. The seeds are indicated by stars and the outliers by small grey crosses.
+* to_csv, which takes two strings, the first containing the path to a folder and the second containing the desired name for the csv file (also with the .csv suffix) and produces the csv file containing the cluster informations.
 
-Outside of the class is also defined the function makeBlobs, which takes the number of points and the number of dimensions, and is a way to test quickly the library, producing some N-dimensional blobs.
+Outside of the class is also defined the function test_blobs, which takes the number of points and the number of dimensions, and is a way to test quickly the library, producing some N-dimensional blobs.
 
 An expample of how the library should be used is:
 ```
 import CLUEstering as c
 
 clust = c.clusterer(1,5,1.5)
-clust.readData(c.makeBlobs(1000,2))
-clust.runCLUE()
-clust.clusterPlotter()
+clust.read_data(c.test_blobs(1000,2))
+clust.run_clue()
+clust.cluster_plotter()
 ```
 <p align="center">
     <img src="./images/blobwithnoise.png" width="400" height="400"> 
 </p>
```

### Comparing `CLUEstering-1.2.0/LICENSE` & `CLUEstering-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CLUEstering-1.2.0/PKG-INFO` & `CLUEstering-1.4.0/CLUEstering.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: CLUEstering
-Version: 1.2.0
-Summary: A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.
+Version: 1.4.0
+Summary: A library that generalizes the original 2-dimensional CLUE
 Author: Simone Balducci
 Author-email: simone.balducci00@gmail.com
 Keywords: Python,Clustering,Binding
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -33,27 +33,29 @@
 </p>
 
 The C++ code is binded using PyBind11, and the module is created locally during the installation of the library.
 
 In this library is defined the clusterer class. The constructor takes the four parameters, dc_, rhoc, outlierDeltaFactor and pPBin. Passing pPBin is optional since by default it is initialized to 10.
 
 The class has several methods:
-* readData, which takes the data in input and inizializes the class members. The data can be in the form of lists, numpy arrays, string containing the path to a csv file or pandas DataFrame;
-* runCLUE, which takes no parameters and runs the CLUE algorithm;
-* inputPlotter, which takes no parameters and plots the data in input;
-* clusterPlotter, which takes no parameters and plots the data using a different colour for each cluster. The seeds are indicated by stars and the outliers by small grey crosses.
-* toCSV, which takes two strings, the first containing the path to a folder and the second containing the desired name for the csv file (also with the .csv suffix) and produces the csv file containing the cluster informations.
+* read_data, which takes the data in input and inizializes the class members. The data can be in the form of list, numpy array, dictionary, string containing the path to a csv file or pandas DataFrame;
+* change_coordinates, which allows to change the coordinate system used for clustering;
+* choose_kernel, which allows to change the convolution kernel used when calculating the local density of each point. The default kernel is a flat kernel with parameter `0.5`, but it can be changed to an exponential or gaussian kernel, or a custom kernel, which is user defined and can be any continuous function;
+* run_clue, which takes no parameters and runs the CLUE algorithm;
+* input_plotter, which plots all the points in input. This method is useful for getting an idea of the shape of the dataset before clustering. In addition to some plot customizations (like the colour or the size of the points, the addition of a grid, the axis labels and so on) it's also possible to pass the functions for the change of coordinates and change the coordinate system used for plotting.
+* cluster_plotter, which plots the data using a different colour for each cluster. The seeds are indicated by stars and the outliers by small grey crosses.
+* to_csv, which takes two strings, the first containing the path to a folder and the second containing the desired name for the csv file (also with the .csv suffix) and produces the csv file containing the cluster informations.
 
-Outside of the class is also defined the function makeBlobs, which takes the number of points and the number of dimensions, and is a way to test quickly the library, producing some N-dimensional blobs.
+Outside of the class is also defined the function test_blobs, which takes the number of points and the number of dimensions, and is a way to test quickly the library, producing some N-dimensional blobs.
 
 An expample of how the library should be used is:
 ```
 import CLUEstering as c
 
 clust = c.clusterer(1,5,1.5)
-clust.readData(c.makeBlobs(1000,2))
-clust.runCLUE()
-clust.clusterPlotter()
+clust.read_data(c.test_blobs(1000,2))
+clust.run_clue()
+clust.cluster_plotter()
 ```
 <p align="center">
     <img src="./images/blobwithnoise.png" width="400" height="400"> 
 </p>
```

### Comparing `CLUEstering-1.2.0/setup.py` & `CLUEstering-1.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+from pathlib import Path
 from setuptools import setup, find_packages
 from pybind11.setup_helpers import Pybind11Extension
-from pathlib import Path
-import codecs
-import os
 
-__version__ = "1.2.0"
+__version__ = "1.4.0"
 this_directory = Path(__file__).parent
-long_description = (this_directory/'README.md').read_text() 
+long_description = (this_directory/'README.md').read_text()
 
 ext_modules = [
 	Pybind11Extension(
 		"CLUEsteringCPP",
 		['CLUEstering/binding.cc'],
+        include_dirs = ['CLUEstering/include/']
 	),
 ]
 
 setup(
     name="CLUEstering",
     version=__version__,
     author="Simone Balducci",
     author_email="simone.balducci00@gmail.com",
-    description="A library that generalizes the original 2-dimensional CLUE algorithm made at CERN.",
+    description='''A library that generalizes the original 2-dimensional CLUE
+				 algorithm made at CERN.''',
 	 long_description=long_description,
 	 long_description_content_type='text/markdown',
 	 packages=find_packages(),
-	 install_requires=['sklearn','numpy','matplotlib','pandas'],
+	 install_requires=['scikit-learn','numpy','matplotlib','pandas'],
 	 ext_modules=ext_modules,
 	 keywords=['Python','Clustering','Binding'],
 	 python_requires='>=3.7',
 	 classifiers=[
 		'Intended Audience :: Developers',
 		'Programming Language :: Python :: 3',
 		'Operating System :: Unix',
```

