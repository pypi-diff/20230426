# Comparing `tmp/ogsapi-0.4.0.tar.gz` & `tmp/ogsapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.4.0.tar", last modified: Wed Apr 26 04:54:51 2023, max compression
+gzip compressed data, was "ogsapi-0.4.1.tar", last modified: Wed Apr 26 05:00:25 2023, max compression
```

## Comparing `ogsapi-0.4.0.tar` & `ogsapi-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 04:54:51.328851 ogsapi-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-26 04:54:35.000000 ogsapi-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 04:54:51.328851 ogsapi-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4998 2023-04-26 04:54:35.000000 ogsapi-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-26 04:54:35.000000 ogsapi-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 04:54:51.328851 ogsapi-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 04:54:51.324267 ogsapi-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 04:54:51.327018 ogsapi-0.4.0/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 04:54:35.000000 ogsapi-0.4.0/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34578 2023-04-26 04:54:35.000000 ogsapi-0.4.0/src/ogsapi/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 04:54:51.327934 ogsapi-0.4.0/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 04:54:51.000000 ogsapi-0.4.0/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-26 04:54:51.000000 ogsapi-0.4.0/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 04:54:51.000000 ogsapi-0.4.0/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 04:54:51.000000 ogsapi-0.4.0/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 04:54:51.000000 ogsapi-0.4.0/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.374884 ogsapi-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-26 05:00:08.000000 ogsapi-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 05:00:25.374884 ogsapi-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2023-04-26 05:00:08.000000 ogsapi-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-26 05:00:08.000000 ogsapi-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 05:00:25.374884 ogsapi-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.369884 ogsapi-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.371884 ogsapi-0.4.1/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 05:00:08.000000 ogsapi-0.4.1/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34578 2023-04-26 05:00:08.000000 ogsapi-0.4.1/src/ogsapi/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 05:00:25.373884 ogsapi-0.4.1/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5432 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 05:00:25.000000 ogsapi-0.4.1/src/ogsapi.egg-info/top_level.txt
```

### Comparing `ogsapi-0.4.0/LICENSE` & `ogsapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.4.0/PKG-INFO` & `ogsapi-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.4.0/README.md` & `ogsapi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.4.0/pyproject.toml` & `ogsapi-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.4.0/src/ogsapi/api.py` & `ogsapi-0.4.1/src/ogsapi/api.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.4.0/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.4.1/src/ogsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

