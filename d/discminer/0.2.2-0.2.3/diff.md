# Comparing `tmp/discminer-0.2.2.tar.gz` & `tmp/discminer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.2.tar", last modified: Fri Apr 21 14:08:39 2023, max compression
+gzip compressed data, was "discminer-0.2.3.tar", last modified: Wed Apr 26 17:35:30 2023, max compression
```

## Comparing `discminer-0.2.2.tar` & `discminer-0.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.110568 discminer-0.2.2/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.2/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-21 14:08:39.110731 discminer-0.2.2/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.2/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.087216 discminer-0.2.2/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.2/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.2/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.2/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.2/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.2/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.2/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.2/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.2/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.2/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.2/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.2/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.2/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.098772 discminer-0.2.2/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.2/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-21 14:07:44.000000 discminer-0.2.2/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.2/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.2/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.2.2/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.2.2/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71196 2023-04-21 14:06:55.000000 discminer-0.2.2/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.2/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.105231 discminer-0.2.2/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.2/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.2/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.2/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.2/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.2/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.2/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.2/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.2/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    29567 2023-04-20 17:31:21.000000 discminer-0.2.2/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.2/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.2/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.107243 discminer-0.2.2/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.2/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.2/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.2/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.2/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.100201 discminer-0.2.2/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-21 14:08:38.000000 discminer-0.2.2/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-21 14:08:38.000000 discminer-0.2.2/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-21 14:08:38.000000 discminer-0.2.2/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-21 14:08:38.000000 discminer-0.2.2/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-21 14:08:38.000000 discminer-0.2.2/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.2/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-21 14:08:39.111142 discminer-0.2.2/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.2/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 14:08:39.109883 discminer-0.2.2/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.2/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.2/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.2/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.2/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.927434 discminer-0.2.3/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.3/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-26 17:35:30.927602 discminer-0.2.3/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.3/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.907942 discminer-0.2.3/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.3/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.3/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.3/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.3/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.3/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.3/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.3/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.3/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.3/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.3/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.3/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.3/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.918342 discminer-0.2.3/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.3/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-26 17:33:09.000000 discminer-0.2.3/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.3/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.3/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.3/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.3/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.3/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.3/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.922450 discminer-0.2.3/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.3/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.3/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.3/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.3/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    29646 2023-04-21 14:29:28.000000 discminer-0.2.3/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.3/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.3/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.923889 discminer-0.2.3/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.3/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.3/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.3/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.3/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.920134 discminer-0.2.3/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-26 17:35:30.000000 discminer-0.2.3/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.3/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-26 17:35:30.928005 discminer-0.2.3/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.3/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-26 17:35:30.926759 discminer-0.2.3/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.3/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.3/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.3/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.3/template/prepare_data.py
```

### Comparing `discminer-0.2.2/LICENSE` & `discminer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/PKG-INFO` & `discminer-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.2 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.3 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.2/README.md` & `discminer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/make_channels.py` & `discminer-0.2.3/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/make_parfile.py` & `discminer-0.2.3/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/make_single_moments.py` & `discminer-0.2.3/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_attributes_model.py` & `discminer-0.2.3/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.3/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_moment+offset.py` & `discminer-0.2.3/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_moment+residuals.py` & `discminer-0.2.3/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_peak_residuals.py` & `discminer-0.2.3/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_radial_profiles.py` & `discminer-0.2.3/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_residuals+all.py` & `discminer-0.2.3/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/plot_residuals+deproj.py` & `discminer-0.2.3/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/_mining/utils.py` & `discminer-0.2.3/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/cart.py` & `discminer-0.2.3/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/core.py` & `discminer-0.2.3/discminer/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         try:
             cube_vel = cube_spe.with_spectral_unit(
                 u.km / u.s,
                 velocity_convention="radio",
                 rest_value=cube_spe.header["RESTFRQ"] * u.Hz,
             )
         except KeyError:
+            #Assume velocity axis is already in km/s
             cube_vel = cube_spe
             
         #In km/s, remove .value to keep astropy units
         vchannels = cube_vel.spectral_axis.value
         header = cube_vel.header
         
         #Get data and beam info
```

### Comparing `discminer-0.2.2/discminer/cube.py` & `discminer-0.2.3/discminer/cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,18 @@
         self.dpc = dpc
         self.pix_size = np.abs(self.header["CDELT1"]) * u.Unit(self.header["CUNIT1"])  # pixel size in CUNIT1 units (usually degrees)
 
         # self.extent = 
         if isinstance(beam, Beam):
             self._init_beam_kernel()  # Get 2D Gaussian kernel from beam
         elif beam is None:
-            pass
+            self.beam_size = None
+            self.beam_area = None
+            self.beam_kernel = None
+            self.beam_area_arcsecs = None
         else:
             raise InputError(beam, "beam must be either None or radio_beam.Beam object")
 
         self._interactive = self._cursor
         self._interactive_path = self._curve
 
     @property
```

### Comparing `discminer-0.2.2/discminer/disc2d.py` & `discminer-0.2.3/discminer/disc2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -657,18 +657,16 @@
         else: linew2d = linewidth2d
         if isinstance(lineslope2d, numbers.Number): lineb2d['upper'] = lineb2d['lower'] = lineslope2d
         else: lineb2d = lineslope2d
     
         v_near, v_far = self.get_line_profile(v_chan, vel2d, linew2d, lineb2d, **kwargs)
         int2d_full = self.line_uplow(int2d_near, int2d_far)
         
