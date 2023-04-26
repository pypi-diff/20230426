# Comparing `tmp/json_strong_typing-0.2.6.tar.gz` & `tmp/json_strong_typing-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_strong_typing-0.2.6.tar", last modified: Tue Mar 21 17:40:04 2023, max compression
+gzip compressed data, was "json_strong_typing-0.2.7.tar", last modified: Tue Apr 25 19:06:14 2023, max compression
```

## Comparing `json_strong_typing-0.2.6.tar` & `json_strong_typing-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-03-21 17:40:04.726790 json_strong_typing-0.2.6/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1171 2023-02-11 10:07:55.000000 json_strong_typing-0.2.6/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13643 2023-03-21 17:40:04.727112 json_strong_typing-0.2.6/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12794 2022-11-15 09:06:08.000000 json_strong_typing-0.2.6/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-03-21 17:40:04.699361 json_strong_typing-0.2.6/json_strong_typing.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13643 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      842 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       68 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       14 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-03-21 17:40:04.000000 json_strong_typing-0.2.6/json_strong_typing.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-06-20 22:11:24.000000 json_strong_typing-0.2.6/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1025 2023-03-21 17:40:04.728379 json_strong_typing-0.2.6/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-02-28 15:02:13.000000 json_strong_typing-0.2.6/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-03-21 17:40:04.715876 json_strong_typing-0.2.6/strong_typing/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      410 2023-03-21 17:35:26.000000 json_strong_typing-0.2.6/strong_typing/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4928 2023-02-11 09:40:56.000000 json_strong_typing-0.2.6/strong_typing/auxiliary.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      724 2023-02-22 07:54:00.000000 json_strong_typing-0.2.6/strong_typing/core.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    30619 2023-03-21 17:06:37.000000 json_strong_typing-0.2.6/strong_typing/deserializer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12538 2023-02-11 09:41:09.000000 json_strong_typing-0.2.6/strong_typing/docstring.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      476 2022-11-16 19:14:59.000000 json_strong_typing-0.2.6/strong_typing/exception.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    22356 2023-03-21 16:31:05.000000 json_strong_typing-0.2.6/strong_typing/inspection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1027 2022-11-18 23:10:53.000000 json_strong_typing-0.2.6/strong_typing/mapping.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4082 2022-11-16 19:15:14.000000 json_strong_typing-0.2.6/strong_typing/name.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25712 2023-02-11 09:41:30.000000 json_strong_typing-0.2.6/strong_typing/schema.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2827 2023-02-11 09:41:35.000000 json_strong_typing-0.2.6/strong_typing/serialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    14161 2023-02-11 09:41:41.000000 json_strong_typing-0.2.6/strong_typing/serializer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2747 2023-02-11 09:25:47.000000 json_strong_typing-0.2.6/strong_typing/topological.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-03-21 17:40:04.725759 json_strong_typing-0.2.6/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8918 2023-03-21 17:12:20.000000 json_strong_typing-0.2.6/tests/test_deserialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9966 2022-11-18 23:23:18.000000 json_strong_typing-0.2.6/tests/test_docstring.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9137 2023-02-11 09:26:42.000000 json_strong_typing-0.2.6/tests/test_inspection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1661 2023-02-11 09:27:08.000000 json_strong_typing-0.2.6/tests/test_name.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3056 2022-12-21 15:40:53.000000 json_strong_typing-0.2.6/tests/test_performance.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12204 2023-02-11 09:27:36.000000 json_strong_typing-0.2.6/tests/test_schema.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7152 2023-03-21 17:12:12.000000 json_strong_typing-0.2.6/tests/test_serialization.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2806 2023-02-11 09:28:23.000000 json_strong_typing-0.2.6/tests/test_topological.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:06:14.127942 json_strong_typing-0.2.7/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1171 2023-02-11 10:07:55.000000 json_strong_typing-0.2.7/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13666 2023-04-25 19:06:14.128288 json_strong_typing-0.2.7/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12794 2022-11-15 09:06:08.000000 json_strong_typing-0.2.7/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:06:14.079762 json_strong_typing-0.2.7/json_strong_typing.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13666 2023-04-25 19:06:14.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      987 2023-04-25 19:06:14.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-25 19:06:14.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       68 2023-04-25 19:06:14.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       14 2023-04-25 19:06:14.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-25 19:06:13.000000 json_strong_typing-0.2.7/json_strong_typing.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-22 08:15:05.000000 json_strong_typing-0.2.7/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1100 2023-04-25 19:06:14.129815 json_strong_typing-0.2.7/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-02-28 15:02:13.000000 json_strong_typing-0.2.7/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:06:14.099099 json_strong_typing-0.2.7/strong_typing/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      410 2023-03-29 22:01:28.000000 json_strong_typing-0.2.7/strong_typing/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5055 2023-04-21 21:53:17.000000 json_strong_typing-0.2.7/strong_typing/auxiliary.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      724 2023-02-22 07:54:00.000000 json_strong_typing-0.2.7/strong_typing/core.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    30683 2023-04-21 20:38:53.000000 json_strong_typing-0.2.7/strong_typing/deserializer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12946 2023-04-21 22:01:03.000000 json_strong_typing-0.2.7/strong_typing/docstring.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      476 2022-11-16 19:14:59.000000 json_strong_typing-0.2.7/strong_typing/exception.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    24076 2023-04-21 22:50:25.000000 json_strong_typing-0.2.7/strong_typing/inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1029 2023-04-21 22:50:41.000000 json_strong_typing-0.2.7/strong_typing/mapping.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4084 2023-04-21 22:49:15.000000 json_strong_typing-0.2.7/strong_typing/name.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:28:31.000000 json_strong_typing-0.2.7/strong_typing/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25630 2023-04-21 22:24:49.000000 json_strong_typing-0.2.7/strong_typing/schema.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2827 2023-04-21 23:07:38.000000 json_strong_typing-0.2.7/strong_typing/serialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    14161 2023-02-11 09:41:41.000000 json_strong_typing-0.2.7/strong_typing/serializer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      749 2023-04-21 20:51:57.000000 json_strong_typing-0.2.7/strong_typing/slots.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2758 2023-04-21 20:52:30.000000 json_strong_typing-0.2.7/strong_typing/topological.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:06:14.126953 json_strong_typing-0.2.7/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9271 2023-04-22 08:37:00.000000 json_strong_typing-0.2.7/tests/test_deserialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10370 2023-04-22 08:36:19.000000 json_strong_typing-0.2.7/tests/test_docstring.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9735 2023-04-22 08:37:03.000000 json_strong_typing-0.2.7/tests/test_inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1685 2023-04-21 22:50:49.000000 json_strong_typing-0.2.7/tests/test_name.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3069 2023-04-22 08:36:57.000000 json_strong_typing-0.2.7/tests/test_performance.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       43 2022-08-04 16:51:47.000000 json_strong_typing-0.2.7/tests/test_sample_exceptions.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4637 2023-04-21 20:53:31.000000 json_strong_typing-0.2.7/tests/test_sample_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12486 2023-04-22 08:37:06.000000 json_strong_typing-0.2.7/tests/test_schema.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7906 2023-04-22 08:37:09.000000 json_strong_typing-0.2.7/tests/test_serialization.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      783 2023-04-22 07:24:15.000000 json_strong_typing-0.2.7/tests/test_slots.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1203 2023-04-22 07:34:47.000000 json_strong_typing-0.2.7/tests/test_timer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2979 2023-04-21 20:58:01.000000 json_strong_typing-0.2.7/tests/test_topological.py
```

### Comparing `json_strong_typing-0.2.6/LICENSE` & `json_strong_typing-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.2.6/PKG-INFO` & `json_strong_typing-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_strong_typing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Type-safe data interchange for Python data classes
 Home-page: https://github.com/hunyadi/strong_typing
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Type-safe data interchange for Python
 
 JSON is a popular message interchange format employed in API design for its simplicity, readability, flexibility and wide support. However, `json.dump` and `json.load` offer no direct support when working with Python data classes employing type annotations. This package offers services for working with strongly-typed Python classes: serializing objects to JSON, deserializing JSON to objects, and producing a JSON schema that matches the data class, e.g. to be used in an OpenAPI specification.
```

### Comparing `json_strong_typing-0.2.6/README.md` & `json_strong_typing-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.2.6/json_strong_typing.egg-info/PKG-INFO` & `json_strong_typing-0.2.7/json_strong_typing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-strong-typing
-Version: 0.2.6
+Version: 0.2.7
 Summary: Type-safe data interchange for Python data classes
 Home-page: https://github.com/hunyadi/strong_typing
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Type-safe data interchange for Python
 
 JSON is a popular message interchange format employed in API design for its simplicity, readability, flexibility and wide support. However, `json.dump` and `json.load` offer no direct support when working with Python data classes employing type annotations. This package offers services for working with strongly-typed Python classes: serializing objects to JSON, deserializing JSON to objects, and producing a JSON schema that matches the data class, e.g. to be used in an OpenAPI specification.
```

### Comparing `json_strong_typing-0.2.6/json_strong_typing.egg-info/SOURCES.txt` & `json_strong_typing-0.2.7/json_strong_typing.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,25 @@
 strong_typing/core.py
 strong_typing/deserializer.py
 strong_typing/docstring.py
 strong_typing/exception.py
 strong_typing/inspection.py
 strong_typing/mapping.py
 strong_typing/name.py
+strong_typing/py.typed
 strong_typing/schema.py
 strong_typing/serialization.py
 strong_typing/serializer.py
+strong_typing/slots.py
 strong_typing/topological.py
 tests/test_deserialization.py
 tests/test_docstring.py
 tests/test_inspection.py
 tests/test_name.py
 tests/test_performance.py
+tests/test_sample_exceptions.py
+tests/test_sample_types.py
 tests/test_schema.py
 tests/test_serialization.py
+tests/test_slots.py
+tests/test_timer.py
 tests/test_topological.py
```

### Comparing `json_strong_typing-0.2.6/setup.cfg` & `json_strong_typing-0.2.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,24 @@
 	Topic :: Text Processing :: Markup :: reStructuredText
 	Typing :: Typed
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
+python_requires = >=3.8
 install_requires = 
 	jsonschema >= 4.17
 	typing_extensions >= 4.5; python_version<"3.10"
 
 [options.packages.find]
 exclude = 
 	tests*
 
