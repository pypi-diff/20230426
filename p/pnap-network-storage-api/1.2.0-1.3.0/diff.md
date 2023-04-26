# Comparing `tmp/pnap-network-storage-api-1.2.0.tar.gz` & `tmp/pnap-network-storage-api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-network-storage-api-1.2.0.tar", last modified: Thu Mar  9 08:59:32 2023, max compression
+gzip compressed data, was "dist/pnap-network-storage-api-1.3.0.tar", last modified: Tue Apr 25 13:58:00 2023, max compression
```

## Comparing `pnap-network-storage-api-1.2.0.tar` & `pnap-network-storage-api-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     7966 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     9888 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/
--rw-r--r--   0 runner    (1001) docker     (116)    16994 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14678 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    12217 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    12333 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network_update.py
--rw-r--r--   0 runner    (1001) docker     (116)    12723 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/status.py
--rw-r--r--   0 runner    (1001) docker     (116)    12920 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/nfs_permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)      358 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13459 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    12026 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)    14739 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume.py
--rw-r--r--   0 runner    (1001) docker     (116)    13348 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    13238 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume_update.py
--rw-r--r--   0 runner    (1001) docker     (116)    14298 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network.py
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39932 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5464 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      236 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    55925 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/api/storage_networks_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)     1084 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83001 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      535 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1665 2023-03-09 08:59:15.000000 pnap-network-storage-api-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9888 2023-03-09 08:59:31.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:59:31.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2023-03-09 08:59:31.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1224 2023-03-09 08:59:32.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:59:31.000000 pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10208 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55925 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/storage_networks_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83001 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12723 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13696 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12920 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12217 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13390 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_volume_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12026 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14739 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13559 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14298 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12087 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16994 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39932 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10208 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-25 13:58:00.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:57:59.000000 pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-25 13:57:44.000000 pnap-network-storage-api-1.3.0/setup.py
```

### Comparing `pnap-network-storage-api-1.2.0/README.md` & `pnap-network-storage-api-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,24 @@
 *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
 
 
 ## Documentation For Models
 
  - [Error](docs/Error.md)
  - [NfsPermissions](docs/NfsPermissions.md)
+ - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
+ - [NfsPermissionsUpdate](docs/NfsPermissionsUpdate.md)
  - [Permissions](docs/Permissions.md)
+ - [PermissionsCreate](docs/PermissionsCreate.md)
+ - [PermissionsUpdate](docs/PermissionsUpdate.md)
  - [Status](docs/Status.md)
  - [StorageNetwork](docs/StorageNetwork.md)
  - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
  - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
+ - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
  - [Volume](docs/Volume.md)
  - [VolumeCreate](docs/VolumeCreate.md)
  - [VolumeUpdate](docs/VolumeUpdate.md)
 
 
 ## Documentation For Authorization
```

### Comparing `pnap-network-storage-api-1.2.0/PKG-INFO` & `pnap-network-storage-api-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-storage-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Network Storage API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api
@@ -140,19 +140,24 @@
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
         
         
         ## Documentation For Models
         
          - [Error](docs/Error.md)
          - [NfsPermissions](docs/NfsPermissions.md)
+         - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
+         - [NfsPermissionsUpdate](docs/NfsPermissionsUpdate.md)
          - [Permissions](docs/Permissions.md)
+         - [PermissionsCreate](docs/PermissionsCreate.md)
+         - [PermissionsUpdate](docs/PermissionsUpdate.md)
          - [Status](docs/Status.md)
          - [StorageNetwork](docs/StorageNetwork.md)
          - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
          - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
+         - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
          - [Volume](docs/Volume.md)
          - [VolumeCreate](docs/VolumeCreate.md)
          - [VolumeUpdate](docs/VolumeUpdate.md)
         
         
         ## Documentation For Authorization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.3.0 Summary:
 Network Storage API Home-page: https://phoenixnap.com/bare-metal-cloud Author:
 PhoenixNAP Team Author-email: support@phoenixnap.com License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api Create, list, edit, and delete storage
 networks with the Network Storage API. Use storage networks to expand storage
 capacity on a private network.
  Knowledge base articles to help you can be found here
