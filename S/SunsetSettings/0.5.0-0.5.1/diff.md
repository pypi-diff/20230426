# Comparing `tmp/SunsetSettings-0.5.0.tar.gz` & `tmp/SunsetSettings-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SunsetSettings-0.5.0.tar", last modified: Sat Apr 22 19:52:25 2023, max compression
+gzip compressed data, was "SunsetSettings-0.5.1.tar", last modified: Wed Apr 26 17:37:17 2023, max compression
```

## Comparing `SunsetSettings-0.5.0.tar` & `SunsetSettings-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1698 2023-01-16 00:48:03.487746 SunsetSettings-0.5.0/.github/workflows/python-build.yml
--rw-r--r--   0        0        0       59 2022-08-04 10:12:23.781547 SunsetSettings-0.5.0/.gitignore
--rw-r--r--   0        0        0      233 2022-12-14 00:54:21.154949 SunsetSettings-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0    32422 2022-03-24 23:57:25.474661 SunsetSettings-0.5.0/LICENSE
--rw-r--r--   0        0        0     6132 2023-04-22 18:12:13.008561 SunsetSettings-0.5.0/README.md
--rw-r--r--   0        0        0      638 2022-08-04 10:11:43.364138 SunsetSettings-0.5.0/docs/Makefile
--rw-r--r--   0        0        0      804 2022-08-04 10:11:43.364138 SunsetSettings-0.5.0/docs/make.bat
--rw-r--r--   0        0        0     1168 2023-04-22 17:44:14.428052 SunsetSettings-0.5.0/docs/source/api.rst
--rw-r--r--   0        0        0     2176 2023-04-22 19:37:56.782226 SunsetSettings-0.5.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     2476 2022-12-19 01:40:30.636872 SunsetSettings-0.5.0/docs/source/conf.py
--rw-r--r--   0        0        0      788 2023-01-16 22:21:36.070670 SunsetSettings-0.5.0/docs/source/index.rst
--rw-r--r--   0        0        0      613 2022-11-20 03:11:09.133654 SunsetSettings-0.5.0/docs/source/installation.rst
--rw-r--r--   0        0        0    16965 2023-04-22 18:11:35.827153 SunsetSettings-0.5.0/docs/source/usage.rst
--rw-r--r--   0        0        0     1314 2022-12-19 15:06:00.615479 SunsetSettings-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1043 2023-04-22 19:17:46.521114 SunsetSettings-0.5.0/sunset/__init__.py
--rw-r--r--   0        0        0     8180 2023-04-22 11:08:18.204704 SunsetSettings-0.5.0/sunset/autosaver.py
--rw-r--r--   0        0        0    10354 2023-04-22 18:12:30.373219 SunsetSettings-0.5.0/sunset/bunch.py
--rw-r--r--   0        0        0     4799 2023-04-22 16:01:00.879583 SunsetSettings-0.5.0/sunset/enum_serializer.py
--rw-r--r--   0        0        0     4186 2023-04-22 10:51:57.496111 SunsetSettings-0.5.0/sunset/exporter.py
--rw-r--r--   0        0        0    15412 2023-04-22 19:10:03.411616 SunsetSettings-0.5.0/sunset/key.py
--rw-r--r--   0        0        0    14951 2023-04-22 18:13:28.415418 SunsetSettings-0.5.0/sunset/list.py
--rw-r--r--   0        0        0      993 2023-04-22 10:45:58.950590 SunsetSettings-0.5.0/sunset/lockable.py
--rw-r--r--   0        0        0     1961 2023-04-22 00:48:12.340576 SunsetSettings-0.5.0/sunset/non_hashable_set.py
--rw-r--r--   0        0        0     5620 2023-04-22 17:56:56.225696 SunsetSettings-0.5.0/sunset/protocols.py
--rw-r--r--   0        0        0        0 2022-04-05 17:36:11.873451 SunsetSettings-0.5.0/sunset/py.typed
--rw-r--r--   0        0        0     2366 2023-04-22 10:18:32.648125 SunsetSettings-0.5.0/sunset/registry.py
--rw-r--r--   0        0        0     2149 2023-04-22 15:22:51.676899 SunsetSettings-0.5.0/sunset/serializers.py
--rw-r--r--   0        0        0    18809 2023-04-22 18:14:03.188735 SunsetSettings-0.5.0/sunset/settings.py
--rw-r--r--   0        0        0     1155 2023-04-22 00:45:06.565561 SunsetSettings-0.5.0/sunset/timer.py
--rw-r--r--   0        0        0        0 2022-03-15 15:31:18.747300 SunsetSettings-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     6001 2023-04-22 00:45:13.261814 SunsetSettings-0.5.0/tests/test_autosaver.py
--rw-r--r--   0        0        0     9958 2023-04-22 00:45:17.709982 SunsetSettings-0.5.0/tests/test_bunch.py
--rw-r--r--   0        0        0     4709 2023-04-22 00:45:18.942028 SunsetSettings-0.5.0/tests/test_concurrency.py
--rw-r--r--   0        0        0     2763 2023-04-22 15:48:31.311277 SunsetSettings-0.5.0/tests/test_enum_serializer.py
--rw-r--r--   0        0        0     3453 2023-04-22 00:45:19.878064 SunsetSettings-0.5.0/tests/test_exporter.py
--rw-r--r--   0        0        0    18091 2023-04-22 19:15:30.535976 SunsetSettings-0.5.0/tests/test_key.py
--rw-r--r--   0        0        0    18679 2023-04-22 18:42:49.545885 SunsetSettings-0.5.0/tests/test_list.py
--rw-r--r--   0        0        0     1498 2023-04-22 00:45:22.574165 SunsetSettings-0.5.0/tests/test_non_hashable_set.py
--rw-r--r--   0        0        0     3949 2023-04-22 00:45:23.574203 SunsetSettings-0.5.0/tests/test_registry.py
--rw-r--r--   0        0        0     2766 2023-04-22 00:45:26.182301 SunsetSettings-0.5.0/tests/test_serializers.py
--rw-r--r--   0        0        0    23284 2023-04-22 18:10:01.511578 SunsetSettings-0.5.0/tests/test_settings.py
--rw-r--r--   0        0        0     1387 2023-04-22 00:45:30.914480 SunsetSettings-0.5.0/tests/test_timer.py
--rw-r--r--   0        0        0      251 2022-12-19 01:40:30.636872 SunsetSettings-0.5.0/tox.ini
--rw-r--r--   0        0        0     7215 1970-01-01 00:00:00.000000 SunsetSettings-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1698 2023-01-16 00:48:03.487746 SunsetSettings-0.5.1/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0       59 2022-08-04 10:12:23.781547 SunsetSettings-0.5.1/.gitignore
+-rw-r--r--   0        0        0      233 2022-12-14 00:54:21.154949 SunsetSettings-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0    32422 2022-03-24 23:57:25.474661 SunsetSettings-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6132 2023-04-22 18:12:13.008561 SunsetSettings-0.5.1/README.md
+-rw-r--r--   0        0        0      638 2022-08-04 10:11:43.364138 SunsetSettings-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-08-04 10:11:43.364138 SunsetSettings-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0     1168 2023-04-22 17:44:14.428052 SunsetSettings-0.5.1/docs/source/api.rst
+-rw-r--r--   0        0        0     2444 2023-04-26 17:35:03.367283 SunsetSettings-0.5.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2476 2022-12-19 01:40:30.636872 SunsetSettings-0.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0      788 2023-01-16 22:21:36.070670 SunsetSettings-0.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0      613 2022-11-20 03:11:09.133654 SunsetSettings-0.5.1/docs/source/installation.rst
+-rw-r--r--   0        0        0    16965 2023-04-22 18:11:35.827153 SunsetSettings-0.5.1/docs/source/usage.rst
+-rw-r--r--   0        0        0     1314 2022-12-19 15:06:00.615479 SunsetSettings-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1043 2023-04-26 17:35:21.479953 SunsetSettings-0.5.1/sunset/__init__.py
+-rw-r--r--   0        0        0     8180 2023-04-22 11:08:18.204704 SunsetSettings-0.5.1/sunset/autosaver.py
+-rw-r--r--   0        0        0    13130 2023-04-26 11:13:09.074925 SunsetSettings-0.5.1/sunset/bunch.py
+-rw-r--r--   0        0        0     5342 2023-04-26 17:18:51.236318 SunsetSettings-0.5.1/sunset/enum_serializer.py
+-rw-r--r--   0        0        0     4204 2023-04-22 23:40:18.194686 SunsetSettings-0.5.1/sunset/exporter.py
+-rw-r--r--   0        0        0    15786 2023-04-25 23:25:20.628967 SunsetSettings-0.5.1/sunset/key.py
+-rw-r--r--   0        0        0    15318 2023-04-25 22:40:56.351737 SunsetSettings-0.5.1/sunset/list.py
+-rw-r--r--   0        0        0      993 2023-04-22 10:45:58.950590 SunsetSettings-0.5.1/sunset/lockable.py
+-rw-r--r--   0        0        0     1961 2023-04-22 00:48:12.340576 SunsetSettings-0.5.1/sunset/non_hashable_set.py
+-rw-r--r--   0        0        0     5782 2023-04-25 22:53:13.491880 SunsetSettings-0.5.1/sunset/protocols.py
+-rw-r--r--   0        0        0        0 2022-04-05 17:36:11.873451 SunsetSettings-0.5.1/sunset/py.typed
+-rw-r--r--   0        0        0     2366 2023-04-22 10:18:32.648125 SunsetSettings-0.5.1/sunset/registry.py
+-rw-r--r--   0        0        0     2149 2023-04-22 15:22:51.676899 SunsetSettings-0.5.1/sunset/serializers.py
+-rw-r--r--   0        0        0    18795 2023-04-24 22:59:31.214434 SunsetSettings-0.5.1/sunset/settings.py
+-rw-r--r--   0        0        0     1155 2023-04-22 00:45:06.565561 SunsetSettings-0.5.1/sunset/timer.py
+-rw-r--r--   0        0        0        0 2022-03-15 15:31:18.747300 SunsetSettings-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     6001 2023-04-22 00:45:13.261814 SunsetSettings-0.5.1/tests/test_autosaver.py
+-rw-r--r--   0        0        0    11979 2023-04-26 11:22:18.362739 SunsetSettings-0.5.1/tests/test_bunch.py
+-rw-r--r--   0        0        0     4709 2023-04-22 00:45:18.942028 SunsetSettings-0.5.1/tests/test_concurrency.py
+-rw-r--r--   0        0        0     3379 2023-04-26 17:26:37.640756 SunsetSettings-0.5.1/tests/test_enum_serializer.py
+-rw-r--r--   0        0        0     3453 2023-04-22 00:45:19.878064 SunsetSettings-0.5.1/tests/test_exporter.py
+-rw-r--r--   0        0        0    18405 2023-04-25 19:09:15.495949 SunsetSettings-0.5.1/tests/test_key.py
+-rw-r--r--   0        0        0    19168 2023-04-25 19:08:45.010995 SunsetSettings-0.5.1/tests/test_list.py
+-rw-r--r--   0        0        0     1498 2023-04-22 00:45:22.574165 SunsetSettings-0.5.1/tests/test_non_hashable_set.py
+-rw-r--r--   0        0        0     3949 2023-04-22 00:45:23.574203 SunsetSettings-0.5.1/tests/test_registry.py
+-rw-r--r--   0        0        0     2766 2023-04-22 00:45:26.182301 SunsetSettings-0.5.1/tests/test_serializers.py
+-rw-r--r--   0        0        0    23284 2023-04-22 18:10:01.511578 SunsetSettings-0.5.1/tests/test_settings.py
+-rw-r--r--   0        0        0     1387 2023-04-22 00:45:30.914480 SunsetSettings-0.5.1/tests/test_timer.py
+-rw-r--r--   0        0        0      251 2022-12-19 01:40:30.636872 SunsetSettings-0.5.1/tox.ini
+-rw-r--r--   0        0        0     7215 1970-01-01 00:00:00.000000 SunsetSettings-0.5.1/PKG-INFO
```

### Comparing `SunsetSettings-0.5.0/.github/workflows/python-build.yml` & `SunsetSettings-0.5.1/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/LICENSE` & `SunsetSettings-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/README.md` & `SunsetSettings-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/Makefile` & `SunsetSettings-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/make.bat` & `SunsetSettings-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/source/api.rst` & `SunsetSettings-0.5.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/source/changelog.rst` & `SunsetSettings-0.5.1/docs/source/changelog.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+SunsetSettings 0.5.1 (2023-04-26)
+---------------------------------
+
+  - Made deserializing an enum case-insensitive when the result is non-ambiguous.
+  - Added ability to instantiate Bunches with default value overrides. This is still experimental and undocumented.
+
 SunsetSettings 0.5.0 (2023-04-22)
 ---------------------------------
 
   - Added ability to set a validator on Keys to limit their possible values.
   - Making a typo in a value when editing a settings file manually no longer causes the entry to be deleted on save.
   - Added ability to serialize Enum subclasses natively.
   - Deprecated now unnecessary SerializableEnum and -Flag classes.
