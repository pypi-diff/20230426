# Comparing `tmp/cdk8s-operator-0.1.93.tar.gz` & `tmp/cdk8s-operator-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-operator-0.1.93.tar", last modified: Tue Apr 25 00:28:24 2023, max compression
+gzip compressed data, was "cdk8s-operator-0.1.94.tar", last modified: Wed Apr 26 00:29:09 2023, max compression
```

## Comparing `cdk8s-operator-0.1.93.tar` & `cdk8s-operator-0.1.94.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.903960 cdk8s-operator-0.1.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/src/cdk8s_operator/
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/src/cdk8s_operator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/bin/cdk8s-server
--rw-r--r--   0 runner    (1001) docker     (123)   123581 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.93.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:28:12.000000 cdk8s-operator-0.1.93/src/cdk8s_operator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:28:24.907960 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-25 00:28:24.000000 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-25 00:28:24.000000 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:28:24.000000 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 00:28:24.000000 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 00:28:24.000000 cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/src/cdk8s_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/src/cdk8s_operator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/bin/cdk8s-server
+-rw-r--r--   0 runner    (1001) docker     (123)   123583 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.94.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:28:57.000000 cdk8s-operator-0.1.94/src/cdk8s_operator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:29:09.063192 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-26 00:29:09.000000 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 00:29:09.000000 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:29:09.000000 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-26 00:29:09.000000 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 00:29:09.000000 cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/top_level.txt
```

### Comparing `cdk8s-operator-0.1.93/LICENSE` & `cdk8s-operator-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.93/PKG-INFO` & `cdk8s-operator-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.93
+Version: 0.1.94
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-operator-0.1.93/README.md` & `cdk8s-operator-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.93/setup.py` & `cdk8s-operator-0.1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-operator",
-    "version": "0.1.93",
+    "version": "0.1.94",
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-operator.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_operator",
         "cdk8s_operator._jsii"
     ],
     "package_data": {
         "cdk8s_operator._jsii": [
-            "cdk8s-operator@0.1.93.jsii.tgz"
+            "cdk8s-operator@0.1.94.jsii.tgz"
         ],
         "cdk8s_operator": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-operator-0.1.93/src/cdk8s_operator/__init__.py` & `cdk8s-operator-0.1.94/src/cdk8s_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.93/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.93.jsii.tgz` & `cdk8s-operator-0.1.94/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.94.jsii.tgz`

 * *Files 22% similar despite different names*

#### Comparing `cdk8s-operator@0.1.93.jsii.tgz-content` & `cdk8s-operator@0.1.94.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'fingerprint'": "'MfRijcxmCuf4w0mD+Tp37KZyqftzL1bQaM+h5SuZHv8='", "'version'": "'0.1.94'"}*

```diff
@@ -68,15 +68,15 @@
             }
         }
     },
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "cWhLIjqDrnJHl5v0sxF0s/2c/ypUEiItWngPhJjeUd8=",
+    "fingerprint": "MfRijcxmCuf4w0mD+Tp37KZyqftzL1bQaM+h5SuZHv8=",
     "homepage": "https://github.com/cdk8s-team/cdk8s-operator.git",
     "jsiiVersion": "1.80.0 (build bce6a1d)",
     "keywords": [
         "cdk8s",
         "crd",
         "kubernetes",
         "operator"
@@ -470,9 +470,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/server:ServerProps"
         }
     },
-    "version": "0.1.93"
+    "version": "0.1.94"
 }
```

##### package/lib/operator.js

###### js-beautify {}

```diff
@@ -89,10 +89,10 @@
         throw new Error(`No custom resource provider found for ${kind}.${apiVersion}`);
     }
 }
 exports.Operator = Operator;
 _a = JSII_RTTI_SYMBOL_1;
 Operator[_a] = {
     fqn: "cdk8s-operator.Operator",
-    version: "0.1.93"
+    version: "0.1.94"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoib3BlcmF0b3IuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvb3BlcmF0b3IudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSx5QkFBeUI7QUFDekIseUJBQXlCO0FBQ3pCLDZCQUE2QjtBQUU3QixpQ0FBbUM7QUFnRG5DOztHQUVHO0FBQ0gsTUFBYSxRQUFTLFNBQVEsV0FBRztJQU8vQixZQUFZLFFBQXVCLEVBQUU7UUFDbkMsTUFBTSxNQUFNLEdBQUcsRUFBRSxDQUFDLFdBQVcsQ0FBQyxJQUFJLENBQUMsSUFBSSxDQUFDLEVBQUUsQ0FBQyxNQUFNLEVBQUUsRUFBRSxPQUFPLENBQUMsQ0FBQyxDQUFDO1FBQy9ELEtBQUssQ0FBQyxFQUFFLE1BQU0sRUFBRSxDQUFDLENBQUM7UUFFbEIsSUFBSSxDQUFDLFNBQVMsR0FBRyxFQUFFLENBQUM7UUFFcEIsSUFBSSxDQUFDLFNBQVMsR0FBRyxLQUFLLENBQUMsU0FBUyxJQUFJLE9BQU8sQ0FBQyxJQUFJLENBQUMsQ0FBQyxDQUFDLElBQUksWUFBWSxDQUFDO1FBQ3BFLElBQUksQ0FBQyxVQUFVLEdBQUcsS0FBSyxDQUFDLFVBQVUsQ0FBQztJQUNyQyxDQUFDO0lBRUQ7OztPQUdHO0lBQ0ksV0FBVyxDQUFDLFFBQWdDO1FBQ2pELElBQUksQ0FBQyxTQUFTLENBQUMsSUFBSSxDQUFDLFFBQVEsQ0FBQyxDQUFDO0lBQ2hDLENBQUM7SUFFRDs7Ozs7Ozs7T0FRRztJQUNJLEtBQUs7UUFDVixNQUFNLEtBQUssR0FBRyxJQUFJLENBQUMsS0FBSyxDQUFDLEVBQUUsQ0FBQyxZQUFZLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSxPQUFPLENBQUMsQ0FBQyxDQUFDO1FBRW5FLElBQUksS0FBSyxDQUFDO1FBQ1YsSUFBSSxJQUFJLENBQUMsVUFBVSxFQUFFO1lBQ25CLE1BQU0sT0FBTyxHQUFHLElBQUksQ0FBQyxVQUFVLENBQUM7WUFDaEMsS0FBSyxHQUFHLENBQUMsSUFBWSxFQUFFLEVBQUUsQ0FBQyxFQUFFLENBQUMsYUFBYSxDQUFDLE9BQU8sRUFBRSxJQUFJLENBQUMsQ0FBQztTQUMzRDthQUFNO1lBQ0wsS0FBSyxHQUFHLENBQUMsSUFBWSxFQUFFLEVBQUUsQ0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLEtBQUssQ0FBQyxJQUFJLENBQUMsQ0FBQztTQUN0RDtRQUVELElBQUksT0FBTSxDQUFDLEtBQUssQ0FBQyxLQUFLLFFBQVEsRUFBRTtZQUM5QixNQUFNLElBQUksS0FBSyxDQUFDLDRDQUE0QyxDQUFDLENBQUM7U0FDL0Q7UUFFRCxNQUFNLFFBQVEsR0FBRyxJQUFJLENBQUMsWUFBWSxDQUFDLEtBQUssQ0FBQyxDQUFDO1FBRTFDLE1BQU0sSUFBSSxHQUFHLEtBQUssQ0FBQyxRQUFRLEVBQUUsSUFBSSxDQUFDO1FBQ2xDLElBQUksQ0FBQyxJQUFJLEVBQUU7WUFDVCxNQUFNLElBQUksS0FBSyxDQUFDLGlDQUFpQyxDQUFDLENBQUM7U0FDcEQ7UUFFRCxNQUFNLFNBQVMsR0FBRyxLQUFLLENBQUMsUUFBUSxFQUFFLFNBQVMsQ0FBQztRQUU1QyxrQkFBa0I7UUFDbEIsTUFBTSxJQUFJLEdBQUcsS0FBSyxDQUFDLElBQUksSUFBSSxFQUFFLENBQUM7UUFFOUIsTUFBTSxLQUFLLEdBQUcsSUFBSSxhQUFLLENBQUMsSUFBSSxFQUFFLElBQUksRUFBRSxFQUFFLFNBQVMsRUFBRSxDQUFDLENBQUM7UUFFbkQsT0FBTyxDQUFDLEtBQUssQ0FBQyxnQkFBZ0IsS0FBSyxDQUFDLElBQUksSUFBSSxLQUFLLENBQUMsVUFBVSxFQUFFLENBQUMsQ0FBQztRQUNoRSxRQUFRLENBQUMsT0FBTyxDQUFDLEtBQUssQ0FBQyxLQUFLLEVBQUUsSUFBSSxFQUFFLElBQUksQ0FBQyxDQUFDO1FBRTFDLEtBQUssQ0FBQyxLQUFLLEVBQUUsQ0FBQztRQUVkLEtBQUssTUFBTSxJQUFJLElBQUksRUFBRSxDQUFDLFdBQVcsQ0FBQyxJQUFJLENBQUMsTUFBTSxDQUFDLEVBQUU7WUFDOUMsTUFBTSxRQUFRLEdBQUcsSUFBSSxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsTUFBTSxFQUFFLElBQUksQ0FBQyxDQUFDO1lBQzlDLE1BQU0sUUFBUSxHQUFHLEVBQUUsQ0FBQyxZQUFZLENBQUMsUUFBUSxDQUFDLENBQUM7WUFDM0MsS0FBSyxDQUFDLFFBQVEsQ0FBQyxDQUFDO1NBQ2pCO0lBQ0gsQ0FBQztJQUVPLFlBQVksQ0FBQyxLQUEyQztRQUM5RCxNQUFNLEVBQUUsVUFBVSxFQUFFLElBQUksRUFBRSxHQUFHLEtBQUssQ0FBQztRQUVuQyxJQUFJLENBQUMsVUFBVSxFQUFFO1lBQ2YsTUFBTSxJQUFJLEtBQUssQ0FBQywwQkFBMEIsQ0FBQyxDQUFDO1NBQzdDO1FBRUQsSUFBSSxDQUFDLElBQUksRUFBRTtZQUNULE1BQU0sSUFBSSxLQUFLLENBQUMsb0JBQW9CLENBQUMsQ0FBQztTQUN2QztRQUVELEtBQUssTUFBTSxDQUFDLElBQUksSUFBSSxDQUFDLFNBQVMsRUFBRTtZQUM5QixJQUFJLENBQUMsQ0FBQyxVQUFVLEtBQUssVUFBVSxJQUFJLENBQUMsQ0FBQyxJQUFJLEtBQUssSUFBSSxFQUFFO2dCQUNsRCxPQUFPLENBQUMsQ0FBQzthQUNWO1NBQ0Y7UUFFRCxNQUFNLElBQUksS0FBSyxDQUFDLHlDQUF5QyxJQUFJLElBQUksVUFBVSxFQUFFLENBQUMsQ0FBQztJQUNqRixDQUFDOztBQTdGSCw0QkE4RkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBmcyBmcm9tICdmcyc7XG5pbXBvcnQgKiBhcyBvcyBmcm9tICdvcyc7XG5pbXBvcnQgKiBhcyBwYXRoIGZyb20gJ3BhdGgnO1xuXG5pbXBvcnQgeyBBcHAsIENoYXJ0IH0gZnJvbSAnY2RrOHMnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbi8qKlxuICogVGhlIGhhbmRsZXIgZm9yIHRoaXMgY3VzdG9tIHJlc291cmNlIHByb3ZpZGVyLlxuICovXG5leHBvcnQgaW50ZXJmYWNlIElDdXN0b21SZXNvdXJjZVByb3ZpZGVySGFuZGxlciB7XG4gIC8vIHJlYWRvbmx5IHNjaGVtYTogYW55O1xuXG4gIGFwcGx5KHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHNwZWM6IGFueSk6IENvbnN0cnVjdDtcbn1cblxuZXhwb3J0IGludGVyZmFjZSBDdXN0b21SZXNvdXJjZVByb3ZpZGVyIHtcbiAgLyoqXG4gICAqIEtpbmQgb2YgdGhpcyBjdXN0b20gcmVzb3VyY2UuXG4gICAqL1xuICByZWFkb25seSBraW5kOiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIEFQSSB2ZXJzaW9uIG9mIHRoZSBjdXN0b20gcmVzb3VyY2UuXG4gICAqXG4gICAqIEBkZWZhdWx0IFwidjFcIlxuICAgKi9cbiAgcmVhZG9ubHkgYXBpVmVyc2lvbjogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBUaGUgY29uc3RydWN0IGhhbmRsZXIuXG4gICAqL1xuICByZWFkb25seSBoYW5kbGVyOiBJQ3VzdG9tUmVzb3VyY2VQcm92aWRlckhhbmRsZXI7XG59XG5cbmV4cG9ydCBpbnRlcmZhY2UgT3BlcmF0b3JQcm9wcyB7XG4gIC8qKlxuICAgKiBBIEt1YmVybmV0ZXMgSlNPTiBtYW5pZmVzdCB3aXRoIGEgc2luZ2xlIHJlc291cmNlIHRoYXQgaXMgbWF0Y2hlZCBhZ2FpbnN0XG4gICAqIG9uZSBvZiB0aGUgcHJvdmlkZXJzIHdpdGhpbiB0aGlzIG9wZXJhdG9yLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIGZpcnN0IHBvc2l0aW9uIGNvbW1hbmQtbGluZSBhcmd1bWVudCBvciBcIi9kZXYvc3RkaW5cIlxuICAgKi9cbiAgcmVhZG9ubHkgaW5wdXRGaWxlPzogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBXaGVyZSB0byB3cml0ZSB0aGUgc3ludGhlc2l6ZWQgb3V0cHV0LlxuICAgKlxuICAgKiBAZGVmYXVsdCBcIi9kZXYvc3Rkb3V0XCJcbiAgICovXG4gIHJlYWRvbmx5IG91dHB1dEZpbGU/OiBzdHJpbmc7XG59XG5cbi8qKlxuICogQSBDREs4cyBhcHAgd2hpY2ggYWxsb3dzIGltcGxlbWVudGluZyBLdWJlcm5ldGVzIG9wZXJhdG9ycyB1c2luZyBDREs4cyBjb25zdHJ1Y3RzLlxuICovXG5leHBvcnQgY2xhc3MgT3BlcmF0b3IgZXh0ZW5kcyBBcHAge1xuXG4gIHByaXZhdGUgcmVhZG9ubHkgaW5wdXRGaWxlOiBzdHJpbmc7XG4gIHByaXZhdGUgcmVhZG9ubHkgb3V0cHV0RmlsZT86IHN0cmluZztcblxuICBwcml2YXRlIHJlYWRvbmx5IHByb3ZpZGVyczogQ3VzdG9tUmVzb3VyY2VQcm92aWRlcltdO1xuXG4gIGNvbnN0cnVjdG9yKHByb3BzOiBPcGVyYXRvclByb3BzID0ge30pIHtcbiAgICBjb25zdCBvdXRkaXIgPSBmcy5ta2R0ZW1wU3luYyhwYXRoLmpvaW4ob3MudG1wZGlyKCksICdjZGs4cycpKTtcbiAgICBzdXBlcih7IG91dGRpciB9KTtcblxuICAgIHRoaXMucHJvdmlkZXJzID0gW107XG5cbiAgICB0aGlzLmlucHV0RmlsZSA9IHByb3BzLmlucHV0RmlsZSA/PyBwcm9jZXNzLmFyZ3ZbMl0gPz8gJy9kZXYvc3RkaW4nO1xuICAgIHRoaXMub3V0cHV0RmlsZSA9IHByb3BzLm91dHB1dEZpbGU7XG4gIH1cblxuICAvKipcbiAgICogQWRkcyBhIGN1c3RvbSByZXNvdXJjZSBwcm92aWRlciB0byB0aGlzIG9wZXJhdG9yLlxuICAgKiBAcGFyYW0gcHJvdmlkZXIgVGhlIHByb3ZpZGVyIHRvIGFkZFxuICAgKi9cbiAgcHVibGljIGFkZFByb3ZpZGVyKHByb3ZpZGVyOiBDdXN0b21SZXNvdXJjZVByb3ZpZGVyKSB7XG4gICAgdGhpcy5wcm92aWRlcnMucHVzaChwcm92aWRlcik7XG4gIH1cblxuICAvKipcbiAgICogUmVhZHMgYSBLdWJlcm5ldGVzIG1hbmlmZXN0IGluIEpTT04gZm9ybWF0IGZyb20gU1RESU4gb3IgdGhlIGZpbGUgc3BlY2lmaWVkXG4gICAqIGFzIHRoZSBmaXJzdCBwb3NpdGlvbmFsIGNvbW1hbmQtbGluZSBhcmd1bWVudC4gVGhpcyBtYW5pZmVzdCBpcyBleHBlY3RlZCB0b1xuICAgKiBpbmNsdWRlIGEgc2luZ2xlIEt1YmVybmV0ZXMgcmVzb3VyY2UuIFRoZW4sIHdlIG1hdGNoIGBhcGlWZXJzaW9uYCBhbmRcbiAgICogYGtpbmRgIHRvIG9uZSBvZiB0aGUgcmVnaXN0ZXJlZCBwcm92aWRlcnMgYW5kIGlmIHdlIGRvLCB3ZSBpbnZva2VcbiAgICogYGFwcGx5KClgLCBwYXNzaW5nIGl0IHRoZSBgc3BlY2Agb2YgdGhlIGlucHV0IG1hbmlmZXN0IGFuZCBhIGNoYXJ0IGFzIGFcbiAgICogc2NvcGUuIFRoZSBjaGFydCBpcyB0aGVuIHN5bnRoZXNpemVkIGFuZCB0aGUgb3V0cHV0IG1hbmlmZXN0IGlzIHdyaXR0ZW4gdG9cbiAgICogU1RET1VULlxuICAgKi9cbiAgcHVibGljIHN5bnRoKCkge1xuICAgIGNvbnN0IGlucHV0ID0gSlNPTi5wYXJzZShmcy5yZWFkRmlsZVN5bmModGhpcy5pbnB1dEZpbGUsICd1dGYtOCcpKTtcblxuICAgIGxldCB3cml0ZTtcbiAgICBpZiAodGhpcy5vdXRwdXRGaWxlKSB7XG4gICAgICBjb25zdCBvdXRmaWxlID0gdGhpcy5vdXRwdXRGaWxlO1xuICAgICAgd3JpdGUgPSAoZGF0YTogQnVmZmVyKSA9PiBmcy53cml0ZUZpbGVTeW5jKG91dGZpbGUsIGRhdGEpO1xuICAgIH0gZWxzZSB7XG4gICAgICB3cml0ZSA9IChkYXRhOiBCdWZmZXIpID0+IHByb2Nlc3Muc3Rkb3V0LndyaXRlKGRhdGEpO1xuICAgIH1cblxuICAgIGlmICh0eXBlb2YoaW5wdXQpICE9PSAnb2JqZWN0Jykge1xuICAgICAgdGhyb3cgbmV3IEVycm9yKCdpbnB1dCBtdXN0IGJlIGEgc2luZ2xlIGt1YmVybmV0ZXMgcmVzb3VyY2UnKTtcbiAgICB9XG5cbiAgICBjb25zdCBwcm92aWRlciA9IHRoaXMuZmluZFByb3ZpZGVyKGlucHV0KTtcblxuICAgIGNvbnN0IG5hbWUgPSBpbnB1dC5tZXRhZGF0YT8ubmFtZTtcbiAgICBpZiAoIW5hbWUpIHtcbiAgICAgIHRocm93IG5ldyBFcnJvcignXCJtZXRhZGF0YS5uYW1lXCIgbXVzdCBiZSBkZWZpbmVkJyk7XG4gICAgfVxuXG4gICAgY29uc3QgbmFtZXNwYWNlID0gaW5wdXQubWV0YWRhdGE/Lm5hbWVzcGFjZTtcblxuICAgIC8vIFRPRE86IG5hbWVzcGFjZVxuICAgIGNvbnN0IHNwZWMgPSBpbnB1dC5zcGVjID8/IHt9O1xuXG4gICAgY29uc3QgY2hhcnQgPSBuZXcgQ2hhcnQodGhpcywgbmFtZSwgeyBuYW1lc3BhY2UgfSk7XG5cbiAgICBjb25zb2xlLmVycm9yKGBTeW50aGVzaXppbmcgJHtpbnB1dC5raW5kfS4ke2lucHV0LmFwaVZlcnNpb259YCk7XG4gICAgcHJvdmlkZXIuaGFuZGxlci5hcHBseShjaGFydCwgbmFtZSwgc3BlYyk7XG5cbiAgICBzdXBlci5zeW50aCgpO1xuXG4gICAgZm9yIChjb25zdCBmaWxlIG9mIGZzLnJlYWRkaXJTeW5jKHRoaXMub3V0ZGlyKSkge1xuICAgICAgY29uc3QgZmlsZXBhdGggPSBwYXRoLmpvaW4odGhpcy5vdXRkaXIsIGZpbGUpO1xuICAgICAgY29uc3QgbWFuaWZlc3QgPSBmcy5yZWFkRmlsZVN5bmMoZmlsZXBhdGgpO1xuICAgICAgd3JpdGUobWFuaWZlc3QpO1xuICAgIH1cbiAgfVxuXG4gIHByaXZhdGUgZmluZFByb3ZpZGVyKGlucHV0OiB7IGtpbmQ6IHN0cmluZzsgYXBpVmVyc2lvbjogc3RyaW5nIH0pIHtcbiAgICBjb25zdCB7IGFwaVZlcnNpb24sIGtpbmQgfSA9IGlucHV0O1xuXG4gICAgaWYgKCFhcGlWZXJzaW9uKSB7XG4gICAgICB0aHJvdyBuZXcgRXJyb3IoJ1wiYXBpVmVyc2lvblwiIGlzIHJlcXVpcmVkJyk7XG4gICAgfVxuXG4gICAgaWYgKCFraW5kKSB7XG4gICAgICB0aHJvdyBuZXcgRXJyb3IoJ1wia2luZFwiIGlzIHJlcXVpcmVkJyk7XG4gICAgfVxuXG4gICAgZm9yIChjb25zdCBwIG9mIHRoaXMucHJvdmlkZXJzKSB7XG4gICAgICBpZiAocC5hcGlWZXJzaW9uID09PSBhcGlWZXJzaW9uICYmIHAua2luZCA9PT0ga2luZCkge1xuICAgICAgICByZXR1cm4gcDtcbiAgICAgIH1cbiAgICB9XG5cbiAgICB0aHJvdyBuZXcgRXJyb3IoYE5vIGN1c3RvbSByZXNvdXJjZSBwcm92aWRlciBmb3VuZCBmb3IgJHtraW5kfS4ke2FwaVZlcnNpb259YCk7XG4gIH1cbn1cblxuIl19
```

##### package/lib/server.js

###### js-beautify {}

```diff
@@ -98,10 +98,10 @@
         });
     }
 }
 exports.Server = Server;
 _a = JSII_RTTI_SYMBOL_1;
 Server[_a] = {
     fqn: "cdk8s-operator.Server",
-    version: "0.1.93"
+    version: "0.1.94"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic2VydmVyLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vc3JjL3NlcnZlci50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLGlEQUFzQztBQUN0QywyQkFBa0U7QUFDbEUsK0JBQTJGO0FBQzNGLDJCQUE0QjtBQUM1QiwrQkFBNEI7QUFTNUIsTUFBYSxNQUFNO0lBS2pCLFlBQVksS0FBa0I7UUFDNUIsSUFBSSxDQUFDLFVBQVUsR0FBRyxLQUFLLENBQUMsVUFBVSxDQUFDO1FBRW5DLElBQUksQ0FBQyxNQUFNLEdBQUcsbUJBQVksQ0FBQyxDQUFDLEdBQUcsRUFBRSxHQUFHLEVBQUUsRUFBRSxDQUFDLElBQUksQ0FBQyxhQUFhLENBQUMsR0FBRyxFQUFFLEdBQUcsQ0FBQyxDQUFDLEtBQUssQ0FBQyxDQUFDLENBQUMsRUFBRTtZQUM5RSxPQUFPLENBQUMsS0FBSyxDQUFDLGdCQUFnQixFQUFFLENBQUMsQ0FBQyxDQUFDO1lBQ25DLEdBQUcsQ0FBQyxVQUFVLEdBQUcsR0FBRyxDQUFDO1lBQ3JCLEdBQUcsQ0FBQyxLQUFLLENBQUMsQ0FBQyxDQUFDLE9BQU8sQ0FBQyxDQUFDO1lBQ3JCLEdBQUcsQ0FBQyxHQUFHLEVBQUUsQ0FBQztRQUNaLENBQUMsQ0FBQyxDQUFDLENBQUM7UUFFSixJQUFJLENBQUMsTUFBTSxHQUFHLGdCQUFXLENBQUMsV0FBSSxDQUFDLFdBQU0sRUFBRSxFQUFFLGlCQUFpQixDQUFDLENBQUMsQ0FBQztJQUMvRCxDQUFDO0lBRUQ7Ozs7O09BS0c7SUFDSSxLQUFLLENBQUMsTUFBTSxDQUFDLElBQWE7UUFDL0IsTUFBTSxLQUFLLEdBQUcsSUFBSSxJQUFJLE9BQU8sQ0FBQyxHQUFHLENBQUMsSUFBSSxJQUFJLENBQUMsQ0FBQztRQUM1QyxPQUFPLElBQUksT0FBTyxDQUFDLENBQUMsRUFBRSxFQUFFLEVBQUUsRUFBRSxFQUFFO1lBQzVCLElBQUksQ0FBQyxNQUFNLENBQUMsTUFBTSxDQUFDLEtBQUssRUFBRSxH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QUMsQ0FBQztZQUN4RixNQUFNLEtBQUssR0FBRyxzQkFBaUIsQ0FBQyxTQUFTLENBQUMsQ0FBQztZQUMzQyxHQUFHLENBQUMsSUFBSSxDQUFDLEtBQUssQ0FBQyxDQUFDO1lBRWhCLEtBQUssQ0FBQyxFQUFFLENBQUMsT0FBTyxFQUFFLEdBQUcsRUFBRTtnQkFDckIsSUFBSTtvQkFDRixNQUFNLFNBQVMsR0FBRyxJQUFJLENBQUMsS0FBSyxDQUFDLGlCQUFZLENBQUMsU0FBUyxFQUFFLE9BQU8sQ0FBQyxDQUFDLENBQUM7b0JBQy9ELE9BQU8sQ0FBQyxLQUFLLENBQUMsVUFBVSxJQUFJLENBQUMsU0FBUyxDQUFDLFNBQVMsQ0FBQyxFQUFFLENBQUMsQ0FBQztvQkFDckQsT0FBTyxFQUFFLENBQUMsU0FBUyxDQUFDLENBQUM7aUJBQ3RCO2dCQUFDLE9BQU8sQ0FBQyxFQUFFO29CQUNWLE9BQU8sRUFBRSxDQUFDLElBQUksS0FBSyxDQUFDLHlDQUF5QyxDQUFDLEVBQUUsQ0FBQyxDQUFDLENBQUM7aUJBQ3BFO1lBQ0gsQ0FBQyxDQUFDLENBQUM7WUFFSCxHQUFHLENBQUMsRUFBRSxDQUFDLE9BQU8sRUFBRSxHQUFHLENBQUMsRUFBRSxDQUFDLEVBQUUsQ0FBQyxHQUFHLENBQUMsT0FBTyxDQUFDLENBQUMsQ0FBQztRQUMxQyxDQUFDLENBQUMsQ0FBQztJQUNMLENBQUM7O0FBNUdILHdCQTZHQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IHNwYXduIH0gZnJvbSAnY2hpbGRfcHJvY2Vzcyc7XG5pbXBvcnQgeyBjcmVhdGVXcml0ZVN0cmVhbSwgbWtkdGVtcFN5bmMsIHJlYWRGaWxlU3luYyB9IGZyb20gJ2ZzJztcbmltcG9ydCB7IGNyZWF0ZVNlcnZlciwgSW5jb21pbmdNZXNzYWdlLCBTZXJ2ZXIgYXMgSHR0cFNlcnZlciwgU2VydmVyUmVzcG9uc2UgfSBmcm9tICdodHRwJztcbmltcG9ydCB7IHRtcGRpciB9IGZyb20gJ29zJztcbmltcG9ydCB7IGpvaW4gfSBmcm9tICdwYXRoJztcblxuZXhwb3J0IGludGVyZmFjZSBTZXJ2ZXJQcm9wcyB7XG4gIC8qKlxuICAgKiBUaGUgY29tbWFuZCB0byBleGVjdXRlIGluIG9yZGVyIHRvIHN5bnRoZXNpemUgdGhlIENESyBhcHAuXG4gICAqL1xuICByZWFkb25seSBhcHBDb21tYW5kOiBzdHJpbmc7XG59XG5cbmV4cG9ydCBjbGFzcyBTZXJ2ZXIge1xuICBwcml2YXRlIHJlYWRvbmx5IHNlcnZlcjogSHR0cFNlcnZlcjtcbiAgcHJpdmF0ZSByZWFkb25seSBhcHBDb21tYW5kOiBzdHJpbmc7XG4gIHByaXZhdGUgcmVhZG9ubHkgdG1wZGlyOiBzdHJpbmc7XG5cbiAgY29uc3RydWN0b3IocHJvcHM6IFNlcnZlclByb3BzKSB7XG4gICAgdGhpcy5hcHBDb21tYW5kID0gcHJvcHMuYXBwQ29tbWFuZDtcblxuICAgIHRoaXMuc2VydmVyID0gY3JlYXRlU2VydmVyKChyZXEsIHJlcykgPT4gdGhpcy5oYW5kbGVSZXF1ZXN0KHJlcSwgcmVzKS5jYXRjaChlID0+IHtcbiAgICAgIGNvbnNvbGUuZXJyb3IoJ3NlcnZlciBlcnJvcjogJywgZSk7XG4gICAgICByZXMuc3RhdHVzQ29kZSA9IDUwMDtcbiAgICAgIHJlcy53cml0ZShlLm1lc3NhZ2UpO1xuICAgICAgcmVzLmVuZCgpO1xuICAgIH0pKTtcblxuICAgIHRoaXMudG1wZGlyID0gbWtkdGVtcFN5bmMoam9pbih0bXBkaXIoKSwgJ2NkazhzLW9wZXJhdG9yLScpKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBTdGFydHMgSFRUUCBzZXJ2ZXIuXG4gICAqIEBwYXJhbSBwb3J0IFRoZSBwb3J0IHRvIGxpc3RlbiB0by4gSWYgbm90IHNwZWNpZmllZCwgdGhlIGBQT1JUYCBlbnZpcm9ubWVudFxuICAgKiB2YXJpYWJsZSB3aWxsIGJlIHVzZWQuIElmIHRoYXQncyBub3Qgc3BlY2lmaWVkIGFuIGF2YWlsYWJsZSBwb3J0IHdpbGwgYmVcbiAgICogYXV0by1zZWxlY3RlZC5cbiAgICovXG4gIHB1YmxpYyBhc3luYyBsaXN0ZW4ocG9ydD86IG51bWJlcik6IFByb21pc2U8bnVtYmVyPiB7XG4gICAgY29uc3QgbHBvcnQgPSBwb3J0ID8/IHByb2Nlc3MuZW52LlBPUlQgPz8gMDtcbiAgICByZXR1cm4gbmV3IFByb21pc2UoKG9rLCBrbykgPT4ge1xuICAgICAgdGhpcy5zZXJ2ZXIubGlzdGVuKGxwb3J0LCAoKSA9PiB7XG4gICAgICAgIGNvbnN0IGFkZHIgPSB0aGlzLnNlcnZlci5hZGRyZXNzKCk7XG4gICAgICAgIGlmICh0eXBlb2YoYWRkcikgPT09ICdzdHJpbmcnKSB7XG4gICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGBjYW5ub3QgZGV0ZXJtaW5lIHBvcnQgZnJvbSBzZXJ2ZXIgYWRkcmVzcyAke2FkZHJ9YCk7XG4gICAgICAgIH1cblxuICAgICAgICByZXR1cm4gb2soYWRkcj8ucG9ydCk7XG4gICAgICB9KTtcblxuICAgICAgdGhpcy5zZXJ2ZXIub24oJ2Vycm9yJywgZXJyID0+IGtvKGVycikpO1xuICAgIH0pO1xuICB9XG5cbiAgLyoqXG4gICAqIFN0b3Agc2VydmVyLlxuICAgKi9cbiAgcHVibGljIGNsb3NlKCkge1xuICAgIHRoaXMuc2VydmVyLmNsb3NlKCk7XG4gIH1cblxuICBwcml2YXRlIGFzeW5jIGhhbmRsZVJlcXVlc3QocmVxOiBJbmNvbWluZ01lc3NhZ2UsIHJlczogU2VydmVyUmVzcG9uc2UpIHtcbiAgICBjb25zdCBpbnB1dGZpbGUgPSBhd2FpdCB0aGlzLndyaXRlSW5wdXRGaWxlKHJlcSk7XG5cbiAgICBjb25zdCBjaGlsZCA9IHNwYXduKHRoaXMuYXBwQ29tbWFuZCwgW2lucHV0ZmlsZV0sIHtcbiAgICAgIHN0ZGlvOiBbJ2lnbm9yZScsICdwaXBlJywgJ3BpcGUnXSxcbiAgICAgIHNoZWxsOiB0cnVlLFxuICAgIH0pO1xuXG4gICAgY29uc3Qgc3RkZXJyID0gbmV3IEFycmF5PEJ1ZmZlcj4oKTtcblxuICAgIHJlcy5zZXRIZWFkZXIoJ0NvbnRlbnQtVHlwZScsICdhcHBsaWNhdGlvbi9qc29uJyk7XG5cbiAgICAvLyBzdGRvdXQgc2hvdWxkIGdvIGRpcmVjdGx5IHRvIHRoZSByZXNwb25zZVxuICAgIGNoaWxkLnN0ZG91dC5vbignZGF0YScsIGNodW5rID0+IHtcbiAgICAgIHByb2Nlc3Muc3RkZXJyLndyaXRlKCdvdXRwdXQ6ICcgKyBjaHVuayk7XG4gICAgICByZXMud3JpdGUoY2h1bmspO1xuICAgIH0pO1xuXG4gICAgLy8gZm9yIHN0ZGVycjogd3JpdGUgdG8gc2VydmVyIHRlcm1pbmFsIGFuZCBvbmx5IHNlbmQgYmFjayBpZiB3ZSBleGl0ZWQgd2l0aCBhIG5vbi16ZXJvXG4gICAgY2hpbGQuc3RkZXJyLm9uKCdkYXRhJywgY2h1bmsgPT4ge1xuICAgICAgcHJvY2Vzcy5zdGRlcnIud3JpdGUoY2h1bmspO1xuICAgICAgc3RkZXJyLnB1c2goY2h1bmspO1xuICAgIH0pO1xuXG4gICAgLy8gd2lsbCBiZSBjYXVzZWQgYnkgdGhlIGFzeW5jIGhhbmRsZXIgYW5kIDUwMCB3aWxsIGJlIHJldHVybmVkLlxuICAgIGNoaWxkLm9uKCdlcnJvcicsIGVyciA9PiB7XG4gICAgICB0aHJvdyBlcnI7XG4gICAgfSk7XG5cbiAgICBjaGlsZC5vbignZXhpdCcsIGNvZGUgPT4ge1xuICAgICAgaWYgKGNvZGUgIT09IDApIHtcbiAgICAgICAgcmVzLnN0YXR1c0NvZGUgPSA1MDA7XG4gICAgICAgIGZvciAoY29uc3QgYyBvZiBzdGRlcnIpIHtcbiAgICAgICAgICByZXMud3JpdGUoYyk7XG4gICAgICAgIH1cbiAgICAgICAgcmVzLmVuZCgpO1xuICAgICAgfVxuXG4gICAgICAvLyBzdWNjZXNzXG4gICAgICByZXR1cm4gcmVzLmVuZCgpO1xuICAgIH0pO1xuICB9XG5cbiAgcHJpdmF0ZSBhc3luYyB3cml0ZUlucHV0RmlsZShyZXE6IEluY29taW5nTWVzc2FnZSk6IFByb21pc2U8c3RyaW5nPiB7XG4gICAgcmV0dXJuIG5ldyBQcm9taXNlKChvaywga28pID0+IHtcbiAgICAgIGNvbnN0IGlucHV0ZmlsZSA9IGpvaW4odGhpcy50bXBkaXIsIGBpbnB1dC0ke01hdGgucm91bmQoTWF0aC5yYW5kb20oKSAqIDk5OTk5OSl9Lmpzb25gKTtcbiAgICAgIGNvbnN0IGlucHV0ID0gY3JlYXRlV3JpdGVTdHJlYW0oaW5wdXRmaWxlKTtcbiAgICAgIHJlcS5waXBlKGlucHV0KTtcblxuICAgICAgaW5wdXQub24oJ2Nsb3NlJywgKCkgPT4ge1xuICAgICAgICB0cnkge1xuICAgICAgICAgIGNvbnN0IGlucHV0SnNvbiA9IEpTT04ucGFyc2UocmVhZEZpbGVTeW5jKGlucHV0ZmlsZSwgJ3V0Zi04JykpO1xuICAgICAgICAgIGNvbnNvbGUuZXJyb3IoYGlucHV0OiAke0pTT04uc3RyaW5naWZ5KGlucHV0SnNvbil9YCk7XG4gICAgICAgICAgcmV0dXJuIG9rKGlucHV0ZmlsZSk7XG4gICAgICAgIH0gY2F0Y2ggKGUpIHtcbiAgICAgICAgICByZXR1cm4ga28obmV3IEVycm9yKGB1bmFibGUgdG8gcGFyc2UgcmVxdWVzdCBib2R5IGFzIEpTT046ICR7ZX1gKSk7XG4gICAgICAgIH1cbiAgICAgIH0pO1xuXG4gICAgICByZXEub24oJ2Vycm9yJywgZXJyID0+IGtvKGVyci5tZXNzYWdlKSk7XG4gICAgfSk7XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9745670995670995%*

 * *Differences: {"'devDependencies'": "{'@cdk8s/projen-common': '^0.0.321', 'constructs': '10.2.7', 'projen': "*

 * *                      "'^0.71.25'}",*

 * * "'version'": "'0.1.94'"}*

```diff
@@ -12,33 +12,33 @@
         "yaml"
     ],
     "dependencies": {
         "yaml": "^1.10.2"
     },
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "devDependencies": {
-        "@cdk8s/projen-common": "^0.0.319",
+        "@cdk8s/projen-common": "^0.0.321",
         "@types/jest": "^27",
         "@types/node": "^14",
         "@typescript-eslint/eslint-plugin": "^5",
         "@typescript-eslint/parser": "^5",
         "cdk8s": "2.7.56",
-        "constructs": "10.2.5",
+        "constructs": "10.2.7",
         "eslint": "^8",
         "eslint-import-resolver-node": "^0.3.7",
         "eslint-import-resolver-typescript": "^2.7.1",
         "eslint-plugin-import": "^2.27.5",
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.80.0",
         "jsii-docgen": "^1.8.110",
         "jsii-pacmak": "^1.80.0",
         "npm-check-updates": "^16",
-        "projen": "^0.71.23",
+        "projen": "^0.71.25",
         "standard-version": "^9",
         "ts-jest": "^27",
         "typescript": "^3.9.10"
     },
     "engines": {
         "node": ">= 14.17.0"
     },
@@ -156,9 +156,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.1.93"
+    "version": "0.1.94"
 }
```

### Comparing `cdk8s-operator-0.1.93/src/cdk8s_operator.egg-info/PKG-INFO` & `cdk8s-operator-0.1.94/src/cdk8s_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.93
+Version: 0.1.94
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
 Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

