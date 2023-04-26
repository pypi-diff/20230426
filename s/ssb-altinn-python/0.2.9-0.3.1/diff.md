# Comparing `tmp/ssb_altinn_python-0.2.9.tar.gz` & `tmp/ssb_altinn_python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.2.9.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.3.1.tar", max compression
```

## Comparing `ssb_altinn_python-0.2.9.tar` & `ssb_altinn_python-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/LICENSE
--rw-r--r--   0        0        0     3941 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/README.md
--rw-r--r--   0        0        0     1967 2023-04-25 16:45:43.540298 ssb_altinn_python-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      188 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/flatten.py
--rw-r--r--   0        0        0     4151 2023-04-25 16:45:43.540298 ssb_altinn_python-0.2.9/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/py.typed
--rw-r--r--   0        0        0      497 2023-04-25 16:45:18.916034 ssb_altinn_python-0.2.9/src/altinn/utils.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-25 16:57:33.912032 ssb_altinn_python-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3941 2023-04-25 16:57:33.912032 ssb_altinn_python-0.3.1/README.md
+-rw-r--r--   0        0        0     1967 2023-04-25 16:57:52.336315 ssb_altinn_python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/flatten.py
+-rw-r--r--   0        0        0     4208 2023-04-25 16:57:52.336315 ssb_altinn_python-0.3.1/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/py.typed
+-rw-r--r--   0        0        0      497 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/utils.py
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.3.1/PKG-INFO
```

### Comparing `ssb_altinn_python-0.2.9/LICENSE` & `ssb_altinn_python-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.9/README.md` & `ssb_altinn_python-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.9/pyproject.toml` & `ssb_altinn_python-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.2.9"
+version = "0.3.1"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.2.9/src/altinn/file.py` & `ssb_altinn_python-0.3.1/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.9/src/altinn/parser.py` & `ssb_altinn_python-0.3.1/src/altinn/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,19 @@
             pd.DataFrame: A DataFrame representation of the XML file.
         """
         xml_dict = self.to_dict()
         df = pd.DataFrame([xml_dict])
         return df
 
 
+def parse_single_file(file: str) -> pd.DataFrame:
+    """Parse a single XML file to a pandas DataFrame."""
+    return ParseSingleXml(file).to_dataframe()
+
+
 class ParseMultipleXml:
     """This class handles multiple Altinn xml-files."""
 
     def __init__(self, folder_path: str) -> None:
         """Initialize a ParseMultipleXml object with the given folder path.
 
         Args:
@@ -132,17 +137,13 @@
             pd.DataFrame: A DataFrame containing data from all XML files.
         """
         logger.info("Starting parsing of XML files...")
 
         xml_files = self.get_xml_files()
 
         with concurrent.futures.ProcessPoolExecutor() as executor:
-            results = list(
-                executor.map(
-                    lambda file: ParseSingleXml(file).to_dataframe(), xml_files
-                )
-            )
+            results = list(executor.map(parse_single_file, xml_files))
 
         combined_df = pd.concat(results, ignore_index=True, join="outer")
 
         logger.info("Parsing of XML files complete.")
         return combined_df
```

### Comparing `ssb_altinn_python-0.2.9/PKG-INFO` & `ssb_altinn_python-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.2.9
+Version: 0.3.1
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

