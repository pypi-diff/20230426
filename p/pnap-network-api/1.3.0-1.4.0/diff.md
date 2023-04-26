# Comparing `tmp/pnap-network-api-1.3.0.tar.gz` & `tmp/pnap-network-api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-network-api-1.3.0.tar", last modified: Thu Mar  9 08:58:56 2023, max compression
+gzip compressed data, was "dist/pnap-network-api-1.4.0.tar", last modified: Tue Apr 25 13:57:58 2023, max compression
```

## Comparing `pnap-network-api-1.3.0.tar` & `pnap-network-api-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)     8031 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     9947 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9947 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1159 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api/
--rw-r--r--   0 runner    (1001) docker     (116)    17325 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    15039 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    12570 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    14518 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/private_network_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    12530 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/private_network_server.py
--rw-r--r--   0 runner    (1001) docker     (116)      350 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12582 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/public_network_membership.py
--rw-r--r--   0 runner    (1001) docker     (116)    12773 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/public_network_modify.py
--rw-r--r--   0 runner    (1001) docker     (116)    15699 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/public_network.py
--rw-r--r--   0 runner    (1001) docker     (116)    12941 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/network_membership.py
--rw-r--r--   0 runner    (1001) docker     (116)    14353 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/public_network_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    12257 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/public_network_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (116)    13310 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/private_network_modify.py
--rw-r--r--   0 runner    (1001) docker     (116)    16472 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model/private_network.py
--rw-r--r--   0 runner    (1001) docker     (116)     1561 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    40261 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5833 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)    39925 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/api/public_networks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      228 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    27715 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/api/private_networks_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)     1098 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83362 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:58:56.000000 pnap-network-api-1.3.0/pnap_network_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      590 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/pnap_network_api/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     2004 2023-03-09 08:58:43.000000 pnap-network-api-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9947 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)    39925 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/public_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28150 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api/private_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15039 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83362 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:57:58.000000 pnap-network-api-1.4.0/pnap_network_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12773 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12582 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_membership.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14730 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16462 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12570 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15699 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12941 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/network_membership.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/public_network_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13310 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/model/private_network_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17325 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40261 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/pnap_network_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-04-25 13:57:45.000000 pnap-network-api-1.4.0/setup.py
```

### Comparing `pnap-network-api-1.3.0/README.md` & `pnap-network-api-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/PKG-INFO` & `pnap-network-api-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Networks API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-api Version: 1.3.0 Summary: Networks
+Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.0 Summary: Networks
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 network-api Create, list, edit and delete public/private networks with the
 Network API. Use public networks to place multiple servers on the same network
 or VLAN. Assign new servers with IP addresses from the same CIDR range. Use
 private networks to avoid unnecessary egress data charges. Model your networks
```

### Comparing `pnap-network-api-1.3.0/pnap_network_api.egg-info/PKG-INFO` & `pnap-network-api-1.4.0/pnap_network_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Networks API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-api Version: 1.3.0 Summary: Networks
+Metadata-Version: 2.1 Name: pnap-network-api Version: 1.4.0 Summary: Networks
 API Home-page: https://phoenixnap.com/bare-metal-cloud Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com License: Apache 2.0 Project-URL:
 Repository, https://github.com/phoenixnap/python-sdk-bmc Description: # pnap-
 network-api Create, list, edit and delete public/private networks with the
 Network API. Use public networks to place multiple servers on the same network
 or VLAN. Assign new servers with IP addresses from the same CIDR range. Use
 private networks to avoid unnecessary egress data charges. Model your networks
```

### Comparing `pnap-network-api-1.3.0/pnap_network_api.egg-info/SOURCES.txt` & `pnap-network-api-1.4.0/pnap_network_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/configuration.py` & `pnap-network-api-1.4.0/pnap_network_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/rest.py` & `pnap-network-api-1.4.0/pnap_network_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/error.py` & `pnap-network-api-1.4.0/pnap_network_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/private_network_create.py` & `pnap-network-api-1.4.0/pnap_network_api/model/private_network_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,48 +91,47 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
             'location': (str,),  # noqa: E501
-            'cidr': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'location_default': (bool,),  # noqa: E501
             'vlan_id': (int,),  # noqa: E501
