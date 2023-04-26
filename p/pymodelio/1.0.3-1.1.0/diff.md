# Comparing `tmp/pymodelio-1.0.3-py3-none-any.whl.zip` & `tmp/pymodelio-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,44 @@
-Zip file size: 26843 bytes, number of entries: 40
--rw-r--r--  2.0 unx      374 b- defN 23-Apr-18 20:44 pymodelio/__init__.py
--rw-r--r--  2.0 unx     1882 b- defN 23-Apr-18 12:32 pymodelio/attribute.py
--rw-r--r--  2.0 unx       67 b- defN 22-Sep-06 22:04 pymodelio/constants.py
--rw-r--r--  2.0 unx      845 b- defN 23-Apr-18 13:35 pymodelio/model_serializer.py
--rw-r--r--  2.0 unx      408 b- defN 23-Apr-17 16:04 pymodelio/pymodelio_cache.py
--rw-r--r--  2.0 unx    10788 b- defN 23-Apr-18 20:37 pymodelio/pymodelio_model.py
+Zip file size: 34290 bytes, number of entries: 42
+-rw-r--r--  2.0 unx      374 b- defN 23-Apr-24 19:56 pymodelio/__init__.py
+-rw-r--r--  2.0 unx     2972 b- defN 23-Apr-25 14:05 pymodelio/attribute.py
+-rw-r--r--  2.0 unx       67 b- defN 23-Apr-20 16:26 pymodelio/constants.py
+-rw-r--r--  2.0 unx     3810 b- defN 23-Apr-25 21:03 pymodelio/model_deserializer.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Apr-25 20:43 pymodelio/model_serializer.py
+-rw-r--r--  2.0 unx     5373 b- defN 23-Apr-25 20:33 pymodelio/pymodelio_meta.py
+-rw-r--r--  2.0 unx     5166 b- defN 23-Apr-25 21:06 pymodelio/pymodelio_model.py
 -rw-r--r--  2.0 unx       44 b- defN 23-Apr-18 14:09 pymodelio/shared_vars.py
 -rw-r--r--  2.0 unx       88 b- defN 23-Apr-13 15:15 pymodelio/undefined.py
--rw-r--r--  2.0 unx      399 b- defN 23-Apr-18 16:31 pymodelio/utils.py
+-rw-r--r--  2.0 unx      442 b- defN 23-Apr-25 21:19 pymodelio/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 11:20 pymodelio/decorators/__init__.py
--rw-r--r--  2.0 unx      495 b- defN 23-Apr-12 22:33 pymodelio/decorators/do_not_serialize.py
--rw-r--r--  2.0 unx      761 b- defN 23-Apr-18 14:51 pymodelio/decorators/pymodelio_cached.py
+-rw-r--r--  2.0 unx      319 b- defN 23-Apr-24 17:33 pymodelio/decorators/deserializes.py
+-rw-r--r--  2.0 unx      495 b- defN 23-Apr-20 16:26 pymodelio/decorators/do_not_serialize.py
 -rw-r--r--  2.0 unx      158 b- defN 23-Apr-17 15:04 pymodelio/exceptions/__init__.py
 -rw-r--r--  2.0 unx       58 b- defN 23-Apr-17 15:04 pymodelio/exceptions/auto_validator_creation_exception.py
 -rw-r--r--  2.0 unx       52 b- defN 22-Sep-06 22:04 pymodelio/exceptions/model_validation_exception.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 14:15 pymodelio/settings/__init__.py
--rw-r--r--  2.0 unx      398 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_setting.py
--rw-r--r--  2.0 unx     1040 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_settings.py
--rw-r--r--  2.0 unx      635 b- defN 23-Apr-18 14:19 pymodelio/validators/__init__.py
--rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/bool_validator.py
--rw-r--r--  2.0 unx      323 b- defN 22-Sep-06 22:04 pymodelio/validators/datetime_validator.py
--rw-r--r--  2.0 unx     5539 b- defN 23-Apr-18 19:48 pymodelio/validators/default_validators_builder.py
--rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/dict_validator.py
--rw-r--r--  2.0 unx      752 b- defN 23-Apr-18 20:42 pymodelio/validators/email_validator.py
--rw-r--r--  2.0 unx      463 b- defN 22-Sep-06 22:04 pymodelio/validators/float_validator.py
--rw-r--r--  2.0 unx      961 b- defN 23-Apr-18 16:31 pymodelio/validators/forward_ref_validator.py
--rw-r--r--  2.0 unx      455 b- defN 22-Sep-06 22:04 pymodelio/validators/int_validator.py
--rw-r--r--  2.0 unx     1331 b- defN 23-Apr-18 19:51 pymodelio/validators/iterable_validator.py
--rw-r--r--  2.0 unx      473 b- defN 22-Sep-06 22:04 pymodelio/validators/list_validator.py
--rw-r--r--  2.0 unx     1010 b- defN 23-Apr-15 15:13 pymodelio/validators/numeric_validator.py
--rw-r--r--  2.0 unx      471 b- defN 23-Apr-16 21:48 pymodelio/validators/set_validator.py
--rw-r--r--  2.0 unx     1341 b- defN 23-Apr-15 15:14 pymodelio/validators/string_validator.py
--rw-r--r--  2.0 unx      475 b- defN 23-Apr-16 21:48 pymodelio/validators/tuple_validator.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Apr-24 17:11 pymodelio/settings/pymodelio_setting.py
+-rw-r--r--  2.0 unx      859 b- defN 23-Apr-24 17:12 pymodelio/settings/pymodelio_settings.py
+-rw-r--r--  2.0 unx      677 b- defN 23-Apr-24 17:30 pymodelio/validators/__init__.py
+-rw-r--r--  2.0 unx      285 b- defN 23-Apr-20 16:26 pymodelio/validators/bool_validator.py
+-rw-r--r--  2.0 unx      311 b- defN 23-Apr-24 17:33 pymodelio/validators/date_validator.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Apr-20 16:26 pymodelio/validators/datetime_validator.py
+-rw-r--r--  2.0 unx     5627 b- defN 23-Apr-24 20:01 pymodelio/validators/default_validators_builder.py
+-rw-r--r--  2.0 unx      285 b- defN 23-Apr-20 16:26 pymodelio/validators/dict_validator.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Apr-24 15:28 pymodelio/validators/email_validator.py
+-rw-r--r--  2.0 unx      463 b- defN 23-Apr-20 16:26 pymodelio/validators/float_validator.py
+-rw-r--r--  2.0 unx     1009 b- defN 23-Apr-20 16:26 pymodelio/validators/forward_ref_validator.py
+-rw-r--r--  2.0 unx      455 b- defN 23-Apr-20 16:26 pymodelio/validators/int_validator.py
+-rw-r--r--  2.0 unx     1333 b- defN 23-Apr-24 15:28 pymodelio/validators/iterable_validator.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Apr-20 16:26 pymodelio/validators/list_validator.py
+-rw-r--r--  2.0 unx     1012 b- defN 23-Apr-24 15:28 pymodelio/validators/numeric_validator.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Apr-20 16:26 pymodelio/validators/set_validator.py
+-rw-r--r--  2.0 unx     1345 b- defN 23-Apr-24 15:28 pymodelio/validators/string_validator.py
+-rw-r--r--  2.0 unx      475 b- defN 23-Apr-20 16:26 pymodelio/validators/tuple_validator.py
 -rw-r--r--  2.0 unx      274 b- defN 22-Sep-06 22:04 pymodelio/validators/validation_patterns.py
