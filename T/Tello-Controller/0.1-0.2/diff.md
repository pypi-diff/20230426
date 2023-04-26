# Comparing `tmp/Tello-Controller-0.1.tar.gz` & `tmp/Tello-Controller-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tello-Controller-0.1.tar", last modified: Wed Apr 26 15:03:04 2023, max compression
+gzip compressed data, was "Tello-Controller-0.2.tar", last modified: Wed Apr 26 15:10:55 2023, max compression
```

## Comparing `Tello-Controller-0.1.tar` & `Tello-Controller-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:03:04.594182 Tello-Controller-0.1/
--rw-rw-rw-   0        0        0     1063 2023-04-26 15:00:53.000000 Tello-Controller-0.1/LICENSE
--rw-rw-rw-   0        0        0     3722 2023-04-26 15:03:04.594182 Tello-Controller-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1871 2023-04-26 15:00:53.000000 Tello-Controller-0.1/README.md
--rw-rw-rw-   0        0        0      757 2023-04-26 15:00:53.000000 Tello-Controller-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 15:03:04.594182 Tello-Controller-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 15:03:04.585177 Tello-Controller-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:03:04.585177 Tello-Controller-0.1/src/Controller/
--rw-rw-rw-   0        0        0       88 2023-04-26 15:00:53.000000 Tello-Controller-0.1/src/Controller/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:03:04.594182 Tello-Controller-0.1/src/Tello_Controller.egg-info/
--rw-rw-rw-   0        0        0     3722 2023-04-26 15:03:04.000000 Tello-Controller-0.1/src/Tello_Controller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-04-26 15:03:04.000000 Tello-Controller-0.1/src/Tello_Controller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:03:04.000000 Tello-Controller-0.1/src/Tello_Controller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 15:03:04.000000 Tello-Controller-0.1/src/Tello_Controller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      394 2023-04-26 15:00:53.000000 Tello-Controller-0.1/src/main.py
--rw-rw-rw-   0        0        0     1890 2023-04-26 15:00:53.000000 Tello-Controller-0.1/src/script_sender.py
--rw-rw-rw-   0        0        0     1384 2023-04-26 15:00:53.000000 Tello-Controller-0.1/src/stats.py
--rw-rw-rw-   0        0        0     1821 2023-04-26 15:00:53.000000 Tello-Controller-0.1/src/tello.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:10:55.068583 Tello-Controller-0.2/
+-rw-rw-rw-   0        0        0     1063 2023-04-26 15:00:53.000000 Tello-Controller-0.2/LICENSE
+-rw-rw-rw-   0        0        0     3722 2023-04-26 15:10:55.068583 Tello-Controller-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1871 2023-04-26 15:00:53.000000 Tello-Controller-0.2/README.md
+-rw-rw-rw-   0        0        0      757 2023-04-26 15:10:38.000000 Tello-Controller-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:10:55.068583 Tello-Controller-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 15:10:55.068583 Tello-Controller-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 15:10:55.068583 Tello-Controller-0.2/src/Controller/
+-rw-rw-rw-   0        0        0       88 2023-04-26 15:00:53.000000 Tello-Controller-0.2/src/Controller/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 15:10:55.068583 Tello-Controller-0.2/src/Tello_Controller.egg-info/
+-rw-rw-rw-   0        0        0     3722 2023-04-26 15:10:55.000000 Tello-Controller-0.2/src/Tello_Controller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-04-26 15:10:55.000000 Tello-Controller-0.2/src/Tello_Controller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 15:10:55.000000 Tello-Controller-0.2/src/Tello_Controller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 15:10:55.000000 Tello-Controller-0.2/src/Tello_Controller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      394 2023-04-26 15:00:53.000000 Tello-Controller-0.2/src/main.py
+-rw-rw-rw-   0        0        0     1890 2023-04-26 15:00:53.000000 Tello-Controller-0.2/src/script_sender.py
+-rw-rw-rw-   0        0        0     1384 2023-04-26 15:00:53.000000 Tello-Controller-0.2/src/stats.py
+-rw-rw-rw-   0        0        0     1821 2023-04-26 15:00:53.000000 Tello-Controller-0.2/src/tello.py
```

### Comparing `Tello-Controller-0.1/LICENSE` & `Tello-Controller-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Tello-Controller-0.1/PKG-INFO` & `Tello-Controller-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tello-Controller
-Version: 0.1
+Version: 0.2
 Summary: Simple library for using DJI Tello drones
 Author-email: Alberto <rossani.alberto4@gmail.com>, botasu06 <botasu06@gmail.com>, Jen1s <lorenzo.uduvidane@itiszuccante.edu.it>
 License: MIT License
         
         Copyright (c) 2023 Xyon40k
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Tello-Controller-0.1/README.md` & `Tello-Controller-0.2/README.md`

 * *Files identical despite different names*

### Comparing `Tello-Controller-0.1/pyproject.toml` & `Tello-Controller-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Tello-Controller"
-version = "0.1"
+version = "0.2"
 description = "Simple library for using DJI Tello drones"
 readme = "README.md"
 authors = [{ name = "Alberto", email = "rossani.alberto4@gmail.com" }, { name = "botasu06", email = "botasu06@gmail.com" }, { name = "Jen1s", email = "lorenzo.uduvidane@itiszuccante.edu.it" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `Tello-Controller-0.1/src/Tello_Controller.egg-info/PKG-INFO` & `Tello-Controller-0.2/src/Tello_Controller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tello-Controller
-Version: 0.1
+Version: 0.2
 Summary: Simple library for using DJI Tello drones
 Author-email: Alberto <rossani.alberto4@gmail.com>, botasu06 <botasu06@gmail.com>, Jen1s <lorenzo.uduvidane@itiszuccante.edu.it>
 License: MIT License
         
         Copyright (c) 2023 Xyon40k
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Tello-Controller-0.1/src/script_sender.py` & `Tello-Controller-0.2/src/script_sender.py`

 * *Files identical despite different names*

### Comparing `Tello-Controller-0.1/src/stats.py` & `Tello-Controller-0.2/src/stats.py`

 * *Files identical despite different names*

### Comparing `Tello-Controller-0.1/src/tello.py` & `Tello-Controller-0.2/src/tello.py`

 * *Files identical despite different names*

