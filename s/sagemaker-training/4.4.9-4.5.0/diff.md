# Comparing `tmp/sagemaker_training-4.4.9.tar.gz` & `tmp/sagemaker_training-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_training-4.4.9.tar", last modified: Wed Apr  5 16:46:19 2023, max compression
+gzip compressed data, was "dist/sagemaker_training-4.5.0.tar", last modified: Wed Apr 26 16:46:59 2023, max compression
```

## Comparing `sagemaker_training-4.4.9.tar` & `sagemaker_training-4.5.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      156 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      100 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11326 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8922 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/README.md
--rw-rw-r--   0 root         (0) root         (0)        6 2023-04-05 16:17:01.000000 sagemaker_training-4.4.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11326 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1374 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/sagemaker_training.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2902 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/src/sagemaker_training/
--rw-rw-r--   0 root         (0) root         (0)     2547 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1664 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/_entry_point_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/src/sagemaker_training/c/
--rw-rw-r--   0 root         (0) root         (0)     3533 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/c/gethostname.c
--rw-rw-r--   0 root         (0) root         (0)     7980 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/c/jsmn.c
--rw-rw-r--   0 root         (0) root         (0)     1759 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/c/jsmn.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 16:46:19.000000 sagemaker_training-4.4.9/src/sagemaker_training/cli/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      802 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/cli/train.py
--rw-rw-r--   0 root         (0) root         (0)      781 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/content_types.py
--rw-rw-r--   0 root         (0) root         (0)     7816 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/encoders.py
--rw-rw-r--   0 root         (0) root         (0)     5806 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/entry_point.py
--rw-rw-r--   0 root         (0) root         (0)    49952 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/environment.py
--rw-rw-r--   0 root         (0) root         (0)     3645 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/errors.py
--rw-rw-r--   0 root         (0) root         (0)     5871 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/files.py
--rw-rw-r--   0 root         (0) root         (0)     3013 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/functions.py
--rw-rw-r--   0 root         (0) root         (0)     8362 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/intermediate_output.py
--rw-rw-r--   0 root         (0) root         (0)     2164 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/logging_config.py
--rw-rw-r--   0 root         (0) root         (0)     6411 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/mapping.py
--rw-rw-r--   0 root         (0) root         (0)     5569 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/modules.py
--rw-rw-r--   0 root         (0) root         (0)    19388 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/mpi.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/params.py
--rw-rw-r--   0 root         (0) root         (0)    15951 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/process.py
--rw-rw-r--   0 root         (0) root         (0)     6583 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/pytorch_xla.py
--rw-rw-r--   0 root         (0) root         (0)    25554 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/record_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     8275 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/recordio.py
--rw-rw-r--   0 root         (0) root         (0)     5574 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/runner.py
--rw-rw-r--   0 root         (0) root         (0)    15735 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/smdataparallel.py
--rw-rw-r--   0 root         (0) root         (0)     1796 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/timeout.py
--rw-rw-r--   0 root         (0) root         (0)     5374 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/torch_distributed.py
--rw-rw-r--   0 root         (0) root         (0)     4459 2023-04-04 19:54:08.000000 sagemaker_training-4.4.9/src/sagemaker_training/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8922 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-04-26 16:16:54.000000 sagemaker_training-4.5.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/sagemaker_training.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2902 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1664 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/_entry_point_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/
+-rw-rw-r--   0 root         (0) root         (0)     3533 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/gethostname.c
+-rw-rw-r--   0 root         (0) root         (0)     7980 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.c
+-rw-rw-r--   0 root         (0) root         (0)     1759 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 16:46:59.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      802 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/cli/train.py
+-rw-rw-r--   0 root         (0) root         (0)      781 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/content_types.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/encoders.py
+-rw-rw-r--   0 root         (0) root         (0)     5806 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/entry_point.py
+-rw-rw-r--   0 root         (0) root         (0)    49952 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     3645 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     5871 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/files.py
+-rw-rw-r--   0 root         (0) root         (0)     3013 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/functions.py
+-rw-rw-r--   0 root         (0) root         (0)     8362 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/intermediate_output.py
+-rw-rw-r--   0 root         (0) root         (0)     2164 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/logging_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6411 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/mapping.py
+-rw-rw-r--   0 root         (0) root         (0)     5569 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/modules.py
+-rw-rw-r--   0 root         (0) root         (0)    20049 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/mpi.py
+-rw-rw-r--   0 root         (0) root         (0)     3297 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/params.py
+-rw-rw-r--   0 root         (0) root         (0)    15951 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/process.py
+-rw-rw-r--   0 root         (0) root         (0)     6583 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/pytorch_xla.py
+-rw-rw-r--   0 root         (0) root         (0)    25554 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/record_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     8275 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/recordio.py
+-rw-rw-r--   0 root         (0) root         (0)     5574 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/runner.py
+-rw-rw-r--   0 root         (0) root         (0)    15735 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/smdataparallel.py
+-rw-rw-r--   0 root         (0) root         (0)     1796 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     5374 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/torch_distributed.py
+-rw-rw-r--   0 root         (0) root         (0)     4459 2023-04-25 21:20:20.000000 sagemaker_training-4.5.0/src/sagemaker_training/trainer.py
```

### Comparing `sagemaker_training-4.4.9/LICENSE` & `sagemaker_training-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/PKG-INFO` & `sagemaker_training-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_training
-Version: 4.4.9
+Version: 4.5.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.4.9/README.md` & `sagemaker_training-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/sagemaker_training.egg-info/PKG-INFO` & `sagemaker_training-4.5.0/sagemaker_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-training
-Version: 4.4.9
+Version: 4.5.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.4.9/sagemaker_training.egg-info/SOURCES.txt` & `sagemaker_training-4.5.0/sagemaker_training.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/setup.py` & `sagemaker_training-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/__init__.py` & `sagemaker_training-4.5.0/src/sagemaker_training/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/_entry_point_type.py` & `sagemaker_training-4.5.0/src/sagemaker_training/_entry_point_type.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/c/gethostname.c` & `sagemaker_training-4.5.0/src/sagemaker_training/c/gethostname.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/c/jsmn.c` & `sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/c/jsmn.h` & `sagemaker_training-4.5.0/src/sagemaker_training/c/jsmn.h`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/cli/train.py` & `sagemaker_training-4.5.0/src/sagemaker_training/cli/train.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/content_types.py` & `sagemaker_training-4.5.0/src/sagemaker_training/content_types.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/encoders.py` & `sagemaker_training-4.5.0/src/sagemaker_training/encoders.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/entry_point.py` & `sagemaker_training-4.5.0/src/sagemaker_training/entry_point.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/environment.py` & `sagemaker_training-4.5.0/src/sagemaker_training/environment.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/errors.py` & `sagemaker_training-4.5.0/src/sagemaker_training/errors.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/files.py` & `sagemaker_training-4.5.0/src/sagemaker_training/files.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/functions.py` & `sagemaker_training-4.5.0/src/sagemaker_training/functions.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/intermediate_output.py` & `sagemaker_training-4.5.0/src/sagemaker_training/intermediate_output.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/logging_config.py` & `sagemaker_training-4.5.0/src/sagemaker_training/logging_config.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/mapping.py` & `sagemaker_training-4.5.0/src/sagemaker_training/mapping.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/modules.py` & `sagemaker_training-4.5.0/src/sagemaker_training/modules.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/mpi.py` & `sagemaker_training-4.5.0/src/sagemaker_training/mpi.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,21 +177,34 @@
         procs = [p for p in psutil.process_iter(attrs=["name"]) if p.info["name"] == "orted"]
         if procs:
             logger.info("Process[es]: %s", procs)
             return procs
         time.sleep(1)
 
 
-def _smddpmprun_command(instance_type):  # type: (str) -> list[str]
-    """When a task is of modelparallel and ddp_dist_backend is auto,
-    we use smddpmprun to set up necessary environment variables if possible.
+def _modelparallel_environment_command(instance_type):  # type: (str) -> list[str]
+    """When a task is of modelparallel
+    1. For torch DLC, we add NCCL_PROTO environment.
+    2. If the torch major version is greater 1, we add NCCL_ALGO environment.
+    3. If ddp_dist_backend is auto, we use smddpmprun to set up necessary environment
+       variables if possible.
     """
     command = []
     env = environment.Environment()
     if env.is_modelparallel_enabled:
+        pytorch_version = os.environ.get("SM_DLC_TORCH_VERSION")
+        if pytorch_version:
+            logger.info(f"PyTorch version is {pytorch_version}")
+            # Set NCCL_PROTO
+            command.extend(["-x", "NCCL_PROTO=simple"])
+            # Set NCCL_ALGO to avoid potential hang, starting from torch2.0.0
+            if int(pytorch_version.split(".")[0]) > 1:
+                command.extend(["-x", "NCCL_ALGO=ring"])
+
+        # Use smddpmprun to set up environment variables
         mp_parameters = json.loads(os.environ.get(params.SM_HP_MP_PARAMETERS, "{}"))
         ddp_dist_backend = mp_parameters.get("ddp_dist_backend", "auto")
         if ddp_dist_backend == "auto":
             if env.is_smddpmprun_installed:
                 command.extend(["smddpmprun", "-i", instance_type, "--allow-bypass"])
         else:
             logger.info(f"{ddp_dist_backend} is used as DDP backend for training")
@@ -353,15 +366,15 @@
         ]:
             if credential in os.environ:
                 command.extend(["-x", credential])
 
         for name in self._env_vars:
             command.extend(["-x", name])
 
-        command.extend(_smddpmprun_command(self._instance_type))
+        command.extend(_modelparallel_environment_command(self._instance_type))
 
         command.extend(super(MasterRunner, self)._create_command())
         return command
 
     def _python_command(self):
         """Use mpi4py to force processes to abort if an uncaught exception occurs.
         https://docs.chainer.org/en/stable/chainermn/tutorial/tips_faqs.html#mpi-process-hangs-after-an-unhandled-python-exception
```

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/params.py` & `sagemaker_training-4.5.0/src/sagemaker_training/params.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/process.py` & `sagemaker_training-4.5.0/src/sagemaker_training/process.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/pytorch_xla.py` & `sagemaker_training-4.5.0/src/sagemaker_training/pytorch_xla.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/record_pb2.py` & `sagemaker_training-4.5.0/src/sagemaker_training/record_pb2.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/recordio.py` & `sagemaker_training-4.5.0/src/sagemaker_training/recordio.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/runner.py` & `sagemaker_training-4.5.0/src/sagemaker_training/runner.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/smdataparallel.py` & `sagemaker_training-4.5.0/src/sagemaker_training/smdataparallel.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/timeout.py` & `sagemaker_training-4.5.0/src/sagemaker_training/timeout.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/torch_distributed.py` & `sagemaker_training-4.5.0/src/sagemaker_training/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.4.9/src/sagemaker_training/trainer.py` & `sagemaker_training-4.5.0/src/sagemaker_training/trainer.py`

 * *Files identical despite different names*

