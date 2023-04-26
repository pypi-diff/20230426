# Comparing `tmp/dtool-lookup-api-0.5.1.tar.gz` & `tmp/dtool-lookup-api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtool-lookup-api-0.5.1.tar", last modified: Sun Oct 23 22:06:08 2022, max compression
+gzip compressed data, was "dtool-lookup-api-0.6.0.tar", last modified: Wed Apr 26 10:26:10 2023, max compression
```

## Comparing `dtool-lookup-api-0.5.1.tar` & `dtool-lookup-api-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 22:06:08.712074 dtool-lookup-api-0.5.1/dtool_lookup_api/
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/dtool_lookup_api/core/
--rw-r--r--   0 runner    (1001) docker     (121)    12987 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/core/LookupClient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5969 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-23 22:06:08.000000 dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 22:06:08.716074 dtool-lookup-api-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/environ.py
--rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/run.sh
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/test_dtool_lookup_api_basics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10266 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/test_dtool_lookup_api_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-10-23 22:05:42.000000 dtool-lookup-api-0.5.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.739995 dtool-lookup-api-0.6.0/dtool_lookup_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/dtool_lookup_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/LookupClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 10:26:10.000000 dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:26:10.743995 dtool-lookup-api-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-26 10:25:50.000000 dtool-lookup-api-0.6.0/tests/utils.py
```

### Comparing `dtool-lookup-api-0.5.1/CHANGELOG.rst` & `dtool-lookup-api-0.6.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGELOG
 =========
 
+0.6.0 (26Apr23)
+---------------
+
+- Server-side pagination
+
 0.5.1 (23Oct22)
 ---------------
 
 - Fixed erroneous interpretation of server response in `register_base_uri` and `update_permissions`.
 - Fixed parsing of text to JSON in `aggregate`.
 - Made all synchronous methods available at top-level via imports in `__init__.py`
```

### Comparing `dtool-lookup-api-0.5.1/CONTRIBUTORS.rst` & `dtool-lookup-api-0.6.0/CONTRIBUTORS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,7 @@
 Contributors
 ============
 
 - `Johannes Hörmman <https://github.com/jotelha/>`_ created this package.
 - `Tjelvar Olsson <https://github.com/tjelvar-olsson>`_ is the main developer behind the `dtool ecosystem <https://github.com/jic-dtool>`_ and this package leans heavily against the structure of his `dtool-lookup-client <https://github.com/jic-dtool/dtool-lookup-client>`_ and `dtool-lookup-server <https://github.com/jic-dtool/dtool-lookup-server>`_.
 - `Lars Pastewka <https://github.com/pastewka>`_ provided the initial `core.LookupClient` implementation.
+- `Ashwin Vazhappilly <https://github.com/ashdroid>`_ implemented pagination.
```

### Comparing `dtool-lookup-api-0.5.1/LICENSE.rst` & `dtool-lookup-api-0.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/PKG-INFO` & `dtool-lookup-api-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dtool-lookup-api
-Version: 0.5.1
+Version: 0.6.0
 Summary: This package offers both synchronous and asynchronous implementations of a standardized Python API to communicate with the dtool lookup server.
 Home-page: https://github.com/IMTEK-Simulation/dtool-lookup-api
-Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.5.1
+Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.0
 Author: Johannes Laurin Hoermann
 Author-email: johannes.hoermann@imtek.uni-freiburg.de
 License: MIT
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 README
@@ -393,10 +393,10 @@
     :alt: PyPI
     :target: https://pypi.org/project/dtool-lookup-api/
 
 .. |github tag| image:: https://img.shields.io/github/v/tag/IMTEK-Simulation/dtool-lookup-api
     :alt: GitHub tag (latest by date)
     :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/tags
 
-.. |github tests| image:: https://img.shields.io/github/workflow/status/IMTEK-Simulation/dtool-lookup-api/test?label=tests
+.. |github tests| image:: https://img.shields.io/github/actions/workflow/status/livMatS/dtool-lookup-api/test.yml?branch=master
     :alt: GitHub Workflow Status
