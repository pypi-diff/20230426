# Comparing `tmp/idds-workflow-1.2.4.tar.gz` & `tmp/idds-workflow-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-workflow-1.2.4.tar", last modified: Tue Apr 25 17:21:31 2023, max compression
+gzip compressed data, was "idds-workflow-1.2.5.tar", last modified: Tue Apr 25 19:18:00 2023, max compression
```

## Comparing `idds-workflow-1.2.4.tar` & `idds-workflow-1.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.566309 idds-workflow-1.2.4/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/lib/idds/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 17:21:25.000000 idds-workflow-1.2.4/lib/idds/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    80253 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/work.py
--rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/lib/idds/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    81692 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/work.py
--rw-r--r--   0 runner    (1001) docker     (123)   103034 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/lib/idds/workflowv2/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/lib/idds_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 17:21:31.000000 idds-workflow-1.2.4/lib/idds_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 17:21:31.000000 idds-workflow-1.2.4/lib/idds_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:21:31.000000 idds-workflow-1.2.4/lib/idds_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 17:21:31.000000 idds-workflow-1.2.4/lib/idds_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 17:21:31.000000 idds-workflow-1.2.4/lib/idds_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-25 17:21:10.000000 idds-workflow-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.566309 idds-workflow-1.2.4/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:21:31.570309 idds-workflow-1.2.4/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-25 17:21:25.000000 idds-workflow-1.2.4/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.636350 idds-workflow-1.2.5/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/lib/idds/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 19:17:56.000000 idds-workflow-1.2.5/lib/idds/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80253 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/lib/idds/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81692 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103034 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/lib/idds/workflowv2/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/lib/idds_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 19:18:00.000000 idds-workflow-1.2.5/lib/idds_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 19:18:00.000000 idds-workflow-1.2.5/lib/idds_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:18:00.000000 idds-workflow-1.2.5/lib/idds_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 19:18:00.000000 idds-workflow-1.2.5/lib/idds_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 19:18:00.000000 idds-workflow-1.2.5/lib/idds_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-25 19:17:47.000000 idds-workflow-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.636350 idds-workflow-1.2.5/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:18:00.640350 idds-workflow-1.2.5/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-25 19:17:56.000000 idds-workflow-1.2.5/tools/env/environment.yml
```

### Comparing `idds-workflow-1.2.4/LICENSE.rst` & `idds-workflow-1.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/PKG-INFO` & `idds-workflow-1.2.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.2.4
+Version: 1.2.5
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/base.py` & `idds-workflow-1.2.5/lib/idds/workflow/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/datawork.py` & `idds-workflow-1.2.5/lib/idds/workflow/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/processingwork.py` & `idds-workflow-1.2.5/lib/idds/workflow/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/utils.py` & `idds-workflow-1.2.5/lib/idds/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/work.py` & `idds-workflow-1.2.5/lib/idds/workflow/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflow/workflow.py` & `idds-workflow-1.2.5/lib/idds/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/base.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/datawork.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/processingwork.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/utils.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/work.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds/workflowv2/workflow.py` & `idds-workflow-1.2.5/lib/idds/workflowv2/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/lib/idds_workflow.egg-info/PKG-INFO` & `idds-workflow-1.2.5/lib/idds_workflow.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.2.4
+Version: 1.2.5
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.2.4/lib/idds_workflow.egg-info/SOURCES.txt` & `idds-workflow-1.2.5/lib/idds_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.4/setup.py` & `idds-workflow-1.2.5/setup.py`

 * *Files identical despite different names*

