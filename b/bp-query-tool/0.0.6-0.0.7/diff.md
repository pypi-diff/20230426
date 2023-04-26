# Comparing `tmp/bp_query_tool-0.0.6.tar.gz` & `tmp/bp_query_tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_query_tool-0.0.6.tar", last modified: Wed Apr 26 08:38:55 2023, max compression
+gzip compressed data, was "bp_query_tool-0.0.7.tar", last modified: Wed Apr 26 09:00:36 2023, max compression
```

## Comparing `bp_query_tool-0.0.6.tar` & `bp_query_tool-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.813880 bp_query_tool-0.0.6/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.6/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.6/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-26 08:38:55.813516 bp_query_tool-0.0.6/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.805029 bp_query_tool-0.0.6/bp_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-26 08:38:55.000000 bp_query_tool-0.0.6/bp_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-26 08:38:55.000000 bp_query_tool-0.0.6/bp_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-26 08:38:55.000000 bp_query_tool-0.0.6/bp_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-26 08:38:55.000000 bp_query_tool-0.0.6/bp_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-26 08:38:55.000000 bp_query_tool-0.0.6/bp_query_tool.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.805452 bp_query_tool-0.0.6/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.6/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.801387 bp_query_tool-0.0.6/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.806255 bp_query_tool-0.0.6/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.807138 bp_query_tool-0.0.6/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-26 07:58:40.000000 bp_query_tool-0.0.6/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1032251 2023-04-26 07:58:40.000000 bp_query_tool-0.0.6/query_tool/frontend/dist/assets/index-ec348719.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-04-26 08:38:09.000000 bp_query_tool-0.0.6/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-26 07:58:39.000000 bp_query_tool-0.0.6/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:38:55.812731 bp_query_tool-0.0.6/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.6/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-26 08:38:55.813992 bp_query_tool-0.0.6/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-26 07:57:02.000000 bp_query_tool-0.0.6/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.504350 bp_query_tool-0.0.7/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.7/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.7/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-26 09:00:36.503599 bp_query_tool-0.0.7/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.489808 bp_query_tool-0.0.7/bp_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-26 09:00:36.000000 bp_query_tool-0.0.7/bp_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-26 09:00:36.000000 bp_query_tool-0.0.7/bp_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-26 09:00:36.000000 bp_query_tool-0.0.7/bp_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-26 09:00:36.000000 bp_query_tool-0.0.7/bp_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-26 09:00:36.000000 bp_query_tool-0.0.7/bp_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.490235 bp_query_tool-0.0.7/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.7/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.484473 bp_query_tool-0.0.7/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.491689 bp_query_tool-0.0.7/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.493699 bp_query_tool-0.0.7/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-26 07:58:40.000000 bp_query_tool-0.0.7/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1032251 2023-04-26 07:58:40.000000 bp_query_tool-0.0.7/query_tool/frontend/dist/assets/index-ec348719.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-04-26 08:38:09.000000 bp_query_tool-0.0.7/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-26 07:58:39.000000 bp_query_tool-0.0.7/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 09:00:36.502493 bp_query_tool-0.0.7/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3839 2023-04-26 08:59:45.000000 bp_query_tool-0.0.7/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.7/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-26 09:00:36.504730 bp_query_tool-0.0.7/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-26 09:00:34.000000 bp_query_tool-0.0.7/setup.py
```

### Comparing `bp_query_tool-0.0.6/LICENSE` & `bp_query_tool-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/bp_query_tool.egg-info/SOURCES.txt` & `bp_query_tool-0.0.7/bp_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/__init__.py` & `bp_query_tool-0.0.7/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/frontend/dist/assets/index-ec348719.js` & `bp_query_tool-0.0.7/query_tool/frontend/dist/assets/index-ec348719.js`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/frontend/dist/index.html` & `bp_query_tool-0.0.7/query_tool/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/frontend/dist/vite.svg` & `bp_query_tool-0.0.7/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/services/dimension_service.py` & `bp_query_tool-0.0.7/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/services/entities_service.py` & `bp_query_tool-0.0.7/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/services/filters_service.py` & `bp_query_tool-0.0.7/query_tool/services/filters_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,21 @@
         self.filter_conditions = []
     
     def __is_string_column(self, column: dict = {}) -> bool:
         return True if column.get('data_type', 'string') == 'string' else False
 
     def get_filter_query(self, filters: List = None, table_aliases: dict = {}):
         if filters is not None:
+            index = 0
             for filter in filters:
+                if index > 0:
+                    self.filter_conditions.append(filter.get("connector", "AND"))
+                index =  index + 1
                 self.__get_filter(filter, table_aliases)
+                
         return self.filter_conditions
 
     def __get_filter(self, filter, table_aliases):
         self.filter_conditions.append("(")
         table, column = filter.get("fqcn", "").rsplit(".", 1)
         if filter.get("operator", "") in OPERATORS:
             self.filter_conditions.append(
```

### Comparing `bp_query_tool-0.0.6/query_tool/services/query_tool_service.py` & `bp_query_tool-0.0.7/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/query_tool/services/register.py` & `bp_query_tool-0.0.7/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.6/setup.py` & `bp_query_tool-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_query_tool",
-    version="0.0.6",
+    version="0.0.7",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

