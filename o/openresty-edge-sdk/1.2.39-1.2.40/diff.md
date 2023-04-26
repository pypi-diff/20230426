# Comparing `tmp/openresty-edge-sdk-1.2.39.tar.gz` & `tmp/openresty-edge-sdk-1.2.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/root/orinc/edge-sdk/python-client/buildroot/dist/.tmp-42eumuzc/openresty-edge-sdk-1.2.39.tar", last modified: Mon Feb 13 13:49:13 2023, max compression
+gzip compressed data, was "/root/orinc/edge-sdk/python-client/buildroot/dist/.tmp-fbl1ixzr/openresty-edge-sdk-1.2.40.tar", last modified: Wed Apr 26 09:09:50 2023, max compression
```

## Comparing `openresty-edge-sdk-1.2.39.tar` & `openresty-edge-sdk-1.2.40.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 13:49:13.149165 openresty-edge-sdk-1.2.39/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1124 2023-02-13 13:49:13.149165 openresty-edge-sdk-1.2.39/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 13:49:13.121164 openresty-edge-sdk-1.2.39/edge2client/
--rw-r--r--   0 root         (0) root         (0)      348 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108628 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/edge2client.py
--rw-r--r--   0 root         (0) root         (0)    14560 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/edge_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 13:49:13.133165 openresty-edge-sdk-1.2.39/edge2client/utils/
--rw-r--r--   0 root         (0) root         (0)      596 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/batch_release.py
--rw-r--r--   0 root         (0) root         (0)     8482 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/copy_app.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/create_app.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/create_apps.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/delete_all_apps.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/export_apps.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/get_app_id_by_global_rule.py
--rw-r--r--   0 root         (0) root         (0)     6943 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/global_ini.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/ngx_emer_conf.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/py_client.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/query_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/release_app.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/remove_useless_conf.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/sync_eureka.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/update_dns.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/update_proxy_timeout.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/update_src_ip.py
--rw-r--r--   0 root         (0) root         (0)     8027 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/update_upstream_group_weight.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/update_upstream_weight.py
--rw-r--r--   0 root         (0) root         (0)     4802 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils/utils_common.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/utils_common.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/edge2client/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 13:49:13.133165 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-02-13 13:49:13.000000 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1748 2023-02-13 13:49:13.000000 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-13 13:49:13.000000 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-13 13:49:13.000000 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-13 13:49:13.000000 openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-13 13:49:13.149165 openresty-edge-sdk-1.2.39/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1302 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-13 13:49:13.149165 openresty-edge-sdk-1.2.39/tests/
--rw-r--r--   0 root         (0) root         (0)      548 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_app.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_app_dymetrics.py
--rw-r--r--   0 root         (0) root         (0)      216 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_app_metrics.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_cache_purge.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5600 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_dns.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1201 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_global_dymetrics.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_global_k8s.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_global_k8s_domain.py
--rw-r--r--   0 root         (0) root         (0)    26128 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_global_rule.py
--rw-r--r--   0 root         (0) root         (0)     1552 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_ip_list.py
--rw-r--r--   0 root         (0) root         (0)     9521 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_k8s_upstream.py
--rw-r--r--   0 root         (0) root         (0)      299 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_lmdb.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_login.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_node_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_partition_lua_module.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_referenced.py
--rw-r--r--   0 root         (0) root         (0)    11029 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_rule_reorder.py
--rw-r--r--   0 root         (0) root         (0)     6703 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_status.py
--rw-r--r--   0 root         (0) root         (0)     8244 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_upstream_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_variable.py
--rw-r--r--   0 root         (0) root         (0)      421 2023-02-13 13:49:01.000000 openresty-edge-sdk-1.2.39/tests/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:09:50.075554 openresty-edge-sdk-1.2.40/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-26 09:09:50.075554 openresty-edge-sdk-1.2.40/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:09:50.071554 openresty-edge-sdk-1.2.40/edge2client/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108622 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/edge2client.py
+-rw-r--r--   0 root         (0) root         (0)    14560 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/edge_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:09:50.071554 openresty-edge-sdk-1.2.40/edge2client/utils/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/batch_release.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/copy_app.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/create_app.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/create_apps.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/delete_all_apps.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/export_apps.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/get_app_id_by_global_rule.py
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/global_ini.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/ngx_emer_conf.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/py_client.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/query_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/release_app.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/remove_useless_conf.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/sync_eureka.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/update_dns.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/update_proxy_timeout.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/update_src_ip.py
+-rw-r--r--   0 root         (0) root         (0)     8027 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/update_upstream_group_weight.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/update_upstream_weight.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils/utils_common.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/utils_common.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/edge2client/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:09:50.071554 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-26 09:09:50.000000 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-04-26 09:09:50.000000 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:09:50.000000 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-26 09:09:50.000000 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 09:09:50.000000 openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 09:09:50.075554 openresty-edge-sdk-1.2.40/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:09:50.075554 openresty-edge-sdk-1.2.40/tests/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_app.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_app_dymetrics.py
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_app_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_cache_purge.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5600 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_dns.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_global_dymetrics.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_global_k8s.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_global_k8s_domain.py
+-rw-r--r--   0 root         (0) root         (0)    26128 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_global_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_ip_list.py
+-rw-r--r--   0 root         (0) root         (0)     9521 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_k8s_upstream.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_lmdb.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_login.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_node_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_partition_lua_module.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_referenced.py
+-rw-r--r--   0 root         (0) root         (0)    11056 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_rule_reorder.py
+-rw-r--r--   0 root         (0) root         (0)     6703 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_status.py
+-rw-r--r--   0 root         (0) root         (0)     8244 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_upstream_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_variable.py
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-26 09:09:42.000000 openresty-edge-sdk-1.2.40/tests/test_version.py
```

### Comparing `openresty-edge-sdk-1.2.39/LICENSE` & `openresty-edge-sdk-1.2.40/LICENSE`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/PKG-INFO` & `openresty-edge-sdk-1.2.40/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openresty-edge-sdk
-Version: 1.2.39
+Version: 1.2.40
 Summary: OpenResty Edge Python SDK
 Home-page: https://www.openresty.com
 Author: OpenResty Inc.
 Author-email: support@openresty.com
 Keywords: openresty-edge-sdk,edge2client,python,sdk
 Platform: Platform Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openresty-edge-sdk-1.2.39/edge2client/edge2client.py` & `openresty-edge-sdk-1.2.40/edge2client/edge2client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1250,15 +1250,15 @@
         return self.do_api('GET', url)
 
     def get_all_cert_keys(self, app_id=None):
         app_id = app_id or self.app_id
         if not app_id:
             raise Exception('no active application selected')
 
-        return self.do_api('GET', AppSslCertUrl.format(app_id))
+        return self.get_all(AppSslCertUrl.format(app_id))
 
     def del_cert_key(self, cert_id):
         if not self.app_id:
             raise Exception('no active application selected')
         if not cert_id:
             raise Exception('no active cert selected')
```

