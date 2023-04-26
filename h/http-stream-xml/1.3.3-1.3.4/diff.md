# Comparing `tmp/http-stream-xml-1.3.3.tar.gz` & `tmp/http-stream-xml-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-stream-xml-1.3.3.tar", last modified: Wed Apr 26 04:47:23 2023, max compression
+gzip compressed data, was "http-stream-xml-1.3.4.tar", last modified: Wed Apr 26 04:50:41 2023, max compression
```

## Comparing `http-stream-xml-1.3.3.tar` & `http-stream-xml-1.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:47:23.154237 http-stream-xml-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 04:47:13.000000 http-stream-xml-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:47:23.154237 http-stream-xml-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-26 04:47:13.000000 http-stream-xml-1.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:47:23.154237 http-stream-xml-1.3.3/http_stream_xml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:47:23.000000 http-stream-xml-1.3.3/http_stream_xml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 04:47:23.000000 http-stream-xml-1.3.3/http_stream_xml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:47:23.000000 http-stream-xml-1.3.3/http_stream_xml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:47:23.000000 http-stream-xml-1.3.3/http_stream_xml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 04:47:23.154237 http-stream-xml-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-26 04:47:13.000000 http-stream-xml-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/http_stream_xml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:50:41.000000 http-stream-xml-1.3.4/http_stream_xml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 04:50:41.182674 http-stream-xml-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-26 04:50:29.000000 http-stream-xml-1.3.4/setup.py
```

### Comparing `http-stream-xml-1.3.3/PKG-INFO` & `http-stream-xml-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Parse XML in HTTP response on the fly, by chunks
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `http-stream-xml-1.3.3/README.rst` & `http-stream-xml-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `http-stream-xml-1.3.3/http_stream_xml.egg-info/PKG-INFO` & `http-stream-xml-1.3.4/http_stream_xml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-stream-xml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Parse XML in HTTP response on the fly, by chunks
 Home-page: https://http-stream-xml.readthedocs.io/en/latest/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: http stream xml chunked
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `http-stream-xml-1.3.3/setup.py` & `http-stream-xml-1.3.4/setup.py`

 * *Files identical despite different names*

