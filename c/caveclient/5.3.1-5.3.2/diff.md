# Comparing `tmp/caveclient-5.3.1.tar.gz` & `tmp/caveclient-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.3.1.tar", last modified: Mon Apr 24 02:26:14 2023, max compression
+gzip compressed data, was "caveclient-5.3.2.tar", last modified: Wed Apr 26 19:29:51 2023, max compression
```

## Comparing `caveclient-5.3.1.tar` & `caveclient-5.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.748138 caveclient-5.3.1/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.1/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-24 02:26:14.747731 caveclient-5.3.1/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.3.1/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.742015 caveclient-5.3.1/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-24 02:26:10.000000 caveclient-5.3.1/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.1/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    85649 2023-04-24 02:23:13.000000 caveclient-5.3.1/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.1/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.744580 caveclient-5.3.1/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.743719 caveclient-5.3.1/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.1/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-24 02:26:14.748217 caveclient-5.3.1/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.1/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.747155 caveclient-5.3.1/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.1/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.3.1/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.1/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.863571 caveclient-5.3.2/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.2/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-26 19:29:51.863273 caveclient-5.3.2/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.3.2/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.855492 caveclient-5.3.2/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-26 19:29:48.000000 caveclient-5.3.2/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.2/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-26 13:55:48.000000 caveclient-5.3.2/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.2/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.3.2/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    85648 2023-04-26 19:29:25.000000 caveclient-5.3.2/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.2/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.857914 caveclient-5.3.2/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.2/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.857101 caveclient-5.3.2/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-26 19:29:51.000000 caveclient-5.3.2/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.2/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-26 19:29:51.863638 caveclient-5.3.2/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.2/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-26 19:29:51.860978 caveclient-5.3.2/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.2/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.3.2/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.2/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.2/tests/test_materialization.py
```

### Comparing `caveclient-5.3.1/README.rst` & `caveclient-5.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/annotationengine.py` & `caveclient-5.3.2/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/auth.py` & `caveclient-5.3.2/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/base.py` & `caveclient-5.3.2/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/chunkedgraph.py` & `caveclient-5.3.2/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/datastack_lookup.py` & `caveclient-5.3.2/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/emannotationschemas.py` & `caveclient-5.3.2/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/endpoints.py` & `caveclient-5.3.2/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/format_utils.py` & `caveclient-5.3.2/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/frameworkclient.py` & `caveclient-5.3.2/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/infoservice.py` & `caveclient-5.3.2/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/jsonservice.py` & `caveclient-5.3.2/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/l2cache.py` & `caveclient-5.3.2/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/materializationengine.py` & `caveclient-5.3.2/caveclient/materializationengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1149,15 +1149,15 @@
 it will likely get removed in future versions. "
         )
         timestamp = convert_timestamp(timestamp)
         return_df = True
         if datastack_name is None:
             datastack_name = self.datastack_name
         if desired_resolution is None:
-            desired_resolution = self.default_resolution
+            desired_resolution = self.desired_resolution
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
         data = {}
         query_args = {}
         query_args["return_pyarrow"] = True
         query_args["merge_reference"] = False
         query_args["allow_missing_lookups"] = allow_missing_lookups
@@ -1870,15 +1870,15 @@
         """
         if datastack_name is None:
             datastack_name = self.datastack_name
         if version is None:
             version = self.version
         endpoint_mapping = self.default_url_mapping
         endpoint_mapping["datastack_name"] = datastack_name
-        endpoint_mapping["version"] = version 
+        endpoint_mapping["version"] = version
         url = self._endpoints["get_views"].format_map(endpoint_mapping)
         response = self.session.get(url, verify=self.verify)
         self.raise_for_status(response)
         return response.json()
 
     def get_view_metadata(self, view_name: str, log_warning: bool = True):
         """get metadata for a view"""
```

### Comparing `caveclient-5.3.1/caveclient/session_config.py` & `caveclient-5.3.2/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/timeit.py` & `caveclient-5.3.2/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/tools/caching.py` & `caveclient-5.3.2/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient/tools/stage.py` & `caveclient-5.3.2/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/caveclient.egg-info/SOURCES.txt` & `caveclient-5.3.2/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/setup.py` & `caveclient-5.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/tests/conftest.py` & `caveclient-5.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/tests/test_annotation.py` & `caveclient-5.3.2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/tests/test_chunkedgraph.py` & `caveclient-5.3.2/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/tests/test_infoservice.py` & `caveclient-5.3.2/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.1/tests/test_materialization.py` & `caveclient-5.3.2/tests/test_materialization.py`

 * *Files identical despite different names*

