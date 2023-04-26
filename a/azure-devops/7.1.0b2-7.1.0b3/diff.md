# Comparing `tmp/azure-devops-7.1.0b2.tar.gz` & `tmp/azure-devops-7.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-devops-7.1.0b2.tar", last modified: Tue Apr 25 19:06:58 2023, max compression
+gzip compressed data, was "azure-devops-7.1.0b3.tar", last modified: Wed Apr 26 17:35:57 2023, max compression
```

## Comparing `azure-devops-7.1.0b2.tar` & `azure-devops-7.1.0b3.tar`

### file list

```diff
@@ -1,601 +1,601 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.280151 azure-devops-7.1.0b2/
--rw-rw-rw-   0        0        0     1114 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/LICENSE.txt
--rw-rw-rw-   0        0        0       21 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0      930 2023-04-25 19:06:58.279142 azure-devops-7.1.0b2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.287441 azure-devops-7.1.0b2/azure/
--rw-rw-rw-   0        0        0      408 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.305009 azure-devops-7.1.0b2/azure/devops/
--rw-rw-rw-   0        0        0      408 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/__init__.py
--rw-rw-rw-   0        0        0     6471 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/_file_cache.py
--rw-rw-rw-   0        0        0     6311 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/_models.py
--rw-rw-rw-   0        0        0    16010 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/client.py
--rw-rw-rw-   0        0        0      770 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/client_configuration.py
--rw-rw-rw-   0        0        0     6471 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/connection.py
--rw-rw-rw-   0        0        0      467 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/credentials.py
--rw-rw-rw-   0        0        0     1550 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.310097 azure-devops-7.1.0b2/azure/devops/issue_tests/
--rw-rw-rw-   0        0        0      557 2021-12-01 09:17:04.000000 azure-devops-7.1.0b2/azure/devops/issue_tests/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/issue_tests/test_issue_268.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.313320 azure-devops-7.1.0b2/azure/devops/released/
--rw-rw-rw-   0        0        0      557 2023-04-17 18:43:56.000000 azure-devops-7.1.0b2/azure/devops/released/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.318344 azure-devops-7.1.0b2/azure/devops/released/accounts/
--rw-rw-rw-   0        0        0      758 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/accounts/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/accounts/accounts_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.322874 azure-devops-7.1.0b2/azure/devops/released/build/
--rw-rw-rw-   0        0        0     3127 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/build/__init__.py
--rw-rw-rw-   0        0        0   111801 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/build/build_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.326873 azure-devops-7.1.0b2/azure/devops/released/cix/
--rw-rw-rw-   0        0        0     1024 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/cix/__init__.py
--rw-rw-rw-   0        0        0     7619 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/cix/cix_client.py
--rw-rw-rw-   0        0        0    21262 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.332048 azure-devops-7.1.0b2/azure/devops/released/core/
--rw-rw-rw-   0        0        0     1287 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/core/__init__.py
--rw-rw-rw-   0        0        0    16996 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/core/core_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.337047 azure-devops-7.1.0b2/azure/devops/released/elastic/
--rw-rw-rw-   0        0        0      957 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/elastic/__init__.py
--rw-rw-rw-   0        0        0     8731 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/elastic/elastic_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.342243 azure-devops-7.1.0b2/azure/devops/released/feed/
--rw-rw-rw-   0        0        0     1446 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/feed/__init__.py
--rw-rw-rw-   0        0        0    52098 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/feed/feed_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.348248 azure-devops-7.1.0b2/azure/devops/released/git/
--rw-rw-rw-   0        0        0     3459 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/git/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-04-25 18:35:24.000000 azure-devops-7.1.0b2/azure/devops/released/git/git_client.py
--rw-rw-rw-   0        0        0   207990 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/git/git_client_base.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.352939 azure-devops-7.1.0b2/azure/devops/released/graph/
--rw-rw-rw-   0        0        0     1323 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/graph/__init__.py
--rw-rw-rw-   0        0        0     5689 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/graph/graph_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.356936 azure-devops-7.1.0b2/azure/devops/released/identity/
--rw-rw-rw-   0        0        0     1181 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/identity/__init__.py
--rw-rw-rw-   0        0        0    14236 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/identity/identity_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.360960 azure-devops-7.1.0b2/azure/devops/released/member_entitlement_management/
--rw-rw-rw-   0        0        0     1731 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/member_entitlement_management/__init__.py
--rw-rw-rw-   0        0        0    18778 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/member_entitlement_management/member_entitlement_management_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.364961 azure-devops-7.1.0b2/azure/devops/released/notification/
--rw-rw-rw-   0        0        0     2632 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/notification/__init__.py
--rw-rw-rw-   0        0        0    16939 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/notification/notification_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.368979 azure-devops-7.1.0b2/azure/devops/released/npm/
--rw-rw-rw-   0        0        0      993 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/npm/__init__.py
--rw-rw-rw-   0        0        0    33791 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/npm/npm_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.374328 azure-devops-7.1.0b2/azure/devops/released/nuget/
--rw-rw-rw-   0        0        0     1002 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/nuget/__init__.py
--rw-rw-rw-   0        0        0     8101 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/nuget/nuget_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.378853 azure-devops-7.1.0b2/azure/devops/released/operations/
--rw-rw-rw-   0        0        0      781 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/operations/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/operations/operations_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.384871 azure-devops-7.1.0b2/azure/devops/released/pipelines/
--rw-rw-rw-   0        0        0     1316 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/pipelines/__init__.py
--rw-rw-rw-   0        0        0    14185 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/pipelines/pipelines_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.390010 azure-devops-7.1.0b2/azure/devops/released/policy/
--rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/policy/__init__.py
--rw-rw-rw-   0        0        0    11569 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/policy/policy_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.395022 azure-devops-7.1.0b2/azure/devops/released/profile/
--rw-rw-rw-   0        0        0      923 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/profile/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/profile/profile_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.399163 azure-devops-7.1.0b2/azure/devops/released/project_analysis/
--rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/project_analysis/__init__.py
--rw-rw-rw-   0        0        0     6350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/project_analysis/project_analysis_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.404169 azure-devops-7.1.0b2/azure/devops/released/release/
--rw-rw-rw-   0        0        0     3488 2023-04-17 18:43:56.000000 azure-devops-7.1.0b2/azure/devops/released/release/__init__.py
--rw-rw-rw-   0        0        0    54731 2023-04-17 18:43:56.000000 azure-devops-7.1.0b2/azure/devops/released/release/release_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.409340 azure-devops-7.1.0b2/azure/devops/released/search/
--rw-rw-rw-   0        0        0     1674 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/search/__init__.py
--rw-rw-rw-   0        0        0     7964 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/search/search_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.414376 azure-devops-7.1.0b2/azure/devops/released/security/
--rw-rw-rw-   0        0        0      914 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/security/__init__.py
--rw-rw-rw-   0        0        0    14139 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/security/security_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.420203 azure-devops-7.1.0b2/azure/devops/released/service_endpoint/
--rw-rw-rw-   0        0        0     1914 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/service_endpoint/__init__.py
--rw-rw-rw-   0        0        0    17368 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/service_endpoint/service_endpoint_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.424208 azure-devops-7.1.0b2/azure/devops/released/service_hooks/
--rw-rw-rw-   0        0        0     1585 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/service_hooks/__init__.py
--rw-rw-rw-   0        0        0    21328 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/service_hooks/service_hooks_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.428210 azure-devops-7.1.0b2/azure/devops/released/symbol/
--rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/symbol/__init__.py
--rw-rw-rw-   0        0        0    13273 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/symbol/symbol_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.432242 azure-devops-7.1.0b2/azure/devops/released/task/
--rw-rw-rw-   0        0        0     1380 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/task/__init__.py
--rw-rw-rw-   0        0        0    27864 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/task/task_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.437244 azure-devops-7.1.0b2/azure/devops/released/task_agent/
--rw-rw-rw-   0        0        0     4218 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/task_agent/__init__.py
--rw-rw-rw-   0        0        0    67774 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/task_agent/task_agent_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.441264 azure-devops-7.1.0b2/azure/devops/released/test/
--rw-rw-rw-   0        0        0     3628 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test/__init__.py
--rw-rw-rw-   0        0        0    68807 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test/test_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.446265 azure-devops-7.1.0b2/azure/devops/released/test_plan/
--rw-rw-rw-   0        0        0     2494 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test_plan/__init__.py
--rw-rw-rw-   0        0        0    55139 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test_plan/test_plan_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.450215 azure-devops-7.1.0b2/azure/devops/released/test_results/
--rw-rw-rw-   0        0        0     3289 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test_results/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/test_results/test_results_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.453214 azure-devops-7.1.0b2/azure/devops/released/tfvc/
--rw-rw-rw-   0        0        0     1599 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/tfvc/__init__.py
--rw-rw-rw-   0        0        0    46550 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/tfvc/tfvc_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.457216 azure-devops-7.1.0b2/azure/devops/released/token_admin/
--rw-rw-rw-   0        0        0      828 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/token_admin/__init__.py
--rw-rw-rw-   0        0        0     5194 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/token_admin/token_admin_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.461239 azure-devops-7.1.0b2/azure/devops/released/wiki/
--rw-rw-rw-   0        0        0     1472 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/wiki/__init__.py
--rw-rw-rw-   0        0        0    37968 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/wiki/wiki_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.464239 azure-devops-7.1.0b2/azure/devops/released/work/
--rw-rw-rw-   0        0        0     2634 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work/__init__.py
--rw-rw-rw-   0        0        0    77478 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work/work_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.467242 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking/
--rw-rw-rw-   0        0        0     3174 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking/__init__.py
--rw-rw-rw-   0        0        0    97796 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking/work_item_tracking_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.471262 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process/
--rw-rw-rw-   0        0        0     1851 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process/__init__.py
--rw-rw-rw-   0        0        0    68350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process/work_item_tracking_process_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.474261 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process_template/
--rw-rw-rw-   0        0        0      937 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process_template/__init__.py
--rw-rw-rw-   0        0        0     6488 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process_template/work_item_tracking_process_template_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.479275 azure-devops-7.1.0b2/azure/devops/v7_0/
--rw-rw-rw-   0        0        0      557 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.485292 azure-devops-7.1.0b2/azure/devops/v7_0/accounts/
--rw-rw-rw-   0        0        0      742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/accounts/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/accounts/accounts_client.py
--rw-rw-rw-   0        0        0     6285 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/accounts/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.491831 azure-devops-7.1.0b2/azure/devops/v7_0/audit/
--rw-rw-rw-   0        0        0      771 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/audit/__init__.py
--rw-rw-rw-   0        0        0     9739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/audit/audit_client.py
--rw-rw-rw-   0        0        0    13099 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/audit/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.496832 azure-devops-7.1.0b2/azure/devops/v7_0/build/
--rw-rw-rw-   0        0        0     3114 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/build/__init__.py
--rw-rw-rw-   0        0        0   130017 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/build/build_client.py
--rw-rw-rw-   0        0        0   150112 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/build/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.504871 azure-devops-7.1.0b2/azure/devops/v7_0/cix/
--rw-rw-rw-   0        0        0     1013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/cix/__init__.py
--rw-rw-rw-   0        0        0     7609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/cix/cix_client.py
--rw-rw-rw-   0        0        0    16667 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/cix/models.py
--rw-rw-rw-   0        0        0    21261 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.510917 azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/
--rw-rw-rw-   0        0        0      694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/client_trace_client.py
--rw-rw-rw-   0        0        0     1978 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.515913 azure-devops-7.1.0b2/azure/devops/v7_0/contributions/
--rw-rw-rw-   0        0        0     1406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/contributions/__init__.py
--rw-rw-rw-   0        0        0     5750 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/contributions/contributions_client.py
--rw-rw-rw-   0        0        0    39700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/contributions/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.522949 azure-devops-7.1.0b2/azure/devops/v7_0/core/
--rw-rw-rw-   0        0        0     1275 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/core/__init__.py
--rw-rw-rw-   0        0        0    26907 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/core/core_client.py
--rw-rw-rw-   0        0        0    39388 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/core/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.528452 azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/
--rw-rw-rw-   0        0        0      730 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/customer_intelligence_client.py
--rw-rw-rw-   0        0        0     1248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.534967 azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/
--rw-rw-rw-   0        0        0     1116 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/__init__.py
--rw-rw-rw-   0        0        0    27966 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/dashboard_client.py
--rw-rw-rw-   0        0        0    40578 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.542999 azure-devops-7.1.0b2/azure/devops/v7_0/elastic/
--rw-rw-rw-   0        0        0      942 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/elastic/__init__.py
--rw-rw-rw-   0        0        0     8717 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/elastic/elastic_client.py
--rw-rw-rw-   0        0        0    24056 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/elastic/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.549292 azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/
--rw-rw-rw-   0        0        0     1787 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/__init__.py
--rw-rw-rw-   0        0        0     8156 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/extension_management_client.py
--rw-rw-rw-   0        0        0    62184 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.555298 azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/
--rw-rw-rw-   0        0        0      737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/__init__.py
--rw-rw-rw-   0        0        0     7737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/feature_availability_client.py
--rw-rw-rw-   0        0        0     1956 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.562327 azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/
--rw-rw-rw-   0        0        0      951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/__init__.py
--rw-rw-rw-   0        0        0    13334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/feature_management_client.py
--rw-rw-rw-   0        0        0    10629 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.570428 azure-devops-7.1.0b2/azure/devops/v7_0/feed/
--rw-rw-rw-   0        0        0     1434 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feed/__init__.py
--rw-rw-rw-   0        0        0    53534 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feed/feed_client.py
--rw-rw-rw-   0        0        0    59930 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/feed/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.575353 azure-devops-7.1.0b2/azure/devops/v7_0/file_container/
--rw-rw-rw-   0        0        0      756 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/file_container/__init__.py
--rw-rw-rw-   0        0        0     7450 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/file_container/file_container_client.py
--rw-rw-rw-   0        0        0     9042 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/file_container/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.582876 azure-devops-7.1.0b2/azure/devops/v7_0/gallery/
--rw-rw-rw-   0        0        0     2229 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/gallery/__init__.py
--rw-rw-rw-   0        0        0   104617 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/gallery/gallery_client.py
--rw-rw-rw-   0        0        0    87099 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/gallery/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.593934 azure-devops-7.1.0b2/azure/devops/v7_0/git/
--rw-rw-rw-   0        0        0     3448 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/git/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-04-25 18:35:48.000000 azure-devops-7.1.0b2/azure/devops/v7_0/git/git_client.py
--rw-rw-rw-   0        0        0   207980 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/git/git_client_base.py
--rw-rw-rw-   0        0        0   170050 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/git/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.600958 azure-devops-7.1.0b2/azure/devops/v7_0/graph/
--rw-rw-rw-   0        0        0     1310 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/graph/__init__.py
--rw-rw-rw-   0        0        0    26571 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/graph/graph_client.py
--rw-rw-rw-   0        0        0    41503 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/graph/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.608971 azure-devops-7.1.0b2/azure/devops/v7_0/identity/
--rw-rw-rw-   0        0        0     1165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/identity/__init__.py
--rw-rw-rw-   0        0        0    29928 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/identity/identity_client.py
--rw-rw-rw-   0        0        0    28794 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/identity/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.616988 azure-devops-7.1.0b2/azure/devops/v7_0/location/
--rw-rw-rw-   0        0        0      838 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/location/__init__.py
--rw-rw-rw-   0        0        0     9773 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/location/location_client.py
--rw-rw-rw-   0        0        0    21179 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/location/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.624218 azure-devops-7.1.0b2/azure/devops/v7_0/maven/
--rw-rw-rw-   0        0        0     1486 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/maven/__init__.py
--rw-rw-rw-   0        0        0    17516 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/maven/maven_client.py
--rw-rw-rw-   0        0        0    31584 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/maven/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.630427 azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/
--rw-rw-rw-   0        0        0     1694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/__init__.py
--rw-rw-rw-   0        0        0    18742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/member_entitlement_management_client.py
--rw-rw-rw-   0        0        0    61490 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.637066 azure-devops-7.1.0b2/azure/devops/v7_0/notification/
--rw-rw-rw-   0        0        0     2612 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/notification/__init__.py
--rw-rw-rw-   0        0        0    77218 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/notification/models.py
--rw-rw-rw-   0        0        0    16920 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/notification/notification_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.644090 azure-devops-7.1.0b2/azure/devops/v7_0/npm/
--rw-rw-rw-   0        0        0      982 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/npm/__init__.py
--rw-rw-rw-   0        0        0    10809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/npm/models.py
--rw-rw-rw-   0        0        0    33781 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/npm/npm_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.650317 azure-devops-7.1.0b2/azure/devops/v7_0/nuget/
--rw-rw-rw-   0        0        0      989 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/nuget/__init__.py
--rw-rw-rw-   0        0        0    10432 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/nuget/models.py
--rw-rw-rw-   0        0        0    16619 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/nuget/nuget_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.656115 azure-devops-7.1.0b2/azure/devops/v7_0/operations/
--rw-rw-rw-   0        0        0      763 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/operations/__init__.py
--rw-rw-rw-   0        0        0     4257 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/operations/models.py
--rw-rw-rw-   0        0        0     2208 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/operations/operations_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.662142 azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/
--rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/__init__.py
--rw-rw-rw-   0        0        0     9418 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/models.py
--rw-rw-rw-   0        0        0     5073 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/pipeline_permissions_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.667143 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/
--rw-rw-rw-   0        0        0     1299 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/__init__.py
--rw-rw-rw-   0        0        0    19588 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/models.py
--rw-rw-rw-   0        0        0    14169 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/pipelines_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.673256 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/
--rw-rw-rw-   0        0        0     1048 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/__init__.py
--rw-rw-rw-   0        0        0    21350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/models.py
--rw-rw-rw-   0        0        0    10429 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/pipelines_checks_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.679271 azure-devops-7.1.0b2/azure/devops/v7_0/policy/
--rw-rw-rw-   0        0        0      884 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/policy/__init__.py
--rw-rw-rw-   0        0        0    15233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/policy/models.py
--rw-rw-rw-   0        0        0    15620 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/policy/policy_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.685280 azure-devops-7.1.0b2/azure/devops/v7_0/profile/
--rw-rw-rw-   0        0        0      908 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile/__init__.py
--rw-rw-rw-   0        0        0    10417 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile/models.py
--rw-rw-rw-   0        0        0     3489 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile/profile_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.690815 azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/
--rw-rw-rw-   0        0        0      739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/__init__.py
--rw-rw-rw-   0        0        0     2886 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/models.py
--rw-rw-rw-   0        0        0     2374 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/profile_regions_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.698321 azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/
--rw-rw-rw-   0        0        0      901 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/__init__.py
--rw-rw-rw-   0        0        0     9580 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/models.py
--rw-rw-rw-   0        0        0     6327 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/project_analysis_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.703845 azure-devops-7.1.0b2/azure/devops/v7_0/provenance/
--rw-rw-rw-   0        0        0      711 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/provenance/__init__.py
--rw-rw-rw-   0        0        0     1967 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/provenance/models.py
--rw-rw-rw-   0        0        0     2501 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/provenance/provenance_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.708878 azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/
--rw-rw-rw-   0        0        0      973 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/__init__.py
--rw-rw-rw-   0        0        0     9738 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/models.py
--rw-rw-rw-   0        0        0    16679 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/py_pi_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.715903 azure-devops-7.1.0b2/azure/devops/v7_0/release/
--rw-rw-rw-   0        0        0     3473 2023-04-14 18:26:51.000000 azure-devops-7.1.0b2/azure/devops/v7_0/release/__init__.py
--rw-rw-rw-   0        0        0   179618 2023-04-14 18:26:51.000000 azure-devops-7.1.0b2/azure/devops/v7_0/release/models.py
--rw-rw-rw-   0        0        0    54717 2023-04-14 18:26:51.000000 azure-devops-7.1.0b2/azure/devops/v7_0/release/release_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.723936 azure-devops-7.1.0b2/azure/devops/v7_0/sbom/
--rw-rw-rw-   0        0        0      820 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/sbom/__init__.py
--rw-rw-rw-   0        0        0    16520 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/sbom/models.py
--rw-rw-rw-   0        0        0     1177 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/sbom/sbom_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.729035 azure-devops-7.1.0b2/azure/devops/v7_0/search/
--rw-rw-rw-   0        0        0     1660 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/search/__init__.py
--rw-rw-rw-   0        0        0    51412 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/search/models.py
--rw-rw-rw-   0        0        0     7951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/search/search_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.735043 azure-devops-7.1.0b2/azure/devops/v7_0/security/
--rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/security/__init__.py
--rw-rw-rw-   0        0        0    13405 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/security/models.py
--rw-rw-rw-   0        0        0    14124 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/security/security_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.744100 azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/
--rw-rw-rw-   0        0        0     1890 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/__init__.py
--rw-rw-rw-   0        0        0    66419 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/models.py
--rw-rw-rw-   0        0        0    17345 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/service_endpoint_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.751141 azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/
--rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/__init__.py
--rw-rw-rw-   0        0        0    64152 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/models.py
--rw-rw-rw-   0        0        0    21308 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/service_hooks_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.756141 azure-devops-7.1.0b2/azure/devops/v7_0/settings/
--rw-rw-rw-   0        0        0      638 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/settings/__init__.py
--rw-rw-rw-   0        0        0     7639 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/settings/settings_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.764172 azure-devops-7.1.0b2/azure/devops/v7_0/symbol/
--rw-rw-rw-   0        0        0      840 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/symbol/__init__.py
--rw-rw-rw-   0        0        0    12241 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/symbol/models.py
--rw-rw-rw-   0        0        0    13260 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/symbol/symbol_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.772231 azure-devops-7.1.0b2/azure/devops/v7_0/task/
--rw-rw-rw-   0        0        0     1368 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task/__init__.py
--rw-rw-rw-   0        0        0    34317 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task/models.py
--rw-rw-rw-   0        0        0    27853 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task/task_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.781308 azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/
--rw-rw-rw-   0        0        0     4200 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/__init__.py
--rw-rw-rw-   0        0        0   192204 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/models.py
--rw-rw-rw-   0        0        0    68198 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/task_agent_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.788419 azure-devops-7.1.0b2/azure/devops/v7_0/test/
--rw-rw-rw-   0        0        0     3616 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test/__init__.py
--rw-rw-rw-   0        0        0   206239 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test/models.py
--rw-rw-rw-   0        0        0    68796 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test/test_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.793939 azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/
--rw-rw-rw-   0        0        0     2477 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/__init__.py
--rw-rw-rw-   0        0        0   106651 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/models.py
--rw-rw-rw-   0        0        0    55123 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/test_plan_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.802978 azure-devops-7.1.0b2/azure/devops/v7_0/test_results/
--rw-rw-rw-   0        0        0     3269 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_results/__init__.py
--rw-rw-rw-   0        0        0   161630 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_results/models.py
--rw-rw-rw-   0        0        0    21339 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/test_results/test_results_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.810001 azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/
--rw-rw-rw-   0        0        0     1587 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/__init__.py
--rw-rw-rw-   0        0        0    56530 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/models.py
--rw-rw-rw-   0        0        0    46539 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/tfvc_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.817010 azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/
--rw-rw-rw-   0        0        0      809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/__init__.py
--rw-rw-rw-   0        0        0     7313 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/models.py
--rw-rw-rw-   0        0        0     5176 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/token_admin_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.823043 azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/
--rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/__init__.py
--rw-rw-rw-   0        0        0     7392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/models.py
--rw-rw-rw-   0        0        0    12373 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/upack_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.830065 azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/
--rw-rw-rw-   0        0        0      861 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/__init__.py
--rw-rw-rw-   0        0        0     4626 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/models.py
--rw-rw-rw-   0        0        0     5165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/upack_packaging_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.835065 azure-devops-7.1.0b2/azure/devops/v7_0/wiki/
--rw-rw-rw-   0        0        0     1460 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/wiki/__init__.py
--rw-rw-rw-   0        0        0    40959 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/wiki/models.py
--rw-rw-rw-   0        0        0    37957 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/wiki/wiki_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.841289 azure-devops-7.1.0b2/azure/devops/v7_0/work/
--rw-rw-rw-   0        0        0     2622 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work/__init__.py
--rw-rw-rw-   0        0        0    87293 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work/models.py
--rw-rw-rw-   0        0        0    77467 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work/work_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.847288 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/
--rw-rw-rw-   0        0        0     3148 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/__init__.py
--rw-rw-rw-   0        0        0   117974 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/models.py
--rw-rw-rw-   0        0        0   114702 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/work_item_tracking_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.853313 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/
--rw-rw-rw-   0        0        0     1817 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/__init__.py
--rw-rw-rw-   0        0        0    57182 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/models.py
--rw-rw-rw-   0        0        0    68317 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/work_item_tracking_process_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.861349 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/
--rw-rw-rw-   0        0        0      894 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/__init__.py
--rw-rw-rw-   0        0        0     8972 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/models.py
--rw-rw-rw-   0        0        0     6446 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/work_item_tracking_process_template_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.865347 azure-devops-7.1.0b2/azure/devops/v7_1/
--rw-rw-rw-   0        0        0      557 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.871862 azure-devops-7.1.0b2/azure/devops/v7_1/accounts/
--rw-rw-rw-   0        0        0      742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/accounts/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/accounts/accounts_client.py
--rw-rw-rw-   0        0        0     6285 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/accounts/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.876860 azure-devops-7.1.0b2/azure/devops/v7_1/audit/
--rw-rw-rw-   0        0        0      771 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/audit/__init__.py
--rw-rw-rw-   0        0        0     9739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/audit/audit_client.py
--rw-rw-rw-   0        0        0    13645 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/audit/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.883896 azure-devops-7.1.0b2/azure/devops/v7_1/build/
--rw-rw-rw-   0        0        0     3114 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/build/__init__.py
--rw-rw-rw-   0        0        0   132013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/build/build_client.py
--rw-rw-rw-   0        0        0   151261 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/build/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.889033 azure-devops-7.1.0b2/azure/devops/v7_1/cix/
--rw-rw-rw-   0        0        0     1013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/cix/__init__.py
--rw-rw-rw-   0        0        0     7713 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/cix/cix_client.py
--rw-rw-rw-   0        0        0    16667 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/cix/models.py
--rw-rw-rw-   0        0        0    21269 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.894048 azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/
--rw-rw-rw-   0        0        0      694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/client_trace_client.py
--rw-rw-rw-   0        0        0     1978 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.898047 azure-devops-7.1.0b2/azure/devops/v7_1/contributions/
--rw-rw-rw-   0        0        0     1406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/contributions/__init__.py
--rw-rw-rw-   0        0        0     5750 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/contributions/contributions_client.py
--rw-rw-rw-   0        0        0    39700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/contributions/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.903166 azure-devops-7.1.0b2/azure/devops/v7_1/core/
--rw-rw-rw-   0        0        0     1275 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/core/__init__.py
--rw-rw-rw-   0        0        0    27326 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/core/core_client.py
--rw-rw-rw-   0        0        0    39744 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/core/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.910270 azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/
--rw-rw-rw-   0        0        0      730 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/customer_intelligence_client.py
--rw-rw-rw-   0        0        0     1248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.915270 azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/
--rw-rw-rw-   0        0        0     1116 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/__init__.py
--rw-rw-rw-   0        0        0    27966 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/dashboard_client.py
--rw-rw-rw-   0        0        0    43220 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.919885 azure-devops-7.1.0b2/azure/devops/v7_1/elastic/
--rw-rw-rw-   0        0        0      942 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/elastic/__init__.py
--rw-rw-rw-   0        0        0     8885 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/elastic/elastic_client.py
--rw-rw-rw-   0        0        0    24700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/elastic/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.924889 azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/
--rw-rw-rw-   0        0        0     1787 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/__init__.py
--rw-rw-rw-   0        0        0     8156 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/extension_management_client.py
--rw-rw-rw-   0        0        0    62180 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.930936 azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/
--rw-rw-rw-   0        0        0      737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/__init__.py
--rw-rw-rw-   0        0        0     7737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/feature_availability_client.py
--rw-rw-rw-   0        0        0     1956 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.935935 azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/
--rw-rw-rw-   0        0        0      951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/__init__.py
--rw-rw-rw-   0        0        0    13334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/feature_management_client.py
--rw-rw-rw-   0        0        0    10629 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.941954 azure-devops-7.1.0b2/azure/devops/v7_1/feed/
--rw-rw-rw-   0        0        0     1455 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feed/__init__.py
--rw-rw-rw-   0        0        0    54406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feed/feed_client.py
--rw-rw-rw-   0        0        0    60661 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/feed/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.946955 azure-devops-7.1.0b2/azure/devops/v7_1/file_container/
--rw-rw-rw-   0        0        0      756 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/file_container/__init__.py
--rw-rw-rw-   0        0        0     7447 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/file_container/file_container_client.py
--rw-rw-rw-   0        0        0     9042 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/file_container/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.952300 azure-devops-7.1.0b2/azure/devops/v7_1/gallery/
--rw-rw-rw-   0        0        0     2229 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/gallery/__init__.py
--rw-rw-rw-   0        0        0   105334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/gallery/gallery_client.py
--rw-rw-rw-   0        0        0    87095 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/gallery/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.960918 azure-devops-7.1.0b2/azure/devops/v7_1/git/
--rw-rw-rw-   0        0        0     3564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/git/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-04-25 18:36:39.000000 azure-devops-7.1.0b2/azure/devops/v7_1/git/git_client.py
--rw-rw-rw-   0        0        0   212306 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/git/git_client_base.py
--rw-rw-rw-   0        0        0   176274 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/git/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.966916 azure-devops-7.1.0b2/azure/devops/v7_1/graph/
--rw-rw-rw-   0        0        0     1640 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/graph/__init__.py
--rw-rw-rw-   0        0        0    31411 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/graph/graph_client.py
--rw-rw-rw-   0        0        0    57092 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/graph/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.972957 azure-devops-7.1.0b2/azure/devops/v7_1/identity/
--rw-rw-rw-   0        0        0     1165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/identity/__init__.py
--rw-rw-rw-   0        0        0    30320 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/identity/identity_client.py
--rw-rw-rw-   0        0        0    28794 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/identity/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.979977 azure-devops-7.1.0b2/azure/devops/v7_1/location/
--rw-rw-rw-   0        0        0      838 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/location/__init__.py
--rw-rw-rw-   0        0        0     9773 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/location/location_client.py
--rw-rw-rw-   0        0        0    21179 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/location/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.988022 azure-devops-7.1.0b2/azure/devops/v7_1/maven/
--rw-rw-rw-   0        0        0     1486 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/maven/__init__.py
--rw-rw-rw-   0        0        0    17516 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/maven/maven_client.py
--rw-rw-rw-   0        0        0    31584 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/maven/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:57.994546 azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/
--rw-rw-rw-   0        0        0     2315 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/__init__.py
--rw-rw-rw-   0        0        0    25642 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/member_entitlement_management_client.py
--rw-rw-rw-   0        0        0    89340 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/models.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.003589 azure-devops-7.1.0b2/azure/devops/v7_1/notification/
--rw-rw-rw-   0        0        0     2612 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/notification/__init__.py
--rw-rw-rw-   0        0        0    77210 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/notification/models.py
--rw-rw-rw-   0        0        0    17344 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/notification/notification_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.010585 azure-devops-7.1.0b2/azure/devops/v7_1/npm/
--rw-rw-rw-   0        0        0      982 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/npm/__init__.py
--rw-rw-rw-   0        0        0    10809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/npm/models.py
--rw-rw-rw-   0        0        0    34333 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/npm/npm_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.018129 azure-devops-7.1.0b2/azure/devops/v7_1/nuget/
--rw-rw-rw-   0        0        0      989 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/nuget/__init__.py
--rw-rw-rw-   0        0        0    10713 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/nuget/models.py
--rw-rw-rw-   0        0        0    16739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/nuget/nuget_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.025189 azure-devops-7.1.0b2/azure/devops/v7_1/operations/
--rw-rw-rw-   0        0        0      763 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/operations/__init__.py
--rw-rw-rw-   0        0        0     4257 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/operations/models.py
--rw-rw-rw-   0        0        0     2228 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/operations/operations_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.033334 azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/
--rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/__init__.py
--rw-rw-rw-   0        0        0     9418 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/models.py
--rw-rw-rw-   0        0        0     5073 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/pipeline_permissions_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.041860 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/
--rw-rw-rw-   0        0        0     1365 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/__init__.py
--rw-rw-rw-   0        0        0    22233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/models.py
--rw-rw-rw-   0        0        0    14409 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/pipelines_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.050912 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/
--rw-rw-rw-   0        0        0     1066 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/__init__.py
--rw-rw-rw-   0        0        0    22399 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/models.py
--rw-rw-rw-   0        0        0    10429 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/pipelines_checks_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.059939 azure-devops-7.1.0b2/azure/devops/v7_1/policy/
--rw-rw-rw-   0        0        0      884 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/policy/__init__.py
--rw-rw-rw-   0        0        0    15233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/policy/models.py
--rw-rw-rw-   0        0        0    15624 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/policy/policy_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.070035 azure-devops-7.1.0b2/azure/devops/v7_1/profile/
--rw-rw-rw-   0        0        0      908 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile/__init__.py
--rw-rw-rw-   0        0        0    10417 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile/models.py
--rw-rw-rw-   0        0        0     3513 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile/profile_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.078035 azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/
--rw-rw-rw-   0        0        0      739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/__init__.py
--rw-rw-rw-   0        0        0     2886 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/models.py
--rw-rw-rw-   0        0        0     2374 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/profile_regions_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.085453 azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/
--rw-rw-rw-   0        0        0      901 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/__init__.py
--rw-rw-rw-   0        0        0     9580 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/models.py
--rw-rw-rw-   0        0        0     6447 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/project_analysis_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.092004 azure-devops-7.1.0b2/azure/devops/v7_1/provenance/
--rw-rw-rw-   0        0        0      711 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/provenance/__init__.py
--rw-rw-rw-   0        0        0     1967 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/provenance/models.py
--rw-rw-rw-   0        0        0     2501 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/provenance/provenance_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.100192 azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/
--rw-rw-rw-   0        0        0      973 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/__init__.py
--rw-rw-rw-   0        0        0     9738 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/models.py
--rw-rw-rw-   0        0        0    16679 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/py_pi_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.106852 azure-devops-7.1.0b2/azure/devops/v7_1/release/
--rw-rw-rw-   0        0        0     3473 2023-04-08 11:33:32.000000 azure-devops-7.1.0b2/azure/devops/v7_1/release/__init__.py
--rw-rw-rw-   0        0        0   179609 2023-04-08 11:33:32.000000 azure-devops-7.1.0b2/azure/devops/v7_1/release/models.py
--rw-rw-rw-   0        0        0    55421 2023-04-08 11:33:32.000000 azure-devops-7.1.0b2/azure/devops/v7_1/release/release_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.114894 azure-devops-7.1.0b2/azure/devops/v7_1/sbom/
--rw-rw-rw-   0        0        0      820 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/sbom/__init__.py
--rw-rw-rw-   0        0        0    16729 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/sbom/models.py
--rw-rw-rw-   0        0        0     1177 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/sbom/sbom_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.123054 azure-devops-7.1.0b2/azure/devops/v7_1/search/
--rw-rw-rw-   0        0        0     1660 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/search/__init__.py
--rw-rw-rw-   0        0        0    51412 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/search/models.py
--rw-rw-rw-   0        0        0     8119 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/search/search_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.131085 azure-devops-7.1.0b2/azure/devops/v7_1/security/
--rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/security/__init__.py
--rw-rw-rw-   0        0        0    13405 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/security/models.py
--rw-rw-rw-   0        0        0    14340 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/security/security_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.141118 azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/
--rw-rw-rw-   0        0        0     1835 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/__init__.py
--rw-rw-rw-   0        0        0    65327 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/models.py
--rw-rw-rw-   0        0        0    17633 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/service_endpoint_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.150147 azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/
--rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/__init__.py
--rw-rw-rw-   0        0        0    64147 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/models.py
--rw-rw-rw-   0        0        0    21860 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/service_hooks_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.155147 azure-devops-7.1.0b2/azure/devops/v7_1/settings/
--rw-rw-rw-   0        0        0      638 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/settings/__init__.py
--rw-rw-rw-   0        0        0     7639 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/settings/settings_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.163177 azure-devops-7.1.0b2/azure/devops/v7_1/symbol/
--rw-rw-rw-   0        0        0      840 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/symbol/__init__.py
--rw-rw-rw-   0        0        0    12241 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/symbol/models.py
--rw-rw-rw-   0        0        0    13596 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/symbol/symbol_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.170128 azure-devops-7.1.0b2/azure/devops/v7_1/task/
--rw-rw-rw-   0        0        0     1408 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task/__init__.py
--rw-rw-rw-   0        0        0    38822 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task/models.py
--rw-rw-rw-   0        0        0    30129 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task/task_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.176129 azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/
--rw-rw-rw-   0        0        0     4145 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/__init__.py
--rw-rw-rw-   0        0        0   192209 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/models.py
--rw-rw-rw-   0        0        0    69590 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/task_agent_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.184309 azure-devops-7.1.0b2/azure/devops/v7_1/test/
--rw-rw-rw-   0        0        0     3616 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test/__init__.py
--rw-rw-rw-   0        0        0   206235 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test/models.py
--rw-rw-rw-   0        0        0    69828 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test/test_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.190856 azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/
--rw-rw-rw-   0        0        0     2477 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/__init__.py
--rw-rw-rw-   0        0        0   106651 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/models.py
--rw-rw-rw-   0        0        0    56067 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/test_plan_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.198890 azure-devops-7.1.0b2/azure/devops/v7_1/test_results/
--rw-rw-rw-   0        0        0     3361 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_results/__init__.py
--rw-rw-rw-   0        0        0   164018 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_results/models.py
--rw-rw-rw-   0        0        0    31216 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/test_results/test_results_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.206900 azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/
--rw-rw-rw-   0        0        0     1587 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/__init__.py
--rw-rw-rw-   0        0        0    56986 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/models.py
--rw-rw-rw-   0        0        0    47091 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/tfvc_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.212926 azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/
--rw-rw-rw-   0        0        0      809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/__init__.py
--rw-rw-rw-   0        0        0     7313 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/models.py
--rw-rw-rw-   0        0        0     5248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/token_admin_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.219945 azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/
--rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/__init__.py
--rw-rw-rw-   0        0        0     7392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/models.py
--rw-rw-rw-   0        0        0    12373 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/upack_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.226955 azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/
--rw-rw-rw-   0        0        0      861 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/__init__.py
--rw-rw-rw-   0        0        0     4626 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/models.py
--rw-rw-rw-   0        0        0     5165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/upack_packaging_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.234990 azure-devops-7.1.0b2/azure/devops/v7_1/wiki/
--rw-rw-rw-   0        0        0     1460 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/wiki/__init__.py
--rw-rw-rw-   0        0        0    41392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/wiki/models.py
--rw-rw-rw-   0        0        0    38413 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/wiki/wiki_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.242026 azure-devops-7.1.0b2/azure/devops/v7_1/work/
--rw-rw-rw-   0        0        0     2622 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work/__init__.py
--rw-rw-rw-   0        0        0    87669 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work/models.py
--rw-rw-rw-   0        0        0    78795 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work/work_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.251055 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/
--rw-rw-rw-   0        0        0     3456 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/__init__.py
--rw-rw-rw-   0        0        0   129996 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/models.py
--rw-rw-rw-   0        0        0   125171 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/work_item_tracking_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.260077 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/
--rw-rw-rw-   0        0        0     1817 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/__init__.py
--rw-rw-rw-   0        0        0    57547 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/models.py
--rw-rw-rw-   0        0        0    69684 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/work_item_tracking_process_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.267084 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/
--rw-rw-rw-   0        0        0      894 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/__init__.py
--rw-rw-rw-   0        0        0     8972 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/models.py
--rw-rw-rw-   0        0        0     6566 2023-04-18 19:56:16.000000 azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/work_item_tracking_process_template_client.py
--rw-rw-rw-   0        0        0      366 2023-04-25 18:23:57.000000 azure-devops-7.1.0b2/azure/devops/version.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:06:58.277118 azure-devops-7.1.0b2/azure_devops.egg-info/
--rw-rw-rw-   0        0        0      930 2023-04-25 19:06:57.000000 azure-devops-7.1.0b2/azure_devops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19370 2023-04-25 19:06:57.000000 azure-devops-7.1.0b2/azure_devops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 19:06:57.000000 azure-devops-7.1.0b2/azure_devops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-25 19:06:57.000000 azure-devops-7.1.0b2/azure_devops.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-25 19:06:57.000000 azure-devops-7.1.0b2/azure_devops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 19:06:58.280151 azure-devops-7.1.0b2/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-04-25 18:23:45.000000 azure-devops-7.1.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.763411 azure-devops-7.1.0b3/
+-rw-rw-rw-   0        0        0     1114 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/LICENSE.txt
+-rw-rw-rw-   0        0        0       21 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0      930 2023-04-26 17:35:57.762409 azure-devops-7.1.0b3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.691260 azure-devops-7.1.0b3/azure/
+-rw-rw-rw-   0        0        0      408 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.763743 azure-devops-7.1.0b3/azure/devops/
+-rw-rw-rw-   0        0        0      408 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/__init__.py
+-rw-rw-rw-   0        0        0     6471 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/_file_cache.py
+-rw-rw-rw-   0        0        0     6311 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/_models.py
+-rw-rw-rw-   0        0        0    16010 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/client.py
+-rw-rw-rw-   0        0        0      770 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/client_configuration.py
+-rw-rw-rw-   0        0        0     6471 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/connection.py
+-rw-rw-rw-   0        0        0      467 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/credentials.py
+-rw-rw-rw-   0        0        0     1550 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.785092 azure-devops-7.1.0b3/azure/devops/issue_tests/
+-rw-rw-rw-   0        0        0      557 2021-12-01 09:17:04.000000 azure-devops-7.1.0b3/azure/devops/issue_tests/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/issue_tests/test_issue_268.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.800967 azure-devops-7.1.0b3/azure/devops/released/
+-rw-rw-rw-   0        0        0      557 2023-04-17 18:43:56.000000 azure-devops-7.1.0b3/azure/devops/released/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.825477 azure-devops-7.1.0b3/azure/devops/released/accounts/
+-rw-rw-rw-   0        0        0      758 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/accounts/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/accounts/accounts_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.855140 azure-devops-7.1.0b3/azure/devops/released/build/
+-rw-rw-rw-   0        0        0     3127 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/build/__init__.py
+-rw-rw-rw-   0        0        0   111801 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/build/build_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.879698 azure-devops-7.1.0b3/azure/devops/released/cix/
+-rw-rw-rw-   0        0        0     1024 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/cix/__init__.py
+-rw-rw-rw-   0        0        0     7619 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/cix/cix_client.py
+-rw-rw-rw-   0        0        0    21262 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.903424 azure-devops-7.1.0b3/azure/devops/released/core/
+-rw-rw-rw-   0        0        0     1287 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/core/__init__.py
+-rw-rw-rw-   0        0        0    16996 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/core/core_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.928612 azure-devops-7.1.0b3/azure/devops/released/elastic/
+-rw-rw-rw-   0        0        0      957 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/elastic/__init__.py
+-rw-rw-rw-   0        0        0     8731 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/elastic/elastic_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.954782 azure-devops-7.1.0b3/azure/devops/released/feed/
+-rw-rw-rw-   0        0        0     1446 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/feed/__init__.py
+-rw-rw-rw-   0        0        0    52098 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/feed/feed_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:52.997007 azure-devops-7.1.0b3/azure/devops/released/git/
+-rw-rw-rw-   0        0        0     3459 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/git/__init__.py
+-rw-rw-rw-   0        0        0     1653 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/released/git/git_client.py
+-rw-rw-rw-   0        0        0   207990 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/git/git_client_base.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.019750 azure-devops-7.1.0b3/azure/devops/released/graph/
+-rw-rw-rw-   0        0        0     1323 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/graph/__init__.py
+-rw-rw-rw-   0        0        0     5689 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/graph/graph_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.043989 azure-devops-7.1.0b3/azure/devops/released/identity/
+-rw-rw-rw-   0        0        0     1181 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/identity/__init__.py
+-rw-rw-rw-   0        0        0    14236 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/identity/identity_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.067069 azure-devops-7.1.0b3/azure/devops/released/member_entitlement_management/
+-rw-rw-rw-   0        0        0     1731 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/member_entitlement_management/__init__.py
+-rw-rw-rw-   0        0        0    18778 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/member_entitlement_management/member_entitlement_management_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.091743 azure-devops-7.1.0b3/azure/devops/released/notification/
+-rw-rw-rw-   0        0        0     2632 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/notification/__init__.py
+-rw-rw-rw-   0        0        0    16939 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/notification/notification_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.115931 azure-devops-7.1.0b3/azure/devops/released/npm/
+-rw-rw-rw-   0        0        0      993 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/npm/__init__.py
+-rw-rw-rw-   0        0        0    33791 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/npm/npm_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.140924 azure-devops-7.1.0b3/azure/devops/released/nuget/
+-rw-rw-rw-   0        0        0     1002 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/nuget/__init__.py
+-rw-rw-rw-   0        0        0     8101 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/nuget/nuget_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.163021 azure-devops-7.1.0b3/azure/devops/released/operations/
+-rw-rw-rw-   0        0        0      781 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/operations/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/operations/operations_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.186595 azure-devops-7.1.0b3/azure/devops/released/pipelines/
+-rw-rw-rw-   0        0        0     1316 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/pipelines/__init__.py
+-rw-rw-rw-   0        0        0    14185 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/pipelines/pipelines_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.210653 azure-devops-7.1.0b3/azure/devops/released/policy/
+-rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/policy/__init__.py
+-rw-rw-rw-   0        0        0    11569 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/policy/policy_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.233250 azure-devops-7.1.0b3/azure/devops/released/profile/
+-rw-rw-rw-   0        0        0      923 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/profile/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/profile/profile_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.257276 azure-devops-7.1.0b3/azure/devops/released/project_analysis/
+-rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/project_analysis/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/project_analysis/project_analysis_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.289624 azure-devops-7.1.0b3/azure/devops/released/release/
+-rw-rw-rw-   0        0        0     3488 2023-04-17 18:43:56.000000 azure-devops-7.1.0b3/azure/devops/released/release/__init__.py
+-rw-rw-rw-   0        0        0    54731 2023-04-17 18:43:56.000000 azure-devops-7.1.0b3/azure/devops/released/release/release_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.313753 azure-devops-7.1.0b3/azure/devops/released/search/
+-rw-rw-rw-   0        0        0     1674 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/search/__init__.py
+-rw-rw-rw-   0        0        0     7964 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/search/search_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.337696 azure-devops-7.1.0b3/azure/devops/released/security/
+-rw-rw-rw-   0        0        0      914 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/security/__init__.py
+-rw-rw-rw-   0        0        0    14139 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/security/security_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.363547 azure-devops-7.1.0b3/azure/devops/released/service_endpoint/
+-rw-rw-rw-   0        0        0     1914 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/service_endpoint/__init__.py
+-rw-rw-rw-   0        0        0    17368 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/service_endpoint/service_endpoint_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.388170 azure-devops-7.1.0b3/azure/devops/released/service_hooks/
+-rw-rw-rw-   0        0        0     1585 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/service_hooks/__init__.py
+-rw-rw-rw-   0        0        0    21328 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/service_hooks/service_hooks_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.411339 azure-devops-7.1.0b3/azure/devops/released/symbol/
+-rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/symbol/__init__.py
+-rw-rw-rw-   0        0        0    13273 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/symbol/symbol_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.437127 azure-devops-7.1.0b3/azure/devops/released/task/
+-rw-rw-rw-   0        0        0     1380 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/task/__init__.py
+-rw-rw-rw-   0        0        0    27864 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/task/task_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.463292 azure-devops-7.1.0b3/azure/devops/released/task_agent/
+-rw-rw-rw-   0        0        0     4218 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/task_agent/__init__.py
+-rw-rw-rw-   0        0        0    67774 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/task_agent/task_agent_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.491378 azure-devops-7.1.0b3/azure/devops/released/test/
+-rw-rw-rw-   0        0        0     3628 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test/__init__.py
+-rw-rw-rw-   0        0        0    68807 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test/test_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.517916 azure-devops-7.1.0b3/azure/devops/released/test_plan/
+-rw-rw-rw-   0        0        0     2494 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test_plan/__init__.py
+-rw-rw-rw-   0        0        0    55139 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test_plan/test_plan_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.541034 azure-devops-7.1.0b3/azure/devops/released/test_results/
+-rw-rw-rw-   0        0        0     3289 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test_results/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/test_results/test_results_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.567197 azure-devops-7.1.0b3/azure/devops/released/tfvc/
+-rw-rw-rw-   0        0        0     1599 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/tfvc/__init__.py
+-rw-rw-rw-   0        0        0    46550 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/tfvc/tfvc_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.591250 azure-devops-7.1.0b3/azure/devops/released/token_admin/
+-rw-rw-rw-   0        0        0      828 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/token_admin/__init__.py
+-rw-rw-rw-   0        0        0     5194 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/token_admin/token_admin_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.615814 azure-devops-7.1.0b3/azure/devops/released/wiki/
+-rw-rw-rw-   0        0        0     1472 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/wiki/__init__.py
+-rw-rw-rw-   0        0        0    37968 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/wiki/wiki_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.642552 azure-devops-7.1.0b3/azure/devops/released/work/
+-rw-rw-rw-   0        0        0     2634 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work/__init__.py
+-rw-rw-rw-   0        0        0    77478 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work/work_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.669861 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking/
+-rw-rw-rw-   0        0        0     3174 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking/__init__.py
+-rw-rw-rw-   0        0        0    97796 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking/work_item_tracking_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.696539 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process/
+-rw-rw-rw-   0        0        0     1851 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process/__init__.py
+-rw-rw-rw-   0        0        0    68350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process/work_item_tracking_process_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.718783 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process_template/
+-rw-rw-rw-   0        0        0      937 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process_template/__init__.py
+-rw-rw-rw-   0        0        0     6488 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process_template/work_item_tracking_process_template_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.734836 azure-devops-7.1.0b3/azure/devops/v7_0/
+-rw-rw-rw-   0        0        0      557 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.767110 azure-devops-7.1.0b3/azure/devops/v7_0/accounts/
+-rw-rw-rw-   0        0        0      742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/accounts/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/accounts/accounts_client.py
+-rw-rw-rw-   0        0        0     6285 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/accounts/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.799982 azure-devops-7.1.0b3/azure/devops/v7_0/audit/
+-rw-rw-rw-   0        0        0      771 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/audit/__init__.py
+-rw-rw-rw-   0        0        0     9739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/audit/audit_client.py
+-rw-rw-rw-   0        0        0    13099 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/audit/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.844644 azure-devops-7.1.0b3/azure/devops/v7_0/build/
+-rw-rw-rw-   0        0        0     3114 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/build/__init__.py
+-rw-rw-rw-   0        0        0   130017 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/build/build_client.py
+-rw-rw-rw-   0        0        0   150112 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/build/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.879792 azure-devops-7.1.0b3/azure/devops/v7_0/cix/
+-rw-rw-rw-   0        0        0     1013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/cix/__init__.py
+-rw-rw-rw-   0        0        0     7609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/cix/cix_client.py
+-rw-rw-rw-   0        0        0    16667 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/cix/models.py
+-rw-rw-rw-   0        0        0    21261 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.910580 azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/
+-rw-rw-rw-   0        0        0      694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/client_trace_client.py
+-rw-rw-rw-   0        0        0     1978 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.942992 azure-devops-7.1.0b3/azure/devops/v7_0/contributions/
+-rw-rw-rw-   0        0        0     1406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/contributions/__init__.py
+-rw-rw-rw-   0        0        0     5750 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/contributions/contributions_client.py
+-rw-rw-rw-   0        0        0    39700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/contributions/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:53.978590 azure-devops-7.1.0b3/azure/devops/v7_0/core/
+-rw-rw-rw-   0        0        0     1275 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/core/__init__.py
+-rw-rw-rw-   0        0        0    26907 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/core/core_client.py
+-rw-rw-rw-   0        0        0    39388 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/core/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.010185 azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/
+-rw-rw-rw-   0        0        0      730 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/customer_intelligence_client.py
+-rw-rw-rw-   0        0        0     1248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.043949 azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/
+-rw-rw-rw-   0        0        0     1116 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/__init__.py
+-rw-rw-rw-   0        0        0    27966 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/dashboard_client.py
+-rw-rw-rw-   0        0        0    40578 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.080433 azure-devops-7.1.0b3/azure/devops/v7_0/elastic/
+-rw-rw-rw-   0        0        0      942 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/elastic/__init__.py
+-rw-rw-rw-   0        0        0     8717 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/elastic/elastic_client.py
+-rw-rw-rw-   0        0        0    24056 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/elastic/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.116746 azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/
+-rw-rw-rw-   0        0        0     1787 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/__init__.py
+-rw-rw-rw-   0        0        0     8156 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/extension_management_client.py
+-rw-rw-rw-   0        0        0    62184 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.149785 azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/
+-rw-rw-rw-   0        0        0      737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/__init__.py
+-rw-rw-rw-   0        0        0     7737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/feature_availability_client.py
+-rw-rw-rw-   0        0        0     1956 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.184691 azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/
+-rw-rw-rw-   0        0        0      951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/__init__.py
+-rw-rw-rw-   0        0        0    13334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/feature_management_client.py
+-rw-rw-rw-   0        0        0    10629 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.223186 azure-devops-7.1.0b3/azure/devops/v7_0/feed/
+-rw-rw-rw-   0        0        0     1434 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feed/__init__.py
+-rw-rw-rw-   0        0        0    53534 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feed/feed_client.py
+-rw-rw-rw-   0        0        0    59930 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/feed/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.263176 azure-devops-7.1.0b3/azure/devops/v7_0/file_container/
+-rw-rw-rw-   0        0        0      756 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/file_container/__init__.py
+-rw-rw-rw-   0        0        0     7450 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/file_container/file_container_client.py
+-rw-rw-rw-   0        0        0     9042 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/file_container/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.311707 azure-devops-7.1.0b3/azure/devops/v7_0/gallery/
+-rw-rw-rw-   0        0        0     2229 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/gallery/__init__.py
+-rw-rw-rw-   0        0        0   104617 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/gallery/gallery_client.py
+-rw-rw-rw-   0        0        0    87099 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/gallery/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.369467 azure-devops-7.1.0b3/azure/devops/v7_0/git/
+-rw-rw-rw-   0        0        0     3448 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/git/__init__.py
+-rw-rw-rw-   0        0        0     1653 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_0/git/git_client.py
+-rw-rw-rw-   0        0        0   207980 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/git/git_client_base.py
+-rw-rw-rw-   0        0        0   169765 2023-04-26 17:21:57.000000 azure-devops-7.1.0b3/azure/devops/v7_0/git/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.409894 azure-devops-7.1.0b3/azure/devops/v7_0/graph/
+-rw-rw-rw-   0        0        0     1310 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/graph/__init__.py
+-rw-rw-rw-   0        0        0    26571 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/graph/graph_client.py
+-rw-rw-rw-   0        0        0    41503 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/graph/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.448020 azure-devops-7.1.0b3/azure/devops/v7_0/identity/
+-rw-rw-rw-   0        0        0     1165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/identity/__init__.py
+-rw-rw-rw-   0        0        0    29928 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/identity/identity_client.py
+-rw-rw-rw-   0        0        0    28794 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/identity/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.485437 azure-devops-7.1.0b3/azure/devops/v7_0/location/
+-rw-rw-rw-   0        0        0      838 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/location/__init__.py
+-rw-rw-rw-   0        0        0     9773 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/location/location_client.py
+-rw-rw-rw-   0        0        0    21179 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/location/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.524639 azure-devops-7.1.0b3/azure/devops/v7_0/maven/
+-rw-rw-rw-   0        0        0     1486 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/maven/__init__.py
+-rw-rw-rw-   0        0        0    17516 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/maven/maven_client.py
+-rw-rw-rw-   0        0        0    31584 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/maven/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.563658 azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/
+-rw-rw-rw-   0        0        0     1694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/__init__.py
+-rw-rw-rw-   0        0        0    18742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/member_entitlement_management_client.py
+-rw-rw-rw-   0        0        0    61490 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.604896 azure-devops-7.1.0b3/azure/devops/v7_0/notification/
+-rw-rw-rw-   0        0        0     2612 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/notification/__init__.py
+-rw-rw-rw-   0        0        0    77218 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/notification/models.py
+-rw-rw-rw-   0        0        0    16920 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/notification/notification_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.642024 azure-devops-7.1.0b3/azure/devops/v7_0/npm/
+-rw-rw-rw-   0        0        0      982 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/npm/__init__.py
+-rw-rw-rw-   0        0        0    10809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/npm/models.py
+-rw-rw-rw-   0        0        0    33781 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/npm/npm_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.681704 azure-devops-7.1.0b3/azure/devops/v7_0/nuget/
+-rw-rw-rw-   0        0        0      989 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/nuget/__init__.py
+-rw-rw-rw-   0        0        0    10432 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/nuget/models.py
+-rw-rw-rw-   0        0        0    16619 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/nuget/nuget_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.722576 azure-devops-7.1.0b3/azure/devops/v7_0/operations/
+-rw-rw-rw-   0        0        0      763 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/operations/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/operations/models.py
+-rw-rw-rw-   0        0        0     2208 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/operations/operations_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.759561 azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/
+-rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/__init__.py
+-rw-rw-rw-   0        0        0     9418 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/models.py
+-rw-rw-rw-   0        0        0     5073 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/pipeline_permissions_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.798890 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/
+-rw-rw-rw-   0        0        0     1299 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/__init__.py
+-rw-rw-rw-   0        0        0    19588 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/models.py
+-rw-rw-rw-   0        0        0    14169 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/pipelines_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.837320 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/
+-rw-rw-rw-   0        0        0     1048 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/__init__.py
+-rw-rw-rw-   0        0        0    21350 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/models.py
+-rw-rw-rw-   0        0        0    10429 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/pipelines_checks_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.873277 azure-devops-7.1.0b3/azure/devops/v7_0/policy/
+-rw-rw-rw-   0        0        0      884 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/policy/__init__.py
+-rw-rw-rw-   0        0        0    15233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/policy/models.py
+-rw-rw-rw-   0        0        0    15620 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/policy/policy_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.910026 azure-devops-7.1.0b3/azure/devops/v7_0/profile/
+-rw-rw-rw-   0        0        0      908 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile/__init__.py
+-rw-rw-rw-   0        0        0    10417 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile/models.py
+-rw-rw-rw-   0        0        0     3489 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile/profile_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.950174 azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/
+-rw-rw-rw-   0        0        0      739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/__init__.py
+-rw-rw-rw-   0        0        0     2886 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/models.py
+-rw-rw-rw-   0        0        0     2374 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/profile_regions_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:54.985678 azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/
+-rw-rw-rw-   0        0        0      901 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/__init__.py
+-rw-rw-rw-   0        0        0     9580 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/models.py
+-rw-rw-rw-   0        0        0     6327 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/project_analysis_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.020890 azure-devops-7.1.0b3/azure/devops/v7_0/provenance/
+-rw-rw-rw-   0        0        0      711 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/provenance/__init__.py
+-rw-rw-rw-   0        0        0     1967 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/provenance/models.py
+-rw-rw-rw-   0        0        0     2501 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/provenance/provenance_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.055684 azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/
+-rw-rw-rw-   0        0        0      973 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/__init__.py
+-rw-rw-rw-   0        0        0     9738 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/models.py
+-rw-rw-rw-   0        0        0    16679 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/py_pi_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.104922 azure-devops-7.1.0b3/azure/devops/v7_0/release/
+-rw-rw-rw-   0        0        0     3473 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_0/release/__init__.py
+-rw-rw-rw-   0        0        0   179618 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_0/release/models.py
+-rw-rw-rw-   0        0        0    54717 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_0/release/release_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.140163 azure-devops-7.1.0b3/azure/devops/v7_0/sbom/
+-rw-rw-rw-   0        0        0      820 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/sbom/__init__.py
+-rw-rw-rw-   0        0        0    16520 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/sbom/models.py
+-rw-rw-rw-   0        0        0     1177 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/sbom/sbom_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.177400 azure-devops-7.1.0b3/azure/devops/v7_0/search/
+-rw-rw-rw-   0        0        0     1660 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/search/__init__.py
+-rw-rw-rw-   0        0        0    51412 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/search/models.py
+-rw-rw-rw-   0        0        0     7951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/search/search_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.213539 azure-devops-7.1.0b3/azure/devops/v7_0/security/
+-rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/security/__init__.py
+-rw-rw-rw-   0        0        0    13405 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/security/models.py
+-rw-rw-rw-   0        0        0    14124 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/security/security_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.253718 azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/
+-rw-rw-rw-   0        0        0     1890 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/__init__.py
+-rw-rw-rw-   0        0        0    66419 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/models.py
+-rw-rw-rw-   0        0        0    17345 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/service_endpoint_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.292808 azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/
+-rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/__init__.py
+-rw-rw-rw-   0        0        0    64152 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/models.py
+-rw-rw-rw-   0        0        0    21308 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/service_hooks_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.316863 azure-devops-7.1.0b3/azure/devops/v7_0/settings/
+-rw-rw-rw-   0        0        0      638 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/settings/__init__.py
+-rw-rw-rw-   0        0        0     7639 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/settings/settings_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.351688 azure-devops-7.1.0b3/azure/devops/v7_0/symbol/
+-rw-rw-rw-   0        0        0      840 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/symbol/__init__.py
+-rw-rw-rw-   0        0        0    12241 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/symbol/models.py
+-rw-rw-rw-   0        0        0    13260 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/symbol/symbol_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.388356 azure-devops-7.1.0b3/azure/devops/v7_0/task/
+-rw-rw-rw-   0        0        0     1368 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task/__init__.py
+-rw-rw-rw-   0        0        0    34317 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task/models.py
+-rw-rw-rw-   0        0        0    27853 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task/task_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.433527 azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/
+-rw-rw-rw-   0        0        0     4200 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/__init__.py
+-rw-rw-rw-   0        0        0   192204 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/models.py
+-rw-rw-rw-   0        0        0    68198 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/task_agent_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.481547 azure-devops-7.1.0b3/azure/devops/v7_0/test/
+-rw-rw-rw-   0        0        0     3616 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test/__init__.py
+-rw-rw-rw-   0        0        0   206239 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test/models.py
+-rw-rw-rw-   0        0        0    68796 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test/test_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.522635 azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/
+-rw-rw-rw-   0        0        0     2477 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/__init__.py
+-rw-rw-rw-   0        0        0   106651 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/models.py
+-rw-rw-rw-   0        0        0    55123 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/test_plan_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.565725 azure-devops-7.1.0b3/azure/devops/v7_0/test_results/
+-rw-rw-rw-   0        0        0     3269 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_results/__init__.py
+-rw-rw-rw-   0        0        0   161630 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_results/models.py
+-rw-rw-rw-   0        0        0    21339 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/test_results/test_results_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.603704 azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/
+-rw-rw-rw-   0        0        0     1587 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/__init__.py
+-rw-rw-rw-   0        0        0    56530 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/models.py
+-rw-rw-rw-   0        0        0    46539 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/tfvc_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.637817 azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/
+-rw-rw-rw-   0        0        0      809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/__init__.py
+-rw-rw-rw-   0        0        0     7313 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/models.py
+-rw-rw-rw-   0        0        0     5176 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/token_admin_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.672572 azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/
+-rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/__init__.py
+-rw-rw-rw-   0        0        0     7392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/models.py
+-rw-rw-rw-   0        0        0    12373 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/upack_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.708359 azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/
+-rw-rw-rw-   0        0        0      861 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/__init__.py
+-rw-rw-rw-   0        0        0     4626 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/models.py
+-rw-rw-rw-   0        0        0     5165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/upack_packaging_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.744963 azure-devops-7.1.0b3/azure/devops/v7_0/wiki/
+-rw-rw-rw-   0        0        0     1460 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/wiki/__init__.py
+-rw-rw-rw-   0        0        0    40959 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/wiki/models.py
+-rw-rw-rw-   0        0        0    37957 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/wiki/wiki_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.785597 azure-devops-7.1.0b3/azure/devops/v7_0/work/
+-rw-rw-rw-   0        0        0     2622 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work/__init__.py
+-rw-rw-rw-   0        0        0    87293 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work/models.py
+-rw-rw-rw-   0        0        0    77467 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work/work_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.829645 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/
+-rw-rw-rw-   0        0        0     3148 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/__init__.py
+-rw-rw-rw-   0        0        0   117974 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/models.py
+-rw-rw-rw-   0        0        0   114702 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/work_item_tracking_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.868548 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/
+-rw-rw-rw-   0        0        0     1817 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/__init__.py
+-rw-rw-rw-   0        0        0    57182 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/models.py
+-rw-rw-rw-   0        0        0    68317 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/work_item_tracking_process_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.901605 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/
+-rw-rw-rw-   0        0        0      894 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/__init__.py
+-rw-rw-rw-   0        0        0     8972 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/models.py
+-rw-rw-rw-   0        0        0     6446 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/work_item_tracking_process_template_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.916859 azure-devops-7.1.0b3/azure/devops/v7_1/
+-rw-rw-rw-   0        0        0      557 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.942933 azure-devops-7.1.0b3/azure/devops/v7_1/accounts/
+-rw-rw-rw-   0        0        0      742 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/accounts/__init__.py
+-rw-rw-rw-   0        0        0     2390 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/accounts/accounts_client.py
+-rw-rw-rw-   0        0        0     6285 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/accounts/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:55.968719 azure-devops-7.1.0b3/azure/devops/v7_1/audit/
+-rw-rw-rw-   0        0        0      771 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/audit/__init__.py
+-rw-rw-rw-   0        0        0     9739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/audit/audit_client.py
+-rw-rw-rw-   0        0        0    13645 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/audit/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.005689 azure-devops-7.1.0b3/azure/devops/v7_1/build/
+-rw-rw-rw-   0        0        0     3114 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/build/__init__.py
+-rw-rw-rw-   0        0        0   132013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/build/build_client.py
+-rw-rw-rw-   0        0        0   151261 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/build/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.040894 azure-devops-7.1.0b3/azure/devops/v7_1/cix/
+-rw-rw-rw-   0        0        0     1013 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/cix/__init__.py
+-rw-rw-rw-   0        0        0     7713 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/cix/cix_client.py
+-rw-rw-rw-   0        0        0    16667 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/cix/models.py
+-rw-rw-rw-   0        0        0    21269 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.056552 azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/
+-rw-rw-rw-   0        0        0      694 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/client_trace_client.py
+-rw-rw-rw-   0        0        0     1978 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.083654 azure-devops-7.1.0b3/azure/devops/v7_1/contributions/
+-rw-rw-rw-   0        0        0     1406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/contributions/__init__.py
+-rw-rw-rw-   0        0        0     5750 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/contributions/contributions_client.py
+-rw-rw-rw-   0        0        0    39700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/contributions/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.111951 azure-devops-7.1.0b3/azure/devops/v7_1/core/
+-rw-rw-rw-   0        0        0     1275 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/core/__init__.py
+-rw-rw-rw-   0        0        0    27326 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/core/core_client.py
+-rw-rw-rw-   0        0        0    39744 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/core/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.127552 azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/
+-rw-rw-rw-   0        0        0      730 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/customer_intelligence_client.py
+-rw-rw-rw-   0        0        0     1248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.155007 azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/
+-rw-rw-rw-   0        0        0     1116 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/__init__.py
+-rw-rw-rw-   0        0        0    27966 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/dashboard_client.py
+-rw-rw-rw-   0        0        0    43220 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.190744 azure-devops-7.1.0b3/azure/devops/v7_1/elastic/
+-rw-rw-rw-   0        0        0      942 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/elastic/__init__.py
+-rw-rw-rw-   0        0        0     8885 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/elastic/elastic_client.py
+-rw-rw-rw-   0        0        0    24700 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/elastic/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.221553 azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/
+-rw-rw-rw-   0        0        0     1787 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/__init__.py
+-rw-rw-rw-   0        0        0     8156 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/extension_management_client.py
+-rw-rw-rw-   0        0        0    62180 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.238664 azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/
+-rw-rw-rw-   0        0        0      737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/__init__.py
+-rw-rw-rw-   0        0        0     7737 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/feature_availability_client.py
+-rw-rw-rw-   0        0        0     1956 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.264918 azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/
+-rw-rw-rw-   0        0        0      951 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/__init__.py
+-rw-rw-rw-   0        0        0    13334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/feature_management_client.py
+-rw-rw-rw-   0        0        0    10629 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.304821 azure-devops-7.1.0b3/azure/devops/v7_1/feed/
+-rw-rw-rw-   0        0        0     1455 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feed/__init__.py
+-rw-rw-rw-   0        0        0    54406 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feed/feed_client.py
+-rw-rw-rw-   0        0        0    60661 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/feed/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.331762 azure-devops-7.1.0b3/azure/devops/v7_1/file_container/
+-rw-rw-rw-   0        0        0      756 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/file_container/__init__.py
+-rw-rw-rw-   0        0        0     7447 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/file_container/file_container_client.py
+-rw-rw-rw-   0        0        0     9042 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/file_container/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.364901 azure-devops-7.1.0b3/azure/devops/v7_1/gallery/
+-rw-rw-rw-   0        0        0     2229 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/gallery/__init__.py
+-rw-rw-rw-   0        0        0   105334 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/gallery/gallery_client.py
+-rw-rw-rw-   0        0        0    87095 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/gallery/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.419973 azure-devops-7.1.0b3/azure/devops/v7_1/git/
+-rw-rw-rw-   0        0        0     3564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/git/__init__.py
+-rw-rw-rw-   0        0        0     1653 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_1/git/git_client.py
+-rw-rw-rw-   0        0        0   212306 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/git/git_client_base.py
+-rw-rw-rw-   0        0        0   175989 2023-04-26 17:21:57.000000 azure-devops-7.1.0b3/azure/devops/v7_1/git/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.458757 azure-devops-7.1.0b3/azure/devops/v7_1/graph/
+-rw-rw-rw-   0        0        0     1640 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/graph/__init__.py
+-rw-rw-rw-   0        0        0    31411 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/graph/graph_client.py
+-rw-rw-rw-   0        0        0    57092 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/graph/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.485720 azure-devops-7.1.0b3/azure/devops/v7_1/identity/
+-rw-rw-rw-   0        0        0     1165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/identity/__init__.py
+-rw-rw-rw-   0        0        0    30320 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/identity/identity_client.py
+-rw-rw-rw-   0        0        0    28794 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/identity/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.520798 azure-devops-7.1.0b3/azure/devops/v7_1/location/
+-rw-rw-rw-   0        0        0      838 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/location/__init__.py
+-rw-rw-rw-   0        0        0     9773 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/location/location_client.py
+-rw-rw-rw-   0        0        0    21179 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/location/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.556027 azure-devops-7.1.0b3/azure/devops/v7_1/maven/
+-rw-rw-rw-   0        0        0     1486 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/maven/__init__.py
+-rw-rw-rw-   0        0        0    17516 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/maven/maven_client.py
+-rw-rw-rw-   0        0        0    31584 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/maven/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.595545 azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/
+-rw-rw-rw-   0        0        0     2315 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/__init__.py
+-rw-rw-rw-   0        0        0    25642 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/member_entitlement_management_client.py
+-rw-rw-rw-   0        0        0    89340 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/models.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.625722 azure-devops-7.1.0b3/azure/devops/v7_1/notification/
+-rw-rw-rw-   0        0        0     2612 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/notification/__init__.py
+-rw-rw-rw-   0        0        0    77210 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/notification/models.py
+-rw-rw-rw-   0        0        0    17344 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/notification/notification_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.652476 azure-devops-7.1.0b3/azure/devops/v7_1/npm/
+-rw-rw-rw-   0        0        0      982 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/npm/__init__.py
+-rw-rw-rw-   0        0        0    10809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/npm/models.py
+-rw-rw-rw-   0        0        0    34333 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/npm/npm_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.677946 azure-devops-7.1.0b3/azure/devops/v7_1/nuget/
+-rw-rw-rw-   0        0        0      989 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/nuget/__init__.py
+-rw-rw-rw-   0        0        0    10713 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/nuget/models.py
+-rw-rw-rw-   0        0        0    16739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/nuget/nuget_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.721642 azure-devops-7.1.0b3/azure/devops/v7_1/operations/
+-rw-rw-rw-   0        0        0      763 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/operations/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/operations/models.py
+-rw-rw-rw-   0        0        0     2228 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/operations/operations_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.746968 azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/
+-rw-rw-rw-   0        0        0      854 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/__init__.py
+-rw-rw-rw-   0        0        0     9418 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/models.py
+-rw-rw-rw-   0        0        0     5073 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/pipeline_permissions_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.790637 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/
+-rw-rw-rw-   0        0        0     1365 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/__init__.py
+-rw-rw-rw-   0        0        0    22233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/models.py
+-rw-rw-rw-   0        0        0    14409 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/pipelines_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.826995 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/
+-rw-rw-rw-   0        0        0     1066 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/__init__.py
+-rw-rw-rw-   0        0        0    22399 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/models.py
+-rw-rw-rw-   0        0        0    10429 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/pipelines_checks_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.853990 azure-devops-7.1.0b3/azure/devops/v7_1/policy/
+-rw-rw-rw-   0        0        0      884 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/policy/__init__.py
+-rw-rw-rw-   0        0        0    15233 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/policy/models.py
+-rw-rw-rw-   0        0        0    15624 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/policy/policy_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.888744 azure-devops-7.1.0b3/azure/devops/v7_1/profile/
+-rw-rw-rw-   0        0        0      908 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile/__init__.py
+-rw-rw-rw-   0        0        0    10417 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile/models.py
+-rw-rw-rw-   0        0        0     3513 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile/profile_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.913894 azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/
+-rw-rw-rw-   0        0        0      739 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/__init__.py
+-rw-rw-rw-   0        0        0     2886 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/models.py
+-rw-rw-rw-   0        0        0     2374 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/profile_regions_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.940323 azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/
+-rw-rw-rw-   0        0        0      901 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/__init__.py
+-rw-rw-rw-   0        0        0     9580 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/models.py
+-rw-rw-rw-   0        0        0     6447 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/project_analysis_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.955854 azure-devops-7.1.0b3/azure/devops/v7_1/provenance/
+-rw-rw-rw-   0        0        0      711 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/provenance/__init__.py
+-rw-rw-rw-   0        0        0     1967 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/provenance/models.py
+-rw-rw-rw-   0        0        0     2501 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/provenance/provenance_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:56.981628 azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/
+-rw-rw-rw-   0        0        0      973 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/__init__.py
+-rw-rw-rw-   0        0        0     9738 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/models.py
+-rw-rw-rw-   0        0        0    16679 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/py_pi_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.018954 azure-devops-7.1.0b3/azure/devops/v7_1/release/
+-rw-rw-rw-   0        0        0     3473 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_1/release/__init__.py
+-rw-rw-rw-   0        0        0   179609 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_1/release/models.py
+-rw-rw-rw-   0        0        0    55421 2023-04-26 17:21:34.000000 azure-devops-7.1.0b3/azure/devops/v7_1/release/release_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.036684 azure-devops-7.1.0b3/azure/devops/v7_1/sbom/
+-rw-rw-rw-   0        0        0      820 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/sbom/__init__.py
+-rw-rw-rw-   0        0        0    16729 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/sbom/models.py
+-rw-rw-rw-   0        0        0     1177 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/sbom/sbom_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.072581 azure-devops-7.1.0b3/azure/devops/v7_1/search/
+-rw-rw-rw-   0        0        0     1660 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/search/__init__.py
+-rw-rw-rw-   0        0        0    51412 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/search/models.py
+-rw-rw-rw-   0        0        0     8119 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/search/search_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.107913 azure-devops-7.1.0b3/azure/devops/v7_1/security/
+-rw-rw-rw-   0        0        0      898 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/security/__init__.py
+-rw-rw-rw-   0        0        0    13405 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/security/models.py
+-rw-rw-rw-   0        0        0    14340 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/security/security_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.145618 azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/
+-rw-rw-rw-   0        0        0     1835 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/__init__.py
+-rw-rw-rw-   0        0        0    65327 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/models.py
+-rw-rw-rw-   0        0        0    17633 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/service_endpoint_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.176552 azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/
+-rw-rw-rw-   0        0        0     1564 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/__init__.py
+-rw-rw-rw-   0        0        0    64147 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/models.py
+-rw-rw-rw-   0        0        0    21860 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/service_hooks_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.189678 azure-devops-7.1.0b3/azure/devops/v7_1/settings/
+-rw-rw-rw-   0        0        0      638 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/settings/__init__.py
+-rw-rw-rw-   0        0        0     7639 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/settings/settings_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.216803 azure-devops-7.1.0b3/azure/devops/v7_1/symbol/
+-rw-rw-rw-   0        0        0      840 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/symbol/__init__.py
+-rw-rw-rw-   0        0        0    12241 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/symbol/models.py
+-rw-rw-rw-   0        0        0    13596 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/symbol/symbol_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.254677 azure-devops-7.1.0b3/azure/devops/v7_1/task/
+-rw-rw-rw-   0        0        0     1408 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task/__init__.py
+-rw-rw-rw-   0        0        0    38822 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task/models.py
+-rw-rw-rw-   0        0        0    30129 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task/task_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.303292 azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/
+-rw-rw-rw-   0        0        0     4145 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/__init__.py
+-rw-rw-rw-   0        0        0   192209 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/models.py
+-rw-rw-rw-   0        0        0    69590 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/task_agent_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.345012 azure-devops-7.1.0b3/azure/devops/v7_1/test/
+-rw-rw-rw-   0        0        0     3616 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test/__init__.py
+-rw-rw-rw-   0        0        0   206235 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test/models.py
+-rw-rw-rw-   0        0        0    69828 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test/test_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.381257 azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/
+-rw-rw-rw-   0        0        0     2477 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/__init__.py
+-rw-rw-rw-   0        0        0   106651 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/models.py
+-rw-rw-rw-   0        0        0    56067 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/test_plan_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.428597 azure-devops-7.1.0b3/azure/devops/v7_1/test_results/
+-rw-rw-rw-   0        0        0     3361 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_results/__init__.py
+-rw-rw-rw-   0        0        0   164018 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_results/models.py
+-rw-rw-rw-   0        0        0    31216 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/test_results/test_results_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.473348 azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/
+-rw-rw-rw-   0        0        0     1587 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/__init__.py
+-rw-rw-rw-   0        0        0    56986 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/models.py
+-rw-rw-rw-   0        0        0    47091 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/tfvc_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.511370 azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/
+-rw-rw-rw-   0        0        0      809 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/__init__.py
+-rw-rw-rw-   0        0        0     7313 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/models.py
+-rw-rw-rw-   0        0        0     5248 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/token_admin_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.539336 azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/
+-rw-rw-rw-   0        0        0      925 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/__init__.py
+-rw-rw-rw-   0        0        0     7392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/models.py
+-rw-rw-rw-   0        0        0    12373 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/upack_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.567138 azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/
+-rw-rw-rw-   0        0        0      861 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/__init__.py
+-rw-rw-rw-   0        0        0     4626 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/models.py
+-rw-rw-rw-   0        0        0     5165 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/upack_packaging_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.597601 azure-devops-7.1.0b3/azure/devops/v7_1/wiki/
+-rw-rw-rw-   0        0        0     1460 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/wiki/__init__.py
+-rw-rw-rw-   0        0        0    41392 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/wiki/models.py
+-rw-rw-rw-   0        0        0    38413 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/wiki/wiki_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.641581 azure-devops-7.1.0b3/azure/devops/v7_1/work/
+-rw-rw-rw-   0        0        0     2622 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work/__init__.py
+-rw-rw-rw-   0        0        0    87669 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work/models.py
+-rw-rw-rw-   0        0        0    78795 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work/work_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.691316 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/
+-rw-rw-rw-   0        0        0     3456 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/__init__.py
+-rw-rw-rw-   0        0        0   129996 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/models.py
+-rw-rw-rw-   0        0        0   125171 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/work_item_tracking_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.724765 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/
+-rw-rw-rw-   0        0        0     1817 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/__init__.py
+-rw-rw-rw-   0        0        0    57547 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/models.py
+-rw-rw-rw-   0        0        0    69684 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/work_item_tracking_process_client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.751386 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/
+-rw-rw-rw-   0        0        0      894 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/__init__.py
+-rw-rw-rw-   0        0        0     8972 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/models.py
+-rw-rw-rw-   0        0        0     6566 2023-04-18 19:56:16.000000 azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/work_item_tracking_process_template_client.py
+-rw-rw-rw-   0        0        0      366 2023-04-26 17:21:57.000000 azure-devops-7.1.0b3/azure/devops/version.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:35:57.760411 azure-devops-7.1.0b3/azure_devops.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-04-26 17:35:52.000000 azure-devops-7.1.0b3/azure_devops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19370 2023-04-26 17:35:52.000000 azure-devops-7.1.0b3/azure_devops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 17:35:52.000000 azure-devops-7.1.0b3/azure_devops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-26 17:35:52.000000 azure-devops-7.1.0b3/azure_devops.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 17:35:52.000000 azure-devops-7.1.0b3/azure_devops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 17:35:57.763411 azure-devops-7.1.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-04-26 17:21:57.000000 azure-devops-7.1.0b3/setup.py
```

### Comparing `azure-devops-7.1.0b2/LICENSE.txt` & `azure-devops-7.1.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/PKG-INFO` & `azure-devops-7.1.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops
-Version: 7.1.0b2
+Version: 7.1.0b3
 Summary: Python wrapper around the Azure DevOps 7.x APIs
 Home-page: https://github.com/microsoft/azure-devops-python-api
 Author: Microsoft Corporation
 License: MIT
 Keywords: Microsoft,VSTS,Team Services,SDK,AzureTfs,AzureDevOps,DevOps
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `azure-devops-7.1.0b2/azure/devops/_file_cache.py` & `azure-devops-7.1.0b3/azure/devops/_file_cache.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/_models.py` & `azure-devops-7.1.0b3/azure/devops/_models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/client.py` & `azure-devops-7.1.0b3/azure/devops/client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/client_configuration.py` & `azure-devops-7.1.0b3/azure/devops/client_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/connection.py` & `azure-devops-7.1.0b3/azure/devops/connection.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/exceptions.py` & `azure-devops-7.1.0b3/azure/devops/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/issue_tests/__init__.py` & `azure-devops-7.1.0b3/azure/devops/issue_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/issue_tests/test_issue_268.py` & `azure-devops-7.1.0b3/azure/devops/issue_tests/test_issue_268.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/accounts/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/accounts/accounts_client.py` & `azure-devops-7.1.0b3/azure/devops/released/accounts/accounts_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/build/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/build/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/build/build_client.py` & `azure-devops-7.1.0b3/azure/devops/released/build/build_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/cix/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/cix/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/cix/cix_client.py` & `azure-devops-7.1.0b3/azure/devops/released/cix/cix_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/client_factory.py` & `azure-devops-7.1.0b3/azure/devops/released/client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/core/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/core/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/core/core_client.py` & `azure-devops-7.1.0b3/azure/devops/released/core/core_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/elastic/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/elastic/elastic_client.py` & `azure-devops-7.1.0b3/azure/devops/released/elastic/elastic_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/feed/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/feed/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/feed/feed_client.py` & `azure-devops-7.1.0b3/azure/devops/released/feed/feed_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/git/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/git/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/git/git_client.py` & `azure-devops-7.1.0b3/azure/devops/released/git/git_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/git/git_client_base.py` & `azure-devops-7.1.0b3/azure/devops/released/git/git_client_base.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/graph/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/graph/graph_client.py` & `azure-devops-7.1.0b3/azure/devops/released/graph/graph_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/identity/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/identity/identity_client.py` & `azure-devops-7.1.0b3/azure/devops/released/identity/identity_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/member_entitlement_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/member_entitlement_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/member_entitlement_management/member_entitlement_management_client.py` & `azure-devops-7.1.0b3/azure/devops/released/member_entitlement_management/member_entitlement_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/notification/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/notification/notification_client.py` & `azure-devops-7.1.0b3/azure/devops/released/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/npm/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/npm/npm_client.py` & `azure-devops-7.1.0b3/azure/devops/released/npm/npm_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/nuget/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/nuget/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/nuget/nuget_client.py` & `azure-devops-7.1.0b3/azure/devops/released/nuget/nuget_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/operations/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/operations/operations_client.py` & `azure-devops-7.1.0b3/azure/devops/released/operations/operations_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/pipelines/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/pipelines/pipelines_client.py` & `azure-devops-7.1.0b3/azure/devops/released/pipelines/pipelines_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/policy/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/policy/policy_client.py` & `azure-devops-7.1.0b3/azure/devops/released/policy/policy_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/profile/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/profile/profile_client.py` & `azure-devops-7.1.0b3/azure/devops/released/profile/profile_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/project_analysis/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/project_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/project_analysis/project_analysis_client.py` & `azure-devops-7.1.0b3/azure/devops/released/project_analysis/project_analysis_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/release/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/release/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/release/release_client.py` & `azure-devops-7.1.0b3/azure/devops/released/release/release_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/search/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/search/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/search/search_client.py` & `azure-devops-7.1.0b3/azure/devops/released/search/search_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/security/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/security/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/security/security_client.py` & `azure-devops-7.1.0b3/azure/devops/released/security/security_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/service_endpoint/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/service_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/service_endpoint/service_endpoint_client.py` & `azure-devops-7.1.0b3/azure/devops/released/service_endpoint/service_endpoint_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/service_hooks/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/service_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/service_hooks/service_hooks_client.py` & `azure-devops-7.1.0b3/azure/devops/released/service_hooks/service_hooks_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/symbol/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/symbol/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/symbol/symbol_client.py` & `azure-devops-7.1.0b3/azure/devops/released/symbol/symbol_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/task/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/task/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/task/task_client.py` & `azure-devops-7.1.0b3/azure/devops/released/task/task_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/task_agent/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/task_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/task_agent/task_agent_client.py` & `azure-devops-7.1.0b3/azure/devops/released/task_agent/task_agent_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/test/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test/test_client.py` & `azure-devops-7.1.0b3/azure/devops/released/test/test_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test_plan/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/test_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test_plan/test_plan_client.py` & `azure-devops-7.1.0b3/azure/devops/released/test_plan/test_plan_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test_results/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/test_results/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/test_results/test_results_client.py` & `azure-devops-7.1.0b3/azure/devops/released/test_results/test_results_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/tfvc/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/tfvc/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/tfvc/tfvc_client.py` & `azure-devops-7.1.0b3/azure/devops/released/tfvc/tfvc_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/token_admin/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/token_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/token_admin/token_admin_client.py` & `azure-devops-7.1.0b3/azure/devops/released/token_admin/token_admin_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/wiki/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/wiki/wiki_client.py` & `azure-devops-7.1.0b3/azure/devops/released/wiki/wiki_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/work/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work/work_client.py` & `azure-devops-7.1.0b3/azure/devops/released/work/work_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking/work_item_tracking_client.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking/work_item_tracking_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process/work_item_tracking_process_client.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process/work_item_tracking_process_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process_template/__init__.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process_template/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/released/work_item_tracking_process_template/work_item_tracking_process_template_client.py` & `azure-devops-7.1.0b3/azure/devops/released/work_item_tracking_process_template/work_item_tracking_process_template_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/accounts/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/accounts/accounts_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/accounts/accounts_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/accounts/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/accounts/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/audit/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/audit/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/audit/audit_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/audit/audit_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/audit/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/audit/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/build/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/build/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/build/build_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/build/build_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/build/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/build/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/cix/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/cix/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/cix/cix_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/cix/cix_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/cix/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/cix/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/client_factory.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/client_trace_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/client_trace_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/client_trace/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/client_trace/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/contributions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/contributions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/contributions/contributions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/contributions/contributions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/contributions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/contributions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/core/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/core/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/core/core_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/core/core_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/core/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/core/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/customer_intelligence_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/customer_intelligence_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/customer_intelligence/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/customer_intelligence/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/dashboard_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/dashboard_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/dashboard/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/dashboard/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/elastic/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/elastic/elastic_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/elastic/elastic_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/elastic/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/elastic/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/extension_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/extension_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/extension_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/extension_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/feature_availability_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/feature_availability_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_availability/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_availability/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/feature_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/feature_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feature_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feature_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feed/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feed/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feed/feed_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feed/feed_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/feed/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/feed/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/file_container/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/file_container/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/file_container/file_container_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/file_container/file_container_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/file_container/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/file_container/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/gallery/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/gallery/gallery_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/gallery/gallery_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/gallery/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/gallery/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/git/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/git/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/git/git_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/git/git_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/git/git_client_base.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/git/git_client_base.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/git/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/git/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,21 +647,21 @@
         self.changes = changes
         self.target_commit = target_commit
 
 
 class GitCommitChanges(Model):
     """
     :param change_counts:
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_0.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes:
     :type changes: list of :class:`object <azure.devops.v7_0.git.models.object>`
     """
 
     _attribute_map = {
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'}
     }
 
     def __init__(self, change_counts=None, changes=None):
         super(GitCommitChanges, self).__init__()
         self.change_counts = change_counts
         self.changes = changes
@@ -680,15 +680,15 @@
     :param comment_truncated: Indicates if the comment is truncated from the full Git commit comment message.
     :type comment_truncated: bool
     :param commit_id: ID (SHA-1) of the commit.
     :type commit_id: str
     :param committer: Committer of the commit.
     :type committer: :class:`GitUserDate <azure.devops.v7_0.git.models.GitUserDate>`
     :param change_counts: Counts of the types of changes (edits, deletes, etc.) included with the commit.
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_0.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes: An enumeration of the changes included with the commit.
     :type changes: list of :class:`object <azure.devops.v7_0.git.models.object>`
     :param parents: An enumeration of the parent commit IDs for this commit.
     :type parents: list of str
     :param push: The push associated with this commit.
     :type push: :class:`GitPushRef <azure.devops.v7_0.git.models.GitPushRef>`
     :param remote_url: Remote URL path to the commit.
@@ -704,15 +704,15 @@
     _attribute_map = {
         '_links': {'key': '_links', 'type': 'ReferenceLinks'},
         'author': {'key': 'author', 'type': 'GitUserDate'},
         'comment': {'key': 'comment', 'type': 'str'},
         'comment_truncated': {'key': 'commentTruncated', 'type': 'bool'},
         'commit_id': {'key': 'commitId', 'type': 'str'},
         'committer': {'key': 'committer', 'type': 'GitUserDate'},
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'},
         'parents': {'key': 'parents', 'type': '[str]'},
         'push': {'key': 'push', 'type': 'GitPushRef'},
         'remote_url': {'key': 'remoteUrl', 'type': 'str'},
         'statuses': {'key': 'statuses', 'type': '[GitStatus]'},
         'url': {'key': 'url', 'type': 'str'},
         'work_items': {'key': 'workItems', 'type': '[ResourceRef]'}
@@ -3365,15 +3365,15 @@
     :param comment_truncated: Indicates if the comment is truncated from the full Git commit comment message.
     :type comment_truncated: bool
     :param commit_id: ID (SHA-1) of the commit.
     :type commit_id: str
     :param committer: Committer of the commit.
     :type committer: :class:`GitUserDate <azure.devops.v7_0.git.models.GitUserDate>`
     :param change_counts: Counts of the types of changes (edits, deletes, etc.) included with the commit.
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_0.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes: An enumeration of the changes included with the commit.
     :type changes: list of :class:`object <azure.devops.v7_0.git.models.object>`
     :param parents: An enumeration of the parent commit IDs for this commit.
     :type parents: list of str
     :param push: The push associated with this commit.
     :type push: :class:`GitPushRef <azure.devops.v7_0.git.models.GitPushRef>`
     :param remote_url: Remote URL path to the commit.
@@ -3391,15 +3391,15 @@
     _attribute_map = {
         '_links': {'key': '_links', 'type': 'ReferenceLinks'},
         'author': {'key': 'author', 'type': 'GitUserDate'},
         'comment': {'key': 'comment', 'type': 'str'},
         'comment_truncated': {'key': 'commentTruncated', 'type': 'bool'},
         'commit_id': {'key': 'commitId', 'type': 'str'},
         'committer': {'key': 'committer', 'type': 'GitUserDate'},
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'},
         'parents': {'key': 'parents', 'type': '[str]'},
         'push': {'key': 'push', 'type': 'GitPushRef'},
         'remote_url': {'key': 'remoteUrl', 'type': 'str'},
         'statuses': {'key': 'statuses', 'type': '[GitStatus]'},
         'url': {'key': 'url', 'type': 'str'},
         'work_items': {'key': 'workItems', 'type': '[ResourceRef]'},
```

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/graph/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/graph/graph_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/graph/graph_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/graph/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/graph/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/identity/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/identity/identity_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/identity/identity_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/identity/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/identity/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/location/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/location/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/location/location_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/location/location_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/location/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/location/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/maven/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/maven/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/maven/maven_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/maven/maven_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/maven/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/maven/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/member_entitlement_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/member_entitlement_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/member_entitlement_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/member_entitlement_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/notification/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/notification/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/notification/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/notification/notification_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/npm/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/npm/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/npm/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/npm/npm_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/npm/npm_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/nuget/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/nuget/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/nuget/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/nuget/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/nuget/nuget_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/nuget/nuget_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/operations/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/operations/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/operations/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/operations/operations_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/operations/operations_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipeline_permissions/pipeline_permissions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipeline_permissions/pipeline_permissions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines/pipelines_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines/pipelines_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/pipelines_checks/pipelines_checks_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/pipelines_checks/pipelines_checks_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/policy/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/policy/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/policy/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/policy/policy_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/policy/policy_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile/profile_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile/profile_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/profile_regions/profile_regions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/profile_regions/profile_regions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/project_analysis/project_analysis_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/project_analysis/project_analysis_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/provenance/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/provenance/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/provenance/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/provenance/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/provenance/provenance_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/provenance/provenance_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/py_pi_api/py_pi_api_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/py_pi_api/py_pi_api_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/release/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/release/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/release/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/release/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/release/release_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/release/release_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/sbom/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/sbom/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/sbom/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/sbom/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/sbom/sbom_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/sbom/sbom_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/search/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/search/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/search/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/search/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/search/search_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/search/search_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/security/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/security/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/security/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/security/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/security/security_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/security/security_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_endpoint/service_endpoint_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_endpoint/service_endpoint_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/service_hooks/service_hooks_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/service_hooks/service_hooks_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/settings/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/settings/settings_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/settings/settings_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/symbol/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/symbol/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/symbol/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/symbol/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/symbol/symbol_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/symbol/symbol_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task/task_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task/task_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/task_agent/task_agent_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/task_agent/task_agent_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test/test_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_plan/test_plan_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_plan/test_plan_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_results/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_results/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_results/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_results/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/test_results/test_results_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/test_results/test_results_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/tfvc/tfvc_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/tfvc/tfvc_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/token_admin/token_admin_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/token_admin/token_admin_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_api/upack_api_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_api/upack_api_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/upack_packaging/upack_packaging_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/upack_packaging/upack_packaging_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/wiki/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/wiki/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/wiki/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/wiki/wiki_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/wiki/wiki_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work/work_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work/work_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking/work_item_tracking_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking/work_item_tracking_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process/work_item_tracking_process_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process/work_item_tracking_process_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_0/work_item_tracking_process_template/work_item_tracking_process_template_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_0/work_item_tracking_process_template/work_item_tracking_process_template_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/accounts/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/accounts/accounts_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/accounts/accounts_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/accounts/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/accounts/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/audit/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/audit/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/audit/audit_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/audit/audit_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/audit/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/audit/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/build/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/build/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/build/build_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/build/build_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/build/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/build/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/cix/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/cix/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/cix/cix_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/cix/cix_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/cix/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/cix/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/client_factory.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/client_trace_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/client_trace_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/client_trace/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/client_trace/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/contributions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/contributions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/contributions/contributions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/contributions/contributions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/contributions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/contributions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/core/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/core/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/core/core_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/core/core_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/core/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/core/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/customer_intelligence_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/customer_intelligence_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/customer_intelligence/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/customer_intelligence/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/dashboard_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/dashboard_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/dashboard/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/dashboard/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/elastic/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/elastic/elastic_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/elastic/elastic_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/elastic/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/elastic/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/extension_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/extension_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/extension_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/extension_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/feature_availability_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/feature_availability_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_availability/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_availability/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/feature_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/feature_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feature_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feature_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feed/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feed/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feed/feed_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feed/feed_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/feed/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/feed/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/file_container/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/file_container/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/file_container/file_container_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/file_container/file_container_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/file_container/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/file_container/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/gallery/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/gallery/gallery_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/gallery/gallery_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/gallery/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/gallery/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/git/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/git/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/git/git_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/git/git_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/git/git_client_base.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/git/git_client_base.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/git/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/git/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,21 +775,21 @@
         self.changes = changes
         self.target_commit = target_commit
 
 
 class GitCommitChanges(Model):
     """
     :param change_counts:
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_1.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes:
     :type changes: list of :class:`object <azure.devops.v7_1.git.models.object>`
     """
 
     _attribute_map = {
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'}
     }
 
     def __init__(self, change_counts=None, changes=None):
         super(GitCommitChanges, self).__init__()
         self.change_counts = change_counts
         self.changes = changes