+[options.package_data]
+strong_typing = 
+	py.typed
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `json_strong_typing-0.2.6/strong_typing/auxiliary.py` & `json_strong_typing-0.2.7/strong_typing/auxiliary.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 :see: https://github.com/hunyadi/strong_typing
 """
 
 import dataclasses
 import sys
 from dataclasses import dataclass
-from typing import Callable, Optional, Type, TypeVar, overload
+from typing import Callable, Dict, Optional, Type, TypeVar, Union, overload
 
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 T = TypeVar("T")
 
 
-def _compact_dataclass_repr(obj) -> str:
+def _compact_dataclass_repr(obj) -> str:  # type: ignore
     "Compact dataclass representation where positional arguments are used instead of keyword arguments."
 
     arglist = ", ".join(
         repr(getattr(obj, field.name)) for field in dataclasses.fields(obj)
     )
     return f"{obj.__class__.__name__}({arglist})"
 
@@ -46,15 +46,17 @@
 @overload
 def typeannotation(
     cls: None, *, eq: bool = True, order: bool = False
 ) -> Callable[[Type[T]], Type[T]]:
     ...
 
 
-def typeannotation(cls: Optional[Type[T]] = None, *, eq=True, order=False):
+def typeannotation(
+    cls: Optional[Type[T]] = None, *, eq: bool = True, order: bool = False
+) -> Union[Type[T], Callable[[Type[T]], Type[T]]]:
     "Returns the same class as was passed in, with dunder methods added based on the fields defined in the class."
 
     def wrap(cls: Type[T]) -> Type[T]:
         setattr(cls, "__repr__", _compact_dataclass_repr)
         if not dataclasses.is_dataclass(cls):
             cls = dataclasses.dataclass(  # type: ignore
                 cls,
@@ -114,15 +116,15 @@
 class Precision:
     "Precision of a floating-point value."
 
     significant_digits: int
     decimal_digits: int = 0
 
     @property
-    def integer_digits(self):
+    def integer_digits(self) -> int:
         return self.significant_digits - self.decimal_digits
 
 
 @typeannotation
 @dataclass(frozen=True)
 class TimePrecision:
     """
@@ -186,20 +188,20 @@
     IntegerRange(0, 18446744073709551615),
 ]
 
 float32: TypeAlias = Annotated[float, Storage(4)]
 float64: TypeAlias = Annotated[float, Storage(8)]
 
 # maps globals of type Annotated[T, ...] defined in this module to their string names
-_auxiliary_types = {}
+_auxiliary_types: Dict[object, str] = {}
 module = sys.modules[__name__]
 for var in dir(module):
     typ = getattr(module, var)
     if getattr(typ, "__metadata__", None) is not None:
         # type is Annotated[T, ...]
         _auxiliary_types[typ] = var
 
 
-def get_auxiliary_format(data_type: type) -> Optional[str]:
+def get_auxiliary_format(data_type: object) -> Optional[str]:
     "Returns the JSON format string corresponding to an auxiliary type."
 
     return _auxiliary_types.get(data_type)
```

### Comparing `json_strong_typing-0.2.6/strong_typing/core.py` & `json_strong_typing-0.2.7/strong_typing/core.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.2.6/strong_typing/deserializer.py` & `json_strong_typing-0.2.7/strong_typing/deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,15 +625,15 @@
             ]
             raise JsonKeyError(
                 f"unrecognized fields in JSON object: {unassigned_names}"
             )
 
         return self.create(**field_values)
 
-    def create(self, **field_values) -> T:
+    def create(self, **field_values) -> T:  # type: ignore
         "Instantiates an object with a collection of property values."
 
         obj: T = create_object(self.class_type)
 
         # use `setattr` on newly created object instance
         for field_name, field_value in field_values.items():
             setattr(obj, field_name, field_value)
@@ -648,25 +648,25 @@
             RequiredFieldDeserializer(
                 field_name, field_name, create_deserializer(field_type)
             )
             for field_name, field_type in get_resolved_hints(class_type).items()
         ]
         super().__init__(class_type, property_parsers)
 
-    def create(self, **field_values) -> NamedTuple:
+    def create(self, **field_values) -> NamedTuple:  # type: ignore
         return self.class_type(**field_values)
 
 
 class DataclassDeserializer(ClassDeserializer[T]):
     "De-serializes a data class from a JSON `object`."
 
     def __init__(self, class_type: Type[T]) -> None:
         property_parsers: List[FieldDeserializer] = []
         resolved_hints = get_resolved_hints(class_type)
-        for field in dataclasses.fields(class_type):
+        for field in dataclasses.fields(class_type):  # type: ignore
             field_type = resolved_hints[field.name]
             property_name = python_field_to_json_property(field.name, field_type)
 
             is_optional = is_type_optional(field_type)
             has_default = field.default is not dataclasses.MISSING
             has_default_factory = field.default_factory is not dataclasses.MISSING
 
@@ -699,15 +699,15 @@
 
         super().__init__(class_type, property_parsers)
 
 
 class FrozenDataclassDeserializer(DataclassDeserializer[T]):
     "De-serializes a frozen data class from a JSON `object`."
 
-    def create(self, **field_values) -> T:
+    def create(self, **field_values) -> T:  # type: ignore
         "Instantiates an object with a collection of property values."
 
         # create object instance without calling `__init__`
         obj: T = create_object(self.class_type)
 
         # can't use `setattr` on frozen dataclasses, pass member variable values to `__init__`
         obj.__init__(**field_values)  # type: ignore
```

### Comparing `json_strong_typing-0.2.6/strong_typing/docstring.py` & `json_strong_typing-0.2.7/strong_typing/docstring.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 """
 
 import builtins
 import dataclasses
 import inspect
 import re
 import types
+import typing
 from dataclasses import dataclass
 from io import StringIO
-from typing import Any, Callable, Dict, Optional, Type
+from typing import Any, Callable, Dict, Optional, Protocol, Type
 
 from .inspection import (
     get_class_properties,
     get_signature,
     is_dataclass_type,
     is_type_enum,
 )
@@ -149,15 +150,19 @@
     )
     return {
         name: class_type
         for name, class_type in inspect.getmembers(module, is_exception)
     }
 
 
-def parse_type(typ: type) -> Docstring:
+class SupportsDoc(Protocol):
+    __doc__: Optional[str]
+
+
+def parse_type(typ: SupportsDoc) -> Docstring:
     """
     Parse the docstring of a type into its components.
 
     :param typ: The type whose documentation string to parse.
     :returns: Components of the documentation string.
     """
 
@@ -166,15 +171,15 @@
         return Docstring()
 
     docstring = parse_text(doc)
     check_docstring(typ, docstring)
 
     # assign parameter and return types
     if is_dataclass_type(typ):
-        properties = dict(get_class_properties(typ))
+        properties = dict(get_class_properties(typing.cast(type, typ)))
 
         for name, param in docstring.params.items():
             param.param_type = properties[name]
 
     elif inspect.isfunction(typ):
         signature = get_signature(typ)
         for name, param in docstring.params.items():
@@ -184,22 +189,27 @@
 
     # assign exception types
     defining_module = inspect.getmodule(typ)
     if defining_module:
         context: Dict[str, type] = {}
         context.update(get_exceptions(builtins))
         context.update(get_exceptions(defining_module))
-        for name, exception in docstring.raises.items():
-            raise_type = context.get(name)
+        for exc_name, exc in docstring.raises.items():
+            raise_type = context.get(exc_name)
             if raise_type is None:
+                type_name = (
+                    getattr(typ, "__qualname__", None)
+                    or getattr(typ, "__name__", None)
+                    or None
+                )
                 raise TypeError(
-                    f"doc-string exception type `{name}` is not an exception defined in the context of `{typ.__qualname__}`"
+                    f"doc-string exception type `{exc_name}` is not an exception defined in the context of `{type_name}`"
                 )
 
-            exception.raise_type = raise_type
+            exc.raise_type = raise_type
 
     return docstring
 
 
 def parse_text(text: str) -> Docstring:
     """
     Parse a ReST-style docstring into its components.
@@ -270,56 +280,61 @@
         short_description=short_description,
         params=params,
         returns=returns,
         raises=raises,
     )
 
 
-def has_default_docstring(typ: type) -> bool:
+def has_default_docstring(typ: SupportsDoc) -> bool:
     "Check if class has the auto-generated string assigned by @dataclass."
 
-    return (
-        is_dataclass_type(typ)
-        and typ.__doc__ is not None
-        and re.match(f"^{re.escape(typ.__name__)}[(].*[)]$", typ.__doc__) is not None
-    ) or (
-        is_type_enum(typ)
-        and typ.__doc__ is not None
-        and typ.__doc__ == "An enumeration."
-    )
+    if not isinstance(typ, type):
+        return False
+
+    if is_dataclass_type(typ):
+        return (
+            typ.__doc__ is not None
+            and re.match(f"^{re.escape(typ.__name__)}[(].*[)]$", typ.__doc__)
+            is not None
+        )
+
+    if is_type_enum(typ):
+        return typ.__doc__ is not None and typ.__doc__ == "An enumeration."
+
+    return False
 
 
-def has_docstring(typ: type) -> bool:
+def has_docstring(typ: SupportsDoc) -> bool:
     "Check if class has a documentation string other than the auto-generated string assigned by @dataclass."
 
     if has_default_docstring(typ):
         return False
 
     return bool(typ.__doc__)
 
 
-def get_docstring(typ: type) -> Optional[str]:
+def get_docstring(typ: SupportsDoc) -> Optional[str]:
     if typ.__doc__ is None:
         return None
 
     if has_default_docstring(typ):
         return None
 
     return typ.__doc__
 
 
-def check_docstring(typ: type, docstring: Docstring, strict: bool = False) -> None:
+def check_docstring(typ: object, docstring: Docstring, strict: bool = False) -> None:
     """
     Verifies the doc-string of a type.
 
     :raises TypeError: Raised on a mismatch between doc-string parameters, and function or type signature.
     """
 
     if is_dataclass_type(typ):
-        check_dataclass_docstring(typ, docstring, strict)
+        check_dataclass_docstring(typ, docstring, strict)  # type: ignore
     elif inspect.isfunction(typ):
         check_function_docstring(typ, docstring, strict)
 
 
 def check_dataclass_docstring(
     typ: type, docstring: Docstring, strict: bool = False
 ) -> None:
```

### Comparing `json_strong_typing-0.2.6/strong_typing/inspection.py` & `json_strong_typing-0.2.7/strong_typing/inspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,41 +40,68 @@
 
 S = TypeVar("S")
 T = TypeVar("T")
 K = TypeVar("K")
 V = TypeVar("V")
 
 
-def is_dataclass_type(typ) -> bool:
+def is_type_like(data_type: object) -> bool:
+    """
+    Checks if the object is a type or type-like object (e.g. generic type).
+
+    :param data_type: The object to validate.
+    :returns: True if the object is a type or type-like object.
+    """
+
+    if isinstance(data_type, type):
+        # a standard type
+        return True
+    elif typing.get_origin(data_type) is not None:
+        # a generic type such as `list`, `dict` or `set`
+        return True
+    elif hasattr(data_type, "__forward_arg__"):
+        # an instance of `ForwardRef`
+        return True
+    elif data_type is Any:
+        # the special form `Any`
+        return True
+    else:
+        return False
+
+
+def is_dataclass_type(typ: Any) -> bool:
     "True if the argument corresponds to a data class type (but not an instance)."
 
     typ = unwrap_annotated_type(typ)
     return isinstance(typ, type) and dataclasses.is_dataclass(typ)
 
 
