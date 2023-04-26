# Comparing `tmp/gbd_tools-4.4.9.tar.gz` & `tmp/gbd_tools-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.4.9.tar", last modified: Tue Apr 25 15:03:17 2023, max compression
+gzip compressed data, was "gbd_tools-4.5.0.tar", last modified: Tue Apr 25 15:21:10 2023, max compression
```

## Comparing `gbd_tools-4.4.9.tar` & `gbd_tools-4.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.691247 gbd_tools-4.4.9/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.9/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 15:03:17.691247 gbd_tools-4.4.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.9/README.md
--rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.4.9/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.9/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8597 2023-04-23 09:05:25.000000 gbd_tools-4.4.9/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.4.9/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.9/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5786 2023-04-20 15:29:05.000000 gbd_tools-4.4.9/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.4.9/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.4.9/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.9/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.9/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.9/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.9/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.9/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.9/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.9/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.9/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.687245 gbd_tools-4.4.9/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.9/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:03:17.691247 gbd_tools-4.4.9/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 15:03:17.000000 gbd_tools-4.4.9/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.4.9/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:03:17.691247 gbd_tools-4.4.9/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-25 15:01:33.000000 gbd_tools-4.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.0/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.5.0/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.111851 gbd_tools-4.5.0/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.0/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8597 2023-04-23 09:05:25.000000 gbd_tools-4.5.0/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.5.0/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.5.0/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5790 2023-04-25 15:20:20.000000 gbd_tools-4.5.0/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.0/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.5.0/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.111851 gbd_tools-4.5.0/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.0/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.0/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.111851 gbd_tools-4.5.0/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.0/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.111851 gbd_tools-4.5.0/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.0/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.0/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.0/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.0/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.0/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.0/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 15:21:09.000000 gbd_tools-4.5.0/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.0/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:21:10.115850 gbd_tools-4.5.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-25 15:20:34.000000 gbd_tools-4.5.0/setup.py
```

### Comparing `gbd_tools-4.4.9/LICENSE` & `gbd_tools-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/PKG-INFO` & `gbd_tools-4.5.0/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gbd_tools
-Version: 4.4.9
+Name: gbd-tools
+Version: 4.5.0
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.9/README.md` & `gbd_tools-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd.py` & `gbd_tools-4.5.0/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/api.py` & `gbd_tools-4.5.0/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/contexts.py` & `gbd_tools-4.5.0/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/database.py` & `gbd_tools-4.5.0/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/grammar.py` & `gbd_tools-4.5.0/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/query.py` & `gbd_tools-4.5.0/gbd_core/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,20 @@
         if collapse and collapse != "none":
             result = [ "{}(DISTINCT({}))".format(collapse, r) for r in result ]
         return "SELECT " + ", ".join(result)
 
 
     def find_translator_feature(self, source_context, target_context):
         for dbname in self.db.get_databases(source_context):
-            print("Checking database {} for translator".format(dbname))
+            #eprint("Checking database {} for translator".format(dbname))
             if "to_"+target_context in self.db.get_features([ dbname ]):
                 return self.db.finfo("to_"+target_context, dbname)
         
         for dbname in self.db.get_databases(target_context):
-            print("Checking database {} for translator".format(dbname))
+            #eprint("Checking database {} for translator".format(dbname))
             if "to_"+source_context in self.db.get_features([ dbname ]):
                 return self.db.finfo("to_"+source_context, dbname)
         
         raise DatabaseException("No translator feature found for contexts {} and {}".format(source_context, target_context))
 
 
     def build_from(self, group, features, join_type="LEFT"):
```

### Comparing `gbd_tools-4.4.9/gbd_core/schema.py` & `gbd_tools-4.5.0/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/util.py` & `gbd_tools-4.5.0/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_core/util_argparse.py` & `gbd_tools-4.5.0/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_init/cnf_extractors.py` & `gbd_tools-4.5.0/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_init/cnf_transformers.py` & `gbd_tools-4.5.0/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_init/gbdhash.py` & `gbd_tools-4.5.0/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_init/initializer.py` & `gbd_tools-4.5.0/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.5.0/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.5.0/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.5.0/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/static/main.css` & `gbd_tools-4.5.0/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/static/w3.js` & `gbd_tools-4.5.0/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_server/templates/index.html` & `gbd_tools-4.5.0/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gbd-tools
-Version: 4.4.9
+Name: gbd_tools
+Version: 4.5.0
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.9/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.5.0/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/server.py` & `gbd_tools-4.5.0/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.9/setup.py` & `gbd_tools-4.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.4.9',
+  version='4.5.0',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

