# Comparing `tmp/TremendousClient-0.0.2.tar.gz` & `tmp/TremendousClient-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TremendousClient-0.0.2.tar", last modified: Wed Apr 26 19:00:03 2023, max compression
+gzip compressed data, was "TremendousClient-0.0.3.tar", last modified: Wed Apr 26 19:04:13 2023, max compression
```

## Comparing `TremendousClient-0.0.2.tar` & `TremendousClient-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.752019 TremendousClient-0.0.2/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.2/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:00:03.751896 TremendousClient-0.0.2/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1248 2023-04-26 18:59:45.000000 TremendousClient-0.0.2/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.750900 TremendousClient-0.0.2/TremendousClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      297 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-26 19:00:03.752057 TremendousClient-0.0.2/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      849 2023-04-26 18:59:54.000000 TremendousClient-0.0.2/setup.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.751582 TremendousClient-0.0.2/tremendous/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      108 2023-04-26 18:53:27.000000 TremendousClient-0.0.2/tremendous/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      292 2023-04-26 18:43:52.000000 TremendousClient-0.0.2/tremendous/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.2/tremendous/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:04:13.397987 TremendousClient-0.0.3/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.3/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:04:13.397787 TremendousClient-0.0.3/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1248 2023-04-26 18:59:45.000000 TremendousClient-0.0.3/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:04:13.395628 TremendousClient-0.0.3/TremendousClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:04:13.000000 TremendousClient-0.0.3/TremendousClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      404 2023-04-26 19:04:13.000000 TremendousClient-0.0.3/TremendousClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-26 19:04:13.000000 TremendousClient-0.0.3/TremendousClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-26 19:04:13.000000 TremendousClient-0.0.3/TremendousClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-04-26 19:04:13.000000 TremendousClient-0.0.3/TremendousClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-26 19:04:13.398043 TremendousClient-0.0.3/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      871 2023-04-26 19:04:06.000000 TremendousClient-0.0.3/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:04:13.396479 TremendousClient-0.0.3/tremendous/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      108 2023-04-26 18:53:27.000000 TremendousClient-0.0.3/tremendous/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      292 2023-04-26 18:43:52.000000 TremendousClient-0.0.3/tremendous/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.3/tremendous/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:04:13.397410 TremendousClient-0.0.3/tremendous/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       50 2023-04-26 18:53:09.000000 TremendousClient-0.0.3/tremendous/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1044 2023-04-26 18:45:03.000000 TremendousClient-0.0.3/tremendous/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      726 2023-04-26 18:46:14.000000 TremendousClient-0.0.3/tremendous/service/tremendous_service.py
```

### Comparing `TremendousClient-0.0.2/LICENSE` & `TremendousClient-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.2/PKG-INFO` & `TremendousClient-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TremendousClient
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tremendous Api Client Python package
 Home-page: https://github.com/blueromans/Tremendous.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Tremendous/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TremendousClient-0.0.2/README.md` & `TremendousClient-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.2/TremendousClient.egg-info/PKG-INFO` & `TremendousClient-0.0.3/TremendousClient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TremendousClient
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tremendous Api Client Python package
 Home-page: https://github.com/blueromans/Tremendous.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/Tremendous/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TremendousClient-0.0.2/setup.py` & `TremendousClient-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='TremendousClient',
-    version="0.0.2",
+    version="0.0.3",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='Tremendous Api Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/Tremendous.git',
     project_urls={
@@ -18,10 +18,10 @@
     },
     install_requires=['requests'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=['tremendous'],
+    packages=['tremendous', 'tremendous.service'],
     python_requires=">=3.6",
 )
```