```

### Comparing `SunsetSettings-0.5.0/docs/source/conf.py` & `SunsetSettings-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/source/index.rst` & `SunsetSettings-0.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/source/installation.rst` & `SunsetSettings-0.5.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/docs/source/usage.rst` & `SunsetSettings-0.5.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/pyproject.toml` & `SunsetSettings-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/__init__.py` & `SunsetSettings-0.5.1/sunset/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 "SunsetSettings: a type-safe, extensible settings system with inheritance."
 
 __project__ = "SunsetSettings"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __author__ = "P. Varet"
 __copyright__ = "2022-2023, P. Varet"
 
 from . import exporter, non_hashable_set, serializers
 
 from .autosaver import AutoSaver
 from .bunch import Bunch
```

### Comparing `SunsetSettings-0.5.0/sunset/autosaver.py` & `SunsetSettings-0.5.1/sunset/autosaver.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/bunch.py` & `SunsetSettings-0.5.1/sunset/bunch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import dataclasses
 import inspect
 import weakref
 
 from typing import (
     Any,
     Callable,
-    Iterable,
     Iterator,
     MutableSet,
     Optional,
-    Type,
     TypeVar,
     cast,
 )
 
 from .non_hashable_set import WeakNonHashableSet
 from .protocols import (
     Containable,
@@ -61,79 +59,139 @@
     """
 
     _parent: Optional[weakref.ref["Bunch"]]
     _children: MutableSet["Bunch"]
     _fields: dict[str, Field]
     _update_notification_callbacks: CallbackRegistry[UpdateNotifier]
     _update_notification_enabled: bool
+    _stored_defaults: dict[str, Any] = {}
 
-    def __new__(cls: Type[Self]) -> Self:
-        # Automatically promote relevant attributes to dataclass fields.
+    def __new__(cls: type[Self], **defaults: Any) -> Self:
+        # Build and return a dataclass constructed from this class. Keep a
+        # reference to that dataclass as a private class attribute, so that we
+        # only construct it once. This allows type identity checks (as in
+        # "type(a) is type (b)") to work.
+
+        del defaults  # unused in __new___().
+
+        _dataclass_attr = "__DATACLASS_CLASS"
+
+        dataclass_class: Optional[type[Self]] = None
+        if (dataclass_class := getattr(cls, _dataclass_attr, None)) is None:
+            # We haven't yet constructed a dataclass from this class. Construct
+            # one here.
+
+            cls_parents = cls.__bases__
+
+            dataclasses_fields: list[Any] = []
+
+            potential_fields = list(vars(cls).items())
+            for name, attr in potential_fields:
+                if inspect.isclass(attr):
+                    if attr.__name__ == name:
+                        # This is probably a class definition that just happens
+                        # to be located inside the containing Bunch definition.
+                        # This is fine.
+
+                        continue
+
+                    raise TypeError(
+                        f"Field '{name}' in the definition of '{cls.__name__}'"
+                        " is uninstantiated"
+                    )
+
+                if isinstance(attr, ItemTemplate):
+                    # Safety check: make sure the user isn't accidentally
+                    # overriding an existing attribute.
+
+                    for cls_parent in cls_parents:
+                        if getattr(cls_parent, name, None) is not None:
+                            raise TypeError(
+                                f"Field '{name}' in the definition of"
+                                f" '{cls.__name__}' overrides attribute of the"
+                                " same name declared in parent class"
+                                f" '{cls_parent.__name__}'; consider renaming"
+                                f" this field to '{name}_' for instance"
+                            )
+
+                    # Create a proper field from the attribute.
+
+                    field = dataclasses.field(default_factory=attr.newInstance)
+                    dataclasses_fields.append((name, attr.typeHint(), field))
+
+                    # Note that we delete the attribute now that the field is
+                    # created. This helps avoid a hard-to-debug problem if the
+                    # user subclasses a Bunch with a custom __init__() that
+                    # doesn't call super().__init__(). That would seem to work,
+                    # but any updates made to attributes of that bunch would
+                    # really be applied to the attribute of the Bunch *class*,
+                    # not the instance, which would cause 'weird action at a
+                    # distance' bugs. Deleting the original class attribute
+                    # prevents this entirely.
+
+                    delattr(cls, name)
+
+            # Create a dataclass based on this class. Note that we will be
+            # providing our own __init__() override below.
+
+            dataclass_class = cast(
+                type[Self],
+                dataclasses.make_dataclass(
+                    cls.__qualname__,
+                    dataclasses_fields,
+                    init=False,
+                    bases=(cls,) + cls_parents,
+                ),
+            )
+
+            # And store it on the class itself for later.
 
-        cls_parents = cls.__bases__
+            setattr(cls, _dataclass_attr, dataclass_class)
 
-        potential_fields = list(vars(cls).items())
-        for name, attr in potential_fields:
-            if inspect.isclass(attr):
-                if attr.__name__ == name:
-                    # This is probably a class definition that just happens to
-                    # be located inside the containing Bunch definition. This
-                    # is fine.
-
-                    continue
-
-                raise TypeError(
-                    f"Field '{name}' in the definition of '{cls.__name__}'"
-                    " is uninstantiated"
-                )
-
-            if isinstance(attr, ItemTemplate):
-                # Safety check: make sure the user isn't accidentally overriding
-                # an existing attribute.
-
-                for cls_parent in cls_parents:
-                    if getattr(cls_parent, name, None) is not None:
-                        raise TypeError(
-                            f"Field '{name}' in the definition of"
-                            f" '{cls.__name__}' overrides attribute of the same"
-                            f" name declared in parent class"
-                            f" '{cls_parent.__name__}'; consider"
-                            f" renaming this field to '{name}_' for instance"
-                        )
-
-                setattr(
-                    cls,
-                    name,
-                    dataclasses.field(default_factory=attr.newInstance),
-                )
-
-                # Dataclass instantiation raises an error if a field does not
-                # have an explicit type annotation. But our Key, List and
-                # Bunch fields are unambiguously typed, so we don't actually
-                # need the annotation. So we just tell the dataclass that the
-                # type of non-explicitly-annotated fields is 'Any'. Turns out,
-                # this works.
-
-                # Also note the subtle dance here: the annotations need to be on
-                # *this* class, and not inherited from a parent class. So we
-                # make sure that the __annotations__ mapping does exist in this
-                # class' namespace.
-
-                if "__annotations__" not in cls.__dict__:
-                    setattr(cls, "__annotations__", {})
-                cls.__annotations__.setdefault(name, Any)
+        # And finally, return an instance of the dataclass. Phew.
 
-        # Create a new instance of this class wrapped as a dataclass.
+        return super().__new__(dataclass_class)
 
-        wrapped = dataclasses.dataclass()(cls)
-        return super().__new__(wrapped)
-
-    def __post_init__(self) -> None:
+    def __init__(self, **defaults: Any) -> None:
         super().__init__()
 
+        self._stored_defaults = {}
+
+        # Set up the Bunch fields.
+
+        # First, look up internal dataclass attribute names.
+
+        fields_attr: str = getattr(dataclasses, "_FIELDS")
+        field_type: Any = getattr(dataclasses, "_FIELD")
+        fields: dict[str, dataclasses.Field[Any]] = getattr(
+            self, fields_attr, {}
+        )
+
+        # Then look up the fields stored in the dataclass.
+
+        for field in fields.values():
+            if getattr(field, "_field_type", None) is not field_type:
+                continue
+
+            if field.default_factory is dataclasses.MISSING:
+                continue
+
+            new_attr = field.default_factory()
+            if (
+                isinstance(new_attr, Field)
+                and (default := defaults.get(field.name, None)) is not None
+            ):
+                new_attr = new_attr.withDefault(default)
+                self._stored_defaults[field.name] = default
+
+            setattr(self, field.name, new_attr)
+
+        self.__post_init__()
+
+    def __post_init__(self) -> None:
         self._parent = None
         self._children = WeakNonHashableSet[Bunch]()
         self._fields = {}
         self._update_notification_callbacks = CallbackRegistry()
         self._update_notification_enabled = True
 
         for label, field in vars(self).items():
@@ -272,15 +330,15 @@
 
         Returns:
             True if any field set on this Bunch is set, else False.
         """
 
         return any(field.isSet() for field in self._fields.values())
 
-    def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+    def dumpFields(self) -> Iterator[tuple[str, Optional[str]]]:
         """
         Internal.
         """
 
         if not self.isPrivate():
             for _, field in sorted(self._fields.items()):
                 yield from field.dumpFields()
@@ -317,17 +375,36 @@
             field = self
 
         self._update_notification_callbacks.callAll(field)
 
         if (container := self.container()) is not None and not self.isPrivate():
             container.triggerUpdateNotification(field)
 
-    def newInstance(self: Self) -> Self:
+    def typeHint(self) -> type:
+        return type(self)
+
+    def newInstance(
+        self: Self, _defaults: Optional[dict[str, Any]] = None
+    ) -> Self:
         """
         Internal. Returns a new instance of this Bunch with the same fields.
 
         Returns:
             A Bunch instance.
         """
 
-        new = self.__class__()
+        # Make sure the defaults are carried along to the new instance.
+
+        defaults = _defaults.copy() if _defaults else {}
+        defaults.update(self._stored_defaults)
+
+        new = self.__class__(**defaults)
         return new
+
+    def withDefault(self: Self, default: Any) -> Self:
+        # If a valid override was provided, return that override.
+
+        return (
+            default.newInstance(self._stored_defaults)
+            if type(default) is type(self)
+            else self
+        )
```

### Comparing `SunsetSettings-0.5.0/sunset/enum_serializer.py` & `SunsetSettings-0.5.1/sunset/enum_serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,22 +79,41 @@
 
         for name, member in self._type.__members__.items():
             if isinstance(member, self._type):
                 members[name] = member
 
         return members
 
+    def _lookupMember(self, name: str) -> Optional[_EnumT]:
+        candidates: list[_EnumT] = []
+
+        for candidate_name, member in self._members().items():
+            candidate_name = candidate_name.strip()
+
+            if candidate_name == name.strip():
+                return member
+
+            candidate_name = candidate_name.strip().lower()
+            if candidate_name == name.strip().lower():
+                candidates.append(member)
+
+        if len(candidates) == 1:
+            return candidates[0]
+
+        return None
+
     def fromStr(self, string: str) -> Optional[_EnumT]:
         # value is either a single word, or, in the case of Flag enums, multiple
         # words separated by a pipe. We handle both cases together here.
 
-        members = self._members()
         names = string.split("|") if "|" in string else [string]
         named_members = [
-            members[n] for name in names if (n := name.strip()) in members
+            member
+            for name in names
+            if (member := self._lookupMember(name)) is not None
         ]
 
         if not named_members:
             return None
 
         if issubclass(self._type, enum.Flag):
             # At this point, we know that all the members are instances of this
```

### Comparing `SunsetSettings-0.5.0/sunset/exporter.py` & `SunsetSettings-0.5.1/sunset/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, Optional, IO
+from typing import Iterable, Iterator, Optional, IO
 
 
 _SECTION_SEPARATOR = "/"
 _PATH_SEPARATOR = "."
 
 
 def normalize(string: str, to_lower: bool = True) -> str:
@@ -102,15 +102,15 @@
 # TODO: turn into a function (like dump_to_ini maybe) that takes the data and
 # yields lines of text, and then use file.writelines.
 def save_to_file(
     file: IO[str],
     data: Iterable[tuple[str, Optional[str]]],
     *,
     blanklines: bool,
-):
+) -> None:
     need_space = False
     current_section = ""
 
     def extract_section(path: str) -> tuple[str, str]:
         if _SECTION_SEPARATOR not in path:
             return "", ""
 
