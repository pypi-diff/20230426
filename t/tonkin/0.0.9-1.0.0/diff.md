# Comparing `tmp/tonkin-0.0.9.tar.gz` & `tmp/tonkin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonkin-0.0.9.tar", last modified: Wed Apr 26 13:56:41 2023, max compression
+gzip compressed data, was "tonkin-1.0.0.tar", last modified: Wed Apr 26 14:56:52 2023, max compression
```

## Comparing `tonkin-0.0.9.tar` & `tonkin-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:56:41.783578 tonkin-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 13:56:06.000000 tonkin-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 13:56:06.000000 tonkin-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 13:56:41.787579 tonkin-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 13:56:06.000000 tonkin-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.771578 tonkin-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.779579 tonkin-0.0.9/src/tonkin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/datvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/listops.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/varsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 13:56:06.000000 tonkin-0.0.9/src/tonkin/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/src/tonkin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 13:56:41.000000 tonkin-0.0.9/src/tonkin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:56:41.783578 tonkin-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 13:56:06.000000 tonkin-0.0.9/tests/test_varsec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:52.906540 tonkin-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 14:56:52.906540 tonkin-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 14:56:39.000000 tonkin-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 14:56:39.000000 tonkin-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-26 14:56:52.906540 tonkin-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 14:56:39.000000 tonkin-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:52.898540 tonkin-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:52.902540 tonkin-1.0.0/src/tonkin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/datfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/datvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/listops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/varsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-26 14:56:39.000000 tonkin-1.0.0/src/tonkin/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:52.906540 tonkin-1.0.0/src/tonkin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 14:56:52.000000 tonkin-1.0.0/src/tonkin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:56:52.906540 tonkin-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-26 14:56:39.000000 tonkin-1.0.0/tests/test_varsec.py
```

### Comparing `tonkin-0.0.9/PKG-INFO` & `tonkin-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkin
-Version: 0.0.9
+Version: 1.0.0
 Summary: Python template package
 Home-page: https://github.com/HWRacing/tonkin
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/tonkin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tonkin-0.0.9/setup.cfg` & `tonkin-1.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tonkin
-version = v0.0.9
+version = v1.0.0
 author = HWRacing
 author_email = fs60@hw.ac.uk
 description = Python template package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/tonkin
 project_urls =
```

### Comparing `tonkin-0.0.9/src/tonkin/datfile.py` & `tonkin-1.0.0/src/tonkin/datfile.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/datvar.py` & `tonkin-1.0.0/src/tonkin/datvar.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/fixed.py` & `tonkin-1.0.0/src/tonkin/fixed.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/listops.py` & `tonkin-1.0.0/src/tonkin/listops.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/packets.py` & `tonkin-1.0.0/src/tonkin/packets.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/parse.py` & `tonkin-1.0.0/src/tonkin/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,7 +29,17 @@
 	data = readDatFileWithA2L(datFile, a2lFile)
 	headers = data[0].keys()
 	with open(outputFile, "w") as csvFile:
 		writer = csv.DictWriter(csvFile, fieldnames=headers)
 		writer.writeheader()
 		for row in data:
 			writer.writerow(row)
+
+def datTo2DWithA2L(datFile: str, a2lFile: str) -> List[List[Union[int, float, bool]]]:
+	data = readDatFileWithA2L(datFile, a2lFile)
+	headers = list(data[0].keys())
+	output = []
+	output.append(headers)
+	for i in data:
+		row = [i.get(key, "") for key in headers]
+		output.append(row)
+	return output
```

### Comparing `tonkin-0.0.9/src/tonkin/values.py` & `tonkin-1.0.0/src/tonkin/values.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin/varsec.py` & `tonkin-1.0.0/src/tonkin/varsec.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,8 +47,9 @@
 	return output
 
 def getVariableListFromA2L(varSection: bytearray, a2lData: List[Union[mea.Measurement, cha.Characteristic]]) -> List[datvar.Datvar]:
 	defs = splitVarSectionToDefs(varSection)
 	variableNames = extractVariableNames(defs)
 	variableList = getDatVarsFromA2L(variableNames, a2lData)
 	variableList.append(datvar.Datvar("time", "single"))
+	variableList.reverse()
 	return variableList
```

### Comparing `tonkin-0.0.9/src/tonkin/verification.py` & `tonkin-1.0.0/src/tonkin/verification.py`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/src/tonkin.egg-info/PKG-INFO` & `tonkin-1.0.0/src/tonkin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonkin
-Version: 0.0.9
+Version: 1.0.0
 Summary: Python template package
 Home-page: https://github.com/HWRacing/tonkin
 Author: HWRacing
 Author-email: fs60@hw.ac.uk
 Project-URL: Bug Tracker, https://github.com/HWRacing/tonkin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `tonkin-0.0.9/src/tonkin.egg-info/SOURCES.txt` & `tonkin-1.0.0/src/tonkin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tonkin-0.0.9/tests/test_varsec.py` & `tonkin-1.0.0/tests/test_varsec.py`

 * *Files identical despite different names*

