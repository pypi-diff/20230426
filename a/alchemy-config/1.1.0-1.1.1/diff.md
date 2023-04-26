# Comparing `tmp/alchemy-config-1.1.0.tar.gz` & `tmp/alchemy-config-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alchemy-config-1.1.0.tar", last modified: Tue Apr 25 18:17:15 2023, max compression
+gzip compressed data, was "dist/alchemy-config-1.1.1.tar", last modified: Tue Apr 25 21:56:59 2023, max compression
```

## Comparing `alchemy-config-1.1.0.tar` & `alchemy-config-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/alchemy_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/test/
--rw-r--r--   0 root         (0) root         (0)    10996 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/test/test_attribute_access_dict.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      964 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 18:17:15.000000 alchemy-config-1.1.0/aconfig/
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/aconfig/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13559 2023-04-25 18:16:48.000000 alchemy-config-1.1.0/aconfig/aconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/test/
+-rw-r--r--   0 root         (0) root         (0)    11628 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/test/test_attribute_access_dict.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/aconfig/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/aconfig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14360 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/aconfig/aconfig.py
```

### Comparing `alchemy-config-1.1.0/LICENSE` & `alchemy-config-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.0/PKG-INFO` & `alchemy-config-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-config
-Version: 1.1.0
+Version: 1.1.1
 Summary: Configuration framework in Python for general configuration use.
 Home-page: https://github.com/IBM/alchemy-config
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: config
 Platform: UNKNOWN
```

### Comparing `alchemy-config-1.1.0/alchemy_config.egg-info/PKG-INFO` & `alchemy-config-1.1.1/alchemy_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-config
-Version: 1.1.0
+Version: 1.1.1
 Summary: Configuration framework in Python for general configuration use.
 Home-page: https://github.com/IBM/alchemy-config
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: config
 Platform: UNKNOWN
```

### Comparing `alchemy-config-1.1.0/setup.py` & `alchemy-config-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.0/test/test_config.py` & `alchemy-config-1.1.1/test/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,7 +263,23 @@
             cfg.key1 = 1
 
     def test_immutable_config_from_mutable_config(self):
         cfg = aconfig.Config({'a': {'b': [{'c': 1}]}})
         immutable_config = aconfig.ImmutableConfig(cfg)
 
         assert cfg == immutable_config
+
+    def test_config_can_be_subclassed(self):
+        """It should be valid to subclass Config if you want your own init semantics"""
+        class MyConfig(aconfig.Config):
+            init_count = 0
+
+            def __init__(self, config_dict: dict):
+                super().__init__(config_dict)
+                # The top-level config init should only be invoked once
+                MyConfig.init_count += 1
+
+        # So initializing this with a nested config dict shouldn't cause the initializer to run
+        # multiple times
+        MyConfig({"nest": {"a thing": "here"}})
+
+        self.assertEqual(MyConfig.init_count, 1)
```

### Comparing `alchemy-config-1.1.0/test/test_attribute_access_dict.py` & `alchemy-config-1.1.1/test/test_attribute_access_dict.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.0/README.md` & `alchemy-config-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.0/aconfig/__init__.py` & `alchemy-config-1.1.1/aconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.0/aconfig/aconfig.py` & `alchemy-config-1.1.1/aconfig/aconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 #*****************************************************************#
 '''Handle all config-based operations.
 '''
 
 import os
 import re
 import copy
+import typing
 
 from yaml.representer import SafeRepresenter
 import yaml
 
+
 class AttributeAccessDict(dict):
     '''Wrapper around Python dict to make it accessible like an object.
     '''
     def __init__(self, input_map):
         '''Recursively assign attribute access and call parent __init__ as well.
 
         Args:
@@ -45,25 +47,34 @@
 
         # make it accessible like native Python dict
         super().__init__(**copied_map)
 
     @classmethod
     def _make_attribute_access_dict(cls, value):
         """Recursively walk down any `dict`s or `list`s and build attribute access dicts
-        🌶️🌶️🌶️: This is a classmethod so that inheritance is respected.
+        🌶️: This is a classmethod so that inheritance is respected.
+        🌶️🌶️🌶️: We don't call the `cls` initializer directly for the recursion, because we
+        don't want the `Config` class or its subclasses to be initialized multiple times.
+        Instead, we ask _recursive_dict_class() to return the (sub)class that should be used.
         """
-        if isinstance(value, cls):
+        recursive_class = cls._recursive_dict_class()
+        if isinstance(value, recursive_class):
             return value
         elif isinstance(value, dict):
-            return cls(value)
+            return recursive_class(value)
         elif isinstance(value, list):
-            return [cls._make_attribute_access_dict(v) for v in value]
+            return [recursive_class._make_attribute_access_dict(v) for v in value]
         else:
             return value
 
+    @classmethod
+    def _recursive_dict_class(cls) -> typing.Type['AttributeAccessDict']:
+        """Returns the class to be used to recursively build the config object"""
+        return AttributeAccessDict
+
     # BELOW MAKES INSTANCE ACCESSIBLE VIA NATIVE PYTHON DICT METHODS ###############################
 
     def __getattr__(self, key, default=None):
         return super().get(key, default)
 
     def __setattr__(self, key, value):
         if isinstance(value, AttributeAccessDict):
@@ -111,14 +122,19 @@
 
     def __setitem__(self, key, value):
         raise TypeError("ImmutableAttributeAccessDict does not support item assignment")
 
     def __setattr__(self, key, value):
         raise AttributeError("ImmutableAttributeAccessDict does not support attribute assignment")
 
+    @classmethod
+    def _recursive_dict_class(cls) -> typing.Type['AttributeAccessDict']:
+        """Make this class available to recursively build a full config"""
+        return ImmutableAttributeAccessDict
+
 
 class Config(AttributeAccessDict):
     '''Config which holds the configurations at the given config location.
     '''
     _search_pattern = re.compile('[.-]')
 
     def __init__(self, config, override_env_vars=True):
```

