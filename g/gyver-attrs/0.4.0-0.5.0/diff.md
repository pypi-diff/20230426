# Comparing `tmp/gyver_attrs-0.4.0.tar.gz` & `tmp/gyver_attrs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver_attrs-0.4.0.tar", max compression
+gzip compressed data, was "gyver_attrs-0.5.0.tar", max compression
```

## Comparing `gyver_attrs-0.4.0.tar` & `gyver_attrs-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11352 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/LICENSE
--rw-r--r--   0        0        0     5279 2023-03-09 20:10:09.521782 gyver_attrs-0.4.0/README.md
--rw-r--r--   0        0        0       80 2023-03-07 06:14:06.117411 gyver_attrs-0.4.0/gyver/__init__.py
--rw-r--r--   0        0        0      543 2023-03-15 09:28:21.878742 gyver_attrs-0.4.0/gyver/attrs/__init__.py
--rw-r--r--   0        0        0     3130 2023-03-15 08:46:14.263540 gyver_attrs-0.4.0/gyver/attrs/camel.py
--rw-r--r--   0        0        0      146 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/converters/__init__.py
--rw-r--r--   0        0        0      751 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/converters/json.py
--rw-r--r--   0        0        0     1516 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/converters/utils.py
--rw-r--r--   0        0        0     5515 2023-03-09 08:32:39.670361 gyver_attrs-0.4.0/gyver/attrs/field.py
--rw-r--r--   0        0        0     1045 2023-03-08 10:49:46.265130 gyver_attrs-0.4.0/gyver/attrs/helpers.py
--rw-r--r--   0        0        0    25193 2023-03-15 09:23:45.121750 gyver_attrs-0.4.0/gyver/attrs/main.py
--rw-r--r--   0        0        0     4817 2023-03-09 08:58:05.737472 gyver_attrs-0.4.0/gyver/attrs/methods.py
--rw-r--r--   0        0        0        0 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/py.typed
--rw-r--r--   0        0        0     3872 2023-03-09 20:40:43.409237 gyver_attrs-0.4.0/gyver/attrs/resolver.py
--rw-r--r--   0        0        0     4074 2023-03-15 09:17:47.915311 gyver_attrs-0.4.0/gyver/attrs/schema.py
--rw-r--r--   0        0        0     2986 2023-03-09 09:37:47.302454 gyver_attrs-0.4.0/gyver/attrs/shortcuts.py
--rw-r--r--   0        0        0        0 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/utils/__init__.py
--rw-r--r--   0        0        0      604 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/utils/factory.py
--rw-r--r--   0        0        0     1501 2023-03-15 09:22:48.082882 gyver_attrs-0.4.0/gyver/attrs/utils/functions.py
--rw-r--r--   0        0        0      298 2023-03-04 12:43:55.291230 gyver_attrs-0.4.0/gyver/attrs/utils/typedef.py
--rw-r--r--   0        0        0      655 2023-03-15 09:28:21.876742 gyver_attrs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 gyver_attrs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5279 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/README.md
+-rw-r--r--   0        0        0       80 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/gyver/__init__.py
+-rw-r--r--   0        0        0      543 2023-04-26 20:28:32.340344 gyver_attrs-0.5.0/gyver/attrs/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-26 20:27:13.432336 gyver_attrs-0.5.0/gyver/attrs/camel.py
+-rw-r--r--   0        0        0      146 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/gyver/attrs/converters/__init__.py
+-rw-r--r--   0        0        0      751 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/gyver/attrs/converters/json.py
+-rw-r--r--   0        0        0     1516 2023-04-26 20:21:33.954424 gyver_attrs-0.5.0/gyver/attrs/converters/utils.py
+-rw-r--r--   0        0        0     5493 2023-04-26 20:27:12.428348 gyver_attrs-0.5.0/gyver/attrs/field.py
+-rw-r--r--   0        0        0     1046 2023-04-26 20:27:13.436336 gyver_attrs-0.5.0/gyver/attrs/helpers.py
+-rw-r--r--   0        0        0    24627 2023-04-26 20:27:13.447335 gyver_attrs-0.5.0/gyver/attrs/main.py
+-rw-r--r--   0        0        0     4793 2023-04-26 20:27:12.441348 gyver_attrs-0.5.0/gyver/attrs/methods.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:21:33.955424 gyver_attrs-0.5.0/gyver/attrs/py.typed
+-rw-r--r--   0        0        0     3872 2023-04-26 20:27:13.451335 gyver_attrs-0.5.0/gyver/attrs/resolver.py
+-rw-r--r--   0        0        0     4048 2023-04-26 20:27:13.454335 gyver_attrs-0.5.0/gyver/attrs/schema.py
+-rw-r--r--   0        0        0     4376 2023-04-26 20:27:13.455335 gyver_attrs-0.5.0/gyver/attrs/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:21:33.955424 gyver_attrs-0.5.0/gyver/attrs/utils/__init__.py
+-rw-r--r--   0        0        0      604 2023-04-26 20:21:33.955424 gyver_attrs-0.5.0/gyver/attrs/utils/factory.py
+-rw-r--r--   0        0        0     1441 2023-04-26 20:27:12.347349 gyver_attrs-0.5.0/gyver/attrs/utils/functions.py
+-rw-r--r--   0        0        0      298 2023-04-26 20:21:33.955424 gyver_attrs-0.5.0/gyver/attrs/utils/typedef.py
+-rw-r--r--   0        0        0      655 2023-04-26 20:28:32.336344 gyver_attrs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 gyver_attrs-0.5.0/PKG-INFO
```

### Comparing `gyver_attrs-0.4.0/LICENSE` & `gyver_attrs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.4.0/README.md` & `gyver_attrs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.4.0/gyver/attrs/__init__.py` & `gyver_attrs-0.5.0/gyver/attrs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from .camel import define_camel
 from .converters import asdict, asjson, fromdict, fromjson
 from .field import info
