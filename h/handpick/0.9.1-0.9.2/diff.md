# Comparing `tmp/handpick-0.9.1-py3-none-any.whl.zip` & `tmp/handpick-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7436 bytes, number of entries: 6
--rw-r--r--  2.0 unx      434 b- defN 80-Jan-01 00:00 handpick/__init__.py
--rw-r--r--  2.0 unx     5871 b- defN 80-Jan-01 00:00 handpick/core.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 handpick-0.9.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 handpick-0.9.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11289 b- defN 16-Jan-01 00:00 handpick-0.9.1.dist-info/METADATA
-?rw-r--r--  2.0 unx      448 b- defN 16-Jan-01 00:00 handpick-0.9.1.dist-info/RECORD
-6 files, 19196 bytes uncompressed, 6634 bytes compressed:  65.4%
+Zip file size: 7506 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      463 b- defN 80-Jan-01 00:00 handpick/__init__.py
+-rw-r--r--  2.0 unx     5879 b- defN 80-Jan-01 00:00 handpick/core.py
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 handpick-0.9.2.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 handpick-0.9.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11510 b- defN 16-Jan-01 00:00 handpick-0.9.2.dist-info/METADATA
+?rw-r--r--  2.0 unx      448 b- defN 16-Jan-01 00:00 handpick-0.9.2.dist-info/RECORD
+6 files, 19454 bytes uncompressed, 6704 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: handpick/__init__.py
 Comment: 
 
 Filename: handpick/core.py
 Comment: 
 
-Filename: handpick-0.9.1.dist-info/LICENSE
+Filename: handpick-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: handpick-0.9.1.dist-info/WHEEL
+Filename: handpick-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: handpick-0.9.1.dist-info/METADATA
+Filename: handpick-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: handpick-0.9.1.dist-info/RECORD
+Filename: handpick-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## handpick/__init__.py

```diff
@@ -10,13 +10,20 @@
     not_type,
     IS_COLLECTION,
     IS_MAPPING,
     values_for_key,
     max_depth,
 )
 
-__version__ = '0.9.1'
+__version__ = "0.9.2"
 
 __all__ = [
-    '__version__', 'pick', 'Predicate', 'is_type', 'not_type',
-    'IS_COLLECTION', 'IS_MAPPING', 'values_for_key', 'max_depth'
+    "__version__",
+    "pick",
+    "Predicate",
+    "is_type",
+    "not_type",
+    "IS_COLLECTION",
+    "IS_MAPPING",
+    "values_for_key",
+    "max_depth",
 ]
```

## handpick/core.py

