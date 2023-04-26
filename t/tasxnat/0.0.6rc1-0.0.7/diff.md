# Comparing `tmp/tasxnat-0.0.6rc1.tar.gz` & `tmp/tasxnat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasxnat-0.0.6rc1.tar", last modified: Wed Apr 26 13:34:41 2023, max compression
+gzip compressed data, was "tasxnat-0.0.7.tar", last modified: Wed Apr 26 15:40:20 2023, max compression
```

## Comparing `tasxnat-0.0.6rc1.tar` & `tasxnat-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.6rc1/LICENSE.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      379 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.6rc1/pyproject.toml
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/setup.cfg
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/tasxnat/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      369 2023-04-26 13:34:08.000000 tasxnat-0.0.6rc1/tasxnat/__init__.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8817 2023-04-26 13:33:56.000000 tasxnat-0.0.6rc1/tasxnat/objects.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8377 2023-04-25 21:52:44.000000 tasxnat-0.0.6rc1/tasxnat/protocols.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     4218 2023-04-25 20:55:28.000000 tasxnat-0.0.6rc1/tasxnat/utilities.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 13:34:41.362916 tasxnat-0.0.6rc1/tasxnat.egg-info/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      379 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/SOURCES.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/dependency_links.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 13:34:41.000000 tasxnat-0.0.6rc1/tasxnat.egg-info/top_level.txt
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.7/LICENSE.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 15:40:20.184740 tasxnat-0.0.7/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.7/pyproject.toml
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 15:40:20.184740 tasxnat-0.0.7/setup.cfg
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/tasxnat/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      455 2023-04-26 15:39:34.000000 tasxnat-0.0.7/tasxnat/__init__.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8912 2023-04-26 15:28:43.000000 tasxnat-0.0.7/tasxnat/objects.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8540 2023-04-26 15:25:33.000000 tasxnat-0.0.7/tasxnat/protocols.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     4219 2023-04-26 13:47:54.000000 tasxnat-0.0.7/tasxnat/utilities.py
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/tasxnat.egg-info/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/top_level.txt
```

### Comparing `tasxnat-0.0.6rc1/LICENSE.txt` & `tasxnat-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.6rc1/pyproject.toml` & `tasxnat-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.6rc1/tasxnat/objects.py` & `tasxnat-0.0.7/tasxnat/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from tasxnat.utilities import *
 
 
 __all__ = (
     (
         "SimpleTaskBroker",
         "SimpleTaskable",
-        "SimpleTaskedCallable"
+        "SimpleTaskedCallable",
+        "AsyncTaskedCallable"
     ))
 
 
 def _simple_identifier(task: typing.Callable):
     return ":".join([task.__module__, task.__name__])
 
 
@@ -41,20 +42,24 @@
     __before_tasks__: _TCStack
     __after_tasks__: _TCStack
 
     @property
     def args(self):
         return self.__called_args__
 
+    @args.setter
+    def args(self, args):
+        self.__called_args__ = args
+
     @property
     def kwds(self):
         return self.__called_kwds__
 
     @property
-    def is_async(self) -> bool:
+    def is_async(self):
         return self._is_async
 
     @property
     def taskable(self):
         return self.__taskable__
 
     def push_before(self, fn):
@@ -289,17 +294,19 @@
                 self._process_tasks(iden, calls)
             return
 
         with mp.Pool(process_count) as p:
             result = p.starmap_async(self._process_tasks, task_call_maps)
             result.get(self._pool_max_timeout)
 
-    def _process_tasks(self,
-                       iden: str,
-                       calls: typing.Iterable[tuple[tuple, dict]]):
+    def _process_tasks(
+            self,
+            iden: str,
+            calls: typing.Iterable[tuple[tuple, dict]]):
+
         strict_mode = self.metadata["strict_mode"]
         root_task = self.__register__[iden]
 
         if root_task.thread_count <= 1:
             _process_tasks(root_task, calls, strict_mode)
         else:
             _process_tasks_multi(root_task, calls, strict_mode)
```

### Comparing `tasxnat-0.0.6rc1/tasxnat/protocols.py` & `tasxnat-0.0.7/tasxnat/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,28 @@
     """
     Callable object that is registered to some
     `TaskBroker` object.
     """
 
     @property
     @abc.abstractmethod
-    def args(self) -> tuple[typing.Any, ...]:
+    def args(self) -> typing.ParamSpecArgs:
         """VarArgs passed into this callable."""
 
+    @args.setter
+    @abc.abstractmethod
+    def args(self, *args: typing.ParamSpecArgs):
+        """
+        Set the VarArgs passed into this
+        callable.
+        """
+
     @property
     @abc.abstractmethod
-    def kwds(self) -> typing.Mapping[str, typing.Any]:
+    def kwds(self) -> typing.ParamSpecKwargs:
         """
         Keyword VarArgs passed into this
         callable.
         """
 
     @property
     def is_async(self) -> bool:
```

### Comparing `tasxnat-0.0.6rc1/tasxnat/utilities.py` & `tasxnat-0.0.7/tasxnat/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     return loop.run_until_complete(coro)
 
 
 def _process_tasks(
         root_task: Taskable,
         calls: typing.Iterable[tuple[tuple, dict]],
         strict_mode: bool):
+
     for args, kwds in calls:
         task = copy.deepcopy(root_task)
 
         task.handle(*args, **kwds)
         if task.is_success:
             continue
```

