# Comparing `tmp/fusion-engine-client-1.18.0rc7.tar.gz` & `tmp/fusion-engine-client-1.18.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.18.0rc7.tar", last modified: Tue Apr  4 18:44:35 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.18.1rc2.tar", last modified: Tue Apr 25 23:02:31 2023, max compression
```

## Comparing `fusion-engine-client-1.18.0rc7.tar` & `fusion-engine-client-1.18.1rc2.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.443581 fusion-engine-client-1.18.0rc7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13148 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.443581 fusion-engine-client-1.18.0rc7/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.443581 fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   100508 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    40985 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53790 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23972 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.443581 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-04 18:44:35.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-04 18:44:35.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:44:35.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-04 18:44:35.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 18:44:35.000000 fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:44:35.447582 fusion-engine-client-1.18.0rc7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-04 18:43:58.000000 fusion-engine-client-1.18.0rc7/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.574766 fusion-engine-client-1.18.1rc2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13145 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.574766 fusion-engine-client-1.18.1rc2/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   105922 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55187 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.582766 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.582766 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.18.0rc7/PKG-INFO` & `fusion-engine-client-1.18.1rc2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.0rc7
+Version: 1.18.1rc2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.0rc7/README.md` & `fusion-engine-client-1.18.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/bin/p1_extract` & `fusion-engine-client-1.18.1rc2/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/bin/p1_print` & `fusion-engine-client-1.18.1rc2/bin/p1_print`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             for message_type in message_types:
                 cls = message_type_to_class[message_type]
                 message = cls()
                 if hasattr(message, 'p1_time'):
                     continue
                 else:
                     timestamps = getattr(message, 'timestamps', None)
-                    if isinstance(timestamps, MeasurementTimestamps):
+                    if isinstance(timestamps, MeasurementDetails):
                         continue
                     else:
                         need_system_time = True
                         break
 
         if need_system_time and options.time is not None:
             _logger.info('Non-P1 time messages requested and time range specified. Disabling index file.')
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 from typing import Tuple, Union, List, Any
 
 from collections import namedtuple, defaultdict
 import copy
+import inspect
 import os
 import sys
 import webbrowser
 
 from gpstime import gpstime
 from palettable.tableau import Tableau_20
 import plotly
@@ -1110,65 +1111,89 @@
         self._plot_wheel_ticks_or_speeds(type='speed')
         self._plot_wheel_ticks_or_speeds(type='tick')
 
     def _plot_wheel_ticks_or_speeds(self, type):
         """!
         @brief Plot wheel speed or tick data.
         """
-        # Read the data.
+        # Read the data. Try to determine which type of wheel output is present in the log (if any).
         if type == 'tick':
-            wheel_measurement_type = WheelTickMeasurement
-            vehicle_measurement_type = VehicleTickMeasurement
             filename = 'wheel_ticks'
             figure_title = 'Measurements: Wheel Encoder Ticks'
+
+            wheel_measurement_type = self._auto_detect_message_type([RawWheelTickOutput, WheelTickInput])
+            vehicle_measurement_type = self._auto_detect_message_type([RawVehicleTickOutput, VehicleTickInput])
+
+            # Wheel ticks are raw (uncorrected) by definition.
+            raw_wheel_measurement_type = wheel_measurement_type
+            raw_vehicle_measurement_type = vehicle_measurement_type
         else:
-            wheel_measurement_type = WheelSpeedMeasurement
-            vehicle_measurement_type = VehicleSpeedMeasurement
             filename = 'wheel_speed'
             figure_title = 'Measurements: Wheel Speed'
 
+            wheel_measurement_type = self._auto_detect_message_type([WheelSpeedOutput, DeprecatedWheelSpeedMeasurement])
+            vehicle_measurement_type = self._auto_detect_message_type([VehicleSpeedOutput,
+                                                                       DeprecatedVehicleSpeedMeasurement])
+
+            raw_wheel_measurement_type = self._auto_detect_message_type([RawWheelSpeedOutput])
+            raw_vehicle_measurement_type = self._auto_detect_message_type([RawVehicleSpeedOutput])
+
+            if wheel_measurement_type is None:
+                wheel_measurement_type = raw_wheel_measurement_type
+            if vehicle_measurement_type is None:
+                vehicle_measurement_type = raw_vehicle_measurement_type
+
         # If the measurement data is very high rate, this plot may be very slow to generate for a multi-hour log.
-        if self.truncate_data:
+        if self.long_log_detected and self.truncate_data:
             params = copy.deepcopy(self.params)
             params['max_messages'] = 2
             dt_sec = None
-            result = self.reader.read(message_types=wheel_measurement_type, remove_nan_times=False, **params)
-            data = result[wheel_measurement_type.MESSAGE_TYPE]
-            if len(data.measurement_time) == 2:
-                dt_sec = data.measurement_time[1] - data.measurement_time[0]
-            else:
+
+            if wheel_measurement_type is not None:
+                result = self.reader.read(message_types=wheel_measurement_type, remove_nan_times=False, **params)
+                data = result[wheel_measurement_type.MESSAGE_TYPE]
+                if len(data.measurement_time) == 2:
+                    dt_sec = data.measurement_time[1] - data.measurement_time[0]
+
+            if dt_sec is None and vehicle_measurement_type is not None:
                 result = self.reader.read(message_types=vehicle_measurement_type, remove_nan_times=False, **params)
                 data = result[vehicle_measurement_type.MESSAGE_TYPE]
                 if len(data.measurement_time) == 2:
                     dt_sec = data.measurement_time[1] - data.measurement_time[0]
 
             if dt_sec is not None:
                 data_rate_hz = round(1.0 / dt_sec)
                 if data_rate_hz > self.HIGH_MEASUREMENT_RATE_HZ:
                     _logger.warning('High rate data detected (%d Hz). Skipping wheel %s plot for very long log. Rerun '
                                     'with --truncate=false to generate this plot.' % (data_rate_hz, type))
                     self._add_figure(name=filename, title=f'{figure_title} (Skipped - Long Log Detected)')
                     return
 
-        result = self.reader.read(message_types=[wheel_measurement_type, vehicle_measurement_type],
+        # Read the data.
+        result = self.reader.read(message_types=[wheel_measurement_type, vehicle_measurement_type,
+                                                 raw_wheel_measurement_type, raw_vehicle_measurement_type],
                                   remove_nan_times=False, **self.params)
 
-        wheel_data = result[wheel_measurement_type.MESSAGE_TYPE]
-        wheel_data_signed = False
-        if len(wheel_data.p1_time) == 0:
-            wheel_data = None
-        elif type == 'speed':
-            wheel_data_signed = np.any(wheel_data.is_signed)
-
-        vehicle_data = result[vehicle_measurement_type.MESSAGE_TYPE]
-        vehicle_data_signed = False
-        if len(vehicle_data.p1_time) == 0:
-            vehicle_data = None
-        elif type == 'speed':
-            vehicle_data_signed = np.any(vehicle_data.is_signed)
+        def _extract_data(measurement_type):
+            if measurement_type is not None:
+                data = result[measurement_type.MESSAGE_TYPE]
+                data_signed = False
+                if len(data.p1_time) == 0:
+                    data = None
+                elif type == 'speed':
+                    data_signed = np.any(data.is_signed)
+            else:
+                data = None
+                data_signed = False
+            return data, data_signed
+
+        wheel_data, wheel_data_signed = _extract_data(wheel_measurement_type)
+        raw_wheel_data, raw_wheel_data_signed = _extract_data(raw_wheel_measurement_type)
+        vehicle_data, vehicle_data_signed = _extract_data(vehicle_measurement_type)
+        raw_vehicle_data, raw_vehicle_data_signed = _extract_data(raw_vehicle_measurement_type)
 
         if wheel_data is None and vehicle_data is None:
             self.logger.info('No wheel %s data available. Skipping plot.' % type)
             return
         elif wheel_data is not None and vehicle_data is not None:
             self.logger.warning('Both wheel and vehicle %s data detected.' % type)
             speed_type = 'Wheel/Vehicle'
@@ -1180,14 +1205,28 @@
             titles = ['%s Tick Count' % speed_type, '%s Tick Rate' % speed_type, 'Gear/Direction']
         else:
             if wheel_data_signed or vehicle_data_signed:
                 titles = ['%s Speed (Signed)' % speed_type, 'Gear/Direction']
             else:
                 titles = ['%s Speed (Unsigned)' % speed_type, 'Gear/Direction']
 
+        if wheel_data is not None:
+            titles[0] += f'<br>Messages: {wheel_measurement_type.__name__}'
+        if raw_wheel_data is not None and wheel_measurement_type != raw_wheel_measurement_type:
+            titles[0] += f', {raw_wheel_measurement_type.__name__}'
+
+        if vehicle_data is not None:
+           if wheel_data is not None:
+               titles[0] += ', '
+           else:
+               titles[0] += '<br>Messages: '
+           titles[0] += f'{vehicle_measurement_type.__name__}'
+        if raw_vehicle_data is not None and vehicle_measurement_type != raw_vehicle_measurement_type:
+            titles[0] += f', {raw_vehicle_measurement_type.__name__}'
+
         figure = make_subplots(rows=len(titles), cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
         figure['layout'].update(showlegend=True, modebar_add=['v1hovermode', 'toggleSpikelines'])
         for i in range(len(titles)):
             figure['layout']['xaxis%d' % (i + 1)].update(title="Time (sec)", showticklabels=True)
 
         if type == 'tick':
@@ -1197,14 +1236,17 @@
             figure['layout']['yaxis1'].update(title="Speed (m/s)")
 
         figure['layout']['yaxis%d' % (len(titles))].update(title="Gear/Direction",
                                                            ticktext=['%s (%d)' % (e.name, e.value) for e in GearType],
                                                            tickvals=[e.value for e in GearType])
 
         # Check if the data has P1 time available. If not, we'll plot in the original source time.
+        #
+        # All output messages from the device should contain P1 time. We should only ever use a non-P1 time source when
+        # plotting logged input messages (uncommon).
         wheel_time_source = None
         vehicle_time_source = None
 
         if wheel_data is not None:
             if np.all(np.isnan(wheel_data.p1_time)):
                 if np.any(np.diff(wheel_data.measurement_time_source) != 0):
                     self.logger.warning('Detected multiple time source types in wheel %s data.' % type)
@@ -1248,37 +1290,14 @@
                 '<br>Time Source: %s (Wheel), %s (Vehicle)' % \
                                                           (self._time_source_to_display_name(wheel_time_source),
                                                            self._time_source_to_display_name(vehicle_time_source))
 
         p1_time_present = (wheel_time_source == SystemTimeSource.P1_TIME or
                            vehicle_time_source == SystemTimeSource.P1_TIME)
 
-        # Plot the data.
-        def _plot_trace(time, data, name, color, text):
-            if type == 'tick':
-                figure.add_trace(go.Scattergl(x=time, y=data, text=text,
-                                              name=name, hoverlabel={'namelength': -1},
-                                              legendgroup=name,
-                                              mode='lines', marker={'color': color}),
-                                 1, 1)
-
-                dt_sec = np.diff(time)
-                ticks_per_sec = np.diff(data) / dt_sec
-                figure.add_trace(go.Scattergl(x=time[1:], y=ticks_per_sec, text=text,
-                                              name=name, hoverlabel={'namelength': -1},
-                                              legendgroup=name, showlegend=False,
-                                              mode='lines', marker={'color': color}),
-                                 2, 1)
-            else:
-                figure.add_trace(go.Scattergl(x=time, y=data, text=text,
-                                              name=name, hoverlabel={'namelength': -1},
-                                              legendgroup=name,
-                                              mode='lines', marker={'color': color}),
-                                 1, 1)
-
         # If plotting speed data, try to plot the navigation engine's speed estimate for reference.
         #
         # Note: Pose data is not read when plotting ticks (ticks do not plot in meters/second). If the wheel data is not
         # in P1 time, we cannot compare against the pose data, which is.
         if type == 'speed' and p1_time_present:
             nav_engine_p1_time = None
             nav_engine_speed_mps = None
@@ -1314,105 +1333,176 @@
                 time = nav_engine_p1_time - float(self.t0)
                 text = ["P1: %.3f sec" % t for t in nav_engine_p1_time]
                 figure.add_trace(go.Scattergl(x=time, y=nav_engine_speed_mps, text=text,
                                               name=nav_engine_speed_name, hoverlabel={'namelength': -1},
                                               mode='lines', line={'color': 'black', 'dash': 'dash'}),
                                  1, 1)
 
-        if wheel_data is not None:
-            abs_time_sec = self._get_measurement_time(wheel_data, wheel_time_source)
+        # Plot the data.
+        def _plot_trace(time, data, name, color, text, style=None):
+            if style is None:
+                style = {}
+            style.setdefault('mode', 'lines')
+            style.setdefault('line', {}).setdefault('color', color)
+
+            if type == 'tick':
+                figure.add_trace(go.Scattergl(x=time, y=data, text=text,
+                                              name=name, hoverlabel={'namelength': -1},
+                                              legendgroup=name,
+                                              **style),
+                                 1, 1)
+
+                dt_sec = np.diff(time)
+                ticks_per_sec = np.diff(data) / dt_sec
+                figure.add_trace(go.Scattergl(x=time[1:], y=ticks_per_sec, text=text,
+                                              name=name, hoverlabel={'namelength': -1},
+                                              legendgroup=name, showlegend=False,
+                                              **style),
+                                 2, 1)
+            else:
+                figure.add_trace(go.Scattergl(x=time, y=data, text=text,
+                                              name=name, hoverlabel={'namelength': -1},
+                                              legendgroup=name,
+                                              **style),
+                                 1, 1)
+
+        def _plot_wheel_data(data, time_source, is_raw=False, show_gear=False, style=None):
+            if data is None:
+                return
+
+            if style is None:
+                style = {}
+            style.setdefault('mode', 'lines')
+            if is_raw:
+                style.setdefault('line', {}).setdefault('dash', 'dash')
+
+            if type == 'tick':
+                var_suffix = 'wheel_ticks'
+                name_suffix = ''
+            else:
+                var_suffix = 'speed_mps'
+                name_suffix = ' (Uncorrected)' if is_raw else ' (Corrected)'
+
+            abs_time_sec = self._get_measurement_time(data, time_source)
             idx = ~np.isnan(abs_time_sec)
             abs_time_sec = abs_time_sec[idx]
 
-            t0 = self._get_t0_for_time_source(wheel_time_source)
+            t0 = self._get_t0_for_time_source(time_source)
             time = abs_time_sec - t0
-            time_name = self._time_source_to_display_name(wheel_time_source)
+            time_name = self._time_source_to_display_name(time_source)
             text = ["%s Time: %.3f sec" % (time_name, t) for t in abs_time_sec]
 
+            _plot_trace(time=time, data=getattr(data, 'front_left_' + var_suffix)[idx], text=text,
+                        name='Front Left Wheel' + name_suffix, color='red', style=style)
+            _plot_trace(time=time, data=getattr(data, 'front_right_' + var_suffix)[idx], text=text,
+                        name='Front Right Wheel' + name_suffix, color='green', style=style)
+            _plot_trace(time=time, data=getattr(data, 'rear_left_' + var_suffix)[idx], text=text,
+                        name='Rear Left Wheel' + name_suffix, color='blue', style=style)
+            _plot_trace(time=time, data=getattr(data, 'rear_right_' + var_suffix)[idx], text=text,
+                        name='Rear Right Wheel' + name_suffix, color='purple', style=style)
+
+            if show_gear:
+                figure.add_trace(go.Scattergl(x=time, y=wheel_data.gear[idx], text=text,
+                                              name='Gear (Wheel Data)', hoverlabel={'namelength': -1},
+                                              mode='markers', marker={'color': 'red'}),
+                                 3 if type == 'tick' else 2, 1)
+
+        # Plot the wheel speed data. If we have both corrected and uncorrected (raw) data, plot them both.
+        _plot_wheel_data(wheel_data, wheel_time_source, is_raw=wheel_measurement_type == raw_wheel_measurement_type,
+                         show_gear=True)
+        if wheel_measurement_type != raw_wheel_measurement_type:
+            _plot_wheel_data(raw_wheel_data, wheel_time_source, is_raw=True, show_gear=False)
+
+        def _plot_vehicle_data(data, time_source, is_raw=False, show_gear=False, style=None):
+            if data is None:
+                return
+
+            if style is None:
+                style = {}
+            style.setdefault('mode', 'lines')
+            if is_raw:
+                style.setdefault('line', {}).setdefault('dash', 'dash')
+
             if type == 'tick':
-                suffix = 'wheel_ticks'
+                var_suffix = 'tick_count'
+                name_suffix = ''
             else:
-                suffix = 'speed_mps'
-
-            _plot_trace(time=time, data=getattr(wheel_data, 'front_left_' + suffix)[idx], text=text,
-                        name='Front Left Wheel', color='red')
-            _plot_trace(time=time, data=getattr(wheel_data, 'front_right_' + suffix)[idx], text=text,
-                        name='Front Right Wheel', color='green')
-            _plot_trace(time=time, data=getattr(wheel_data, 'rear_left_' + suffix)[idx], text=text,
-                        name='Rear Left Wheel', color='blue')
-            _plot_trace(time=time, data=getattr(wheel_data, 'rear_right_' + suffix)[idx], text=text,
-                        name='Rear Right Wheel', color='purple')
-
-            figure.add_trace(go.Scattergl(x=time, y=wheel_data.gear[idx], text=text,
-                                          name='Gear (Wheel Data)', hoverlabel={'namelength': -1},
-                                          mode='markers', marker={'color': 'red'}),
-                             3 if type == 'tick' else 2, 1)
+                var_suffix = 'vehicle_speed_mps'
+                name_suffix = ' (Uncorrected)' if is_raw else ' (Corrected)'
 
-        if vehicle_data is not None:
-            abs_time_sec = self._get_measurement_time(vehicle_data, vehicle_time_source)
+            abs_time_sec = self._get_measurement_time(data, time_source)
             idx = ~np.isnan(abs_time_sec)
             abs_time_sec = abs_time_sec[idx]
 
-            t0 = self._get_t0_for_time_source(vehicle_time_source)
+            t0 = self._get_t0_for_time_source(time_source)
             time = abs_time_sec - t0
-            time_name = self._time_source_to_display_name(vehicle_time_source)
+            time_name = self._time_source_to_display_name(time_source)
             text = ["%s Time: %.3f sec" % (time_name, t) for t in abs_time_sec]
 
-            if type == 'tick':
-                attr = 'tick_count'
-            else:
-                attr = 'vehicle_speed_mps'
+            _plot_trace(time=time, data=getattr(data, var_suffix)[idx], text=text,
+                        name='Speed Measurement' + name_suffix, color='orange', style=style)
 
-            _plot_trace(time=time, data=getattr(vehicle_data, attr)[idx], text=text,
-                        name='Speed Measurement', color='orange')
-
-            figure.add_trace(go.Scattergl(x=time, y=vehicle_data.gear[idx], text=text,
-                                          name='Gear (Vehicle Data)', hoverlabel={'namelength': -1},
-                                          mode='markers', marker={'color': 'orange'}),
-                             3 if type == 'tick' else 2, 1)
+            if show_gear:
+                figure.add_trace(go.Scattergl(x=time, y=data.gear[idx], text=text,
+                                              name='Gear (Vehicle Data)', hoverlabel={'namelength': -1},
+                                              mode='markers', marker={'color': 'orange'}),
+                                 3 if type == 'tick' else 2, 1)
+
+        # Plot the vehicle speed data. If we have both corrected and uncorrected (raw) data, plot them both.
+        _plot_vehicle_data(vehicle_data, vehicle_time_source,
+                           is_raw=vehicle_measurement_type == raw_vehicle_measurement_type, show_gear=True)
+        if vehicle_measurement_type != raw_vehicle_measurement_type:
+            _plot_vehicle_data(raw_vehicle_data, vehicle_time_source, is_raw=True, show_gear=False)
 
         self._add_figure(name=filename, figure=figure, title=figure_title)
 
     def plot_imu(self):
         """!
         @brief Plot the IMU data.
         """
         if self.output_dir is None:
             return
 
-        filename ='imu'
-        figure_title ='Measurements: IMU'
+        self._plot_imu_data(message_cls=IMUOutput, filename='imu', figure_title='Measurements: IMU')
+        self._plot_imu_data(message_cls=RawIMUOutput, filename='raw_imu',
+                            figure_title='Measurements: IMU (Uncorrected)')
 
+    def _plot_imu_data(self, message_cls, filename, figure_title):
         # If the measurement data is very high rate, this plot may be very slow to generate for a multi-hour log.
         if self.truncate_data:
             params = copy.deepcopy(self.params)
             params['max_messages'] = 2
-            result = self.reader.read(message_types=[IMUMeasurement], **params)
-            data = result[IMUMeasurement.MESSAGE_TYPE]
+            result = self.reader.read(message_types=[message_cls], **params)
+            data = result[message_cls.MESSAGE_TYPE]
             if len(data.p1_time) == 2:
                 dt_sec = data.p1_time[1] - data.p1_time[0]
                 data_rate_hz = round(1.0 / dt_sec)
                 if data_rate_hz > self.HIGH_MEASUREMENT_RATE_HZ:
                     _logger.warning('High rate IMU data detected (%d Hz). Skipping IMU plot for very long log. Rerun '
                                     'with --truncate=false to generate this plot.' % data_rate_hz)
                     self._add_figure(name=filename, title=f'{figure_title} (Skipped - Long Log Detected)')
                     return
 
         # Read the data.
-        result = self.reader.read(message_types=[IMUMeasurement], **self.params)
-        data = result[IMUMeasurement.MESSAGE_TYPE]
+        result = self.reader.read(message_types=[message_cls], **self.params)
+        data = result[message_cls.MESSAGE_TYPE]
 
         if len(data.p1_time) == 0:
             self.logger.info('No IMU data available. Skipping plot.')
             return
 
         time = data.p1_time - float(self.t0)
 
-        figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True,
-                               subplot_titles=['Acceleration', 'Gyro'])
+        titles = ['Acceleration', 'Gyro']
+        if message_cls == RawIMUOutput:
+            titles = [t + ' (Uncorrected)' for t in titles]
+        else:
+            titles = [t + ' (Corrected)' for t in titles]
+
+        figure = make_subplots(rows=2, cols=1, print_grid=False, shared_xaxes=True, subplot_titles=titles)
 
         figure['layout'].update(showlegend=True)
         figure['layout']['xaxis1'].update(title="Time (sec)", showticklabels=True)
         figure['layout']['xaxis2'].update(title="Time (sec)", showticklabels=True)
         figure['layout']['yaxis1'].update(title="Acceleration (m/s^2)")
         figure['layout']['yaxis2'].update(title="Rotation Rate (rad/s)")
 
@@ -1931,14 +2021,28 @@
         elif time_source == SystemTimeSource.GPS_TIME:
             return 0.0
         elif time_source == SystemTimeSource.SENDER_SYSTEM_TIME:
             return 0.0
         elif time_source == SystemTimeSource.TIMESTAMPED_ON_RECEPTION:
             return float(self.system_t0)
 
+    def _auto_detect_message_type(self, types: List[MessageType]):
+        types = [t.MESSAGE_TYPE if inspect.isclass(t) else t for t in types]
+
+        params = copy.deepcopy(self.params)
+        params['max_messages'] = 1
+        selected_type = None
+        for message_type in types:
+            result = self.reader.read(message_types=message_type, remove_nan_times=False, **params)
+            data = result[message_type]
+            if len(data.p1_time) > 0:
+                selected_type = message_type_to_class[message_type]
+                break
+        return selected_type
+
     @classmethod
     def _get_measurement_time(cls, data, time_source: SystemTimeSource) -> np.ndarray:
         if time_source == SystemTimeSource.P1_TIME:
             return data.p1_time
         else:
             return data.measurement_time
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,16 @@
         if message_types is None:
             pass
         elif isinstance(message_types, MessageType):
             message_types = set((message_types,))
         elif MessagePayload.is_subclass(message_types):
             message_types = set((message_types.get_type(),))
         else:
-            message_types = set([(t.get_type() if MessagePayload.is_subclass(t) else t) for t in message_types])
+            message_types = set([(t.get_type() if MessagePayload.is_subclass(t) else t) for t in message_types
+                                 if t is not None])
             if len(message_types) == 0:
                 message_types = None
 
         # If the message type list is empty, read all messages.
         if message_types is None or len(message_types) == 0:
             message_types = list(message_type_to_class.keys())
 
@@ -579,15 +580,15 @@
         """!
         @brief Convert UTC or GPS timestamps to P1 time.
 
         @param times A list of one or more timestamps to be converted, using any of the following formats:
                - `datetime` - A UTC or local timezone date and time
                - `gpstime` - A GPS timestamp
                - A @ref fusion_engine_client.messages.timestamps.Timestamp containing GPS time or P1 time
-               - A @ref fusion_engine_client.messages.timestamps.MeasurementTimestamps containing GPS time or P1 time
+               - A @ref fusion_engine_client.messages.timestamps.MeasurementDetails containing GPS time or P1 time
                - `float` - A GPS or P1 time value (in seconds)
                  - Note that UTC timestamps cannot be specified `float` unless `assume_utc == True`
         @param assume_utc If `True`:
                - For `float` values, assume values greater than the POSIX offset for 2000/1/1 are UTC timestamps in
                  seconds.
                - For `datetime`, if `tzinfo` is not set, assume it is `timezone.utc`. Otherwise, interpret the timestamp
                  in the local timezone.
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     VEHICLE_DETAILS = 20
     WHEEL_CONFIG = 21
     HARDWARE_TICK_CONFIG = 22
     ENABLED_GNSS_SYSTEMS = 50
     ENABLED_GNSS_FREQUENCY_BANDS = 51
     LEAP_SECOND = 52
     GPS_WEEK_ROLLOVER = 53
+    IONOSPHERE_CONFIG = 54
+    TROPOSPHERE_CONFIG = 55
     INTERFACE_CONFIG = 200
     UART1_BAUD = 256
     UART2_BAUD = 257
     UART1_OUTPUT_DIAGNOSTICS_MESSAGES = 258
     UART2_OUTPUT_DIAGNOSTICS_MESSAGES = 259
     ENABLE_WATCHDOG_TIMER = 300
 
@@ -203,14 +205,23 @@
     PQTMVERNO = 1200
     PQTMVER = 1201
     PQTMGNSS = 1202
     PQTMVERNO_SUB = 1203
     PQTMVER_SUB = 1204
     PQTMTXT = 1205
 
+class IonoDelayModel(IntEnum):
+    AUTO = 0
+    OFF = 1
+    KLOBUCHAR = 2
+
+class TropoDelayModel(IntEnum):
+    AUTO = 0
+    OFF = 1
+    SAASTAMOINEN = 2
 
 def get_message_type_string(protocol: ProtocolType, message_id: int):
     if message_id == ALL_MESSAGES_ID:
         return 'ALL (%d)' % message_id
     else:
         enum = None
         try:
@@ -556,14 +567,38 @@
     HardwareTickConfigConstruct = Struct(
         "tick_mode" / AutoEnum(Int8ul, TickMode),
         "tick_direction" / AutoEnum(Int8ul, TickDirection),
         Padding(2),
         "wheel_ticks_to_m" / Float32l,
     )
 
+    class IonosphereConfig(NamedTuple):
+        """!
+        @brief Ionospheric delay model configuration.
+        """
+        ## The ionospheric delay model to use.
+        iono_delay_model: IonoDelayModel = IonoDelayModel.AUTO
+
+    IonosphereConfigConstruct = Struct(
+        "iono_delay_model" / AutoEnum(Int8ul, IonoDelayModel),
+        Padding(3),
+    )
+
+    class TroposphereConfig(NamedTuple):
+        """!
+        @brief Tropospheric delay model configuration.
+        """
+        ## The tropospheric delay model to use.
+        tropo_delay_model: TropoDelayModel = TropoDelayModel.AUTO
+
+    TroposphereConfigConstruct = Struct(
+        "tropo_delay_model" / AutoEnum(Int8ul, TropoDelayModel),
+        Padding(3),
+    )
+
     class Empty(NamedTuple):
         """!
         @brief Dummy specifier for empty config.
         """
         pass
 
     # Empty construct
@@ -640,14 +675,29 @@
 
     Set to -1 to disable week rollover override and re-enable internal handling.
     """
     def __new__(cls, value: int = -1):
         return super().__new__(cls, value)
 
 
+@_conf_gen.create_config_class(ConfigType.IONOSPHERE_CONFIG, _conf_gen.IonosphereConfigConstruct)
+class IonosphereConfig(_conf_gen.IonosphereConfig):
+    """!
+    @brief Ionospheric delay model configuration.
+    """
+    pass
+
+@_conf_gen.create_config_class(ConfigType.TROPOSPHERE_CONFIG, _conf_gen.TroposphereConfigConstruct)
+class TroposphereConfig(_conf_gen.TroposphereConfig):
+    """!
+    @brief Tropospheric delay model configuration.
+    """
+    pass
+
+
 @_conf_gen.create_config_class(ConfigType.UART1_BAUD, _conf_gen.UInt32Construct)
 class Uart1BaudConfig(_conf_gen.IntegerVal):
     """!
     @brief The UART1 serial baud rate (in bits/second).
     """
     pass
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import struct
 import sys
 from typing import Dict, List, Optional, Set, Type, Union
 from zlib import crc32
 
 import numpy as np
 
+from .measurement_details import *
 from .signal_defs import *
 from .timestamp import *
 from ..utils import trace as logging
 from ..utils.enum_utils import IntEnum
 
 _logger = logging.getLogger('point_one.fusion_engine.messages.defs')
 
@@ -23,14 +24,21 @@
     def _remove_suffix(s, suffix):
         if s.endswith(suffix):
             return s[:-len(suffix)]
         else:
             return s
 
 
+def _remove_suffixes(s, suffixes):
+    result = s
+    for suffix in suffixes:
+        result = _remove_suffix(result, suffix)
+    return result
+
+
 class SolutionType(IntEnum):
     # Invalid, no position available.
     Invalid = 0
     # Standalone GNSS fix, no correction data used.
     AutonomousGPS = 1
     # Differential GNSS pseudorange solution using a local RTK base station or SSR or SBAS corrections.
     DGPS = 2
@@ -85,22 +93,34 @@
     CALIBRATION_STATUS = 10004
     RELATIVE_ENU_POSITION = 10005
 
     # Device status messages.
     SYSTEM_STATUS = 10500
 
     # Sensor measurement messages.
-    IMU_MEASUREMENT = 11000
+    IMU_OUTPUT = 11000
     HEADING_MEASUREMENT = 11001
+    RAW_IMU_MEASUREMENT = 11002
 
     # Vehicle measurement messages.
-    WHEEL_SPEED_MEASUREMENT = 11101
-    VEHICLE_SPEED_MEASUREMENT = 11102
-    WHEEL_TICK_MEASUREMENT = 11103
-    VEHICLE_TICK_MEASUREMENT = 11104
+    DEPRECATED_WHEEL_SPEED_MEASUREMENT = 11101
+    DEPRECATED_VEHICLE_SPEED_MEASUREMENT = 11102
+
+    WHEEL_TICK_INPUT = 11103
+    VEHICLE_TICK_INPUT = 11104
+    WHEEL_SPEED_INPUT = 11105
+    VEHICLE_SPEED_INPUT = 11106
+
+    RAW_WHEEL_TICK_OUTPUT = 11123
+    RAW_VEHICLE_TICK_OUTPUT = 11124
+    RAW_WHEEL_SPEED_OUTPUT = 11125
+    RAW_VEHICLE_SPEED_OUTPUT = 11126
+
+    WHEEL_SPEED_OUTPUT = 11135
+    VEHICLE_SPEED_OUTPUT = 11136
 
     # ROS messages.
     ROS_POSE = 12000
     ROS_GPS_FIX = 12010
     ROS_IMU = 12011
 
     # Command and control messages.
@@ -426,19 +446,20 @@
                              if re.match(re_pattern, k, flags=re.IGNORECASE)]
             if len(matched_types) == 0:
                 _logger.warning("No message types matching pattern '%s'." % pattern)
                 continue
 
             # Check for exact matches with "Message" and "Measurement" suffixes removed.
             if len(matched_types) > 1 and not allow_multiple:
-                def _remove_suffixes(s):
-                    return _remove_suffix(_remove_suffix(s.lower(), 'message'), 'measurement')
-                pattern_no_suffix = _remove_suffixes(pattern)
+                def _remove_message_suffixes(s):
+                    return _remove_suffixes(s.lower(), ['message', 'measurement', 'input', 'output'])
+                pattern_no_suffix = _remove_message_suffixes(pattern)
                 exact_matches = [t for t in matched_types
-                                 if _remove_suffixes(cls.message_type_to_class[t].__name__) == pattern_no_suffix]
+                                 if _remove_message_suffixes(cls.message_type_to_class[t].__name__) ==
+                                 pattern_no_suffix]
                 if len(exact_matches) == 1:
                     matched_types = exact_matches
 
             # If there are still too many matches, fail.
             if len(matched_types) > 1 and not allow_multiple:
                 class_names = [cls.message_type_to_class[t].__name__ for t in matched_types]
                 raise ValueError("Pattern '%s' matches multiple message types:%s\n\nAdd a wildcard (%s*) to display "
@@ -503,25 +524,25 @@
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         raise NotImplementedError('pack() not implemented.')
 
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = _UNSPECIFIED_VERSION) -> int:
         raise NotImplementedError('unpack() not implemented.')
 
     def get_p1_time(self) -> Timestamp:
-        measurement_timestamps = getattr(self, 'timestamps', None)
-        if isinstance(measurement_timestamps, MeasurementTimestamps):
-            return measurement_timestamps.p1_time
+        measurement_details = getattr(self, 'details', None)
+        if isinstance(measurement_details, MeasurementDetails):
+            return measurement_details.p1_time
         else:
             return getattr(self, 'p1_time', None)
 
     def get_system_time_ns(self) -> float:
-        measurement_timestamps = getattr(self, 'timestamps', None)
-        if isinstance(measurement_timestamps, MeasurementTimestamps):
-            if measurement_timestamps.measurement_time_source == SystemTimeSource.TIMESTAMPED_ON_RECEPTION:
-                return float(measurement_timestamps.measurement_time)
+        measurement_details = getattr(self, 'details', None)
+        if isinstance(measurement_details, MeasurementDetails):
+            if measurement_details.measurement_time_source == SystemTimeSource.TIMESTAMPED_ON_RECEPTION:
+                return float(measurement_details.measurement_time)
             else:
                 return np.nan
         else:
             return getattr(self, 'system_time_ns', None)
 
     def get_system_time_sec(self) -> float:
         system_time_ns = self.get_system_time_ns()
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,22 +519,22 @@
                 self.message_types = set((key,))
                 self.filtered_message_types = True
             elif MessagePayload.is_subclass(key):
                 self.message_types = set((key.get_type(),))
                 self.filtered_message_types = True
             # Return entries for a list of message types.
             elif isinstance(key, (set, list, tuple)) and len(key) > 0 and isinstance(next(iter(key)), MessageType):
-                new_message_types = set(key)
+                new_message_types = {t for t in key if t is not None}
                 if self.message_types is None:
                     self.message_types = new_message_types
                 else:
                     self.message_types = self.message_types & new_message_types
                 self.filtered_message_types = True
             elif isinstance(key, (set, list, tuple)) and len(key) > 0 and MessagePayload.is_subclass(next(iter(key))):
-                new_message_types = set([t.get_type() for t in key])
+                new_message_types = set([t.get_type() for t in key if t is not None])
                 if self.message_types is None:
                     self.message_types = new_message_types
                 else:
                     self.message_types = self.message_types & new_message_types
                 self.filtered_message_types = True
             # Key is a slice in time. Return a subset of the data.
             elif isinstance(key, slice) and (isinstance(key.start, (Timestamp, float)) or
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/construct_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,41 @@
+import math
 import re
 from typing import Optional
 
 from construct import Adapter, Enum, Struct
 
 from .enum_utils import IntEnum
 
 
+class FixedPointAdapter(Adapter):
+    def __init__(self, scale, *args, invalid=None):
+        super().__init__(*args)
+        self.scale = scale
+        self.invalid = invalid
+
+        is_signed = self.subcon.fmtstr.islower()
+        if self.invalid is not None and is_signed:
+            max_negative_mag = 2 ** (self.subcon.sizeof() * 8 - 1)
+            if self.invalid == max_negative_mag:
+                self.invalid = -self.invalid
+
+    def _decode(self, obj, context, path):
+        if obj == self.invalid:
+            return math.nan
+        else:
+            return float(obj * self.scale)
+
+    def _encode(self, obj, context, path):
+        if math.isnan(obj) and self.invalid is not None:
+            return self.invalid
+        else:
+            return int(round(obj / self.scale))
+
+
 class NamedTupleAdapter(Adapter):
     """!
     @brief Adapter for automatically converting between construct streams and
            NamedTuples with corresponding fields.
 
     Usage Example:
     ```{.py}
