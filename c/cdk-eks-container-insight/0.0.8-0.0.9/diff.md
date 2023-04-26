# Comparing `tmp/cdk-eks-container-insight-0.0.8.tar.gz` & `tmp/cdk-eks-container-insight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-eks-container-insight-0.0.8.tar", last modified: Sat Apr  1 08:34:29 2023, max compression
+gzip compressed data, was "cdk-eks-container-insight-0.0.9.tar", last modified: Wed Apr 26 01:26:29 2023, max compression
```

## Comparing `cdk-eks-container-insight-0.0.8.tar` & `cdk-eks-container-insight-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:34:29.846925 cdk-eks-container-insight-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-01 08:34:29.842925 cdk-eks-container-insight-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 08:34:29.846925 cdk-eks-container-insight-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:34:29.842925 cdk-eks-container-insight-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:34:29.842925 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:34:29.842925 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   457489 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/_jsii/cdk-eks-container-insight@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 08:34:15.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:34:29.842925 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-01 08:34:29.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-01 08:34:29.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 08:34:29.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-01 08:34:29.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-01 08:34:29.000000 cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:26:29.227960 cdk-eks-container-insight-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-26 01:26:29.223960 cdk-eks-container-insight-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:26:29.227960 cdk-eks-container-insight-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:26:29.223960 cdk-eks-container-insight-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:26:29.223960 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:26:29.223960 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   457503 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/_jsii/cdk-eks-container-insight@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:26:14.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:26:29.223960 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-26 01:26:29.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 01:26:29.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:26:29.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 01:26:29.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 01:26:29.000000 cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/top_level.txt
```

### Comparing `cdk-eks-container-insight-0.0.8/LICENSE` & `cdk-eks-container-insight-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-eks-container-insight-0.0.8/PKG-INFO` & `cdk-eks-container-insight-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-eks-container-insight
-Version: 0.0.8
+Version: 0.0.9
 Summary: CDK construct library that allows you enable an AWS EKS cluster for CloudWatch Container Insight
 Home-page: https://github.com/aws-samples/cdk-eks-container-insight.git
 Author: Greg Huang<huadebin@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-eks-container-insight.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-eks-container-insight-0.0.8/README.md` & `cdk-eks-container-insight-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-eks-container-insight-0.0.8/setup.py` & `cdk-eks-container-insight-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-eks-container-insight",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "CDK construct library that allows you enable an AWS EKS cluster for CloudWatch Container Insight",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-eks-container-insight.git",
     "long_description_content_type": "text/markdown",
     "author": "Greg Huang<huadebin@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_eks_container_insight",
         "cdk_eks_container_insight._jsii"
     ],
     "package_data": {
         "cdk_eks_container_insight._jsii": [
-            "cdk-eks-container-insight@0.0.8.jsii.tgz"
+            "cdk-eks-container-insight@0.0.9.jsii.tgz"
         ],
         "cdk_eks_container_insight": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight/__init__.py` & `cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/PKG-INFO` & `cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-eks-container-insight
-Version: 0.0.8
+Version: 0.0.9
 Summary: CDK construct library that allows you enable an AWS EKS cluster for CloudWatch Container Insight
 Home-page: https://github.com/aws-samples/cdk-eks-container-insight.git
 Author: Greg Huang<huadebin@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-eks-container-insight.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-eks-container-insight-0.0.8/src/cdk_eks_container_insight.egg-info/SOURCES.txt` & `cdk-eks-container-insight-0.0.9/src/cdk_eks_container_insight.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_eks_container_insight/py.typed
 src/cdk_eks_container_insight.egg-info/PKG-INFO
 src/cdk_eks_container_insight.egg-info/SOURCES.txt
 src/cdk_eks_container_insight.egg-info/dependency_links.txt
 src/cdk_eks_container_insight.egg-info/requires.txt
 src/cdk_eks_container_insight.egg-info/top_level.txt
 src/cdk_eks_container_insight/_jsii/__init__.py
-src/cdk_eks_container_insight/_jsii/cdk-eks-container-insight@0.0.8.jsii.tgz
+src/cdk_eks_container_insight/_jsii/cdk-eks-container-insight@0.0.9.jsii.tgz
```