@@ -139,15 +139,15 @@
             if dump is not None:
                 file.write(f" {maybe_escape(dump)}")
             file.write("\n")
 
 
 def load_from_file(
     file: IO[str], main: str
-) -> Iterable[tuple[str, Optional[str]]]:
+) -> Iterator[tuple[str, Optional[str]]]:
     main = normalize(main)
 
     current_section = ""
 
     for line in file:
         line = line.strip()
```

### Comparing `SunsetSettings-0.5.0/sunset/key.py` & `SunsetSettings-0.5.1/sunset/key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import weakref
 
+from types import GenericAlias
 from typing import (
     Any,
     Callable,
     Generic,
-    Iterable,
     Iterator,
     Optional,
     TypeVar,
     cast,
 )
 
 from .exporter import maybe_escape
@@ -405,15 +405,15 @@
         Returns:
             An iterator over Keys of the same type as this one.
         """
 
         for child in self._children:
             yield cast(Self, child)
 
-    def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+    def dumpFields(self) -> Iterator[tuple[str, Optional[str]]]:
         if not self.isPrivate():
             if self.isSet():
                 yield self.fieldPath(), self._serializer.toStr(self.get())
 
             elif self._bad_value_string is not None:
                 # If a bad value was set in the settings file for this Key, and
                 # the Key was not modified since, then save the bad value again.
@@ -470,25 +470,35 @@
             return
 
         self._update_notification_callbacks.callAll(self)
 
         if (container := self.container()) is not None and not self.isPrivate():
             container.triggerUpdateNotification(self)
 
-    def newInstance(self: Self) -> Self:
+    def typeHint(self) -> GenericAlias:
+        return GenericAlias(type(self), self._type)
+
+    def newInstance(self: Self, _default: Optional[_T] = None) -> Self:
         """
         Internal. Returns a new instance of this Key with the same default
         value.
 
         Returns:
             A new Key.
         """
 
-        return self.__class__(
-            default=self._default, serializer=self._serializer
+        default = _default if _default is not None else self._default
+
+        return self.__class__(default=default, serializer=self._serializer)
+
+    def withDefault(self: Self, default: Any) -> Self:
+        return (
+            self.newInstance(default)
+            if isinstance(default, self._type)
+            else self
         )
 
     def __repr__(self) -> str:
         type_name = self._type.__name__
         value = maybe_escape(self._serializer.toStr(self.get()))
         if not self.isSet():
             value = f"({value})"
```

### Comparing `SunsetSettings-0.5.0/sunset/list.py` & `SunsetSettings-0.5.1/sunset/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import weakref
 
 from enum import Enum, auto
+from types import GenericAlias
 from typing import (
     Any,
     Callable,
     Iterable,
     Iterator,
     MutableSequence,
     Optional,
@@ -415,15 +416,15 @@
         Note:
             This method does not increase the reference count of the given
             callback.
         """
 
         self._update_notification_callbacks.add(callback)
 
