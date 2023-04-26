# Comparing `tmp/xh-py-project-versioning-0.0.2.tar.gz` & `tmp/xh-py-project-versioning-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-py-project-versioning-0.0.2.tar", last modified: Tue Apr 18 06:58:51 2023, max compression
+gzip compressed data, was "xh-py-project-versioning-0.0.3.tar", last modified: Wed Apr 26 09:37:32 2023, max compression
```

## Comparing `xh-py-project-versioning-0.0.2.tar` & `xh-py-project-versioning-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.684875 xh-py-project-versioning-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyPiRepo.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyProject.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:32.817540 xh-py-project-versioning-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 09:37:32.817540 xh-py-project-versioning-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:37:32.817540 xh-py-project-versioning-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:32.813540 xh-py-project-versioning-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:32.817540 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/PyPiRepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/PyProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-26 09:37:21.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:37:32.817540 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 09:37:32.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 09:37:32.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:37:32.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 09:37:32.000000 xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/top_level.txt
```

### Comparing `xh-py-project-versioning-0.0.2/LICENSE.txt` & `xh-py-project-versioning-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-py-project-versioning-0.0.2/PKG-INFO` & `xh-py-project-versioning-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-py-project-versioning
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for increate version number and check version mismatch
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-py-project-versioning
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-py-project-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-py-project-versioning-0.0.2/pyproject.toml` & `xh-py-project-versioning-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-py-project-versioning"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library for increate version number and check version mismatch"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "xethhung"
 email = "pypi@xethh.dev"
```

### Comparing `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyProject.py` & `xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/PyProject.py`

 * *Files identical despite different names*

### Comparing `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/__main__.py` & `xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,22 +56,27 @@
             print(f"Remote version[{str(online_version)}] != Local version[{version_str}]")
         exit()
 
     sem_ver = SemVer.from_str(version_str)
     old_version = str(sem_ver)
     op_tag = ""
     if argv.release:
+        if sem_ver.build is None:
+            raise Exception(f"Version[{sem_ver}] is applicable for release due to build meta is empty")
         sem_ver.unset_build()
         sem_ver.unset_pre_release()
         op_tag = "release"
     elif sem_ver.is_pre_release_not_set():
         if version_mod == "major":
             sem_ver.increase_major()
+            sem_ver.minor = 0
+            sem_ver.patch = 0
         elif version_mod == "minor":
             sem_ver.increase_minor()
+            sem_ver.patch = 0
         elif version_mod == "patch":
             sem_ver.increase_patch()
 
         sem_ver.set_pre_release(pre_build_tag)
         sem_ver.set_build(0)
         op_tag="dev start"
```

### Comparing `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/versioning.py` & `xh-py-project-versioning-0.0.3/src/xh_py_project_versioning/versioning.py`

 * *Files identical despite different names*

### Comparing `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/PKG-INFO` & `xh-py-project-versioning-0.0.3/src/xh_py_project_versioning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-py-project-versioning
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for increate version number and check version mismatch
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-py-project-versioning
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-py-project-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

