# Comparing `tmp/hagis-0.4.2.tar.gz` & `tmp/hagis-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.4.2.tar", last modified: Tue Apr 25 20:12:44 2023, max compression
+gzip compressed data, was "hagis-0.4.3.tar", last modified: Wed Apr 26 12:24:40 2023, max compression
```

## Comparing `hagis-0.4.2.tar` & `hagis-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 20:12:44.512939 hagis-0.4.2/
--rw-rw-rw-   0        0        0      923 2023-04-25 20:12:44.511941 hagis-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 20:12:44.502942 hagis-0.4.2/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.2/hagis/__init__.py
--rw-rw-rw-   0        0        0    14023 2023-04-25 19:57:17.000000 hagis-0.4.2/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-25 20:12:44.509937 hagis-0.4.2/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-25 20:12:44.000000 hagis-0.4.2/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-25 20:12:44.000000 hagis-0.4.2/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 20:12:44.000000 hagis-0.4.2/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-25 20:12:44.000000 hagis-0.4.2/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-25 19:59:09.000000 hagis-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 20:12:44.513939 hagis-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.378947 hagis-0.4.3/
+-rw-rw-rw-   0        0        0      923 2023-04-26 12:24:40.378947 hagis-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.338128 hagis-0.4.3/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.3/hagis/__init__.py
+-rw-rw-rw-   0        0        0    14858 2023-04-26 12:20:31.000000 hagis-0.4.3/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:24:40.370697 hagis-0.4.3/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 12:24:40.000000 hagis-0.4.3/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-26 12:23:53.000000 hagis-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 12:24:40.387134 hagis-0.4.3/setup.cfg
```

### Comparing `hagis-0.4.2/PKG-INFO` & `hagis-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.2
+Version: 0.4.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.2/hagis/hagis.py` & `hagis-0.4.3/hagis/hagis.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from datetime import datetime
 from hashlib import md5
 from inspect import signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
-from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
+from uuid import UUID
 from requests import post
 
 T = TypeVar("T")
 
 
 class Layer(Generic[T]):  # pylint: disable=too-many-instance-attributes
     """ Layer class.
@@ -113,24 +114,24 @@
 
         Args:
             token (str): Token.
         """
         self._generate_token = lambda: token
 
     def query(self, where_clause: Optional[str] = None, record_count: Optional[int] = None, wkid: Optional[int] = None,
-              **kwargs: Any) -> Iterable[T]:
+              **kwargs: Any) -> Iterator[T]:
         """ Executes a query.
 
         Args:
             where_clause (str, optional): Where clause.  Defaults to None.
             record_count (Optional[int], optional): Maximum record count.  Defaults to None.
             wkid (Optional[int], optional): Spatial reference.  Defaults to None.
 
         Returns:
-            Iterable[T]: Items.
+            Iterator[T]: Items.
         """
         if not where_clause:
             where_clause = "1=1"
 
         if record_count == 0:
             return
 
@@ -187,15 +188,16 @@
 
         Args:
             oid (int): Object ID.
 
         Returns:
             Optional[T]: Item if found (otherwise None).
         """
-        items = list(self.query(f"{self._oid_field}={oid}", **kwargs))
+        where_clause = self.generate_where_clause(oid)
+        items = list(self.query(where_clause, **kwargs))
         return items[0] if items else None
 
     def apply_edits(self,
                     adds: Optional[List[T]] = None,
                     updates: Optional[List[T]] = None,
                     deletes: Union[List[int], List[str], None] = None, **kwargs: Any) -> SimpleNamespace:
         """ Applies multiple edits atomically.
@@ -237,14 +239,35 @@
         """ Deletes items based on a where clause.
 
         Args:
             where_clause (str): Where clause use for deleting.
         """
         self._call("deleteFeatures", where=where_clause, **kwargs)
 
+    def generate_where_clause(self, *ids: Union[int, str, UUID], id_field: Optional[str] = None) -> str:
+        """ Generates a where clause from a list of Object ID, Global ID or some other identifiers.
+
+        Args:
+            id_field (Optional[str], optional): Name of the ID field. Defaults to None.
+
+        Returns:
+            str: Where clause.
+        """
+        if not ids:
+            return "(1=0)"
+
+        if isinstance(ids[0], int):
+            field_name = id_field if id_field else self._oid_field
+            id_set = set(map(str, ids))
+        else:
+            field_name = id_field if id_field else "globalid"
+            id_set = set((f"'{_id}'" for _id in ids))
+
+        return f"({field_name} IN ({','.join(id_set)}))"
+
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
@@ -305,15 +328,15 @@
                 shape = self._shape_property_type(row.geometry.__dict__)
             else:
                 shape = self._shape_property_type()
                 shape.__dict__ = row.geometry.__dict__
 
         return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
 
-    def _query(self, where_clause: str, fields: str, keep_querying: bool, **kwargs: Any) -> Iterable[SimpleNamespace]:
+    def _query(self, where_clause: str, fields: str, keep_querying: bool, **kwargs: Any) -> Iterator[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
         rows, exceeded_transfer_limit = get_rows(where_clause)
 
         for row in rows:
             yield self._map(row)
```

### Comparing `hagis-0.4.2/hagis.egg-info/PKG-INFO` & `hagis-0.4.3/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.2
+Version: 0.4.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.2/pyproject.toml` & `hagis-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

