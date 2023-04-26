# Comparing `tmp/mango-0.0.4.tar.gz` & `tmp/mango-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-0.0.4.tar", last modified: Wed Apr 19 10:56:30 2023, max compression
+gzip compressed data, was "mango-0.0.5.tar", last modified: Wed Apr 26 11:38:15 2023, max compression
```

## Comparing `mango-0.0.4.tar` & `mango-0.0.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-19 10:56:17.000000 mango-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 10:56:17.000000 mango-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 10:56:30.779928 mango-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 10:56:17.000000 mango-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 10:56:17.000000 mango-0.0.4/mango/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/email_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-19 10:56:17.000000 mango-0.0.4/mango/clients/google_cloud_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/config/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 10:56:17.000000 mango-0.0.4/mango/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-19 10:56:17.000000 mango-0.0.4/mango/config/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/data/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 10:56:17.000000 mango-0.0.4/mango/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-19 10:56:17.000000 mango-0.0.4/mango/data/ts_dataset.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-19 10:56:17.000000 mango-0.0.4/mango/images/images_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-19 10:56:17.000000 mango-0.0.4/mango/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/models/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-19 10:56:17.000000 mango-0.0.4/mango/models/neural_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-19 10:56:17.000000 mango-0.0.4/mango/plots/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-19 10:56:17.000000 mango-0.0.4/mango/processing/processing_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-19 10:56:17.000000 mango-0.0.4/mango/schemas/location.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 10:56:17.000000 mango-0.0.4/mango/shared/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/table/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21180 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/pytups_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/pytups_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 10:56:17.000000 mango-0.0.4/mango/table/table_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.779928 mango-0.0.4/mango/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/json_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_bad_type.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_bad_value.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/data/test_good.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_arcgis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_date_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_object_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_processing_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    41638 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-19 10:56:17.000000 mango-0.0.4/mango/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:56:30.775928 mango-0.0.4/mango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 10:56:30.000000 mango-0.0.4/mango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:56:30.779928 mango-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-19 10:56:17.000000 mango-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.674650 mango-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-26 11:38:07.000000 mango-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 11:38:07.000000 mango-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 11:38:15.674650 mango-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:38:07.000000 mango-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 11:38:07.000000 mango-0.0.5/mango/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/email_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-26 11:38:07.000000 mango-0.0.5/mango/clients/google_cloud_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 11:38:07.000000 mango-0.0.5/mango/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-26 11:38:07.000000 mango-0.0.5/mango/config/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 11:38:07.000000 mango-0.0.5/mango/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60080 2023-04-26 11:38:07.000000 mango-0.0.5/mango/data/ts_dataset.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-26 11:38:07.000000 mango-0.0.5/mango/images/images_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-26 11:38:07.000000 mango-0.0.5/mango/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 11:38:07.000000 mango-0.0.5/mango/models/neural_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-26 11:38:07.000000 mango-0.0.5/mango/plots/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-26 11:38:07.000000 mango-0.0.5/mango/processing/processing_time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 11:38:07.000000 mango-0.0.5/mango/schemas/location.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 11:38:07.000000 mango-0.0.5/mango/shared/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/pytups_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/pytups_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-26 11:38:07.000000 mango-0.0.5/mango/table/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.670650 mango-0.0.5/mango/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.674650 mango-0.0.5/mango/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/json_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_bad_type.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_bad_value.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/data/test_good.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_arcgis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_object_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_processing_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42962 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 11:38:07.000000 mango-0.0.5/mango/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:38:15.666650 mango-0.0.5/mango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 11:38:15.000000 mango-0.0.5/mango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:38:15.674650 mango-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-26 11:38:07.000000 mango-0.0.5/setup.py
```

### Comparing `mango-0.0.4/LICENSE` & `mango-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/PKG-INFO` & `mango-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.4/mango/clients/arcgis.py` & `mango-0.0.5/mango/clients/arcgis.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/clients/email_downloader.py` & `mango-0.0.5/mango/clients/email_downloader.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/clients/email_sender.py` & `mango-0.0.5/mango/clients/email_sender.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/clients/google_cloud_storage.py` & `mango-0.0.5/mango/clients/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/config/base_config.py` & `mango-0.0.5/mango/config/base_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/data/ts_dataset.pkl` & `mango-0.0.5/mango/data/ts_dataset.pkl`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/images/images_functions.py` & `mango-0.0.5/mango/images/images_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/logging/chrono.py` & `mango-0.0.5/mango/logging/chrono.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/logging/decorators.py` & `mango-0.0.5/mango/logging/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/logging/logger.py` & `mango-0.0.5/mango/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/models/neural_networks.py` & `mango-0.0.5/mango/models/neural_networks.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/plots/plots.py` & `mango-0.0.5/mango/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/processing/__init__.py` & `mango-0.0.5/mango/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/processing/date_functions.py` & `mango-0.0.5/mango/processing/date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/processing/file_functions.py` & `mango-0.0.5/mango/processing/file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/processing/object_functions.py` & `mango-0.0.5/mango/processing/object_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,11 +132,11 @@
     as_list([1,2]) -> [1,2]
     as_list({1,2}) -> [1,2]
     as_list((1,2)) -> [1,2]
 
     :param x: an object
     :return: a list
     """
-    if isinstance(x, Iterable) and not isinstance(x, str):
+    if isinstance(x, Iterable) and not isinstance(x, str) and not isinstance(x, dict):
         return list(x)
     else:
         return [x]
```

