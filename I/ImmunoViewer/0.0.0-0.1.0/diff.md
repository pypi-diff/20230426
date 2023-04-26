# Comparing `tmp/ImmunoViewer-0.0.0.tar.gz` & `tmp/ImmunoViewer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImmunoViewer-0.0.0.tar", last modified: Wed Apr 26 21:00:39 2023, max compression
+gzip compressed data, was "ImmunoViewer-0.1.0.tar", last modified: Wed Apr 26 21:07:06 2023, max compression
```

## Comparing `ImmunoViewer-0.0.0.tar` & `ImmunoViewer-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:00:39.910942 ImmunoViewer-0.0.0/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1077 2023-04-26 17:09:31.000000 ImmunoViewer-0.0.0/LICENSE
--rw-r--r--   0 vanijzen   (503) staff       (20)     2238 2023-04-26 21:00:39.910690 ImmunoViewer-0.0.0/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)      840 2023-04-26 20:45:59.000000 ImmunoViewer-0.0.0/README.md
--rw-r--r--   0 vanijzen   (503) staff       (20)       38 2023-04-26 21:00:39.910993 ImmunoViewer-0.0.0/setup.cfg
--rw-r--r--   0 vanijzen   (503) staff       (20)     2146 2023-04-26 18:55:10.000000 ImmunoViewer-0.0.0/setup.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:00:39.902868 ImmunoViewer-0.0.0/src/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:00:39.905790 ImmunoViewer-0.0.0/src/ImmunoViewer/
--rw-r--r--   0 vanijzen   (503) staff       (20)       21 2023-04-26 17:12:12.000000 ImmunoViewer-0.0.0/src/ImmunoViewer/__init__.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     1975 2023-04-26 18:54:59.000000 ImmunoViewer-0.0.0/src/ImmunoViewer/process_folder.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     5761 2023-04-26 18:55:18.000000 ImmunoViewer-0.0.0/src/ImmunoViewer/server.py
--rwxr-xr-x   0 vanijzen   (503) staff       (20)     9247 2023-04-26 18:55:06.000000 ImmunoViewer-0.0.0/src/ImmunoViewer/tile.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:00:39.909326 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/
--rw-r--r--   0 vanijzen   (503) staff       (20)     2238 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)      384 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/SOURCES.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)        1 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/dependency_links.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/entry_points.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      126 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/requires.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)       13 2023-04-26 21:00:39.000000 ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/top_level.txt
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.456934 ImmunoViewer-0.1.0/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1077 2023-04-26 17:09:31.000000 ImmunoViewer-0.1.0/LICENSE
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:07:06.456684 ImmunoViewer-0.1.0/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)      840 2023-04-26 21:02:31.000000 ImmunoViewer-0.1.0/README.md
+-rw-r--r--   0 vanijzen   (503) staff       (20)       38 2023-04-26 21:07:06.456989 ImmunoViewer-0.1.0/setup.cfg
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2023-04-26 21:06:55.000000 ImmunoViewer-0.1.0/setup.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.447994 ImmunoViewer-0.1.0/src/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.452170 ImmunoViewer-0.1.0/src/ImmunoViewer/
+-rw-r--r--   0 vanijzen   (503) staff       (20)       21 2023-04-26 17:12:12.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/__init__.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1975 2023-04-26 18:54:59.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/process_folder.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5761 2023-04-26 18:55:18.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/server.py
+-rwxr-xr-x   0 vanijzen   (503) staff       (20)     9247 2023-04-26 18:55:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/tile.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.456360 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)      384 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)        1 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/entry_points.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      126 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/requires.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)       13 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/top_level.txt
```

### Comparing `ImmunoViewer-0.0.0/LICENSE` & `ImmunoViewer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.0.0/PKG-INFO` & `ImmunoViewer-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.0.0
+Version: 0.1.0
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
-Home-page: https://github.com/tomchen/example_pypi_package
+Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
 Keywords: big tif,immuno,viewer,annotate,annotation,discover,discovery,image,images,tif,tiff,multi-channel,multi c
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ImmunoViewer-0.0.0/README.md` & `ImmunoViewer-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.0.0/setup.py` & `ImmunoViewer-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
+    version='0.1.0',
     name='ImmunoViewer',
     author='David van IJzendoorn',
     author_email='davidvanijzendoorn@gmail.com',
     description='Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer',
     keywords='big tif, immuno, viewer, annotate, annotation, discover, discovery, image, images, tif, tiff, multi-channel, multi c',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/tomchen/example_pypi_package',
+    url='https://github.com/davidvi/ImmunoViewer',
     project_urls={
         'Documentation': 'https://github.com/davidvi/ImmunoViewer',
         'Bug Reports':
         'https://github.com/davidvi/ImmunoViewer/issues',
         'Source Code': 'https://github.com/davidvi/ImmunoViewer'
     },
     package_dir={'': 'src'},
```

### Comparing `ImmunoViewer-0.0.0/src/ImmunoViewer/process_folder.py` & `ImmunoViewer-0.1.0/src/ImmunoViewer/process_folder.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.0.0/src/ImmunoViewer/server.py` & `ImmunoViewer-0.1.0/src/ImmunoViewer/server.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.0.0/src/ImmunoViewer/tile.py` & `ImmunoViewer-0.1.0/src/ImmunoViewer/tile.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.0.0/src/ImmunoViewer.egg-info/PKG-INFO` & `ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.0.0
+Version: 0.1.0
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
-Home-page: https://github.com/tomchen/example_pypi_package
+Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
 Keywords: big tif,immuno,viewer,annotate,annotation,discover,discovery,image,images,tif,tiff,multi-channel,multi c
 Classifier: Development Status :: 5 - Production/Stable
```

