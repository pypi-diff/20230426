# Comparing `tmp/verifit-3.0.0.tar.gz` & `tmp/verifit-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-3.0.0.tar", last modified: Wed Apr 26 08:29:12 2023, max compression
+gzip compressed data, was "verifit-3.0.1.tar", last modified: Wed Apr 26 08:32:43 2023, max compression
```

## Comparing `verifit-3.0.0.tar` & `verifit-3.0.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:29:12.824580 verifit-3.0.0/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-3.0.0/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       67 2023-03-06 16:27:14.000000 verifit-3.0.0/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:29:12.824386 verifit-3.0.0/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)     9668 2023-04-26 08:27:28.000000 verifit-3.0.0/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2023-04-26 07:41:08.000000 verifit-3.0.0/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      114 2023-04-26 07:14:27.000000 verifit-3.0.0/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2023-04-26 08:29:12.824621 verifit-3.0.0/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:29:12.819391 verifit-3.0.0/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:29:12.823432 verifit-3.0.0/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      225 2023-03-31 18:28:37.000000 verifit-3.0.0/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1405 2023-03-31 17:39:37.000000 verifit-3.0.0/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      698 2023-03-31 17:39:37.000000 verifit-3.0.0/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      295 2023-03-14 17:26:30.000000 verifit-3.0.0/src/verifit/date_diff.py
--rw-r--r--   0 sorel      (501) staff       (20)     1711 2023-04-01 15:18:03.000000 verifit-3.0.0/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-3.0.0/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     2674 2023-04-26 08:00:17.000000 verifit-3.0.0/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)      407 2023-04-03 13:23:28.000000 verifit-3.0.0/src/verifit/memoize.py
--rw-r--r--   0 sorel      (501) staff       (20)      310 2023-03-27 10:54:45.000000 verifit-3.0.0/src/verifit/prop.py
--rw-r--r--   0 sorel      (501) staff       (20)     2059 2023-04-01 15:01:48.000000 verifit-3.0.0/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)     2068 2023-03-24 18:38:29.000000 verifit-3.0.0/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:29:12.824184 verifit-3.0.0/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:29:12.000000 verifit-3.0.0/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      474 2023-04-26 08:29:12.000000 verifit-3.0.0/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2023-04-26 08:29:12.000000 verifit-3.0.0/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2023-04-26 08:29:12.000000 verifit-3.0.0/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2023-04-26 08:29:12.000000 verifit-3.0.0/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.075963 verifit-3.0.1/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-3.0.1/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       67 2023-03-06 16:27:14.000000 verifit-3.0.1/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:32:43.075783 verifit-3.0.1/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)     9668 2023-04-26 08:27:28.000000 verifit-3.0.1/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2023-04-26 08:32:32.000000 verifit-3.0.1/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      114 2023-04-26 07:14:27.000000 verifit-3.0.1/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2023-04-26 08:32:43.076004 verifit-3.0.1/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.071468 verifit-3.0.1/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.074898 verifit-3.0.1/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      204 2023-04-26 08:31:59.000000 verifit-3.0.1/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1405 2023-03-31 17:39:37.000000 verifit-3.0.1/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      698 2023-03-31 17:39:37.000000 verifit-3.0.1/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      295 2023-03-14 17:26:30.000000 verifit-3.0.1/src/verifit/date_diff.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-3.0.1/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2674 2023-04-26 08:00:17.000000 verifit-3.0.1/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)      407 2023-04-03 13:23:28.000000 verifit-3.0.1/src/verifit/memoize.py
+-rw-r--r--   0 sorel      (501) staff       (20)      310 2023-03-27 10:54:45.000000 verifit-3.0.1/src/verifit/prop.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2059 2023-04-01 15:01:48.000000 verifit-3.0.1/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2068 2023-03-24 18:38:29.000000 verifit-3.0.1/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.075592 verifit-3.0.1/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      452 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/top_level.txt
```

### Comparing `verifit-3.0.0/LICENSE` & `verifit-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/PKG-INFO` & `verifit-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 3.0.0
+Version: 3.0.1
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `verifit-3.0.0/Readme.md` & `verifit-3.0.1/Readme.md`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/pyproject.toml` & `verifit-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "3.0.0"
+version = "3.0.1"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-3.0.0/src/verifit/cache.py` & `verifit-3.0.1/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/src/verifit/config.py` & `verifit-3.0.1/src/verifit/config.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/src/verifit/login.py` & `verifit-3.0.1/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/src/verifit/retrieve.py` & `verifit-3.0.1/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/src/verifit/web_sockets.py` & `verifit-3.0.1/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.0/verifit.egg-info/PKG-INFO` & `verifit-3.0.1/verifit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 3.0.0
+Version: 3.0.1
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

