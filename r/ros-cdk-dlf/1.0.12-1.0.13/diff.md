# Comparing `tmp/ros-cdk-dlf-1.0.12.tar.gz` & `tmp/ros-cdk-dlf-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-dlf-1.0.12.tar", last modified: Tue Feb 14 09:07:50 2023, max compression
+gzip compressed data, was "dist/ros-cdk-dlf-1.0.13.tar", last modified: Wed Apr 26 07:18:39 2023, max compression
```

## Comparing `ros-cdk-dlf-1.0.12.tar` & `ros-cdk-dlf-1.0.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1241 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/README.md
--rw-r--r--   0 root         (0) root         (0)      236 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1825 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/
--rw-r--r--   0 root         (0) root         (0)    20553 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29633 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/_jsii/ros-cdk-dlf@1.0.12.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 09:07:50.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-14 09:07:49.000000 ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/
+-rw-r--r--   0 root         (0) root         (0)    20553 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29633 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/_jsii/ros-cdk-dlf@1.0.13.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 07:18:39.000000 ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/top_level.txt
```

### Comparing `ros-cdk-dlf-1.0.12/LICENSE` & `ros-cdk-dlf-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-dlf-1.0.12/PKG-INFO` & `ros-cdk-dlf-1.0.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dlf
-Version: 1.0.12
+Version: 1.0.13
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DLF Construct Library
         
@@ -19,12 +19,13 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-dlf-1.0.12/setup.py` & `ros-cdk-dlf-1.0.13/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-dlf",
-    "version": "1.0.12",
+    "version": "1.0.13",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "ros_cdk_dlf",
         "ros_cdk_dlf._jsii"
     ],
     "package_data": {
         "ros_cdk_dlf._jsii": [
-            "ros-cdk-dlf@1.0.12.jsii.tgz"
+            "ros-cdk-dlf@1.0.13.jsii.tgz"
         ],
         "ros_cdk_dlf": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-dlf-1.0.12/src/ros_cdk_dlf/__init__.py` & `ros-cdk-dlf-1.0.13/src/ros_cdk_dlf/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-dlf-1.0.12/src/ros_cdk_dlf.egg-info/PKG-INFO` & `ros-cdk-dlf-1.0.13/src/ros_cdk_dlf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-dlf
-Version: 1.0.12
+Version: 1.0.13
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DLF Construct Library
         
@@ -19,12 +19,13 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