```diff
@@ -1,77 +1,76 @@
 from collections.abc import Mapping, Iterable
 
 _ERRORS = (TypeError, ValueError, IndexError, KeyError, AttributeError)
 
 
-def pick(data, predicate, collections=True, dict_keys=False, strings=False,
-         bytes_like=False):
+def pick(
+    data, predicate, collections=True, dict_keys=False, strings=False, bytes_like=False
+):
     """Pick objects from `data` based on `predicate`.
 
     Traverse `data` recursively and yield all objects for which
-    `predicate(obj)` is True or truthy.
+    `predicate(obj)` is True or truthy. `data` should be an iterable
+    collection. `predicate` should be a callable taking one argument
+    and returning a Boolean value.
 
-    `data` should be an iterable collection.
-
-    `predicate` should be a callable taking one argument and returning
-    a Boolean value. If `predicate` is not callable, equality will be
-    used as the picking criteria, i.e. objects for which
-    `obj == predicate` will be yielded.
+    If `predicate` is not callable, equality will be used as the picking
+    criteria, i.e. objects for which `obj == predicate` will be yielded.
 
     By default, collections of other objects are yielded just like any
-    other objects. To exclude collections, set `collections` to False.
+    other objects. To exclude collections, pass `collections=False`.
 
-    When traversing a mapping, only its values are inspected by
-    default. If `dict_keys` is set to True, both keys and values of the
-    mapping are inspected.
+    When traversing a mapping, only its values are inspected by default.
+    To inspect both keys and values of mappings, pass `dict_keys=True`.
 
     By default, strings are not treated as collections of other objects
     and therefore not iterated by the recursive algorithm. This can be
-    changed by setting `strings` to True. Strings of length 1 are never
+    changed by passing `strings=True`. Strings of length 1 are never
     iterated.
 
     By default, bytes-like sequences (bytes and bytearrays) are not
     treated as collections of other objects and therefore not iterated
-    by the recursive algorithm. This can be changed by setting
-    `bytes_like` to True.
+    by the recursive algorithm. This can be changed by passing
+    `bytes_like=True`.
     """
     if not isinstance(data, Iterable):
         return
     if isinstance(data, str) and (not strings or len(data) == 1):
         return
     if isinstance(data, (bytes, bytearray)) and not bytes_like:
         return
 
     is_mapping = IS_MAPPING(data)
     predicate_callable = callable(predicate)
     for obj in data:
         if is_mapping:
-            # key-value pair or just value
+            # (key, value) or just (value,)
             obj = (obj, data[obj]) if dict_keys else (data[obj],)
         elif collections or not IS_COLLECTION(obj):
+            # test object against predicate
             if predicate_callable:
                 if predicate(obj):
                     yield obj
             elif obj == predicate:
                 yield obj
-        yield from pick(
-            obj, predicate, collections, dict_keys, strings, bytes_like
-        )
+        # inspect object recursively
+        yield from pick(obj, predicate, collections, dict_keys, strings, bytes_like)
 
 
 class Predicate:
     """Decorator wrapping a function in a predicate object.
 
     The decorated function can be combined with other predicates using
     the operators `&` (and) and `|` (or), as well as negated using the
     operator `~` (not).
 
     Predicate objects are intended to be used as the `predicate`
     argument to the `pick` function.
     """
+
     def __init__(self, func):
         self.func = func
 
     def __call__(self, obj):
         try:
             return self.func(obj)
         except _ERRORS:
@@ -121,33 +120,36 @@
             return not self.func(obj)
 
         return self.from_function(fn)
 
 
 # predicate factories
 
+
 def is_type(type_or_types):
     """Predicate factory. Return a predicate that returns True if
     object is an instance of specified type(s).
 
     `type_or_types` must be a type or tuple of types.
     """
+
     @Predicate
     def new_predicate(obj):
         return isinstance(obj, type_or_types)
 
     return new_predicate
 
 
 def not_type(type_or_types):
     """Predicate factory. Return a predicate that returns True if
     object is not an instance of specified type(s).
 
     `type_or_types` must be a type or tuple of types.
     """
+
     @Predicate
     def new_predicate(obj):
         return not isinstance(obj, type_or_types)
 
     return new_predicate
 
 
@@ -160,20 +162,21 @@
 
 IS_MAPPING = is_type(Mapping)
 """Predicate that returns True for dictionaries and other mappings."""
 
 
 # useful functions
 
+
 def values_for_key(data, key):
     """Pick values associated with a specific key.
 
     Traverse `data` recursively and yield a sequence of dictionary
-    values that are mapped to `key`. A list of multiple keys can be
-    passed as the `key` argument.
+    values that are mapped to `key`. `key` may be a list of multiple
+    keys.
     """
     if not isinstance(key, list):
         key = [key]
 
     for mapping in pick([data], IS_MAPPING):
         for k in key:
             if k in mapping:
```

## Comparing `handpick-0.9.1.dist-info/LICENSE` & `handpick-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `handpick-0.9.1.dist-info/METADATA` & `handpick-0.9.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: handpick
-Version: 0.9.1
+Version: 0.9.2
 Summary: Inspect nested data structures.
 Home-page: https://github.com/mportesdev/handpick
 License: MIT
 Author: Michal Porteš
 Author-email: michalportes1@gmail.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6.2,<4.0.0
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 
-|tests| |coverage| |release| |license| |pyversions| |format| |downloads|
+|build| |coverage| |version| |pyversions| |license| |format| |downloads|
 
 ========
 Handpick
 ========
 
 Handpick is a tool to traverse nested data structures and pick all
 objects that meet certain criteria.
