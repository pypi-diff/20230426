# Comparing `tmp/servicex-2.6.3a1.tar.gz` & `tmp/servicex-2.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex-2.6.3a1.tar", last modified: Tue Apr 25 21:26:35 2023, max compression
+gzip compressed data, was "/home/runner/work/ServiceX_frontend/ServiceX_frontend/dist/.tmp-_ow85y6s/servicex-2.6b1.tar", last modified: Thu Nov 24 14:35:20 2022, max compression
```

## Comparing `servicex-2.6.3a1.tar` & `servicex-2.6b1.tar`

### file list

```diff
@@ -1,35 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:26:35.564077 servicex-2.6.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    25801 2023-04-25 21:26:35.564077 servicex-2.6.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-04-25 21:26:23.000000 servicex-2.6.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:26:35.564077 servicex-2.6.3a1/servicex/
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/ConfigSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/minio_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    44275 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicex.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicex_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicex_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicex_python_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/servicexabc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21389 2023-04-25 21:26:23.000000 servicex-2.6.3a1/servicex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:26:35.564077 servicex-2.6.3a1/servicex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25801 2023-04-25 21:26:35.000000 servicex-2.6.3a1/servicex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-25 21:26:35.000000 servicex-2.6.3a1/servicex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:26:35.000000 servicex-2.6.3a1/servicex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-25 21:26:35.000000 servicex-2.6.3a1/servicex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 21:26:35.000000 servicex-2.6.3a1/servicex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:26:35.564077 servicex-2.6.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-25 21:26:23.000000 servicex-2.6.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:26:35.564077 servicex-2.6.3a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_ConfigSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_minio_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    79191 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_servicex.py
--rw-r--r--   0 runner    (1001) docker     (123)    17877 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_servicex_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_servicex_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_servicexabc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-04-25 21:26:23.000000 servicex-2.6.3a1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/
+-rw-r--r--   0 runner    (1001) docker     (122)    25091 2022-11-24 14:35:20.000000 servicex-2.6b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24217 2022-11-24 14:35:04.000000 servicex-2.6b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/ConfigSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17870 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5775 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9347 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/minio_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42677 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10203 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8121 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2763 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_python_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7266 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/servicexabc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21388 2022-11-24 14:35:04.000000 servicex-2.6b1/servicex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25091 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-24 14:35:20.000000 servicex-2.6b1/servicex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 14:35:20.000000 servicex-2.6b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-11-24 14:35:04.000000 servicex-2.6b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `servicex-2.6.3a1/PKG-INFO` & `servicex-2.6b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex
-Version: 2.6.3a1
+Version: 2.6b1
 Summary: Front-end for the ServiceX Data Server
 Home-page: https://github.com/ssl-hep/ServiceX_frontend
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: TBD
@@ -12,20 +12,18 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # ServiceX Client Library
 
  Client access library for ServiceX
 
@@ -44,15 +42,15 @@
 - [func_adl.uproot](https://github.com/iris-hep/func_adl.uproot) (for flat ntuples)
 - [tcut_to_castle](https://pypi.org/project/tcut-to-qastle/) (translates `TCut` like syntax into a `servicex` query - should work for both)
 
 ## Prerequisites
 
 Before you can use this library you'll need:
 
-- An environment based on python 3.7 or later. 3.11 is highest supported at the moment.
+- An environment based on python 3.6 or later
 - A `ServiceX` end-point. This is usually gotten by logging into and getting approved at the servicex endpoint. Once you do that, you'll have an API token, which this library needs to access the `ServiceX` endpoint, and the web address where you got that token (the `endpoint` address).
 
 ### How to access your endpoint
 
 The API access information is normally placed in a configuration file (see the section below). Create a config file, `servicex.yaml`, in the `yaml` format, in the appropriate place for your work that contains the following (for the `xaod` backend; use `uproot` for the `type` for the uproot backend):
 
 ```yaml
@@ -217,18 +215,14 @@
   - Windows: `cache_path: "C:\\Users\\gordo\\Desktop\\cacheme"`
   - Linux: `cache_path: "/home/servicex-cache"`
 
 - `backend_types` - a list of yaml dictionaries that contains some defaults for the backends. By default only the `return_data` is there, which for `xaod` is `root` and `uproot` is `parquet`. There is also a `cms_run1_aod` which returns `root`. Allows `servicex` to convert to `pandas.DataFrame` or `awkward` if requested by the user.
 
 All strings are expanded using python's [os.path.expand](https://docs.python.org/3/library/os.path.html#os.path.expandvars) method - so `$NAME` and `${NAME}` will work to expand existing environment variables.
 
-For non-standard use cases, the user can specify:
-- The code generator that is used by the backend. This is done by passing a `codegen` argument to ServiceXDataset. This argument is normally inherited from the backend type set in `servicex.yaml`, but can be overridden with any valid `codegen` contained in the default type listing. A `codegen` entry can also be added to a backend in the yaml file to use as default.
-- The type of backend, using the `backend_type` argument on ServiceXDataset. This overrides the backend type setting in the `servicex.yaml` file.
-
 ## Features
 
 Implemented:
 
 - Accepts a `qastle` formatted query
 - Exceptions are used to report back errors of all sorts from the service to the user's code.
 - Data is return in the following forms:
@@ -247,15 +241,15 @@
   into repositories.
 
 ## Testing
 
 This code has been tested in several environments:
 
 - Windows, Linux, MacOS
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.6, 3.7, 3.8
 - Jupyter Notebooks (not automated), regular python command-line invoked source files
 
 ### Non-standard backends
 
 When doing backend development, often ports 9000 and 5000 are forwarded to the local machine exposing the `minio` and `ServiceX_App` instances. In that case, you'll need to create a configuration file that has `http://localhost:5000` as the end point. No API token is necessary if the development `ServiceX` instance doesn't have authorization turned on.
 
 ## API
