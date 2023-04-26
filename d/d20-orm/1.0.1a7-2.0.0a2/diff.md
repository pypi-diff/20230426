# Comparing `tmp/d20-orm-1.0.1a7.tar.gz` & `tmp/d20-orm-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-xghf5k62\d20-orm-1.0.1a7.tar", last modified: Tue Feb 28 01:52:22 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\arangodb_python_orm\dist\.tmp-to0ynwmh\d20-orm-2.0.0a2.tar", last modified: Wed Apr 26 00:17:11 2023, max compression
```

## Comparing `d20-orm-1.0.1a7.tar` & `d20-orm-2.0.0a2.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 01:52:22.080930 d20-orm-1.0.1a7/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-1.0.1a7/LICENSE
--rw-rw-rw-   0        0        0      794 2023-02-28 01:52:22.080930 d20-orm-1.0.1a7/PKG-INFO
--rw-rw-rw-   0        0        0      241 2022-08-08 23:27:23.000000 d20-orm-1.0.1a7/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-1.0.1a7/pyproject.toml
--rw-rw-rw-   0        0        0       72 2023-02-28 01:52:22.090473 d20-orm-1.0.1a7/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-02-28 01:52:03.000000 d20-orm-1.0.1a7/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-28 01:52:22.004162 d20-orm-1.0.1a7/src/
-drwxrwxrwx   0        0        0        0 2023-02-28 01:52:22.045252 d20-orm-1.0.1a7/src/d20_orm.egg-info/
--rw-rw-rw-   0        0        0      794 2023-02-28 01:52:21.000000 d20-orm-1.0.1a7/src/d20_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-02-28 01:52:21.000000 d20-orm-1.0.1a7/src/d20_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 01:52:21.000000 d20-orm-1.0.1a7/src/d20_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-28 01:52:21.000000 d20-orm-1.0.1a7/src/d20_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-28 01:52:21.000000 d20-orm-1.0.1a7/src/d20_orm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 01:52:22.078977 d20-orm-1.0.1a7/src/dtwentyORM/
--rw-rw-rw-   0        0        0    17021 2023-02-28 01:49:16.000000 d20-orm-1.0.1a7/src/dtwentyORM/BasicElement.py
--rw-rw-rw-   0        0        0     6134 2022-08-05 22:47:50.000000 d20-orm-1.0.1a7/src/dtwentyORM/Element.py
--rw-rw-rw-   0        0        0     7477 2022-05-21 15:54:32.000000 d20-orm-1.0.1a7/src/dtwentyORM/Error.py
--rw-rw-rw-   0        0        0     3367 2022-05-20 22:19:47.000000 d20-orm-1.0.1a7/src/dtwentyORM/GraphClassFactory.py
--rw-rw-rw-   0        0        0     7662 2023-02-28 01:48:22.000000 d20-orm-1.0.1a7/src/dtwentyORM/Metadata.py
--rw-rw-rw-   0        0        0       76 2021-09-22 23:58:20.000000 d20-orm-1.0.1a7/src/dtwentyORM/__init__.py
--rw-rw-rw-   0        0        0       73 2023-02-28 01:32:51.000000 d20-orm-1.0.1a7/src/dtwentyORM/__version__.py
--rw-rw-rw-   0        0        0     1427 2021-09-10 22:14:26.000000 d20-orm-1.0.1a7/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-04-26 00:17:11.060244 d20-orm-2.0.0a2/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-orm-2.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0      895 2023-04-26 00:17:11.060244 d20-orm-2.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-25 02:17:24.000000 d20-orm-2.0.0a2/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-orm-2.0.0a2/pyproject.toml
+-rw-rw-rw-   0        0        0       72 2023-04-26 00:17:11.061244 d20-orm-2.0.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      880 2023-04-26 00:16:34.000000 d20-orm-2.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 00:17:10.861710 d20-orm-2.0.0a2/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 00:17:10.930773 d20-orm-2.0.0a2/src/d20_orm.egg-info/
+-rw-rw-rw-   0        0        0      895 2023-04-26 00:17:10.000000 d20-orm-2.0.0a2/src/d20_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-04-26 00:17:10.000000 d20-orm-2.0.0a2/src/d20_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 00:17:10.000000 d20-orm-2.0.0a2/src/d20_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-26 00:17:10.000000 d20-orm-2.0.0a2/src/d20_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 00:17:10.000000 d20-orm-2.0.0a2/src/d20_orm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 00:17:10.983379 d20-orm-2.0.0a2/src/dtwentyORM/
+-rw-rw-rw-   0        0        0     8911 2023-04-25 23:14:04.000000 d20-orm-2.0.0a2/src/dtwentyORM/BasicElement.py
+-rw-rw-rw-   0        0        0     7199 2023-04-25 23:14:04.000000 d20-orm-2.0.0a2/src/dtwentyORM/DBConnector.py
+-rw-rw-rw-   0        0        0     4749 2023-04-26 00:06:49.000000 d20-orm-2.0.0a2/src/dtwentyORM/Element.py
+-rw-rw-rw-   0        0        0     7462 2023-04-06 00:37:34.000000 d20-orm-2.0.0a2/src/dtwentyORM/Error.py
+-rw-rw-rw-   0        0        0     3632 2023-04-18 00:32:09.000000 d20-orm-2.0.0a2/src/dtwentyORM/GraphClassFactory.py
+-rw-rw-rw-   0        0        0     5167 2023-04-25 23:14:04.000000 d20-orm-2.0.0a2/src/dtwentyORM/Metadata.py
+-rw-rw-rw-   0        0        0       95 2023-04-06 00:37:34.000000 d20-orm-2.0.0a2/src/dtwentyORM/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-02-28 02:21:55.000000 d20-orm-2.0.0a2/src/dtwentyORM/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-18 00:31:28.000000 d20-orm-2.0.0a2/src/dtwentyORM/support.py
+drwxrwxrwx   0        0        0        0 2023-04-26 00:17:11.058712 d20-orm-2.0.0a2/test/
+-rw-rw-rw-   0        0        0      476 2023-04-25 02:17:24.000000 d20-orm-2.0.0a2/test/test_basic_element_test.py
+-rw-rw-rw-   0        0        0      611 2023-04-25 02:17:24.000000 d20-orm-2.0.0a2/test/test_build_db.py
+-rw-rw-rw-   0        0        0      331 2023-04-25 02:17:24.000000 d20-orm-2.0.0a2/test/test_crud_collection.py
+-rw-rw-rw-   0        0        0      253 2023-04-25 02:17:24.000000 d20-orm-2.0.0a2/test/test_metadata.py
+-rw-rw-rw-   0        0        0      105 2023-04-05 22:18:50.000000 d20-orm-2.0.0a2/test/test_params.py
```

### Comparing `d20-orm-1.0.1a7/LICENSE` & `d20-orm-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-orm-1.0.1a7/PKG-INFO` & `d20-orm-2.0.0a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 1.0.1a7
+Version: 2.0.0a2
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,11 +12,13 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # arangodb_python_orm
 ORM for datafield based apps on Python and ArangoDB
 
