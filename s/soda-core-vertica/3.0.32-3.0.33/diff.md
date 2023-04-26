# Comparing `tmp/soda-core-vertica-3.0.32.tar.gz` & `tmp/soda-core-vertica-3.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.0.32.tar", last modified: Mon Apr  3 09:24:10 2023, max compression
+gzip compressed data, was "soda-core-vertica-3.0.33.tar", last modified: Tue Apr 25 14:16:06 2023, max compression
```

## Comparing `soda-core-vertica-3.0.32.tar` & `soda-core-vertica-3.0.33.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-03 09:22:58.000000 soda-core-vertica-3.0.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-04-03 09:22:58.000000 soda-core-vertica-3.0.32/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-03 09:24:10.000000 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-03 09:24:10.000000 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-03 09:24:10.000000 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-03 09:24:10.000000 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-03 09:24:10.000000 soda-core-vertica-3.0.32/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-03 09:24:10.095764 soda-core-vertica-3.0.32/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-03 09:22:58.000000 soda-core-vertica-3.0.32/tests/test_vertica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:16:06.434990 soda-core-vertica-3.0.33/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-25 14:16:06.434990 soda-core-vertica-3.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 14:16:06.434990 soda-core-vertica-3.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-25 14:14:25.000000 soda-core-vertica-3.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:16:06.430990 soda-core-vertica-3.0.33/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:16:06.430990 soda-core-vertica-3.0.33/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-04-25 14:14:25.000000 soda-core-vertica-3.0.33/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:16:06.434990 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-25 14:16:06.000000 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-25 14:16:06.000000 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:16:06.000000 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-25 14:16:06.000000 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-25 14:16:06.000000 soda-core-vertica-3.0.33/soda_core_vertica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:16:06.434990 soda-core-vertica-3.0.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-25 14:14:25.000000 soda-core-vertica-3.0.33/tests/test_vertica.py
```

### Comparing `soda-core-vertica-3.0.32/setup.py` & `soda-core-vertica-3.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-vertica"
-package_version = "3.0.32"
+package_version = "3.0.33"
 description = "Soda Core Vertica Package"
 
 requires = [f"soda-core=={package_version}", "vertica-python>=1.0.3, <2.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-vertica-3.0.32/soda/data_sources/vertica_data_source.py` & `soda-core-vertica-3.0.33/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

