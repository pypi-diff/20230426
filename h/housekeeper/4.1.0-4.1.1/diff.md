# Comparing `tmp/housekeeper-4.1.0.tar.gz` & `tmp/housekeeper-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.1.0.tar", last modified: Fri Apr 21 14:00:47 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.1.1.tar", last modified: Wed Apr 26 11:13:49 2023, max compression
```

## Comparing `housekeeper-4.1.0.tar` & `housekeeper-4.1.1.tar`

### file list

```diff
@@ -1,102 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-21 14:00:36.000000 housekeeper-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-21 14:00:36.000000 housekeeper-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-21 14:00:47.000000 housekeeper-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-21 14:00:36.000000 housekeeper-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/file_tags_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 14:00:36.000000 housekeeper-4.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 14:00:36.000000 housekeeper-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 14:00:47.000000 housekeeper-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-21 14:00:36.000000 housekeeper-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_file_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_find_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_store_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 11:13:41.000000 housekeeper-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 11:13:41.000000 housekeeper-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-26 11:13:49.000000 housekeeper-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-26 11:13:41.000000 housekeeper-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/file_tags_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-26 11:13:41.000000 housekeeper-4.1.1/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 11:13:49.000000 housekeeper-4.1.1/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 11:13:41.000000 housekeeper-4.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 11:13:41.000000 housekeeper-4.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 11:13:49.000000 housekeeper-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-26 11:13:41.000000 housekeeper-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:13:49.000000 housekeeper-4.1.1/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_add_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_add_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_file_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_find_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_store_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/store/test_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-26 11:13:41.000000 housekeeper-4.1.1/tests/test_include.py
```

### Comparing `housekeeper-4.1.0/LICENSE` & `housekeeper-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/PKG-INFO` & `housekeeper-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.1.0
+Version: 4.1.1
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.1.0/README.md` & `housekeeper-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/add.py` & `housekeeper-4.1.1/housekeeper/cli/add.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/core.py` & `housekeeper-4.1.1/housekeeper/cli/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/delete.py` & `housekeeper-4.1.1/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/get.py` & `housekeeper-4.1.1/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/include.py` & `housekeeper-4.1.1/housekeeper/cli/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/init.py` & `housekeeper-4.1.1/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/cli/tables.py` & `housekeeper-4.1.1/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/date.py` & `housekeeper-4.1.1/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/files.py` & `housekeeper-4.1.1/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/include.py` & `housekeeper-4.1.1/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/api/core.py` & `housekeeper-4.1.1/housekeeper/store/api/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import logging
 from pathlib import Path
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, scoped_session
 
 from housekeeper.store.models import Model
-from housekeeper.store.api.add import AddHandler
-from housekeeper.store.api.find import FindHandler
+from housekeeper.store.api.handlers.create import CreateHandler
+from housekeeper.store.api.handlers.read import ReadHandler
 
 LOG = logging.getLogger(__name__)
 
 
-class CoreHandler(FindHandler, AddHandler):
+class CoreHandler(ReadHandler, CreateHandler):
     """Aggregating class for the store api handlers"""
 
     def __init__(self, session):
-        FindHandler(session=session)
-        AddHandler(session=session)
+        ReadHandler(session=session)
+        CreateHandler(session=session)
 
 
 class Store(CoreHandler):
 
     """
     Handles interactions with the database in the context when a temporary
     database connection is needed, e.g. a command line interface.
```

### Comparing `housekeeper-4.1.0/housekeeper/store/api/schema.py` & `housekeeper-4.1.1/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/file_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/file_tags_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/file_tags_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/filters/version_filters.py` & `housekeeper-4.1.1/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper/store/models.py` & `housekeeper-4.1.1/housekeeper/store/models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.1.1/housekeeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.1.0
+Version: 4.1.1
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.1.0/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.1.1/housekeeper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,15 @@
 housekeeper/cli/get.py
 housekeeper/cli/include.py
 housekeeper/cli/init.py
 housekeeper/cli/tables.py
 housekeeper/store/__init__.py
 housekeeper/store/models.py
 housekeeper/store/api/__init__.py
-housekeeper/store/api/add.py
-housekeeper/store/api/base.py
 housekeeper/store/api/core.py
-housekeeper/store/api/find.py
 housekeeper/store/api/schema.py
 housekeeper/store/filters/__init__.py
 housekeeper/store/filters/bundle_filters.py
 housekeeper/store/filters/file_filters.py
 housekeeper/store/filters/file_tags_filters.py
 housekeeper/store/filters/tag_filters.py
 housekeeper/store/filters/version_bundle_filters.py
```

### Comparing `housekeeper-4.1.0/setup.py` & `housekeeper-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.1.0",
+    version="4.1.1",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.1.0/tests/cli/add/conftest.py` & `housekeeper-4.1.1/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.1.1/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.1.1/tests/cli/add/test_cli_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.1.1/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.1.1/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/conftest.py` & `housekeeper-4.1.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.1.1/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.1.1/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.1.1/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.1.1/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/get/test_get_bundle.py` & `housekeeper-4.1.1/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/get/test_get_files.py` & `housekeeper-4.1.1/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/get/test_get_tag.py` & `housekeeper-4.1.1/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/get/test_get_version.py` & `housekeeper-4.1.1/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/test_cli_core.py` & `housekeeper-4.1.1/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/cli/test_cli_include.py` & `housekeeper-4.1.1/tests/cli/test_cli_include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/conftest.py` & `housekeeper-4.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/helper_functions.py` & `housekeeper-4.1.1/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/conftest.py` & `housekeeper-4.1.1/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_add_core.py` & `housekeeper-4.1.1/tests/store/test_add_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_add_file.py` & `housekeeper-4.1.1/tests/store/test_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_bundle_filters.py` & `housekeeper-4.1.1/tests/store/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_file_filters.py` & `housekeeper-4.1.1/tests/store/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_file_tag_filters.py` & `housekeeper-4.1.1/tests/store/test_file_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_find_tag.py` & `housekeeper-4.1.1/tests/store/test_find_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_store_api.py` & `housekeeper-4.1.1/tests/store/test_store_api.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_store_models.py` & `housekeeper-4.1.1/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_tag_filters.py` & `housekeeper-4.1.1/tests/store/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_version_bundle_filters.py` & `housekeeper-4.1.1/tests/store/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/store/test_version_filters.py` & `housekeeper-4.1.1/tests/store/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/test_date.py` & `housekeeper-4.1.1/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.1.0/tests/test_include.py` & `housekeeper-4.1.1/tests/test_include.py`

 * *Files identical despite different names*

