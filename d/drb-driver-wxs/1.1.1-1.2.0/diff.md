# Comparing `tmp/drb-driver-wxs-1.1.1.tar.gz` & `tmp/drb-driver-wxs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-wxs-1.1.1.tar", last modified: Wed Dec 21 14:10:10 2022, max compression
+gzip compressed data, was "drb-driver-wxs-1.2.0.tar", last modified: Tue Apr 25 17:30:33 2023, max compression
```

## Comparing `drb-driver-wxs-1.1.1.tar` & `drb-driver-wxs-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 10:49:06.000000 drb-driver-wxs-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3705 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3246 2022-12-21 13:24:02.000000 drb-driver-wxs-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.560943 drb-driver-wxs-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.560943 drb-driver-wxs-1.1.1/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/drb/drivers/wxs/
--rw-rw-rw-   0 root         (0) root         (0)      265 2022-12-21 10:49:07.000000 drb-driver-wxs-1.1.1/drb/drivers/wxs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/drb/drivers/wxs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9743 2022-12-21 10:49:07.000000 drb-driver-wxs-1.1.1/drb/drivers/wxs/wXs_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.564943 drb-driver-wxs-1.1.1/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 10:49:07.000000 drb-driver-wxs-1.1.1/drb/exceptions/wxs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3705 2022-12-21 14:10:10.000000 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      366 2022-12-21 14:10:10.000000 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-21 14:10:10.000000 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2022-12-21 14:10:10.000000 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-21 14:10:10.000000 drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-12-21 13:24:02.000000 drb-driver-wxs-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-12-21 14:10:10.568944 drb-driver-wxs-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      921 2022-12-21 14:03:50.000000 drb-driver-wxs-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-06-28 08:40:45.000000 drb-driver-wxs-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.604760 drb-driver-wxs-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:27:24.000000 drb-driver-wxs-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-21 10:49:06.000000 drb-driver-wxs-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-04-25 17:30:33.604760 drb-driver-wxs-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2022-12-21 13:24:02.000000 drb-driver-wxs-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.592760 drb-driver-wxs-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.588760 drb-driver-wxs-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.608760 drb-driver-wxs-1.2.0/drb/drivers/wxs/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2022-12-21 10:49:07.000000 drb-driver-wxs-1.2.0/drb/drivers/wxs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-25 17:30:33.608760 drb-driver-wxs-1.2.0/drb/drivers/wxs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8651 2023-04-25 15:47:28.000000 drb-driver-wxs-1.2.0/drb/drivers/wxs/wXs_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.600760 drb-driver-wxs-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2022-12-21 10:49:07.000000 drb-driver-wxs-1.2.0/drb/exceptions/wxs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.604760 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-25 17:30:33.000000 drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-21 12:15:44.000000 drb-driver-wxs-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-21 12:15:44.000000 drb-driver-wxs-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-04-25 17:30:33.608760 drb-driver-wxs-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-21 12:15:44.000000 drb-driver-wxs-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:30:33.604760 drb-driver-wxs-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    18118 2023-04-25 15:47:28.000000 drb-driver-wxs-1.2.0/tests/test_wXs.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-06-28 08:40:45.000000 drb-driver-wxs-1.2.0/versioneer.py
```

### Comparing `drb-driver-wxs-1.1.1/PKG-INFO` & `drb-driver-wxs-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wxs
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB WXS OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wXs
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wXs
+Project-URL: Source, https://gitlab.com/drb-python/impl/wXs
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WXS driver
 
 This drb-driver-wxs module implements the OWS services (WFS, WMS, WCS, ...).
 For more information about OWS Service see https://www.ogc.org/ or/and
 https://www.ogc.org/standards/wms
 OGC catalog, this driver is abstract, it means that to have a usable
@@ -122,9 +123,7 @@
 # FORMAT=GEOTIFF_INT16&
 # SUBSET=X(-1784000%2C-1140000)&SUBSET=Y(1356000%2C1863000)&
 # SUBSETTINGCRS=http%3A%2F%2Fwww.opengis.net%2Fdef%2Fcrs%2FEPSG%2F0%2F152160&
 # OUTPUTCRS=http%3A%2F%2Fwww.opengis.net%2Fdef%2Fcrs%2FEPSG%2F0%2F152160
 # => return the image
 
 ```
-
-
```

### Comparing `drb-driver-wxs-1.1.1/README.md` & `drb-driver-wxs-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-wxs-1.1.1/drb/drivers/wxs/wXs_node.py` & `drb-driver-wxs-1.2.0/drb/drivers/wxs/wXs_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import abc
 import io
 