@@ -88,14 +114,15 @@
 
     def make_default(self):
         return self.cls()
 
     def _decode(self, obj, context, path):
         val = self.cls()
         val.__dict__.update(obj)
+        del val.__dict__['_io']
         return val
 
     def _encode(self, obj, context, path):
         return obj.__dict__
 
 
 class EnumAdapter(Adapter):
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.0rc7
+Version: 1.18.1rc2
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.0rc7/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 fusion_engine_client/messages/__init__.py
 fusion_engine_client/messages/configuration.py
 fusion_engine_client/messages/control.py
 fusion_engine_client/messages/core.py
 fusion_engine_client/messages/defs.py
 fusion_engine_client/messages/device.py
 fusion_engine_client/messages/fault_control.py
+fusion_engine_client/messages/measurement_details.py
 fusion_engine_client/messages/measurements.py
 fusion_engine_client/messages/ros.py
 fusion_engine_client/messages/signal_defs.py
 fusion_engine_client/messages/solution.py
 fusion_engine_client/messages/timestamp.py
 fusion_engine_client/parsers/__init__.py
 fusion_engine_client/parsers/decoder.py
@@ -36,14 +37,16 @@
 fusion_engine_client/utils/construct_utils.py
 fusion_engine_client/utils/enum_utils.py
 fusion_engine_client/utils/log.py
 fusion_engine_client/utils/numpy_utils.py
 fusion_engine_client/utils/time_range.py
 fusion_engine_client/utils/trace.py
 tests/test_config.py
