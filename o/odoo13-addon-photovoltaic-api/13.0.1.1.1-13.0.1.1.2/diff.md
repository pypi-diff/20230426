# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.1.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.1.tar", last modified: Thu Apr 20 10:15:45 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.2.tar", last modified: Wed Apr 26 09:30:44 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.458816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.458816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.462816 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.463817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.463817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.464817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.467817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.468817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.470817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4651 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/account.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/allocations.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/contracts.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/info.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.471817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6052 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 10:15:45.473817 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-20 10:15:45.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 10:15:45.474817 odoo13-addon-photovoltaic_api-13.0.1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-20 10:15:23.000000 odoo13-addon-photovoltaic_api-13.0.1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.347264 odoo13-addon-photovoltaic_api-13.0.1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-26 09:30:44.347264 odoo13-addon-photovoltaic_api-13.0.1.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.331263 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.331263 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.335263 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.336264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.336264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.337263 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.340264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.340264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.343264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.344264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:30:44.346264 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 09:30:44.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 09:30:44.347264 odoo13-addon-photovoltaic_api-13.0.1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-26 09:30:21.000000 odoo13-addon-photovoltaic_api-13.0.1.1.2/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/CHANGELOG.md` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 All notable changes to this project will be documented in this file. (from version 13.0.1.1.0 onwards)
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [v13.0.1.1.1] - 20-04-2023
+## [13.0.1.1.2] - 26-04-2023
+
+### Fixed
+- User update process
+- Password regex to allow symbols
+
+## [13.0.1.1.1] - 20-04-2023
 
 ### Fixed
 - Selection of contacts on signup request
 
-## [v13.0.1.1.0] - 11-04-2023
+## [13.0.1.1.0] - 11-04-2023
 
 ### Fixed
 - Incorrect retrieval of account allocations
 - Count of allocations to use correct search domain
 - Naming of company users
 - Location of a user
 - Allocations shown based on check
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.1.1',
+    'version': '13.0.1.1.2',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         return {
             'vat':      {'type': 'string'}
         }
 
     def _validator_signup(self):
         return {
             'token':    {'type': 'string'},
-            'password': {'type': 'string', 'regex': '^(?=.*\d)(?=.*[a-zA-Z])[a-zA-Z0-9]{8,}$'}
+            'password': {'type': 'string', 'regex': '^(?=.*\d)(?=.*[a-zA-Z]).{8,}$'}
         }
 
     def _validator_login(self):
         return {
             'vat':      {'type': 'string'},
             'password': {'type': 'string'}
         }
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/powerstation.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/powerstation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/services/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     @restapi.method(
         [(['/'], 'PUT')],
         input_param=restapi.PydanticModel(UserIn),
         output_param=restapi.PydanticModel(UserOut)
     )
     def update(self, user_in):
-        duplicated_vat_partners = self.env['res.partner'].sudo().search([('vat', '=', user_in.vat)])
+        duplicated_vat_partners = self.env['res.partner'].sudo().search([('vat', '=', user_in.vat), ('participant', '=', True)])
         if user_in.vat and len(duplicated_vat_partners) > 0 and duplicated_vat_partners[0]['id'] != self.env.user.partner_id.id:
             raise UserError('vat already exists')
 
         user_dict = user_in.dict(exclude_unset=True, exclude={'representative', 'interests'})
         if (user_in.zip or user_in.state_id or user_in.country_id):
             user_dict['zip_id'] = None
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/common.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.1/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.2/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

