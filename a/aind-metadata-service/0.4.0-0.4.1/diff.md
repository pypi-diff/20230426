# Comparing `tmp/aind_metadata_service-0.4.0.tar.gz` & `tmp/aind_metadata_service-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.0.tar", last modified: Fri Apr 21 16:41:02 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.1.tar", last modified: Wed Apr 26 17:07:51 2023, max compression
```

## Comparing `aind_metadata_service-0.4.0.tar` & `aind_metadata_service-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.852521 aind_metadata_service-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102957 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/src/aind_metadata_service/sharepoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:41:02.000000 aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.856521 aind_metadata_service-0.4.0/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:41:02.860521 aind_metadata_service-0.4.0/tests/sharepoint/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item7.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item9.json
--rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-21 16:40:44.000000 aind_metadata_service-0.4.0/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 17:07:25.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2019/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/src/aind_metadata_service/sharepoint/nsb2023/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.335894 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:07:51.000000 aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.339894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.331893 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.343894 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:51.347895 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-26 17:07:24.000000 aind_metadata_service-0.4.1/tests/test_response_handle.py
```

### Comparing `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/.github/workflows/ci.yml` & `aind_metadata_service-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/.github/workflows/publish.yml` & `aind_metadata_service-0.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/.gitignore` & `aind_metadata_service-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/Dockerfile` & `aind_metadata_service-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/LICENSE` & `aind_metadata_service-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/PKG-INFO` & `aind_metadata_service-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.0
+Version: 0.4.1
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.0/README.md` & `aind_metadata_service-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/doc_template/Makefile` & `aind_metadata_service-0.4.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/doc_template/make.bat` & `aind_metadata_service-0.4.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.1/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/doc_template/source/conf.py` & `aind_metadata_service-0.4.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/pyproject.toml` & `aind_metadata_service-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.1/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.1/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.1/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.1/src/aind_metadata_service/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,17 +24,21 @@
 labtracks_driver = os.getenv("ODBC_DRIVER")
 labtracks_server = os.getenv("LABTRACKS_SERVER")
 labtracks_port = os.getenv("LABTRACKS_PORT")
 labtracks_db = os.getenv("LABTRACKS_DATABASE")
 labtracks_user = os.getenv("LABTRACKS_USER")
 labtracks_password = os.getenv("LABTRACKS_PASSWORD")
 
-sharepoint_url = os.getenv("SHAREPOINT_URL")
-sharepoint_user = os.getenv("SHAREPOINT_USER")
-sharepoint_password = os.getenv("SHAREPOINT_PASSWORD")
+nsb_sharepoint_url = os.getenv("NSB_SHAREPOINT_URL")
+nsb_sharepoint_list_2019 = os.getenv("NSB_2019_LIST", default="SWR 2019-2022")
+nsb_sharepoint_list_2023 = os.getenv(
+    "NSB_2023_LIST", default="SWR 2023-Present"
+)
+nsb_sharepoint_user = os.getenv("NSB_SHAREPOINT_USER")
+nsb_sharepoint_password = os.getenv("NSB_SHAREPOINT_PASSWORD")
 
 
 @app.get("/subject/{subject_id}")
 async def retrieve_subject(subject_id):
     """
     Retrieves subject from Labtracks server
     """
@@ -52,17 +56,19 @@
 
 @app.get("/procedures/{subject_id}")
 async def retrieve_procedures(subject_id):
     """
     Retrieves procedure info from SharePoint
     """
     sharepoint_client = SharePointClient(
-        site_url=sharepoint_url,
-        client_id=sharepoint_user,
-        client_secret=sharepoint_password,
+        nsb_site_url=nsb_sharepoint_url,
+        nsb_list_title_2019=nsb_sharepoint_list_2019,
+        nsb_list_title_2023=nsb_sharepoint_list_2023,
+        client_id=nsb_sharepoint_user,
+        client_secret=nsb_sharepoint_password,
     )
 
     response = sharepoint_client.get_procedure_info(subject_id=subject_id)
 
     return response
```

### Comparing `aind_metadata_service-0.4.0/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.1/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.0
+Version: 0.4.1
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.0/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.1/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.1/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.1/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item1.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item10.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item11.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item12.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item13.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item14.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item15.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item16.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'Headpost'": "'AI Straight bar'"}*

```diff
@@ -57,15 +57,15 @@
     "FirstInjectionIsoDuration": null,
     "FirstInjectionWeightAfter": null,
     "FirstInjectionWeightBefor": null,
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
-    "Headpost": "AI Straight Bar",
+    "Headpost": "AI Straight bar",
     "HeadpostType": "No Well",
     "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
     "Hemisphere2ndInj": "Left",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
```

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item17.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item2.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 2% similar despite different names*