-        if self.beam_kernel:
-            inf_mask = np.isnan(int2d_full)
-            int2d_full = np.where(inf_mask, 0.0, int2d_full) # Use np.nan_to_num instead
-            int2d_full = self.beam_area*convolve(int2d_full, self.beam_kernel, preserve_nan=False)
+        if self.beam_kernel is not None:
+            int2d_full = self.beam_area*convolve(np.nan_to_num(int2d_full), self.beam_kernel, preserve_nan=False)
 
         return int2d_full
 
     def get_cube(self, vchannels, velocity2d, intensity2d, linewidth2d, lineslope2d, make_convolve=True,
                  rms=None, tb={'nu': False, 'beam': False, 'full': True}, return_data_only=False, header=None, dpc=None, **kwargs_line):
         
         vel2d, int2d, linew2d, lineb2d = velocity2d, {}, {}, {}
```

### Comparing `discminer-0.2.2/discminer/grid.py` & `discminer-0.2.3/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_box.png` & `discminer-0.2.3/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_cursor.jpeg` & `discminer-0.2.3/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_path.png` & `discminer-0.2.3/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_return.png` & `discminer-0.2.3/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_surface.png` & `discminer-0.2.3/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/icons/button_trash.jpg` & `discminer-0.2.3/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/pick.py` & `discminer-0.2.3/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/plottools.py` & `discminer-0.2.3/discminer/plottools.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,16 @@
 def add_cbar_ax(fig, ax, perc=4, orientation='horizontal', subplots=True):
     figx, figy = fig.get_size_inches()
     figr = figy/figx
     axp = ax.get_position()
     x0, x1, y0, y1 = axp.x0, axp.x1, axp.y0, axp.y1
     w = x1 - x0
     h = y1 - y0
-    dy = 0.01*perc
-    dx = dy*figr    
+    dx = dy = 0.01*perc
+    
     if subplots:
         if orientation=='horizontal': return fig.add_axes([x0, y0, w, dy])
         if orientation=='vertical': return fig.add_axes([x1+0.5*dx, y0+0.1*h, dx, h-0.2*h])        
     else:
         if orientation=='horizontal': return fig.add_axes([x0, y0-0.5*dy, w, dy])
         if orientation=='vertical': return fig.add_axes([x1+0.5*dx, y0, dx, h])        
         
@@ -513,19 +513,23 @@
 
 
 def make_polar_map(
         map2d, levels, R, PHI, Rout,
         Rin = 0.0,
         fig=None, ax=None, 
         cmap=get_discminer_cmap('velocity'),
-        fmt='%5.2f', clabel=None, gradient=0, 
+        fmt='%5.2f', clabel=None, gradient=0,
+        **kwargs_cbar
         #,filaments=[],                            
 ):
     from scipy.interpolate import griddata
 
+    kwargs_cb = dict(orientation='vertical', subplots=False, perc=2)
+    kwargs_cb.update(kwargs_cbar)
+    
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(12, 3))
     Rout = Rout.to('au').value
     try:
         Rin = Rin.to('au').value
     except AttributeError:
@@ -594,15 +598,15 @@
     make_up_ax(ax, labelbottom=True, labeltop=False, labelsize=SMALL_SIZE+1,
                xlims=(-180.1, 180.1), ylims=(1.1*Rin, 0.95*Rout))
     ax.set_xticks(np.linspace(-180, 180, 13))
     ax.set_xlabel('Azimuth [deg]', fontsize=MEDIUM_SIZE)
     ax.set_ylabel('Radius [au]', fontsize=MEDIUM_SIZE)
     mod_major_ticks(ax, axis='y', nbins=10)
                        
-    cax = add_cbar_ax(fig, ax, orientation='vertical', subplots=False, perc=6)    
+    cax = add_cbar_ax(fig, ax, **kwargs_cb)
     cbar = plt.colorbar(im, cax=cax, format=fmt, orientation='vertical', ticks=np.linspace(levels.min(), levels.max(), 5))
     cbar.ax.tick_params(which='major', direction='in', width=2.7, size=4.8, pad=4, labelsize=SMALL_SIZE)
     cbar.ax.tick_params(which='minor', direction='in', width=2.7, size=3.3)
     cbar.set_label(clabel, fontsize=SMALL_SIZE, labelpad=20, rotation=270)
     mod_minor_ticks(cbar.ax)
 
     return fig, ax, cbar
```

### Comparing `discminer-0.2.2/discminer/rail.py` & `discminer-0.2.3/discminer/rail.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/testyapf.py` & `discminer-0.2.3/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/tools/discminer.mplstyle` & `discminer-0.2.3/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/tools/fit_kernel.py` & `discminer-0.2.3/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer/tools/utils.py` & `discminer-0.2.3/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/discminer.egg-info/PKG-INFO` & `discminer-0.2.3/discminer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.2 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.3 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.2/discminer.egg-info/SOURCES.txt` & `discminer-0.2.3/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/setup.py` & `discminer-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/template/README.rst` & `discminer-0.2.3/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/template/download_MAPS.sh` & `discminer-0.2.3/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.3/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.2/template/prepare_data.py` & `discminer-0.2.3/template/prepare_data.py`

 * *Files identical despite different names*