@@ -86,28 +86,32 @@
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get)
 | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a
 storage network's volume details. *StorageNetworksApi* |
 [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch)
 | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a
 storage network's volume details. ## Documentation For Models - [Error](docs/
-Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [Permissions](docs/
-Permissions.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
+Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [NfsPermissionsCreate]
+(docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate](docs/
+NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
+[PermissionsCreate](docs/PermissionsCreate.md) - [PermissionsUpdate](docs/
+PermissionsUpdate.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
 StorageNetwork.md) - [StorageNetworkCreate](docs/StorageNetworkCreate.md) -
-[StorageNetworkUpdate](docs/StorageNetworkUpdate.md) - [Volume](docs/Volume.md)
-- [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/VolumeUpdate.md)
-## Documentation For Authorization ## OAuth2 - **Type**: OAuth - **Flow**:
-application - **Authorization URL**: - **Scopes**: - **networkstorage**: Grants
-full access to Network Storage API. - **networkstorage.read**: Grants read only
-access to Network Storage API. ## Author support@phoenixnap.com ## Notes for
-Large OpenAPI documents If the OpenAPI document is large, imports in
-pnap_network_storage_api.apis and pnap_network_storage_api.models may fail with
-a RecursionError indicating the maximum recursion limit has been exceeded. In
-that case, there are a couple of solutions: Solution 1: Use specific imports
-for apis and models like: - `from pnap_network_storage_api.api.default_api
-import DefaultApi` - `from pnap_network_storage_api.model.pet import Pet`
-Solution 2: Before importing the package, adjust the maximum recursion limit as
-shown below: ``` import sys sys.setrecursionlimit(1500) import
-pnap_network_storage_api from pnap_network_storage_api.apis import * from
-pnap_network_storage_api.models import * ``` Keywords: OpenAPI,OpenAPI-
-Generator,Network Storage API Platform: UNKNOWN Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[StorageNetworkUpdate](docs/StorageNetworkUpdate.md) -
+[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) - [Volume]
+(docs/Volume.md) - [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/
+VolumeUpdate.md) ## Documentation For Authorization ## OAuth2 - **Type**: OAuth
+- **Flow**: application - **Authorization URL**: - **Scopes**: -
+**networkstorage**: Grants full access to Network Storage API. -
+**networkstorage.read**: Grants read only access to Network Storage API. ##
+Author support@phoenixnap.com ## Notes for Large OpenAPI documents If the
+OpenAPI document is large, imports in pnap_network_storage_api.apis and
+pnap_network_storage_api.models may fail with a RecursionError indicating the
+maximum recursion limit has been exceeded. In that case, there are a couple of
+solutions: Solution 1: Use specific imports for apis and models like: - `from
+pnap_network_storage_api.api.default_api import DefaultApi` - `from
+pnap_network_storage_api.model.pet import Pet` Solution 2: Before importing the
+package, adjust the maximum recursion limit as shown below: ``` import sys
+sys.setrecursionlimit(1500) import pnap_network_storage_api from
+pnap_network_storage_api.apis import * from pnap_network_storage_api.models
+import * ``` Keywords: OpenAPI,OpenAPI-Generator,Network Storage API Platform:
+UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/configuration.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/rest.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/error.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network_update.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_update.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/status.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/status.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/nfs_permissions.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/nfs_permissions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network_create.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from pnap_network_storage_api.model.volume_create import VolumeCreate
-    globals()['VolumeCreate'] = VolumeCreate
+    from pnap_network_storage_api.model.storage_network_volume_create import StorageNetworkVolumeCreate
+    globals()['StorageNetworkVolumeCreate'] = StorageNetworkVolumeCreate
 
 
 class StorageNetworkCreate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -97,15 +97,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'location': (str,),  # noqa: E501
-            'volumes': ([VolumeCreate],),  # noqa: E501
+            'volumes': ([StorageNetworkVolumeCreate],),  # noqa: E501
             'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -126,15 +126,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, location, volumes, *args, **kwargs):  # noqa: E501
         """StorageNetworkCreate - a model defined in OpenAPI
 
         Args:
             name (str): Storage network friendly name.
             location (str): Location of storage network. Currently this field should be set to `PHX` or `ASH`.
-            volumes ([VolumeCreate]): Volume to be created alongside storage. Currently only 1 volume is supported.
+            volumes ([StorageNetworkVolumeCreate]): Volume to be created alongside storage. Currently only 1 volume is supported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,15 +220,15 @@
     @convert_js_args_to_python_args
     def __init__(self, name, location, volumes, *args, **kwargs):  # noqa: E501
         """StorageNetworkCreate - a model defined in OpenAPI
 
         Args:
             name (str): Storage network friendly name.
             location (str): Location of storage network. Currently this field should be set to `PHX` or `ASH`.
-            volumes ([VolumeCreate]): Volume to be created alongside storage. Currently only 1 volume is supported.
+            volumes ([StorageNetworkVolumeCreate]): Volume to be created alongside storage. Currently only 1 volume is supported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/permissions.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/permissions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume_create.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network_volume_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
 
-class VolumeCreate(ModelNormal):
+class StorageNetworkVolumeCreate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -121,15 +121,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, capacity_in_gb, *args, **kwargs):  # noqa: E501
-        """VolumeCreate - a model defined in OpenAPI
+        """StorageNetworkVolumeCreate - a model defined in OpenAPI
 
         Args:
             name (str): Volume friendly name.
             capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -214,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, name, capacity_in_gb, *args, **kwargs):  # noqa: E501
