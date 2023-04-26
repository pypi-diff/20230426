# Comparing `tmp/gwdetchar-2.0.7.tar.gz` & `tmp/gwdetchar-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.0.7.tar", last modified: Tue Apr 25 15:53:01 2023, max compression
+gzip compressed data, was "gwdetchar-2.0.8.tar", last modified: Tue Apr 25 23:12:37 2023, max compression
```

## Comparing `gwdetchar-2.0.7.tar` & `gwdetchar-2.0.8.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.311886 gwdetchar-2.0.7/
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)      100 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 15:53:01.312105 gwdetchar-2.0.7/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.313414 gwdetchar-2.0.7/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1113 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-04-25 15:53:01.313619 gwdetchar-2.0.7/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4716 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.0.7/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3044 2023-04-25 15:49:41.000000 gwdetchar-2.0.7/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.271388 gwdetchar-2.0.7/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7367 2023-02-28 19:11:25.000000 gwdetchar-2.0.7/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41524 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.274670 gwdetchar-2.0.7/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    23271 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.279403 gwdetchar-2.0.7/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35157 2022-10-03 17:36:21.000000 gwdetchar-2.0.7/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.0.7/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.282303 gwdetchar-2.0.7/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3965 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.284438 gwdetchar-2.0.7/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.285860 gwdetchar-2.0.7/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.291169 gwdetchar-2.0.7/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12666 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.296232 gwdetchar-2.0.7/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13619 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.298131 gwdetchar-2.0.7/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.299403 gwdetchar-2.0.7/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.302931 gwdetchar-2.0.7/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.306018 gwdetchar-2.0.7/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.311295 gwdetchar-2.0.7/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.0.7/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.0.7/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 15:53:01.268432 gwdetchar-2.0.7/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2419 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-02 22:06:25.000000 gwdetchar-2.0.7/gwdetchar.egg-info/not-zip-safe
--rw-r--r--   0 egoetz     (501) staff       (20)      292 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-04-25 15:53:01.000000 gwdetchar-2.0.7/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3000 2023-04-25 15:53:01.313063 gwdetchar-2.0.7/setup.cfg
--rw-r--r--   0 egoetz     (501) staff       (20)     1205 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/setup.py
--rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-04-24 20:03:47.000000 gwdetchar-2.0.7/versioneer.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.721923 gwdetchar-2.0.8/
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)      100 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 23:12:37.722127 gwdetchar-2.0.8/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.724659 gwdetchar-2.0.8/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1113 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-04-25 23:12:37.724775 gwdetchar-2.0.8/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4716 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3044 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.691360 gwdetchar-2.0.8/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7367 2023-02-28 19:11:25.000000 gwdetchar-2.0.8/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41524 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.693427 gwdetchar-2.0.8/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24193 2023-04-25 22:58:28.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.696694 gwdetchar-2.0.8/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    35157 2022-10-03 17:36:21.000000 gwdetchar-2.0.8/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.0.8/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.699200 gwdetchar-2.0.8/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3965 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.700826 gwdetchar-2.0.8/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.701964 gwdetchar-2.0.8/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.705942 gwdetchar-2.0.8/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12666 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.710132 gwdetchar-2.0.8/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13619 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.711554 gwdetchar-2.0.8/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.712423 gwdetchar-2.0.8/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.714717 gwdetchar-2.0.8/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.716918 gwdetchar-2.0.8/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.721562 gwdetchar-2.0.8/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.0.8/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.0.8/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-25 23:12:37.689130 gwdetchar-2.0.8/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2419 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-02 22:06:25.000000 gwdetchar-2.0.8/gwdetchar.egg-info/not-zip-safe
+-rw-r--r--   0 egoetz     (501) staff       (20)      292 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-04-25 23:12:37.000000 gwdetchar-2.0.8/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3000 2023-04-25 23:12:37.724103 gwdetchar-2.0.8/setup.cfg
+-rw-r--r--   0 egoetz     (501) staff       (20)     1205 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/setup.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-04-24 20:03:47.000000 gwdetchar-2.0.8/versioneer.py
```

### Comparing `gwdetchar-2.0.7/LICENSE` & `gwdetchar-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/PKG-INFO` & `gwdetchar-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.7
+Version: 2.0.8
 Summary: A python package for gravitational-wave detector characterisation
 Home-page: https://github.com/gwdetchar/gwdetchar/
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gwdetchar-2.0.7/README.rst` & `gwdetchar-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/__init__.py` & `gwdetchar-2.0.8/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/cds.py` & `gwdetchar-2.0.8/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/cli.py` & `gwdetchar-2.0.8/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/condor.py` & `gwdetchar-2.0.8/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/conftest.py` & `gwdetchar-2.0.8/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/conlog.py` & `gwdetchar-2.0.8/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/const.py` & `gwdetchar-2.0.8/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/daq.py` & `gwdetchar-2.0.8/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/__init__.py` & `gwdetchar-2.0.8/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/datafind.py` & `gwdetchar-2.0.8/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/html.py` & `gwdetchar-2.0.8/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/ligolw.py` & `gwdetchar-2.0.8/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.0.8/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.0.8/gwdetchar/io/tests/test_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,37 +69,48 @@
 <div class="container">
 </body>
 </html>""" % (STYLESHEETS, SCRIPTS)
 
 TEST_CONFIGURATION = """[section]
 key = value"""
 
-if pygments_version >= "2.11.0":
+if pygments_version >= "2.14.0":
+    pygments_space_span = '<span style="color: #bbbbbb"> </span>'
+    pygments_output = (
+        '\n'
+        '<span style="color: #687822">key</span>'
+        f'{pygments_space_span}'
+        '<span style="color: #666666">=</span>'
+        f'{pygments_space_span}'
+        '<span style="color: #BA2121">value</span>'
+    )
+elif pygments_version >= "2.11.0":
     pygments_output = (
         '<span style="color: #bbbbbb"></span>\n'
         '<span style="color: #687822">key</span>'
         '<span style="color: #bbbbbb"> </span>'
         '<span style="color: #666666">=</span>'
         '<span style="color: #bbbbbb"> </span>'
         '<span style="color: #BA2121">value</span>'
         '<span style="color: #bbbbbb"></span>'
     )
+    pygments_space_span = ' '
 else:
     pygments_output = (
         '\n'
         '<span style="color: #7D9029">key</span> '
         '<span style="color: #666666">=</span> '
         '<span style="color: #BA2121">value</span>'
     )
 
 ABOUT = f"""<div class="row">
 <div class="col-md-12">
 <h2>On the command-line</h2>
 <p>This page was generated with the following command-line call:</p>