@@ -810,15 +810,15 @@
     :param commit_id: ID (SHA-1) of the commit.
     :type commit_id: str
     :param committer: Committer of the commit.
     :type committer: :class:`GitUserDate <azure.devops.v7_1.git.models.GitUserDate>`
     :param commit_too_many_changes: Indicates that commit contains too many changes to be displayed
     :type commit_too_many_changes: bool
     :param change_counts: Counts of the types of changes (edits, deletes, etc.) included with the commit.
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_1.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes: An enumeration of the changes included with the commit.
     :type changes: list of :class:`object <azure.devops.v7_1.git.models.object>`
     :param parents: An enumeration of the parent commit IDs for this commit.
     :type parents: list of str
     :param push: The push associated with this commit.
     :type push: :class:`GitPushRef <azure.devops.v7_1.git.models.GitPushRef>`
     :param remote_url: Remote URL path to the commit.
@@ -835,15 +835,15 @@
         '_links': {'key': '_links', 'type': 'ReferenceLinks'},
         'author': {'key': 'author', 'type': 'GitUserDate'},
         'comment': {'key': 'comment', 'type': 'str'},
         'comment_truncated': {'key': 'commentTruncated', 'type': 'bool'},
         'commit_id': {'key': 'commitId', 'type': 'str'},
         'committer': {'key': 'committer', 'type': 'GitUserDate'},
         'commit_too_many_changes': {'key': 'commitTooManyChanges', 'type': 'bool'},
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'},
         'parents': {'key': 'parents', 'type': '[str]'},
         'push': {'key': 'push', 'type': 'GitPushRef'},
         'remote_url': {'key': 'remoteUrl', 'type': 'str'},
         'statuses': {'key': 'statuses', 'type': '[GitStatus]'},
         'url': {'key': 'url', 'type': 'str'},
         'work_items': {'key': 'workItems', 'type': '[ResourceRef]'}