-    def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+    def dumpFields(self) -> Iterator[tuple[str, Optional[str]]]:
         """
         Internal.
         """
 
         if not self.isPrivate():
             for item in self._contents:
                 if not item.isSet():
@@ -478,24 +479,32 @@
             field = self
 
         self._update_notification_callbacks.callAll(field)
 
         if (container := self.container()) is not None and not self.isPrivate():
             container.triggerUpdateNotification(field)
 
-    def newInstance(self: Self) -> Self:
+    def typeHint(self) -> GenericAlias:
+        return GenericAlias(type(self), type(self._template))
+
+    def newInstance(self: Self, _template: Optional[ListItemT] = None) -> Self:
         """
         Internal. Returns a new instance of this List capable of holding the
         same type.
 
         Returns:
             A new List.
         """
 
-        return self.__class__(template=self._template, order=self._iter_order)
+        template = _template if _template is not None else self._template
+
+        return self.__class__(template=template, order=self._iter_order)
+
+    def withDefault(self: Self, default: Any) -> Self:
+        return self.newInstance(self._template.withDefault(default))
 
     def __repr__(self) -> str:
         parent = self.parent()
         items = [repr(item) for item in self.iter(order=IterOrder.NO_PARENT)]
         if parent is not None and self._iter_order == IterOrder.PARENT_FIRST:
             items.insert(0, "<parent>")
         if parent is not None and self._iter_order == IterOrder.PARENT_LAST:
```

### Comparing `SunsetSettings-0.5.0/sunset/lockable.py` & `SunsetSettings-0.5.1/sunset/lockable.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/non_hashable_set.py` & `SunsetSettings-0.5.1/sunset/non_hashable_set.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/protocols.py` & `SunsetSettings-0.5.1/sunset/protocols.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import weakref
 
+from types import GenericAlias
 from typing import (
     Any,
     Callable,
     Generic,
-    Iterable,
     Iterator,
     Optional,
     Protocol,
     TypeVar,
+    Union,
     runtime_checkable,
 )
 
 
 Self = TypeVar("Self")
 _T = TypeVar("_T")
 
@@ -88,15 +89,15 @@
 
     def children(self: Self) -> Iterator[Self]:
         ...
 
 
 @runtime_checkable
 class Dumpable(Protocol):
-    def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+    def dumpFields(self) -> Iterator[tuple[str, Optional[str]]]:
         ...
 
     def restoreField(self, path: str, value: Optional[str]) -> bool:
         ...
 
     def isSet(self) -> bool:
         ...
@@ -106,17 +107,23 @@
 class UpdateNotifier(Protocol):
     def onUpdateCall(self, callback: Callable[[Any], Any]) -> None:
         ...
 
 
 @runtime_checkable
 class ItemTemplate(Protocol):
