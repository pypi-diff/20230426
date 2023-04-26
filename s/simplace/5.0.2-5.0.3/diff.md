# Comparing `tmp/simplace-5.0.2.tar.gz` & `tmp/simplace-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplace-5.0.2.tar", last modified: Wed Mar  1 13:02:24 2023, max compression
+gzip compressed data, was "simplace-5.0.3.tar", last modified: Wed Apr 26 11:31:27 2023, max compression
```

## Comparing `simplace-5.0.2.tar` & `simplace-5.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 13:02:24.069388 simplace-5.0.2/
--rw-rw-rw-   0        0        0     3309 2023-03-01 13:01:43.000000 simplace-5.0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    35141 2017-07-20 15:04:53.000000 simplace-5.0.2/LICENSE
--rw-rw-rw-   0        0        0       41 2016-11-17 17:32:58.000000 simplace-5.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1293 2023-03-01 13:02:24.068389 simplace-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      743 2022-04-19 11:42:59.000000 simplace-5.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-01 13:02:24.069388 simplace-5.0.2/setup.cfg
--rw-rw-rw-   0        0        0      995 2021-11-25 08:32:20.000000 simplace-5.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 13:02:24.020416 simplace-5.0.2/simplace/
--rw-rw-rw-   0        0        0     6267 2023-03-01 12:31:13.000000 simplace-5.0.2/simplace/SimplaceClasses.py
--rw-rw-rw-   0        0        0      125 2016-11-17 17:32:58.000000 simplace-5.0.2/simplace/__init__.py
--rw-rw-rw-   0        0        0       77 2023-03-01 13:01:53.000000 simplace-5.0.2/simplace/_version.py
--rw-rw-rw-   0        0        0    23795 2023-03-01 13:00:14.000000 simplace-5.0.2/simplace/simplace.py
-drwxrwxrwx   0        0        0        0 2023-03-01 13:02:24.066390 simplace-5.0.2/simplace.egg-info/
--rw-rw-rw-   0        0        0     1293 2023-03-01 13:02:23.000000 simplace-5.0.2/simplace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-03-01 13:02:23.000000 simplace-5.0.2/simplace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 13:02:23.000000 simplace-5.0.2/simplace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-24 10:54:28.000000 simplace-5.0.2/simplace.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-03-01 13:02:23.000000 simplace-5.0.2/simplace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-01 13:02:23.000000 simplace-5.0.2/simplace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 11:31:27.239037 simplace-5.0.3/
+-rw-rw-rw-   0        0        0     3499 2023-04-26 11:30:20.000000 simplace-5.0.3/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    35141 2017-07-20 15:04:53.000000 simplace-5.0.3/LICENSE
+-rw-rw-rw-   0        0        0       41 2016-11-17 17:32:58.000000 simplace-5.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1293 2023-04-26 11:31:27.239037 simplace-5.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2022-04-19 11:42:59.000000 simplace-5.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-26 11:31:27.240037 simplace-5.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      995 2021-11-25 08:32:20.000000 simplace-5.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:31:27.191231 simplace-5.0.3/simplace/
+-rw-rw-rw-   0        0        0     6267 2023-03-01 12:31:13.000000 simplace-5.0.3/simplace/SimplaceClasses.py
+-rw-rw-rw-   0        0        0      125 2016-11-17 17:32:58.000000 simplace-5.0.3/simplace/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-04-26 11:27:11.000000 simplace-5.0.3/simplace/_version.py
+-rw-rw-rw-   0        0        0    24064 2023-04-26 11:29:44.000000 simplace-5.0.3/simplace/simplace.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:31:27.236035 simplace-5.0.3/simplace.egg-info/
+-rw-rw-rw-   0        0        0     1293 2023-04-26 11:31:26.000000 simplace-5.0.3/simplace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-04-26 11:31:26.000000 simplace-5.0.3/simplace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 11:31:26.000000 simplace-5.0.3/simplace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-24 10:54:28.000000 simplace-5.0.3/simplace.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-26 11:31:26.000000 simplace-5.0.3/simplace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 11:31:26.000000 simplace-5.0.3/simplace.egg-info/top_level.txt
```

### Comparing `simplace-5.0.2/CHANGELOG.rst` & `simplace-5.0.3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 5.0.3
+~~~~~~~~~~~~~
+ * InstallationDir can point also to a folder containing lib subfolder with required simplace .jars
+ * findSimplaceInstallation now checks more directories
+
 Version 5.0.2
 ~~~~~~~~~~~~~
  * Set correct workdir for setting "lapclient"
 
 Version 5.0.1
 ~~~~~~~~~~~~~
  * Parameter InstallationDir is now optional, tries to fetch it automatically
```

### Comparing `simplace-5.0.2/LICENSE` & `simplace-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplace-5.0.2/PKG-INFO` & `simplace-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplace
-Version: 5.0.2
+Version: 5.0.3
 Summary: Interact with the simulation framework Simplace
 Home-page: https://www.simplace.net/
 Author: Gunther Krauss
 Author-email: guntherkrauss@uni-bonn.de
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simplace-5.0.2/README.rst` & `simplace-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `simplace-5.0.2/setup.py` & `simplace-5.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `simplace-5.0.2/simplace/SimplaceClasses.py` & `simplace-5.0.3/simplace/SimplaceClasses.py`

 * *Files identical despite different names*

### Comparing `simplace-5.0.2/simplace/simplace.py` & `simplace-5.0.3/simplace/simplace.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     if(outputDir == None):
         outputDir = os.path.join(installDir,'simplace_run/output/')
 
     cpliblist = [os.path.join(directory,filenm)
                 for directory, _, files in os.walk(os.path.join(installDir,"simplace_core","lib"))
                     for filenm in files
                         if filenm.lower().endswith('.jar')]
+    cpliblist = cpliblist + [os.path.join(directory,filenm)
+                for directory, _, files in os.walk(os.path.join(installDir,"lib"))
+                    for filenm in files
+                        if filenm.lower().endswith('.jar')]
 
     cplist = [
         'simplace_core/build/classes',
         'simplace_core/conf',
         'simplace_modules/build/classes',
         'simplace_run/build/classes',
         'simplace_run/conf',
@@ -512,15 +516,15 @@
         list: List of paths to Simplace installations
     """
     parents = []
     home = os.environ.get('HOME')
     if(home!=None):
         parents = [home]
     parents += ["d:","c:","e:","f:","g:",os.getcwd()]
-    subdirs = ["workspace/","simplace/","java/simplace/"]
+    subdirs = ["workspace/","simplace/","java/simplace/","simplace/workspace/"]
     dirs = directories
     if(tryStandardDirs):
         dirs = dirs + [p+"/"+s for p in parents for s in subdirs]
     required = {"simplace_core", "simplace_modules"}
     if(not ignoreSimulationsDir):
         required = required.union({simulationsDir})
     found = [d.rstrip("\\/")+"/" for d in dirs
```

### Comparing `simplace-5.0.2/simplace.egg-info/PKG-INFO` & `simplace-5.0.3/simplace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplace
-Version: 5.0.2
+Version: 5.0.3
 Summary: Interact with the simulation framework Simplace
 Home-page: https://www.simplace.net/
 Author: Gunther Krauss
 Author-email: guntherkrauss@uni-bonn.de
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