-from drb.utils.keyringconnection import kr_get_auth, kr_check
+import keyring
+from deprecated.classic import deprecated
 from drb.exceptions.core import DrbException, DrbNotImplementationException, \
     DrbFactoryException
 
 from defusedxml import ElementTree
 
 from drb.core import DrbNode
 from drb.nodes.abstract_node import AbstractNode
 from drb.core.path import ParsedPath
-from requests.auth import AuthBase
-from typing import Any, Dict, List, Optional, Tuple
+from requests.auth import AuthBase, HTTPBasicAuth
+from typing import Any, List, Optional
 
 from drb.topics.resolver import create
 from drb.drivers.http import DrbHttpNode
 from drb.drivers.xml import XmlNode
 
 
 class WXSServiceNode(AbstractNode, abc.ABC):
@@ -28,56 +29,58 @@
         self._original_service_url = service_url
         self._service_url = service_url
         self.__auth = auth
         self._children = None
         self.__path = None
         self.__other_key = kwargs
         self._version = None
+        self._available_impl.clear()
 
     def read_capabilities(self, xml_node: DrbNode):
-        for key_attr in xml_node.attributes.keys():
+        for key_attr in xml_node.attribute_names():
             if key_attr[0].lower() == 'version':
-                self._version = xml_node.get_attribute(key_attr[0])
+                self._version = xml_node @ key_attr[0]
         self.read_version_service(xml_node)
-        if xml_node.has_child('OperationsMetadata'):
+        if 'OperationsMetadata' in xml_node:
             self.read_capabilities_operations_metadata(xml_node)
 
     def read_version_service(self, xmlnode_tree):
-        if xmlnode_tree.has_child('ServiceIdentification'):
+        if 'ServiceIdentification' in xmlnode_tree:
             xmlnode = xmlnode_tree['ServiceIdentification']
-            if xmlnode.has_child('ServiceTypeVersion'):
+            if 'ServiceTypeVersion' in xmlnode:
                 versions = xmlnode['ServiceTypeVersion', None, :]
                 version_max = versions[0].value
                 for version_item in versions[1:]:
                     version = version_item.value
                     if version[0] > version_max[0]:
                         version_max = version
                     elif version[0] == version_max[0]:
                         if version[2] > version_max[2]:
                             version_max = version
                         elif version[2] == version_max[2]:
                             if version[4] > version_max[4]:
                                 version_max = version
                 self._version = version_max
 
+    @abc.abstractmethod
     def manage_predefined_operations_metadata(self, name, request_cap, attr):
         return None
 
     def read_capabilities_operations_metadata(self, xmlnode_tree):
         for xmlnode in xmlnode_tree.children:
 
             if xmlnode.name == 'OperationsMetadata':
                 for request_cap in xmlnode.children:
                     for child in request_cap.children:
                         if child.name == 'DCP':
                             DCPType = request_cap['DCP']
 
                     attr = {('DCP', None): DCPType}
 
