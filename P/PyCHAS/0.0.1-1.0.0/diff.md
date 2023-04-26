# Comparing `tmp/PyCHAS-0.0.1.tar.gz` & `tmp/PyCHAS-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCHAS-0.0.1.tar", last modified: Mon Apr 24 16:52:54 2023, max compression
+gzip compressed data, was "PyCHAS-1.0.0.tar", last modified: Tue Apr 25 16:12:08 2023, max compression
```

## Comparing `PyCHAS-0.0.1.tar` & `PyCHAS-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:52:54.108677 PyCHAS-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 16:52:54.108677 PyCHAS-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:52:54.108677 PyCHAS-0.0.1/PyCHAS/
--rw-r--r--   0 runner    (1001) docker     (123)    31626 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/PyCHAS/chas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:52:54.108677 PyCHAS-0.0.1/PyCHAS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 16:52:54.000000 PyCHAS-0.0.1/PyCHAS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 16:52:54.000000 PyCHAS-0.0.1/PyCHAS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:52:54.000000 PyCHAS-0.0.1/PyCHAS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 16:52:54.000000 PyCHAS-0.0.1/PyCHAS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:52:54.000000 PyCHAS-0.0.1/PyCHAS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-24 16:52:54.108677 PyCHAS-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-24 16:52:42.000000 PyCHAS-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PyCHAS/
+-rw-r--r--   0 runner    (1001) docker     (123)    31662 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/PyCHAS/chas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/PyCHAS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 16:12:08.000000 PyCHAS-1.0.0/PyCHAS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 16:12:08.392333 PyCHAS-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 16:11:57.000000 PyCHAS-1.0.0/setup.py
```

### Comparing `PyCHAS-0.0.1/LICENSE` & `PyCHAS-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCHAS-0.0.1/PyCHAS/chas.py` & `PyCHAS-1.0.0/PyCHAS/chas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright goes here
 
+# Based off of Corrade ACME, however modified and maintained for modern C++
+
 import argparse
 import codecs
 import re
 import os
 import logging
 import subprocess
 
@@ -634,15 +636,15 @@
             lines[i] = line.replace(placeholder, stats)
 
     logging.info('Writing %i lines to %s', len(lines), output)
     with open(output, 'w') as of:
         for line in lines:
             of.write(line)
 
-def entry():
+def main():
     parser = argparse.ArgumentParser(
         description=r"""Creates single-header libraries from given top-level input file.""",
         epilog="""If output exists and is a directory, the file is saved inside with the same name as the input.""")
     parser.add_argument('file', help='top-level file')
     parser.add_argument('-o', '--output', help="output file or directory", default='output')
     parser.add_argument('--debug', help="verbose debug output", action='store_true')
     args = parser.parse_args()
@@ -659,10 +661,7 @@
         output = os.path.join(output, os.path.basename(args.file))
 
     # Otherwise assume it's a filename, create all directories above it if they
     # don't exist
     else: os.makedirs(os.path.dirname(output), exist_ok=True)
 
     chas(args.file, output)
-
-if __name__ == '__main__':
-    entry()
```

