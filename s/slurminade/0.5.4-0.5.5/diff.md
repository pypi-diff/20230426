# Comparing `tmp/slurminade-0.5.4.tar.gz` & `tmp/slurminade-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurminade-0.5.4.tar", last modified: Tue Apr 25 18:09:43 2023, max compression
+gzip compressed data, was "slurminade-0.5.5.tar", last modified: Tue Apr 25 18:41:02 2023, max compression
```

## Comparing `slurminade-0.5.4.tar` & `slurminade-0.5.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:09:43.661662 slurminade-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 18:09:36.000000 slurminade-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-25 18:09:43.661662 slurminade-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-25 18:09:36.000000 slurminade-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 18:09:36.000000 slurminade-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:09:43.661662 slurminade-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-25 18:09:36.000000 slurminade-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:09:43.661662 slurminade-0.5.4/slurminade/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/function_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 18:09:36.000000 slurminade-0.5.4/slurminade/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:09:43.661662 slurminade-0.5.4/slurminade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 18:09:43.000000 slurminade-0.5.4/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.638523 slurminade-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 18:40:57.000000 slurminade-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-25 18:41:02.638523 slurminade-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-25 18:40:57.000000 slurminade-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 18:40:57.000000 slurminade-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:41:02.638523 slurminade-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-25 18:40:57.000000 slurminade-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.634523 slurminade-0.5.5/slurminade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 18:40:57.000000 slurminade-0.5.5/slurminade/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:41:02.638523 slurminade-0.5.5/slurminade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 18:41:02.000000 slurminade-0.5.5/slurminade.egg-info/top_level.txt
```

### Comparing `slurminade-0.5.4/LICENSE` & `slurminade-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/PKG-INFO` & `slurminade-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 0.5.4
+Version: 0.5.5
 Summary: A decorator-based slurm runner
 Home-page: https://github.com/d-krupke/slurminade
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: slurm
 Platform: UNKNOWN
@@ -212,14 +212,15 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
```

### Comparing `slurminade-0.5.4/README.md` & `slurminade-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
```

### Comparing `slurminade-0.5.4/setup.py` & `slurminade-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="slurminade",
-    version="0.5.4",
+    version="0.5.5",
     description="A decorator-based slurm runner",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `slurminade-0.5.4/slurminade/__init__.py` & `slurminade-0.5.5/slurminade/__init__.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/batch.py` & `slurminade-0.5.5/slurminade/batch.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/conf.py` & `slurminade-0.5.5/slurminade/conf.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/dispatcher.py` & `slurminade-0.5.5/slurminade/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     def __init__(self):
         super().__init__()
         self.max_arg_length = DEFAULT_MAX_ARG_LENGTH
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
+        dispatch_guard()
         command = create_slurminade_command(funcs, self.max_arg_length)
         os.system(command)
         return -1
 
     def srun(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
         dispatch_guard()
         subprocess.run(command, check=True)
```

### Comparing `slurminade-0.5.4/slurminade/execute.py` & `slurminade-0.5.5/slurminade/execute.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/function.py` & `slurminade-0.5.5/slurminade/function.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/function_map.py` & `slurminade-0.5.5/slurminade/function_map.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/guard.py` & `slurminade-0.5.5/slurminade/guard.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade/options.py` & `slurminade-0.5.5/slurminade/options.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.4/slurminade.egg-info/PKG-INFO` & `slurminade-0.5.5/slurminade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 0.5.4
+Version: 0.5.5
 Summary: A decorator-based slurm runner
 Home-page: https://github.com/d-krupke/slurminade
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: slurm
 Platform: UNKNOWN
@@ -212,14 +212,15 @@
 - function.py: Contains the code for making a function slurm-compatible.
 - function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.5: Fixing bug guard bug in subprocess dispatcher.
 * 0.5.4: Dispatched function calls that are too long for the command line now use a temporary file instead.
 * 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
```