### Comparing `openresty-edge-sdk-1.2.39/edge2client/edge_common.py` & `openresty-edge-sdk-1.2.40/edge2client/edge_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/batch_release.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/batch_release.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/copy_app.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/copy_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/create_app.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/create_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/create_apps.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/create_apps.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/export_apps.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/export_apps.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/get_app_id_by_global_rule.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/get_app_id_by_global_rule.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/global_ini.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/global_ini.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/ngx_emer_conf.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/ngx_emer_conf.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/py_client.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/py_client.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/query_rule_id.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/query_rule_id.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/release_app.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/release_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/remove_useless_conf.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/remove_useless_conf.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/sync_eureka.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/sync_eureka.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/update_dns.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/update_dns.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/update_proxy_timeout.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/update_proxy_timeout.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/update_src_ip.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/update_src_ip.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/update_upstream_group_weight.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/update_upstream_group_weight.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/update_upstream_weight.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/update_upstream_weight.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils/utils_common.py` & `openresty-edge-sdk-1.2.40/edge2client/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/edge2client/utils_common.py` & `openresty-edge-sdk-1.2.40/edge2client/utils_common.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/PKG-INFO` & `openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openresty-edge-sdk
-Version: 1.2.39
+Version: 1.2.40
 Summary: OpenResty Edge Python SDK
 Home-page: https://www.openresty.com
 Author: OpenResty Inc.
 Author-email: support@openresty.com
 Keywords: openresty-edge-sdk,edge2client,python,sdk
 Platform: Platform Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openresty-edge-sdk-1.2.39/openresty_edge_sdk.egg-info/SOURCES.txt` & `openresty-edge-sdk-1.2.40/openresty_edge_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/setup.py` & `openresty-edge-sdk-1.2.40/setup.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test.py` & `openresty-edge-sdk-1.2.40/tests/test.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_app.py` & `openresty-edge-sdk-1.2.40/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_app_dymetrics.py` & `openresty-edge-sdk-1.2.40/tests/test_app_dymetrics.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_cache_purge.py` & `openresty-edge-sdk-1.2.40/tests/test_cache_purge.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_cluster.py` & `openresty-edge-sdk-1.2.40/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_dns.py` & `openresty-edge-sdk-1.2.40/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_gateway.py` & `openresty-edge-sdk-1.2.40/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_global_dymetrics.py` & `openresty-edge-sdk-1.2.40/tests/test_global_dymetrics.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_global_k8s.py` & `openresty-edge-sdk-1.2.40/tests/test_global_k8s.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_global_k8s_domain.py` & `openresty-edge-sdk-1.2.40/tests/test_global_k8s_domain.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_global_rule.py` & `openresty-edge-sdk-1.2.40/tests/test_global_rule.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_ip_list.py` & `openresty-edge-sdk-1.2.40/tests/test_ip_list.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_k8s_upstream.py` & `openresty-edge-sdk-1.2.40/tests/test_k8s_upstream.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_login.py` & `openresty-edge-sdk-1.2.40/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_node_monitor.py` & `openresty-edge-sdk-1.2.40/tests/test_node_monitor.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_nodes.py` & `openresty-edge-sdk-1.2.40/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_partition_lua_module.py` & `openresty-edge-sdk-1.2.40/tests/test_partition_lua_module.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_rule.py` & `openresty-edge-sdk-1.2.40/tests/test_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         self.assertGreater(new_file_id, 0)
 
         ok = self.client.put_rule(rule_id=rule_id,
                                   content={'favicon': new_file_id})
         self.assertTrue(ok)
 
         data = self.client.get_rule(rule_id)
