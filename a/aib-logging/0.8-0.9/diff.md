# Comparing `tmp/aib_logging-0.8.tar.gz` & `tmp/aib_logging-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-0.8.tar", last modified: Thu Apr 20 18:12:04 2023, max compression
+gzip compressed data, was "aib_logging-0.9.tar", last modified: Wed Apr 26 07:09:11 2023, max compression
```

## Comparing `aib_logging-0.8.tar` & `aib_logging-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 18:12:04.248056 aib_logging-0.8/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-0.8/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-20 18:12:04.248056 aib_logging-0.8/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-0.8/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      621 2023-04-20 18:11:02.000000 aib_logging-0.8/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-04-20 18:12:04.249056 aib_logging-0.8/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 18:12:04.241056 aib_logging-0.8/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 18:12:04.246056 aib_logging-0.8/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-0.8/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    12450 2023-04-20 18:10:45.000000 aib_logging-0.8/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-20 18:12:04.247056 aib_logging-0.8/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-20 18:12:04.000000 aib_logging-0.8/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-04-20 18:12:04.000000 aib_logging-0.8/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-04-20 18:12:04.000000 aib_logging-0.8/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-04-20 18:12:04.000000 aib_logging-0.8/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-04-20 18:12:04.000000 aib_logging-0.8/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.756364 aib_logging-0.9/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-0.9/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-26 07:09:11.756364 aib_logging-0.9/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-0.9/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      621 2023-04-26 07:08:30.000000 aib_logging-0.9/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-04-26 07:09:11.756364 aib_logging-0.9/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.751363 aib_logging-0.9/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.754364 aib_logging-0.9/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-0.9/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14074 2023-04-26 07:08:23.000000 aib_logging-0.9/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-04-26 07:09:11.756364 aib_logging-0.9/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      526 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-04-26 07:09:11.000000 aib_logging-0.9/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-0.8/LICENSE.txt` & `aib_logging-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-0.8/PKG-INFO` & `aib_logging-0.9/src/aib_logging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aib_logging
-Version: 0.8
+Name: aib-logging
+Version: 0.9
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-0.8/pyproject.toml` & `aib_logging-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "0.8"
+version = "0.9"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aib_logging-0.8/src/aib_logging/logger.py` & `aib_logging-0.9/src/aib_logging/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,8 @@
 class aib_logger:
-    """
-    This class use to add custom logs for vertex AI
-    ...
-
-    Atributes:
-        project(str): project id where your vertex AI pipeline running
-        pipeline_name(str): name of pipeline
-        logger_name(str): name of custom logger 
-            (default is aib_custom_logger)
-    ...
-
-    Methods:
-        score_logs(): to log model performance score in custom logs.
-        data_stat_log(): to log data statistic in custom logs.
-    """
     from enum import Enum
     
     class Categories(Enum):
         MODEL="Model"
         DATA="Data"
         METRIC="Metric"
         OTHER="Other"
@@ -34,16 +19,24 @@
     class Severities(Enum):
         INFO="INFO"
         WARNING="WARNING"
         ERROR="ERROR"
 
     def __init__(self, project:str, pipeline_name:str="", logger_name:str="aib_custom_logger"):
         """
+        This class use to add custom logs for vertex AI.
         class initialization with given project and pipeline name.
 
+        ...
+        Methods:
+        score_logs(): to log model performance score in custom logs.
+        data_stat_log(): to log data statistic in custom logs.
+        model_log(): to log model information in logs.
+        ...
+
         Args:
             project(str): project id where your vertex AI pipeline running
             pipeline_name(str): name of pipeline
             logger_name(str): name of custom logger 
                 (default is aib_custom_logger)
         Returns:
             None
@@ -322,7 +315,64 @@
             "message":msg,
             "object":object
         }
         for key, value in kwargs.items():
                 payload[key]=value
         # Send the Log request
         self.logger.log_struct(payload, severity=severity.value)
+    
+    def model_log(
+        self,
+        msg:str,
+        category:Categories=Categories.MODEL,
+        severity:Severities=Severities.INFO,
+        model_name:str='AIB-test-model',
+        action:str='Create',
+        version:str='default',
+        extra_labels:list=[],
+        object:dict={},
+        **kwargs
+        ):
+        """
+        Method to add model information into logs
+
+        example:
+        from aib_logging.logger import aib_logger
+        logger = aib_logger("my-gcp-project-name",pipeline_name="pipeline_job_name")
+    
+        logger.model_log(
+            "This is test for model info",
+            model_name='AIB-test-model',
+            action='update',
+            version='champion',
+            )
+
+        Args:
+            msg:str,
+            category: Categories of log type 
+                default is model,
+            action(str): Actions perform for logs 
+                default is 'create',
+            severity: Severities for logs,
+                default is INFO,
+            model_name(str): Name of model
+                default is 'AIB-test-model'
+            version(str): Model version
+                default is 'default'
+        """
+        import inspect
+        payload={
+            "pipeline_run_name":self.pipeline_name,
+            "component_name": inspect.stack()[1].function,
+            "project":self.project,
+            "category":category.value,
+            "action":action,
+            "model_name":model_name,
+            "version":version,
+            "extra_labels":extra_labels,
+            "message":msg,
+            "object":object
+        }
+        for key, value in kwargs.items():
+                payload[key]=value
+        # Send the Log request
+        self.logger.log_struct(payload, severity=severity.value)
```

### Comparing `aib_logging-0.8/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aib-logging
-Version: 0.8
+Name: aib_logging
+Version: 0.9
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

