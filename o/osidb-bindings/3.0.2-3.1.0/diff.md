# Comparing `tmp/osidb-bindings-3.0.2.tar.gz` & `tmp/osidb-bindings-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osidb-bindings-3.0.2.tar", last modified: Tue Apr  4 15:24:33 2023, max compression
+gzip compressed data, was "osidb-bindings-3.1.0.tar", last modified: Wed Apr 26 21:08:58 2023, max compression
```

## Comparing `osidb-bindings-3.0.2.tar` & `osidb-bindings-3.1.0.tar`

### file list

```diff
@@ -1,188 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.844414 osidb-bindings-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-04 15:24:33.844414 osidb-bindings-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.804413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.804413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.808413 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.844414 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affectedness_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/blank_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/comment_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/epss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/erratum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    31074 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_source_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/impact_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/meta_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    22141 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/resolution_01f_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/resolution_3_ac_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/state_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/supported_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/type_0d0_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/osidb_bindings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.800413 osidb-bindings-3.0.2/osidb_bindings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-04 15:24:33.000000 osidb-bindings-3.0.2/osidb_bindings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-04 15:24:33.000000 osidb-bindings-3.0.2/osidb_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:24:33.000000 osidb-bindings-3.0.2/osidb_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 15:24:33.000000 osidb-bindings-3.0.2/osidb_bindings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 15:24:33.000000 osidb-bindings-3.0.2/osidb_bindings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:24:33.844414 osidb-bindings-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:33.844414 osidb-bindings-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-04 15:24:16.000000 osidb-bindings-3.0.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.473001 osidb-bindings-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-26 21:08:58.473001 osidb-bindings-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.449001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.449001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61427 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68872 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.449001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.453001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.469001 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18836 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18101 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affectedness_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/blank_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/comment_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/epss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/erratum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29673 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/impact_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_issue_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_issue_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_issue_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/jira_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/meta_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20632 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/resolution_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/source_666_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/supported_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/type_0d0_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/type_5b2_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/type_824_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/osidb_bindings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.445001 osidb-bindings-3.1.0/osidb_bindings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-26 21:08:58.000000 osidb-bindings-3.1.0/osidb_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-04-26 21:08:58.000000 osidb-bindings-3.1.0/osidb_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:08:58.000000 osidb-bindings-3.1.0/osidb_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 21:08:58.000000 osidb-bindings-3.1.0/osidb_bindings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 21:08:58.000000 osidb-bindings-3.1.0/osidb_bindings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:08:58.473001 osidb-bindings-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:58.473001 osidb-bindings-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-26 21:08:32.000000 osidb-bindings-3.1.0/tests/test_core.py
```

### Comparing `osidb-bindings-3.0.2/LICENSE` & `osidb-bindings-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/PKG-INFO` & `osidb-bindings-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.0.2
+Version: 3.1.0
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.0.2/README.md` & `osidb-bindings-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/__init__.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.affect import Affect
-from ...models.osidb_api_v1_affects_create_response_201 import (
-    OsidbApiV1AffectsCreateResponse201,
+from ...models.flaw_post import FlawPost
+from ...models.osidb_api_v1_flaws_create_response_201 import (
+    OsidbApiV1FlawsCreateResponse201,
 )
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = Affect
+REQUEST_BODY_TYPE = FlawPost
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/affects".format(
+    url = "{}/osidb/api/v1/flaws".format(
         client.base_url,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
@@ -39,45 +39,45 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1AffectsCreateResponse201]:
+) -> Optional[OsidbApiV1FlawsCreateResponse201]:
     if response.status_code == 201:
         _response_201 = response.json()
-        response_201: OsidbApiV1AffectsCreateResponse201
+        response_201: OsidbApiV1FlawsCreateResponse201
         if isinstance(_response_201, Unset):
             response_201 = UNSET
         else:
-            response_201 = OsidbApiV1AffectsCreateResponse201.from_dict(_response_201)
+            response_201 = OsidbApiV1FlawsCreateResponse201.from_dict(_response_201)
 
         return response_201
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1AffectsCreateResponse201]:
+) -> Response[OsidbApiV1FlawsCreateResponse201]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-) -> Response[OsidbApiV1AffectsCreateResponse201]:
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Response[OsidbApiV1FlawsCreateResponse201]:
     kwargs = _get_kwargs(
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
     )
 
@@ -91,18 +91,18 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
-    form_data: Affect,
-    multipart_data: Affect,
-    json_body: Affect,
-) -> Optional[OsidbApiV1AffectsCreateResponse201]:
+    form_data: FlawPost,
+    multipart_data: FlawPost,
+    json_body: FlawPost,
+) -> Optional[OsidbApiV1FlawsCreateResponse201]:
     """ """
 
     return sync_detailed(
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
 from ...models.flaw import Flaw
-from ...models.osidb_api_v1_flaws_create_response_201 import (
-    OsidbApiV1FlawsCreateResponse201,
+from ...models.osidb_api_v1_flaws_update_response_200 import (
+    OsidbApiV1FlawsUpdateResponse200,
 )
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
 REQUEST_BODY_TYPE = Flaw
 
 
 def _get_kwargs(
+    id: str,
     *,
     client: AuthenticatedClient,
     form_data: Flaw,
     multipart_data: Flaw,
     json_body: Flaw,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/flaws".format(
+    url = "{}/osidb/api/v1/flaws/{id}".format(
         client.base_url,
+        id=id,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
     json_json_body: Dict[str, Any] = UNSET
     if not isinstance(json_body, Unset):
         json_body.to_dict()
@@ -39,71 +41,75 @@
         "headers": headers,
         "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1FlawsCreateResponse201]:
-    if response.status_code == 201:
-        _response_201 = response.json()
-        response_201: OsidbApiV1FlawsCreateResponse201
-        if isinstance(_response_201, Unset):
-            response_201 = UNSET
+) -> Optional[OsidbApiV1FlawsUpdateResponse200]:
+    if response.status_code == 200:
+        _response_200 = response.json()
+        response_200: OsidbApiV1FlawsUpdateResponse200
+        if isinstance(_response_200, Unset):
+            response_200 = UNSET
         else:
-            response_201 = OsidbApiV1FlawsCreateResponse201.from_dict(_response_201)
+            response_200 = OsidbApiV1FlawsUpdateResponse200.from_dict(_response_200)
 
-        return response_201
+        return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1FlawsCreateResponse201]:
+) -> Response[OsidbApiV1FlawsUpdateResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    id: str,
     *,
     client: AuthenticatedClient,
     form_data: Flaw,
     multipart_data: Flaw,
     json_body: Flaw,
-) -> Response[OsidbApiV1FlawsCreateResponse201]:
+) -> Response[OsidbApiV1FlawsUpdateResponse200]:
     kwargs = _get_kwargs(
+        id=id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
     )
 
-    response = requests.post(
+    response = requests.put(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
+    id: str,
     *,
     client: AuthenticatedClient,
     form_data: Flaw,
     multipart_data: Flaw,
     json_body: Flaw,
-) -> Optional[OsidbApiV1FlawsCreateResponse201]:
+) -> Optional[OsidbApiV1FlawsUpdateResponse200]:
     """ """
 
     return sync_detailed(
+        id=id,
         client=client,
         form_data=form_data,
         multipart_data=multipart_data,
         json_body=json_body,
     ).parsed
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,96 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from ...client import AuthenticatedClient
-from ...models.flaw import Flaw
-from ...models.osidb_api_v1_flaws_update_response_200 import (
-    OsidbApiV1FlawsUpdateResponse200,
+from ...models.taskman_api_v1_task_retrieve_response_200 import (
+    TaskmanApiV1TaskRetrieveResponse200,
 )
 from ...types import UNSET, Response, Unset
 
 QUERY_PARAMS = {}
-REQUEST_BODY_TYPE = Flaw
 
 
 def _get_kwargs(
-    id: str,
+    task_key: str,
     *,
     client: AuthenticatedClient,
-    form_data: Flaw,
-    multipart_data: Flaw,
-    json_body: Flaw,
+    jira_authentication: str,
 ) -> Dict[str, Any]:
-    url = "{}/osidb/api/v1/flaws/{id}".format(
+    url = "{}/taskman/api/v1/task/{task_key}".format(
         client.base_url,
-        id=id,
+        task_key=task_key,
     )
 
     headers: Dict[str, Any] = client.get_headers()
 
-    json_json_body: Dict[str, Any] = UNSET
-    if not isinstance(json_body, Unset):
-        json_body.to_dict()
-
-    multipart_multipart_data: Dict[str, Any] = UNSET
-    if not isinstance(multipart_data, Unset):
-        multipart_data.to_multipart()
+    headers["jira-authentication"] = jira_authentication
 
     return {
         "url": url,
         "headers": headers,
-        "data": form_data.to_dict(),
     }
 
 
 def _parse_response(
     *, response: requests.Response
-) -> Optional[OsidbApiV1FlawsUpdateResponse200]:
+) -> Optional[TaskmanApiV1TaskRetrieveResponse200]:
     if response.status_code == 200:
         _response_200 = response.json()
-        response_200: OsidbApiV1FlawsUpdateResponse200
+        response_200: TaskmanApiV1TaskRetrieveResponse200
         if isinstance(_response_200, Unset):
             response_200 = UNSET
         else:
-            response_200 = OsidbApiV1FlawsUpdateResponse200.from_dict(_response_200)
+            response_200 = TaskmanApiV1TaskRetrieveResponse200.from_dict(_response_200)
 
         return response_200
     return None
 
 
 def _build_response(
     *, response: requests.Response
-) -> Response[OsidbApiV1FlawsUpdateResponse200]:
+) -> Response[TaskmanApiV1TaskRetrieveResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: str,
+    task_key: str,
     *,
     client: AuthenticatedClient,
-    form_data: Flaw,
-    multipart_data: Flaw,
-    json_body: Flaw,
-) -> Response[OsidbApiV1FlawsUpdateResponse200]:
+    jira_authentication: str,
+) -> Response[TaskmanApiV1TaskRetrieveResponse200]:
     kwargs = _get_kwargs(
-        id=id,
+        task_key=task_key,
         client=client,
-        form_data=form_data,
-        multipart_data=multipart_data,
-        json_body=json_body,
+        jira_authentication=jira_authentication,
     )
 
-    response = requests.put(
+    response = requests.get(
         verify=client.verify_ssl,
         auth=client.auth,
         timeout=client.timeout,
         **kwargs,
     )
     response.raise_for_status()
 
     return _build_response(response=response)
 
 
 def sync(
-    id: str,
+    task_key: str,
     *,
     client: AuthenticatedClient,
-    form_data: Flaw,
-    multipart_data: Flaw,
-    json_body: Flaw,
-) -> Optional[OsidbApiV1FlawsUpdateResponse200]:
-    """ """
+    jira_authentication: str,
+) -> Optional[TaskmanApiV1TaskRetrieveResponse200]:
+    """Get a task from Jira given a task key"""
 
     return sync_detailed(
-        id=id,
+        task_key=task_key,
         client=client,
-        form_data=form_data,
-        multipart_data=multipart_data,
-        json_body=json_body,
+        jira_authentication=jira_authentication,
     ).parsed
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/client.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/client.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import json
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect_meta_attr import AffectMetaAttr
-from ..models.affect_type_enum import AffectTypeEnum
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
-from ..models.resolution_3_ac_enum import Resolution3AcEnum
+from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
+from ..models.type_5b2_enum import Type5B2Enum
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="Affect")
 
 
 @attr.s(auto_attribs=True)
 class Affect(OSIDBModel):
