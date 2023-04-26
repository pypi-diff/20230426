# Comparing `tmp/spectresc-1.0.0rc2.tar.gz` & `tmp/spectresc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectresc-1.0.0rc2.tar", last modified: Tue Apr 25 22:51:22 2023, max compression
+gzip compressed data, was "spectresc-1.0.1.tar", last modified: Wed Apr 26 00:48:44 2023, max compression
```

## Comparing `spectresc-1.0.0rc2.tar` & `spectresc-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/spectresc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-25 22:51:22.000000 spectresc-1.0.0rc2/spectresc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 22:51:22.000000 spectresc-1.0.0rc2/spectresc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:51:22.000000 spectresc-1.0.0rc2/spectresc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:51:22.000000 spectresc-1.0.0rc2/spectresc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 22:51:22.000000 spectresc-1.0.0rc2/spectresc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:51:22.797008 spectresc-1.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/src/spectresc/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/src/spectresc/spectres.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:51:22.801008 spectresc-1.0.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 22:51:12.000000 spectresc-1.0.0rc2/test/test_with_numpy_arange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:48:44.911664 spectresc-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 00:48:33.000000 spectresc-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 00:48:33.000000 spectresc-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 00:48:44.911664 spectresc-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-26 00:48:33.000000 spectresc-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-26 00:48:33.000000 spectresc-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 00:48:44.911664 spectresc-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-26 00:48:33.000000 spectresc-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:48:44.911664 spectresc-1.0.1/spectresc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 00:48:44.000000 spectresc-1.0.1/spectresc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:48:44.907664 spectresc-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:48:44.911664 spectresc-1.0.1/src/spectresc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-26 00:48:33.000000 spectresc-1.0.1/src/spectresc/spectres.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:48:44.911664 spectresc-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-26 00:48:33.000000 spectresc-1.0.1/test/test_with_numpy_arange.py
```

### Comparing `spectresc-1.0.0rc2/LICENSE` & `spectresc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectresc-1.0.0rc2/PKG-INFO` & `spectresc-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectresc
-Version: 1.0.0rc2
+Version: 1.0.1
 Summary: SpectRes in C
 Download-URL: https://github.com/cylammarco/SpectResC
 Author: Marco C Lam
 Maintainer: Marco C Lam
 Maintainer-email: lam@mail.tau.ac.il
 Platform: Windows
 Platform: Linux
```

### Comparing `spectresc-1.0.0rc2/README.md` & `spectresc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spectresc-1.0.0rc2/pyproject.toml` & `spectresc-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spectresc-1.0.0rc2/setup.py` & `spectresc-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 import numpy
 
 setup(
     name="spectresc",
     maintainer="Marco C Lam",
     maintainer_email="lam@mail.tau.ac.il",
-    version="1.0.0.rc2",
+    version="1.0.1",
+    install_requires=[         
+        'numpy',
+    ],
     description="SpectRes in C",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     author="Marco C Lam",
     download_url="https://github.com/cylammarco/SpectResC",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `spectresc-1.0.0rc2/spectresc.egg-info/PKG-INFO` & `spectresc-1.0.1/spectresc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectresc
-Version: 1.0.0rc2
+Version: 1.0.1
 Summary: SpectRes in C
 Download-URL: https://github.com/cylammarco/SpectResC
 Author: Marco C Lam
 Maintainer: Marco C Lam
 Maintainer-email: lam@mail.tau.ac.il
 Platform: Windows
 Platform: Linux
```

### Comparing `spectresc-1.0.0rc2/src/spectresc/spectres.c` & `spectresc-1.0.1/src/spectresc/spectres.c`

 * *Files identical despite different names*

### Comparing `spectresc-1.0.0rc2/test/test_with_numpy_arange.py` & `spectresc-1.0.1/test/test_with_numpy_arange.py`

 * *Files identical despite different names*