```

### Comparing `servicex-2.6.3a1/README.md` & `servicex-2.6b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - [func_adl.uproot](https://github.com/iris-hep/func_adl.uproot) (for flat ntuples)
 - [tcut_to_castle](https://pypi.org/project/tcut-to-qastle/) (translates `TCut` like syntax into a `servicex` query - should work for both)
 
 ## Prerequisites
 
 Before you can use this library you'll need:
 
-- An environment based on python 3.7 or later. 3.11 is highest supported at the moment.
+- An environment based on python 3.6 or later
 - A `ServiceX` end-point. This is usually gotten by logging into and getting approved at the servicex endpoint. Once you do that, you'll have an API token, which this library needs to access the `ServiceX` endpoint, and the web address where you got that token (the `endpoint` address).
 
 ### How to access your endpoint
 
 The API access information is normally placed in a configuration file (see the section below). Create a config file, `servicex.yaml`, in the `yaml` format, in the appropriate place for your work that contains the following (for the `xaod` backend; use `uproot` for the `type` for the uproot backend):
 
 ```yaml
@@ -190,18 +190,14 @@
   - Windows: `cache_path: "C:\\Users\\gordo\\Desktop\\cacheme"`
   - Linux: `cache_path: "/home/servicex-cache"`
 
 - `backend_types` - a list of yaml dictionaries that contains some defaults for the backends. By default only the `return_data` is there, which for `xaod` is `root` and `uproot` is `parquet`. There is also a `cms_run1_aod` which returns `root`. Allows `servicex` to convert to `pandas.DataFrame` or `awkward` if requested by the user.
 
 All strings are expanded using python's [os.path.expand](https://docs.python.org/3/library/os.path.html#os.path.expandvars) method - so `$NAME` and `${NAME}` will work to expand existing environment variables.
 
-For non-standard use cases, the user can specify:
-- The code generator that is used by the backend. This is done by passing a `codegen` argument to ServiceXDataset. This argument is normally inherited from the backend type set in `servicex.yaml`, but can be overridden with any valid `codegen` contained in the default type listing. A `codegen` entry can also be added to a backend in the yaml file to use as default.
-- The type of backend, using the `backend_type` argument on ServiceXDataset. This overrides the backend type setting in the `servicex.yaml` file.
-
 ## Features
 
 Implemented:
 
 - Accepts a `qastle` formatted query
 - Exceptions are used to report back errors of all sorts from the service to the user's code.
 - Data is return in the following forms:
@@ -220,15 +216,15 @@
   into repositories.
 
 ## Testing
 
 This code has been tested in several environments:
 
 - Windows, Linux, MacOS
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.6, 3.7, 3.8
 - Jupyter Notebooks (not automated), regular python command-line invoked source files
 
 ### Non-standard backends
 
 When doing backend development, often ports 9000 and 5000 are forwarded to the local machine exposing the `minio` and `ServiceX_App` instances. In that case, you'll need to create a configuration file that has `http://localhost:5000` as the end point. No API token is necessary if the development `ServiceX` instance doesn't have authorization turned on.
 
 ## API
```

### Comparing `servicex-2.6.3a1/servicex/ConfigSettings.py` & `servicex-2.6b1/servicex/ConfigSettings.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/__init__.py` & `servicex-2.6b1/servicex/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/cache.py` & `servicex-2.6b1/servicex/cache.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/config_default.yaml` & `servicex-2.6b1/servicex/config_default.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,14 @@
   - endpoint: http://localhost:5000
     name: default
     type: xaod
     # token: xxx
   - endpoint: http://localhost:5000
     name: default
     type: cms_run1_aod
-  - endpoint: http://localhost:5000
-    name: default
-    type: uproot
 
 # This is the path of the cache. The "/tmp" will be translated, platform appropriate, and
 # the env variable USER will be replaced.
 cache_path: /tmp/servicex_${USER}
 
 # This is a dummy value, here only to make sure that unit testing
 # works properly before package release.
@@ -26,18 +23,12 @@
 # xaod backend.
 default_return_data: parquet
 
 # Defaults for the various types of servicex backends that we might deal with.
 # Easy enough to add a new one here...
 backend_types:
   - type: xaod
-    return_data: root-file
-    codegen: atlasxaod
+    return_data: root
   - type: uproot
     return_data: parquet
-    codegen: uproot
   - type: cms_run1_aod
-    return_data: root-file
-    codegen: cms
-  - type: python
-    return_data: parquet
-    codegen: python
+    return_data: root
```

### Comparing `servicex-2.6.3a1/servicex/data_conversions.py` & `servicex-2.6b1/servicex/data_conversions.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
         Args:
             default_file_type (str): The default file type (`parquet` or `root`)
         """
         self._default_file_type = default_file_type
 
     async def convert_to_pandas(self, file: Path, file_type: Optional[str] = None):
-        """Convert to a pandas DataFrame from data stored in a file of a particular file_type
+        """Convert to a pandas dataframe from data stored in a file of a particular file_type
 
         Args:
             file (Path): Path to the file
             file_type (str): What the file contains (root, parquet, etc)
         """
         file_type = file_type if file_type is not None else self._default_file_type
-        if file_type == "root-file":
+        if file_type == "root":
             return await self._convert_root_to_pandas(file)
         elif file_type == "parquet":
             return await self._convert_parquet_to_pandas(file)
         else:
             raise ServiceXException(
                 f"Conversion from {file_type} into an pandas DF is not " "yet supported"
             )
@@ -44,29 +44,29 @@
         """Convert to an awkward data array from data stored in a file of a particular file_type
 
         Args:
             file (Path): Path to the file
             file_type (str): What the file contains (root, parquet, etc)
         """
         file_type = file_type if file_type is not None else self._default_file_type
-        if file_type == "root-file":
+        if file_type == "root":
             return await self._convert_root_to_awkward(file)
         elif file_type == "parquet":
             return await self._convert_parquet_to_awkward(file)
         else:
             raise ServiceXException(
                 f"Conversion from {file_type} into an awkward array is not "
                 "yet supported"
             )
 
     def combine_pandas(self, dfs: Iterable[pd.DataFrame]) -> pd.DataFrame:
-        """Combine many pandas DataFrame into a single one, in order.
+        """Combine many pandas dataframes into a single one, in order.
 
         Args:
-            dfs (Iterable[pd.DataFrame]): The list of DataFrames
+            dfs (Iterable[pd.DataFrame]): The list of dataframes
         """
         return pd.concat(dfs)
 
     def combine_awkward(self, awks: Iterable[ak.Array]) -> ak.Array:
         """Combine many awkward arrays into a single one, in order.
 
         Args:
@@ -80,15 +80,15 @@
 
         Arguments:
 
             file        A `Path` to the file containing the pandas data
 
         Returns:
 
-            DataFrame   A pandas DataFrame
+            DataFrame   A pandas dataframe
 
         Note:
 
             - Work is done on a second thread.
             - Pandas is only imported if this is called.
 
         """
@@ -109,15 +109,15 @@
 
         Arguments:
 
             file        A `Path` to the file containing the pandas data
 
         Returns:
 
-            DataFrame   A pandas DataFrame
+            DataFrame   A pandas dataframe
 
         Note:
 
             - Work is done on a second thread.
             - Pandas is only imported if this is called.
 
         """
@@ -134,22 +134,22 @@
 
         Arguments:
 
             file        A `Path` to the file containing the pandas data
 
         Returns:
 
-            DataFrame   A pandas DataFrame
+            DataFrame   A pandas dataframe
 
         Note:
 
             - Work is done on a second thread.
             - Awkward is only imported if this is called.
             - A LazyArray is returned, so it isn't completely loaded into memory. That also means
-              this will leak file handles - as that has to be left open.
+              this will leak filehandles - as that has to be left open.
 
         """
 
         def do_the_work(file: Path) -> ak.Array:
             import uproot as uproot
 
             with uproot.open(file) as f_in:
@@ -165,15 +165,15 @@
 
         Arguments:
 
             file        A `Path` to the file containing the pandas data
 
         Returns:
 
-            DataFrame   A pandas DataFrame
+            DataFrame   A pandas dataframe
 
         Note:
 
             - Work is done on a second thread.
             - Pandas is only imported if this is called.
 
         """
```

### Comparing `servicex-2.6.3a1/servicex/minio_adaptor.py` & `servicex-2.6b1/servicex/minio_adaptor.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/servicex.py` & `servicex-2.6b1/servicex/servicex.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,14 @@
     get_configured_cache_path,
     log_adaptor,
     on_exception_itr,
     stream_status_updates,
     stream_unique_updates_only,
 )
 
-# The allowed file formats.
-# You could modify this if you wanted to add new...
-g_allowed_formats = ["parquet", "root-file"]
-
 
 class StreamInfoBase:
     """Contains base information about results that are streamed back from
     ServiceX.
     """
 
     def __init__(self, file: str):
@@ -102,15 +98,15 @@
         Returns:
             str: The URL of the transformed data for this file.
         """
         return self._url
 
     @property
     def bucket(self) -> str:
-        """Returns the buck name - unique and constant across transformations.
+        """Returns the buck name - unique and constant accross transformations.
         Can be used to order the results
 
         Returns:
             str: The bucket name as produced by ServiceX
         """
         return self._bucket
 
@@ -162,25 +158,23 @@
             Any: The ServiceX transformed data for this file.
         """
         return self._data
 
 
 class ServiceXDataset(ServiceXABC):
     """
-    Used to access an instance of ServiceX at an end point on the internet. Support conversion
+    Used to access an instance of ServiceX at an end point on the internet. Support convieration
     by configuration object `config_adaptor` or by creating the adaptors defined in the `__init__`
     function.
     """
 
     def __init__(
         self,
         dataset: DatasetType,
         backend_name: Optional[str] = None,
-        backend_type: Optional[str] = None,
-        codegen: Optional[str] = None,
         image: Optional[str] = None,
         max_workers: int = 20,
         result_destination: str = "object-store",
         servicex_adaptor: Optional[ServiceXAdaptor] = None,
         minio_adaptor: Optional[Union[MinioAdaptor, MinioAdaptorFactory]] = None,
         cache_adaptor: Optional[Cache] = None,
         status_callback_factory: Optional[StatusUpdateFactory] = _run_default_wrapper,
@@ -199,31 +193,24 @@
 
             dataset                     Name of a dataset from which queries will be selected.
             backend_name                The type of backend. Used only if we need to find an
                                         end-point. If we do not have a `servicex_adaptor` then this
                                         will default to xaod, unless you have any endpoint listed
                                         in your servicex file. It will default to best match there,
                                         or fail if a name has been given.
-            backend_type                The type of backend. Overrides the `type` in the `yaml`
-                                        config file.
-            codegen                     The type of code generator passed to the backend to
-                                        generate the code that powers the requested transform.
-                                        Don't use unless you know what you are doing - sometimes
-                                        the return filetype is also needed. Better to use
-                                        `backend_type`!
             image                       Name of transformer image to use to transform the data. If
                                         left as default, `None`, then the default image for the
                                         ServiceX backend will be used.
             max_workers                 Maximum number of transformers to run simultaneously on
                                         ServiceX.
             result_destination          Where the transformers should write the results.
                                         Defaults to object-store, but could be used to save
                                         results to a posix volume
             servicex_adaptor            Object to control communication with the servicex instance
-                                        at a particular ip address with certain login credentials.
+                                        at a particular ip address with certian login credentials.
                                         Will be configured via the `config_adaptor` by default.
             minio_adaptor               Object to control communication with the minio servicex
                                         instance.
             cache_adaptor               Runs the caching for data and queries that are sent up and
                                         down.
             status_callback_factory     Factory to create a status notification callback for each
                                         query. One is created per query.
@@ -251,15 +238,14 @@
                be processed (and some files can even be completed before that is known).
             -  The full description of calling parameters is recorded in the local cache, including
                things like `image` name and tag.
         """
         ServiceXABC.__init__(
             self,
             dataset,
-            codegen,
             image,
             max_workers,
             result_destination,
             status_callback_factory,
         )
 
         # Get the local settings
@@ -278,17 +264,15 @@
             )
             if cache_adaptor is None
             else cache_adaptor
         )
 
         if not servicex_adaptor:
             # Given servicex adaptor is none, this should be ok. Fixes type checkers