--rw-r--r--  2.0 unx     1372 b- defN 23-Apr-18 19:50 pymodelio/validators/validator.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    24491 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3608 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/RECORD
-40 files, 63573 bytes uncompressed, 20941 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1434 b- defN 23-Apr-24 15:28 pymodelio/validators/validator.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-25 21:27 pymodelio-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    49493 b- defN 23-Apr-25 21:27 pymodelio-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 21:27 pymodelio-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-25 21:27 pymodelio-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3785 b- defN 23-Apr-25 21:27 pymodelio-1.1.0.dist-info/RECORD
+42 files, 92721 bytes uncompressed, 28108 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,18 +3,21 @@
 
 Filename: pymodelio/attribute.py
 Comment: 
 
 Filename: pymodelio/constants.py
 Comment: 
 
+Filename: pymodelio/model_deserializer.py
+Comment: 
+
 Filename: pymodelio/model_serializer.py
 Comment: 
 
-Filename: pymodelio/pymodelio_cache.py
+Filename: pymodelio/pymodelio_meta.py
 Comment: 
 
 Filename: pymodelio/pymodelio_model.py
 Comment: 
 
 Filename: pymodelio/shared_vars.py
 Comment: 
@@ -24,18 +27,18 @@
 
 Filename: pymodelio/utils.py
 Comment: 
 
 Filename: pymodelio/decorators/__init__.py
 Comment: 
 
-Filename: pymodelio/decorators/do_not_serialize.py
+Filename: pymodelio/decorators/deserializes.py
 Comment: 
 
-Filename: pymodelio/decorators/pymodelio_cached.py
+Filename: pymodelio/decorators/do_not_serialize.py
 Comment: 
 
 Filename: pymodelio/exceptions/__init__.py
 Comment: 
 
 Filename: pymodelio/exceptions/auto_validator_creation_exception.py
 Comment: 
@@ -54,14 +57,17 @@
 
 Filename: pymodelio/validators/__init__.py
 Comment: 
 
 Filename: pymodelio/validators/bool_validator.py
 Comment: 
 
+Filename: pymodelio/validators/date_validator.py
+Comment: 
+
 Filename: pymodelio/validators/datetime_validator.py
 Comment: 
 
 Filename: pymodelio/validators/default_validators_builder.py
 Comment: 
 
 Filename: pymodelio/validators/dict_validator.py
@@ -99,23 +105,23 @@
 
 Filename: pymodelio/validators/validation_patterns.py
 Comment: 
 
 Filename: pymodelio/validators/validator.py
 Comment: 
 
-Filename: pymodelio-1.0.3.dist-info/LICENSE.txt
+Filename: pymodelio-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pymodelio-1.0.3.dist-info/METADATA
+Filename: pymodelio-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pymodelio-1.0.3.dist-info/WHEEL
+Filename: pymodelio-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pymodelio-1.0.3.dist-info/top_level.txt
+Filename: pymodelio-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pymodelio-1.0.3.dist-info/RECORD
+Filename: pymodelio-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymodelio/__init__.py

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = '1.0.3'
+__version__ = '1.1.0'
 
 # constants
 from .constants import UNDEFINED
 
 # Settings
 from .settings.pymodelio_setting import PymodelioSetting
 from .settings.pymodelio_settings import PymodelioSettings
```

## pymodelio/attribute.py

```diff
@@ -1,24 +1,39 @@
-from typing import Callable, Optional, Any, TypeVar, Union
+from typing import Callable, Optional, Any, TypeVar, Union, Tuple, Iterable
 
 from pymodelio import UNDEFINED, PymodelioSettings, PymodelioSetting
 from pymodelio.undefined import Undefined
 from pymodelio.validators.default_validators_builder import DefaultValidatorsBuilder
 from pymodelio.validators.validator import Validator
 
 T = TypeVar('T')
 
 
 class PymodelioAttr:
+    __slots__ = (
+        '_attr_type', '_initable', '_default_factory', '_init_aliases', '_validator', '_compare'
+    )
+
     def __init__(self, attr_type: T, validator: Optional[Validator] = UNDEFINED, initable: bool = True,
-                 default_factory: Callable = None) -> None:
+                 init_alias: Optional[str] = None, init_aliases: Optional[Iterable[str]] = None,
+                 default_factory: Callable = None, compare: bool = True) -> None:
         self._attr_type = attr_type
-        self._initable = initable
-        self._default_factory = default_factory or (lambda: None)
+        self._init_attr_aliases(init_alias, init_aliases)
+        self._initable = initable or len(self._init_aliases) > 0
+        self._default_factory = default_factory if default_factory is not None else (lambda: None)
         self._init_validator(validator)
+        self._compare = compare
+
+    def _init_attr_aliases(self, init_alias: Optional[str], init_aliases: Optional[Iterable[str]]) -> None:
+        if init_aliases is not None:
+            self._init_aliases = tuple(init_aliases)
+        elif init_alias is not None:
+            self._init_aliases = (init_alias,)
+        else:
+            self._init_aliases = tuple()
 
     def _init_validator(self, validator: Union[Validator, None, Undefined]) -> None:
         if validator == UNDEFINED:
             if PymodelioSettings.get(PymodelioSetting.USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED):
                 self._validator = DefaultValidatorsBuilder.build(self.attr_type)
             else:
                 self._validator = None
