# Comparing `tmp/anzo_jupyter-2.2.3.tar.gz` & `tmp/anzo_jupyter-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anzo_jupyter-2.2.3.tar", last modified: Wed Mar 15 16:10:12 2023, max compression
+gzip compressed data, was "anzo_jupyter-2.2.4.tar", last modified: Tue Apr 25 17:26:07 2023, max compression
```

## Comparing `anzo_jupyter-2.2.3.tar` & `anzo_jupyter-2.2.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/
--rw-r--r--   0 silverfang   (501) staff       (20)    13296 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/PKG-INFO
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter/
--rw-r--r--   0 silverfang   (501) staff       (20)     3924 2022-08-17 19:41:12.000000 anzo_jupyter-2.2.3/anzo_jupyter/secrets_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     9796 2023-03-15 16:08:29.000000 anzo_jupyter-2.2.3/anzo_jupyter/graph_vis.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1335 2022-08-17 19:40:16.000000 anzo_jupyter-2.2.3/anzo_jupyter/anzo_jupyter_util.py
--rw-r--r--   0 silverfang   (501) staff       (20)      522 2021-04-12 15:36:53.000000 anzo_jupyter-2.2.3/anzo_jupyter/__init__.py
--rw-r--r--   0 silverfang   (501) staff       (20)    19933 2022-08-17 19:50:46.000000 anzo_jupyter-2.2.3/anzo_jupyter/anzo_jupyter.py
--rw-r--r--   0 silverfang   (501) staff       (20)     5030 2022-08-17 19:40:49.000000 anzo_jupyter-2.2.3/anzo_jupyter/arrow_flight_magics.py
--rw-r--r--   0 silverfang   (501) staff       (20)     7899 2022-08-17 19:40:23.000000 anzo_jupyter-2.2.3/anzo_jupyter/anzo_magics.py
--rw-r--r--   0 silverfang   (501) staff       (20)     5144 2022-08-17 19:40:31.000000 anzo_jupyter-2.2.3/anzo_jupyter/anzo_managers.py
--rw-r--r--   0 silverfang   (501) staff       (20)     3574 2022-08-17 19:40:43.000000 anzo_jupyter-2.2.3/anzo_jupyter/anzo_queries.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/
--rw-r--r--   0 silverfang   (501) staff       (20)    13296 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2021-01-06 22:01:00.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/not-zip-safe
--rw-r--r--   0 silverfang   (501) staff       (20)     1822 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 silverfang   (501) staff       (20)       20 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 silverfang   (501) staff       (20)       13 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/top_level.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/anzo_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        0 2023-03-15 16:05:24.000000 anzo_jupyter-2.2.3/LICENSE
--rw-r--r--   0 silverfang   (501) staff       (20)      955 2023-03-15 16:05:24.000000 anzo_jupyter-2.2.3/pyproject.toml
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/
--rw-r--r--   0 silverfang   (501) staff       (20)    28535 2022-08-17 19:37:09.000000 anzo_jupyter-2.2.3/tests/test_basic.py
--rw-r--r--   0 silverfang   (501) staff       (20)      338 2021-03-29 18:02:58.000000 anzo_jupyter-2.2.3/tests/test_common.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1624 2021-03-31 14:54:15.000000 anzo_jupyter-2.2.3/tests/test_flight_magics.py
--rw-r--r--   0 silverfang   (501) staff       (20)     5210 2021-03-31 14:54:15.000000 anzo_jupyter-2.2.3/tests/sample_flight_server.py
--rw-r--r--   0 silverfang   (501) staff       (20)        0 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/tests/__init__.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/trig/
--rwxr-xr-x   0 silverfang   (501) staff       (20)    23048 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)     3210 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
--rw-r--r--   0 silverfang   (501) staff       (20)     3426 2021-04-23 02:03:17.000000 anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_AZG.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/
--rw-r--r--   0 silverfang   (501) staff       (20)     3483 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/flds.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
--rw-r--r--   0 silverfang   (501) staff       (20)      339 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
--rw-r--r--   0 silverfang   (501) staff       (20)       39 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
--rw-r--r--   0 silverfang   (501) staff       (20)      154 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/onts/
--rw-r--r--   0 silverfang   (501) staff       (20)     3237 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
--rw-r--r--   0 silverfang   (501) staff       (20)       50 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
--rw-r--r--   0 silverfang   (501) staff       (20)      102 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/.lsdir
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/export_flds/
--rw-r--r--   0 silverfang   (501) staff       (20)     4126 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.3/tests/test_assets/export_flds/flds.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/tests/test_assets/export_flds/onts/
--rw-r--r--   0 silverfang   (501) staff       (20)     3237 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.3/tests/test_assets/export_flds/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
--rw-r--r--   0 silverfang   (501) staff       (20)       50 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.3/tests/test_assets/export_flds/onts/.ontsdir
--rw-r--r--   0 silverfang   (501) staff       (20)     4158 2021-06-15 15:33:58.000000 anzo_jupyter-2.2.3/tests/test_graph_vis.py
--rw-r--r--   0 silverfang   (501) staff       (20)      247 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/MANIFEST.in
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/docs/
--rw-r--r--   0 silverfang   (501) staff       (20)      298 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/index.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       34 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/contributing.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      613 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/Makefile
--rwxr-xr-x   0 silverfang   (501) staff       (20)     4927 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/conf.py
--rw-r--r--   0 silverfang   (501) staff       (20)      353 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/anzo_jupyter.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       73 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/modules.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       31 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/usage.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      774 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/make.bat
--rw-r--r--   0 silverfang   (501) staff       (20)       29 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/history.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       74 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/installation.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       28 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.3/docs/readme.rst
--rw-r--r--   0 silverfang   (501) staff       (20)    10299 2022-08-19 02:09:29.000000 anzo_jupyter-2.2.3/README.md
--rw-r--r--   0 silverfang   (501) staff       (20)     1376 2023-03-15 16:07:05.000000 anzo_jupyter-2.2.3/setup.py
--rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-03-15 16:10:12.000000 anzo_jupyter-2.2.3/setup.cfg
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.050788 anzo_jupyter-2.2.4/
+-rw-r--r--   0 silverfang   (501) staff       (20)        0 2023-03-15 16:05:24.000000 anzo_jupyter-2.2.4/LICENSE
+-rw-r--r--   0 silverfang   (501) staff       (20)      247 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/MANIFEST.in
+-rw-r--r--   0 silverfang   (501) staff       (20)    11127 2023-04-25 17:26:07.050924 anzo_jupyter-2.2.4/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)    10299 2022-08-19 02:09:29.000000 anzo_jupyter-2.2.4/README.md
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.035721 anzo_jupyter-2.2.4/anzo_jupyter/
+-rw-r--r--   0 silverfang   (501) staff       (20)      522 2021-04-12 15:36:53.000000 anzo_jupyter-2.2.4/anzo_jupyter/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    19933 2022-08-17 19:50:46.000000 anzo_jupyter-2.2.4/anzo_jupyter/anzo_jupyter.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1335 2022-08-17 19:40:16.000000 anzo_jupyter-2.2.4/anzo_jupyter/anzo_jupyter_util.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     7899 2022-08-17 19:40:23.000000 anzo_jupyter-2.2.4/anzo_jupyter/anzo_magics.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     5144 2022-08-17 19:40:31.000000 anzo_jupyter-2.2.4/anzo_jupyter/anzo_managers.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     3574 2022-08-17 19:40:43.000000 anzo_jupyter-2.2.4/anzo_jupyter/anzo_queries.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     5030 2022-08-17 19:40:49.000000 anzo_jupyter-2.2.4/anzo_jupyter/arrow_flight_magics.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     9796 2023-03-15 16:08:29.000000 anzo_jupyter-2.2.4/anzo_jupyter/graph_vis.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     3924 2022-08-17 19:41:12.000000 anzo_jupyter-2.2.4/anzo_jupyter/secrets_manager.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.037728 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/
+-rw-r--r--   0 silverfang   (501) staff       (20)    11127 2023-04-25 17:26:06.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)     1818 2023-04-25 17:26:07.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-04-25 17:26:06.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2021-01-06 22:01:00.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/not-zip-safe
+-rw-r--r--   0 silverfang   (501) staff       (20)      146 2023-04-25 17:26:06.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/requires.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)       13 2023-04-25 17:26:06.000000 anzo_jupyter-2.2.4/anzo_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.041587 anzo_jupyter-2.2.4/docs/
+-rw-r--r--   0 silverfang   (501) staff       (20)      613 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/Makefile
+-rw-r--r--   0 silverfang   (501) staff       (20)      353 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/anzo_jupyter.rst
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     4927 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/conf.py
+-rw-r--r--   0 silverfang   (501) staff       (20)       34 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/contributing.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       29 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/history.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      298 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/index.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       74 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/installation.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      774 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/make.bat
+-rw-r--r--   0 silverfang   (501) staff       (20)       73 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/modules.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       28 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/readme.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       31 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/docs/usage.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      955 2023-04-25 17:25:13.000000 anzo_jupyter-2.2.4/pyproject.toml
+-rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-04-25 17:26:07.051471 anzo_jupyter-2.2.4/setup.cfg
+-rw-r--r--   0 silverfang   (501) staff       (20)     1376 2023-04-25 17:25:22.000000 anzo_jupyter-2.2.4/setup.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.044247 anzo_jupyter-2.2.4/tests/
+-rw-r--r--   0 silverfang   (501) staff       (20)        0 2021-01-06 21:57:23.000000 anzo_jupyter-2.2.4/tests/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     5210 2021-03-31 14:54:15.000000 anzo_jupyter-2.2.4/tests/sample_flight_server.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.029360 anzo_jupyter-2.2.4/tests/test_assets/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.044748 anzo_jupyter-2.2.4/tests/test_assets/export_flds/
+-rw-r--r--   0 silverfang   (501) staff       (20)     4126 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.4/tests/test_assets/export_flds/flds.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.045662 anzo_jupyter-2.2.4/tests/test_assets/export_flds/onts/
+-rw-r--r--   0 silverfang   (501) staff       (20)       50 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.4/tests/test_assets/export_flds/onts/.ontsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3237 2021-09-13 15:53:36.000000 anzo_jupyter-2.2.4/tests/test_assets/export_flds/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.046576 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/
+-rw-r--r--   0 silverfang   (501) staff       (20)      102 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3483 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/flds.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.047364 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/onts/
+-rw-r--r--   0 silverfang   (501) staff       (20)       50 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3237 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.029085 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.029199 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.048674 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
+-rw-r--r--   0 silverfang   (501) staff       (20)      154 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
+-rw-r--r--   0 silverfang   (501) staff       (20)       39 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)      339 2022-08-17 19:36:42.000000 anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-25 17:26:07.050467 anzo_jupyter-2.2.4/tests/test_assets/trig/
+-rw-r--r--   0 silverfang   (501) staff       (20)     3426 2021-04-23 02:03:17.000000 anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_AZG.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)    23048 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     3210 2021-03-15 14:47:31.000000 anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)    28535 2022-08-17 19:37:09.000000 anzo_jupyter-2.2.4/tests/test_basic.py
+-rw-r--r--   0 silverfang   (501) staff       (20)      338 2021-03-29 18:02:58.000000 anzo_jupyter-2.2.4/tests/test_common.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1624 2021-03-31 14:54:15.000000 anzo_jupyter-2.2.4/tests/test_flight_magics.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     4158 2021-06-15 15:33:58.000000 anzo_jupyter-2.2.4/tests/test_graph_vis.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/secrets_manager.py` & `anzo_jupyter-2.2.4/anzo_jupyter/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/graph_vis.py` & `anzo_jupyter-2.2.4/anzo_jupyter/graph_vis.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/anzo_jupyter_util.py` & `anzo_jupyter-2.2.4/anzo_jupyter/anzo_jupyter_util.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/__init__.py` & `anzo_jupyter-2.2.4/anzo_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/anzo_jupyter.py` & `anzo_jupyter-2.2.4/anzo_jupyter/anzo_jupyter.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/arrow_flight_magics.py` & `anzo_jupyter-2.2.4/anzo_jupyter/arrow_flight_magics.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/anzo_magics.py` & `anzo_jupyter-2.2.4/anzo_jupyter/anzo_magics.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/anzo_managers.py` & `anzo_jupyter-2.2.4/anzo_jupyter/anzo_managers.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter/anzo_queries.py` & `anzo_jupyter-2.2.4/anzo_jupyter/anzo_queries.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/anzo_jupyter.egg-info/SOURCES.txt` & `anzo_jupyter-2.2.4/anzo_jupyter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 anzo_jupyter/anzo_queries.py
 anzo_jupyter/arrow_flight_magics.py
 anzo_jupyter/graph_vis.py
 anzo_jupyter/secrets_manager.py
 anzo_jupyter.egg-info/PKG-INFO
 anzo_jupyter.egg-info/SOURCES.txt
 anzo_jupyter.egg-info/dependency_links.txt