-            end_point, token = config.get_servicex_adaptor_config(
-                backend_name, backend_type=backend_type
-            )
+            end_point, token = config.get_servicex_adaptor_config(backend_name)
             servicex_adaptor = ServiceXAdaptor(end_point, token)
         self._servicex_adaptor = servicex_adaptor
 
         if not minio_adaptor:
             self._minio_adaptor = MinioAdaptorFactory()
         else:
             if isinstance(minio_adaptor, MinioAdaptor):
@@ -300,32 +284,21 @@
 
         self._session_generator = (
             session_generator
             if session_generator is not None
             else default_client_session
         )
 
-        self._return_types = [
-            config.get_default_returned_datatype(
-                backend_name, backend_type=backend_type
-            )
-        ]
+        self._return_types = [config.get_default_returned_datatype(backend_name)]
         self._converter = (
             data_convert_adaptor
             if data_convert_adaptor is not None
             else DataConverterAdaptor(self._return_types[0])
         )
 
-        # TODO - this should not be in the ABC backend since we have to have some intelligence
-        # in setting it, it turns out.
-        if self._codegen is None:
-            self._codegen = config.get_backend_info(
-                backend_name, "codegen", backend_type=backend_type
-            )
-
     def first_supported_datatype(
         self, datatypes: Union[List[str], str]
     ) -> Optional[str]:
         """Return the first datatype format that this dataset/servicex instance can return.
 
         Different instances of `ServiceX` are capable of returning different datatypes. Pass in
         the datatypes that your app supports, and this will return the first one that the servicex
@@ -343,16 +316,16 @@
         for dt in datatypes:
             if dt in self._return_types:
                 return dt
 
         return None
 
     def ignore_cache(self):
-        """Return a context manager that, as long as it is held, will cause any queries against
-        just this dataset to ignore any locally cached data.
+        """Return a context manager that, as long as it is held, will cause any queries against just
+        this dataset to ignore any locally cached data.
 
         Returns:
             ContextManager: As long as this is held, the local query cache will be ignored.
         """
         return self._cache.ignore_cache()
 
     @functools.wraps(ServiceXABC.get_data_rootfiles_async, updated=())