### Comparing `mango-0.0.4/mango/processing/processing_time_series.py` & `mango-0.0.5/mango/processing/processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/shared/const.py` & `mango-0.0.5/mango/shared/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/shared/decorators.py` & `mango-0.0.5/mango/shared/decorators.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/table/pytups_table.py` & `mango-0.0.5/mango/table/pytups_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return TupList(self).take(indices, use_numpy)
 
     # New or modified methods
     def __str__(self):
         if self.len():
             if not isinstance(self[0], dict):
                 return super.__str__(self)
-            columns = len(as_list(self[0])) if self[0] is not None else 0
+            columns = len(self[0]) if self[0] is not None else 0
             return f"Table ({self.len()} rows, {columns} columns):\n" + self.show_rows(
                 0, self.len()
             )
         else:
             return "Empty table"
 
     def show_rows(self, n1, n2=None):
@@ -189,29 +189,29 @@
 
         :param group_by: name of the columns to group.
         :param func: function to apply to the named column. ex: a = first, b = mean
         :return: a table (Tuplist of dict).
         """
         return Table(group_mutate(self, group_by, **func))
 
-    def sum_all(self, group_by) -> "Table":
+    def sum_all(self, group_by=None) -> "Table":
         """
         Group by the given columns and sum the others.
 
         :param group_by: name of the columns to group.
         :return: a table (Tuplist of dict)
         """
         return Table(sum_all(self, group_by))
 
-    def summarise(self, group_by, default: Callable = sum, **func) -> "Table":
+    def summarise(self, group_by=None, default: Callable = None, **func) -> "Table":
         """
         Group by the given columns and apply the given functions to the others.
 
         :param group_by: name of the columns to group.
-        :param default: default function to apply to non grouped columns.
+        :param default: default function to apply to non-grouped columns.
         :param func: function to apply to the named column. ex: a = first, b = mean
         :return: a table (Tuplist of dict).
         """
         return Table(summarise(self, group_by, default=default, **func))
 
     def join(self, table2, by=None, suffix=None, jtype="full", empty=None) -> "Table":
         """
```

### Comparing `mango-0.0.4/mango/table/pytups_tools.py` & `mango-0.0.5/mango/table/pytups_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,25 @@
         table2 = table2.to_dictlist([i for i in range(len(table2[0]))])
 
     # Update table
     nrow = table2.len()
     for k, v in kwargs.items():
         if isinstance(v, Callable):
             table2 = [{**row, **{k: v(row)}} for row in table2]
-        elif len(as_list(v)) == nrow:
-            table2 = [{**row, **{k: v[i]}} for i, row in enumerate(table2)]
         elif v is None or len(as_list(v)) == 1:
             table2 = [{**row, **{k: v}} for row in table2]
+        elif len(as_list(v)) == nrow:
+            table2 = [{**row, **{k: v[i]}} for i, row in enumerate(table2)]
         else:
             raise TypeError(f"Unexpected argument to mutate {v}")
 
     return TupList(table2)
 
 
-def sum_all(table, group_by):
+def sum_all(table, group_by=None):
     """
     Group by the given columns and sum the others.
 
     Example:
     table = TupList([{'a':2, 'b':3, "val":3}, {'a':3, 'b':6, "val":6}, {'a':3, 'b':6, "val":5}])
     result=sum_all(table, group_by=["a", "b"])
     result: [{'a': 2, 'b': 3, 'val': 3}, {'a': 3, 'b': 6, 'val': 11}]
@@ -65,14 +65,16 @@
     :param table: a table (TupList of dict).
     :param group_by: name of the columns to group.
     :return: a table (TupList of dict)
     """
     assert isinstance(table, TupList)
     if len(table) == 0:
         return table