-        """VolumeCreate - a model defined in OpenAPI
+        """StorageNetworkVolumeCreate - a model defined in OpenAPI
 
         Args:
             name (str): Volume friendly name.
             capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/volume_update.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/volume_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from pnap_network_storage_api.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from pnap_network_storage_api.model.permissions_update import PermissionsUpdate
+    globals()['PermissionsUpdate'] = PermissionsUpdate
+
 
 class VolumeUpdate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -80,45 +84,49 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'capacity_in_gb': (int,),  # noqa: E501
             'path_suffix': (str,),  # noqa: E501
+            'permissions': (PermissionsUpdate,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'capacity_in_gb': 'capacityInGb',  # noqa: E501
         'path_suffix': 'pathSuffix',  # noqa: E501
+        'permissions': 'permissions',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -158,14 +166,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): Volume friendly name.. [optional]  # noqa: E501
             description (str): Volume description.. [optional]  # noqa: E501
             capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.. [optional]  # noqa: E501
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
+            permissions (PermissionsUpdate): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +256,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): Volume friendly name.. [optional]  # noqa: E501
             description (str): Volume description.. [optional]  # noqa: E501
             capacity_in_gb (int): Capacity of Volume in GB. Currently only whole numbers and multiples of 1000GB are supported.. [optional]  # noqa: E501
             path_suffix (str): Last part of volume's path.. [optional]  # noqa: E501
+            permissions (PermissionsUpdate): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model/storage_network.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model/storage_network.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/__init__.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/api_client.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/exceptions.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/api/storage_networks_api.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/api/storage_networks_api.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/models/__init__.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 # from from pnap_network_storage_api.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from pnap_network_storage_api.model.error import Error
 from pnap_network_storage_api.model.nfs_permissions import NfsPermissions
+from pnap_network_storage_api.model.nfs_permissions_create import NfsPermissionsCreate
+from pnap_network_storage_api.model.nfs_permissions_update import NfsPermissionsUpdate
 from pnap_network_storage_api.model.permissions import Permissions
