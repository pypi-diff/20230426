# Comparing `tmp/neptune_aws-1.0.0.tar.gz` & `tmp/neptune_aws-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_aws-1.0.0.tar", max compression
+gzip compressed data, was "neptune_aws-1.0.1.tar", max compression
```

## Comparing `neptune_aws-1.0.0.tar` & `neptune_aws-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      420 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    11354 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/LICENSE
--rw-r--r--   0        0        0      402 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/README.md
--rw-r--r--   0        0        0     2384 2023-04-04 12:10:55.743590 neptune_aws-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      700 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/src/neptune_aws/__init__.py
--rw-r--r--   0        0        0     3137 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/src/neptune_aws/impl/__init__.py
--rw-r--r--   0        0        0      733 2023-04-04 12:10:44.663451 neptune_aws-1.0.0/src/neptune_aws/impl/version.py
--rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 neptune_aws-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      561 2023-04-26 08:56:00.848619 neptune_aws-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11354 2023-04-26 08:56:00.848619 neptune_aws-1.0.1/LICENSE
+-rw-r--r--   0        0        0      402 2023-04-26 08:56:00.848619 neptune_aws-1.0.1/README.md
+-rw-r--r--   0        0        0     2416 2023-04-26 08:56:18.316709 neptune_aws-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      700 2023-04-26 08:56:00.852619 neptune_aws-1.0.1/src/neptune_aws/__init__.py
+-rw-r--r--   0        0        0     3137 2023-04-26 08:56:00.852619 neptune_aws-1.0.1/src/neptune_aws/impl/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-26 08:56:00.852619 neptune_aws-1.0.1/src/neptune_aws/impl/version.py
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 neptune_aws-1.0.1/PKG-INFO
```

### Comparing `neptune_aws-1.0.0/LICENSE` & `neptune_aws-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_aws-1.0.0/pyproject.toml` & `neptune_aws-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Python lack of functionalities from future versions
 importlib-metadata = { version = "*", python = "<3.8" }
 
+# Base requirements
+boto3 = "*"
 
 # dev
 pre-commit = { version = "*", optional = true }
 pytest = { version = ">=5.0", optional = true }
 pytest-cov = { version = "2.10.1", optional = true }
 neptune = { version = ">=1.0.0", optional = true }
 
@@ -35,15 +37,15 @@
 repository = "https://github.com/neptune-ai/neptune_aws"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations/aws/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-aws"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_aws-1.0.0/src/neptune_aws/__init__.py` & `neptune_aws-1.0.1/src/neptune_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_aws-1.0.0/src/neptune_aws/impl/__init__.py` & `neptune_aws-1.0.1/src/neptune_aws/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_aws-1.0.0/src/neptune_aws/impl/version.py` & `neptune_aws-1.0.1/src/neptune_aws/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_aws-1.0.0/PKG-INFO` & `neptune_aws-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-aws
-Version: 1.0.0
+Version: 1.0.1
 Summary: Neptune.ai Tools for using Neptune client on AWS integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
+Requires-Dist: boto3
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: neptune (>=1.0.0) ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest (>=5.0) ; extra == "dev"
 Requires-Dist: pytest-cov (==2.10.1) ; extra == "dev"
 Project-URL: Documentation, https://docs.neptune.ai/integrations/aws/
 Project-URL: Repository, https://github.com/neptune-ai/neptune_aws
```

