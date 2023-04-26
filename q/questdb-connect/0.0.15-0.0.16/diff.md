# Comparing `tmp/questdb-connect-0.0.15.tar.gz` & `tmp/questdb-connect-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.15.tar", last modified: Wed Apr 26 14:18:50 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.16.tar", last modified: Wed Apr 26 14:52:45 2023, max compression
```

## Comparing `questdb-connect-0.0.15.tar` & `questdb-connect-0.0.16.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.449398 questdb-connect-0.0.15/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.15/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:18:50.449259 questdb-connect-0.0.15/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.15/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 13:30:53.000000 questdb-connect-0.0.15/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 14:18:50.449435 questdb-connect-0.0.15/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.444857 questdb-connect-0.0.15/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.447276 questdb-connect-0.0.15/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1355 2023-04-26 13:17:59.000000 questdb-connect-0.0.15/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9739 2023-04-26 14:03:15.000000 questdb-connect-0.0.15/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     7941 2023-04-26 12:20:15.000000 questdb-connect-0.0.15/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     7073 2023-04-26 14:04:36.000000 questdb-connect-0.0.15/src/questdb_connect/types.py
--rw-r--r--   0 marregui   (501) staff       (20)     5788 2023-04-26 13:30:18.000000 questdb-connect-0.0.15/src/questdb_connect/types_copy.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.448225 questdb-connect-0.0.15/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      522 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 14:18:50.000000 questdb-connect-0.0.15/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:18:50.448972 questdb-connect-0.0.15/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.15/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.15/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.15/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:52:45.946339 questdb-connect-0.0.16/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.16/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:52:45.946167 questdb-connect-0.0.16/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.16/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 14:52:31.000000 questdb-connect-0.0.16/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 14:52:45.946380 questdb-connect-0.0.16/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:52:45.941426 questdb-connect-0.0.16/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:52:45.943604 questdb-connect-0.0.16/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1355 2023-04-26 13:17:59.000000 questdb-connect-0.0.16/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9739 2023-04-26 14:03:15.000000 questdb-connect-0.0.16/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7864 2023-04-26 14:52:31.000000 questdb-connect-0.0.16/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5454 2023-04-26 14:40:59.000000 questdb-connect-0.0.16/src/questdb_connect/types.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5788 2023-04-26 13:30:18.000000 questdb-connect-0.0.16/src/questdb_connect/types_copy.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:52:45.944734 questdb-connect-0.0.16/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      522 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 14:52:45.000000 questdb-connect-0.0.16/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 14:52:45.945509 questdb-connect-0.0.16/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.16/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.16/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.16/tests/test_types.py
```

### Comparing `questdb-connect-0.0.15/LICENSE` & `questdb-connect-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/PKG-INFO` & `questdb-connect-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.15
+Version: 0.0.16
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.15/README.md` & `questdb-connect-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/pyproject.toml` & `questdb-connect-0.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.15"
+version = "0.0.16"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.15/src/questdb_connect/__init__.py` & `questdb-connect-0.0.16/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/src/questdb_connect/dialect.py` & `questdb-connect-0.0.16/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.16/src/questdb_connect/superset_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,22 +120,22 @@
         if type_u == 'DATE':
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
-    @classmethod
-    def get_datatype(cls, type_code: Any) -> Optional[str]:
-        """Change column type code from cursor description to string representation.
-        :param type_code: Type code from cursor description
-        :return: String representation of type code
-        """
-        logger.info('QUEST get_datatype(type_code: %s)', type_code)
-        return type_code
+    # @classmethod
+    # def get_datatype(cls, type_code: Any) -> Optional[str]:
+    #     """Change column type code from cursor description to string representation.
+    #     :param type_code: Type code from cursor description
+    #     :return: String representation of type code
+    #     """
+    #     logger.info('QUEST get_datatype(type_code: %s)', type_code)
+    #     return type_code
 
     @classmethod
     def get_column_types(
             cls,
             column_type: Optional[str],
     ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
         if not column_type:
@@ -166,13 +166,12 @@
             generic_type = GenericDataType.NUMERIC
         elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
             generic_type = GenericDataType.STRING
         elif name_u in ('DATE', 'TIMESTAMP'):
             generic_type = GenericDataType.TEMPORAL
         elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
             generic_type = GenericDataType.STRING
-        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
+        return utils.ColumnSpec(sqla_type(), generic_type, generic_type == GenericDataType.TEMPORAL)
 
     @classmethod
     def column_datatype_to_string(cls, sqla_column_type: TypeEngine, *_args):
-        logger.info('QUEST column_datatype_to_string(sqla_column_type: %s)', sqla_column_type)
         return sqla_column_type.compile()
```

### Comparing `questdb-connect-0.0.15/src/questdb_connect/types.py` & `questdb-connect-0.0.16/src/questdb_connect/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,36 +38,22 @@
     HOUR = 4
     WEEK = 5
 
 
 # ===== QUESTDB DATA TYPES =====
 
 _QUOTES = ("'", '"')
-_TYPE_CACHE = {
-    # key:   '__visit_name__' of the implementor of QDBTypeMixin
-    # value: implementor class itself
-}
-
-
-def quote_identifier(identifier: str):
-    if not identifier:
-        return None
-    first = 0
-    last = len(identifier)
-    if identifier[first] in _QUOTES:
-        first += 1
-    if identifier[last - 1] in _QUOTES:
-        last -= 1
-    return f"'{identifier[first:last]}'"
-
-
 _GEOHASH_BYTE_MAX = 8
 _GEOHASH_SHORT_MAX = 16
 _GEOHASH_INT_MAX = 32
 _GEOHASH_LONG_BITS = 60
+_TYPE_CACHE = {
+    # key:   '__visit_name__' of the implementor of QDBTypeMixin
+    # value: implementor class itself
+}
 
 
 def geohash_type_name(bits):
     if not isinstance(bits, int) or bits < 0 or bits > _GEOHASH_LONG_BITS:
         raise ArgumentError(f'geohash precision must be int [0, {_GEOHASH_LONG_BITS}]')
     if 0 < bits <= _GEOHASH_BYTE_MAX:
         return f'GEOHASH(8b)'
@@ -86,168 +72,119 @@
     elif _GEOHASH_BYTE_MAX < bits <= _GEOHASH_SHORT_MAX:
         return GeohashShort
     elif _GEOHASH_SHORT_MAX < bits <= _GEOHASH_INT_MAX:
         return GeohashInt
     return GeohashLong
 
 
-class QDBTypeMixin:
+def quote_identifier(identifier: str):
+    if not identifier:
+        return None
+    first = 0
+    last = len(identifier)
+    if identifier[first] in _QUOTES:
+        first += 1
+    if identifier[last - 1] in _QUOTES:
+        last -= 1
+    return f"'{identifier[first:last]}'"
+
+
+class QDBTypeMixin(sqla.types.TypeDecorator):
     __visit_name__ = 'QDBTypeMixin'
+    impl = sqla.types.String
+    cache_ok = True
 
     @classmethod
     def matches_type_name(cls, type_name):
         return cls if type_name == cls.__visit_name__ else None
 
     def column_spec(self, column_name):
         return f"{quote_identifier(column_name)} {self.__visit_name__}"
 
 
-class Boolean(QDBTypeMixin, sqla.types.Boolean):
+class Boolean(QDBTypeMixin):
     __visit_name__ = 'BOOLEAN'
-
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 1
+    impl = sqla.types.Boolean
 
 
-class Byte(QDBTypeMixin, sqla.types.Integer):
+class Byte(QDBTypeMixin):
     __visit_name__ = 'BYTE'
-
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 2
+    impl = sqla.types.Integer
 
 
-class Short(QDBTypeMixin, sqla.types.Integer):
+class Short(QDBTypeMixin):
     __visit_name__ = 'SHORT'
+    impl = sqla.types.Integer
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 3
 
-
-class Char(QDBTypeMixin, sqla.types.String):
+class Char(QDBTypeMixin):
     __visit_name__ = 'CHAR'
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 4
-
 
-class Int(QDBTypeMixin, sqla.types.Integer):
+class Int(QDBTypeMixin):
     __visit_name__ = 'INT'
-
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 5
+    impl = sqla.types.Integer
 
 
-class Long(QDBTypeMixin, sqla.types.Integer):
+class Long(QDBTypeMixin):
     __visit_name__ = 'LONG'
+    impl = sqla.types.Integer
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 6
 
-
-class Date(QDBTypeMixin, sqla.types.Date):
+class Date(QDBTypeMixin):
     __visit_name__ = 'DATE'
-
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 7
+    impl = sqla.types.Date
 
 
-class Timestamp(QDBTypeMixin, sqla.types.DateTime):
+class Timestamp(QDBTypeMixin):
     __visit_name__ = 'TIMESTAMP'
+    impl = sqla.types.DateTime
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 8
 
-
-class Float(QDBTypeMixin, sqla.types.Float):
+class Float(QDBTypeMixin):
     __visit_name__ = 'FLOAT'
-
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 9
+    impl = sqla.types.Float
 
 
-class Double(QDBTypeMixin, sqla.types.Float):
+class Double(QDBTypeMixin):
     __visit_name__ = 'DOUBLE'
+    impl = sqla.types.Float
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 10
 
-
-class String(QDBTypeMixin, sqla.types.String):
+class String(QDBTypeMixin):
     __visit_name__ = 'STRING'
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 11
-
 
-class Symbol(QDBTypeMixin, sqla.types.String):
+class Symbol(QDBTypeMixin):
     __visit_name__ = 'SYMBOL'
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 12
-
 
-class Long256(QDBTypeMixin, sqla.types.String):
+class Long256(QDBTypeMixin):
     __visit_name__ = 'LONG256'
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 13
 
-
-class GeohashByte(QDBTypeMixin, sqla.types.String):
+class GeohashByte(QDBTypeMixin):
     __visit_name__ = geohash_type_name(8)
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 14
-
 
-class GeohashShort(QDBTypeMixin, sqla.types.String):
+class GeohashShort(QDBTypeMixin):
     __visit_name__ = geohash_type_name(16)
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 15
-
 
-class GeohashInt(QDBTypeMixin, sqla.types.String):
+class GeohashInt(QDBTypeMixin):
     __visit_name__ = geohash_type_name(32)
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 16
 
-
-class GeohashLong(QDBTypeMixin, sqla.types.String):
+class GeohashLong(QDBTypeMixin):
     __visit_name__ = geohash_type_name(60)
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 17
-
 
-class UUID(QDBTypeMixin, sqla.types.String):
+class UUID(QDBTypeMixin):
     __visit_name__ = 'UUID'
 
-    def __init__(self, **kw):
-        super().__init__(**kw)
-        self.type_code = 19
-
 
 QUESTDB_TYPES = [
     Long256,
     Boolean,
     Byte,
     Short,
     Char,
```

### Comparing `questdb-connect-0.0.15/src/questdb_connect/types_copy.py` & `questdb-connect-0.0.16/src/questdb_connect/types_copy.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.16/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.15
+Version: 0.0.16
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.15/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.16/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/tests/test_dialect.py` & `questdb-connect-0.0.16/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/tests/test_superset.py` & `questdb-connect-0.0.16/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.15/tests/test_types.py` & `questdb-connect-0.0.16/tests/test_types.py`

 * *Files identical despite different names*

