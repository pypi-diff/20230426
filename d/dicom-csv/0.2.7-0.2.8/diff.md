# Comparing `tmp/dicom_csv-0.2.7.tar.gz` & `tmp/dicom_csv-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom_csv-0.2.7.tar", last modified: Wed Feb 22 20:29:46 2023, max compression
+gzip compressed data, was "dicom_csv-0.2.8.tar", last modified: Wed Apr 26 07:38:32 2023, max compression
```

## Comparing `dicom_csv-0.2.7.tar` & `dicom_csv-0.2.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:29:46.144235 dicom_csv-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-22 20:29:46.144235 dicom_csv-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:29:46.144235 dicom_csv-0.2.7/dicom_csv/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/rtstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/dicom_csv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:29:46.144235 dicom_csv-0.2.7/dicom_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 20:29:46.000000 dicom_csv-0.2.7/dicom_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:29:46.144235 dicom_csv-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-02-22 20:29:43.000000 dicom_csv-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/dicom_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/rtstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/dicom_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/setup.py
```

### Comparing `dicom_csv-0.2.7/LICENSE` & `dicom_csv-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/PKG-INFO` & `dicom_csv-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dicom_csv
-Version: 0.2.7
+Version: 0.2.8
 Summary: Utils for gathering, aggregation and handling metadata from DICOM files.
 Home-page: https://github.com/neuro-ml/dicom-csv
 License: MIT
-Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.7.tar.gz
+Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.8.tar.gz
 Keywords: DICOM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dicom_csv-0.2.7/README.md` & `dicom_csv-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/aggregation.py` & `dicom_csv-0.2.8/dicom_csv/aggregation.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/convert.py` & `dicom_csv-0.2.8/dicom_csv/convert.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/crawler.py` & `dicom_csv-0.2.8/dicom_csv/crawler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -106,21 +106,21 @@
             continue
         if value is None:
             continue
 
         if isinstance(value, PERSON_CLASS):
             result[attr] = str(value)
 
+        elif isinstance(value, (int, float, str)):
+            result[attr] = value
+
         elif attr in SERIAL:
             for pos, num in enumerate(value):
                 result[f'{attr}{pos}'] = num
 
-        elif isinstance(value, (int, float, str)):
-            result[attr] = value
-
     return result
 
 
 def join_tree(top: PathLike, ignore_extensions: Sequence[str] = (), relative: bool = True, verbose: int = 0,
               read_pixel_array: bool = False, force: bool = True, unpack_volumetric: bool = True,
               total: bool = False) -> pd.DataFrame:
     """
```

### Comparing `dicom_csv-0.2.7/dicom_csv/interface.py` & `dicom_csv-0.2.8/dicom_csv/interface.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/misc.py` & `dicom_csv-0.2.8/dicom_csv/misc.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/rtstruct.py` & `dicom_csv-0.2.8/dicom_csv/rtstruct.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/scripts.py` & `dicom_csv-0.2.8/dicom_csv/scripts.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/spatial.py` & `dicom_csv-0.2.8/dicom_csv/spatial.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/tags.py` & `dicom_csv-0.2.8/dicom_csv/tags.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv/utils.py` & `dicom_csv-0.2.8/dicom_csv/utils.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/dicom_csv.egg-info/PKG-INFO` & `dicom_csv-0.2.8/dicom_csv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dicom-csv
-Version: 0.2.7
+Version: 0.2.8
 Summary: Utils for gathering, aggregation and handling metadata from DICOM files.
 Home-page: https://github.com/neuro-ml/dicom-csv
 License: MIT
-Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.7.tar.gz
+Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.8.tar.gz
 Keywords: DICOM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dicom_csv-0.2.7/dicom_csv.egg-info/SOURCES.txt` & `dicom_csv-0.2.8/dicom_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/pyproject.toml` & `dicom_csv-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.7/setup.py` & `dicom_csv-0.2.8/setup.py`

 * *Files identical despite different names*