-    :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/actions?query=workflow%3Atest
+    :target: https://github.com/livMatS/dtool-lookup-api/actions/workflows/test.yml
```

### Comparing `dtool-lookup-api-0.5.1/README.rst` & `dtool-lookup-api-0.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -381,10 +381,10 @@
     :alt: PyPI
     :target: https://pypi.org/project/dtool-lookup-api/
 
 .. |github tag| image:: https://img.shields.io/github/v/tag/IMTEK-Simulation/dtool-lookup-api
     :alt: GitHub tag (latest by date)
     :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/tags
 
-.. |github tests| image:: https://img.shields.io/github/workflow/status/IMTEK-Simulation/dtool-lookup-api/test?label=tests
+.. |github tests| image:: https://img.shields.io/github/actions/workflow/status/livMatS/dtool-lookup-api/test.yml?branch=master
     :alt: GitHub Workflow Status
-    :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/actions?query=workflow%3Atest
+    :target: https://github.com/livMatS/dtool-lookup-api/actions/workflows/test.yml
```

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api/__init__.py` & `dtool-lookup-api-0.6.0/dtool_lookup_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api/asynchronous.py` & `dtool-lookup-api-0.6.0/dtool_lookup_api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api/core/__init__.py` & `dtool-lookup-api-0.6.0/dtool_lookup_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api/core/config.py` & `dtool-lookup-api-0.6.0/dtool_lookup_api/core/config.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api/synchronous.py` & `dtool-lookup-api-0.6.0/dtool_lookup_api/synchronous.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/PKG-INFO` & `dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dtool-lookup-api
-Version: 0.5.1
+Version: 0.6.0
 Summary: This package offers both synchronous and asynchronous implementations of a standardized Python API to communicate with the dtool lookup server.
 Home-page: https://github.com/IMTEK-Simulation/dtool-lookup-api
-Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.5.1
+Download-URL: https://github.com/IMTEK-Simulation/dtool-lookup-api/tarball/0.6.0
 Author: Johannes Laurin Hoermann
 Author-email: johannes.hoermann@imtek.uni-freiburg.de
 License: MIT
 Provides-Extra: testing
 License-File: LICENSE.rst
 
 README
@@ -393,10 +393,10 @@
     :alt: PyPI
     :target: https://pypi.org/project/dtool-lookup-api/
 
 .. |github tag| image:: https://img.shields.io/github/v/tag/IMTEK-Simulation/dtool-lookup-api
     :alt: GitHub tag (latest by date)
     :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/tags
 
-.. |github tests| image:: https://img.shields.io/github/workflow/status/IMTEK-Simulation/dtool-lookup-api/test?label=tests
+.. |github tests| image:: https://img.shields.io/github/actions/workflow/status/livMatS/dtool-lookup-api/test.yml?branch=master
     :alt: GitHub Workflow Status
-    :target: https://github.com/IMTEK-Simulation/dtool-lookup-api/actions?query=workflow%3Atest
+    :target: https://github.com/livMatS/dtool-lookup-api/actions/workflows/test.yml
```

### Comparing `dtool-lookup-api-0.5.1/dtool_lookup_api.egg-info/SOURCES.txt` & `dtool-lookup-api-0.6.0/dtool_lookup_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.rst
+CONTRIBUTING.md
 CONTRIBUTORS.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 dtool_lookup_api/__init__.py
```

### Comparing `dtool-lookup-api-0.5.1/setup.py` & `dtool-lookup-api-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/conftest.py` & `dtool-lookup-api-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/environ.py` & `dtool-lookup-api-0.6.0/tests/environ.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/metadata.py` & `dtool-lookup-api-0.6.0/tests/metadata.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/run.sh` & `dtool-lookup-api-0.6.0/tests/run.sh`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/test_dtool_lookup_api_synchronous.py` & `dtool-lookup-api-0.6.0/tests/test_dtool_lookup_api_synchronous.py`

 * *Files identical despite different names*

### Comparing `dtool-lookup-api-0.5.1/tests/utils.py` & `dtool-lookup-api-0.6.0/tests/utils.py`

 * *Files identical despite different names*

