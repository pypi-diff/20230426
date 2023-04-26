# Comparing `tmp/dyndesign-0.9.6.tar.gz` & `tmp/dyndesign-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyndesign-0.9.6.tar", max compression
+gzip compressed data, was "dyndesign-0.9.7.tar", max compression
```

## Comparing `dyndesign-0.9.6.tar` & `dyndesign-0.9.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12892 2023-04-18 10:57:56.029367 dyndesign-0.9.6/README.rst
--rw-r--r--   0        0        0      172 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/__init__.py
--rw-r--r--   0        0        0     7465 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/classmerger.py
--rw-r--r--   0        0        0      643 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/dynloader.py
--rw-r--r--   0        0        0     5948 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/dynmethod.py
--rw-r--r--   0        0        0     1512 2023-04-18 10:57:56.029367 dyndesign-0.9.6/dyndesign/singletonmeta.py
--rw-r--r--   0        0        0     1160 2023-04-18 10:57:56.029367 dyndesign-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    14254 1970-01-01 00:00:00.000000 dyndesign-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    13552 2023-04-26 08:04:11.677638 dyndesign-0.9.7/README.rst
+-rw-r--r--   0        0        0      172 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/__init__.py
+-rw-r--r--   0        0        0     7497 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/classmerger.py
+-rw-r--r--   0        0        0      643 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/dynloader.py
+-rw-r--r--   0        0        0     5948 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/dynmethod.py
+-rw-r--r--   0        0        0     1512 2023-04-26 08:04:11.677638 dyndesign-0.9.7/dyndesign/singletonmeta.py
+-rw-r--r--   0        0        0     1160 2023-04-26 08:04:11.677638 dyndesign-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    14914 1970-01-01 00:00:00.000000 dyndesign-0.9.7/PKG-INFO
```

### Comparing `dyndesign-0.9.6/README.rst` & `dyndesign-0.9.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     # Method `m2` of class `Base`
 
 
 When a merged class is instantiated with arguments, the constructor of each
 merging class is invoked, since constructors are excluded from being overloaded.
 Also, arguments passed to each constructor are adaptively filtered based on the
 constructor signature so that each constructor takes just the arguments it
-requires, and no exception is raised for exceeding or missing arguments passed:
+requires, and no exception is raised for exceeding arguments passed:
 
 .. code:: python
 
     class A:
         def __init__(self):
             print("No argument passed to class `A`")
 
@@ -137,18 +137,38 @@
     MergedClass("Alpha", "Beta", kw1="kwarg #1", kw2="kwarg #2")
 
     # No argument passed to class `A`
     # Argument a='Alpha' passed to class `B`
     # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
     # Argument kw2='kwarg #2' passed to class `D`
 
+On the other hand, if any required positional argument is missing, an exception
+is raised. If `MergedClass` of the above example is initialized with no
+parameters, and exception is raised when the constructor of class `B` is called:
+
+.. code:: python
+
+    ...
+    MergedClass()
+
+    # ...
+    # TypeError: B.__init__() missing 1 required positional argument: 'a'
+
+So as to have constructor instances with missing positional arguments silently
+skipped, `strict_merged_args` can be set to False in `mergeclasses`. In the
+above example, constructors of class `B` and `C` are skipped:
+
+.. code:: python
+
+    ...
+    MergedClass = mergeclasses(A, B, C, D, strict_merged_args=False)
     MergedClass()
 
     # No argument passed to class `A`
-    # Argument kw2='kwarg #2' passed to class `D`
+    # Argument kw2=None passed to class `D`
 
 
 It is also possible to extend the same behavior of the constructor ``__init__``
 (i.e., all the methods from all the merged classes are invoked rather than being
 overloaded by the same name method from the rightmost class) to other methods. A
 list of method names whose instances have to be all invoked can be specified in
 the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