+    if group_by is None:
+        group_by=[]
 
     return (
         table.to_dict(indices=group_by, result_col=None, is_list=True)
         .vapply(lambda v: invert_dict_list(v, unique=False))
         .vapply(lambda v: {k: sum(v[k]) if k not in group_by else v[k][0] for k in v})
         .values_tl()
     )
@@ -86,15 +88,15 @@
     :param col: single name of list of columns to use to group the rows
     :return a SuperDict
     """
     assert isinstance(table, TupList)
     return table.to_dict(indices=col, result_col=None, is_list=True)
 
 
-def summarise(table, group_by, default: [None, Callable] = sum, **func):
+def summarise(table, group_by, default: [None, Callable] = None, **func):
     """
     Group by the given columns and apply the given functions to the others.
 
     Example:
     table = TupList([{'a':2, 'b':3, "c":3}, {'a':3, 'b':6, "c":6}, {'a':3, 'b':6, "c":5}])
     result = summarise(table, "a", b=sum, c=len)
     result: [{'a': 2, 'b': 3, 'c': 1}, {'a': 3, 'b': 12, 'c': 2}]
@@ -105,15 +107,16 @@
     :param func: function to apply to the named column. ex: a = first, b = mean
     :return: a table (TupList of dict).
     """
     assert isinstance(table, TupList)
     # todo: should it create an error?
     if len(table) == 0:
         return table
-
+    if group_by is None:
+        group_by=[]
     if default is not None:
         apply_func = {k: default for k in table[0] if k not in group_by}
     else:
         apply_func = {}
     apply_func.update(dict(**func))
     return (
         table.to_dict(indices=group_by, result_col=None, is_list=True)
@@ -172,14 +175,18 @@
 
     :param table: a table
     :param args: names of the columns to select
     :return: a table (TupList) with the selected columns.
     """
     assert isinstance(table, TupList)
 
+    if not len(table):
+        print("Warning: applying select on an empty table")
+        return TupList()
+
     keep = as_list(args)
     missing = [k for k in keep if k not in get_col_names(table)]
     if len(missing):
         raise ValueError("Column %s not found" % missing)
     return table.vapply(lambda v: {k: v[k] for k in keep})
```

### Comparing `mango-0.0.4/mango/table/table_tools.py` & `mango-0.0.5/mango/table/table_tools.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/const.py` & `mango-0.0.5/mango/tests/const.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/data/json_dataset.json` & `mango-0.0.5/mango/tests/data/json_dataset.json`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/data/test.xlsx` & `mango-0.0.5/mango/tests/data/test.xlsx`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_arcgis_client.py` & `mango-0.0.5/mango/tests/test_arcgis_client.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_config.py` & `mango-0.0.5/mango/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_date_functions.py` & `mango-0.0.5/mango/tests/test_date_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_file_functions.py` & `mango-0.0.5/mango/tests/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_images.py` & `mango-0.0.5/mango/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_logging.py` & `mango-0.0.5/mango/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_models.py` & `mango-0.0.5/mango/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_object_functions.py` & `mango-0.0.5/mango/tests/test_object_functions.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_processing_time_series.py` & `mango-0.0.5/mango/tests/test_processing_time_series.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango/tests/test_table.py` & `mango-0.0.5/mango/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,24 @@
                 {"Name": "Bernard", "Age": 25, "const": 5},
                 {"Name": "Charlie", "Age": 30, "const": 5},
                 {"Name": "Daniel", "Age": 35, "const": 5},
             ]
         )
         self.assertEqual(df, expected, msg=msg)
 
