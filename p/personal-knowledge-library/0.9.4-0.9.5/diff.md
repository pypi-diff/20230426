# Comparing `tmp/personal_knowledge_library-0.9.4.tar.gz` & `tmp/personal_knowledge_library-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-0.9.4.tar", last modified: Fri Mar 24 09:04:46 2023, max compression
+gzip compressed data, was "personal_knowledge_library-0.9.5.tar", last modified: Wed Apr 26 14:53:20 2023, max compression
```

## Comparing `personal_knowledge_library-0.9.4.tar` & `personal_knowledge_library-0.9.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.032056 personal_knowledge_library-0.9.4/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.032056 personal_knowledge_library-0.9.4/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    51156 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.032056 personal_knowledge_library-0.9.4/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)   312127 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26750 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    48427 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    28407 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-03-24 09:04:45.000000 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-24 09:04:45.000000 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 09:04:45.000000 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 09:04:45.000000 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-24 09:04:45.000000 personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 09:04:46.036056 personal_knowledge_library-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-24 09:04:30.000000 personal_knowledge_library-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55252 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   312127 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26750 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51751 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28407 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 14:53:20.530277 personal_knowledge_library-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/setup.py
```

### Comparing `personal_knowledge_library-0.9.4/LICENSE` & `personal_knowledge_library-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/PKG-INFO` & `personal_knowledge_library-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 0.9.4
+Version: 0.9.5
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Description: # Wacom Personal Knowledge Library
```

### Comparing `personal_knowledge_library-0.9.4/README.md` & `personal_knowledge_library-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/__init__.py` & `personal_knowledge_library-0.9.5/knowledge/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
+# Copyright © 2021-23 Wacom. All rights reserved.
 """"Personal knowledge Library"""
 import logging
 from typing import Optional
 
 __author__ = "Markus Weber"
-__copyright__ = "Copyright 2021 Wacom. All rights reserved."
+__copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
+__version__ = "0.9.5"
 
 # Create the Logger
 logger: Optional[logging.Logger] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
@@ -29,9 +30,9 @@
 
 from knowledge import base
 from knowledge import nel
 from knowledge import public
 from knowledge import services
 from knowledge import utils
 
