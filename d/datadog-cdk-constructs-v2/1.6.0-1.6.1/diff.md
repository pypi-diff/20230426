# Comparing `tmp/datadog-cdk-constructs-v2-1.6.0.tar.gz` & `tmp/datadog-cdk-constructs-v2-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-v2-1.6.0.tar", last modified: Wed Apr 19 16:57:09 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-v2-1.6.1.tar", last modified: Tue Apr 25 15:46:03 2023, max compression
```

## Comparing `datadog-cdk-constructs-v2-1.6.0.tar` & `datadog-cdk-constructs-v2-1.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 16:57:09.484167 datadog-cdk-constructs-v2-1.6.0/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    11358 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/LICENSE
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       23 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/MANIFEST.in
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22293 2023-04-19 16:57:09.484006 datadog-cdk-constructs-v2-1.6.0/PKG-INFO
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    21313 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/README.md
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      236 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/pyproject.toml
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       38 2023-04-19 16:57:09.484218 datadog-cdk-constructs-v2-1.6.0/setup.cfg
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)     1921 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/setup.py
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 16:57:09.481575 datadog-cdk-constructs-v2-1.6.0/src/
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 16:57:09.482717 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    83134 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/__init__.py
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 16:57:09.483718 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/_jsii/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      475 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/_jsii/__init__.py
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)   130876 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.0.jsii.tgz
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 16:57:05.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/py.typed
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 16:57:09.483429 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22293 2023-04-19 16:57:09.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      523 2023-04-19 16:57:09.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 16:57:09.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      161 2023-04-19 16:57:09.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/requires.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       26 2023-04-19 16:57:09.000000 datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.785806 datadog-cdk-constructs-v2-1.6.1/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    11358 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/LICENSE
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       23 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/MANIFEST.in
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    22293 2023-04-25 15:46:03.785655 datadog-cdk-constructs-v2-1.6.1/PKG-INFO
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    21313 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/README.md
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      236 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/pyproject.toml
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       38 2023-04-25 15:46:03.785879 datadog-cdk-constructs-v2-1.6.1/setup.cfg
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)     1921 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/setup.py
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.782670 datadog-cdk-constructs-v2-1.6.1/src/
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.784058 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    83134 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/__init__.py
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.785341 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      475 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/__init__.py
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)   106621 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.1.jsii.tgz
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-04-25 15:46:00.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/py.typed
+drwxr-xr-x   0 stephen.firrincieli   (503) staff       (20)        0 2023-04-25 15:46:03.784968 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)    22293 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      523 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)        1 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)      161 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/requires.txt
+-rw-r--r--   0 stephen.firrincieli   (503) staff       (20)       26 2023-04-25 15:46:03.000000 datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-v2-1.6.0/LICENSE` & `datadog-cdk-constructs-v2-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.6.0/PKG-INFO` & `datadog-cdk-constructs-v2-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.6.0
+Version: 1.6.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.6.0/README.md` & `datadog-cdk-constructs-v2-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.6.0/setup.py` & `datadog-cdk-constructs-v2-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs-v2",
-    "version": "1.6.0",
+    "version": "1.6.1",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs_v2",
         "datadog_cdk_constructs_v2._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs_v2._jsii": [
-            "datadog-cdk-constructs-v2@1.6.0.jsii.tgz"
+            "datadog-cdk-constructs-v2@1.6.1.jsii.tgz"
         ],
         "datadog_cdk_constructs_v2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2/__init__.py` & `datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO` & `datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.6.0
+Version: 1.6.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `datadog-cdk-constructs-v2-1.6.0/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt` & `datadog-cdk-constructs-v2-1.6.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/datadog_cdk_constructs_v2/py.typed
 src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
 src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
 src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
 src/datadog_cdk_constructs_v2.egg-info/requires.txt
 src/datadog_cdk_constructs_v2.egg-info/top_level.txt
 src/datadog_cdk_constructs_v2/_jsii/__init__.py
-src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.0.jsii.tgz
+src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.6.1.jsii.tgz
```