@@ -366,24 +339,24 @@
         self, selection_query: str, title: Optional[str] = None
     ) -> AsyncIterator[StreamInfoPath]:
         """Returns, as an async iterator, each completed batch of work from Servicex.
         The `StreamInfoPath` contains a path where downstream consumers can directly
         access the data.
 
         Args:
-            selection_query (str): The `qastle` query for the data to retrieve.
+            selection_query (str): The `qastle` query for the data to retreive.
 
         Yields:
             AsyncIterator[StreamInfoPath]: As ServiceX completes the data, and it is downloaded
                                            to the local machine, the async iterator returns
                                            a `StreamInfoPath` which can be used to access the
                                            file locally.
         """
         async for f_info in self._stream_local_files(
-            selection_query, title, "root-file"
+            selection_query, title, "root-files"
         ):  # type: ignore
             yield f_info
 
     @functools.wraps(ServiceXABC.get_data_parquet_async, updated=())
     @_wrap_in_memory_sx_cache
     async def get_data_parquet_async(
         self, selection_query: str, title: Optional[str] = None
@@ -394,15 +367,15 @@
         self, selection_query: str, title: Optional[str] = None
     ) -> AsyncIterator[StreamInfoPath]:
         """Returns, as an async iterator, each completed batch of work from Servicex.
         The `StreamInfoPath` contains a path where downstream consumers can directly
         access the data.
 
         Args:
-            selection_query (str): The `qastle` query for the data to retrieve.
+            selection_query (str): The `qastle` query for the data to retreive.
 
         Yields:
             AsyncIterator[StreamInfoPath]: As ServiceX completes the data, and it is downloaded
                                            to the local machine, the async iterator returns
                                            a `StreamInfoPath` which can be used to access the
                                            file locally.
         """
@@ -412,47 +385,39 @@
             yield f_info
 
     @functools.wraps(ServiceXABC.get_data_pandas_df_async, updated=())
     @_wrap_in_memory_sx_cache
     async def get_data_pandas_df_async(
         self, selection_query: str, title: Optional[str] = None
     ):
-        data_format = self._return_types[0]
         return self._converter.combine_pandas(
             await self._data_return(
-                selection_query,
-                lambda f: self._converter.convert_to_pandas(f),
-                title,
-                data_format=data_format,
+                selection_query, lambda f: self._converter.convert_to_pandas(f), title
             )
         )
 
     @functools.wraps(ServiceXABC.get_data_awkward_async, updated=())
     @_wrap_in_memory_sx_cache
     async def get_data_awkward_async(
         self, selection_query: str, title: Optional[str] = None
     ):
-        data_format = self._return_types[0]
         return self._converter.combine_awkward(
             await self._data_return(
-                selection_query,
-                lambda f: self._converter.convert_to_awkward(f),
-                title,
-                data_format=data_format,
+                selection_query, lambda f: self._converter.convert_to_awkward(f), title
             )
         )
 
     async def get_data_awkward_stream(
         self, selection_query: str, title: Optional[str] = None
     ) -> AsyncGenerator[StreamInfoData, None]:
         """Returns, as an async iterator, each completed batch of work from Servicex
         as a separate `awkward` array. The data is returned in a `StreamInfoData` object.
 
         Args:
-            selection_query (str): The `qastle` query for the data to retrieve.
+            selection_query (str): The `qastle` query for the data to retreive.
 
         Yields:
             AsyncIterator[StreamInfoData]: As ServiceX completes the data, and it is downloaded
                                            to the local machine, the async iterator returns
                                            a `StreamInfoData` which can be used to access the
                                            data that has been loaded from the file.
         """
@@ -464,15 +429,15 @@
     async def get_data_pandas_stream(
         self, selection_query: str, title: Optional[str] = None
     ) -> AsyncGenerator[StreamInfoData, None]:
         """Returns, as an async iterator, each completed batch of work from Servicex
         as a separate `pandas.DataFrame` array. The data is returned in a `StreamInfoData` object.
 
         Args:
-            selection_query (str): The `qastle` query for the data to retrieve.
+            selection_query (str): The `qastle` query for the data to retreive.
 
         Yields:
             AsyncIterator[StreamInfoData]: As ServiceX completes the data, and it is downloaded
                                            to the local machine, the async iterator returns
                                            a `StreamInfoData` which can be used to access the
                                            data that has been loaded from the file.
         """
