# Comparing `tmp/sqlalchemy_bind_manager-0.2.0.tar.gz` & `tmp/sqlalchemy_bind_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.2.0.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.2.1.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.2.0.tar` & `sqlalchemy_bind_manager-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0    11748 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/README.md
--rw-r--r--   0        0        0     1957 2023-04-25 16:21:08.130027 sqlalchemy_bind_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      301 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5221 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      136 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     5958 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0     6778 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     5520 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3125 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1698 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_unit_of_work.py
--rw-r--r--   0        0        0      310 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0     1995 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-04-25 16:20:54.966057 sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0    13392 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/LICENSE
+-rw-r--r--   0        0        0    11748 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/README.md
+-rw-r--r--   0        0        0     1957 2023-04-25 17:00:09.547293 sqlalchemy_bind_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5221 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      136 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     5959 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0     6296 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     5521 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3125 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_transaction_handler.py
+-rw-r--r--   0        0        0     1698 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_unit_of_work.py
+-rw-r--r--   0        0        0      310 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0     1995 2023-04-25 16:59:54.454825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:59:54.454825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0    13392 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.2.1/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.2.0/LICENSE` & `sqlalchemy_bind_manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/README.md` & `sqlalchemy_bind_manager-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/pyproject.toml` & `sqlalchemy_bind_manager-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.2.0"
+version = "0.2.1"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
 keywords = ["sqlalchemy", "config", "manager"]
```

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     ) -> None:
         """Deletes a model.
 
         :param entity: The model instance or the primary key
         :type entity: Union[MODEL, PRIMARY_KEY]
         """
         # TODO: delete without loading the model
-        obj = entity if self._is_mapped_object(entity) else await self.get(entity)  # type: ignore
+        obj = entity if isinstance(entity, self._model) else await self.get(entity)  # type: ignore
         async with self._get_session() as session:
             await session.delete(obj)
 
     async def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
```

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Mapping,
     List,
     Collection,
 )
 
 from pydantic.generics import GenericModel
 from sqlalchemy import asc, desc, select, func
-from sqlalchemy.orm import object_mapper, class_mapper, Mapper, lazyload
-from sqlalchemy.orm.exc import UnmappedInstanceError
+from sqlalchemy.orm import class_mapper, Mapper, lazyload
+from sqlalchemy.orm.exc import UnmappedClassError
 from sqlalchemy.sql import Select
 
 from sqlalchemy_bind_manager.exceptions import InvalidModel, UnmappedProperty
 
 MODEL = TypeVar("MODEL")
 PRIMARY_KEY = Union[str, int, tuple, dict]
 
@@ -44,39 +44,33 @@
     _max_query_limit: int = 50
     _model: Type[MODEL]
 
     def __init__(self, model_class: Union[Type[MODEL], None] = None) -> None:
         if getattr(self, "_model", None) is None and model_class is not None:
             self._model = model_class
 
-        if getattr(self, "_model", None) is None or not self._is_mapped_object(
-            self._model()
+        if getattr(self, "_model", None) is None or not self._is_mapped_class(
+            self._model
         ):
             raise InvalidModel(
                 "You need to supply a valid model class either in the `model_class` parameter"
                 " or in the `_model` class property."
             )
 
-    def _is_mapped_object(self, obj: object) -> bool:
-        """Checks if the object is handled by the repository and is mapped in SQLAlchemy.
+    def _is_mapped_class(self, class_: Type[MODEL]) -> bool:
+        """Checks if the class is mapped in SQLAlchemy.
 
-        :param obj: a mapped object instance
-        :return: True if the object is mapped and matches self._model type, False if it's not a mapped object
+        :param class_: the model class
+        :return: True if the Type is mapped, False otherwise
         :rtype: bool
-        :raises InvalidModel: when the object is mapped but doesn't match self._model type
         """
-        # TODO: This is probably redundant, we could do these checks once in __init__
         try:
-            object_mapper(obj)
-            if isinstance(obj, self._model):
-                return True
-            raise InvalidModel(
-                f"This repository can handle only `{self._model}` models. `{type(obj)}` has been passed."
-            )
-        except UnmappedInstanceError:
+            class_mapper(class_)
+            return True
+        except UnmappedClassError:
             return False
 
     def _validate_mapped_property(self, property_name: str) -> None:
         """Checks if a property is mapped in the model class.
 
         :param property_name: The name of the property to be evaluated.
         :type property_name: str
```

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def delete(self, entity: Union[MODEL, PRIMARY_KEY]) -> None:
         """Deletes a model.
 
         :param entity: The model instance or the primary key
         :type entity: Union[MODEL, PRIMARY_KEY]
         """
         # TODO: delete without loading the model
-        obj = entity if self._is_mapped_object(entity) else self.get(entity)  # type: ignore
+        obj = entity if isinstance(entity, self._model) else self.get(entity)  # type: ignore
         with self._get_session() as session:
             session.delete(obj)
 
     def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
```

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_transaction_handler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/_unit_of_work.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.0/PKG-INFO` & `sqlalchemy_bind_manager-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://github.com/febus982/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
```