@@ -41,12 +56,21 @@
     def default_factory(self) -> Callable:
         return self._default_factory
 
     @property
     def attr_type(self) -> T:
         return self._attr_type
 
+    @property
+    def init_aliases(self) -> Tuple[str]:
+        return self._init_aliases
+
+    @property
+    def compare(self) -> bool:
+        return self._compare
+
 
-def Attr(attr_type: T, validator: Optional[Validator] = UNDEFINED, initable: bool = True,
-         default_factory: Callable = None) -> T:
-    return PymodelioAttr(attr_type=attr_type, validator=validator, initable=initable,
-                         default_factory=default_factory)
+def Attr(attr_type: T, /, *, validator: Optional[Validator] = UNDEFINED, initable: bool = True,
+         init_alias: Optional[str] = None, init_aliases: Iterable[str] = None, default_factory: Callable = None,
+         compare: bool = True) -> T:
+    return PymodelioAttr(attr_type=attr_type, validator=validator, initable=initable, init_alias=init_alias,
+                         init_aliases=init_aliases, default_factory=default_factory, compare=compare)
```

## pymodelio/model_serializer.py

```diff
@@ -1,26 +1,24 @@
-from datetime import datetime
+from datetime import datetime, date
 from typing import Any
 
 
 class ModelSerializer:
 
     @classmethod
     def serialize(cls, value: Any) -> Any:
-        if cls._is_model(value):
+        if getattr(value, '__is_pymodelio_model__', False):
             return cls._serialize_model(value)
         if isinstance(value, (list, tuple, set)):
             return [cls.serialize(x) for x in value]
         if isinstance(value, datetime):
             return value.isoformat()
+        if isinstance(value, date):
+            return value.strftime('%Y-%m-%d')
         return value
 
     @classmethod
     def _serialize_model(cls, model: Any) -> dict:
         serialized = {}
         for attr_name, attr_value in model._get_serializable_attrs():
             serialized[attr_name] = cls.serialize(attr_value)
         return serialized
-
-    @classmethod
-    def _is_model(cls, attr_value: Any) -> bool:
-        return hasattr(attr_value, '_is_pymodelio_model') and getattr(attr_value, '_is_pymodelio_model')()
```

## pymodelio/pymodelio_model.py

```diff
@@ -1,244 +1,125 @@
-from datetime import datetime
-from typing import List, Any, Optional, Tuple
+from datetime import datetime, date
+from typing import List, Any, Tuple, TypeVar, Callable, Dict, Type
 
-from pymodelio import PymodelioSettings, PymodelioSetting, shared_vars
 from pymodelio.attribute import PymodelioAttr
 from pymodelio.constants import UNDEFINED
-from pymodelio.decorators.pymodelio_cached import pymodelio_cached
+from pymodelio.model_deserializer import ModelDeserializer
 from pymodelio.model_serializer import ModelSerializer
-from pymodelio.utils import to_datetime
+from pymodelio.pymodelio_meta import PymodelioMeta
 
+T = TypeVar('T')
 
-class PymodelioModel:
-    __GENERIC_ALIASES = {'_GenericAlias', '_UnionGenericAlias'}
-    __ANNOTATIONS_KEY__ = '__annotations__'
 
-    def __init__(self, *args, auto_validate: bool = True, **kwargs) -> None:
-        shared_vars.model_globals[self.__class__.__name__] = self.__class__
-        self._model_attrs = self.__get_model_attrs()
-        if not kwargs.get('from_dict', False):
-            self.__constructor__(*args, auto_validate=auto_validate, **kwargs)
+class PymodelioModel(metaclass=PymodelioMeta):
+    # Only for intellisense
+    __is_pymodelio_model__ = True
+    __inner_pymodelio_model__ = None
+    __is_pymodelio_inner_model__ = False
+    __model_attrs__: Tuple[str, PymodelioAttr] = tuple()
+    __pymodelio_parent__ = None
+    __serializable_attrs__ = []
+    __exposed_attrs__ = {}
+    __protected_attrs__ = set()
+    __private_attrs__ = set()
+    __deserializers__: Dict[str, Callable] = dict()
 
-    def __constructor__(self, *args, auto_validate: bool = True, **kwargs) -> None:
-        self.__before_init__(*args, **kwargs)
+    def __init__(self, *args, auto_validate: bool = True, **kwargs) -> None:
+        args, kwargs = self.__before_init__(*args, auto_validate=auto_validate, **kwargs)
         self.__set_attributes(kwargs)
         self.__before_validate__()
         if auto_validate:
             self.validate()
         self.__once_validated__()
 
-    @classmethod
-    def _is_pymodelio_model(cls) -> bool:
-        return True
-
     def __set_attributes(self, kwargs: dict) -> None:
-        for attr_name in self._model_attrs:
-            model_attr = self._model_attrs[attr_name]
-            if not self.__is_initable(attr_name, model_attr):
-                if self.__get_exposed_attr_name(attr_name) in kwargs:
-                    raise NameError('%s attribute is not initable for class %s' % (attr_name, self.__class__.__name__))
-                else:
-                    attr_value = model_attr.default_factory()
-            else:
-                exposed_attr_name = self.__get_exposed_attr_name(attr_name)
-                attr_value = kwargs.get(exposed_attr_name, model_attr.default_factory())
-                if attr_value == UNDEFINED:
-                    attr_value = model_attr.default_factory()
+        for attr_name, model_attr in self.__model_attrs__:
+            exposed_attr_names = self.__get_exposed_attr_names(attr_name)
+            attr_value = UNDEFINED
+            for exposed_attr_name in exposed_attr_names:
+                if exposed_attr_name in kwargs:
+                    if not model_attr.initable:
+                        raise NameError(
+                            '%s attribute is not initable for class %s' % (attr_name, self.__class__.__name__))
+                    attr_value = kwargs[exposed_attr_name]
+                    break
+            if attr_value == UNDEFINED:
+                attr_value = model_attr.default_factory()
             setattr(self, attr_name, attr_value)
 
-    def __before_init__(self, *args, **kwargs) -> None:
-        pass
+    def __before_init__(self, *args, **kwargs) -> Tuple[Tuple[Any], Dict[Any, Any]]:
+        return args, kwargs
 
     def __before_validate__(self) -> None:
-        pass
+        return
 
     def __once_validated__(self) -> None:
-        pass
+        return
 
