# Comparing `tmp/clj-0.3.0.tar.gz` & `tmp/clj-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clj-0.3.0.tar", max compression
+gzip compressed data, was "clj-0.3.1.tar", max compression
```

## Comparing `clj-0.3.0.tar` & `clj-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-05-22 20:24:56.245362 clj-0.3.0/LICENSE
--rw-r--r--   0        0        0      638 2022-05-22 20:24:56.245362 clj-0.3.0/clj/__init__.py
--rw-r--r--   0        0        0     2406 2022-05-22 20:24:56.245362 clj-0.3.0/clj/fns.py
--rw-r--r--   0        0        0        0 2022-05-22 20:24:56.245362 clj-0.3.0/clj/py.typed
--rw-r--r--   0        0        0    19759 2022-05-22 20:24:56.249362 clj-0.3.0/clj/seqs.py
--rw-r--r--   0        0        0      409 2022-05-22 20:24:56.249362 clj-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      519 2022-05-22 20:27:48.674765 clj-0.3.0/setup.py
--rw-r--r--   0        0        0      422 2022-05-22 20:27:48.675091 clj-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-26 13:45:34.511186 clj-0.3.1/LICENSE
+-rw-r--r--   0        0        0    18671 2023-04-26 13:45:34.511186 clj-0.3.1/README.md
+-rw-r--r--   0        0        0      671 2023-04-26 13:45:34.511186 clj-0.3.1/clj/__init__.py
+-rw-r--r--   0        0        0     2406 2023-04-26 13:45:34.511186 clj-0.3.1/clj/fns.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:45:34.511186 clj-0.3.1/clj/py.typed
+-rw-r--r--   0        0        0    20964 2023-04-26 13:45:34.511186 clj-0.3.1/clj/seqs.py
+-rw-r--r--   0        0        0      499 2023-04-26 13:45:34.511186 clj-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    19352 1970-01-01 00:00:00.000000 clj-0.3.1/PKG-INFO
```

### Comparing `clj-0.3.0/LICENSE` & `clj-0.3.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2016-2022 – Baptiste Fontaine
+Copyright © 2016-2023 – Baptiste Fontaine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `clj-0.3.0/clj/fns.py` & `clj-0.3.1/clj/fns.py`

 * *Files identical despite different names*

### Comparing `clj-0.3.0/clj/seqs.py` & `clj-0.3.1/clj/seqs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: UTF-8 -*-
 import random
 import collections
 import itertools
 import collections.abc as collections_abc
 
-# We use this as a default value for some arguments in order to check if they
-# were provided or not
 from typing import Iterable, TypeVar, Any, Callable, Iterator, Union, Tuple, Dict, Optional, List, Set, cast, Deque
 
+import clj
+
+# We use this as a default value for some arguments in order to check if they
+# were provided or not
 _nil = object()
 
 # We redefine `range` below so keep a reference to the original one here
 _range = range
 
 T = TypeVar('T')
 T2 = TypeVar('T2')
 
 
 def _is_collection_abc(x):
     return isinstance(x, collections_abc.Sized) and \
-           isinstance(x, collections_abc.Iterable)
+        isinstance(x, collections_abc.Iterable)
 
 
 def _make_gen(g: Iterable[T]) -> Iterator[T]:
     for e in g:
         yield e
 
 
@@ -38,14 +40,15 @@
     for e in coll:
         if e not in seen:
             seen.add(e)
             yield e
 
 
 # alias
+# noinspection PyShadowingBuiltins
 filter = filter
 
 
 def remove(pred: Callable[[T], Any], coll: Iterable[T]) -> Iterable[T]:
     """
     Return a generator of the items in ``coll`` for which ``pred(item)``
     returns a falsy value.
@@ -71,33 +74,32 @@
         if res is not None:
             yield res
 
 
 def cons(x: T2, seq: Iterable[T]) -> Iterable[Union[T, T2]]:
     """
     Return a generator where ``x`` is the first element and ``seq`` is the
-    rest. Note, this differs from Clojure’s ``cons`` which returns a non-lazy
-    list.
+    rest. Note, this differs from Clojure’s ``cons`` which returns a non-lazy list.
     """
     yield x
     for e in seq:
         yield e
 
 
 def concat(*xs):
     """
-    Returns a generator representing the concatenation of the elements in the
-    supplied colls.
+    Returns a generator representing the concatenation of the elements in the supplied collections.
 
     This is equivalent to ``itertools.chain``.
     """
     return itertools.chain(*xs)
 
 
 # alias
+# noinspection PyShadowingBuiltins
 map = map
 
 
 def mapcat(f: Callable[[Any], Iterable], *colls):
     """
     Returns a generator representing the result of applying concat to the
     result of applying ``map`` to ``f`` and ``colls``. Thus function ``f``
@@ -614,26 +616,36 @@
     """
     kwargs = {}
     if n is not None:
         kwargs["times"] = n
     return itertools.repeat(x, **kwargs)
 
 
+# noinspection PyShadowingBuiltins
 def range(*args: int) -> Iterator[int]:
     """
     Usage: range()
            range(end)
            range(start, end)
            range(start, end, step)
 
     Returns a generator of numbers from ``start`` (inclusive) to ``end``
     (exclusive), by ``step``, where ``start`` defaults to ``0``, ``step`` to
     ``1``, and ``end`` to infinity. When ``step`` is equal to ``0``, returns an
     infinite sequence of ``start``.
 
+    This can be used to make an infinite int generator:
+
+        >>> import clj
+        >>> gen = iter(clj.range())
+        >>> next(gen)
+        0
+        >>> next(gen)
+        1
+
     Note that this delegates to Python’s built-in ``range`` if there are arguments.
     """
     if args:
         for e in _range(*args):
             yield e
         return
 
@@ -734,7 +746,45 @@
     if pad is not None and 0 < partition_index < partition_end:
         for pad_element in pad:
             current_partition.append(pad_element)
             if partition_index == partition_end:
                 break
 
         yield current_partition
+
+
+def partition_by(f: Callable[[T], Any], coll: Iterable[T]) -> Iterable[List[T]]:
+    current: List[T] = []
+    current_value = None
+    for element in coll:
+        if not current:
+            current_value = f(element)
+            current.append(element)
+            continue
+
+        value = f(element)
+        if value == current_value:
+            current.append(element)
+            continue
+
+        yield current
+        current = [element]
+        current_value = value
+
+    if current:
+        yield current
+
+
+def seq_gen(coll: Iterable[T]) -> Optional[Iterable[T]]:
+    """
+    Like Clojure’s ``seq``, but return a lazy iterable that’s equivalent to ``coll`` if not empty.
+
+    >>> seq_gen([])
+    None
+
+    >>> list(seq_gen([1, 2, 3]))
+    [1, 2, 3]
+    """
+    first_element, _is_empty = _first(coll)
+    if _is_empty:
+        return None
+    return clj.concat([first_element], _iter(coll, 1))
```