-def is_dataclass_instance(obj) -> bool:
+def is_dataclass_instance(obj: Any) -> bool:
     "True if the argument corresponds to a data class instance (but not a type)."
 
     return not isinstance(obj, type) and dataclasses.is_dataclass(obj)
 
 
-def is_named_tuple_instance(obj: object) -> TypeGuard[NamedTuple]:
+def is_named_tuple_instance(obj: Any) -> TypeGuard[NamedTuple]:
     "True if the argument corresponds to a named tuple instance."
 
     return is_named_tuple_type(type(obj))
 
 
-def is_named_tuple_type(typ: Type[T]) -> TypeGuard[Type[NamedTuple]]:
+def is_named_tuple_type(typ: Any) -> TypeGuard[Type[NamedTuple]]:
     """
     True if the argument corresponds to a named tuple type.
 
     Calling the function `collections.namedtuple` gives a new type that is a subclass of `tuple` (and no other classes)
     with a member named `_fields` that is a tuple whose items are all strings.
     """
 
+    if not isinstance(typ, type):
+        return False
+
     typ = unwrap_annotated_type(typ)
 
     b = getattr(typ, "__bases__", None)
     if b is None:
         return False
 
     if len(b) != 1 or b[0] != tuple:
@@ -83,44 +110,60 @@
     f = getattr(typ, "_fields", None)
     if not isinstance(f, tuple):
         return False
 
     return all(type(n) == str for n in f)
 
 
-def is_type_enum(typ: type) -> TypeGuard[Type[enum.Enum]]:
-    "True if the specified type is an enumeration type."
+if sys.version_info >= (3, 11):
 
-    typ = unwrap_annotated_type(typ)
+    def is_type_enum(typ: object) -> TypeGuard[Type[enum.Enum]]:
+        "True if the specified type is an enumeration type."
 
-    if sys.version_info >= (3, 11):
+        typ = unwrap_annotated_type(typ)
         return isinstance(typ, enum.EnumType)
-    else:
+
+else:
+
+    def is_type_enum(typ: object) -> TypeGuard[Type[enum.Enum]]:
+        "True if the specified type is an enumeration type."
+
+        typ = unwrap_annotated_type(typ)
+
         # use an explicit isinstance(..., type) check to filter out special forms like generics
         return isinstance(typ, type) and issubclass(typ, enum.Enum)
 
 
 def enum_value_types(enum_type: Type[enum.Enum]) -> List[type]:
     """
     Returns all unique value types of the `enum.Enum` type in definition order.
     """
 
     # filter unique enumeration value types by keeping definition order
     return list(dict.fromkeys(type(e.value) for e in enum_type))
 
 
-def _is_union_like(typ: type) -> bool:
-    "True if type is a union such as `Union[T1, T2, ...]` or a union type `T1 | T2`."
+if sys.version_info >= (3, 10):
+
+    def _is_union_like(typ: object) -> bool:
+        "True if type is a union such as `Union[T1, T2, ...]` or a union type `T1 | T2`."
+
+        return typing.get_origin(typ) is Union or isinstance(typ, types.UnionType)
+
+else:
+
+    def _is_union_like(typ: object) -> bool:
+        "True if type is a union such as `Union[T1, T2, ...]` or a union type `T1 | T2`."
 
-    is_generic_union = typing.get_origin(typ) is Union
-    is_union_expr = sys.version_info >= (3, 10) and isinstance(typ, types.UnionType)
-    return is_generic_union or is_union_expr
+        return typing.get_origin(typ) is Union
 
 
-def is_type_optional(typ: type, strict: bool = False) -> TypeGuard[Type[Optional[Any]]]:
+def is_type_optional(
+    typ: object, strict: bool = False
+) -> TypeGuard[Type[Optional[Any]]]:
     """
     True if the type annotation corresponds to an optional type (e.g. `Optional[T]` or `Union[T1,T2,None]`).
 
     `Optional[T]` is represented as `Union[T, None]` is classic style, and is equivalent to `T | None` in new style.
 
     :param strict: True if only `Optional[T]` qualifies as an optional type but `Union[T1, T2, None]` does not.
     """
@@ -157,44 +200,43 @@
 
     # will automatically unwrap Union[T] into T
     return Union[
         tuple(filter(lambda item: item is not type(None), typing.get_args(typ)))  # type: ignore
     ]
 
 
-def is_type_union(typ: type) -> bool:
+def is_type_union(typ: object) -> bool:
     "True if the type annotation corresponds to a union type (e.g. `Union[T1,T2,T3]`)."
 
     typ = unwrap_annotated_type(typ)
 
     if _is_union_like(typ):
         args = typing.get_args(typ)
         return len(args) > 2 or type(None) not in args
 
     return False
 
 
-def unwrap_union_types(typ: type) -> Tuple[type, ...]:
+def unwrap_union_types(typ: object) -> Tuple[object, ...]:
     """
     Extracts the inner types of a union type.
 
     :param typ: The union type `Union[T1, T2, ...]`.
     :returns: The inner types `T1`, `T2`, etc.
     """
 
     return _unwrap_union_types(typ)
 
 
-def _unwrap_union_types(typ: type) -> Tuple[type, ...]:
+def _unwrap_union_types(typ: object) -> Tuple[object, ...]:
     "Extracts the types in a union (e.g. returns a tuple of types `T1` and `T2` for `Union[T1, T2]`)."
 
-    if typing.get_origin(typ) is not Union:
+    if not _is_union_like(typ):
         raise TypeError("union type must have un-subscripted type of Union")
 
-    # will automatically unwrap Union[T] into T
     return typing.get_args(typ)
 
 
 def is_type_literal(typ: type) -> bool:
     "True if the specified type is a literal of one or more constant values, e.g. `Literal['string']` or `Literal[42]`."
 
     typ = unwrap_annotated_type(typ)
@@ -235,15 +277,15 @@
     :param typ: The literal type `Literal[value, ...]`.
     :returns: A tuple of item types `T` such that `type(value) == T`.
     """
 
     return tuple(type(t) for t in unwrap_literal_values(typ))
 
 
-def is_generic_list(typ: type) -> TypeGuard[Type[list]]:
+def is_generic_list(typ: object) -> TypeGuard[Type[list]]:
     "True if the specified type is a generic list, i.e. `List[T]`."
 
     typ = unwrap_annotated_type(typ)
     return typing.get_origin(typ) is list
 
 
 def unwrap_generic_list(typ: Type[List[T]]) -> Type[T]:
@@ -260,15 +302,15 @@
 def _unwrap_generic_list(typ: Type[List[T]]) -> Type[T]:
     "Extracts the item type of a list type (e.g. returns `T` for `List[T]`)."
 
     (list_type,) = typing.get_args(typ)  # unpack single tuple element
     return list_type
 
 
-def is_generic_dict(typ: type) -> TypeGuard[Type[dict]]:
+def is_generic_dict(typ: object) -> TypeGuard[Type[dict]]:
     "True if the specified type is a generic dictionary, i.e. `Dict[KeyType, ValueType]`."
 
     typ = unwrap_annotated_type(typ)
     return typing.get_origin(typ) is dict
 
 
 def unwrap_generic_dict(typ: Type[Dict[K, V]]) -> Tuple[Type[K], Type[V]]:
@@ -285,21 +327,21 @@
 def _unwrap_generic_dict(typ: Type[Dict[K, V]]) -> Tuple[Type[K], Type[V]]:
     "Extracts the key and value types of a dict type (e.g. returns (`K`, `V`) for `Dict[K, V]`)."
 
     key_type, value_type = typing.get_args(typ)
     return key_type, value_type
 
 
-def is_type_annotated(typ: type) -> bool:
+def is_type_annotated(typ: object) -> bool:
     "True if the type annotation corresponds to an annotated type (i.e. `Annotated[T, ...]`)."
 
     return getattr(typ, "__metadata__", None) is not None
 
 
-def get_annotation(data_type: type, annotation_type: Type[T]) -> Optional[T]:
+def get_annotation(data_type: object, annotation_type: Type[T]) -> Optional[T]:
     """
     Returns the first annotation on a data type that matches the expected annotation type.
 
     :param data_type: The annotated type from which to extract the annotation.
     :param annotation_type: The annotation class to look for.
     :returns: The annotation class instance found (if any).
     """
@@ -309,15 +351,15 @@
         for annotation in metadata:
             if isinstance(annotation, annotation_type):
                 return annotation
 
     return None
 
 
-def unwrap_annotated_type(typ: Type[T]) -> Type[T]:
+def unwrap_annotated_type(typ: T) -> T:
     "Extracts the wrapped type from an annotated type (e.g. returns `T` for `Annotated[T, ...]`)."
 
     if is_type_annotated(typ):
         # type is Annotated[T, ...]
         return typing.get_args(typ)[0]
     else:
         # type is a regular type
@@ -355,18 +397,22 @@
 
     is_class_member = (
         lambda member: inspect.isclass(member) and member.__module__ == module.__name__
     )
     return [class_type for _, class_type in inspect.getmembers(module, is_class_member)]
 
 
-def get_resolved_hints(typ: type) -> Dict[str, type]:
-    if sys.version_info >= (3, 9):
+if sys.version_info >= (3, 9):
+
+    def get_resolved_hints(typ: type) -> Dict[str, type]:
         return typing.get_type_hints(typ, include_extras=True)
-    else:
+
+else:
+
+    def get_resolved_hints(typ: type) -> Dict[str, type]:
         return typing.get_type_hints(typ)
 
 
 def get_class_properties(typ: type) -> Iterable[Tuple[str, type]]:
     "Returns all properties of a class."
 
     if is_dataclass_type(typ):
@@ -381,46 +427,55 @@
 
     for property_name, property_type in get_class_properties(typ):
         if name == property_name:
             return property_type
     return None
 
 
-def get_referenced_types(typ: type) -> List[type]:
+def get_referenced_types(typ: object) -> List[type]:
     """
     Extracts types indirectly referenced by this type.
 
     For example, extract `T` from `List[T]`, `Optional[T]` or `Annotated[T, ...]`, `K` and `V` from `Dict[K,V]`,
     `A` and `B` from `Union[A,B]`.
