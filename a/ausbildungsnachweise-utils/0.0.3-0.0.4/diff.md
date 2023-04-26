# Comparing `tmp/ausbildungsnachweise_utils-0.0.3.tar.gz` & `tmp/ausbildungsnachweise_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ausbildungsnachweise_utils-0.0.3.tar", last modified: Fri Apr 14 06:12:28 2023, max compression
+gzip compressed data, was "ausbildungsnachweise_utils-0.0.4.tar", last modified: Wed Apr 26 10:36:57 2023, max compression
```

## Comparing `ausbildungsnachweise_utils-0.0.3.tar` & `ausbildungsnachweise_utils-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-14 06:12:28.128364 ausbildungsnachweise_utils-0.0.3/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      400 2023-04-14 06:12:28.128364 ausbildungsnachweise_utils-0.0.3/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       28 2023-04-14 05:04:10.000000 ausbildungsnachweise_utils-0.0.3/README.md
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-14 06:12:28.128364 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)        0 2023-04-12 08:24:39.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/__init__.py
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       90 2023-04-14 05:13:06.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/__main__.py
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     3085 2023-04-12 09:28:07.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/processor.py
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       54 2023-04-14 06:01:02.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/starter.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-14 06:12:28.128364 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      400 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      476 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)        1 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       87 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/entry_points.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       20 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/requires.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       27 2023-04-14 06:12:28.000000 ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils.egg-info/top_level.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       38 2023-04-14 06:12:28.128364 ausbildungsnachweise_utils-0.0.3/setup.cfg
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      889 2023-04-14 06:08:43.000000 ausbildungsnachweise_utils-0.0.3/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 10:36:57.906361 ausbildungsnachweise_utils-0.0.4/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-04-26 10:36:57.906361 ausbildungsnachweise_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.4/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 10:36:57.906361 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3085 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/processor.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      995 2023-04-24 13:40:47.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/starter.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-26 10:36:57.906361 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-04-26 10:36:57.000000 ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-04-26 10:36:57.906361 ausbildungsnachweise_utils-0.0.4/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.4/setup.py
```

### Comparing `ausbildungsnachweise_utils-0.0.3/ausbildungsnachweise_utils/processor.py` & `ausbildungsnachweise_utils-0.0.4/ausbildungsnachweise_utils/processor.py`

 * *Files identical despite different names*

### Comparing `ausbildungsnachweise_utils-0.0.3/setup.py` & `ausbildungsnachweise_utils-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     long_description=read('README.md'),
     install_requires=[
         "PyMuPDF",
         "python-docx"
     ],
     entry_points={
         'console_scripts': [
-            'ausbildungsnachweis_utils = ausbildungsnachweis_utils.starter:start',
+            'ausbildungsnachweise_utils = ausbildungsnachweise_utils.starter:start',
         ]
     }
 )
```