+    def typeHint(self) -> Union[type, GenericAlias]:
+        ...
+
     def newInstance(self: Self) -> Self:
         ...
 
+    def withDefault(self: Self, default: Any) -> Self:
+        ...
+
 
 @runtime_checkable
 class Containable(Protocol):
     _PATH_SEPARATOR: str
 
     def setContainer(
         self, label: str, container: Optional["Container"]
```

### Comparing `SunsetSettings-0.5.0/sunset/registry.py` & `SunsetSettings-0.5.1/sunset/registry.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/serializers.py` & `SunsetSettings-0.5.1/sunset/serializers.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/sunset/settings.py` & `SunsetSettings-0.5.1/sunset/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pathlib
 
 from typing import (
     Any,
     Callable,
     ContextManager,
     IO,
-    Iterable,
     Iterator,
     MutableSet,
     Optional,
     TypeVar,
     Union,
 )
 
@@ -427,15 +426,15 @@
             + ("?" if self.isPrivate() else self.sectionName())
             + self._SECTION_SEPARATOR
         )
 
     def isPrivate(self) -> bool:
         return self.sectionName() == ""
 
-    def dumpFields(self) -> Iterable[tuple[str, Optional[str]]]:
+    def dumpFields(self) -> Iterator[tuple[str, Optional[str]]]:
         """
         Internal.
         """
 
         if not self.isPrivate():
             # Ensure the section is dumped event if empty. Dumping an empty
             # section is valid.