@@ -3507,15 +3507,15 @@
     :param commit_id: ID (SHA-1) of the commit.
     :type commit_id: str
     :param committer: Committer of the commit.
     :type committer: :class:`GitUserDate <azure.devops.v7_1.git.models.GitUserDate>`
     :param commit_too_many_changes: Indicates that commit contains too many changes to be displayed
     :type commit_too_many_changes: bool
     :param change_counts: Counts of the types of changes (edits, deletes, etc.) included with the commit.
-    :type change_counts: :class:`ChangeCountDictionary <azure.devops.v7_1.git.models.ChangeCountDictionary>`
+    :type change_counts: dict
     :param changes: An enumeration of the changes included with the commit.
     :type changes: list of :class:`object <azure.devops.v7_1.git.models.object>`
     :param parents: An enumeration of the parent commit IDs for this commit.
     :type parents: list of str
     :param push: The push associated with this commit.
     :type push: :class:`GitPushRef <azure.devops.v7_1.git.models.GitPushRef>`
     :param remote_url: Remote URL path to the commit.
@@ -3534,15 +3534,15 @@
         '_links': {'key': '_links', 'type': 'ReferenceLinks'},
         'author': {'key': 'author', 'type': 'GitUserDate'},
         'comment': {'key': 'comment', 'type': 'str'},
         'comment_truncated': {'key': 'commentTruncated', 'type': 'bool'},
         'commit_id': {'key': 'commitId', 'type': 'str'},
         'committer': {'key': 'committer', 'type': 'GitUserDate'},
         'commit_too_many_changes': {'key': 'commitTooManyChanges', 'type': 'bool'},