-        self.assertEqual(data['content']['favicon'], new_file_id)
+
+        self.assertEqual(data['content']['file'], new_file_id)
         self.assertEqual(data['conditions'][0]['values'][0]['val'],
                          '/favicon.ico')
 
         ok = self.client.del_rule(rule_id)
         self.assertTrue(ok)
 
         ok = self.client.del_favicon(file_id)
@@ -279,10 +280,12 @@
                                   order=1)
         self.assertTrue(ok)
 
         data = self.client.get_rule(rule_id)
         self.assertEqual(data['order'], 1)
 
         ok = self.client.del_rule(rule_id)
+        self.assertTrue(ok)
+
         ok = self.client.del_favicon(file_id)
         ok = self.client.del_favicon(new_file_id)
         self.assertTrue(ok)
```

### Comparing `openresty-edge-sdk-1.2.39/tests/test_rule_reorder.py` & `openresty-edge-sdk-1.2.40/tests/test_rule_reorder.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_search.py` & `openresty-edge-sdk-1.2.40/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_status.py` & `openresty-edge-sdk-1.2.40/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_upstream_proxy.py` & `openresty-edge-sdk-1.2.40/tests/test_upstream_proxy.py`

 * *Files identical despite different names*

### Comparing `openresty-edge-sdk-1.2.39/tests/test_variable.py` & `openresty-edge-sdk-1.2.40/tests/test_variable.py`

 * *Files identical despite different names*

