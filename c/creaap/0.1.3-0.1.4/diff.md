# Comparing `tmp/creaap-0.1.3.tar.gz` & `tmp/creaap-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creaap-0.1.3.tar", last modified: Fri Nov 25 08:03:32 2022, max compression
+gzip compressed data, was "creaap-0.1.4.tar", last modified: Wed Apr 26 12:30:20 2023, max compression
```

## Comparing `creaap-0.1.3.tar` & `creaap-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.816122 creaap-0.1.3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1051 2022-11-25 08:02:40.000000 creaap-0.1.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       39 2022-11-25 08:02:40.000000 creaap-0.1.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    11746 2022-11-25 08:03:32.816122 creaap-0.1.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11047 2022-11-25 08:02:40.000000 creaap-0.1.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.808122 creaap-0.1.3/creaap/
--rw-r--r--   0 vsts      (1001) docker     (122)      145 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3797 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/formats.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1690 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/io.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5784 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.812122 creaap-0.1.3/creaap/spatial/
--rw-r--r--   0 vsts      (1001) docker     (122)      271 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.812122 creaap-0.1.3/creaap/spatial/data/
--rw-r--r--   0 vsts      (1001) docker     (122)    49041 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/data/nuts0
--rw-r--r--   0 vsts      (1001) docker     (122)    80472 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/data/nuts1
--rw-r--r--   0 vsts      (1001) docker     (122)   126320 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/data/nuts2
--rw-r--r--   0 vsts      (1001) docker     (122)   288809 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/data/nuts3
--rw-r--r--   0 vsts      (1001) docker     (122)    10355 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/match.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7559 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/spatial/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.816122 creaap-0.1.3/creaap/storage/
--rw-r--r--   0 vsts      (1001) docker     (122)      197 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8234 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/storage/blob.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6705 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/storage/file.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9152 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/storage/table.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.816122 creaap-0.1.3/creaap/users/
--rw-r--r--   0 vsts      (1001) docker     (122)      281 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9799 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/users/aad.py
--rw-r--r--   0 vsts      (1001) docker     (122)      743 2022-11-25 08:02:40.000000 creaap-0.1.3/creaap/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-25 08:03:32.812122 creaap-0.1.3/creaap.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    11746 2022-11-25 08:03:32.000000 creaap-0.1.3/creaap.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      591 2022-11-25 08:03:32.000000 creaap-0.1.3/creaap.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-25 08:03:32.000000 creaap-0.1.3/creaap.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      146 2022-11-25 08:03:32.000000 creaap-0.1.3/creaap.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2022-11-25 08:03:32.000000 creaap-0.1.3/creaap.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-25 08:03:32.816122 creaap-0.1.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1476 2022-11-25 08:02:40.000000 creaap-0.1.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1051 2023-04-26 12:29:40.000000 creaap-0.1.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       39 2023-04-26 12:29:40.000000 creaap-0.1.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)    11746 2023-04-26 12:30:20.087722 creaap-0.1.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11047 2023-04-26 12:29:40.000000 creaap-0.1.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap/
+-rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3797 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/formats.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1690 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/io.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5784 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap/spatial/
+-rw-r--r--   0 vsts      (1001) docker     (123)      271 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/spatial/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    49041 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts0
+-rw-r--r--   0 vsts      (1001) docker     (123)    80472 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts1
+-rw-r--r--   0 vsts      (1001) docker     (123)   126320 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts2
+-rw-r--r--   0 vsts      (1001) docker     (123)   288809 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/data/nuts3
+-rw-r--r--   0 vsts      (1001) docker     (123)    10355 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7559 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/spatial/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/storage/
+-rw-r--r--   0 vsts      (1001) docker     (123)      197 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8318 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/blob.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6705 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9152 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/storage/table.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.087722 creaap-0.1.4/creaap/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9799 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/users/aad.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      743 2023-04-26 12:29:40.000000 creaap-0.1.4/creaap/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-26 12:30:20.083722 creaap-0.1.4/creaap.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11746 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      146 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        7 2023-04-26 12:30:20.000000 creaap-0.1.4/creaap.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-26 12:30:20.087722 creaap-0.1.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-04-26 12:29:40.000000 creaap-0.1.4/setup.py
```

### Comparing `creaap-0.1.3/LICENSE` & `creaap-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/PKG-INFO` & `creaap-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.3
+Version: 0.1.4
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `creaap-0.1.3/README.md` & `creaap-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/formats.py` & `creaap-0.1.4/creaap/formats.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/io.py` & `creaap-0.1.4/creaap/io.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/models.py` & `creaap-0.1.4/creaap/models.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/data/nuts0` & `creaap-0.1.4/creaap/spatial/data/nuts0`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/data/nuts1` & `creaap-0.1.4/creaap/spatial/data/nuts1`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/data/nuts2` & `creaap-0.1.4/creaap/spatial/data/nuts2`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/data/nuts3` & `creaap-0.1.4/creaap/spatial/data/nuts3`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/match.py` & `creaap-0.1.4/creaap/spatial/match.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/spatial/utils.py` & `creaap-0.1.4/creaap/spatial/utils.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/storage/blob.py` & `creaap-0.1.4/creaap/storage/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         dest: string
             blob path for the uploaded file
 
         Returns
         -------
         None
         '''
-        self.client.upload_blob(name=dest, data=data)
+        self.client.upload_blob(name=dest, data=data, overwrite=True)
 
     def upload_dir(self, source, dest):
         '''
         Upload a directory to a path inside the container
 
         Parameters
         ----------
@@ -209,17 +209,17 @@
             strings that represent items in the container
         '''
         if not path == '' and not path.endswith('/'):
             path += '/'
 
         blob_iter = self.client.list_blobs(name_starts_with=path)
         for blob in blob_iter:
-            relative_path = os.path.relpath(blob.name, path)
+            relative_path = blob.name.lstrip(path)
             if recursive or not '/' in relative_path:
-                yield relative_path
+                yield blob.name
 
     def ls_dirs(self, path, recursive=False):
         '''
         List directories under a path, optionally recursively.
         Mind that in Azure Blob Storage directories are not "real" directories
         like in a file system, but rather prefeixes you use to better organize
         your blobs.
@@ -238,19 +238,21 @@
             strings that represent "directories" in the container
         -------
         '''
         if not path == '' and not path.endswith('/'):
             path += '/'
 
         blob_iter = self.client.list_blobs(name_starts_with=path)
-        dirs = []
+        dirs = set()
         for blob in blob_iter:
-            relative_dir = os.path.dirname(os.path.relpath(blob.name, path))
+            # here we just have to strip the filename
+            relative_dir = '/'.join(blob.name.split('/')[:-1])
             if relative_dir and (recursive or not '/' in relative_dir) and not relative_dir in dirs:
                 yield relative_dir
+                dirs.add(relative_dir)
     
     def delete_file(self,path):
         '''
         Delete a single file inside the container
 
         Parameters
         ----------
```

