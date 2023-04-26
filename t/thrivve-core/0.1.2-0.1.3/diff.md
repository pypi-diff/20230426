# Comparing `tmp/thrivve_core-0.1.2.tar.gz` & `tmp/thrivve_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-co9au7at/thrivve_core-0.1.2.tar", last modified: Wed Apr 26 11:19:40 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-aofrlret/thrivve_core-0.1.3.tar", last modified: Wed Apr 26 13:04:12 2023, max compression
```

## Comparing `thrivve_core-0.1.2.tar` & `thrivve_core-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12351 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-26 11:19:30.000000 thrivve_core-0.1.2/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-26 11:19:40.000000 thrivve_core-0.1.2/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12351 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-26 13:03:59.000000 thrivve_core-0.1.3/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-26 13:04:12.000000 thrivve_core-0.1.3/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.1.2/PKG-INFO` & `thrivve_core-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.1.2
+Version: 0.1.3
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.2/setup.py` & `thrivve_core-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.1.2",
+    version="0.1.3",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.1.2/thrivve_core/__init__.py` & `thrivve_core-0.1.3/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.1.3/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.1.3/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.1.3/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.1.3/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.1.3/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/base.py` & `thrivve_core-0.1.3/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.1.3/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.1.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.1.3/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.1.3/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.1.3/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.1.3/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.1.3/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/auth.py` & `thrivve_core-0.1.3/thrivve_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/config.py` & `thrivve_core-0.1.3/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.1.3/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.1.3/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/enums.py` & `thrivve_core-0.1.3/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.1.3/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.1.3/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/filters.py` & `thrivve_core-0.1.3/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.1.3/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.1.3/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/kafka_listener.py` & `thrivve_core-0.1.3/thrivve_core/helpers/kafka_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import time
 import traceback
 
 from confluent_kafka import Consumer
 
 from thrivve_core import ThrivveCore
 from thrivve_core.app_decorators import handle_exceptions
+from thrivve_core.helpers.exceptions import AppValidationError
 
 
 def start_kafka_listener(topics):
     """
     Start Kafka listener
     """
-
     app = ThrivveCore.get_app()
