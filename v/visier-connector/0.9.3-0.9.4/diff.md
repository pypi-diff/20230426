# Comparing `tmp/visier-connector-0.9.3.tar.gz` & `tmp/visier-connector-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.3.tar", last modified: Fri Apr 14 17:29:26 2023, max compression
+gzip compressed data, was "visier-connector-0.9.4.tar", last modified: Wed Apr 26 17:26:29 2023, max compression
```

## Comparing `visier-connector-0.9.3.tar` & `visier-connector-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.989873 visier-connector-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 17:29:15.000000 visier-connector-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:29:26.989873 visier-connector-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-14 17:29:15.000000 visier-connector-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 17:29:15.000000 visier-connector-0.9.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-14 17:29:15.000000 visier-connector-0.9.3/examples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:29:26.989873 visier-connector-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 17:29:15.000000 visier-connector-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.567140 visier-connector-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 17:26:06.000000 visier-connector-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-04-26 17:26:29.567140 visier-connector-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-26 17:26:06.000000 visier-connector-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-26 17:26:06.000000 visier-connector-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:26:29.567140 visier-connector-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.3/LICENSE` & `visier-connector-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.3/README.md` & `visier-connector-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.3/examples/__init__.py` & `visier-connector-0.9.4/visier/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License, Version 2.0 for more details.
 #
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
-Visier Public Python Connector Example Queries
+Visier Public Python Connector
 """
 
-from .util import *
+__version__ = "0.9.4"
```

### Comparing `visier-connector-0.9.3/visier/connector/__init__.py` & `visier-connector-0.9.4/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.3/visier/connector/authentication.py` & `visier-connector-0.9.4/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.3/visier/connector/sessions.py` & `visier-connector-0.9.4/visier/connector/sessions.py`

 * *Files identical despite different names*

