# Comparing `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.3.3.tar.gz` & `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.3.3.tar", last modified: Fri Apr 21 14:33:48 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.3.4.tar", last modified: Wed Apr 26 16:54:25 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3.tar` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 14:33:48.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:33:48.989458 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-21 14:31:35.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:25.368177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-26 16:54:25.368177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:25.364177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:25.368177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 16:54:25.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 16:54:25.372177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:54:25.368177 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 16:52:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.3.4/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.3.3
+Version: 3.3.4
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/README.md` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers/__init__.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers/config.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.3.3
+Version: 3.3.4
 Summary: AWS Loadbalancers Cleaner Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.3.3/setup.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-aws-loadbalancers",
-    version="3.3.3",
+    version="3.3.4",
     description="AWS Loadbalancers Cleaner Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": [
```