```

### Comparing `dyndesign-0.9.6/dyndesign/classmerger.py` & `dyndesign-0.9.7/dyndesign/classmerger.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,26 +155,26 @@
     return [importclass(class_id) if type(class_id) == str else class_id for class_id in all_classes]
 
 
 def mergeclasses(
     base_class: Any,
     *extension_classes: Any,
     invoke_all: Union[List[str], None] = None,
-    strict_merged_args = False
+    strict_merged_args = True
 ) -> Type:
     """Merge (i.e., extend) a base class with one or more extension classes. If more than one extension classes are
     provided, then the classes are extended in sequence following the order of `extension_classes`.
 
     :param base_class: base class.
     :param extension_classes: extension classes.
     :param invoke_all: list of methods (in addition to `__init__`) whose instances are invoked (if present) from all
                        the merged classes, rather than being overloaded by the instance from the rightmost class.
     :param strict_merged_args: controls whether a `TypeError` exception is raised or not in case one or more positional
-                               arguments are missing in the `invoke_all` methods. It is set to True if an exception is
-                               raised, or False if the methods are silently skipped.
+                               arguments are missing in the `invoke_all` methods. If it is set to True (default value)
+                               an exception is raised, otherwise methods with missing arguments are silently skipped.
     :return: merged class.
     """
     all_classes = __preprocess_classes((base_class,) + extension_classes)
     invoke_all = ["__init__"] + (invoke_all or [])
     methods_not_oveloaded = {
         method: merged for method in invoke_all if (
             merged := __merge_not_overloaded(all_classes, method, strict_merged_args)
```

### Comparing `dyndesign-0.9.6/dyndesign/dynloader.py` & `dyndesign-0.9.7/dyndesign/dynloader.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.6/dyndesign/dynmethod.py` & `dyndesign-0.9.7/dyndesign/dynmethod.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.6/dyndesign/singletonmeta.py` & `dyndesign-0.9.7/dyndesign/singletonmeta.py`

 * *Files identical despite different names*

### Comparing `dyndesign-0.9.6/pyproject.toml` & `dyndesign-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dyndesign"
-version = "0.9.6"
+version = "0.9.7"
 description = "Toolset for Dynamic Design Patterns in Python."
 authors = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 maintainers = ["Patrizio Gelosi <patrizio.gelosi@amarulasolutions.com>"]
 repository = "https://github.com/amarula/dyndesign"
 license = "MIT"
 readme = "README.rst"
 keywords = ["design", "pattern", "dynamic", "decorator", "inheritance"]
```

### Comparing `dyndesign-0.9.6/PKG-INFO` & `dyndesign-0.9.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyndesign
-Version: 0.9.6
+Version: 0.9.7
 Summary: Toolset for Dynamic Design Patterns in Python.
 Home-page: https://github.com/amarula/dyndesign
 License: MIT
 Keywords: design,pattern,dynamic,decorator,inheritance
 Author: Patrizio Gelosi
 Author-email: patrizio.gelosi@amarulasolutions.com
 Maintainer: Patrizio Gelosi
@@ -141,15 +141,15 @@
     # Method `m2` of class `Base`
 
 
 When a merged class is instantiated with arguments, the constructor of each
 merging class is invoked, since constructors are excluded from being overloaded.
 Also, arguments passed to each constructor are adaptively filtered based on the
 constructor signature so that each constructor takes just the arguments it
-requires, and no exception is raised for exceeding or missing arguments passed:
+requires, and no exception is raised for exceeding arguments passed:
 
 .. code:: python
 
     class A:
         def __init__(self):
             print("No argument passed to class `A`")
 
@@ -169,18 +169,38 @@
     MergedClass("Alpha", "Beta", kw1="kwarg #1", kw2="kwarg #2")
 
     # No argument passed to class `A`
     # Argument a='Alpha' passed to class `B`
     # Argument a='Alpha', b='Beta' and kw1='kwarg #1' passed to class `C`
     # Argument kw2='kwarg #2' passed to class `D`
 
+On the other hand, if any required positional argument is missing, an exception
+is raised. If `MergedClass` of the above example is initialized with no
+parameters, and exception is raised when the constructor of class `B` is called:
+
+.. code:: python
+
+    ...
+    MergedClass()
+
+    # ...
+    # TypeError: B.__init__() missing 1 required positional argument: 'a'
+
+So as to have constructor instances with missing positional arguments silently
+skipped, `strict_merged_args` can be set to False in `mergeclasses`. In the
+above example, constructors of class `B` and `C` are skipped:
+
+.. code:: python
+
+    ...
+    MergedClass = mergeclasses(A, B, C, D, strict_merged_args=False)
     MergedClass()
 
     # No argument passed to class `A`
-    # Argument kw2='kwarg #2' passed to class `D`
+    # Argument kw2=None passed to class `D`
 
 
 It is also possible to extend the same behavior of the constructor ``__init__``
 (i.e., all the methods from all the merged classes are invoked rather than being
 overloaded by the same name method from the rightmost class) to other methods. A
 list of method names whose instances have to be all invoked can be specified in
 the ``invoke_all`` argument of ``mergeclasses``. Adaptive filtering of the
```

