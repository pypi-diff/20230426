# Comparing `tmp/dequeai-0.766.tar.gz` & `tmp/dequeai-0.768.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.766.tar", last modified: Wed Apr 26 14:48:51 2023, max compression
+gzip compressed data, was "dequeai-0.768.tar", last modified: Wed Apr 26 15:27:57 2023, max compression
```

## Comparing `dequeai-0.766.tar` & `dequeai-0.768.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:48:51.869507 dequeai-0.766/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 14:48:51.869507 dequeai-0.766/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:48:51.869507 dequeai-0.766/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.766/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.766/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.766/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.766/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-25 19:31:26.000000 dequeai-0.766/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29846 2023-04-26 14:48:28.000000 dequeai-0.766/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.766/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.766/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.766/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.766/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:48:51.869507 dequeai-0.766/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 14:48:51.000000 dequeai-0.766/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 14:48:51.000000 dequeai-0.766/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:48:51.000000 dequeai-0.766/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-26 14:48:51.000000 dequeai-0.766/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 14:48:51.000000 dequeai-0.766/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:48:51.869507 dequeai-0.766/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-26 14:48:38.000000 dequeai-0.766/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.535545 dequeai-0.768/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 15:27:57.535545 dequeai-0.768/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.531545 dequeai-0.768/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.768/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.768/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.768/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.768/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.768/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29846 2023-04-26 14:48:28.000000 dequeai-0.768/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.768/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.768/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.768/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.768/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.531545 dequeai-0.768/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:27:57.535545 dequeai-0.768/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-26 15:27:42.000000 dequeai-0.768/setup.py
```

### Comparing `dequeai-0.766/dequeai/datatypes.py` & `dequeai-0.768/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.766/dequeai/dequeai.py` & `dequeai-0.768/dequeai/dequeai.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from dequeai.dequeai_run import Run
 
 run = Run()
 
 
-def init( user_name, project_name, api_key):
-    run.init(user_name, project_name, api_key)
+def init( user_name, api_key, project_name):
+    run.init(user_name=user_name, api_key=api_key, project_name=project_name)
 
 def finish():
     run.finish()
 
 def log( data, step=None, commit=True):
-    run.log(data, step, commit)
+    run.log(data=data, step=step, commit=commit)
 
 def log_hyperparams( hyperparams):
-    run.log_hyperparams(hyperparams)
+    run.log_hyperparams(hyperparams=hyperparams)
 
 def log_artifact(artifact_type, path):
-    run.log_artifact(artifact_type, path)
+    run.log_artifact(artifact_type=artifact_type, path=path)
 
 def load_artifact(artifact_type, run_id):
-    run.load_artifact(artifact_type, run_id)
+    run.load_artifact(artifact_type=artifact_type, run_id=run_id)
 
 def register_artifacts(latest=True, label=None, tags=None):
-    run.register_artifacts(latest, label, tags)
+    run.register_artifacts(latest=latest, label=label, tags=tags)
 
 def compare_runs(project_name, metric_key):
-    run.compare_runs(project_name, metric_key)
+    run.compare_runs(project_name=project_name, metric_key=metric_key)
 
 def read_best_run(project_name, metric_key):
-    run.read_best_run(project_name, metric_key)
+    run.read_best_run(project_name=project_name, metric_key=metric_key)
```

### Comparing `dequeai-0.766/dequeai/dequeai_run.py` & `dequeai-0.768/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.766/dequeai/parsing_service.py` & `dequeai-0.768/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.766/dequeai/rest_connect.py` & `dequeai-0.768/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.766/dequeai/util.py` & `dequeai-0.768/dequeai/util.py`

 * *Files identical despite different names*