+
+    :param typ: A type or special form.
+    :returns: Types referenced by the given type or special form.
     """
 
     metadata = getattr(typ, "__metadata__", None)
     if metadata is not None:
         # type is Annotated[T, ...]
         arg = typing.get_args(typ)[0]
         return get_referenced_types(arg)
 
     # type is a regular type
     result = []
     origin = typing.get_origin(typ)
     if origin is not None:
         for arg in typing.get_args(typ):
             result.extend(get_referenced_types(arg))
-    elif typ is not type(None):
+    elif isinstance(typ, type) and typ is not type(None):
         result.append(typ)
 
     return result
 
 
-def get_signature(fn: Callable[..., Any]) -> inspect.Signature:
-    "Extracts the signature of a function."
+if sys.version_info >= (3, 10):
+
+    def get_signature(fn: Callable[..., Any]) -> inspect.Signature:
+        "Extracts the signature of a function."
 
-    if sys.version_info >= (3, 10):
         return inspect.signature(fn, eval_str=True)
-    else:
+
+else:
+
+    def get_signature(fn: Callable[..., Any]) -> inspect.Signature:
+        "Extracts the signature of a function."
+
         return inspect.signature(fn)
 
 
 def is_reserved_property(name: str) -> bool:
     "True if the name stands for an internal property."
 
     # filter built-in and special properties
@@ -430,27 +485,39 @@
     # filter built-in special names
     if name in ["_abc_impl"]:
         return True
 
     return False
 
 
-def create_data_type(class_name: str, fields: List[Tuple[str, type]]) -> type:
-    """
-    Creates a new data-class type dynamically.
+if sys.version_info >= (3, 10):
 
-    :param class_name: The name of new data-class type.
-    :param fields: A list of fields (and their type) that the new data-class type is expected to have.
-    :returns: The newly created data-class type.
-    """
+    def create_data_type(class_name: str, fields: List[Tuple[str, type]]) -> type:
+        """
+        Creates a new data-class type dynamically.
+
+        :param class_name: The name of new data-class type.
+        :param fields: A list of fields (and their type) that the new data-class type is expected to have.
+        :returns: The newly created data-class type.
+        """
 
-    if sys.version_info >= (3, 10):
         # has the `slots` parameter
-        cls = dataclasses.make_dataclass(class_name, fields, slots=True)
-    else:
+        return dataclasses.make_dataclass(class_name, fields, slots=True)
+
+else:
+
+    def create_data_type(class_name: str, fields: List[Tuple[str, type]]) -> type:
+        """
+        Creates a new data-class type dynamically.
+
+        :param class_name: The name of new data-class type.
+        :param fields: A list of fields (and their type) that the new data-class type is expected to have.
+        :returns: The newly created data-class type.
+        """
+
         cls = dataclasses.make_dataclass(class_name, fields)
 
         cls_dict = dict(cls.__dict__)
         field_names = tuple(field.name for field in dataclasses.fields(cls))
 
         cls_dict["__slots__"] = field_names
 
@@ -459,29 +526,29 @@
         cls_dict.pop("__dict__", None)
 
         qualname = getattr(cls, "__qualname__", None)
         cls = type(cls)(cls.__name__, (), cls_dict)
         if qualname is not None:
             cls.__qualname__ = qualname
 
-    return cls
+        return cls
 
 
 def create_object(typ: Type[T]) -> T:
     "Creates an instance of a type."
 
     if issubclass(typ, Exception):
         # exception types need special treatment
         e = typ.__new__(typ)
         return typing.cast(T, e)
     else:
         return object.__new__(typ)
 
 
-def is_generic_instance(obj: Any, typ: type) -> bool:
+def is_generic_instance(obj: Any, typ: object) -> bool:
     """
     Returns whether an object is an instance of a generic class, a standard class or of a subclass thereof.
 
     This function checks the following items recursively:
     * items of a list
     * keys and values of a dictionary
     * members of a set
@@ -649,15 +716,15 @@
             return all(
                 self.check(property_type, getattr(obj, property_name))
                 for property_name, property_type in get_class_properties(typ)
             )
 
 
 def check_recursive(
-    obj: Any,
+    obj: T,
     /,
     *,
     pred: Optional[Callable[[Type[T], T], bool]] = None,
     type_pred: Optional[Callable[[Type[T]], bool]] = None,
     value_pred: Optional[Callable[[T], bool]] = None,
 ) -> bool:
     """
```

### Comparing `json_strong_typing-0.2.6/strong_typing/mapping.py` & `json_strong_typing-0.2.7/strong_typing/mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 
 from .auxiliary import Alias
 from .inspection import get_annotation
 
 
 def python_field_to_json_property(
-    python_id: str, python_type: Optional[type] = None
+    python_id: str, python_type: Optional[object] = None
 ) -> str:
     """
     Map a Python field identifier to a JSON property name.
 
     Authors may use an underscore appended at the end of a Python identifier as per PEP 8 if it clashes with a Python
     keyword: e.g. `in` would become `in_` and `from` would become `from_`. Remove these suffixes when exporting to JSON.
```

### Comparing `json_strong_typing-0.2.6/strong_typing/name.py` & `json_strong_typing-0.2.7/strong_typing/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         args = ", ".join(repr(m) for m in metadata)
         return f"Annotated[{s}, {args}]"
     else:
         # type is a regular type
         return _python_type_to_str(data_type)
 
 
-def python_type_to_name(data_type: type, force: bool = False) -> str:
+def python_type_to_name(data_type: object, force: bool = False) -> str:
     """
     Returns the short name of a Python type.
 
     :param force: Whether to produce a name for composite types such as generics.
     """
 
     # use compact name for alias types
```

### Comparing `json_strong_typing-0.2.6/strong_typing/schema.py` & `json_strong_typing-0.2.7/strong_typing/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,51 +42,40 @@
 )
 from .core import JsonArray, JsonObject, JsonType, Schema, StrictJsonType
 from .inspection import (
     enum_value_types,
     get_annotation,
     get_class_properties,
     is_type_enum,
+    is_type_like,
     is_type_optional,
     unwrap_optional_type,
 )
 from .name import python_type_to_name
 from .serialization import object_to_json
 
 # determines the maximum number of distinct enum members up to which a Dict[EnumType, Any] is converted into a JSON
 # schema with explicitly listed properties (rather than employing a pattern constraint on property names)
 OBJECT_ENUM_EXPANSION_LIMIT = 4
 
 
 T = TypeVar("T")
 
 
-def check_type(data_type: type) -> None:
+def check_type(data_type: object) -> None:
     """
     Checks if the object is a type or type-like object (e.g. generic type).
 
     :param data_type: The object to validate.
     """
 
-    if isinstance(data_type, type):
-        # a standard type
-        return
-    elif typing.get_origin(data_type) is not None:
-        # a generic type such as `list`, `dict` or `set`
-        return
-    elif hasattr(data_type, "__forward_arg__"):
-        # an instance of `ForwardRef`
-        return
-    elif data_type is Any:
-        # the special form `Any`
-        return
-
-    raise TypeError(
-        f"expected a type but got an instance of {type(data_type)}: {data_type}"
-    )
+    if not is_type_like(data_type):
+        raise TypeError(
+            f"expected a type but got an instance of {type(data_type)}: {data_type}"
+        )
 
 
 def get_class_docstrings(data_type: type) -> Tuple[Optional[str], Optional[str]]:
     check_type(data_type)
     docstr = docstring.parse_type(data_type)
 
     # check if class has a doc-string other than the auto-generated string assigned by @dataclass
@@ -167,48 +156,47 @@
     identifier: str
     examples: Optional[JsonType] = None
 
 
 class TypeCatalog:
     "Maintains an association of well-known Python types to their JSON schema."
 
-    _by_type: Dict[type, TypeCatalogEntry]
+    _by_type: Dict[object, TypeCatalogEntry]
     _by_name: Dict[str, TypeCatalogEntry]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._by_type = {}
         self._by_name = {}
 
-    def __contains__(self, data_type: type) -> bool:
+    def __contains__(self, data_type: object) -> bool:
         if isinstance(data_type, typing.ForwardRef):
             fwd: typing.ForwardRef = data_type
             name = fwd.__forward_arg__
             return name in self._by_name
         else:
             return data_type in self._by_type
 
     def add(
         self,
-        data_type: type,
+        data_type: object,
         schema: Optional[Schema],
         identifier: str,
         examples: Optional[List[JsonType]] = None,
     ) -> None:
-
         if isinstance(data_type, typing.ForwardRef):
             raise TypeError("forward references cannot be used to register a type")
 
         if data_type in self._by_type:
             raise ValueError(f"type {data_type} is already registered in the catalog")
 
         entry = TypeCatalogEntry(schema, identifier, examples)
         self._by_type[data_type] = entry
         self._by_name[identifier] = entry
 
-    def get(self, data_type: type) -> TypeCatalogEntry:
+    def get(self, data_type: object) -> TypeCatalogEntry:
         if isinstance(data_type, typing.ForwardRef):
             fwd: typing.ForwardRef = data_type
             name = fwd.__forward_arg__
             return self._by_name[name]
         else:
             return self._by_type[data_type]
 
@@ -221,26 +209,26 @@
     property_description_fun: Optional[Callable[[type, str, str], str]] = None
 
 
 class JsonSchemaGenerator:
     "Creates a JSON schema with user-defined type definitions."
 
     type_catalog: ClassVar[TypeCatalog] = TypeCatalog()
-    types_used: Dict[str, type]
+    types_used: Dict[str, object]
     options: SchemaOptions
 
     def __init__(self, options: Optional[SchemaOptions] = None):
         if options is None:
             self.options = SchemaOptions()
         else:
             self.options = options
         self.types_used = {}
 
     @functools.singledispatchmethod
-    def _metadata_to_schema(self, arg) -> Schema:
+    def _metadata_to_schema(self, arg: object) -> Schema:
         # unrecognized annotation
         return {}
 
     @_metadata_to_schema.register
     def _(self, arg: IntegerRange) -> Schema:
         return {"minimum": arg.minimum, "maximum": arg.maximum}
 
@@ -264,16 +252,20 @@
         self, type_schema: Schema, metadata: Optional[Tuple[Any, ...]]
     ) -> Schema:
         if metadata:
             for m in metadata:
                 type_schema.update(self._metadata_to_schema(m))
         return type_schema
 
-    def _simple_type_to_schema(self, typ: type) -> Optional[Schema]:
-        "Returns the JSON schema associated with a simple, unrestricted type."
+    def _simple_type_to_schema(self, typ: object) -> Optional[Schema]:
+        """
+        Returns the JSON schema associated with a simple, unrestricted type.
+
+        :returns: The schema for a simple type, or `None`.
+        """
 
         if typ is type(None):
             return {"type": "null"}
         elif typ is bool:
             return {"type": "boolean"}
         elif typ is int:
             return {"type": "integer"}
@@ -315,15 +307,15 @@
             return {"type": "object"}
         elif typ is JsonArray:
             return {"type": "array"}
         else:
             # not a simple type
             return None
 
-    def type_to_schema(self, data_type: type, force_expand: bool = False) -> Schema:
+    def type_to_schema(self, data_type: object, force_expand: bool = False) -> Schema:
         """
         Returns the JSON schema associated with a type.
 
         :param data_type: The Python type whose JSON schema to return.
         :param force_expand: Forces a JSON schema to be returned even if the type is registered in the catalog of known types.
         :returns: The JSON schema associated with the type.
         """