-### Version 1.0.1
+### Version 2.0.0
+Added GraphClassFactory wich allows you to create your DB, collections and graphs with no effort.
+
 Added support for Metada DB prefix
 Auto-gen Element table if not present
 Search does not get rid of deleted items automatically, new parameter added
```

### Comparing `d20-orm-1.0.1a7/src/d20_orm.egg-info/PKG-INFO` & `d20-orm-2.0.0a2/src/d20_orm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-orm
-Version: 1.0.1a7
+Version: 2.0.0a2
 Summary: A small ORM for multimodel DBs
 Home-page: https://github.com/d20services/arangodb_python_orm
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/arangodb_python_orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,11 +12,13 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # arangodb_python_orm
 ORM for datafield based apps on Python and ArangoDB
 
-### Version 1.0.1
+### Version 2.0.0
+Added GraphClassFactory wich allows you to create your DB, collections and graphs with no effort.
+
 Added support for Metada DB prefix
 Auto-gen Element table if not present
 Search does not get rid of deleted items automatically, new parameter added
```

### Comparing `d20-orm-1.0.1a7/src/dtwentyORM/Element.py` & `d20-orm-2.0.0a2/src/dtwentyORM/Element.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,105 @@
 # File: ArangoDB ORM
 # Author: alexsanchezvega
 # Company: d20
 # Version: 2.0
 
