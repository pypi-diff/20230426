# Comparing `tmp/admem-1.9.0.tar.gz` & `tmp/admem-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-1.9.0.tar", last modified: Fri Jan 13 10:16:56 2023, max compression
+gzip compressed data, was "admem-2.0.0.tar", last modified: Wed Apr 26 00:03:00 2023, max compression
```

## Comparing `admem-1.9.0.tar` & `admem-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 10:16:56.692778 admem-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-01-13 07:41:40.000000 admem-1.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      331 2023-01-13 10:16:56.696779 admem-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-01-13 10:16:56.696779 admem-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 10:16:56.680778 admem-1.9.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 10:16:56.688778 admem-1.9.0/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-01-13 09:19:31.000000 admem-1.9.0/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6083 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     5453 2023-01-13 09:19:31.000000 admem-1.9.0/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-13 07:41:40.000000 admem-1.9.0/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 10:16:56.692778 admem-1.9.0/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      331 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      565 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      147 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-13 10:16:56.000000 admem-1.9.0/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.387689 admem-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-26 00:03:00.387689 admem-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-26 00:03:00.387689 admem-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.355688 admem-2.0.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.375689 admem-2.0.0/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-25 23:38:34.000000 admem-2.0.0/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6524 2023-04-25 23:57:00.000000 admem-2.0.0/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2023-04-25 23:38:34.000000 admem-2.0.0/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-04-25 23:57:00.000000 admem-2.0.0/source/admem/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.387689 admem-2.0.0/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 00:02:17.000000 admem-2.0.0/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/top_level.txt
```

### Comparing `admem-1.9.0/LICENSE.txt` & `admem-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/setup.cfg` & `admem-2.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,37 +11,47 @@
 zip_safe = False
 packages = find:
 package_dir = 
 	= source
 python_requires = >=3.10
 install_requires = 
 	django-db
+scripts = 
 
 [options.packages.find]
 where = source
 
 [options.entry_points]
 console_scripts = 
 
 [options.package_data]
 * = *.typed
 admem = 
 	source/admem/py.typed
 
 [options.extras_require]
+dev = 
+	adaux==2.4.0
+	pre-commit>=2.20
+	mypy==1.1.1
+	pylint==2.17.1
+	django-stubs==1.12.0
 test = 
 	pytest>=7.2
 	pytest-cov~=4.0
 docs = 
-	sphinx>=5.2.0
+	sphinx>=5.3.0
 	sphinx-rtd-theme>=1.0.0
 	sphinx-click>=4.3
 	jupyter-sphinx>=0.4
 	bash_kernel>=0.8
 
 [tool:pytest]
+markers = 
+	merge_only: run test only on merge request
+addopts = --strict-markers -m "not merge_only"
 cache_dir = devops/cache/pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `admem-1.9.0/source/admem/__init__.py` & `admem-2.0.0/source/admem/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 from django.conf import settings
 
 from . import _create_django_model
 from . import _decorator
 from . import _inspect_dataclass
 from . import _store_setup
 from . import _sync_store
+from . import fields
 from ._create_django_model import *
 from ._decorator import *
 from ._inspect_dataclass import *
 from ._store_setup import *
 from ._sync_store import *
+from .fields import *
 
 
 __all__ = (
     _decorator.__all__
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
+    + fields.__all__
 )
 
 
-__version__ = "1.9.0"
+__version__ = "2.0.0"
```

### Comparing `admem-1.9.0/source/admem/_backend_manager_proxy.py` & `admem-2.0.0/source/admem/_backend_manager_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/source/admem/_create_django_model.py` & `admem-2.0.0/source/admem/_create_django_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import django.db  # pylint: disable=unused-import
 from django.db import models
 
 from ._decorator import BACKEND_LINKER
 from ._decorator import django_model
 from ._inspect_dataclass import InspectDataclass
 from ._util import public_name
+from .fields import DjangoPathField
 
 # 2023-Q1: sphinx has a bug regarding adjusting the signature for attributes,
 # hence I need fully qualified imports for typing and django.db
 
 __all__ = ["CreateDjangoModel", "create_django_model"]
 
 
