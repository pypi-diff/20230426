# Comparing `tmp/tonkin-0.0.8.tar.gz` & `tmp/tonkin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonkin-0.0.8.tar", last modified: Wed Apr 26 13:12:50 2023, max compression
+gzip compressed data, was "tonkin-0.0.9.tar", last modified: Wed Apr 26 13:56:41 2023, max compression
```

## Comparing `tonkin-0.0.8.tar` & `tonkin-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:50.093029 tonkin-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:12:50.093029 tonkin-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 13:12:37.000000 tonkin-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 13:12:37.000000 tonkin-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 13:12:50.093029 tonkin-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 13:12:37.000000 tonkin-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:50.093029 tonkin-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:50.093029 tonkin-0.0.8/src/tonkin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/datfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/datvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/varsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 13:12:37.000000 tonkin-0.0.8/src/tonkin/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:50.093029 tonkin-0.0.8/src/tonkin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:12:50.000000 tonkin-0.0.8/src/tonkin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 13:12:50.000000 tonkin-0.0.8/src/tonkin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:12:50.000000 tonkin-0.0.8/src/tonkin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:12:49.000000 tonkin-0.0.8/src/tonkin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 13:12:50.000000 tonkin-0.0.8/src/tonkin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 13:12:50.000000 tonkin-0.0.8/src/tonkin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:12:50.093029 tonkin-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 13:12:37.000000 tonkin-0.0.8/tests/test_varsec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:56:41.783578 tonkin-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 13:56:06.000000 tonkin-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 13:56:06.000000 tonkin-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 13:56:41.787579 tonkin-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 13:56:06.000000 tonkin-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.771578 tonkin-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.779579 tonkin-0.0.9/src/tonkin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/varsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/src/tonkin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 13:56:06.000000 tonkin-0.0.9/tests/test_varsec.py
```

### Comparing `tonkin-0.0.8/PKG-INFO` & `tonkin-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python template package
 Home-page: https://github.com/HWRacing/tonkin
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/tonkin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tonkin-0.0.8/setup.cfg` & `tonkin-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tonkin
-version = v0.0.8
+version = v0.0.9
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = Python template package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/tonkin
 project_urls =
```

### Comparing `tonkin-0.0.8/src/tonkin/datfile.py` & `tonkin-0.0.9/src/tonkin/datfile.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/datvar.py` & `tonkin-0.0.9/src/tonkin/datvar.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/fixed.py` & `tonkin-0.0.9/src/tonkin/fixed.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/listops.py` & `tonkin-0.0.9/src/tonkin/listops.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 	return output
 
 def splitListIntoLengthsGen(input: List[Any], lengths: int) -> Iterator[List[Any]]:
 	for i in range(0, len(input), lengths):
 		yield input[i:i + lengths]
 
 def splitListIntoLengths(input: List[Any], lengths: int) -> List[Any]:
-	return list(splitListIntoLengths(input, lengths))
+	return list(splitListIntoLengthsGen(input, lengths))
```

### Comparing `tonkin-0.0.8/src/tonkin/packets.py` & `tonkin-0.0.9/src/tonkin/packets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tonkin.datvar
 import tonkin.values
 from typing import List, Dict, Union
 
 def _splitPacket(rawPacket: bytearray, vars: List[tonkin.datvar.Datvar]) -> List[bytearray]:
 	splitPacket = []
 	for var in vars:
-		splitPacket.append(rawPacket[:var.getLength()])
+		splitPacket.append(bytearray(rawPacket[:var.getLength()]))
 		rawPacket = rawPacket[var.getLength():]
 	return splitPacket
 
 def readRawPacket(rawPacket: bytearray, vars: List[tonkin.datvar.Datvar]) -> Dict[str, Union[int, float, bool]]:
 	vals = _splitPacket(rawPacket, vars)
 	packet = {}
 	for index, var in enumerate(vars):
```

### Comparing `tonkin-0.0.8/src/tonkin/parse.py` & `tonkin-0.0.9/src/tonkin/parse.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/values.py` & `tonkin-0.0.9/src/tonkin/values.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/varsec.py` & `tonkin-0.0.9/src/tonkin/varsec.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin/verification.py` & `tonkin-0.0.9/src/tonkin/verification.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/src/tonkin.egg-info/PKG-INFO` & `tonkin-0.0.9/src/tonkin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python template package
 Home-page: https://github.com/HWRacing/tonkin
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/tonkin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tonkin-0.0.8/src/tonkin.egg-info/SOURCES.txt` & `tonkin-0.0.9/src/tonkin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.8/tests/test_varsec.py` & `tonkin-0.0.9/tests/test_varsec.py`

 * *Files identical despite different names*

