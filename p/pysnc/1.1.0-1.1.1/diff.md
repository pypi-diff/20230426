# Comparing `tmp/pysnc-1.1.0.tar.gz` & `tmp/pysnc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.0.tar", max compression
+gzip compressed data, was "pysnc-1.1.1.tar", max compression
```

## Comparing `pysnc-1.1.0.tar` & `pysnc-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-04-26 00:11:09.588473 pysnc-1.1.0/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-26 00:11:09.588473 pysnc-1.1.0/README.md
--rw-r--r--   0        0        0      984 2023-04-26 00:11:09.592473 pysnc-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/__version__.py
--rw-r--r--   0        0        0     8875 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/attachment.py
--rw-r--r--   0        0        0     3778 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/auth.py
--rw-r--r--   0        0        0    15715 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/client.py
--rw-r--r--   0        0        0      953 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/exceptions.py
--rw-r--r--   0        0        0     3809 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/query.py
--rw-r--r--   0        0        0    35456 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-04-26 00:11:09.592473 pysnc-1.1.0/pysnc/utils.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-04-26 00:41:10.768887 pysnc-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1590 2023-04-26 00:41:10.768887 pysnc-1.1.1/README.md
+-rw-r--r--   0        0        0      984 2023-04-26 00:41:10.772887 pysnc-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/__version__.py
+-rw-r--r--   0        0        0     8875 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/attachment.py
+-rw-r--r--   0        0        0     3778 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/auth.py
+-rw-r--r--   0        0        0    15782 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3809 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/query.py
+-rw-r--r--   0        0        0    37242 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-04-26 00:41:10.772887 pysnc-1.1.1/pysnc/utils.py
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.1/PKG-INFO
```

### Comparing `pysnc-1.1.0/LICENSE` & `pysnc-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/README.md` & `pysnc-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/pyproject.toml` & `pysnc-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
```

### Comparing `pysnc-1.1.0/pysnc/attachment.py` & `pysnc-1.1.1/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/pysnc/auth.py` & `pysnc-1.1.1/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/pysnc/client.py` & `pysnc-1.1.1/pysnc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,18 @@
         self._client = client
 
     @property
     def session(self):
         return self._client.session
 
     # noinspection PyMethodMayBeStatic
-    def _set_params(self, record=None):
-        params = {} if record == None else record._parameters()
-        params['sysparm_display_value'] = 'all'
+    def _set_params(self, record: GlideRecord=None):
+        params = {} if record is None else record._parameters()
+        if 'sysparm_display_value' not in params:
+            params['sysparm_display_value'] = 'all'
         params['sysparm_exclude_reference_link'] = 'true'  # Scratch it!
         params['sysparm_suppress_pagination_header'] = 'true'  # Required for large queries
         return params
 
     # noinspection PyMethodMayBeStatic
     def _validate_response(self, response: requests.Response) -> None:
         assert response is not None, f"response argument required"
```

### Comparing `pysnc-1.1.0/pysnc/exceptions.py` & `pysnc-1.1.1/pysnc/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,9 +43,14 @@
 class RequestException(Exception):
     pass
 
 
 class InstanceException(Exception):
     pass
 
+
 class UploadException(Exception):
-    pass
+    pass
+
+
+class NoRecordException(Exception):
+    pass
```

### Comparing `pysnc-1.1.0/pysnc/query.py` & `pysnc-1.1.1/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/pysnc/record.py` & `pysnc-1.1.1/pysnc/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,48 +14,52 @@
 TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S%z"
 
 
 class GlideElement(object):
     """
     Object backing the value/display values of a given record entry.
     """
-    def __init__(self, name: str, value=None, display_value=None):
+    def __init__(self, name: str, value=None, display_value=None, parent_record=None):
         self._name = name
         self._value = None
         self._display_value = None
         self._changed = False
         if isinstance(value, dict):
             self._value = value['value']
             # only bother to set display value if it's different
             if self._value != value['display_value']:
                 self._display_value = value['display_value']
         else:
             self._value = value
         if display_value:
             self._display_value = display_value
 
+        self._parent_record = parent_record
+
     def get_name(self) -> str:
         """
         get the name of the field
         """
         return self._name
 
     def get_value(self) -> Any:
         """
         get the value of the field
         """
-        return self._value
+        if self._value is not None:
+            return self._value
+        return self._display_value  # if we are display only
 
     def get_display_value(self) -> Any:
         """
-        get the display value of the field
+        get the display value of the field, if it has one, else just the value
         """
         if self._display_value:
             return self._display_value
-        return self.get_value()
+        return self._value
 
     def set_value(self, value):
         """
         set the value for the field. Will also set the display_value to `None`
         """
         if isinstance(value, GlideElement):
             value = value.get_value()
@@ -180,15 +184,23 @@
 
     def __ge__(self, other):
         return self.__magic('__ge__', other)
 
     def __getattr__(self, item):
         if item in GlideElement.__class__.__dict__:
             return self.__getattribute__(item)