+            'cidr': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'location': 'location',  # noqa: E501
-        'cidr': 'cidr',  # noqa: E501
         'description': 'description',  # noqa: E501
         'location_default': 'locationDefault',  # noqa: E501
         'vlan_id': 'vlanId',  # noqa: E501
+        'cidr': 'cidr',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, location, cidr, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, name, location, *args, **kwargs):  # noqa: E501
         """PrivateNetworkCreate - a model defined in OpenAPI
 
         Args:
             name (str): The friendly name of this private network. This name should be unique.
             location (str): The location of this private network. Supported values are `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` and `AUS`.
-            cidr (str): IP range associated with this private network in CIDR notation.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -160,14 +159,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): The description of this private network.. [optional]  # noqa: E501
             location_default (bool): Identifies network as the default private network for the specified location.. [optional] if omitted the server will use the default value of False  # noqa: E501
             vlan_id (int): The VLAN that will be assigned to this network.. [optional]  # noqa: E501
+            cidr (str): IP range associated with this private network in CIDR notation.<br> Setting the `force` query parameter to `true` allows you to skip assigning a specific IP range to network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +193,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.location = location
-        self.cidr = cidr
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -214,21 +213,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, location, cidr, *args, **kwargs):  # noqa: E501
+    def __init__(self, name, location, *args, **kwargs):  # noqa: E501
         """PrivateNetworkCreate - a model defined in OpenAPI
 
         Args:
             name (str): The friendly name of this private network. This name should be unique.
             location (str): The location of this private network. Supported values are `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` and `AUS`.
-            cidr (str): IP range associated with this private network in CIDR notation.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -256,14 +254,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): The description of this private network.. [optional]  # noqa: E501
             location_default (bool): Identifies network as the default private network for the specified location.. [optional] if omitted the server will use the default value of False  # noqa: E501
             vlan_id (int): The VLAN that will be assigned to this network.. [optional]  # noqa: E501
+            cidr (str): IP range associated with this private network in CIDR notation.<br> Setting the `force` query parameter to `true` allows you to skip assigning a specific IP range to network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -287,15 +286,14 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.location = location
-        self.cidr = cidr
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/private_network_server.py` & `pnap-network-api-1.4.0/pnap_network_api/model/private_network_server.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/public_network_membership.py` & `pnap-network-api-1.4.0/pnap_network_api/model/public_network_membership.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/public_network_modify.py` & `pnap-network-api-1.4.0/pnap_network_api/model/public_network_modify.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/public_network.py` & `pnap-network-api-1.4.0/pnap_network_api/model/public_network.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/network_membership.py` & `pnap-network-api-1.4.0/pnap_network_api/model/network_membership.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/public_network_create.py` & `pnap-network-api-1.4.0/pnap_network_api/model/public_network_create.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/public_network_ip_block.py` & `pnap-network-api-1.4.0/pnap_network_api/model/public_network_ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/private_network_modify.py` & `pnap-network-api-1.4.0/pnap_network_api/model/private_network_modify.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model/private_network.py` & `pnap-network-api-1.4.0/pnap_network_api/model/private_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,60 +99,59 @@
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'vlan_id': (int,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'location': (str,),  # noqa: E501
             'location_default': (bool,),  # noqa: E501
-            'cidr': (str,),  # noqa: E501
             'servers': ([PrivateNetworkServer],),  # noqa: E501
             'memberships': ([NetworkMembership],),  # noqa: E501
             'status': (str,),  # noqa: E501
             'created_on': (datetime,),  # noqa: E501
             'description': (str,),  # noqa: E501
+            'cidr': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'vlan_id': 'vlanId',  # noqa: E501
         'type': 'type',  # noqa: E501
         'location': 'location',  # noqa: E501
         'location_default': 'locationDefault',  # noqa: E501
-        'cidr': 'cidr',  # noqa: E501
         'servers': 'servers',  # noqa: E501
         'memberships': 'memberships',  # noqa: E501
         'status': 'status',  # noqa: E501
         'created_on': 'createdOn',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'cidr': 'cidr',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, vlan_id, type, location, location_default, cidr, servers, memberships, status, created_on, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, name, vlan_id, type, location, location_default, servers, memberships, status, created_on, *args, **kwargs):  # noqa: E501
         """PrivateNetwork - a model defined in OpenAPI
 
         Args:
             id (str): The private network identifier.
             name (str): The friendly name of this private network.
             vlan_id (int): The VLAN of this private network.
             type (str): The type of the private network.
             location (str): The location of this private network.
             location_default (bool): Identifies network as the default private network for the specified location.
-            cidr (str): IP range associated with this private network in CIDR notation.
             servers ([PrivateNetworkServer]):
             memberships ([NetworkMembership]): A list of resources that are members of this private network.
             status (str): The status of the private network. Can have one of the following values: `BUSY` or `READY`.
             created_on (datetime): Date and time when this private network was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -182,14 +181,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): The description of this private network.. [optional]  # noqa: E501
+            cidr (str): IP range associated with this private network in CIDR notation.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,15 +219,14 @@
 
         self.id = id
         self.name = name
         self.vlan_id = vlan_id
         self.type = type
         self.location = location
         self.location_default = location_default
-        self.cidr = cidr
         self.servers = servers
         self.memberships = memberships
         self.status = status
         self.created_on = created_on
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
@@ -244,25 +243,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, vlan_id, type, location, location_default, cidr, servers, memberships, status, created_on, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, name, vlan_id, type, location, location_default, servers, memberships, status, created_on, *args, **kwargs):  # noqa: E501
         """PrivateNetwork - a model defined in OpenAPI
 
         Args:
             id (str): The private network identifier.
             name (str): The friendly name of this private network.
             vlan_id (int): The VLAN of this private network.
             type (str): The type of the private network.
             location (str): The location of this private network.
             location_default (bool): Identifies network as the default private network for the specified location.