-__all__ = ['__copyright__', '__credits__', '__license__', '__maintainer__', '__email__', '__status__',
+__all__ = ['__copyright__', '__credits__', '__license__', '__maintainer__', '__email__', '__status__', '__version__',
            'logger', 'base', 'nel', 'public', 'services', 'utils']
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/base/access.py` & `personal_knowledge_library-0.9.5/knowledge/base/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
+# Copyright © 2021-23 Wacom. All rights reserved.
 from typing import List
 
 
 class AccessRight(object):
     """
     Access rights for entities within a tenant.
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/base/entity.py` & `personal_knowledge_library-0.9.5/knowledge/base/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 OWNER_ID_TAG: str = 'ownerId'
 GROUP_IDS: str = 'groupIds'
 LOCALIZED_CONTENT_TAG: str = 'LocalizedContent'
 STATUS_FLAG_TAG: str = 'status'
 CONTENT_TAG: str = 'value'
 URI_TAG: str = 'uri'
 URIS_TAG: str = 'uris'
+FORCE_TAG: str = 'force'
 ERRORS_TAG: str = 'errors'
 TEXT_TAG: str = 'text'
 TYPE_TAG: str = 'type'
 IMAGE_TAG: str = 'image'
 DESCRIPTION_TAG: str = 'description'
 COMMENT_TAG: str = 'text'
 COMMENTS_TAG: str = 'comments'
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/base/ontology.py` & `personal_knowledge_library-0.9.5/knowledge/base/ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 # ---------------------------------------------- Vocabulary base URI ---------------------------------------------------
 PREFIX: str = "xsd"
 BASE_URI: str = "http://www.w3.org/2001/XMLSchema#"
 # ---------------------------------------------------- Constants -------------------------------------------------------
 SUB_CLASS_OF_TAG: str = 'subClassOf'
 TENANT_ID: str = 'tenantId'
 NAME_TAG: str = "name"
-SUPPORTED_LANGUAGES: List[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'zh_CN']
-
+SUPPORTED_LOCALES: List[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'zh_CN']
+SUPPORTED_LANGUAGES: List[str] = ['ja', 'en', 'de', 'bg', 'fr', 'it', 'es', 'zh']
+LANGUAGE_LOCALE_MAPPING: Dict[str, str] = dict([(lang, locale)
+                                                for lang, locale in zip(SUPPORTED_LANGUAGES, SUPPORTED_LOCALES)])
 
 class PropertyType(enum.Enum):
     """
     PropertyType
     -----------
     Within the ontology two different property types are defined. A data- and an object property.
     """
@@ -1154,14 +1156,32 @@
         """Relations of the concept."""
         return self.__object_properties
 
     @object_properties.setter
     def object_properties(self, relations: Dict[OntologyPropertyReference, ObjectProperty]):
         self.__object_properties = relations
 
+    def data_property_lang(self, property: OntologyPropertyReference, language_code: LanguageCode) \
+            -> List[DataProperty]:
+        """
+        Get data property for language_code code.
+
+        Parameters
+        ----------
+        property: OntologyPropertyReference
+            Data property.
+        language_code: LanguageCode
+            Requested language_code code
+        Returns
+        -------
+        data_properties: List[DataProperty]
+            Returns a list of data properties for a specific language code
+        """
+        return [d for d in self.data_properties.get(property, []) if d.language_code == language_code]
+
     @property
     def alias(self) -> List[Label]:
         """Alternative labels of the concept."""
         return self.__alias
 
     @alias.setter
     def alias(self, alias: List[Label]):
@@ -1276,15 +1296,15 @@
     @staticmethod
     def from_dict(entity: Dict[str, Any]) -> 'ThingObject':
         labels: List[Label] = []
         alias: List[Label] = []
         descriptions: List[Description] = []
 
         for label in entity[LABELS_TAG]:
-            if label[LOCALE_TAG] in SUPPORTED_LANGUAGES:
+            if label[LOCALE_TAG] in SUPPORTED_LOCALES:
                 if label[IS_MAIN_TAG]:
                     labels.append(Label.create_from_dict(label))
                 else:
                     alias.append(Label.create_from_dict(label))
 
         for desc in entity[DESCRIPTIONS_TAG]:
             descriptions.append(Description.create_from_dict(desc))
@@ -1320,14 +1340,73 @@
                 thing.add_relation(obj)
         thing.alias = alias
         # Finally, retrieve rights
         if TENANT_RIGHTS_TAG in entity:
             thing.tenant_access_right = TenantAccessRight.parse(entity[TENANT_RIGHTS_TAG])
         return thing
 
+    def __getstate__(self) -> Dict[str, Any]:
+        return self.__dict__()
+
+    def __setstate__(self, state: Dict[str, Any]):
+        self.__label: List[Label] = []
+        self.__description: List[Description] = []
+        self.__alias: List[Label] = []
+        self.__data_properties: Dict[OntologyPropertyReference, List[DataProperty]] = {}
+        self.__object_properties: Dict[OntologyPropertyReference, ObjectProperty] = {}
+        self.__status_flag: EntityStatus = EntityStatus.UNKNOWN
+        self.__ontology_types: Optional[Set[str]] = None
+        self.__owner_id: Optional[str] = None
+        self.__group_ids: List[str] = []
+        self.__visibility: Optional[str] = None
+
+        for label in state[LABELS_TAG]:
+            if label[LOCALE_TAG] in SUPPORTED_LOCALES:
+                if label[IS_MAIN_TAG]:
+                    self.__label.append(Label.create_from_dict(label))
+                else:
+                    self.__alias.append(Label.create_from_dict(label))
+
+        for desc in state[DESCRIPTIONS_TAG]:
+            self.__description.append(Description.create_from_dict(desc))
+
+        use_nel: bool = state.get(USE_NEL_TAG, True)
+        visibility: Optional[str] = state.get(VISIBILITY_TAG)
+        self.__icon=state[IMAGE_TAG]
+        self.__uri=state[URI_TAG]
+        self.__concept_type=OntologyClassReference.parse(state[TYPE_TAG])
+        self.__owner=state.get(OWNER_TAG, True)
+        self.__use_for_nel=use_nel
+        self.__visibility = visibility
+        self.__owner_id = state.get(OWNER_ID_TAG)
+        self.__group_ids = state.get(GROUP_IDS)
+        if DATA_PROPERTIES_TAG in state:
+            if isinstance(state[DATA_PROPERTIES_TAG], dict):
+                for data_property_type_str, data_properties in state[DATA_PROPERTIES_TAG].items():
+                    data_property_type: OntologyPropertyReference = \
+                        OntologyPropertyReference.parse(data_property_type_str)
+                    for data_property in data_properties:
+                        language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
+                        value: str = data_property[VALUE_TAG]
+                        self.add_data_property(DataProperty(value, data_property_type, language_code))
+            elif isinstance(state[DATA_PROPERTIES_TAG], list):
+                for data_property in state[DATA_PROPERTIES_TAG]:
+                    language_code: LanguageCode = LanguageCode(data_property[LOCALE_TAG])
+                    value: str = data_property[VALUE_TAG]
+                    data_property_type: OntologyPropertyReference = \
+                        OntologyPropertyReference.parse(data_property[DATA_PROPERTY_TAG])
+                    self.add_data_property(DataProperty(value, data_property_type, language_code))
+        if OBJECT_PROPERTIES_TAG in state:
+            for object_property in state[OBJECT_PROPERTIES_TAG].values():
+                prop, obj = ObjectProperty.create_from_dict(object_property)
+                self.add_relation(obj)
+        # Finally, retrieve rights
+        if TENANT_RIGHTS_TAG in state:
+            self.tenant_access_right = TenantAccessRight.parse(state[TENANT_RIGHTS_TAG])
+
     def __hash__(self):
         return 0
 
     def __eq__(self, other):
         # another object is equal to self, iff
         # it is an instance of MyClass
         return isinstance(other, ThingObject) and other.uri == self.uri
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/nel/base.py` & `personal_knowledge_library-0.9.5/knowledge/nel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
+# Copyright © 2021-23 Wacom. All rights reserved.
 import abc
 from enum import Enum
 from typing import List, Optional
 
 from knowledge.base.entity import LanguageCode
 from knowledge.base.ontology import THING_CLASS, OntologyClassReference
 from knowledge.services.base import WacomServiceAPIClient, RESTAPIClient
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/public/__init__.py` & `personal_knowledge_library-0.9.5/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/public/wikidata.py` & `personal_knowledge_library-0.9.5/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/base.py` & `personal_knowledge_library-0.9.5/knowledge/services/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,20 +123,22 @@
             try:
                 response_token: Dict[str, str] = response.json()
                 try:
                     date_object: datetime = parse(response_token['expirationDate'])
                 except (ParserError, OverflowError) as _:
                     date_object: datetime = datetime.now()
                 return response_token['accessToken'], response_token['refreshToken'], date_object
-            except:
-                return response.text, '', datetime.now()
+            except Exception as e:
+                raise WacomServiceException(f'Login failed'
+                                            f'Response code:={response.status_code}, response text:= {response.text}, '
+                                            f'exception:= {e} ')
         raise WacomServiceException(f'User login failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def refresh_token(self, refresh_token: str) -> Tuple[str, str, str]:
+    def refresh_token(self, refresh_token: str) -> Tuple[str, str, datetime]:
         """
         Refreshing a token.
 
         Parameters
         ----------
         refresh_token: str
             Refresh token
@@ -162,15 +164,19 @@
         }
         payload: Dict[str, str] = {
             REFRESH_TOKEN_TAG: refresh_token
         }
         response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
         if response.ok:
             response_token: Dict[str, str] = response.json()