-        'change_counts': {'key': 'changeCounts', 'type': 'ChangeCountDictionary'},
+        'change_counts': {'key': 'changeCounts', 'type': '{int}'},
         'changes': {'key': 'changes', 'type': '[object]'},
         'parents': {'key': 'parents', 'type': '[str]'},
         'push': {'key': 'push', 'type': 'GitPushRef'},
         'remote_url': {'key': 'remoteUrl', 'type': 'str'},
         'statuses': {'key': 'statuses', 'type': '[GitStatus]'},
         'url': {'key': 'url', 'type': 'str'},
         'work_items': {'key': 'workItems', 'type': '[ResourceRef]'},
```

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/graph/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/graph/graph_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/graph/graph_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/graph/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/graph/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/identity/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/identity/identity_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/identity/identity_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/identity/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/identity/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/location/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/location/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/location/location_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/location/location_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/location/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/location/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/maven/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/maven/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/maven/maven_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/maven/maven_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/maven/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/maven/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/member_entitlement_management_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/member_entitlement_management_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/member_entitlement_management/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/member_entitlement_management/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/notification/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/notification/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/notification/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/notification/notification_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/npm/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/npm/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/npm/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/npm/npm_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/npm/npm_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/nuget/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/nuget/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/nuget/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/nuget/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/nuget/nuget_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/nuget/nuget_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/operations/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/operations/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/operations/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/operations/operations_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/operations/operations_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipeline_permissions/pipeline_permissions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipeline_permissions/pipeline_permissions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines/pipelines_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines/pipelines_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/pipelines_checks/pipelines_checks_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/pipelines_checks/pipelines_checks_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/policy/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/policy/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/policy/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/policy/policy_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/policy/policy_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile/profile_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile/profile_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/profile_regions/profile_regions_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/profile_regions/profile_regions_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/project_analysis/project_analysis_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/project_analysis/project_analysis_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/provenance/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/provenance/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/provenance/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/provenance/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/provenance/provenance_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/provenance/provenance_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/py_pi_api/py_pi_api_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/py_pi_api/py_pi_api_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/release/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/release/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/release/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/release/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/release/release_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/release/release_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/sbom/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/sbom/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/sbom/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/sbom/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/sbom/sbom_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/sbom/sbom_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/search/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/search/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/search/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/search/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/search/search_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/search/search_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/security/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/security/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/security/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/security/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/security/security_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/security/security_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_endpoint/service_endpoint_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_endpoint/service_endpoint_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/service_hooks/service_hooks_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/service_hooks/service_hooks_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/settings/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/settings/settings_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/settings/settings_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/symbol/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/symbol/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/symbol/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/symbol/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/symbol/symbol_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/symbol/symbol_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task/task_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task/task_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/task_agent/task_agent_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/task_agent/task_agent_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test/test_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_plan/test_plan_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_plan/test_plan_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_results/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_results/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_results/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_results/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/test_results/test_results_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/test_results/test_results_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/tfvc/tfvc_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/tfvc/tfvc_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/token_admin/token_admin_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/token_admin/token_admin_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_api/upack_api_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_api/upack_api_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/upack_packaging/upack_packaging_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/upack_packaging/upack_packaging_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/wiki/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/wiki/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/wiki/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/wiki/wiki_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/wiki/wiki_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work/work_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work/work_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking/work_item_tracking_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking/work_item_tracking_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process/work_item_tracking_process_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process/work_item_tracking_process_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/__init__.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/models.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/models.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure/devops/v7_1/work_item_tracking_process_template/work_item_tracking_process_template_client.py` & `azure-devops-7.1.0b3/azure/devops/v7_1/work_item_tracking_process_template/work_item_tracking_process_template_client.py`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/azure_devops.egg-info/PKG-INFO` & `azure-devops-7.1.0b3/azure_devops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops
-Version: 7.1.0b2
+Version: 7.1.0b3
 Summary: Python wrapper around the Azure DevOps 7.x APIs
 Home-page: https://github.com/microsoft/azure-devops-python-api
 Author: Microsoft Corporation
 License: MIT
 Keywords: Microsoft,VSTS,Team Services,SDK,AzureTfs,AzureDevOps,DevOps
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `azure-devops-7.1.0b2/azure_devops.egg-info/SOURCES.txt` & `azure-devops-7.1.0b3/azure_devops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-devops-7.1.0b2/setup.py` & `azure-devops-7.1.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 from setuptools import setup, find_packages
 
 NAME = "azure-devops"
-VERSION = "7.1.0b2"
+VERSION = "7.1.0b3"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

