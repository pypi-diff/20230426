# Comparing `tmp/dhosting_api-0.1.tar.gz` & `tmp/dhosting_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhosting_api-0.1.tar", last modified: Wed Apr 26 06:25:25 2023, max compression
+gzip compressed data, was "dhosting_api-0.1.2.tar", last modified: Wed Apr 26 08:28:38 2023, max compression
```

## Comparing `dhosting_api-0.1.tar` & `dhosting_api-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/
--rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-26 06:25:25.126963 dhosting_api-0.1/PKG-INFO
--rw-rw-r--   0 maks      (1000) maks      (1000)      552 2023-04-25 13:32:50.000000 dhosting_api-0.1/README.rst
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/dhosting/
--rw-rw-r--   0 maks      (1000) maks      (1000)        0 2023-04-19 07:56:05.000000 dhosting_api-0.1/dhosting/__init__.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     2757 2023-04-25 11:34:03.000000 dhosting_api-0.1/dhosting/adapter.py
--rw-rw-r--   0 maks      (1000) maks      (1000)      830 2023-04-19 12:47:28.000000 dhosting_api-0.1/dhosting/base_email.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     4397 2023-04-25 12:19:42.000000 dhosting_api-0.1/dhosting/connection.py
--rw-rw-r--   0 maks      (1000) maks      (1000)      564 2023-04-21 06:23:02.000000 dhosting_api-0.1/dhosting/exceptions.py
--rw-rw-r--   0 maks      (1000) maks      (1000)     2971 2023-04-25 11:55:46.000000 dhosting_api-0.1/dhosting/utils.py
-drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 06:25:25.126963 dhosting_api-0.1/dhosting_api.egg-info/
--rw-rw-r--   0 maks      (1000) maks      (1000)      736 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/PKG-INFO
--rw-rw-r--   0 maks      (1000) maks      (1000)      326 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/SOURCES.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)        1 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/dependency_links.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)       16 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/requires.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)        9 2023-04-26 06:25:25.000000 dhosting_api-0.1/dhosting_api.egg-info/top_level.txt
--rw-rw-r--   0 maks      (1000) maks      (1000)       38 2023-04-26 06:25:25.126963 dhosting_api-0.1/setup.cfg
--rw-rw-r--   0 maks      (1000) maks      (1000)      478 2023-04-25 13:49:58.000000 dhosting_api-0.1/setup.py
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 08:28:38.541054 dhosting_api-0.1.2/
+-rw-rw-r--   0 maks      (1000) maks      (1000)      738 2023-04-26 08:28:38.541054 dhosting_api-0.1.2/PKG-INFO
+-rw-rw-r--   0 maks      (1000) maks      (1000)      552 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/README.rst
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 08:28:38.541054 dhosting_api-0.1.2/dhosting_api/
+-rw-rw-r--   0 maks      (1000) maks      (1000)        0 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/__init__.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     2757 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/adapter.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)      830 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/base_email.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     4397 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/connection.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)      564 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/exceptions.py
+-rw-rw-r--   0 maks      (1000) maks      (1000)     2971 2023-04-26 08:08:44.000000 dhosting_api-0.1.2/dhosting_api/utils.py
+drwxrwxr-x   0 maks      (1000) maks      (1000)        0 2023-04-26 08:28:38.541054 dhosting_api-0.1.2/dhosting_api.egg-info/
+-rw-rw-r--   0 maks      (1000) maks      (1000)      738 2023-04-26 08:28:38.000000 dhosting_api-0.1.2/dhosting_api.egg-info/PKG-INFO
+-rw-rw-r--   0 maks      (1000) maks      (1000)      350 2023-04-26 08:28:38.000000 dhosting_api-0.1.2/dhosting_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)        1 2023-04-26 08:28:38.000000 dhosting_api-0.1.2/dhosting_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       16 2023-04-26 08:28:38.000000 dhosting_api-0.1.2/dhosting_api.egg-info/requires.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       13 2023-04-26 08:28:38.000000 dhosting_api-0.1.2/dhosting_api.egg-info/top_level.txt
+-rw-rw-r--   0 maks      (1000) maks      (1000)       38 2023-04-26 08:28:38.541054 dhosting_api-0.1.2/setup.cfg
+-rw-rw-r--   0 maks      (1000) maks      (1000)      484 2023-04-26 08:27:45.000000 dhosting_api-0.1.2/setup.py
```

### Comparing `dhosting_api-0.1/PKG-INFO` & `dhosting_api-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhosting_api
-Version: 0.1
+Version: 0.1.2
 Summary: Package to connect with dhosting_api
 Author: Maks Galbierczyk
 Author-email: maksymilian.galbierczyk@apz.pl
 License: MIT
 
 Package to communicate with DhostingApi
 ===============================================================================
```

### Comparing `dhosting_api-0.1/README.rst` & `dhosting_api-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/adapter.py` & `dhosting_api-0.1.2/dhosting_api/adapter.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/base_email.py` & `dhosting_api-0.1.2/dhosting_api/base_email.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/connection.py` & `dhosting_api-0.1.2/dhosting_api/connection.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/exceptions.py` & `dhosting_api-0.1.2/dhosting_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting/utils.py` & `dhosting_api-0.1.2/dhosting_api/utils.py`

 * *Files identical despite different names*

### Comparing `dhosting_api-0.1/dhosting_api.egg-info/PKG-INFO` & `dhosting_api-0.1.2/dhosting_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhosting-api
-Version: 0.1
+Version: 0.1.2
 Summary: Package to connect with dhosting_api
 Author: Maks Galbierczyk
 Author-email: maksymilian.galbierczyk@apz.pl
 License: MIT
 
 Package to communicate with DhostingApi
 ===============================================================================
```