@@ -535,15 +527,15 @@
             schema["additionalProperties"] = False
         if len(required) > 0:
             schema["required"] = required  # type: ignore
         if self.options.use_descriptions:
             schema.update(docstring_to_schema(typ))
         return schema
 
-    def _type_to_schema_with_lookup(self, data_type: type) -> Schema:
+    def _type_to_schema_with_lookup(self, data_type: object) -> Schema:
         """
         Returns the JSON schema associated with a type that may be registered in the catalog of known types.
 
         :param data_type: The type whose JSON schema we seek.
         :returns: The JSON schema associated with the type.
         """
 
@@ -551,25 +543,27 @@
         if entry.schema is None:
             type_schema = self.type_to_schema(data_type, force_expand=True)
         else:
             type_schema = deepcopy(entry.schema)
 
         # add descriptive text (if present)
         if self.options.use_descriptions:
-            if not isinstance(data_type, typing.ForwardRef):
+            if isinstance(data_type, type) and not isinstance(
+                data_type, typing.ForwardRef
+            ):
                 type_schema.update(docstring_to_schema(data_type))
 
         # add example (if present)
         if self.options.use_examples and entry.examples:
             type_schema["examples"] = entry.examples
 
         return type_schema
 
     def classdef_to_schema(
-        self, data_type: type, force_expand: bool = False
+        self, data_type: object, force_expand: bool = False
     ) -> Tuple[Schema, Dict[str, Schema]]:
         """
         Returns the JSON schema associated with a type and any nested types.
 
         :param data_type: The type whose JSON schema to return.
         :param force_expand: True if a full JSON schema is to be returned even for well-known types; false if a schema
         reference is to be used for well-known types.
@@ -606,15 +600,15 @@
     Draft7 = jsonschema.Draft7Validator
     Draft201909 = jsonschema.Draft201909Validator
     Draft202012 = jsonschema.Draft202012Validator
     Latest = jsonschema.Draft202012Validator
 
 
 def classdef_to_schema(
-    data_type: type,
+    data_type: object,
     options: Optional[SchemaOptions] = None,
     validator: Validator = Validator.Latest,
 ) -> Schema:
     """
     Returns the JSON schema corresponding to the given type.
 
     :param data_type: The Python type used to generate the JSON schema
@@ -714,15 +708,15 @@
 
 
 def json_schema_type(
     cls: Optional[Type[T]] = None,
     *,
     schema: Optional[Schema] = None,
     examples: Optional[List[JsonType]] = None,
-):
+) -> Union[Type[T], Callable[[Type[T]], Type[T]]]:
     """Decorator to add user-defined schema definition to a class."""
 
     def wrap(cls: Type[T]) -> Type[T]:
         return register_schema(cls, schema, examples=examples)
 
     # see if decorator is used as @json_schema_type or @json_schema_type()
     if cls is None:
```

### Comparing `json_strong_typing-0.2.6/strong_typing/serialization.py` & `json_strong_typing-0.2.7/strong_typing/serialization.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.2.6/strong_typing/serializer.py` & `json_strong_typing-0.2.7/strong_typing/serializer.py`

 * *Files identical despite different names*

### Comparing `json_strong_typing-0.2.6/strong_typing/topological.py` & `json_strong_typing-0.2.7/strong_typing/topological.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
 
     # empty list that will contain the sorted nodes (in reverse order)
     ordered: List[T] = []
 
     seen: Dict[T, bool] = {}
 
-    def _visit(n):
+    def _visit(n: T) -> None:
         status = seen.get(n)
         if status is not None:
             if status:  # node has a permanent mark
                 return
             else:  # node has a temporary mark
                 raise RuntimeError(f"cycle detected in graph for node {n}")
```

### Comparing `json_strong_typing-0.2.6/tests/test_deserialization.py` & `json_strong_typing-0.2.7/tests/test_deserialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 import datetime
 import unittest
 import uuid
-from typing import Dict, List, Optional, Set, Union
+from typing import Dict, List, Literal, Optional, Set, Union
 
-from sample_types import *
+from test_sample_types import (
+    UID,
+    BinaryValueWrapper,
+    ClassA,
+    ClassB,
+    ClassC,
+    FrozenValueWrapper,
+    LiteralWrapper,
+    NestedDataclass,
+    OptionalValueWrapper,
+    Side,
+    SimpleDataclass,
+    SimpleDerivedClass,
+    SimpleValueWrapper,
+    Suit,
+)
 
 from strong_typing.exception import JsonKeyError, JsonTypeError, JsonValueError
 from strong_typing.serialization import json_to_object, object_to_json
 
 
-def test_function():
+def test_function() -> None:
     pass
 
 
-async def test_async_function():
+async def test_async_function() -> None:
     pass
 
 
 class TestDeserialization(unittest.TestCase):
-    def test_deserialization_simple(self):
+    def test_deserialization_simple(self) -> None:
         self.assertEqual(json_to_object(type(None), None), None)
         self.assertEqual(json_to_object(bool, True), True)
         self.assertEqual(json_to_object(int, 23), 23)
         self.assertEqual(json_to_object(float, 4.5), 4.5)
         self.assertEqual(json_to_object(str, "an"), "an")
         self.assertEqual(json_to_object(bytes, "QU4="), bytes([65, 78]))
         self.assertEqual(json_to_object(Side, "L"), Side.LEFT)
@@ -39,44 +54,44 @@
         with self.assertRaises(JsonTypeError):
             json_to_object(int, "int")
         with self.assertRaises(JsonTypeError):
             json_to_object(str, None)
         with self.assertRaises(JsonTypeError):
             json_to_object(str, 1982)
 
-    def test_deserialization_datetime(self):
+    def test_deserialization_datetime(self) -> None:
         self.assertEqual(
             json_to_object(datetime.datetime, "1989-10-23T01:45:50Z"),
             datetime.datetime(1989, 10, 23, 1, 45, 50, tzinfo=datetime.timezone.utc),
         )
         timezone_cet = datetime.timezone(datetime.timedelta(seconds=3600))
         self.assertEqual(
             json_to_object(datetime.datetime, "1989-10-23T01:45:50+01:00"),
             datetime.datetime(1989, 10, 23, 1, 45, 50, tzinfo=timezone_cet),
         )
         with self.assertRaises(JsonValueError):
             json_to_object(datetime.datetime, "1989-10-23T01:45:50")
 
-    def test_deserialization_class(self):
+    def test_deserialization_class(self) -> None:
         self.assertEqual(
             json_to_object(SimpleValueWrapper, {"value": 42}), SimpleValueWrapper(42)
         )
         self.assertEqual(
             json_to_object(FrozenValueWrapper, {"value": 42}),
             FrozenValueWrapper(42),
         )
 
-    def test_deserialization_composite(self):
+    def test_deserialization_composite(self) -> None:
         self.assertEqual(json_to_object(UID, "1.2.3.4567.8900"), UID("1.2.3.4567.8900"))
         self.assertEqual(
             json_to_object(BinaryValueWrapper, {"value": "QU4="}),
             BinaryValueWrapper(bytes([65, 78])),
         )
 
-    def test_deserialization_collection(self):
+    def test_deserialization_collection(self) -> None:
         self.assertEqual(json_to_object(List[int], [1, 2, 3]), [1, 2, 3])
         self.assertEqual(
             json_to_object(Dict[str, int], {"a": 1, "b": 2, "c": 3}),
             {"a": 1, "b": 2, "c": 3},
         )
         self.assertEqual(json_to_object(Set[int], [1, 2, 3]), set([1, 2, 3]))
 
@@ -92,15 +107,15 @@
         with self.assertRaises(TypeError):
             json_to_object(dict, {"key": 42})
         with self.assertRaises(TypeError):
             json_to_object(set, [1, 2, 3])
         with self.assertRaises(TypeError):
             json_to_object(tuple, [1, "two"])
 
-    def test_deserialization_optional(self):
+    def test_deserialization_optional(self) -> None:
         self.assertEqual(json_to_object(Optional[int], None), None)
         self.assertEqual(json_to_object(Optional[int], 42), 42)
 
         self.assertEqual(
             json_to_object(OptionalValueWrapper, {}),
             OptionalValueWrapper(None),
         )
@@ -108,15 +123,15 @@
             json_to_object(OptionalValueWrapper, {"value": 42}),
             OptionalValueWrapper(42),
         )
 
         with self.assertRaises(JsonKeyError):
             json_to_object(OptionalValueWrapper, {"value": 23, "extra": 42})
 
-    def test_deserialization_literal(self):
+    def test_deserialization_literal(self) -> None:
         self.assertEqual(
             json_to_object(Literal["val1", "val2", "val3"], "val1"), "val1"
         )
         self.assertEqual(
             json_to_object(Literal["val1", "val2", "val3"], "val3"), "val3"
         )
         self.assertEqual(json_to_object(Literal[1, 2, 3], 1), 1)
@@ -135,15 +150,15 @@
         with self.assertRaises(TypeError):
             json_to_object(Literal["value", 1], "value")
         with self.assertRaises(TypeError):
             json_to_object(Literal[1, "value"], "value")
         with self.assertRaises(JsonTypeError):
             json_to_object(Literal["val1", "val2", "val3"], "value")
 
-    def test_deserialization_union(self):
+    def test_deserialization_union(self) -> None:
         # built-in types
         self.assertEqual(json_to_object(Union[int, str], 42), 42)
         self.assertEqual(json_to_object(Union[int, str], "a string"), "a string")
         self.assertEqual(json_to_object(Union[str, int], 42), 42)
         self.assertEqual(json_to_object(Union[str, int], "a string"), "a string")
         with self.assertRaises(JsonKeyError):
             json_to_object(Union[int, str], 10.23)
@@ -221,15 +236,15 @@
             json_to_object(
                 Union[ClassA, ClassB, ClassC],
                 {"type": "B", "name": "b", "value": "string"},
             ),
             ClassB(name="b", type="B", value="string"),
         )
 
-    def test_object_deserialization(self):
+    def test_object_deserialization(self) -> None:
         """Test composition and inheritance with object de-serialization."""
 
         json_dict = object_to_json(NestedDataclass())
         obj = json_to_object(NestedDataclass, json_dict)
         self.assertEqual(obj, NestedDataclass())
```

### Comparing `json_strong_typing-0.2.6/tests/test_docstring.py` & `json_strong_typing-0.2.7/tests/test_docstring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import enum
 import inspect
 import sys
+import typing
 import unittest
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, TypeVar
+
+from test_sample_exceptions import CustomException
 
 from strong_typing.docstring import has_default_docstring, has_docstring, parse_type
 
-from sample_exceptions import CustomException
+T = TypeVar("T")
+
+
+def required(obj: Optional[T]) -> T:
+    "Casts an optional type to a required type."
+
+    return typing.cast(T, obj)
 
 
 class NoDescriptionClass:
     pass
 
 
 @dataclass
