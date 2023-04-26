# Comparing `tmp/google-cloud-discoveryengine-0.4.1.tar.gz` & `tmp/google-cloud-discoveryengine-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.4.1.tar", last modified: Mon Mar 27 14:58:36 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.5.0.tar", last modified: Tue Apr 25 18:08:22 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.4.1.tar` & `google-cloud-discoveryengine-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,118 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.980013 google-cloud-discoveryengine-0.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-03-27 14:58:36.980013 google-cloud-discoveryengine-0.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.964011 google-cloud-discoveryengine-0.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.964011 google-cloud-discoveryengine-0.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.968011 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     3566 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.968011 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     2882 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     5224 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.968011 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.968011 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42757 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    53226 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.968011 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9576 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20553 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20965 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    54046 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.972012 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.972012 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22701 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.972012 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.972012 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40240 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.976012 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2196 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3826 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     3540 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9433 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    17303 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003    10596 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003    27197 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.976012 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3647 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:36.000000 google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-27 14:58:36.980013 google-cloud-discoveryengine-0.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.976012 google-cloud-discoveryengine-0.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.976012 google-cloud-discoveryengine-0.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.976012 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:36.980013 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   187646 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   119713 2023-03-27 14:55:35.000000 google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.897393 google-cloud-discoveryengine-0.5.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.897393 google-cloud-discoveryengine-0.5.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5454 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4164 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8894 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22544 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42805 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    53274 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9576 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20553 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20965 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    54046 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17422 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22701 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38222 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    48576 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17633 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22431 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27473 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40240 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2995 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5269 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4646 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6373 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    18586 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    35635 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27269 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6123 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   188394 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168594 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93887 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119713 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.4.1/LICENSE` & `google-cloud-discoveryengine-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/MANIFEST.in` & `google-cloud-discoveryengine-0.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/PKG-INFO` & `google-cloud-discoveryengine-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.4.1
+Version: 0.5.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.4.1/README.rst` & `google-cloud-discoveryengine-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,108 +9,134 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.discoveryengine import gapic_version as package_version
+from google.cloud.discoveryengine_v1beta import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.discoveryengine_v1beta.services.document_service.async_client import (
-    DocumentServiceAsyncClient,
+from .services.completion_service import (
+    CompletionServiceAsyncClient,
+    CompletionServiceClient,
 )
-from google.cloud.discoveryengine_v1beta.services.document_service.client import (
-    DocumentServiceClient,
-)
-from google.cloud.discoveryengine_v1beta.services.recommendation_service.async_client import (
+from .services.document_service import DocumentServiceAsyncClient, DocumentServiceClient
+from .services.recommendation_service import (
     RecommendationServiceAsyncClient,
-)
-from google.cloud.discoveryengine_v1beta.services.recommendation_service.client import (
     RecommendationServiceClient,
 )
-from google.cloud.discoveryengine_v1beta.services.user_event_service.async_client import (
+from .services.schema_service import SchemaServiceAsyncClient, SchemaServiceClient
+from .services.search_service import SearchServiceAsyncClient, SearchServiceClient
+from .services.user_event_service import (
     UserEventServiceAsyncClient,
-)
-from google.cloud.discoveryengine_v1beta.services.user_event_service.client import (
     UserEventServiceClient,
 )
-from google.cloud.discoveryengine_v1beta.types.common import CustomAttribute, UserInfo
-from google.cloud.discoveryengine_v1beta.types.document import Document
-from google.cloud.discoveryengine_v1beta.types.document_service import (
+from .types.common import CustomAttribute, Interval, UserInfo
+from .types.completion_service import CompleteQueryRequest, CompleteQueryResponse
+from .types.document import Document
+from .types.document_service import (
     CreateDocumentRequest,
     DeleteDocumentRequest,
     GetDocumentRequest,
     ListDocumentsRequest,
     ListDocumentsResponse,
     UpdateDocumentRequest,
 )
-from google.cloud.discoveryengine_v1beta.types.import_config import (
+from .types.import_config import (
     BigQuerySource,
     GcsSource,
     ImportDocumentsMetadata,
     ImportDocumentsRequest,
     ImportDocumentsResponse,
     ImportErrorConfig,
     ImportUserEventsMetadata,
     ImportUserEventsRequest,
     ImportUserEventsResponse,
 )
-from google.cloud.discoveryengine_v1beta.types.recommendation_service import (
-    RecommendRequest,
-    RecommendResponse,
+from .types.recommendation_service import RecommendRequest, RecommendResponse
+from .types.schema import Schema
+from .types.schema_service import (
+    CreateSchemaMetadata,
+    CreateSchemaRequest,
+    DeleteSchemaMetadata,
+    DeleteSchemaRequest,
+    GetSchemaRequest,
+    ListSchemasRequest,
+    ListSchemasResponse,
+    UpdateSchemaMetadata,
+    UpdateSchemaRequest,
 )
-from google.cloud.discoveryengine_v1beta.types.user_event import (
+from .types.search_service import SearchRequest, SearchResponse
+from .types.user_event import (
     CompletionInfo,
     DocumentInfo,
     MediaInfo,
     PageInfo,
     PanelInfo,
     SearchInfo,
     TransactionInfo,
     UserEvent,
 )
-from google.cloud.discoveryengine_v1beta.types.user_event_service import (
-    CollectUserEventRequest,
-    WriteUserEventRequest,
-)
+from .types.user_event_service import CollectUserEventRequest, WriteUserEventRequest
 
 __all__ = (
-    "DocumentServiceClient",
+    "CompletionServiceAsyncClient",
     "DocumentServiceAsyncClient",
-    "RecommendationServiceClient",
     "RecommendationServiceAsyncClient",
-    "UserEventServiceClient",
+    "SchemaServiceAsyncClient",
+    "SearchServiceAsyncClient",
     "UserEventServiceAsyncClient",
-    "CustomAttribute",
-    "UserInfo",
-    "Document",
+    "BigQuerySource",
+    "CollectUserEventRequest",
+    "CompleteQueryRequest",
+    "CompleteQueryResponse",
+    "CompletionInfo",
+    "CompletionServiceClient",
     "CreateDocumentRequest",
+    "CreateSchemaMetadata",
+    "CreateSchemaRequest",
+    "CustomAttribute",
     "DeleteDocumentRequest",
-    "GetDocumentRequest",
-    "ListDocumentsRequest",
-    "ListDocumentsResponse",
-    "UpdateDocumentRequest",
-    "BigQuerySource",
+    "DeleteSchemaMetadata",
+    "DeleteSchemaRequest",
+    "Document",
+    "DocumentInfo",
+    "DocumentServiceClient",
     "GcsSource",
+    "GetDocumentRequest",
+    "GetSchemaRequest",
     "ImportDocumentsMetadata",
     "ImportDocumentsRequest",
     "ImportDocumentsResponse",
     "ImportErrorConfig",
     "ImportUserEventsMetadata",
     "ImportUserEventsRequest",
     "ImportUserEventsResponse",
-    "RecommendRequest",
-    "RecommendResponse",
-    "CompletionInfo",
-    "DocumentInfo",
+    "Interval",
+    "ListDocumentsRequest",
+    "ListDocumentsResponse",
+    "ListSchemasRequest",
+    "ListSchemasResponse",
     "MediaInfo",
     "PageInfo",
     "PanelInfo",
+    "RecommendRequest",
+    "RecommendResponse",
+    "RecommendationServiceClient",
+    "Schema",
+    "SchemaServiceClient",
     "SearchInfo",
+    "SearchRequest",
+    "SearchResponse",
+    "SearchServiceClient",
     "TransactionInfo",
+    "UpdateDocumentRequest",
+    "UpdateSchemaMetadata",
+    "UpdateSchemaRequest",
     "UserEvent",
-    "CollectUserEventRequest",
+    "UserEventServiceClient",
+    "UserInfo",
     "WriteUserEventRequest",
 )
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.4.1"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'services'": "{'CompletionService': OrderedDict([('clients', OrderedDict([('grpc', "*

 * *               "OrderedDict([('libraryClient', 'CompletionServiceClient'), ('rpcs', "*

 * *               "OrderedDict([('CompleteQuery', OrderedDict([('methods', "*

 * *               "['complete_query'])]))]))])), ('grpc-async', OrderedDict([('libraryClient', "*

 * *               "'CompletionServiceAsyncClient'), ('rpcs', OrderedDict([('CompleteQuery', "*

 * *               "OrderedDict([('methods', ['complete_query'])]))]))])), ('rest',  […]*

```diff
@@ -1,14 +1,48 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
     "libraryPackage": "google.cloud.discoveryengine_v1beta",
     "protoPackage": "google.cloud.discoveryengine.v1beta",
     "schema": "1.0",
     "services": {
+        "CompletionService": {
+            "clients": {
+                "grpc": {
+                    "libraryClient": "CompletionServiceClient",
+                    "rpcs": {
+                        "CompleteQuery": {
+                            "methods": [
+                                "complete_query"
+                            ]
+                        }
+                    }
+                },
+                "grpc-async": {
+                    "libraryClient": "CompletionServiceAsyncClient",
+                    "rpcs": {
+                        "CompleteQuery": {
+                            "methods": [
+                                "complete_query"
+                            ]
+                        }
+                    }
+                },
+                "rest": {
+                    "libraryClient": "CompletionServiceClient",
+                    "rpcs": {
+                        "CompleteQuery": {
+                            "methods": [
+                                "complete_query"
+                            ]
+                        }
+                    }
+                }
+            }
+        },
         "DocumentService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "DocumentServiceClient",
                     "rpcs": {
                         "CreateDocument": {
                             "methods": [
@@ -144,14 +178,142 @@
                                 "recommend"
                             ]
                         }
                     }
                 }
             }
         },
+        "SchemaService": {
+            "clients": {
+                "grpc": {
+                    "libraryClient": "SchemaServiceClient",
+                    "rpcs": {
+                        "CreateSchema": {
+                            "methods": [
+                                "create_schema"
+                            ]
+                        },
+                        "DeleteSchema": {
+                            "methods": [
+                                "delete_schema"
+                            ]
+                        },
+                        "GetSchema": {
+                            "methods": [
+                                "get_schema"
+                            ]
+                        },
+                        "ListSchemas": {
+                            "methods": [
+                                "list_schemas"
+                            ]
+                        },
+                        "UpdateSchema": {
+                            "methods": [
+                                "update_schema"
+                            ]
+                        }
+                    }
+                },
+                "grpc-async": {
+                    "libraryClient": "SchemaServiceAsyncClient",
+                    "rpcs": {
+                        "CreateSchema": {
+                            "methods": [
+                                "create_schema"
+                            ]
+                        },
+                        "DeleteSchema": {
+                            "methods": [
+                                "delete_schema"
+                            ]
+                        },
+                        "GetSchema": {
+                            "methods": [
+                                "get_schema"
+                            ]
+                        },
+                        "ListSchemas": {
+                            "methods": [
+                                "list_schemas"
+                            ]
+                        },
+                        "UpdateSchema": {
+                            "methods": [
+                                "update_schema"
+                            ]
+                        }
+                    }
+                },
+                "rest": {
+                    "libraryClient": "SchemaServiceClient",
+                    "rpcs": {
+                        "CreateSchema": {
+                            "methods": [
+                                "create_schema"
+                            ]
+                        },
+                        "DeleteSchema": {
+                            "methods": [
+                                "delete_schema"
+                            ]
+                        },
+                        "GetSchema": {
+                            "methods": [
+                                "get_schema"
+                            ]
+                        },
+                        "ListSchemas": {
+                            "methods": [
+                                "list_schemas"
+                            ]
+                        },
+                        "UpdateSchema": {
+                            "methods": [
+                                "update_schema"
+                            ]
+                        }
+                    }
+                }
+            }
+        },
+        "SearchService": {
+            "clients": {
+                "grpc": {
+                    "libraryClient": "SearchServiceClient",
+                    "rpcs": {
+                        "Search": {
+                            "methods": [
+                                "search"
+                            ]
+                        }
+                    }
+                },
+                "grpc-async": {
+                    "libraryClient": "SearchServiceAsyncClient",
+                    "rpcs": {
+                        "Search": {
+                            "methods": [
+                                "search"
+                            ]
+                        }
+                    }
+                },
+                "rest": {
+                    "libraryClient": "SearchServiceClient",
+                    "rpcs": {
+                        "Search": {
+                            "methods": [
+                                "search"
+                            ]
+                        }
+                    }
+                }
+            }
+        },
         "UserEventService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "UserEventServiceClient",
                     "rpcs": {
                         "CollectUserEvent": {
                             "methods": [
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.4.1"  # {x-release-please-version}
+__version__ = "0.5.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,19 +273,19 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
                 If the caller does not have permission to access the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 If the requested
                 [Document][google.cloud.discoveryengine.v1beta.Document]
-                does not exist, a NOT_FOUND error is returned.
+                does not exist, a ``NOT_FOUND`` error is returned.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -389,16 +389,16 @@
                 Required. The parent branch resource name, such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}``.
                 Use ``default_branch`` as the branch ID, to list
                 documents under the default branch.
 
                 If the caller does not have permission to list
                 [Documents][]s under this branch, regardless of whether
-                or not this branch exists, a PERMISSION_DENIED error is
-                returned.
+                or not this branch exists, a ``PERMISSION_DENIED`` error
+                is returned.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -532,26 +532,26 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 which will become the final component of the
                 [Document.name][google.cloud.discoveryengine.v1beta.Document.name].
 
                 If the caller does not have permission to create the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 This field must be unique among all
                 [Document][google.cloud.discoveryengine.v1beta.Document]s
                 with the same
                 [parent][google.cloud.discoveryengine.v1beta.CreateDocumentRequest.parent].
-                Otherwise, an ALREADY_EXISTS error is returned.
+                Otherwise, an ``ALREADY_EXISTS`` error is returned.
 
                 This field must conform to
                 `RFC-1034 <https://tools.ietf.org/html/rfc1034>`__
                 standard with a length limit of 63 characters.
-                Otherwise, an INVALID_ARGUMENT error is returned.
+                Otherwise, an ``INVALID_ARGUMENT`` error is returned.
 
                 This corresponds to the ``document_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -740,19 +740,20 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
                 If the caller does not have permission to delete the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 If the
                 [Document][google.cloud.discoveryengine.v1beta.Document]
-                to delete does not exist, a NOT_FOUND error is returned.
+                to delete does not exist, a ``NOT_FOUND`` error is
+                returned.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,19 +528,19 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
                 If the caller does not have permission to access the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 If the requested
                 [Document][google.cloud.discoveryengine.v1beta.Document]
-                does not exist, a NOT_FOUND error is returned.
+                does not exist, a ``NOT_FOUND`` error is returned.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -644,16 +644,16 @@
                 Required. The parent branch resource name, such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}``.
                 Use ``default_branch`` as the branch ID, to list
                 documents under the default branch.
 
                 If the caller does not have permission to list
                 [Documents][]s under this branch, regardless of whether
-                or not this branch exists, a PERMISSION_DENIED error is
-                returned.
+                or not this branch exists, a ``PERMISSION_DENIED`` error
+                is returned.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -787,26 +787,26 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 which will become the final component of the
                 [Document.name][google.cloud.discoveryengine.v1beta.Document.name].
 
                 If the caller does not have permission to create the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 This field must be unique among all
                 [Document][google.cloud.discoveryengine.v1beta.Document]s
                 with the same
                 [parent][google.cloud.discoveryengine.v1beta.CreateDocumentRequest.parent].
-                Otherwise, an ALREADY_EXISTS error is returned.
+                Otherwise, an ``ALREADY_EXISTS`` error is returned.
 
                 This field must conform to
                 `RFC-1034 <https://tools.ietf.org/html/rfc1034>`__
                 standard with a length limit of 63 characters.
-                Otherwise, an INVALID_ARGUMENT error is returned.
+                Otherwise, an ``INVALID_ARGUMENT`` error is returned.
 
                 This corresponds to the ``document_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -996,19 +996,20 @@
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 such as
                 ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
                 If the caller does not have permission to delete the
                 [Document][google.cloud.discoveryengine.v1beta.Document],
                 regardless of whether or not it exists, a
-                PERMISSION_DENIED error is returned.
+                ``PERMISSION_DENIED`` error is returned.
 
                 If the
                 [Document][google.cloud.discoveryengine.v1beta.Document]
-                to delete does not exist, a NOT_FOUND error is returned.
+                to delete does not exist, a ``NOT_FOUND`` error is
+                returned.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,96 +13,97 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
-from google.protobuf import struct_pb2  # type: ignore
 import proto  # type: ignore
 
+from google.cloud.discoveryengine_v1beta.types import user_event as gcd_user_event
+
 __protobuf__ = proto.module(
     package="google.cloud.discoveryengine.v1beta",
     manifest={
-        "Document",
+        "WriteUserEventRequest",
+        "CollectUserEventRequest",
     },
 )
 
 
-class Document(proto.Message):
-    r"""Document captures all raw metadata information of items to be
-    recommended or searched.
-
-    This message has `oneof`_ fields (mutually exclusive fields).
-    For each oneof, at most one member field can be set at the same time.
-    Setting any member of the oneof automatically clears all other
-    members.
+class WriteUserEventRequest(proto.Message):
+    r"""Request message for WriteUserEvent method.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        struct_data (google.protobuf.struct_pb2.Struct):
-            The structured JSON data for the document. It should conform
-            to the registered [schema][] or an INVALID_ARGUMENT error is
-            thrown.
-
-            This field is a member of `oneof`_ ``data``.
-        json_data (str):
-            The JSON string representation of the document. It should
-            conform to the registered [schema][] or an INVALID_ARGUMENT
-            error is thrown.
-
-            This field is a member of `oneof`_ ``data``.
-        name (str):
-            Immutable. The full resource name of the document. Format:
-            ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document_id}``.
-
-            This field must be a UTF-8 encoded string with a length
-            limit of 1024 characters.
-        id (str):
-            Immutable. The identifier of the document.
-
-            Id should conform to
-            `RFC-1034 <https://tools.ietf.org/html/rfc1034>`__ standard
-            with a length limit of 63 characters.
-        schema_id (str):
-            The identifier of the schema located in the
-            same data store.
-        parent_document_id (str):
-            The identifier of the parent document. Currently supports at
-            most two level document hierarchy.
-
-            Id should conform to
-            `RFC-1034 <https://tools.ietf.org/html/rfc1034>`__ standard
-            with a length limit of 63 characters.
+        parent (str):
+            Required. The parent DataStore resource name, such as
+            ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}``.
+        user_event (google.cloud.discoveryengine_v1beta.types.UserEvent):
+            Required. User event to write.
+
+            This field is a member of `oneof`_ ``_user_event``.
     """
 
-    struct_data: struct_pb2.Struct = proto.Field(
-        proto.MESSAGE,
-        number=4,
-        oneof="data",
-        message=struct_pb2.Struct,
-    )
-    json_data: str = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
-        number=5,
-        oneof="data",
+        number=1,
     )
-    name: str = proto.Field(
+    user_event: gcd_user_event.UserEvent = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        optional=True,
+        message=gcd_user_event.UserEvent,
+    )
+
+
+class CollectUserEventRequest(proto.Message):
+    r"""Request message for CollectUserEvent method.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        parent (str):
+            Required. The parent DataStore resource name, such as
+            ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}``.
+        user_event (str):
+            Required. URL encoded UserEvent proto with a
+            length limit of 2,000,000 characters.
+        uri (str):
+            The URL including cgi-parameters but
+            excluding the hash fragment with a length limit
+            of 5,000 characters. This is often more useful
+            than the referer URL, because many browsers only
+            send the domain for 3rd party requests.
+
+            This field is a member of `oneof`_ ``_uri``.
+        ets (int):
+            The event timestamp in milliseconds. This
+            prevents browser caching of otherwise identical
+            get requests. The name is abbreviated to reduce
+            the payload bytes.
+
+            This field is a member of `oneof`_ ``_ets``.
+    """
+
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    id: str = proto.Field(
+    user_event: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    schema_id: str = proto.Field(
+    uri: str = proto.Field(
         proto.STRING,
         number=3,
+        optional=True,
     )
-    parent_document_id: str = proto.Field(
-        proto.STRING,
-        number=7,
+    ets: int = proto.Field(
+        proto.INT64,
+        number=4,
+        optional=True,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,20 +44,20 @@
             Required. Full resource name of
             [Document][google.cloud.discoveryengine.v1beta.Document],
             such as
             ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
             If the caller does not have permission to access the
             [Document][google.cloud.discoveryengine.v1beta.Document],
-            regardless of whether or not it exists, a PERMISSION_DENIED
-            error is returned.
+            regardless of whether or not it exists, a
+            ``PERMISSION_DENIED`` error is returned.
 
             If the requested
             [Document][google.cloud.discoveryengine.v1beta.Document]
-            does not exist, a NOT_FOUND error is returned.
+            does not exist, a ``NOT_FOUND`` error is returned.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
@@ -72,35 +72,35 @@
             Required. The parent branch resource name, such as
             ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}``.
             Use ``default_branch`` as the branch ID, to list documents
             under the default branch.
 
             If the caller does not have permission to list
             [Documents][]s under this branch, regardless of whether or
-            not this branch exists, a PERMISSION_DENIED error is
+            not this branch exists, a ``PERMISSION_DENIED`` error is
             returned.
         page_size (int):
             Maximum number of
             [Document][google.cloud.discoveryengine.v1beta.Document]s to
             return. If unspecified, defaults to 100. The maximum allowed
             value is 1000. Values above 1000 will be coerced to 1000.
 
-            If this field is negative, an INVALID_ARGUMENT error is
+            If this field is negative, an ``INVALID_ARGUMENT`` error is
             returned.
         page_token (str):
             A page token
             [ListDocumentsResponse.next_page_token][google.cloud.discoveryengine.v1beta.ListDocumentsResponse.next_page_token],
             received from a previous
             [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments]
             call. Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to
             [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments]
             must match the call that provided the page token. Otherwise,
-            an INVALID_ARGUMENT error is returned.
+            an ``INVALID_ARGUMENT`` error is returned.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
@@ -161,27 +161,27 @@
             Required. The ID to use for the
             [Document][google.cloud.discoveryengine.v1beta.Document],
             which will become the final component of the
             [Document.name][google.cloud.discoveryengine.v1beta.Document.name].
 
             If the caller does not have permission to create the
             [Document][google.cloud.discoveryengine.v1beta.Document],
-            regardless of whether or not it exists, a PERMISSION_DENIED
-            error is returned.
+            regardless of whether or not it exists, a
+            ``PERMISSION_DENIED`` error is returned.
 
             This field must be unique among all
             [Document][google.cloud.discoveryengine.v1beta.Document]s
             with the same
             [parent][google.cloud.discoveryengine.v1beta.CreateDocumentRequest.parent].
-            Otherwise, an ALREADY_EXISTS error is returned.
+            Otherwise, an ``ALREADY_EXISTS`` error is returned.
 
             This field must conform to
             `RFC-1034 <https://tools.ietf.org/html/rfc1034>`__ standard
             with a length limit of 63 characters. Otherwise, an
-            INVALID_ARGUMENT error is returned.
+            ``INVALID_ARGUMENT`` error is returned.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     document: gcd_document.Document = proto.Field(
@@ -202,22 +202,22 @@
 
     Attributes:
         document (google.cloud.discoveryengine_v1beta.types.Document):
             Required. The document to update/create.
 
             If the caller does not have permission to update the
             [Document][google.cloud.discoveryengine.v1beta.Document],
-            regardless of whether or not it exists, a PERMISSION_DENIED
-            error is returned.
+            regardless of whether or not it exists, a
+            ``PERMISSION_DENIED`` error is returned.
 
             If the
             [Document][google.cloud.discoveryengine.v1beta.Document] to
             update does not exist and
             [allow_missing][google.cloud.discoveryengine.v1beta.UpdateDocumentRequest.allow_missing]
-            is not set, a NOT_FOUND error is returned.
+            is not set, a ``NOT_FOUND`` error is returned.
         allow_missing (bool):
             If set to true, and the
             [Document][google.cloud.discoveryengine.v1beta.Document] is
             not found, a new
             [Document][google.cloud.discoveryengine.v1beta.Document]
             will be created.
     """
@@ -243,20 +243,20 @@
             Required. Full resource name of
             [Document][google.cloud.discoveryengine.v1beta.Document],
             such as
             ``projects/{project}/locations/{location}/collections/{collection}/dataStores/{data_store}/branches/{branch}/documents/{document}``.
 
             If the caller does not have permission to delete the
             [Document][google.cloud.discoveryengine.v1beta.Document],
-            regardless of whether or not it exists, a PERMISSION_DENIED
-            error is returned.
+            regardless of whether or not it exists, a
+            ``PERMISSION_DENIED`` error is returned.
 
             If the
             [Document][google.cloud.discoveryengine.v1beta.Document] to
-            delete does not exist, a NOT_FOUND error is returned.
+            delete does not exist, a ``NOT_FOUND`` error is returned.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,25 +45,37 @@
 
     Attributes:
         input_uris (MutableSequence[str]):
             Required. Cloud Storage URIs to input files. URI can be up
             to 2000 characters long. URIs can match the full object path
             (for example, ``gs://bucket/directory/object.json``) or a
             pattern matching one or more files, such as
-            ``gs://bucket/directory/*.json``. A request can contain at
-            most 100 files, and each file can be up to 2 GB.
+            ``gs://bucket/directory/*.json``.
+
+            A request can contain at most 100 files (or 100,000 files if
+            ``data_schema`` is ``content``). Each file can be up to 2 GB
+            (or 100 MB if ``data_schema`` is ``content``).
         data_schema (str):
             The schema to use when parsing the data from the source.
 
             Supported values for document imports:
 
             -  ``document`` (default): One JSON
                [Document][google.cloud.discoveryengine.v1beta.Document]
                per line. Each document must have a valid
                [Document.id][google.cloud.discoveryengine.v1beta.Document.id].
+            -  ``content``: Unstructured data (e.g. PDF, HTML). Each
+               file matched by ``input_uris`` will become a document,
+               with the ID set to the first 128 bits of SHA256(URI)
+               encoded as a hex string.
+            -  ``custom``: One custom data JSON per row in arbitrary
+               format that conforms the defined
+               [Schema][google.cloud.discoveryengine.v1beta.Schema] of
+               the data store. This can only be used by the GENERIC Data
+               Store vertical.
 
             Supported values for user even imports:
 
             -  ``user_event`` (default): One JSON
                [UserEvent][google.cloud.discoveryengine.v1beta.UserEvent]
                per line.
     """
@@ -106,24 +118,35 @@
             the import with a length limit of 2,000
             characters. Can be specified if one wants to
             have the BigQuery export to a specific Cloud
             Storage directory.
         data_schema (str):
             The schema to use when parsing the data from the source.
 
-            Supported values for imports:
+            Supported values for user event imports:
 
-            -  ``user_event`` (default): One JSON
+            -  ``user_event`` (default): One
                [UserEvent][google.cloud.discoveryengine.v1beta.UserEvent]
-               per line.
+               per row.
 
-            -  ``document`` (default): One JSON
+            Supported values for document imports:
+
+            -  ``document`` (default): One
                [Document][google.cloud.discoveryengine.v1beta.Document]
-               per line. Each document must have a valid
-               [document.id][].
+               format per row. Each document must have a valid
+               [Document.id][google.cloud.discoveryengine.v1beta.Document.id]
+               and one of
+               [Document.json_data][google.cloud.discoveryengine.v1beta.Document.json_data]
+               or
+               [Document.struct_data][google.cloud.discoveryengine.v1beta.Document.struct_data].
+            -  ``custom``: One custom data per row in arbitrary format
+               that conforms the defined
+               [Schema][google.cloud.discoveryengine.v1beta.Schema] of
+               the data store. This can only be used by the GENERIC Data
+               Store vertical.
     """
 
     partition_date: date_pb2.Date = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="partition",
         message=date_pb2.Date,
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class RecommendRequest(proto.Message):
     r"""Request message for Recommend method.
 
     Attributes:
         serving_config (str):
             Required. Full resource name of the format:
-            projects/\ */locations/global/collections/*/dataStores/*/servingConfigs/*
+            ``projects/*/locations/global/collections/*/dataStores/*/servingConfigs/*``
 
             Before you can request recommendations from your model, you
             must create at least one serving config for it.
         user_event (google.cloud.discoveryengine_v1beta.types.UserEvent):
             Required. Context about the user, what they are looking at
             and what action they took to trigger the Recommend request.
             Note that this user event detail won't be ingested to
@@ -70,29 +70,28 @@
         filter (str):
             Filter for restricting recommendation results with a length
             limit of 5,000 characters. Currently, only filter
             expressions on the ``filter_tags`` attribute is supported.
 
             Examples:
 
-            -  (filter_tags: ANY("Red", "Blue") OR filter_tags:
-               ANY("Hot", "Cold"))
-            -  (filter_tags: ANY("Red", "Blue")) AND NOT (filter_tags:
-               ANY("Green"))
+            -  ``(filter_tags: ANY("Red", "Blue") OR filter_tags: ANY("Hot", "Cold"))``
+            -  ``(filter_tags: ANY("Red", "Blue")) AND NOT (filter_tags: ANY("Green"))``
 
             If your filter blocks all results, the API will return
             generic (unfiltered) popular Documents. If you only want
             results strictly matching the filters, set
             ``strictFiltering`` to True in
             [RecommendRequest.params][google.cloud.discoveryengine.v1beta.RecommendRequest.params]
             to receive empty results instead.
 
-            Note that the API will never return Documents with
-            storageStatus of "EXPIRED" or "DELETED" regardless of filter
-            choices.
+            Note that the API will never return
+            [Document][google.cloud.discoveryengine.v1beta.Document]s
+            with ``storageStatus`` of ``EXPIRED`` or ``DELETED``
+            regardless of filter choices.
         validate_only (bool):
             Use validate only mode for this
             recommendation query. If set to true, a fake
             model will be used that returns arbitrary
             Document IDs. Note that the validate only mode
             should only be used for testing the API, or if
             the model is not ready.
@@ -100,34 +99,34 @@
             Additional domain specific parameters for the
             recommendations.
 
             Allowed values:
 
             -  ``returnDocument``: Boolean. If set to true, the
                associated Document object will be returned in
-               [RecommendResponse.results.document][RecommendationResult.document].
+               [RecommendResponse.RecommendationResult.document][google.cloud.discoveryengine.v1beta.RecommendResponse.RecommendationResult.document].
             -  ``returnScore``: Boolean. If set to true, the
                recommendation 'score' corresponding to each returned
                Document will be set in
-               [RecommendResponse.results.metadata][RecommendationResult.metadata].
+               [RecommendResponse.RecommendationResult.metadata][google.cloud.discoveryengine.v1beta.RecommendResponse.RecommendationResult.metadata].
                The given 'score' indicates the probability of a Document
                conversion given the user's context and history.
             -  ``strictFiltering``: Boolean. True by default. If set to
                false, the service will return generic (unfiltered)
                popular Documents instead of empty if your filter blocks
                all recommendation results.
             -  ``diversityLevel``: String. Default empty. If set to be
                non-empty, then it needs to be one of:
 
-               -  'no-diversity'
-               -  'low-diversity'
-               -  'medium-diversity'
-               -  'high-diversity'
-               -  'auto-diversity' This gives request-level control and
-                  adjusts recommendation results based on Document
+               -  ``no-diversity``
+               -  ``low-diversity``
+               -  ``medium-diversity``
+               -  ``high-diversity``
+               -  ``auto-diversity`` This gives request-level control
+                  and adjusts recommendation results based on Document
                   category.
         user_labels (MutableMapping[str, str]):
             The user labels applied to a resource must meet the
             following requirements:
 
             -  Each resource can have multiple labels, up to a maximum
                of 64.
```

### Comparing `google-cloud-discoveryengine-0.4.1/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
             The value must be one of:
 
             -  [PredictResponse.attribution_token][] for events that are
                the result of [PredictionService.Predict][].
             -  [SearchResponse.attribution_token][google.cloud.discoveryengine.v1beta.SearchResponse.attribution_token]
                for events that are the result of
-               [SearchService.Search][].
+               [SearchService.Search][google.cloud.discoveryengine.v1beta.SearchService.Search].
             -  [CompleteQueryResponse.attribution_token][] for events
                that are the result of [SearchService.CompleteQuery][].
 
             This token enables us to accurately attribute page view or
             conversion completion back to the event and the particular
             predict response containing this clicked/purchased product.
             If user clicks on product K in the recommendation results,
@@ -226,28 +226,28 @@
             prediction requests. Custom attribute formatting must be
             consistent between imported events and events provided with
             prediction requests. This lets the Discovery Engine API use
             those custom attributes when training models and serving
             predictions, which helps improve recommendation quality.
 
             This field needs to pass all below criteria, otherwise an
-            INVALID_ARGUMENT error is returned:
+            ``INVALID_ARGUMENT`` error is returned:
 
             -  The key must be a UTF-8 encoded string with a length
                limit of 5,000 characters.
             -  For text attributes, at most 400 values are allowed.
                Empty values are not allowed. Each value must be a UTF-8
                encoded string with a length limit of 256 characters.
             -  For number attributes, at most 400 values are allowed.
 
             For product recommendations, an example of extra user
-            information is traffic_channel, which is how a user arrives
-            at the site. Users can arrive at the site by coming to the
-            site directly, coming through Google search, or in other
-            ways.
+            information is ``traffic_channel``, which is how a user
+            arrives at the site. Users can arrive at the site by coming
+            to the site directly, coming through Google search, or in
+            other ways.
         media_info (google.cloud.discoveryengine_v1beta.types.MediaInfo):
             Media-specific info.
     """
 
     event_type: str = proto.Field(
         proto.STRING,
         number=1,
@@ -601,15 +601,15 @@
     Attributes:
         id (str):
             Required. The Document resource ID.
 
             This field is a member of `oneof`_ ``document_descriptor``.
         name (str):
             Required. The Document resource full name, of the form:
-            projects/{project_id}/locations/{location}/collections/{collection_id}/dataStores/{data_store_id}/branches/{branch_id}/documents/{document_id}
+            ``projects/{project_id}/locations/{location}/collections/{collection_id}/dataStores/{data_store_id}/branches/{branch_id}/documents/{document_id}``
 
             This field is a member of `oneof`_ ``document_descriptor``.
         quantity (int):
             Quantity of the Document associated with the user event.
             Defaults to 1.
 
             For example, this field will be 2 if two quantities of the
@@ -706,15 +706,15 @@
             playback video, then
             [MediaInfo.media_progress_duration.seconds][Duration.seconds]
             should be set to 90.
         media_progress_percentage (float):
             Media progress should be computed using only the
             media_progress_duration relative to the media total length.
 
-            This value must be between [0, 1.0] inclusive.
+            This value must be between ``[0, 1.0]`` inclusive.
 
             If this is not a playback or the progress cannot be computed
             (e.g. ongoing livestream), this field should be unset.
 
             This field is a member of `oneof`_ ``_media_progress_percentage``.
     """
```

### Comparing `google-cloud-discoveryengine-0.4.1/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.4.1
+Version: 0.5.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.4.1/setup.py` & `google-cloud-discoveryengine-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/__init__.py` & `google-cloud-discoveryengine-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2909,15 +2909,21 @@
     }
     request_init["document"] = {
         "struct_data": {"fields": {}},
         "json_data": "json_data_value",
         "name": "name_value",
         "id": "id_value",
         "schema_id": "schema_id_value",
+        "content": {
+            "raw_bytes": b"raw_bytes_blob",
+            "uri": "uri_value",
+            "mime_type": "mime_type_value",
+        },
         "parent_document_id": "parent_document_id_value",
+        "derived_struct_data": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = gcd_document.Document(
@@ -3134,15 +3140,21 @@
     }
     request_init["document"] = {
         "struct_data": {"fields": {}},
         "json_data": "json_data_value",
         "name": "name_value",
         "id": "id_value",
         "schema_id": "schema_id_value",
+        "content": {
+            "raw_bytes": b"raw_bytes_blob",
+            "uri": "uri_value",
+            "mime_type": "mime_type_value",
+        },
         "parent_document_id": "parent_document_id_value",
+        "derived_struct_data": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -3259,15 +3271,21 @@
     }
     request_init["document"] = {
         "struct_data": {"fields": {}},
         "json_data": "json_data_value",
         "name": "projects/sample1/locations/sample2/dataStores/sample3/branches/sample4/documents/sample5",
         "id": "id_value",
         "schema_id": "schema_id_value",
+        "content": {
+            "raw_bytes": b"raw_bytes_blob",
+            "uri": "uri_value",
+            "mime_type": "mime_type_value",
+        },
         "parent_document_id": "parent_document_id_value",
+        "derived_struct_data": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = document.Document(
@@ -3457,15 +3475,21 @@
     }
     request_init["document"] = {
         "struct_data": {"fields": {}},
         "json_data": "json_data_value",
         "name": "projects/sample1/locations/sample2/dataStores/sample3/branches/sample4/documents/sample5",
         "id": "id_value",
         "schema_id": "schema_id_value",
+        "content": {
+            "raw_bytes": b"raw_bytes_blob",
+            "uri": "uri_value",
+            "mime_type": "mime_type_value",
+        },
         "parent_document_id": "parent_document_id_value",
+        "derived_struct_data": {},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
```

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.4.1/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files identical despite different names*

