# Comparing `tmp/workercontext-0.0.2.tar.gz` & `tmp/workercontext-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workercontext-0.0.2.tar", last modified: Wed Apr 26 09:18:37 2023, max compression
+gzip compressed data, was "workercontext-0.0.3.tar", last modified: Wed Apr 26 09:52:39 2023, max compression
```

## Comparing `workercontext-0.0.2.tar` & `workercontext-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:18:37.633995 workercontext-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-04-26 08:49:47.000000 workercontext-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     6061 2023-04-26 09:18:37.631995 workercontext-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4197 2023-04-26 09:11:22.000000 workercontext-0.0.2/README.md
--rw-rw-rw-   0        0        0      738 2023-04-26 09:16:58.000000 workercontext-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 09:18:37.634995 workercontext-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 09:18:37.577997 workercontext-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 09:18:37.600998 workercontext-0.0.2/src/workercontext/
--rw-rw-rw-   0        0        0       37 2023-04-26 09:18:25.000000 workercontext-0.0.2/src/workercontext/__init__.py
--rw-rw-rw-   0        0        0     4254 2023-04-26 09:07:24.000000 workercontext-0.0.2/src/workercontext/multiworker.py
--rw-rw-rw-   0        0        0     4069 2023-04-26 08:33:40.000000 workercontext-0.0.2/src/workercontext/reductions.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:18:37.612995 workercontext-0.0.2/src/workercontext.egg-info/
--rw-rw-rw-   0        0        0     6061 2023-04-26 09:18:37.000000 workercontext-0.0.2/src/workercontext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-04-26 09:18:37.000000 workercontext-0.0.2/src/workercontext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:18:37.000000 workercontext-0.0.2/src/workercontext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 09:18:37.000000 workercontext-0.0.2/src/workercontext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 09:18:37.627995 workercontext-0.0.2/tests/
--rw-rw-rw-   0        0        0     2416 2023-04-26 09:07:46.000000 workercontext-0.0.2/tests/test_multiworker.py
--rw-rw-rw-   0        0        0     1291 2023-04-26 09:06:41.000000 workercontext-0.0.2/tests/test_performance.py
--rw-rw-rw-   0        0        0     2452 2023-04-26 09:06:54.000000 workercontext-0.0.2/tests/test_reduction.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.238947 workercontext-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-26 08:49:47.000000 workercontext-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6043 2023-04-26 09:52:39.235945 workercontext-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4179 2023-04-26 09:51:06.000000 workercontext-0.0.3/README.md
+-rw-rw-rw-   0        0        0      738 2023-04-26 09:50:36.000000 workercontext-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:52:39.238947 workercontext-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.181948 workercontext-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.203945 workercontext-0.0.3/src/workercontext/
+-rw-rw-rw-   0        0        0       37 2023-04-26 09:18:25.000000 workercontext-0.0.3/src/workercontext/__init__.py
+-rw-rw-rw-   0        0        0     4254 2023-04-26 09:07:24.000000 workercontext-0.0.3/src/workercontext/multiworker.py
+-rw-rw-rw-   0        0        0     4069 2023-04-26 08:33:40.000000 workercontext-0.0.3/src/workercontext/reductions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.216946 workercontext-0.0.3/src/workercontext.egg-info/
+-rw-rw-rw-   0        0        0     6043 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 09:52:39.000000 workercontext-0.0.3/src/workercontext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:39.232948 workercontext-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2416 2023-04-26 09:07:46.000000 workercontext-0.0.3/tests/test_multiworker.py
+-rw-rw-rw-   0        0        0     1291 2023-04-26 09:06:41.000000 workercontext-0.0.3/tests/test_performance.py
+-rw-rw-rw-   0        0        0     2452 2023-04-26 09:06:54.000000 workercontext-0.0.3/tests/test_reduction.py
```

### Comparing `workercontext-0.0.2/LICENSE` & `workercontext-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.2/PKG-INFO` & `workercontext-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workercontext
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package that provides a context to spin up multiple workers to execute a function
 Author-email: Owen Elliott <none@none.com>
 License: MIT License
         
         Copyright (c) 2023 Owen Elliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,78 +59,78 @@
 def my_func(arr: List[int]) -> List[int]:
     return [el*2 for el in arr]
 ```
 
 This can be simply split across multiple workers as follows:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8) as f:
+with MultiWorker(my_func, n_processes=8) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
 
-with workercontext(my_func, n_processes=8, reduction=reductions) as f:
+with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
     res = f(arr)
 print(res)
 ```
 
 This makes res be a single `float`.
 
 ### Using other parameters
 
 You can batch work on other parameters by specifying them in the constructor.
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 def my_func(l1: List[int], l2: List[int]) -> int:
     for i in range(len(l2)):
         for el1 in l1:
             l2[i] += el1
     return l2
 
 arr1 = list(range(100))
 arr2 = list(range(100))
 