@@ -125,54 +134,54 @@
         """
         Short description of a static method.
 
         :param a: Short description for `a`.
         """
         pass
 
-    def no_type_annotation_method(self):
+    def no_type_annotation_method(self):  # type: ignore
         """
         Short description of an instance method without parameter or return value annotation.
 
         :returns: A return value.
         """
         pass
 
 
 class TestDocstring(unittest.TestCase):
-    def test_default_docstring(self):
+    def test_default_docstring(self) -> None:
         self.assertFalse(has_default_docstring(NoDescriptionClass))
         self.assertTrue(has_default_docstring(NoDescriptionDataclass))
         self.assertFalse(has_default_docstring(ShortDescriptionClass))
         if sys.version_info >= (3, 11):
             self.assertFalse(has_default_docstring(NoDescriptionEnumeration))
         else:
             self.assertTrue(has_default_docstring(NoDescriptionEnumeration))
 
-    def test_any_docstring(self):
+    def test_any_docstring(self) -> None:
         self.assertFalse(has_docstring(NoDescriptionClass))
         self.assertFalse(has_docstring(NoDescriptionDataclass))
         self.assertFalse(has_docstring(NoDescriptionEnumeration))
         self.assertTrue(has_docstring(ShortDescriptionClass))
 
-    def test_no_description(self):
+    def test_no_description(self) -> None:
         docstring = parse_type(NoDescriptionClass)
         self.assertIsNone(docstring.short_description)
         self.assertIsNone(docstring.long_description)
         self.assertFalse(docstring.params)
         self.assertIsNone(docstring.returns)
         self.assertEqual(str(docstring), "")
 
-    def test_short_description(self):
+    def test_short_description(self) -> None:
         docstring = parse_type(ShortDescriptionClass)
         self.assertEqual(docstring.short_description, "Short description.")
         self.assertIsNone(docstring.long_description)
         self.assertEqual(str(docstring), ShortDescriptionClass.__doc__)
 
-    def test_multi_line_description(self):
+    def test_multi_line_description(self) -> None:
         docstring = parse_type(MultiLineShortDescriptionClass)
         self.assertEqual(
             docstring.short_description,
             "A short description that spans multiple lines.",
         )
         self.assertIsNone(docstring.long_description)
         self.assertEqual(
@@ -185,24 +194,25 @@
             docstring.long_description, "A description text that\nspans multiple lines."
         )
         self.assertEqual(
             str(docstring),
             "Short description.\n\nA description text that\nspans multiple lines.",
         )
 
-    def test_dataclass_parameter_list(self):
+    def test_dataclass_parameter_list(self) -> None:
         docstring = parse_type(ShortDescriptionParameterClass)
         self.assertEqual(docstring.short_description, "Short description.")
         self.assertIsNone(docstring.long_description)
         self.assertEqual(len(docstring.params), 1)
         self.assertEqual(
             docstring.params["a"].description, "Short description for `a`."
         )
         self.assertEqual(
-            str(docstring), inspect.cleandoc(ShortDescriptionParameterClass.__doc__)
+            str(docstring),
+            inspect.cleandoc(ShortDescriptionParameterClass.__doc__ or ""),
         )
 
         docstring = parse_type(MultiLineDescriptionParametersClass)
         self.assertEqual(docstring.short_description, "Short description.")
         self.assertEqual(
             docstring.long_description, "A description text that\nspans multiple lines."
         )
@@ -234,28 +244,29 @@
                 ]
             ),
         )
 
         with self.assertRaises(TypeError):
             parse_type(MissingMemberClass)
 
-    def test_function_parameter_list(self):
+    def test_function_parameter_list(self) -> None:
         docstring = parse_type(SampleClass.instance_method)
         self.assertEqual(
             docstring.short_description, "Short description of an instance method."
         )
         self.assertIsNone(docstring.long_description)
         self.assertEqual(len(docstring.params), 2)
         self.assertEqual(
             docstring.params["a"].description, "Short description for `a`."
         )
         self.assertEqual(
             docstring.params["b"].description, "Short description for `b`."
         )
-        self.assertEqual(docstring.returns.description, "A return value.")
+        self.assertIsNotNone(docstring.returns)
+        self.assertEqual(required(docstring.returns).description, "A return value.")
 
         self.assertEqual(len(docstring.raises), 3)
         self.assertEqual(
             docstring.raises["TypeError"].description,
             "A type exception rarely raised.",
         )
         self.assertEqual(docstring.raises["TypeError"].raise_type, TypeError)
@@ -270,43 +281,45 @@
         )
         self.assertEqual(
             docstring.raises["CustomException"].raise_type, CustomException
         )
 
         docstring = parse_type(SampleClass.other_instance_method)
         self.assertEqual(
-            str(docstring), inspect.cleandoc(SampleClass.other_instance_method.__doc__)
+            str(docstring),
+            inspect.cleandoc(SampleClass.other_instance_method.__doc__ or ""),
         )
 
         docstring = parse_type(SampleClass.class_method)
         self.assertEqual(
             docstring.short_description, "Short description of a class method."
         )
         self.assertIsNone(docstring.long_description)
         self.assertEqual(len(docstring.params), 1)
         self.assertEqual(
             docstring.params["a"].description, "Short description for `a`."
         )
-        self.assertEqual(docstring.returns.description, "A return value.")
+        self.assertIsNotNone(docstring.returns)
+        self.assertEqual(required(docstring.returns).description, "A return value.")
         self.assertEqual(
-            str(docstring), inspect.cleandoc(SampleClass.class_method.__doc__)
+            str(docstring), inspect.cleandoc(SampleClass.class_method.__doc__ or "")
         )
 
         docstring = parse_type(SampleClass.static_method)
         self.assertEqual(
             docstring.short_description, "Short description of a static method."
         )
         self.assertIsNone(docstring.long_description)
         self.assertEqual(len(docstring.params), 1)
         self.assertEqual(
             docstring.params["a"].description, "Short description for `a`."
         )
         self.assertIsNone(docstring.returns)
         self.assertEqual(
-            str(docstring), inspect.cleandoc(SampleClass.static_method.__doc__)
+            str(docstring), inspect.cleandoc(SampleClass.static_method.__doc__ or "")
         )
 
         with self.assertRaises(TypeError):
             parse_type(SampleClass.no_type_annotation_method)
 
 
 if __name__ == "__main__":
```

### Comparing `json_strong_typing-0.2.6/tests/test_inspection.py` & `json_strong_typing-0.2.7/tests/test_inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import enum
 import sys
 import unittest
 from dataclasses import dataclass
 from typing import Dict, List, NamedTuple, Optional, Set, Tuple, Union
 
-from sample_types import *
+from test_sample_types import CompositeDataclass, NestedDataclass, SimpleDataclass
 
 from strong_typing.auxiliary import Annotated, typeannotation
 from strong_typing.inspection import (
     check_recursive,
     get_class_properties,
     get_module_classes,
     get_referenced_types,
@@ -19,14 +19,15 @@
     is_generic_list,
     is_named_tuple_type,
     is_type_enum,
     is_type_optional,
     is_type_union,
     unwrap_generic_dict,
     unwrap_generic_list,
+    unwrap_union_types,
 )
 
 
 class Side(enum.Enum):
     "An enumeration with string values."
 
     LEFT = "L"
@@ -62,116 +63,126 @@
 
 @typeannotation
 class SimpleAnnotation:
     pass
 
 
 class TestInspection(unittest.TestCase):
-    def test_simple(self):
+    def test_simple(self) -> None:
         self.assertEqual(get_referenced_types(type(None)), [])
         self.assertEqual(get_referenced_types(int), [int])
         self.assertEqual(get_referenced_types(Optional[str]), [str])
         self.assertEqual(get_referenced_types(List[str]), [str])
         self.assertEqual(get_referenced_types(Dict[int, bool]), [int, bool])
         self.assertEqual(get_referenced_types(Union[int, bool, str]), [int, bool, str])
         self.assertEqual(
             get_referenced_types(Union[None, int, datetime.datetime]),
             [int, datetime.datetime],
         )
 
-    def test_enum(self):
+    def test_enum(self) -> None:
         self.assertTrue(is_type_enum(Side))
         self.assertTrue(is_type_enum(Suit))
         self.assertFalse(is_type_enum(Side.LEFT))
         self.assertFalse(is_type_enum(Suit.Diamonds))
         self.assertFalse(is_type_enum(int))
         self.assertFalse(is_type_enum(str))
         self.assertFalse(is_type_enum(SimpleObject))
 
-    def test_optional(self):
+    def test_optional(self) -> None:
         self.assertTrue(is_type_optional(Optional[int]))
         self.assertTrue(is_type_optional(Union[None, int]))
         self.assertTrue(is_type_optional(Union[int, None]))
 
         if sys.version_info >= (3, 10):
             self.assertTrue(is_type_optional(None | int))
             self.assertTrue(is_type_optional(int | None))
 
         self.assertFalse(is_type_optional(int))
         self.assertFalse(is_type_optional(Union[int, str]))
 
-    def test_strict_optional(self):
+    def test_strict_optional(self) -> None:
         self.assertTrue(is_type_optional(Union[None, int], strict=True))
         self.assertTrue(is_type_optional(Union[int, None], strict=True))
         self.assertTrue(is_type_optional(Union[None, int, str]))
         self.assertTrue(is_type_optional(Union[int, None, str]))
         self.assertFalse(is_type_optional(Union[None, int, str], strict=True))
         self.assertFalse(is_type_optional(Union[int, None, str], strict=True))
 
-    def test_union(self):
+    def test_union(self) -> None:
         self.assertTrue(is_type_union(Union[int, str]))
         self.assertTrue(is_type_union(Union[bool, int, str]))
         self.assertTrue(is_type_union(Union[int, str, None]))
         self.assertTrue(is_type_union(Union[bool, int, str, None]))
 
         if sys.version_info >= (3, 10):
             self.assertTrue(is_type_union(int | str))
             self.assertTrue(is_type_union(bool | int | str))
             self.assertTrue(is_type_union(int | str | None))
             self.assertTrue(is_type_union(bool | int | str | None))
 
         self.assertFalse(is_type_union(int))
 
-    def test_list(self):
+        self.assertEqual(unwrap_union_types(Union[int, str]), (int, str))
+        self.assertEqual(
+            unwrap_union_types(Union[int, str, None]), (int, str, type(None))
+        )
+        if sys.version_info >= (3, 10):
+            self.assertEqual(unwrap_union_types(int | str), (int, str))
+            self.assertEqual(
+                unwrap_union_types(int | str | None), (int, str, type(None))
+            )
+
+    def test_list(self) -> None:
         self.assertTrue(is_generic_list(List[int]))
         self.assertTrue(is_generic_list(List[str]))
         self.assertTrue(is_generic_list(List[SimpleObject]))
         self.assertFalse(is_generic_list(list))
         self.assertFalse(is_generic_list([]))
 
         self.assertEqual(unwrap_generic_list(List[int]), int)
         self.assertEqual(unwrap_generic_list(List[str]), str)
         self.assertEqual(unwrap_generic_list(List[List[str]]), List[str])
 