-
-    app.logger.info(f"Start Kafka listen to [{' - '.join(topics)}]..")
+    app.logger.info(f"Start Kafka listening to topics [{' - '.join(topics)}]..")
 
     consumer = Consumer(
         {
             "bootstrap.servers": app.config.get("BOOTSTRAP_SERVERS"),
             "sasl.username": app.config.get("SASL_USERNAME"),
             "sasl.password": app.config.get("SASL_PASSWORD"),
             "security.protocol": "SASL_SSL",
@@ -44,37 +43,48 @@
             if msg.error():
                 app.logger.error("error: {0}".format(msg.error()))
                 continue
 
             app.logger.info("Got a message..")
 
             # message_key = msg.key()
-            message_payload = json.loads(msg.value())
-
-            app.logger.debug(message_payload)
-
-            if not message_payload:
-                continue
 
-            function_name = message_payload.get("function_name")
-            function_params = message_payload.get("function_params")
-            if not function_name:
+            try:
+                consume_message(msg.value())
+            except AppValidationError:
+                # app.logger.error(traceback.format_exc())
                 continue
 
-            @handle_exceptions
-            def _execute_method():
-                function_file, function_call = os.path.splitext(function_name)
-                module = importlib.import_module(function_file)
-                method = getattr(module, function_call[1:])
-
-                return method(**function_params)
-
-            function_result = _execute_method()
-            app.logger.debug(function_result)
-
             time.sleep(1)
 
     except KeyboardInterrupt:
         app.logger.debug("Keyboard interrupted..")
     finally:
         app.logger.error(traceback.format_exc())
         consumer.close()
+
+
+def consume_message(message_payload):
+    message_payload = json.loads(message_payload)
+
+    app = ThrivveCore.get_app()
+
+    app.logger.debug(message_payload)
+
+    if not message_payload:
+        raise AppValidationError("No message payload found..")
+
+    function_name = message_payload.get("function_name")
+    function_params = message_payload.get("function_params") or {}
+    if not function_name:
+        raise AppValidationError("No function name found..")
+
+    @handle_exceptions
+    def _execute_method():
+        function_file, function_call = os.path.splitext(function_name)
+        module = importlib.import_module(function_file)
+        method = getattr(module, function_call[1:])
+
+        return method(**function_params)
+
+    function_result = _execute_method()
+    app.logger.debug(function_result)
```

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.1.3/thrivve_core/helpers/kafka_producer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import random
 import string
-
+import traceback
 
 from confluent_kafka import Producer as kafka_Producer
 from thrivve_core import ThrivveCore
 
 
 class Producer:
     app = None
@@ -30,14 +30,25 @@
 
     def send_topic(self, topic, datajson):
 
         if not self.app:
             return True
 
         self.app.logger.debug(datajson)
+        is_test_kafka = self.app.config.get("IS_TEST_KAFKA")
+
+        if is_test_kafka and datajson.get("producer_version") == 2:
+            self.app.logger.debug("Test Kafka is enabled")
+            try:
+                from app.kafka.test import execute
+                execute(json.dumps(datajson.get('datajson')))
+
+            except Exception:
+                self.app.logger.error(traceback.format_exc())
+            return True
 
         if self._producer is None:
             self.app.logger.debug(
                 "Can not send Kafka message, this is {} environment".format(
                     self.app.config.get("FLASK_ENV")
                 )
             )
```

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/kafka_producers/notification_center.py` & `thrivve_core-0.1.3/thrivve_core/helpers/kafka_producers/notification_center.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from datetime import datetime
 
-from thrivve_core.helpers.kafka_producer import Producer
 from thrivve_core import ThrivveCore
 from thrivve_core.helpers.topics import Topics
+from thrivve_core.helpers import kafka_producers
 
 
 def send_critical_error(message, channel=None):
     channel = channel or "critical-errors"
     send_notification_message(
         channel=channel,
         title="critical",
@@ -40,15 +40,16 @@
             ),
             "text": message,
             "color": color,
             "icon_emoji": emoji,
         },
     }
     app.logger.debug(data)
-    Producer().send_topic(topic=Topics.INTERNAL_NOTIFICATION_MESSAGE, datajson=data)
+    kafka_producers.send_topic(topic=Topics.INTERNAL_NOTIFICATION_MESSAGE, datajson=data)
+
 
 
 def send_push_notification(
         message, reference_type, user_ids, payload=None, created_by=None
 ):
     # token = None
     base_payload = dict(
@@ -67,14 +68,14 @@
 
     data = dict(
         message=message,
         reference_type=reference_type,
         user_ids=user_ids,
         payload=base_payload,
         created_by=created_by,
-        language="ar"
+        # language="ar"
     )
 
-    Producer().send_topic(topic=Topics.THRIVVE_SEND_PUSH_NOTIFICATION, datajson=dict(
+    kafka_producers.send_topic(topic=Topics.THRIVVE_SEND_PUSH_NOTIFICATION, datajson=dict(
         function_name='app.business_logic.notification.send_push_notification.execute',
         function_params=data
     ))
```

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/log_config.py` & `thrivve_core-0.1.3/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.1.3/thrivve_core/helpers/micro_fetcher.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/search_function.py` & `thrivve_core-0.1.3/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/service_config.py` & `thrivve_core-0.1.3/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/sql.py` & `thrivve_core-0.1.3/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/time.py` & `thrivve_core-0.1.3/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.1.3/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.1.3/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.2/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.1.3/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.2/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.1.3/thrivve_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,9 @@
 thrivve_core/helpers/amazon/get_s3_client.py
 thrivve_core/helpers/amazon/upload_file.py
 thrivve_core/helpers/database/__init__.py
 thrivve_core/helpers/database/base_model.py
 thrivve_core/helpers/database/log_model.py
 thrivve_core/helpers/kafka_producers/__init__.py
 thrivve_core/helpers/kafka_producers/log_model_changes.py
-thrivve_core/helpers/kafka_producers/notification_center.py
+thrivve_core/helpers/kafka_producers/notification_center.py
+thrivve_core/helpers/kafka_producers/send_topic.py
```

