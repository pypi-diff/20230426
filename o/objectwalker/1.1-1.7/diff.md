# Comparing `tmp/objectwalker-1.1.tar.gz` & `tmp/objectwalker-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectwalker-1.1.tar", last modified: Wed Apr 26 08:56:50 2023, max compression
+gzip compressed data, was "objectwalker-1.7.tar", last modified: Wed Apr 26 14:19:49 2023, max compression
```

## Comparing `objectwalker-1.1.tar` & `objectwalker-1.7.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 08:56:50.901183 objectwalker-1.1/
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 08:56:50.901183 objectwalker-1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      328 2023-04-26 07:35:05.000000 objectwalker-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 08:56:50.901183 objectwalker-1.1/objectwalker/
--rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 08:29:12.000000 objectwalker-1.1/objectwalker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2363 2023-04-26 08:54:12.000000 objectwalker-1.1/objectwalker/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     2137 2023-04-26 08:50:27.000000 objectwalker-1.1/objectwalker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 08:56:50.901183 objectwalker-1.1/objectwalker/filters/
--rw-rw-r--   0 root         (0) root         (0)      339 2023-04-26 08:27:17.000000 objectwalker-1.1/objectwalker/filters/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1216 2023-04-26 08:41:51.000000 objectwalker-1.1/objectwalker/filters/filter_object.py
--rw-rw-r--   0 root         (0) root         (0)     1742 2023-04-26 08:42:30.000000 objectwalker-1.1/objectwalker/filters/filter_path.py
--rw-rw-r--   0 root         (0) root         (0)     1519 2023-04-26 08:36:17.000000 objectwalker-1.1/objectwalker/filters/filter_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 08:56:50.901183 objectwalker-1.1/objectwalker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 08:56:50.000000 objectwalker-1.1/objectwalker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-26 08:56:50.000000 objectwalker-1.1/objectwalker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 08:56:50.000000 objectwalker-1.1/objectwalker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 08:56:50.000000 objectwalker-1.1/objectwalker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 08:56:50.000000 objectwalker-1.1/objectwalker.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 08:56:50.901183 objectwalker-1.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1163 2023-04-26 08:28:23.000000 objectwalker-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-04-26 07:33:18.000000 objectwalker-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:19:49.400818 objectwalker-1.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1275 2023-04-26 14:17:47.000000 objectwalker-1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.396818 objectwalker-1.7/objectwalker/
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6291 2023-04-26 14:19:25.000000 objectwalker-1.7/objectwalker/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     1729 2023-04-26 14:05:14.000000 objectwalker-1.7/objectwalker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/objectwalker/filters/
+-rw-rw-r--   0 root         (0) root         (0)     1301 2023-04-26 14:08:12.000000 objectwalker-1.7/objectwalker/filters/EmptyFilter.py
+-rw-rw-r--   0 root         (0) root         (0)      978 2023-04-26 14:06:59.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameContains.py
+-rw-rw-r--   0 root         (0) root         (0)      985 2023-04-26 14:06:59.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      970 2023-04-26 14:07:02.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameEquals.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2023-04-26 14:07:05.000000 objectwalker-1.7/objectwalker/filters/FilterObjectNameStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      862 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathContains.py
+-rw-rw-r--   0 root         (0) root         (0)      862 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathEndsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      868 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterPathStartsWith.py
+-rw-rw-r--   0 root         (0) root         (0)      573 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsBuiltinFunctionOrMethod.py
+-rw-rw-r--   0 root         (0) root         (0)      531 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsMethodWrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2411 2023-04-26 13:36:23.000000 objectwalker-1.7/objectwalker/filters/FilterTypeIsModule.py
+-rw-rw-r--   0 root         (0) root         (0)      896 2023-04-26 13:58:25.000000 objectwalker-1.7/objectwalker/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:19:49.400818 objectwalker-1.7/objectwalker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 14:19:49.000000 objectwalker-1.7/objectwalker.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-26 08:18:35.000000 objectwalker-1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:19:49.400818 objectwalker-1.7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1163 2023-04-26 13:43:25.000000 objectwalker-1.7/setup.py
```

### Comparing `objectwalker-1.1/objectwalker/core.py` & `objectwalker-1.7/objectwalker/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,23 +28,19 @@
                         subobj = eval("obj.%s" % subkey, {'obj': obj})
                     except SyntaxError as e:
                         continue
 
                     path_to_obj = path+[subkey]
 
                     if any([f.check(subobj, path_to_obj) for f in self.filters]):
-                        # Print the found path
-                        if self.no_colors:
-                            print("[%-50s] [type=%s] | %s" % (str(subobj)[:50], str(type(subobj)), '.'.join(path_to_obj)))
-                        else:
-                            print("[\x1b[94m%-50s\x1b[0m] [\x1b[95mtype=%s\x1b[0m] | \x1b[93m%s\x1b[0m" % (str(subobj)[:50], str(type(subobj)), '.'.join(path_to_obj)))
+
                         # Save the found path
                         found.append(path_to_obj)
