# Comparing `tmp/dequeai-0.750.tar.gz` & `tmp/dequeai-0.764.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.750.tar", last modified: Tue Apr 25 19:07:47 2023, max compression
+gzip compressed data, was "dequeai-0.764.tar", last modified: Tue Apr 25 23:00:30 2023, max compression
```

## Comparing `dequeai-0.750.tar` & `dequeai-0.764.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:47.522387 dequeai-0.750/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-25 19:07:47.522387 dequeai-0.750/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:47.522387 dequeai-0.750/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.750/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.750/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.750/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.750/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.750/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29598 2023-04-25 19:07:23.000000 dequeai-0.750/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.750/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.750/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.750/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.750/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:47.522387 dequeai-0.750/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-25 19:07:47.000000 dequeai-0.750/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-25 19:07:47.000000 dequeai-0.750/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 19:07:47.000000 dequeai-0.750/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-25 19:07:47.000000 dequeai-0.750/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 19:07:47.000000 dequeai-0.750/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 19:07:47.522387 dequeai-0.750/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-24 00:07:51.000000 dequeai-0.750/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:00:30.431484 dequeai-0.764/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-25 23:00:30.431484 dequeai-0.764/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:00:30.431484 dequeai-0.764/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.764/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.764/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.764/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.764/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-25 19:31:26.000000 dequeai-0.764/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29594 2023-04-25 19:11:46.000000 dequeai-0.764/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.764/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.764/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.764/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.764/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:00:30.431484 dequeai-0.764/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-25 23:00:29.000000 dequeai-0.764/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-25 23:00:30.000000 dequeai-0.764/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 23:00:30.000000 dequeai-0.764/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-25 23:00:30.000000 dequeai-0.764/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 23:00:30.000000 dequeai-0.764/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 23:00:30.431484 dequeai-0.764/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-25 23:00:17.000000 dequeai-0.764/setup.py
```

### Comparing `dequeai-0.750/dequeai/datatypes.py` & `dequeai-0.764/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.750/dequeai/dequeai.py` & `dequeai-0.764/dequeai/dequeai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dequeai.dequeai_run import Run
 
 run = Run()
 
 
-def init( user_name, project_name=None, api_key=None):
+def init( user_name, project_name, api_key):
     run.init(user_name, project_name, api_key)
 
 def finish():
     run.finish()
 
 def log( data, step=None, commit=True):
     run.log(data, step, commit)
```

### Comparing `dequeai-0.750/dequeai/dequeai_run.py` & `dequeai-0.764/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         #if self._workload_type is None or self._workload_id is None:
             #raise ValueError(
                # "Deque AI package is only supported wihtin the Creator's App. Download the app from https://deque.ai")
 
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
         if project_name is None:
-                raise ValueError("Project name cannot be empty")
+            raise ValueError("Project name cannot be empty")
         else:
             self._project_name = project_name
         self._run_id = str(coolname.generate_slug(2))
         self._step = 1
         # p2 = multiprocessing.Process(target=self._start_parser)
         # p2.start()
         self._run_meta_data = {"submission_id": self._submission_id, "run_id": self._run_id,
```

### Comparing `dequeai-0.750/dequeai/parsing_service.py` & `dequeai-0.764/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.750/dequeai/rest_connect.py` & `dequeai-0.764/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.750/dequeai/util.py` & `dequeai-0.764/dequeai/util.py`

 * *Files identical despite different names*