-from pyArango.connection import *
-from pyArango.collection import *
-from pyArango.graph import *
 from .support import *
 from .BasicElement import BasicElement
 
 class Element(BasicElement):
 
-    from .Metadata import Metadata
-
-    def get_class(self):
-        return 'Element'
-
     def dict_by_scope(self, scopes=[]):
         res = {}
         for s in scopes:
             if s in self.get('scopes'):
                 for a in self.get('scopes')[s]:
                     res[a] = self.get(a)
         return res
 
     def make(self):
-        df = self.Metadata.DataField('set', {'obj_type':self.get_class().lower(), 'active': True, 'deleted': False})
+        from .Metadata import Metadata
+        df = Metadata.DataField(obj_type=self.__class__.__name__.lower())
         df.get_all()
-        dfa = df.get('datafields')
-        self.data_fields = dfa
-        self.attributes = []
-        [self.attributes.append(f.get('name')) for f in self.data_fields]
+        self.data_fields = df.get('found')
         self.scopes = {}
         self.obj_attributes = []
+        self.attributes = []
         for f in self.data_fields:
+            self.attributes.append(f.get('name'))
             if f.get('type') == 'object' and f.get('isArray') != True:
                 self.obj_attributes.append({'name':f.get('name'), 'obj_type':f.get('subtype')})
             if not f.get('scope') in self.get('scopes'):
                 self.scopes[f.get('scope')] = []
             self.scopes[f.get('scope')].append(f.get('name'))
         for key in self.attributes:
             setattr(self, key, None)
             
     def get_related_object(self, otype, okey):
-        cached_res = search_obj_cache(otype, okey)
-        if cached_res != None:
-            return cached_res
-        ans = []
-        obj = self.db[self.Metadata.DataField.class_to_coll(otype)].fetchDocument(okey)
-        df = self.Metadata.DataField('set', {'obj_type':self.Metadata.DataField.coll_to_class(otype).lower(), 'active': True, 'deleted' :False, 'search_extract':True})
+        from .Metadata import Metadata
+        obj = globals()[otype](id=okey)
+        obj.load()
+        df = Metadata.DataField(obj_type=otype.lower(), data={'active': True, 'deleted' :False, 'search_extract':True})
         df.get_all()
-        dfb = self.Metadata.DataField('set', {'obj_type':self.Metadata.DataField.coll_to_class(otype).lower(), 'active': True, 'deleted' :False, 'scope':'basic'})
+        dfb = Metadata.DataField(obj_type=otype.lower(), data={'active': True, 'deleted' :False, 'scope':'basic'})
         dfb.get_all()
-        schema = df.get('datafields', [])
-        schema_basic = dfb.get('datafields', [])
-        ans = [obj.getStore(), schema, schema_basic]
-        add_obj_cache(otype, okey, obj.getStore(), schema, schema_basic)
+        schema = df.get('found', [])
+        schema_basic = dfb.get('found', [])
+        ans = [obj.to_dict(), schema, schema_basic]
         return ans
 
