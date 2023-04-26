# Comparing `tmp/soda_svg-1.1.8.tar.gz` & `tmp/soda_svg-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_svg-1.1.8.tar", max compression
+gzip compressed data, was "soda_svg-1.1.9.tar", max compression
```

## Comparing `soda_svg-1.1.8.tar` & `soda_svg-1.1.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-04-26 16:07:17.683223 soda_svg-1.1.8/LICENSE
--rw-r--r--   0        0        0    13152 2023-04-26 16:07:17.683223 soda_svg-1.1.8/README.md
--rw-r--r--   0        0        0      515 2023-04-26 16:07:17.683223 soda_svg-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      317 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/__init__.py
--rw-r--r--   0        0        0      123 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/config_mod.py
--rw-r--r--   0        0        0     2513 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/custom_tags.py
--rw-r--r--   0        0        0     7357 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/paths.py
--rw-r--r--   0        0        0    11689 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/point.py
--rw-r--r--   0        0        0    10460 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/tags.py
--rw-r--r--   0        0        0     1838 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/utils.py
--rw-r--r--   0        0        0      924 2023-04-26 16:07:17.683223 soda_svg-1.1.8/soda/xml_parse.py
--rw-r--r--   0        0        0    13838 1970-01-01 00:00:00.000000 soda_svg-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-26 16:43:52.177430 soda_svg-1.1.9/LICENSE
+-rw-r--r--   0        0        0    13152 2023-04-26 16:43:52.177430 soda_svg-1.1.9/README.md
+-rw-r--r--   0        0        0      515 2023-04-26 16:43:52.177430 soda_svg-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/config_mod.py
+-rw-r--r--   0        0        0     2513 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/custom_tags.py
+-rw-r--r--   0        0        0     7357 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/paths.py
+-rw-r--r--   0        0        0    11689 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/point.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/py.typed
+-rw-r--r--   0        0        0    10460 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/tags.py
+-rw-r--r--   0        0        0     1838 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/utils.py
+-rw-r--r--   0        0        0      924 2023-04-26 16:43:52.177430 soda_svg-1.1.9/soda/xml_parse.py
+-rw-r--r--   0        0        0    13838 1970-01-01 00:00:00.000000 soda_svg-1.1.9/PKG-INFO
```

### Comparing `soda_svg-1.1.8/LICENSE` & `soda_svg-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/README.md` & `soda_svg-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/pyproject.toml` & `soda_svg-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "soda-svg"
 packages = [{include = "soda"}]
-version = "1.1.8"
+version = "1.1.9"
 description = "Fast SVG generation tool"
 authors = ["Dmitry Gritsenko <soda@evtn.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/soda"
 homepage = "https://github.com/evtn/soda"
 keywords = ["soda", "svg", "xml"]
```

### Comparing `soda_svg-1.1.8/soda/custom_tags.py` & `soda_svg-1.1.9/soda/custom_tags.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/soda/paths.py` & `soda_svg-1.1.9/soda/paths.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/soda/point.py` & `soda_svg-1.1.9/soda/point.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/soda/tags.py` & `soda_svg-1.1.9/soda/tags.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/soda/utils.py` & `soda_svg-1.1.9/soda/utils.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/soda/xml_parse.py` & `soda_svg-1.1.9/soda/xml_parse.py`

 * *Files identical despite different names*

### Comparing `soda_svg-1.1.8/PKG-INFO` & `soda_svg-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-svg
-Version: 1.1.8
+Version: 1.1.9
 Summary: Fast SVG generation tool
 Home-page: https://github.com/evtn/soda
 License: MIT
 Keywords: soda,svg,xml
 Author: Dmitry Gritsenko
 Author-email: soda@evtn.ru
 Requires-Python: >=3.7.0
```

