# Comparing `tmp/tasxnat-0.0.7.tar.gz` & `tmp/tasxnat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasxnat-0.0.7.tar", last modified: Wed Apr 26 15:40:20 2023, max compression
+gzip compressed data, was "tasxnat-0.0.8.tar", last modified: Wed Apr 26 18:48:42 2023, max compression
```

## Comparing `tasxnat-0.0.7.tar` & `tasxnat-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.7/LICENSE.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 15:40:20.184740 tasxnat-0.0.7/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.7/pyproject.toml
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 15:40:20.184740 tasxnat-0.0.7/setup.cfg
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/tasxnat/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      455 2023-04-26 15:39:34.000000 tasxnat-0.0.7/tasxnat/__init__.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8912 2023-04-26 15:28:43.000000 tasxnat-0.0.7/tasxnat/objects.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8540 2023-04-26 15:25:33.000000 tasxnat-0.0.7/tasxnat/protocols.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     4219 2023-04-26 13:47:54.000000 tasxnat-0.0.7/tasxnat/utilities.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 15:40:20.184740 tasxnat-0.0.7/tasxnat.egg-info/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/SOURCES.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/dependency_links.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 15:40:20.000000 tasxnat-0.0.7/tasxnat.egg-info/top_level.txt
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 18:48:42.419986 tasxnat-0.0.8/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.8/LICENSE.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 18:48:42.419986 tasxnat-0.0.8/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      594 2023-04-17 14:47:22.000000 tasxnat-0.0.8/pyproject.toml
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-26 18:48:42.419986 tasxnat-0.0.8/setup.cfg
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 18:48:42.419986 tasxnat-0.0.8/tasxnat/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      455 2023-04-26 18:47:30.000000 tasxnat-0.0.8/tasxnat/__init__.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     9758 2023-04-26 17:49:09.000000 tasxnat-0.0.8/tasxnat/objects.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     9555 2023-04-26 18:05:49.000000 tasxnat-0.0.8/tasxnat/protocols.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     5217 2023-04-26 18:42:59.000000 tasxnat-0.0.8/tasxnat/utilities.py
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-26 18:48:42.419986 tasxnat-0.0.8/tasxnat.egg-info/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      376 2023-04-26 18:48:42.000000 tasxnat-0.0.8/tasxnat.egg-info/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      231 2023-04-26 18:48:42.000000 tasxnat-0.0.8/tasxnat.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-26 18:48:42.000000 tasxnat-0.0.8/tasxnat.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-26 18:48:42.000000 tasxnat-0.0.8/tasxnat.egg-info/top_level.txt
```

### Comparing `tasxnat-0.0.7/LICENSE.txt` & `tasxnat-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.7/pyproject.toml` & `tasxnat-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tasxnat-0.0.7/tasxnat/objects.py` & `tasxnat-0.0.8/tasxnat/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import inspect, multiprocessing as mp
+import inspect, time, multiprocessing as mp
 import typing
 from multiprocessing import pool
 
 from tasxnat.protocols import\
 (
     Taskable,
     TaskBroker,
@@ -182,14 +182,41 @@
                       broker,
                       fn,
                       thread_count=None,
                       is_strict=None,
                       is_async=None):
         return cls(broker, fn, thread_count, is_strict, is_async)
 
+    def set_thread_pool(self, pool, queue):
+        if self.thread_count <= 1:
+            raise RuntimeError(f"Threading was not enable for this task.")
+
+        self._thread_pool = pool
+        self._thread_queue = queue
+
+    def request_new_thread(
+            self,
+            fn,
+            callargs,
+            *,
+            timeout: int | float | None = None):
+
+        if self.thread_count <= 1:
+            raise RuntimeError(f"Threading was not enable for this task.")
+
+        tqueue = self._thread_queue
+        request_t = time.monotonic()
+        while (len(tqueue) + 1) == tqueue.maxlen:
+            time.sleep(0.1)
+            curr_t = time.monotonic()
+            if timeout and (curr_t - request_t) > timeout:
+                raise TimeoutError("Thread request took too long.")
+
+        tqueue.append((fn, callargs))
+
     def __init__(self,
                  broker: TaskBroker,
                  fn: typing.Callable,
                  thread_count: typing.Optional[int] = None,
                  is_strict: typing.Optional[bool] = None,
                  is_async: typing.Optional[bool] = None):
         self._broker = broker
```

### Comparing `tasxnat-0.0.7/tasxnat/protocols.py` & `tasxnat-0.0.8/tasxnat/protocols.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import abc, typing
+from collections import deque
+from concurrent.futures import ThreadPoolExecutor
 from multiprocessing import pool
 
 __all__ = (
     (
         "_PoolFactory",
+        "_TCStack",
         "TaskedCallable",
         "TaskBroker",
         "Taskable"
     ))
 
 _Ps = typing.ParamSpec("_Ps")
 _RT = typing.TypeVar("_RT")
 _RT_co = typing.TypeVar("_RT_co", covariant=True)
 _PoolFactory = type[pool.Pool] | typing.Callable[[], pool.Pool]
 _TCStackCallable = typing.Callable[["TaskedCallable"], None]
 _TaskableCallable = typing.Callable[typing.Concatenate["Taskable", _Ps], _RT]
 
 
