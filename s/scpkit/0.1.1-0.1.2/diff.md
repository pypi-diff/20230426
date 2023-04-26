# Comparing `tmp/scpkit-0.1.1.tar.gz` & `tmp/scpkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.1.1.tar", last modified: Tue Apr 25 00:52:00 2023, max compression
+gzip compressed data, was "scpkit-0.1.2.tar", last modified: Tue Apr 25 18:00:00 2023, max compression
```

## Comparing `scpkit-0.1.1.tar` & `scpkit-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 00:51:51.000000 scpkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 00:52:00.847450 scpkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-25 00:51:51.000000 scpkit-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 00:51:51.000000 scpkit-0.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.843450 scpkit-0.1.1/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 00:52:00.847450 scpkit-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:51:51.000000 scpkit-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-25 00:51:51.000000 scpkit-0.1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 17:59:51.000000 scpkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-25 18:00:00.870787 scpkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-25 17:59:51.000000 scpkit-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 17:59:51.000000 scpkit-0.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.866787 scpkit-0.1.2/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-25 17:59:51.000000 scpkit-0.1.2/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 18:00:00.000000 scpkit-0.1.2/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 18:00:00.870787 scpkit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:59:51.000000 scpkit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:00:00.870787 scpkit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-25 17:59:51.000000 scpkit-0.1.2/tests/test.py
```

### Comparing `scpkit-0.1.1/LICENSE` & `scpkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.1/scpkit/main.py` & `scpkit-0.1.2/scpkit/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Usage:
     main.py (validate | merge) [--sourcefiles sourcefiles] [--profile profile] [ --outdir outdir] [--validate-after-merge] [--readable]
 
 Options:
     -h --help                   Show this screen.
     --version                   Show version.
     --sourcefiles sourcefiles   Directory path to SCP files in json format
-    --outdir outdir             Directory to write new SCP files
+    --outdir outdir             Directory to write new SCP files [Default: ./]
     --profile profile           AWS profile name
     --validate-after-merge      Validate the policies after merging them
     --readable                  Leave indentation and some whitespace to make the SCPs readable
 """
 from docopt import docopt
 from .src.validate import validate_policies
 from .src.merge import scp_merge, get_files_in_dir
```

### Comparing `scpkit-0.1.1/scpkit/src/merge.py` & `scpkit-0.1.2/scpkit/src/merge.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.1/scpkit/src/model.py` & `scpkit-0.1.2/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.1/scpkit/src/util.py` & `scpkit-0.1.2/scpkit/src/util.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.1/scpkit/src/validate.py` & `scpkit-0.1.2/scpkit/src/validate.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.1.1/setup.cfg` & `scpkit-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.1.1
+version = 0.1.2
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.1.1/tests/test.py` & `scpkit-0.1.2/tests/test.py`

 * *Files identical despite different names*

