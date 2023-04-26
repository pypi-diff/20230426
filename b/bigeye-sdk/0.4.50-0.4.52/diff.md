# Comparing `tmp/bigeye_sdk-0.4.50.tar.gz` & `tmp/bigeye_sdk-0.4.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.50.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.52.tar", max compression
```

## Comparing `bigeye_sdk-0.4.50.tar` & `bigeye_sdk-0.4.52.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     2092 2023-01-13 19:29:40.987774 bigeye_sdk-0.4.50/LICENSE
--rw-r--r--   0        0        0      873 2022-09-21 14:26:02.564243 bigeye_sdk-0.4.50/README.md
--rw-r--r--   0        0        0     3727 2022-09-21 19:14:17.084238 bigeye_sdk-0.4.50/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2022-09-21 19:14:17.084343 bigeye_sdk-0.4.50/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.564505 bigeye_sdk-0.4.50/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-03-24 00:17:08.953130 bigeye_sdk-0.4.50/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     2009 2023-01-13 19:29:40.988022 bigeye_sdk-0.4.50/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2022-09-21 14:26:02.564714 bigeye_sdk-0.4.50/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.084676 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0     9870 2023-03-24 00:17:08.953474 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-03-24 00:17:08.953740 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-03-24 00:17:08.953972 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2022-09-21 19:14:17.085326 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-03-24 00:17:08.954155 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-03-24 00:17:08.954346 bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565379 bigeye_sdk-0.4.50/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2022-09-21 14:26:02.565502 bigeye_sdk-0.4.50/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2022-10-11 14:47:52.093321 bigeye_sdk-0.4.50/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565649 bigeye_sdk-0.4.50/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2022-12-01 16:53:45.901990 bigeye_sdk-0.4.50/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39770 2023-03-24 00:17:08.954904 bigeye_sdk-0.4.50/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2022-09-21 14:26:02.566284 bigeye_sdk-0.4.50/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    37136 2023-03-29 13:58:35.688056 bigeye_sdk-0.4.50/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.086145 bigeye_sdk-0.4.50/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2022-11-30 18:19:48.731219 bigeye_sdk-0.4.50/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    32261 2023-03-29 13:58:35.688936 bigeye_sdk-0.4.50/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.566925 bigeye_sdk-0.4.50/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2022-09-21 19:14:17.086414 bigeye_sdk-0.4.50/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2022-09-21 14:26:02.567122 bigeye_sdk-0.4.50/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      907 2023-03-24 00:17:08.955789 bigeye_sdk-0.4.50/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.567221 bigeye_sdk-0.4.50/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-01-13 19:29:40.988379 bigeye_sdk-0.4.50/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2022-10-18 15:49:05.166354 bigeye_sdk-0.4.50/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-02-03 22:21:16.752839 bigeye_sdk-0.4.50/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2022-09-21 14:26:02.567414 bigeye_sdk-0.4.50/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2022-09-21 19:14:17.086730 bigeye_sdk-0.4.50/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2022-11-30 18:19:48.731507 bigeye_sdk-0.4.50/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-03-24 00:17:08.955960 bigeye_sdk-0.4.50/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      116 2022-09-21 14:26:02.567705 bigeye_sdk-0.4.50/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20233 2022-11-30 18:19:48.731658 bigeye_sdk-0.4.50/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     1554 2022-12-01 16:53:45.902364 bigeye_sdk-0.4.50/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2022-10-11 14:47:52.094658 bigeye_sdk-0.4.50/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-01-13 19:29:40.988609 bigeye_sdk-0.4.50/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5089 2023-03-24 00:17:08.956184 bigeye_sdk-0.4.50/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4032 2023-03-24 00:17:08.956445 bigeye_sdk-0.4.50/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1611 2022-09-21 14:26:02.569178 bigeye_sdk-0.4.50/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-03-29 14:34:03.837677 bigeye_sdk-0.4.50/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 14:34:03.837755 bigeye_sdk-0.4.50/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 14:34:03.837825 bigeye_sdk-0.4.50/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 14:34:03.837879 bigeye_sdk-0.4.50/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   198728 2023-03-29 14:34:03.837969 bigeye_sdk-0.4.50/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-03-29 14:34:03.840309 bigeye_sdk-0.4.50/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-03-29 14:34:03.840371 bigeye_sdk-0.4.50/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2022-09-21 14:26:02.569285 bigeye_sdk-0.4.50/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2022-09-21 19:14:17.088368 bigeye_sdk-0.4.50/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2022-09-21 19:14:17.088495 bigeye_sdk-0.4.50/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    22303 2023-03-24 00:17:08.956794 bigeye_sdk-0.4.50/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-02-23 17:53:03.561875 bigeye_sdk-0.4.50/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0      937 2023-03-20 21:46:22.944778 bigeye_sdk-0.4.50/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-03-24 00:17:08.957102 bigeye_sdk-0.4.50/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-01-13 19:29:40.989263 bigeye_sdk-0.4.50/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8412 2023-03-24 00:17:08.957318 bigeye_sdk-0.4.50/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2022-11-30 18:19:48.733054 bigeye_sdk-0.4.50/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    43510 2023-03-29 13:58:35.690715 bigeye_sdk-0.4.50/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-02-22 23:48:15.904646 bigeye_sdk-0.4.50/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7114 2023-03-24 00:17:08.957856 bigeye_sdk-0.4.50/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3709 2023-03-24 00:17:08.958353 bigeye_sdk-0.4.50/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.50/setup.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.50/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/LICENSE
+-rw-r--r--   0        0        0      873 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/README.md
+-rw-r--r--   0        0        0     3727 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    17489 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0     2122 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10223 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39770 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    38235 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    32599 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      907 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      117 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20233 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     1554 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5089 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4032 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   202792 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      507 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    22303 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3584 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    45112 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7114 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3709 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.52/setup.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.52/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.50/LICENSE` & `bigeye_sdk-0.4.52/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/README.md` & `bigeye_sdk-0.4.52/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.52/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.52/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.52/bigeye_sdk/authentication/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 import json
 from dataclasses import dataclass
 from typing import TypeVar
 
 from bigeye_sdk.functions.aws import get_secret
 
 from bigeye_sdk.log import get_logger
+from bigeye_sdk.serializable import PydanticSubtypeSerializable
 
 log = get_logger(__file__)
 
 
-class Credential(abc.ABC):
+class Credential(abc.ABC, PydanticSubtypeSerializable):
     pass
 
 
 CREDENTIAL = TypeVar('CREDENTIAL', bound='Credential')
 
 
 class LocalFileCredential(Credential):
 
     @classmethod
     def load_from_file(cls, file: str) -> CREDENTIAL:
         log.info(f'Loading API Conf: {file}')
         with open(file) as fin:
