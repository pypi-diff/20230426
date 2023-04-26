# Comparing `tmp/changelog-0.5.8.tar.gz` & `tmp/changelog-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog-0.5.8.tar", last modified: Tue Jun 14 23:05:11 2022, max compression
+gzip compressed data, was "changelog-0.6.0.tar", last modified: Tue Apr 25 23:30:53 2023, max compression
```

## Comparing `changelog-0.5.8.tar` & `changelog-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 23:05:11.904870 changelog-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-06-14 23:04:56.000000 changelog-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-14 23:04:56.000000 changelog-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4969 2022-06-14 23:05:11.904870 changelog-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-06-14 23:04:56.000000 changelog-0.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 23:05:11.904870 changelog-0.5.8/changelog/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/changelog.css
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    14183 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/docutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (121)     9238 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/mdwriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-06-14 23:04:56.000000 changelog-0.5.8/changelog/sphinxext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 23:05:11.904870 changelog-0.5.8/changelog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4969 2022-06-14 23:05:11.000000 changelog-0.5.8/changelog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-06-14 23:05:11.000000 changelog-0.5.8/changelog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 23:05:11.000000 changelog-0.5.8/changelog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-14 23:05:11.000000 changelog-0.5.8/changelog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 23:05:09.000000 changelog-0.5.8/changelog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-14 23:05:11.000000 changelog-0.5.8/changelog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-06-14 23:05:11.904870 changelog-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-06-14 23:04:56.000000 changelog-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:53.887848 changelog-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-25 23:30:39.000000 changelog-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 23:30:39.000000 changelog-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-25 23:30:53.887848 changelog-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-25 23:30:39.000000 changelog-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:53.883848 changelog-0.6.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/changelog.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/mdwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-25 23:30:39.000000 changelog-0.6.0/changelog/sphinxext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:30:53.883848 changelog-0.6.0/changelog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 23:30:53.000000 changelog-0.6.0/changelog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 23:30:53.887848 changelog-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 23:30:39.000000 changelog-0.6.0/setup.py
```

### Comparing `changelog-0.5.8/LICENSE` & `changelog-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/PKG-INFO` & `changelog-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog
-Version: 0.5.8
+Version: 0.6.0
 Summary: Provides simple Sphinx markup to render changelog displays.
 Home-page: https://github.com/sqlalchemyorg/changelog
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Keywords: Sphinx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `changelog-0.5.8/README.rst` & `changelog-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog/cmd.py` & `changelog-0.6.0/changelog/cmd.py`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog/docutils.py` & `changelog-0.6.0/changelog/docutils.py`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog/environment.py` & `changelog-0.6.0/changelog/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,20 @@
 
     @classmethod
     def register(cls, env_class):
         cls.env_classes = (env_class,) + cls.env_classes
 
     @classmethod
     def from_document_settings(cls, settings):
-        try:
-            return settings._changelog_env
-        except AttributeError:
-            for cls in cls.env_classes:
-                e = cls.from_document_settings(settings)
-                if e is not None:
-                    settings._changelog_env = e
-                    return e
+        for cls in cls.env_classes:
+            e = cls.from_document_settings(settings)
+            if e is not None:
+                return e
 
-            raise NotImplementedError("TODO")
+        raise NotImplementedError("TODO")
 
     @property
     def temp_data(self):
         raise NotImplementedError()
 
     @property
     def changelog_sections(self):
```

### Comparing `changelog-0.5.8/changelog/generate_rst.py` & `changelog-0.6.0/changelog/generate_rst.py`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog/mdwriter.py` & `changelog-0.6.0/changelog/mdwriter.py`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog/sphinxext.py` & `changelog-0.6.0/changelog/sphinxext.py`

 * *Files identical despite different names*

### Comparing `changelog-0.5.8/changelog.egg-info/PKG-INFO` & `changelog-0.6.0/changelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog
-Version: 0.5.8
+Version: 0.6.0
 Summary: Provides simple Sphinx markup to render changelog displays.
 Home-page: https://github.com/sqlalchemyorg/changelog
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Keywords: Sphinx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `changelog-0.5.8/setup.py` & `changelog-0.6.0/setup.py`

 * *Files identical despite different names*

