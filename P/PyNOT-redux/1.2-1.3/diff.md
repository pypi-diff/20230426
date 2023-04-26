# Comparing `tmp/PyNOT-redux-1.2.tar.gz` & `tmp/PyNOT-redux-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNOT-redux-1.2.tar", last modified: Tue Apr 25 06:53:49 2023, max compression
+gzip compressed data, was "PyNOT-redux-1.3.tar", last modified: Tue Apr 25 14:38:29 2023, max compression
```

## Comparing `PyNOT-redux-1.2.tar` & `PyNOT-redux-1.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.379552 PyNOT-redux-1.2/
--rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-04-24 12:09:15.000000 PyNOT-redux-1.2/.DS_Store
--rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/.gitattributes
--rw-r--r--   0 krogager   (501) staff       (20)     1878 2022-05-09 07:03:03.000000 PyNOT-redux-1.2/.gitignore
--rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 06:53:49.379227 PyNOT-redux-1.2/PKG-INFO
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.365605 PyNOT-redux-1.2/PyNOT_redux.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       42 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)      113 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-04-25 06:53:49.000000 PyNOT-redux-1.2/PyNOT_redux.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/README.md
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.372052 PyNOT-redux-1.2/pynot/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.extract_msg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.identify_msg
--rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.2/pynot/.instrument.cfg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/.response_msg
--rw-r--r--   0 krogager   (501) staff       (20)        4 2023-04-25 06:53:37.000000 PyNOT-redux-1.2/pynot/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.2/pynot/alfosc.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.374581 PyNOT-redux-1.2/pynot/calib/
--rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/HeAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/HeNe_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ThAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr18_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr19_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr4_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/al-gr7_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/alfosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/default_options.yml
--rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/calib/default_options_img.yml
--rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr13_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr14_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr1_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/ef-gr3_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/efosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/lapalma.ext
--rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/lasilla.ext
--rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/paranal.ext
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.377807 PyNOT-redux-1.2/pynot/calib/std/
--rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd174708.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd262606.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd332642.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/bd75325.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/eg21.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/feige110.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/feige34.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd153.dat
--rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd50.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/gd71.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd19445.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd84937.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hd93521.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/he3.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/hiltner600.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/ltt3864.dat
--rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/tcs_namelist.txt
--rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/calib/std/wolf1346.dat
--rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.2/pynot/calibs.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.378590 PyNOT-redux-1.2/pynot/data/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/alfosc.rules
--rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/efosc.rules
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 06:53:49.379022 PyNOT-redux-1.2/pynot/data/help/
--rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_extract.html
--rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_identify.html
--rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/help/welcome_msg_response.html
--rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/io.py
--rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/obs.py
--rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/data/organizer.py
--rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.2/pynot/efosc.py
--rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.2/pynot/extract_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.2/pynot/extraction.py
--rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/fitsio.py
--rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/functions.py
--rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.2/pynot/identify_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.2/pynot/insconfig.py
--rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/logging.py
--rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/main.py
--rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.2/pynot/phot.py
--rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/phot_redux.py
--rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.2/pynot/redux.py
--rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/reports.py
--rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/response.py
--rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/response_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.2/pynot/scired.py
--rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.2/pynot/scombine.py
--rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/tasks.py
--rw-r--r--   0 krogager   (501) staff       (20)     9248 2022-06-07 07:35:54.000000 PyNOT-redux-1.2/pynot/transients.py
--rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.2/pynot/txtio.py
--rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/wavecal.py
--rw-r--r--   0 krogager   (501) staff       (20)    13375 2023-04-25 06:53:15.000000 PyNOT-redux-1.2/pynot/wcs.py
--rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pynot/welcome.py
--rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.2/pyproject.toml
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-04-25 06:53:49.379582 PyNOT-redux-1.2/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.2/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.634014 PyNOT-redux-1.3/
+-rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-04-24 12:09:15.000000 PyNOT-redux-1.3/.DS_Store
+-rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/.gitattributes
+-rw-r--r--   0 krogager   (501) staff       (20)     1878 2022-05-09 07:03:03.000000 PyNOT-redux-1.3/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 14:38:29.633835 PyNOT-redux-1.3/PKG-INFO
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.617897 PyNOT-redux-1.3/PyNOT_redux.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)    13888 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       42 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      113 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-04-25 14:38:29.000000 PyNOT-redux-1.3/PyNOT_redux.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/README.md
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.625752 PyNOT-redux-1.3/pynot/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.extract_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.identify_msg
+-rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3/pynot/.instrument.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/.response_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        4 2023-04-25 14:38:05.000000 PyNOT-redux-1.3/pynot/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3/pynot/alfosc.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.629320 PyNOT-redux-1.3/pynot/calib/
+-rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/HeAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/HeNe_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ThAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr18_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr19_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr4_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/al-gr7_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/alfosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/default_options.yml
+-rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/calib/default_options_img.yml
+-rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr13_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr14_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr1_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/ef-gr3_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/efosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/lapalma.ext
+-rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/lasilla.ext
+-rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/paranal.ext
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.632424 PyNOT-redux-1.3/pynot/calib/std/
+-rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd174708.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd262606.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd332642.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/bd75325.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/eg21.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/feige110.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/feige34.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd153.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd50.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/gd71.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd19445.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd84937.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hd93521.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/he3.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/hiltner600.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/ltt3864.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/tcs_namelist.txt
+-rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/calib/std/wolf1346.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3/pynot/calibs.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.633157 PyNOT-redux-1.3/pynot/data/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/alfosc.rules
+-rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/efosc.rules
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-04-25 14:38:29.633623 PyNOT-redux-1.3/pynot/data/help/
+-rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_extract.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_identify.html
+-rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/help/welcome_msg_response.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/io.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/obs.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/data/organizer.py
+-rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3/pynot/efosc.py
+-rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3/pynot/extract_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3/pynot/extraction.py
+-rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/fitsio.py
+-rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/functions.py
+-rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3/pynot/identify_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3/pynot/insconfig.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/logging.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/main.py
+-rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3/pynot/phot.py
+-rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/phot_redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3/pynot/redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/reports.py
+-rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/response.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/response_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3/pynot/scired.py
+-rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3/pynot/scombine.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/tasks.py
+-rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3/pynot/transients.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3/pynot/txtio.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/wavecal.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13375 2023-04-25 06:53:15.000000 PyNOT-redux-1.3/pynot/wcs.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pynot/welcome.py
+-rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3/pyproject.toml
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2023-04-25 14:38:29.634047 PyNOT-redux-1.3/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3/setup.py
```

### Comparing `PyNOT-redux-1.2/.DS_Store` & `PyNOT-redux-1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/.gitignore` & `PyNOT-redux-1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/LICENSE` & `PyNOT-redux-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/PKG-INFO` & `PyNOT-redux-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.2
+Version: 1.3
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.2/PyNOT_redux.egg-info/PKG-INFO` & `PyNOT-redux-1.3/PyNOT_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.2
+Version: 1.3
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.2/PyNOT_redux.egg-info/SOURCES.txt` & `PyNOT-redux-1.3/PyNOT_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/README.md` & `PyNOT-redux-1.3/README.md`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/__init__.py` & `PyNOT-redux-1.3/pynot/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/alfosc.py` & `PyNOT-redux-1.3/pynot/alfosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/HeAr_linelist.dat` & `PyNOT-redux-1.3/pynot/calib/HeAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/HeNe_linelist.dat` & `PyNOT-redux-1.3/pynot/calib/HeNe_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/ThAr_linelist.dat` & `PyNOT-redux-1.3/pynot/calib/ThAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/alfosc_filters.dat` & `PyNOT-redux-1.3/pynot/calib/alfosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/default_options.yml` & `PyNOT-redux-1.3/pynot/calib/default_options.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/default_options_img.yml` & `PyNOT-redux-1.3/pynot/calib/default_options_img.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/efosc_filters.dat` & `PyNOT-redux-1.3/pynot/calib/efosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/lapalma.ext` & `PyNOT-redux-1.3/pynot/calib/lapalma.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/lasilla.ext` & `PyNOT-redux-1.3/pynot/calib/lasilla.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/paranal.ext` & `PyNOT-redux-1.3/pynot/calib/paranal.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/bd174708.dat` & `PyNOT-redux-1.3/pynot/calib/std/bd174708.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/bd262606.dat` & `PyNOT-redux-1.3/pynot/calib/std/bd262606.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/bd332642.dat` & `PyNOT-redux-1.3/pynot/calib/std/bd332642.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/bd75325.dat` & `PyNOT-redux-1.3/pynot/calib/std/bd75325.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/eg21.dat` & `PyNOT-redux-1.3/pynot/calib/std/eg21.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/feige110.dat` & `PyNOT-redux-1.3/pynot/calib/std/feige110.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/feige34.dat` & `PyNOT-redux-1.3/pynot/calib/std/feige34.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/gd153.dat` & `PyNOT-redux-1.3/pynot/calib/std/gd153.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/gd50.dat` & `PyNOT-redux-1.3/pynot/calib/std/gd50.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/gd71.dat` & `PyNOT-redux-1.3/pynot/calib/std/gd71.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/hd19445.dat` & `PyNOT-redux-1.3/pynot/calib/std/hd19445.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/hd84937.dat` & `PyNOT-redux-1.3/pynot/calib/std/hd84937.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/hd93521.dat` & `PyNOT-redux-1.3/pynot/calib/std/hd93521.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/he3.dat` & `PyNOT-redux-1.3/pynot/calib/std/he3.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/hiltner600.dat` & `PyNOT-redux-1.3/pynot/calib/std/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/ltt3864.dat` & `PyNOT-redux-1.3/pynot/calib/std/ltt3864.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calib/std/wolf1346.dat` & `PyNOT-redux-1.3/pynot/calib/std/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/calibs.py` & `PyNOT-redux-1.3/pynot/calibs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/alfosc.rules` & `PyNOT-redux-1.3/pynot/data/alfosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/efosc.rules` & `PyNOT-redux-1.3/pynot/data/efosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/help/welcome_msg_extract.html` & `PyNOT-redux-1.3/pynot/data/help/welcome_msg_extract.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/help/welcome_msg_identify.html` & `PyNOT-redux-1.3/pynot/data/help/welcome_msg_identify.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/help/welcome_msg_response.html` & `PyNOT-redux-1.3/pynot/data/help/welcome_msg_response.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/io.py` & `PyNOT-redux-1.3/pynot/data/io.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/obs.py` & `PyNOT-redux-1.3/pynot/data/obs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/data/organizer.py` & `PyNOT-redux-1.3/pynot/data/organizer.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/efosc.py` & `PyNOT-redux-1.3/pynot/efosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/extract_gui.py` & `PyNOT-redux-1.3/pynot/extract_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/extraction.py` & `PyNOT-redux-1.3/pynot/extraction.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/fitsio.py` & `PyNOT-redux-1.3/pynot/fitsio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/functions.py` & `PyNOT-redux-1.3/pynot/functions.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/identify_gui.py` & `PyNOT-redux-1.3/pynot/identify_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/insconfig.py` & `PyNOT-redux-1.3/pynot/insconfig.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/logging.py` & `PyNOT-redux-1.3/pynot/logging.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/main.py` & `PyNOT-redux-1.3/pynot/main.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/phot.py` & `PyNOT-redux-1.3/pynot/phot.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/phot_redux.py` & `PyNOT-redux-1.3/pynot/phot_redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/redux.py` & `PyNOT-redux-1.3/pynot/redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/reports.py` & `PyNOT-redux-1.3/pynot/reports.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/response.py` & `PyNOT-redux-1.3/pynot/response.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/response_gui.py` & `PyNOT-redux-1.3/pynot/response_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/scired.py` & `PyNOT-redux-1.3/pynot/scired.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/scombine.py` & `PyNOT-redux-1.3/pynot/scombine.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/tasks.py` & `PyNOT-redux-1.3/pynot/tasks.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/transients.py` & `PyNOT-redux-1.3/pynot/transients.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from astropy.wcs import WCS
 from astropy.io import fits
 from astropy.table import Table
 from astropy.utils.exceptions import AstropyWarning
+from astropy.coordinates import SkyCoord
+import astropy.units as u
 
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 import warnings
 
 from pynot.wcs import get_gaia_catalog
@@ -14,20 +16,37 @@
 
 
 def mad(x):
     return np.median(np.abs(x-np.median(x)))
 
 
 def find_sources_without_gaia(sep_cat, gaia, limit=1.5):
+    """
+    Find sources without a match in Gaia assuming a matching radius
+    
+    sep_cat : astropy.table.Table
+        A Table containing source photometry from the image.
+        Must contain the columns ra and dec in degrees.
+    
+    gaia : astropy.table.Table
+        A Table containing source photometry from the Gaia catalog.
+        Must contain the columns ra and dec in degrees.
+    
+    limit : float  [default=1.5]
+        The matching radius in arcsec.
+    
+    Returns
+        astropy.table.Table of the sources with no match in Gaia
+    """
     no_match_list = list()
-    refs = np.array([gaia['ra'], gaia['dec']]).T
+    pos_gaia = SkyCoord(gaia['ra']*u.deg, gaia['dec']*u.deg, frame='icrs')
     for row in sep_cat:
-        xy = np.array([row['ra'], row['dec']])
-        dist = np.sqrt(np.sum((refs - xy)**2, axis=1))
-        if np.min(dist) < limit/3600.:
+        pos = SkyCoord(row['ra']*u.deg, row['dec']*u.deg, frame='icrs')
+        dist = pos.separation(pos_gaia)
+        if np.min(dist) < limit*u.arcsec:
             pass
         else:
             no_match_list.append(np.array(row))
     no_match_list = np.array(no_match_list)
     return Table(no_match_list)
```

### Comparing `PyNOT-redux-1.2/pynot/txtio.py` & `PyNOT-redux-1.3/pynot/txtio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/wavecal.py` & `PyNOT-redux-1.3/pynot/wavecal.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/wcs.py` & `PyNOT-redux-1.3/pynot/wcs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/pynot/welcome.py` & `PyNOT-redux-1.3/pynot/welcome.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.2/setup.py` & `PyNOT-redux-1.3/setup.py`

 * *Files identical despite different names*