-    @pymodelio_cached
-    def __get_annotations(self) -> dict:
-        annotations = self.__annotations__ if hasattr(self, self.__ANNOTATIONS_KEY__) else {}
-        for parent in self.__class__.__bases__:
-            if hasattr(parent, self.__ANNOTATIONS_KEY__):
-                annotations = {**annotations, **parent.__annotations__}
-        return annotations
-
-    @pymodelio_cached
-    def __get_model_attrs(self) -> dict:
-        validated_attrs = {}
-        annotations = self.__get_annotations()
-        for k in annotations:
-            v = annotations[k]
-            if isinstance(v, PymodelioAttr):
-                validated_attrs[k] = v
-        return validated_attrs
-
-    @classmethod
-    def __generate_private_attr_prefix(cls, cls_type: type) -> str:
-        return '_%s__' % cls_type.__name__
-
-    @pymodelio_cached
-    def __get_parent_private_attr_prefixes(self) -> List[str]:
-        # Iterate all the parents
-        prefixes = []
-        for cls in self.__class__.__bases__:
-            prefixes.append(self.__generate_private_attr_prefix(cls))
-        return prefixes
-
-    @pymodelio_cached
-    def __get_private_attr_prefixes(self) -> List[str]:
-        return ['__', self.__generate_private_attr_prefix(self.__class__)] + self.__get_parent_private_attr_prefixes()
-
-    @pymodelio_cached
-    def __get_exposed_attr_name(self, attr_name: str) -> str:
-        # Private attributes
-        private_attr_prefix = self.__get_private_attr_prefix(attr_name)
-        if private_attr_prefix is not None:
-            exposed_attr_name = attr_name[len(private_attr_prefix):]
-            if exposed_attr_name.endswith('__'):
-                exposed_attr_name = exposed_attr_name[:-2]
-            return exposed_attr_name
-        # Protected attributes
-        if self.__is_protected_attr_name(attr_name, private_checked=True):
-            exposed_attr_name = attr_name[1:]
-            if exposed_attr_name.endswith('_'):
-                exposed_attr_name = exposed_attr_name[:-1]
-            return exposed_attr_name
-        # Public attributes
-        return attr_name
-
-    def __is_protected_attr_name(self, attr_name: str, private_checked: bool = False) -> bool:
-        if private_checked:
-            is_private = False
-        else:
-            is_private = self.__is_private_attr_name(attr_name)
-        return (not is_private) and attr_name.startswith('_')
-
-    def __is_private_attr_name(self, attr_name: str) -> bool:
-        return self.__get_private_attr_prefix(attr_name) is not None
-
-    def __get_private_attr_prefix(self, attr_name: str) -> Optional[str]:
-        private_attr_prefixes = self.__get_private_attr_prefixes()
-        for private_attr_prefix in private_attr_prefixes:
-            if attr_name.startswith(private_attr_prefix):
-                return private_attr_prefix
-        return None
+    def __get_exposed_attr_names(self, attr_name: str) -> Tuple[str]:
+        return self.__exposed_attrs__.get(attr_name)
 
     def __is_initable(self, attr_name: str, model_attr: PymodelioAttr) -> bool:
-        if not model_attr.initable:
-            return False
-        if (not PymodelioSettings.get(PymodelioSetting.INIT_PROTECTED_ATTRS_BY_DEFAULT)) \
-                and self.__is_protected_attr_name(attr_name):
-            return False
-        if (not PymodelioSettings.get(PymodelioSetting.INIT_PRIVATE_ATTRS_BY_DEFAULT)) \
-                and self.__is_private_attr_name(attr_name):
-            return False
-        return True
+        return model_attr.initable and \
+            attr_name not in self.__protected_attrs__ and \
+            attr_name in self.__private_attrs__
 
     def validate(self, path: str = None) -> None:
         """
         It must raise ModelValidationException in case of an invalid attribute
         """
-        # model_attrs = self._get_model_attrs()
-        for attr_name in self._model_attrs:
-            pymodelio_attr = self._model_attrs[attr_name]
+        for attr_name, model_attr in self.__model_attrs__:
             attr_value = getattr(self, attr_name)
-            exposed_attr_name = self.__get_exposed_attr_name(attr_name)
-            parent_path = path or self.__class__.__name__
-            attr_path = '%s.%s' % (parent_path, exposed_attr_name)
-            self._when_validating_attr(attr_name, exposed_attr_name, attr_value, attr_path, parent_path,
-                                       pymodelio_attr)
-            pymodelio_attr.validate(attr_value, path=attr_path)
-
-    def _when_validating_attr(self, internal_attr_name: str, exposed_attr_name: str, attr_value: Any, attr_path: str,
-                              parent_path: str, attr: PymodelioAttr) -> None:
-        pass
+            parent_path = path if path is not None else self.__class__.__name__
+            attr_path = '%s.%s' % (parent_path, attr_name)
+            model_attr.validate(attr_value, path=attr_path)
+            self.__when_validating_an_attr__(attr_name, attr_value, attr_path, parent_path, model_attr)
+
+    def __when_validating_an_attr__(self, attr_name: str, attr_value: Any, attr_path: str,
+                                    parent_path: str, attr: PymodelioAttr) -> None:
+        return
 
     @classmethod
-    def from_dict(cls, data: dict, auto_validate: bool = True) -> Any:
-        instance = cls(from_dict=True)
-        attrs = {}
-        # model_attrs = instance._get_model_attrs()
-        for attr_name in instance._model_attrs:
-            model_attr = instance._model_attrs[attr_name]
-            exposed_attr_name = instance.__get_exposed_attr_name(attr_name)
-            if model_attr.initable:
-                attrs[exposed_attr_name] = cls.__map_attribute(data, exposed_attr_name, model_attr)
-        return cls(**attrs, auto_validate=auto_validate)
-
-    @classmethod
-    def __map_attribute(cls, data: dict, exposed_attr_name: str, model_attr: PymodelioAttr) -> Any:  # noqa: C901
-        attr_value = data.get(exposed_attr_name, model_attr.default_factory())
-        if attr_value == UNDEFINED:
-            return model_attr.default_factory()
-        # Parse dates
-        if model_attr.attr_type == datetime and isinstance(attr_value, str):
-            try:
-                return to_datetime(attr_value)
-            except Exception:
-                return attr_value
-        if hasattr(model_attr.attr_type, '_is_pymodelio_model') and model_attr.attr_type._is_pymodelio_model() and \
-                isinstance(attr_value, dict):
-            return model_attr.attr_type.from_dict(attr_value, auto_validate=False)
-        if isinstance(attr_value, list):
-            if model_attr.attr_type == list or len(model_attr.attr_type.__args__) == 0:
-                list_type = None
-            else:
-                list_type = model_attr.attr_type.__args__[0]
-            # If the type of the list is not specified. For instance -> a: List
-            if list_type is None:
-                return attr_value
-            # If the type is more than one. For instance -> a: List[Union[int, float]]
-            if list_type.__class__.__name__ in cls.__GENERIC_ALIASES:
-                print('WARNING: pymodelio automatic deserialization does not handle multi typed lists of models')
-                return attr_value
-            # If the type is not a model
-            if not hasattr(list_type, '_is_pymodelio_model') or not list_type._is_pymodelio_model():
-                return attr_value
-            # At this point, the list is a list of models
-            return [list_type.from_dict(x, auto_validate=False) for x in attr_value]
-        return attr_value
+    def from_dict(cls: Type[T], data: dict, auto_validate: bool = True) -> T:
+        return ModelDeserializer.deserialize(cls, data, auto_validate)
 
     def to_dict(self) -> dict:
         return ModelSerializer.serialize(self)
 
     def _get_serializable_attrs(self) -> List[Tuple[str, Any]]:
         attrs = []
