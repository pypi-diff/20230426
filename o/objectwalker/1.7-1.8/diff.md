# Comparing `tmp/objectwalker-1.7.tar.gz` & `tmp/objectwalker-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-1.7.tar", last modified: Wed Apr 26 14:19:49 2023, max compression
+gzip compressed data, was "objectwalker-1.8.tar", last modified: Wed Apr 26 14:54:18 2023, max compression
```

## Comparing `objectwalker-1.7.tar` & `objectwalker-1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:19:49.400818 objectwalker-1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1275 2023-04-26 14:17:47.000000 objectwalker-1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.396818 objectwalker-1.7/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6291 2023-04-26 14:19:25.000000 objectwalker-1.7/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     1729 2023-04-26 14:05:14.000000 objectwalker-1.7/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)     1301 2023-04-26 14:08:12.000000 objectwalker-1.7/objectwalker/filters/EmptyFilter.py
--rw-rw-r--   0 root         (0) root         (0)      978 2023-04-26 14:06:59.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameContains.py
--rw-rw-r--   0 root         (0) root         (0)      985 2023-04-26 14:06:59.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)      970 2023-04-26 14:07:02.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameEquals.py
--rw-rw-r--   0 root         (0) root         (0)      995 2023-04-26 14:07:05.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      862 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathContains.py
--rw-rw-r--   0 root         (0) root         (0)      862 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathEndsWith.py
--rw-rw-r--   0 root         (0) root         (0)      868 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathStartsWith.py
--rw-rw-r--   0 root         (0) root         (0)      573 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
--rw-rw-r--   0 root         (0) root         (0)      531 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsMethodWrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsModule.py
--rw-rw-r--   0 root         (0) root         (0)      896 2023-04-26 13:58:25.000000 objectwalker-1.7/objectwalker/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:19:49.400818 objectwalker-1.7/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1163 2023-04-26 13:43:25.000000 objectwalker-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:54:18.807955 objectwalker-1.8/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:54:18.807955 objectwalker-1.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1541 2023-04-26 14:23:16.000000 objectwalker-1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:54:18.803955 objectwalker-1.8/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.8/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6291 2023-04-26 14:48:59.000000 objectwalker-1.8/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     1729 2023-04-26 14:05:14.000000 objectwalker-1.8/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:54:18.807955 objectwalker-1.8/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1301 2023-04-26 14:08:12.000000 objectwalker-1.8/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      978 2023-04-26 14:06:59.000000 objectwalker-1.8/objectwalker/filters/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)      985 2023-04-26 14:06:59.000000 objectwalker-1.8/objectwalker/filters/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      970 2023-04-26 14:07:02.000000 objectwalker-1.8/objectwalker/filters/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2023-04-26 14:07:05.000000 objectwalker-1.8/objectwalker/filters/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      853 2023-04-26 14:47:01.000000 objectwalker-1.8/objectwalker/filters/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)      860 2023-04-26 14:46:39.000000 objectwalker-1.8/objectwalker/filters/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      868 2023-04-26 14:46:48.000000 objectwalker-1.8/objectwalker/filters/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      573 2023-04-26 13:36:23.000000 objectwalker-1.8/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      531 2023-04-26 13:36:23.000000 objectwalker-1.8/objectwalker/filters/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-04-26 13:36:23.000000 objectwalker-1.8/objectwalker/filters/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      896 2023-04-26 13:58:25.000000 objectwalker-1.8/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:54:18.803955 objectwalker-1.8/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:54:18.000000 objectwalker-1.8/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-26 14:54:18.000000 objectwalker-1.8/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:54:18.000000 objectwalker-1.8/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 14:54:18.000000 objectwalker-1.8/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 14:54:18.000000 objectwalker-1.8/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:54:18.807955 objectwalker-1.8/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1163 2023-04-26 14:48:53.000000 objectwalker-1.8/setup.py
```

### Comparing `objectwalker-1.7/README.md` & `objectwalker-1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -24,10 +24,19 @@
 
 You can now install it from pypi (latest version is <img alt="PyPI" src="https://img.shields.io/pypi/v/objectwalker">) with this command:
 
 ```
 sudo python3 -m pip install objectwalker
 ```
 
+## Example commands
+
+ + We want to find all the paths to the `os` module in the module `jinja2`:
+    ```
+    objectwalker -m jinja2 --filter-object-is-module os --max-depth 15
+    ```
+    We get the following output:
+    ![](./.github/find_module_os_in_jinja2.png)
+
 ## Contributing
 
 Pull requests are welcome. Feel free to open an issue if you want to add other features.
