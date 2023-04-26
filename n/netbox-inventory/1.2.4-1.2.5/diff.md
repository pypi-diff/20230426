# Comparing `tmp/netbox-inventory-1.2.4.tar.gz` & `tmp/netbox-inventory-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.2.4.tar", last modified: Fri Apr 21 16:16:23 2023, max compression
+gzip compressed data, was "netbox-inventory-1.2.5.tar", last modified: Wed Apr 26 11:31:54 2023, max compression
```

## Comparing `netbox-inventory-1.2.4.tar` & `netbox-inventory-1.2.5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.087334 netbox-inventory-1.2.4/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.087334 netbox-inventory-1.2.4/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.079334 netbox-inventory-1.2.4/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.091333 netbox-inventory-1.2.4/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.095333 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:16:23.083334 netbox-inventory-1.2.4/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 16:16:23.000000 netbox-inventory-1.2.4/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 16:16:11.000000 netbox-inventory-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:16:23.099333 netbox-inventory-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.476765 netbox-inventory-1.2.5/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.480765 netbox-inventory-1.2.5/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.488765 netbox-inventory-1.2.5/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.492765 netbox-inventory-1.2.5/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.460765 netbox-inventory-1.2.5/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.500765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.500765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.504765 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.508765 netbox-inventory-1.2.5/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.512765 netbox-inventory-1.2.5/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.512765 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.516765 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:31:54.480765 netbox-inventory-1.2.5/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 11:31:54.000000 netbox-inventory-1.2.5/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 11:31:43.000000 netbox-inventory-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:31:54.524765 netbox-inventory-1.2.5/setup.cfg
```

### Comparing `netbox-inventory-1.2.4/LICENSE` & `netbox-inventory-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/PKG-INFO` & `netbox-inventory-1.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-inventory
-Version: 1.2.4
-Summary: Inventory asset management in NetBox
-Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
-Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
-Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
-Keywords: netbox,netbox-plugin,inventory
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NetBox Inventory Plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin for hardware inventory.
 
 ## Features
 
 Keep track of your hardware, whether it is installed or in storage. You can
@@ -164,14 +149,16 @@
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
+| `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
+| `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
     'netbox_inventory.Asset.status+': (
         ('repair', 'In repair', 'orange'),
```

### Comparing `netbox-inventory-1.2.4/README.md` & `netbox-inventory-1.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: netbox-inventory
+Version: 1.2.5
+Summary: Inventory asset management in NetBox
+Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
+Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
+Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
+Keywords: netbox,netbox-plugin,inventory
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # NetBox Inventory Plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin for hardware inventory.
 
 ## Features
 
 Keep track of your hardware, whether it is installed or in storage. You can
@@ -149,14 +164,16 @@
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
+| `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
+| `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
     'netbox_inventory.Asset.status+': (
         ('repair', 'In repair', 'orange'),
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/__init__.py` & `netbox-inventory-1.2.5/netbox_inventory/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
         'asset_import_create_module_type': False,
         'asset_import_create_inventoryitem_type': False,
         'asset_import_create_tenant': False,
         'asset_disable_editing_fields_for_tags': {},
         'asset_disable_deletion_for_tags': [],
+        'prefill_asset_name_create_inventoryitem': False,
+        'prefill_asset_tag_create_inventoryitem': False,
     }
 
     def ready(self):
         super().ready()
         import netbox_inventory.signals
 
 config = NetBoxInventoryConfig
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/analyzers.py` & `netbox-inventory-1.2.5/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.2.5/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/api/serializers.py` & `netbox-inventory-1.2.5/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/api/urls.py` & `netbox-inventory-1.2.5/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/api/views.py` & `netbox-inventory-1.2.5/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/filtersets.py` & `netbox-inventory-1.2.5/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/assign.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,33 +75,44 @@
     )
     warranty_start = forms.CharField(
         required=False,
     )
     warranty_end = forms.CharField(
         required=False,
     )
