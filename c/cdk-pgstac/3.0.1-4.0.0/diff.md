# Comparing `tmp/cdk-pgstac-3.0.1.tar.gz` & `tmp/cdk-pgstac-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pgstac-3.0.1.tar", last modified: Fri Apr 14 03:17:20 2023, max compression
+gzip compressed data, was "cdk-pgstac-4.0.0.tar", last modified: Tue Apr 25 14:43:16 2023, max compression
```

## Comparing `cdk-pgstac-3.0.1.tar` & `cdk-pgstac-4.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:20.968851 cdk-pgstac-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/src/cdk_pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)   123391 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/src/cdk_pgstac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/src/cdk_pgstac/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/src/cdk_pgstac/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/src/cdk_pgstac/_jsii/cdk-pgstac@3.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:17:09.000000 cdk-pgstac-3.0.1/src/cdk_pgstac/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:20.972851 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 03:17:20.000000 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 03:17:20.000000 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:17:20.000000 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 03:17:20.000000 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 03:17:20.000000 cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)   123992 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160948 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/cdk-pgstac@4.0.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 14:43:15.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:15.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/top_level.txt
```

### Comparing `cdk-pgstac-3.0.1/LICENSE` & `cdk-pgstac-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-3.0.1/PKG-INFO` & `cdk-pgstac-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 3.0.1
+Version: 4.0.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-pgstac-3.0.1/README.md` & `cdk-pgstac-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-3.0.1/setup.py` & `cdk-pgstac-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pgstac",
-    "version": "3.0.1",
+    "version": "4.0.0",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/cdk-pgstac.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pgstac",
         "cdk_pgstac._jsii"
     ],
     "package_data": {
         "cdk_pgstac._jsii": [
-            "cdk-pgstac@3.0.1.jsii.tgz"
+            "cdk-pgstac@4.0.0.jsii.tgz"
         ],
         "cdk_pgstac": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pgstac-3.0.1/src/cdk_pgstac/__init__.py` & `cdk-pgstac-4.0.0/src/cdk_pgstac/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2196,14 +2196,29 @@
             api_env=api_env,
             api_policy=api_policy,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
+    @jsii.member(jsii_name="handlerRole")
+    def handler_role(self) -> aws_cdk.aws_iam.Role:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(aws_cdk.aws_iam.Role, jsii.get(self, "handlerRole"))
+
+    @handler_role.setter
+    def handler_role(self, value: aws_cdk.aws_iam.Role) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(StacIngestor, "handler_role").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "handlerRole", value)
+
+    @builtins.property
     @jsii.member(jsii_name="table")
     def table(self) -> aws_cdk.aws_dynamodb.Table:
         '''
         :stability: experimental
         '''
         return typing.cast(aws_cdk.aws_dynamodb.Table, jsii.get(self, "table"))
```

### Comparing `cdk-pgstac-3.0.1/src/cdk_pgstac.egg-info/PKG-INFO` & `cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 3.0.1
+Version: 4.0.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

