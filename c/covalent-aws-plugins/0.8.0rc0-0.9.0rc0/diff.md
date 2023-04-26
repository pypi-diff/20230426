# Comparing `tmp/covalent-aws-plugins-0.8.0rc0.tar.gz` & `tmp/covalent-aws-plugins-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-aws-plugins-0.8.0rc0.tar", last modified: Thu Oct 27 21:26:33 2022, max compression
+gzip compressed data, was "covalent-aws-plugins-0.9.0rc0.tar", last modified: Thu Oct 27 22:22:46 2022, max compression
```

## Comparing `covalent-aws-plugins-0.8.0rc0.tar` & `covalent-aws-plugins-0.9.0rc0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/awsexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/client_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/invalid_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-10-27 21:26:33.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-10-27 21:26:33.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 21:26:33.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-27 21:26:33.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-27 21:26:33.000000 covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 21:26:33.095491 covalent-aws-plugins-0.8.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-10-27 21:26:25.000000 covalent-aws-plugins-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/awsexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/client_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/invalid_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-10-27 22:22:46.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-10-27 22:22:46.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 22:22:46.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-27 22:22:46.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-27 22:22:46.000000 covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-27 22:22:46.374611 covalent-aws-plugins-0.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-10-27 22:22:39.000000 covalent-aws-plugins-0.9.0rc0/setup.py
```

### Comparing `covalent-aws-plugins-0.8.0rc0/LICENSE` & `covalent-aws-plugins-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/PKG-INFO` & `covalent-aws-plugins-0.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-aws-plugins
-Version: 0.8.0rc0
+Version: 0.9.0rc0
 Summary: Covalent AWS Plugins
 Home-page: https://github.com/AgnostiqHQ/covalent-aws-plugins
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-aws-plugins/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-aws-plugins/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="./doc/static/AWS_Plugins.png" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
```

### Comparing `covalent-aws-plugins-0.8.0rc0/README.md` & `covalent-aws-plugins-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/__init__.py` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/awsexecutor.py` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/awsexecutor.py`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/__init__.py` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/client_exception.py` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/client_exception.py`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins/exceptions/invalid_credentials.py` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins/exceptions/invalid_credentials.py`

 * *Files identical despite different names*

### Comparing `covalent-aws-plugins-0.8.0rc0/covalent_aws_plugins.egg-info/PKG-INFO` & `covalent-aws-plugins-0.9.0rc0/covalent_aws_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-aws-plugins
-Version: 0.8.0rc0
+Version: 0.9.0rc0
 Summary: Covalent AWS Plugins
 Home-page: https://github.com/AgnostiqHQ/covalent-aws-plugins
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-aws-plugins/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-aws-plugins/archive/v0.9.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="./doc/static/AWS_Plugins.png" width=150%>
         
         [![covalent](https://img.shields.io/badge/covalent-0.177.0-purple)](https://github.com/AgnostiqHQ/covalent)
```

### Comparing `covalent-aws-plugins-0.8.0rc0/setup.py` & `covalent-aws-plugins-0.9.0rc0/setup.py`

 * *Files identical despite different names*