@@ -493,15 +458,15 @@
 
         Args:
             selection_query (str): The ServiceX Selection
             title (str): Optional title for transform request
             as_signed_url (bool): Return the uri as a presigned http url?
         """
         async for f_info in self._stream_url_buckets(
-            selection_query, "root-file", title, as_signed_url
+            selection_query, "root-files", title, as_signed_url
         ):  # type: ignore
             yield f_info
 
     async def get_data_rootfiles_uri_async(
         self,
         selection_query: str,
         title: Optional[str] = None,
@@ -566,15 +531,15 @@
     async def _file_return(
         self, selection_query: str, data_format: str, title: Optional[str]
     ):
         """
         Given a query, return the list of files, in a unique order, that hold
         the data for the query.
 
-        For certain types of exceptions, the queries will be repeated. For example,
+        For certian types of exceptions, the queries will be repeated. For example,
         if `ServiceX` indicates that it was restarted in the middle of the query, then
         the query will be re-submitted.
 
         Arguments:
 
             selection_query     `qastle` data that makes up the selection request.
             data_format         The file-based data format (root or parquet)
@@ -622,14 +587,15 @@
                                            The dict will have entries for:
                                              bucket: The minio bucket name
                                              file: the completed file in the bucket
         """
         query = self._build_json_query(selection_query, data_format, title)
 
         async with aiohttp.ClientSession() as client:
+
             # Get a request id - which might be cached, but if not, submit it.
             request_id = await self._get_request_id(client, query)
 
             # Make sure cache status exists (user could have deleted, see #176)
             if not self._cache.query_status_exists(request_id):
                 await self._update_query_status(client, request_id)
 
@@ -697,15 +663,15 @@
         converter: Callable[[Path], Awaitable[Any]],
         title: Optional[str],
         data_format: str = "root-file",
     ) -> List[Any]:
         """Given a query, return the data, in a unique order, that hold
         the data for the query.
 
-        For certain types of exceptions, the queries will be repeated. For example,
+        For certian types of exceptions, the queries will be repeated. For example,
         if `ServiceX` indicates that it was restarted in the middle of the query, then
         the query will be re-submitted.
 
         Arguments:
 
             selection_query     `qastle` data that makes up the selection request.
             converter           A `Callable` that will convert the data returned from
@@ -737,15 +703,15 @@
         title: Optional[str],
         converter: Callable[[Path], Awaitable[Any]],
         data_format: str = "root-file",
     ) -> AsyncIterator[StreamInfoData]:
         """Given a query, return the data, in the order it arrives back
         converted as appropriate.
 
-        For certain types of exceptions, the queries will be repeated. For example,
+        For certian types of exceptions, the queries will be repeated. For example,
         if `ServiceX` indicates that it was restarted in the middle of the query, then
         the query will be re-submitted.
 
         Arguments:
 
             selection_query     `qastle` data that makes up the selection request.
             converter           A `Callable` that will convert the data returned from
@@ -768,15 +734,15 @@
         self, selection_query: str, title: Optional[str], data_format: str = "root-file"
     ) -> AsyncGenerator[StreamInfoPath, None]:
         """
         Given a query, return the data as a list of paths pointing to local files
         that contain the results of the query. This is an async generator, and files
         are returned as they arrive.
 
-        For certain types of exceptions, the queries will be repeated. For example,
+        For certian types of exceptions, the queries will be repeated. For example,
         if `ServiceX` indicates that it was restarted in the middle of the query, then
         the query will be re-submitted.
 
         Arguments:
 
             selection_query     `qastle` data that makes up the selection request.
 
@@ -798,59 +764,60 @@
 
         async for name, a_path in as_files:
             yield StreamInfoPath(name, Path(await a_path))
 
     async def _get_files(
         self,
         selection_query: str,
-        data_format: str,
+        data_type: str,
         notifier: _status_update_wrapper,
         title: Optional[str],
     ) -> AsyncIterator[Tuple[str, Awaitable[Path]]]:
         """
         Return a list of files from servicex as they have been downloaded to this machine. The
         return type is an awaitable that will yield the path to the file.
 
-        For certain types of `ServiceX` failures we will automatically attempt a few retries:
+        For certian types of `ServiceX` failures we will automatically attempt a few retries:
 
             - When `ServiceX` forgets the query. This sometimes happens when a user submits a
               query, and then disconnects from the network, `ServiceX` is restarted, and then the
               user attempts to download the files from that "no-longer-existing" request.
 
         Up to 3 re-tries are attempted automatically.
 
         Arguments:
 
             selection_query             The query string to send to ServiceX
-            data_format                 The type of data that we want to come back.
+            data_type                   The type of data that we want to come back.
             notifier                    Status callback to let our progress be advertised
             title                       Title to pass to servicex backend.
 
         Returns
             Awaitable[Path]             An awaitable that is a path. When it completes, the
                                         path will be valid and point to an existing file.
                                         This is returned this way so a number of downloads can run
                                         simultaneously.
         """
-        query = self._build_json_query(selection_query, data_format, title)
+        query = self._build_json_query(selection_query, data_type, title)
 
         async with aiohttp.ClientSession() as client:
+
             # Get a request id - which might be cached, but if not, submit it.
             request_id = await self._get_request_id(client, query)
 
             # Make sure cache status exists (user could have deleted, see #176)
             if not self._cache.query_status_exists(request_id):
                 await self._update_query_status(client, request_id)
 
             # Get the minio adaptor we are going to use for downloading.
             minio_adaptor = self._minio_adaptor.from_best(
                 self._cache.lookup_query_status(request_id)
             )
 
