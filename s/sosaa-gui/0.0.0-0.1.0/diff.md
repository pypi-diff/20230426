# Comparing `tmp/sosaa-gui-0.0.0.tar.gz` & `tmp/sosaa-gui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sosaa-gui/sosaa-gui/dist/.tmp-w_d9q_s7/sosaa-gui-0.0.0.tar", last modified: Wed Apr 26 16:39:12 2023, max compression
+gzip compressed data, was "/home/runner/work/sosaa-gui/sosaa-gui/dist/.tmp-1mjy_t4h/sosaa-gui-0.1.0.tar", last modified: Wed Apr 26 17:03:03 2023, max compression
```

## Comparing `sosaa-gui-0.0.0.tar` & `sosaa-gui-0.1.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/LICENSE-GPL
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44818 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/conf/minimal.init
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/browse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/loadsave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/ccn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/rsm/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/gui/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/load.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/recompile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/save-as.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/save-defaults.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/save-inactive.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/save.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-splash-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-splash-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/layouts/about.py
--rw-r--r--   0 runner    (1001) docker     (123)   134791 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/layouts/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/settings/from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/settings/from_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/clump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/expand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/aerosol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/anthropogenic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/biogenic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/meteorology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/ccn.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/icarus/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/icarus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/icarus/analyse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/perturb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/sosaa_padre_rf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/sosaa_rf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 16:38:58.000000 sosaa-gui-0.0.0/sosaa_gui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44818 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 16:39:12.000000 sosaa-gui-0.0.0/sosaa_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/LICENSE-GPL
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44818 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/conf/minimal.init
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/browse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/loadsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/ccn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/rsm/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/gui/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/load.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/recompile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/save-as.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/save-defaults.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/save-inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-splash-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-splash-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/layouts/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134791 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/layouts/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/settings/from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/settings/from_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/clump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/expand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/aerosol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/anthropogenic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/biogenic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/meteorology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/ccn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/icarus/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/icarus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/icarus/analyse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/perturb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:03.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/sosaa_padre_rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/sosaa_rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 17:02:50.000000 sosaa-gui-0.1.0/sosaa_gui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44818 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 17:03:02.000000 sosaa-gui-0.1.0/sosaa_gui.egg-info/top_level.txt
```

### Comparing `sosaa-gui-0.0.0/LICENSE` & `sosaa-gui-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/LICENSE-GPL` & `sosaa-gui-0.1.0/LICENSE-GPL`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/PKG-INFO` & `sosaa-gui-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosaa-gui
-Version: 0.0.0
+Version: 0.1.0
 Summary: Graphical User Interface for Configuring, Running, and Approximating the SOSAA Model
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>, Petri Clusius <petri.clusius@helsinki.fi>, Multi-Scale Modelling group <sosaa@helsinki.fi>
 Maintainer-email: Multi-Scale Modelling group <sosaa@helsinki.fi>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `sosaa-gui-0.0.0/README.md` & `sosaa-gui-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/pyproject.toml` & `sosaa-gui-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sosaa-gui"
-version = "0.0.0"
+version = "0.1.0"
 requires-python = ">=3.7"
 description = "Graphical User Interface for Configuring, Running, and Approximating the SOSAA Model"
 readme = "README.md"
 license = { file = "LICENSE-GPL" }
 authors = [
     { name = "Juniper Tyree", email = "juniper.tyree@helsinki.fi" },
     { name = "Petri Clusius", email = "petri.clusius@helsinki.fi" },
@@ -53,15 +53,15 @@
 profile = "black"
 line_length = 79
 
 [tool.flake8]
 exclude = "sosaa_gui/layouts/*.py"
 
 [tool.bumpver]
-current_version = "0.0.0"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `sosaa-gui-0.0.0/sosaa_gui/__main__.py` & `sosaa-gui-0.1.0/sosaa_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/conf/minimal.init` & `sosaa-gui-0.1.0/sosaa_gui/conf/minimal.init`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/config.py` & `sosaa-gui-0.1.0/sosaa_gui/config.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/browse.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/browse.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/compile.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/compile.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/dirs.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/dirs.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/help.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/help.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/loadsave.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/loadsave.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/modules.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/modules.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/output.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/output.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/build.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/build.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from .diff import update_plot as _update_diff_plot
 
 
 def update_rsm_plots(gui):
     if gui.rsm_plots_dirty:
         _init_rsm_plots(gui)
 
+        if not getattr(gui, "rsm_plot_init", False):
+            return
+
         _update_ccn_plot(gui)
         _update_diff_plot(gui)
 
     gui.rsm_plots_dirty = False
 
 
 def _init_rsm_plots(gui):
```

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/ccn.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/ccn.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/plot/diff.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/plot/diff.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/predict.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/predict.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/progress.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/progress.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/rsm/worker.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/rsm/worker.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/run.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/run.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/scenario.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/scenario.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/style.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/style.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/syntax.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/syntax.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/gui/terminal.py` & `sosaa-gui-0.1.0/sosaa_gui/gui/terminal.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/load.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/load.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/recompile.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/recompile.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/save-as.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/save-defaults.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/save-defaults.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/save-inactive.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/save-inactive.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/save.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/save.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-icon.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-icon.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-splash-dark.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-splash-dark.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/icons/sosaa-splash-light.svg` & `sosaa-gui-0.1.0/sosaa_gui/icons/sosaa-splash-light.svg`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/layouts/about.py` & `sosaa-gui-0.1.0/sosaa_gui/layouts/about.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/layouts/gui.py` & `sosaa-gui-0.1.0/sosaa_gui/layouts/gui.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/qt.py` & `sosaa-gui-0.1.0/sosaa_gui/qt.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/settings/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/settings/from_file.py` & `sosaa-gui-0.1.0/sosaa_gui/settings/from_file.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/settings/from_gui.py` & `sosaa-gui-0.1.0/sosaa_gui/settings/from_gui.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/clump.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/clump.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/expand.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/expand.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/aerosol.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/aerosol.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/anthropogenic.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/anthropogenic.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/biogenic.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/biogenic.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/features/extract/meteorology.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/features/extract/meteorology.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/labels/ccn.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/labels/ccn.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/netcdf.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/netcdf.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/paths.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/paths.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/dataset/utils.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/icarus/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/icarus/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/icarus/analyse.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/icarus/analyse.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/__init__.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/evaluate.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/evaluate.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/model/perturb.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/model/perturb.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/sosaa_padre_rf.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/sosaa_padre_rf.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/sosaa_rsm/rsms/sosaa_rf.py` & `sosaa-gui-0.1.0/sosaa_gui/sosaa_rsm/rsms/sosaa_rf.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui/style.py` & `sosaa-gui-0.1.0/sosaa_gui/style.py`

 * *Files identical despite different names*

### Comparing `sosaa-gui-0.0.0/sosaa_gui.egg-info/PKG-INFO` & `sosaa-gui-0.1.0/sosaa_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosaa-gui
-Version: 0.0.0
+Version: 0.1.0
 Summary: Graphical User Interface for Configuring, Running, and Approximating the SOSAA Model
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>, Petri Clusius <petri.clusius@helsinki.fi>, Multi-Scale Modelling group <sosaa@helsinki.fi>
 Maintainer-email: Multi-Scale Modelling group <sosaa@helsinki.fi>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `sosaa-gui-0.0.0/sosaa_gui.egg-info/SOURCES.txt` & `sosaa-gui-0.1.0/sosaa_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