-            return cls(**json.load(fin))
+            return cls.parse_obj(**json.load(fin))
 
 
 class AwsSecretCredential(Credential):
 
     @classmethod
     def load_from_aws_secret(cls, secret_name: str, region_name: str = 'us-west-2') -> CREDENTIAL:
         log.info(f'Loading Secret: {secret_name}')
-        return cls(**get_secret(region_name=region_name, secret_name=secret_name))
+        return cls.parse_obj(**get_secret(region_name=region_name, secret_name=secret_name))
 
 
 class LoadableCredential(LocalFileCredential, AwsSecretCredential):
     pass
 
 
 class DatabaseCredential(LoadableCredential):
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.52/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from betterproto import Casing
 from pydantic import Field
 from pydantic_yaml import YamlStrEnum
 
 from bigeye_sdk import DatawatchObject
 from bigeye_sdk.bigconfig_validation.validation_models import ValidationError
 from bigeye_sdk.exceptions.exceptions import BigConfigValidationException
-from bigeye_sdk.generated.com.bigeye.models.generated import MetricSuiteResponse, Source, CohortDefinition
+from bigeye_sdk.generated.com.bigeye.models.generated import MetricSuiteResponse, CohortDefinition, \
+    InvalidAssetMetricDefinitionApplication
 from bigeye_sdk.log import get_logger