-            # Look up the cache, and then fetch an iterator going through the results
+            # Look up the cache, and then fetch an iterator going thorugh the results
             # from either servicex or the cache, depending.
             try:
                 cached_files = self._cache.lookup_files(request_id)
                 stream_local_files = (
                     self._get_cached_files(cached_files, notifier)
                     if cached_files is not None
                     else self._get_files_from_servicex(
@@ -979,14 +946,15 @@
         """
         Fetch query result files from `servicex`. Given the `request_id` we will download
         files as they become available. We also coordinate caching.
         """
         start_time = time.monotonic()
         good = True
         try:
+
             # Get the stream of minio bucket new files.
             stream_new_object = self._get_minio_bucket_files_from_servicex(
                 request_id, client, minio_adaptor, notifier
             )
 
             # Next, download the files as they are found (and return them):
             stream_downloaded = self._download_a_file(
@@ -1035,14 +1003,15 @@
                                                back to the user
 
         Yields:
             [type]: Returns xxx and yyy.
         """
         start_time = time.monotonic()
         try:
+
             # Setup the status sequence from servicex
             stream_status = transform_status_stream(
                 self._servicex_adaptor, client, request_id
             )
             stream_notified = stream_status_updates(stream_status, notifier)
             stream_watched = trap_servicex_failures(stream_notified)
             stream_unique = stream_unique_updates_only(stream_watched)
@@ -1061,38 +1030,33 @@
             run_time = timedelta(seconds=end_time - start_time)
             logging.getLogger(__name__).info(
                 f"Running servicex query for "
                 f"{request_id} took {run_time} (no files downloaded)"
             )
 
     def _build_json_query(
-        self, selection_query: str, data_format: str, title: Optional[str]
+        self, selection_query: str, data_type: str, title: Optional[str]
     ) -> Dict[str, Union[str, Iterable[str]]]:
         """
         Returns a list of locally written files for a given selection query.
 
         Arguments:
             selection_query         The query to be send into the ServiceX API
-            data_format             What is the output data type (parquet, root-file, etc.)
+            data_type               What is the output data type (parquet, root-file, etc.)
 
         Notes:
             - Internal routine.
         """
-        assert data_format in g_allowed_formats
-
         # Items that must always be present
-        codegen = self._codegen if self._codegen is not None else "default"
-
         json_query: Dict[str, Union[str, Iterable[str]]] = {
             "selection": selection_query,
             "result-destination": self._result_destination,
-            "result-format": data_format,
+            "result-format": "parquet" if data_type == "parquet" else "root-file",
             "chunk-size": "1000",
             "workers": str(self._max_workers),
-            "codegen": codegen,
         }
 
         # Add the appropriate did.
         # Capture full did as well as single item files (see  #178)
         if isinstance(self._dataset, str):
             if self._dataset[0:7].lower() in ["root://", "http://"]:
                 json_query["file-list"] = [self._dataset]
```

### Comparing `servicex-2.6.3a1/servicex/servicex_adaptor.py` & `servicex-2.6b1/servicex/servicex_adaptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from datetime import datetime
 from typing import AsyncIterator, Dict, Optional, Tuple
 import logging
 
 import aiohttp
 from google.auth import jwt
-import os
+
 from .utils import (
     ServiceXException,
     ServiceXFailedFileTransform,
     ServiceXFatalTransformException,
     ServiceXUnknownRequestID,
     TransformTuple,
 )
@@ -38,28 +38,15 @@
                 j = await response.json()
                 self._token = j["access_token"]
             else:
                 raise ServiceXException(
                     f"ServiceX access token request rejected: {status}"
                 )
 
-    def _get_bearer_token_file(self):
-        bearer_token_file = os.environ.get('BEARER_TOKEN_FILE')
-        bearer_token = None
-        if bearer_token_file:
-            with open(bearer_token_file, "r") as f:
-                bearer_token = f.read().strip()
-        print("BEARER", bearer_token)
-        return bearer_token
-
     async def _get_authorization(self, client: aiohttp.ClientSession):
-        bearer_token = self._get_bearer_token_file()
-        if bearer_token:
-            self._coffea_casa_bearer_token = bearer_token
-            return {"Authorization": f"Bearer {self._coffea_casa_bearer_token}"}
         if not self._refresh_token:
             return {}
         now = datetime.utcnow().timestamp()
         if not self._token or jwt.decode(self._token, verify=False)["exp"] - now < 0:
             await self._get_token(client)
         return {"Authorization": f"Bearer {self._token}"}
```

### Comparing `servicex-2.6.3a1/servicex/servicex_config.py` & `servicex-2.6b1/servicex/servicex_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     things the user has given us and program parameters. This concentrates all the complex config
     logic in on place, and, hopefully, leaves the logic out of all the other code.
     """
 
     def __init__(self, config: Optional[ConfigView] = None):
         """The config needed for the app.
 
-        Note: The config is held onto and only queried when the information is required.
+        Note: The config is held onto and only queired when the information is required.
 
         Args:
             config (ConfigView): The config information for the app. If null, then we just use the
                                  standard servicex name.
         """
         self._settings = (
             config if config is not None else ConfigSettings("servicex", "servicex")
@@ -33,59 +33,50 @@
         Eventually this should not be used other than for testing!
 
         Returns:
             ConfigSettings: The config settings that gives us a view on everything the user wants
         """
         return self._settings
 
-    def get_default_returned_datatype(
-        self, backend_name: Optional[str], backend_type: Optional[str] = None
-    ) -> str:
-        """Return the default return data type, given the backend is a certain type.
+    def get_default_returned_datatype(self, backend_name: Optional[str]) -> str:
+        """Return the default return data type, given the backend is a certian type.
 
         Args:
             backend_name (Optional[str]): The backend type string (`xaod`, `uproot`, etc)
 
         Returns:
             str: The backend datatype, like `root` or `parquet`.
         """
         # Check to see if we know about the backend info
-        r = self.get_backend_info(
-            backend_name, "return_data", backend_type=backend_type
-        )
+        r = self.get_backend_info(backend_name, "return_data")
 
         if r is None:
             raise ServiceXException(
                 "A default default_return_data is missing from config files "
                 "- is servicex installed correctly?"
             )
 
         return r
 
-    def get_backend_info(
-        self, backend_name: Optional[str], key: str, backend_type: Optional[str] = None
-    ) -> Optional[str]:
+    def get_backend_info(self, backend_name: Optional[str], key: str) -> Optional[str]:
         """Find an item in the backend info, searching first for the backend
         name/type and then the defaults with a given type.
 
         Args:
             backend_name (str): Backend name
             key (str): The key for the info we are after
-            backend_type (str): The backend type, if we are overriding normal lookup
 
         Returns:
             Optional[str]: Return a string for the info we are after, or return None if we can't
                            find it.
         """
-        config = self._get_backend_info(backend_name, backend_type)
+        config = self._get_backend_info(backend_name)
         return config[key] if key in config else None
 
-    def _get_backend_info(
-        self, backend_name: Optional[str], backend_type: Optional[str]
-    ) -> Dict[str, str]:
+    def _get_backend_info(self, backend_name: Optional[str]) -> Dict[str, str]:
         """Returns all the info for a backend name/type.
 
         Search algorithm is non-trivial:
         1. If `backend_name` is not `None`:
            1. Look at the `api_endpoints` for a `name` matching `backend_name`.
            2. Look at the `api_endpoints` for a `type` matching `backend_name`,
               complain that `name` wasn't present.
@@ -94,16 +85,14 @@
            1. Use the first end point in the list, and complain.
 
         Given the above is done, then look at `backend_types` for a matching `type`,
         and for any key found there not already present, add it, and return the dictionary.
 
         Args:
             backend_name (str): Name or type of the api end point we are going to look up.
-            backend_type (str): Override the backend type, if we are looking for a specific
-                                type behavior.
 
         Returns:
             Dict[str, str]: Attributes for this backend's configuration
         """
         # Find a list of all endpoints.
         # It is an error if this is not specified somewhere.
         endpoints = self.settings["api_endpoints"]
@@ -166,22 +155,16 @@
             # If we are here - then... it just isn't going to work!
             raise ServiceXException(
                 "Not even a default set of configurations are here! Bad "
                 " install of the servicex package!"
             )
 
         # Now, extract the type and see if we can figure out any defaults from the
-        # `backend_types` info. Skip this if we have a type we are passed in.
-        type_lookup = (
-            backend_type
-            if backend_type is not None
-            else config["type"]
-            if "type" in config
-            else backend_name
-        )
+        # `backend_types` info.
+        type_lookup = config["type"] if "type" in config else backend_name
         if type_lookup is None:
             return config
 
         backend_defaults = self.settings["backend_types"]
         for bd in backend_defaults:
             if bd["type"].as_str_expanded() == type_lookup:
                 for k in bd.keys():
@@ -194,28 +177,26 @@
                 config["return_data"] = str(
                     self.settings["default_return_data"].as_str_expanded()
                 )
 
         return config
 
     def get_servicex_adaptor_config(
-        self,
-        backend_name: Optional[str] = None,
-        backend_type: Optional[str] = None,
+        self, backend_name: Optional[str] = None
     ) -> Tuple[str, Optional[str]]:
         """Return the servicex (endpoint, token) from a given backend configuration.
 
         Args:
             backend_name (str): The backend name (like `xaod`) which we hopefully can find in the
             configuration file.
 
         Returns:
             Tuple[str, str]: The tuple of info to create a `ServiceXAdaptor`: end point,
             token (optionally).
         """
-        config = self._get_backend_info(backend_name, backend_type)
+        config = self._get_backend_info(backend_name)
 
         endpoint = config["endpoint"]
         token = config["token"] if "token" in config else None
 
         # We can default these to "None"
         return (endpoint, token)  # type: ignore
```

### Comparing `servicex-2.6.3a1/servicex/servicex_python_function.py` & `servicex-2.6b1/servicex/servicex_python_function.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/servicex_utils.py` & `servicex-2.6b1/servicex/servicex_utils.py`

 * *Files identical despite different names*

### Comparing `servicex-2.6.3a1/servicex/servicexabc.py` & `servicex-2.6b1/servicex/servicexabc.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,25 @@
     with ServiceX file access, including the dataset name. Subclasses implement the various access
     methods. Note that not all methods may be accessible!
     """
 
     def __init__(
         self,
         dataset: DatasetType,
-        codegen: Optional[str] = None,
         image: Optional[str] = None,
         max_workers: int = 20,
         result_destination: str = "object-store",
         status_callback_factory: Optional[StatusUpdateFactory] = _run_default_wrapper,
     ):
         """
         Create and configure a ServiceX object for a dataset.
 
         Arguments
 
             dataset                     Name of a dataset from which queries will be selected.
-            codegen                     The type of code generator passed to the backend to
-                                        generate the code that powers the requested transform.
             image                       Name of transformer image to use to transform the data. If
                                         None the default implementation is used.
             cache_adaptor               Runs the caching for data and queries that are sent up and
                                         down.
             max_workers                 Maximum number of transformers to run simultaneously on
                                         ServiceX.
             result_destination          Where the transformers should write the results.
@@ -64,15 +61,14 @@
                jupyter extensions installed). If `status_callback` is specified as None, no
                updates will be rendered. A custom callback function can also be specified which
                takes `(total_files, transformed, downloaded, skipped)` as an argument. The
                `total_files` parameter may be `None` until the system knows how many files need to
                be processed (and some files can even be completed before that is known).
         """
         self._dataset = dataset
-        self._codegen = codegen
         self._image = image
         self._max_workers = max_workers
         self._result_destination = result_destination
 
         # We can't create the notifier until the actual query,
         # so only need to save the status update.
         self._status_callback_factory = (
@@ -119,23 +115,23 @@
 
     @abstractmethod
     async def get_data_pandas_df_async(
         self, selection_query: str, title: Optional[str] = None
     ) -> pd.DataFrame:
         """
         Fetch query data from ServiceX matching `selection_query` and return it as
-        a pandas DataFrame. The data is uniquely ordered (the same query will always
+        a pandas dataframe. The data is uniquely ordered (the same query will always
         return the same order).
 
         Arguments:
             selection_query     The `qastle` string specifying the data to be queried
             title               Title reported to the ServiceX backend for status reporting
 
         Returns:
-            df                  The pandas DataFrame
+            df                  The pandas dataframe
 
         Exceptions:
             xxx                 If the data is not the correct shape (e.g. a flat,
                                 rectangular table).
         """
 
     @abstractmethod
```

### Comparing `servicex-2.6.3a1/servicex/utils.py` & `servicex-2.6b1/servicex/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 dynamic_ncols=True,
                 bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}]",
             )
 
     def _update_bar(
         self, bar: Optional[tqdm], total: Optional[int], num: int, failed: int
     ):
-        assert bar is not None, "Internal error - bar was not initialized"
+        assert bar is not None, "Internal error - bar was not initalized"
         if total is not None:
             if bar.total != total:
                 # There is a bug in the tqm library if running in a notebook
                 # See https://github.com/tqdm/tqdm/issues/688
                 # This forces us to do the reset, sadly.
                 old_num = bar.n  # type: int
                 bar.reset(total)
@@ -413,15 +413,15 @@
     Normalize the variables in a qastle expression. Should make the
     linq expression more easily comparable even if the algorithm that
     generates the underlying variable numbers changes. If the selection algorithm will violate
     the qastle syntax, it is returned unaltered and with no errors.
 
     Arguments
 
-        q           String containing the qastle code`
+        q           Strign containing the qastle code`
 
     Returns
 
         clean_q     Sanitized query - lambda arguments are given a uniform source code
                     labeling so that two queries with the same structure are marked as the same.
     """
     from collections import namedtuple
```

### Comparing `servicex-2.6.3a1/servicex.egg-info/PKG-INFO` & `servicex-2.6b1/servicex.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex
-Version: 2.6.3a1
+Version: 2.6b1
 Summary: Front-end for the ServiceX Data Server
 Home-page: https://github.com/ssl-hep/ServiceX_frontend
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
 License: TBD
@@ -12,20 +12,18 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # ServiceX Client Library
 
  Client access library for ServiceX
 
@@ -44,15 +42,15 @@
 - [func_adl.uproot](https://github.com/iris-hep/func_adl.uproot) (for flat ntuples)
 - [tcut_to_castle](https://pypi.org/project/tcut-to-qastle/) (translates `TCut` like syntax into a `servicex` query - should work for both)
 
 ## Prerequisites
 
 Before you can use this library you'll need:
 
-- An environment based on python 3.7 or later. 3.11 is highest supported at the moment.
+- An environment based on python 3.6 or later
 - A `ServiceX` end-point. This is usually gotten by logging into and getting approved at the servicex endpoint. Once you do that, you'll have an API token, which this library needs to access the `ServiceX` endpoint, and the web address where you got that token (the `endpoint` address).
 
 ### How to access your endpoint
 
 The API access information is normally placed in a configuration file (see the section below). Create a config file, `servicex.yaml`, in the `yaml` format, in the appropriate place for your work that contains the following (for the `xaod` backend; use `uproot` for the `type` for the uproot backend):
 
 ```yaml
@@ -217,18 +215,14 @@
   - Windows: `cache_path: "C:\\Users\\gordo\\Desktop\\cacheme"`
   - Linux: `cache_path: "/home/servicex-cache"`
 
 - `backend_types` - a list of yaml dictionaries that contains some defaults for the backends. By default only the `return_data` is there, which for `xaod` is `root` and `uproot` is `parquet`. There is also a `cms_run1_aod` which returns `root`. Allows `servicex` to convert to `pandas.DataFrame` or `awkward` if requested by the user.
 
 All strings are expanded using python's [os.path.expand](https://docs.python.org/3/library/os.path.html#os.path.expandvars) method - so `$NAME` and `${NAME}` will work to expand existing environment variables.
 
-For non-standard use cases, the user can specify:
-- The code generator that is used by the backend. This is done by passing a `codegen` argument to ServiceXDataset. This argument is normally inherited from the backend type set in `servicex.yaml`, but can be overridden with any valid `codegen` contained in the default type listing. A `codegen` entry can also be added to a backend in the yaml file to use as default.
-- The type of backend, using the `backend_type` argument on ServiceXDataset. This overrides the backend type setting in the `servicex.yaml` file.
-
 ## Features
 
 Implemented:
 
 - Accepts a `qastle` formatted query
 - Exceptions are used to report back errors of all sorts from the service to the user's code.
 - Data is return in the following forms:
@@ -247,15 +241,15 @@
   into repositories.
 
 ## Testing
 
 This code has been tested in several environments:
 
 - Windows, Linux, MacOS
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.6, 3.7, 3.8
 - Jupyter Notebooks (not automated), regular python command-line invoked source files
 
 ### Non-standard backends
 
 When doing backend development, often ports 9000 and 5000 are forwarded to the local machine exposing the `minio` and `ServiceX_App` instances. In that case, you'll need to create a configuration file that has `http://localhost:5000` as the end point. No API token is necessary if the development `ServiceX` instance doesn't have authorization turned on.
 
 ## API
```

### Comparing `servicex-2.6.3a1/setup.py` & `servicex-2.6b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import sys
 import os
 
 # Use the readme as the long description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+if sys.version_info[0] < 3:
+    raise NotImplementedError("Do not support version 2 of python")
+
 extra_test_packages = []
 if sys.version_info[1] < 8:
     extra_test_packages.append("asyncmock")
 
 version = os.getenv("servicex_version")
 if version is None:
     version = "0.1a1"
@@ -28,29 +31,29 @@
     long_description_content_type="text/markdown",
     author="G. Watts (IRIS-HEP/UW Seattle)",
     author_email="gwatts@uw.edu",
     maintainer="Gordon Watts (IRIS-HEP/UW Seattle)",
     maintainer_email="gwatts@uw.edu",
     url="https://github.com/ssl-hep/ServiceX_frontend",
     license="TBD",
-    python_requires=">=3.7",
+    python_requires=">=3.6, <3.11",
     test_suite="tests",
     install_requires=[
         "idna==2.10",  # Required to thread version needle with requests library
         "pandas~=1.0",
         "uproot>=4.0.1, <5",
         "awkward>=1.0.1, <2",
         "backoff>=2.0",
         "aiohttp~=3.6",
         "minio~=5.0",
         "tqdm~=4.0",
-        "qastle>=0.10",
-        "make_it_sync>= 1.0.0",
+        "qastle>=0.10, <1.0",
+        "make_it_sync==1.0.0",
         "google-auth",
-        "confuse",
+        "confuse==1.3.0",
         "pyarrow>=1.0",
     ],
     extras_require={
         "test": [
             "pytest>=3.9",
             "pytest-asyncio",
             "pytest-mock",
@@ -74,18 +77,16 @@
         # "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Topic :: Software Development",
         "Topic :: Utilities",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     package_data={
         "servicex": ["config_default.yaml"],
     },
     platforms="Any",
 )
```

