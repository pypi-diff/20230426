# Comparing `tmp/resoto-plugin-posthog-3.3.3.tar.gz` & `tmp/resoto-plugin-posthog-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-posthog-3.3.3.tar", last modified: Fri Apr 21 14:36:30 2023, max compression
+gzip compressed data, was "resoto-plugin-posthog-3.3.4.tar", last modified: Wed Apr 26 16:51:15 2023, max compression
```

## Comparing `resoto-plugin-posthog-3.3.3.tar` & `resoto-plugin-posthog-3.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 14:36:30.000000 resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:30.929604 resoto-plugin-posthog-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 14:34:33.000000 resoto-plugin-posthog-3.3.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:15.920910 resoto-plugin-posthog-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-26 16:51:15.920910 resoto-plugin-posthog-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:15.916909 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:15.920910 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 16:51:15.000000 resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:51:15.920910 resoto-plugin-posthog-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:51:15.920910 resoto-plugin-posthog-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 16:49:31.000000 resoto-plugin-posthog-3.3.4/test/test_config.py
```

### Comparing `resoto-plugin-posthog-3.3.3/PKG-INFO` & `resoto-plugin-posthog-3.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.3.3/README.md` & `resoto-plugin-posthog-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/__init__.py` & `resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/posthog.py` & `resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.3/resoto_plugin_posthog/resources.py` & `resoto-plugin-posthog-3.3.4/resoto_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/PKG-INFO` & `resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-posthog
-Version: 3.3.3
+Version: 3.3.4
 Summary: Resoto Posthog Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/posthog
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-posthog-3.3.3/resoto_plugin_posthog.egg-info/SOURCES.txt` & `resoto-plugin-posthog-3.3.4/resoto_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-posthog-3.3.3/setup.py` & `resoto-plugin-posthog-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-posthog",
-    version="3.3.3",
+    version="3.3.4",
     description="Resoto Posthog Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["posthog = resoto_plugin_posthog:PosthogCollectorPlugin"]},
     include_package_data=True,
```

