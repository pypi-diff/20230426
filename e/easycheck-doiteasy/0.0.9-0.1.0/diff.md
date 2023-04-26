# Comparing `tmp/easycheck_doiteasy-0.0.9.tar.gz` & `tmp/easycheck_doiteasy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.9.tar", last modified: Wed Apr 26 21:20:25 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.1.0.tar", last modified: Wed Apr 26 21:39:57 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.9.tar` & `easycheck_doiteasy-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:20:25.952927 easycheck_doiteasy-0.0.9/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.9/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 21:20:25.952927 easycheck_doiteasy-0.0.9/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.9/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:20:25.952927 easycheck_doiteasy-0.0.9/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     6518 2023-04-26 21:17:32.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:20:25.952927 easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 21:20:25.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-26 21:20:25.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-26 21:20:25.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-26 21:20:25.000000 easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.9/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-26 21:20:25.956927 easycheck_doiteasy-0.0.9/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:39:57.652682 easycheck_doiteasy-0.1.0/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.1.0/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 21:39:57.652682 easycheck_doiteasy-0.1.0/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.1.0/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:39:57.652682 easycheck_doiteasy-0.1.0/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     6528 2023-04-26 21:36:07.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-26 21:39:57.652682 easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-26 21:39:57.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-26 21:39:57.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-26 21:39:57.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-26 21:39:57.000000 easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.1.0/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-26 21:39:57.652682 easycheck_doiteasy-0.1.0/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.9/LICENSE.txt` & `easycheck_doiteasy-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.9/PKG-INFO` & `easycheck_doiteasy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.9/README.md` & `easycheck_doiteasy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.9/easycheck_doiteasy/easycheck_doiteasy.py` & `easycheck_doiteasy-0.1.0/easycheck_doiteasy/easycheck_doiteasy.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         except Exception as e:
             logging.error(e)
 
 
     def create_subejecution(self, name: str):
         headers = {}
         domain = self.domain
-        path = '/api/base/ejecution_line/create/'
+        path = '/api/base/ejecution_line/create_ejecution/'
         url = f'{domain}{path}'
         data = {
             'name': name,
             'state': 'init',
             'register_token': self.token
         }
         try:
```

### Comparing `easycheck_doiteasy-0.0.9/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.1.0/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.9/setup.cfg` & `easycheck_doiteasy-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.9
+version = 0.1.0
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://etlcheck.com/
 project_urls =
```