@@ -254,14 +254,23 @@
 
     >>> list(only_values)
     [0, '1', b'2']
 
 **Note:** Despite being iterable, strings and bytes-like objects are
 not treated as collections of other objects by ``IS_COLLECTION``.
 
+The same as above can be achieved by specifying the ``collections`` keyword
+argument to ``pick``:
+
+.. code::
+
+    >>> only_values = pick(data, lambda obj: True, collections=False)
+    >>> list(only_values)
+    [0, '1', b'2']
+
 
 Useful functions
 ----------------
 
 
 The ``values_for_key`` function
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -338,94 +347,124 @@
     >>> list(flat_data)
     [0, 1, 2, 3, 4, 5]
 
 
 API reference
 =============
 
-handpick.pick(data, predicate, collections=True, dict_keys=False, strings=False, bytes_like=False)
-    Pick objects from ``data`` based on ``predicate``.
+pick
+----
+
+*handpick.pick(data, predicate, collections=True, dict_keys=False, strings=False, bytes_like=False)*
+
+Pick objects from ``data`` based on ``predicate``.
+
+Traverse ``data`` recursively and yield all objects for which
+``predicate(obj)`` is True or truthy. ``data`` should be an iterable
+collection. ``predicate`` should be a callable taking one argument
+and returning a Boolean value.
+
+If ``predicate`` is not callable, equality will be used as the picking
+criteria, i.e. objects for which ``obj == predicate`` will be yielded.
+
+By default, collections of other objects are yielded just like any
+other objects. To exclude collections, pass ``collections=False``.
+
+When traversing a mapping, only its values are inspected by default.
+To inspect both keys and values of mappings, pass ``dict_keys=True``.
+
+By default, strings are not treated as collections of other objects
+and therefore not iterated by the recursive algorithm. This can be
+changed by passing ``strings=True``. Strings of length 1 are never
+iterated.
 
-    Traverse ``data`` recursively and yield all objects for which
-    ``predicate(obj)`` is True or truthy.
+By default, bytes-like sequences (bytes and bytearrays) are not
+treated as collections of other objects and therefore not iterated
+by the recursive algorithm. This can be changed by passing
+``bytes_like=True``.
 
-    ``data`` should be an iterable collection.
+Predicate
+---------
 
-    ``predicate`` should be a callable taking one argument and returning
-    a Boolean value. If ``predicate`` is not callable, equality will be
-    used as the picking criteria, i.e. objects for which
-    ``obj == predicate`` will be yielded.
+*@handpick.Predicate(func)*
 
-    By default, collections of other objects are yielded just like any
-    other objects. To exclude collections, set ``collections`` to False.
+Decorator wrapping a function in a predicate object.
 
-    When traversing a mapping, only its values are inspected by
-    default. If ``dict_keys`` is set to True, both keys and values of the
-    mapping are inspected.
+The decorated function can be combined with other predicates using
+the operators ``&`` (and) and ``|`` (or), as well as negated using the
+operator ``~`` (not).
 
-    By default, strings are not treated as collections of other objects
-    and therefore not iterated by the recursive algorithm. This can be
-    changed by setting ``strings`` to True. Strings of length 1 are never
-    iterated.
+Predicate objects are intended to be used as the ``predicate``
+argument to the ``pick`` function.
 
-    By default, bytes-like sequences (bytes and bytearrays) are not
-    treated as collections of other objects and therefore not iterated
-    by the recursive algorithm. This can be changed by setting
-    ``bytes_like`` to True.
+is_type
+-------
 
-@handpick.Predicate(func)
-    Decorator wrapping a function in a predicate object.
+*handpick.is_type(type_or_types)*
 