```

#### html2text {}

```diff
@@ -4,9 +4,12 @@
    [GitHub release (latest by date)] [https://img.shields.io/twitter/follow/
    podalirius_?label=Podalirius&style=social] [YouTube_Channel_Subscribers]
 ## Features - [x] Python module to use in pdb after a `breakpoint()`. - [x]
 Standalone tool to explore paths in python modules. - [x] Multiple built-in
 filters. - [x] Possibility to implement custom filters and pass them to
 ObjectWalker(). ## Demonstration ## Installation You can now install it from
 pypi (latest version is [PyPI]) with this command: ``` sudo python3 -m pip
-install objectwalker ``` ## Contributing Pull requests are welcome. Feel free
-to open an issue if you want to add other features.
+install objectwalker ``` ## Example commands + We want to find all the paths to
+the `os` module in the module `jinja2`: ``` objectwalker -m jinja2 --filter-
+object-is-module os --max-depth 15 ``` We get the following output: ![]
+(./.github/find_module_os_in_jinja2.png) ## Contributing Pull requests are
+welcome. Feel free to open an issue if you want to add other features.
```

### Comparing `objectwalker-1.7/objectwalker/__main__.py` & `objectwalker-1.8/objectwalker/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import argparse
 import sys
 import objectwalker
 from objectwalker.filters import *
 
 
-VERSION = "1.7"
+VERSION = "1.8"
 
 
 banner = r"""
        ____  __      _           __ _       __      ____            
       / __ \/ /_    (_)__  _____/ /| |     / /___ _/ / /_____  _____
      / / / / __ \  / / _ \/ ___/ __/ | /| / / __ `/ / //_/ _ \/ ___/
     / /_/ / /_/ / / /  __/ /__/ /_ | |/ |/ / /_/ / / ,< /  __/ /      v%s
```

### Comparing `objectwalker-1.7/objectwalker/core.py` & `objectwalker-1.8/objectwalker/core.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/EmptyFilter.py` & `objectwalker-1.8/objectwalker/filters/EmptyFilter.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterObjectNameContains.py` & `objectwalker-1.8/objectwalker/filters/FilterObjectNameContains.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterObjectNameEndsWith.py` & `objectwalker-1.8/objectwalker/filters/FilterObjectNameEndsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterObjectNameEquals.py` & `objectwalker-1.8/objectwalker/filters/FilterObjectNameEquals.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterObjectNameStartsWith.py` & `objectwalker-1.8/objectwalker/filters/FilterObjectNameStartsWith.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterPathContains.py` & `objectwalker-1.8/objectwalker/filters/FilterPathEndsWith.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : FilterPathContains.py
+# File name          : FilterPathEndsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
 from .EmptyFilter import EmptyFilter
 
 
-class FilterPathContains(EmptyFilter):
+class FilterPathEndsWith(EmptyFilter):
     """
-    Documentation for class FilterPathContains
+    Documentation for class FilterPathEndsWith
     """
     values = []
     no_colors = False
 
     def __init__(self, values, no_colors=False):
         super(EmptyFilter, self).__init__()
         self.__filter_name = __name__.split('.')[-1]
         self.no_colors = no_colors
         self.values = values
 
     def check(self, obj, path_to_obj):
         matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value in element:
-                    matches_filter = True
-                    return matches_filter
+
+        if any(['.'.join(path_to_obj).endswith(value) for value in self.values]):
+            matches_filter = True
+
+        if matches_filter:
+            self.print_result(obj, path_to_obj)
         return matches_filter
```

### Comparing `objectwalker-1.7/objectwalker/filters/FilterPathStartsWith.py` & `objectwalker-1.8/objectwalker/filters/FilterPathStartsWith.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,13 +18,14 @@
         super(EmptyFilter, self).__init__()
         self.__filter_name = __name__.split('.')[-1]
         self.no_colors = no_colors
         self.values = values
 
     def check(self, obj, path_to_obj):
         matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value in element:
-                    matches_filter = True
-                    return matches_filter
+
+        if any(['.'.join(path_to_obj).startswith(value) for value in self.values]):
+            matches_filter = True
+
+        if matches_filter:
+            self.print_result(obj, path_to_obj)
         return matches_filter
```

### Comparing `objectwalker-1.7/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py` & `objectwalker-1.8/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterTypeIsMethodWrapper.py` & `objectwalker-1.8/objectwalker/filters/FilterTypeIsMethodWrapper.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/FilterTypeIsModule.py` & `objectwalker-1.8/objectwalker/filters/FilterTypeIsModule.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker/filters/__init__.py` & `objectwalker-1.8/objectwalker/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/objectwalker.egg-info/SOURCES.txt` & `objectwalker-1.8/objectwalker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objectwalker-1.7/setup.py` & `objectwalker-1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = """e"""
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="1.7",
+    version="1.8",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```

