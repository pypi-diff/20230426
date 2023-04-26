# Comparing `tmp/PyCHAS-1.0.0.tar.gz` & `tmp/PyCHAS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCHAS-1.0.0.tar", last modified: Tue Apr 25 16:12:08 2023, max compression
+gzip compressed data, was "PyCHAS-1.0.1.tar", last modified: Wed Apr 26 14:37:11 2023, max compression
```

## Comparing `PyCHAS-1.0.0.tar` & `PyCHAS-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PyCHAS/
--rw-r--r--   0 runner    (1001) docker     (123)    31662 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/PyCHAS/chas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PyCHAS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:37:11.898774 PyCHAS-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-26 14:37:11.898774 PyCHAS-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:37:11.898774 PyCHAS-1.0.1/PyCHAS/
+-rw-r--r--   0 runner    (1001) docker     (123)    31852 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/PyCHAS/pychas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:37:11.898774 PyCHAS-1.0.1/PyCHAS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-26 14:37:11.000000 PyCHAS-1.0.1/PyCHAS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 14:37:11.000000 PyCHAS-1.0.1/PyCHAS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:37:11.000000 PyCHAS-1.0.1/PyCHAS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 14:37:11.000000 PyCHAS-1.0.1/PyCHAS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 14:37:11.000000 PyCHAS-1.0.1/PyCHAS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-26 14:37:11.902774 PyCHAS-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-26 14:36:51.000000 PyCHAS-1.0.1/setup.py
```

### Comparing `PyCHAS-1.0.0/LICENSE` & `PyCHAS-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCHAS-1.0.0/PyCHAS/chas.py` & `PyCHAS-1.0.1/PyCHAS/pychas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-# Copyright goes here
+#
+# Copyright (c) 2023 Kara Wilson.
+#
+# This file is part of PyCHAS
+# (see https://github.com/EinKara/PyCHAS/).
+#
+# License: 3-clause BSD, see https://opensource.org/licenses/BSD-3-Clause#
 
-# Based off of Corrade ACME, however modified and maintained for modern C++
+# Based off of Corrade ACME. Modified and maintained for modern C++, with some extra features.
 
 import argparse
 import codecs
 import re
 import os
 import logging
 import subprocess
@@ -193,15 +199,15 @@
                 continue
 
             # Otherwise complain
             raise ValueError("First copyright found for {} is missing years {}, supply an explicit combined copyright instead".format(email, repr(years - email_dict[email][0])))
 
     return output
 
-def chas(toplevel_file, output) -> List[str]:
+def pychas(toplevel_file, output) -> List[str]:
     base_directory = os.path.dirname(toplevel_file)
 
     write_comments = True
     paths = []
     local_include_prefixes = []
     local_includes_noexpand = set()
     all_includes = set()
@@ -660,8 +666,8 @@
     if os.path.exists(output) and os.path.isdir(output):
         output = os.path.join(output, os.path.basename(args.file))
 
     # Otherwise assume it's a filename, create all directories above it if they
     # don't exist
     else: os.makedirs(os.path.dirname(output), exist_ok=True)
 
-    chas(args.file, output)
+    pychas(args.file, output)
```

