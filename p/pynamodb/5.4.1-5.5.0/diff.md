# Comparing `tmp/pynamodb-5.4.1.tar.gz` & `tmp/pynamodb-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb-5.4.1.tar", last modified: Tue Feb 21 04:05:16 2023, max compression
+gzip compressed data, was "pynamodb-5.5.0.tar", last modified: Wed Apr 26 00:02:46 2023, max compression
```

## Comparing `pynamodb-5.4.1.tar` & `pynamodb-5.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 04:05:16.334115 pynamodb-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-21 04:04:56.000000 pynamodb-5.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-21 04:04:56.000000 pynamodb-5.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-02-21 04:05:16.334115 pynamodb-5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-02-21 04:04:56.000000 pynamodb-5.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-21 04:04:56.000000 pynamodb-5.4.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 04:05:16.334115 pynamodb-5.4.1/pynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    49126 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 04:05:16.334115 pynamodb-5.4.1/pynamodb/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/connection/_botocore_private.py
--rw-r--r--   0 runner    (1001) docker     (123)    60648 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/connection/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/connection/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 04:05:16.334115 pynamodb-5.4.1/pynamodb/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/operand.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/expressions/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-21 04:04:56.000000 pynamodb-5.4.1/pynamodb/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 04:05:16.334115 pynamodb-5.4.1/pynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-02-21 04:05:16.000000 pynamodb-5.4.1/pynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-21 04:05:16.000000 pynamodb-5.4.1/pynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 04:05:16.000000 pynamodb-5.4.1/pynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 04:05:15.000000 pynamodb-5.4.1/pynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-21 04:05:16.000000 pynamodb-5.4.1/pynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-21 04:05:16.000000 pynamodb-5.4.1/pynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-21 04:04:56.000000 pynamodb-5.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-21 04:05:16.334115 pynamodb-5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-02-21 04:04:56.000000 pynamodb-5.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-21 04:04:56.000000 pynamodb-5.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:46.274784 pynamodb-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-26 00:02:22.000000 pynamodb-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 00:02:22.000000 pynamodb-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-26 00:02:46.274784 pynamodb-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-26 00:02:22.000000 pynamodb-5.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 00:02:22.000000 pynamodb-5.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:46.270784 pynamodb-5.5.0/pynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49189 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:46.274784 pynamodb-5.5.0/pynamodb/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/connection/_botocore_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60648 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/connection/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/connection/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:46.274784 pynamodb-5.5.0/pynamodb/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13382 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/operand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/expressions/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51486 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-26 00:02:22.000000 pynamodb-5.5.0/pynamodb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 00:02:46.270784 pynamodb-5.5.0/pynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-26 00:02:46.000000 pynamodb-5.5.0/pynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 00:02:46.000000 pynamodb-5.5.0/pynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:02:46.000000 pynamodb-5.5.0/pynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 00:02:45.000000 pynamodb-5.5.0/pynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 00:02:46.000000 pynamodb-5.5.0/pynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 00:02:46.000000 pynamodb-5.5.0/pynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-26 00:02:22.000000 pynamodb-5.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-26 00:02:46.274784 pynamodb-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 00:02:22.000000 pynamodb-5.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 00:02:22.000000 pynamodb-5.5.0/tox.ini
```

### Comparing `pynamodb-5.4.1/LICENSE` & `pynamodb-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/PKG-INFO` & `pynamodb-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 5.4.1
+Version: 5.5.0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Keywords: python dynamodb amazon
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynamodb-5.4.1/README.rst` & `pynamodb-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/attributes.py` & `pynamodb-5.5.0/pynamodb/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,15 +620,15 @@
         Returns a set from a JSON list of numbers.
         """
         return {json.loads(v) for v in value}
 
 
 class VersionAttribute(NumberAttribute):
     """
-    A version attribute
+    A number attribute that implements :ref:`optimistic locking <optimistic_locking>`.
     """
     null = True
 
     def __set__(self, instance, value):
         """
         Cast assigned value to int.
         """
```

### Comparing `pynamodb-5.4.1/pynamodb/connection/_botocore_private.py` & `pynamodb-5.5.0/pynamodb/connection/_botocore_private.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/connection/base.py` & `pynamodb-5.5.0/pynamodb/connection/base.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/connection/table.py` & `pynamodb-5.5.0/pynamodb/connection/table.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/constants.py` & `pynamodb-5.5.0/pynamodb/constants.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/exceptions.py` & `pynamodb-5.5.0/pynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/expressions/condition.py` & `pynamodb-5.5.0/pynamodb/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/expressions/operand.py` & `pynamodb-5.5.0/pynamodb/expressions/operand.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/expressions/projection.py` & `pynamodb-5.5.0/pynamodb/expressions/projection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/expressions/update.py` & `pynamodb-5.5.0/pynamodb/expressions/update.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/expressions/util.py` & `pynamodb-5.5.0/pynamodb/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/indexes.py` & `pynamodb-5.5.0/pynamodb/indexes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/models.py` & `pynamodb-5.5.0/pynamodb/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -398,58 +398,67 @@
         hash_key, range_key = self._get_serialized_keys()
         if self._range_keyname:
             msg = "{}<{}, {}>".format(self.Meta.table_name, hash_key, range_key)
         else:
             msg = "{}<{}>".format(self.Meta.table_name, hash_key)
         return msg
 
-    def delete(self, condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default) -> Any:
+    def delete(self, condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default,
+               *, add_version_condition: bool = True) -> Any:
         """