```diff
@@ -147,182 +147,180 @@
 00000920: 222c 0a20 2022 496e 6a32 4c65 6e67 6874  ",.  "Inj2Lenght
 00000930: 6f66 5469 6d65 223a 206e 756c 6c2c 0a20  ofTime": null,. 
 00000940: 2022 496e 6a31 4375 7272 656e 7422 3a20   "Inj1Current": 
 00000950: 2235 7541 222c 0a20 2022 496e 6a32 4375  "5uA",.  "Inj2Cu
 00000960: 7272 656e 7422 3a20 2235 7541 222c 0a20  rrent": "5uA",. 
 00000970: 2022 496e 6a31 416c 7465 726e 6174 696e   "Inj1Alternatin
 00000980: 6754 696d 6522 3a20 2237 2f37 222c 0a20  gTime": "7/7",. 
-00000990: 2022 496e 6a31 416c 7465 726e 6174 696e   "Inj1Alternatin
-000009a0: 6754 696d 6522 3a20 2237 2f37 222c 0a20  gTime": "7/7",. 
-000009b0: 2022 496e 6a32 416c 7465 726e 6174 696e   "Inj2Alternatin
-000009c0: 6754 696d 6522 3a20 6e75 6c6c 2c0a 2020  gTime": null,.  
-000009d0: 2246 6972 7374 496e 6a65 6374 696f 6e57  "FirstInjectionW
-000009e0: 6569 6768 7442 6566 6f72 223a 206e 756c  eightBefor": nul
-000009f0: 6c2c 0a20 2022 4669 7273 7449 6e6a 6563  l,.  "FirstInjec
-00000a00: 7469 6f6e 5765 6967 6874 4166 7465 7222  tionWeightAfter"
-00000a10: 3a20 6e75 6c6c 2c0a 2020 2246 6972 7374  : null,.  "First
-00000a20: 496e 6a65 6374 696f 6e49 736f 4475 7261  InjectionIsoDura
-00000a30: 7469 6f6e 223a 206e 756c 6c2c 0a20 2022  tion": null,.  "
-00000a40: 5365 636f 6e64 496e 6a65 6374 696f 6e57  SecondInjectionW
-00000a50: 6569 6768 7442 6566 6f72 6522 3a20 6e75  eightBefore": nu
-00000a60: 6c6c 2c0a 2020 2253 6563 6f6e 6449 6e6a  ll,.  "SecondInj
-00000a70: 6563 7469 6f6e 5765 6967 6874 4166 7465  ectionWeightAfte
-00000a80: 7222 3a20 6e75 6c6c 2c0a 2020 2253 6563  r": null,.  "Sec
-00000a90: 6f6e 6449 6e6a 6563 7469 6f6e 4973 6f44  ondInjectionIsoD
-00000aa0: 7572 6174 696f 6e22 3a20 6e75 6c6c 2c0a  uration": null,.
-00000ab0: 2020 2249 6e6a 3152 6f75 6e64 223a 2022    "Inj1Round": "
-00000ac0: 3173 7422 2c0a 2020 2249 6e6a 3252 6f75  1st",.  "Inj2Rou
-00000ad0: 6e64 223a 2022 326e 6422 2c0a 2020 2248  nd": "2nd",.  "H
-00000ae0: 5049 736f 4c65 7665 6c22 3a20 2253 656c  PIsoLevel": "Sel
-00000af0: 6563 742e 2e2e 222c 0a20 2022 526f 756e  ect...",.  "Roun
-00000b00: 6431 496e 6a49 736f 6c65 7665 6c22 3a20  d1InjIsolevel": 
-00000b10: 2253 656c 6563 742e 2e2e 222c 0a20 2022  "Select...",.  "
-00000b20: 526f 756e 6432 496e 6a49 736f 6c65 7665  Round2InjIsoleve
-00000b30: 6c22 3a20 2253 656c 6563 742e 2e2e 222c  l": "Select...",
-00000b40: 0a20 2022 5465 7374 3149 6422 3a20 3239  .  "Test1Id": 29
-00000b50: 3136 2c0a 2020 2254 6573 7431 5374 7269  16,.  "Test1Stri
-00000b60: 6e67 4964 223a 2022 3239 3136 222c 0a20  ngId": "2916",. 
-00000b70: 2022 5445 5354 5f78 3030 3230 5f32 6e64   "TEST_x0020_2nd
-00000b80: 5f78 3030 3230 5f52 6f75 6e64 5f78 3030  _x0020_Round_x00
-00000b90: 3230 4964 223a 206e 756c 6c2c 0a20 2022  20Id": null,.  "
-00000ba0: 5445 5354 5f78 3030 3230 5f32 6e64 5f78  TEST_x0020_2nd_x
-00000bb0: 3030 3230 5f52 6f75 6e64 5f78 3030 3230  0020_Round_x0020
-00000bc0: 5374 7269 6e67 4964 223a 206e 756c 6c2c  StringId": null,
-00000bd0: 0a20 2022 5445 5354 5f78 3030 3230 5f31  .  "TEST_x0020_1
-00000be0: 7374 5f78 3030 3230 5f52 6f75 6e64 5f78  st_x0020_Round_x
-00000bf0: 3030 3230 4964 223a 2032 3931 362c 0a20  0020Id": 2916,. 
-00000c00: 2022 5445 5354 5f78 3030 3230 5f31 7374   "TEST_x0020_1st
-00000c10: 5f78 3030 3230 5f52 6f75 6e64 5f78 3030  _x0020_Round_x00
-00000c20: 3230 5374 7269 6e67 4964 223a 2022 3239  20StringId": "29
-00000c30: 3136 222c 0a20 2022 4f44 6174 615f 5f78  16",.  "OData__x
-00000c40: 3030 3331 5f48 505f 7830 3032 305f 5265  0031_HP_x0020_Re
-00000c50: 7175 6573 746f 725f 7830 3032 305f 223a  questor_x0020_":
-00000c60: 206e 756c 6c2c 0a20 2022 4973 7375 6522   null,.  "Issue"
-00000c70: 3a20 2253 656c 6563 742e 2e2e 222c 0a20  : "Select...",. 
-00000c80: 2022 546f 7563 685f 7830 3032 305f 5570   "Touch_x0020_Up
-00000c90: 5f78 3030 3230 5f53 7461 7475 7322 3a20  _x0020_Status": 
-00000ca0: 2253 656c 6563 742e 2e2e 222c 0a20 2022  "Select...",.  "
-00000cb0: 546f 7563 685f 7830 3032 305f 5570 5f78  Touch_x0020_Up_x
-00000cc0: 3030 3230 5f53 7572 6765 6f6e 4964 223a  0020_SurgeonId":
-00000cd0: 206e 756c 6c2c 0a20 2022 546f 7563 685f   null,.  "Touch_
-00000ce0: 7830 3032 305f 5570 5f78 3030 3230 5f53  x0020_Up_x0020_S
-00000cf0: 7572 6765 6f6e 5374 7269 6e67 4964 223a  urgeonStringId":
-00000d00: 206e 756c 6c2c 0a20 2022 546f 7563 685f   null,.  "Touch_
-00000d10: 7830 3032 305f 5570 5f78 3030 3230 5f5f  x0020_Up_x0020__
-00000d20: 7830 3032 305f 436f 6d70 223a 206e 756c  x0020_Comp": nul
-00000d30: 6c2c 0a20 2022 4578 7564 6174 655f 7830  l,.  "Exudate_x0
-00000d40: 3032 305f 5365 7665 7269 7479 223a 2022  020_Severity": "
-00000d50: 5365 6c65 6374 2e2e 2e22 2c0a 2020 2253  Select...",.  "S
-00000d60: 6361 6262 696e 6722 3a20 2253 656c 6563  cabbing": "Selec
-00000d70: 742e 2e2e 222c 0a20 2022 4579 655f 7830  t...",.  "Eye_x0
-00000d80: 3032 305f 4973 7375 6522 3a20 2253 656c  020_Issue": "Sel
-00000d90: 6563 742e 2e2e 222c 0a20 2022 4579 655f  ect...",.  "Eye_
-00000da0: 7830 3032 305f 4166 6665 6374 6564 223a  x0020_Affected":
-00000db0: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
-00000dc0: 2254 6f75 6368 5f78 3030 3230 5f55 705f  "Touch_x0020_Up_
-00000dd0: 7830 3032 305f 5765 6967 6874 5f78 3030  x0020_Weight_x00
-00000de0: 3222 3a20 6e75 6c6c 2c0a 2020 224c 494d  2": null,.  "LIM
-00000df0: 535f 7830 3032 305f 6c69 6e6b 223a 2022  S_x0020_link": "
-00000e00: 3c61 2068 7265 663d 2768 7474 703a 2f2f  <a href='http://
-00000e10: 6c69 6d73 322f 7370 6563 696d 656e 733f  lims2/specimens?
-00000e20: 7365 6172 6368 3635 3031 3032 273e 5365  search650102'>Se
-00000e30: 6172 6368 3c2f 613e 222c 0a20 2022 4850  arch</a>",.  "HP
-00000e40: 5f78 3030 3230 5f5f 7830 3032 365f 5f78  _x0020__x0026__x
-00000e50: 3030 3230 5f49 6e6a 223a 2022 5965 7322  0020_Inj": "Yes"
-00000e60: 2c0a 2020 2266 6965 6c64 3330 223a 2022  ,.  "field30": "
-00000e70: 3233 222c 0a20 2022 6669 656c 6435 3022  23",.  "field50"
-00000e80: 3a20 2232 3322 2c0a 2020 224c 494d 5374  : "23",.  "LIMSt
-00000e90: 6173 6b66 6c6f 7731 223a 206e 756c 6c2c  askflow1": null,
-00000ea0: 0a20 2022 436f 6d70 6c69 616e 6365 4173  .  "ComplianceAs
-00000eb0: 7365 7449 6422 3a20 6e75 6c6c 2c0a 2020  setId": null,.  
-00000ec0: 2243 7265 6174 6564 223a 2022 3230 3232  "Created": "2022
-00000ed0: 2d31 322d 3032 5431 373a 3034 3a33 375a  -12-02T17:04:37Z
-00000ee0: 222c 0a20 2022 4175 7468 6f72 4964 223a  ",.  "AuthorId":
-00000ef0: 2031 3837 2c0a 2020 2245 6469 746f 7249   187,.  "EditorI
-00000f00: 6422 3a20 3239 3136 2c0a 2020 224d 6f64  d": 2916,.  "Mod
-00000f10: 6966 6965 6422 3a20 2232 3032 322d 3132  ified": "2022-12
-00000f20: 2d30 3254 3138 3a31 353a 3336 5a22 2c0a  -02T18:15:36Z",.
-00000f30: 2020 2248 5052 6571 7565 7374 6f72 436f    "HPRequestorCo
-00000f40: 6d6d 656e 7473 506c 6169 6e74 6578 7422  mmentsPlaintext"
-00000f50: 3a20 6e75 6c6c 2c0a 2020 224e 616e 6f6a  : null,.  "Nanoj
-00000f60: 6563 744e 756d 6265 7249 6e6a 3222 3a20  ectNumberInj2": 
-00000f70: 224e 4a23 3422 2c0a 2020 224e 616e 6f6a  "NJ#4",.  "Nanoj
-00000f80: 6563 744e 756d 6265 7249 6e6a 3130 223a  ectNumberInj10":
-00000f90: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
-00000fa0: 2249 6f6e 746f 4e75 6d62 6572 496e 6a31  "IontoNumberInj1
-00000fb0: 223a 2022 5365 6c65 6374 2e2e 2e22 2c0a  ": "Select...",.
-00000fc0: 2020 2249 6f6e 746f 4e75 6d62 6572 496e    "IontoNumberIn
-00000fd0: 6a32 223a 2022 5365 6c65 6374 2e2e 2e22  j2": "Select..."
-00000fe0: 2c0a 2020 2249 6f6e 746f 4e75 6d62 6572  ,.  "IontoNumber
-00000ff0: 4850 494e 4a22 3a20 6e75 6c6c 2c0a 2020  HPINJ": null,.  
-00001000: 2269 6e6a 3176 6f6c 7065 7264 6570 7468  "inj1volperdepth
-00001010: 223a 206e 756c 6c2c 0a20 2022 696e 6a32  ": null,.  "inj2
-00001020: 766f 6c70 6572 6465 7074 6822 3a20 6e75  volperdepth": nu
-00001030: 6c6c 2c0a 2020 2249 6e6a 3161 6e67 6c65  ll,.  "Inj1angle
-00001040: 3022 3a20 2230 2064 6567 7265 6573 222c  0": "0 degrees",
-00001050: 0a20 2022 496e 6a32 616e 676c 6530 223a  .  "Inj2angle0":
-00001060: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
-00001070: 2243 6f6e 7475 7369 6f6e 223a 2022 5365  "Contusion": "Se
-00001080: 6c65 6374 2e2e 2e22 2c0a 2020 2248 5053  lect...",.  "HPS
-00001090: 7572 6765 6f6e 436f 6d6d 656e 7473 223a  urgeonComments":
-000010a0: 206e 756c 6c2c 0a20 2022 7374 526f 756e   null,.  "stRoun
-000010b0: 6449 6e6a 6563 7469 6f6e 436f 6d6d 656e  dInjectionCommen
-000010c0: 7473 223a 206e 756c 6c2c 0a20 2022 6e64  ts": null,.  "nd
-000010d0: 526f 756e 6749 6e6a 6563 7469 6f6e 436f  RoungInjectionCo
-000010e0: 6d6d 656e 7473 223a 206e 756c 6c2c 0a20  mments": null,. 
-000010f0: 2022 4669 7273 7452 6f75 6e64 496f 6e74   "FirstRoundIont
-00001100: 6f49 7373 7565 223a 2022 5365 6c65 6374  oIssue": "Select
-00001110: 2e2e 2e22 2c0a 2020 2248 5052 6563 6f76  ...",.  "HPRecov
-00001120: 6572 7922 3a20 6e75 6c6c 2c0a 2020 2246  ery": null,.  "F
-00001130: 6972 7374 496e 6a52 6563 6f76 6572 7922  irstInjRecovery"
-00001140: 3a20 6e75 6c6c 2c0a 2020 2253 6563 6f6e  : null,.  "Secon
-00001150: 6449 6e6a 5265 636f 7665 7222 3a20 6e75  dInjRecover": nu
-00001160: 6c6c 2c0a 2020 2253 6563 6f6e 6452 6f75  ll,.  "SecondRou
-00001170: 6e64 496f 6e74 6f49 7373 7565 223a 2022  ndIontoIssue": "
-00001180: 5365 6c65 6374 2e2e 2e22 2c0a 2020 224c  Select...",.  "L
-00001190: 6f6e 6753 7572 6765 6f6e 436f 6d6d 656e  ongSurgeonCommen
-000011a0: 7473 223a 206e 756c 6c2c 0a20 2022 4c6f  ts": null,.  "Lo
-000011b0: 6e67 3173 7452 6f75 6e64 496e 6a43 6d74  ng1stRoundInjCmt
-000011c0: 7322 3a20 6e75 6c6c 2c0a 2020 224c 6f6e  s": null,.  "Lon
-000011d0: 6732 6e64 526e 6449 6e6a 436d 7473 223a  g2ndRndInjCmts":
-000011e0: 206e 756c 6c2c 0a20 2022 4c6f 6e67 5265   null,.  "LongRe
-000011f0: 7175 6573 746f 7243 6f6d 6d65 6e74 7322  questorComments"
-00001200: 3a20 6e75 6c6c 2c0a 2020 2249 6e6a 3156  : null,.  "Inj1V
-00001210: 6972 7573 5374 7261 696e 5f72 7422 3a20  irusStrain_rt": 
-00001220: 6e75 6c6c 2c0a 2020 2249 6e6a 3256 6972  null,.  "Inj2Vir
-00001230: 7573 5374 7261 696e 5f72 7422 3a20 6e75  usStrain_rt": nu
-00001240: 6c6c 2c0a 2020 2272 6574 5365 7474 696e  ll,.  "retSettin
-00001250: 6730 223a 2022 4f66 6622 2c0a 2020 2272  g0": "Off",.  "r
-00001260: 6574 5365 7474 696e 6731 223a 2022 4f66  etSetting1": "Of
-00001270: 6622 2c0a 2020 2253 7461 7274 5f78 3030  f",.  "Start_x00
-00001280: 3230 5f4f 665f 7830 3032 305f 5765 656b  20_Of_x0020_Week
-00001290: 223a 2022 3230 3232 2d31 322d 3035 5430  ": "2022-12-05T0
-000012a0: 383a 3030 3a30 305a 222c 0a20 2022 456e  8:00:00Z",.  "En
-000012b0: 645f 7830 3032 305f 6f66 5f78 3030 3230  d_x0020_of_x0020
-000012c0: 5f57 6565 6b22 3a20 2232 3032 322d 3132  _Week": "2022-12
-000012d0: 2d30 3954 3038 3a30 303a 3030 5a22 2c0a  -09T08:00:00Z",.
-000012e0: 2020 2241 6765 5f78 3030 3230 5f61 745f    "Age_x0020_at_
-000012f0: 7830 3032 305f 496e 6a65 6374 696f 6e22  x0020_Injection"
-00001300: 3a20 2234 3439 3031 2e30 3030 3030 3030  : "44901.0000000
-00001310: 3030 3022 2c0a 2020 2243 7261 6e69 6f74  000",.  "Craniot
-00001320: 6f6d 7954 7970 6522 3a20 2257 4843 204e  omyType": "WHC N
-00001330: 5022 2c0a 2020 2249 6d70 6c61 6e74 4944  P",.  "ImplantID
-00001340: 436f 7665 7273 6c69 7054 7970 6522 3a20  CoverslipType": 
-00001350: 2235 6d6d 2063 6f76 6572 736c 6970 222c  "5mm coverslip",
-00001360: 0a20 2022 496e 6a31 416e 676c 655f 7632  .  "Inj1Angle_v2
-00001370: 223a 2022 3022 2c0a 2020 2249 6e6a 3241  ": "0",.  "Inj2A
-00001380: 6e67 6c65 5f76 3222 3a20 2230 222c 0a20  ngle_v2": "0",. 
-00001390: 2022 4669 6265 7249 6d70 6c61 6e74 3122   "FiberImplant1"
-000013a0: 3a20 6661 6c73 652c 0a20 2022 4669 6265  : false,.  "Fibe
-000013b0: 7249 6d70 6c61 6e74 3144 5622 3a20 2234  rImplant1DV": "4
-000013c0: 2e32 222c 0a20 2022 4669 6265 7249 6d70  .2",.  "FiberImp
-000013d0: 6c61 6e74 3222 3a20 6661 6c73 652c 0a20  lant2": false,. 
-000013e0: 2022 4669 6265 7249 6d70 6c61 6e74 3244   "FiberImplant2D
-000013f0: 5622 3a20 2234 2e32 222c 0a20 2022 4944  V": "4.2",.  "ID
-00001400: 223a 2035 3535 342c 0a20 2022 4f44 6174  ": 5554,.  "ODat
-00001410: 615f 5f55 4956 6572 7369 6f6e 5374 7269  a__UIVersionStri
-00001420: 6e67 223a 2022 342e 3022 2c0a 2020 2241  ng": "4.0",.  "A
-00001430: 7474 6163 686d 656e 7473 223a 2066 616c  ttachments": fal
-00001440: 7365 2c0a 2020 2247 5549 4422 3a20 2230  se,.  "GUID": "0
-00001450: 3063 3363 3333 332d 6334 6130 2d34 3261  0c3c333-c4a0-42a
-00001460: 612d 6164 6162 2d38 3831 3833 6333 3234  a-adab-88183c324
-00001470: 3230 3122 0a7d 0a0a                      201".}..
+00000990: 2022 496e 6a32 416c 7465 726e 6174 696e   "Inj2Alternatin
+000009a0: 6754 696d 6522 3a20 6e75 6c6c 2c0a 2020  gTime": null,.  
+000009b0: 2246 6972 7374 496e 6a65 6374 696f 6e57  "FirstInjectionW
+000009c0: 6569 6768 7442 6566 6f72 223a 206e 756c  eightBefor": nul
+000009d0: 6c2c 0a20 2022 4669 7273 7449 6e6a 6563  l,.  "FirstInjec
+000009e0: 7469 6f6e 5765 6967 6874 4166 7465 7222  tionWeightAfter"
+000009f0: 3a20 6e75 6c6c 2c0a 2020 2246 6972 7374  : null,.  "First
+00000a00: 496e 6a65 6374 696f 6e49 736f 4475 7261  InjectionIsoDura
+00000a10: 7469 6f6e 223a 206e 756c 6c2c 0a20 2022  tion": null,.  "
+00000a20: 5365 636f 6e64 496e 6a65 6374 696f 6e57  SecondInjectionW
+00000a30: 6569 6768 7442 6566 6f72 6522 3a20 6e75  eightBefore": nu
+00000a40: 6c6c 2c0a 2020 2253 6563 6f6e 6449 6e6a  ll,.  "SecondInj
+00000a50: 6563 7469 6f6e 5765 6967 6874 4166 7465  ectionWeightAfte
+00000a60: 7222 3a20 6e75 6c6c 2c0a 2020 2253 6563  r": null,.  "Sec
+00000a70: 6f6e 6449 6e6a 6563 7469 6f6e 4973 6f44  ondInjectionIsoD
+00000a80: 7572 6174 696f 6e22 3a20 6e75 6c6c 2c0a  uration": null,.
+00000a90: 2020 2249 6e6a 3152 6f75 6e64 223a 2022    "Inj1Round": "
+00000aa0: 3173 7422 2c0a 2020 2249 6e6a 3252 6f75  1st",.  "Inj2Rou
+00000ab0: 6e64 223a 2022 326e 6422 2c0a 2020 2248  nd": "2nd",.  "H
+00000ac0: 5049 736f 4c65 7665 6c22 3a20 2253 656c  PIsoLevel": "Sel
+00000ad0: 6563 742e 2e2e 222c 0a20 2022 526f 756e  ect...",.  "Roun
+00000ae0: 6431 496e 6a49 736f 6c65 7665 6c22 3a20  d1InjIsolevel": 
+00000af0: 2253 656c 6563 742e 2e2e 222c 0a20 2022  "Select...",.  "
+00000b00: 526f 756e 6432 496e 6a49 736f 6c65 7665  Round2InjIsoleve
+00000b10: 6c22 3a20 2253 656c 6563 742e 2e2e 222c  l": "Select...",
+00000b20: 0a20 2022 5465 7374 3149 6422 3a20 3239  .  "Test1Id": 29
+00000b30: 3136 2c0a 2020 2254 6573 7431 5374 7269  16,.  "Test1Stri
+00000b40: 6e67 4964 223a 2022 3239 3136 222c 0a20  ngId": "2916",. 
+00000b50: 2022 5445 5354 5f78 3030 3230 5f32 6e64   "TEST_x0020_2nd
+00000b60: 5f78 3030 3230 5f52 6f75 6e64 5f78 3030  _x0020_Round_x00
+00000b70: 3230 4964 223a 206e 756c 6c2c 0a20 2022  20Id": null,.  "
+00000b80: 5445 5354 5f78 3030 3230 5f32 6e64 5f78  TEST_x0020_2nd_x
+00000b90: 3030 3230 5f52 6f75 6e64 5f78 3030 3230  0020_Round_x0020
+00000ba0: 5374 7269 6e67 4964 223a 206e 756c 6c2c  StringId": null,
+00000bb0: 0a20 2022 5445 5354 5f78 3030 3230 5f31  .  "TEST_x0020_1
+00000bc0: 7374 5f78 3030 3230 5f52 6f75 6e64 5f78  st_x0020_Round_x
+00000bd0: 3030 3230 4964 223a 2032 3931 362c 0a20  0020Id": 2916,. 
+00000be0: 2022 5445 5354 5f78 3030 3230 5f31 7374   "TEST_x0020_1st
+00000bf0: 5f78 3030 3230 5f52 6f75 6e64 5f78 3030  _x0020_Round_x00
+00000c00: 3230 5374 7269 6e67 4964 223a 2022 3239  20StringId": "29
+00000c10: 3136 222c 0a20 2022 4f44 6174 615f 5f78  16",.  "OData__x
+00000c20: 3030 3331 5f48 505f 7830 3032 305f 5265  0031_HP_x0020_Re
+00000c30: 7175 6573 746f 725f 7830 3032 305f 223a  questor_x0020_":
+00000c40: 206e 756c 6c2c 0a20 2022 4973 7375 6522   null,.  "Issue"
+00000c50: 3a20 2253 656c 6563 742e 2e2e 222c 0a20  : "Select...",. 
+00000c60: 2022 546f 7563 685f 7830 3032 305f 5570   "Touch_x0020_Up
+00000c70: 5f78 3030 3230 5f53 7461 7475 7322 3a20  _x0020_Status": 
+00000c80: 2253 656c 6563 742e 2e2e 222c 0a20 2022  "Select...",.  "
+00000c90: 546f 7563 685f 7830 3032 305f 5570 5f78  Touch_x0020_Up_x
+00000ca0: 3030 3230 5f53 7572 6765 6f6e 4964 223a  0020_SurgeonId":
+00000cb0: 206e 756c 6c2c 0a20 2022 546f 7563 685f   null,.  "Touch_
+00000cc0: 7830 3032 305f 5570 5f78 3030 3230 5f53  x0020_Up_x0020_S
+00000cd0: 7572 6765 6f6e 5374 7269 6e67 4964 223a  urgeonStringId":
+00000ce0: 206e 756c 6c2c 0a20 2022 546f 7563 685f   null,.  "Touch_
+00000cf0: 7830 3032 305f 5570 5f78 3030 3230 5f5f  x0020_Up_x0020__
+00000d00: 7830 3032 305f 436f 6d70 223a 206e 756c  x0020_Comp": nul
+00000d10: 6c2c 0a20 2022 4578 7564 6174 655f 7830  l,.  "Exudate_x0
+00000d20: 3032 305f 5365 7665 7269 7479 223a 2022  020_Severity": "
+00000d30: 5365 6c65 6374 2e2e 2e22 2c0a 2020 2253  Select...",.  "S
+00000d40: 6361 6262 696e 6722 3a20 2253 656c 6563  cabbing": "Selec
+00000d50: 742e 2e2e 222c 0a20 2022 4579 655f 7830  t...",.  "Eye_x0
+00000d60: 3032 305f 4973 7375 6522 3a20 2253 656c  020_Issue": "Sel
+00000d70: 6563 742e 2e2e 222c 0a20 2022 4579 655f  ect...",.  "Eye_
+00000d80: 7830 3032 305f 4166 6665 6374 6564 223a  x0020_Affected":
+00000d90: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
+00000da0: 2254 6f75 6368 5f78 3030 3230 5f55 705f  "Touch_x0020_Up_
+00000db0: 7830 3032 305f 5765 6967 6874 5f78 3030  x0020_Weight_x00
+00000dc0: 3222 3a20 6e75 6c6c 2c0a 2020 224c 494d  2": null,.  "LIM
+00000dd0: 535f 7830 3032 305f 6c69 6e6b 223a 2022  S_x0020_link": "
+00000de0: 3c61 2068 7265 663d 2768 7474 703a 2f2f  <a href='http://
+00000df0: 6c69 6d73 322f 7370 6563 696d 656e 733f  lims2/specimens?
+00000e00: 7365 6172 6368 3635 3031 3032 273e 5365  search650102'>Se
+00000e10: 6172 6368 3c2f 613e 222c 0a20 2022 4850  arch</a>",.  "HP
+00000e20: 5f78 3030 3230 5f5f 7830 3032 365f 5f78  _x0020__x0026__x
+00000e30: 3030 3230 5f49 6e6a 223a 2022 5965 7322  0020_Inj": "Yes"
+00000e40: 2c0a 2020 2266 6965 6c64 3330 223a 2022  ,.  "field30": "
+00000e50: 3233 222c 0a20 2022 6669 656c 6435 3022  23",.  "field50"
+00000e60: 3a20 2232 3322 2c0a 2020 224c 494d 5374  : "23",.  "LIMSt
+00000e70: 6173 6b66 6c6f 7731 223a 206e 756c 6c2c  askflow1": null,
+00000e80: 0a20 2022 436f 6d70 6c69 616e 6365 4173  .  "ComplianceAs
+00000e90: 7365 7449 6422 3a20 6e75 6c6c 2c0a 2020  setId": null,.  
+00000ea0: 2243 7265 6174 6564 223a 2022 3230 3232  "Created": "2022
+00000eb0: 2d31 322d 3032 5431 373a 3034 3a33 375a  -12-02T17:04:37Z
+00000ec0: 222c 0a20 2022 4175 7468 6f72 4964 223a  ",.  "AuthorId":
+00000ed0: 2031 3837 2c0a 2020 2245 6469 746f 7249   187,.  "EditorI
+00000ee0: 6422 3a20 3239 3136 2c0a 2020 224d 6f64  d": 2916,.  "Mod
+00000ef0: 6966 6965 6422 3a20 2232 3032 322d 3132  ified": "2022-12
+00000f00: 2d30 3254 3138 3a31 353a 3336 5a22 2c0a  -02T18:15:36Z",.
+00000f10: 2020 2248 5052 6571 7565 7374 6f72 436f    "HPRequestorCo
+00000f20: 6d6d 656e 7473 506c 6169 6e74 6578 7422  mmentsPlaintext"
+00000f30: 3a20 6e75 6c6c 2c0a 2020 224e 616e 6f6a  : null,.  "Nanoj
+00000f40: 6563 744e 756d 6265 7249 6e6a 3222 3a20  ectNumberInj2": 
+00000f50: 224e 4a23 3422 2c0a 2020 224e 616e 6f6a  "NJ#4",.  "Nanoj
+00000f60: 6563 744e 756d 6265 7249 6e6a 3130 223a  ectNumberInj10":
+00000f70: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
+00000f80: 2249 6f6e 746f 4e75 6d62 6572 496e 6a31  "IontoNumberInj1
+00000f90: 223a 2022 5365 6c65 6374 2e2e 2e22 2c0a  ": "Select...",.
+00000fa0: 2020 2249 6f6e 746f 4e75 6d62 6572 496e    "IontoNumberIn
+00000fb0: 6a32 223a 2022 5365 6c65 6374 2e2e 2e22  j2": "Select..."
+00000fc0: 2c0a 2020 2249 6f6e 746f 4e75 6d62 6572  ,.  "IontoNumber
+00000fd0: 4850 494e 4a22 3a20 6e75 6c6c 2c0a 2020  HPINJ": null,.  
+00000fe0: 2269 6e6a 3176 6f6c 7065 7264 6570 7468  "inj1volperdepth
+00000ff0: 223a 206e 756c 6c2c 0a20 2022 696e 6a32  ": null,.  "inj2
+00001000: 766f 6c70 6572 6465 7074 6822 3a20 6e75  volperdepth": nu
+00001010: 6c6c 2c0a 2020 2249 6e6a 3161 6e67 6c65  ll,.  "Inj1angle
+00001020: 3022 3a20 2230 2064 6567 7265 6573 222c  0": "0 degrees",
+00001030: 0a20 2022 496e 6a32 616e 676c 6530 223a  .  "Inj2angle0":
+00001040: 2022 5365 6c65 6374 2e2e 2e22 2c0a 2020   "Select...",.  
+00001050: 2243 6f6e 7475 7369 6f6e 223a 2022 5365  "Contusion": "Se
+00001060: 6c65 6374 2e2e 2e22 2c0a 2020 2248 5053  lect...",.  "HPS
+00001070: 7572 6765 6f6e 436f 6d6d 656e 7473 223a  urgeonComments":
+00001080: 206e 756c 6c2c 0a20 2022 7374 526f 756e   null,.  "stRoun
+00001090: 6449 6e6a 6563 7469 6f6e 436f 6d6d 656e  dInjectionCommen
+000010a0: 7473 223a 206e 756c 6c2c 0a20 2022 6e64  ts": null,.  "nd
+000010b0: 526f 756e 6749 6e6a 6563 7469 6f6e 436f  RoungInjectionCo
+000010c0: 6d6d 656e 7473 223a 206e 756c 6c2c 0a20  mments": null,. 
+000010d0: 2022 4669 7273 7452 6f75 6e64 496f 6e74   "FirstRoundIont
+000010e0: 6f49 7373 7565 223a 2022 5365 6c65 6374  oIssue": "Select
+000010f0: 2e2e 2e22 2c0a 2020 2248 5052 6563 6f76  ...",.  "HPRecov
+00001100: 6572 7922 3a20 6e75 6c6c 2c0a 2020 2246  ery": null,.  "F
+00001110: 6972 7374 496e 6a52 6563 6f76 6572 7922  irstInjRecovery"
+00001120: 3a20 6e75 6c6c 2c0a 2020 2253 6563 6f6e  : null,.  "Secon
+00001130: 6449 6e6a 5265 636f 7665 7222 3a20 6e75  dInjRecover": nu
+00001140: 6c6c 2c0a 2020 2253 6563 6f6e 6452 6f75  ll,.  "SecondRou
+00001150: 6e64 496f 6e74 6f49 7373 7565 223a 2022  ndIontoIssue": "
+00001160: 5365 6c65 6374 2e2e 2e22 2c0a 2020 224c  Select...",.  "L
+00001170: 6f6e 6753 7572 6765 6f6e 436f 6d6d 656e  ongSurgeonCommen
+00001180: 7473 223a 206e 756c 6c2c 0a20 2022 4c6f  ts": null,.  "Lo
+00001190: 6e67 3173 7452 6f75 6e64 496e 6a43 6d74  ng1stRoundInjCmt
+000011a0: 7322 3a20 6e75 6c6c 2c0a 2020 224c 6f6e  s": null,.  "Lon
+000011b0: 6732 6e64 526e 6449 6e6a 436d 7473 223a  g2ndRndInjCmts":
+000011c0: 206e 756c 6c2c 0a20 2022 4c6f 6e67 5265   null,.  "LongRe
+000011d0: 7175 6573 746f 7243 6f6d 6d65 6e74 7322  questorComments"
+000011e0: 3a20 6e75 6c6c 2c0a 2020 2249 6e6a 3156  : null,.  "Inj1V
+000011f0: 6972 7573 5374 7261 696e 5f72 7422 3a20  irusStrain_rt": 
+00001200: 6e75 6c6c 2c0a 2020 2249 6e6a 3256 6972  null,.  "Inj2Vir
+00001210: 7573 5374 7261 696e 5f72 7422 3a20 6e75  usStrain_rt": nu
+00001220: 6c6c 2c0a 2020 2272 6574 5365 7474 696e  ll,.  "retSettin
+00001230: 6730 223a 2022 4f66 6622 2c0a 2020 2272  g0": "Off",.  "r
+00001240: 6574 5365 7474 696e 6731 223a 2022 4f66  etSetting1": "Of
+00001250: 6622 2c0a 2020 2253 7461 7274 5f78 3030  f",.  "Start_x00
+00001260: 3230 5f4f 665f 7830 3032 305f 5765 656b  20_Of_x0020_Week
+00001270: 223a 2022 3230 3232 2d31 322d 3035 5430  ": "2022-12-05T0
+00001280: 383a 3030 3a30 305a 222c 0a20 2022 456e  8:00:00Z",.  "En
+00001290: 645f 7830 3032 305f 6f66 5f78 3030 3230  d_x0020_of_x0020
+000012a0: 5f57 6565 6b22 3a20 2232 3032 322d 3132  _Week": "2022-12
+000012b0: 2d30 3954 3038 3a30 303a 3030 5a22 2c0a  -09T08:00:00Z",.
+000012c0: 2020 2241 6765 5f78 3030 3230 5f61 745f    "Age_x0020_at_
+000012d0: 7830 3032 305f 496e 6a65 6374 696f 6e22  x0020_Injection"
+000012e0: 3a20 2234 3439 3031 2e30 3030 3030 3030  : "44901.0000000
+000012f0: 3030 3022 2c0a 2020 2243 7261 6e69 6f74  000",.  "Craniot
+00001300: 6f6d 7954 7970 6522 3a20 2257 4843 204e  omyType": "WHC N
+00001310: 5022 2c0a 2020 2249 6d70 6c61 6e74 4944  P",.  "ImplantID
+00001320: 436f 7665 7273 6c69 7054 7970 6522 3a20  CoverslipType": 
+00001330: 2235 6d6d 2063 6f76 6572 736c 6970 222c  "5mm coverslip",
+00001340: 0a20 2022 496e 6a31 416e 676c 655f 7632  .  "Inj1Angle_v2
+00001350: 223a 2022 3022 2c0a 2020 2249 6e6a 3241  ": "0",.  "Inj2A
+00001360: 6e67 6c65 5f76 3222 3a20 2230 222c 0a20  ngle_v2": "0",. 
+00001370: 2022 4669 6265 7249 6d70 6c61 6e74 3122   "FiberImplant1"
+00001380: 3a20 6661 6c73 652c 0a20 2022 4669 6265  : false,.  "Fibe
+00001390: 7249 6d70 6c61 6e74 3144 5622 3a20 2234  rImplant1DV": "4
+000013a0: 2e32 222c 0a20 2022 4669 6265 7249 6d70  .2",.  "FiberImp
+000013b0: 6c61 6e74 3222 3a20 6661 6c73 652c 0a20  lant2": false,. 
+000013c0: 2022 4669 6265 7249 6d70 6c61 6e74 3244   "FiberImplant2D
+000013d0: 5622 3a20 2234 2e32 222c 0a20 2022 4944  V": "4.2",.  "ID
+000013e0: 223a 2035 3535 342c 0a20 2022 4f44 6174  ": 5554,.  "ODat
+000013f0: 615f 5f55 4956 6572 7369 6f6e 5374 7269  a__UIVersionStri
+00001400: 6e67 223a 2022 342e 3022 2c0a 2020 2241  ng": "4.0",.  "A
+00001410: 7474 6163 686d 656e 7473 223a 2066 616c  ttachments": fal
+00001420: 7365 2c0a 2020 2247 5549 4422 3a20 2230  se,.  "GUID": "0
+00001430: 3063 3363 3333 332d 6334 6130 2d34 3261  0c3c333-c4a0-42a
+00001440: 612d 6164 6162 2d38 3831 3833 6333 3234  a-adab-88183c324
+00001450: 3230 3122 0a7d 0a0a                      201".}..
```

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item3.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'Procedure'": "'HP+C+Injection+Optic Fiber Implant'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "HP+Injection+Optic Fiber Implant+C",
+    "Procedure": "HP+C+Injection+Optic Fiber Implant",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
```

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item4.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item5.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item6.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item7.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'Procedure'": "'HP+C CAM'"}*

```diff
@@ -104,15 +104,15 @@
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "4.0",
     "OData__x0031_HP_x0020_Requestor_x0020_": null,
     "PIId": 5313,
     "PIStringId": "5313",
     "PedigreeName": "Slc6a3-Cre-650102",
-    "Procedure": "C CAM+HP",
+    "Procedure": "HP+C CAM",
     "Project_x0020_ID_x0020__x0028_te": "122-01-001-10 Neural Dynamics Scientific Activities",
     "Round1InjIsolevel": "Select...",
     "Round2InjIsolevel": "Select...",
     "Scabbing": "Select...",
     "SecondInjRecover": null,
     "SecondInjectionIsoDuration": null,
     "SecondInjectionWeightAfter": null,
```

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item8.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/sharepoint/resources/list_item9.json` & `aind_metadata_service-0.4.1/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/test_client.py` & `aind_metadata_service-0.4.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.0/tests/test_response_handle.py` & `aind_metadata_service-0.4.1/tests/test_response_handle.py`

 * *Files identical despite different names*

