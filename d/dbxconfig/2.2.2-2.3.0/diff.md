# Comparing `tmp/dbxconfig-2.2.2.tar.gz` & `tmp/dbxconfig-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-2.2.2.tar", last modified: Sun Apr 23 10:15:56 2023, max compression
+gzip compressed data, was "dbxconfig-2.3.0.tar", last modified: Tue Apr 25 23:45:15 2023, max compression
```

## Comparing `dbxconfig-2.2.2.tar` & `dbxconfig-2.3.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      463 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1204 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3115 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-23 10:15:56.000000 dbxconfig-2.2.2/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-23 10:15:56.059765 dbxconfig-2.2.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1082 2023-04-23 10:15:02.000000 dbxconfig-2.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3158 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      463 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2848 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1204 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3314 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3115 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3710 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-25 23:45:15.000000 dbxconfig-2.3.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-25 23:45:15.738387 dbxconfig-2.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-04-25 23:44:16.000000 dbxconfig-2.3.0/setup.py
```

### Comparing `dbxconfig-2.2.2/PKG-INFO` & `dbxconfig-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.2.2
+Version: 2.3.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.2.2/README.md` & `dbxconfig-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/_config.py` & `dbxconfig-2.3.0/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/_table.py` & `dbxconfig-2.3.0/dbxconfig/_table.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/_tables.py` & `dbxconfig-2.3.0/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/_timeslice.py` & `dbxconfig-2.3.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/_utils.py` & `dbxconfig-2.3.0/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.3.0/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.3.0/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/dataset/_factory.py` & `dbxconfig-2.3.0/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig/dataset/_read.py` & `dbxconfig-2.3.0/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-2.2.2/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.3.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 2.2.2
+Version: 2.3.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-2.2.2/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.3.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,11 @@
 dbxconfig.egg-info/requires.txt
 dbxconfig.egg-info/top_level.txt
 dbxconfig/dataset/__init__.py
 dbxconfig/dataset/_dataset.py
 dbxconfig/dataset/_deltalake.py
 dbxconfig/dataset/_factory.py
 dbxconfig/dataset/_read.py
-dbxconfig/dataset/_write.py
+dbxconfig/dataset/_write.py
+dbxconfig/workflow/__init__.py
+dbxconfig/workflow/_multi_threaded.py
+dbxconfig/workflow/_notebook.py
```

### Comparing `dbxconfig-2.2.2/setup.py` & `dbxconfig-2.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="2.2.2",
+    version="2.3.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
@@ -25,15 +25,16 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=[
         "dbxconfig",
-        "dbxconfig.dataset"
+        "dbxconfig.dataset",
+        "dbxconfig.workflow"
     ],
     install_requires=[
           'PyYAML',
           'jinja2',
           'pydantic'
       ],
     zip_safe=False
```