+tests/test_construct_utils.py
 tests/test_data_loader.py
 tests/test_decoder.py
 tests/test_encoder.py
+tests/test_enum_utils.py
 tests/test_file_index.py
 tests/test_message_defs.py
 tests/test_mixed_log_reader.py
 tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.18.0rc7/setup.py` & `fusion-engine-client-1.18.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_config.py` & `fusion-engine-client-1.18.1rc2/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pytest
 from fusion_engine_client.messages import (
-    ConfigurationSource, ConfigResponseMessage, ConfigType, SetConfigMessage,
-    AppliedSpeedType, InterfaceBaudRateConfig, ConfigResponseMessage, ConfigType,
-    ConfigurationSource, DeviceCourseOrientationConfig, Direction, EnabledGNSSFrequencyBandsConfig,
-    EnabledGNSSSystemsConfig, FrequencyBand, FrequencyBandMask, GetConfigMessage,
-    GNSSLeverArmConfig, HardwareTickConfig, InterfaceConfigSubmessage, InterfaceID,
-    InterfaceConfigType, InvalidConfig, MessageRate, MessageRateResponse,
-    RateResponseEntry, SatelliteType, SatelliteTypeMask, SetConfigMessage,
-    SteeringType, TickDirection, TickMode, TransportType, Uart1BaudConfig,
-    VehicleDetailsConfig, VehicleModel, WheelConfig, WheelSensorType)
+    AppliedSpeedType, ConfigurationSource, ConfigResponseMessage, ConfigType,
+    InterfaceBaudRateConfig, ConfigResponseMessage, ConfigType, ConfigurationSource, DeviceCourseOrientationConfig,
+    Direction, EnabledGNSSFrequencyBandsConfig,EnabledGNSSSystemsConfig, FrequencyBand, FrequencyBandMask,
+    GetConfigMessage, GNSSLeverArmConfig, HardwareTickConfig, IonoDelayModel, IonosphereConfig,
+    InterfaceConfigSubmessage, InterfaceID, InterfaceConfigType, InvalidConfig, MessageRate, MessageRateResponse,
+    RateResponseEntry, SatelliteType, SatelliteTypeMask, SetConfigMessage,SteeringType, TickDirection, TickMode,
+    TransportType, TropoDelayModel, TroposphereConfig, Uart1BaudConfig, VehicleDetailsConfig, VehicleModel,
+    WheelConfig, WheelSensorType)
 from fusion_engine_client.messages.configuration import \
     _RateResponseEntryConstructRaw
 from fusion_engine_client.utils import trace as logging
 
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logging.getLogger('point_one').setLevel(logging.DEBUG)
@@ -30,14 +29,20 @@
     set_msg = SetConfigMessage(WheelConfig(WheelSensorType.NONE, AppliedSpeedType.NONE,
                                            SteeringType.UNKNOWN, 1., 2., 3., 4., 1000, False, True))
     assert len(set_msg.pack()) == BASE_SIZE + 28
 
     set_msg = SetConfigMessage(HardwareTickConfig(TickMode.OFF, TickDirection.OFF, 0.1))
     assert len(set_msg.pack()) == BASE_SIZE + 8
 
+    set_msg = SetConfigMessage(IonosphereConfig(IonoDelayModel.AUTO))
+    assert len(set_msg.pack()) == BASE_SIZE + 4
+
+    set_msg = SetConfigMessage(TroposphereConfig(TropoDelayModel.AUTO))
+    assert len(set_msg.pack()) == BASE_SIZE + 4
+
     set_msg = SetConfigMessage(GNSSLeverArmConfig(1, 2, 3))
     assert len(set_msg.pack()) == BASE_SIZE + 12
 
     set_msg = SetConfigMessage()
     set_msg.config_object = Uart1BaudConfig(9600)
     uart_data = set_msg.pack()
     assert len(uart_data) == BASE_SIZE + 4
```

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_data_loader.py` & `fusion-engine-client-1.18.1rc2/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_decoder.py` & `fusion-engine-client-1.18.1rc2/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_encoder.py` & `fusion-engine-client-1.18.1rc2/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_file_index.py` & `fusion-engine-client-1.18.1rc2/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_message_defs.py` & `fusion-engine-client-1.18.1rc2/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.18.1rc2/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.0rc7/tests/test_time_range.py` & `fusion-engine-client-1.18.1rc2/tests/test_time_range.py`

 * *Files identical despite different names*