+from pnap_network_storage_api.model.permissions_create import PermissionsCreate
+from pnap_network_storage_api.model.permissions_update import PermissionsUpdate
 from pnap_network_storage_api.model.status import Status
 from pnap_network_storage_api.model.storage_network import StorageNetwork
 from pnap_network_storage_api.model.storage_network_create import StorageNetworkCreate
 from pnap_network_storage_api.model.storage_network_update import StorageNetworkUpdate
+from pnap_network_storage_api.model.storage_network_volume_create import StorageNetworkVolumeCreate
 from pnap_network_storage_api.model.volume import Volume
 from pnap_network_storage_api.model.volume_create import VolumeCreate
 from pnap_network_storage_api.model.volume_update import VolumeUpdate
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/model_utils.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api/apis/__init__.py` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/setup.py` & `pnap-network-storage-api-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/PKG-INFO` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-network-storage-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Network Storage API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api
@@ -140,19 +140,24 @@
         *StorageNetworksApi* | [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch) | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a storage network&#39;s volume details.
         
         
         ## Documentation For Models
         
          - [Error](docs/Error.md)
          - [NfsPermissions](docs/NfsPermissions.md)
+         - [NfsPermissionsCreate](docs/NfsPermissionsCreate.md)
+         - [NfsPermissionsUpdate](docs/NfsPermissionsUpdate.md)
          - [Permissions](docs/Permissions.md)
+         - [PermissionsCreate](docs/PermissionsCreate.md)
+         - [PermissionsUpdate](docs/PermissionsUpdate.md)
          - [Status](docs/Status.md)
          - [StorageNetwork](docs/StorageNetwork.md)
          - [StorageNetworkCreate](docs/StorageNetworkCreate.md)
          - [StorageNetworkUpdate](docs/StorageNetworkUpdate.md)
+         - [StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md)
          - [Volume](docs/Volume.md)
          - [VolumeCreate](docs/VolumeCreate.md)
          - [VolumeUpdate](docs/VolumeUpdate.md)
         
         
         ## Documentation For Authorization
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: pnap-network-storage-api Version: 1.3.0 Summary:
 Network Storage API Home-page: https://phoenixnap.com/bare-metal-cloud Author:
 PhoenixNAP Team Author-email: support@phoenixnap.com License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-network-storage-api Create, list, edit, and delete storage
 networks with the Network Storage API. Use storage networks to expand storage
 capacity on a private network.
  Knowledge base articles to help you can be found here
