# Comparing `tmp/pipupload-0.1.1.tar.gz` & `tmp/pipupload-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pipupload-0.1.1.tar", last modified: Wed Apr 26 13:04:04 2023, max compression
+gzip compressed data, was "dist\pipupload-0.1.2.tar", last modified: Wed Apr 26 13:09:32 2023, max compression
```

## Comparing `pipupload-0.1.1.tar` & `pipupload-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 13:04:04.000000 pipupload-0.1.1/
--rw-rw-rw-   0        0        0      283 2023-04-26 13:04:04.000000 pipupload-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload/
--rw-rw-rw-   0        0        0      130 2023-04-26 07:28:59.000000 pipupload-0.1.1/pipupload/__init__.py
--rw-rw-rw-   0        0        0       59 2023-04-25 10:40:21.000000 pipupload-0.1.1/pipupload/add_num.py
--rw-rw-rw-   0        0        0      141 2023-04-26 07:28:59.000000 pipupload-0.1.1/pipupload/maintest.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/
--rw-rw-rw-   0        0        0      283 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 13:04:04.000000 pipupload-0.1.1/pipupload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-26 13:04:04.000000 pipupload-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-04-26 13:03:15.000000 pipupload-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:09:32.000000 pipupload-0.1.2/
+-rw-rw-rw-   0        0        0      283 2023-04-26 13:09:32.000000 pipupload-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload/
+-rw-rw-rw-   0        0        0      130 2023-04-26 07:28:59.000000 pipupload-0.1.2/pipupload/__init__.py
+-rw-rw-rw-   0        0        0       59 2023-04-25 10:40:21.000000 pipupload-0.1.2/pipupload/add_num.py
+-rw-rw-rw-   0        0        0      141 2023-04-26 13:08:14.000000 pipupload-0.1.2/pipupload/maintest.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 13:09:32.000000 pipupload-0.1.2/pipupload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 13:04:04.000000 pipupload-0.1.2/pipupload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-26 13:09:32.000000 pipupload-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-04-26 13:09:27.000000 pipupload-0.1.2/setup.py
```

### Comparing `pipupload-0.1.1/setup.py` & `pipupload-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     package_dir={'requests': 'requests'},)
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="pipupload",
-    version="0.1.1",
+    version="0.1.2",
     keywords=["pip", "pip_test", "python", "layUI"],
     description="pip_test",
     long_description="pipupload",
     license="MIT",
     url="https://github.com/MrClin/python_pip_install.git",
     author="cl",
     author_email="cl459134@163.com",
```