@@ -27,17 +27,17 @@
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
-    type: Union[Unset, AffectTypeEnum] = UNSET
+    type: Union[Unset, Type5B2Enum] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
-    resolution: Union[BlankEnum, Resolution3AcEnum, Unset] = UNSET
+    resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -69,15 +69,15 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         flaw = self.flaw
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = AffectTypeEnum(self.type).value
+            type = Type5B2Enum(self.type).value
 
         affectedness: Union[Unset, str]
         if isinstance(self.affectedness, Unset):
             affectedness = UNSET
         elif isinstance(self.affectedness, AffectednessEnum):
             affectedness = UNSET
             if not isinstance(self.affectedness, Unset):
@@ -89,19 +89,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -211,15 +211,15 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         flaw = self.flaw if self.flaw is UNSET else (None, str(self.flaw), "text/plain")
         type: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = AffectTypeEnum(self.type).value
+            type = Type5B2Enum(self.type).value
 
         affectedness: Union[Unset, str]
         if isinstance(self.affectedness, Unset):
             affectedness = UNSET
         elif isinstance(self.affectedness, AffectednessEnum):
             affectedness = UNSET
             if not isinstance(self.affectedness, Unset):
@@ -231,19 +231,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -373,19 +373,19 @@
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
         flaw = d.pop("flaw", UNSET)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, AffectTypeEnum]
+        type: Union[Unset, Type5B2Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AffectTypeEnum(_type)
+            type = Type5B2Enum(_type)
 
         def _parse_affectedness(
             data: object,
         ) -> Union[AffectednessEnum, BlankEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
@@ -410,28 +410,26 @@
             else:
                 affectedness_type_1 = BlankEnum(_affectedness_type_1)
 
             return affectedness_type_1
 
         affectedness = _parse_affectedness(d.pop("affectedness", UNSET))
 
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution3AcEnum, Unset]:
+        def _parse_resolution(data: object) -> Union[BlankEnum, ResolutionEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution3AcEnum]
+                resolution_type_0: Union[Unset, ResolutionEnum]
                 if isinstance(_resolution_type_0, Unset):
                     resolution_type_0 = UNSET
                 else:
-                    resolution_type_0 = Resolution3AcEnum(_resolution_type_0)
+                    resolution_type_0 = ResolutionEnum(_resolution_type_0)
 
                 return resolution_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _resolution_type_1 = data
@@ -515,17 +513,17 @@
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
-            "type": AffectTypeEnum,
+            "type": Type5B2Enum,
             "affectedness": Union[AffectednessEnum, BlankEnum],
-            "resolution": Union[BlankEnum, Resolution3AcEnum],
+            "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
             "cvss2": str,
             "cvss2_score": float,
             "cvss3": str,
             "cvss3_score": float,
         }
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect_meta_attr.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/affect_report_data.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/affect_report_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
-from ..models.resolution_3_ac_enum import Resolution3AcEnum
+from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker_report_data import TrackerReportData
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="AffectReportData")
 
 
 @attr.s(auto_attribs=True)
 class AffectReportData(OSIDBModel):
     """ """
 
     ps_module: str
     ps_component: str
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
-    resolution: Union[BlankEnum, Resolution3AcEnum, Unset] = UNSET
+    resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     trackers: Union[Unset, List[TrackerReportData]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         ps_module = self.ps_module
         ps_component = self.ps_component
         affectedness: Union[Unset, str]
@@ -39,19 +39,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -114,28 +114,26 @@
             else:
                 affectedness_type_1 = BlankEnum(_affectedness_type_1)
 
             return affectedness_type_1
 
         affectedness = _parse_affectedness(d.pop("affectedness", UNSET))
 
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution3AcEnum, Unset]:
+        def _parse_resolution(data: object) -> Union[BlankEnum, ResolutionEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution3AcEnum]
+                resolution_type_0: Union[Unset, ResolutionEnum]
                 if isinstance(_resolution_type_0, Unset):
                     resolution_type_0 = UNSET
                 else:
-                    resolution_type_0 = Resolution3AcEnum(_resolution_type_0)
+                    resolution_type_0 = ResolutionEnum(_resolution_type_0)
 
                 return resolution_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _resolution_type_1 = data
@@ -177,15 +175,15 @@
 
     @staticmethod
     def get_fields():
         return {
             "ps_module": str,
             "ps_component": str,
             "affectedness": Union[AffectednessEnum, BlankEnum],
-            "resolution": Union[BlankEnum, Resolution3AcEnum],
+            "resolution": Union[BlankEnum, ResolutionEnum],
             "trackers": List[TrackerReportData],
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/comment.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/comment.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/comment_meta_attr.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/epss.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/epss.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/erratum.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/erratum.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,64 +7,66 @@
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.cv_ev_5_package_versions import CVEv5PackageVersions
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_meta_attr import FlawMetaAttr
-from ..models.flaw_source_enum import FlawSourceEnum
-from ..models.flaw_type_enum import FlawTypeEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.meta import Meta
-from ..models.resolution_01f_enum import Resolution01FEnum
-from ..models.state_enum import StateEnum
+from ..models.source_666_enum import Source666Enum
+from ..models.type_824_enum import Type824Enum
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="Flaw")
 
 
 @attr.s(auto_attribs=True)
 class Flaw(OSIDBModel):
     """serialize flaw model"""
 
     uuid: str
+    state: str
+    resolution: str
     title: str
     trackers: List[str]
     description: str
     affects: List[Affect]
     meta: List[Meta]
     comments: List[Comment]
     meta_attr: FlawMetaAttr
     package_versions: List[CVEv5PackageVersions]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
-    type: Union[Unset, FlawTypeEnum] = UNSET
+    type: Union[Unset, Type824Enum] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
-    state: Union[Unset, StateEnum] = UNSET
-    resolution: Union[BlankEnum, Resolution01FEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
+    component: Union[Unset, str] = UNSET
     summary: Union[Unset, str] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
-    source: Union[BlankEnum, FlawSourceEnum, Unset] = UNSET
+    source: Union[BlankEnum, Source666Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
+    mitigation: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     nvd_cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     nvd_cvss3: Union[Unset, str] = UNSET
     is_major_incident: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
+        state = self.state
+        resolution = self.resolution
         title = self.title
         trackers: List[str] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = self.trackers
 
         description = self.description
         affects: List[Dict[str, Any]] = UNSET
@@ -123,37 +125,17 @@
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawTypeEnum(self.type).value
+            type = Type824Enum(self.type).value
 
         cve_id = self.cve_id
-        state: Union[Unset, str] = UNSET
-        if not isinstance(self.state, Unset):
-
-            state = StateEnum(self.state).value
-
-        resolution: Union[Unset, str]
-        if isinstance(self.resolution, Unset):
-            resolution = UNSET
-        elif isinstance(self.resolution, Resolution01FEnum):
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = Resolution01FEnum(self.resolution).value
-
-        else:
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = BlankEnum(self.resolution).value
-
         impact: Union[Unset, str]
         if isinstance(self.impact, Unset):
             impact = UNSET
         elif isinstance(self.impact, ImpactEnum):
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
@@ -161,52 +143,58 @@
 
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
+        component = self.component
         summary = self.summary
         statement = self.statement
         cwe_id = self.cwe_id
         unembargo_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.unembargo_dt, Unset):
             unembargo_dt = self.unembargo_dt.isoformat() if self.unembargo_dt else None
 
         source: Union[Unset, str]
         if isinstance(self.source, Unset):
             source = UNSET
-        elif isinstance(self.source, FlawSourceEnum):
+        elif isinstance(self.source, Source666Enum):
             source = UNSET
             if not isinstance(self.source, Unset):
 
-                source = FlawSourceEnum(self.source).value
+                source = Source666Enum(self.source).value
 
         else:
             source = UNSET
             if not isinstance(self.source, Unset):
 
                 source = BlankEnum(self.source).value
 
         reported_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.reported_dt, Unset):
             reported_dt = self.reported_dt.isoformat() if self.reported_dt else None
 
+        mitigation = self.mitigation
         cvss2 = self.cvss2
         cvss2_score = self.cvss2_score
         nvd_cvss2 = self.nvd_cvss2
         cvss3 = self.cvss3
         cvss3_score = self.cvss3_score
         nvd_cvss3 = self.nvd_cvss3
         is_major_incident = self.is_major_incident
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
+        if state is not UNSET:
+            field_dict["state"] = state
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if title is not UNSET:
             field_dict["title"] = title
         if trackers is not UNSET:
             field_dict["trackers"] = trackers
         if description is not UNSET:
             field_dict["description"] = description
         if affects is not UNSET:
@@ -227,32 +215,32 @@
             field_dict["updated_dt"] = updated_dt
         if classification is not UNSET:
             field_dict["classification"] = classification
         if type is not UNSET:
             field_dict["type"] = type
         if cve_id is not UNSET:
             field_dict["cve_id"] = cve_id
-        if state is not UNSET:
-            field_dict["state"] = state
-        if resolution is not UNSET:
-            field_dict["resolution"] = resolution
         if impact is not UNSET:
             field_dict["impact"] = impact
+        if component is not UNSET:
+            field_dict["component"] = component
         if summary is not UNSET:
             field_dict["summary"] = summary
         if statement is not UNSET:
             field_dict["statement"] = statement
         if cwe_id is not UNSET:
             field_dict["cwe_id"] = cwe_id
         if unembargo_dt is not UNSET:
             field_dict["unembargo_dt"] = unembargo_dt
         if source is not UNSET:
             field_dict["source"] = source
         if reported_dt is not UNSET:
             field_dict["reported_dt"] = reported_dt
+        if mitigation is not UNSET:
+            field_dict["mitigation"] = mitigation
         if cvss2 is not UNSET:
             field_dict["cvss2"] = cvss2
         if cvss2_score is not UNSET:
             field_dict["cvss2_score"] = cvss2_score
         if nvd_cvss2 is not UNSET:
             field_dict["nvd_cvss2"] = nvd_cvss2
         if cvss3 is not UNSET:
@@ -264,14 +252,22 @@
         if is_major_incident is not UNSET:
             field_dict["is_major_incident"] = is_major_incident
 
         return field_dict
 
     def to_multipart(self) -> Dict[str, Any]:
         uuid = self.uuid if self.uuid is UNSET else (None, str(self.uuid), "text/plain")
+        state = (
+            self.state if self.state is UNSET else (None, str(self.state), "text/plain")
+        )
+        resolution = (
+            self.resolution
+            if self.resolution is UNSET
+            else (None, str(self.resolution), "text/plain")
+        )
         title = (
             self.title if self.title is UNSET else (None, str(self.title), "text/plain")
         )
         trackers: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.trackers, Unset):
             _temp_trackers = self.trackers
             trackers = (None, json.dumps(_temp_trackers), "application/json")
