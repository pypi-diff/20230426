# Comparing `tmp/pyplanpro-0.0.2.tar.gz` & `tmp/pyplanpro-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplanpro-0.0.2.tar", last modified: Wed Apr 26 05:45:22 2023, max compression
+gzip compressed data, was "pyplanpro-0.0.3.tar", last modified: Wed Apr 26 06:19:49 2023, max compression
```

## Comparing `pyplanpro-0.0.2.tar` & `pyplanpro-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/PyPlanPro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/PyPlanPro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/models/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/PyPlanPro/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/PyPlanPro/scheduler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/pyplanpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 05:45:22.000000 pyplanpro-0.0.2/pyplanpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 05:45:22.000000 pyplanpro-0.0.2/pyplanpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:45:22.000000 pyplanpro-0.0.2/pyplanpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 05:45:22.000000 pyplanpro-0.0.2/pyplanpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 05:45:22.000000 pyplanpro-0.0.2/pyplanpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:22.962628 pyplanpro-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:45:09.000000 pyplanpro-0.0.2/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.973352 pyplanpro-0.0.3/PyPlanPro/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/PyPlanPro/scheduler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/pyplanpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 06:19:49.000000 pyplanpro-0.0.3/pyplanpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:49.977352 pyplanpro-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:19:36.000000 pyplanpro-0.0.3/tests/test_scheduler.py
```

### Comparing `pyplanpro-0.0.2/LICENSE` & `pyplanpro-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.2/PKG-INFO` & `pyplanpro-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.2
+Version: 0.0.3
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.2/PyPlanPro/models/task.py` & `pyplanpro-0.0.3/PyPlanPro/models/task.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.2/PyPlanPro/scheduler/core.py` & `pyplanpro-0.0.3/PyPlanPro/scheduler/core.py`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.2/README.md` & `pyplanpro-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyplanpro-0.0.2/pyplanpro.egg-info/PKG-INFO` & `pyplanpro-0.0.3/pyplanpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplanpro
-Version: 0.0.2
+Version: 0.0.3
 Summary: Task scheduler for python
 Home-page: https://github.com/Oestergaard-A-S/PyPlanPro
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyplanpro-0.0.2/setup.py` & `pyplanpro-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 setup(
     name='pyplanpro',
-    version='0.0.2',
+    version='0.0.3',
     author='Jacob Østergaard Nielsen',
     author_email='jaoe@oestergaard-as.dk',
     description='Task scheduler for python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     url='https://github.com/Oestergaard-A-S/PyPlanPro',
     install_requires= read_requirements("requirements.txt"),
```