-    def test_dict(self):
+    def test_dict(self) -> None:
         self.assertTrue(is_generic_dict(Dict[int, str]))
         self.assertTrue(is_generic_dict(Dict[str, SimpleObject]))
         self.assertFalse(is_generic_dict(dict))
         self.assertFalse(is_generic_dict({}))
 
         self.assertEqual(unwrap_generic_dict(Dict[int, str]), (int, str))
         self.assertEqual(
             unwrap_generic_dict(Dict[str, SimpleObject]), (str, SimpleObject)
         )
         self.assertEqual(
             unwrap_generic_dict(Dict[str, List[SimpleObject]]),
             (str, List[SimpleObject]),
         )
 
-    def test_annotated(self):
+    def test_annotated(self) -> None:
         self.assertTrue(is_type_enum(Annotated[Suit, SimpleAnnotation()]))
         self.assertTrue(is_generic_list(Annotated[List[int], SimpleAnnotation()]))
         self.assertTrue(is_generic_dict(Annotated[Dict[int, str], SimpleAnnotation()]))
 
-    def test_classes(self):
+    def test_classes(self) -> None:
         classes = get_module_classes(sys.modules[__name__])
         self.assertCountEqual(
             classes,
             [
                 Side,
                 Suit,
                 SimpleAnnotation,
                 SimpleObject,
                 SimpleDataClass,
                 SimpleNamedTuple,
                 TestInspection,
             ],
         )
 
-    def test_properties(self):
+    def test_properties(self) -> None:
         properties = [
             (name, data_type) for name, data_type in get_class_properties(SimpleObject)
         ]
         self.assertCountEqual(properties, [("value", int)])
 
         self.assertTrue(is_dataclass_type(SimpleDataClass))
         properties = [
@@ -183,15 +194,15 @@
         self.assertTrue(is_named_tuple_type(SimpleNamedTuple))
         properties = [
             (name, data_type)
             for name, data_type in get_class_properties(SimpleNamedTuple)
         ]
         self.assertCountEqual(properties, [("integer", int), ("string", str)])
 
-    def test_generic(self):
+    def test_generic(self) -> None:
         obj = SimpleObject()
         self.assertTrue(is_generic_instance(obj, SimpleObject))
         self.assertFalse(is_generic_instance(None, SimpleObject))
         self.assertFalse(is_generic_instance(42, SimpleObject))
         self.assertFalse(is_generic_instance("string", SimpleObject))
 
         self.assertTrue(is_generic_instance([], List[int]))
@@ -217,15 +228,15 @@
         self.assertTrue(is_generic_instance(42, Union[str, int]))
         self.assertFalse(is_generic_instance(None, Union[str, int]))
 
         self.assertTrue(is_generic_instance(None, Optional[str]))
         self.assertTrue(is_generic_instance("string", Optional[str]))
         self.assertFalse(is_generic_instance(42, Optional[str]))
 
-    def test_recursive(self):
+    def test_recursive(self) -> None:
         self.assertTrue(
             check_recursive(
                 SimpleObject(),
                 pred=lambda typ, obj: isinstance(obj, typ),
             )
         )
         self.assertTrue(
```

### Comparing `json_strong_typing-0.2.6/tests/test_name.py` & `json_strong_typing-0.2.7/tests/test_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from strong_typing.auxiliary import Alias, Annotated
 from strong_typing.mapping import python_field_to_json_property
 from strong_typing.name import python_type_to_name
 
 
 class TestName(unittest.TestCase):
-    def test_builtin(self):
+    def test_builtin(self) -> None:
         self.assertEqual(python_type_to_name(type(None)), "NoneType")
         self.assertEqual(python_type_to_name(int), "int")
         self.assertEqual(python_type_to_name(str), "str")
 
-    def test_generic(self):
+    def test_generic(self) -> None:
         self.assertEqual(
             python_type_to_name(Optional[str], force=True),
             "Optional__str",
         )
         self.assertEqual(
             python_type_to_name(List[int], force=True),
             "List__int",
@@ -35,15 +35,15 @@
         with self.assertRaises(TypeError):
             python_type_to_name(List[int])
         with self.assertRaises(TypeError):
             python_type_to_name(Dict[str, int])
         with self.assertRaises(TypeError):
             python_type_to_name(Union[str, int, None])
 
-    def test_alias(self):
+    def test_alias(self) -> None:
         self.assertEqual(python_field_to_json_property("id"), "id")
         self.assertEqual(
             python_field_to_json_property("id", Annotated[str, Alias("alias")]), "alias"
         )
 
 
 if __name__ == "__main__":
```

### Comparing `json_strong_typing-0.2.6/tests/test_performance.py` & `json_strong_typing-0.2.7/tests/test_performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import random
 import string
 import unittest
 import uuid
 from dataclasses import dataclass
 
-from strong_typing.serialization import json_to_object, object_to_json
+from test_timer import Timer
 
-from timer import Timer
+from strong_typing.serialization import json_to_object, object_to_json
 
 
 def time_today(time_of_day: datetime.time) -> datetime.datetime:
     return datetime.datetime.combine(
         datetime.datetime.today(), time_of_day, time_of_day.tzinfo
     )
 
@@ -81,15 +81,15 @@
             datetime.datetime(2022, 9, 25, 18, 45, 0, tzinfo=datetime.timezone.utc),
         ),
         guid_value=uuid.uuid4(),
     )
 
 
 class TestPerformance(unittest.TestCase):
-    def test_serialization(self):
+    def test_serialization(self) -> None:
         original_items = [create_randomized_object() for k in range(100000)]
 
         with Timer("serialization"):
             serialized_items = [object_to_json(item) for item in original_items]
 
         with Timer("deserialization"):
             deserialized_items = [
```

### Comparing `json_strong_typing-0.2.6/tests/test_schema.py` & `json_strong_typing-0.2.7/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import datetime
 import decimal
 import unittest
 import uuid
 from typing import Any, Dict, List, Set, Tuple, Union
 
-from sample_types import *
+from test_sample_types import (
+    UID,
+    AnnotatedSimpleDataclass,
+    BinaryTree,
+    Side,
+    SimpleDataclass,
+    SimpleTypedNamedTuple,
+    SimpleValueWrapper,
+    Suit,
+    ValueExample,
+)
 
 from strong_typing.auxiliary import Annotated, IntegerRange, Precision, int32, uint64
+from strong_typing.core import JsonType
 from strong_typing.schema import (
     JsonSchemaGenerator,
     JsonType,
     SchemaOptions,
     Validator,
     classdef_to_schema,
     get_class_docstrings,
 )
 
 
 class TestSchema(unittest.TestCase):
-    def test_schema(self):
+    def test_schema(self) -> None:
         options = SchemaOptions(use_descriptions=True)
         generator = JsonSchemaGenerator(options)
         self.assertEqual(generator.type_to_schema(type(None)), {"type": "null"})
         self.assertEqual(generator.type_to_schema(bool), {"type": "boolean"})
         self.assertEqual(generator.type_to_schema(int), {"type": "integer"})
         self.assertEqual(generator.type_to_schema(float), {"type": "number"})
         self.assertEqual(generator.type_to_schema(str), {"type": "string"})
@@ -142,30 +153,30 @@
                         "title": "A unique identifier in DICOM.",
                     }
                 },
                 "$ref": "#/definitions/UID",
             },
         )
 
-    def test_recursive(self):
+    def test_recursive(self) -> None:
         options = SchemaOptions(use_descriptions=False)
         generator = JsonSchemaGenerator(options)
         self.assertEqual(
             generator.type_to_schema(BinaryTree, force_expand=True),
             {
                 "type": "object",
                 "properties": {
                     "left": {"$ref": "#/definitions/BinaryTree"},
                     "right": {"$ref": "#/definitions/BinaryTree"},
                 },
                 "additionalProperties": False,
             },
         )
 
-    def test_registered(self):
+    def test_registered(self) -> None:
         options = SchemaOptions(use_descriptions=False)
         generator = JsonSchemaGenerator(options)
         self.assertEqual(
             generator.type_to_schema(JsonType, force_expand=True),
             {
                 "oneOf": [
                     {"type": "null"},
@@ -220,15 +231,15 @@
                         ],
                     }
                 },
                 "$ref": "#/definitions/JsonType",
             },
         )
 
-    def test_annotated(self):
+    def test_annotated(self) -> None:
         options = SchemaOptions(use_descriptions=False)
         generator = JsonSchemaGenerator(options)
         self.assertEqual(
             generator.type_to_schema(Annotated[int, IntegerRange(23, 82)]),
             {
                 "type": "integer",
                 "minimum": 23,
@@ -278,38 +289,40 @@
                     },
                 },
                 "additionalProperties": False,
                 "required": ["int_value", "float_value", "str_value"],
             },
         )
 
-    def test_fixed_width(self):
+    def test_fixed_width(self) -> None:
         options = SchemaOptions(use_descriptions=True)
         generator = JsonSchemaGenerator(options)
         self.assertEqual(
             generator.type_to_schema(int32), {"format": "int32", "type": "integer"}
         )
         self.assertEqual(
             generator.type_to_schema(uint64), {"format": "uint64", "type": "integer"}
         )
 
-    def _assert_docstring_equal(self, generator: JsonSchemaGenerator, typ: type):
+    def _assert_docstring_equal(
+        self, generator: JsonSchemaGenerator, typ: type
+    ) -> None:
         "Checks if the Python class docstring matches the title and description strings in the generated JSON schema."
 
         short_description, long_description = get_class_docstrings(typ)
         self.assertEqual(
             generator.type_to_schema(typ).get("title"),
             short_description,
         )
         self.assertEqual(
             generator.type_to_schema(typ).get("description"),
             long_description,
         )
 
-    def test_docstring(self):
+    def test_docstring(self) -> None:
         self.maxDiff = None
         options = SchemaOptions(use_descriptions=True)
         generator = JsonSchemaGenerator(options)
 
         # never extract docstring simple types
         self.assertEqual(generator.type_to_schema(type(None)), {"type": "null"})
         self.assertEqual(generator.type_to_schema(bool), {"type": "boolean"})
```

### Comparing `json_strong_typing-0.2.6/tests/test_serialization.py` & `json_strong_typing-0.2.7/tests/test_serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 import datetime
+import typing
 import unittest
 import uuid
+from typing import Dict
 
-from sample_types import *
+from test_sample_types import (
+    UID,
+    AnnotatedSimpleDataclass,
+    BinaryValueWrapper,
+    CompositeDataclass,
+    FrozenValueWrapper,
+    LiteralWrapper,
+    MultipleInheritanceDerivedClass,
+    NestedDataclass,
+    Side,
+    SimpleDataclass,
+    SimpleTypedClass,
+    SimpleTypedNamedTuple,
+    SimpleUntypedClass,
+    SimpleUntypedNamedTuple,
+    SimpleValueWrapper,
+    Suit,
+)
 