-            cidr (str): IP range associated with this private network in CIDR notation.
             servers ([PrivateNetworkServer]):
             memberships ([NetworkMembership]): A list of resources that are members of this private network.
             status (str): The status of the private network. Can have one of the following values: `BUSY` or `READY`.
             created_on (datetime): Date and time when this private network was created.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -292,14 +290,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): The description of this private network.. [optional]  # noqa: E501
+            cidr (str): IP range associated with this private network in CIDR notation.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -327,15 +326,14 @@
 
         self.id = id
         self.name = name
         self.vlan_id = vlan_id
         self.type = type
         self.location = location
         self.location_default = location_default
-        self.cidr = cidr
         self.servers = servers
         self.memberships = memberships
         self.status = status
         self.created_on = created_on
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `pnap-network-api-1.3.0/pnap_network_api/__init__.py` & `pnap-network-api-1.4.0/pnap_network_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/api_client.py` & `pnap-network-api-1.4.0/pnap_network_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/exceptions.py` & `pnap-network-api-1.4.0/pnap_network_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/api/public_networks_api.py` & `pnap-network-api-1.4.0/pnap_network_api/api/public_networks_api.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/api/private_networks_api.py` & `pnap-network-api-1.4.0/pnap_network_api/api/private_networks_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,14 +256,15 @@
                 'endpoint_path': '/private-networks',
                 'operation_id': 'private_networks_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'force',
                     'private_network_create',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
@@ -272,20 +273,24 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'force':
+                        (bool,),
                     'private_network_create':
                         (PrivateNetworkCreate,),
                 },
                 'attribute_map': {
+                    'force': 'force',
                 },
                 'location_map': {
+                    'force': 'query',
                     'private_network_create': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -638,14 +643,15 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.private_networks_post(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
+            force (bool): Query parameter controlling advanced features availability. Currently applicable for networking. It is advised to use with caution since it might lead to unhealthy setups.. [optional] if omitted the server will use the default value of False
             private_network_create (PrivateNetworkCreate): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `pnap-network-api-1.3.0/pnap_network_api/models/__init__.py` & `pnap-network-api-1.4.0/pnap_network_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/model_utils.py` & `pnap-network-api-1.4.0/pnap_network_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/pnap_network_api/apis/__init__.py` & `pnap-network-api-1.4.0/pnap_network_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-api-1.3.0/setup.py` & `pnap-network-api-1.4.0/setup.py`

 * *Files identical despite different names*

