# Comparing `tmp/mammath-0.1.8.tar.gz` & `tmp/mammath-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammath-0.1.8.tar", last modified: Sat Apr 22 17:24:32 2023, max compression
+gzip compressed data, was "mammath-0.1.9.tar", last modified: Wed Apr 26 15:57:10 2023, max compression
```

## Comparing `mammath-0.1.8.tar` & `mammath-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.201384 mammath-0.1.8/
--rw-rw-rw-   0        0        0      968 2023-04-22 17:24:32.200387 mammath-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      525 2022-04-20 06:39:37.000000 mammath-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.190413 mammath-0.1.8/mammath/
--rw-rw-rw-   0        0        0    47932 2023-04-22 17:17:39.000000 mammath-0.1.8/mammath/__init__.py
--rw-rw-rw-   0        0        0    47932 2023-04-22 16:01:57.000000 mammath-0.1.8/mammath/mammath.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.199390 mammath-0.1.8/mammath.egg-info/
--rw-rw-rw-   0        0        0      968 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-10-13 04:05:08.000000 mammath-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 17:24:32.201384 mammath-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-04-22 16:00:25.000000 mammath-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:57:10.473706 mammath-0.1.9/
+-rw-rw-rw-   0        0        0     3245 2023-04-26 15:57:10.472708 mammath-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2791 2023-04-26 15:55:50.000000 mammath-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 15:57:10.461742 mammath-0.1.9/mammath/
+-rw-rw-rw-   0        0        0    95388 2023-04-26 15:35:43.000000 mammath-0.1.9/mammath/__init__.py
+-rw-rw-rw-   0        0        0    95388 2023-04-26 15:28:19.000000 mammath-0.1.9/mammath/mammath.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:57:10.471711 mammath-0.1.9/mammath.egg-info/
+-rw-rw-rw-   0        0        0     3245 2023-04-26 15:57:10.000000 mammath-0.1.9/mammath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-26 15:57:10.000000 mammath-0.1.9/mammath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:57:10.000000 mammath-0.1.9/mammath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-26 15:57:10.000000 mammath-0.1.9/mammath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 15:57:10.000000 mammath-0.1.9/mammath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-10-13 04:05:08.000000 mammath-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:57:10.473706 mammath-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-04-26 15:48:12.000000 mammath-0.1.9/setup.py
```

### Comparing `mammath-0.1.8/setup.py` & `mammath-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mammath",
-    version="0.1.8",
+    version="0.1.9",
     author="Vihaan Mathur & Harihar Rengan",
     author_email="vihaan.harihar314@gmail.com",
-    description="A package that contains all you will need when you need to do maths in python",
+    description="A package that contains all you will need when you need to do maths or science in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
```