-    def find(self):
-        try:
-            found = self.db[self.get_collection()].fetchDocument(self._key)
-            if found.getStore().get('deleted') == True:
-                found = None
-            for key in self.attributes:
-                setattr(self, key, found.getStore()[key] if key in found.getStore() else self.get(key))
-            for att in self.obj_attributes:
-                try:
-                    otype = att['obj_type']
-                    att_val = self.get(att['name'])
-                    if '_to' == att['name']:
-                        otype = self.get('_to').split("/")[0]
-                        self._to = self.get('_to').split("/")[1]
-                        [o_to, schema, schema_basic] = self.get_related_object(otype, self._to)
-                        if len(schema) > 0:
-                            alias = schema[0]['name']
-                            if alias in o_to:
-                                self.alias_to = o_to[alias]
-                            else:
-                                self.alias_to = ''
-                            self.attributes.append('alias_to')
-                            self.scopes['basic'].append('alias_to')
-                            self.obj_to = {}
-                            for df in schema_basic:
-                                if df['name'] in o_to:
-                                    self.obj_to[df['name']] = o_to[df['name']] 
-                            self.attributes.append('obj_to')
-                            self.scopes['basic'].append('obj_to')
-                    elif '_from' == att['name']:
-                        otype = self.get('_from').split("/")[0]
-                        self._from = self.get('_from').split("/")[1]
-                        [o_from, schema, schema_basic] = self.get_related_object(otype, self._from)
-                        if len(schema) > 0:
-                            alias = schema[0]['name']
-                            if alias in o_from:
-                                self.alias_from = o_from[alias]
-                            else:
-                                self.alias_from = ''
-                            self.attributes.append('alias_from')
-                            self.scopes['basic'].append('alias_from')
-                            self.obj_from = {}
-                            for df in schema_basic:
-                                if df['name'] in o_from:
-                                    self.obj_from[df['name']] = o_from[df['name']] 
-                            self.attributes.append('obj_from')
-                            self.scopes['basic'].append('obj_from')
-                    elif self.get(att['name']) != '' and self.get(att['name']) != [] and self.get(att['name']) != None:
-                        [obj, schema, schema_basic] = self.get_related_object(otype, att_val)
-                        if len(schema) > 0:
-                            alias = schema[0]['name']
-                            if alias in obj:
-                                self.__setattr__(f'alias_{att["name"]}',obj[alias])
-                                self.attributes.append(f'alias_{att["name"]}')
-                                self.scopes['basic'].append(f'alias_{att["name"]}')
-                            obj_p = {}
-                            for df in schema_basic:
-                                if df['name'] in obj:
-                                    obj_p[df['name']] = obj[df['name']]
-                            self.__setattr__(f'obj_{att["name"]}',obj_p)
-                            self.attributes.append(f'obj_{att["name"]}')
-                            self.scopes['basic'].append(f'obj_{att["name"]}')
-                except:
-                    pass
-            self.status = True
-        except:
-            self._key = None
-            self.status = False
+    def load(self, get_if_deleted=False):
+        super.load(get_if_deleted=get_if_deleted)
+        for att in self.obj_attributes:
+            otype = att['obj_type']
+            att_val = self.get(att['name'])
+            if '_to' == att['name']:
+                otype = self.get('_to').split("/")[0]
+                self._to = self.get('_to').split("/")[1]
+                [o_to, schema, schema_basic] = self.get_related_object(otype, self._to)
+                if len(schema) > 0:
+                    alias = schema[0]['name']
+                    if alias in o_to:
+                        self.alias_to = o_to[alias]
+                    else:
+                        self.alias_to = ''
+                    self.attributes.append('alias_to')
+                    self.scopes['basic'].append('alias_to')
+                    self.obj_to = {}
+                    for df in schema_basic:
+                        if df['name'] in o_to:
+                            self.obj_to[df['name']] = o_to[df['name']] 
+                    self.attributes.append('obj_to')
+                    self.scopes['basic'].append('obj_to')
+            elif '_from' == att['name']:
+                otype = self.get('_from').split("/")[0]
+                self._from = self.get('_from').split("/")[1]
+                [o_from, schema, schema_basic] = self.get_related_object(otype, self._from)
+                if len(schema) > 0:
+                    alias = schema[0]['name']
+                    if alias in o_from:
+                        self.alias_from = o_from[alias]
+                    else:
+                        self.alias_from = ''
+                    self.attributes.append('alias_from')
+                    self.scopes['basic'].append('alias_from')
+                    self.obj_from = {}
+                    for df in schema_basic:
+                        if df['name'] in o_from:
+                            self.obj_from[df['name']] = o_from[df['name']] 
+                    self.attributes.append('obj_from')
+                    self.scopes['basic'].append('obj_from')
+            elif self.get(att['name']) != '' and self.get(att['name']) != [] and self.get(att['name']) != None:
+                [obj, schema, schema_basic] = self.get_related_object(otype, att_val)
+                if len(schema) > 0:
+                    alias = schema[0]['name']
+                    if alias in obj:
+                        self.__setattr__(f'alias_{att["name"]}',obj[alias])
+                        self.attributes.append(f'alias_{att["name"]}')
+                        self.scopes['basic'].append(f'alias_{att["name"]}')
+                    obj_p = {}
+                    for df in schema_basic:
+                        if df['name'] in obj:
+                            obj_p[df['name']] = obj[df['name']]
+                    self.__setattr__(f'obj_{att["name"]}',obj_p)
+                    self.attributes.append(f'obj_{att["name"]}')
+                    self.scopes['basic'].append(f'obj_{att["name"]}')
```

### Comparing `d20-orm-1.0.1a7/src/dtwentyORM/Error.py` & `d20-orm-2.0.0a2/src/dtwentyORM/Error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from flask import jsonify
+class DBNotExists(Exception):
+    
+    def __init__(self, message="DB does not exist. Add create_if_not_exists=True?"):
+        self.message = message
+        super().__init__(self.message)
 
 class MissingConfigurationException(Exception):
     
     def __init__(self, message="No configuration given, cannot start."):
         self.message = message
         super().__init__(self.message)
 