-        Deletes this object from dynamodb
+        Deletes this object from DynamoDB.
 
+        :param add_version_condition: For models which have a :class:`~pynamodb.attributes.VersionAttribute`,
+          specifies whether the item should only be deleted if its current version matches the expected one.
+          Set to `False` for a 'delete anyway' strategy.
         :raises pynamodb.exceptions.DeleteError: If the record can not be deleted
         """
         hk_value, rk_value = self._get_hash_range_key_serialized_values()
+
         version_condition = self._handle_version_attribute()
-        if version_condition is not None:
+        if add_version_condition and version_condition is not None:
             condition &= version_condition
 
         return self._get_connection().delete_item(hk_value, range_key=rk_value, condition=condition, settings=settings)
 
-    def update(self, actions: List[Action], condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default) -> Any:
+    def update(self, actions: List[Action], condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default, *, add_version_condition: bool = True) -> Any:
         """
         Updates an item using the UpdateItem operation.
 
         :param actions: a list of Action updates to apply
         :param condition: an optional Condition on which to update
         :param settings: per-operation settings
+        :param add_version_condition: For models which have a :class:`~pynamodb.attributes.VersionAttribute`,
+          specifies whether only to update if the version matches the model that is currently loaded.
+          Set to `False` for a 'last write wins' strategy.
+          Regardless, the version will always be incremented to prevent "rollbacks" by concurrent :meth:`save` calls.
         :raises ModelInstance.DoesNotExist: if the object to be updated does not exist
         :raises pynamodb.exceptions.UpdateError: if the `condition` is not met
         """
         if not isinstance(actions, list) or len(actions) == 0:
             raise TypeError("the value of `actions` is expected to be a non-empty list")
 
         hk_value, rk_value = self._get_hash_range_key_serialized_values()
         version_condition = self._handle_version_attribute(actions=actions)
-        if version_condition is not None:
+        if add_version_condition and version_condition is not None:
             condition &= version_condition
 
         data = self._get_connection().update_item(hk_value, range_key=rk_value, return_values=ALL_NEW, condition=condition, actions=actions, settings=settings)
         item_data = data[ATTRIBUTES]
         stored_cls = self._get_discriminator_class(item_data)
         if stored_cls and stored_cls != type(self):
             raise ValueError("Cannot update this item from the returned class: {}".format(stored_cls.__name__))
         self.deserialize(item_data)
         return data
 
-    def save(self, condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default) -> Dict[str, Any]:
+    def save(self, condition: Optional[Condition] = None, settings: OperationSettings = OperationSettings.default, *, add_version_condition: bool = True) -> Dict[str, Any]:
         """
         Save this object to dynamodb
         """
-        args, kwargs = self._get_save_args(condition=condition)
+        args, kwargs = self._get_save_args(condition=condition, add_version_condition=add_version_condition)
         kwargs['settings'] = settings
         data = self._get_connection().put_item(*args, **kwargs)
         self.update_local_version_attribute()
         return data
 
     def refresh(self, consistent_read: bool = False, settings: OperationSettings = OperationSettings.default) -> None:
         """
@@ -470,32 +479,36 @@
         self.deserialize(item_data)
 
     def get_update_kwargs_from_instance(
         self,
         actions: List[Action],
         condition: Optional[Condition] = None,
         return_values_on_condition_failure: Optional[str] = None,
+        *,
+        add_version_condition: bool = True,
     ) -> Dict[str, Any]:
         hk_value, rk_value = self._get_hash_range_key_serialized_values()
 
         version_condition = self._handle_version_attribute(actions=actions)
-        if version_condition is not None:
+        if add_version_condition and version_condition is not None:
             condition &= version_condition
 
         return self._get_connection().get_operation_kwargs(hk_value, range_key=rk_value, key=KEY, actions=actions, condition=condition, return_values_on_condition_failure=return_values_on_condition_failure)
 
     def get_delete_kwargs_from_instance(
         self,
         condition: Optional[Condition] = None,
         return_values_on_condition_failure: Optional[str] = None,
+        *,
+        add_version_condition: bool = True,
     ) -> Dict[str, Any]:
         hk_value, rk_value = self._get_hash_range_key_serialized_values()
 
         version_condition = self._handle_version_attribute()