-                    elif self.verbose:
-                        print("[SKIPPED] %s" % ('.'.join(path_to_obj)))
+                    # elif self.debug:
+                    #     print("[SKIPPED] %s" % ('.'.join(path_to_obj)))
 
                     # Explore further
                     if id(subobj) not in self.knownids:
                         self.knownids.append(id(subobj))
                         found = self.walk(obj=subobj, found=found, path=path+[subkey], depth=(depth+1), maxdepth=maxdepth, verbose=verbose)
 
                 except AttributeError as e:
```

### Comparing `objectwalker-1.1/objectwalker/filters/filter_object.py` & `objectwalker-1.7/objectwalker/filters/FilterPathEndsWith.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : filter_object.py
+# File name          : FilterPathEndsWith.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-class FilterObjNameEq(object):
-    """
-    Documentation for class FilterObjNameEq
-    """
-    values = []
-    def __init__(self, values):
-        super(FilterObjNameEq, self).__init__()
-        self.values = values
-
-    def check(self, obj, path_to_obj):
-        matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value == element:
-                    matches_filter = True
-                    return matches_filter
-        return matches_filter
+from .EmptyFilter import EmptyFilter
 
 
-class FilterObjNameContains(object):
+class FilterPathEndsWith(EmptyFilter):
     """
-    Documentation for class FilterObjNameContains
+    Documentation for class FilterPathEndsWith
     """
     values = []
-    def __init__(self, values):
-        super(FilterObjNameContains, self).__init__()
+    no_colors = False
+
+    def __init__(self, values, no_colors=False):
+        super(EmptyFilter, self).__init__()
+        self.__filter_name = __name__.split('.')[-1]
+        self.no_colors = no_colors
         self.values = values
 
     def check(self, obj, path_to_obj):
         matches_filter = False
         for element in path_to_obj:
             for value in self.values:
                 if value in element:
                     matches_filter = True
                     return matches_filter
-        return matches_filter
+        return matches_filter
```

### Comparing `objectwalker-1.1/objectwalker/filters/filter_path.py` & `objectwalker-1.7/objectwalker/filters/FilterObjectNameContains.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# File name          : filter_path.py
+# File name          : FilterObjectNameContains.py
 # Author             : Podalirius (@podalirius_)
 # Date created       : 26 Apr 2023
 
-class FilterPathContains(object):
-    """
-    Documentation for class FilterPathContains
-    """
-    values = []
-    def __init__(self, values):
-        super(FilterPathContains, self).__init__()
-        self.values = values
+from .EmptyFilter import EmptyFilter
 
-    def check(self, obj, path_to_obj):
-        matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value in element:
-                    matches_filter = True
-                    return matches_filter
-        return matches_filter
 
-
-class FilterPathStartsWith(object):
+class FilterObjectNameContains(EmptyFilter):
     """
-    Documentation for class FilterPathStartsWith
+    Documentation for class FilterObjectNameContains
     """
     values = []
-    def __init__(self, values):
-        super(FilterPathStartsWith, self).__init__()
+    no_colors = False
+
+    def __init__(self, values, no_colors=False):
+        super(FilterObjectNameContains, self).__init__()
+        self.__filter_name = __name__.split('.')[-1]
+        self.no_colors = no_colors
         self.values = values
 
     def check(self, obj, path_to_obj):
         matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value in element:
-                    matches_filter = True
-                    return matches_filter
-        return matches_filter
 
+        if any([(value in str(path_to_obj[-1])) for value in self.values]):
+            matches_filter = True
 
-class FilterPathEndsWith(object):
-    """
-    Documentation for class FilterPathEndsWith
-    """
-    values = []
-    def __init__(self, values):
-        super(FilterPathEndsWith, self).__init__()
-        self.values = values
+        if matches_filter:
+            self.print_result(obj, path_to_obj)
+        return matches_filter
 
-    def check(self, obj, path_to_obj):
-        matches_filter = False
-        for element in path_to_obj:
-            for value in self.values:
-                if value in element:
-                    matches_filter = True
-                    return matches_filter
-        return matches_filter
+    def __repr__(self):
+        return "<%s values=%s>" % (self.__filter_name, self.values)
```

### Comparing `objectwalker-1.1/setup.py` & `objectwalker-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = """e"""
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = [x.strip() for x in f.readlines()]
 
 setuptools.setup(
     name="objectwalker",
-    version="1.1",
+    version="1.7",
     description="",
     url="https://github.com/p0dalirius/objectwalker",
     author="Podalirius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="podalirius@protonmail.com",
     packages=["objectwalker", "objectwalker.filters"],
```

