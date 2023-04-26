# Comparing `tmp/firepup650-1.0.6.tar.gz` & `tmp/firepup650-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepup650-1.0.6.tar", last modified: Sat Apr 22 18:25:30 2023, max compression
+gzip compressed data, was "firepup650-1.0.7.tar", last modified: Wed Apr 26 16:53:15 2023, max compression
```

## Comparing `firepup650-1.0.6.tar` & `firepup650-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 18:25:30.502800 firepup650-1.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.6/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1514 2023-04-22 18:25:30.502800 firepup650-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2023-04-22 18:22:06.000000 firepup650-1.0.6/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-04-22 18:25:04.000000 firepup650-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      928 2023-04-22 18:25:30.542800 firepup650-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)       36 2023-04-22 18:16:18.000000 firepup650-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 18:25:30.494800 firepup650-1.0.6/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 18:25:30.498800 firepup650-1.0.6/src/firepup650/
--rw-r--r--   0 runner    (1000) runner    (1000)     3382 2023-04-21 14:40:17.000000 firepup650-1.0.6/src/firepup650/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-22 18:25:30.502800 firepup650-1.0.6/src/firepup650.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1514 2023-04-22 18:25:30.000000 firepup650-1.0.6/src/firepup650.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      267 2023-04-22 18:25:30.000000 firepup650-1.0.6/src/firepup650.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-22 18:25:30.000000 firepup650-1.0.6/src/firepup650.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-04-22 18:25:30.000000 firepup650-1.0.6/src/firepup650.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-22 18:25:30.000000 firepup650-1.0.6/src/firepup650.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 16:53:15.622596 firepup650-1.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1685 2023-04-26 16:53:15.622596 firepup650-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      690 2023-04-26 16:49:19.000000 firepup650-1.0.7/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2023-04-26 16:46:56.000000 firepup650-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      949 2023-04-26 16:53:15.622596 firepup650-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-26 16:38:44.000000 firepup650-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 16:53:15.622596 firepup650-1.0.7/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 16:53:15.622596 firepup650-1.0.7/src/firepup650/
+-rw-r--r--   0 runner    (1000) runner    (1000)    12877 2023-04-26 16:48:55.000000 firepup650-1.0.7/src/firepup650/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-26 16:53:15.622596 firepup650-1.0.7/src/firepup650.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1685 2023-04-26 16:53:15.000000 firepup650-1.0.7/src/firepup650.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      267 2023-04-26 16:53:15.000000 firepup650-1.0.7/src/firepup650.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-26 16:53:15.000000 firepup650-1.0.7/src/firepup650.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2023-04-26 16:53:15.000000 firepup650-1.0.7/src/firepup650.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-26 16:53:15.000000 firepup650-1.0.7/src/firepup650.egg-info/top_level.txt
```

### Comparing `firepup650-1.0.6/LICENSE` & `firepup650-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.6/PKG-INFO` & `firepup650-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.7:
+        Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
         ###### v.1.0.6:
         Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
         ###### v.1.0.5:
         Hopefully, fixes an issue where the package doesn't install it's dependencies
         ###### v.1.0.4:
         Subscript errors
         ###### v.1.0.3:
```

### Comparing `firepup650-1.0.6/README.md` & `firepup650-1.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Firepup650
 Package containing various shorthand things I use, and a few imports I almost always use
 #### Change log:
+###### v.1.0.7:
+Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
 ###### v.1.0.6:
 Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
 ###### v.1.0.5:
 Hopefully, fixes an issue where the package doesn't install it's dependencies
 ###### v.1.0.4:
 Subscript errors
 ###### v.1.0.3:
```

### Comparing `firepup650-1.0.6/setup.cfg` & `firepup650-1.0.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = firepup650
-version = 1.0.6
+version = 1.0.7
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = Package containing various shorthand things I use, and a few imports I almost always use
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/firepup650-PYPI
 project_urls = 
@@ -22,14 +22,16 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	fkeycapture
+	collections
+	typing
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `firepup650-1.0.6/src/firepup650.egg-info/PKG-INFO` & `firepup650-1.0.7/src/firepup650.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.7:
+        Adds `console` (class), `bcolors` (class), and `Color` (function). Fixes type hinting on various things (Lots of thanks to @bigminiboss!).
         ###### v.1.0.6:
         Hopefully, fixes an issue where the package doesn't install it's dependencies (Again. Hopefully.)
         ###### v.1.0.5:
         Hopefully, fixes an issue where the package doesn't install it's dependencies
         ###### v.1.0.4:
         Subscript errors
         ###### v.1.0.3:
```