+from strong_typing.core import JsonType
 from strong_typing.exception import JsonValueError
 from strong_typing.schema import validate_object
 from strong_typing.serialization import object_to_json
 
 
-def test_function():
+def test_function() -> None:
     pass
 
 
-async def test_async_function():
+async def test_async_function() -> None:
     pass
 
 
 class TestSerialization(unittest.TestCase):
-    def test_composite_object(self):
+    def test_composite_object(self) -> None:
         json_dict = object_to_json(SimpleDataclass())
         validate_object(SimpleDataclass, json_dict)
 
         json_dict = object_to_json(AnnotatedSimpleDataclass())
         validate_object(AnnotatedSimpleDataclass, json_dict)
 
         json_dict = object_to_json(CompositeDataclass())
         validate_object(CompositeDataclass, json_dict)
 
         json_dict = object_to_json(NestedDataclass())
         validate_object(NestedDataclass, json_dict)
 
-    def test_serialization_simple(self):
+    def test_serialization_simple(self) -> None:
         self.assertEqual(object_to_json(None), None)
         self.assertEqual(object_to_json(True), True)
         self.assertEqual(object_to_json(23), 23)
         self.assertEqual(object_to_json(4.5), 4.5)
         self.assertEqual(object_to_json("an"), "an")
         self.assertEqual(object_to_json(bytes([65, 78])), "QU4=")
         self.assertEqual(object_to_json(Side.LEFT), "L")
         self.assertEqual(object_to_json(Suit.Diamonds), 1)
         self.assertEqual(
             object_to_json(uuid.UUID("f81d4fae-7dec-11d0-a765-00a0c91e6bf6")),
             "f81d4fae-7dec-11d0-a765-00a0c91e6bf6",
         )
 
-    def test_serialization_datetime(self):
+    def test_serialization_datetime(self) -> None:
         self.assertEqual(
             object_to_json(
                 datetime.datetime(1989, 10, 23, 1, 45, 50, tzinfo=datetime.timezone.utc)
             ),
             "1989-10-23T01:45:50Z",
         )
         timezone_cet = datetime.timezone(datetime.timedelta(seconds=3600))
@@ -58,100 +78,105 @@
                 datetime.datetime(1989, 10, 23, 1, 45, 50, tzinfo=timezone_cet)
             ),
             "1989-10-23T01:45:50+01:00",
         )
         with self.assertRaises(JsonValueError):
             object_to_json(datetime.datetime(1989, 10, 23, 1, 45, 50))
 
-    def test_serialization_literal(self):
+    def test_serialization_literal(self) -> None:
         self.assertEqual(object_to_json(LiteralWrapper("val1")), {"value": "val1"})
         self.assertEqual(object_to_json(LiteralWrapper("val2")), {"value": "val2"})
         self.assertEqual(object_to_json(LiteralWrapper("val3")), {"value": "val3"})
 
-    def test_serialization_namedtuple(self):
+    def test_serialization_namedtuple(self) -> None:
         self.assertEqual(
             object_to_json(SimpleTypedNamedTuple(42, "string")),
             {"int_value": 42, "str_value": "string"},
         )
         self.assertEqual(
             object_to_json(SimpleUntypedNamedTuple(42, "string")),
             {"int_value": 42, "str_value": "string"},
         )
 
-    def test_serialization_class(self):
+    def test_serialization_class(self) -> None:
         self.assertEqual(object_to_json(SimpleValueWrapper(42)), {"value": 42})
         self.assertEqual(object_to_json(FrozenValueWrapper(42)), {"value": 42})
         self.assertEqual(
             object_to_json(SimpleTypedClass(42, "string")),
             {"int_value": 42, "str_value": "string"},
         )
         self.assertEqual(
             object_to_json(SimpleUntypedClass(42, "string")),
             {"int_value": 42, "str_value": "string"},
         )
 
-    def test_serialization_collection(self):
+    def test_serialization_collection(self) -> None:
         self.assertEqual(object_to_json([1, 2, 3]), [1, 2, 3])
         self.assertEqual(
             object_to_json({"a": 1, "b": 2, "c": 3}), {"a": 1, "b": 2, "c": 3}
         )
         self.assertEqual(object_to_json(set([1, 2, 3])), [1, 2, 3])
         self.assertEqual(object_to_json(tuple([1, "two"])), [1, "two"])
 
-    def test_serialization_composite(self):
+    def test_serialization_composite(self) -> None:
         self.assertEqual(object_to_json(UID("1.2.3.4567.8900")), "1.2.3.4567.8900")
         self.assertEqual(
             object_to_json(BinaryValueWrapper(bytes([65, 78]))), {"value": "QU4="}
         )
 
-    def test_serialization_type_mismatch(self):
+    def test_serialization_type_mismatch(self) -> None:
         self.assertRaises(TypeError, object_to_json, test_function)  # function
         self.assertRaises(TypeError, object_to_json, test_async_function)  # function
         self.assertRaises(TypeError, object_to_json, TestSerialization)  # class
         self.assertRaises(
             TypeError, object_to_json, self.test_serialization_type_mismatch
         )  # method
 
-    def test_object_serialization(self):
+    def test_object_serialization(self) -> None:
         """Test composition and inheritance with object serialization."""
 
-        json_dict = object_to_json(SimpleDataclass())
+        json_dict = typing.cast(Dict[str, JsonType], object_to_json(SimpleDataclass()))
         self.assertDictEqual(
             json_dict,
             {
                 "bool_value": True,
                 "int_value": 23,
                 "float_value": 4.5,
                 "str_value": "string",
                 "date_value": "1970-01-01",
                 "time_value": "06:15:30",
                 "datetime_value": "1989-10-23T01:45:50Z",
                 "guid_value": "f81d4fae-7dec-11d0-a765-00a0c91e6bf6",
             },
         )
 
-        json_dict = object_to_json(
-            CompositeDataclass(
-                list_value=["a", "b", "c"],
-                dict_value={"key": 42},
-                set_value=set(i for i in range(0, 4)),
-            )
+        json_dict = typing.cast(
+            Dict[str, JsonType],
+            object_to_json(
+                CompositeDataclass(
+                    list_value=["a", "b", "c"],
+                    dict_value={"key": 42},
+                    set_value=set(i for i in range(0, 4)),
+                )
+            ),
         )
         self.assertDictEqual(
             json_dict,
             {
                 "list_value": ["a", "b", "c"],
                 "dict_value": {"key": 42},
                 "set_value": [0, 1, 2, 3],
                 "tuple_value": [True, 2, "three"],
                 "named_tuple_value": {"int_value": 1, "str_value": "second"},
             },
         )
 
-        json_dict = object_to_json(MultipleInheritanceDerivedClass())
+        json_dict = typing.cast(
+            Dict[str, JsonType], object_to_json(MultipleInheritanceDerivedClass())
+        )
         self.assertDictEqual(
             json_dict,
             {
                 "bool_value": True,
                 "int_value": 23,
                 "float_value": 4.5,
                 "str_value": "string",
@@ -166,15 +191,15 @@
                 "named_tuple_value": {"int_value": 1, "str_value": "second"},
                 "extra_int_value": 0,
                 "extra_str_value": "zero",
                 "extra_optional_value": "value",
             },
         )
 
-        json_dict = object_to_json(NestedDataclass())
+        json_dict = typing.cast(Dict[str, JsonType], object_to_json(NestedDataclass()))
         self.assertDictEqual(
             json_dict,
             {
                 "obj_value": {
                     "list_value": ["a", "b", "c"],
                     "dict_value": {"key": 42},
                     "set_value": [],
```

### Comparing `json_strong_typing-0.2.6/tests/test_topological.py` & `json_strong_typing-0.2.7/tests/test_topological.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import decimal
 import unittest
 import uuid
 from dataclasses import dataclass
-from typing import List, TypeVar
+from typing import Dict, List, Set, TypeVar
 
 from strong_typing.inspection import is_dataclass_type
 from strong_typing.topological import topological_sort, type_topological_sort
 
 T = TypeVar("T")
 
 
@@ -43,51 +43,56 @@
 
 class TestTopological(unittest.TestCase):
     def assertOrder(self, order: List[T], first: T, second: T) -> None:
         self.assertIn(first, order)
         self.assertIn(second, order)
         self.assertLess(order.index(first), order.index(second))
 
-    def test_simple(self):
-        graph = {
+    def test_simple(self) -> None:
+        graph: Dict[int, Set[int]] = {
             0: set(),
             1: set(),
             2: set([3]),
             3: set([1]),
             4: set([0, 1]),
             5: set([0, 2]),
         }
         order = topological_sort(graph)
         self.assertEqual(order, [0, 1, 3, 2, 4, 5])
 
-    def test_loop(self):
-        graph = {0: set([0])}
+    def test_loop(self) -> None:
+        graph: Dict[int, Set[int]] = {0: set([0])}
         order = topological_sort(graph)
         self.assertEqual(order, [0])
 
-    def test_cycle(self):
-        graph = {0: set([1, 2]), 1: set([2]), 2: set([0, 3]), 3: set()}
+    def test_cycle(self) -> None:
+        graph: Dict[int, Set[int]] = {
+            0: set([1, 2]),
+            1: set([2]),
+            2: set([0, 3]),
+            3: set(),
+        }
         with self.assertRaises(RuntimeError):
             topological_sort(graph)
 
-    def test_types(self):
+    def test_types(self) -> None:
         order = type_topological_sort([CompositeClass])
         self.assertNotIn(decimal.Decimal, order)
         self.assertOrder(order, bool, SimpleDataClass)
         self.assertOrder(order, int, SimpleDataClass)
         self.assertOrder(order, str, SimpleDataClass)
         self.assertOrder(order, datetime.datetime, SimpleDataClass)
         self.assertOrder(order, SimpleClass, NestedDataClass)
         self.assertOrder(order, SimpleDataClass, NestedDataClass)
         self.assertOrder(order, int, CompositeClass)
         self.assertOrder(order, uuid.UUID, CompositeClass)
         self.assertOrder(order, SimpleDataClass, CompositeClass)
         self.assertOrder(order, NestedDataClass, CompositeClass)
 
-    def test_types_with_dependencies(self):
+    def test_types_with_dependencies(self) -> None:
         order = type_topological_sort([NestedDataClass])
         self.assertNotIn(decimal.Decimal, order)
 
         fn = lambda cls: [decimal.Decimal] if is_dataclass_type(cls) else []
         order = type_topological_sort([NestedDataClass], fn)
         self.assertOrder(order, decimal.Decimal, SimpleDataClass)
         self.assertOrder(order, decimal.Decimal, NestedDataClass)
```