+from bigeye_sdk.model.protobuf_message_facade import SimpleMetricType
 from bigeye_sdk.serializable import File
 
 # TODO: Add error stats to API Execution Messages.
 FAILED_API_EXECUTION_MSG = textwrap.dedent(
     """
 
     -=- REPORT -=-
@@ -70,14 +72,22 @@
 
 BIGCONFIG_REPORT = TypeVar('BIGCONFIG_REPORT', bound='BigConfigReport')
 REPORTS: List[BIGCONFIG_REPORT] = []
 
 log = get_logger(__file__)
 
 
+def metric_type_not_supported(invalid: InvalidAssetMetricDefinitionApplication) -> bool:
+    not_supported = True
+    return not_supported in [
+        True if f"Metric type {mm.predefined_metric} not supported on table {invalid.fq_asset_name}" in
+                invalid.error_messages else False for mm in SimpleMetricType.get_metadata_metrics()
+    ]
+
+
 def process_reports(output_path: str):
     report_files = []
     errors_reported = False
 
     source_reports = []
 
     for report in REPORTS:
@@ -241,19 +251,18 @@
 
         def is_wildcard_search(cohort: CohortDefinition):
             return '*' in cohort.column_name_pattern or \
                 '*' in cohort.table_name_pattern or \
                 '*' in cohort.schema_name_pattern
 
         for mae in obj.metric_application_errors:
-            if not is_wildcard_search(mae.from_cohort):
-                "Only adding error reporting where the metrics were not applied to a asset name containing wild cards." \
-                "This reduces the noise around reporting.  Customers will understand that assets matched using wild" \
-                "cards are likely to produce invalid metric applications."
-
+            if is_wildcard_search(mae.from_cohort) and metric_type_not_supported(mae):
+                continue
+            else:
+                "Adding error reporting where the metrics were not applied to assets containing wild cards and MMs not supported."
                 metric_application_errors.append(mae.to_dict())
                 # TODO add validation error.  Problem is that I cannot match back to the full fq pattern.
 
         invalid_asset_identifier_errors = [ice.to_dict() for ice in obj.invalid_cohort_errors]
 
         pr = MetricSuiteReport(
             process_stage=process_stage,
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.52/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.52/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     GetNamedSchedulesRequest, NamedScheduleSortField, GetNamedSchedulesResponse, \
     SchemaList, SchemaSearchRequest, DataNodeType, CreateDataNodeRequest, DataNode, \
     CreateLineageRelationshipRequest, LineageRelationship, CreateCollectionResponse, TimeRange, NotificationChannel, \
     CreateMetricTemplateRequest, MetricTemplate, MetricTemplateParametersFieldEntry, Warehouse, \
     CreateMetricTemplateResponse, VirtualTableRequest, VirtualTable, MetricTemplateParameterType, FieldType, \
     GetMetricTemplateListRequest, GetMetricTemplateListResponse, MetricTemplateSortField, UpdateVirtualTableRequest, \
     SchemaChangeSortField, GetSchemaChangesRequest, GetSchemaChangesResponse, SchemaChange, IntegrationsResponse, \
-    Integration, TableauWorkbook, GetIntegrationEntitiesResponse, ConfigValue, GetConfigListResponse, WorkflowResponse, \
-    WorkflowStatusResponse
+    TableauWorkbook, Integration, GetIntegrationEntitiesResponse, ConfigValue, GetConfigListResponse, WorkflowResponse, \
+    WorkflowStatusResponse, GetLineageRelationshipsForNodeResponse
+
 # create logger
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.protobuf_enum_facade import SimpleFieldType, SimpleMetricTemplateParameterType
 
 log = get_logger(__file__)
 
 
@@ -562,33 +563,50 @@
         log.info(f'Begin delete for warehouse ID: {warehouse_id}')
 
     def get_issues(
             self,
             *,
             current_status: List[IssueStatus] = [],
             warehouse_ids: List[int] = [],
-            schemas: List[str] = [],
+            schema_ids: List[int] = [],
             metric_ids: List[int] = [],
             collection_ids: List[int] = [],
-            issue_ids: List[int] = []) -> List[Issue]:
+            issue_ids: List[int] = [],
+            schema_names: List[str] = [],
+            table_ids: List[int] = [],
+            column_ids: List[int] = [],
+            related_issue_ids: List[int]= []) -> List[Issue]:
 
         url = '/api/v1/issues/fetch'
 
         # TODO: Will require update when GetIssuesRequest refactors to collection_ids
 
         request = GetIssuesRequest()
         request.current_status = current_status
         request.warehouse_ids = warehouse_ids
-        request.schema_names = schemas
+        request.schema_ids = schema_ids
         request.metric_ids = metric_ids
         request.sla_ids = collection_ids
         request.issue_ids = issue_ids
+        request.schema_names = schema_names
+        request.table_ids = table_ids
+        request.column_ids = column_ids
+        request.related_issue_ids = related_issue_ids
 
-        response = self._call_datawatch(Method.POST, url, request.to_json())
-        return GetIssuesResponse().from_dict(response).issue
+        response = GetIssuesResponse().from_dict(
+            self._call_datawatch(method=Method.POST, url=url, body=request.to_json())
+        )
+        issues: List[Issue] = response.issue
+        while response.pagination_info.next_cursor:
+            request.page_cursor = response.pagination_info.next_cursor
+            response = self._call_datawatch(method=Method.POST, url=url, body=request.to_json())
+            issues.extend(
+                GetIssuesResponse().from_dict(response).issue
+            )
+        return issues
 
     def get_issue(self, issue_id: int) -> Issue:
         return self.get_issues(issue_ids=[issue_id])[0]
 
     def update_issue(self,
                      *,
                      issue_id: int,
@@ -683,14 +701,21 @@
 
         url = '/api/v1/lineage/nodes'
 
         response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
 
         return DataNode().from_dict(response)
 
+    def get_relationships_for_data_nodes(self, *, data_node_id: int) -> GetLineageRelationshipsForNodeResponse:
+
+        url = f'/api/v1/lineage/nodes/{data_node_id}/relationships'
+        return GetLineageRelationshipsForNodeResponse().from_dict(
+            self._call_datawatch(Method.GET, url=url)
+        )
+
     def delete_data_node(self, *, data_node_id: int):
 
         url = f"/api/v1/lineage/nodes/{data_node_id}"
         log.info(f"Deleting data node {data_node_id}")
         self._call_datawatch(Method.DELETE, url=url)
 
     def create_table_lineage_relationship(self,
@@ -884,15 +909,15 @@
         url = "/api/v1/integrations"
         return IntegrationsResponse().from_dict(
             self._call_datawatch(Method.GET, url=url)
         ).integrations
 
     def get_integration_entities(self, *, integration_id: int) -> List[TableauWorkbook]:
         # TODO: Will require change once we onboard more integrations.
-        url = f"/api/vi/integrations/{integration_id}/entities"
+        url = f"/api/v1/integrations/{integration_id}/entities"
         return GetIntegrationEntitiesResponse().from_dict(
             self._call_datawatch(Method.GET, url=url)
         ).tableau_workbooks
 
     def get_advanced_configs(self) -> List[ConfigValue]:
         url = "/api/v1/configs/fetch"
         return GetConfigListResponse().from_dict(
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from bigeye_sdk.generated.com.bigeye.models.generated import Source, CohortDefinition, \
     MetricSuite, CohortAndMetricDefinition, CatalogEntityType, MetricDefinition, FieldType, NamedSchedule
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.big_config import BigConfig, RowCreationTimes, TagDeployment, TableDeployment, \
     SavedMetricDefinitions
 from bigeye_sdk.model.protobuf_enum_facade import SimplePredefinedMetricName, SimpleLookbackType
 from bigeye_sdk.model.protobuf_message_facade import SimpleCollection, SimpleMetricDefinition, SimpleSLA, SimpleLookback
+
 from bigeye_sdk.serializable import File, BIGCONFIG_FILE
 
 log = get_logger(__file__)
 
 
 def get_fq_name_from_cohort(cohort: CohortDefinition, source_name: str = None):
     """
@@ -105,32 +106,38 @@
         Args:
             bigconfig: Bigconfig.
 
         Returns: a list of upserted SLAs
 
         """
         existing_collections = {c.name: c for c in self.client.get_collections().collections}
+        merged_or_new: SimpleCollection
         deployment_collections = []
-        if apply:
-            for collection in bigconfig.get_collections():
-                if collection.name in existing_collections.keys():
-                    existing = SimpleCollection.from_datawatch_object(existing_collections[collection.name])
-                    merged = collection.merge_for_upsert(existing=existing, overwrite=overwrite)
-                    deployment_collections.append(merged)
-                    self.client.update_collection(collection=merged.to_datawatch_object())
-                else:
-                    c = collection.to_datawatch_object()
-                    c = self.client.create_collection(
-                        collection_name=c.name,
-                        description=c.description,
-                        metric_ids=c.metric_ids,
-                        notification_channels=c.notification_channels,
-                        muted_until_timestamp=c.muted_until_timestamp
-                    ).collection
-                    deployment_collections.append(SimpleCollection.from_datawatch_object(c))
+
+        for collection in bigconfig.get_collections():
+            if collection.name in existing_collections.keys():
+                """If the collection exists, send the collection ID as part of a plan and only update for apply"""
+                existing = SimpleCollection.from_datawatch_object(existing_collections[collection.name])
+                merged_or_new = collection.merge_for_upsert(existing=existing, overwrite=overwrite)
+                deployment_collections.append(merged_or_new)
+                if apply:
+                    self.client.update_collection(collection=merged_or_new.to_datawatch_object())
+            elif apply:
+                """If it doesn't exist, only create it during apply"""
+                c = collection.to_datawatch_object()
+                c = self.client.create_collection(
+                    collection_name=c.name,
+                    description=c.description,
+                    metric_ids=c.metric_ids,
+                    notification_channels=c.notification_channels,
+                    muted_until_timestamp=c.muted_until_timestamp
+                ).collection
+                merged_or_new = SimpleCollection.from_datawatch_object(c)
+                deployment_collections.append(merged_or_new)
+
 
         return deployment_collections
 
     def row_creation_times_to_cohort(self, row_creation_times: RowCreationTimes) -> Dict[int, List[CohortDefinition]]:
         r: Dict[int, List[CohortDefinition]] = {}
 
         for cs in row_creation_times.column_selectors:
@@ -221,14 +228,15 @@
         for m in tag_deployment.metrics:
             """segregate table level metrics from column level and add slas"""
             if deployment_collection and deployment_collection.id not in m.collection_ids:
                 m.collection_ids.append(deployment_collection.id)
             if m.metric_schedule and m.metric_schedule.named_schedule:
                 m.metric_schedule.named_schedule.id = [s.id for s in named_schedules
                                                        if s.name == m.metric_schedule.named_schedule.name][0]
+
             if not m.lookback:
                 m.lookback = default_lookback
 
             mdwo = m.to_datawatch_object()
             if _is_table_level_metric(metric_type=m.metric_type, table_level_metrics=self.table_level_metrics):
                 mdwo.is_table_metric = True
                 table_metrics.append((m, mdwo))
@@ -294,23 +302,23 @@
 
         return cmds
 
     def table_deployment_to_cohort_and_metric_def(self,
                                                   table_deployment: TableDeployment,
                                                   named_schedules: List[NamedSchedule],
                                                   default_lookback: SimpleLookback,
-                                                  deployment_sla: Union[SimpleSLA, SimpleCollection] = None) -> \
+                                                  deployment_collection: Union[SimpleSLA, SimpleCollection] = None) -> \
             Dict[int, List[CohortAndMetricDefinition]]:
         """
         Builds a Cohort and MetricDefinition from a TableDeployment object
         Args:
             table_deployment: table deployment from which to generate cohort and metric definition
             named_schedules: a list of named schedules from the workspace
             default_lookback: the lookback corresponding to "metric.data_time_window.default"
-            deployment_sla: SLA to which metrics will be added.
+            deployment_collection: Collection to which metrics will be added.
 
         Returns: Dict[warehouse_id: int, CohortAndMetricDefinition]
         """
 
         result: Dict[int, List[CohortAndMetricDefinition]] = {}
 
         fq_names_list = table_deployment.explode_fq_table_name()