-<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span>$ gwdetchar-scattering -i X1
+<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span>${pygments_space_span}gwdetchar-scattering{pygments_space_span}-i{pygments_space_span}X1
 </pre></div>
 
 <p>The install path used was <code>{sys.prefix}</code>.</p>
 <h2>Configuration files</h2>
 <p>The following INI-format configuration file(s) were passed on the comand-line and are reproduced here in full:</p>
 <div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span><span style="color: #008000; font-weight: bold">[section]</span>{pygments_output}
 </pre></div>
@@ -108,15 +119,15 @@
 </div>
 </div>"""  # noqa: E501
 
 ABOUT_WITH_CONFIG_LIST = f"""<div class="row">
 <div class="col-md-12">
 <h2>On the command-line</h2>
 <p>This page was generated with the following command-line call:</p>
-<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span>$ gwdetchar-scattering -i X1
+<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span>${pygments_space_span}gwdetchar-scattering{pygments_space_span}-i{pygments_space_span}X1
 </pre></div>
 
 <p>The install path used was <code>{sys.prefix}</code>.</p>
 <h2>Configuration files</h2>
 <p>The following INI-format configuration file(s) were passed on the comand-line and are reproduced here in full:</p>
 <div id="accordion">
 <div class="card mb-1 shadow-sm">