### Comparing `creaap-0.1.3/creaap/storage/file.py` & `creaap-0.1.4/creaap/storage/file.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/storage/table.py` & `creaap-0.1.4/creaap/storage/table.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/users/aad.py` & `creaap-0.1.4/creaap/users/aad.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap/utils.py` & `creaap-0.1.4/creaap/utils.py`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/creaap.egg-info/PKG-INFO` & `creaap-0.1.4/creaap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creaap
-Version: 0.1.3
+Version: 0.1.4
 Summary: CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.
 Home-page: https://dev.azure.com/dariodenart/_git/CREA%20Application%20Python%20toolkit
 Author: CREA
 Author-email: dario.denart@crea.gov.it
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `creaap-0.1.3/creaap.egg-info/SOURCES.txt` & `creaap-0.1.4/creaap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creaap-0.1.3/setup.py` & `creaap-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
    name='creaap',
-   version='0.1.3',
+   version='0.1.4',
    description='CREA Applications in Python toolkit. A bundle of tools to speed up the deelopment of new Python applications in Azure. Allows you to abstract a little over persistence and to manage spatial data.',
    author='CREA',
    author_email='dario.denart@crea.gov.it',
    packages=['creaap', 'creaap.spatial', 'creaap.storage', 'creaap.users'],
    classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

