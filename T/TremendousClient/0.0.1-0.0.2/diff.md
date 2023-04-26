# Comparing `tmp/TremendousClient-0.0.1.tar.gz` & `tmp/TremendousClient-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TremendousClient-0.0.1.tar", last modified: Wed Apr 26 18:49:25 2023, max compression
+gzip compressed data, was "TremendousClient-0.0.2.tar", last modified: Wed Apr 26 19:00:03 2023, max compression
```

## Comparing `TremendousClient-0.0.1.tar` & `TremendousClient-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 18:49:25.401101 TremendousClient-0.0.1/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.1/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1961 2023-04-26 18:49:25.400978 TremendousClient-0.0.1/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1435 2023-04-26 13:00:06.000000 TremendousClient-0.0.1/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 18:49:25.400416 TremendousClient-0.0.1/TremendousClient.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1961 2023-04-26 18:49:25.000000 TremendousClient-0.0.1/TremendousClient.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      297 2023-04-26 18:49:25.000000 TremendousClient-0.0.1/TremendousClient.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-26 18:49:25.000000 TremendousClient-0.0.1/TremendousClient.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-26 18:49:25.000000 TremendousClient-0.0.1/TremendousClient.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-04-26 18:49:25.000000 TremendousClient-0.0.1/TremendousClient.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-26 18:49:25.401142 TremendousClient-0.0.1/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      849 2023-04-26 18:49:14.000000 TremendousClient-0.0.1/setup.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 18:49:25.400798 TremendousClient-0.0.1/tremendous/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       99 2022-11-20 13:13:27.000000 TremendousClient-0.0.1/tremendous/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      292 2023-04-26 18:43:52.000000 TremendousClient-0.0.1/tremendous/exception.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.1/tremendous/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.752019 TremendousClient-0.0.2/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 TremendousClient-0.0.2/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:00:03.751896 TremendousClient-0.0.2/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1248 2023-04-26 18:59:45.000000 TremendousClient-0.0.2/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.750900 TremendousClient-0.0.2/TremendousClient.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1774 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      297 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        9 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       11 2023-04-26 19:00:03.000000 TremendousClient-0.0.2/TremendousClient.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-04-26 19:00:03.752057 TremendousClient-0.0.2/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      849 2023-04-26 18:59:54.000000 TremendousClient-0.0.2/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-04-26 19:00:03.751582 TremendousClient-0.0.2/tremendous/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      108 2023-04-26 18:53:27.000000 TremendousClient-0.0.2/tremendous/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      292 2023-04-26 18:43:52.000000 TremendousClient-0.0.2/tremendous/exception.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2022-05-12 10:14:01.000000 TremendousClient-0.0.2/tremendous/serializer.py
```

### Comparing `TremendousClient-0.0.1/LICENSE` & `TremendousClient-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TremendousClient-0.0.1/setup.py` & `TremendousClient-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='TremendousClient',
-    version="0.0.1",
+    version="0.0.2",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='Tremendous Api Client Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/Tremendous.git',
     project_urls={
```