+    def test_mutate_constant_len_1(self):
+        msg = "mutate with a constant for the new column."
+        df = Table([{"Name": "Albert", "Age": 20}]).mutate(const=5)
+        expected = Table(
+            [
+                {"Name": "Albert", "Age": 20, "const": 5},
+            ]
+        )
+        self.assertEqual(df, expected, msg=msg)
+
     def test_mutate_vect(self):
         msg = "mutate with a vector for the new column."
         points = [5, 8, 4, 6]
         df = Table(self.default_data).mutate(points=points)
         expected = Table(
             [
                 {"Name": "Albert", "Age": 20, "points": 5},
@@ -225,14 +235,24 @@
             group_by="Under_25", Points=sum, default=None
         )
         expected = Table(
             [{"Points": 13, "Under_25": True}, {"Points": 10, "Under_25": False}]
         )
         self.assertEqual(df, expected, msg=msg)
 
+    def test_summarise_group_by_none(self):
+        msg = "summarise with group_by = None"
+        df = Table(self.default_data2).summarise(
+            group_by=None, Points=sum, default=None
+        )
+        expected = Table(
+            [{"Points": 23}]
+        )
+        self.assertEqual(df, expected, msg=msg)
+
     def test_select(self):
         msg = "select 2 columns"
         df = Table(self.default_data2).select("Name", "Points")
         expected = Table(
             [
                 {"Name": "Albert", "Points": 5},
                 {"Name": "Bernard", "Points": 8},
@@ -247,14 +267,20 @@
 
         def try_select():
             return Table(self.default_data2).select("unknown", "Points")
 
         self.assertRaises(ValueError, try_select)
 
 
+    def test_select_empty(self):
+        msg = "select on empty table return empty table"
+        df = Table().select("Name")
+        self.assertEqual(df, Table())
+
+
     def test_drop(self):
         msg = "drop 3 columns"
         df = Table(self.default_data2).drop("Under_25", "Points", "Male")
         expected = Table(
             [
                 {"Name": "Albert", "Age": 20},
                 {"Name": "Bernard", "Age": 25},
@@ -474,14 +500,20 @@
             {
                 "Name": "Albert",
                 "Age": 20,
             }
         ]
         self.assertEqual(table, expected, msg=msg)
 
+    def test_filter_empty(self):
+        msg = "filter an empty table"
+        df = Table().filter(lambda v: v["Age"] == 20)
+        expected = Table()
+        self.assertEqual(df, expected, msg=msg)
+
     def test_get_col_names(self):
         msg = "get column names with get_col_names"
         result = Table(self.default_data).get_col_names()
         expected = ["Name", "Age"]
         self.assertEqual(result, expected, msg=msg)
 
     def test_to_columns(self):
@@ -1036,14 +1068,22 @@
         result = Table(self.default_data2).drop("Name").sum_all("Under_25")
         expected = [
             {"Age": 45, "Male": 2, "Points": 13, "Under_25": True},
             {"Age": 65, "Male": 2, "Points": 10, "Under_25": False},
         ]
         self.assertEqual(result, expected, msg=msg)
 
+    def test_sum_all_no_group(self):
+        msg = "sum_all sum every columns"
+        result = Table(self.default_data2).drop("Name").sum_all(None)
+        expected = [
+            {"Age": 110, "Male": 4, "Points": 23, "Under_25": 2},
+        ]
+        self.assertEqual(result, expected, msg=msg)
+
     def test_to_set2(self):
         msg1 = "to_set2 on one column creates a list of values"
         result1 = Table(self.default_data2).to_set2("Points")
         expected1 = [8, 4, 5, 6]
         msg2 = "to_set2 on 2 columns creates a list of tuples"
         result2 = Table(self.default_data2).to_set2(["Age", "Points"])
         expected2 = [(20, 5), (30, 4), (25, 8), (35, 6)]
```

### Comparing `mango-0.0.4/mango/tests/test_tools.py` & `mango-0.0.5/mango/tests/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self.assertEqual(as_list([]), [])
         self.assertEqual(as_list(1), [1])
         self.assertEqual(as_list("one"), ["one"])
         self.assertEqual(as_list(["one", "two"]), ["one", "two"])
         self.assertEqual(as_list((1, 2)), [1, 2])
         self.assertEqual(as_list([1, 2]), [1, 2])
         self.assertEqual(as_list({1, 2}), [1, 2])
+        self.assertEqual(as_list({"a":2}), [{"a":2}])
 
     def test_str_key(self):
         self.assertEqual(str_key({}), {})
         self.assertEqual(str_key({1: "a", 2: "b"}), {"1": "a", "2": "b"})
 
     def test_str_key_warning(self):
         self.assertWarns(SyntaxWarning, str_key, {"1": "a", 1: "b"})
```

### Comparing `mango-0.0.4/mango/tests/test_validation.py` & `mango-0.0.5/mango/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/mango.egg-info/PKG-INFO` & `mango-0.0.5/mango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library with a collection of useful classes and methods to DRY
 Home-page: https://github.com/baobabsoluciones/mango
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: MANGO
         -----
```

### Comparing `mango-0.0.4/mango.egg-info/SOURCES.txt` & `mango-0.0.5/mango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-0.0.4/setup.py` & `mango-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "xlsxwriter",
     ],
 }
 
 
 setuptools.setup(
     name="mango",
-    version="0.0.4",
+    version="0.0.5",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Library with a collection of useful classes and methods to DRY",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/mango",
     packages=setuptools.find_packages(),
     classifiers=[
```