+    tenant = DynamicModelChoiceField(
+        queryset=Tenant.objects.all(),
+        help_text=Asset._meta.get_field('tenant').help_text,
+        required=not Asset._meta.get_field('tenant').blank,
+    )
+    contact = DynamicModelChoiceField(
+        queryset=Contact.objects.all(),
+        help_text=Asset._meta.get_field('contact').help_text,
+        required=not Asset._meta.get_field('contact').blank,
+    )
     storage_location = DynamicModelChoiceField(
         queryset=Location.objects.all(),
         help_text=Asset._meta.get_field('storage_location').help_text,
         required=False,
     )
     comments = CommentField(
         required=False,
     )
 
     model = Asset
     fieldsets = (
         ('General', ('name', 'status')),
         ('Hardware', ('device_type', 'device', 'module_type', 'module')),
         ('Purchase', ('owner', 'purchase', 'warranty_start', 'warranty_end')), 
+        ('Assigned to', ('tenant', 'contact')), 
         ('Location', ('storage_location',)),
     )
     nullable_fields = (
-        'name', 'device', 'module', 'owner', 'purchase', 'warranty_start',
-        'warranty_end',
+        'name', 'device', 'module', 'owner', 'purchase', 'tenant', 'contact',
+        'warranty_start', 'warranty_end',
     )
 
 
 class AssetImportForm(NetBoxModelImportForm):
     hardware_kind = CSVChoiceField(
         choices=HardwareKindChoices,
         required=True,
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/create.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 
 from dcim.forms import DeviceForm, InventoryItemForm, ModuleForm
 from dcim.models.device_components import ConsolePort, ConsoleServerPort, FrontPort, Interface, PowerOutlet, PowerPort, RearPort
 from utilities.forms import DynamicModelChoiceField, StaticSelect
+from ..utils import get_plugin_setting
 
 __all__ = (
     'AssetDeviceCreateForm',
     'AssetModuleCreateForm',
     'AssetInventoryItemCreateForm',
 )
 
@@ -150,14 +151,19 @@
             self.fields['serial'].disabled = True
             self.fields['asset_tag'].disabled = True
             self.fields['part_id'].disabled = True
             self.initial['serial'] = asset.serial
             self.initial['asset_tag'] = asset.asset_tag if asset.asset_tag else None
             self.initial['part_id'] = asset.inventoryitem_type.part_number or asset.inventoryitem_type.model
 
+            if get_plugin_setting('prefill_asset_name_create_inventoryitem'):
+                self.initial['name'] = asset.name if asset.name else None
+            if get_plugin_setting('prefill_asset_tag_create_inventoryitem'):
+                self.initial['tags'] = asset.tags.all() if asset.tags else None
+
             self.fields['manufacturer'].widget = StaticSelect(attrs={'readonly':True, 'disabled':True})
             self.fields['manufacturer'].choices = [(asset.inventoryitem_type.manufacturer.pk, asset.inventoryitem_type.manufacturer)]
 
     def clean(self):
         super().clean()
         component_set = None
         for field_name in COMPONENT_FIELDS:
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/filters.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/models.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelForm
 from netbox_inventory.choices import HardwareKindChoices
 from utilities.forms import CommentField, DatePicker, DynamicModelChoiceField, SlugField
-from tenancy.models import Tenant
+from tenancy.models import Contact, Tenant
 from ..models import Asset, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_tags_and_edit_protected_asset_fields
 
 __all__ = (
     'AssetForm',
     'SupplierForm',
     'PurchaseForm',
@@ -19,14 +19,15 @@
 
     manufacturer = DynamicModelChoiceField(
         queryset=Manufacturer.objects.all(),
         required=False,
         initial_params={
             'device_types': '$device_type',
             'module_types': '$module_type',
+            'inventoryitem_types': '$inventoryitem_type',
         },
     )
     device_type = DynamicModelChoiceField(
         queryset=DeviceType.objects.all(),
         required=False,
         query_params={
             'manufacturer_id': '$manufacturer',
@@ -53,14 +54,24 @@
         required=not Asset._meta.get_field('owner').blank,
     )
     purchase = DynamicModelChoiceField(
         queryset=Purchase.objects.all(),
         help_text=Asset._meta.get_field('purchase').help_text,
         required=not Asset._meta.get_field('purchase').blank,
     )
+    tenant = DynamicModelChoiceField(
+        queryset=Tenant.objects.all(),
+        help_text=Asset._meta.get_field('tenant').help_text,
+        required=not Asset._meta.get_field('tenant').blank,
+    )
+    contact = DynamicModelChoiceField(
+        queryset=Contact.objects.all(),
+        help_text=Asset._meta.get_field('contact').help_text,
+        required=not Asset._meta.get_field('contact').blank,
+    )
     storage_site = DynamicModelChoiceField(
         queryset=Site.objects.all(),
         required=False,
         initial_params={
             'locations': '$storage_location',
         },
     )
@@ -92,14 +103,21 @@
                 'owner',
                 'purchase',
                 'warranty_start',
                 'warranty_end',
             ),
         ),
         (
+            'Assigned to',
+            (
+                'tenant',
+                'contact',
+            ),
+        ),
+        (
             'Location',
             (
                 'storage_site',
                 'storage_location',
             ),
         ),
     )