+class TaskQueue(deque[tuple[typing.Callable, tuple[tuple, dict]]]):
+    ...
+
+
 class _TCStack(typing.Sequence[_TCStackCallable]):
     """
     Sequence of callable objects run in First In
     First Called (FIFC).
     """
 
     @abc.abstractmethod
@@ -174,25 +181,53 @@
         """
         Executes this task with the arguments
         passed.
         """
 
     @classmethod
     @abc.abstractmethod
-    def from_callable(cls,
-                      broker: "TaskBroker",
-                      fn: typing.Callable,
-                      thread_count: typing.Optional[int],
-                      is_strict: typing.Optional[bool],
-                      is_async: typing.Optional[bool]) -> typing.Self:
+    def from_callable(
+        cls,
+        broker: "TaskBroker",
+        fn: typing.Callable,
+        thread_count: typing.Optional[int],
+        is_strict: typing.Optional[bool],
+        is_async: typing.Optional[bool]) -> typing.Self:
         """
         Create a `Taskable` from a callable
         object.
         """
 
+    @abc.abstractmethod
+    def set_thread_pool(self, pool: ThreadPoolExecutor, queue: TaskQueue):
+        """
+        Sets the thread pool object to be used
+        in multi-threaded mode. This method is
+        intended for internal use only.
+
+        Throws an error if this `Taskable` is not
+        meant to be run in multi-threaded mode.
+        """
+
+    @abc.abstractmethod
+    def request_new_thread(
+        self,
+        fn: typing.Callable,
+        callargs: tuple[tuple, dict],
+        *,
+        timeout: int | float | None):
+        """
+        Attempt to run some process in the
+        attached thread pool. If successful, the
+        call will be sent to the queue.
+
+        Throws an error if this `Taskable` is not
+        meant to be run in multi-threaded mode.
+        """
+
 
 @typing.runtime_checkable
 class TaskBroker(typing.Protocol):
     """
     Manages `Taskable` objects. This includes
     instantiation, execution and evaluation of
     execution results.
@@ -206,63 +241,72 @@
     @typing.overload
     @abc.abstractmethod
     def task(self, fn: typing.Callable, /) -> TaskedCallable:
         ...
 
     @typing.overload
     @abc.abstractmethod
-    def task(self,
-             *,
-             klass: typing.Optional[type[Taskable]],
-             thread_count: typing.Optional[int],
-             is_strict: typing.Optional[bool],
-             is_async: typing.Optional[bool]) -> typing.Callable[[], TaskedCallable]:
+    def task(
+        self,
+        /,
+        *,
+        klass: typing.Optional[type[Taskable]],
+        thread_count: typing.Optional[int],
+        is_strict: typing.Optional[bool],
+        is_async: typing.Optional[bool]
+        ) -> typing.Callable[[], TaskedCallable]:
         ...
 
     @abc.abstractmethod
-    def task(self,
-             fn: typing.Callable | None = None,
-             *,
-             klass: typing.Optional[type[Taskable]] = None,
-             thread_count: typing.Optional[int] = None,
-             is_strict: typing.Optional[bool] = None,
-             is_async: typing.Optional[bool] = None) -> TaskedCallable | typing.Callable[[], TaskedCallable]: 
+    def task(
+        self,
+        fn: typing.Callable | None = None, /,
+        *,
+        klass: typing.Optional[type[Taskable]] = None,
+        thread_count: typing.Optional[int] = None,
+        is_strict: typing.Optional[bool] = None,
+        is_async: typing.Optional[bool] = None,
+        ) -> TaskedCallable | typing.Callable[[], TaskedCallable]: 
         """
         Creates and registers a `Taskable`
         object.
         """
 
     @typing.overload
     @abc.abstractmethod
     def before(
         self,
-        fn: _TCStackCallable, /) -> typing.Callable[[], TaskedCallable]:
+        fn: _TCStackCallable,
+        /) -> typing.Callable[[], TaskedCallable]:
         ...
 
     @typing.overload
     @abc.abstractmethod
     def before(
         self,
         fn1: TaskedCallable,
-        fn2: _TCStackCallable, /) -> TaskedCallable:
+        fn2: _TCStackCallable,
+        /) -> TaskedCallable:
         ...
 
     @typing.overload
     @abc.abstractmethod
     def before(
         self,
         fn1: TaskedCallable | _TCStackCallable,
-        fn2: TaskedCallable | _TCStackCallable | None, /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
+        fn2: TaskedCallable | _TCStackCallable | None,
+        /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
         ...
 
     @abc.abstractmethod
     def before(
         self,
         fn1: TaskedCallable | _TCStackCallable,
-        fn2: TaskedCallable | _TCStackCallable | None = None) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
+        fn2: TaskedCallable | _TCStackCallable | None = None,
+        /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
         """
         Push the target callable on to the
         *before* stack of the given
         `TaskedCallable`.
         """
 
     @typing.overload
@@ -281,22 +325,24 @@
         ...
 
     @typing.overload
     @abc.abstractmethod
     def after(
         self,
         fn1: TaskedCallable | _TCStackCallable,
-        fn2: TaskedCallable | _TCStackCallable | None, /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
+        fn2: TaskedCallable | _TCStackCallable | None,
+        /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
         ...
 
     @abc.abstractmethod
     def after(
         self,
         fn1: TaskedCallable | _TCStackCallable,
-        fn2: TaskedCallable | _TCStackCallable | None = None) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
+        fn2: TaskedCallable | _TCStackCallable | None = None,
+        /) -> TaskedCallable | typing.Callable[[], TaskedCallable]:
         """
         Push the target callable on to the
         *after* stack of the given
         `TaskedCallable`.
         """
 
     @abc.abstractmethod
@@ -304,26 +350,28 @@
         """
         Register a `Taskable` object to this.
         task manager.
         """
 
     @typing.overload
     @abc.abstractmethod
-    def process_tasks(self, *task_callers: str) -> None:
+    def process_tasks(self, /, *task_callers: str) -> None:
         ...
 
     @typing.overload
     @abc.abstractmethod
     def process_tasks(self,
+                      /,
                       *task_callers: str,
                       process_count: typing.Optional[int]) -> None:
         ...
 
     @abc.abstractmethod
     def process_tasks(self,
+                      /,
                       *task_callers: str,
                       process_count: typing.Optional[int] = None) -> None:
         """
         Executes given tasks from their
         identifiers.
 
         :task_callers: series of strings in the