-        if version_condition is not None:
+        if add_version_condition and version_condition is not None:
             condition &= version_condition
 
         return self._get_connection().get_operation_kwargs(hk_value, range_key=rk_value, key=KEY, condition=condition, return_values_on_condition_failure=return_values_on_condition_failure)
 
     def get_save_kwargs_from_instance(
         self,
         condition: Optional[Condition] = None,
@@ -896,36 +909,39 @@
                 attr_cls = cls.get_attributes()[cls._dynamo_to_python_attr(attr_name)]
                 schema['attribute_definitions'].append({
                     ATTR_NAME: attr_cls.attr_name,
                     ATTR_TYPE: attr_cls.attr_type
                 })
         return schema
 
-    def _get_save_args(self, null_check: bool = True, condition: Optional[Condition] = None) -> Tuple[Iterable[Any], Dict[str, Any]]:
+    def _get_save_args(self, null_check: bool = True, condition: Optional[Condition] = None, *, add_version_condition: bool = True) -> Tuple[Iterable[Any], Dict[str, Any]]:
         """
         Gets the proper *args, **kwargs for saving and retrieving this object
 
         This is used for serializing items to be saved, or for serializing just the keys.
 
         :param null_check: If True, then attributes are checked for null.
         :param condition: If set, a condition
+        :param add_version_condition: For models which have a :class:`~pynamodb.attributes.VersionAttribute`,
+          specifies whether the item should only be saved if its current version matches the expected one.
+          Set to `False` for a 'last-write-wins' strategy.
         """
         attribute_values = self.serialize(null_check)
         hash_key_attribute = self._hash_key_attribute()
         hash_key = attribute_values.pop(hash_key_attribute.attr_name, {}).get(hash_key_attribute.attr_type)
         range_key = None
         range_key_attribute = self._range_key_attribute()
         if range_key_attribute:
             range_key = attribute_values.pop(range_key_attribute.attr_name, {}).get(range_key_attribute.attr_type)
         args = (hash_key, )
         kwargs = {}
         if range_key is not None:
             kwargs['range_key'] = range_key
         version_condition = self._handle_version_attribute(attributes=attribute_values)
-        if version_condition is not None:
+        if add_version_condition and version_condition is not None:
             condition &= version_condition
         kwargs['attributes'] = attribute_values
         kwargs['condition'] = condition
         return args, kwargs
 
     def _get_hash_range_key_serialized_values(self) -> Tuple[Any, Optional[Any]]:
         if self._hash_keyname is None:
```

### Comparing `pynamodb-5.4.1/pynamodb/pagination.py` & `pynamodb-5.5.0/pynamodb/pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/settings.py` & `pynamodb-5.5.0/pynamodb/settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/signals.py` & `pynamodb-5.5.0/pynamodb/signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb/transactions.py` & `pynamodb-5.5.0/pynamodb/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,31 +96,38 @@
         operation_kwargs = model_cls.get_operation_kwargs_from_class(
             hash_key,
             range_key=range_key,
             condition=condition
         )
         self._condition_check_items.append(operation_kwargs)
 
-    def delete(self, model: _M, condition: Optional[Condition] = None) -> None:
-        operation_kwargs = model.get_delete_kwargs_from_instance(condition=condition)
+    def delete(self, model: _M, condition: Optional[Condition] = None, *, add_version_condition: bool = True) -> None:
+        operation_kwargs = model.get_delete_kwargs_from_instance(
+            condition=condition,
+            add_version_condition=add_version_condition,
+        )
         self._delete_items.append(operation_kwargs)
 
     def save(self, model: _M, condition: Optional[Condition] = None, return_values: Optional[str] = None) -> None:
         operation_kwargs = model.get_save_kwargs_from_instance(
             condition=condition,
             return_values_on_condition_failure=return_values
         )
         self._put_items.append(operation_kwargs)
         self._models_for_version_attribute_update.append(model)
 
-    def update(self, model: _M, actions: List[Action], condition: Optional[Condition] = None, return_values: Optional[str] = None) -> None:
+    def update(self, model: _M, actions: List[Action], condition: Optional[Condition] = None,
+               return_values: Optional[str] = None,
+               *,
+               add_version_condition: bool = True) -> None:
         operation_kwargs = model.get_update_kwargs_from_instance(
             actions=actions,
             condition=condition,
-            return_values_on_condition_failure=return_values
+            return_values_on_condition_failure=return_values,
+            add_version_condition=add_version_condition,
         )
         self._update_items.append(operation_kwargs)
         self._models_for_version_attribute_update.append(model)
 
     def _commit(self) -> Any:
         response = self._connection.transact_write_items(
             condition_check_items=self._condition_check_items,
```

### Comparing `pynamodb-5.4.1/pynamodb/util.py` & `pynamodb-5.5.0/pynamodb/util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/pynamodb.egg-info/PKG-INFO` & `pynamodb-5.5.0/pynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 5.4.1
+Version: 5.5.0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Keywords: python dynamodb amazon
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynamodb-5.4.1/pynamodb.egg-info/SOURCES.txt` & `pynamodb-5.5.0/pynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamodb-5.4.1/setup.py` & `pynamodb-5.5.0/setup.py`

 * *Files identical despite different names*

