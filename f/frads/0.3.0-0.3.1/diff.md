# Comparing `tmp/frads-0.3.0.tar.gz` & `tmp/frads-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frads-0.3.0.tar", last modified: Tue Apr 18 20:38:14 2023, max compression
+gzip compressed data, was "frads-0.3.1.tar", last modified: Tue Apr 25 17:58:47 2023, max compression
```

## Comparing `frads-0.3.0.tar` & `frads-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.585332 frads-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 20:38:01.000000 frads-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-04-18 20:38:14.585332 frads-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-18 20:38:01.000000 frads-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4088 2023-04-18 20:38:01.000000 frads-0.3.0/frads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33367 2023-04-18 20:38:01.000000 frads-0.3.0/frads/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-18 20:38:01.000000 frads-0.3.0/frads/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    60540 2023-04-18 20:38:01.000000 frads-0.3.0/frads/color_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads/data/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-18 20:38:01.000000 frads-0.3.0/frads/data/WC.DAT
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 20:38:01.000000 frads-0.3.0/frads/data/mrad_default.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    23025 2023-04-18 20:38:01.000000 frads-0.3.0/frads/epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-04-18 20:38:01.000000 frads-0.3.0/frads/eprad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15845 2023-04-18 20:38:01.000000 frads-0.3.0/frads/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14588 2023-04-18 20:38:01.000000 frads-0.3.0/frads/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37712 2023-04-18 20:38:01.000000 frads-0.3.0/frads/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-18 20:38:01.000000 frads-0.3.0/frads/mtxmult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17474 2023-04-18 20:38:01.000000 frads-0.3.0/frads/ncp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-04-18 20:38:01.000000 frads-0.3.0/frads/parsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-04-18 20:38:01.000000 frads-0.3.0/frads/room.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20846 2023-04-18 20:38:01.000000 frads-0.3.0/frads/sky.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-04-18 20:38:01.000000 frads-0.3.0/frads/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19079 2023-04-18 20:38:01.000000 frads-0.3.0/frads/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-18 20:38:01.000000 frads-0.3.0/frads/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-18 20:38:01.000000 frads-0.3.0/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-18 20:38:01.000000 frads-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 20:38:14.585332 frads-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.581332 frads-0.3.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.585332 frads-0.3.0/test/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)  1640229 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)   449366 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/blinds30.xml
--rw-r--r--   0 runner    (1001) docker     (123)   846532 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/klems_aniso_high.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150134 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/oak.wea
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/test.wea
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_mtxmult.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_ncp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_sky.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:47.002461 frads-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-25 17:58:29.000000 frads-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-25 17:58:47.002461 frads-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-25 17:58:29.000000 frads-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:46.994461 frads-0.3.1/frads/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-25 17:58:29.000000 frads-0.3.1/frads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33367 2023-04-25 17:58:29.000000 frads-0.3.1/frads/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-25 17:58:29.000000 frads-0.3.1/frads/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60540 2023-04-25 17:58:29.000000 frads-0.3.1/frads/color_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:46.998461 frads-0.3.1/frads/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-25 17:58:29.000000 frads-0.3.1/frads/data/WC.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-25 17:58:29.000000 frads-0.3.1/frads/data/mrad_default.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22992 2023-04-25 17:58:29.000000 frads-0.3.1/frads/epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-04-25 17:58:29.000000 frads-0.3.1/frads/eprad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15845 2023-04-25 17:58:29.000000 frads-0.3.1/frads/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13948 2023-04-25 17:58:29.000000 frads-0.3.1/frads/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37712 2023-04-25 17:58:29.000000 frads-0.3.1/frads/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-25 17:58:29.000000 frads-0.3.1/frads/mtxmult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17504 2023-04-25 17:58:29.000000 frads-0.3.1/frads/ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-04-25 17:58:29.000000 frads-0.3.1/frads/parsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7465 2023-04-25 17:58:29.000000 frads-0.3.1/frads/room.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18645 2023-04-25 17:58:29.000000 frads-0.3.1/frads/sky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-25 17:58:29.000000 frads-0.3.1/frads/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19079 2023-04-25 17:58:29.000000 frads-0.3.1/frads/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-25 17:58:29.000000 frads-0.3.1/frads/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:46.994461 frads-0.3.1/frads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 17:58:46.000000 frads-0.3.1/frads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-25 17:58:29.000000 frads-0.3.1/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 17:58:29.000000 frads-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 17:58:47.002461 frads-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:46.998461 frads-0.3.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:58:47.002461 frads-0.3.1/test/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  1640229 2023-04-25 17:58:29.000000 frads-0.3.1/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)   449366 2023-04-25 17:58:29.000000 frads-0.3.1/test/Resources/blinds30.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   846532 2023-04-25 17:58:29.000000 frads-0.3.1/test/Resources/klems_aniso_high.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150134 2023-04-25 17:58:29.000000 frads-0.3.1/test/Resources/oak.wea
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-25 17:58:29.000000 frads-0.3.1/test/Resources/test.wea
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_mtxmult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_sky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-25 17:58:29.000000 frads-0.3.1/test/test_window.py
```

### Comparing `frads-0.3.0/PKG-INFO` & `frads-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frads
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wrapper for Radiance related simulation workflows
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
@@ -63,30 +63,27 @@
 
 	>>> import frads
 	>>> print(frads.__version__)
 	0.2.7
 
 ### Optional external library
 