-        return getattr(self.get_value(), item)
+
+        if self._parent_record:
+            if tv := self._parent_record.get_element(f"{self._name}.{item}"):
+                return tv
+
+        if hasattr(self.get_value(), item):
+            return getattr(self.get_value(), item)
+
+        raise AttributeError(f"{type(self.get_value())} has no attribute '{item}' nor GlideElement '{self._name}.{item}' -- did you mean to add this to the GlideRecord fields?")
 
     def __deepcopy__(self, memo):
         """
         ultimately for copy.deepcopy and the use of .pop_record(), avoids recusion doing it this way
         """
         ne = GlideElement(self.get_name(), self.get_value())
         if self._display_value:
@@ -218,14 +230,15 @@
         self.__field_limits = None
         self.__view = None
         self.__total = None
         self.__limit = None
         self.__page = -1
         self.__order = None
         self.__is_new_record = False
+        self.__display_value = 'all'
 
     def _clear_query(self):
         self.__query = Query(self.__table)
 
     def _parameters(self):
         ret = dict(
             sysparm_query=self.__query.generate_query(encoded_query=self.__encoded_query, order_by=self.__order)
@@ -234,14 +247,16 @@
             c = self.__field_limits
             if 'sys_id' not in self.__field_limits:
                 c.insert(0, 'sys_id')
 
             ret['sysparm_fields'] = ','.join(c)
         if self.__view:
             ret['sysparm_view'] = self.__view
+
+        ret['sysparm_display_value'] = str(self.display_value).lower()
         # Batch size matters! Transaction limits will exceed.
         # This also means we have to be pretty specific with limits
         limit = None
         if self.__limit:
             if self.__limit >= self.batch_size:
                 # need to re-calc as our actual queried count will end up greater than our limit
                 # this keeps us at our actual limit even when between batch size boundaries
@@ -357,14 +372,28 @@
         Set the current location
 
         :param location: the location to be at
         """
         assert -1 <= location < self.__total
         self.__current = location
 
+    @property
+    def display_value(self):
+        return self.__display_value
+
+    @display_value.setter
+    def display_value(self, display_value):
+        """
+        True: Returns the display values for all fields.
+        False: Returns the actual values from the database.
+        all: Returns both actual and display values.
+        """
+        assert display_value in [True, False, 'all']
+        self.__display_value = display_value
+
     def order_by(self, column: str):
         """
         Set the order in ascending
 
         :param column: Column to sort by
         """
         if column:
@@ -602,14 +631,16 @@
             self._client.batch_api.put(e, handle)
 
         self._client.batch_api.execute()
         return updated
 
     def _get_value(self, item, key='value'):
         obj = self._current()
+        if obj is None:
+            raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
         if item in obj:
             o = obj[item]
             if key == 'display_value':
                 return o.get_display_value()
             return o.get_value()
         return None
 
@@ -636,39 +667,45 @@
         """
         Return the backing GlideElement for the given field. This is the only method to directly access this element.
 
         :param str field: The Field
         :return: The GlideElement class or ``None``
         """
         c = self._current()
+        if c is None:
+            raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
         return self._current()[field] if field in c else None
 
     def set_value(self, field, value):
         """
         Set the value for a field.
 
         :param str field: The field
         :param value: The Value
         """
         c = self._current()
+        if c is None:
+            raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
         if field not in c:
-            c[field] = GlideElement(field, value)
+            c[field] = GlideElement(field, value, parent_record=self)
         else:
             c[field].set_value(value)
 
     def set_display_value(self, field, value):
         """
         Set the display value for a field.
 
         :param str field: The field
         :param value: The Value
         """
         c = self._current()
+        if c is None:
+            raise NoRecordException('cannot get a value from nothing, did you forget to call next() or initialize()?')
         if field not in c:
-            c[field] = GlideElement(field, display_value=value)
+            c[field] = GlideElement(field, display_value=value, parent_record=self)
         else:
             c[field].set_display_value(value)
 
     def get_link(self, no_stack=False) -> str:
         """
         Generate a full URL to the current record. sys_id will be null if there is no current record.
 
@@ -723,15 +760,15 @@
         if self.sys_id:
             attachment.add_query('table_sys_id', self.sys_id)
         attachment.query()
         return attachment
 
     def add_attachment(self, file_name, file, content_type=None, encryption_context=None):
         if self._current() is None:
-            raise UpdateException('Cannot attach to non existant record')
+            raise NoRecordException('cannot add attachment to nothing, did you forget to call next() or initialize()?')
 
         attachment = self._client.Attachment(self.__table)
         attachment.add_attachment(self.sys_id, file_name, file, content_type, encryption_context)
 
     def add_active_query(self) -> QueryCondition:
         """
         Equivilant to the following::
@@ -1013,15 +1050,15 @@
         l = len(self.__results)
         if l > 0 and self.__current + 1 < l:
             return True
         return False
 
     def _transform_result(self, result):
         for key, value in result.items():
-            result[key] = GlideElement(key, value)
+            result[key] = GlideElement(key, value, parent_record=self)
         return result
 
     def __str__(self):
         return """{}({})""".format(
             self.__table,
             self._serialize(self._current(), False)
         )
```

### Comparing `pysnc-1.1.0/pysnc/utils.py` & `pysnc-1.1.1/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.0/PKG-INFO` & `pysnc-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
```