-anzo_jupyter.egg-info/entry_points.txt
 anzo_jupyter.egg-info/not-zip-safe
+anzo_jupyter.egg-info/requires.txt
 anzo_jupyter.egg-info/top_level.txt
 docs/Makefile
 docs/anzo_jupyter.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
```

### Comparing `anzo_jupyter-2.2.3/pyproject.toml` & `anzo_jupyter-2.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anzo_jupyter"
-version = "2.0.0"
+version = "2.2.4"
 authors = [
   { name="Tommy Fang, Adam Sachs, Alex Ledger", email="info@cambridgesemantics.com" },
 ]
 description = "Jupyter"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `anzo_jupyter-2.2.3/tests/test_basic.py` & `anzo_jupyter-2.2.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_flight_magics.py` & `anzo_jupyter-2.2.4/tests/test_flight_magics.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/sample_flight_server.py` & `anzo_jupyter-2.2.4/tests/sample_flight_server.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig` & `anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig` & `anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_AZG.trig` & `anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_AZG.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/trig/PyAnzo_Graphmart_export.trig` & `anzo_jupyter-2.2.4/tests/test_assets/trig/PyAnzo_Graphmart_export.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/flds.trig` & `anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/flds.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig` & `anzo_jupyter-2.2.4/tests/test_assets/export_flds/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/export_flds/flds.trig` & `anzo_jupyter-2.2.4/tests/test_assets/export_flds/flds.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_assets/export_flds/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig` & `anzo_jupyter-2.2.4/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/tests/test_graph_vis.py` & `anzo_jupyter-2.2.4/tests/test_graph_vis.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/docs/Makefile` & `anzo_jupyter-2.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/docs/conf.py` & `anzo_jupyter-2.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/docs/make.bat` & `anzo_jupyter-2.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/README.md` & `anzo_jupyter-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `anzo_jupyter-2.2.3/setup.py` & `anzo_jupyter-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords='anzo_jupyter',
     name='anzo_jupyter',
     packages=find_packages(include=['anzo_jupyter', 'anzo_jupyter.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='',
-    version='2.2.3',
+    version='2.2.4',
     zip_safe=False,
 )
```

