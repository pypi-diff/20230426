# Comparing `tmp/dds_cli-2.2.63.tar.gz` & `tmp/dds_cli-2.2.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dds_cli-2.2.63.tar", last modified: Mon Mar 13 07:20:15 2023, max compression
+gzip compressed data, was "dds_cli-2.2.64.tar", last modified: Wed Apr 26 07:07:13 2023, max compression
```

## Comparing `dds_cli-2.2.63.tar` & `dds_cli-2.2.64.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:20:15.573516 dds_cli-2.2.63/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-13 07:19:35.000000 dds_cli-2.2.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-13 07:20:15.573516 dds_cli-2.2.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-03-13 07:19:35.000000 dds_cli-2.2.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:20:15.569516 dds_cli-2.2.63/dds_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75062 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/custom_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/data_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22599 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/data_lister.py
--rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/data_putter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/data_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/file_handler_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/maintenance_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/project_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/project_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/project_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/text_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/unit_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 07:19:35.000000 dds_cli-2.2.63/dds_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:20:15.569516 dds_cli-2.2.63/dds_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 07:19:57.000000 dds_cli-2.2.63/dds_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-13 07:20:15.000000 dds_cli-2.2.63/dds_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-13 07:19:35.000000 dds_cli-2.2.63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 07:20:15.573516 dds_cli-2.2.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-13 07:19:35.000000 dds_cli-2.2.63/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 07:20:15.569516 dds_cli-2.2.63/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_data_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_file_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_file_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_file_handler_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_maintenance_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_motd_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-03-13 07:19:35.000000 dds_cli-2.2.63/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-26 07:06:39.000000 dds_cli-2.2.64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-26 07:07:13.969940 dds_cli-2.2.64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-26 07:06:39.000000 dds_cli-2.2.64/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.965940 dds_cli-2.2.64/dds_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76580 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/custom_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22599 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_putter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/file_handler_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/maintenance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/project_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/text_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/unit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 07:06:39.000000 dds_cli-2.2.64/dds_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/dds_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:06:58.000000 dds_cli-2.2.64/dds_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 07:07:13.000000 dds_cli-2.2.64/dds_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 07:06:39.000000 dds_cli-2.2.64/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:07:13.969940 dds_cli-2.2.64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 07:06:39.000000 dds_cli-2.2.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:07:13.969940 dds_cli-2.2.64/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_data_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_file_handler_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_maintenance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_motd_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-26 07:06:39.000000 dds_cli-2.2.64/tests/test_utils.py
```

### Comparing `dds_cli-2.2.63/LICENSE` & `dds_cli-2.2.64/LICENSE`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/PKG-INFO` & `dds_cli-2.2.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds_cli
-Version: 2.2.63
+Version: 2.2.64
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dds_cli Version: 2.2.63 Summary: A command line
+Metadata-Version: 2.1 Name: dds_cli Version: 2.2.64 Summary: A command line
 tool to manage data and projects in the SciLifeLab Data Delivery System. Home-
 page: https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data
 Centre License: MIT Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `dds_cli-2.2.63/README.md` & `dds_cli-2.2.64/README.md`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/__init__.py` & `dds_cli-2.2.64/dds_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/__main__.py` & `dds_cli-2.2.64/dds_cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Standard library
 import concurrent.futures
 import itertools
 import logging
 import os
 import sys
+import typing
 
 # Installed
 import pathlib
 import rich_click as click
 import click_pathlib
 import rich
 import rich.logging
@@ -2077,7 +2078,50 @@
         dds_cli.exceptions.ApiResponseError,
         dds_cli.exceptions.ApiRequestError,
         dds_cli.exceptions.DDSCLIException,
         dds_cli.exceptions.InvalidMethodError,
     ) as err:
         LOG.error(err)
         sys.exit(1)
+
+
+# Stats
+
+
+@dds_main.command(name="stats", no_args_is_help=False)
+@click.argument(
+    "stat_type", nargs=1, type=click.Choice(["active", "all", "size"], case_sensitive=True)
+)
+@click.pass_obj
+def get_stats(click_ctx, stat_type):
+    """Get statistics in the DDS."""
+    try:
+        # Num projects
+        with dds_cli.data_lister.DataLister(
+            show_usage=True,
+            no_prompt=click_ctx.get("NO_PROMPT", False),
+            json=True,
+            token_path=click_ctx.get("TOKEN_PATH"),
+        ) as lister:
+            # Get projects, only active by default
+            projects: typing.List = lister.list_projects(show_all=(stat_type == "all"))
+
+            if stat_type == "size":
+                # Calculate total amount of saved data in active projects
+                title_bold_part: str = "Bytes"
+                title_rest: str = "currently stored in DDS"
+                value: int = sum([x["Size"] for x in projects])
+            else:
+                # Get number of projects
+                title_bold_part: str = "Active" if stat_type == "active" else "Total"
+                title_rest: str = "projects"
+                value: int = len(projects)
+
+            LOG.info(f"[bold]{title_bold_part}[/bold] {title_rest}: {value}")
+    except (
+        dds_cli.exceptions.APIError,
+        dds_cli.exceptions.AuthenticationError,
+        dds_cli.exceptions.ApiResponseError,
+        dds_cli.exceptions.ApiRequestError,
+    ) as err:
+        LOG.error(err)
+        sys.exit(1)
```