@@ -25,18 +26,27 @@
 class CreateDjangoModel(InspectDataclass):
     alt_field_type: "dict[str, type[django.db.models.Field[typing.Any, typing.Any]]]" = dc.field(
         default_factory=dict
     )
 
     def __post_init__(self) -> None:
         # evaluate the Meta class
-        pk_key, unique_together, extra_kwgs, ordering = self.extract_meta()
+        (
+            pk_key,
+            unique_together,
+            extra_kwgs,
+            ordering,
+            app_label,
+            db_table,
+        ) = self.extract_meta()
         # translate fields
         fields: dict[str, tp.Any] = self.translate_fields(pk_key, extra_kwgs)
-        fields["Meta"] = self.generate_meta(unique_together, ordering)
+        fields["Meta"] = self.generate_meta(
+            unique_together, ordering, app_label, db_table
+        )
         # pylint: disable=comparison-with-callable
         if self.dataclass.__str__ != object.__str__:  # type: ignore
             fields["__str__"] = self.dataclass.__str__
         fields["__module__"] = fields["Meta"].app_label
         dj_model = type(self.dataclass.__name__, (models.Model,), fields)
         BACKEND_LINKER.link(self.dataclass, dj_model)
 
@@ -69,20 +79,31 @@
             raise RuntimeError(
                 f"unused alt_field_type ({self.alt_field_type}) found for {self.dataclass}, please adjust!"
             )
 
         return fields
 
     def generate_meta(
-        self, unique_together: list[str] | None, ordering: list[str] | None
+        self,
+        unique_together: list[str] | None,
+        ordering: list[str] | None,
+        app_label: str | None,
+        db_table: str | None,
     ) -> type:
-        class Meta:
+        if app_label is None:
             app_label = public_name(self.dataclass, without_cls=True)
+        if db_table is None:
             db_table = public_name(self.dataclass)
 
+        class Meta:
+            pass
+
+        Meta.app_label = app_label  # type: ignore
+        Meta.db_table = db_table  # type: ignore
+
         if unique_together:
             Meta.unique_together = unique_together  # type: ignore
 
         if ordering:
             Meta.ordering = ordering  # type: ignore
 
         return Meta
@@ -136,15 +157,15 @@
             for val in type_.__members__.values():
                 choices.append((val.value, val.value))
                 assert len(val.value) < max_length
 
             return models.CharField, dict(max_length=max_length, choices=choices)
 
         if issubclass(type_, Path):
-            return models.FileField, dict(max_length=255)
+            return DjangoPathField, dict(max_length=1024)
 
         try:  # try Foreign Key relation (many-to-one)
             fk_class = BACKEND_LINKER.backend_class(type_)
             assert issubclass(fk_class, models.Model)
             return models.ForeignKey, dict(
                 to=fk_class, on_delete=models.CASCADE, related_name="+"
             )
```

### Comparing `admem-1.9.0/source/admem/_decorator.py` & `admem-2.0.0/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/source/admem/_django_store.py` & `admem-2.0.0/source/admem/_django_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Copyright (c) 2022-2023 Mario S. Könz; License: MIT
 import dataclasses as dc
 import enum
 import types
 import typing as tp
 from pathlib import Path
 
-from django.conf import settings
-from django.core.files import File
 from django.db import models
 
 from ._create_django_model import InspectDataclass
 from ._decorator import BACKEND_LINKER
 from ._decorator import django_model
 from ._protocols import T
+from .fields import DjangoPath
 
 
 @dc.dataclass
 class DjangoStore:
     identifier: str
 
     def dump(self, dc_obj: tp.Any) -> "tuple[models.Model, bool]":
@@ -62,29 +61,15 @@
             key = field.name
             val = getattr(dc_obj, key)
             if type(val) in BACKEND_LINKER.dc_to_backend:
                 val, _ = self.dump(val)
             if isinstance(val, enum.Enum):
                 val = val.value
             if isinstance(val, Path) and val is not None:
-
-                def get_file(path: Path) -> "File[tp.Any]":
-                    return File(
-                        open(path, "rb"),  # pylint: disable=consider-using-with
-                        name=path.name,
-                    )
-
-                try:
-                    val = get_file(val)
-                    update_origin[key] = lambda x: Path(x.url)
-                except FileNotFoundError as err:
-                    loc = Path(settings.MEDIA_ROOT) / val.relative_to(val.root)
-                    if not loc.exists():
-                        raise err
-                    val = get_file(loc)
+                update_origin[key] = DjangoPath
 
             # pylint: disable=protected-access
             dj_model = model._meta.get_field(key)
             if isinstance(dj_model, models.ManyToManyField):
                 m2m[key] = val
             else:
                 kwgs[key] = val
@@ -122,16 +107,15 @@
                     val = {self.django_to_dataclass(x) for x in val.all()}
                 else:
                     raise RuntimeError(f"field type {origin} not supported yet!")
 
             if issubclass(field_type, enum.Enum):
                 val = field_type(val)
             if issubclass(field_type, Path):
-                val = Path(val.url)
-
+                pass
             obj_kwgs[field.name] = val
         return dataclass(**obj_kwgs)
 
     parse = django_to_dataclass
 
     def backend_manager(self, dataclass: type[T]) -> tp.Any:
         return django_model(dataclass).objects.using(self.identifier)
```

### Comparing `admem-1.9.0/source/admem/_inspect_dataclass.py` & `admem-2.0.0/source/admem/_inspect_dataclass.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,16 +12,25 @@
     def extract_meta(
         self,
     ) -> tuple[
         str | None,
         list[str] | None,
         dict[str, dict[str, tp.Any]] | None,
         list[str] | None,
+        str | None,
+        str | None,
     ]:
-        pk_key, unique_together, extra_kwgs, ordering = None, None, None, None
+        pk_key, unique_together, extra_kwgs, ordering, app_label, db_table = (
+            None,
+            None,
+            None,
+            None,
+            None,
+            None,
+        )
         if hasattr(self.dataclass, "Meta"):
             meta = self.dataclass.Meta
             if hasattr(meta, "primary_key"):
                 pk_key = meta.primary_key
                 if not isinstance(pk_key, str):
                     raise RuntimeError("primary_key must be a string, please fix!")
             if hasattr(meta, "unique_together"):
@@ -29,19 +38,25 @@
                 assert isinstance(unique_together, list)
             if hasattr(meta, "extra"):
                 extra_kwgs = meta.extra
                 assert isinstance(extra_kwgs, dict)
             if hasattr(meta, "ordering"):
                 ordering = meta.ordering
                 assert isinstance(ordering, list)
+            if hasattr(meta, "app_label"):
+                app_label = meta.app_label
+                assert isinstance(app_label, str)
+            if hasattr(meta, "db_table"):
+                db_table = meta.db_table
+                assert isinstance(db_table, str)
 
-        return pk_key, unique_together, extra_kwgs, ordering
+        return pk_key, unique_together, extra_kwgs, ordering, app_label, db_table
 
     def get_identifying_parameter(self) -> set[str]:
-        pk_key, unique_together, _, _ = self.extract_meta()
+        pk_key, unique_together, *_ = self.extract_meta()
         res = set()
         if pk_key is not None:
             res.add(pk_key)
         if unique_together is not None:
             res.update(unique_together)
         return res
```

### Comparing `admem-1.9.0/source/admem/_protocols.py` & `admem-2.0.0/source/admem/_protocols.py`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/source/admem/_store_setup.py` & `admem-2.0.0/source/admem/_store_setup.py`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/source/admem/_sync_store.py` & `admem-2.0.0/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-1.9.0/source/admem.egg-info/SOURCES.txt` & `admem-2.0.0/source/admem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 source/admem/_decorator.py
 source/admem/_django_store.py
 source/admem/_inspect_dataclass.py
 source/admem/_protocols.py
 source/admem/_store_setup.py
 source/admem/_sync_store.py
 source/admem/_util.py
+source/admem/fields.py
 source/admem/py.typed
 source/admem.egg-info/PKG-INFO
 source/admem.egg-info/SOURCES.txt
 source/admem.egg-info/dependency_links.txt
 source/admem.egg-info/not-zip-safe
 source/admem.egg-info/requires.txt
 source/admem.egg-info/top_level.txt
```

