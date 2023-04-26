# Comparing `tmp/aquasec-cli-0.0.3.tar.gz` & `tmp/aquasec-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aquasec-cli-0.0.3.tar", last modified: Tue Apr 25 18:54:14 2023, max compression
+gzip compressed data, was "aquasec-cli-0.0.4.tar", last modified: Tue Apr 25 19:24:47 2023, max compression
```

## Comparing `aquasec-cli-0.0.3.tar` & `aquasec-cli-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:54:14.843088 aquasec-cli-0.0.3/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/LICENSE
--rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/MANIFEST.in
--rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 18:54:14.843408 aquasec-cli-0.0.3/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     2153 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/README.md
--rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/README.rst
--rw-rw-r--   0 adamt      (501) staff       (20)      520 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/SECURITY.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:54:14.839039 aquasec-cli-0.0.3/aquasec_cli/
--rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/_version.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:54:14.842806 aquasec-cli-0.0.3/aquasec_cli/commands/
--rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/commands/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1530 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/commands/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     1916 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/commands/report.py
--rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/main.py
--rw-rw-r--   0 adamt      (501) staff       (20)      570 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/aquasec_cli/utils.py
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 18:54:14.841738 aquasec-cli-0.0.3/aquasec_cli.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      526 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       53 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/entry_points.txt
--rw-r--r--   0 adamt      (501) staff       (20)      107 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/top_level.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 18:54:14.000000 aquasec-cli-0.0.3/aquasec_cli.egg-info/zip-safe
--rw-rw-r--   0 adamt      (501) staff       (20)      931 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/pyproject.toml
--rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/requirements.txt
--rw-rw-r--   0 adamt      (501) staff       (20)      725 2023-04-25 18:54:14.844257 aquasec-cli-0.0.3/setup.cfg
--rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-04-25 18:53:27.000000 aquasec-cli-0.0.3/setup.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.673781 aquasec-cli-0.0.4/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/LICENSE
+-rw-rw-r--   0 adamt      (501) staff       (20)       97 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/MANIFEST.in
+-rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 19:24:47.674174 aquasec-cli-0.0.4/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)     2211 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/README.md
+-rw-rw-r--   0 adamt      (501) staff       (20)     2667 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/README.rst
+-rw-rw-r--   0 adamt      (501) staff       (20)      520 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/SECURITY.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.667005 aquasec-cli-0.0.4/aquasec_cli/
+-rw-rw-r--   0 adamt      (501) staff       (20)       60 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/_version.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.673238 aquasec-cli-0.0.4/aquasec_cli/commands/
+-rw-rw-r--   0 adamt      (501) staff       (20)        0 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1530 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1916 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/commands/report.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      290 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/main.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      570 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/aquasec_cli/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-04-25 19:24:47.671271 aquasec-cli-0.0.4/aquasec_cli.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    44107 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      526 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       53 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/entry_points.txt
+-rw-r--r--   0 adamt      (501) staff       (20)      107 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-04-25 19:24:47.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/top_level.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-04-25 19:24:41.000000 aquasec-cli-0.0.4/aquasec_cli.egg-info/zip-safe
+-rw-rw-r--   0 adamt      (501) staff       (20)      931 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       61 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/requirements.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)      725 2023-04-25 19:24:47.675164 aquasec-cli-0.0.4/setup.cfg
+-rw-rw-r--   0 adamt      (501) staff       (20)      111 2023-04-25 19:23:15.000000 aquasec-cli-0.0.4/setup.py
```

### Comparing `aquasec-cli-0.0.3/LICENSE` & `aquasec-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/PKG-INFO` & `aquasec-cli-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `aquasec-cli-0.0.3/README.md` & `aquasec-cli-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 >>> aquasec-cli delete                                              
 Are you sure you want to delete the auth api token? [y/N]: y
 Deleted Auth
 ```
 
 ## Release Info
 
+### v0.0.4
+
+* fixed issue with broken aquasec-api v0.0.3
+
 ### v0.0.3
 
 * Fixed installation and dependencies
 * locked down dependencies
 * added toml and setup.cfg to support furture installations
 
 ### v0.0.2
```

### Comparing `aquasec-cli-0.0.3/README.rst` & `aquasec-cli-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/SECURITY.md` & `aquasec-cli-0.0.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/aquasec_cli/commands/api.py` & `aquasec-cli-0.0.4/aquasec_cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/aquasec_cli/commands/report.py` & `aquasec-cli-0.0.4/aquasec_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/aquasec_cli/utils.py` & `aquasec-cli-0.0.4/aquasec_cli/utils.py`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/aquasec_cli.egg-info/PKG-INFO` & `aquasec-cli-0.0.4/aquasec_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquasec-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Aqua Security cli
 Author: atav928
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `aquasec-cli-0.0.3/aquasec_cli.egg-info/SOURCES.txt` & `aquasec-cli-0.0.4/aquasec_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquasec-cli-0.0.3/pyproject.toml` & `aquasec-cli-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requires-python = ">=3.8"
 keywords = ['aquasec', 'aqua security', 'workload protection']
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "aquasec-api==0.0.3",
+    "aquasec-api==0.0.2",
     "click>=8.1.3",
     "dataclasses>=0.6",
     "PyYAML>=6.0",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version", "readme", "entry-points"]
```

### Comparing `aquasec-cli-0.0.3/setup.cfg` & `aquasec-cli-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 license = GNU
 
 [options]
 python_requires = >3.8, <4
 include_package_data = True
 packages = find:
 install_requires = 
-	aquasec-api == 0.0.3
+	aquasec-api == 0.0.2
 	click >= 8.1.3
 	dataclasses >= 0.6
 	PyYAML >= 6.0
 zip_safe = True
 
 [options.packages.find]
 include = aquasec_cli*
```

