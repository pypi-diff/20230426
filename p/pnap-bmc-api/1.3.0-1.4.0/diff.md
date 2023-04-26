# Comparing `tmp/pnap-bmc-api-1.3.0.tar.gz` & `tmp/pnap-bmc-api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pnap-bmc-api-1.3.0.tar", last modified: Thu Mar  9 08:53:44 2023, max compression
+gzip compressed data, was "dist/pnap-bmc-api-1.4.0.tar", last modified: Tue Apr 25 13:58:03 2023, max compression
```

## Comparing `pnap-bmc-api-1.3.0.tar` & `pnap-bmc-api-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)    10914 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    13122 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)    13122 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1798 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/
--rw-r--r--   0 runner    (1001) docker     (116)    17089 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14821 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)    23583 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server.py
--rw-r--r--   0 runner    (1001) docker     (116)    12348 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    13555 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map_esxi.py
--rw-r--r--   0 runner    (1001) docker     (116)    12989 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_cloud_init.py
--rw-r--r--   0 runner    (1001) docker     (116)    12238 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    13317 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/tag_assignment.py
--rw-r--r--   0 runner    (1001) docker     (116)    12438 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    12387 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (116)    12862 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    13047 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map.py
--rw-r--r--   0 runner    (1001) docker     (116)    12085 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/action_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    12675 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key_update.py
--rw-r--r--   0 runner    (1001) docker     (116)      346 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12904 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/reset_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    13106 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/tag_assignment_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    20399 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_create.py
--rw-r--r--   0 runner    (1001) docker     (116)    14608 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_private_network.py
--rw-r--r--   0 runner    (1001) docker     (116)    12373 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/delete_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    12661 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/public_network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14037 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (116)    13614 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_reset.py
--rw-r--r--   0 runner    (1001) docker     (116)    12587 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_windows.py
--rw-r--r--   0 runner    (1001) docker     (116)    14575 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/private_network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    14408 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/network_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    12425 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/delete_ssh_key_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    12450 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_reserve.py
--rw-r--r--   0 runner    (1001) docker     (116)    12299 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/relinquish_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (116)    15248 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    15012 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request_details.py
--rw-r--r--   0 runner    (1001) docker     (116)    12525 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_patch.py
--rw-r--r--   0 runner    (1001) docker     (116)    13520 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/ip_blocks_configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)    13534 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_public_network.py
--rw-r--r--   0 runner    (1001) docker     (116)    13568 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map_proxmox.py
--rw-r--r--   0 runner    (1001) docker     (116)    14631 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota.py
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39978 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5619 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      215 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    26456 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api/ssh_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    16527 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api/quotas_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   107443 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/api/servers_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)     2623 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83144 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-09 08:53:44.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      578 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       18 2023-03-09 08:53:34.000000 pnap-bmc-api-1.3.0/pnap_bmc_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    13973 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11725 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13973 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16527 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/quotas_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26456 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)   121100 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api/servers_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14821 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    83144 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5619 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 13:58:03.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/
+-rw-r--r--   0 runner    (1001) docker     (122)    13546 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ip_blocks_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12425 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_ssh_key_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12348 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12238 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_network_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13614 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13603 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_esxi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13530 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_softgate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14631 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12904 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/reset_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12373 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_cloud_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12862 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16770 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14632 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14601 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/private_network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14408 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/public_network_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14037 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12299 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/relinquish_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_netris_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12525 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_patch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13317 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24169 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13616 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_proxmox.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12675 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12085 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/action_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_windows.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15012 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13106 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12438 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12411 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12450 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reserve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20659 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13558 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_public_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17089 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39978 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/pnap_bmc_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-04-25 13:57:45.000000 pnap-bmc-api-1.4.0/setup.py
```

### Comparing `pnap-bmc-api-1.3.0/README.md` & `pnap-bmc-api-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -135,16 +135,18 @@
 *ServersApi* | [**servers_server_id_actions_reset_post**](docs/ServersApi.md#servers_server_id_actions_reset_post) | **POST** /servers/{serverId}/actions/reset | Reset server.
 *ServersApi* | [**servers_server_id_actions_shutdown_post**](docs/ServersApi.md#servers_server_id_actions_shutdown_post) | **POST** /servers/{serverId}/actions/shutdown | Shutdown server.
 *ServersApi* | [**servers_server_id_delete**](docs/ServersApi.md#servers_server_id_delete) | **DELETE** /servers/{serverId} | Delete server.
 *ServersApi* | [**servers_server_id_get**](docs/ServersApi.md#servers_server_id_get) | **GET** /servers/{serverId} | Get server.
 *ServersApi* | [**servers_server_id_ip_blocks_ip_block_id_delete**](docs/ServersApi.md#servers_server_id_ip_blocks_ip_block_id_delete) | **DELETE** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks/{ipBlockId} | Unassign IP Block from Server.
 *ServersApi* | [**servers_server_id_ip_blocks_post**](docs/ServersApi.md#servers_server_id_ip_blocks_post) | **POST** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks | Assign IP Block to Server.
 *ServersApi* | [**servers_server_id_patch**](docs/ServersApi.md#servers_server_id_patch) | **PATCH** /servers/{serverId} | Patch a Server.
+*ServersApi* | [**servers_server_id_private_networks_patch**](docs/ServersApi.md#servers_server_id_private_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/private-network-configuration/private-networks/{privateNetworkId} | Updates the server&#39;s private network&#39;s IP addresses
 *ServersApi* | [**servers_server_id_private_networks_post**](docs/ServersApi.md#servers_server_id_private_networks_post) | **POST** /servers/{serverId}/network-configuration/private-network-configuration/private-networks | Adds the server to a private network.
 *ServersApi* | [**servers_server_id_public_networks_delete**](docs/ServersApi.md#servers_server_id_public_networks_delete) | **DELETE** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Removes the server from the Public Network
+*ServersApi* | [**servers_server_id_public_networks_patch**](docs/ServersApi.md#servers_server_id_public_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Updates the server&#39;s public network&#39;s IP addresses.
 *ServersApi* | [**servers_server_id_public_networks_post**](docs/ServersApi.md#servers_server_id_public_networks_post) | **POST** /servers/{serverId}/network-configuration/public-network-configuration/public-networks | Adds the server to a Public Network.
 *ServersApi* | [**servers_server_id_tags_put**](docs/ServersApi.md#servers_server_id_tags_put) | **PUT** /servers/{serverId}/tags | Overwrite tags assigned for Server.
 
 
 ## Documentation For Models
 
  - [ActionResult](docs/ActionResult.md)
@@ -154,26 +156,29 @@
  - [IpBlocksConfiguration](docs/IpBlocksConfiguration.md)
  - [NetworkConfiguration](docs/NetworkConfiguration.md)
  - [OsConfiguration](docs/OsConfiguration.md)
  - [OsConfigurationCloudInit](docs/OsConfigurationCloudInit.md)
  - [OsConfigurationMap](docs/OsConfigurationMap.md)
  - [OsConfigurationMapEsxi](docs/OsConfigurationMapEsxi.md)
  - [OsConfigurationMapProxmox](docs/OsConfigurationMapProxmox.md)
+ - [OsConfigurationNetrisController](docs/OsConfigurationNetrisController.md)
+ - [OsConfigurationNetrisSoftgate](docs/OsConfigurationNetrisSoftgate.md)
  - [OsConfigurationWindows](docs/OsConfigurationWindows.md)
  - [PrivateNetworkConfiguration](docs/PrivateNetworkConfiguration.md)
  - [PublicNetworkConfiguration](docs/PublicNetworkConfiguration.md)
  - [Quota](docs/Quota.md)
  - [QuotaEditLimitRequest](docs/QuotaEditLimitRequest.md)
  - [QuotaEditLimitRequestDetails](docs/QuotaEditLimitRequestDetails.md)
  - [QuotaEditLimitRequestDetailsAllOf](docs/QuotaEditLimitRequestDetailsAllOf.md)
  - [RelinquishIpBlock](docs/RelinquishIpBlock.md)
  - [ResetResult](docs/ResetResult.md)
  - [Server](docs/Server.md)
  - [ServerCreate](docs/ServerCreate.md)
  - [ServerIpBlock](docs/ServerIpBlock.md)
+ - [ServerNetworkUpdate](docs/ServerNetworkUpdate.md)
  - [ServerPatch](docs/ServerPatch.md)
  - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
  - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
  - [ServerReserve](docs/ServerReserve.md)
  - [ServerReset](docs/ServerReset.md)
  - [SshKey](docs/SshKey.md)
  - [SshKeyCreate](docs/SshKeyCreate.md)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/PKG-INFO` & `pnap-bmc-api-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-bmc-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Bare Metal Cloud API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-bmc-api
@@ -144,16 +144,18 @@
         *ServersApi* | [**servers_server_id_actions_reset_post**](docs/ServersApi.md#servers_server_id_actions_reset_post) | **POST** /servers/{serverId}/actions/reset | Reset server.
         *ServersApi* | [**servers_server_id_actions_shutdown_post**](docs/ServersApi.md#servers_server_id_actions_shutdown_post) | **POST** /servers/{serverId}/actions/shutdown | Shutdown server.
         *ServersApi* | [**servers_server_id_delete**](docs/ServersApi.md#servers_server_id_delete) | **DELETE** /servers/{serverId} | Delete server.
         *ServersApi* | [**servers_server_id_get**](docs/ServersApi.md#servers_server_id_get) | **GET** /servers/{serverId} | Get server.
         *ServersApi* | [**servers_server_id_ip_blocks_ip_block_id_delete**](docs/ServersApi.md#servers_server_id_ip_blocks_ip_block_id_delete) | **DELETE** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks/{ipBlockId} | Unassign IP Block from Server.
         *ServersApi* | [**servers_server_id_ip_blocks_post**](docs/ServersApi.md#servers_server_id_ip_blocks_post) | **POST** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks | Assign IP Block to Server.
         *ServersApi* | [**servers_server_id_patch**](docs/ServersApi.md#servers_server_id_patch) | **PATCH** /servers/{serverId} | Patch a Server.
+        *ServersApi* | [**servers_server_id_private_networks_patch**](docs/ServersApi.md#servers_server_id_private_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/private-network-configuration/private-networks/{privateNetworkId} | Updates the server&#39;s private network&#39;s IP addresses
         *ServersApi* | [**servers_server_id_private_networks_post**](docs/ServersApi.md#servers_server_id_private_networks_post) | **POST** /servers/{serverId}/network-configuration/private-network-configuration/private-networks | Adds the server to a private network.
         *ServersApi* | [**servers_server_id_public_networks_delete**](docs/ServersApi.md#servers_server_id_public_networks_delete) | **DELETE** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Removes the server from the Public Network
+        *ServersApi* | [**servers_server_id_public_networks_patch**](docs/ServersApi.md#servers_server_id_public_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Updates the server&#39;s public network&#39;s IP addresses.
         *ServersApi* | [**servers_server_id_public_networks_post**](docs/ServersApi.md#servers_server_id_public_networks_post) | **POST** /servers/{serverId}/network-configuration/public-network-configuration/public-networks | Adds the server to a Public Network.
         *ServersApi* | [**servers_server_id_tags_put**](docs/ServersApi.md#servers_server_id_tags_put) | **PUT** /servers/{serverId}/tags | Overwrite tags assigned for Server.
         
         
         ## Documentation For Models
         
          - [ActionResult](docs/ActionResult.md)
@@ -163,26 +165,29 @@
          - [IpBlocksConfiguration](docs/IpBlocksConfiguration.md)
          - [NetworkConfiguration](docs/NetworkConfiguration.md)
          - [OsConfiguration](docs/OsConfiguration.md)
          - [OsConfigurationCloudInit](docs/OsConfigurationCloudInit.md)
          - [OsConfigurationMap](docs/OsConfigurationMap.md)
          - [OsConfigurationMapEsxi](docs/OsConfigurationMapEsxi.md)
          - [OsConfigurationMapProxmox](docs/OsConfigurationMapProxmox.md)
+         - [OsConfigurationNetrisController](docs/OsConfigurationNetrisController.md)
+         - [OsConfigurationNetrisSoftgate](docs/OsConfigurationNetrisSoftgate.md)
          - [OsConfigurationWindows](docs/OsConfigurationWindows.md)
          - [PrivateNetworkConfiguration](docs/PrivateNetworkConfiguration.md)
          - [PublicNetworkConfiguration](docs/PublicNetworkConfiguration.md)
          - [Quota](docs/Quota.md)
          - [QuotaEditLimitRequest](docs/QuotaEditLimitRequest.md)
          - [QuotaEditLimitRequestDetails](docs/QuotaEditLimitRequestDetails.md)
          - [QuotaEditLimitRequestDetailsAllOf](docs/QuotaEditLimitRequestDetailsAllOf.md)
          - [RelinquishIpBlock](docs/RelinquishIpBlock.md)
          - [ResetResult](docs/ResetResult.md)
          - [Server](docs/Server.md)
          - [ServerCreate](docs/ServerCreate.md)
          - [ServerIpBlock](docs/ServerIpBlock.md)
+         - [ServerNetworkUpdate](docs/ServerNetworkUpdate.md)
          - [ServerPatch](docs/ServerPatch.md)
          - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
          - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
          - [ServerReserve](docs/ServerReserve.md)
          - [ServerReset](docs/ServerReset.md)
          - [SshKey](docs/SshKey.md)
          - [SshKeyCreate](docs/SshKeyCreate.md)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api.egg-info/SOURCES.txt` & `pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,29 @@
 pnap_bmc_api/model/ip_blocks_configuration.py
 pnap_bmc_api/model/network_configuration.py
 pnap_bmc_api/model/os_configuration.py
 pnap_bmc_api/model/os_configuration_cloud_init.py
 pnap_bmc_api/model/os_configuration_map.py
 pnap_bmc_api/model/os_configuration_map_esxi.py
 pnap_bmc_api/model/os_configuration_map_proxmox.py
+pnap_bmc_api/model/os_configuration_netris_controller.py
+pnap_bmc_api/model/os_configuration_netris_softgate.py
 pnap_bmc_api/model/os_configuration_windows.py
 pnap_bmc_api/model/private_network_configuration.py
 pnap_bmc_api/model/public_network_configuration.py
 pnap_bmc_api/model/quota.py
 pnap_bmc_api/model/quota_edit_limit_request.py
 pnap_bmc_api/model/quota_edit_limit_request_details.py
 pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py
 pnap_bmc_api/model/relinquish_ip_block.py
 pnap_bmc_api/model/reset_result.py
 pnap_bmc_api/model/server.py
 pnap_bmc_api/model/server_create.py
 pnap_bmc_api/model/server_ip_block.py
+pnap_bmc_api/model/server_network_update.py
 pnap_bmc_api/model/server_patch.py
 pnap_bmc_api/model/server_private_network.py
 pnap_bmc_api/model/server_public_network.py
 pnap_bmc_api/model/server_reserve.py
 pnap_bmc_api/model/server_reset.py
 pnap_bmc_api/model/ssh_key.py
 pnap_bmc_api/model/ssh_key_create.py
```

### Comparing `pnap-bmc-api-1.3.0/PKG-INFO` & `pnap-bmc-api-1.4.0/pnap_bmc_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnap-bmc-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Bare Metal Cloud API
 Home-page: https://phoenixnap.com/bare-metal-cloud
 Author: PhoenixNAP Team
 Author-email: support@phoenixnap.com
 License: Apache 2.0
 Project-URL: Repository, https://github.com/phoenixnap/python-sdk-bmc
 Description: # pnap-bmc-api
@@ -144,16 +144,18 @@
         *ServersApi* | [**servers_server_id_actions_reset_post**](docs/ServersApi.md#servers_server_id_actions_reset_post) | **POST** /servers/{serverId}/actions/reset | Reset server.
         *ServersApi* | [**servers_server_id_actions_shutdown_post**](docs/ServersApi.md#servers_server_id_actions_shutdown_post) | **POST** /servers/{serverId}/actions/shutdown | Shutdown server.
         *ServersApi* | [**servers_server_id_delete**](docs/ServersApi.md#servers_server_id_delete) | **DELETE** /servers/{serverId} | Delete server.
         *ServersApi* | [**servers_server_id_get**](docs/ServersApi.md#servers_server_id_get) | **GET** /servers/{serverId} | Get server.
         *ServersApi* | [**servers_server_id_ip_blocks_ip_block_id_delete**](docs/ServersApi.md#servers_server_id_ip_blocks_ip_block_id_delete) | **DELETE** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks/{ipBlockId} | Unassign IP Block from Server.
         *ServersApi* | [**servers_server_id_ip_blocks_post**](docs/ServersApi.md#servers_server_id_ip_blocks_post) | **POST** /servers/{serverId}/network-configuration/ip-block-configurations/ip-blocks | Assign IP Block to Server.
         *ServersApi* | [**servers_server_id_patch**](docs/ServersApi.md#servers_server_id_patch) | **PATCH** /servers/{serverId} | Patch a Server.
+        *ServersApi* | [**servers_server_id_private_networks_patch**](docs/ServersApi.md#servers_server_id_private_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/private-network-configuration/private-networks/{privateNetworkId} | Updates the server&#39;s private network&#39;s IP addresses
         *ServersApi* | [**servers_server_id_private_networks_post**](docs/ServersApi.md#servers_server_id_private_networks_post) | **POST** /servers/{serverId}/network-configuration/private-network-configuration/private-networks | Adds the server to a private network.
         *ServersApi* | [**servers_server_id_public_networks_delete**](docs/ServersApi.md#servers_server_id_public_networks_delete) | **DELETE** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Removes the server from the Public Network
+        *ServersApi* | [**servers_server_id_public_networks_patch**](docs/ServersApi.md#servers_server_id_public_networks_patch) | **PATCH** /servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId} | Updates the server&#39;s public network&#39;s IP addresses.
         *ServersApi* | [**servers_server_id_public_networks_post**](docs/ServersApi.md#servers_server_id_public_networks_post) | **POST** /servers/{serverId}/network-configuration/public-network-configuration/public-networks | Adds the server to a Public Network.
         *ServersApi* | [**servers_server_id_tags_put**](docs/ServersApi.md#servers_server_id_tags_put) | **PUT** /servers/{serverId}/tags | Overwrite tags assigned for Server.
         
         
         ## Documentation For Models
         
          - [ActionResult](docs/ActionResult.md)
@@ -163,26 +165,29 @@
          - [IpBlocksConfiguration](docs/IpBlocksConfiguration.md)
          - [NetworkConfiguration](docs/NetworkConfiguration.md)
          - [OsConfiguration](docs/OsConfiguration.md)
          - [OsConfigurationCloudInit](docs/OsConfigurationCloudInit.md)
          - [OsConfigurationMap](docs/OsConfigurationMap.md)
          - [OsConfigurationMapEsxi](docs/OsConfigurationMapEsxi.md)
          - [OsConfigurationMapProxmox](docs/OsConfigurationMapProxmox.md)
+         - [OsConfigurationNetrisController](docs/OsConfigurationNetrisController.md)
+         - [OsConfigurationNetrisSoftgate](docs/OsConfigurationNetrisSoftgate.md)
          - [OsConfigurationWindows](docs/OsConfigurationWindows.md)
          - [PrivateNetworkConfiguration](docs/PrivateNetworkConfiguration.md)
          - [PublicNetworkConfiguration](docs/PublicNetworkConfiguration.md)
          - [Quota](docs/Quota.md)
          - [QuotaEditLimitRequest](docs/QuotaEditLimitRequest.md)
          - [QuotaEditLimitRequestDetails](docs/QuotaEditLimitRequestDetails.md)
          - [QuotaEditLimitRequestDetailsAllOf](docs/QuotaEditLimitRequestDetailsAllOf.md)
          - [RelinquishIpBlock](docs/RelinquishIpBlock.md)
          - [ResetResult](docs/ResetResult.md)
          - [Server](docs/Server.md)
          - [ServerCreate](docs/ServerCreate.md)
          - [ServerIpBlock](docs/ServerIpBlock.md)
+         - [ServerNetworkUpdate](docs/ServerNetworkUpdate.md)
          - [ServerPatch](docs/ServerPatch.md)
          - [ServerPrivateNetwork](docs/ServerPrivateNetwork.md)
          - [ServerPublicNetwork](docs/ServerPublicNetwork.md)
          - [ServerReserve](docs/ServerReserve.md)
          - [ServerReset](docs/ServerReset.md)
          - [SshKey](docs/SshKey.md)
          - [SshKeyCreate](docs/SshKeyCreate.md)
```

### Comparing `pnap-bmc-api-1.3.0/setup.py` & `pnap-bmc-api-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/rest.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/rest.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,16 +185,16 @@
     def _from_openapi_data(cls, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, *args, **kwargs):  # noqa: E501
         """Server - a model defined in OpenAPI
 
         Args:
             id (str): The unique identifier of the server.
             status (str): The status of the server.
             hostname (str): Hostname of server.
-            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `debian/bullseye` or `proxmox/bullseye`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge` or `d2.c4.storage.pliops1`.
+            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
             cpu (str): A description of the machine CPU.
             cpu_count (int): The number of CPUs available in the system.
             cores_per_cpu (int): The number of physical cores present on each CPU.
             cpu_frequency (float): The CPU frequency in GHz.
             ram (str): A description of the machine RAM.
             storage (str): A description of the machine storage.
@@ -232,15 +232,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             public_ip_addresses ([str]): Public IP addresses assigned to server.. [optional]  # noqa: E501
             reservation_id (str): The reservation reference id if any.. [optional]  # noqa: E501
-            password (str): Password set for user Admin on Windows server or user root on ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            password (str): Auto-generated password set for user `Admin` on Windows server, user `root` on ESXi servers, user `root` on Proxmox server and user `netris` on Netris servers.<br> The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
             network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             cluster_id (str): The cluster reference id if any.. [optional]  # noqa: E501
             tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
             provisioned_on (datetime): Date and time when server was provisioned.. [optional]  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
         """
 
@@ -312,16 +312,16 @@
     def __init__(self, id, status, hostname, os, type, location, cpu, cpu_count, cores_per_cpu, cpu_frequency, ram, storage, private_ip_addresses, network_configuration, *args, **kwargs):  # noqa: E501
         """Server - a model defined in OpenAPI
 
         Args:
             id (str): The unique identifier of the server.
             status (str): The status of the server.
             hostname (str): Hostname of server.
-            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `debian/bullseye` or `proxmox/bullseye`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge` or `d2.c4.storage.pliops1`.
+            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
             cpu (str): A description of the machine CPU.
             cpu_count (int): The number of CPUs available in the system.
             cores_per_cpu (int): The number of physical cores present on each CPU.
             cpu_frequency (float): The CPU frequency in GHz.
             ram (str): A description of the machine RAM.
             storage (str): A description of the machine storage.
@@ -359,15 +359,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             description (str): Description of server.. [optional]  # noqa: E501
             public_ip_addresses ([str]): Public IP addresses assigned to server.. [optional]  # noqa: E501
             reservation_id (str): The reservation reference id if any.. [optional]  # noqa: E501
-            password (str): Password set for user Admin on Windows server or user root on ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            password (str): Auto-generated password set for user `Admin` on Windows server, user `root` on ESXi servers, user `root` on Proxmox server and user `netris` on Netris servers.<br> The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
             network_type (str): The type of network configuration for this server. Currently this field should be set to `PUBLIC_AND_PRIVATE` or `PRIVATE_ONLY`.. [optional] if omitted the server will use the default value of "PUBLIC_AND_PRIVATE"  # noqa: E501
             cluster_id (str): The cluster reference id if any.. [optional]  # noqa: E501
             tags ([TagAssignment]): The tags assigned if any.. [optional]  # noqa: E501
             provisioned_on (datetime): Date and time when server was provisioned.. [optional]  # noqa: E501
             os_configuration (OsConfiguration): [optional]  # noqa: E501
         """
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/error.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/error.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map_esxi.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_esxi.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            root_password (str): Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -228,16 +228,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            root_password (str): Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_cloud_init.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_cloud_init.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details_all_of.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/tag_assignment.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_ip_block.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_ip_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            vlan_id (int): The VLAN on which this IP block has been configured within the network switch.. [optional]  # noqa: E501
+            vlan_id (int): (Read-only) The VLAN on which this IP block has been configured within the network switch.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,15 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            vlan_id (int): The VLAN on which this IP block has been configured within the network switch.. [optional]  # noqa: E501
+            vlan_id (int): (Read-only) The VLAN on which this IP block has been configured within the network switch.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key_create.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_create.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/action_result.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/action_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key_update.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key_update.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/reset_result.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/reset_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/tag_assignment_request.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/tag_assignment_request.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_create.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, hostname, os, type, location, *args, **kwargs):  # noqa: E501
         """ServerCreate - a model defined in OpenAPI
 
         Args:
             hostname (str): Hostname of server.
-            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`,`centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `debian/bullseye` or `proxmox/bullseye`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge` or `d2.c4.storage.pliops1`.
+            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -253,16 +253,16 @@
 
     @convert_js_args_to_python_args
     def __init__(self, hostname, os, type, location, *args, **kwargs):  # noqa: E501
         """ServerCreate - a model defined in OpenAPI
 
         Args:
             hostname (str): Hostname of server.
-            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`,`centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `debian/bullseye` or `proxmox/bullseye`.
-            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge` or `d2.c4.storage.pliops1`.
+            os (str): The server’s OS ID used when the server was created. Currently this field should be set to either `ubuntu/bionic`, `ubuntu/focal`, `ubuntu/jammy`, `centos/centos7`, `centos/centos8`, `windows/srv2019std`, `windows/srv2019dc`, `esxi/esxi70`, `esxi/esxi80`, `debian/bullseye`, `proxmox/bullseye`, `netris/controller`, `netris/softgate_1g` or `netris/softgate_10g`.
+            type (str): Server type ID. Cannot be changed once a server is created. Currently this field should be set to either `s0.d1.small`, `s0.d1.medium`, `s1.c1.small`, `s1.c1.medium`, `s1.c2.medium`, `s1.c2.large`, `s1.e1.small`, `s1.e1.medium`, `s1.e1.large`, `s2.c1.small`, `s2.c1.medium`, `s2.c1.large`, `s2.c2.small`, `s2.c2.medium`, `s2.c2.large`, `d1.c1.small`, `d1.c2.small`, `d1.c3.small`, `d1.c4.small`, `d1.c1.medium`, `d1.c2.medium`, `d1.c3.medium`, `d1.c4.medium`, `d1.c1.large`, `d1.c2.large`, `d1.c3.large`, `d1.c4.large`, `d1.m1.medium`, `d1.m2.medium`, `d1.m3.medium`, `d1.m4.medium`, `d2.c1.medium`, `d2.c2.medium`, `d2.c3.medium`, `d2.c4.medium`, `d2.c5.medium`, `d2.c1.large`, `d2.c2.large`, `d2.c3.large`, `d2.c4.large`, `d2.c5.large`, `d2.m1.medium`, `d2.m1.large`, `d2.m2.medium`, `d2.m2.large`, `d2.m2.xlarge`, `d2.c4.storage.pliops1`, `d3.m4.xlarge`, `d3.m5.xlarge` or `d3.m6.xlarge`.
             location (str): Server location ID. Cannot be changed once a server is created. Currently this field should be set to `PHX`, `ASH`, `SGP`, `NLD`, `CHI`, `SEA` or `AUS`.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_private_network.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_private_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             ips ([str]): IPs to configure/configured on the server.<br> Should be null or empty list if DHCP is true. IPs must be within the network's range.<br> If field is undefined and DHCP is false, next available IP in network will be automatically allocated.<br> If the network contains a membership of type 'storage', the first twelve IPs are already reserved by BMC and not usable.<br> Setting the `force` query parameter to `true` allows you to:<ul> <li> Assign no specific IP addresses by designating an empty array of IPs. Note that at least one IP is required for the gateway address to be selected from this network. <li> Assign one or more IP addresses which are already configured on other resource(s) in network.</ul>. [optional]  # noqa: E501
             dhcp (bool): Determines whether DHCP is enabled for this server. Should be false if any IPs are provided. Not supported for Proxmox OS and ESXi OS.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            status_description (str): The status of the network.. [optional]  # noqa: E501
+            status_description (str): (Read-only) The status of the network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,15 +238,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             ips ([str]): IPs to configure/configured on the server.<br> Should be null or empty list if DHCP is true. IPs must be within the network's range.<br> If field is undefined and DHCP is false, next available IP in network will be automatically allocated.<br> If the network contains a membership of type 'storage', the first twelve IPs are already reserved by BMC and not usable.<br> Setting the `force` query parameter to `true` allows you to:<ul> <li> Assign no specific IP addresses by designating an empty array of IPs. Note that at least one IP is required for the gateway address to be selected from this network. <li> Assign one or more IP addresses which are already configured on other resource(s) in network.</ul>. [optional]  # noqa: E501
             dhcp (bool): Determines whether DHCP is enabled for this server. Should be false if any IPs are provided. Not supported for Proxmox OS and ESXi OS.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            status_description (str): The status of the network.. [optional]  # noqa: E501
+            status_description (str): (Read-only) The status of the network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/delete_result.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/public_network_configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/public_network_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/ssh_key.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_reset.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reset.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_windows.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_windows.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/private_network_configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/private_network_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gateway_address (str): Deprecated in favour of a common gateway address across all networks available under NetworkConfiguration.<br> The address of the gateway assigned / to assign to the server.<br> When used as part of request body, IP address has to be part of private network assigned to this server.<br> Gateway address also has to be assigned on an already deployed resource unless the `force` query parameter is true.. [optional]  # noqa: E501
-            configuration_type (str): Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
             private_networks ([ServerPrivateNetwork]): The list of private networks this server is member of. When this field is part of request body, it'll be used to specify the private networks to assign to this server upon provisioning. Used alongside the `USER_DEFINED` configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -230,15 +230,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             gateway_address (str): Deprecated in favour of a common gateway address across all networks available under NetworkConfiguration.<br> The address of the gateway assigned / to assign to the server.<br> When used as part of request body, IP address has to be part of private network assigned to this server.<br> Gateway address also has to be assigned on an already deployed resource unless the `force` query parameter is true.. [optional]  # noqa: E501
-            configuration_type (str): Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring private network(s) for the server being provisioned. Currently this field should be set to `USE_OR_CREATE_DEFAULT` or `USER_DEFINED`.. [optional] if omitted the server will use the default value of "USE_OR_CREATE_DEFAULT"  # noqa: E501
             private_networks ([ServerPrivateNetwork]): The list of private networks this server is member of. When this field is part of request body, it'll be used to specify the private networks to assign to this server upon provisioning. Used alongside the `USER_DEFINED` configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/network_configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/network_configuration.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/delete_ssh_key_result.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/delete_ssh_key_result.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_reserve.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_reserve.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/relinquish_ip_block.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/relinquish_ip_block.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,20 @@
     OpenApiModel
 )
 from pnap_bmc_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from pnap_bmc_api.model.os_configuration_cloud_init import OsConfigurationCloudInit
+    from pnap_bmc_api.model.os_configuration_netris_controller import OsConfigurationNetrisController
+    from pnap_bmc_api.model.os_configuration_netris_softgate import OsConfigurationNetrisSoftgate
     from pnap_bmc_api.model.os_configuration_windows import OsConfigurationWindows
     globals()['OsConfigurationCloudInit'] = OsConfigurationCloudInit
+    globals()['OsConfigurationNetrisController'] = OsConfigurationNetrisController
+    globals()['OsConfigurationNetrisSoftgate'] = OsConfigurationNetrisSoftgate
     globals()['OsConfigurationWindows'] = OsConfigurationWindows
 
 
 class OsConfiguration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -89,28 +93,32 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'netris_controller': (OsConfigurationNetrisController,),  # noqa: E501
+            'netris_softgate': (OsConfigurationNetrisSoftgate,),  # noqa: E501
             'windows': (OsConfigurationWindows,),  # noqa: E501
             'root_password': (str,),  # noqa: E501
             'management_ui_url': (str,),  # noqa: E501
             'management_access_allowed_ips': ([str],),  # noqa: E501
             'install_os_to_ram': (bool,),  # noqa: E501
             'cloud_init': (OsConfigurationCloudInit,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'netris_controller': 'netrisController',  # noqa: E501
+        'netris_softgate': 'netrisSoftgate',  # noqa: E501
         'windows': 'windows',  # noqa: E501
         'root_password': 'rootPassword',  # noqa: E501
         'management_ui_url': 'managementUiUrl',  # noqa: E501
         'management_access_allowed_ips': 'managementAccessAllowedIps',  # noqa: E501
         'install_os_to_ram': 'installOsToRam',  # noqa: E501
         'cloud_init': 'cloudInit',  # noqa: E501
     }
@@ -154,19 +162,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            netris_controller (OsConfigurationNetrisController): [optional]  # noqa: E501
+            netris_softgate (OsConfigurationNetrisSoftgate): [optional]  # noqa: E501
             windows (OsConfigurationWindows): [optional]  # noqa: E501
-            root_password (str): Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Auto-generated password set for user 'root' on an ESXi or Proxmox server.<br>  The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            install_os_to_ram (bool): If true, OS will be installed to and booted from the server's RAM. On restart RAM OS will be lost and the server will not be reachable unless a custom bootable OS has been deployed. Only supported for ubuntu/focal and ubuntu/jammy.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            install_os_to_ram (bool): If true, OS will be installed to and booted from the server's RAM. On restart RAM OS will be lost and the server will not be reachable unless a custom bootable OS has been deployed. Follow the <a href='https://phoenixnap.com/kb/bmc-custom-os' target='_blank'>instructions</a> on how to install custom OS on BMC. Only supported for ubuntu/focal and ubuntu/jammy.. [optional] if omitted the server will use the default value of False  # noqa: E501
             cloud_init (OsConfigurationCloudInit): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -245,19 +255,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            netris_controller (OsConfigurationNetrisController): [optional]  # noqa: E501
+            netris_softgate (OsConfigurationNetrisSoftgate): [optional]  # noqa: E501
             windows (OsConfigurationWindows): [optional]  # noqa: E501
-            root_password (str): Password set for user root on an ESXi server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Auto-generated password set for user 'root' on an ESXi or Proxmox server.<br>  The password is not stored and therefore will only be returned in response to provisioning a server. Copy and save it for future reference.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            install_os_to_ram (bool): If true, OS will be installed to and booted from the server's RAM. On restart RAM OS will be lost and the server will not be reachable unless a custom bootable OS has been deployed. Only supported for ubuntu/focal and ubuntu/jammy.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            install_os_to_ram (bool): If true, OS will be installed to and booted from the server's RAM. On restart RAM OS will be lost and the server will not be reachable unless a custom bootable OS has been deployed. Follow the <a href='https://phoenixnap.com/kb/bmc-custom-os' target='_blank'>instructions</a> on how to install custom OS on BMC. Only supported for ubuntu/focal and ubuntu/jammy.. [optional] if omitted the server will use the default value of False  # noqa: E501
             cloud_init (OsConfigurationCloudInit): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota_edit_limit_request_details.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota_edit_limit_request_details.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_patch.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_patch.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/ip_blocks_configuration.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/ip_blocks_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            configuration_type (str): Determines the approach for configuring IP blocks for the server being provisioned. If PURCHASE_NEW is selected, the smallest supported range, depending on the operating system, is allocated to the server.. [optional] if omitted the server will use the default value of "PURCHASE_NEW"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring IP blocks for the server being provisioned. If PURCHASE_NEW is selected, the smallest supported range, depending on the operating system, is allocated to the server.. [optional] if omitted the server will use the default value of "PURCHASE_NEW"  # noqa: E501
             ip_blocks ([ServerIpBlock]): Used to specify the previously purchased IP blocks to assign to this server upon provisioning. Used alongside the USER_DEFINED configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -234,15 +234,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            configuration_type (str): Determines the approach for configuring IP blocks for the server being provisioned. If PURCHASE_NEW is selected, the smallest supported range, depending on the operating system, is allocated to the server.. [optional] if omitted the server will use the default value of "PURCHASE_NEW"  # noqa: E501
+            configuration_type (str): (Write-only) Determines the approach for configuring IP blocks for the server being provisioned. If PURCHASE_NEW is selected, the smallest supported range, depending on the operating system, is allocated to the server.. [optional] if omitted the server will use the default value of "PURCHASE_NEW"  # noqa: E501
             ip_blocks ([ServerIpBlock]): Used to specify the previously purchased IP blocks to assign to this server upon provisioning. Used alongside the USER_DEFINED configurationType.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/server_public_network.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/server_public_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             ips ([str]): Configurable/configured IPs on the server.<br> At least 1 IP address is required. All IPs must be within the network's range.<br> Setting the `force` query parameter to `true` allows you to:<ul> <li> Assign no specific IP addresses by designating an empty array of IPs. Note that at least one IP is required for the gateway address to be selected from this network. <li> Assign one or more IP addresses which are already configured on other resource(s) in network.</ul>. [optional]  # noqa: E501
-            status_description (str): The status of the assignment to the network.. [optional]  # noqa: E501
+            status_description (str): (Read-only) The status of the assignment to the network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -231,15 +231,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             ips ([str]): Configurable/configured IPs on the server.<br> At least 1 IP address is required. All IPs must be within the network's range.<br> Setting the `force` query parameter to `true` allows you to:<ul> <li> Assign no specific IP addresses by designating an empty array of IPs. Note that at least one IP is required for the gateway address to be selected from this network. <li> Assign one or more IP addresses which are already configured on other resource(s) in network.</ul>. [optional]  # noqa: E501
-            status_description (str): The status of the assignment to the network.. [optional]  # noqa: E501
+            status_description (str): (Read-only) The status of the assignment to the network.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/os_configuration_map_proxmox.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/os_configuration_map_proxmox.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            root_password (str): Password set for user root on a Proxmox server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Password set for user root on a Proxmox server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -228,16 +228,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            root_password (str): Password set for user root on a Proxmox server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
-            management_ui_url (str): The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            root_password (str): (Read-only) Password set for user root on a Proxmox server which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
+            management_ui_url (str): (Read-only) The URL of the management UI which will only be returned in response to provisioning a server.. [optional]  # noqa: E501
             management_access_allowed_ips ([str]): List of IPs allowed to access the Management UI. Supported in single IP, CIDR and range format. When undefined, Management UI is disabled. This will only be returned in response to provisioning a server.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model/quota.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model/quota.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/__init__.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/api_client.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/api_client.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/exceptions.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/api/ssh_keys_api.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/api/ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/api/quotas_api.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/api/quotas_api.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/api/servers_api.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/api/servers_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pnap_bmc_api.model.delete_result import DeleteResult
 from pnap_bmc_api.model.error import Error
 from pnap_bmc_api.model.relinquish_ip_block import RelinquishIpBlock
 from pnap_bmc_api.model.reset_result import ResetResult
 from pnap_bmc_api.model.server import Server
 from pnap_bmc_api.model.server_create import ServerCreate
 from pnap_bmc_api.model.server_ip_block import ServerIpBlock
+from pnap_bmc_api.model.server_network_update import ServerNetworkUpdate
 from pnap_bmc_api.model.server_patch import ServerPatch
 from pnap_bmc_api.model.server_private_network import ServerPrivateNetwork
 from pnap_bmc_api.model.server_public_network import ServerPublicNetwork
 from pnap_bmc_api.model.server_reserve import ServerReserve
 from pnap_bmc_api.model.server_reset import ServerReset
 from pnap_bmc_api.model.tag_assignment_request import TagAssignmentRequest
 
@@ -861,14 +862,82 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.servers_server_id_private_networks_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (ServerPrivateNetwork,),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/servers/{serverId}/network-configuration/private-network-configuration/private-networks/{privateNetworkId}',
+                'operation_id': 'servers_server_id_private_networks_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'server_id',
+                    'private_network_id',
+                    'force',
+                    'server_network_update',
+                ],
+                'required': [
+                    'server_id',
+                    'private_network_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'server_id':
+                        (str,),
+                    'private_network_id':
+                        (str,),
+                    'force':
+                        (bool,),
+                    'server_network_update':
+                        (ServerNetworkUpdate,),
+                },
+                'attribute_map': {
+                    'server_id': 'serverId',
+                    'private_network_id': 'privateNetworkId',
+                    'force': 'force',
+                },
+                'location_map': {
+                    'server_id': 'path',
+                    'private_network_id': 'path',
+                    'force': 'query',
+                    'server_network_update': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.servers_server_id_private_networks_post_endpoint = _Endpoint(
             settings={
                 'response_type': (ServerPrivateNetwork,),
                 'auth': [
                     'OAuth2'
                 ],
                 'endpoint_path': '/servers/{serverId}/network-configuration/private-network-configuration/private-networks',
@@ -980,14 +1049,82 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.servers_server_id_public_networks_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (ServerPublicNetwork,),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/servers/{serverId}/network-configuration/public-network-configuration/public-networks/{publicNetworkId}',
+                'operation_id': 'servers_server_id_public_networks_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'server_id',
+                    'public_network_id',
+                    'force',
+                    'server_network_update',
+                ],
+                'required': [
+                    'server_id',
+                    'public_network_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'server_id':
+                        (str,),
+                    'public_network_id':
+                        (str,),
+                    'force':
+                        (bool,),
+                    'server_network_update':
+                        (ServerNetworkUpdate,),
+                },
+                'attribute_map': {
+                    'server_id': 'serverId',
+                    'public_network_id': 'publicNetworkId',
+                    'force': 'force',
+                },
+                'location_map': {
+                    'server_id': 'path',
+                    'public_network_id': 'path',
+                    'force': 'query',
+                    'server_network_update': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.servers_server_id_public_networks_post_endpoint = _Endpoint(
             settings={
                 'response_type': (ServerPublicNetwork,),
                 'auth': [
                     'OAuth2'
                 ],
                 'endpoint_path': '/servers/{serverId}/network-configuration/public-network-configuration/public-networks',
@@ -2352,14 +2489,103 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['server_id'] = \
             server_id
         return self.servers_server_id_patch_endpoint.call_with_http_info(**kwargs)
 
+    def servers_server_id_private_networks_patch(
+        self,
+        server_id,
+        private_network_id,
+        **kwargs
+    ):
+        """Updates the server's private network's IP addresses  # noqa: E501
+
+        IP address changes intended to keep the BMC data up to date with server's operating system. We do not have access to the server's operating system and therefore manual configuration is required to apply the changes on the host. Knowledge base article to help you can be found <a href='https://phoenixnap.com/kb/bmc-server-management-via-api#ftoc-heading-6' target='_blank'>here</a>  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.servers_server_id_private_networks_patch(server_id, private_network_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            server_id (str): The server's ID.
+            private_network_id (str): The private network identifier.
+
+        Keyword Args:
+            force (bool): Query parameter controlling advanced features availability. Currently applicable for networking. It is advised to use with caution since it might lead to unhealthy setups.. [optional] if omitted the server will use the default value of False
+            server_network_update (ServerNetworkUpdate): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ServerPrivateNetwork
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['server_id'] = \
+            server_id
+        kwargs['private_network_id'] = \
+            private_network_id
+        return self.servers_server_id_private_networks_patch_endpoint.call_with_http_info(**kwargs)
+
     def servers_server_id_private_networks_post(
         self,
         server_id,
         **kwargs
     ):
         """Adds the server to a private network.  # noqa: E501
 
@@ -2524,14 +2750,103 @@
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['server_id'] = \
             server_id
         kwargs['public_network_id'] = \
             public_network_id
         return self.servers_server_id_public_networks_delete_endpoint.call_with_http_info(**kwargs)
 
+    def servers_server_id_public_networks_patch(
+        self,
+        server_id,
+        public_network_id,
+        **kwargs
+    ):
+        """Updates the server's public network's IP addresses.  # noqa: E501
+
+        IP address changes intended to keep the BMC data up to date with server's operating system. We do not have access to the server's operating system and therefore manual configuration is required to apply the changes on the host. Knowledge base article to help you can be found <a href='https://phoenixnap.com/kb/bmc-server-management-via-api#ftoc-heading-6' target='_blank'>here</a>  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.servers_server_id_public_networks_patch(server_id, public_network_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            server_id (str): The server's ID.
+            public_network_id (str): The Public Network identifier.
+
+        Keyword Args:
+            force (bool): Query parameter controlling advanced features availability. Currently applicable for networking. It is advised to use with caution since it might lead to unhealthy setups.. [optional] if omitted the server will use the default value of False
+            server_network_update (ServerNetworkUpdate): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ServerPublicNetwork
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['server_id'] = \
+            server_id
+        kwargs['public_network_id'] = \
+            public_network_id
+        return self.servers_server_id_public_networks_patch_endpoint.call_with_http_info(**kwargs)
+
     def servers_server_id_public_networks_post(
         self,
         server_id,
         **kwargs
     ):
         """Adds the server to a Public Network.  # noqa: E501
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/models/__init__.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 from pnap_bmc_api.model.ip_blocks_configuration import IpBlocksConfiguration
 from pnap_bmc_api.model.network_configuration import NetworkConfiguration
 from pnap_bmc_api.model.os_configuration import OsConfiguration
 from pnap_bmc_api.model.os_configuration_cloud_init import OsConfigurationCloudInit
 from pnap_bmc_api.model.os_configuration_map import OsConfigurationMap
 from pnap_bmc_api.model.os_configuration_map_esxi import OsConfigurationMapEsxi
 from pnap_bmc_api.model.os_configuration_map_proxmox import OsConfigurationMapProxmox
+from pnap_bmc_api.model.os_configuration_netris_controller import OsConfigurationNetrisController
+from pnap_bmc_api.model.os_configuration_netris_softgate import OsConfigurationNetrisSoftgate
 from pnap_bmc_api.model.os_configuration_windows import OsConfigurationWindows
 from pnap_bmc_api.model.private_network_configuration import PrivateNetworkConfiguration
 from pnap_bmc_api.model.public_network_configuration import PublicNetworkConfiguration
 from pnap_bmc_api.model.quota import Quota
 from pnap_bmc_api.model.quota_edit_limit_request import QuotaEditLimitRequest
 from pnap_bmc_api.model.quota_edit_limit_request_details import QuotaEditLimitRequestDetails
 from pnap_bmc_api.model.quota_edit_limit_request_details_all_of import QuotaEditLimitRequestDetailsAllOf
 from pnap_bmc_api.model.relinquish_ip_block import RelinquishIpBlock
 from pnap_bmc_api.model.reset_result import ResetResult
 from pnap_bmc_api.model.server import Server
 from pnap_bmc_api.model.server_create import ServerCreate
 from pnap_bmc_api.model.server_ip_block import ServerIpBlock
+from pnap_bmc_api.model.server_network_update import ServerNetworkUpdate
 from pnap_bmc_api.model.server_patch import ServerPatch
 from pnap_bmc_api.model.server_private_network import ServerPrivateNetwork
 from pnap_bmc_api.model.server_public_network import ServerPublicNetwork
 from pnap_bmc_api.model.server_reserve import ServerReserve
 from pnap_bmc_api.model.server_reset import ServerReset
 from pnap_bmc_api.model.ssh_key import SshKey
 from pnap_bmc_api.model.ssh_key_create import SshKeyCreate
```

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/model_utils.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `pnap-bmc-api-1.3.0/pnap_bmc_api/apis/__init__.py` & `pnap-bmc-api-1.4.0/pnap_bmc_api/apis/__init__.py`

 * *Files identical despite different names*