@@ -116,29 +134,50 @@
             'module_type',
             'inventoryitem_type',
             'storage_location',
             'owner',
             'purchase',
             'warranty_start',
             'warranty_end',
+            'tenant',
+            'contact',
             'tags',
             'comments',
             'storage_site',
         )
         widgets = {
             'warranty_start': DatePicker(),
             'warranty_end': DatePicker(),
         }
 
     def __init__(self, *args, **kwargs):
-        """Override the default __init__ method to add custom logic to the form.
-        We need to disable fields that are not editable based on the tags that are assigned to the asset.
-        """
         super().__init__(*args, **kwargs)
 
+        self._disable_fields_by_tags()
+
+        # Used for picking the default active tab for hardware type selection
+        self.no_hardware_type = True
+        if self.instance:
+            if (self.instance.device_type or self.instance.module_type
+                or self.instance.inventoryitem_type):
+                self.no_hardware_type = False
+
+        # if assigned to device/module/inventoryitem we can't change device_type/...
+        if (
+            self.instance.device or self.instance.module
+            or self.instance.inventoryitem
+        ):
+            self.fields['manufacturer'].disabled = True
+            for kind in HardwareKindChoices.values():
+                self.fields[f'{kind}_type'].disabled = True
+
+    def _disable_fields_by_tags(self):
+        """
+        We need to disable fields that are not editable based on the tags that are assigned to the asset.
+        """
         if not self.instance.pk:
             # If we are creating a new asset we can't disable fields
             return
 
         # Disable fields that should not be edited
         tags = self.instance.tags.all().values_list('slug', flat=True)
         tags_and_disabled_fields = get_tags_and_edit_protected_asset_fields()
@@ -147,23 +186,14 @@
             if tag not in tags_and_disabled_fields:
                 continue
 
             for field in tags_and_disabled_fields[tag]:
                 if field in self.fields:
                     self.fields[field].disabled = True
 