@@ -222,14 +233,20 @@
 </div>
 </div>
 </li>
 </ul>
 </div>
 </div>"""  # noqa: E501
 
+CMDLINE = f"""<p>This page was generated with the following command-line call:</p>
+<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span>${pygments_space_span}gwdetchar-conlog{pygments_space_span}-i{pygments_space_span}X1
+</pre></div>
+
+<p>The install path used was <code>{sys.prefix}.</p>"""  # noqa: E501
+
 
 # -- HTML unit tests ----------------------------------------------------------
 
 def test_fancy_plot():
     # create a dummy FancyPlot instance
     test = html.FancyPlot('test.png')
     assert test.img == 'test.png'
@@ -356,15 +373,16 @@
 
 def test_get_command_line():
     testargs = ['/opt/bin/gwdetchar-conlog',
                 '--html-only',
                 '-i', 'X1']
     with mock.patch.object(sys, 'argv', testargs):
         cmdline = str(html.get_command_line())
-        assert 'gwdetchar-conlog -i X1' in cmdline
+        assert (f'gwdetchar-conlog{pygments_space_span}-i'
+                f'{pygments_space_span}X1') in cmdline
         assert not ('--html-only' in cmdline)
         assert 'The install path used was <code>{}</code>'.format(
             sys.prefix) in cmdline
 
 
 @pytest.mark.parametrize('args, kwargs, result', [
     (('test.html', 'Test link'), {},
```

#### html2text {}

```diff
@@ -20,19 +20,23 @@
 '.format(css) for css in html.CSS_FILES]) SCRIPTS = '\n'.join([ '
 '.format(js) for js in html.JS_FILES]) NEW_BOOTSTRAP_PAGE = """
 
 
 
  %s %s
 """ % (STYLESHEETS, SCRIPTS) TEST_CONFIGURATION = """[section] key = value"""
-if pygments_version >= "2.11.0": pygments_output = ( '\n' 'key' ' ' '=' ' '
-'value' '' ) else: pygments_output = ( '\n' 'key ' '= ' 'value' ) ABOUT = f"""
+if pygments_version >= "2.14.0": pygments_space_span = ' ' pygments_output =
+( '\n' 'key' f'{pygments_space_span}' '=' f'{pygments_space_span}' 'value' )
+elif pygments_version >= "2.11.0": pygments_output = ( '\n' 'key' ' ' '=' ' '
+'value' '' ) pygments_space_span = ' ' else: pygments_output = ( '\n' 'key ' '=
+' 'value' ) ABOUT = f"""
 ***** On the command-line *****
 This page was generated with the following command-line call:
-$ gwdetchar-scattering -i X1
+${pygments_space_span}gwdetchar-scattering{pygments_space_span}-i
+{pygments_space_span}X1
 The install path used was {sys.prefix}.
 ***** Configuration files *****
 The following INI-format configuration file(s) were passed on the comand-line
 and are reproduced here in full:
 [section]{pygments_output}
 ***** Environment *****
 Table of packages
@@ -42,15 +46,16 @@
 Name      Version
 gwdetchar 1.2.3
 gwpy      1.0.0
 Export to CSV
 """ # noqa: E501 ABOUT_WITH_CONFIG_LIST = f"""
 ***** On the command-line *****
 This page was generated with the following command-line call:
-$ gwdetchar-scattering -i X1
+${pygments_space_span}gwdetchar-scattering{pygments_space_span}-i
+{pygments_space_span}X1
 The install path used was {sys.prefix}.
 ***** Configuration files *****
 The following INI-format configuration file(s) were passed on the comand-line
 and are reproduced here in full:
 test.ini
 [section]{pygments_output}
 ***** Environment *****
@@ -91,14 +96,19 @@
 ', plots='') FLAG = DataQualityFlag(known=[(0, 66)], active=[(0, 66)],
 name='X1:TEST_FLAG') OMEGA_SCAFFOLD = """
 ** X1:STRAIN **
     * * 1126259462 *
       [X1-STRAIN-qscan_whitened-1.png]
       [X1-STRAIN-qscan_whitened-4.png]
       [X1-STRAIN-qscan_whitened-16.png]
+""" # noqa: E501 CMDLINE = f"""
+This page was generated with the following command-line call:
+${pygments_space_span}gwdetchar-conlog{pygments_space_span}-i
+{pygments_space_span}X1
+The install path used was {sys.prefix}.
 """ # noqa: E501 # -- HTML unit tests -----------------------------------------
 ----------------- def test_fancy_plot(): # create a dummy FancyPlot instance
 test = html.FancyPlot('test.png') assert test.img == 'test.png' assert
 test.caption == 'test.png' # check that its properties are unchanged when the
 argument # to FancyPlot() is also a FancyPlot instance test = html.FancyPlot
 (test) assert test.img == 'test.png' assert test.caption == 'test.png' def
 test_finalize_static_urls(tmpdir): base = str(tmpdir) static = os.path.join
@@ -166,24 +176,25 @@
 scattering', '-i', 'X1'] with mock.patch.object(sys, 'argv', testargs): # test
 with a single config file about = html.about_this_page(config_file) assert
 parse_html(about) == parse_html(ABOUT) # test with a list of config files about
 = html.about_this_page([config_file]) assert parse_html(about) == parse_html
 (ABOUT_WITH_CONFIG_LIST) # clean up shutil.rmtree(outdir, ignore_errors=True)
 def test_get_command_line(): testargs = ['/opt/bin/gwdetchar-conlog', '--html-
 only', '-i', 'X1'] with mock.patch.object(sys, 'argv', testargs): cmdline = str
-(html.get_command_line()) assert 'gwdetchar-conlog -i X1' in cmdline assert not
-('--html-only' in cmdline) assert 'The install path used was {}'.format
-( sys.prefix) in cmdline @pytest.mark.parametrize('args, kwargs, result', [ (
-('test.html', 'Test link'), {}, 'Test_link'), (('test.html', 'Test link'),
-{'class_': 'test-case'}, 'Test_link'), ]) def test_html_link(args, kwargs,
-result): h1 = parse_html(html.html_link(*args, **kwargs)) h2 = parse_html
-(result) assert h1 == h2 def test_cis_link(): h1 = parse_html(html.cis_link
-('X1:TEST-CHANNEL')) h2 = parse_html( 'X1:TEST-CHANNEL' ) assert h1 == h2 def
-test_fancybox_img(): img = html.FancyPlot('X1-TEST_AUX-test-4.png') out =
-html.fancybox_img(img) assert parse_html(out) == parse_html( '
+(html.get_command_line()) assert (f'gwdetchar-conlog{pygments_space_span}-i' f'
+{pygments_space_span}X1') in cmdline assert not ('--html-only' in cmdline)
+assert 'The install path used was {}'.format( sys.prefix) in cmdline
+@pytest.mark.parametrize('args, kwargs, result', [ (('test.html', 'Test link'),
+{}, 'Test_link'), (('test.html', 'Test link'), {'class_': 'test-case'}, 'Test
+link'), ]) def test_html_link(args, kwargs, result): h1 = parse_html
+(html.html_link(*args, **kwargs)) h2 = parse_html(result) assert h1 == h2 def
+test_cis_link(): h1 = parse_html(html.cis_link('X1:TEST-CHANNEL')) h2 =
+parse_html( 'X1:TEST-CHANNEL' ) assert h1 == h2 def test_fancybox_img(): img =
+html.FancyPlot('X1-TEST_AUX-test-4.png') out = html.fancybox_img(img) assert
+parse_html(out) == parse_html( '
  'title="X1-TEST_AUX-test-4.png" class="fancybox" target="_blank" ' 'data-
 caption="X1-TEST_AUX-test-4.png" data-fancybox="gallery" ' 'data-fancybox-
 group="images">\n
  'alt="X1-TEST_AUX-test-4.png" class="img-fluid w-100" ' 'src="X1-TEST_AUX-
 test-4.png" />\n
 ') def test_scaffold_plots(): h1 = html.scaffold_plots([ html.FancyPlot('X1-
 TEST_AUX-test-4.png'), html.FancyPlot('X1-TEST_AUX-test-16.png')], nperrow=2)
```

### Comparing `gwdetchar-2.0.7/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.0.8/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/__init__.py` & `gwdetchar-2.0.8/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/__main__.py` & `gwdetchar-2.0.8/gwdetchar/lasso/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/core.py` & `gwdetchar-2.0.8/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/old.py` & `gwdetchar-2.0.8/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/plot.py` & `gwdetchar-2.0.8/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.0.8/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/mct.py` & `gwdetchar-2.0.8/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/nagios/__init__.py` & `gwdetchar-2.0.8/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/nagios/__main__.py` & `gwdetchar-2.0.8/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/nagios/core.py` & `gwdetchar-2.0.8/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.0.8/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/__init__.py` & `gwdetchar-2.0.8/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/__main__.py` & `gwdetchar-2.0.8/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/batch.py` & `gwdetchar-2.0.8/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/config.py` & `gwdetchar-2.0.8/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/core.py` & `gwdetchar-2.0.8/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/html.py` & `gwdetchar-2.0.8/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/plot.py` & `gwdetchar-2.0.8/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.0.8/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/overflow.py` & `gwdetchar-2.0.8/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/plot.py` & `gwdetchar-2.0.8/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/saturation/__init__.py` & `gwdetchar-2.0.8/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/saturation/__main__.py` & `gwdetchar-2.0.8/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/saturation/core.py` & `gwdetchar-2.0.8/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.0.8/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/__init__.py` & `gwdetchar-2.0.8/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/__main__.py` & `gwdetchar-2.0.8/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/core.py` & `gwdetchar-2.0.8/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/plot.py` & `gwdetchar-2.0.8/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/simple.py` & `gwdetchar-2.0.8/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.0.8/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/__init__.py` & `gwdetchar-2.0.8/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_cds.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_cli.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_condor.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_const.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_daq.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_plot.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/tests/test_utils.py` & `gwdetchar-2.0.8/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar/utils.py` & `gwdetchar-2.0.8/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.0.8/gwdetchar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.7
+Version: 2.0.8
 Summary: A python package for gravitational-wave detector characterisation
 Home-page: https://github.com/gwdetchar/gwdetchar/
 Author: Alex Urban, Duncan Macleod
 Author-email: alexander.urban@ligo.org
 License: GPL-3.0-or-later
 Keywords: physics,astronomy,gravitational-waves,ligo
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gwdetchar-2.0.7/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.0.8/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.0.8/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/setup.cfg` & `gwdetchar-2.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/setup.py` & `gwdetchar-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.7/versioneer.py` & `gwdetchar-2.0.8/versioneer.py`

 * *Files identical despite different names*