@@ -43,21 +47,14 @@
         self.code = code
         super().__init__(self.id, self.name, self.hint, self.message)
 
     def to_dict(self):
         dict = {'code':self.code , 'name':self.name, 'hint':self.hint, 'message':self.message, 'id':self.id}
         return dict
 
-    def make_error(self, format='json'):
-        if format == 'json':
-            return self.to_json(), self.code
-
-    def to_json(self):
-        return jsonify(self.to_dict())
-
 class DuplicateUserKeyError(HTTPError):
     """ Error to be sent when a duplicate user key is sent for insertion """
 
     def __init__(self) -> None:
         self.id = 'user_create_duplicateKey'
         self.name = 'Duplicate user key'
         self.hint = 'Check for unique key restrictions'
```

### Comparing `d20-orm-1.0.1a7/src/dtwentyORM/GraphClassFactory.py` & `d20-orm-2.0.0a2/src/dtwentyORM/GraphClassFactory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-from pyArango.connection import *
-from pyArango.collection import *
-from pyArango.graph import *
-from dtwentyORM import Metadata, Element
-from .Error import *
-import pyArango
-import os
-import json
-
-
-
-class ClassFactory():
-
-
-    class paymentsgraph(pyArango.graph.Graph):
-        _edgeDefinitions = (pyArango.graph.EdgeDefinition ('PaysWith',
-                                        fromCollections = ['Users'],
-                                        toCollections = ['PaymentMethods']),
-                            pyArango.graph.EdgeDefinition ('PaidBy',
-                                        fromCollections = ['Charges'],
-                                        toCollections = ['PaymentMethods']),
-                            pyArango.graph.EdgeDefinition ('Settled',
-                                        fromCollections = ['Charges'],
-                                        toCollections = ['Payments']),
-                            pyArango.graph.EdgeDefinition ('Checkout',
-                                        fromCollections = ['Orders'],
-                                        toCollections = ['Payments']),
-        )
-        _orphanedCollections = []
-
-
-
-
-
-    def __init__(self, graphname, collections = [], edges = [], orphans = [], edgeDefinitions=(), prefix='', conf=None):
-        if type(conf) != dict and os.environ.get(f'{prefix}_CONF') != None:
-            conf = json.loads(os.environ.get(f'{prefix}_CONF'))
-            arangoURL=conf.get(f'{prefix}_DBURL')
-            username=conf.get(f'{prefix}_DBUSERNAME')
-            password=conf.get(f'{prefix}_DBPASSWORD')
-            self.db_name=conf.get(f'{prefix}_DBNAME')        
-        else:
-            raise MissingConfigurationException
-        arangoURL=conf.get(f'{prefix}_DBURL')
-        username=conf.get(f'{prefix}_DBUSERNAME')
-        password=conf.get(f'{prefix}_DBPASSWORD')
-        self.db_name=conf.get(f'{prefix}_DBNAME')
-
-        self.db_client = Connection(arangoURL=arangoURL, username=username, password=password, verify=True, verbose=True, statsdClient=None, reportFileName=None, loadBalancing='round-robin', use_grequests=False, use_jwt_authentication=False, use_lock_for_reseting_jwt=True, max_retries=10)
-
-        db_collections = collections
-        db_edges = edges
-        db_orphans = orphans
-        db_edgeDefinitions = edgeDefinitions
-
-        globals()[graphname] = type(graphname, (pyArango.graph.Graph,), {"_edgeDefinitions" : tuple(db_edgeDefinitions), "_orphanedCollections" : db_orphans })
-
-        for cl in db_collections:
-            globals()[cl] = type(cl, (Collection,), {"_fields" : {}})
-
-        for cl in db_edges:
-            globals()[cl] = type(cl, (Edges,), {"_fields" : {}})
-
-        if not self.db_client.hasDatabase(self.db_name):
-            self.db = self.db_client.createDatabase(self.db_name)
-        else:
-            self.db = self.db_client[self.db_name]
-        for col in db_collections:
-            if not self.db.hasCollection(col):
-                self.db.createCollection(className='Collection', name=col)
-        for col in db_edges:
-            if not self.db.hasCollection(col):
-                self.db.createCollection(className='Edges', name=col)
-        if not self.db.hasGraph(graphname):
-            self.db.createGraph(graphname)
-
-
-
-
+import pyArango
+from pyArango.connection import *
+from pyArango.collection import *
+from pyArango.graph import *
+from .Error import *
+from .DBConnector import DBConnector
+
+
+class ClassFactory():
+
+    def __init__(self, graphname, db_name, collections = [], edgeDefinitions={}, conf=None):
+        '''
+            Initialiazes graph and elements. If Database is not in server, creates it. If collections or edges are added, creates them. Edges with no definition are ignored
+
+            graphname - Name of graph to use or create
+            db_name - Name of database to use or create
+            collections - List of collection names
+            edgeDefinitions - dictionary with the structure {edgeName: { fromCollections : list, toCollections: list }}
+            prefix - Added before db name
+            conf - dictionary to override os.eviron, required keys: DBURL, DBUSERNAME, DBPASSWORD
+
+            If from/toCollections contain collections not in collections list, adds them as collections
+
+        '''
+        
+        self.db_connector = DBConnector(db_name, conf=conf, create_if_not_exists=True)
+        # Create edgeDefinitions tuple from parameter dictionary
+        db_edgeDefinitions = tuple([pyArango.graph.EdgeDefinition (edge,fromCollections = edgeDefinitions[edge]['fromCollections'],toCollections = edgeDefinitions[edge]['toCollections']) for edge in edgeDefinitions])
+
+        # Determine all collections connected in the edgeDefinitions
+        db_connected = []
+        db_edges = [edge for edge in edgeDefinitions]
+        for edge in edgeDefinitions:
+            for colFrom in edgeDefinitions[edge]['fromCollections']:
+                if colFrom not in db_connected:
+                    db_connected.append(colFrom)
+            for colTo in edgeDefinitions[edge]['toCollections']:
+                if colTo not in db_connected:
+                    db_connected.append(colTo)
+        # Collections given and not connected are orphans
+        db_orphans = [collection for collection in collections if collection not in db_connected]
+
+        # All connected collections need to be created
+        db_collections = collections
+        db_collections.extend(db_connected)
+        db_collections = list(set(db_collections))
+
+        # Create graph class for instancing
+        if len(db_edgeDefinitions) > 0 and graphname != '':
+            globals()[graphname] = type(graphname, (pyArango.graph.Graph,), {"_edgeDefinitions" : db_edgeDefinitions, "_orphanedCollections" : db_orphans })
+
+        # Create each collection and edge class for instancing
+        for cl in db_collections:
+            globals()[cl] = type(cl, (Collection,), {"_fields" : {}})
+        for cl in db_edges:
+            globals()[cl] = type(cl, (Edges,), {"_fields" : {}})
+
+        # Look for collections, edges and graph and reference or create
+        for col in db_collections:
+            if not self.db_connector.db.hasCollection(col):
+                self.db_connector.db.createCollection(className='Collection', name=col)
+        for col in db_edges:
+            if not self.db_connector.db.hasCollection(col):
+                self.db_connector.db.createCollection(className='Edges', name=col)
+        if not self.db_connector.db.hasGraph(graphname) and len(db_edgeDefinitions) > 0 and graphname != '':
+            self.db_connector.db.createGraph(graphname)
+
+        self.graphname = graphname
+        self.collections = db_collections
+        self.edges = db_edges
+        self.edgeDefinitions = edgeDefinitions
+
+    def __str__(self):
+        desc = f'Graph Class for {self.db_connector.db_name}'
+        return desc
+
+    
+
```

### Comparing `d20-orm-1.0.1a7/src/dtwentyORM/support.py` & `d20-orm-2.0.0a2/src/dtwentyORM/support.py`

 * *Files identical despite different names*

