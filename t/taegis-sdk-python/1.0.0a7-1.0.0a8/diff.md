# Comparing `tmp/taegis-sdk-python-1.0.0a7.tar.gz` & `tmp/taegis-sdk-python-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.0a7.tar", last modified: Wed Apr 12 20:03:55 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.0a8.tar", last modified: Tue Apr 25 17:56:51 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.0a7.tar` & `taegis-sdk-python-1.0.0a8.tar`

### file list

```diff
@@ -1,174 +1,184 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.653665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8552 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.654665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    11461 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.654665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.655665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.656665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.657665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.658665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9259 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12852 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24754 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.658665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.659665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.660665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15763 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    22552 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    30927 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.661665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.662665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8037 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.662665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.663665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4109 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.664665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.665665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12950 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.666665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22054 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27703 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39186 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.666665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6558 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    36501 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.667665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9242 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.668665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.669665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6685 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.670665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16048 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.670665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.671665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10847 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31499 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.672665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13732 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.673665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7946 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.674665 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25285 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-12 19:27:04.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:03:55.653665 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6829 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 20:03:55.000000 taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.483963 taegis-sdk-python-1.0.0a8/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-25 17:56:29.000000 taegis-sdk-python-1.0.0a8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-04-25 17:56:51.482963 taegis-sdk-python-1.0.0a8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 17:56:51.483963 taegis-sdk-python-1.0.0a8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-04-25 17:56:29.000000 taegis-sdk-python-1.0.0a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.458963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8552 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.459963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    11799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.460963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.461963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.461963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.463963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.463963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9259 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12852 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24754 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.464963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.465963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.466963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15774 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    22563 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    30929 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.467963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.468963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.469963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.470963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.470963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.471963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.472963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12950 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24248 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.473963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22054 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27703 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39186 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.474963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6558 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    36501 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.475963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9242 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.476963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.477963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.478963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16048 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.478963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.479963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31540 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.480963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13732 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.481963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.482963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25501 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.459963 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.0a7/LICENSE` & `taegis-sdk-python-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/PKG-INFO` & `taegis-sdk-python-1.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a7/README.md` & `taegis-sdk-python-1.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/setup.py` & `taegis-sdk-python-1.0.0a8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     author="Secureworks",
     author_email="sdks@secureworks.com",
     description="Taegis Python SDK",
     long_description=README.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/secureworks/taegis-sdk-python",
     packages=setuptools.find_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         package.replace("==", ">=")
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from taegis_sdk_python.services.comments import CommentsService
 from taegis_sdk_python.services.endpoint_command_manager import (
     EndpointCommandManagerService,
 )
 from taegis_sdk_python.services.endpoint_management_service import (
     EndpointManagementServiceService,
 )
+from taegis_sdk_python.services.entity_profile import EntityProfileService
 from taegis_sdk_python.services.event_search import EventSearchService
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
@@ -88,14 +89,15 @@
         self._assets2 = None
         self._audits = None
         self._clients = None
         self._collector = None
         self._comments = None
         self._endpoint_command_manager = None
         self._endpoint_management_service = None
+        self._entity_profile = None
         self._event_search = None
         self._events = None
         self._exports = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
         self._notebooks = None
@@ -251,14 +253,21 @@
     def endpoint_management_service(self):
         """Endpoint Management Service Endpoint."""
         if not self._endpoint_management_service:
             self._endpoint_management_service = EndpointManagementServiceService(self)
         return self._endpoint_management_service
 
     @property
+    def entity_profile(self):
+        """Entity Profile Service Endpoint."""
+        if not self._entity_profile:
+            self._entity_profile = EntityProfileService(self)
+        return self._entity_profile
+
+    @property
     def event_search(self):
         """Events Search Service Endpoint."""
         if not self._event_search:
             self._event_search = EventSearchService(self)
         return self._event_search
 
     @property
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             },
             output="",
         )
         if result.get(endpoint) is not None:
             return result.get(endpoint)
         raise GraphQLNoRowsInResultSetError("for mutation deleteOSConfig")
 
-    def add_host(self, cluster_id: str, host_input: HostsInput) -> Any:
+    def add_host(self, cluster_id: str, host_input: HostsInput) -> Dict[str, Any]:
         """Add a address:hostname mapping to a given cluster."""
         endpoint = "addHost"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "clusterID": prepare_input(cluster_id),
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             },
             output=build_output_string(Credentials),
         )
         if result.get(endpoint) is not None:
             return Credentials.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query getClusterCredentials")
 
-    def get_hosts(self, cluster_id: str) -> Any:
+    def get_hosts(self, cluster_id: str) -> Dict[str, Any]:
         """Get all of the host->address mappings associated with a given cluster."""
         endpoint = "getHosts"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
                 "clusterID": prepare_input(cluster_id),
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     """EndpointInput."""
 
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
     address: Optional[str] = field(default=None, metadata=config(field_name="address"))
     port: Optional[int] = field(default=None, metadata=config(field_name="port"))
-    credentials: Optional[str] = field(
+    credentials: Optional[Any] = field(
         default=None, metadata=config(field_name="credentials")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class ValidityPeriod:
@@ -190,20 +190,20 @@
 class Network:
     """Network."""
 
     dhcp: Optional[bool] = field(default=None, metadata=config(field_name="dhcp"))
     hostname: Optional[str] = field(
         default=None, metadata=config(field_name="hostname")
     )
-    hosts: Optional[Any] = field(default=None, metadata=config(field_name="hosts"))
+    hosts: Optional[dict] = field(default=None, metadata=config(field_name="hosts"))
     address: Optional[str] = field(default=None, metadata=config(field_name="address"))
     mask: Optional[str] = field(default=None, metadata=config(field_name="mask"))
     gateway: Optional[str] = field(default=None, metadata=config(field_name="gateway"))
-    dns: Optional[Any] = field(default=None, metadata=config(field_name="dns"))
-    ntp: Optional[Any] = field(default=None, metadata=config(field_name="ntp"))
+    dns: Optional[str] = field(default=None, metadata=config(field_name="dns"))
+    ntp: Optional[str] = field(default=None, metadata=config(field_name="ntp"))
     proxy: Optional[str] = field(default=None, metadata=config(field_name="proxy"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class HostsInput:
     """HostsInput."""
@@ -524,20 +524,20 @@
     status_message: Optional[str] = field(
         default=None, metadata=config(field_name="statusMessage")
     )
     dhcp: Optional[bool] = field(default=None, metadata=config(field_name="dhcp"))
     hostname: Optional[str] = field(
         default=None, metadata=config(field_name="hostname")
     )
-    hosts: Optional[Any] = field(default=None, metadata=config(field_name="hosts"))
+    hosts: Optional[dict] = field(default=None, metadata=config(field_name="hosts"))
     address: Optional[str] = field(default=None, metadata=config(field_name="address"))
     mask: Optional[str] = field(default=None, metadata=config(field_name="mask"))
     gateway: Optional[str] = field(default=None, metadata=config(field_name="gateway"))
-    dns: Optional[Any] = field(default=None, metadata=config(field_name="dns"))
-    ntp: Optional[Any] = field(default=None, metadata=config(field_name="ntp"))
+    dns: Optional[str] = field(default=None, metadata=config(field_name="dns"))
+    ntp: Optional[str] = field(default=None, metadata=config(field_name="ntp"))
     proxy: Optional[str] = field(default=None, metadata=config(field_name="proxy"))
     status: Optional[ConfigStatus] = field(
         default=None, metadata=config(field_name="status")
     )
 
 
 @dataclass_json
@@ -587,15 +587,15 @@
     )
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
     )
     address: Optional[str] = field(default=None, metadata=config(field_name="address"))
     port: Optional[int] = field(default=None, metadata=config(field_name="port"))
-    credentials: Optional[str] = field(
+    credentials: Optional[Any] = field(
         default=None, metadata=config(field_name="credentials")
     )
     validity: Optional[ValidityPeriod] = field(
         default=None, metadata=config(field_name="validity")
     )
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 from enum import Enum
 
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 
 
+class HashType(str, Enum):
+    """HashType."""
+
+    SHA1 = "SHA1"
+    SHA256 = "SHA256"
+    SHA512 = "SHA512"
+
+
 class FetchRequestPathTypeEnum(str, Enum):
     """FetchRequestPathTypeEnum."""
 
     FILE = "FILE"
 
 
 class FetchRequestReasonCodeEnum(str, Enum):
@@ -168,14 +176,23 @@
     rule_id: Optional[str] = field(default=None, metadata=config(field_name="RuleID"))
     success: Optional[bool] = field(default=None, metadata=config(field_name="Success"))
     reason: Optional[str] = field(default=None, metadata=config(field_name="Reason"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class HashAndType:
+    """HashAndType."""
+
+    value: Optional[str] = field(default=None, metadata=config(field_name="Value"))
+    type: Optional[HashType] = field(default=None, metadata=config(field_name="Type"))
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class IsolationExclusionRule:
     """IsolationExclusionRule."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="Name"))
     rule_id: Optional[str] = field(default=None, metadata=config(field_name="RuleID"))
     create_time: Optional[str] = field(
         default=None, metadata=config(field_name="CreateTime")
@@ -189,32 +206,14 @@
     )
     user_id: Optional[str] = field(default=None, metadata=config(field_name="UserID"))
     user: Optional[UserInfo] = field(default=None, metadata=config(field_name="User"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class FetchRequestInput:
-    """FetchRequestInput."""
-
-    endpoint_id: Optional[str] = field(
-        default=None, metadata=config(field_name="endpointID")
-    )
-    reason: Optional[str] = field(default=None, metadata=config(field_name="reason"))
-    path: Optional[str] = field(default=None, metadata=config(field_name="path"))
-    path_type: Optional[FetchRequestPathTypeEnum] = field(
-        default=None, metadata=config(field_name="pathType")
-    )
-    reason_code: Optional[FetchRequestReasonCodeEnum] = field(
-        default=None, metadata=config(field_name="reasonCode")
-    )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
 class HistoryEntry:
     """HistoryEntry."""
 
     command: Optional[str] = field(default=None, metadata=config(field_name="Command"))
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="UpdatedAt")
     )
@@ -245,7 +244,28 @@
 
     history: Optional[List[HistoryEntry]] = field(
         default=None, metadata=config(field_name="history")
     )
     partial_page_info: Optional[HistoryPartialPageInfo] = field(
         default=None, metadata=config(field_name="partialPageInfo")
     )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class FetchRequestInput:
+    """FetchRequestInput."""
+
+    endpoint_id: Optional[str] = field(
+        default=None, metadata=config(field_name="endpointID")
+    )
+    reason: Optional[str] = field(default=None, metadata=config(field_name="reason"))
+    path: Optional[str] = field(default=None, metadata=config(field_name="path"))
+    path_type: Optional[FetchRequestPathTypeEnum] = field(
+        default=None, metadata=config(field_name="pathType")
+    )
+    reason_code: Optional[FetchRequestReasonCodeEnum] = field(
+        default=None, metadata=config(field_name="reasonCode")
+    )
+    hash_and_type: Optional[HashAndType] = field(
+        default=None, metadata=config(field_name="hashAndType")
+    )
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     query: Optional[str] = field(default=None, metadata=config(field_name="query"))
     limit: Optional[int] = field(default=None, metadata=config(field_name="limit"))
     offset: Optional[int] = field(default=None, metadata=config(field_name="offset"))
     search_id: Optional[str] = field(
         default=None, metadata=config(field_name="search_id")
     )
+    with_event_data: Optional[bool] = field(
+        default=None, metadata=config(field_name="with_event_data")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AsynchronousEventsSearchPrepInput:
     """AsynchronousEventsSearchPrepInput."""
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,22 +142,25 @@
             },
             output=build_output_string(Notification),
         )
         if result.get(endpoint) is not None:
             return Notification.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation readNotification")
 
-    def bulk_read_notification(self, ids: List[str]) -> List[Notification]:
+    def bulk_read_notification(
+        self, ids: List[str], mark_all_as_read: Optional[bool] = None
+    ) -> List[Notification]:
         """Marks a list of notifications as read."""
         endpoint = "bulkReadNotification"
 
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "ids": prepare_input(ids),
+                "mark_all_as_read": prepare_input(mark_all_as_read),
             },
             output=build_output_string(Notification),
         )
         if result.get(endpoint) is not None:
             return Notification.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -279,7 +279,25 @@
                 "tenantUpdate": prepare_input(tenant_update),
             },
             output=build_output_string(Tenant),
         )
         if result.get(endpoint) is not None:
             return Tenant.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation updateTenant")
+
+    def change_tenant_hierarchy(
+        self, tenant_id: str, new_partner_tenant_id: str
+    ) -> Tenant:
+        """Allows changing the tenant's parent (tenant partner hierarchy)."""
+        endpoint = "changeTenantHierarchy"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={
+                "tenantID": prepare_input(tenant_id),
+                "newPartnerTenantID": prepare_input(new_partner_tenant_id),
+            },
+            output=build_output_string(Tenant),
+        )
+        if result.get(endpoint) is not None:
+            return Tenant.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation changeTenantHierarchy")
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dataclasses_json import dataclass_json, config
 
 
 class AuthzObject(str, Enum):
     """AuthzObject."""
 
     TENANT = "Tenant"
+    TENANT_HIERARCHY = "TenantHierarchy"
     ENTERPRISE_SSO_CONNECTION = "EnterpriseSSOConnection"
 
 
 class AuthzAction(str, Enum):
     """AuthzAction."""
 
     UPDATE = "Update"
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,20 @@
     )
     created_at: Optional[str] = field(
         default=None, metadata=config(field_name="created_at")
     )
     updated_at: Optional[str] = field(
         default=None, metadata=config(field_name="updated_at")
     )
+    created_by: Optional[str] = field(
+        default=None, metadata=config(field_name="created_by")
+    )
+    updated_by: Optional[str] = field(
+        default=None, metadata=config(field_name="updated_by")
+    )
     allowed_environments: Optional[List[str]] = field(
         default=None, metadata=config(field_name="allowed_environments")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a7/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements-dev.txt
+requirements-test.txt
+requirements.txt
 setup.py
 taegis_sdk_python/__init__.py
 taegis_sdk_python/_consts.py
 taegis_sdk_python/_version.py
 taegis_sdk_python/authentication.py
 taegis_sdk_python/config.py
 taegis_sdk_python/errors.py
@@ -67,14 +71,19 @@
 taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
 taegis_sdk_python/services/endpoint_command_manager/types.py
 taegis_sdk_python/services/endpoint_management_service/__init__.py
 taegis_sdk_python/services/endpoint_management_service/mutations.py
 taegis_sdk_python/services/endpoint_management_service/queries.py
 taegis_sdk_python/services/endpoint_management_service/subscriptions.py
 taegis_sdk_python/services/endpoint_management_service/types.py
+taegis_sdk_python/services/entity_profile/__init__.py
+taegis_sdk_python/services/entity_profile/mutations.py
+taegis_sdk_python/services/entity_profile/queries.py
+taegis_sdk_python/services/entity_profile/subscriptions.py
+taegis_sdk_python/services/entity_profile/types.py
 taegis_sdk_python/services/event_search/__init__.py
 taegis_sdk_python/services/event_search/mutations.py
 taegis_sdk_python/services/event_search/queries.py
 taegis_sdk_python/services/event_search/subscriptions.py
 taegis_sdk_python/services/event_search/types.py
 taegis_sdk_python/services/events/__init__.py
 taegis_sdk_python/services/events/mutations.py
```

