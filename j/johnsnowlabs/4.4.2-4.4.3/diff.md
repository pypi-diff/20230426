# Comparing `tmp/johnsnowlabs-4.4.2.tar.gz` & `tmp/johnsnowlabs-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.4.2.tar", last modified: Tue Apr 18 10:04:43 2023, max compression
+gzip compressed data, was "johnsnowlabs-4.4.3.tar", last modified: Wed Apr 26 21:07:20 2023, max compression
```

## Comparing `johnsnowlabs-4.4.2.tar` & `johnsnowlabs-4.4.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.404204 johnsnowlabs-4.4.2/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.2/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-18 10:04:43.404204 johnsnowlabs-4.4.2/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.2/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-18 08:56:13.000000 johnsnowlabs-4.4.2/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3188 2023-04-17 01:32:57.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-18 08:56:13.000000 johnsnowlabs-4.4.2/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-18 09:05:22.000000 johnsnowlabs-4.4.2/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-18 09:06:36.000000 johnsnowlabs-4.4.2/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.2/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-04-18 09:06:53.000000 johnsnowlabs-4.4.2/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4197 2023-04-18 08:56:13.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.404204 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-18 08:56:13.000000 johnsnowlabs-4.4.2/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.2/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-18 10:04:43.400204 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-18 10:04:43.000000 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-04-18 10:04:43.000000 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-04-18 10:04:43.000000 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-04-18 10:04:43.000000 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-04-18 10:04:43.000000 johnsnowlabs-4.4.2/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-04-18 10:04:43.404204 johnsnowlabs-4.4.2/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2063 2023-04-17 01:32:53.000000 johnsnowlabs-4.4.2/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.3/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.3/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.147242 johnsnowlabs-4.4.3/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.3/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-04-26 14:33:09.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.3/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.3/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4526 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.3/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.3/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-04-26 14:32:25.000000 johnsnowlabs-4.4.3/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:00:41.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 14:39:50.000000 johnsnowlabs-4.4.3/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.3/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.3/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-26 21:07:20.000000 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-04-26 21:07:20.000000 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-04-26 21:07:20.000000 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-04-26 21:07:20.000000 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-04-26 21:07:20.000000 johnsnowlabs-4.4.3/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-04-26 21:07:20.151242 johnsnowlabs-4.4.3/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2054 2023-04-18 10:05:06.000000 johnsnowlabs-4.4.3/setup.py
```

### Comparing `johnsnowlabs-4.4.2/LICENSE` & `johnsnowlabs-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/PKG-INFO` & `johnsnowlabs-4.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.2
+Version: 4.4.3
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.2/README.md` & `johnsnowlabs-4.4.3/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/__init__.py` & `johnsnowlabs-4.4.3/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-4.4.3/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,28 +46,27 @@
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
         }
     }
