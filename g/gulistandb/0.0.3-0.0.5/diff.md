# Comparing `tmp/gulistandb-0.0.3.tar.gz` & `tmp/gulistandb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulistandb-0.0.3.tar", last modified: Mon Apr 24 14:48:50 2023, max compression
+gzip compressed data, was "gulistandb-0.0.5.tar", last modified: Wed Apr 26 14:08:26 2023, max compression
```

## Comparing `gulistandb-0.0.3.tar` & `gulistandb-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:48:50.165248 gulistandb-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.3/License
--rw-rw-rw-   0        0        0     2575 2023-04-24 14:48:50.162244 gulistandb-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3720 2023-04-24 14:43:20.000000 gulistandb-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 14:48:50.166247 gulistandb-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-04-24 14:46:55.000000 gulistandb-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:48:50.121268 gulistandb-0.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:48:50.157247 gulistandb-0.0.3/src/gulistandb.egg-info/
--rw-rw-rw-   0        0        0     2575 2023-04-24 14:48:49.000000 gulistandb-0.0.3/src/gulistandb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-24 14:48:49.000000 gulistandb-0.0.3/src/gulistandb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:48:49.000000 gulistandb-0.0.3/src/gulistandb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 14:48:49.000000 gulistandb-0.0.3/src/gulistandb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-24 14:48:49.000000 gulistandb-0.0.3/src/gulistandb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4089 2023-04-24 06:51:18.000000 gulistandb-0.0.3/src/gulistandb.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.559048 gulistandb-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.5/License
+-rw-rw-rw-   0        0        0     2760 2023-04-26 14:08:26.556040 gulistandb-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4086 2023-04-26 13:39:56.000000 gulistandb-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:08:26.561036 gulistandb-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-04-26 14:00:02.000000 gulistandb-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.509067 gulistandb-0.0.5/src/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.5/src/__init__.py
+-rw-rw-rw-   0        0        0     1065 2023-04-26 11:40:19.000000 gulistandb-0.0.5/src/editor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:08:26.551041 gulistandb-0.0.5/src/gulistandb.egg-info/
+-rw-rw-rw-   0        0        0     2760 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:08:26.000000 gulistandb-0.0.5/src/gulistandb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6013 2023-04-26 13:13:08.000000 gulistandb-0.0.5/src/gulistandb.py
+-rw-rw-rw-   0        0        0     1361 2023-04-26 11:39:19.000000 gulistandb-0.0.5/src/reader.py
+-rw-rw-rw-   0        0        0     1750 2023-04-26 11:37:12.000000 gulistandb-0.0.5/src/writter.py
```

### Comparing `gulistandb-0.0.3/License` & `gulistandb-0.0.5/License`

 * *Files identical despite different names*

### Comparing `gulistandb-0.0.3/setup.py` & `gulistandb-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-16') as f:
     long_description = f.read()
 
 setup(
     name='gulistandb',
-    version='0.0.3',
+    version='0.0.5',
     install_requires=[
         'pandas',
         # add more dependencies as needed
     ],
     package_dir={'': 'src'},
 
     # metadata
```

