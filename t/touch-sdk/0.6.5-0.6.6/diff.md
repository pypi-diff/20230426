# Comparing `tmp/touch_sdk-0.6.5.tar.gz` & `tmp/touch_sdk-0.6.6.tar.gz`

## Comparing `touch_sdk-0.6.5.tar` & `touch_sdk-0.6.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.DS_Store
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.gitlab-ci.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.pylintrc
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/version.sh
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/basic.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/basic_threaded.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/custom_data.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/magnetometer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/osc.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/plotter.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/pressure.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/raycasting.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/sensors.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/basic.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/pressure.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/gatt_scanner.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/uuids.py
--rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/watch.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/watch_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/vec_pb2.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_input_pb2.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_output_pb2.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.gitignore
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/LICENSE
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.DS_Store
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.pylintrc
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/version.sh
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/basic.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/basic_threaded.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/custom_data.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/magnetometer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/osc.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/plotter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/pressure.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/raycasting.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/examples/sensors.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/basic.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/pressure.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/gatt_scanner.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/uuids.py
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/watch.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/watch_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/vec_pb2.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_input_pb2.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_output_pb2.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/.gitignore
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.6/PKG-INFO
```

### Comparing `touch_sdk-0.6.5/.DS_Store` & `touch_sdk-0.6.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/basic.py` & `touch_sdk-0.6.6/examples/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/basic_threaded.py` & `touch_sdk-0.6.6/examples/basic_threaded.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/magnetometer.py` & `touch_sdk-0.6.6/examples/magnetometer.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/plotter.py` & `touch_sdk-0.6.6/examples/plotter.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/raycasting.py` & `touch_sdk-0.6.6/examples/raycasting.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/examples/sensors.py` & `touch_sdk-0.6.6/examples/sensors.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/basic.py` & `touch_sdk-0.6.6/src/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/gatt_scanner.py` & `touch_sdk-0.6.6/src/touch_sdk/gatt_scanner.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/utils.py` & `touch_sdk-0.6.6/src/touch_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/watch.py` & `touch_sdk-0.6.6/src/touch_sdk/watch.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/watch_connector.py` & `touch_sdk-0.6.6/src/touch_sdk/watch_connector.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/protobuf/vec_pb2.py` & `touch_sdk-0.6.6/src/touch_sdk/protobuf/vec_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_input_pb2.py` & `touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_input_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_output_pb2.py` & `touch_sdk-0.6.6/src/touch_sdk/protobuf/watch_output_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/LICENSE` & `touch_sdk-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/README.md` & `touch_sdk-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.5/pyproject.toml` & `touch_sdk-0.6.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "touch-sdk"
-version = "0.6.5"
+version = "0.6.6"
 description = "Port 6 Touch SDK"
 license = "ISC"
 authors = [
     { name="Port 6", email="developer@port6.io" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -21,15 +21,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: Android",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
 ]
 dependencies = [
-    "bleak==0.20.1",
-    "protobuf==3.20.0",
-    "asyncio-atexit==1.0.1",
+    "bleak~=0.20.1",
+    "protobuf~=3.20.0",
+    "asyncio-atexit~=1.0.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/port6io/touch-sdk-py#readme"
 "Bug Tracker" = "https://github.com/port6io/touch-sdk-py/issues"
```

### Comparing `touch_sdk-0.6.5/PKG-INFO` & `touch_sdk-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touch-sdk
-Version: 0.6.5
+Version: 0.6.6
 Summary: Port 6 Touch SDK
 Project-URL: Homepage, https://github.com/port6io/touch-sdk-py#readme
 Project-URL: Bug Tracker, https://github.com/port6io/touch-sdk-py/issues
 Author-email: Port 6 <developer@port6.io>
 License-Expression: ISC
 License-File: LICENSE
 Keywords: bluetooth
@@ -14,17 +14,17 @@
 Classifier: Operating System :: Android
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.8
-Requires-Dist: asyncio-atexit==1.0.1
-Requires-Dist: bleak==0.20.1
-Requires-Dist: protobuf==3.20.0
+Requires-Dist: asyncio-atexit~=1.0.1
+Requires-Dist: bleak~=0.20.1
+Requires-Dist: protobuf~=3.20.0
 Description-Content-Type: text/markdown
 
 # Touch SDK py
 
 ![PyPI](https://img.shields.io/pypi/v/touch-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/touch-sdk)
 ![PyPI - License](https://img.shields.io/pypi/l/touch-sdk)
```