-with workercontext(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
 # Documentation
 
-## workercontext
+## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
 + `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
 + `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
 ## Supported Reductions
```

### Comparing `workercontext-0.0.2/README.md` & `workercontext-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,78 +24,78 @@
 def my_func(arr: List[int]) -> List[int]:
     return [el*2 for el in arr]
 ```
 
 This can be simply split across multiple workers as follows:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8) as f:
+with MultiWorker(my_func, n_processes=8) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
 
-with workercontext(my_func, n_processes=8, reduction=reductions) as f:
+with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
     res = f(arr)
 print(res)
 ```
 
 This makes res be a single `float`.
 
 ### Using other parameters
 
 You can batch work on other parameters by specifying them in the constructor.
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 def my_func(l1: List[int], l2: List[int]) -> int:
     for i in range(len(l2)):
         for el1 in l1:
             l2[i] += el1
     return l2
 
 arr1 = list(range(100))
 arr2 = list(range(100))
 
-with workercontext(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
 # Documentation
 
-## workercontext
+## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
 + `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
 + `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
 ## Supported Reductions
```

### Comparing `workercontext-0.0.2/pyproject.toml` & `workercontext-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "workercontext"
-version = "0.0.2"
+version = "0.0.3"
 description = "A small package that provides a context to spin up multiple workers to execute a function"
 readme = "README.md"
 authors = [
   { name = "Owen Elliott", email = "none@none.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `workercontext-0.0.2/src/workercontext/multiworker.py` & `workercontext-0.0.3/src/workercontext/multiworker.py`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.2/src/workercontext/reductions.py` & `workercontext-0.0.3/src/workercontext/reductions.py`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.2/src/workercontext.egg-info/PKG-INFO` & `workercontext-0.0.3/src/workercontext.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workercontext
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package that provides a context to spin up multiple workers to execute a function
 Author-email: Owen Elliott <none@none.com>
 License: MIT License
         
         Copyright (c) 2023 Owen Elliott
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,78 +59,78 @@
 def my_func(arr: List[int]) -> List[int]:
     return [el*2 for el in arr]
 ```
 
 This can be simply split across multiple workers as follows:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8) as f:
+with MultiWorker(my_func, n_processes=8) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will be a list of lists of `ints` in this case, if you would like to reduce across all workers then you can pass a reduction:
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 arr = list(range(100))
 
-with workercontext(my_func, n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr)
 print(res)
 ```
 
 `res` will now a list of `int`.
 
 If you wanted to combine multiple reductions then you can use the reduction composition class
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import ReductionComposition, flatten_reduction, average_reduction
 
 reductions = ReductionComposition([flatten_reduction, average_reduction])
 
-with workercontext(my_func, n_processes=8, reduction=reductions) as f:
+with MultiWorker(my_func, n_processes=8, reduction=reductions) as f:
     res = f(arr)
 print(res)
 ```
 
 This makes res be a single `float`.
 
 ### Using other parameters
 
 You can batch work on other parameters by specifying them in the constructor.
 
 ```python
-from workercontext import workercontext
+from workercontext import MultiWorker
 from workercontext.reductions import flatten_reduction
 
 def my_func(l1: List[int], l2: List[int]) -> int:
     for i in range(len(l2)):
         for el1 in l1:
             l2[i] += el1
     return l2
 
 arr1 = list(range(100))
 arr2 = list(range(100))
 
-with workercontext(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
+with MultiWorker(my_func, batched_arg='l2', n_processes=8, reduction=flatten_reduction) as f:
     res = f(arr1, arr2)
 print(res)
 ```
 
 # Documentation
 
-## workercontext
+## MultiWorker
 ### parameters
 + `function` (`Callable`): The function to create the context for.
 + `n_processes` (`int`): The number of processes to spawn.
 + `batched_arg` (`str`, `optional`): The argument to batch on, if None the the first arg is used. Defaults to None.
 + `verbose` (`bool`, `optional`): Whether or not to print information about the processing. Defaults to False.
 + `reduction` (`Callable[[List[Any]], Any]`, `optional`): A reduction function to be applied across the outputs of the pool. Defaults to None.
 ## Supported Reductions
```

### Comparing `workercontext-0.0.2/tests/test_multiworker.py` & `workercontext-0.0.3/tests/test_multiworker.py`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.2/tests/test_performance.py` & `workercontext-0.0.3/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `workercontext-0.0.2/tests/test_reduction.py` & `workercontext-0.0.3/tests/test_reduction.py`

 * *Files identical despite different names*

