# Comparing `tmp/helix_mockserver_client-1.0.5.tar.gz` & `tmp/helix_mockserver_client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helix_mockserver_client-1.0.5.tar", last modified: Wed Apr 26 03:12:02 2023, max compression
+gzip compressed data, was "dist/helix_mockserver_client-1.0.6.tar", last modified: Wed Apr 26 06:33:46 2023, max compression
```

## Comparing `helix_mockserver_client-1.0.5.tar` & `helix_mockserver_client-1.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/mockserver_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/_timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_request_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/match_request_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/mock_expectation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13165 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/mock_requests_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/mockserver_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/mockserver_verify_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/mockserver_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 03:12:01.000000 helix_mockserver_client-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/from_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file/test_mock_server_from_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_mismatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_mismatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_expectation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_expectation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:02.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 03:11:14.000000 helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/mockserver_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_request_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/match_request_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/mock_expectation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/mock_requests_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/mockserver_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/mockserver_verify_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/mockserver_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 06:33:45.000000 helix_mockserver_client-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/from_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file/test_mock_server_from_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_mismatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_mismatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_expectation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_expectation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:33:46.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 06:32:54.000000 helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py
```

### Comparing `helix_mockserver_client-1.0.5/LICENSE` & `helix_mockserver_client-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/Makefile` & `helix_mockserver_client-1.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/PKG-INFO` & `helix_mockserver_client-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix_mockserver_client
-Version: 1.0.5
+Version: 1.0.6
 Summary: mockserver_client
 Home-page: https://github.com/icanbwell/mockserver_client
 Author: Imran Qureshi
 Author-email: imran.qureshi@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix_mockserver_client-1.0.5/README.md` & `helix_mockserver_client-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/PKG-INFO` & `helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix-mockserver-client
-Version: 1.0.5
+Version: 1.0.6
 Summary: mockserver_client
 Home-page: https://github.com/icanbwell/mockserver_client
 Author: Imran Qureshi
 Author-email: imran.qureshi@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix_mockserver_client-1.0.5/helix_mockserver_client.egg-info/SOURCES.txt` & `helix_mockserver_client-1.0.6/helix_mockserver_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py` & `helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py` & `helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/exceptions/mock_server_request_not_found_exception.py` & `helix_mockserver_client-1.0.6/mockserver_client/exceptions/mock_server_request_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/mock_expectation.py` & `helix_mockserver_client-1.0.6/mockserver_client/mock_expectation.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/mock_request.py` & `helix_mockserver_client-1.0.6/mockserver_client/mock_request.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/mock_requests_loader.py` & `helix_mockserver_client-1.0.6/mockserver_client/mock_requests_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,14 +63,61 @@
                     url_prefix=url_prefix,
                     response_body=response_body,
                 )
 
     return files
 
 
+def load_mock_fhir_requests_for_single_file(
+    folder: Path,
+    single_file_name: str,
+    mock_client: MockServerFriendlyClient,
+    method: str = "POST",
+    relative_path: Optional[str] = None,
+    query_string: Optional[Dict[str, Any]] = None,
+    url_prefix: Optional[str] = None,
+    response_body: Optional[str] = None,
+) -> List[str]:
+    """
+    Loads a single .json file from the given folder
+
+    from https://pypi.org/project/mockserver-friendly-client/
+
+    :param folder: where to look for a given .json file
+    :param single_file_name: a single json file name
+    :param mock_client: client to mock server
+    :param method:
+    :param relative_path:
+    :param query_string:
+    :param url_prefix:
+    :param response_body:
+    """
+
+    file_name: str
+    files: List[str] = sorted(
+        glob(str(folder.joinpath(f"**/{single_file_name}")), recursive=True)
+    )
+    for file_name in files:
+        # load file as json
+        with open(file_name, "r") as file:
+            contents = json.loads(file.read())
+
+            mock_single_request(
+                fhir_request=contents,
+                method=method,
+                mock_client=mock_client,
+                relative_path=relative_path,
+                query_string=query_string,
+                url_prefix=url_prefix,
+                response_body=response_body,
+            )
+
+    return files
+
+
 def mock_single_request(
     fhir_request: Dict[str, Any],
     method: str,
     mock_client: MockServerFriendlyClient,
     relative_path: Optional[str],
     query_string: Optional[Dict[str, Any]],
     url_prefix: Optional[str],
```

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/mockserver_client.py` & `helix_mockserver_client-1.0.6/mockserver_client/mockserver_client.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/mockserver_client/mockserver_verify_exception.py` & `helix_mockserver_client-1.0.6/mockserver_client/mockserver_verify_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/setup.py` & `helix_mockserver_client-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/tests/from_file/test_mock_server_from_file.py` & `helix_mockserver_client-1.0.6/tests/from_file/test_mock_server_from_file.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py` & `helix_mockserver_client-1.0.6/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py` & `helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py` & `helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.0.5/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py` & `helix_mockserver_client-1.0.6/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py`

 * *Files identical despite different names*