-`Frads` uses Python standard library for all of its functionalities. However, it will take advantage of [Numpy](https://numpy.org) if you have it installed. It will greatly accelerate the matrix multiplication process, especially for progressive simulation workflow.
-
-The [gencolorsky](other_cli.md#gencolorsky) command line tool in `frads` also relies on [libRadTran](http://www.libradtran.org/) a radiative transfer library for computing the spectrally-resolved radiation data. You'd need to install it first to use [gencolorsky](other_cli.md#gencolorsky).
-
 _frads_ runs from the terminal prompt (command line) on Windows, Mac, and Linux OS. Radiance must be [installed](https://www.radiance-online.org/download-install/radiance-source-code/latest-release) prior to use of _frads_.  You can then install _frads_ by entering the following command in your terminal/cmd/powershell:
 
 ```
 pip install frads
 ```
 
-You can also install _frads_ from this Github repository using this command:
+You can also install latest _frads_ from this Github repository using this command:
 
 ```
-pip install git+https://github.com/LBNL-ETA/frads.git
+pip install git+https://github.com/LBNL-ETA/frads@develop
 ```
 
+
 ## Reference
 
 Wang, T., "Frads: A Python Library for Radiance Simulation Control", 2021 Radiance workshop, Bilbao, Spain, August 19, 2021, [ppt](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2/presentations/19_thursday/frads.pdf) , [voice recording](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2)
 
 Wang, T., Ward, G., and Lee, E.S. (2021), A Python Library for Radiance Matrix-based Simulation Control and EnergyPlus Integration, Proceedings of Building Simulation 2021, International Building Performance Simulation Association, Bruges, September 1-3, 2021. Publication to be posted: [pdf](https://www.researchgate.net/publication/358969936_A_Python_Library_for_Radiance_Matrix-based_Simulation_Control_and_EnergyPlus_Integration)
 
 *** License Agreement ***
```

### Comparing `frads-0.3.0/README.md` & `frads-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,28 +54,25 @@
 
 	>>> import frads
 	>>> print(frads.__version__)
 	0.2.7
 
 ### Optional external library
 
-`Frads` uses Python standard library for all of its functionalities. However, it will take advantage of [Numpy](https://numpy.org) if you have it installed. It will greatly accelerate the matrix multiplication process, especially for progressive simulation workflow.
-
-The [gencolorsky](other_cli.md#gencolorsky) command line tool in `frads` also relies on [libRadTran](http://www.libradtran.org/) a radiative transfer library for computing the spectrally-resolved radiation data. You'd need to install it first to use [gencolorsky](other_cli.md#gencolorsky).
-
 _frads_ runs from the terminal prompt (command line) on Windows, Mac, and Linux OS. Radiance must be [installed](https://www.radiance-online.org/download-install/radiance-source-code/latest-release) prior to use of _frads_.  You can then install _frads_ by entering the following command in your terminal/cmd/powershell:
 
 ```
 pip install frads
 ```
 
-You can also install _frads_ from this Github repository using this command:
+You can also install latest _frads_ from this Github repository using this command:
 
 ```
-pip install git+https://github.com/LBNL-ETA/frads.git
+pip install git+https://github.com/LBNL-ETA/frads@develop
 ```
 
+
 ## Reference
 
 Wang, T., "Frads: A Python Library for Radiance Simulation Control", 2021 Radiance workshop, Bilbao, Spain, August 19, 2021, [ppt](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2/presentations/19_thursday/frads.pdf) , [voice recording](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2)
 
 Wang, T., Ward, G., and Lee, E.S. (2021), A Python Library for Radiance Matrix-based Simulation Control and EnergyPlus Integration, Proceedings of Building Simulation 2021, International Building Performance Simulation Association, Bruges, September 1-3, 2021. Publication to be posted: [pdf](https://www.researchgate.net/publication/358969936_A_Python_Library_for_Radiance_Matrix-based_Simulation_Control_and_EnergyPlus_Integration)
```

### Comparing `frads-0.3.0/frads/__init__.py` & `frads-0.3.1/frads/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,24 +81,23 @@
     gen_perez_sky,
     genskymtx,
     WeaData,
     WeaMetaData,
 )
 
 from .types import (
-    Primitive,
     View,
 )
 
 
 from .utils import gen_grid, unpack_primitives
 
 from .window import GlazingSystem, AIR, ARGON, KRYPTON, XENON
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # Check if Radiance is installed more or less
 rad_progs = [
     "rfluxmtx",
     "total",
@@ -132,15 +131,14 @@
     "load_epmodel",
     "load_matrix",
     "multiply_rgb",
     "parse_epw",
     "parse_mrad_config",
     "parse_wea",
     "parse_polygon",
-    "Primitive",
     "points_as_sender",
     "rfluxmtx",
     "sky_as_receiver",
     "surface_as_receiver",
     "sun_as_receiver",
     "surface_as_sender",
     "three_phase",
```

### Comparing `frads-0.3.0/frads/cli.py` & `frads-0.3.1/frads/cli.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/color.py` & `frads-0.3.1/frads/color.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/color_data.py` & `frads-0.3.1/frads/color_data.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/data/WC.DAT` & `frads-0.3.1/frads/data/WC.DAT`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/epjson2rad.py` & `frads-0.3.1/frads/epjson2rad.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     EPlusOpaqueMaterial,
     EPlusWindowMaterial,
     EPlusWindowMaterialComplexShade,
     EPlusConstruction,
     EPlusOpaqueSurface,
     EPlusFenestration,
     EPlusZone,
-    Primitive,
 )
 
 
 logger: logging.Logger = logging.getLogger("frads.epjson2rad")
 
 
 def tmit2tmis(tmit: float) -> float:
@@ -161,20 +160,20 @@
     """Parser EP Material."""
     name = name.replace(" ", "_")
     roughness = material.get("roughness", "Smooth")
     thickness = material.get("thickness", 0.0)
     solar_absorptance = material.get("solar_absorptance", 0.7)
     visible_absorptance = material.get("visible_absorptance", 0.7)
     visible_reflectance = round(1 - visible_absorptance, 2)
-    primitive = Primitive(
+    primitive = pr.Primitive(
         "void",
         "plastic",
         name,
-        ["0"],
-        [5, visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
+        [],
+        [visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
     )
     return EPlusOpaqueMaterial(
         name,
         roughness,
         solar_absorptance,
         visible_absorptance,
         visible_reflectance,
@@ -186,20 +185,20 @@
 def parse_material_nomass(name: str, material: dict) -> EPlusOpaqueMaterial:
     """Parse EP Material:NoMass"""
     name = name.replace(" ", "_")
     roughness = material.get("roughness", "Smooth")
     solar_absorptance = material.get("solar_absorptance", 0.7)
     visible_absorptance = material.get("visible_absorptance", 0.7)
     visible_reflectance = round(1 - visible_absorptance, 2)
-    primitive = Primitive(
+    primitive = pr.Primitive(
         "void",
         "plastic",
         name,
-        ["0"],
-        [5, visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
+        [],
+        [visible_reflectance, visible_reflectance, visible_reflectance, 0, 0],
     )
     return EPlusOpaqueMaterial(
         name,
         roughness,
         solar_absorptance,
         visible_absorptance,
         visible_reflectance,
@@ -257,38 +256,38 @@
     name: str, material: dict
 ) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:SimpleGlazingSystem"""
     identifier = name.replace(" ", "_")
     shgc = material["solar_heat_gain_coefficient"]
     tmit = material.get("visible_transmittance", shgc)
     tmis = tmit2tmis(tmit)
-    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
+    primitive = pr.Primitive("void", "glass", identifier, [], [tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_simpleglazing(
     name: str, material: dict
 ) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Simpleglazing"""
     identifier = name.replace(" ", "_")
     tmit = material["visible_transmittance"]
     tmis = tmit2tmis(tmit)
-    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
+    primitive = pr.Primitive("void", "glass", identifier, [], [tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_glazing(name: str, material: dict) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Glazing"""
     identifier = name.replace(" ", "_")
     if material["optical_data_type"].lower() == "bsdf":
         tmit = 1
     else:
         tmit = material["visible_transmittance_at_normal_incidence"]
     tmis = tmit2tmis(tmit)
-    primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
+    primitive = pr.Primitive("void", "glass", identifier, [], [tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_blind(inp: dict) -> dict:
     """Parse EP WindowMaterial:Blind"""
     blind_prims = {}
     for key, val in inp.items():
@@ -297,20 +296,20 @@
         # back_diff_vis_refl = val['back_side_slat_diffuse_visible_reflectance']
         # front_beam_vis_refl = val['front_side_slat_beam_visible_reflectance']
         front_diff_vis_refl = val["front_side_slat_diffuse_visible_reflectance"]
         # slat_width = val['slat_width']
         # slat_thickness = val['slat_thickness']
         # slat_separation = val['slat_separation']
         # slat_angle = val['slat_angle']
-        blind_prims[key] = Primitive(
+        blind_prims[key] = pr.Primitive(
             "void",
             "plastic",
             _id,
-            ["0"],
-            [5, front_diff_vis_refl, front_diff_vis_refl, front_diff_vis_refl, 0, 0],
+            [],
+            [front_diff_vis_refl, front_diff_vis_refl, front_diff_vis_refl, 0, 0],
         )
         # genblinds_cmd = f"genblinds {_id} {_id} {slat_width} 3
         # {20*slat_separation} {slat_angle}"
     return blind_prims
 
 
 def parse_epjson_material(epjs: dict) -> dict:
```

### Comparing `frads-0.3.0/frads/eprad.py` & `frads-0.3.1/frads/eprad.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/geom.py` & `frads-0.3.1/frads/geom.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/matrix.py` & `frads-0.3.1/frads/matrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 from __future__ import annotations
 from dataclasses import dataclass
 import logging
 import os
 from pathlib import Path
-import subprocess as sp
 import tempfile as tf
 from typing import List, Optional, Union, Sequence
 
 from frads import geom, parsers, sky, utils
 import numpy as np
 import pyradiance as pr
 
@@ -96,52 +95,33 @@
         raise ValueError("Need to specify resolution")
     res_eval = pr.vwrays(
         view=view.args(), xres=xres, yres=yres, dimensions=True
     ).split()
     new_xres, new_yres = int(res_eval[1]), int(res_eval[3])
     if (new_xres != xres) and (new_yres != yres):
         logger.info("Changed resolution to %s %s", new_xres, new_yres)
-    # vwrays_cmd = ["vwrays", "-ff", "-x", str(new_xres), "-y", str(new_yres)]
-    vwrays_cmd = ["vwrays", "-ff"]
-    if ray_cnt > 1:
-        vwrays_cmd.extend(["-c", str(ray_cnt), "-pj", "0.7"])
-    logger.debug("Ray count is %s", ray_cnt)
-    vwrays_cmd += view.args()
-    vwrays_cmd += ["-x", str(new_xres), "-y", str(new_yres)]
-    logger.info("Generate view rays with: \n%s", " ".join(vwrays_cmd))
-    vwrays_proc = sp.run(vwrays_cmd, check=True, stdout=sp.PIPE)
     vwrays_proc = pr.vwrays(
         view=view.args(),
         outform="f",
         xres=new_xres,
         yres=new_yres,
         ray_count=ray_cnt,
         pixel_jitter=0.7,
     )
     if view.vtype == "a":
-        flush_cmd = [
-            "rcalc",
-            "-if6",
-            "-of",
-            "-e",
-            f"DIM:{xres};CNT:{ray_cnt}",
-            "-e",
-            "pn=(recno-1)/CNT+.5",
-            "-e",
-            "frac(x):x-floor(x)",
-            "-e",
-            "xpos=frac(pn/DIM);ypos=pn/(DIM*DIM)",
-            "-e",
-            "incir=if(.25-(xpos-.5)*(xpos-.5)-(ypos-.5)*(ypos-.5),1,0)",
-            "-e",
-            "$1=$1;$2=$2;$3=$3;$4=$4*incir;$5=$5*incir;$6=$6*incir",
-        ]
-        logger.info("Flushing -vta corner rays: \n%s", " ".join(flush_cmd))
-        flush_proc = sp.run(flush_cmd, check=True, input=vwrays_proc, stdout=sp.PIPE)
-        vrays = flush_proc.stdout
+        ray_flush_exp = (
+            f"DIM:{xres};CNT:{ray_cnt};"
+            "pn=(recno-1)/CNT+.5;"
+            "frac(x):x-floor(x);"
+            "xpos=frac(pn/DIM);ypos=pn/(DIM*DIM);"
+            "incir=if(.25-(xpos-.5)*(xpos-.5)-(ypos-.5)*(ypos-.5),1,0);"
+            "$1=$1;$2=$2;$3=$3;$4=$4*incir;$5=$5*incir;$6=$6*incir;"
+        )
+        flushed_rays = pr.rcalc(vwrays_proc, inform='f', incount=6, outform="f", expr=ray_flush_exp)
+        vrays = flushed_rays
     else:
         vrays = vwrays_proc
     logger.debug("View sender:\n%s", vrays)
     return Sender("v", vrays, xres, yres)
 
 
 def load_matrix(file: Union[bytes, str, Path], dtype: str = "float"):
@@ -398,18 +378,19 @@
         None
     """
 
     with tf.TemporaryDirectory() as tempd:
         receiver_path = os.path.join(tempd, "rcvr_path")
         with open(receiver_path, "w", encoding="utf-8") as wtr:
             wtr.write(receiver.receiver)
-        ocmd = ["oconv", "-f", *map(str, env), receiver_path]
-        logger.info("Generate octree with:\n%s", " ".join(ocmd))
+        # ocmd = ["oconv", "-f", *map(str, env), receiver_path]
+        # logger.info("Generate octree with:\n%s", " ".join(ocmd))
         with open(oct_path, "wb") as wtr:
-            sp.run(ocmd, check=True, stdout=wtr)
+            # sp.run(ocmd, check=True, stdout=wtr)
+            wtr.write(pr.oconv(*map(str, env), receiver_path, frozen=True))
 
 
 def rcontrib(
     sender,
     modifier: str,
     octree: Union[str, Path],
     out: Union[str, Path],
```

### Comparing `frads-0.3.0/frads/methods.py` & `frads-0.3.1/frads/methods.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/mtxmult.py` & `frads-0.3.1/frads/mtxmult.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/ncp.py` & `frads-0.3.1/frads/ncp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from pathlib import Path
 import subprocess as sp
 import tempfile as tf
 from typing import List
 from typing import Optional
 from typing import Sequence
 
+import pyradiance as pr
 from frads import matrix
 from frads import geom
 from frads import parsers
-from frads.types import Primitive
+# from frads.types import Primitive
 from frads.types import NcpModel
 from frads import utils
 
 logger: logging.Logger = logging.getLogger("frads.mfacade")
 
 
 def ncp_compute_back(
@@ -59,15 +60,15 @@
         matrix.rfluxmtx(sender=sndr, receiver=front_rcvr, env=model.env, opt=opt)
 
 
 def ncp_compute_front(model: NcpModel, src_dict, opt, refl: bool = False) -> None:
     """compute back side calculation."""
     sndr_prim = []
     for p in model.ports:
-        np = Primitive(
+        np = pr.Primitive(
             p.modifier,
             p.ptype,
             p.identifier,
             p.str_arg,
             parsers.parse_polygon(p.real_arg).flip().to_real(),
         )
         sndr_prim.append(np)
@@ -367,44 +368,44 @@
     #     cmd += f" > {os.path.join(dirname, oname)}.xml"
     #     os.system(cmd)
     #     shutil.rmtree(td)
     #     [os.remove(mtx) for mtx in mtxs]
 
 
 def gen_port_prims_from_window_ncp(
-    wprim: Sequence[Primitive], nprim: Sequence[Primitive]
-) -> List[Primitive]:
+    wprim: Sequence[pr.Primitive], nprim: Sequence[pr.Primitive]
+) -> List[pr.Primitive]:
     """Generate port primitives from window and non-coplanar shading primitives."""
     if len(wprim) > 1:
         awprim = merge_windows(wprim)
     else:
         awprim = wprim[0]
-    wplg = parsers.parse_polygon(awprim.real_arg)
-    nplgs = [parsers.parse_polygon(p.real_arg) for p in nprim if p.ptype == "polygon"]
+    wplg = parsers.parse_polygon(awprim.fargs)
+    nplgs = [parsers.parse_polygon(p.fargs) for p in nprim if p.ptype == "polygon"]
     all_ports = gen_ports_from_window_ncp(wplg, nplgs)
     port_prims = []
     for idx, plg in enumerate(all_ports):
         new_prim = utils.polygon2prim(plg, "port", f"portf{idx+1}")
         logger.debug(str(new_prim))
         port_prims.append(new_prim)
     return port_prims
 
 
 def gen_port_prims_from_window(
-    wprim: Sequence[Primitive], depth: float, scale_factor: float
-) -> List[Primitive]:
+    wprim: Sequence[pr.Primitive], depth: float, scale_factor: float
+) -> List[pr.Primitive]:
     """Generate port primitives from window primitives, depth, and scale factor."""
     if len(wprim) > 1:
         awprim = merge_windows(wprim)
     else:
         awprim = wprim[0]
-    wpoly = parsers.parse_polygon(awprim.real_arg)
+    wpoly = parsers.parse_polygon(awprim.fargs)
     extrude_vector = wpoly.normal.reverse().scale(depth)
     scale_vector = geom.Vector(scale_factor, scale_factor, scale_factor)
-    scaled_window = wpoly.scale(scale_vector, wpoly.centroid())
+    scaled_window = wpoly.scale(scale_vector, wpoly.centroid)
     all_ports = scaled_window.extrude(extrude_vector)[1:]
     port_prims = []
     for idx, plg in enumerate(all_ports):
         new_prim = utils.polygon2prim(plg, "port", f"portf{idx+1}")
         logger.debug(str(new_prim))
         port_prims.append(new_prim)
     return port_prims
@@ -438,34 +439,34 @@
     area_list = []
     win_normals = []
     # Find axiel aligned rotation angle
     bboxes = []
     for deg in range(90):
         rad = math.radians(deg)
         win_polygon_r = wp.rotate(zaxis, rad)
-        win_normals.append(win_polygon_r.normal())
+        win_normals.append(win_polygon_r.normal)
         ncs_polygon_r = [p.rotate(zaxis, rad) for p in np]
         ncs_polygon_r.append(win_polygon_r)
         _bbox = geom.getbbox(ncs_polygon_r, offset=0.0)
         bboxes.append(_bbox)
-        area_list.append(_bbox[0].area())
+        area_list.append(_bbox[0].area)
     # Rotate to position
     deg = area_list.index(min(area_list))
     rrad = math.radians(deg)
     bbox = bboxes[deg]
     _win_normal = [round(i, 1) for i in win_normals[deg].to_list()]
     del bbox[rm_pg.index(_win_normal) + 2]
     rotate_back = [pg.rotate(zaxis, rrad * -1) for pg in bbox]
     return rotate_back
 
 
-def merge_windows(prims: Sequence[Primitive]) -> Primitive:
+def merge_windows(prims: Sequence[pr.Primitive]) -> pr.Primitive:
     """Merge rectangles if coplanar."""
-    polygons = [parsers.parse_polygon(p.real_arg) for p in prims]
-    normals = [p.normal() for p in polygons]
+    polygons = [parsers.parse_polygon(p.fargs) for p in prims]
+    normals = [p.normal for p in polygons]
     if len(set(normals)) > 1:
         raise ValueError("Windows not co-planar")
     points = [i for p in polygons for i in p.vertices]
     hull_polygon = geom.convexhull(points, normals[0])
     modifier = prims[0].modifier
     identifier = prims[0].identifier
     new_prim = utils.polygon2prim(hull_polygon, modifier, identifier)
```

### Comparing `frads-0.3.0/frads/parsers.py` & `frads-0.3.1/frads/parsers.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/room.py` & `frads-0.3.1/frads/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Generic room model"""
 from typing import List
 from typing import Optional
 
+import pyradiance as pr
 from frads import geom
 from frads import utils
-from frads.types import Primitive
 
 
 class Surface:
     """Surface object."""
 
     def __init__(self, base: geom.Polygon) -> None:
         """."""
@@ -16,15 +16,15 @@
         self._vertices = base.vertices
         self._vect1 = (base.vertices[1] - base.vertices[0]).normalize()
         self._vect2 = (base.vertices[2] - base.vertices[1]).normalize()
         self.polygons: List[geom.Polygon] = [self.base]
         self.windows: List[Surface] = []
         self._modifier: str = "void"
         self._identifier: str = "void"
-        self._primitives: Optional[List[Primitive]] = None
+        self._primitives: Optional[List[pr.Primitive]] = None
 
     @property
     def modifier(self):
         """."""
         return self._modifier
 
     @property
@@ -39,24 +39,24 @@
 
     @identifier.setter
     def identifier(self, identifier):
         """."""
         self._identifier = identifier
 
     @property
-    def primitives(self) -> Optional[List[Primitive]]:
+    def primitives(self) -> Optional[List[pr.Primitive]]:
         """."""
         self._primitives = []
         for idx, polygon in enumerate(self.polygons):
             self._primitives.append(
-                Primitive(
+                pr.Primitive(
                     self.modifier,
                     "polygon",
                     f"{self.identifier}_{idx:02d}",
-                    ["0"],
+                    [],
                     polygon.to_real(),
                 )
             )
         return self._primitives
 
     def make_window_wwr(self, wwr: float) -> None:
         """Make a window based on window-to-wall ratio."""
@@ -91,20 +91,20 @@
         direction = self.base.normal.scale(distance)
         self.windows = [Surface(window.base.move(direction)) for window in self.windows]
 
     def rotate(self, deg):
         """Rotate the surface counter clock-wise."""
         polygons = []
         for plg in self.polygons:
-            polygons.append(plg.rotate3d(deg, geom.Vector(0, 0, 1)))
+            polygons.append(plg.rotate(deg, geom.Vector(0, 0, 1)))
         self.polygons = polygons
         for window in self.windows:
             wpolygons = []
             for plg in window.polygons:
-                wpolygons.append(plg.rotate3d(deg, geom.Vector(0, 0, 1)))
+                wpolygons.append(plg.rotate(deg, geom.Vector(0, 0, 1)))
 
 
 class Room:
     """Make a shoebox."""
 
     def __init__(self, floor: Surface, ceiling, swall, ewall, nwall, wwall) -> None:
         """."""
```

### Comparing `frads-0.3.0/frads/sky.py` & `frads-0.3.1/frads/sky.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 """
 
 import datetime
 import logging
 import math
 import os
 from pathlib import Path
-import subprocess as sp
 from typing import Any, List, NamedTuple, Optional, Sequence, Tuple, Union
 
 import pyradiance as pr
 
 from frads import geom, utils
 
 logger: logging.Logger = logging.getLogger("frads.sky")
 
-# Solar disk solid angle (sr)
-SOLAR_SA = 6.7967e-5
-
 
 class WeaMetaData(NamedTuple):
     """Weather related meta data object.
 
     Attributes:
         city: City.
         country: Country.
@@ -170,21 +166,18 @@
         corresponding modifier strings, and the full set of modifier string.
     """
     runlen = 144 * mf**2 + 3
     dirs, _ = utils.calc_reinsrc_dir(mf)
     full_mod_str = os.linesep.join([f"sol{i}" for i in range(1, runlen)])
     win_norm = []
     if smx_path is not None:
-        cmd1 = ["rmtxop", "-ff", "-c", ".3", ".6", ".1", "-t", str(smx_path)]
-        cmd2 = ["getinfo", "-"]
-        cmd3 = ["total", f"-if{runlen-1}", "-t,"]
-        proc1 = sp.run(cmd1, check=True, stdout=sp.PIPE)
-        proc2 = sp.run(cmd2, check=True, input=proc1.stdout, stdout=sp.PIPE)
-        proc3 = sp.run(cmd3, check=True, input=proc2.stdout, stdout=sp.PIPE)
-        dtot = [float(i) for i in proc3.stdout.split(b",")]
+        cmd1 = pr.rmtxop(str(smx_path), outform='f', transpose=True, transform=(.3, .6, .1))
+        cmd2 = pr.getinfo(cmd1, strip_header=True)
+        proc3 = pr.total(cmd2, inform='f', incount=runlen-1, sep=',')
+        dtot = [float(i) for i in proc3.split(b",")]
     else:
         dtot = [1] * runlen
     out_lines = []
     mod_str = []
     if window_normals is not None:
         win_norm = window_normals
         for i, d in enumerate(dirs):
@@ -269,15 +262,15 @@
                 elevation=meta.elevation,
                 location=meta.city + meta.country,
             ).encode()
         else:
             raise ValueError("Either a .wea path or wea data is required.")
     else:
         inp = wpath
-    _err, _out = pr.gendaymtx(
+    _out = pr.gendaymtx(
         inp,
         header=header,
         average=average,
         sun_only=sun_only,
         sky_only=sky_only,
         solar_radiance=solar_radiance,
         sun_file=sun_file,
@@ -286,65 +279,16 @@
         sky_color=sky_color,
         ground_color=ground_color,
         rotate=rotate,
         outform=outform,
         onesun=onesun,
         mfactor=mfactor,
     )
-    logger.warning(_err)
     return _out
 
-    # stdin = None
-    # cmd = ["gendaymtx", "-m", str(mf)]
-    # if binary:
-    #     cmd.append("-of")
-    # if direct:
-    #     cmd.append("-d")
-    # if onesun:
-    #     cmd.extend(["-5", ".533"])
-    # if rotate is not None:
-    #     cmd.extend(["-r", str(rotate)])
-    # if solar:
-    #     cmd.append("-O1")
-    # if wpath is not None:
-    #     cmd.append(str(wpath))
-    # elif (data is not None) and (meta is not None):
-    #     wea_input = meta.wea_header() + "\n".join(map(str, data))
-    #     stdin = wea_input.encode("utf-8")
-    # else:
-    #     raise ValueError("Need to specify either .wea path or wea data.")
-    # if out is not None:
-    #     with open(out, "wb") as wtr:
-    #         logger.info("Calling gendaymtx with:\n%s", " ".join(cmd))
-    #         sp.run(cmd, check=True, input=stdin, stdout=wtr)
-    # return cmd
-
-
-# def gen_perez_sky(row: WeaData, meta, grefl: float = 0.2, spect: str = "0", rotate=None) -> str:
-#     solar = False if spect == "0" else True
-#     gendaylit = gendaylit_cmd(
-#         str(row.time.month),
-#         str(row.time.day),
-#         str(row.time.hour + row.time.minute / 60 + row.time.second / 3600),
-#         str(meta.latitude),
-#         str(meta.longitude),
-#         str(meta.timezone),
-#         dir_norm_ir=str(row.dni),
-#         dif_hor_ir=str(row.dhi),
-#         solar=solar,
-#         grefl=grefl,
-#     )
-#     out = []
-#     rot = f"| xform -rz {rotate}" if rotate is not None else ""
-#     out.append(f"!{' '.join(gendaylit)}{rot} \n")
-#     out.append("skyfunc glow sglow 0 0 4 1 1 1 0\n")
-#     out.append("sglow source sky 0 0 4 0 0 1 180\n")
-#     out.append("sglow source ground 0 0 4 0 0 -1 180\n")
-#     return " ".join(out)
-
 
 def gen_perez_sky(
     dt,
     latitude: float,
     longitude: float,
     timezone: int,
     year: Optional[int] = None,
@@ -540,25 +484,16 @@
         data: Sequence[WeaData],
         meta: WeaMetaData,
         window_normal: Optional[Sequence[geom.Vector]] = None,
     Returns:
         data(List[WeaData]):
     """
     wea_input = meta.wea_header() + "\n".join(map(str, data))
-    # pr.gendaymtx(wea_input, daylight_only=True, )
-    proc = sp.run(
-        ["gendaymtx", "-u", "-D", "-"],
-        check=True,
-        input=wea_input,
-        encoding="ascii",
-        stderr=sp.PIPE,
-        stdout=sp.PIPE,
-    )
-    # prims = parsers.parse_primitive(proc.stdout.splitlines())
-    prims = pr.parse_primitive(proc.stdout)
+    out = pr.gendaymtx(wea_input.encode(), sun_file='-', daylight_hours_only=True)
+    prims = pr.parse_primitive(out.decode())
     light_prims = [prim for prim in prims if prim.ptype == "light"]
     keep_minutes = []
     if window_normal is not None:
         source_prims = [prim for prim in prims if prim.ptype == "source"]
         for lpr, spr in zip(light_prims, source_prims):
             if lpr.fargs[0] > 0:
                 sdir = geom.Vector(*spr.fargs[:3])
```

### Comparing `frads-0.3.0/frads/types.py` & `frads-0.3.1/frads/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,74 +6,19 @@
 """
 
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from typing import Dict, Iterable, List, NamedTuple, Optional, Sequence, Tuple, Union
 
-
+import pyradiance as pr
 from frads.geom import Polygon
 from frads.geom import Vector
 
 
-class Primitive(NamedTuple):
-    """Radiance Primitive.
-
-    Attributes one-to-one mapped from Radiance.
-
-    Attributes:
-        modifier: modifier, which primitive modifies this one
-        ptype: primitive type
-        identifier: identifier, name of this primitive
-        str_arg: string argument
-        real_arg: real argument
-        int_arg: integer argument, not used in Radiance (default="0")
-    """
-
-    modifier: str
-    ptype: str
-    identifier: str
-    str_arg: Sequence[str]
-    real_arg: Sequence[Union[int, float]]
-    int_arg: str = "0"
-
-    def __repr__(self) -> str:
-        output = (
-            f"Primitive({self.modifier}, {self.ptype}, "
-            f"{self.identifier}, {self.str_arg}, "
-            f"{self.int_arg}, {self.real_arg})"
-        )
-        return output
-
-    def __str__(self) -> str:
-        output = (
-            f"{self.modifier} {self.ptype} {self.identifier}\n"
-            f"{int(self.str_arg[0])} {' '.join(self.str_arg[1:])}\n"
-            f"{self.int_arg}\n"
-            f"{int(self.real_arg[0])} "
-            f"{' '.join(map(str, self.real_arg[1:]))}\n"
-        )
-        return output
-
-
-@dataclass
-class Alias:
-    modifier: str
-    name_to: str
-    name_from: str
-
-    def __repr__(self) -> str:
-        output = f"Alias({self.modifier}, {self.name_to}, {self.name_from})"
-        return output
-
-    def __str__(self) -> str:
-        output = f"{self.modifier} alias {self.name_to} {self.name_from}"
-        return output
-
-
 class PaneProperty(NamedTuple):
     """Window pane property object.
 
     Attributes:
         name str: material name.
         thickness float: pane thickness.
         gtype str: material type.
@@ -138,15 +83,15 @@
         ncp_shades: The list of non-coplanar shading files.
         black_env_path: Blackened environment file path.
 
     """
 
     name: str
     material_path: Path
-    window_groups: Dict[str, List[Primitive]]
+    window_groups: Dict[str, List[pr.Primitive]]
     window_normals: List[Vector]
     sender_grid: dict
     sender_view: dict
     views: dict
     bsdf_xml: dict
     cfs_paths: list
     ncp_shades: dict
@@ -202,16 +147,16 @@
     smx_sun_img: Path = field(default_factory=Path)
 
 
 @dataclass
 class NcpModel:
     """Non-coplanar data model."""
 
-    windows: Sequence[Primitive]
-    ports: Sequence[Primitive]
+    windows: Sequence[pr.Primitive]
+    ports: Sequence[pr.Primitive]
     env: Iterable[Path]
     sbasis: str
     rbasis: str
 
 
 @dataclass
 class EPlusWindowGas:
@@ -229,25 +174,25 @@
     """EnergyPlus Opaque material data container."""
 
     name: str
     roughness: str
     solar_absorptance: float
     visible_absorptance: float
     visible_reflectance: float
-    primitive: Primitive
+    primitive: pr.Primitive
     thickness: float = 0.0
 
 
 @dataclass
 class EPlusWindowMaterial:
     """EnergyPlus regular window material data container."""
 
     name: str
     visible_transmittance: float
-    primitive: Primitive
+    primitive: pr.Primitive
 
 
 @dataclass
 class EPlusWindowMaterialComplexShade:
     """EnergyPlus complex window material data container."""
 
     name: str
```

### Comparing `frads-0.3.0/frads/utils.py` & `frads-0.3.1/frads/utils.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads/window.py` & `frads-0.3.1/frads/window.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/frads.egg-info/PKG-INFO` & `frads-0.3.1/frads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frads
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wrapper for Radiance related simulation workflows
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
@@ -63,30 +63,27 @@
 
 	>>> import frads
 	>>> print(frads.__version__)
 	0.2.7
 
 ### Optional external library
 
-`Frads` uses Python standard library for all of its functionalities. However, it will take advantage of [Numpy](https://numpy.org) if you have it installed. It will greatly accelerate the matrix multiplication process, especially for progressive simulation workflow.
-
-The [gencolorsky](other_cli.md#gencolorsky) command line tool in `frads` also relies on [libRadTran](http://www.libradtran.org/) a radiative transfer library for computing the spectrally-resolved radiation data. You'd need to install it first to use [gencolorsky](other_cli.md#gencolorsky).
-
 _frads_ runs from the terminal prompt (command line) on Windows, Mac, and Linux OS. Radiance must be [installed](https://www.radiance-online.org/download-install/radiance-source-code/latest-release) prior to use of _frads_.  You can then install _frads_ by entering the following command in your terminal/cmd/powershell:
 
 ```
 pip install frads
 ```
 
-You can also install _frads_ from this Github repository using this command:
+You can also install latest _frads_ from this Github repository using this command:
 
 ```
-pip install git+https://github.com/LBNL-ETA/frads.git
+pip install git+https://github.com/LBNL-ETA/frads@develop
 ```
 
+
 ## Reference
 
 Wang, T., "Frads: A Python Library for Radiance Simulation Control", 2021 Radiance workshop, Bilbao, Spain, August 19, 2021, [ppt](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2/presentations/19_thursday/frads.pdf) , [voice recording](https://www.radiance-online.org/community/workshops/2021-bilbao-spain-2)
 
 Wang, T., Ward, G., and Lee, E.S. (2021), A Python Library for Radiance Matrix-based Simulation Control and EnergyPlus Integration, Proceedings of Building Simulation 2021, International Building Performance Simulation Association, Bruges, September 1-3, 2021. Publication to be posted: [pdf](https://www.researchgate.net/publication/358969936_A_Python_Library_for_Radiance_Matrix-based_Simulation_Control_and_EnergyPlus_Integration)
 
 *** License Agreement ***
```

### Comparing `frads-0.3.0/frads.egg-info/SOURCES.txt` & `frads-0.3.1/frads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/license.txt` & `frads-0.3.1/license.txt`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/setup.cfg` & `frads-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw` & `frads-0.3.1/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/Resources/blinds30.xml` & `frads-0.3.1/test/Resources/blinds30.xml`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/Resources/klems_aniso_high.xml` & `frads-0.3.1/test/Resources/klems_aniso_high.xml`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/Resources/oak.wea` & `frads-0.3.1/test/Resources/oak.wea`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_color.py` & `frads-0.3.1/test/test_color.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_epjson2rad.py` & `frads-0.3.1/test/test_epjson2rad.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_geom.py` & `frads-0.3.1/test/test_geom.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_matrix.py` & `frads-0.3.1/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_methods.py` & `frads-0.3.1/test/test_methods.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_mtxmult.py` & `frads-0.3.1/test/test_mtxmult.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_ncp.py` & `frads-0.3.1/test/test_ncp.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_parsers.py` & `frads-0.3.1/test/test_parsers.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_sky.py` & `frads-0.3.1/test/test_sky.py`

 * *Files identical despite different names*

### Comparing `frads-0.3.0/test/test_utils.py` & `frads-0.3.1/test/test_utils.py`

 * *Files identical despite different names*

