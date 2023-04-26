# Comparing `tmp/executors-0.6a0-py2.py3-none-any.whl.zip` & `tmp/executors-0.6a1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13020 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1600 b- defN 23-Apr-25 21:19 executors/__init__.py
--rw-r--r--  2.0 unx      234 b- defN 23-Apr-25 21:23 executors/__version__.py
--rw-r--r--  2.0 unx      494 b- defN 23-Apr-25 21:19 executors/commons/__init__.py
--rw-r--r--  2.0 unx      129 b- defN 23-Apr-25 21:19 executors/exceptions/__init__.py
--rw-r--r--  2.0 unx     3176 b- defN 23-Apr-25 21:19 executors/local/__init__.py
--rw-r--r--  2.0 unx     6034 b- defN 23-Apr-25 21:19 executors/lsf/__init__.py
--rw-r--r--  2.0 unx     5556 b- defN 23-Apr-25 21:19 executors/models/__init__.py
--rw-r--r--  2.0 unx     8350 b- defN 23-Apr-25 21:19 executors/pbsubmit/__init__.py
--rw-r--r--  2.0 unx     9725 b- defN 23-Apr-25 21:20 executors/slurm/__init__.py
--rw-r--r--  2.0 unx      265 b- defN 23-Apr-25 21:25 executors-0.6a0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-25 21:25 executors-0.6a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-25 21:25 executors-0.6a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1059 b- defN 23-Apr-25 21:25 executors-0.6a0.dist-info/RECORD
-13 files, 36742 bytes uncompressed, 11252 bytes compressed:  69.4%
+Zip file size: 13050 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1600 b- defN 23-Apr-25 22:11 executors/__init__.py
+-rw-r--r--  2.0 unx      234 b- defN 23-Apr-25 22:15 executors/__version__.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Apr-25 22:11 executors/commons/__init__.py
+-rw-r--r--  2.0 unx      129 b- defN 23-Apr-25 22:11 executors/exceptions/__init__.py
+-rw-r--r--  2.0 unx     3176 b- defN 23-Apr-25 22:11 executors/local/__init__.py
+-rw-r--r--  2.0 unx     6034 b- defN 23-Apr-25 22:11 executors/lsf/__init__.py
+-rw-r--r--  2.0 unx     5596 b- defN 23-Apr-25 22:12 executors/models/__init__.py
+-rw-r--r--  2.0 unx     8350 b- defN 23-Apr-25 22:11 executors/pbsubmit/__init__.py
+-rw-r--r--  2.0 unx     9729 b- defN 23-Apr-25 22:12 executors/slurm/__init__.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Apr-25 22:22 executors-0.6a1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-25 22:22 executors-0.6a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-25 22:22 executors-0.6a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1059 b- defN 23-Apr-25 22:22 executors-0.6a1.dist-info/RECORD
+13 files, 36805 bytes uncompressed, 11282 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: executors/pbsubmit/__init__.py
 Comment: 
 
 Filename: executors/slurm/__init__.py
 Comment: 
 
-Filename: executors-0.6a0.dist-info/METADATA
+Filename: executors-0.6a1.dist-info/METADATA
 Comment: 
 
-Filename: executors-0.6a0.dist-info/WHEEL
+Filename: executors-0.6a1.dist-info/WHEEL
 Comment: 
 
-Filename: executors-0.6a0.dist-info/top_level.txt
+Filename: executors-0.6a1.dist-info/top_level.txt
 Comment: 
 
-Filename: executors-0.6a0.dist-info/RECORD
+Filename: executors-0.6a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## executors/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'executors'
 __description__ = 'Job scheduling abstractions'
 __url__ = 'https://github.com/harvard-nrg/executors'
-__version__ = '0.6a0'
+__version__ = '0.6a1'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## executors/models/__init__.py

```diff
@@ -2,28 +2,29 @@
 import time
 import logging
 import executors.commons as commons
 
 logger = logging.getLogger(__name__)
 
 class Job(object):
-    def __init__(self, command, memory, time, cpus=1, nodes=1, name=None, output=None, error=None, parent=None):
+    def __init__(self, command, memory, time, cpus=1, nodes=1, gpus=None, name=None, output=None, error=None, parent=None):
         self.name = name
         self.command = command
         self.memory = memory
         self.time = time
         self.parent = parent
         self.output = output
         self.error = error
-        # these are set by the Executor object
+        self.cpus = cpus
+        self.gpus = gpus
+        self.nodes = nodes
+        # these fields are managed by an Executor
         self.pid = None
         self.returncode = None
         self.active = None
-        self.cpus = None
-        self.nodes = None
 
 class JobArray(object):
     def __init__(self, executor, cancel_on_fail=False):
         '''
         :param executor: Executor instance
         :type executor: :mod:`executors.models.AbstractExecutor`
         :param cancel_on_fail: Cancel remaining jobs if any job fails
```

## executors/slurm/__init__.py

```diff
@@ -266,15 +266,15 @@
         if hasattr(job, 'name') and job.name:
             arguments.extend(['--job-name', job.name])
         if hasattr(job, 'memory') and job.memory:
             arguments.extend(['--mem', job.memory])
         if hasattr(job, 'cpus') and job.cpus:
             arguments.extend(['--ntasks', str(job.cpus)])
         if hasattr(job, 'gpus') and job.gpus:
-            arguments.extend(['--gres', str(job.gpus)])
+            arguments.extend(['--gres', f'gpu:{job.gpus}'])
         if hasattr(job, 'nodes') and job.nodes:
             arguments.extend(['--nodes', str(job.nodes)])
         if hasattr(job, 'output') and job.output:
             arguments.extend(['--output', os.path.expanduser(job.output)])
         if hasattr(job, 'error') and job.error:
             arguments.extend(['--error', os.path.expanduser(job.error)])
         if hasattr(job, 'time') and job.time:
```