-            return response_token['accessToken'], response_token['refreshToken'], response_token['expirationDate']
+            try:
+                date_object: datetime = parse(response_token['expirationDate'])
+            except (ParserError, OverflowError) as _:
+                date_object: datetime = datetime.now()
+            return response_token['accessToken'], response_token['refreshToken'], date_object
         raise WacomServiceException(f'Refresh failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     @staticmethod
     def unpack_token(auth_token: str) -> Dict[str, Any]:
         return jwt.decode(auth_token, options={"verify_signature": False})
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/graph.py` & `personal_knowledge_library-0.9.5/knowledge/services/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import os
 import urllib
 from pathlib import Path
 from typing import List, Dict, Any, Tuple, Optional
 
 import requests
 from requests import Response
+from requests.adapters import HTTPAdapter
+from urllib3 import Retry
 
 from knowledge.base.access import TenantAccessRight
 from knowledge.base.entity import LanguageCode, DATA_PROPERTIES_TAG, DATA_PROPERTY_TAG, VALUE_TAG, IMAGE_TAG, \
     DESCRIPTION_TAG, TYPE_TAG, URI_TAG, LABELS_TAG, IS_MAIN_TAG, DESCRIPTIONS_TAG, RELATIONS_TAG, SEND_TO_NEL_TAG, \
-    LOCALE_TAG, EntityStatus, Label, Description, URIS_TAG
+    LOCALE_TAG, EntityStatus, Label, Description, URIS_TAG, FORCE_TAG
 from knowledge.base.ontology import DataProperty, OntologyPropertyReference, ThingObject, OntologyClassReference, \
     ObjectProperty
 from knowledge.services import USER_AGENT_STR
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException, AUTHORIZATION_HEADER_FLAG, \
     USER_AGENT_HEADER_FLAG, CONTENT_TYPE_HEADER_FLAG
 
 
@@ -184,26 +186,32 @@
                 thing.tenant_access_right = TenantAccessRight.parse(e[TENANT_RIGHTS_TAG])
             else:
                 thing.tenant_access_right = TenantAccessRight()
             return thing
         raise WacomServiceException(f'Retrieving of entity content failed. URI:={uri}. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def delete_entities(self, auth_key: str, uris: List[str], force: bool = False):
+    def delete_entities(self, auth_key: str, uris: List[str], force: bool = False, max_retries: int = 3,
+                        backoff_factor: float = 0.1):
         """
         Delete a list of entities.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         uris: List[str]
             List of URI of entities. **Remark:** More than 100 entities are not possible in one request
         force: bool
             Force deletion process
+        max_retries: int
+            Maximum number of retries
+        backoff_factor: float
+            A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
+            second try without a delay)
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         if len(uris) > 100:
@@ -211,50 +219,68 @@
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}'
         headers: Dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: Dict[str, Any] = {
             URIS_TAG: uris,
-            'forceDelete': force
+            FORCE_TAG: force
         }
-        response: Response = requests.delete(url, headers=headers, params=params, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Deletion of entity failed.'
-                                        f'Response code:={response.status_code}, exception:= {response.content}')
+        mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(total=max_retries,
+                                   backoff_factor=backoff_factor,
+                                   status_forcelist=[502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.delete(url, headers=headers, params=params, verify=self.verify_calls)
+            if not response.ok:
+                raise WacomServiceException(f'Deletion of entities failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def delete_entity(self, auth_key: str, uri: str, force: bool = False):
+    def delete_entity(self, auth_key: str, uri: str, force: bool = False, max_retries: int = 3,
+                      backoff_factor: float = 0.1):
         """
         Deletes an entity.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         uri: str
             URI of entity
         force: bool
             Force deletion process
+        max_retries: int
+            Maximum number of retries
+        backoff_factor: float
+            A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
+            second try without a delay)
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{uri}'
         headers: Dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.delete(url, headers=headers, params={'forceDelete': force},
-                                             verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException('Deletion of entity failed. Response code:={}, exception:= {}'
-                                        .format(response.status_code,
-                                                response.content))
+        mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(total=max_retries,
+                                   backoff_factor=backoff_factor,
+                                   status_forcelist=[502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.delete(url, headers=headers, params={FORCE_TAG: force},
+                                                verify=self.verify_calls)
+            if not response.ok:
+                raise WacomServiceException(f'Deletion of entity (URI:={uri}) failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.content}')
+
 
     def exists(self, auth_key: str, uri: str) -> bool:
         """
         Check if entity exists in knowledge graph.
 
         Parameters
         ----------
@@ -374,58 +400,69 @@
                 for idx, uri in enumerate(response_dict[URIS_TAG]):
                     if entities[bulk_idx + idx].image is not None and entities[bulk_idx + idx].image != '':
                         self.set_entity_image_url(auth_key, uri, entities[bulk_idx + idx].image)
                     entities[bulk_idx + idx].uri = response_dict[URIS_TAG][idx]
 
         return entities
 
-    def create_entity(self, auth_key: str, entity: ThingObject) -> str:
+    def create_entity(self, auth_key: str, entity: ThingObject, max_retries: int = 3, backoff_factor: float = 0.1,
+                      ignore_image: bool = False) \
+            -> str:
         """
         Creates entity in graph.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
         entity: ThingObject
-            entity object
+            Entity object that needs to be created
+        max_retries: int
+            Maximum number of retries
+        backoff_factor: float
+            A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
+            second try without a delay)
 
         Returns
         -------
         uri: str
             URI of entity
 
+
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}'
-
         # Header info
-        headers: dict = {
+        headers: Dict[str, str] = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             CONTENT_TYPE_HEADER_FLAG: APPLICATION_JSON_HEADER,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         payload: Dict[str, Any] = WacomKnowledgeService.__entity__(entity)
-        try:
-            response: Response = requests.post(url, json=payload, headers=headers, verify=self.verify_calls, timeout=5)
-        except Exception as e:
-            raise WacomServiceException(f"Timeout after 5 sec. [Exception:={str(e)}]")
-        if response.ok:
-            uri: str = response.json()[URI_TAG]
-            if entity.image is not None and entity.image.startswith('file:'):
-                from urllib.parse import urlparse
-
-                p = urlparse(entity.image)
-                self.set_entity_image_local(auth_key, uri, Path(p.path))
-            elif entity.image is not None and entity.image != '':
-                self.set_entity_image_url(auth_key, uri, entity.image)
-            return uri
+        mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(total=max_retries,
+                                   backoff_factor=backoff_factor,
+                                   status_forcelist=[502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.post(url, json=payload, headers=headers, verify=self.verify_calls, timeout=5)
+
+            if response.ok and not ignore_image:
+                uri: str = response.json()[URI_TAG]
+                # Set image
+                if entity.image is not None and entity.image.startswith('file:'):
+                    from urllib.parse import urlparse
+                    p = urlparse(entity.image)
+                    self.set_entity_image_local(auth_key, uri, Path(p.path))
+                elif entity.image is not None and entity.image != '':
+                    self.set_entity_image_url(auth_key, uri, entity.image)
+                return uri
         raise WacomServiceException(f'Pushing entity failed. '
                                     f'Response code:={response.status_code}, exception:= {response.content}. '
                                     f'Payload: \n{json.dumps(payload, indent=4)}')
 
     def update_entity(self, auth_key: str, entity: ThingObject):
         """
         Updates entity in graph.
@@ -649,15 +686,21 @@
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: dict = {
             RELATION_TAG: relation.iri,
             TARGET: target
         }
-        response: Response = requests.post(url, params=params, headers=headers, verify=self.verify_calls)
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        session: requests.Session = requests.Session()
+        retries: Retry = Retry(backoff_factor=0.1,
+                               status_forcelist=[500, 502, 503, 504])
+        session.mount(mount_point, HTTPAdapter(max_retries=retries))
+        response: Response = session.post(url, params=params, headers=headers, verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Create relations failed. '
                                         f'Response code:={response.status_code}, exception:= {response.content}. '
                                         f'URL: {url}'
                                         f'Parameters: \n{json.dumps(params, indent=4)}')
 
     def remove_relation(self, auth_key: str, source: str, relation: OntologyPropertyReference, target: str):
@@ -745,15 +788,15 @@
                     things[r[SUBJECT]].add_relation(ObjectProperty(relation, outgoing=[r[OBJECT]]))
             return things, relations
         raise WacomServiceException(f'Activation failed, uris:= {uris} activation:={depth}). '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def listing(self, auth_key: str, filter_type: OntologyClassReference, page_id: Optional[str] = None,
                 limit: int = 30, locale: Optional[LanguageCode] = None, visibility: Optional[Visibility] = None,
-                estimate_count: bool = False) \
+                estimate_count: bool = False, max_retries: int = 3, backoff_factor: float = 0.1) \
             -> Tuple[List[ThingObject], int, str]:
         """
         List all entities visible to users.
 
         Parameters
         ----------
         auth_key: str
@@ -766,14 +809,20 @@
             Limit of the returned entities.
         locale: Optional[LanguageCode] [default:=None]
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., en_US.
         visibility: Optional[Visibility] [default:=None]
             Filter the entities based on its visibilities
         estimate_count: bool [default:=False]
             Request an estimate of the entities in a tenant.
+        max_retries: int
+            Maximum number of retries
+        backoff_factor: float
+            A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
+            second try without a delay)
+
         Returns
         -------
         entities: List[ThingObject]
             List of entities
         estimated_total_number: int
             Number of all entities
         next_page_id: str
@@ -799,14 +848,20 @@
         if locale:
             parameters[LOCALE_TAG] = locale
         if visibility:
             parameters[VISIBILITY_TAG] = str(visibility.value)
         # If filtering is configured
         if page_id is not None:
             parameters[NEXT_PAGE_ID_TAG] = page_id
+        mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(total=max_retries,
+                                   backoff_factor=backoff_factor,
+                                   status_forcelist=[502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
         # Send request
         response: Response = requests.get(url, params=parameters, headers=headers, verify=self.verify_calls)
         # If response is successful
         if response.ok:
             entities_resp: dict = response.json()
             next_page_id: str = entities_resp[NEXT_PAGE_ID_TAG]
             estimated_total_number: int = entities_resp.get(TOTAL_COUNT, 0)
@@ -1166,16 +1221,16 @@
         ------
         WacomServiceException
             If the graph service returns an error code.
         """
         with requests.session() as session:
             headers: Dict[str, str] = {
                 USER_AGENT_HEADER_FLAG:
-                    'ImageFetcher/0.1 (https://github.com/Wacom-Developer/personal-knowledge-library)'
-                    ' personal-knowledge-library/0.2.4'
+                    f'ImageFetcher/0.1 (https://github.com/Wacom-Developer/personal-knowledge-library)'
+                    f' personal-knowledge-library/0.9.5'
             }
             response: Response = session.get(image_url, headers=headers)
             if response.ok:
                 image_bytes: bytes = response.content
                 file_name: str = image_url if file_name is None else file_name
                 if mime_type is None:
                     _, file_extension = os.path.splitext(file_name.lower())
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/group.py` & `personal_knowledge_library-0.9.5/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/ontology.py` & `personal_knowledge_library-0.9.5/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/tenant.py` & `personal_knowledge_library-0.9.5/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/knowledge/services/users.py` & `personal_knowledge_library-0.9.5/knowledge/services/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 USER_ID_TAG: str = 'userId'
 LIMIT_TAG: str = 'limit'
 OFFSET_TAG: str = 'offset'
 ROLES_TAG: str = 'roles'
 META_DATA_TAG: str = 'metaData'
 INTERNAL_USER_ID_TAG: str = 'internalUserId'
 EXTERNAL_USER_ID_TAG: str = 'externalUserId'
+FORCE_TAG: str = 'force'
 CONTENT_TYPE_FLAG: str = 'Content-Type'
 TENANT_API_KEY_FLAG: str = 'x-tenant-api-key'
 USER_AGENT_TAG: str = "User-Agent"
 
 
 class UserRole(enum.Enum):
     """
@@ -128,15 +129,15 @@
     service_endpoint: str
         Base endpoint
     """
 
     USER_DETAILS_ENDPOINT: str = f'{WacomServiceAPIClient.USER_ENDPOINT}/internal-id'
 
     def __init__(self, service_url: str = WacomServiceAPIClient.SERVICE_URL, service_endpoint: str = 'graph/v1'):
-        super().__init__("GroupManagementServiceAPI", service_url=service_url, service_endpoint=service_endpoint)
+        super().__init__("UserManagementServiceAPI", service_url=service_url, service_endpoint=service_endpoint)
 
     # ------------------------------------------ Users handling --------------------------------------------------------
 
     def create_user(self, tenant_key: str, external_id: str, meta_data: Dict[str, str] = None,
                     roles: List[UserRole] = None) -> Tuple[User, str, str, datetime]:
         """
         Creates user for a tenant.
@@ -229,39 +230,42 @@
             EXTERNAL_USER_ID_TAG: external_id
         }
         response: Response = requests.patch(url, headers=headers, json=payload, params=params, verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Updating user failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def delete_user(self, tenant_key: str, external_id: str, internal_id: str):
+    def delete_user(self, tenant_key: str, external_id: str, internal_id: str, force: bool = False):
         """Deletes user from tenant.
 
         Parameters
         ----------
         tenant_key: str
             API key for tenant
         external_id: str
             External id of user identification service.
         internal_id: str
             Internal id of user.
+        force: bool
+            If set to true removes all user data including groups and entities.
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{UserManagementServiceAPI.USER_ENDPOINT}'
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             TENANT_API_KEY_FLAG: tenant_key
         }
         params: Dict[str, str] = {
             USER_ID_TAG: internal_id,
-            EXTERNAL_USER_ID_TAG: external_id
+            EXTERNAL_USER_ID_TAG: external_id,
+            FORCE_TAG: force
         }
         response: Response = requests.delete(url, headers=headers, params=params, verify=self.verify_calls)
         if not response.ok:
             raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def user_internal_id(self, tenant_key: str, external_id: str) -> str:
         """User internal id.
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/utils/rdf.py` & `personal_knowledge_library-0.9.5/knowledge/utils/rdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2022 Wacom Authors. All Rights Reserved.
+# Copyright © 2022-23 Wacom Authors. All Rights Reserved.
 from typing import Optional, List
 
 from rdflib import Graph, RDF, RDFS, OWL, URIRef, Literal
 
 from knowledge.base.entity import Comment, LanguageCode, OntologyLabel
 from knowledge.base.ontology import Ontology, OntologyClass, OntologyClassReference, OntologyPropertyReference, \
     OntologyProperty, PropertyType, INVERSE_DATA_PROPERTY_TYPE_MAPPING, DataPropertyType
```

### Comparing `personal_knowledge_library-0.9.4/knowledge/utils/wikipedia.py` & `personal_knowledge_library-0.9.5/knowledge/utils/wikipedia.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021 Wacom. All rights reserved.
+# Copyright © 2021-23 Wacom. All rights reserved.
 from http import HTTPStatus
 from typing import Dict, Any
 
 import requests
 from requests import Response
 
 from knowledge import logger
 from knowledge.base.entity import LanguageCode
 
 
 class ExtractionException(Exception):
+    """
+    Exception for extraction errors.
+    """
     pass
 
 
 def __extract_abstract__(title: str, language: str = 'en') -> str:
     """Extracting an abstract.
 
     Parameters
```

### Comparing `personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 0.9.4
+Version: 0.9.5
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Description: # Wacom Personal Knowledge Library
```

### Comparing `personal_knowledge_library-0.9.4/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.4/setup.py` & `personal_knowledge_library-0.9.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```