### Comparing `dds_cli-2.2.63/dds_cli/account_manager.py` & `dds_cli-2.2.64/dds_cli/account_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/auth.py` & `dds_cli-2.2.64/dds_cli/auth.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/base.py` & `dds_cli-2.2.64/dds_cli/base.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/custom_decorators.py` & `dds_cli-2.2.64/dds_cli/custom_decorators.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/data_getter.py` & `dds_cli-2.2.64/dds_cli/data_getter.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/data_lister.py` & `dds_cli-2.2.64/dds_cli/data_lister.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/data_putter.py` & `dds_cli-2.2.64/dds_cli/data_putter.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/data_remover.py` & `dds_cli-2.2.64/dds_cli/data_remover.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/directory.py` & `dds_cli-2.2.64/dds_cli/directory.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/exceptions.py` & `dds_cli-2.2.64/dds_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/file_compressor.py` & `dds_cli-2.2.64/dds_cli/file_compressor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/file_encryptor.py` & `dds_cli-2.2.64/dds_cli/file_encryptor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/file_handler.py` & `dds_cli-2.2.64/dds_cli/file_handler.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/file_handler_local.py` & `dds_cli-2.2.64/dds_cli/file_handler_local.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/file_handler_remote.py` & `dds_cli-2.2.64/dds_cli/file_handler_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,18 +86,14 @@
             raise dds_cli.exceptions.DDSCLIException(
                 "Error in response. Not enough info returned despite ok request."
             )
 
         folder_contents = file_info.get("folder_contents", {})
         files = file_info.get("files")
 
-        LOG.debug(f"Attempted: \n{all_paths}")
-        LOG.debug(f"Files: \n{files}")
-        LOG.debug(f"Folder contents: \n{folder_contents}")
-
         # Cancel download of those files or folders not found in the db
         self.failed = {
             x: {"error": "Not found in DB."}
             for x in all_paths
             if x not in files and x not in folder_contents
         }
 
@@ -128,15 +124,14 @@
                         / pathlib.Path(k["subpath"])
                         / pathlib.Path(k["name_in_bucket"]),
                     }
                     for j, k in y.items()
                 }
             )
 
-        LOG.debug(f"Data (files and folders):\n {data}")
         return data
 
     # Public methods ############ Public methods #
     def create_download_status_dict(self):
         """Create dict for tracking file download status."""
         return {
             x: {
```

### Comparing `dds_cli-2.2.63/dds_cli/maintenance_manager.py` & `dds_cli-2.2.64/dds_cli/maintenance_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/motd_manager.py` & `dds_cli-2.2.64/dds_cli/motd_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/options.py` & `dds_cli-2.2.64/dds_cli/options.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/project_creator.py` & `dds_cli-2.2.64/dds_cli/project_creator.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/project_info.py` & `dds_cli-2.2.64/dds_cli/project_info.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/project_status.py` & `dds_cli-2.2.64/dds_cli/project_status.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/s3_connector.py` & `dds_cli-2.2.64/dds_cli/s3_connector.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/status.py` & `dds_cli-2.2.64/dds_cli/status.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/text_handler.py` & `dds_cli-2.2.64/dds_cli/text_handler.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/timestamp.py` & `dds_cli-2.2.64/dds_cli/timestamp.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/unit_manager.py` & `dds_cli-2.2.64/dds_cli/unit_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/user.py` & `dds_cli-2.2.64/dds_cli/user.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli/utils.py` & `dds_cli-2.2.64/dds_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/dds_cli.egg-info/PKG-INFO` & `dds_cli-2.2.64/dds_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dds-cli
-Version: 2.2.63
+Version: 2.2.64
 Summary: A command line tool to manage data and projects in the SciLifeLab Data Delivery System.
 Home-page: https://github.com/ScilifelabDataCentre/dds_cli
 Author: SciLifeLab Data Centre
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dds-cli Version: 2.2.63 Summary: A command line
+Metadata-Version: 2.1 Name: dds-cli Version: 2.2.64 Summary: A command line
 tool to manage data and projects in the SciLifeLab Data Delivery System. Home-
 page: https://github.com/ScilifelabDataCentre/dds_cli Author: SciLifeLab Data
 Centre License: MIT Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `dds_cli-2.2.63/dds_cli.egg-info/SOURCES.txt` & `dds_cli-2.2.64/dds_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/setup.py` & `dds_cli-2.2.64/setup.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_account_manager.py` & `dds_cli-2.2.64/tests/test_account_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_data_remover.py` & `dds_cli-2.2.64/tests/test_data_remover.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_file_compressor.py` & `dds_cli-2.2.64/tests/test_file_compressor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_file_encryptor.py` & `dds_cli-2.2.64/tests/test_file_encryptor.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_file_handler_local.py` & `dds_cli-2.2.64/tests/test_file_handler_local.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_maintenance_manager.py` & `dds_cli-2.2.64/tests/test_maintenance_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_motd_manager.py` & `dds_cli-2.2.64/tests/test_motd_manager.py`

 * *Files identical despite different names*

### Comparing `dds_cli-2.2.63/tests/test_utils.py` & `dds_cli-2.2.64/tests/test_utils.py`

 * *Files identical despite different names*