-                    name = request_cap.get_attribute('name')
+                    name = request_cap @ 'name'
                     operation = self.manage_predefined_operations_metadata(
                         name,
                         request_cap,
                         attr)
                     if operation is None:
                         operation = WXSNodeOperation(
                             self,
@@ -93,42 +96,37 @@
     def get_auth(self) -> Optional[AuthBase]:
         """
         Returns the associated authentication required to access to the Wxs
         service.
         :returns: an authentication compatible with requests library.
         :rtype: AuthBase
         """
-        if self.__auth is not None:
-            return self.__auth
-        if kr_check(self._original_service_url):
-            return kr_get_auth(self._original_service_url)
+        if self.__auth is None:
+            credential = keyring.get_credential(
+                service_name=self.path.path,
+                username=None
+            )
+            if credential is not None:
+                self.__auth = HTTPBasicAuth(
+                    credential.username,
+                    credential.password
+                )
+        return self.__auth
 
     @property
     @abc.abstractmethod
     def type_service(self):
         raise NotImplementedError
 
     @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
     def path(self) -> ParsedPath:
         if self.__path is None:
             self.__path = ParsedPath(self._service_url)
         return self.__path
 
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return {}
-
     @staticmethod
     def compute_key_url(url, arguments: dict):
         if arguments is not None:
             for (key, value) in arguments.items():
                 if isinstance(value, (list, tuple)):
                     for value_item in value:
                         url += f'&{key}={value_item}'
@@ -139,135 +137,92 @@
     def url_service(self, request: str):
         url = f'{self._service_url}?request={request}' \
                f'&service={self.type_service}'
         return WXSServiceNode.compute_key_url(url, self.__other_key)
 
     def get_capabilities(self):
         get_caps = WXSNodeOperationGetCapabilities(self)
-        return get_caps.children()
+        return get_caps.children()[0]
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
             try:
                 self.read_capabilities(self.get_capabilities())
             except DrbException as ex:
                 raise DrbFactoryException(
                     f'Unsupported Wxs service: {self.name}')
 
         return self._children
 
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        raise DrbException('WxsNode has no attribute')
-
-    def close(self) -> None:
-        pass
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbException(f"Wxs Not doesn't support {impl} implementation")
 
     def __eq__(self, other):
         return isinstance(other, WXSServiceNode) and \
             self._service_url == other._service_url
 
     def __hash__(self):
         return hash(self._service_url)
 
 
 class WXSNodeOperation(AbstractNode):
 
-    def close(self) -> None:
-        pass
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbNotImplementationException(f'no {impl} '
                                             f'implementation found')
 
     def __compute_url(self, arguments: dict):
-        url = self.__parent.url_service(self.name)
+        url = self._parent.url_service(self.name)
         if self._version is not None and len(self._version) > 0 \
                 and 'version' not in arguments.keys():
             url = WXSServiceNode.compute_key_url(url,
                                                  {'version': self._version})
         return WXSServiceNode.compute_key_url(url, arguments)
 
     def __init__(self,
                  source: WXSServiceNode,
                  name: str,
                  namespace: str,
                  attributes: dict = {},
                  version: str = None):
         super(AbstractNode, self).__init__()
 
-        self._name = name
-        self._attributes = attributes
-        self._namespace = namespace
-        self.__parent = source
+        self.name = name
+        self.namespace_uri = namespace
+        self.parent = source
         self._version = version
+        self.__init_attributes(attributes)
+        self._available_impl.clear()
 
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return self._namespace
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def path(self) -> ParsedPath:
-        return self.__path
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self.__parent
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {}
-            for attribute_name in self._data_set.ncattrs():
-                self._attributes[(attribute_name, None)] = \
-                    getattr(self._data_set, attribute_name)
-
-        return self._attributes
+    def __init_attributes(self, attr: dict):
+        for key in attr.keys():
+            self @= (key[0], key[1], attr[key])
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         return []
 
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        key = (name, namespace_uri)
-        if key in self.attributes.keys():
-            return self.attributes[key]
-        raise DrbException(f'Attribute not found name: {name}, '
-                           f'namespace: {namespace_uri}')
-
     @staticmethod
     def _get_content_type(node):
         content_type = ''
-        for attr_key in node.attributes:
+        for attr_key in node.attribute_names():
             if attr_key[0].lower() == 'content-type':
-                content_type = node.get_attribute(attr_key[0])
+                content_type = node @ attr_key[0]
         return content_type
 
     def _get_child(self, item):
         if isinstance(item, dict):
             url = self.__compute_url(item)
-            node = DrbHttpNode(url, auth=self.__parent.get_auth())
+            node = DrbHttpNode(url, auth=self._parent.get_auth())
             impl = node.get_impl(io.BytesIO)
 
             content_type = self._get_content_type(node)
             if 'text/xml' in content_type:
                 tree = ElementTree.parse(impl)
                 node_child = XmlNode(tree.getroot())
             elif 'text/html' in content_type:
@@ -285,8 +240,8 @@
 
 class WXSNodeOperationGetCapabilities(WXSNodeOperation):
     def __init__(self,
                  source: WXSServiceNode):
         super().__init__(source, 'GetCapabilities', None)
 
     def children(self) -> List[DrbNode]:
-        return self._get_child({})
+        return [self._get_child({})]
```

### Comparing `drb-driver-wxs-1.1.1/drb_driver_wxs.egg-info/PKG-INFO` & `drb-driver-wxs-1.2.0/drb_driver_wxs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-wxs
-Version: 1.1.1
+Version: 1.2.0
 Summary: DRB WXS OGC Service driver
-Home-page: https://gitlab.com/drb-python/impl/wXs
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/wXs
+Project-URL: Source, https://gitlab.com/drb-python/impl/wXs
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # WXS driver
 
 This drb-driver-wxs module implements the OWS services (WFS, WMS, WCS, ...).
 For more information about OWS Service see https://www.ogc.org/ or/and
 https://www.ogc.org/standards/wms
 OGC catalog, this driver is abstract, it means that to have a usable
@@ -122,9 +123,7 @@
 # FORMAT=GEOTIFF_INT16&
 # SUBSET=X(-1784000%2C-1140000)&SUBSET=Y(1356000%2C1863000)&
 # SUBSETTINGCRS=http%3A%2F%2Fwww.opengis.net%2Fdef%2Fcrs%2FEPSG%2F0%2F152160&
 # OUTPUTCRS=http%3A%2F%2Fwww.opengis.net%2Fdef%2Fcrs%2FEPSG%2F0%2F152160
 # => return the image
 
 ```
-
-
```

### Comparing `drb-driver-wxs-1.1.1/versioneer.py` & `drb-driver-wxs-1.2.0/versioneer.py`

 * *Files identical despite different names*