-        for attr_name in self.__get_serializable_attr_names():
+        for attr_name in self.__serializable_attrs__:
             attr_value = getattr(self, attr_name)
             # If it is a function, we ignore it
             if not callable(attr_value):
                 attrs.append((attr_name, attr_value))
         return attrs
 
-    @pymodelio_cached
-    def __get_serializable_attr_names(self) -> List[str]:
-        return [attr_name for attr_name in dir(self) if
-                not attr_name.startswith('_') and not self.__is_marked_as_do_not_serialize(attr_name)]
-
-    def __is_marked_as_do_not_serialize(self, attr_name: str) -> bool:
-        class_qualname = self.__class__.__qualname__
-        if class_qualname not in shared_vars.to_do_not_serialize:
-            return False
-        return attr_name in shared_vars.to_do_not_serialize[class_qualname]
-
     def __repr__(self) -> str:
         formatted_fields = []
-
         for attr_name, attr_value in self._get_serializable_attrs():
             formatted_attr_value = self.__format_attr_value(attr_value)
             formatted_fields.append('%s=%s' % (attr_name, formatted_attr_value))
-        return '%s(%s)' % (self.__class__.__name__, ', '.join(formatted_fields))
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(sorted(formatted_fields)))
 
     @classmethod
     def __format_attr_value(cls, value: Any) -> Any:
         if isinstance(value, str):
             return "'%s'" % value
         if isinstance(value, PymodelioModel):
             return str(value)
         if isinstance(value, datetime):
             return "datetime(%s, %s, %s, %s, %s, %s, %s, %s)" % (
                 value.year, value.month, value.day, value.hour, value.minute, value.second, value.microsecond,
                 value.tzinfo
             )
+        if isinstance(value, date):
+            return "date(%s, %s, %s)" % (value.year, value.month, value.day)
         return value
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, self.__class__):
+            return False
+        for attr_name, pymodelio_attr in self.__model_attrs__:
+            if pymodelio_attr.compare and getattr(self, attr_name) != getattr(other, attr_name):
+                return False
+        return True
```

## pymodelio/utils.py

```diff
@@ -1,16 +1,17 @@
-from datetime import timezone, datetime
+from datetime import timezone, datetime, date
 
 import ciso8601
 
 from pymodelio import PymodelioSetting, PymodelioSettings
 
 
-def default_is_pymodelio_model() -> bool:
-    return False
+def to_date(str_date: str) -> date:
+    dt = to_datetime(str_date)
+    return dt.date()
 
 
-def to_datetime(str_date: str) -> datetime:
-    dt = ciso8601.parse_datetime(str_date)
+def to_datetime(str_datetime: str) -> datetime:
+    dt = ciso8601.parse_datetime(str_datetime)
     if PymodelioSettings.get(PymodelioSetting.AUTO_PARSE_DATES_AS_UTC):
         return dt.replace(tzinfo=timezone.utc)
     return dt
```

## pymodelio/settings/pymodelio_setting.py

```diff
@@ -1,9 +1,6 @@
 from enum import Enum
 
 
 class PymodelioSetting(Enum):
-    INIT_PROTECTED_ATTRS_BY_DEFAULT = 'INIT_PROTECTED_ATTRS_BY_DEFAULT'
-    INIT_PRIVATE_ATTRS_BY_DEFAULT = 'INIT_PRIVATE_ATTRS_BY_DEFAULT'
-    USE_CACHE_OPTIMIZATIONS = 'USE_CACHE_OPTIMIZATIONS'
     AUTO_PARSE_DATES_AS_UTC = 'AUTO_PARSE_DATES_AS_UTC'
     USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED = 'USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED'
```

## pymodelio/settings/pymodelio_settings.py

```diff
@@ -2,18 +2,15 @@
 from typing import Any
 
 from pymodelio.settings.pymodelio_setting import PymodelioSetting
 
 
 class PymodelioSettings:
     __initial_settings = {
-        PymodelioSetting.INIT_PROTECTED_ATTRS_BY_DEFAULT: True,
-        PymodelioSetting.INIT_PRIVATE_ATTRS_BY_DEFAULT: True,
-        PymodelioSetting.USE_CACHE_OPTIMIZATIONS: True,
-        PymodelioSetting.AUTO_PARSE_DATES_AS_UTC: True,
+        PymodelioSetting.AUTO_PARSE_DATES_AS_UTC: False,
         PymodelioSetting.USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED: True
     }
 
     __settings = deepcopy(__initial_settings)
 
     @classmethod
     def set(cls, setting: PymodelioSetting, value: Any) -> None:
```

## pymodelio/validators/__init__.py

```diff
@@ -1,10 +1,11 @@
 # flake8: noqa
 from .validator import Validator
 from .bool_validator import BoolValidator
+from .date_validator import DateValidator
 from .datetime_validator import DatetimeValidator
 from .dict_validator import DictValidator
 from .string_validator import StringValidator
 from .email_validator import EmailValidator
 from .numeric_validator import NumericValidator
 from .float_validator import FloatValidator
 from .int_validator import IntValidator
```

## pymodelio/validators/default_validators_builder.py

```diff
@@ -1,72 +1,64 @@
 import typing
