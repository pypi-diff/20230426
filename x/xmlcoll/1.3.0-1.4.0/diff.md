# Comparing `tmp/xmlcoll-1.3.0.tar.gz` & `tmp/xmlcoll-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bradleymeyer/Desktop/work/xmlcoll/dist/.tmp-fr8dki2s/xmlcoll-1.3.0.tar", last modified: Sun Jan  1 13:22:22 2023, max compression
+gzip compressed data, was "xmlcoll-1.4.0.tar", last modified: Tue Apr 25 18:31:39 2023, max compression
```

## Comparing `xmlcoll-1.3.0.tar` & `xmlcoll-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35149 2022-09-25 02:03:11.000000 xmlcoll-1.3.0/LICENSE
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      131 2022-10-08 14:31:38.000000 xmlcoll-1.3.0/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1939 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1046 2023-01-01 13:21:01.000000 xmlcoll-1.3.0/README.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       38 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6131 2022-10-08 15:55:41.000000 xmlcoll-1.3.0/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      291 2023-01-01 13:21:01.000000 xmlcoll-1.3.0/xmlcoll/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      372 2022-10-13 18:49:56.000000 xmlcoll-1.3.0/xmlcoll/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1037 2022-10-08 15:55:41.000000 xmlcoll-1.3.0/xmlcoll/base.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5609 2022-10-08 15:55:41.000000 xmlcoll-1.3.0/xmlcoll/coll.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll/xsd_pub/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      334 2022-10-08 15:04:19.000000 xmlcoll-1.3.0/xmlcoll/xsd_pub/catalog
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1984 2022-10-08 15:04:19.000000 xmlcoll-1.3.0/xmlcoll/xsd_pub/xmlcoll.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3965 2022-10-08 15:04:19.000000 xmlcoll-1.3.0/xmlcoll/xsd_pub/xmlcoll_types.xsd
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1939 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      352 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       44 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-01-01 13:22:22.000000 xmlcoll-1.3.0/xmlcoll.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-25 18:31:39.795628 xmlcoll-1.4.0/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35149 2022-09-25 02:03:11.000000 xmlcoll-1.4.0/LICENSE
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      131 2022-10-08 14:31:38.000000 xmlcoll-1.4.0/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1938 2023-04-25 18:31:39.794872 xmlcoll-1.4.0/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1045 2023-04-25 18:28:58.000000 xmlcoll-1.4.0/README.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       38 2023-04-25 18:31:39.795861 xmlcoll-1.4.0/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6141 2023-04-25 18:28:58.000000 xmlcoll-1.4.0/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-25 18:31:39.782234 xmlcoll-1.4.0/xmlcoll/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      291 2023-04-25 18:28:58.000000 xmlcoll-1.4.0/xmlcoll/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      372 2022-10-13 18:49:56.000000 xmlcoll-1.4.0/xmlcoll/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1037 2022-10-08 15:55:41.000000 xmlcoll-1.4.0/xmlcoll/base.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     8376 2023-04-25 18:28:58.000000 xmlcoll-1.4.0/xmlcoll/coll.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-25 18:31:39.793341 xmlcoll-1.4.0/xmlcoll/xsd_pub/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      334 2023-04-25 18:31:22.000000 xmlcoll-1.4.0/xmlcoll/xsd_pub/catalog
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1984 2023-04-25 18:31:22.000000 xmlcoll-1.4.0/xmlcoll/xsd_pub/xmlcoll.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3965 2023-04-25 18:31:22.000000 xmlcoll-1.4.0/xmlcoll/xsd_pub/xmlcoll_types.xsd
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-25 18:31:39.788825 xmlcoll-1.4.0/xmlcoll.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1938 2023-04-25 18:31:39.000000 xmlcoll-1.4.0/xmlcoll.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      352 2023-04-25 18:31:39.000000 xmlcoll-1.4.0/xmlcoll.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-25 18:31:39.000000 xmlcoll-1.4.0/xmlcoll.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       51 2023-04-25 18:31:39.000000 xmlcoll-1.4.0/xmlcoll.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-04-25 18:31:39.000000 xmlcoll-1.4.0/xmlcoll.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xmlcoll-1.3.0/LICENSE` & `xmlcoll-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlcoll-1.3.0/PKG-INFO` & `xmlcoll-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlcoll
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python project to work with xml data of a collection of items.
 Home-page: https://github.com/mbradle/xmlcoll
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/xmlcoll/issues
 Project-URL: Source, https://github.com/mbradle/xmlcoll/
@@ -25,15 +25,15 @@
 ========
 
 xmlcoll is a python package for working with collections of items.
 The items have heterogeneous data stored as
 `properties` in a dictionary with keys given by a
 name and optional tags.  The package API has routines to write data to and
 retrieve data from `XML <https://www.w3.org/XML/>`_ and to validate that
-XML against a schema..
+XML against a schema.
 
 Installation
 ------------
 
 Install from `PyPI <https://pypi.org/project/xmlcoll>`_ with pip by
 typing in your favorite terminal::
```

### Comparing `xmlcoll-1.3.0/README.rst` & `xmlcoll-1.4.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ========
 
 xmlcoll is a python package for working with collections of items.
 The items have heterogeneous data stored as
 `properties` in a dictionary with keys given by a
 name and optional tags.  The package API has routines to write data to and
 retrieve data from `XML <https://www.w3.org/XML/>`_ and to validate that
-XML against a schema..
+XML against a schema.
 
 Installation
 ------------
 
 Install from `PyPI <https://pypi.org/project/xmlcoll>`_ with pip by
 typing in your favorite terminal::
```

### Comparing `xmlcoll-1.3.0/setup.py` & `xmlcoll-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     packages=find_packages(exclude=["contrib", "docs", "tests"]),  # Required
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=["lxml"],  # Optional
+    install_requires=["lxml", "pandas"],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

### Comparing `xmlcoll-1.3.0/xmlcoll/base.py` & `xmlcoll-1.4.0/xmlcoll/base.py`

 * *Files identical despite different names*

### Comparing `xmlcoll-1.3.0/xmlcoll/xsd_pub/xmlcoll.xsd` & `xmlcoll-1.4.0/xmlcoll/xsd_pub/xmlcoll.xsd`

 * *Files identical despite different names*

### Comparing `xmlcoll-1.3.0/xmlcoll/xsd_pub/xmlcoll_types.xsd` & `xmlcoll-1.4.0/xmlcoll/xsd_pub/xmlcoll_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlcoll-1.3.0/xmlcoll.egg-info/PKG-INFO` & `xmlcoll-1.4.0/xmlcoll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlcoll
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python project to work with xml data of a collection of items.
 Home-page: https://github.com/mbradle/xmlcoll
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/xmlcoll/issues
 Project-URL: Source, https://github.com/mbradle/xmlcoll/
@@ -25,15 +25,15 @@
 ========
 
 xmlcoll is a python package for working with collections of items.
 The items have heterogeneous data stored as
 `properties` in a dictionary with keys given by a
 name and optional tags.  The package API has routines to write data to and
 retrieve data from `XML <https://www.w3.org/XML/>`_ and to validate that
-XML against a schema..
+XML against a schema.
 
 Installation
 ------------
 
 Install from `PyPI <https://pypi.org/project/xmlcoll>`_ with pip by
 typing in your favorite terminal::
```