@@ -86,28 +86,32 @@
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_get)
 | **GET** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Get a
 storage network's volume details. *StorageNetworksApi* |
 [**storage_networks_storage_network_id_volumes_volume_id_patch**](docs/
 StorageNetworksApi.md#storage_networks_storage_network_id_volumes_volume_id_patch)
 | **PATCH** /storage-networks/{storageNetworkId}/volumes/{volumeId} | Update a
 storage network's volume details. ## Documentation For Models - [Error](docs/
-Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [Permissions](docs/
-Permissions.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
+Error.md) - [NfsPermissions](docs/NfsPermissions.md) - [NfsPermissionsCreate]
+(docs/NfsPermissionsCreate.md) - [NfsPermissionsUpdate](docs/
+NfsPermissionsUpdate.md) - [Permissions](docs/Permissions.md) -
+[PermissionsCreate](docs/PermissionsCreate.md) - [PermissionsUpdate](docs/
+PermissionsUpdate.md) - [Status](docs/Status.md) - [StorageNetwork](docs/
 StorageNetwork.md) - [StorageNetworkCreate](docs/StorageNetworkCreate.md) -
-[StorageNetworkUpdate](docs/StorageNetworkUpdate.md) - [Volume](docs/Volume.md)
-- [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/VolumeUpdate.md)
-## Documentation For Authorization ## OAuth2 - **Type**: OAuth - **Flow**:
-application - **Authorization URL**: - **Scopes**: - **networkstorage**: Grants
-full access to Network Storage API. - **networkstorage.read**: Grants read only
-access to Network Storage API. ## Author support@phoenixnap.com ## Notes for
-Large OpenAPI documents If the OpenAPI document is large, imports in
-pnap_network_storage_api.apis and pnap_network_storage_api.models may fail with
-a RecursionError indicating the maximum recursion limit has been exceeded. In
-that case, there are a couple of solutions: Solution 1: Use specific imports
-for apis and models like: - `from pnap_network_storage_api.api.default_api
-import DefaultApi` - `from pnap_network_storage_api.model.pet import Pet`
-Solution 2: Before importing the package, adjust the maximum recursion limit as
-shown below: ``` import sys sys.setrecursionlimit(1500) import
-pnap_network_storage_api from pnap_network_storage_api.apis import * from
-pnap_network_storage_api.models import * ``` Keywords: OpenAPI,OpenAPI-
-Generator,Network Storage API Platform: UNKNOWN Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[StorageNetworkUpdate](docs/StorageNetworkUpdate.md) -
+[StorageNetworkVolumeCreate](docs/StorageNetworkVolumeCreate.md) - [Volume]
+(docs/Volume.md) - [VolumeCreate](docs/VolumeCreate.md) - [VolumeUpdate](docs/
+VolumeUpdate.md) ## Documentation For Authorization ## OAuth2 - **Type**: OAuth
+- **Flow**: application - **Authorization URL**: - **Scopes**: -
+**networkstorage**: Grants full access to Network Storage API. -
+**networkstorage.read**: Grants read only access to Network Storage API. ##
+Author support@phoenixnap.com ## Notes for Large OpenAPI documents If the
+OpenAPI document is large, imports in pnap_network_storage_api.apis and
+pnap_network_storage_api.models may fail with a RecursionError indicating the
+maximum recursion limit has been exceeded. In that case, there are a couple of
+solutions: Solution 1: Use specific imports for apis and models like: - `from
+pnap_network_storage_api.api.default_api import DefaultApi` - `from
+pnap_network_storage_api.model.pet import Pet` Solution 2: Before importing the
+package, adjust the maximum recursion limit as shown below: ``` import sys
+sys.setrecursionlimit(1500) import pnap_network_storage_api from
+pnap_network_storage_api.apis import * from pnap_network_storage_api.models
+import * ``` Keywords: OpenAPI,OpenAPI-Generator,Network Storage API Platform:
+UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `pnap-network-storage-api-1.2.0/pnap_network_storage_api.egg-info/SOURCES.txt` & `pnap-network-storage-api-1.3.0/pnap_network_storage_api.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 pnap_network_storage_api.egg-info/top_level.txt
 pnap_network_storage_api/api/__init__.py
 pnap_network_storage_api/api/storage_networks_api.py
 pnap_network_storage_api/apis/__init__.py
 pnap_network_storage_api/model/__init__.py
 pnap_network_storage_api/model/error.py
 pnap_network_storage_api/model/nfs_permissions.py
+pnap_network_storage_api/model/nfs_permissions_create.py
+pnap_network_storage_api/model/nfs_permissions_update.py
 pnap_network_storage_api/model/permissions.py
+pnap_network_storage_api/model/permissions_create.py
+pnap_network_storage_api/model/permissions_update.py
 pnap_network_storage_api/model/status.py
 pnap_network_storage_api/model/storage_network.py
 pnap_network_storage_api/model/storage_network_create.py
 pnap_network_storage_api/model/storage_network_update.py
+pnap_network_storage_api/model/storage_network_volume_create.py
 pnap_network_storage_api/model/volume.py
 pnap_network_storage_api/model/volume_create.py
 pnap_network_storage_api/model/volume_update.py
 pnap_network_storage_api/models/__init__.py
```

