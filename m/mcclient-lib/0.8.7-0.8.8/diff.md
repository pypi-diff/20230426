# Comparing `tmp/mcclient-lib-0.8.7.tar.gz` & `tmp/mcclient-lib-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcclient-lib-0.8.7.tar", last modified: Fri Jan 13 15:34:37 2023, max compression
+gzip compressed data, was "mcclient-lib-0.8.8.tar", last modified: Fri Jan 13 15:43:07 2023, max compression
```

## Comparing `mcclient-lib-0.8.7.tar` & `mcclient-lib-0.8.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 15:34:37.477710 mcclient-lib-0.8.7/
--rw-rw-rw-   0        0        0     1075 2022-12-26 17:27:07.000000 mcclient-lib-0.8.7/LICENSE
--rw-rw-rw-   0        0        0     2008 2023-01-13 15:34:37.476711 mcclient-lib-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-01-13 15:30:49.000000 mcclient-lib-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 15:34:37.454311 mcclient-lib-0.8.7/mcclient/
--rw-rw-rw-   0        0        0      225 2023-01-08 15:57:16.000000 mcclient-lib-0.8.7/mcclient/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-01-08 16:00:02.000000 mcclient-lib-0.8.7/mcclient/address.py
--rw-rw-rw-   0        0        0     2307 2023-01-08 16:03:54.000000 mcclient-lib-0.8.7/mcclient/base_client.py
--rw-rw-rw-   0        0        0     1363 2023-01-08 00:44:37.000000 mcclient-lib-0.8.7/mcclient/bedrock_slp.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:34:37.458312 mcclient-lib-0.8.7/mcclient/encoding/
--rw-rw-rw-   0        0        0        0 2022-12-15 16:55:04.000000 mcclient-lib-0.8.7/mcclient/encoding/__init__.py
--rw-rw-rw-   0        0        0      912 2022-12-15 16:56:27.000000 mcclient-lib-0.8.7/mcclient/encoding/packet.py
--rw-rw-rw-   0        0        0      655 2022-12-15 16:49:17.000000 mcclient-lib-0.8.7/mcclient/encoding/varint.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:34:37.461455 mcclient-lib-0.8.7/mcclient/query/
--rw-rw-rw-   0        0        0        0 2022-12-15 17:01:43.000000 mcclient-lib-0.8.7/mcclient/query/__init__.py
--rw-rw-rw-   0        0        0      413 2022-12-16 22:27:05.000000 mcclient-lib-0.8.7/mcclient/query/packet.py
--rw-rw-rw-   0        0        0     3047 2022-12-29 15:58:34.000000 mcclient-lib-0.8.7/mcclient/query/query_client.py
--rw-rw-rw-   0        0        0     5753 2023-01-01 16:31:18.000000 mcclient-lib-0.8.7/mcclient/response.py
--rw-rw-rw-   0        0        0     1883 2023-01-08 16:03:09.000000 mcclient-lib-0.8.7/mcclient/slp.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:34:37.475713 mcclient-lib-0.8.7/mcclient_lib.egg-info/
--rw-rw-rw-   0        0        0     2008 2023-01-13 15:34:37.000000 mcclient-lib-0.8.7/mcclient_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-01-13 15:34:37.000000 mcclient-lib-0.8.7/mcclient_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 15:34:37.000000 mcclient-lib-0.8.7/mcclient_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-01-13 15:34:37.000000 mcclient-lib-0.8.7/mcclient_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-13 15:34:37.000000 mcclient-lib-0.8.7/mcclient_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-01-13 15:32:32.000000 mcclient-lib-0.8.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-13 15:34:37.477710 mcclient-lib-0.8.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/
+-rw-rw-rw-   0        0        0     1075 2022-12-26 17:27:07.000000 mcclient-lib-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     2008 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-01-13 15:30:49.000000 mcclient-lib-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.952734 mcclient-lib-0.8.8/mcclient/
+-rw-rw-rw-   0        0        0      225 2023-01-08 15:57:16.000000 mcclient-lib-0.8.8/mcclient/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-01-08 16:00:02.000000 mcclient-lib-0.8.8/mcclient/address.py
+-rw-rw-rw-   0        0        0     2307 2023-01-08 16:03:54.000000 mcclient-lib-0.8.8/mcclient/base_client.py
+-rw-rw-rw-   0        0        0     1363 2023-01-08 00:44:37.000000 mcclient-lib-0.8.8/mcclient/bedrock_slp.py
+drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.955736 mcclient-lib-0.8.8/mcclient/encoding/
+-rw-rw-rw-   0        0        0        0 2022-12-15 16:55:04.000000 mcclient-lib-0.8.8/mcclient/encoding/__init__.py
+-rw-rw-rw-   0        0        0      912 2022-12-15 16:56:27.000000 mcclient-lib-0.8.8/mcclient/encoding/packet.py
+-rw-rw-rw-   0        0        0      655 2022-12-15 16:49:17.000000 mcclient-lib-0.8.8/mcclient/encoding/varint.py
+drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.959242 mcclient-lib-0.8.8/mcclient/query/
+-rw-rw-rw-   0        0        0        0 2022-12-15 17:01:43.000000 mcclient-lib-0.8.8/mcclient/query/__init__.py
+-rw-rw-rw-   0        0        0      413 2022-12-16 22:27:05.000000 mcclient-lib-0.8.8/mcclient/query/packet.py
+-rw-rw-rw-   0        0        0     3047 2022-12-29 15:58:34.000000 mcclient-lib-0.8.8/mcclient/query/query_client.py
+-rw-rw-rw-   0        0        0     5753 2023-01-01 16:31:18.000000 mcclient-lib-0.8.8/mcclient/response.py
+-rw-rw-rw-   0        0        0     1883 2023-01-08 16:03:09.000000 mcclient-lib-0.8.8/mcclient/slp.py
+drwxrwxrwx   0        0        0        0 2023-01-13 15:43:07.972765 mcclient-lib-0.8.8/mcclient_lib.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-01-13 15:43:07.000000 mcclient-lib-0.8.8/mcclient_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-01-13 15:42:54.000000 mcclient-lib-0.8.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-13 15:43:07.974768 mcclient-lib-0.8.8/setup.cfg
```

### Comparing `mcclient-lib-0.8.7/LICENSE` & `mcclient-lib-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/PKG-INFO` & `mcclient-lib-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcclient-lib
-Version: 0.8.7
+Version: 0.8.8
 Summary: A lightweight Minecraft client
 Author-email: Sch8ill <noreply@noreply.com>
 Project-URL: Homepage, https://www.youtube.com/watch?v=dQw4w9WgXcQ
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mcclient-lib-0.8.7/README.md` & `mcclient-lib-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/address.py` & `mcclient-lib-0.8.8/mcclient/address.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/base_client.py` & `mcclient-lib-0.8.8/mcclient/base_client.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/bedrock_slp.py` & `mcclient-lib-0.8.8/mcclient/bedrock_slp.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/encoding/packet.py` & `mcclient-lib-0.8.8/mcclient/encoding/packet.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/encoding/varint.py` & `mcclient-lib-0.8.8/mcclient/encoding/varint.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/query/query_client.py` & `mcclient-lib-0.8.8/mcclient/query/query_client.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/response.py` & `mcclient-lib-0.8.8/mcclient/response.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient/slp.py` & `mcclient-lib-0.8.8/mcclient/slp.py`

 * *Files identical despite different names*

### Comparing `mcclient-lib-0.8.7/mcclient_lib.egg-info/PKG-INFO` & `mcclient-lib-0.8.8/mcclient_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcclient-lib
-Version: 0.8.7
+Version: 0.8.8
 Summary: A lightweight Minecraft client
 Author-email: Sch8ill <noreply@noreply.com>
 Project-URL: Homepage, https://www.youtube.com/watch?v=dQw4w9WgXcQ
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=dQw4w9WgXcQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mcclient-lib-0.8.7/pyproject.toml` & `mcclient-lib-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mcclient-lib"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
   {name="Sch8ill", email="noreply@noreply.com"},
 ]
 description = "A lightweight Minecraft client"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