-from dataclasses import dataclass, field
-from datetime import datetime
+from collections import namedtuple
+from datetime import datetime, date
 from typing import Optional, _SpecialForm
 
 from pymodelio.exceptions import AutoValidatorCreationException
 from pymodelio.validators import Validator, StringValidator, FloatValidator, IntValidator, BoolValidator, \
     DictValidator, ListValidator, DatetimeValidator, SetValidator, TupleValidator
+from pymodelio.validators.date_validator import DateValidator
 from pymodelio.validators.forward_ref_validator import ForwardRefValidator
 
+# We use namedtuple for performance
+_DestructuredType = namedtuple('_DestructuredType', 'outer outer_nullable inners')
 
-def _generate_validators_mapping() -> dict:
-    return {
+
+class DefaultValidatorsBuilder:
+    _VALIDATORS_MAPPING = {
         str: StringValidator,
         bool: BoolValidator,
         int: IntValidator,
         float: FloatValidator,
         dict: DictValidator,
         list: ListValidator,
         set: SetValidator,
         tuple: TupleValidator,
+        date: DateValidator,
         datetime: DatetimeValidator,
         typing.Dict: DictValidator,
         typing.List: ListValidator,
         typing.Tuple: TupleValidator,
         typing.Set: SetValidator,
         typing.Any: Validator
     }
 
-
-@dataclass
-class _DestructuredType:
-    outer: typing.Union[type, _SpecialForm]
-    outer_nullable: bool = field(default_factory=lambda: False)
-    inners: typing.List['_DestructuredType'] = field(default_factory=list)
-
-    def is_plain(self) -> bool:
-        return len(self.inners) == 0
-
-
-class DefaultValidatorsBuilder:
-    _VALIDATORS_MAPPING = _generate_validators_mapping()
-
     @classmethod
     def build(cls, attr_type: type) -> Optional[Validator]:
         destructured = cls._destructurate(attr_type)
         return cls._instantiate_from_destructured(destructured)
 
     @classmethod
     def _destructurate(cls, attr_type: type) -> _DestructuredType:  # noqa: C901
         if attr_type in cls._VALIDATORS_MAPPING or (
-                hasattr(attr_type, '_is_pymodelio_model') and attr_type._is_pymodelio_model()):
-            return _DestructuredType(outer=attr_type)
+                hasattr(attr_type, '__is_pymodelio_model__') and attr_type.__is_pymodelio_model__):
+            return _DestructuredType(outer=attr_type, outer_nullable=False, inners=[])
         if attr_type == typing.Any:
-            return _DestructuredType(outer=typing.Any)
+            return _DestructuredType(outer=typing.Any, outer_nullable=False, inners=[])
         # typing.ForwardRef
         if isinstance(attr_type, typing.ForwardRef):
-            return _DestructuredType(outer=typing.ForwardRef, inners=[attr_type])
+            return _DestructuredType(outer=typing.ForwardRef, outer_nullable=False, inners=[attr_type])
         if isinstance(attr_type, str):
-            return _DestructuredType(outer=typing.ForwardRef, inners=[typing.ForwardRef(attr_type)])
+            return _DestructuredType(outer=typing.ForwardRef, outer_nullable=False,
+                                     inners=[typing.ForwardRef(attr_type)])
         # other typings
         if attr_type.__module__ == 'typing' and hasattr(attr_type, '__reduce__'):
             reduced = attr_type.__reduce__()[1]
             if len(reduced) == 1:
-                return _DestructuredType(outer=reduced[0])
+                return _DestructuredType(outer=reduced[0], outer_nullable=False, inners=[])
             _type, args = reduced
             if _type == typing.Union:
                 # Optional
                 if len(args) == 2 and type(None) in args:
                     return _DestructuredType(outer=typing.Optional, outer_nullable=True, inners=[
                         cls._destructurate(x) for x in args if x != type(None)  # noqa: E721
                     ])
@@ -79,20 +71,20 @@
                             is_nullable = True
                         else:
                             inners.append(cls._destructurate(x))
                     return _DestructuredType(outer=typing.Union, outer_nullable=is_nullable, inners=inners)
             if _type in (typing.List, typing.Tuple, typing.Set):
                 return _DestructuredType(outer=_type, outer_nullable=True, inners=[cls._destructurate(args)])
             if _type == typing.Dict:
-                return _DestructuredType(outer=dict)
-        return _DestructuredType(outer=attr_type)
+                return _DestructuredType(outer=dict, outer_nullable=False, inners=[])
+        return _DestructuredType(outer=attr_type, outer_nullable=False, inners=[])
 
     @classmethod
     def _instantiate_from_destructured(cls, destructured: _DestructuredType, nullable: bool = False) -> Validator:
-        if destructured.is_plain():
+        if len(destructured.inners) == 0:
             return cls._instantiate_validator(destructured.outer, nullable)
         if destructured.outer == typing.ForwardRef:
             return ForwardRefValidator(ref=destructured.inners[0], nullable=nullable)
         if destructured.outer == typing.Optional:
             # TODO: Define limitations
             return cls._instantiate_from_destructured(destructured.inners[0], nullable=True)
         if destructured.outer == typing.Union:
```

## pymodelio/validators/email_validator.py

```diff
@@ -10,10 +10,10 @@
     def __init__(self, nullable: bool = False, message: Optional[str] = None) -> None:
         super().__init__(nullable=nullable, message=message)
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
-        # Is override for adding a custom message and validating the string as lowercase
+        # Is overriden for adding a custom message and validating the string as lowercase
         if re.compile(EMAIL_VALIDATION_PATTERN).match(value.lower()) is None:
-            self.raise_validation_error(path, 'is not a valid email address')
+            self._raise_validation_error(path, 'is not a valid email address')
```

## pymodelio/validators/forward_ref_validator.py

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Optional, ForwardRef
 
 from pymodelio import shared_vars
 from pymodelio.validators import Validator
 
 
 class ForwardRefValidator(Validator):
+    __slots__ = Validator.__slots__ + ('_ref',)
 
     def __init__(self, ref: ForwardRef, nullable: bool = False, message: Optional[str] = None) -> None:
         self._ref = ref
         super().__init__(expected_type=ForwardRef, nullable=nullable, message=message)
 
     def validate(self, value: Any, path: str = None) -> None:
         if self._expected_types == (ForwardRef,):
```

## pymodelio/validators/iterable_validator.py