-
     compatible_spark_to_py_map = {
         SparkVersion.spark3xx: {
             # TODO HARDCODE HASH!!! OR grap from enum or somwhere comfy. Maybe configs/settings file?
             PyInstallTypes.wheel: UrlDependency(
-                url="https://files.pythonhosted.org/packages/e2/80/22d2fca3662ecb658ee43c8b4cad5bbfd899444ba004daf87298f1154d8e/spark_nlp-{lib_version}-py2.py3-none-any.whl",
+                url="https://files.pythonhosted.org/packages/65/19/c439d42f7afd75d6c9c20207db8ee0c95d7c82177b759303c7601120e91a/spark_nlp-{lib_version}-py2.py3-none-any.whl",
                 dependency_type=PyInstallTypes.wheel,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
             PyInstallTypes.tar: UrlDependency(
-                url="https://files.pythonhosted.org/packages/2e/aa/19e34297e3cc22a0f361c22cc366418158612bca8f5b9e3959c1f066f747/spark-nlp-{lib_version}.tar.gz",
+                url="https://files.pythonhosted.org/packages/62/86/6b6c79f923db6ece28dd1c96d088fd2cc01ef7c748021ecb5fe73355635a/spark-nlp-{lib_version}.tar.gz",
                 dependency_type=PyInstallTypes.tar,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
         }
```

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-4.4.3/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/finance.py` & `johnsnowlabs-4.4.3/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/legal.py` & `johnsnowlabs-4.4.3/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/medical.py` & `johnsnowlabs-4.4.3/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/nlp.py` & `johnsnowlabs-4.4.3/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-4.4.3/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-4.4.3/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-4.4.3/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-4.4.3/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/settings.py` & `johnsnowlabs-4.4.3/johnsnowlabs/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.2"
-raw_version_nlp = "4.4.0"
+raw_version_jsl_lib = "4.4.3"
+raw_version_nlp = "4.4.1"
 raw_version_nlu = "4.2.0"
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
 raw_version_medical = "4.4.0"
 raw_version_secret_medical = "4.4.0"
```

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/enums.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/env_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import ast
 import importlib
 import os
 import site
 import subprocess
+from typing import List
+
 
 logged_imports = []
 
 
-def inject_modules(imports: list[str], g):
+def inject_modules(imports: List[str], g):
     # Imports a list of modules in the global scope g
     for module_name in imports:
         try:
             if "." not in module_name:
                 # plain module import
                 g[module_name] = importlib.import_module(module_name)
                 continue
@@ -33,15 +35,15 @@
             g[name] = getattr(importlib.import_module(module), attr)
         except Exception as e:  # ImportError
             if module_name not in logged_imports:
                 logged_imports.append(module_name)
                 print(f"Warning: Could not import module={module_name} error = {e}")
 
 
-def collect_all_imports(source_code) -> list[str]:
+def collect_all_imports(source_code) -> List[str]:
     # collect all import statements from source code string
     tree = ast.parse(source_code)
     imports = []
     for node in ast.walk(tree):
         if isinstance(node, ast.Import):
             for alias in node.names:
                 if alias.asname is None:
@@ -59,15 +61,17 @@
 
 def reverse_compatibility_import(script_path, g):
     """
     Fallback when import fails, this will read source code and import 1-by-1 and add to globals of the calling module
     :param script_path: tge script path, should be fetched with __file__ from calling module
     :param g: globals() from calling script into which we inject imports
     """
-    inject_modules(collect_all_imports(ast.parse(open(script_path).read())), g)
+    inject_modules(
+        collect_all_imports(ast.parse(open(script_path, encoding="utf8").read())), g
+    )
 
 
 def try_import(lib):
     try:
         importlib.reload(site)
         globals()[lib] = importlib.import_module(lib)
         importlib.import_module(lib)
```

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/functional.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-4.4.3/johnsnowlabs/utils/venv_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     print("______________STDERR:")
     print(result.stderr.decode())
 
 
 #
 # @dataclass
 # class VenvState:
-#     installed_libs: list[str]
+#     installed_libs: List[str]
 #     py_version: str
 
 
 class VenvWrapper:
     """
     Utils to install into a Python Executable, which is not the same as current the currently running one
     I.e. whenever you want to install to a local python executable which is != sys.executable use this
```

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs/visual.py` & `johnsnowlabs-4.4.3/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-4.4.3/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.2
+Version: 4.4.3
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.2/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-4.4.3/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.2/setup.py` & `johnsnowlabs-4.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 import johnsnowlabs.settings
+
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
-    f'pyspark=={johnsnowlabs.settings.raw_version_pyspark}',
-    f'spark-nlp=={johnsnowlabs.settings.raw_version_nlp}',
-    f'nlu=={johnsnowlabs.settings.raw_version_nlu}',
-    f'spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}',
-    'numpy',
-    'dataclasses',
-    'requests',
-    'databricks-api',
-    'pydantic',
-    'colorama'
+    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
+    f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
+    f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
+    f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
+    "numpy",
+    "dataclasses",
+    "requests",
+    "databricks-api",
+    "pydantic",
+    "colorama",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
     # name='johnsnowlabs_for_databricks',
-    name='johnsnowlabs',
-    description='The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for '
-                'Finance, Legal and Medical domains. Easily scalable to Spark Cluster ',
+    name="johnsnowlabs",
+    description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
+    "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
-    long_description_content_type='text/markdown',
-    url='https://www.johnsnowlabs.com/',
-    author='John Snow Labs',
-    author_email='christian@johnsnowlabs.com',
+    long_description_content_type="text/markdown",
+    url="https://www.johnsnowlabs.com/",
+    author="John Snow Labs",
+    author_email="christian@johnsnowlabs.com",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: Apache Software License',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: Apache Software License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
     ],
-    keywords='Spark NLP OCR Finance Legal Medical John Snow Labs  ',
-    packages=find_packages(exclude=['test*', 'tmp*']),  # exclude=['test']
-    include_package_data=True
+    keywords="Spark NLP OCR Finance Legal Medical John Snow Labs  ",
+    packages=find_packages(exclude=["test*", "tmp*"]),  # exclude=['test']
+    include_package_data=True,
 )
```

