# Comparing `tmp/flytekitplugins-snowflake-1.6.0a1.tar.gz` & `tmp/flytekitplugins-snowflake-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-snowflake-1.6.0a1.tar", last modified: Wed Apr 26 20:37:33 2023, max compression
+gzip compressed data, was "flytekitplugins-snowflake-1.6.0b0.tar", last modified: Wed Apr 19 20:54:35 2023, max compression
```

## Comparing `flytekitplugins-snowflake-1.6.0a1.tar` & `flytekitplugins-snowflake-1.6.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:33.765519 flytekitplugins-snowflake-1.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-26 20:37:33.765519 flytekitplugins-snowflake-1.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-26 20:36:40.000000 flytekitplugins-snowflake-1.6.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:33.765519 flytekitplugins-snowflake-1.6.0a1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:33.765519 flytekitplugins-snowflake-1.6.0a1/flytekitplugins/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 20:36:40.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-26 20:36:40.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins/snowflake/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:37:33.765519 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 20:37:33.000000 flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:37:33.769518 flytekitplugins-snowflake-1.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 20:37:20.000000 flytekitplugins-snowflake-1.6.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-19 20:54:06.000000 flytekitplugins-snowflake-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/flytekitplugins/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 20:54:06.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-19 20:54:06.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins/snowflake/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:35.000000 flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:35.139158 flytekitplugins-snowflake-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-19 20:54:25.000000 flytekitplugins-snowflake-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-snowflake-1.6.0a1/PKG-INFO` & `flytekitplugins-snowflake-1.6.0b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.6.0a1/README.md` & `flytekitplugins-snowflake-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.6.0a1/flytekitplugins/snowflake/task.py` & `flytekitplugins-snowflake-1.6.0b0/flytekitplugins/snowflake/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.6.0a1/flytekitplugins_snowflake.egg-info/PKG-INFO` & `flytekitplugins-snowflake-1.6.0b0/flytekitplugins_snowflake.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.6.0a1
+Version: 1.6.0b0
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.6.0a1/setup.py` & `flytekitplugins-snowflake-1.6.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "snowflake"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.6.0a1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Snowflake plugins for flytekit",
```