```diff
@@ -12,17 +12,17 @@
         self.allow_empty = allow_empty
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if len(value) == 0 and not self.allow_empty:
-            self.raise_validation_error(path, 'must not be empty')
+            self._raise_validation_error(path, 'must not be empty')
         for i, x in enumerate(value):
             sub_path = '%s[%s]' % (path, i)
             if self.elements_type != (None,) and not isinstance(x, self.elements_type):
-                self.raise_validation_error(
+                self._raise_validation_error(
                     sub_path, 'is not instance of %s' % (' or '.join([t.__name__ for t in self.elements_type]))
                 )
             # If it is a model
             if hasattr(x, 'validate'):
                 x.validate(sub_path)
```

## pymodelio/validators/numeric_validator.py

```diff
@@ -14,10 +14,10 @@
         self.max_value = max_value
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if self.min_value is not None and value < self.min_value:
-            self.raise_validation_error(path, 'is less than %s' % self.min_value)
+            self._raise_validation_error(path, 'is less than %s' % self.min_value)
         if self.max_value is not None and value > self.max_value:
-            self.raise_validation_error(path, 'is greater than %s' % self.max_value)
+            self._raise_validation_error(path, 'is greater than %s' % self.max_value)
```

## pymodelio/validators/string_validator.py

```diff
@@ -15,14 +15,14 @@
         self.regex = regex
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if self.min_len is not None and len(value) < self.min_len:
-            self.raise_validation_error(path, 'is shorter than %s' % self.min_len)
+            self._raise_validation_error(path, 'is shorter than %s' % self.min_len)
         if self.max_len is not None and len(value) > self.max_len:
-            self.raise_validation_error(path, 'is longer than %s' % self.max_len)
+            self._raise_validation_error(path, 'is longer than %s' % self.max_len)
         if self.fixed_len is not None and len(value) != self.fixed_len:
-            self.raise_validation_error(path, 'length is different than %s' % self.fixed_len)
+            self._raise_validation_error(path, 'length is different than %s' % self.fixed_len)
         if self.regex is not None and re.compile(self.regex).match(value) is None:
-            self.raise_validation_error(path, 'does not match configured regex')
+            self._raise_validation_error(path, 'does not match configured regex')
```

## pymodelio/validators/validator.py

```diff
@@ -1,33 +1,34 @@
 from typing import Any, Union, List, Optional
 
 from pymodelio.exceptions.model_validation_exception import ModelValidationException
 
 
 class Validator:
+    __slots__ = ('nullable', 'message', '_expected_types')
 
     def __init__(self, expected_type: Union[type, List[type]] = None, nullable: bool = False,
                  message: Optional[str] = None) -> None:
         self.nullable = nullable
         self.message = message
         if expected_type is None:
             self._expected_types = None
         else:
             self._expected_types = tuple(expected_type) if isinstance(expected_type, (list, tuple, set)) else (
                 expected_type,)
 
     def validate(self, value: Any, path: str = None) -> None:
         if value is None:
             if not self.nullable:
-                self.raise_validation_error(path, 'must not be None')
+                self._raise_validation_error(path, 'must not be None')
             return
         if self._expected_types is not None and not isinstance(value, self._expected_types):
-            self.raise_validation_error(
+            self._raise_validation_error(
                 path, 'is not instance of %s' % (' or '.join([t.__name__ for t in self._expected_types]))
             )
         # If it is a model
         if hasattr(value, 'validate'):
             value.validate(path)
 
-    def raise_validation_error(self, path: str, message: str) -> None:
+    def _raise_validation_error(self, path: str, message: str) -> None:
         _message = message if self.message is None else self.message
         raise ModelValidationException('%s %s' % (path, _message))
```

## Comparing `pymodelio-1.0.3.dist-info/LICENSE.txt` & `pymodelio-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pymodelio-1.0.3.dist-info/RECORD` & `pymodelio-1.1.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-pymodelio/__init__.py,sha256=SRItuevLvz-A8BUpZdujEDmTXPJ5fb6Z8rNdqQQrl7k,374
-pymodelio/attribute.py,sha256=W9z_mZg6892XqqQ_t1fvwHJG-cJ7UyrGNUHdvcSwlQU,1882
+pymodelio/__init__.py,sha256=87tduTPfRohUqeu5-_vqFlDysAgLgX7ArIg6BhMYJcI,374
+pymodelio/attribute.py,sha256=nQuVe-6ZfD11IAtl3WxTvb46RYmv_jdbgriBDFM1MT4,2972
 pymodelio/constants.py,sha256=qDMrr5LAO8nm9yVfWJbCJ6MV9WenSypNm4GBVopNgwY,67
-pymodelio/model_serializer.py,sha256=S3Ywak4tdorwSYsI4mvUMRXlA7d8H0_fC6wvHOl5YU0,845
-pymodelio/pymodelio_cache.py,sha256=BQ9tWj8oIcTBIqlwI_-XR3Nm4DAadLy6OVZSgmr-W84,408
-pymodelio/pymodelio_model.py,sha256=v9WK8rkZIaxoCJp0P7zyXIjUGjyilKEL4pHcQ5UMjdA,10788
+pymodelio/model_deserializer.py,sha256=rRwgoQEPNgnGd6n0ma_1bQVxX8yRmwbc2moxt2asOg0,3810
+pymodelio/model_serializer.py,sha256=PppEt0BpQSKkRFq0sJ7xqhIN6VaWfkvnmIJZRja4phI,786
+pymodelio/pymodelio_meta.py,sha256=wNFtVCMxNOFeUbYC2PKEnJVaT3J1MzwMWrjCIofgjqM,5373
+pymodelio/pymodelio_model.py,sha256=hbjJ6qruztbFMVQCPR8RudfNv4L_amnYjZxy-HctB4Y,5166
 pymodelio/shared_vars.py,sha256=grXRCAaGUhOG1-tENkcZgJEndtZJSQvF_QU7qbRjycc,44
 pymodelio/undefined.py,sha256=dvmNY7_3EmfidEGomJNzWXkOdbg8VfJski1t05mniH0,88
-pymodelio/utils.py,sha256=tjtv8aFhsqu3XKorq6UtJDx541L4stPJOgGla6tINWU,399
+pymodelio/utils.py,sha256=jJvU9X_d_ZA5pCxnADABKmAyWNX30DjWxhllg58e0Ls,442
 pymodelio/decorators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pymodelio/decorators/deserializes.py,sha256=WzyQJwLSu9tJBrM0RL-1vLlEGAE-gsmtK934i8Rf0IM,319
 pymodelio/decorators/do_not_serialize.py,sha256=4XoufTgS3g0HYSPVc-8_oYKMMf3d1XYIJgF5Bz3-kp8,495