+from .helpers import call_init, fields
 from .main import define
-from .camel import define_camel
-from .helpers import fields, call_init
+from .shortcuts import kw_only, mutable
 from .utils.factory import mark_factory
-from .shortcuts import mutable, kw_only
 
 __all__ = [
     "info",
     "define",
     "define_camel",
     "mark_factory",
     "asdict",
@@ -17,9 +17,9 @@
     "fromjson",
     "fields",
     "call_init",
     "mutable",
     "kw_only",
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __version_info__ = tuple(map(int, __version__.split(".")))
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/camel.py` & `gyver_attrs-0.5.0/gyver/attrs/camel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Any, Callable, Literal, Optional, TypeVar, Union, overload
+
 import typing_extensions
 
 from gyver.attrs.main import define
+
 from .field import Field, FieldInfo, info
-from typing import Literal, Optional, TypeVar, Union, Callable, Any, overload
-from .utils.typedef import DisassembledType
 from .utils.functions import to_camel, to_upper_camel
+from .utils.typedef import DisassembledType
 
 T = TypeVar("T")
 
 
 class ToCamelField(Field):
     def __init__(
         self,
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/converters/json.py` & `gyver_attrs-0.5.0/gyver/attrs/converters/json.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.4.0/gyver/attrs/converters/utils.py` & `gyver_attrs-0.5.0/gyver/attrs/converters/utils.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.4.0/gyver/attrs/field.py` & `gyver_attrs-0.5.0/gyver/attrs/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 
     @property
     def field_type(self) -> type:
         return self.origin or self.declared_type
 
     @property
     def has_default(self) -> bool:
-        return self.default is not MISSING and not is_factory_marked(
-            self.default
-        )
+        return self.default is not MISSING and not is_factory_marked(self.default)
 
     @property
     def has_default_factory(self) -> bool:
         return is_factory_marked(self.default)
 
     @property
     def allow_none(self) -> bool:
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/helpers.py` & `gyver_attrs-0.5.0/gyver/attrs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, TypeVar, cast
-from typing_extensions import ParamSpec, Concatenate
+
+from typing_extensions import Concatenate, ParamSpec
 
 from .field import Field
 
 T = TypeVar("T")
 R = TypeVar("R")
 P = ParamSpec("P")
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/main.py` & `gyver_attrs-0.5.0/gyver/attrs/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import dataclasses
-from enum import Enum
 import typing
 from collections.abc import Callable
 from datetime import date, datetime, time, timedelta
+from enum import Enum
 
 import typing_extensions
 
-from gyver.attrs.converters.utils import (
-    deserialize,
-    deserialize_mapping,
-    fromdict,
-)
+from gyver.attrs import schema
+from gyver.attrs.converters.utils import (deserialize, deserialize_mapping,
+                                          fromdict)
 from gyver.attrs.field import Field, FieldInfo, info
 from gyver.attrs.methods import MethodBuilder, MethodType
 from gyver.attrs.resolver import FieldsBuilder
-from gyver.attrs import schema
 from gyver.attrs.utils.functions import frozen as freeze
 from gyver.attrs.utils.functions import indent
 from gyver.attrs.utils.typedef import MISSING, Descriptor, InitOptions
 
 T = typing.TypeVar("T")
 
 FieldMap = dict[str, Field]
@@ -32,15 +29,15 @@
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: typing.Optional[bool] = None,
-    pydantic: typing.Optional[bool] = None,
+    pydantic: bool = False,
     dataclass_fields: bool = False,
     field_class: type[Field] = Field,
 ) -> Callable[[type[T]], type[T]]:
     ...
 
 
 @typing.overload
@@ -51,15 +48,15 @@
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: typing.Optional[bool] = None,
-    pydantic: typing.Optional[bool] = None,
+    pydantic: bool = False,
     dataclass_fields: bool = False,
     field_class: type[Field] = Field,
 ) -> type[T]:
     ...
 
 
 @typing_extensions.dataclass_transform(
@@ -75,15 +72,15 @@
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: typing.Optional[bool] = None,
-    pydantic: typing.Optional[bool] = None,
+    pydantic: bool = False,
     dataclass_fields: bool = False,
     field_class: type[Field] = Field,
 ) -> typing.Union[Callable[[type[T]], type[T]], type[T]]:
     """
     Decorator function that adds functionality to a data class.
 
     :param maybe_cls: Optional[type[T]], a type argument that needs to be
@@ -129,16 +126,16 @@
         if eq:
             clsdict |= _get_eq(cls, field_map)
             clsdict |= _get_ne(cls)
         if order:
             clsdict |= _get_order(cls, field_map)
         if hash or (hash is None and frozen):
             clsdict |= _get_hash(cls, field_map, bool(hash))
-        if pydantic is not False:
-            clsdict |= _maybe_get_pydantic(cls, field_map, pydantic is True)
+        if pydantic:
+            clsdict |= _get_pydantic_handlers(cls, field_map)
         if dataclass_fields:
             clsdict |= _make_dataclass_fields(field_map)
         maybe_freeze = freeze if frozen else lambda a: a
         return maybe_freeze(
             type(cls)(  # type: ignore
                 cls.__name__,
                 cls.__bases__,
@@ -160,25 +157,22 @@
 def _get_slots_metadata(
     cls: type,
     field_map: FieldMap,
 ) -> typing.Mapping[str, typing.Any]:
     inherited_slots: dict[str, typing.Any] = {}
     for base_cls in cls.mro()[1:-1]:
         inherited_slots |= {
-            name: getattr(base_cls, name)
-            for name in getattr(base_cls, "__slots__", ())
+            name: getattr(base_cls, name) for name in getattr(base_cls, "__slots__", ())
         }
     reused_slots = {
         slot: descriptor
         for slot, descriptor in inherited_slots.items()
         if slot in field_map
     }
-    slot_names = tuple(
-        field for field in field_map if field not in reused_slots
-    )
+    slot_names = tuple(field for field in field_map if field not in reused_slots)
     for value in cls.__dict__.values():
         if _is_descriptor_type(value):
             slot_names += (value.private_name,)
     return inherited_slots | reused_slots | {"__slots__": tuple(slot_names)}
 
 
 def _is_descriptor_type(
@@ -190,17 +184,15 @@
 def _get_cls_metadata(cls: type):
     return {"__qualname__": cls.__qualname__}
 
 
 def _make_setattr(frozen: bool):
     def _setattr(field: str, arg: typing.Any):
         return (
-            f"_setattr(self, '{field}', {arg})"
-            if frozen
-            else f"self.{field} = {arg}"
+            f"_setattr(self, '{field}', {arg})" if frozen else f"self.{field} = {arg}"
         )
 
     return _setattr
 
 
 def _get_init(cls: type, field_map: FieldMap, opts: InitOptions):
     builder = MethodBuilder(
@@ -264,17 +256,15 @@
 
 
 _othername = "other"
 
 
 def _get_eq(cls: type, field_map: FieldMap):
     fields_to_compare = {
-        name: field
-        for name, field in field_map.items()
-        if field.eq is not False
+        name: field for name, field in field_map.items() if field.eq is not False
     }
     builder = MethodBuilder("__eq__").add_funcarg(_othername)
     if fields_to_compare:
         return _build_field_comparison(builder, fields_to_compare, cls)
     returnline = "return _object_eq(self, other)"
     return (
         builder.add_glob("_object_eq", object.__eq__)
@@ -325,16 +315,15 @@
         .add_annotation("alias", bool)
         .add_annotation("return", typing.Mapping[str, typing.Any])
     )
     for name, field in field_map.items():
         field_type = field.origin or field.declared_type
         if isinstance(field_type, str):
             raise NotImplementedError(
-                "For now gyver-attrs cannot deal correctly"
-                " with forward references"
+                "For now gyver-attrs cannot deal correctly" " with forward references"
             )
         builder.add_glob(f"field_type_{field.name}", field_type)
         if hasattr(field_type, "__parse_dict__"):
             arg = f"'{{name}}': self.{name}.__parse_dict__(alias)"
         elif not isinstance(field_type, type):
             arg = f"'{{name}}': self.{name}"
         elif issubclass(field_type, (list, tuple, set, dict)):
@@ -420,16 +409,15 @@
         .add_annotation("mapping", typing.Mapping[str, typing.Any])
         .set_type(MethodType.CLASS)
     )
     for field in field_map.values():
         field_type = field.origin or field.declared_type
         builder.add_glob(f"_field_type_{field.name}", field_type)
         get_line = (
-            f"dict_get(mapping, {field.name!r}, {field.alias!r},"
-            "sentinel, _dict_get)"
+            f"dict_get(mapping, {field.name!r}, {field.alias!r}," "sentinel, _dict_get)"
         )
         if hasattr(field_type, "__gserialize__"):
             arg = f"_field_type_{field.name}.__gserialize__({get_line})"
         elif field_type in (date, datetime):
             arg = f"_field_type_{field.name}.fromisoformat" f"({get_line})"
         elif not isinstance(field_type, type):
             arg = f"({get_line})"
@@ -445,16 +433,15 @@
 
 def _get_gserialize_sequence_arg(
     field: Field,
 ) -> tuple[str, typing.Mapping[str, typing.Any]]:
     field_type = field.origin or field.declared_type
     globs = {}
     default_line = (
-        f"dict_get(mapping, {field.name!r}, {field.alias!r},"
-        "sentinel, _dict_get)"
+        f"dict_get(mapping, {field.name!r}, {field.alias!r}," "sentinel, _dict_get)"
     )
 
     returnline = default_line
     if not field.args:
         pass
     elif (
         len(field.args) > 1
@@ -585,33 +572,24 @@
     return (
         builder.add_scriptline(f"return hash(({', '.join(args)}))")
         .add_annotation("return", int)
         .build(cls)
     )
 
 
-def _maybe_get_pydantic(cls: type, fields_map: FieldMap, wants_pydantic: bool):
-    try:
-        return _get_pydantic_handlers(cls, fields_map)
-    except Exception:
-        if wants_pydantic:
-            raise
-        return {}
-
-
 def _get_pydantic_handlers(cls: type, fields_map: FieldMap):
     namespace = {}
 
     # Create Validation Function
-    builder = MethodBuilder(
-        "__pydantic_validate__", {"fromdict": fromdict}
-    ).set_type(MethodType.CLASS)
-    builder.add_funcarg("value").add_annotation(
-        "value", typing.Any
-    ).add_annotation("return", cls)
+    builder = MethodBuilder("__pydantic_validate__", {"fromdict": fromdict}).set_type(
+        MethodType.CLASS
+    )
+    builder.add_funcarg("value").add_annotation("value", typing.Any).add_annotation(
+        "return", cls
+    )
     builder.add_scriptlines(
         "if isinstance(value, cls):",
         indent("return value"),
         "try:",
         indent("return fromdict(cls, dict(value))"),
         "except (TypeError, ValueError) as e:",
         indent(
@@ -650,27 +628,23 @@
 
 
 def _generate_schema_lines(fields_map: FieldMap) -> dict[str, schema.HasStr]:
     schemas: dict[str, schema.HasStr] = {}
     for field in fields_map.values():
         field_type = field.field_type
         if current_map := getattr(field_type, "__gyver_attrs__", None):
-            required = [
-                f.argname for f in current_map.values() if f.default is MISSING
-            ]
+            required = [f.argname for f in current_map.values() if f.default is MISSING]
             schemas[field.argname] = schema.Schema(
                 field_type.__name__,
                 "object",
                 required,
                 properties=_generate_schema_lines(current_map),
             )
         else:
-            schemas[field.argname] = _resolve_schematype(
-                field.field_type, field.args
-            )
+            schemas[field.argname] = _resolve_schematype(field.field_type, field.args)
     return schemas
 
 
 def _resolve_schematype(
     field_type: type, args: typing.Sequence[type]
 ) -> schema.HasToString:
     _type_map = {
@@ -682,18 +656,15 @@
     }
     if val := _type_map.get(field_type):
         return schema.DictSchema(val)
     if field_type in (list, set, tuple):
         extras = {}
         if args:
             extras["items"] = schema.Items(
-                *(
-                    _resolve_schematype(arg, typing.get_args(arg))
-                    for arg in args
-                )
+                *(_resolve_schematype(arg, typing.get_args(arg)) for arg in args)
             )
         return schema.DictSchema("array", **extras)
     if field_type is dict:
         extras = {}
         if args:
             keyt, valt = args
             if keyt is not str:
@@ -702,27 +673,23 @@
                     keyt,
                 )
             extras["additional_properties"] = _resolve_schematype(
                 valt, typing.get_args(valt)
             )
         return schema.DictSchema("object", **extras)
     if current_map := getattr(field_type, "__gyver_attrs__", None):
-        required = [
-            f.argname for f in current_map.values() if f.default is MISSING
-        ]
+        required = [f.argname for f in current_map.values() if f.default is MISSING]
         return schema.Schema(
             field_type.__name__,
             "object",
             required,
             properties=_generate_schema_lines(current_map),
         )
     if field_type is typing.Union:
-        choices = [
-            _resolve_schematype(arg, typing.get_args(arg)) for arg in args
-        ]
+        choices = [_resolve_schematype(arg, typing.get_args(arg)) for arg in args]
         return schema.ListSchema("anyOf", *choices)
     if issubclass(field_type, Enum):
         # remove from parents cls, enum.Enum and object
         # uses only the first of the mro
         parent, *_ = field_type.mro()[1:-2]
         if parent:
             if ft := _type_map.get(parent):
@@ -739,17 +706,15 @@
     if issubclass(field_type, datetime):
         return schema.DictSchema("string", format=schema.str_cast("date-time"))
     if issubclass(field_type, date):
         return schema.DictSchema("string", format=schema.str_cast("date"))
     if issubclass(field_type, time):
         return schema.DictSchema("string", format=schema.str_cast("time"))
     if issubclass(field_type, timedelta):
-        return schema.DictSchema(
-            "number", format=schema.str_cast("time-delta")
-        )
+        return schema.DictSchema("number", format=schema.str_cast("time-delta"))
     raise NotImplementedError
 
 
 def _make_dataclass_fields(fields_map: FieldMap):
     dc_fields = {}
     for field in fields_map.values():
         kwargs = {}
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/methods.py` & `gyver_attrs-0.5.0/gyver/attrs/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,15 @@
         else:
             self.funcargs.insert(0, "self")
         args = ", ".join(self.funcargs)
         if self.funckargs:
             args += f'{", " if args else ""}*, {", ".join(self.funckargs)}'
         method_signature = method_header + args + method_footer
 
-        method_body = (
-            "\n    ".join(self.script_lines) if self.script_lines else "pass"
-        )
+        method_body = "\n    ".join(self.script_lines) if self.script_lines else "pass"
         if method_decorator:
             method_signature = method_decorator + method_signature
 
         method_annotations = {
             name: value
             for name, value in self.annotations.items()
             if value is not Ellipsis
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/resolver.py` & `gyver_attrs-0.5.0/gyver/attrs/resolver.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 from typing import Sequence, cast
 
 from .field import Field, FieldInfo, default_info
-from .utils.functions import disassemble_type
 from .utils.factory import is_factory_marked, mark_factory
+from .utils.functions import disassemble_type
 from .utils.typedef import MISSING
 
 
 class FieldsBuilder:
     __slots__ = (
         "cls",
         "kw_only",
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/schema.py` & `gyver_attrs-0.5.0/gyver/attrs/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Protocol, Sequence, Union
+
 from .utils.functions import to_camel
 
 template = (
     '"title": "{title}"',
     '"type": "{type}"',
 )
 
@@ -49,16 +50,15 @@
         if not self.extras:
             return ""
         lines = [
             f'"{to_camel(name)}":'
             + (
                 " {"
                 + ", ".join(
-                    f'"{to_camel(key)}": {value!s}'
-                    for key, value in props.items()
+                    f'"{to_camel(key)}": {value!s}' for key, value in props.items()
                 )
                 + "}"
                 if isinstance(props, dict)
                 else str(props)
             )
             for name, props in self.extras.items()
         ]
@@ -153,15 +153,15 @@
         for name, props in self.extras.items():
             props_str = self._make_prop_str(props)
             lines.append(f'"{to_camel(name)}": {props_str}')
         return ", ".join(lines)
 
     def _make_prop_str(self, props: PropsType):
         if not isinstance(props, dict):
-            return props.to_string()
+            return str(props)
         props_str = ",".join(
             f'"{to_camel(key)}": {value!s}' for key, value in props.items()
         )
         return f"{{{props_str}}}"
 
     def build_required(self) -> str:
         return (
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/shortcuts.py` & `gyver_attrs-0.5.0/gyver/attrs/shortcuts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import typing
+
 import typing_extensions
-from .main import define
+
 from .field import FieldInfo, info
+from .main import define
 
 T = typing.TypeVar("T")
 
 ReturnT = typing.Union[typing.Callable[[type[T]], type[T]], type[T]]
 OptionalTypeT = typing.Optional[type[T]]
 
 
@@ -60,15 +62,15 @@
     order: bool = True,
     hash: typing.Optional[bool] = None,
     pydantic: bool = True,
     dataclass_fields: bool = True,
 ) -> ReturnT[T]:
     return define(
         maybe_cls,
-        frozen=True,
+        frozen=False,
         kw_only=kw_only,
         slots=slots,
         repr=repr,
         eq=eq,
         order=order,
         hash=hash,
         pydantic=pydantic,
@@ -137,7 +139,74 @@
         repr=repr,
         eq=eq,
         order=order,
         hash=hash,
         pydantic=pydantic,
         dataclass_fields=dataclass_fields,
     )
+
+
+@typing.overload
+def schema_class(
+    maybe_cls: None = None,
+    /,
+    *,
+    frozen: bool = False,
+    kw_only: bool = False,
+    slots: bool = True,
+    repr: bool = True,
+    eq: bool = True,
+    order: bool = True,
+    hash: typing.Optional[bool] = None,
+    dataclass_fields: bool = True,
+) -> typing.Callable[[type[T]], type[T]]:
+    ...
+
+
+@typing.overload
+def schema_class(
+    maybe_cls: type[T],
+    /,
+    *,
+    frozen: bool = False,
+    kw_only: bool = False,
+    slots: bool = True,
+    repr: bool = True,
+    eq: bool = True,
+    order: bool = True,
+    hash: typing.Optional[bool] = None,
+    dataclass_fields: bool = True,
+) -> type[T]:
+    ...
+
+
+@typing_extensions.dataclass_transform(
+    order_default=True,
+    frozen_default=True,
+    kw_only_default=False,
+    field_specifiers=(FieldInfo, info),
+)
+def schema_class(
+    maybe_cls: OptionalTypeT[T] = None,
+    /,
+    *,
+    frozen: bool = True,
+    kw_only: bool = False,
+    slots: bool = True,
+    repr: bool = True,
+    eq: bool = True,
+    order: bool = True,
+    hash: typing.Optional[bool] = None,
+    dataclass_fields: bool = True,
+) -> ReturnT[T]:
+    return define(
+        maybe_cls,
+        frozen=frozen,
+        kw_only=kw_only,
+        slots=slots,
+        repr=repr,
+        eq=eq,
+        order=order,
+        hash=hash,
+        pydantic=True,
+        dataclass_fields=dataclass_fields,
+    )
```

### Comparing `gyver_attrs-0.4.0/gyver/attrs/utils/factory.py` & `gyver_attrs-0.5.0/gyver/attrs/utils/factory.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.4.0/gyver/attrs/utils/functions.py` & `gyver_attrs-0.5.0/gyver/attrs/utils/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,28 +41,22 @@
 
 def implements(cls: type, name: str):
     attr = getattr(cls, name, _sentinel)
     if attr is _sentinel:
         return False
 
     return next(
-        (
-            False
-            for base_cls in cls.mro()[1:]
-            if getattr(base_cls, name, None) is attr
-        ),
+        (False for base_cls in cls.mro()[1:] if getattr(base_cls, name, None) is attr),
         True,
     )
 
 
 _to_camel_regex = re.compile("_([a-zA-Z])")
 
 
 def to_camel(string: str) -> str:
-    return _to_camel_regex.sub(
-        lambda match: match[1].upper(), string.strip("_")
-    )
+    return _to_camel_regex.sub(lambda match: match[1].upper(), string.strip("_"))
 
 
 def to_upper_camel(string: str) -> str:
     result = to_camel(string)
     return result[:1].upper() + result[1:]
```

### Comparing `gyver_attrs-0.4.0/pyproject.toml` & `gyver_attrs-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "gyver-attrs"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Gustavo Cardoso <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gyver" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 orjson = { version = "^3.8.6" }
-gyver-attrs-converter = { version = "^0.4.0" }
+gyver-attrs-converter = { version = "^0.5.0" }
 
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 autoflake = "^2.0.1"
 flake8 = "^6.0.0"
```

### Comparing `gyver_attrs-0.4.0/PKG-INFO` & `gyver_attrs-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: gyver-attrs
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Gustavo Cardoso
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gyver-attrs-converter (>=0.4.0,<0.5.0)
+Requires-Dist: gyver-attrs-converter (>=0.5.0,<0.6.0)
 Requires-Dist: orjson (>=3.8.6,<4.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Gyver Attrs
 
 Gyver-attrs is a Python library that provides a more flexible and feature-rich alternative to the built-in attrs and dataclasses libraries for defining classes. The main function provided by Gyver-attrs is define, which allows users to define classes with a range of options and features.
```