@@ -353,41 +349,21 @@
                 json.dumps(self.classification.to_dict()),
                 "application/json",
             )
 
         type: Union[Unset, Tuple[None, str, str]] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawTypeEnum(self.type).value
+            type = Type824Enum(self.type).value
 
         cve_id = (
             self.cve_id
             if self.cve_id is UNSET
             else (None, str(self.cve_id), "text/plain")
         )
-        state: Union[Unset, Tuple[None, str, str]] = UNSET
-        if not isinstance(self.state, Unset):
-
-            state = StateEnum(self.state).value
-
-        resolution: Union[Unset, str]
-        if isinstance(self.resolution, Unset):
-            resolution = UNSET
-        elif isinstance(self.resolution, Resolution01FEnum):
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = Resolution01FEnum(self.resolution).value
-
-        else:
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = BlankEnum(self.resolution).value
-
         impact: Union[Unset, str]
         if isinstance(self.impact, Unset):
             impact = UNSET
         elif isinstance(self.impact, ImpactEnum):
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
@@ -395,14 +371,19 @@
 
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
+        component = (
+            self.component
+            if self.component is UNSET
+            else (None, str(self.component), "text/plain")
+        )
         summary = (
             self.summary
             if self.summary is UNSET
             else (None, str(self.summary), "text/plain")
         )
         statement = (
             self.statement
@@ -417,30 +398,35 @@
         unembargo_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.unembargo_dt, Unset):
             unembargo_dt = self.unembargo_dt.isoformat() if self.unembargo_dt else None
 
         source: Union[Unset, str]
         if isinstance(self.source, Unset):
             source = UNSET
-        elif isinstance(self.source, FlawSourceEnum):
+        elif isinstance(self.source, Source666Enum):
             source = UNSET
             if not isinstance(self.source, Unset):
 
-                source = FlawSourceEnum(self.source).value
+                source = Source666Enum(self.source).value
 
         else:
             source = UNSET
             if not isinstance(self.source, Unset):
 
                 source = BlankEnum(self.source).value
 
         reported_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.reported_dt, Unset):
             reported_dt = self.reported_dt.isoformat() if self.reported_dt else None
 
+        mitigation = (
+            self.mitigation
+            if self.mitigation is UNSET
+            else (None, str(self.mitigation), "text/plain")
+        )
         cvss2 = (
             self.cvss2 if self.cvss2 is UNSET else (None, str(self.cvss2), "text/plain")
         )
         cvss2_score = (
             self.cvss2_score
             if self.cvss2_score is UNSET
             else (None, str(self.cvss2_score), "text/plain")
@@ -474,14 +460,18 @@
             {
                 key: (None, str(value), "text/plain")
                 for key, value in self.additional_properties.items()
             }
         )
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
+        if state is not UNSET:
+            field_dict["state"] = state
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if title is not UNSET:
             field_dict["title"] = title
         if trackers is not UNSET:
             field_dict["trackers"] = trackers
         if description is not UNSET:
             field_dict["description"] = description
         if affects is not UNSET:
@@ -502,32 +492,32 @@
             field_dict["updated_dt"] = updated_dt
         if classification is not UNSET:
             field_dict["classification"] = classification
         if type is not UNSET:
             field_dict["type"] = type
         if cve_id is not UNSET:
             field_dict["cve_id"] = cve_id
-        if state is not UNSET:
-            field_dict["state"] = state
-        if resolution is not UNSET:
-            field_dict["resolution"] = resolution
         if impact is not UNSET:
             field_dict["impact"] = impact
+        if component is not UNSET:
+            field_dict["component"] = component
         if summary is not UNSET:
             field_dict["summary"] = summary
         if statement is not UNSET:
             field_dict["statement"] = statement
         if cwe_id is not UNSET:
             field_dict["cwe_id"] = cwe_id
         if unembargo_dt is not UNSET:
             field_dict["unembargo_dt"] = unembargo_dt
         if source is not UNSET:
             field_dict["source"] = source
         if reported_dt is not UNSET:
             field_dict["reported_dt"] = reported_dt
+        if mitigation is not UNSET:
+            field_dict["mitigation"] = mitigation
         if cvss2 is not UNSET:
             field_dict["cvss2"] = cvss2
         if cvss2_score is not UNSET:
             field_dict["cvss2_score"] = cvss2_score
         if nvd_cvss2 is not UNSET:
             field_dict["nvd_cvss2"] = nvd_cvss2
         if cvss3 is not UNSET:
@@ -542,14 +532,18 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
+        state = d.pop("state", UNSET)
+
+        resolution = d.pop("resolution", UNSET)
+
         title = d.pop("title", UNSET)
 
         trackers = cast(List[str], d.pop("trackers", UNSET))
 
         description = d.pop("description", UNSET)
 
         affects = []