@@ -343,21 +351,23 @@
 
                 table_deployment.register_validation_error(
                     error_lines=m.get_error_lines(),
                     error_context_lines=table_deployment.get_table_metrics_error_lines(),
                     error_message=METRIC_APPLICATION_ERROR.format(errmsg=errmsg)
                 )
             else:
-                if deployment_sla and deployment_sla.id not in m.sla_ids:
-                    m.sla_ids.append(deployment_sla.id)
+                if deployment_collection and deployment_collection.id not in m.collection_ids:
+                    m.collection_ids.append(deployment_collection.id)
                 if m.metric_schedule and m.metric_schedule.named_schedule:
                     m.metric_schedule.named_schedule.id = [s.id for s in named_schedules
                                                            if s.name == m.metric_schedule.named_schedule.name][0]
+
                 if not m.lookback:
                     m.lookback = default_lookback
+
                 mdwo = m.to_datawatch_object()
                 mdwo.is_table_metric = True
                 table_metrics.append(mdwo)
 
         if table_metrics:
             "Only add the cohort if metrics actually exist for it."
             cmds.append(
@@ -380,21 +390,23 @@
 
                     table_deployment.register_validation_error(
                         error_lines=m.get_error_lines(),
                         error_context_lines=table_deployment.get_error_lines(),
                         error_message=METRIC_APPLICATION_ERROR.format(errmsg=errmsg)
                     )
                 else:
-                    if deployment_sla and deployment_sla.id not in m.collection_ids:
-                        m.collection_ids.append(deployment_sla.id)
+                    if deployment_collection and deployment_collection.id not in m.collection_ids:
+                        m.collection_ids.append(deployment_collection.id)
                     if m.metric_schedule and m.metric_schedule.named_schedule:
                         m.metric_schedule.named_schedule.id = [s.id for s in named_schedules
                                                                if s.name == m.metric_schedule.named_schedule.name][0]
+
                     if not m.lookback:
                         m.lookback = default_lookback
+
                     mdwo = m.to_datawatch_object()
                     col_metrics.append(mdwo)
 
             if col_metrics:
                 "Only add the cohort if metrics actually exist for it."
                 cmds.append(
                     CohortAndMetricDefinition(cohorts=[cohort], metrics=col_metrics))
@@ -421,15 +433,14 @@
 
         cmds: Dict[int, List[CohortAndMetricDefinition]] = {}
 
         rct_cohorts: Dict[int, List[CohortDefinition]] = self.row_creation_times_to_cohort(bigconfig.row_creation_times)
         named_schedules: List[NamedSchedule] = self.client.get_named_schedule().named_schedules
         default_lookback_type: bool = [ac.boolean_value for ac in self.client.get_advanced_configs()
                                        if ac.key == "metric.data_time_window.default"][0]
-
         default_lookback = SimpleLookback() if default_lookback_type \
             else SimpleLookback(lookback_type=SimpleLookbackType.DATA_TIME)
 
         for tag_d_suite in bigconfig.tag_deployments:
             for tag_d in tag_d_suite.deployments:
                 """Process all tag deployments into CohortAndMetricDefinitions.  One tag deployment per CMD"""
                 if tag_d_suite.collection:
@@ -456,15 +467,15 @@
                     deployment_sla = deployment_collections.get(table_d_suite.collection.name, None)
                 else:
                     deployment_sla = None
                 r = self.table_deployment_to_cohort_and_metric_def(
                     table_deployment=table_d,
                     named_schedules=named_schedules,
                     default_lookback=default_lookback,
-                    deployment_sla=deployment_sla
+                    deployment_collection=deployment_sla
                 )
                 for sid, definitions in r.items():
                     """consolidate based on sources"""
                     if sid in cmds:
                         cmds[sid].extend(definitions)
                     else:
                         cmds[sid] = definitions
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.52/bigeye_sdk/functions/urlfuncts.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,30 +32,31 @@
     """
     value = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', value)
     value = re.sub('__([A-Z])', r'_\1', value)
     value = re.sub('([a-z0-9])([A-Z])', r'\1_\2', value)
     return value.lower()
 
 
-def encode_url_params(d: dict, doseq: bool = True, remove_keys: List[str] = []) -> str:
+def encode_url_params(d: dict, doseq: bool = True, remove_keys: List[str] = [], to_camel: bool = True) -> str:
     """
     Encodes the keys and values of a dictionary to url formatted string.
 
     :param d: The dictionary to encode.
     :param doseq: If any values in the query arg are sequences and doseq is true, each
     sequence element is converted to a separate parameter.
     :param remove_keys: Any keys to remove from the dictionary.
+    :param to_camel: Convert snake case to camel case
 
     :returns: str
     """
     remove_keys.append('self')
     filtered = {}
     for k, v in d.items():
         if v is not None and k not in remove_keys:
-            if '_' in k:
+            if '_' in k and to_camel:
                 filtered[to_camel_case(k)] = v
             else:
                 filtered[k] = v
 
     return f'?{urlencode(filtered, doseq)}'
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,23 @@
     AUTOTHRESHOLD_SENSITIVITY_UNSPECIFIED = 0
     AUTOTHRESHOLD_SENSITIVITY_NARROW = 1
     AUTOTHRESHOLD_SENSITIVITY_MEDIUM = 2
     AUTOTHRESHOLD_SENSITIVITY_WIDE = 3
     AUTOTHRESHOLD_SENSITIVITY_XWIDE = 4
 
 
+class CollectionInfoSortField(betterproto.Enum):
+    COLLECTION_SORT_FIELD_UNSPECIFIED = 0
+    COLLECTION_SORT_FIELD_FAVORITE = 1
+    COLLECTION_SORT_FIELD_ISSUE_COUNT = 2
+    COLLECTION_SORT_FIELD_METRIC_COUNT = 3
+    COLLECTION_SORT_FIELD_UPDATED_AT = 4
+    COLLECTION_SORT_FIELD_NAME = 5
+
+
 class MetricRunStatus(betterproto.Enum):
     METRIC_RUN_STATUS_UNSPECIFIED = 0
     METRIC_RUN_STATUS_UPPERBOUND_CRITICAL = 1
     METRIC_RUN_STATUS_LOWERBOUND_CRITICAL = 2
     METRIC_RUN_STATUS_OK = 3
     # METRIC_RUN_STATUS_GROUPS_CRITICAL is not a valid value for MetricRun.status
     # (it only applies to MetricInfo.status)
@@ -421,14 +430,21 @@
     METRIC_SORT_FIELD_ALERTING = 3
     METRIC_SORT_FIELD_SCHEMA = 4
     METRIC_SORT_FIELD_TABLE = 5
     METRIC_SORT_FIELD_COLUMN = 6
     METRIC_SORT_FIELD_FAVORITE = 7
 
 
+class MetricStatus(betterproto.Enum):
+    METRIC_STATUS_UNSPECIFIED = 0
+    METRIC_STATUS_ALERTING = 1
+    METRIC_STATUS_FAILED = 2
+    METRIC_STATUS_HEALTHY = 3
+
+
 class CacheOperation(betterproto.Enum):
     CACHE_OPERATION_UNSPECIFIED = 0
     CACHE_OPERATION_CLEAR_CONFIG = 1
     CACHE_OPERATION_CLEAR_USERS = 2
     CACHE_OPERATION_CLEAR_KEYS = 3
 
 
@@ -525,14 +541,16 @@
     WORKFLOW_PROCESSING_TYPE_CATALOG_INDEX_DATASET = 3
     WORKFLOW_PROCESSING_TYPE_LINEAGE = 4
     WORKFLOW_PROCESSING_TYPE_METADATA_METRICS = 5
     WORKFLOW_PROCESSING_TYPE_GENERATE_AUTOMETRICS = 6
     WORKFLOW_PROCESSING_TYPE_GENERATE_POP_SCORES = 7
     WORKFLOW_PROCESSING_TYPE_CATALOG_INDEX_INTEGRATION = 8
     WORKFLOW_PROCESSING_TYPE_APPLY_BIGCONFIG = 9
+    WORKFLOW_PROCESSING_TYPE_RUN_DELTA = 10
+    WORKFLOW_PROCESSING_TYPE_RUN_COMPARISON_TABLE = 11
 
 
 class CatalogIndexOperationType(betterproto.Enum):
     CATALOG_INDEX_OPERATION_TYPE_UNSPECIFIED = 0
     CATALOG_INDEX_OPERATION_TYPE_ADD = 1
     CATALOG_INDEX_OPERATION_TYPE_UPDATE = 2
     CATALOG_INDEX_OPERATION_TYPE_DELETE = 3
@@ -552,25 +570,33 @@
     SCHEMA_CHANGE_SORT_FIELD_TABLE = 3
     SCHEMA_CHANGE_SORT_FIELD_COLUMN = 4
     SCHEMA_CHANGE_SORT_FIELD_NEW = 5
     SCHEMA_CHANGE_SORT_FIELD_PREVIOUS = 6
     SCHEMA_CHANGE_SORT_FIELD_DETECTED_TIME = 7
 
 
+class RevisionType(betterproto.Enum):
+    REVISION_TYPE_UNSPECIFIED = 0
+    REVISION_TYPE_CREATE = 1
+    REVISION_TYPE_UPDATE = 2
+    REVISION_TYPE_DELETE = 3
+
+
 class ModelTypes(betterproto.Enum):
     MODEL_TYPE_UNDEFINED = 0
     MODEL_TYPE_MONOCLE = 1
 
 
 class MetadataOperation(betterproto.Enum):
     METADATA_OPERATION_UNSPECIFIED = 0
     METADATA_OPERATION_GET_TABLE_INDICIES = 1
     METADATA_OPERATION_GET_TABLE_METADATA = 2
     METADATA_OPERATION_GET_TABLE_LIST = 3
     METADATA_OPERATION_GET_SCHEMA_LIST = 4
+    METADATA_OPERATION_GET_SQL_SERVER_TABLE_LIST = 5
 
 
 class QueryErrorType(betterproto.Enum):
     QUERY_ERROR_TYPE_UNSPECIFIED = 0
     QUERY_ERROR_TYPE_CONNECTION_FAILURE = 1
     QUERY_ERROR_TYPE_QUERY_FAILURE = 2
     QUERY_ERROR_TYPE_METADATA_QUERY_FAILURE = 3
@@ -701,14 +727,15 @@
 
 
 @dataclass
 class TestSlackRequest(betterproto.Message):
     channel_name: str = betterproto.string_field(1)
     metric_id: int = betterproto.int32_field(2)
     collection_id: int = betterproto.int32_field(3)
+    delta_id: int = betterproto.int32_field(4)
 
 
 @dataclass
 class WebhookHeader(betterproto.Message):
     key: str = betterproto.string_field(1)
     value: str = betterproto.string_field(2)
 
@@ -962,14 +989,17 @@
 @dataclass
 class CollectionMetricStatus(betterproto.Message):
     metrics_count: int = betterproto.int32_field(1)
     alerting_metrics_count: int = betterproto.int32_field(2)
     earliest_updated_metric_seconds: int = betterproto.int64_field(3)
     latest_updated_metric_seconds: int = betterproto.int64_field(4)
     open_issues_count: int = betterproto.int32_field(5)
+    triage_issues_count: int = betterproto.int32_field(6)
+    acknowledge_issues_count: int = betterproto.int32_field(7)
+    monitoring_issues_count: int = betterproto.int32_field(8)
 
 
 @dataclass
 class CollectionInfo(betterproto.Message):
     collection_configuration: "Collection" = betterproto.message_field(1)
     collection_metric_status: "CollectionMetricStatus" = betterproto.message_field(2)
 
@@ -981,14 +1011,29 @@
 
 @dataclass
 class GetAllCollectionInfosResponse(betterproto.Message):
     collection_infos: List["CollectionInfo"] = betterproto.message_field(1)
 
 
 @dataclass
+class GetPaginatedCollectionInfosRequest(betterproto.Message):
+    page_size: int = betterproto.int32_field(1)
+    page_cursor: str = betterproto.string_field(2)
+    sort_field: "CollectionInfoSortField" = betterproto.enum_field(3)
+    sort_direction: "SortDirection" = betterproto.enum_field(4)
+    search: str = betterproto.string_field(5)
+
+
+@dataclass
+class GetPaginatedCollectionInfosResponse(betterproto.Message):
+    collection_infos: List["CollectionInfo"] = betterproto.message_field(1)
+    pagination_info: "PaginationInfo" = betterproto.message_field(2)
+
+
+@dataclass
 class Collection(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     description: str = betterproto.string_field(3)
     entity_info: "EntityInfo" = betterproto.message_field(4)
     owner: int = betterproto.int32_field(5)
     metric_ids: List[int] = betterproto.int32_field(6)
@@ -1087,14 +1132,15 @@
     schema_name: str = betterproto.string_field(9)
     warehouse_id: int = betterproto.int32_field(10)
     dataset_id: int = betterproto.int32_field(11)
     created_at: int = betterproto.int64_field(12)
     companion_metrics: List["CompanionMetric"] = betterproto.message_field(13)
     is_favorite: bool = betterproto.bool_field(14)
     metric_history_begin_at: int = betterproto.int64_field(15)
+    current_metric_status: "MetricStatus" = betterproto.enum_field(16)
 
 
 @dataclass
 class CompanionMetric(betterproto.Message):
     id: int = betterproto.int32_field(1)
     type: "CompanionMetricType" = betterproto.enum_field(2)
     metric_info: "IdAndDisplayName" = betterproto.message_field(3)
@@ -1485,14 +1531,15 @@
     views_count: int = betterproto.int32_field(11)
     popularity_score: float = betterproto.double_field(12)
     last_edited_at: int = betterproto.int64_field(13)
     created_at: int = betterproto.int64_field(14)
     updated_at: int = betterproto.int64_field(15)
     data_node_id: int = betterproto.int32_field(16)
     is_favorite: bool = betterproto.bool_field(17)
+    workspace_id: int = betterproto.int32_field(18)
 
 
 @dataclass
 class UpdateIntegrationRequestWrapper(betterproto.Message):
     integration_id: int = betterproto.int32_field(1)
     request: "CreateOrUpdateIntegrationRequest" = betterproto.message_field(2)
 
@@ -2393,14 +2440,19 @@
     warehouse_ids: List[int] = betterproto.int32_field(16)
     schema_ids: List[int] = betterproto.int32_field(17)
     schema_names: List[str] = betterproto.string_field(18)
     table_ids: List[int] = betterproto.int32_field(19)
     column_ids: List[int] = betterproto.int32_field(20)
     sla_ids: List[int] = betterproto.int32_field(21)
     related_issue_ids: List[int] = betterproto.int32_field(22)
+    priority: List["IssuePriority"] = betterproto.enum_field(23)
+    metric_status: List["MetricStatus"] = betterproto.enum_field(24)
+    metric_type: List["MetricType"] = betterproto.message_field(25)
+    min_opened_time: int = betterproto.int64_field(26)
+    max_opened_time: int = betterproto.int64_field(27)
 
 
 @dataclass
 class GetIssuesResponse(betterproto.Message):
     issue: List["Issue"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -2837,14 +2889,16 @@
 
 @dataclass
 class SourcePermission(betterproto.Message):
     source_id: int = betterproto.int32_field(1)
     type: "SourcePermissionType" = betterproto.enum_field(2)
     is_successful: bool = betterproto.bool_field(3)
     last_run_at: int = betterproto.int64_field(4)
+    exception_class: str = betterproto.string_field(5)
+    exception_message: str = betterproto.string_field(6)
 
 
 @dataclass
 class GetSourcePermissionResponse(betterproto.Message):
     permissions: List["SourcePermission"] = betterproto.message_field(1)
 
 
@@ -2996,14 +3050,20 @@
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
     priority: int = betterproto.int32_field(3)
     is_first_indexing: bool = betterproto.bool_field(4)
     indexed_at: int = betterproto.int64_field(5)
 
 
 @dataclass
+class DeltaRunRequest(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    workflow_info: "WorkflowInfo" = betterproto.message_field(2)
+
+
+@dataclass
 class IntegrationIndexRequest(betterproto.Message):
     integration_id: int = betterproto.int32_field(1)
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
     priority: int = betterproto.int32_field(3)
 
 
 @dataclass
@@ -3219,14 +3279,56 @@
 
 @dataclass
 class GetDeltaResponse(betterproto.Message):
     delta_info: "DeltaInfo" = betterproto.message_field(1)
 
 
 @dataclass
+class Workspace(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    name: str = betterproto.string_field(2)
+    is_default: bool = betterproto.bool_field(3)
+    sources: List["Source"] = betterproto.message_field(4)
+
+
+@dataclass
+class CreateOrUpdateWorkspaceRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+
+
+@dataclass
+class RevisionInfo(betterproto.Message):
+    type: "RevisionType" = betterproto.enum_field(1)
+    epoch_seconds: int = betterproto.int64_field(2)
+    revised_by: "User" = betterproto.message_field(3)
+
+
+@dataclass
+class WorkspaceRevision(betterproto.Message):
+    revision_info: "RevisionInfo" = betterproto.message_field(1)
+    workspace: "Workspace" = betterproto.message_field(2)
+
+
+@dataclass
+class GetWorkspaceAuditLogResponse(betterproto.Message):
+    revisions: List["WorkspaceRevision"] = betterproto.message_field(1)
+
+
+@dataclass
+class UserRevision(betterproto.Message):
+    revision_info: "RevisionInfo" = betterproto.message_field(1)
+    user: "User" = betterproto.message_field(2)
+
+
+@dataclass
+class GetUserAuditLogResponse(betterproto.Message):
+    revisions: List["UserRevision"] = betterproto.message_field(1)
+
+
+@dataclass
 class Empty(betterproto.Message):
     pass
 
 
 @dataclass
 class DimensionRun(betterproto.Message):
     dim_name: str = betterproto.string_field(1)
@@ -3355,14 +3457,16 @@
 
 
 @dataclass
 class SqlQueryResponse(betterproto.Message):
     results: List["QueryResult"] = betterproto.message_field(1)
     size: int = betterproto.int64_field(2)
     version: str = betterproto.string_field(3)
+    database_name: str = betterproto.string_field(4)
+    timeout_seconds: int = betterproto.int32_field(5)
 
 
 @dataclass
 class QueryResult(betterproto.Message):
     error: "QueryError" = betterproto.message_field(1)
     col_names: List[str] = betterproto.string_field(2)
     col_types: List[str] = betterproto.string_field(3)
@@ -4829,14 +4933,19 @@
         warehouse_ids: List[int] = [],
         schema_ids: List[int] = [],
         schema_names: List[str] = [],
         table_ids: List[int] = [],
         column_ids: List[int] = [],
         sla_ids: List[int] = [],
         related_issue_ids: List[int] = [],
+        priority: List["IssuePriority"] = [],
+        metric_status: List["MetricStatus"] = [],
+        metric_type: List["MetricType"] = [],
+        min_opened_time: int = 0,
+        max_opened_time: int = 0,
     ) -> GetIssuesResponse:
         """Get issues"""
 
         request = GetIssuesRequest()
         request.issue_ids = issue_ids
         request.current_status = current_status
         request.metric_ids = metric_ids
@@ -4849,14 +4958,20 @@
         request.warehouse_ids = warehouse_ids
         request.schema_ids = schema_ids
         request.schema_names = schema_names
         request.table_ids = table_ids
         request.column_ids = column_ids
         request.sla_ids = sla_ids
         request.related_issue_ids = related_issue_ids
+        request.priority = priority
+        request.metric_status = metric_status
+        if metric_type is not None:
+            request.metric_type = metric_type
+        request.min_opened_time = min_opened_time
+        request.max_opened_time = max_opened_time
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.IssueService/GetIssues",
             request,
             GetIssuesResponse,
         )
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.52/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
+from enum import Enum
 from itertools import chain
 from typing import List
 
 import betterproto
 from pydantic_yaml import YamlStrEnum
 
 from bigeye_sdk.functions.casing import snake_case
 from bigeye_sdk.generated.com.bigeye.models.generated import MetricType, PredefinedMetric, PredefinedMetricName, \
     AutothresholdSensitivity, FieldType, TimeIntervalType, LookbackType, AggregationType, DataNodeType, \
-    MetricTemplateParameterType, MetricTemplateSortField, SortDirection
+    MetricTemplateParameterType
 
 
 def _remove_protobuf_type(protobuf_enum_cls: type(betterproto.Enum), member_name: str) -> str:
     """
     Processes an enum type prefix or postfix out of an enum member name.
 
     >>> _remove_protobuf_type(AutothresholdSensitivity, AutothresholdSensitivity.AUTOTHRESHOLD_SENSITIVITY_MEDIUM.name)
@@ -214,9 +215,9 @@
     BOOLEAN = SimpleFieldType.BOOLEAN
     NUMERIC = SimpleFieldType.NUMERIC
 
 
 @datawatch_enum_facade
 class SimpleDbtTestToMetricType(YamlStrEnum):
     not_null = SimplePredefinedMetricName.COUNT_NULL
-    unique = SimplePredefinedMetricName.PERCENT_UNIQUE
+    unique = SimplePredefinedMetricName.COUNT_DUPLICATES
     accepted_values = SimplePredefinedMetricName.PERCENT_VALUE_IN_LIST
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bigeye_sdk.exceptions import InvalidConfigurationException
 from bigeye_sdk.functions.search_and_match_functions import fuzzy_match
 from bigeye_sdk.functions.table_functions import get_table_column_id
 from bigeye_sdk.generated.com.bigeye.models.generated import Threshold, SimpleBoundType, ConstantThreshold, \
     SimpleBound, NamedSchedule, ComparisonColumnMapping, Table, IdAndDisplayName, ColumnNamePair, TimeInterval, \
     MetricParameter, MetricType, PredefinedMetric, TemplateMetric, AutoThreshold, ForecastModelType, RelativeThreshold, \
     StandardDeviationThreshold, FreshnessScheduleThreshold, NotificationChannel, MetricDefinition, MetricConfiguration, \
-    Collection, SlackChannelInfo, Webhook, WebhookHeader, MetricSchedule, TimeIntervalType
+    Collection, SlackChannelInfo, Webhook, WebhookHeader, MetricSchedule
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.base_datawatch_facade import DatawatchFacade
 from bigeye_sdk.model.protobuf_enum_facade import SimplePredefinedMetricName, SimpleTimeIntervalType, \
     SimpleAutothresholdSensitivity, SimpleLookbackType, SimpleAggregationType
 from bigeye_sdk.serializable import PydanticSubtypeSerializable
 
 log = get_logger(__file__)
@@ -50,14 +50,30 @@
         return [SimplePredefinedMetric(type="PREDEFINED", predefined_metric=i) for i in freshness_metric_names]
 
     @classmethod
     def is_freshness_metric(cls, predefined_metric):
         return predefined_metric in cls.get_freshness_metric_types()
 
     @classmethod
+    def is_freshness_volume(cls, predefined_metric):
+        return predefined_metric in [
+            SimplePredefinedMetric(type="PREDEFINED", predefined_metric=SimplePredefinedMetricName.FRESHNESS),
+            SimplePredefinedMetric(type="PREDEFINED", predefined_metric=SimplePredefinedMetricName.VOLUME)
+        ]
+
+    @classmethod
+    def get_metadata_metrics(cls) -> List[SimplePredefinedMetric]:
+        metadata_metrics = [SimplePredefinedMetricName.HOURS_SINCE_LAST_LOAD,
+                            SimplePredefinedMetricName.FRESHNESS,
+                            SimplePredefinedMetricName.VOLUME,
+                            SimplePredefinedMetricName.ROWS_INSERTED,
+                            SimplePredefinedMetricName.COUNT_READ_QUERIES]
+        return [SimplePredefinedMetric(type="PREDEFINED", predefined_metric=i) for i in metadata_metrics]
+
+    @classmethod
     def from_datawatch_object(cls, obj: MetricType) -> SimpleMetricType:
         t = betterproto.which_one_of(obj, "metric_type")[0]
         if not t:
             t = get_type_from_dict(obj)
         if t == 'template_metric':
             tm = obj.template_metric
             return SimpleTemplateMetric(type='TEMPLATE',
@@ -728,14 +744,15 @@
     schedule_frequency: Optional[SimpleTimeInterval] = None
     conditions: Optional[List[str]] = None
     group_by: Optional[List[str]] = None
     threshold: Optional[SimpleThreshold] = None
     notification_channels: Optional[List[SimpleNotificationChannel]] = None
     parameters: Optional[List[SimpleMetricParameter]] = None
     lookback: Optional[SimpleLookback] = None
+    grain_seconds: Optional[int] = 0
     muted_until_epoch_seconds: Optional[int] = 0
     sla_ids: Optional[List[int]] = Field(default_factory=lambda: [])
     collection_ids: Optional[List[int]] = Field(default_factory=lambda: [])
     metric_schedule: Optional[SimpleMetricSchedule] = None
 
     @validator('threshold', always=True, pre=False)
     def set_default_threshold(cls, threshold, values):
@@ -782,14 +799,21 @@
         elif metric_type \
                 and metric_type in SimpleMetricType.get_freshness_metric_types():
             """Freshness metrics should execute every 6 hours by default WIZ-1623"""
             values['schedule_frequency'] = SimpleTimeInterval(
                 interval_type=SimpleTimeIntervalType.HOURS, interval_value=6
             )
             return values
+        elif metric_type \
+                and SimpleMetricType.is_freshness_volume(metric_type):
+            """Freshness and volume should execute every 6 hours by default"""
+            values['schedule_frequency'] = SimpleTimeInterval(
+                interval_type=SimpleTimeIntervalType.HOURS, interval_value=6
+            )
+            return values
         else:
             """All other metrics should execute every 24 hours by default WIZ-1623"""
             values['schedule_frequency'] = SimpleTimeInterval(
                 interval_type=SimpleTimeIntervalType.HOURS, interval_value=24
             )
             return values
 
@@ -805,15 +829,15 @@
             return safe_split_dict_entry_lines('saved_metric_id', self.saved_metric_id)
         else:
             return self.yaml(exclude_unset=True, exclude_defaults=True,
                              exclude_none=True, indent=True).splitlines()
 
     @validator('metric_type', pre=True)
     def must_be_dict_type(cls, metric_type):
-        if isinstance(metric_type, SimplePredefinedMetric):
+        if isinstance(metric_type, (SimplePredefinedMetric, SimpleTemplateMetric)):
             return metric_type
 
         if metric_type and not isinstance(metric_type, dict):
             errlns = yaml.safe_dump({'metric_type': metric_type}, indent=True, sort_keys=False)
             SimpleMetricDefinition.register_validation_error(
                 error_lines=[errlns],
                 error_message=FORMATTING_ERRMSG.format(
@@ -896,15 +920,15 @@
                                            error_context_lines=config_error_lines,
                                            error_message=error_message)
 
     def saved_metrics_must_have_id(self, config_error_lines: List[str]):
         """
         Saved Metric Definitions must have a saved metric id.
         Args:
-            config_error_lines: The congiruation serialized to yaml and split to lines.
+            config_error_lines: The configuration serialized to yaml and split to lines.
 
         Returns: None
         """
         if not self.saved_metric_id:
             error_mesage = MUST_HAVE_METRIC_ID_ERRMSG.format(config_error_lines=config_error_lines)
             self.register_validation_error(error_lines=self.get_error_lines(),
                                            error_context_lines=config_error_lines,
@@ -930,21 +954,25 @@
         builder.parameters = [SimpleMetricParameter.from_datawatch_object(p) for p in obj.parameters]
 
         builder.lookback = SimpleLookback(lookback_window=SimpleTimeInterval.from_datawatch_object(obj.lookback),
                                           lookback_type=SimpleLookbackType.from_datawatch_object(obj.lookback_type),
                                           bucket_size=BucketSize.from_seconds(obj.grain_seconds))
 
         builder.muted_until_epoch_seconds = obj.muted_until_epoch_seconds
+        builder.grain_seconds = obj.grain_seconds
 
         builder.collection_ids = obj.collection_ids
         builder.metric_schedule = SimpleMetricSchedule.from_datawatch_object(obj.metric_schedule)
         return builder
 
-    def to_datawatch_object(self, **kwargs) -> MetricDefinition:
-        builder = MetricDefinition()
+    def to_datawatch_object(self, to_config: bool = False, **kwargs) -> Union[MetricDefinition, MetricConfiguration]:
+        if to_config:
+            builder = MetricConfiguration()
+        else:
+            builder = MetricDefinition()
 
         # Verifying that metric_type has been set before serializing to datawatch object.
         if self.metric_type:
             builder.metric_type = self.metric_type.to_datawatch_object()
         else:
             InvalidConfigurationException(
                 "Metric Type cannot be None.  Verify that Saved Metric IDs have been applied.")
@@ -976,14 +1004,18 @@
 
             """Freshness metrics require data time lookback"""
             if SimpleMetricType.is_freshness_metric(self.metric_type):
                 builder.lookback_type = SimpleLookbackType.DATA_TIME.to_datawatch_object()
 
             builder.grain_seconds = self.lookback.bucket_size.to_seconds()
 
+        if SimpleMetricType.is_freshness_volume(self.metric_type):
+            builder.grain_seconds = BucketSize.HOUR.to_seconds()
+
+
         builder.muted_until_epoch_seconds = self.muted_until_epoch_seconds
 
         if self.collection_ids:
             builder.collection_ids = self.collection_ids
         if self.metric_schedule:
             builder.metric_schedule = self.metric_schedule.to_datawatch_object()
```

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.52/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.52/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.50/pyproject.toml` & `bigeye_sdk-0.4.52/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.50"
+version = "0.4.52"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.50/setup.py` & `bigeye_sdk-0.4.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'requests==2.28.1',
  'setuptools>=59.6.0,<60.0.0',
  'smart-open>=6.1.0,<7.0.0',
  'types-PyYAML>=6.0.11,<7.0.0']
 
 setup_kwargs = {
     'name': 'bigeye-sdk',
-    'version': '0.4.50',
+    'version': '0.4.52',
     'description': 'Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.',
     'long_description': '# Bigeye SDK\n\nBigeye SDK is a collection of protobuf generated code, functions, and models used to interact programmatically\nwith the Bigeye API.  Bigeye currently supports a Python SDK.  The main entry point is the DatawatchClient \nabstraction and, in this core package, a basic auth client has been implemented.  The abstract base class \nincludes core functionality (methods to interact with the API) and each implementation should enable a \ndifferent authorization methods.\n\n## Install\n\n```shell\npip install bigeye_sdk\n```\n\n## Basic Auth\n\nBasic authorization credentials can be stored as Json either on disk or in a secrets/credentials manager.  This\nformat will be marshalled into an instance of [BasicAuthRequestLibApiConf](bigeye_sdk/authentication/api_authentication.py).\n\n```json\n{\n    "base_url": "https://app.bigeye.com",\n    "user": "",\n    "password": ""\n}\n```\n',
     'author': 'Bigeye',
     'author_email': 'support@bigeye.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docs.bigeye.com/docs',
```

### Comparing `bigeye_sdk-0.4.50/PKG-INFO` & `bigeye_sdk-0.4.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.50
+Version: 0.4.52
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: Other/Proprietary License
```

