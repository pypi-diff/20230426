# Comparing `tmp/ImmunoViewer-0.1.0.tar.gz` & `tmp/ImmunoViewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImmunoViewer-0.1.0.tar", last modified: Wed Apr 26 21:07:06 2023, max compression
+gzip compressed data, was "ImmunoViewer-0.1.1.tar", last modified: Wed Apr 26 21:23:36 2023, max compression
```

## Comparing `ImmunoViewer-0.1.0.tar` & `ImmunoViewer-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.456934 ImmunoViewer-0.1.0/
--rw-r--r--   0 vanijzen   (503) staff       (20)     1077 2023-04-26 17:09:31.000000 ImmunoViewer-0.1.0/LICENSE
--rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:07:06.456684 ImmunoViewer-0.1.0/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)      840 2023-04-26 21:02:31.000000 ImmunoViewer-0.1.0/README.md
--rw-r--r--   0 vanijzen   (503) staff       (20)       38 2023-04-26 21:07:06.456989 ImmunoViewer-0.1.0/setup.cfg
--rw-r--r--   0 vanijzen   (503) staff       (20)     2159 2023-04-26 21:06:55.000000 ImmunoViewer-0.1.0/setup.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.447994 ImmunoViewer-0.1.0/src/
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.452170 ImmunoViewer-0.1.0/src/ImmunoViewer/
--rw-r--r--   0 vanijzen   (503) staff       (20)       21 2023-04-26 17:12:12.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/__init__.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     1975 2023-04-26 18:54:59.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/process_folder.py
--rw-r--r--   0 vanijzen   (503) staff       (20)     5761 2023-04-26 18:55:18.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/server.py
--rwxr-xr-x   0 vanijzen   (503) staff       (20)     9247 2023-04-26 18:55:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer/tile.py
-drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:07:06.456360 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/
--rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/PKG-INFO
--rw-r--r--   0 vanijzen   (503) staff       (20)      384 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/SOURCES.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)        1 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/dependency_links.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/entry_points.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)      126 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/requires.txt
--rw-r--r--   0 vanijzen   (503) staff       (20)       13 2023-04-26 21:07:06.000000 ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/top_level.txt
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:23:36.653352 ImmunoViewer-0.1.1/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1077 2023-04-26 17:09:31.000000 ImmunoViewer-0.1.1/LICENSE
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:23:36.652706 ImmunoViewer-0.1.1/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)      840 2023-04-26 21:02:31.000000 ImmunoViewer-0.1.1/README.md
+-rw-r--r--   0 vanijzen   (503) staff       (20)       38 2023-04-26 21:23:36.653401 ImmunoViewer-0.1.1/setup.cfg
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2213 2023-04-26 21:21:19.000000 ImmunoViewer-0.1.1/setup.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:23:36.644437 ImmunoViewer-0.1.1/src/
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:23:36.647850 ImmunoViewer-0.1.1/src/ImmunoViewer/
+-rw-r--r--   0 vanijzen   (503) staff       (20)       21 2023-04-26 17:12:12.000000 ImmunoViewer-0.1.1/src/ImmunoViewer/__init__.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     1975 2023-04-26 18:54:59.000000 ImmunoViewer-0.1.1/src/ImmunoViewer/process_folder.py
+-rw-r--r--   0 vanijzen   (503) staff       (20)     5751 2023-04-26 21:23:07.000000 ImmunoViewer-0.1.1/src/ImmunoViewer/server.py
+-rwxr-xr-x   0 vanijzen   (503) staff       (20)     9247 2023-04-26 18:55:06.000000 ImmunoViewer-0.1.1/src/ImmunoViewer/tile.py
+drwxr-xr-x   0 vanijzen   (503) staff       (20)        0 2023-04-26 21:23:36.652257 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/
+-rw-r--r--   0 vanijzen   (503) staff       (20)     2230 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/PKG-INFO
+-rw-r--r--   0 vanijzen   (503) staff       (20)      384 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)        1 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      119 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/entry_points.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)      126 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/requires.txt
+-rw-r--r--   0 vanijzen   (503) staff       (20)       13 2023-04-26 21:23:36.000000 ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/top_level.txt
```

### Comparing `ImmunoViewer-0.1.0/LICENSE` & `ImmunoViewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.0/PKG-INFO` & `ImmunoViewer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
 Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
```

### Comparing `ImmunoViewer-0.1.0/README.md` & `ImmunoViewer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.0/setup.py` & `ImmunoViewer-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    version='0.1.0',
+    version='0.1.1',
     name='ImmunoViewer',
     author='David van IJzendoorn',
     author_email='davidvanijzendoorn@gmail.com',
     description='Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer',
     keywords='big tif, immuno, viewer, annotate, annotation, discover, discovery, image, images, tif, tiff, multi-channel, multi c',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -16,14 +16,17 @@
     project_urls={
         'Documentation': 'https://github.com/davidvi/ImmunoViewer',
         'Bug Reports':
         'https://github.com/davidvi/ImmunoViewer/issues',
         'Source Code': 'https://github.com/davidvi/ImmunoViewer'
     },
     package_dir={'': 'src'},
+    package_data={
+        'client': ['*']
+        },
     packages=setuptools.find_packages(where='src'),
     classifiers=[
         # see https://pypi.org/classifiers/
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
```

### Comparing `ImmunoViewer-0.1.0/src/ImmunoViewer/process_folder.py` & `ImmunoViewer-0.1.1/src/ImmunoViewer/process_folder.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.0/src/ImmunoViewer/server.py` & `ImmunoViewer-0.1.1/src/ImmunoViewer/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 
 
 @app.route('/', defaults={'path': ''})
 @app.route('/<path:path>')
 @cross_origin()
 def index(path):
     if path and (path.startswith('assets') or path.startswith('favicon') or path.startswith('images')):
-        return send_from_directory(os.path.abspath("client/dist"), path)
+        return send_from_directory(os.path.abspath("client"), path)
     else:
-        return send_from_directory(os.path.abspath("client/dist"), 'index.html')
+        return send_from_directory(os.path.abspath("client"), 'index.html')
 
 @app.route('/samples.json')
 @cross_origin()
 def samples():
     file_json = find_directories_with_files_folders(os.path.abspath(app.config['SLIDE_DIR']))
 
     buf = {}
```

### Comparing `ImmunoViewer-0.1.0/src/ImmunoViewer/tile.py` & `ImmunoViewer-0.1.1/src/ImmunoViewer/tile.py`

 * *Files identical despite different names*

### Comparing `ImmunoViewer-0.1.0/src/ImmunoViewer.egg-info/PKG-INFO` & `ImmunoViewer-0.1.1/src/ImmunoViewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImmunoViewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discover and annotate your (multi-channel) big TIF files with this user-friendly viewer
 Home-page: https://github.com/davidvi/ImmunoViewer
 Author: David van IJzendoorn
 Author-email: davidvanijzendoorn@gmail.com
 Project-URL: Documentation, https://github.com/davidvi/ImmunoViewer
 Project-URL: Bug Reports, https://github.com/davidvi/ImmunoViewer/issues
 Project-URL: Source Code, https://github.com/davidvi/ImmunoViewer
```