-    The decorated function can be combined with other predicates using
-    the operators ``&`` (and) and ``|`` (or), as well as negated using the
-    operator ``~`` (not).
+Predicate factory. Return a predicate that returns True if
+object is an instance of specified type(s).
 
-    Predicate objects are intended to be used as the ``predicate``
-    argument to the ``pick`` function.
+``type_or_types`` must be a type or tuple of types.
 
-handpick.is_type(type_or_types)
-    Predicate factory. Return a predicate that returns True if
-    object is an instance of specified type(s).
+not_type
+--------
 
-    ``type_or_types`` must be a type or tuple of types.
+*handpick.not_type(type_or_types)*
 
-handpick.not_type(type_or_types)
-    Predicate factory. Return a predicate that returns True if
-    object is not an instance of specified type(s).
+Predicate factory. Return a predicate that returns True if
+object is not an instance of specified type(s).
 
-    ``type_or_types`` must be a type or tuple of types.
+``type_or_types`` must be a type or tuple of types.
 
-handpick.IS_COLLECTION
-    Predicate that returns True for iterable collections of other
-    objects. Strings and bytes-like objects are not treated as collections.
+IS_COLLECTION
+-------------
 
-handpick.IS_MAPPING
-    Predicate that returns True for dictionaries and other mappings.
+*handpick.IS_COLLECTION*
 
-handpick.values_for_key(data, key)
-    Pick values associated with a specific key.
+Predicate that returns True for iterable collections of other
+objects. Strings and bytes-like objects are not treated as collections.
 
-    Traverse ``data`` recursively and yield a sequence of dictionary
-    values that are mapped to a dictionary key ``key``.
+IS_MAPPING
+----------
+
+*handpick.IS_MAPPING*
+
+Predicate that returns True for dictionaries and other mappings.
+
+values_for_key
+--------------
+
+*handpick.values_for_key(data, key)*
+
+Pick values associated with a specific key.
+
+Traverse ``data`` recursively and yield a sequence of dictionary
+values that are mapped to ``key``. ``key`` may be a list of multiple
+keys.
 
-handpick.max_depth(data)
-    Return maximum nested depth of ``data``.
+max_depth
+---------
 
-    ``data`` should be an iterable collection. Depth is counted from zero,
-    i.e. the direct elements of ``data`` are in depth 0.
+*handpick.max_depth(data)*
 
+Return maximum nested depth of ``data``.
 
-.. |tests| image:: https://github.com/mportesdev/handpick/actions/workflows/tests.yml/badge.svg
+``data`` should be an iterable collection. Depth is counted from zero,
+i.e. the direct elements of ``data`` are in depth 0.
+
+
+.. |build| image:: https://github.com/mportesdev/handpick/actions/workflows/build-test.yml/badge.svg
     :target: https://github.com/mportesdev/handpick/actions
 .. |coverage| image:: https://img.shields.io/codecov/c/gh/mportesdev/handpick
     :target: https://codecov.io/gh/mportesdev/handpick
-.. |release| image:: https://img.shields.io/github/v/release/mportesdev/handpick
-    :target: https://github.com/mportesdev/handpick/releases/latest
-.. |license| image:: https://img.shields.io/github/license/mportesdev/handpick
-    :target: https://github.com/mportesdev/handpick/blob/main/LICENSE
+.. |version| image:: https://img.shields.io/pypi/v/handpick
+    :target: https://pypi.org/project/handpick
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/handpick
     :target: https://pypi.org/project/handpick
+.. |license| image:: https://img.shields.io/github/license/mportesdev/handpick
+    :target: https://github.com/mportesdev/handpick/blob/main/LICENSE
 .. |format| image:: https://img.shields.io/pypi/format/handpick
     :target: https://pypi.org/project/handpick/#files
 .. |downloads| image:: https://pepy.tech/badge/handpick
     :target: https://pepy.tech/project/handpick
```