```

### Comparing `SunsetSettings-0.5.0/sunset/timer.py` & `SunsetSettings-0.5.1/sunset/timer.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_autosaver.py` & `SunsetSettings-0.5.1/tests/test_autosaver.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_bunch.py` & `SunsetSettings-0.5.1/tests/test_bunch.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,29 @@
         assert child_bunch in parent_bunch.children()
         assert child_bunch.parent() is parent_bunch
 
         child_bunch.setParent(None)
         assert child_bunch not in parent_bunch.children()
         assert child_bunch.parent() is None
 
+    def test_bunch_dataclass_mro(self) -> None:
+        # Bunch instantiation is a tad tricky. Here we make sure that attributes
+        # of a Bunch that are not SunsetSetting fields do work as expected.
+
+        class ExampleBunchSubclass(Bunch):
+            a = Key("test a")
+            b = "random attribute"
+
+            def test_a(self) -> str:
+                return self.a.get()
+
+        bunch = ExampleBunchSubclass()
+        assert bunch.test_a() == "test a"
+        assert bunch.b == "random attribute"
+
     def test_parenting(self) -> None:
         parent_bunch = ExampleBunch()
         child_bunch = ExampleBunch()
         child_bunch.setParent(parent_bunch)
 
         assert child_bunch.parent() is parent_bunch
         assert child_bunch in parent_bunch.children()
@@ -300,7 +315,59 @@
         class Dummy:
             pass
 
         def callback(_: ExampleBunch) -> Dummy:
             return Dummy()
 
         bunch.onUpdateCall(callback)