-pymodelio/decorators/pymodelio_cached.py,sha256=C2tz_A1omw_meDO7QZmZLnj8V_yYbkQd9FD3VRQgW_A,761
 pymodelio/exceptions/__init__.py,sha256=xufuLIo1wPqOVDrYisHdUOl51-GPe_bWKesAb89FFAo,158
 pymodelio/exceptions/auto_validator_creation_exception.py,sha256=gAlViH6kPTq8hWE6uCGHmImhXM16eAmXUGDpy1Z0jMk,58
 pymodelio/exceptions/model_validation_exception.py,sha256=JfxWxtfdT3Y6ruigYs8X8usBIJC4dwSte3r7oPGUxb8,52
 pymodelio/settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pymodelio/settings/pymodelio_setting.py,sha256=iaG5QqJHLqWJcbV2KPVOnu40qU8pmrRJ2pOGTpn6_p0,398
-pymodelio/settings/pymodelio_settings.py,sha256=4BqMNG9Rx9PNRk1aOV2G4aWKyHH5eVPtFUEfblKjXXE,1040
-pymodelio/validators/__init__.py,sha256=D2ACgRBgX97IRmKurhDZNegxtW_6ZYnUioqocYMRQkc,635
+pymodelio/settings/pymodelio_setting.py,sha256=a9JZsDASvOyjeJtRkBox6S_whZQnHqxbZHeinzVmJMY,202
+pymodelio/settings/pymodelio_settings.py,sha256=06Mf0I8wo5VyRS_EGLSa7vGNE4pf0meF6lLvs1HAnvY,859
+pymodelio/validators/__init__.py,sha256=uHLcZqEjSkZ8ffpTZES9mkNBzql6Ff86YogMIigSEAU,677
 pymodelio/validators/bool_validator.py,sha256=KHTd2I0QRUX-8Lcrxvtg1wqLZvsMotlwv1VpCiZi-cc,285
+pymodelio/validators/date_validator.py,sha256=rBW6T1s-6zQy00RZvklvW_I1A_yHeH4nySz0ViF9CBE,311
 pymodelio/validators/datetime_validator.py,sha256=TZ9Pt_zJZT49OIhAZyf7U37bKWesHQXpJoy6bg6mCjc,323
-pymodelio/validators/default_validators_builder.py,sha256=hQtRE9DkXxSQsamfr5_1Lovk_ohEUJBMXjQpHjS7l88,5539
+pymodelio/validators/default_validators_builder.py,sha256=wX269iUN8_HF76FwTAtEYb79z_FmtHsaraaPtOnr40k,5627
 pymodelio/validators/dict_validator.py,sha256=Y_NmLEFdySBbuDcEdbPCVRF3Sf_mrnyUbdROA8zwSTk,285
-pymodelio/validators/email_validator.py,sha256=xFHPHRNoznLWnd8QVuEbH9BSJxnoszR1RgdkOVCXwN0,752
+pymodelio/validators/email_validator.py,sha256=sFhlnojWWB74JAB6Q7dlemD9Q3Ja3ZEphVyz68iEzsU,754
 pymodelio/validators/float_validator.py,sha256=LOy0OEYn7_7FxILFVngYd24gYEeUF6D5IFJCc44PVXI,463
-pymodelio/validators/forward_ref_validator.py,sha256=8uk-vdrX9TPmg7CnNEhAxPm_mlt1D3o8SCqymddoJyo,961
+pymodelio/validators/forward_ref_validator.py,sha256=tTSLQI6r8z1Gz-MxLDRdqs6-xhvVJOqX9cE5QbzVj4I,1009
 pymodelio/validators/int_validator.py,sha256=_3TJIKZN9G8wprtizbV4JgBiNX2rvsiZmugHjRcno54,455
-pymodelio/validators/iterable_validator.py,sha256=jgtBWEjO54lzDYD_X14aai6qkR301303w4YNOxC8CZw,1331
+pymodelio/validators/iterable_validator.py,sha256=J_NlBQSobVoSYGskPG9hsOaPlqj6v72eYAH8QEXelcY,1333
 pymodelio/validators/list_validator.py,sha256=T5-7KDGyLsg8o7WFAO7djOkKLGrmqzb9Q8Pv2TcvuvY,473
-pymodelio/validators/numeric_validator.py,sha256=M6TpOVg69P460AvBPeu32_sGv9xE_TedmC9nXl7peaA,1010
+pymodelio/validators/numeric_validator.py,sha256=chYQlNL79h6AsA_KkXq8rIz-wPDniVCgfMRBYiPG92o,1012
 pymodelio/validators/set_validator.py,sha256=X7XcbS6Az4E9snK4g_Vr6jXEnGJTY4qGBOQ8HC8ycUQ,471
-pymodelio/validators/string_validator.py,sha256=HidLUkuIYmDhDIZuWa5LYVX6w1rm2XupYhzQY_G9rZM,1341
+pymodelio/validators/string_validator.py,sha256=9IIxCQQonq1GDFoPHWaD3tdsAY3ioimlpyf6aMNPC0Q,1345
 pymodelio/validators/tuple_validator.py,sha256=GLva3HKUmGWTfohgfC1mW2q7DfPl_qIQ5RAH6V8KWt4,475
 pymodelio/validators/validation_patterns.py,sha256=-gSYH0dt_J-K2A10VeAv6bEIi4TRV8x8OWLkYuLZrk4,274
-pymodelio/validators/validator.py,sha256=JvkMDxCpGre4oIJARzF1D7ZED3xsbI1kUmkdp7t0CcE,1372
-pymodelio-1.0.3.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
-pymodelio-1.0.3.dist-info/METADATA,sha256=3rrRNzAMYFiLyDbpbIIkCita0DOuHO09mje4QFPcD-0,24491
-pymodelio-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pymodelio-1.0.3.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
-pymodelio-1.0.3.dist-info/RECORD,,
+pymodelio/validators/validator.py,sha256=zOJApgBcBJ-4hBYRBJuGFDQaJ61EKhU2gXN4Xxk5EhA,1434
+pymodelio-1.1.0.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
+pymodelio-1.1.0.dist-info/METADATA,sha256=9FvxHRIXymuFX-T4wfxMc4IhVz6EGKwozIpzSforPlA,49493
+pymodelio-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pymodelio-1.1.0.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
+pymodelio-1.1.0.dist-info/RECORD,,
```

