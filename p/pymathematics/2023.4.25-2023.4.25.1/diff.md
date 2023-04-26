# Comparing `tmp/pymathematics-2023.4.25.tar.gz` & `tmp/pymathematics-2023.4.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.25.tar", last modified: Tue Apr 25 12:48:00 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.25.1.tar", last modified: Tue Apr 25 13:56:12 2023, max compression
```

## Comparing `pymathematics-2023.4.25.tar` & `pymathematics-2023.4.25.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:48:00.193707 pymathematics-2023.4.25/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.25/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-25 12:48:00.160705 pymathematics-2023.4.25/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-25 12:30:26.000000 pymathematics-2023.4.25/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:47:59.685701 pymathematics-2023.4.25/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    22007 2023-04-25 12:27:38.000000 pymathematics-2023.4.25/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-25 12:30:01.000000 pymathematics-2023.4.25/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 12:47:59.978706 pymathematics-2023.4.25/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/requires.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-25 12:47:57.000000 pymathematics-2023.4.25/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-25 12:48:00.200708 pymathematics-2023.4.25/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      696 2023-04-25 12:47:36.000000 pymathematics-2023.4.25/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.944833 pymathematics-2023.4.25.1/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.25.1/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-25 13:56:12.930831 pymathematics-2023.4.25.1/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      152 2023-04-25 13:51:05.000000 pymathematics-2023.4.25.1/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.565835 pymathematics-2023.4.25.1/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    21998 2023-04-25 13:01:09.000000 pymathematics-2023.4.25.1/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-25 13:01:18.000000 pymathematics-2023.4.25.1/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-25 13:56:12.869835 pymathematics-2023.4.25.1/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      258 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        6 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/requires.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-25 13:56:11.000000 pymathematics-2023.4.25.1/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-25 13:56:12.949833 pymathematics-2023.4.25.1/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      698 2023-04-25 13:02:38.000000 pymathematics-2023.4.25.1/setup.py
```

### Comparing `pymathematics-2023.4.25/LICENSE` & `pymathematics-2023.4.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.25/pymathematics/__init__.py` & `pymathematics-2023.4.25.1/pymathematics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     
     def shape(matrix_):
         if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
         return len(matrix_),len(matrix_[0])
     
     def size(matrix_):
-        if not matrix.ismatrix(matrix_) == False:
+        if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
         return len(matrix_)*len(matrix_[0])
 
     def determinant(matrix_):
         if not matrix.ismatrix(matrix_):
             raise ValueError("elements of each rows aren't the same")
         if not matrix.ifsquare(matrix_):
```

### Comparing `pymathematics-2023.4.25/setup.py` & `pymathematics-2023.4.25.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.25",
+    version = "2023.4.25.1",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