-        # if assigned to device/module/inventoryitem we can't change device_type/...
-        if (
-            self.instance.device or self.instance.module
-            or self.instance.inventoryitem
-        ):
-            self.fields['manufacturer'].disabled = True
-            for kind in HardwareKindChoices.values():
-                self.fields[f'{kind}_type'].disabled = True
-
 
 class SupplierForm(NetBoxModelForm):
     slug = SlugField(slug_source='name')
     comments = CommentField()
 
     fieldsets = (('Supplier', ('name', 'slug', 'description', 'tags')),)
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.2.5/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.2.5/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.2.5/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.2.5/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/models.py` & `netbox-inventory-1.2.5/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/navigation.py` & `netbox-inventory-1.2.5/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/search.py` & `netbox-inventory-1.2.5/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/signals.py` & `netbox-inventory-1.2.5/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tables.py` & `netbox-inventory-1.2.5/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/template_content.py` & `netbox-inventory-1.2.5/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_tenant.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.2.5/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/custom.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/settings.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.2.5/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.2.4"
+        assert __version__ == "1.2.5"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/urls.py` & `netbox-inventory-1.2.5/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/utils.py` & `netbox-inventory-1.2.5/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/asset.py` & `netbox-inventory-1.2.5/netbox_inventory/views/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     filterset = filtersets.AssetFilterSet
     filterset_form = forms.AssetFilterForm
 
 
 class AssetBulkCreateView(generic.BulkCreateView):
     queryset = models.Asset.objects.all()
     form = forms.AssetBulkAddForm
-    model_form = forms.AssetForm
+    model_form = forms.AssetBulkAddModelForm
     pattern_target = None
     template_name = 'netbox_inventory/asset_bulk_add.html'
 
     def _create_objects(self, form, request):
         new_objects = []
         for _ in range(form.cleaned_data['count']):
             # Reinstantiate the model form each time to avoid overwriting the same instance. Use a mutable
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.2.5/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.2.5/netbox_inventory/views/asset_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,7 +56,12 @@
 
 class AssetInventoryItemCreateView(AssetCreateView):
     queryset = InventoryItem.objects.all()
     form = AssetInventoryItemCreateForm
 
     def get_object(self, **kwargs):
         return InventoryItem(assigned_asset=self.asset)
+
+    def get_extra_context(self, request, instance):
+        context = super().get_extra_context(request, instance)
+        context['template_extends'] = 'dcim/inventoryitem_edit.html'
+        return context
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.2.5/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.2.5/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/purchase.py` & `netbox-inventory-1.2.5/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/supplier.py` & `netbox-inventory-1.2.5/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory/views/tabs.py` & `netbox-inventory-1.2.5/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.2.5/netbox_inventory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.2.4
+Version: 1.2.5
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -164,14 +164,16 @@
 | `asset_import_create_purchase` | `False` | When importing assets, automatically create purchase (and supplier) if it doesn't exist |
 | `asset_import_create_device_type` | `False` | When importing a device type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_module_type` | `False` | When importing a module type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_inventoryitem_type` | `False` | When importing an inventory type asset, automatically create manufacturer and/or device type if it doesn't exist |
 | `asset_import_create_tenant` | `False` | When importing an asset, with owner or tenant, automatically create tenant if it doesn't exist |
 | `asset_disable_editing_fields_for_tags` | `{}` | A dictionary of tags and fields that should be disabled for editing. This is useful if you want to prevent editing of certain fields for certain assets. The dictionary is in the form of `{tag: [field1, field2]}`. Example: `{'no-edit': ['serial_number', 'asset_tag']}`. This only affects the UI, the API can still be used to edit the fields. |
 | `asset_disable_deletion_for_tags` | `[]` | List of tags that will disable deletion of assets. This only affects the UI, not the API. |
+| `prefill_asset_name_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the InventoryItem name to match the asset name. |
+| `prefill_asset_tag_create_inventoryitem` | `False` | When hardware inventory item is created from an asset, prefill the tags to match the tags associated to the asset. |
 
 You can extend or define your own status choices for Asset, via [`FIELD_CHOICES`](https://docs.netbox.dev/en/stable/configuration/data-validation/#field_choices) setting in Netbox:
 
 ```
 FIELD_CHOICES = {
     'netbox_inventory.Asset.status+': (
         ('repair', 'In repair', 'orange'),
```

### Comparing `netbox-inventory-1.2.4/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.2.5/netbox_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.2.4/pyproject.toml` & `netbox-inventory-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