@@ -641,60 +635,22 @@
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawTypeEnum]
+        type: Union[Unset, Type824Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = FlawTypeEnum(_type)
+            type = Type824Enum(_type)
 
         cve_id = d.pop("cve_id", UNSET)
 
-        _state = d.pop("state", UNSET)
-        state: Union[Unset, StateEnum]
-        if isinstance(_state, Unset):
-            state = UNSET
-        else:
-            state = StateEnum(_state)
-
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution01FEnum, Unset]:
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, str):
-                    raise TypeError()
-                _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution01FEnum]
-                if isinstance(_resolution_type_0, Unset):
-                    resolution_type_0 = UNSET
-                else:
-                    resolution_type_0 = Resolution01FEnum(_resolution_type_0)
-
-                return resolution_type_0
-            except:  # noqa: E722
-                pass
-            if not isinstance(data, str):
-                raise TypeError()
-            _resolution_type_1 = data
-            resolution_type_1: Union[Unset, BlankEnum]
-            if isinstance(_resolution_type_1, Unset):
-                resolution_type_1 = UNSET
-            else:
-                resolution_type_1 = BlankEnum(_resolution_type_1)
-
-            return resolution_type_1
-
-        resolution = _parse_resolution(d.pop("resolution", UNSET))
-
         def _parse_impact(data: object) -> Union[BlankEnum, ImpactEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _impact_type_0 = data
@@ -716,14 +672,16 @@
             else:
                 impact_type_1 = BlankEnum(_impact_type_1)
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
+        component = d.pop("component", UNSET)
+
         summary = d.pop("summary", UNSET)
 
         statement = d.pop("statement", UNSET)
 
         cwe_id = d.pop("cwe_id", UNSET)
 
         _unembargo_dt = d.pop("unembargo_dt", UNSET)
@@ -731,26 +689,26 @@
         if _unembargo_dt is None:
             unembargo_dt = None
         elif isinstance(_unembargo_dt, Unset):
             unembargo_dt = UNSET
         else:
             unembargo_dt = isoparse(_unembargo_dt)
 
-        def _parse_source(data: object) -> Union[BlankEnum, FlawSourceEnum, Unset]:
+        def _parse_source(data: object) -> Union[BlankEnum, Source666Enum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _source_type_0 = data
-                source_type_0: Union[Unset, FlawSourceEnum]
+                source_type_0: Union[Unset, Source666Enum]
                 if isinstance(_source_type_0, Unset):
                     source_type_0 = UNSET
                 else:
-                    source_type_0 = FlawSourceEnum(_source_type_0)
+                    source_type_0 = Source666Enum(_source_type_0)
 
                 return source_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _source_type_1 = data
@@ -769,14 +727,16 @@
         if _reported_dt is None:
             reported_dt = None
         elif isinstance(_reported_dt, Unset):
             reported_dt = UNSET
         else:
             reported_dt = isoparse(_reported_dt)
 
+        mitigation = d.pop("mitigation", UNSET)
+
         cvss2 = d.pop("cvss2", UNSET)
 
         cvss2_score = d.pop("cvss2_score", UNSET)
 
         nvd_cvss2 = d.pop("nvd_cvss2", UNSET)
 
         cvss3 = d.pop("cvss3", UNSET)
@@ -785,37 +745,39 @@
 
         nvd_cvss3 = d.pop("nvd_cvss3", UNSET)
 
         is_major_incident = d.pop("is_major_incident", UNSET)
 
         flaw = cls(
             uuid=uuid,
+            state=state,
+            resolution=resolution,
             title=title,
             trackers=trackers,
             description=description,
             affects=affects,
             meta=meta,
             comments=comments,
             meta_attr=meta_attr,
             package_versions=package_versions,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
             type=type,
             cve_id=cve_id,
-            state=state,
-            resolution=resolution,
             impact=impact,
+            component=component,
             summary=summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
+            mitigation=mitigation,
             cvss2=cvss2,
             cvss2_score=cvss2_score,
             nvd_cvss2=nvd_cvss2,
             cvss3=cvss3,
             cvss3_score=cvss3_score,
             nvd_cvss3=nvd_cvss3,
             is_major_incident=is_major_incident,
@@ -824,37 +786,39 @@
         flaw.additional_properties = d
         return flaw
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
+            "state": str,
+            "resolution": str,
             "title": str,
             "trackers": List[str],
             "description": str,
             "affects": List[Affect],
             "meta": List[Meta],
             "comments": List[Comment],
             "meta_attr": FlawMetaAttr,
             "package_versions": List[CVEv5PackageVersions],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
-            "type": FlawTypeEnum,
+            "type": Type824Enum,
             "cve_id": str,
-            "state": StateEnum,
-            "resolution": Union[BlankEnum, Resolution01FEnum],
             "impact": Union[BlankEnum, ImpactEnum],
+            "component": str,
             "summary": str,
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
-            "source": Union[BlankEnum, FlawSourceEnum],
+            "source": Union[BlankEnum, Source666Enum],
             "reported_dt": datetime.datetime,
+            "mitigation": str,
             "cvss2": str,
             "cvss2_score": float,
             "nvd_cvss2": str,
             "cvss3": str,
             "cvss3_score": float,
             "nvd_cvss3": str,
             "is_major_incident": bool,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_classification.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_classification.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="FlawMetaAttr")
+T = TypeVar("T", bound="FlawPostMetaAttr")
 
 
 @attr.s(auto_attribs=True)
-class FlawMetaAttr(OSIDBModel):
+class FlawPostMetaAttr(OSIDBModel):
     """ """
 
     acknowledgments: Union[Unset, str] = UNSET
     acks_not_needed: Union[Unset, str] = UNSET
     affects: Union[Unset, str] = UNSET
     alias: Union[Unset, str] = UNSET
     bz_datascore: Union[Unset, str] = UNSET
@@ -32,15 +32,17 @@
     jira_trackers: Union[Unset, str] = UNSET
     mitigate: Union[Unset, str] = UNSET
     mitigation: Union[Unset, str] = UNSET
     public: Union[Unset, str] = UNSET
     references: Union[Unset, str] = UNSET
     related_cves: Union[Unset, str] = UNSET
     reported: Union[Unset, str] = UNSET
+    resolution: Union[Unset, str] = UNSET
     source: Union[Unset, str] = UNSET
+    state: Union[Unset, str] = UNSET
     statement: Union[Unset, str] = UNSET
     task_owner: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         acknowledgments = self.acknowledgments
         acks_not_needed = self.acks_not_needed
@@ -63,15 +65,17 @@
         jira_trackers = self.jira_trackers
         mitigate = self.mitigate
         mitigation = self.mitigation
         public = self.public
         references = self.references
         related_cves = self.related_cves
         reported = self.reported
+        resolution = self.resolution
         source = self.source
+        state = self.state
         statement = self.statement
         task_owner = self.task_owner
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if acknowledgments is not UNSET:
             field_dict["acknowledgments"] = acknowledgments
@@ -119,16 +123,20 @@
             field_dict["public"] = public
         if references is not UNSET:
             field_dict["references"] = references
         if related_cves is not UNSET:
             field_dict["related_cves"] = related_cves
         if reported is not UNSET:
             field_dict["reported"] = reported
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if source is not UNSET:
             field_dict["source"] = source
+        if state is not UNSET:
+            field_dict["state"] = state
         if statement is not UNSET:
             field_dict["statement"] = statement
         if task_owner is not UNSET:
             field_dict["task_owner"] = task_owner
 
         return field_dict
 
@@ -181,21 +189,25 @@
 
         references = d.pop("references", UNSET)
 
         related_cves = d.pop("related_cves", UNSET)
 
         reported = d.pop("reported", UNSET)
 
+        resolution = d.pop("resolution", UNSET)
+
         source = d.pop("source", UNSET)
 
+        state = d.pop("state", UNSET)
+
         statement = d.pop("statement", UNSET)
 
         task_owner = d.pop("task_owner", UNSET)
 
-        flaw_meta_attr = cls(
+        flaw_post_meta_attr = cls(
             acknowledgments=acknowledgments,
             acks_not_needed=acks_not_needed,
             affects=affects,
             alias=alias,
             bz_datascore=bz_datascore,
             bz_id=bz_id,
             checklists=checklists,
@@ -213,21 +225,23 @@
             jira_trackers=jira_trackers,
             mitigate=mitigate,
             mitigation=mitigation,
             public=public,
             references=references,
             related_cves=related_cves,
             reported=reported,
+            resolution=resolution,
             source=source,
+            state=state,
             statement=statement,
             task_owner=task_owner,
         )
 
-        flaw_meta_attr.additional_properties = d
-        return flaw_meta_attr
+        flaw_post_meta_attr.additional_properties = d
+        return flaw_post_meta_attr
 
     @staticmethod
     def get_fields():
         return {
             "acknowledgments": str,
             "acks_not_needed": str,
             "affects": str,
@@ -249,15 +263,17 @@
             "jira_trackers": str,
             "mitigate": str,
             "mitigation": str,
             "public": str,
             "references": str,
             "related_cves": str,
             "reported": str,
+            "resolution": str,
             "source": str,
+            "state": str,
             "statement": str,
             "task_owner": str,
         }
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/flaw_source_enum.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/source_666_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class FlawSourceEnum(str, Enum):
+class Source666Enum(str, Enum):
     ADOBE = "ADOBE"
     APPLE = "APPLE"
     ASF = "ASF"
     BIND = "BIND"
     BK = "BK"
     BUGTRAQ = "BUGTRAQ"
     BUGZILLA = "BUGZILLA"
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/meta.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/meta.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/meta_meta_attr.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect_meta_attr import AffectMetaAttr
-from ..models.affect_type_enum import AffectTypeEnum
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
-from ..models.resolution_3_ac_enum import Resolution3AcEnum
+from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
+from ..models.type_5b2_enum import Type5B2Enum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1AffectsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsCreateResponse201(OSIDBModel):
+class OsidbApiV1AffectsRetrieveResponse200(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
-    type: Union[Unset, AffectTypeEnum] = UNSET
+    type: Union[Unset, Type5B2Enum] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
-    resolution: Union[BlankEnum, Resolution3AcEnum, Unset] = UNSET
+    resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -72,15 +72,15 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         flaw = self.flaw
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = AffectTypeEnum(self.type).value
+            type = Type5B2Enum(self.type).value
 
         affectedness: Union[Unset, str]
         if isinstance(self.affectedness, Unset):
             affectedness = UNSET
         elif isinstance(self.affectedness, AffectednessEnum):
             affectedness = UNSET
             if not isinstance(self.affectedness, Unset):
@@ -92,19 +92,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -232,19 +232,19 @@
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
         flaw = d.pop("flaw", UNSET)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, AffectTypeEnum]
+        type: Union[Unset, Type5B2Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AffectTypeEnum(_type)
+            type = Type5B2Enum(_type)
 
         def _parse_affectedness(
             data: object,
         ) -> Union[AffectednessEnum, BlankEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
@@ -269,28 +269,26 @@
             else:
                 affectedness_type_1 = BlankEnum(_affectedness_type_1)
 
             return affectedness_type_1
 
         affectedness = _parse_affectedness(d.pop("affectedness", UNSET))
 
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution3AcEnum, Unset]:
+        def _parse_resolution(data: object) -> Union[BlankEnum, ResolutionEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution3AcEnum]
+                resolution_type_0: Union[Unset, ResolutionEnum]
                 if isinstance(_resolution_type_0, Unset):
                     resolution_type_0 = UNSET
                 else:
-                    resolution_type_0 = Resolution3AcEnum(_resolution_type_0)
+                    resolution_type_0 = ResolutionEnum(_resolution_type_0)
 
                 return resolution_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _resolution_type_1 = data
@@ -350,15 +348,15 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_create_response_201 = cls(
+        osidb_api_v1_affects_retrieve_response_200 = cls(
             uuid=uuid,
             ps_module=ps_module,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             embargoed=embargoed,
@@ -375,33 +373,33 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_create_response_201.additional_properties = d
-        return osidb_api_v1_affects_create_response_201
+        osidb_api_v1_affects_retrieve_response_200.additional_properties = d
+        return osidb_api_v1_affects_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
-            "type": AffectTypeEnum,
+            "type": Type5B2Enum,
             "affectedness": Union[AffectednessEnum, BlankEnum],
-            "resolution": Union[BlankEnum, Resolution3AcEnum],
+            "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
             "cvss2": str,
             "cvss2_score": float,
             "cvss3": str,
             "cvss3_score": float,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect_meta_attr import AffectMetaAttr
-from ..models.affect_type_enum import AffectTypeEnum
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
-from ..models.resolution_3_ac_enum import Resolution3AcEnum
+from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
+from ..models.type_5b2_enum import Type5B2Enum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsRetrieveResponse200")
+T = TypeVar("T", bound="OsidbApiV1AffectsUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsRetrieveResponse200(OSIDBModel):
+class OsidbApiV1AffectsUpdateResponse200(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
-    type: Union[Unset, AffectTypeEnum] = UNSET
+    type: Union[Unset, Type5B2Enum] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
-    resolution: Union[BlankEnum, Resolution3AcEnum, Unset] = UNSET
+    resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -72,15 +72,15 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         flaw = self.flaw
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = AffectTypeEnum(self.type).value
+            type = Type5B2Enum(self.type).value
 
         affectedness: Union[Unset, str]
         if isinstance(self.affectedness, Unset):
             affectedness = UNSET
         elif isinstance(self.affectedness, AffectednessEnum):
             affectedness = UNSET
             if not isinstance(self.affectedness, Unset):
@@ -92,19 +92,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -232,19 +232,19 @@
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
         flaw = d.pop("flaw", UNSET)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, AffectTypeEnum]
+        type: Union[Unset, Type5B2Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AffectTypeEnum(_type)
+            type = Type5B2Enum(_type)
 
         def _parse_affectedness(
             data: object,
         ) -> Union[AffectednessEnum, BlankEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
@@ -269,28 +269,26 @@
             else:
                 affectedness_type_1 = BlankEnum(_affectedness_type_1)
 
             return affectedness_type_1
 
         affectedness = _parse_affectedness(d.pop("affectedness", UNSET))
 
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution3AcEnum, Unset]:
+        def _parse_resolution(data: object) -> Union[BlankEnum, ResolutionEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution3AcEnum]
+                resolution_type_0: Union[Unset, ResolutionEnum]
                 if isinstance(_resolution_type_0, Unset):
                     resolution_type_0 = UNSET
                 else:
-                    resolution_type_0 = Resolution3AcEnum(_resolution_type_0)
+                    resolution_type_0 = ResolutionEnum(_resolution_type_0)
 
                 return resolution_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _resolution_type_1 = data
@@ -350,15 +348,15 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_retrieve_response_200 = cls(
+        osidb_api_v1_affects_update_response_200 = cls(
             uuid=uuid,
             ps_module=ps_module,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             embargoed=embargoed,
@@ -375,33 +373,33 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_retrieve_response_200.additional_properties = d
-        return osidb_api_v1_affects_retrieve_response_200
+        osidb_api_v1_affects_update_response_200.additional_properties = d
+        return osidb_api_v1_affects_update_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
-            "type": AffectTypeEnum,
+            "type": Type5B2Enum,
             "affectedness": Union[AffectednessEnum, BlankEnum],
-            "resolution": Union[BlankEnum, Resolution3AcEnum],
+            "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
             "cvss2": str,
             "cvss2_score": float,
             "cvss3": str,
             "cvss3_score": float,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.affect_meta_attr import AffectMetaAttr
-from ..models.affect_type_enum import AffectTypeEnum
 from ..models.affectedness_enum import AffectednessEnum
 from ..models.blank_enum import BlankEnum
 from ..models.impact_enum import ImpactEnum
-from ..models.resolution_3_ac_enum import Resolution3AcEnum
+from ..models.resolution_enum import ResolutionEnum
 from ..models.tracker import Tracker
+from ..models.type_5b2_enum import Type5B2Enum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1AffectsUpdateResponse200")
+T = TypeVar("T", bound="OsidbApiV1AffectsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1AffectsUpdateResponse200(OSIDBModel):
+class OsidbApiV1AffectsCreateResponse201(OSIDBModel):
     """ """
 
     uuid: str
     ps_module: str
     ps_component: str
     trackers: List[Tracker]
     meta_attr: AffectMetaAttr
     delegated_resolution: str
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     flaw: Optional[str]
-    type: Union[Unset, AffectTypeEnum] = UNSET
+    type: Union[Unset, Type5B2Enum] = UNSET
     affectedness: Union[AffectednessEnum, BlankEnum, Unset] = UNSET
-    resolution: Union[BlankEnum, Resolution3AcEnum, Unset] = UNSET
+    resolution: Union[BlankEnum, ResolutionEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     dt: Union[Unset, datetime.datetime] = UNSET
     env: Union[Unset, str] = UNSET
@@ -72,15 +72,15 @@
         if not isinstance(self.updated_dt, Unset):
             updated_dt = self.updated_dt.isoformat()
 
         flaw = self.flaw
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = AffectTypeEnum(self.type).value
+            type = Type5B2Enum(self.type).value
 
         affectedness: Union[Unset, str]
         if isinstance(self.affectedness, Unset):
             affectedness = UNSET
         elif isinstance(self.affectedness, AffectednessEnum):
             affectedness = UNSET
             if not isinstance(self.affectedness, Unset):
@@ -92,19 +92,19 @@
             if not isinstance(self.affectedness, Unset):
 
                 affectedness = BlankEnum(self.affectedness).value
 
         resolution: Union[Unset, str]
         if isinstance(self.resolution, Unset):
             resolution = UNSET
-        elif isinstance(self.resolution, Resolution3AcEnum):
+        elif isinstance(self.resolution, ResolutionEnum):
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
-                resolution = Resolution3AcEnum(self.resolution).value
+                resolution = ResolutionEnum(self.resolution).value
 
         else:
             resolution = UNSET
             if not isinstance(self.resolution, Unset):
 
                 resolution = BlankEnum(self.resolution).value
 
@@ -232,19 +232,19 @@
             updated_dt = UNSET
         else:
             updated_dt = isoparse(_updated_dt)
 
         flaw = d.pop("flaw", UNSET)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, AffectTypeEnum]
+        type: Union[Unset, Type5B2Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = AffectTypeEnum(_type)
+            type = Type5B2Enum(_type)
 
         def _parse_affectedness(
             data: object,
         ) -> Union[AffectednessEnum, BlankEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
@@ -269,28 +269,26 @@
             else:
                 affectedness_type_1 = BlankEnum(_affectedness_type_1)
 
             return affectedness_type_1
 
         affectedness = _parse_affectedness(d.pop("affectedness", UNSET))
 
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution3AcEnum, Unset]:
+        def _parse_resolution(data: object) -> Union[BlankEnum, ResolutionEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution3AcEnum]
+                resolution_type_0: Union[Unset, ResolutionEnum]
                 if isinstance(_resolution_type_0, Unset):
                     resolution_type_0 = UNSET
                 else:
-                    resolution_type_0 = Resolution3AcEnum(_resolution_type_0)
+                    resolution_type_0 = ResolutionEnum(_resolution_type_0)
 
                 return resolution_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _resolution_type_1 = data
@@ -350,15 +348,15 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_affects_update_response_200 = cls(
+        osidb_api_v1_affects_create_response_201 = cls(
             uuid=uuid,
             ps_module=ps_module,
             ps_component=ps_component,
             trackers=trackers,
             meta_attr=meta_attr,
             delegated_resolution=delegated_resolution,
             embargoed=embargoed,
@@ -375,33 +373,33 @@
             cvss3_score=cvss3_score,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_affects_update_response_200.additional_properties = d
-        return osidb_api_v1_affects_update_response_200
+        osidb_api_v1_affects_create_response_201.additional_properties = d
+        return osidb_api_v1_affects_create_response_201
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
             "ps_module": str,
             "ps_component": str,
             "trackers": List[Tracker],
             "meta_attr": AffectMetaAttr,
             "delegated_resolution": str,
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "flaw": str,
-            "type": AffectTypeEnum,
+            "type": Type5B2Enum,
             "affectedness": Union[AffectednessEnum, BlankEnum],
-            "resolution": Union[BlankEnum, Resolution3AcEnum],
+            "resolution": Union[BlankEnum, ResolutionEnum],
             "impact": Union[BlankEnum, ImpactEnum],
             "cvss2": str,
             "cvss2_score": float,
             "cvss3": str,
             "cvss3_score": float,
             "dt": datetime.datetime,
             "env": str,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.cv_ev_5_package_versions import CVEv5PackageVersions
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_meta_attr import FlawMetaAttr
-from ..models.flaw_source_enum import FlawSourceEnum
-from ..models.flaw_type_enum import FlawTypeEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.meta import Meta
-from ..models.resolution_01f_enum import Resolution01FEnum
-from ..models.state_enum import StateEnum
+from ..models.source_666_enum import Source666Enum
+from ..models.type_824_enum import Type824Enum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsCreateResponse201")
+T = TypeVar("T", bound="OsidbApiV1FlawsUpdateResponse200")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsCreateResponse201(OSIDBModel):
+class OsidbApiV1FlawsUpdateResponse200(OSIDBModel):
     """ """
 
     uuid: str
+    state: str
+    resolution: str
     title: str
     trackers: List[str]
     description: str
     affects: List[Affect]
     meta: List[Meta]
     comments: List[Comment]
     meta_attr: FlawMetaAttr
     package_versions: List[CVEv5PackageVersions]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
-    type: Union[Unset, FlawTypeEnum] = UNSET
+    type: Union[Unset, Type824Enum] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
-    state: Union[Unset, StateEnum] = UNSET
-    resolution: Union[BlankEnum, Resolution01FEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
+    component: Union[Unset, str] = UNSET
     summary: Union[Unset, str] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
-    source: Union[BlankEnum, FlawSourceEnum, Unset] = UNSET
+    source: Union[BlankEnum, Source666Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
+    mitigation: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     nvd_cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     nvd_cvss3: Union[Unset, str] = UNSET
     is_major_incident: Union[Unset, bool] = UNSET
@@ -60,14 +60,16 @@
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
+        state = self.state
+        resolution = self.resolution
         title = self.title
         trackers: List[str] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = self.trackers
 
         description = self.description
         affects: List[Dict[str, Any]] = UNSET
@@ -126,37 +128,17 @@
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawTypeEnum(self.type).value
+            type = Type824Enum(self.type).value
 
         cve_id = self.cve_id
-        state: Union[Unset, str] = UNSET
-        if not isinstance(self.state, Unset):
-
-            state = StateEnum(self.state).value
-
-        resolution: Union[Unset, str]
-        if isinstance(self.resolution, Unset):
-            resolution = UNSET
-        elif isinstance(self.resolution, Resolution01FEnum):
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = Resolution01FEnum(self.resolution).value
-
-        else:
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = BlankEnum(self.resolution).value
-
         impact: Union[Unset, str]
         if isinstance(self.impact, Unset):
             impact = UNSET
         elif isinstance(self.impact, ImpactEnum):
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
@@ -164,40 +146,42 @@
 
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
+        component = self.component
         summary = self.summary
         statement = self.statement
         cwe_id = self.cwe_id
         unembargo_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.unembargo_dt, Unset):
             unembargo_dt = self.unembargo_dt.isoformat() if self.unembargo_dt else None
 
         source: Union[Unset, str]
         if isinstance(self.source, Unset):
             source = UNSET
-        elif isinstance(self.source, FlawSourceEnum):
+        elif isinstance(self.source, Source666Enum):
             source = UNSET
             if not isinstance(self.source, Unset):
 
-                source = FlawSourceEnum(self.source).value
+                source = Source666Enum(self.source).value
 
         else:
             source = UNSET
             if not isinstance(self.source, Unset):
 
                 source = BlankEnum(self.source).value
 
         reported_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.reported_dt, Unset):
             reported_dt = self.reported_dt.isoformat() if self.reported_dt else None
 
+        mitigation = self.mitigation
         cvss2 = self.cvss2
         cvss2_score = self.cvss2_score
         nvd_cvss2 = self.nvd_cvss2
         cvss3 = self.cvss3
         cvss3_score = self.cvss3_score
         nvd_cvss3 = self.nvd_cvss3
         is_major_incident = self.is_major_incident
@@ -209,14 +193,18 @@
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
+        if state is not UNSET:
+            field_dict["state"] = state
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if title is not UNSET:
             field_dict["title"] = title
         if trackers is not UNSET:
             field_dict["trackers"] = trackers
         if description is not UNSET:
             field_dict["description"] = description
         if affects is not UNSET:
@@ -237,32 +225,32 @@
             field_dict["updated_dt"] = updated_dt
         if classification is not UNSET:
             field_dict["classification"] = classification
         if type is not UNSET:
             field_dict["type"] = type
         if cve_id is not UNSET:
             field_dict["cve_id"] = cve_id
-        if state is not UNSET:
-            field_dict["state"] = state
-        if resolution is not UNSET:
-            field_dict["resolution"] = resolution
         if impact is not UNSET:
             field_dict["impact"] = impact
+        if component is not UNSET:
+            field_dict["component"] = component
         if summary is not UNSET:
             field_dict["summary"] = summary
         if statement is not UNSET:
             field_dict["statement"] = statement
         if cwe_id is not UNSET:
             field_dict["cwe_id"] = cwe_id
         if unembargo_dt is not UNSET:
             field_dict["unembargo_dt"] = unembargo_dt
         if source is not UNSET:
             field_dict["source"] = source
         if reported_dt is not UNSET:
             field_dict["reported_dt"] = reported_dt
+        if mitigation is not UNSET:
+            field_dict["mitigation"] = mitigation
         if cvss2 is not UNSET:
             field_dict["cvss2"] = cvss2
         if cvss2_score is not UNSET:
             field_dict["cvss2_score"] = cvss2_score
         if nvd_cvss2 is not UNSET:
             field_dict["nvd_cvss2"] = nvd_cvss2
         if cvss3 is not UNSET:
@@ -285,14 +273,18 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
+        state = d.pop("state", UNSET)
+
+        resolution = d.pop("resolution", UNSET)
+
         title = d.pop("title", UNSET)
 
         trackers = cast(List[str], d.pop("trackers", UNSET))
 
         description = d.pop("description", UNSET)
 
         affects = []
@@ -384,60 +376,22 @@
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawTypeEnum]
+        type: Union[Unset, Type824Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = FlawTypeEnum(_type)
+            type = Type824Enum(_type)
 
         cve_id = d.pop("cve_id", UNSET)
 
-        _state = d.pop("state", UNSET)
-        state: Union[Unset, StateEnum]
-        if isinstance(_state, Unset):
-            state = UNSET
-        else:
-            state = StateEnum(_state)
-
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution01FEnum, Unset]:
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, str):
-                    raise TypeError()
-                _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution01FEnum]
-                if isinstance(_resolution_type_0, Unset):
-                    resolution_type_0 = UNSET
-                else:
-                    resolution_type_0 = Resolution01FEnum(_resolution_type_0)
-
-                return resolution_type_0
-            except:  # noqa: E722
-                pass
-            if not isinstance(data, str):
-                raise TypeError()
-            _resolution_type_1 = data
-            resolution_type_1: Union[Unset, BlankEnum]
-            if isinstance(_resolution_type_1, Unset):
-                resolution_type_1 = UNSET
-            else:
-                resolution_type_1 = BlankEnum(_resolution_type_1)
-
-            return resolution_type_1
-
-        resolution = _parse_resolution(d.pop("resolution", UNSET))
-
         def _parse_impact(data: object) -> Union[BlankEnum, ImpactEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _impact_type_0 = data
@@ -459,14 +413,16 @@
             else:
                 impact_type_1 = BlankEnum(_impact_type_1)
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
+        component = d.pop("component", UNSET)
+
         summary = d.pop("summary", UNSET)
 
         statement = d.pop("statement", UNSET)
 
         cwe_id = d.pop("cwe_id", UNSET)
 
         _unembargo_dt = d.pop("unembargo_dt", UNSET)
@@ -474,26 +430,26 @@
         if _unembargo_dt is None:
             unembargo_dt = None
         elif isinstance(_unembargo_dt, Unset):
             unembargo_dt = UNSET
         else:
             unembargo_dt = isoparse(_unembargo_dt)
 
-        def _parse_source(data: object) -> Union[BlankEnum, FlawSourceEnum, Unset]:
+        def _parse_source(data: object) -> Union[BlankEnum, Source666Enum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _source_type_0 = data
-                source_type_0: Union[Unset, FlawSourceEnum]
+                source_type_0: Union[Unset, Source666Enum]
                 if isinstance(_source_type_0, Unset):
                     source_type_0 = UNSET
                 else:
-                    source_type_0 = FlawSourceEnum(_source_type_0)
+                    source_type_0 = Source666Enum(_source_type_0)
 
                 return source_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _source_type_1 = data
@@ -512,14 +468,16 @@
         if _reported_dt is None:
             reported_dt = None
         elif isinstance(_reported_dt, Unset):
             reported_dt = UNSET
         else:
             reported_dt = isoparse(_reported_dt)
 
+        mitigation = d.pop("mitigation", UNSET)
+
         cvss2 = d.pop("cvss2", UNSET)
 
         cvss2_score = d.pop("cvss2_score", UNSET)
 
         nvd_cvss2 = d.pop("nvd_cvss2", UNSET)
 
         cvss3 = d.pop("cvss3", UNSET)
@@ -539,82 +497,86 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_create_response_201 = cls(
+        osidb_api_v1_flaws_update_response_200 = cls(
             uuid=uuid,
+            state=state,
+            resolution=resolution,
             title=title,
             trackers=trackers,
             description=description,
             affects=affects,
             meta=meta,
             comments=comments,
             meta_attr=meta_attr,
             package_versions=package_versions,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
             type=type,
             cve_id=cve_id,
-            state=state,
-            resolution=resolution,
             impact=impact,
+            component=component,
             summary=summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
+            mitigation=mitigation,
             cvss2=cvss2,
             cvss2_score=cvss2_score,
             nvd_cvss2=nvd_cvss2,
             cvss3=cvss3,
             cvss3_score=cvss3_score,
             nvd_cvss3=nvd_cvss3,
             is_major_incident=is_major_incident,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_create_response_201.additional_properties = d
-        return osidb_api_v1_flaws_create_response_201
+        osidb_api_v1_flaws_update_response_200.additional_properties = d
+        return osidb_api_v1_flaws_update_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
+            "state": str,
+            "resolution": str,
             "title": str,
             "trackers": List[str],
             "description": str,
             "affects": List[Affect],
             "meta": List[Meta],
             "comments": List[Comment],
             "meta_attr": FlawMetaAttr,
             "package_versions": List[CVEv5PackageVersions],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
-            "type": FlawTypeEnum,
+            "type": Type824Enum,
             "cve_id": str,
-            "state": StateEnum,
-            "resolution": Union[BlankEnum, Resolution01FEnum],
             "impact": Union[BlankEnum, ImpactEnum],
+            "component": str,
             "summary": str,
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
-            "source": Union[BlankEnum, FlawSourceEnum],
+            "source": Union[BlankEnum, Source666Enum],
             "reported_dt": datetime.datetime,
+            "mitigation": str,
             "cvss2": str,
             "cvss2_score": float,
             "nvd_cvss2": str,
             "cvss3": str,
             "cvss3_score": float,
             "nvd_cvss3": str,
             "is_major_incident": bool,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.cv_ev_5_package_versions import CVEv5PackageVersions
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_meta_attr import FlawMetaAttr
-from ..models.flaw_source_enum import FlawSourceEnum
-from ..models.flaw_type_enum import FlawTypeEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.meta import Meta
-from ..models.resolution_01f_enum import Resolution01FEnum
-from ..models.state_enum import StateEnum
+from ..models.source_666_enum import Source666Enum
+from ..models.type_824_enum import Type824Enum
 from ..types import UNSET, OSIDBModel, Unset
 
 T = TypeVar("T", bound="OsidbApiV1FlawsRetrieveResponse200")
 
 
 @attr.s(auto_attribs=True)
 class OsidbApiV1FlawsRetrieveResponse200(OSIDBModel):
     """ """
 
     uuid: str
+    state: str
+    resolution: str
     title: str
     trackers: List[str]
     description: str
     affects: List[Affect]
     meta: List[Meta]
     comments: List[Comment]
     meta_attr: FlawMetaAttr
     package_versions: List[CVEv5PackageVersions]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
-    type: Union[Unset, FlawTypeEnum] = UNSET
+    type: Union[Unset, Type824Enum] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
-    state: Union[Unset, StateEnum] = UNSET
-    resolution: Union[BlankEnum, Resolution01FEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
+    component: Union[Unset, str] = UNSET
     summary: Union[Unset, str] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
-    source: Union[BlankEnum, FlawSourceEnum, Unset] = UNSET
+    source: Union[BlankEnum, Source666Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
+    mitigation: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     nvd_cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     nvd_cvss3: Union[Unset, str] = UNSET
     is_major_incident: Union[Unset, bool] = UNSET
@@ -60,14 +60,16 @@
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
+        state = self.state
+        resolution = self.resolution
         title = self.title
         trackers: List[str] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = self.trackers
 
         description = self.description
         affects: List[Dict[str, Any]] = UNSET
@@ -126,37 +128,17 @@
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawTypeEnum(self.type).value
+            type = Type824Enum(self.type).value
 
         cve_id = self.cve_id
-        state: Union[Unset, str] = UNSET
-        if not isinstance(self.state, Unset):
-
-            state = StateEnum(self.state).value
-
-        resolution: Union[Unset, str]
-        if isinstance(self.resolution, Unset):
-            resolution = UNSET
-        elif isinstance(self.resolution, Resolution01FEnum):
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = Resolution01FEnum(self.resolution).value
-
-        else:
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = BlankEnum(self.resolution).value
-
         impact: Union[Unset, str]
         if isinstance(self.impact, Unset):
             impact = UNSET
         elif isinstance(self.impact, ImpactEnum):
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
@@ -164,40 +146,42 @@
 
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
+        component = self.component
         summary = self.summary
         statement = self.statement
         cwe_id = self.cwe_id
         unembargo_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.unembargo_dt, Unset):
             unembargo_dt = self.unembargo_dt.isoformat() if self.unembargo_dt else None
 
         source: Union[Unset, str]
         if isinstance(self.source, Unset):
             source = UNSET
-        elif isinstance(self.source, FlawSourceEnum):
+        elif isinstance(self.source, Source666Enum):
             source = UNSET
             if not isinstance(self.source, Unset):
 
-                source = FlawSourceEnum(self.source).value
+                source = Source666Enum(self.source).value
 
         else:
             source = UNSET
             if not isinstance(self.source, Unset):
 
                 source = BlankEnum(self.source).value
 
         reported_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.reported_dt, Unset):
             reported_dt = self.reported_dt.isoformat() if self.reported_dt else None
 
+        mitigation = self.mitigation
         cvss2 = self.cvss2
         cvss2_score = self.cvss2_score
         nvd_cvss2 = self.nvd_cvss2
         cvss3 = self.cvss3
         cvss3_score = self.cvss3_score
         nvd_cvss3 = self.nvd_cvss3
         is_major_incident = self.is_major_incident
@@ -209,14 +193,18 @@
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
+        if state is not UNSET:
+            field_dict["state"] = state
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if title is not UNSET:
             field_dict["title"] = title
         if trackers is not UNSET:
             field_dict["trackers"] = trackers
         if description is not UNSET:
             field_dict["description"] = description
         if affects is not UNSET:
@@ -237,32 +225,32 @@
             field_dict["updated_dt"] = updated_dt
         if classification is not UNSET:
             field_dict["classification"] = classification
         if type is not UNSET:
             field_dict["type"] = type
         if cve_id is not UNSET:
             field_dict["cve_id"] = cve_id
-        if state is not UNSET:
-            field_dict["state"] = state
-        if resolution is not UNSET:
-            field_dict["resolution"] = resolution
         if impact is not UNSET:
             field_dict["impact"] = impact
+        if component is not UNSET:
+            field_dict["component"] = component
         if summary is not UNSET:
             field_dict["summary"] = summary
         if statement is not UNSET:
             field_dict["statement"] = statement
         if cwe_id is not UNSET:
             field_dict["cwe_id"] = cwe_id
         if unembargo_dt is not UNSET:
             field_dict["unembargo_dt"] = unembargo_dt
         if source is not UNSET:
             field_dict["source"] = source
         if reported_dt is not UNSET:
             field_dict["reported_dt"] = reported_dt
+        if mitigation is not UNSET:
+            field_dict["mitigation"] = mitigation
         if cvss2 is not UNSET:
             field_dict["cvss2"] = cvss2
         if cvss2_score is not UNSET:
             field_dict["cvss2_score"] = cvss2_score
         if nvd_cvss2 is not UNSET:
             field_dict["nvd_cvss2"] = nvd_cvss2
         if cvss3 is not UNSET:
@@ -285,14 +273,18 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
+        state = d.pop("state", UNSET)
+
+        resolution = d.pop("resolution", UNSET)
+
         title = d.pop("title", UNSET)
 
         trackers = cast(List[str], d.pop("trackers", UNSET))
 
         description = d.pop("description", UNSET)
 
         affects = []
@@ -384,60 +376,22 @@
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawTypeEnum]
+        type: Union[Unset, Type824Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = FlawTypeEnum(_type)
+            type = Type824Enum(_type)
 
         cve_id = d.pop("cve_id", UNSET)
 
-        _state = d.pop("state", UNSET)
-        state: Union[Unset, StateEnum]
-        if isinstance(_state, Unset):
-            state = UNSET
-        else:
-            state = StateEnum(_state)
-
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution01FEnum, Unset]:
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, str):
-                    raise TypeError()
-                _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution01FEnum]
-                if isinstance(_resolution_type_0, Unset):
-                    resolution_type_0 = UNSET
-                else:
-                    resolution_type_0 = Resolution01FEnum(_resolution_type_0)
-
-                return resolution_type_0
-            except:  # noqa: E722
-                pass
-            if not isinstance(data, str):
-                raise TypeError()
-            _resolution_type_1 = data
-            resolution_type_1: Union[Unset, BlankEnum]
-            if isinstance(_resolution_type_1, Unset):
-                resolution_type_1 = UNSET
-            else:
-                resolution_type_1 = BlankEnum(_resolution_type_1)
-
-            return resolution_type_1
-
-        resolution = _parse_resolution(d.pop("resolution", UNSET))
-
         def _parse_impact(data: object) -> Union[BlankEnum, ImpactEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _impact_type_0 = data
@@ -459,14 +413,16 @@
             else:
                 impact_type_1 = BlankEnum(_impact_type_1)
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
+        component = d.pop("component", UNSET)
+
         summary = d.pop("summary", UNSET)
 
         statement = d.pop("statement", UNSET)
 
         cwe_id = d.pop("cwe_id", UNSET)
 
         _unembargo_dt = d.pop("unembargo_dt", UNSET)
@@ -474,26 +430,26 @@
         if _unembargo_dt is None:
             unembargo_dt = None
         elif isinstance(_unembargo_dt, Unset):
             unembargo_dt = UNSET
         else:
             unembargo_dt = isoparse(_unembargo_dt)
 
-        def _parse_source(data: object) -> Union[BlankEnum, FlawSourceEnum, Unset]:
+        def _parse_source(data: object) -> Union[BlankEnum, Source666Enum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _source_type_0 = data
-                source_type_0: Union[Unset, FlawSourceEnum]
+                source_type_0: Union[Unset, Source666Enum]
                 if isinstance(_source_type_0, Unset):
                     source_type_0 = UNSET
                 else:
-                    source_type_0 = FlawSourceEnum(_source_type_0)
+                    source_type_0 = Source666Enum(_source_type_0)
 
                 return source_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _source_type_1 = data
@@ -512,14 +468,16 @@
         if _reported_dt is None:
             reported_dt = None
         elif isinstance(_reported_dt, Unset):
             reported_dt = UNSET
         else:
             reported_dt = isoparse(_reported_dt)
 
+        mitigation = d.pop("mitigation", UNSET)
+
         cvss2 = d.pop("cvss2", UNSET)
 
         cvss2_score = d.pop("cvss2_score", UNSET)
 
         nvd_cvss2 = d.pop("nvd_cvss2", UNSET)
 
         cvss3 = d.pop("cvss3", UNSET)
@@ -541,37 +499,39 @@
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
         osidb_api_v1_flaws_retrieve_response_200 = cls(
             uuid=uuid,
+            state=state,
+            resolution=resolution,
             title=title,
             trackers=trackers,
             description=description,
             affects=affects,
             meta=meta,
             comments=comments,
             meta_attr=meta_attr,
             package_versions=package_versions,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
             type=type,
             cve_id=cve_id,
-            state=state,
-            resolution=resolution,
             impact=impact,
+            component=component,
             summary=summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
+            mitigation=mitigation,
             cvss2=cvss2,
             cvss2_score=cvss2_score,
             nvd_cvss2=nvd_cvss2,
             cvss3=cvss3,
             cvss3_score=cvss3_score,
             nvd_cvss3=nvd_cvss3,
             is_major_incident=is_major_incident,
@@ -584,37 +544,39 @@
         osidb_api_v1_flaws_retrieve_response_200.additional_properties = d
         return osidb_api_v1_flaws_retrieve_response_200
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
+            "state": str,
+            "resolution": str,
             "title": str,
             "trackers": List[str],
             "description": str,
             "affects": List[Affect],
             "meta": List[Meta],
             "comments": List[Comment],
             "meta_attr": FlawMetaAttr,
             "package_versions": List[CVEv5PackageVersions],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
-            "type": FlawTypeEnum,
+            "type": Type824Enum,
             "cve_id": str,
-            "state": StateEnum,
-            "resolution": Union[BlankEnum, Resolution01FEnum],
             "impact": Union[BlankEnum, ImpactEnum],
+            "component": str,
             "summary": str,
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
-            "source": Union[BlankEnum, FlawSourceEnum],
+            "source": Union[BlankEnum, Source666Enum],
             "reported_dt": datetime.datetime,
+            "mitigation": str,
             "cvss2": str,
             "cvss2_score": float,
             "nvd_cvss2": str,
             "cvss3": str,
             "cvss3_score": float,
             "nvd_cvss3": str,
             "is_major_incident": bool,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 
 from ..models.affect import Affect
 from ..models.blank_enum import BlankEnum
 from ..models.comment import Comment
 from ..models.cv_ev_5_package_versions import CVEv5PackageVersions
 from ..models.flaw_classification import FlawClassification
 from ..models.flaw_meta_attr import FlawMetaAttr
-from ..models.flaw_source_enum import FlawSourceEnum
-from ..models.flaw_type_enum import FlawTypeEnum
 from ..models.impact_enum import ImpactEnum
 from ..models.meta import Meta
-from ..models.resolution_01f_enum import Resolution01FEnum
-from ..models.state_enum import StateEnum
+from ..models.source_666_enum import Source666Enum
+from ..models.type_824_enum import Type824Enum
 from ..types import UNSET, OSIDBModel, Unset
 
-T = TypeVar("T", bound="OsidbApiV1FlawsUpdateResponse200")
+T = TypeVar("T", bound="OsidbApiV1FlawsCreateResponse201")
 
 
 @attr.s(auto_attribs=True)
-class OsidbApiV1FlawsUpdateResponse200(OSIDBModel):
+class OsidbApiV1FlawsCreateResponse201(OSIDBModel):
     """ """
 
     uuid: str
+    state: str
+    resolution: str
     title: str
     trackers: List[str]
     description: str
     affects: List[Affect]
     meta: List[Meta]
     comments: List[Comment]
     meta_attr: FlawMetaAttr
     package_versions: List[CVEv5PackageVersions]
     embargoed: bool
     created_dt: datetime.datetime
     updated_dt: datetime.datetime
     classification: FlawClassification
-    type: Union[Unset, FlawTypeEnum] = UNSET
+    type: Union[Unset, Type824Enum] = UNSET
     cve_id: Union[Unset, None, str] = UNSET
-    state: Union[Unset, StateEnum] = UNSET
-    resolution: Union[BlankEnum, Resolution01FEnum, Unset] = UNSET
     impact: Union[BlankEnum, ImpactEnum, Unset] = UNSET
+    component: Union[Unset, str] = UNSET
     summary: Union[Unset, str] = UNSET
     statement: Union[Unset, str] = UNSET
     cwe_id: Union[Unset, str] = UNSET
     unembargo_dt: Union[Unset, None, datetime.datetime] = UNSET
-    source: Union[BlankEnum, FlawSourceEnum, Unset] = UNSET
+    source: Union[BlankEnum, Source666Enum, Unset] = UNSET
     reported_dt: Union[Unset, None, datetime.datetime] = UNSET
+    mitigation: Union[Unset, str] = UNSET
     cvss2: Union[Unset, str] = UNSET
     cvss2_score: Union[Unset, None, float] = UNSET
     nvd_cvss2: Union[Unset, str] = UNSET
     cvss3: Union[Unset, str] = UNSET
     cvss3_score: Union[Unset, None, float] = UNSET
     nvd_cvss3: Union[Unset, str] = UNSET
     is_major_incident: Union[Unset, bool] = UNSET
@@ -60,14 +60,16 @@
     env: Union[Unset, str] = UNSET
     revision: Union[Unset, str] = UNSET
     version: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         uuid = self.uuid
+        state = self.state
+        resolution = self.resolution
         title = self.title
         trackers: List[str] = UNSET
         if not isinstance(self.trackers, Unset):
             trackers = self.trackers
 
         description = self.description
         affects: List[Dict[str, Any]] = UNSET
@@ -126,37 +128,17 @@
         classification: Dict[str, Any] = UNSET
         if not isinstance(self.classification, Unset):
             classification = self.classification.to_dict()
 
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
 
-            type = FlawTypeEnum(self.type).value
+            type = Type824Enum(self.type).value
 
         cve_id = self.cve_id
-        state: Union[Unset, str] = UNSET
-        if not isinstance(self.state, Unset):
-
-            state = StateEnum(self.state).value
-
-        resolution: Union[Unset, str]
-        if isinstance(self.resolution, Unset):
-            resolution = UNSET
-        elif isinstance(self.resolution, Resolution01FEnum):
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = Resolution01FEnum(self.resolution).value
-
-        else:
-            resolution = UNSET
-            if not isinstance(self.resolution, Unset):
-
-                resolution = BlankEnum(self.resolution).value
-
         impact: Union[Unset, str]
         if isinstance(self.impact, Unset):
             impact = UNSET
         elif isinstance(self.impact, ImpactEnum):
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
@@ -164,40 +146,42 @@
 
         else:
             impact = UNSET
             if not isinstance(self.impact, Unset):
 
                 impact = BlankEnum(self.impact).value
 
+        component = self.component
         summary = self.summary
         statement = self.statement
         cwe_id = self.cwe_id
         unembargo_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.unembargo_dt, Unset):
             unembargo_dt = self.unembargo_dt.isoformat() if self.unembargo_dt else None
 
         source: Union[Unset, str]
         if isinstance(self.source, Unset):
             source = UNSET
-        elif isinstance(self.source, FlawSourceEnum):
+        elif isinstance(self.source, Source666Enum):
             source = UNSET
             if not isinstance(self.source, Unset):
 
-                source = FlawSourceEnum(self.source).value
+                source = Source666Enum(self.source).value
 
         else:
             source = UNSET
             if not isinstance(self.source, Unset):
 
                 source = BlankEnum(self.source).value
 
         reported_dt: Union[Unset, None, str] = UNSET
         if not isinstance(self.reported_dt, Unset):
             reported_dt = self.reported_dt.isoformat() if self.reported_dt else None
 
+        mitigation = self.mitigation
         cvss2 = self.cvss2
         cvss2_score = self.cvss2_score
         nvd_cvss2 = self.nvd_cvss2
         cvss3 = self.cvss3
         cvss3_score = self.cvss3_score
         nvd_cvss3 = self.nvd_cvss3
         is_major_incident = self.is_major_incident
@@ -209,14 +193,18 @@
         revision = self.revision
         version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         if uuid is not UNSET:
             field_dict["uuid"] = uuid
+        if state is not UNSET:
+            field_dict["state"] = state
+        if resolution is not UNSET:
+            field_dict["resolution"] = resolution
         if title is not UNSET:
             field_dict["title"] = title
         if trackers is not UNSET:
             field_dict["trackers"] = trackers
         if description is not UNSET:
             field_dict["description"] = description
         if affects is not UNSET:
@@ -237,32 +225,32 @@
             field_dict["updated_dt"] = updated_dt
         if classification is not UNSET:
             field_dict["classification"] = classification
         if type is not UNSET:
             field_dict["type"] = type
         if cve_id is not UNSET:
             field_dict["cve_id"] = cve_id
-        if state is not UNSET:
-            field_dict["state"] = state
-        if resolution is not UNSET:
-            field_dict["resolution"] = resolution
         if impact is not UNSET:
             field_dict["impact"] = impact
+        if component is not UNSET:
+            field_dict["component"] = component
         if summary is not UNSET:
             field_dict["summary"] = summary
         if statement is not UNSET:
             field_dict["statement"] = statement
         if cwe_id is not UNSET:
             field_dict["cwe_id"] = cwe_id
         if unembargo_dt is not UNSET:
             field_dict["unembargo_dt"] = unembargo_dt
         if source is not UNSET:
             field_dict["source"] = source
         if reported_dt is not UNSET:
             field_dict["reported_dt"] = reported_dt
+        if mitigation is not UNSET:
+            field_dict["mitigation"] = mitigation
         if cvss2 is not UNSET:
             field_dict["cvss2"] = cvss2
         if cvss2_score is not UNSET:
             field_dict["cvss2_score"] = cvss2_score
         if nvd_cvss2 is not UNSET:
             field_dict["nvd_cvss2"] = nvd_cvss2
         if cvss3 is not UNSET:
@@ -285,14 +273,18 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         uuid = d.pop("uuid", UNSET)
 
+        state = d.pop("state", UNSET)
+
+        resolution = d.pop("resolution", UNSET)
+
         title = d.pop("title", UNSET)
 
         trackers = cast(List[str], d.pop("trackers", UNSET))
 
         description = d.pop("description", UNSET)
 
         affects = []
@@ -384,60 +376,22 @@
         classification: FlawClassification
         if isinstance(_classification, Unset):
             classification = UNSET
         else:
             classification = FlawClassification.from_dict(_classification)
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, FlawTypeEnum]
+        type: Union[Unset, Type824Enum]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = FlawTypeEnum(_type)
+            type = Type824Enum(_type)
 
         cve_id = d.pop("cve_id", UNSET)
 
-        _state = d.pop("state", UNSET)
-        state: Union[Unset, StateEnum]
-        if isinstance(_state, Unset):
-            state = UNSET
-        else:
-            state = StateEnum(_state)
-
-        def _parse_resolution(
-            data: object,
-        ) -> Union[BlankEnum, Resolution01FEnum, Unset]:
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, str):
-                    raise TypeError()
-                _resolution_type_0 = data
-                resolution_type_0: Union[Unset, Resolution01FEnum]
-                if isinstance(_resolution_type_0, Unset):
-                    resolution_type_0 = UNSET
-                else:
-                    resolution_type_0 = Resolution01FEnum(_resolution_type_0)
-
-                return resolution_type_0
-            except:  # noqa: E722
-                pass
-            if not isinstance(data, str):
-                raise TypeError()
-            _resolution_type_1 = data
-            resolution_type_1: Union[Unset, BlankEnum]
-            if isinstance(_resolution_type_1, Unset):
-                resolution_type_1 = UNSET
-            else:
-                resolution_type_1 = BlankEnum(_resolution_type_1)
-
-            return resolution_type_1
-
-        resolution = _parse_resolution(d.pop("resolution", UNSET))
-
         def _parse_impact(data: object) -> Union[BlankEnum, ImpactEnum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _impact_type_0 = data
@@ -459,14 +413,16 @@
             else:
                 impact_type_1 = BlankEnum(_impact_type_1)
 
             return impact_type_1
 
         impact = _parse_impact(d.pop("impact", UNSET))
 
+        component = d.pop("component", UNSET)
+
         summary = d.pop("summary", UNSET)
 
         statement = d.pop("statement", UNSET)
 
         cwe_id = d.pop("cwe_id", UNSET)
 
         _unembargo_dt = d.pop("unembargo_dt", UNSET)
@@ -474,26 +430,26 @@
         if _unembargo_dt is None:
             unembargo_dt = None
         elif isinstance(_unembargo_dt, Unset):
             unembargo_dt = UNSET
         else:
             unembargo_dt = isoparse(_unembargo_dt)
 
-        def _parse_source(data: object) -> Union[BlankEnum, FlawSourceEnum, Unset]:
+        def _parse_source(data: object) -> Union[BlankEnum, Source666Enum, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
                 _source_type_0 = data
-                source_type_0: Union[Unset, FlawSourceEnum]
+                source_type_0: Union[Unset, Source666Enum]
                 if isinstance(_source_type_0, Unset):
                     source_type_0 = UNSET
                 else:
-                    source_type_0 = FlawSourceEnum(_source_type_0)
+                    source_type_0 = Source666Enum(_source_type_0)
 
                 return source_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, str):
                 raise TypeError()
             _source_type_1 = data
@@ -512,14 +468,16 @@
         if _reported_dt is None:
             reported_dt = None
         elif isinstance(_reported_dt, Unset):
             reported_dt = UNSET
         else:
             reported_dt = isoparse(_reported_dt)
 
+        mitigation = d.pop("mitigation", UNSET)
+
         cvss2 = d.pop("cvss2", UNSET)
 
         cvss2_score = d.pop("cvss2_score", UNSET)
 
         nvd_cvss2 = d.pop("nvd_cvss2", UNSET)
 
         cvss3 = d.pop("cvss3", UNSET)
@@ -539,82 +497,86 @@
 
         env = d.pop("env", UNSET)
 
         revision = d.pop("revision", UNSET)
 
         version = d.pop("version", UNSET)
 
-        osidb_api_v1_flaws_update_response_200 = cls(
+        osidb_api_v1_flaws_create_response_201 = cls(
             uuid=uuid,
+            state=state,
+            resolution=resolution,
             title=title,
             trackers=trackers,
             description=description,
             affects=affects,
             meta=meta,
             comments=comments,
             meta_attr=meta_attr,
             package_versions=package_versions,
             embargoed=embargoed,
             created_dt=created_dt,
             updated_dt=updated_dt,
             classification=classification,
             type=type,
             cve_id=cve_id,
-            state=state,
-            resolution=resolution,
             impact=impact,
+            component=component,
             summary=summary,
             statement=statement,
             cwe_id=cwe_id,
             unembargo_dt=unembargo_dt,
             source=source,
             reported_dt=reported_dt,
+            mitigation=mitigation,
             cvss2=cvss2,
             cvss2_score=cvss2_score,
             nvd_cvss2=nvd_cvss2,
             cvss3=cvss3,
             cvss3_score=cvss3_score,
             nvd_cvss3=nvd_cvss3,
             is_major_incident=is_major_incident,
             dt=dt,
             env=env,
             revision=revision,
             version=version,
         )
 
-        osidb_api_v1_flaws_update_response_200.additional_properties = d
-        return osidb_api_v1_flaws_update_response_200
+        osidb_api_v1_flaws_create_response_201.additional_properties = d
+        return osidb_api_v1_flaws_create_response_201
 
     @staticmethod
     def get_fields():
         return {
             "uuid": str,
+            "state": str,
+            "resolution": str,
             "title": str,
             "trackers": List[str],
             "description": str,
             "affects": List[Affect],
             "meta": List[Meta],
             "comments": List[Comment],
             "meta_attr": FlawMetaAttr,
             "package_versions": List[CVEv5PackageVersions],
             "embargoed": bool,
             "created_dt": datetime.datetime,
             "updated_dt": datetime.datetime,
             "classification": FlawClassification,
-            "type": FlawTypeEnum,
+            "type": Type824Enum,
             "cve_id": str,
-            "state": StateEnum,
-            "resolution": Union[BlankEnum, Resolution01FEnum],
             "impact": Union[BlankEnum, ImpactEnum],
+            "component": str,
             "summary": str,
             "statement": str,
             "cwe_id": str,
             "unembargo_dt": datetime.datetime,
-            "source": Union[BlankEnum, FlawSourceEnum],
+            "source": Union[BlankEnum, Source666Enum],
             "reported_dt": datetime.datetime,
+            "mitigation": str,
             "cvss2": str,
             "cvss2_score": float,
             "nvd_cvss2": str,
             "cvss3": str,
             "cvss3_score": float,
             "nvd_cvss3": str,
             "is_major_incident": bool,
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_affect_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_epss_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/supported_products.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/supported_products.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_obtain_pair.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_refresh.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_refresh.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/token_verify.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/token_verify.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/models/tracker_report_data.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/bindings/python_client/types.py` & `osidb-bindings-3.1.0/osidb_bindings/bindings/python_client/types.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings/session.py` & `osidb-bindings-3.1.0/osidb_bindings/session.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.0.2/osidb_bindings.egg-info/PKG-INFO` & `osidb-bindings-3.1.0/osidb_bindings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.0.2
+Version: 3.1.0
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.0.2/osidb_bindings.egg-info/SOURCES.txt` & `osidb-bindings-3.1.0/osidb_bindings.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -54,19 +54,32 @@
 osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
 osidb_bindings/bindings/python_client/api/osim/__init__.py
 osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
 osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
 osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
 osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
 osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
+osidb_bindings/bindings/python_client/api/taskman/__init__.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py
+osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py
 osidb_bindings/bindings/python_client/models/__init__.py
 osidb_bindings/bindings/python_client/models/affect.py
 osidb_bindings/bindings/python_client/models/affect_meta_attr.py
+osidb_bindings/bindings/python_client/models/affect_post.py
+osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/affect_report_data.py
-osidb_bindings/bindings/python_client/models/affect_type_enum.py
 osidb_bindings/bindings/python_client/models/affectedness_enum.py
 osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
 osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
 osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
 osidb_bindings/bindings/python_client/models/blank_enum.py
 osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
@@ -101,47 +114,72 @@
 osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
 osidb_bindings/bindings/python_client/models/flaw.py
 osidb_bindings/bindings/python_client/models/flaw_classification.py
 osidb_bindings/bindings/python_client/models/flaw_classification_state.py
 osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
+osidb_bindings/bindings/python_client/models/flaw_post.py
+osidb_bindings/bindings/python_client/models/flaw_post_classification.py
+osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
+osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
 osidb_bindings/bindings/python_client/models/flaw_report_data.py
-osidb_bindings/bindings/python_client/models/flaw_source_enum.py
-osidb_bindings/bindings/python_client/models/flaw_type_enum.py
 osidb_bindings/bindings/python_client/models/impact_enum.py
+osidb_bindings/bindings/python_client/models/jira_comment.py
+osidb_bindings/bindings/python_client/models/jira_issue.py
+osidb_bindings/bindings/python_client/models/jira_issue_fields.py
+osidb_bindings/bindings/python_client/models/jira_issue_query_result.py
+osidb_bindings/bindings/python_client/models/jira_issue_type.py
+osidb_bindings/bindings/python_client/models/jira_user.py
 osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
 osidb_bindings/bindings/python_client/models/meta.py
 osidb_bindings/bindings/python_client/models/meta_meta_attr.py
 osidb_bindings/bindings/python_client/models/meta_type_enum.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
-osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_resolution.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
-osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_state.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
+osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
 osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
 osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
@@ -152,22 +190,35 @@
 osidb_bindings/bindings/python_client/models/paginated_affect_list.py
 osidb_bindings/bindings/python_client/models/paginated_epss_list.py
 osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
 osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
 osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
 osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
 osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
-osidb_bindings/bindings/python_client/models/resolution_01f_enum.py
-osidb_bindings/bindings/python_client/models/resolution_3_ac_enum.py
-osidb_bindings/bindings/python_client/models/state_enum.py
+osidb_bindings/bindings/python_client/models/resolution_enum.py
+osidb_bindings/bindings/python_client/models/source_666_enum.py
 osidb_bindings/bindings/python_client/models/status_enum.py
 osidb_bindings/bindings/python_client/models/supported_products.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_204.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_204.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_204.py
+osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_status.py
+osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py
 osidb_bindings/bindings/python_client/models/token_obtain_pair.py
 osidb_bindings/bindings/python_client/models/token_refresh.py
 osidb_bindings/bindings/python_client/models/token_verify.py
 osidb_bindings/bindings/python_client/models/tracker.py
 osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
 osidb_bindings/bindings/python_client/models/tracker_report_data.py
 osidb_bindings/bindings/python_client/models/type_0d0_enum.py
+osidb_bindings/bindings/python_client/models/type_5b2_enum.py
+osidb_bindings/bindings/python_client/models/type_824_enum.py
 tests/__init__.py
 tests/conftest.py
 tests/test_core.py
```

### Comparing `osidb-bindings-3.0.2/setup.py` & `osidb-bindings-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="osidb-bindings",
-    version="3.0.2",
+    version="3.1.0",
     author="Jakub Frejlach, Red Hat Product Security",
     author_email="jfrejlac@redhat.com",
     description="Python bindings for accessing OSIDB API",
     url="https://github.com/RedHatProductSecurity/osidb-bindings",
     project_urls={
         "Changelog": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md",
         "Documentation": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md",
```

