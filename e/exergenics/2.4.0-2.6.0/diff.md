# Comparing `tmp/exergenics-2.4.0.tar.gz` & `tmp/exergenics-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-2.4.0.tar", last modified: Thu Apr  6 06:05:04 2023, max compression
+gzip compressed data, was "exergenics-2.6.0.tar", last modified: Wed Apr 26 01:25:10 2023, max compression
```

## Comparing `exergenics-2.4.0.tar` & `exergenics-2.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 06:05:04.551427 exergenics-2.4.0/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-06 06:05:04.551427 exergenics-2.4.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 06:05:04.551427 exergenics-2.4.0/exergenics/
--rw-rw-r--   0 root         (0) root         (0)       37 2023-04-06 06:03:46.000000 exergenics-2.4.0/exergenics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    59324 2023-04-06 06:03:46.000000 exergenics-2.4.0/exergenics/exergenics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 06:05:04.551427 exergenics-2.4.0/exergenics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-06 06:05:04.000000 exergenics-2.4.0/exergenics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-06 06:05:04.000000 exergenics-2.4.0/exergenics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 06:05:04.000000 exergenics-2.4.0/exergenics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-06 06:05:04.000000 exergenics-2.4.0/exergenics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-06 06:05:04.000000 exergenics-2.4.0/exergenics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 06:05:04.551427 exergenics-2.4.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      672 2023-04-06 06:05:02.000000 exergenics-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.543620 exergenics-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-26 01:25:10.543620 exergenics-2.6.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.539620 exergenics-2.6.0/exergenics/
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-04-26 01:23:52.000000 exergenics-2.6.0/exergenics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    59324 2023-04-26 01:23:52.000000 exergenics-2.6.0/exergenics/exergenics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.543620 exergenics-2.6.0/exergenics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 01:25:10.543620 exergenics-2.6.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      672 2023-04-26 01:25:08.000000 exergenics-2.6.0/setup.py
```

### Comparing `exergenics-2.4.0/exergenics/exergenics.py` & `exergenics-2.6.0/exergenics/exergenics.py`

 * *Files identical despite different names*

### Comparing `exergenics-2.4.0/setup.py` & `exergenics-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='exergenics',
-    version='2.4.0',
+    version='2.6.0',
     author="John Christian",
     author_email='john.christian@exergenics.com',
     packages=['exergenics'],
     long_description="",
     long_description_content_type="text/markdown",
     # package_dir={'': 'src'},
     url='https://github.com/Exergenics/internal-portal-api',
```