```

### Comparing `tasxnat-0.0.7/tasxnat/utilities.py` & `tasxnat-0.0.8/tasxnat/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import asyncio, copy, re
+import asyncio, copy, inspect, re
 import typing
 from concurrent import futures
 from concurrent.futures import ThreadPoolExecutor
 
-from tasxnat.protocols import Taskable
+from tasxnat.protocols import Taskable, TaskQueue
 
 
 __all__ = (
     (
         "_parse_task_call",
         "_flatten_to_taskmaps",
         "_handle_coroutine",
@@ -86,61 +86,90 @@
             taskable_map[iden] = (callargs,)
 
     # Flatten the taskable map for pool
     # consumption
     return [(iden, calls) for iden, calls in taskable_map.items()]
 
 
-def _handle_coroutine(coro: typing.Coroutine):
+def _handle_coroutine(
+        coro: typing.Coroutine,
+        multithread_mode: bool | None = None):
     policy = asyncio.get_event_loop_policy()
     try:
         loop = policy.get_event_loop()
     except RuntimeError:
         loop = policy.new_event_loop()
 
-    return loop.run_until_complete(coro)
+    ret = loop.run_until_complete(coro)
+    if multithread_mode:
+        # Closing the loop after running the
+        # coroutine. Should prevent issues when
+        # loop.__del__ is called.
+        loop.close()
+
+    return ret
 
 
 def _process_tasks(
         root_task: Taskable,
         calls: typing.Iterable[tuple[tuple, dict]],
         strict_mode: bool):
 
     for args, kwds in calls:
         task = copy.deepcopy(root_task)
-
         task.handle(*args, **kwds)
+
         if task.is_success:
             continue
 
         # Bail on first failure if strict mode.
         if strict_mode and task.is_strict:
             if task.failure[1]:
                 raise task.failure[1]
 
 
 def _process_tasks_multi(
         root_task: Taskable,
         calls: typing.Iterable[tuple[tuple, dict]],
         strict_mode: bool):
-    tpool = ThreadPoolExecutor(root_task.thread_count, root_task.identifier)
     # loop = asyncio.get_event_loop_policy().get_event_loop()
 
-    def inner(call: tuple[tuple, dict]):
-        args, kwds = call
+    def inner(*args, **kwds):
         task = copy.deepcopy(root_task)
+        task.set_thread_pool(tpool, tqueue)
         task.handle(*args, **kwds)
 
         if task.is_success:
             return
 
         if strict_mode and task.is_strict:
             _, err = task.failure
             raise err #type: ignore[misc]
 
+    tpool  = ThreadPoolExecutor(root_task.thread_count, root_task.identifier)
+    tqueue = TaskQueue([(inner, c) for c in calls], root_task.thread_count) #type: ignore[misc]
+
     with tpool:
-        results = futures.wait([
-            tpool.submit(inner, call)
-            for call in calls], 30, "FIRST_EXCEPTION")
+        while True:
+
+            next_calls = []
+            while len(tqueue):
+                next_calls.append(tqueue.pop())
+
+            submitted = []
+            for fn, callargs in next_calls:
+                # Transform callable if it is a
+                # coroutine.
+                if inspect.iscoroutinefunction(fn):
+                    callargs = ((fn(*callargs[0], **callargs[1]), True), {})
+                    fn = _handle_coroutine
+
+                # Submit function call to executor.
+                submitted.append(tpool.submit(fn, *callargs[0], **callargs[1]))
+
+            # Await results from futures.
+            results = futures.wait(submitted, 30, "FIRST_EXCEPTION")
+            for result in results.done:
+                result.result()
 
-        for result in results.done:
-            result.result()
+            if not len(tqueue):
+                break
```