+
+    def test_with_defaults(self) -> None:
+        bunch = ExampleBunch(
+            a="overridden",
+            inner_bunch=ExampleBunch.InnerBunch(b=101),
+        )
+
+        assert bunch.a.get() == "overridden"
+        assert not bunch.a.isSet()
+        assert bunch.a.parent() is None
+        assert bunch.inner_bunch.b.get() == 101
+        assert not bunch.inner_bunch.b.isSet()
+
+    def test_defaults_persist_to_new_instances(self) -> None:
+        class TestBunch(Bunch):
+            a = Key(default=0)
+            b = Key(default=0)
+            c = Key(default=0)
+
+        bunch = TestBunch(a=1, b=1).withDefault(
+            TestBunch(b=2).withDefault(TestBunch(a=2, c=1))
+        )
+
+        assert bunch.a.get() == 2
+        assert bunch.b.get() == 2
+        assert bunch.c.get() == 1
+
+    def test_init_properly_called(self) -> None:
+        called: list[Bunch] = []
+
+        class TestBunch(Bunch):
+            a = Key(default=0)
+
+            def __init__(self) -> None:
+                super().__init__()
+                called.append(self)
+
+        bunch = TestBunch()
+        assert bunch in called
+        assert bunch.a.get() == 0
+
+    def test_missing_init_super_causes_attribute_error(self) -> None:
+        class TestBunch(Bunch):
+            a = Key(default=0)
+
+            def __init__(self) -> None:
+                # This incorrectly fails to call super().__init__().
+                pass
+
+        bunch = TestBunch()
+        with pytest.raises(AttributeError):
+            bunch.a
```

### Comparing `SunsetSettings-0.5.0/tests/test_concurrency.py` & `SunsetSettings-0.5.1/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_enum_serializer.py` & `SunsetSettings-0.5.1/tests/test_enum_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,7 +82,22 @@
 
     def test_int_flag(self) -> None:
         serializer = lookup(IntFlagExample)
         assert serializer is not None
 
         assert serializer.toStr(IntFlagExample.A | IntFlagExample.B) == "A|B"
         assert serializer.fromStr("A|B") == IntFlagExample.A | IntFlagExample.B
+
+    def test_flexible_case_matching(self) -> None:
+        class TestEnum(enum.Enum):
+            TEST1 = enum.auto()
+            test1 = enum.auto()
+            TEST2 = enum.auto()
+
+        serializer = lookup(TestEnum)
+        assert serializer is not None
+        assert serializer.fromStr("TEST1") == TestEnum.TEST1
+        assert serializer.fromStr("test1") == TestEnum.test1
+        assert serializer.fromStr("Test1") is None
+        assert serializer.fromStr("TEST2") == TestEnum.TEST2
+        assert serializer.fromStr("test2") == TestEnum.TEST2
+        assert serializer.fromStr("Test2") == TestEnum.TEST2
```

### Comparing `SunsetSettings-0.5.0/tests/test_exporter.py` & `SunsetSettings-0.5.1/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_key.py` & `SunsetSettings-0.5.1/tests/test_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -588,7 +588,18 @@
                 return NotSerializable()
 
         key = Key(default=NotSerializable(), serializer=Serializer())
         other_key = key.newInstance()
         other_key.set(NotSerializable())
 
         assert list(other_key.dumpFields()) == [("", "test")]
+
+    def test_with_default(self) -> None:
+        key = Key(default=0)
+        other_key = key.withDefault(1)
+
+        assert other_key.get() == 1
+        assert not other_key.isSet()
+        assert other_key.parent() is None
+
+        invalid_key = key.withDefault("invalid")
+        assert invalid_key.get() == 0
```

### Comparing `SunsetSettings-0.5.0/tests/test_list.py` & `SunsetSettings-0.5.1/tests/test_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -589,7 +589,21 @@
         list_iter_no_parent.appendOne().set(1)
         list_iter_parent_first.appendOne().set(1)
         list_iter_parent_last.appendOne().set(1)
 
         assert repr(list_iter_no_parent) == "[<Key[int]:1>]"
         assert repr(list_iter_parent_first) == "[<parent>,<Key[int]:1>]"
         assert repr(list_iter_parent_last) == "[<Key[int]:1>,<parent>]"
+
+    def test_with_default(self) -> None:
+        default_list = List(Key(default=0))
+
+        other_list = default_list.withDefault(1)
+        other_list.appendOne()
+        assert len(other_list) == 1
+        assert other_list[0].get() == 1
+        assert not other_list[0].isSet()
+
+        invalid_default_list = default_list.withDefault("invalid")
+        invalid_default_list.appendOne()
+        assert len(invalid_default_list) == 1
+        assert invalid_default_list[0].get() == 0
```

### Comparing `SunsetSettings-0.5.0/tests/test_non_hashable_set.py` & `SunsetSettings-0.5.1/tests/test_non_hashable_set.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_registry.py` & `SunsetSettings-0.5.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_serializers.py` & `SunsetSettings-0.5.1/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_settings.py` & `SunsetSettings-0.5.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/tests/test_timer.py` & `SunsetSettings-0.5.1/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `SunsetSettings-0.5.0/PKG-INFO` & `SunsetSettings-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunsetSettings
-Version: 0.5.0
+Version: 0.5.1
 Summary: SunsetSettings: a type-safe, extensible settings system with inheritance.
 Author-email: "P. Varet" <p.varet@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

