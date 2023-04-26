# Comparing `tmp/tasxnat-0.0.6.tar.gz` & `tmp/tasxnat-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasxnat-0.0.6.tar", last modified: Wed Apr 26 13:30:54 2023, max compression
+gzip compressed data, was "tasxnat-0.0.6rc1.tar", last modified: Wed Apr 26 13:34:41 2023, max compression
```

## Comparing `tasxnat-0.0.6.tar` & `tasxnat-0.0.6rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:30:54.572449 tasxnat-0.0.6/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.6/LICENSE.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 13:30:54.572449 tasxnat-0.0.6/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.6/pyproject.toml
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 13:30:54.572449 tasxnat-0.0.6/setup.cfg
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:30:54.568449 tasxnat-0.0.6/tasxnat/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      362 2023-04-25 21:10:12.000000 tasxnat-0.0.6/tasxnat/__init__.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8797 2023-04-26 13:29:55.000000 tasxnat-0.0.6/tasxnat/objects.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8377 2023-04-25 21:52:44.000000 tasxnat-0.0.6/tasxnat/protocols.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     4218 2023-04-25 20:55:28.000000 tasxnat-0.0.6/tasxnat/utilities.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:30:54.568449 tasxnat-0.0.6/tasxnat.egg-info/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 13:30:54.000000 tasxnat-0.0.6/tasxnat.egg-info/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 13:30:54.000000 tasxnat-0.0.6/tasxnat.egg-info/SOURCES.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 13:30:54.000000 tasxnat-0.0.6/tasxnat.egg-info/dependency_links.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 13:30:54.000000 tasxnat-0.0.6/tasxnat.egg-info/top_level.txt
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.6rc1/LICENSE.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      379 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.6rc1/pyproject.toml
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/setup.cfg
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/tasxnat/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      369 2023-04-26 13:34:08.000000 tasxnat-0.0.6rc1/tasxnat/__init__.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8817 2023-04-26 13:33:56.000000 tasxnat-0.0.6rc1/tasxnat/objects.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8377 2023-04-25 21:52:44.000000 tasxnat-0.0.6rc1/tasxnat/protocols.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     4218 2023-04-25 20:55:28.000000 tasxnat-0.0.6rc1/tasxnat/utilities.py
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/tasxnat.egg-info/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      379 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/top_level.txt
```

### Comparing `tasxnat-0.0.6/LICENSE.txt` & `tasxnat-0.0.6rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.6/pyproject.toml` & `tasxnat-0.0.6rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.6/tasxnat/objects.py` & `tasxnat-0.0.6rc1/tasxnat/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,19 +81,19 @@
         self.__before__()
         rt = self.__task__(self.taskable, *self.args, **self.kwds)
         self.__after__()
 
         return rt
 
     def __before__(self):
-        for fn in self.__before_tasks__:
+        for fn in reversed(self.__before_tasks__):
             fn(self)
 
     def __after__(self) -> None:
-        for fn in self.__after_tasks__:
+        for fn in reversed(self.__after_tasks__):
             fn(self)
 
 
 class AsyncTaskedCallable(SimpleTaskedCallable):
 
     async def __call__(self, *args, **kwds):
         self.__called_args__ = args
```

### Comparing `tasxnat-0.0.6/tasxnat/protocols.py` & `tasxnat-0.0.6rc1/tasxnat/protocols.py`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.6/tasxnat/utilities.py` & `tasxnat-0.0.6rc1/tasxnat/utilities.py`

 * *Files identical despite different names*

