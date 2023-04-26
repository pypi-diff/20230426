# Comparing `tmp/ProteoformQuant-0.52.tar.gz` & `tmp/ProteoformQuant-0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProteoformQuant-0.52.tar", last modified: Wed Apr 26 15:27:45 2023, max compression
+gzip compressed data, was "ProteoformQuant-0.53.tar", last modified: Wed Apr 26 15:27:54 2023, max compression
```

## Comparing `ProteoformQuant-0.52.tar` & `ProteoformQuant-0.53.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-04-26 15:27:45.436491 ProteoformQuant-0.52/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2023-03-17 14:28:03.000000 ProteoformQuant-0.52/MANIFEST.in
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1692 2023-04-26 15:27:45.436491 ProteoformQuant-0.52/PKG-INFO
-drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-04-26 15:27:45.436491 ProteoformQuant-0.52/ProteoformQuant.egg-info/
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1692 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/PKG-INFO
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/SOURCES.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/dependency_links.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/entry_points.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/requires.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2023-04-26 15:27:45.000000 ProteoformQuant-0.52/ProteoformQuant.egg-info/top_level.txt
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2023-04-26 15:27:45.436491 ProteoformQuant-0.52/setup.cfg
--rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2023-03-20 10:27:03.000000 ProteoformQuant-0.52/setup.py
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-04-26 15:27:54.420430 ProteoformQuant-0.53/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        0 2023-03-17 14:28:03.000000 ProteoformQuant-0.53/MANIFEST.in
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1692 2023-04-26 15:27:54.420430 ProteoformQuant-0.53/PKG-INFO
+drwxrwxr-x   0 agrimaud (332419330) agrimaud (332419330)        0 2023-04-26 15:27:54.420430 ProteoformQuant-0.53/ProteoformQuant.egg-info/
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1692 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/PKG-INFO
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     1070 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/SOURCES.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)        1 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/dependency_links.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       57 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/entry_points.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)      349 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/requires.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       16 2023-04-26 15:27:54.000000 ProteoformQuant-0.53/ProteoformQuant.egg-info/top_level.txt
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)       38 2023-04-26 15:27:54.420430 ProteoformQuant-0.53/setup.cfg
+-rw-rw-r--   0 agrimaud (332419330) agrimaud (332419330)     3372 2023-03-20 10:27:03.000000 ProteoformQuant-0.53/setup.py
```

### Comparing `ProteoformQuant-0.52/PKG-INFO` & `ProteoformQuant-0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProteoformQuant
-Version: 0.52
+Version: 0.53
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: 
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `ProteoformQuant-0.52/ProteoformQuant.egg-info/PKG-INFO` & `ProteoformQuant-0.53/ProteoformQuant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProteoformQuant
-Version: 0.52
+Version: 0.53
 Summary: A python command line tool for the quantification of peptidoform/proteoforms
 Home-page: 
 Author: Arthur Grimaud
 Author-email: 
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `ProteoformQuant-0.52/ProteoformQuant.egg-info/SOURCES.txt` & `ProteoformQuant-0.53/ProteoformQuant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProteoformQuant-0.52/setup.py` & `ProteoformQuant-0.53/setup.py`

 * *Files identical despite different names*

